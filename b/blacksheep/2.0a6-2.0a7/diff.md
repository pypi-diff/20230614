# Comparing `tmp/blacksheep-2.0a6.tar.gz` & `tmp/blacksheep-2.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blacksheep-2.0a6.tar", last modified: Fri Apr 28 06:03:13 2023, max compression
+gzip compressed data, was "blacksheep-2.0a7.tar", last modified: Wed May 31 06:10:13 2023, max compression
```

## Comparing `blacksheep-2.0a6.tar` & `blacksheep-2.0a7.tar`

### file list

```diff
@@ -1,179 +1,179 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 06:03:13.771270 blacksheep-2.0a6/
--rw-rw-rw-   0        0        0     1072 2023-04-28 05:59:52.000000 blacksheep-2.0a6/LICENSE
--rw-rw-rw-   0        0        0      233 2023-04-28 05:59:52.000000 blacksheep-2.0a6/MANIFEST.in
--rw-rw-rw-   0        0        0    10662 2023-04-28 06:03:13.771270 blacksheep-2.0a6/PKG-INFO
--rw-rw-rw-   0        0        0     9484 2023-04-28 05:59:52.000000 blacksheep-2.0a6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 06:03:13.708769 blacksheep-2.0a6/blacksheep/
--rw-rw-rw-   0        0        0     4197 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/__init__.py
--rw-rw-rw-   0        0        0      433 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/asgi.pyi
--rw-rw-rw-   0        0        0   708668 2023-04-28 06:02:25.000000 blacksheep-2.0a6/blacksheep/baseapp.c
--rw-rw-rw-   0        0        0      567 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/baseapp.pxd
--rw-rw-rw-   0        0        0     1535 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/baseapp.pyi
--rw-rw-rw-   0        0        0     6169 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/baseapp.pyx
-drwxrwxrwx   0        0        0        0 2023-04-28 06:03:13.708769 blacksheep-2.0a6/blacksheep/client/
--rw-rw-rw-   0        0        0      396 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/client/__init__.py
--rw-rw-rw-   0        0        0    13126 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/client/connection.py
--rw-rw-rw-   0        0        0    10499 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/client/cookies.py
--rw-rw-rw-   0        0        0     2004 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/client/exceptions.py
--rw-rw-rw-   0        0        0     4753 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/client/pool.py
--rw-rw-rw-   0        0        0    15045 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/client/session.py
-drwxrwxrwx   0        0        0        0 2023-04-28 06:03:13.724394 blacksheep-2.0a6/blacksheep/common/
--rw-rw-rw-   0        0        0      397 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 06:03:13.724394 blacksheep-2.0a6/blacksheep/common/files/
--rw-rw-rw-   0        0        0        0 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/common/files/__init__.py
--rw-rw-rw-   0        0        0     3371 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/common/files/asyncfs.py
--rw-rw-rw-   0        0        0      938 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/common/files/info.py
--rw-rw-rw-   0        0        0      679 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/common/files/pathsutils.py
--rw-rw-rw-   0        0        0     1457 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/common/types.py
--rw-rw-rw-   0        0        0   966615 2023-04-28 06:02:22.000000 blacksheep-2.0a6/blacksheep/contents.c
--rw-rw-rw-   0        0        0     1042 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/contents.pxd
--rw-rw-rw-   0        0        0     3061 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/contents.pyi
--rw-rw-rw-   0        0        0     7476 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/contents.pyx
--rw-rw-rw-   0        0        0   709232 2023-04-28 06:02:21.000000 blacksheep-2.0a6/blacksheep/cookies.c
--rw-rw-rw-   0        0        0      981 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/cookies.pxd
--rw-rw-rw-   0        0        0     1332 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/cookies.pyi
--rw-rw-rw-   0        0        0     6498 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/cookies.pyx
--rw-rw-rw-   0        0        0   699602 2023-04-28 06:02:19.000000 blacksheep-2.0a6/blacksheep/exceptions.c
--rw-rw-rw-   0        0        0      421 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/exceptions.pxd
--rw-rw-rw-   0        0        0     1707 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/exceptions.pyi
--rw-rw-rw-   0        0        0     1774 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/exceptions.pyx
--rw-rw-rw-   0        0        0   588852 2023-04-28 06:02:20.000000 blacksheep-2.0a6/blacksheep/headers.c
--rw-rw-rw-   0        0        0      798 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/headers.pxd
--rw-rw-rw-   0        0        0     1876 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/headers.pyi
--rw-rw-rw-   0        0        0     5660 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/headers.pyx
-drwxrwxrwx   0        0        0        0 2023-04-28 06:03:13.724394 blacksheep-2.0a6/blacksheep/includes/
--rw-rw-rw-   0        0        0       44 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/includes/consts.pxi
--rw-rw-rw-   0        0        0  1182891 2023-04-28 06:02:23.000000 blacksheep-2.0a6/blacksheep/messages.c
--rw-rw-rw-   0        0        0     2123 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/messages.pxd
--rw-rw-rw-   0        0        0     5566 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/messages.pyi
--rw-rw-rw-   0        0        0    18461 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/messages.pyx
--rw-rw-rw-   0        0        0      587 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/middlewares.py
--rw-rw-rw-   0        0        0     3320 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/multipart.py
--rw-rw-rw-   0        0        0      434 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/normalization.py
--rw-rw-rw-   0        0        0        0 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/py.typed
--rw-rw-rw-   0        0        0     5564 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/ranges.py
--rw-rw-rw-   0        0        0   630854 2023-04-28 06:02:24.000000 blacksheep-2.0a6/blacksheep/scribe.c
--rw-rw-rw-   0        0        0      753 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/scribe.pxd
--rw-rw-rw-   0        0        0      841 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/scribe.pyi
--rw-rw-rw-   0        0        0     9277 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/scribe.pyx
-drwxrwxrwx   0        0        0        0 2023-04-28 06:03:13.724394 blacksheep-2.0a6/blacksheep/server/
--rw-rw-rw-   0        0        0      180 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/__init__.py
--rw-rw-rw-   0        0        0    29511 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/application.py
--rw-rw-rw-   0        0        0     2537 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/asgi.py
-drwxrwxrwx   0        0        0        0 2023-04-28 06:03:13.724394 blacksheep-2.0a6/blacksheep/server/authentication/
--rw-rw-rw-   0        0        0     1838 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/authentication/__init__.py
--rw-rw-rw-   0        0        0     4376 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/authentication/cookie.py
--rw-rw-rw-   0        0        0     5125 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/authentication/jwt.py
--rw-rw-rw-   0        0        0    37888 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/authentication/oidc.py
-drwxrwxrwx   0        0        0        0 2023-04-28 06:03:13.724394 blacksheep-2.0a6/blacksheep/server/authorization/
--rw-rw-rw-   0        0        0     3345 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/authorization/__init__.py
--rw-rw-rw-   0        0        0    27359 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/bindings.py
--rw-rw-rw-   0        0        0     4337 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/compression.py
--rw-rw-rw-   0        0        0    13325 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/controllers.py
--rw-rw-rw-   0        0        0    11278 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/cors.py
--rw-rw-rw-   0        0        0    13278 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/csrf.py
--rw-rw-rw-   0        0        0     1581 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/dataprotection.py
--rw-rw-rw-   0        0        0     1932 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/di.py
--rw-rw-rw-   0        0        0     1316 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/env.py
--rw-rw-rw-   0        0        0     1679 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/errors.py
-drwxrwxrwx   0        0        0        0 2023-04-28 06:03:13.740024 blacksheep-2.0a6/blacksheep/server/files/
--rw-rw-rw-   0        0        0     9368 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/files/__init__.py
--rw-rw-rw-   0        0        0     8717 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/files/dynamic.py
--rw-rw-rw-   0        0        0     1134 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/files/static.py
-drwxrwxrwx   0        0        0        0 2023-04-28 06:03:13.740024 blacksheep-2.0a6/blacksheep/server/headers/
--rw-rw-rw-   0        0        0        0 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/headers/__init__.py
--rw-rw-rw-   0        0        0    11234 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/headers/cache.py
--rw-rw-rw-   0        0        0    19420 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/normalization.py
-drwxrwxrwx   0        0        0        0 2023-04-28 06:03:13.740024 blacksheep-2.0a6/blacksheep/server/openapi/
--rw-rw-rw-   0        0        0        0 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/openapi/__init__.py
--rw-rw-rw-   0        0        0    13187 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/openapi/common.py
--rw-rw-rw-   0        0        0    16431 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/openapi/docstrings.py
--rw-rw-rw-   0        0        0      814 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/openapi/exceptions.py
--rw-rw-rw-   0        0        0     2831 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/openapi/ui.py
--rw-rw-rw-   0        0        0    38098 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/openapi/v3.py
-drwxrwxrwx   0        0        0        0 2023-04-28 06:03:13.740024 blacksheep-2.0a6/blacksheep/server/remotes/
--rw-rw-rw-   0        0        0        0 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/remotes/__init__.py
--rw-rw-rw-   0        0        0    13119 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/remotes/forwarding.py
--rw-rw-rw-   0        0        0      963 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/remotes/hosts.py
-drwxrwxrwx   0        0        0        0 2023-04-28 06:03:13.740024 blacksheep-2.0a6/blacksheep/server/rendering/
--rw-rw-rw-   0        0        0        0 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/rendering/__init__.py
--rw-rw-rw-   0        0        0      765 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/rendering/abc.py
--rw-rw-rw-   0        0        0     4016 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/rendering/jinja2.py
--rw-rw-rw-   0        0        0      417 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/rendering/models.py
-drwxrwxrwx   0        0        0        0 2023-04-28 06:03:13.740024 blacksheep-2.0a6/blacksheep/server/res/
--rw-rw-rw-   0        0        0        0 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/res/__init__.py
--rw-rw-rw-   0        0        0     1356 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/res/error.css
--rw-rw-rw-   0        0        0     1028 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/res/error.html
--rw-rw-rw-   0        0        0      331 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/res/fileslist.html
--rw-rw-rw-   0        0        0      590 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/res/redoc-ui.html
--rw-rw-rw-   0        0        0      841 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/res/swagger-ui.html
--rw-rw-rw-   0        0        0      263 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/resources.py
--rw-rw-rw-   0        0        0    10477 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/responses.py
--rw-rw-rw-   0        0        0    26805 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/routing.py
-drwxrwxrwx   0        0        0        0 2023-04-28 06:03:13.740024 blacksheep-2.0a6/blacksheep/server/security/
--rw-rw-rw-   0        0        0      417 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/security/__init__.py
--rw-rw-rw-   0        0        0      848 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/security/hsts.py
--rw-rw-rw-   0        0        0     5352 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/server/websocket.py
-drwxrwxrwx   0        0        0        0 2023-04-28 06:03:13.740024 blacksheep-2.0a6/blacksheep/sessions/
--rw-rw-rw-   0        0        0     5399 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/sessions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 06:03:13.755643 blacksheep-2.0a6/blacksheep/settings/
--rw-rw-rw-   0        0        0       76 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/settings/__init__.py
--rw-rw-rw-   0        0        0      538 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/settings/di.py
--rw-rw-rw-   0        0        0     1073 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/settings/html.py
--rw-rw-rw-   0        0        0      894 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/settings/json.py
-drwxrwxrwx   0        0        0        0 2023-04-28 06:03:13.755643 blacksheep-2.0a6/blacksheep/testing/
--rw-rw-rw-   0        0        0      398 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/testing/__init__.py
--rw-rw-rw-   0        0        0     4379 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/testing/client.py
--rw-rw-rw-   0        0        0     3755 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/testing/helpers.py
--rw-rw-rw-   0        0        0     1440 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/testing/messages.py
--rw-rw-rw-   0        0        0     2659 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/testing/simulator.py
--rw-rw-rw-   0        0        0   417993 2023-04-28 06:02:19.000000 blacksheep-2.0a6/blacksheep/url.c
--rw-rw-rw-   0        0        0      751 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/url.pxd
--rw-rw-rw-   0        0        0      707 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/url.pyi
--rw-rw-rw-   0        0        0     4061 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/url.pyx
-drwxrwxrwx   0        0        0        0 2023-04-28 06:03:13.755643 blacksheep-2.0a6/blacksheep/utils/
--rw-rw-rw-   0        0        0     1115 2023-04-28 05:59:52.000000 blacksheep-2.0a6/blacksheep/utils/__init__.py
--rw-rw-rw-   0        0        0     2733 2023-04-28 05:59:53.000000 blacksheep-2.0a6/blacksheep/utils/aio.py
--rw-rw-rw-   0        0        0      693 2023-04-28 05:59:53.000000 blacksheep-2.0a6/blacksheep/utils/meta.py
-drwxrwxrwx   0        0        0        0 2023-04-28 06:03:13.708769 blacksheep-2.0a6/blacksheep.egg-info/
--rw-rw-rw-   0        0        0    10662 2023-04-28 06:03:13.000000 blacksheep-2.0a6/blacksheep.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4301 2023-04-28 06:03:13.000000 blacksheep-2.0a6/blacksheep.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 06:03:13.000000 blacksheep-2.0a6/blacksheep.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      268 2023-04-28 06:03:13.000000 blacksheep-2.0a6/blacksheep.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-28 06:03:13.000000 blacksheep-2.0a6/blacksheep.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1352 2023-04-28 05:59:53.000000 blacksheep-2.0a6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-28 06:03:13.771270 blacksheep-2.0a6/setup.cfg
--rw-rw-rw-   0        0        0     1275 2023-04-28 05:59:53.000000 blacksheep-2.0a6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 06:03:13.771270 blacksheep-2.0a6/tests/
--rw-rw-rw-   0        0        0   113290 2023-04-28 05:59:53.000000 blacksheep-2.0a6/tests/test_application.py
--rw-rw-rw-   0        0        0    18585 2023-04-28 05:59:53.000000 blacksheep-2.0a6/tests/test_auth.py
--rw-rw-rw-   0        0        0     2294 2023-04-28 05:59:53.000000 blacksheep-2.0a6/tests/test_auth_cookie.py
--rw-rw-rw-   0        0        0    19745 2023-04-28 05:59:53.000000 blacksheep-2.0a6/tests/test_bindings.py
--rw-rw-rw-   0        0        0     3540 2023-04-28 05:59:53.000000 blacksheep-2.0a6/tests/test_caching.py
--rw-rw-rw-   0        0        0     9781 2023-04-28 05:59:53.000000 blacksheep-2.0a6/tests/test_contents.py
--rw-rw-rw-   0        0        0    26270 2023-04-28 05:59:53.000000 blacksheep-2.0a6/tests/test_controllers.py
--rw-rw-rw-   0        0        0     7424 2023-04-28 05:59:53.000000 blacksheep-2.0a6/tests/test_cookies.py
--rw-rw-rw-   0        0        0    20542 2023-04-28 05:59:53.000000 blacksheep-2.0a6/tests/test_cors.py
--rw-rw-rw-   0        0        0    21340 2023-04-28 05:59:53.000000 blacksheep-2.0a6/tests/test_csrf.py
--rw-rw-rw-   0        0        0     1427 2023-04-28 05:59:53.000000 blacksheep-2.0a6/tests/test_dataprotection.py
--rw-rw-rw-   0        0        0      464 2023-04-28 05:59:53.000000 blacksheep-2.0a6/tests/test_env.py
--rw-rw-rw-   0        0        0     5565 2023-04-28 05:59:53.000000 blacksheep-2.0a6/tests/test_files_handler.py
--rw-rw-rw-   0        0        0    25887 2023-04-28 05:59:53.000000 blacksheep-2.0a6/tests/test_files_serving.py
--rw-rw-rw-   0        0        0    20844 2023-04-28 05:59:53.000000 blacksheep-2.0a6/tests/test_forwarding.py
--rw-rw-rw-   0        0        0     3531 2023-04-28 05:59:53.000000 blacksheep-2.0a6/tests/test_gzip.py
--rw-rw-rw-   0        0        0     6298 2023-04-28 05:59:53.000000 blacksheep-2.0a6/tests/test_headers.py
--rw-rw-rw-   0        0        0     5620 2023-04-28 05:59:53.000000 blacksheep-2.0a6/tests/test_multipart.py
--rw-rw-rw-   0        0        0    19342 2023-04-28 05:59:53.000000 blacksheep-2.0a6/tests/test_normalization.py
--rw-rw-rw-   0        0        0    28307 2023-04-28 05:59:53.000000 blacksheep-2.0a6/tests/test_openapi_docstrings.py
--rw-rw-rw-   0        0        0    70967 2023-04-28 05:59:53.000000 blacksheep-2.0a6/tests/test_openapi_v3.py
--rw-rw-rw-   0        0        0     1141 2023-04-28 05:59:53.000000 blacksheep-2.0a6/tests/test_pathutils.py
--rw-rw-rw-   0        0        0     5288 2023-04-28 05:59:53.000000 blacksheep-2.0a6/tests/test_ranges.py
--rw-rw-rw-   0        0        0    16338 2023-04-28 05:59:53.000000 blacksheep-2.0a6/tests/test_requests.py
--rw-rw-rw-   0        0        0    28976 2023-04-28 05:59:53.000000 blacksheep-2.0a6/tests/test_responses.py
--rw-rw-rw-   0        0        0    26915 2023-04-28 05:59:53.000000 blacksheep-2.0a6/tests/test_router.py
--rw-rw-rw-   0        0        0     8607 2023-04-28 05:59:53.000000 blacksheep-2.0a6/tests/test_sessions.py
--rw-rw-rw-   0        0        0     8666 2023-04-28 05:59:53.000000 blacksheep-2.0a6/tests/test_templating.py
--rw-rw-rw-   0        0        0     7043 2023-04-28 05:59:53.000000 blacksheep-2.0a6/tests/test_testing.py
--rw-rw-rw-   0        0        0     3220 2023-04-28 05:59:53.000000 blacksheep-2.0a6/tests/test_url.py
--rw-rw-rw-   0        0        0     1401 2023-04-28 05:59:53.000000 blacksheep-2.0a6/tests/test_utils.py
--rw-rw-rw-   0        0        0    12812 2023-04-28 05:59:53.000000 blacksheep-2.0a6/tests/test_websocket.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:10:13.637802 blacksheep-2.0a7/
+-rw-rw-rw-   0        0        0     1072 2023-05-31 06:09:09.000000 blacksheep-2.0a7/LICENSE
+-rw-rw-rw-   0        0        0      233 2023-05-31 06:09:09.000000 blacksheep-2.0a7/MANIFEST.in
+-rw-rw-rw-   0        0        0    10662 2023-05-31 06:10:13.637802 blacksheep-2.0a7/PKG-INFO
+-rw-rw-rw-   0        0        0     9484 2023-05-31 06:09:09.000000 blacksheep-2.0a7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 06:10:13.575302 blacksheep-2.0a7/blacksheep/
+-rw-rw-rw-   0        0        0     4197 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/__init__.py
+-rw-rw-rw-   0        0        0      433 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/asgi.pyi
+-rw-rw-rw-   0        0        0   710102 2023-05-31 06:09:44.000000 blacksheep-2.0a7/blacksheep/baseapp.c
+-rw-rw-rw-   0        0        0      567 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/baseapp.pxd
+-rw-rw-rw-   0        0        0     1535 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/baseapp.pyi
+-rw-rw-rw-   0        0        0     6169 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/baseapp.pyx
+drwxrwxrwx   0        0        0        0 2023-05-31 06:10:13.575302 blacksheep-2.0a7/blacksheep/client/
+-rw-rw-rw-   0        0        0      396 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/client/__init__.py
+-rw-rw-rw-   0        0        0    13126 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/client/connection.py
+-rw-rw-rw-   0        0        0    10499 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/client/cookies.py
+-rw-rw-rw-   0        0        0     2004 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/client/exceptions.py
+-rw-rw-rw-   0        0        0     4753 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/client/pool.py
+-rw-rw-rw-   0        0        0    15045 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/client/session.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:10:13.575302 blacksheep-2.0a7/blacksheep/common/
+-rw-rw-rw-   0        0        0      397 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:10:13.575302 blacksheep-2.0a7/blacksheep/common/files/
+-rw-rw-rw-   0        0        0        0 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/common/files/__init__.py
+-rw-rw-rw-   0        0        0     3371 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/common/files/asyncfs.py
+-rw-rw-rw-   0        0        0      938 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/common/files/info.py
+-rw-rw-rw-   0        0        0      679 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/common/files/pathsutils.py
+-rw-rw-rw-   0        0        0     1457 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/common/types.py
+-rw-rw-rw-   0        0        0   967940 2023-05-31 06:09:42.000000 blacksheep-2.0a7/blacksheep/contents.c
+-rw-rw-rw-   0        0        0     1042 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/contents.pxd
+-rw-rw-rw-   0        0        0     3061 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/contents.pyi
+-rw-rw-rw-   0        0        0     7476 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/contents.pyx
+-rw-rw-rw-   0        0        0   709915 2023-05-31 06:09:40.000000 blacksheep-2.0a7/blacksheep/cookies.c
+-rw-rw-rw-   0        0        0      981 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/cookies.pxd
+-rw-rw-rw-   0        0        0     1332 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/cookies.pyi
+-rw-rw-rw-   0        0        0     6498 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/cookies.pyx
+-rw-rw-rw-   0        0        0   700177 2023-05-31 06:09:39.000000 blacksheep-2.0a7/blacksheep/exceptions.c
+-rw-rw-rw-   0        0        0      421 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/exceptions.pxd
+-rw-rw-rw-   0        0        0     1707 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/exceptions.pyi
+-rw-rw-rw-   0        0        0     1774 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/exceptions.pyx
+-rw-rw-rw-   0        0        0   589288 2023-05-31 06:09:39.000000 blacksheep-2.0a7/blacksheep/headers.c
+-rw-rw-rw-   0        0        0      798 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/headers.pxd
+-rw-rw-rw-   0        0        0     1876 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/headers.pyi
+-rw-rw-rw-   0        0        0     5660 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/headers.pyx
+drwxrwxrwx   0        0        0        0 2023-05-31 06:10:13.575302 blacksheep-2.0a7/blacksheep/includes/
+-rw-rw-rw-   0        0        0       44 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/includes/consts.pxi
+-rw-rw-rw-   0        0        0  1184581 2023-05-31 06:09:43.000000 blacksheep-2.0a7/blacksheep/messages.c
+-rw-rw-rw-   0        0        0     2123 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/messages.pxd
+-rw-rw-rw-   0        0        0     5566 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/messages.pyi
+-rw-rw-rw-   0        0        0    18461 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/messages.pyx
+-rw-rw-rw-   0        0        0      587 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/middlewares.py
+-rw-rw-rw-   0        0        0     3320 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/multipart.py
+-rw-rw-rw-   0        0        0      434 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/normalization.py
+-rw-rw-rw-   0        0        0        0 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/py.typed
+-rw-rw-rw-   0        0        0     5564 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/ranges.py
+-rw-rw-rw-   0        0        0   632523 2023-05-31 06:09:43.000000 blacksheep-2.0a7/blacksheep/scribe.c
+-rw-rw-rw-   0        0        0      753 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/scribe.pxd
+-rw-rw-rw-   0        0        0      841 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/scribe.pyi
+-rw-rw-rw-   0        0        0     9277 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/scribe.pyx
+drwxrwxrwx   0        0        0        0 2023-05-31 06:10:13.590928 blacksheep-2.0a7/blacksheep/server/
+-rw-rw-rw-   0        0        0      180 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/__init__.py
+-rw-rw-rw-   0        0        0    29511 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/application.py
+-rw-rw-rw-   0        0        0     2537 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/asgi.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:10:13.590928 blacksheep-2.0a7/blacksheep/server/authentication/
+-rw-rw-rw-   0        0        0     1838 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/authentication/__init__.py
+-rw-rw-rw-   0        0        0     4376 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/authentication/cookie.py
+-rw-rw-rw-   0        0        0     5275 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/authentication/jwt.py
+-rw-rw-rw-   0        0        0    37888 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/authentication/oidc.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:10:13.590928 blacksheep-2.0a7/blacksheep/server/authorization/
+-rw-rw-rw-   0        0        0     3345 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/authorization/__init__.py
+-rw-rw-rw-   0        0        0    27359 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/bindings.py
+-rw-rw-rw-   0        0        0     4337 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/compression.py
+-rw-rw-rw-   0        0        0    13325 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/controllers.py
+-rw-rw-rw-   0        0        0    11679 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/cors.py
+-rw-rw-rw-   0        0        0    13278 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/csrf.py
+-rw-rw-rw-   0        0        0     1581 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/dataprotection.py
+-rw-rw-rw-   0        0        0     1932 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/di.py
+-rw-rw-rw-   0        0        0     1316 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/env.py
+-rw-rw-rw-   0        0        0     1679 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/errors.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:10:13.590928 blacksheep-2.0a7/blacksheep/server/files/
+-rw-rw-rw-   0        0        0     9368 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/files/__init__.py
+-rw-rw-rw-   0        0        0     8717 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/files/dynamic.py
+-rw-rw-rw-   0        0        0     1134 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/files/static.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:10:13.590928 blacksheep-2.0a7/blacksheep/server/headers/
+-rw-rw-rw-   0        0        0        0 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/headers/__init__.py
+-rw-rw-rw-   0        0        0    11234 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/headers/cache.py
+-rw-rw-rw-   0        0        0    19420 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/normalization.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:10:13.590928 blacksheep-2.0a7/blacksheep/server/openapi/
+-rw-rw-rw-   0        0        0        0 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/openapi/__init__.py
+-rw-rw-rw-   0        0        0    13395 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/openapi/common.py
+-rw-rw-rw-   0        0        0    16431 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/openapi/docstrings.py
+-rw-rw-rw-   0        0        0      814 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/openapi/exceptions.py
+-rw-rw-rw-   0        0        0     2831 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/openapi/ui.py
+-rw-rw-rw-   0        0        0    39317 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/openapi/v3.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:10:13.606551 blacksheep-2.0a7/blacksheep/server/remotes/
+-rw-rw-rw-   0        0        0        0 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/remotes/__init__.py
+-rw-rw-rw-   0        0        0    13119 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/remotes/forwarding.py
+-rw-rw-rw-   0        0        0      963 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/remotes/hosts.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:10:13.606551 blacksheep-2.0a7/blacksheep/server/rendering/
+-rw-rw-rw-   0        0        0        0 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/rendering/__init__.py
+-rw-rw-rw-   0        0        0      765 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/rendering/abc.py
+-rw-rw-rw-   0        0        0     4016 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/rendering/jinja2.py
+-rw-rw-rw-   0        0        0      417 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/rendering/models.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:10:13.606551 blacksheep-2.0a7/blacksheep/server/res/
+-rw-rw-rw-   0        0        0        0 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/res/__init__.py
+-rw-rw-rw-   0        0        0     1356 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/res/error.css
+-rw-rw-rw-   0        0        0     1028 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/res/error.html
+-rw-rw-rw-   0        0        0      331 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/res/fileslist.html
+-rw-rw-rw-   0        0        0      590 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/res/redoc-ui.html
+-rw-rw-rw-   0        0        0      841 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/res/swagger-ui.html
+-rw-rw-rw-   0        0        0      263 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/resources.py
+-rw-rw-rw-   0        0        0    10477 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/responses.py
+-rw-rw-rw-   0        0        0    26805 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/routing.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:10:13.606551 blacksheep-2.0a7/blacksheep/server/security/
+-rw-rw-rw-   0        0        0      417 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/security/__init__.py
+-rw-rw-rw-   0        0        0      848 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/security/hsts.py
+-rw-rw-rw-   0        0        0     5352 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/server/websocket.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:10:13.606551 blacksheep-2.0a7/blacksheep/sessions/
+-rw-rw-rw-   0        0        0     5399 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/sessions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:10:13.606551 blacksheep-2.0a7/blacksheep/settings/
+-rw-rw-rw-   0        0        0       76 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/settings/__init__.py
+-rw-rw-rw-   0        0        0      538 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/settings/di.py
+-rw-rw-rw-   0        0        0     1073 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/settings/html.py
+-rw-rw-rw-   0        0        0      894 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/settings/json.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:10:13.606551 blacksheep-2.0a7/blacksheep/testing/
+-rw-rw-rw-   0        0        0      398 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/testing/__init__.py
+-rw-rw-rw-   0        0        0     4379 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/testing/client.py
+-rw-rw-rw-   0        0        0     3755 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/testing/helpers.py
+-rw-rw-rw-   0        0        0     1440 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/testing/messages.py
+-rw-rw-rw-   0        0        0     2659 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/testing/simulator.py
+-rw-rw-rw-   0        0        0   418258 2023-05-31 06:09:38.000000 blacksheep-2.0a7/blacksheep/url.c
+-rw-rw-rw-   0        0        0      751 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/url.pxd
+-rw-rw-rw-   0        0        0      707 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/url.pyi
+-rw-rw-rw-   0        0        0     4061 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/url.pyx
+drwxrwxrwx   0        0        0        0 2023-05-31 06:10:13.606551 blacksheep-2.0a7/blacksheep/utils/
+-rw-rw-rw-   0        0        0     1115 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/utils/__init__.py
+-rw-rw-rw-   0        0        0     2733 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/utils/aio.py
+-rw-rw-rw-   0        0        0      712 2023-05-31 06:09:09.000000 blacksheep-2.0a7/blacksheep/utils/meta.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:10:13.575302 blacksheep-2.0a7/blacksheep.egg-info/
+-rw-rw-rw-   0        0        0    10662 2023-05-31 06:10:13.000000 blacksheep-2.0a7/blacksheep.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4301 2023-05-31 06:10:13.000000 blacksheep-2.0a7/blacksheep.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 06:10:13.000000 blacksheep-2.0a7/blacksheep.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      268 2023-05-31 06:10:13.000000 blacksheep-2.0a7/blacksheep.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-31 06:10:13.000000 blacksheep-2.0a7/blacksheep.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1352 2023-05-31 06:09:09.000000 blacksheep-2.0a7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-31 06:10:13.637802 blacksheep-2.0a7/setup.cfg
+-rw-rw-rw-   0        0        0     1275 2023-05-31 06:09:09.000000 blacksheep-2.0a7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:10:13.637802 blacksheep-2.0a7/tests/
+-rw-rw-rw-   0        0        0   113290 2023-05-31 06:09:09.000000 blacksheep-2.0a7/tests/test_application.py
+-rw-rw-rw-   0        0        0    18585 2023-05-31 06:09:09.000000 blacksheep-2.0a7/tests/test_auth.py
+-rw-rw-rw-   0        0        0     2294 2023-05-31 06:09:09.000000 blacksheep-2.0a7/tests/test_auth_cookie.py
+-rw-rw-rw-   0        0        0    19745 2023-05-31 06:09:09.000000 blacksheep-2.0a7/tests/test_bindings.py
+-rw-rw-rw-   0        0        0     3540 2023-05-31 06:09:09.000000 blacksheep-2.0a7/tests/test_caching.py
+-rw-rw-rw-   0        0        0     9781 2023-05-31 06:09:09.000000 blacksheep-2.0a7/tests/test_contents.py
+-rw-rw-rw-   0        0        0    26270 2023-05-31 06:09:09.000000 blacksheep-2.0a7/tests/test_controllers.py
+-rw-rw-rw-   0        0        0     7424 2023-05-31 06:09:09.000000 blacksheep-2.0a7/tests/test_cookies.py
+-rw-rw-rw-   0        0        0    21883 2023-05-31 06:09:09.000000 blacksheep-2.0a7/tests/test_cors.py
+-rw-rw-rw-   0        0        0    21340 2023-05-31 06:09:09.000000 blacksheep-2.0a7/tests/test_csrf.py
+-rw-rw-rw-   0        0        0     1427 2023-05-31 06:09:09.000000 blacksheep-2.0a7/tests/test_dataprotection.py
+-rw-rw-rw-   0        0        0      464 2023-05-31 06:09:09.000000 blacksheep-2.0a7/tests/test_env.py
+-rw-rw-rw-   0        0        0     5565 2023-05-31 06:09:09.000000 blacksheep-2.0a7/tests/test_files_handler.py
+-rw-rw-rw-   0        0        0    25887 2023-05-31 06:09:09.000000 blacksheep-2.0a7/tests/test_files_serving.py
+-rw-rw-rw-   0        0        0    20844 2023-05-31 06:09:09.000000 blacksheep-2.0a7/tests/test_forwarding.py
+-rw-rw-rw-   0        0        0     3531 2023-05-31 06:09:09.000000 blacksheep-2.0a7/tests/test_gzip.py
+-rw-rw-rw-   0        0        0     6298 2023-05-31 06:09:09.000000 blacksheep-2.0a7/tests/test_headers.py
+-rw-rw-rw-   0        0        0     5620 2023-05-31 06:09:09.000000 blacksheep-2.0a7/tests/test_multipart.py
+-rw-rw-rw-   0        0        0    19342 2023-05-31 06:09:09.000000 blacksheep-2.0a7/tests/test_normalization.py
+-rw-rw-rw-   0        0        0    28307 2023-05-31 06:09:09.000000 blacksheep-2.0a7/tests/test_openapi_docstrings.py
+-rw-rw-rw-   0        0        0    74098 2023-05-31 06:09:09.000000 blacksheep-2.0a7/tests/test_openapi_v3.py
+-rw-rw-rw-   0        0        0     1141 2023-05-31 06:09:09.000000 blacksheep-2.0a7/tests/test_pathutils.py
+-rw-rw-rw-   0        0        0     5288 2023-05-31 06:09:09.000000 blacksheep-2.0a7/tests/test_ranges.py
+-rw-rw-rw-   0        0        0    16338 2023-05-31 06:09:09.000000 blacksheep-2.0a7/tests/test_requests.py
+-rw-rw-rw-   0        0        0    28976 2023-05-31 06:09:09.000000 blacksheep-2.0a7/tests/test_responses.py
+-rw-rw-rw-   0        0        0    26915 2023-05-31 06:09:09.000000 blacksheep-2.0a7/tests/test_router.py
+-rw-rw-rw-   0        0        0     8607 2023-05-31 06:09:09.000000 blacksheep-2.0a7/tests/test_sessions.py
+-rw-rw-rw-   0        0        0     8666 2023-05-31 06:09:09.000000 blacksheep-2.0a7/tests/test_templating.py
+-rw-rw-rw-   0        0        0     7043 2023-05-31 06:09:09.000000 blacksheep-2.0a7/tests/test_testing.py
+-rw-rw-rw-   0        0        0     3220 2023-05-31 06:09:09.000000 blacksheep-2.0a7/tests/test_url.py
+-rw-rw-rw-   0        0        0     1401 2023-05-31 06:09:09.000000 blacksheep-2.0a7/tests/test_utils.py
+-rw-rw-rw-   0        0        0    12812 2023-05-31 06:09:09.000000 blacksheep-2.0a7/tests/test_websocket.py
```

### Comparing `blacksheep-2.0a6/LICENSE` & `blacksheep-2.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/PKG-INFO` & `blacksheep-2.0a7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blacksheep
-Version: 2.0a6
+Version: 2.0a7
 Summary: Fast web framework for Python asyncio
 Author-email: Roberto Prevato <roberto.prevato@gmail.com>
 Project-URL: Homepage, https://github.com/Neoteroi/BlackSheep
 Project-URL: Bug Tracker, https://github.com/Neoteroi/BlackSheep/issues
 Keywords: blacksheep,web framework,asyncio
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: blacksheep Version: 2.0a6 Summary: Fast web
+Metadata-Version: 2.1 Name: blacksheep Version: 2.0a7 Summary: Fast web
 framework for Python asyncio Author-email: Roberto Prevato
 prevato@gmail.com> Project-URL: Homepage, https://github.com/Neoteroi/
 BlackSheep Project-URL: Bug Tracker, https://github.com/Neoteroi/BlackSheep/
 issues Keywords: blacksheep,web framework,asyncio Classifier: Development
 Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `blacksheep-2.0a6/README.md` & `blacksheep-2.0a7/README.md`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/__init__.py` & `blacksheep-2.0a7/blacksheep/__init__.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/baseapp.c` & `blacksheep-2.0a7/blacksheep/baseapp.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.35 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -74,16 +74,20 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -2146,30 +2150,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
@@ -2227,15 +2231,15 @@
 #endif
 #define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* FunctionImport.proto */
-static int __Pyx_ImportFunction(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
+static int __Pyx_ImportFunction_0_29_35(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 static PyObject *__pyx_f_10blacksheep_7baseapp_15BaseApplication_get_http_exception_handler(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, struct __pyx_obj_10blacksheep_10exceptions_HTTPException *__pyx_v_http_exception); /* proto*/
 static PyObject *__pyx_f_10blacksheep_7baseapp_15BaseApplication_get_exception_handler(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, PyObject *__pyx_v_exception); /* proto*/
 
@@ -10087,15 +10091,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct__handle_not_found *__pyx_freelist_10blacksheep_7baseapp___pyx_scope_struct__handle_not_found[8];
 static int __pyx_freecount_10blacksheep_7baseapp___pyx_scope_struct__handle_not_found = 0;
 
@@ -10204,15 +10208,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_1_handle_bad_request *__pyx_freelist_10blacksheep_7baseapp___pyx_scope_struct_1_handle_bad_request[8];
 static int __pyx_freecount_10blacksheep_7baseapp___pyx_scope_struct_1_handle_bad_request = 0;
 
@@ -10321,15 +10325,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_2_common_http_exception_handler *__pyx_freelist_10blacksheep_7baseapp___pyx_scope_struct_2_common_http_exception_handler[8];
 static int __pyx_freecount_10blacksheep_7baseapp___pyx_scope_struct_2_common_http_exception_handler = 0;
 
@@ -10438,15 +10442,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_3_log_unhandled_exc *__pyx_freelist_10blacksheep_7baseapp___pyx_scope_struct_3_log_unhandled_exc[8];
 static int __pyx_freecount_10blacksheep_7baseapp___pyx_scope_struct_3_log_unhandled_exc = 0;
 
@@ -10555,15 +10559,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_4_log_handled_exc *__pyx_freelist_10blacksheep_7baseapp___pyx_scope_struct_4_log_handled_exc[8];
 static int __pyx_freecount_10blacksheep_7baseapp___pyx_scope_struct_4_log_handled_exc = 0;
 
@@ -10672,15 +10676,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_5_handle *__pyx_freelist_10blacksheep_7baseapp___pyx_scope_struct_5_handle[8];
 static int __pyx_freecount_10blacksheep_7baseapp___pyx_scope_struct_5_handle = 0;
 
@@ -10821,15 +10825,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_6_handle_request_handler_exception *__pyx_freelist_10blacksheep_7baseapp___pyx_scope_struct_6_handle_request_handler_exception[8];
 static int __pyx_freecount_10blacksheep_7baseapp___pyx_scope_struct_6_handle_request_handler_exception = 0;
 
@@ -10938,15 +10942,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_7_handle_internal_server_error *__pyx_freelist_10blacksheep_7baseapp___pyx_scope_struct_7_handle_internal_server_error[8];
 static int __pyx_freecount_10blacksheep_7baseapp___pyx_scope_struct_7_handle_internal_server_error = 0;
 
@@ -11067,15 +11071,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_8__apply_exception_handler *__pyx_freelist_10blacksheep_7baseapp___pyx_scope_struct_8__apply_exception_handler[8];
 static int __pyx_freecount_10blacksheep_7baseapp___pyx_scope_struct_8__apply_exception_handler = 0;
 
@@ -11216,15 +11220,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_9_handle_http_exception *__pyx_freelist_10blacksheep_7baseapp___pyx_scope_struct_9_handle_http_exception[8];
 static int __pyx_freecount_10blacksheep_7baseapp___pyx_scope_struct_9_handle_http_exception = 0;
 
@@ -11337,15 +11341,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_10_handle_exception *__pyx_freelist_10blacksheep_7baseapp___pyx_scope_struct_10_handle_exception[8];
 static int __pyx_freecount_10blacksheep_7baseapp___pyx_scope_struct_10_handle_exception = 0;
 
@@ -11458,15 +11462,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -11933,123 +11937,70 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule("blacksheep.exceptions"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_10blacksheep_10exceptions_MessageAborted = __Pyx_ImportType(__pyx_t_1, "blacksheep.exceptions", "MessageAborted", sizeof(struct __pyx_obj_10blacksheep_10exceptions_MessageAborted), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_10exceptions_MessageAborted),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_10exceptions_MessageAborted) __PYX_ERR(4, 4, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_HTTPException = __Pyx_ImportType(__pyx_t_1, "blacksheep.exceptions", "HTTPException", sizeof(struct __pyx_obj_10blacksheep_10exceptions_HTTPException), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_10exceptions_HTTPException),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_10exceptions_HTTPException) __PYX_ERR(4, 8, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_BadRequest = __Pyx_ImportType(__pyx_t_1, "blacksheep.exceptions", "BadRequest", sizeof(struct __pyx_obj_10blacksheep_10exceptions_BadRequest), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_10exceptions_BadRequest),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_10exceptions_BadRequest) __PYX_ERR(4, 12, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_BadRequestFormat = __Pyx_ImportType(__pyx_t_1, "blacksheep.exceptions", "BadRequestFormat", sizeof(struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_10exceptions_BadRequestFormat) __PYX_ERR(4, 16, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_NotFound = __Pyx_ImportType(__pyx_t_1, "blacksheep.exceptions", "NotFound", sizeof(struct __pyx_obj_10blacksheep_10exceptions_NotFound), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_10exceptions_NotFound),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_10exceptions_NotFound) __PYX_ERR(4, 20, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_InvalidArgument = __Pyx_ImportType(__pyx_t_1, "blacksheep.exceptions", "InvalidArgument", sizeof(struct __pyx_obj_10blacksheep_10exceptions_InvalidArgument), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_10exceptions_InvalidArgument),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_10exceptions_InvalidArgument) __PYX_ERR(4, 24, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_InvalidOperation = __Pyx_ImportType(__pyx_t_1, "blacksheep.exceptions", "InvalidOperation", sizeof(struct __pyx_obj_10blacksheep_10exceptions_InvalidOperation), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_10exceptions_InvalidOperation),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_10exceptions_InvalidOperation) __PYX_ERR(4, 28, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_MessageAborted = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "MessageAborted", sizeof(struct __pyx_obj_10blacksheep_10exceptions_MessageAborted), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_MessageAborted),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_MessageAborted) __PYX_ERR(4, 4, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_HTTPException = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "HTTPException", sizeof(struct __pyx_obj_10blacksheep_10exceptions_HTTPException), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_HTTPException),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_HTTPException) __PYX_ERR(4, 8, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_BadRequest = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "BadRequest", sizeof(struct __pyx_obj_10blacksheep_10exceptions_BadRequest), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_BadRequest),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_BadRequest) __PYX_ERR(4, 12, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_BadRequestFormat = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "BadRequestFormat", sizeof(struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_BadRequestFormat) __PYX_ERR(4, 16, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_NotFound = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "NotFound", sizeof(struct __pyx_obj_10blacksheep_10exceptions_NotFound), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_NotFound),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_NotFound) __PYX_ERR(4, 20, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_InvalidArgument = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "InvalidArgument", sizeof(struct __pyx_obj_10blacksheep_10exceptions_InvalidArgument), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_InvalidArgument),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_InvalidArgument) __PYX_ERR(4, 24, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_InvalidOperation = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "InvalidOperation", sizeof(struct __pyx_obj_10blacksheep_10exceptions_InvalidOperation), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_InvalidOperation),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_InvalidOperation) __PYX_ERR(4, 28, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("blacksheep.contents"); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_10blacksheep_8contents_Content = __Pyx_ImportType(__pyx_t_1, "blacksheep.contents", "Content", sizeof(struct __pyx_obj_10blacksheep_8contents_Content), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_8contents_Content),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_8contents_Content) __PYX_ERR(5, 8, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_StreamedContent = __Pyx_ImportType(__pyx_t_1, "blacksheep.contents", "StreamedContent", sizeof(struct __pyx_obj_10blacksheep_8contents_StreamedContent), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_8contents_StreamedContent),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_8contents_StreamedContent) __PYX_ERR(5, 14, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_ASGIContent = __Pyx_ImportType(__pyx_t_1, "blacksheep.contents", "ASGIContent", sizeof(struct __pyx_obj_10blacksheep_8contents_ASGIContent), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_8contents_ASGIContent),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_8contents_ASGIContent) __PYX_ERR(5, 18, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_Content = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "Content", sizeof(struct __pyx_obj_10blacksheep_8contents_Content), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_Content),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_Content) __PYX_ERR(5, 8, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_StreamedContent = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "StreamedContent", sizeof(struct __pyx_obj_10blacksheep_8contents_StreamedContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_StreamedContent),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_StreamedContent) __PYX_ERR(5, 14, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_ASGIContent = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "ASGIContent", sizeof(struct __pyx_obj_10blacksheep_8contents_ASGIContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_ASGIContent),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_ASGIContent) __PYX_ERR(5, 18, __pyx_L1_error)
   __pyx_vtabptr_10blacksheep_8contents_ASGIContent = (struct __pyx_vtabstruct_10blacksheep_8contents_ASGIContent*)__Pyx_GetVtable(__pyx_ptype_10blacksheep_8contents_ASGIContent->tp_dict); if (unlikely(!__pyx_vtabptr_10blacksheep_8contents_ASGIContent)) __PYX_ERR(5, 18, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_TextContent = __Pyx_ImportType(__pyx_t_1, "blacksheep.contents", "TextContent", sizeof(struct __pyx_obj_10blacksheep_8contents_TextContent), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_8contents_TextContent),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_8contents_TextContent) __PYX_ERR(5, 23, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_HTMLContent = __Pyx_ImportType(__pyx_t_1, "blacksheep.contents", "HTMLContent", sizeof(struct __pyx_obj_10blacksheep_8contents_HTMLContent), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_8contents_HTMLContent),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_8contents_HTMLContent) __PYX_ERR(5, 27, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_JSONContent = __Pyx_ImportType(__pyx_t_1, "blacksheep.contents", "JSONContent", sizeof(struct __pyx_obj_10blacksheep_8contents_JSONContent), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_8contents_JSONContent),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_8contents_JSONContent) __PYX_ERR(5, 31, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_FormContent = __Pyx_ImportType(__pyx_t_1, "blacksheep.contents", "FormContent", sizeof(struct __pyx_obj_10blacksheep_8contents_FormContent), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_8contents_FormContent),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_8contents_FormContent) __PYX_ERR(5, 35, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_FormPart = __Pyx_ImportType(__pyx_t_1, "blacksheep.contents", "FormPart", sizeof(struct __pyx_obj_10blacksheep_8contents_FormPart), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_8contents_FormPart),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_8contents_FormPart) __PYX_ERR(5, 39, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_MultiPartFormData = __Pyx_ImportType(__pyx_t_1, "blacksheep.contents", "MultiPartFormData", sizeof(struct __pyx_obj_10blacksheep_8contents_MultiPartFormData), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_8contents_MultiPartFormData),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_8contents_MultiPartFormData) __PYX_ERR(5, 47, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_TextContent = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "TextContent", sizeof(struct __pyx_obj_10blacksheep_8contents_TextContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_TextContent),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_TextContent) __PYX_ERR(5, 23, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_HTMLContent = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "HTMLContent", sizeof(struct __pyx_obj_10blacksheep_8contents_HTMLContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_HTMLContent),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_HTMLContent) __PYX_ERR(5, 27, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_JSONContent = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "JSONContent", sizeof(struct __pyx_obj_10blacksheep_8contents_JSONContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_JSONContent),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_JSONContent) __PYX_ERR(5, 31, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_FormContent = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "FormContent", sizeof(struct __pyx_obj_10blacksheep_8contents_FormContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_FormContent),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_FormContent) __PYX_ERR(5, 35, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_FormPart = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "FormPart", sizeof(struct __pyx_obj_10blacksheep_8contents_FormPart), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_FormPart),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_FormPart) __PYX_ERR(5, 39, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_MultiPartFormData = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "MultiPartFormData", sizeof(struct __pyx_obj_10blacksheep_8contents_MultiPartFormData), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_MultiPartFormData),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_MultiPartFormData) __PYX_ERR(5, 47, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(6, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(6, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("datetime"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_8datetime_date = __Pyx_ImportType(__pyx_t_1, "datetime", "date", sizeof(PyDateTime_Date), __PYX_GET_STRUCT_ALIGNMENT(PyDateTime_Date),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_8datetime_date) __PYX_ERR(3, 9, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_time = __Pyx_ImportType(__pyx_t_1, "datetime", "time", sizeof(PyDateTime_Time), __PYX_GET_STRUCT_ALIGNMENT(PyDateTime_Time),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_8datetime_time) __PYX_ERR(3, 12, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_datetime = __Pyx_ImportType(__pyx_t_1, "datetime", "datetime", sizeof(PyDateTime_DateTime), __PYX_GET_STRUCT_ALIGNMENT(PyDateTime_DateTime),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_8datetime_datetime) __PYX_ERR(3, 15, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_timedelta = __Pyx_ImportType(__pyx_t_1, "datetime", "timedelta", sizeof(PyDateTime_Delta), __PYX_GET_STRUCT_ALIGNMENT(PyDateTime_Delta),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_8datetime_timedelta) __PYX_ERR(3, 18, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_tzinfo = __Pyx_ImportType(__pyx_t_1, "datetime", "tzinfo", sizeof(PyDateTime_TZInfo), __PYX_GET_STRUCT_ALIGNMENT(PyDateTime_TZInfo),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_8datetime_tzinfo) __PYX_ERR(3, 21, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_date = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "date", sizeof(PyDateTime_Date), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_Date),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_date) __PYX_ERR(3, 9, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_time = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "time", sizeof(PyDateTime_Time), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_Time),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_time) __PYX_ERR(3, 12, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_datetime = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "datetime", sizeof(PyDateTime_DateTime), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_DateTime),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_datetime) __PYX_ERR(3, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_timedelta = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "timedelta", sizeof(PyDateTime_Delta), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_Delta),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_timedelta) __PYX_ERR(3, 18, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_tzinfo = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "tzinfo", sizeof(PyDateTime_TZInfo), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_TZInfo),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_tzinfo) __PYX_ERR(3, 21, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("blacksheep.cookies"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_10blacksheep_7cookies_Cookie = __Pyx_ImportType(__pyx_t_1, "blacksheep.cookies", "Cookie", sizeof(struct __pyx_obj_10blacksheep_7cookies_Cookie), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_7cookies_Cookie),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_7cookies_Cookie) __PYX_ERR(7, 17, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_7cookies_Cookie = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.cookies", "Cookie", sizeof(struct __pyx_obj_10blacksheep_7cookies_Cookie), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_7cookies_Cookie),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_7cookies_Cookie) __PYX_ERR(7, 17, __pyx_L1_error)
   __pyx_vtabptr_10blacksheep_7cookies_Cookie = (struct __pyx_vtabstruct_10blacksheep_7cookies_Cookie*)__Pyx_GetVtable(__pyx_ptype_10blacksheep_7cookies_Cookie->tp_dict); if (unlikely(!__pyx_vtabptr_10blacksheep_7cookies_Cookie)) __PYX_ERR(7, 17, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("blacksheep.url"); if (unlikely(!__pyx_t_1)) __PYX_ERR(8, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_10blacksheep_3url_URL = __Pyx_ImportType(__pyx_t_1, "blacksheep.url", "URL", sizeof(struct __pyx_obj_10blacksheep_3url_URL), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_3url_URL),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_3url_URL) __PYX_ERR(8, 8, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_3url_URL = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.url", "URL", sizeof(struct __pyx_obj_10blacksheep_3url_URL), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_3url_URL),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_3url_URL) __PYX_ERR(8, 8, __pyx_L1_error)
   __pyx_vtabptr_10blacksheep_3url_URL = (struct __pyx_vtabstruct_10blacksheep_3url_URL*)__Pyx_GetVtable(__pyx_ptype_10blacksheep_3url_URL->tp_dict); if (unlikely(!__pyx_vtabptr_10blacksheep_3url_URL)) __PYX_ERR(8, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("blacksheep.messages"); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_10blacksheep_8messages_Message = __Pyx_ImportType(__pyx_t_1, "blacksheep.messages", "Message", sizeof(struct __pyx_obj_10blacksheep_8messages_Message), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_8messages_Message),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_8messages_Message) __PYX_ERR(9, 18, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8messages_Message = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.messages", "Message", sizeof(struct __pyx_obj_10blacksheep_8messages_Message), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8messages_Message),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8messages_Message) __PYX_ERR(9, 18, __pyx_L1_error)
   __pyx_vtabptr_10blacksheep_8messages_Message = (struct __pyx_vtabstruct_10blacksheep_8messages_Message*)__Pyx_GetVtable(__pyx_ptype_10blacksheep_8messages_Message->tp_dict); if (unlikely(!__pyx_vtabptr_10blacksheep_8messages_Message)) __PYX_ERR(9, 18, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8messages_Request = __Pyx_ImportType(__pyx_t_1, "blacksheep.messages", "Request", sizeof(struct __pyx_obj_10blacksheep_8messages_Request), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_8messages_Request),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_8messages_Request) __PYX_ERR(9, 45, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8messages_Request = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.messages", "Request", sizeof(struct __pyx_obj_10blacksheep_8messages_Request), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8messages_Request),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8messages_Request) __PYX_ERR(9, 45, __pyx_L1_error)
   __pyx_vtabptr_10blacksheep_8messages_Request = (struct __pyx_vtabstruct_10blacksheep_8messages_Request*)__Pyx_GetVtable(__pyx_ptype_10blacksheep_8messages_Request->tp_dict); if (unlikely(!__pyx_vtabptr_10blacksheep_8messages_Request)) __PYX_ERR(9, 45, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8messages_Response = __Pyx_ImportType(__pyx_t_1, "blacksheep.messages", "Response", sizeof(struct __pyx_obj_10blacksheep_8messages_Response), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_8messages_Response),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_8messages_Response) __PYX_ERR(9, 58, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8messages_Response = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.messages", "Response", sizeof(struct __pyx_obj_10blacksheep_8messages_Response), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8messages_Response),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8messages_Response) __PYX_ERR(9, 58, __pyx_L1_error)
   __pyx_vtabptr_10blacksheep_8messages_Response = (struct __pyx_vtabstruct_10blacksheep_8messages_Response*)__Pyx_GetVtable(__pyx_ptype_10blacksheep_8messages_Response->tp_dict); if (unlikely(!__pyx_vtabptr_10blacksheep_8messages_Response)) __PYX_ERR(9, 58, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -12070,21 +12021,21 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __pyx_t_1 = PyImport_ImportModule("blacksheep.contents"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportFunction(__pyx_t_1, "parse_www_form_urlencoded", (void (**)(void))&__pyx_f_10blacksheep_8contents_parse_www_form_urlencoded, "PyObject *(PyObject *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "parse_www_form_urlencoded", (void (**)(void))&__pyx_f_10blacksheep_8contents_parse_www_form_urlencoded, "PyObject *(PyObject *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("blacksheep.cookies"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportFunction(__pyx_t_1, "parse_cookie", (void (**)(void))&__pyx_f_10blacksheep_7cookies_parse_cookie, "struct __pyx_obj_10blacksheep_7cookies_Cookie *(PyObject *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "datetime_to_cookie_format", (void (**)(void))&__pyx_f_10blacksheep_7cookies_datetime_to_cookie_format, "PyObject *(PyDateTime_DateTime *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "write_cookie_for_response", (void (**)(void))&__pyx_f_10blacksheep_7cookies_write_cookie_for_response, "PyObject *(struct __pyx_obj_10blacksheep_7cookies_Cookie *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "parse_cookie", (void (**)(void))&__pyx_f_10blacksheep_7cookies_parse_cookie, "struct __pyx_obj_10blacksheep_7cookies_Cookie *(PyObject *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "datetime_to_cookie_format", (void (**)(void))&__pyx_f_10blacksheep_7cookies_datetime_to_cookie_format, "PyObject *(PyDateTime_DateTime *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "write_cookie_for_response", (void (**)(void))&__pyx_f_10blacksheep_7cookies_write_cookie_for_response, "PyObject *(struct __pyx_obj_10blacksheep_7cookies_Cookie *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -14531,15 +14482,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 #if PY_VERSION_HEX < 0x030500B1 || defined(__Pyx_IterableCoroutine_USED) || CYTHON_USE_ASYNC_SLOTS
 static CYTHON_INLINE PyObject *__Pyx__Coroutine_await(PyObject *coroutine) {
     __pyx_CoroutineAwaitObject *await = PyObject_GC_New(__pyx_CoroutineAwaitObject, __pyx_CoroutineAwaitType);
     if (unlikely(!await)) return NULL;
@@ -14683,15 +14637,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_Coroutine_init(void) {
     __pyx_CoroutineType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx_CoroutineType = __Pyx_FetchCommonType(&__pyx_CoroutineType_type);
     if (unlikely(!__pyx_CoroutineType))
@@ -14759,15 +14716,15 @@
 #if PY_VERSION_HEX >= 0x030500B2 || defined(PyCoro_CheckExact)
     if (PyCoro_CheckExact(obj)) {
         return __Pyx_NewRef(obj);
     } else
 #endif
 #if CYTHON_COMPILING_IN_CPYTHON && defined(CO_ITERABLE_COROUTINE)
 #if PY_VERSION_HEX >= 0x030C00A6
-    if (PyGen_CheckExact(obj) && (PyGen_GetCode(obj)->co_flags & CO_ITERABLE_COROUTINE)) {
+    if (PyGen_CheckExact(obj) && (PyGen_GetCode((PyGenObject*)obj)->co_flags & CO_ITERABLE_COROUTINE)) {
 #else
     if (PyGen_CheckExact(obj) && ((PyGenObject*)obj)->gi_code && ((PyCodeObject *)((PyGenObject*)obj)->gi_code)->co_flags & CO_ITERABLE_COROUTINE) {
 #endif
         return __Pyx_NewRef(obj);
     } else
 #endif
     {
@@ -15466,18 +15423,18 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -15523,22 +15480,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -15875,15 +15832,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -16147,15 +16104,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -16422,17 +16379,17 @@
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
 }
 
 /* FunctionImport */
-  #ifndef __PYX_HAVE_RT_ImportFunction
-#define __PYX_HAVE_RT_ImportFunction
-static int __Pyx_ImportFunction(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
+  #ifndef __PYX_HAVE_RT_ImportFunction_0_29_35
+#define __PYX_HAVE_RT_ImportFunction_0_29_35
+static int __Pyx_ImportFunction_0_29_35(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
     PyObject *d = 0;
     PyObject *cobj = 0;
     union {
         void (*fp)(void);
         void *p;
     } tmp;
     d = PyObject_GetAttrString(module, (char *)"__pyx_capi__");
```

### Comparing `blacksheep-2.0a6/blacksheep/baseapp.pxd` & `blacksheep-2.0a7/blacksheep/baseapp.pxd`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/baseapp.pyi` & `blacksheep-2.0a7/blacksheep/baseapp.pyi`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/baseapp.pyx` & `blacksheep-2.0a7/blacksheep/baseapp.pyx`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/client/connection.py` & `blacksheep-2.0a7/blacksheep/client/connection.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/client/cookies.py` & `blacksheep-2.0a7/blacksheep/client/cookies.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/client/exceptions.py` & `blacksheep-2.0a7/blacksheep/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/client/pool.py` & `blacksheep-2.0a7/blacksheep/client/pool.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/client/session.py` & `blacksheep-2.0a7/blacksheep/client/session.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/common/files/asyncfs.py` & `blacksheep-2.0a7/blacksheep/common/files/asyncfs.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/common/files/info.py` & `blacksheep-2.0a7/blacksheep/common/files/info.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/common/files/pathsutils.py` & `blacksheep-2.0a7/blacksheep/common/files/pathsutils.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/common/types.py` & `blacksheep-2.0a7/blacksheep/common/types.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/contents.c` & `blacksheep-2.0a7/blacksheep/contents.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.35 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -74,16 +74,20 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -1879,30 +1883,30 @@
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* SetVTable.proto */
 static int __Pyx_SetVtable(PyObject *dict, void *vtable);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* PatchInspect.proto */
 static PyObject* __Pyx_patch_inspect(PyObject* module);
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
@@ -15093,15 +15097,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_10blacksheep_8contents_StreamedContent(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_10blacksheep_8contents_StreamedContent *p;
   PyObject *o = __pyx_tp_new_10blacksheep_8contents_Content(t, a, k);
@@ -15116,18 +15120,15 @@
   #if CYTHON_USE_TP_FINALIZE
   if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->generator);
-  #if CYTHON_USE_TYPE_SLOTS
-  if (PyType_IS_GC(Py_TYPE(o)->tp_base))
-  #endif
-  PyObject_GC_Track(o);
+  if (PyType_IS_GC(__pyx_ptype_10blacksheep_8contents_Content)) PyObject_GC_Track(o);
   __pyx_tp_dealloc_10blacksheep_8contents_Content(o);
 }
 
 static int __pyx_tp_traverse_10blacksheep_8contents_StreamedContent(PyObject *o, visitproc v, void *a) {
   int e;
   struct __pyx_obj_10blacksheep_8contents_StreamedContent *p = (struct __pyx_obj_10blacksheep_8contents_StreamedContent *)o;
   e = ((likely(__pyx_ptype_10blacksheep_8contents_Content)) ? ((__pyx_ptype_10blacksheep_8contents_Content->tp_traverse) ? __pyx_ptype_10blacksheep_8contents_Content->tp_traverse(o, v, a) : 0) : __Pyx_call_next_tp_traverse(o, v, a, __pyx_tp_traverse_10blacksheep_8contents_StreamedContent)); if (e) return e;
@@ -15227,15 +15228,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_10blacksheep_8contents_ASGIContent __pyx_vtable_10blacksheep_8contents_ASGIContent;
 
 static PyObject *__pyx_tp_new_10blacksheep_8contents_ASGIContent(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_10blacksheep_8contents_ASGIContent *p;
@@ -15252,18 +15253,15 @@
   #if CYTHON_USE_TP_FINALIZE
   if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->receive);
-  #if CYTHON_USE_TYPE_SLOTS
-  if (PyType_IS_GC(Py_TYPE(o)->tp_base))
-  #endif
-  PyObject_GC_Track(o);
+  if (PyType_IS_GC(__pyx_ptype_10blacksheep_8contents_Content)) PyObject_GC_Track(o);
   __pyx_tp_dealloc_10blacksheep_8contents_Content(o);
 }
 
 static int __pyx_tp_traverse_10blacksheep_8contents_ASGIContent(PyObject *o, visitproc v, void *a) {
   int e;
   struct __pyx_obj_10blacksheep_8contents_ASGIContent *p = (struct __pyx_obj_10blacksheep_8contents_ASGIContent *)o;
   e = ((likely(__pyx_ptype_10blacksheep_8contents_Content)) ? ((__pyx_ptype_10blacksheep_8contents_Content->tp_traverse) ? __pyx_ptype_10blacksheep_8contents_Content->tp_traverse(o, v, a) : 0) : __Pyx_call_next_tp_traverse(o, v, a, __pyx_tp_traverse_10blacksheep_8contents_ASGIContent)); if (e) return e;
@@ -15355,15 +15353,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_10blacksheep_8contents_TextContent(PyTypeObject *t, PyObject *a, PyObject *k) {
   PyObject *o = __pyx_tp_new_10blacksheep_8contents_Content(t, a, k);
   if (unlikely(!o)) return 0;
@@ -15439,15 +15437,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_10blacksheep_8contents_HTMLContent(PyTypeObject *t, PyObject *a, PyObject *k) {
   PyObject *o = __pyx_tp_new_10blacksheep_8contents_Content(t, a, k);
   if (unlikely(!o)) return 0;
@@ -15523,15 +15521,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_10blacksheep_8contents_JSONContent(PyTypeObject *t, PyObject *a, PyObject *k) {
   PyObject *o = __pyx_tp_new_10blacksheep_8contents_Content(t, a, k);
   if (unlikely(!o)) return 0;
@@ -15607,15 +15605,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_10blacksheep_8contents_FormContent(PyTypeObject *t, PyObject *a, PyObject *k) {
   PyObject *o = __pyx_tp_new_10blacksheep_8contents_Content(t, a, k);
   if (unlikely(!o)) return 0;
@@ -15691,15 +15689,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_10blacksheep_8contents_FormPart(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_10blacksheep_8contents_FormPart *p;
   PyObject *o;
@@ -15853,15 +15851,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_10blacksheep_8contents_MultiPartFormData(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_10blacksheep_8contents_MultiPartFormData *p;
   PyObject *o = __pyx_tp_new_10blacksheep_8contents_Content(t, a, k);
@@ -15878,18 +15876,15 @@
   if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->parts);
   Py_CLEAR(p->boundary);
-  #if CYTHON_USE_TYPE_SLOTS
-  if (PyType_IS_GC(Py_TYPE(o)->tp_base))
-  #endif
-  PyObject_GC_Track(o);
+  if (PyType_IS_GC(__pyx_ptype_10blacksheep_8contents_Content)) PyObject_GC_Track(o);
   __pyx_tp_dealloc_10blacksheep_8contents_Content(o);
 }
 
 static int __pyx_tp_traverse_10blacksheep_8contents_MultiPartFormData(PyObject *o, visitproc v, void *a) {
   int e;
   struct __pyx_obj_10blacksheep_8contents_MultiPartFormData *p = (struct __pyx_obj_10blacksheep_8contents_MultiPartFormData *)o;
   e = ((likely(__pyx_ptype_10blacksheep_8contents_Content)) ? ((__pyx_ptype_10blacksheep_8contents_Content->tp_traverse) ? __pyx_ptype_10blacksheep_8contents_Content->tp_traverse(o, v, a) : 0) : __Pyx_call_next_tp_traverse(o, v, a, __pyx_tp_traverse_10blacksheep_8contents_MultiPartFormData)); if (e) return e;
@@ -15992,15 +15987,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10blacksheep_8contents___pyx_scope_struct__read *__pyx_freelist_10blacksheep_8contents___pyx_scope_struct__read[8];
 static int __pyx_freecount_10blacksheep_8contents___pyx_scope_struct__read = 0;
 
@@ -16101,15 +16096,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10blacksheep_8contents___pyx_scope_struct_1_read *__pyx_freelist_10blacksheep_8contents___pyx_scope_struct_1_read[8];
 static int __pyx_freecount_10blacksheep_8contents___pyx_scope_struct_1_read = 0;
 
@@ -16219,15 +16214,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10blacksheep_8contents___pyx_scope_struct_2_get_parts *__pyx_freelist_10blacksheep_8contents___pyx_scope_struct_2_get_parts[8];
 static int __pyx_freecount_10blacksheep_8contents___pyx_scope_struct_2_get_parts = 0;
 
@@ -16336,15 +16331,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10blacksheep_8contents___pyx_scope_struct_3_stream *__pyx_freelist_10blacksheep_8contents___pyx_scope_struct_3_stream[8];
 static int __pyx_freecount_10blacksheep_8contents___pyx_scope_struct_3_stream = 0;
 
@@ -16449,15 +16444,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10blacksheep_8contents___pyx_scope_struct_4_read *__pyx_freelist_10blacksheep_8contents___pyx_scope_struct_4_read[8];
 static int __pyx_freecount_10blacksheep_8contents___pyx_scope_struct_4_read = 0;
 
@@ -16563,15 +16558,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {"parse_www_form", (PyCFunction)__pyx_pw_10blacksheep_8contents_1parse_www_form, METH_O, 0},
   {"write_multipart_part", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10blacksheep_8contents_3write_multipart_part, METH_VARARGS|METH_KEYWORDS, 0},
@@ -17088,35 +17083,21 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule("blacksheep.exceptions"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_10blacksheep_10exceptions_MessageAborted = __Pyx_ImportType(__pyx_t_1, "blacksheep.exceptions", "MessageAborted", sizeof(struct __pyx_obj_10blacksheep_10exceptions_MessageAborted), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_10exceptions_MessageAborted),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_10exceptions_MessageAborted) __PYX_ERR(3, 4, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_HTTPException = __Pyx_ImportType(__pyx_t_1, "blacksheep.exceptions", "HTTPException", sizeof(struct __pyx_obj_10blacksheep_10exceptions_HTTPException), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_10exceptions_HTTPException),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_10exceptions_HTTPException) __PYX_ERR(3, 8, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_BadRequest = __Pyx_ImportType(__pyx_t_1, "blacksheep.exceptions", "BadRequest", sizeof(struct __pyx_obj_10blacksheep_10exceptions_BadRequest), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_10exceptions_BadRequest),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_10exceptions_BadRequest) __PYX_ERR(3, 12, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_BadRequestFormat = __Pyx_ImportType(__pyx_t_1, "blacksheep.exceptions", "BadRequestFormat", sizeof(struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_10exceptions_BadRequestFormat) __PYX_ERR(3, 16, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_NotFound = __Pyx_ImportType(__pyx_t_1, "blacksheep.exceptions", "NotFound", sizeof(struct __pyx_obj_10blacksheep_10exceptions_NotFound), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_10exceptions_NotFound),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_10exceptions_NotFound) __PYX_ERR(3, 20, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_InvalidArgument = __Pyx_ImportType(__pyx_t_1, "blacksheep.exceptions", "InvalidArgument", sizeof(struct __pyx_obj_10blacksheep_10exceptions_InvalidArgument), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_10exceptions_InvalidArgument),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_10exceptions_InvalidArgument) __PYX_ERR(3, 24, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_InvalidOperation = __Pyx_ImportType(__pyx_t_1, "blacksheep.exceptions", "InvalidOperation", sizeof(struct __pyx_obj_10blacksheep_10exceptions_InvalidOperation), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_10exceptions_InvalidOperation),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_10exceptions_InvalidOperation) __PYX_ERR(3, 28, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_MessageAborted = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "MessageAborted", sizeof(struct __pyx_obj_10blacksheep_10exceptions_MessageAborted), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_MessageAborted),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_MessageAborted) __PYX_ERR(3, 4, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_HTTPException = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "HTTPException", sizeof(struct __pyx_obj_10blacksheep_10exceptions_HTTPException), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_HTTPException),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_HTTPException) __PYX_ERR(3, 8, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_BadRequest = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "BadRequest", sizeof(struct __pyx_obj_10blacksheep_10exceptions_BadRequest), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_BadRequest),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_BadRequest) __PYX_ERR(3, 12, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_BadRequestFormat = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "BadRequestFormat", sizeof(struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_BadRequestFormat) __PYX_ERR(3, 16, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_NotFound = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "NotFound", sizeof(struct __pyx_obj_10blacksheep_10exceptions_NotFound), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_NotFound),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_NotFound) __PYX_ERR(3, 20, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_InvalidArgument = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "InvalidArgument", sizeof(struct __pyx_obj_10blacksheep_10exceptions_InvalidArgument), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_InvalidArgument),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_InvalidArgument) __PYX_ERR(3, 24, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_InvalidOperation = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "InvalidOperation", sizeof(struct __pyx_obj_10blacksheep_10exceptions_InvalidOperation), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_InvalidOperation),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_InvalidOperation) __PYX_ERR(3, 28, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -18619,15 +18600,15 @@
 #if PY_VERSION_HEX >= 0x030500B2 || defined(PyCoro_CheckExact)
     if (PyCoro_CheckExact(obj)) {
         return __Pyx_NewRef(obj);
     } else
 #endif
 #if CYTHON_COMPILING_IN_CPYTHON && defined(CO_ITERABLE_COROUTINE)
 #if PY_VERSION_HEX >= 0x030C00A6
-    if (PyGen_CheckExact(obj) && (PyGen_GetCode(obj)->co_flags & CO_ITERABLE_COROUTINE)) {
+    if (PyGen_CheckExact(obj) && (PyGen_GetCode((PyGenObject*)obj)->co_flags & CO_ITERABLE_COROUTINE)) {
 #else
     if (PyGen_CheckExact(obj) && ((PyGenObject*)obj)->gi_code && ((PyCodeObject *)((PyGenObject*)obj)->gi_code)->co_flags & CO_ITERABLE_COROUTINE) {
 #endif
         return __Pyx_NewRef(obj);
     } else
 #endif
     {
@@ -19935,15 +19916,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 #if PY_VERSION_HEX < 0x030500B1 || defined(__Pyx_IterableCoroutine_USED) || CYTHON_USE_ASYNC_SLOTS
 static CYTHON_INLINE PyObject *__Pyx__Coroutine_await(PyObject *coroutine) {
     __pyx_CoroutineAwaitObject *await = PyObject_GC_New(__pyx_CoroutineAwaitObject, __pyx_CoroutineAwaitType);
     if (unlikely(!await)) return NULL;
@@ -20087,15 +20071,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_Coroutine_init(void) {
     __pyx_CoroutineType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx_CoroutineType = __Pyx_FetchCommonType(&__pyx_CoroutineType_type);
     if (unlikely(!__pyx_CoroutineType))
@@ -21131,18 +21118,18 @@
     return 0;
 bad:
     Py_XDECREF(ob);
     return -1;
 }
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -21188,22 +21175,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -21583,15 +21570,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -21779,15 +21766,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -22339,15 +22326,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int
 __Pyx_PyAsyncGen_ClearFreeLists(void)
 {
     int ret = __Pyx_ag_value_freelist_free + __Pyx_ag_asend_freelist_free;
@@ -22537,15 +22527,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static PyObject *
 __Pyx_async_gen_asend_new(__pyx_PyAsyncGenObject *gen, PyObject *sendval)
 {
     __pyx_PyAsyncGenASend *o;
@@ -22639,15 +22632,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static PyObject *
 __Pyx__PyAsyncGenValueWrapperNew(PyObject *val)
 {
     __pyx__PyAsyncGenWrappedValue *o;
@@ -22880,15 +22876,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static PyObject *
 __Pyx_async_gen_athrow_new(__pyx_PyAsyncGenObject *gen, PyObject *args)
 {
     __pyx_PyAsyncGenAThrow *o;
```

### Comparing `blacksheep-2.0a6/blacksheep/contents.pxd` & `blacksheep-2.0a7/blacksheep/contents.pxd`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/contents.pyi` & `blacksheep-2.0a7/blacksheep/contents.pyi`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/contents.pyx` & `blacksheep-2.0a7/blacksheep/contents.pyx`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/cookies.c` & `blacksheep-2.0a7/blacksheep/cookies.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.35 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -74,16 +74,20 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -1572,30 +1576,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* CalculateMetaclass.proto */
 static PyObject *__Pyx_CalculateMetaclass(PyTypeObject *metaclass, PyObject *bases);
 
 /* SetNameInClass.proto */
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1
@@ -11685,15 +11689,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_10blacksheep_7cookies_CookieError(PyTypeObject *t, PyObject *a, PyObject *k) {
   PyObject *o = (&((PyTypeObject*)PyExc_Exception)[0])->tp_new(t, a, k);
   if (unlikely(!o)) return 0;
@@ -11791,15 +11795,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_10blacksheep_7cookies_CookieValueExceedsMaximumLength(PyTypeObject *t, PyObject *a, PyObject *k) {
   PyObject *o = __pyx_tp_new_10blacksheep_7cookies_CookieError(t, a, k);
   if (unlikely(!o)) return 0;
@@ -11875,15 +11879,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new___Pyx_EnumMeta(PyTypeObject *t, PyObject *a, PyObject *k) {
   PyObject *o = (&PyType_Type)->tp_new(t, a, k);
   if (unlikely(!o)) return 0;
@@ -12007,15 +12011,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {"datetime_to_cookie_format", (PyCFunction)__pyx_pw_10blacksheep_7cookies_1datetime_to_cookie_format, METH_O, 0},
   {"datetime_from_cookie_format", (PyCFunction)__pyx_pw_10blacksheep_7cookies_3datetime_from_cookie_format, METH_O, 0},
@@ -12437,40 +12441,29 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("datetime"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_8datetime_date = __Pyx_ImportType(__pyx_t_1, "datetime", "date", sizeof(PyDateTime_Date), __PYX_GET_STRUCT_ALIGNMENT(PyDateTime_Date),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_8datetime_date) __PYX_ERR(3, 9, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_time = __Pyx_ImportType(__pyx_t_1, "datetime", "time", sizeof(PyDateTime_Time), __PYX_GET_STRUCT_ALIGNMENT(PyDateTime_Time),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_8datetime_time) __PYX_ERR(3, 12, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_datetime = __Pyx_ImportType(__pyx_t_1, "datetime", "datetime", sizeof(PyDateTime_DateTime), __PYX_GET_STRUCT_ALIGNMENT(PyDateTime_DateTime),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_8datetime_datetime) __PYX_ERR(3, 15, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_timedelta = __Pyx_ImportType(__pyx_t_1, "datetime", "timedelta", sizeof(PyDateTime_Delta), __PYX_GET_STRUCT_ALIGNMENT(PyDateTime_Delta),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_8datetime_timedelta) __PYX_ERR(3, 18, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_tzinfo = __Pyx_ImportType(__pyx_t_1, "datetime", "tzinfo", sizeof(PyDateTime_TZInfo), __PYX_GET_STRUCT_ALIGNMENT(PyDateTime_TZInfo),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_8datetime_tzinfo) __PYX_ERR(3, 21, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_date = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "date", sizeof(PyDateTime_Date), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_Date),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_date) __PYX_ERR(3, 9, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_time = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "time", sizeof(PyDateTime_Time), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_Time),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_time) __PYX_ERR(3, 12, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_datetime = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "datetime", sizeof(PyDateTime_DateTime), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_DateTime),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_datetime) __PYX_ERR(3, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_timedelta = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "timedelta", sizeof(PyDateTime_Delta), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_Delta),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_timedelta) __PYX_ERR(3, 18, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_tzinfo = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "tzinfo", sizeof(PyDateTime_TZInfo), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_TZInfo),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_tzinfo) __PYX_ERR(3, 21, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -15179,18 +15172,18 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -15236,22 +15229,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -15914,15 +15907,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
@@ -16425,15 +16421,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -16659,15 +16655,15 @@
                         } else if (8 * sizeof(enum __pyx_t_10blacksheep_7cookies_CookieSameSiteMode) >= 4 * PyLong_SHIFT) {
                             return (enum __pyx_t_10blacksheep_7cookies_CookieSameSiteMode) (((((((((enum __pyx_t_10blacksheep_7cookies_CookieSameSiteMode)digits[3]) << PyLong_SHIFT) | (enum __pyx_t_10blacksheep_7cookies_CookieSameSiteMode)digits[2]) << PyLong_SHIFT) | (enum __pyx_t_10blacksheep_7cookies_CookieSameSiteMode)digits[1]) << PyLong_SHIFT) | (enum __pyx_t_10blacksheep_7cookies_CookieSameSiteMode)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -16855,15 +16851,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `blacksheep-2.0a6/blacksheep/cookies.pxd` & `blacksheep-2.0a7/blacksheep/cookies.pxd`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/cookies.pyi` & `blacksheep-2.0a7/blacksheep/cookies.pyi`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/cookies.pyx` & `blacksheep-2.0a7/blacksheep/cookies.pyx`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/exceptions.c` & `blacksheep-2.0a7/blacksheep/exceptions.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.35 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -74,16 +74,20 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -12012,15 +12016,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_10blacksheep_10exceptions_HTTPException(PyTypeObject *t, PyObject *a, PyObject *k) {
   PyObject *o = (&((PyTypeObject*)PyExc_Exception)[0])->tp_new(t, a, k);
   if (unlikely(!o)) return 0;
@@ -12137,15 +12141,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_10blacksheep_10exceptions_BadRequest(PyTypeObject *t, PyObject *a, PyObject *k) {
   PyObject *o = __pyx_tp_new_10blacksheep_10exceptions_HTTPException(t, a, k);
   if (unlikely(!o)) return 0;
@@ -12221,15 +12225,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_10blacksheep_10exceptions_BadRequestFormat(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat *p;
   PyObject *o = __pyx_tp_new_10blacksheep_10exceptions_BadRequest(t, a, k);
@@ -12359,15 +12363,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_10blacksheep_10exceptions_NotFound(PyTypeObject *t, PyObject *a, PyObject *k) {
   PyObject *o = __pyx_tp_new_10blacksheep_10exceptions_HTTPException(t, a, k);
   if (unlikely(!o)) return 0;
@@ -12443,15 +12447,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_10blacksheep_10exceptions_InvalidArgument(PyTypeObject *t, PyObject *a, PyObject *k) {
   PyObject *o = (&((PyTypeObject*)PyExc_Exception)[0])->tp_new(t, a, k);
   if (unlikely(!o)) return 0;
@@ -12549,15 +12553,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_10blacksheep_10exceptions_InvalidOperation(PyTypeObject *t, PyObject *a, PyObject *k) {
   PyObject *o = (&((PyTypeObject*)PyExc_Exception)[0])->tp_new(t, a, k);
   if (unlikely(!o)) return 0;
@@ -12655,15 +12659,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_10blacksheep_10exceptions_Unauthorized(PyTypeObject *t, PyObject *a, PyObject *k) {
   PyObject *o = __pyx_tp_new_10blacksheep_10exceptions_HTTPException(t, a, k);
   if (unlikely(!o)) return 0;
@@ -12739,15 +12743,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_10blacksheep_10exceptions_Forbidden(PyTypeObject *t, PyObject *a, PyObject *k) {
   PyObject *o = __pyx_tp_new_10blacksheep_10exceptions_HTTPException(t, a, k);
   if (unlikely(!o)) return 0;
@@ -12823,15 +12827,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_10blacksheep_10exceptions_RangeNotSatisfiable(PyTypeObject *t, PyObject *a, PyObject *k) {
   PyObject *o = __pyx_tp_new_10blacksheep_10exceptions_HTTPException(t, a, k);
   if (unlikely(!o)) return 0;
@@ -12907,15 +12911,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_10blacksheep_10exceptions_InternalServerError(PyTypeObject *t, PyObject *a, PyObject *k) {
   PyObject *o = __pyx_tp_new_10blacksheep_10exceptions_HTTPException(t, a, k);
   if (unlikely(!o)) return 0;
@@ -12991,15 +12995,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_10blacksheep_10exceptions_NotImplementedByServer(PyTypeObject *t, PyObject *a, PyObject *k) {
   PyObject *o = __pyx_tp_new_10blacksheep_10exceptions_HTTPException(t, a, k);
   if (unlikely(!o)) return 0;
@@ -13075,15 +13079,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -15425,15 +15429,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -15621,15 +15625,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `blacksheep-2.0a6/blacksheep/exceptions.pyi` & `blacksheep-2.0a7/blacksheep/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/exceptions.pyx` & `blacksheep-2.0a7/blacksheep/exceptions.pyx`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/headers.c` & `blacksheep-2.0a7/blacksheep/headers.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.35 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -74,16 +74,20 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -9123,15 +9127,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_10blacksheep_7headers_Headers __pyx_vtable_10blacksheep_7headers_Headers;
 
 static PyObject *__pyx_tp_new_10blacksheep_7headers_Headers(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_10blacksheep_7headers_Headers *p;
@@ -9369,15 +9373,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10blacksheep_7headers___pyx_scope_struct____iter__ *__pyx_freelist_10blacksheep_7headers___pyx_scope_struct____iter__[8];
 static int __pyx_freecount_10blacksheep_7headers___pyx_scope_struct____iter__ = 0;
 
@@ -9478,15 +9482,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10blacksheep_7headers___pyx_scope_struct_1_items *__pyx_freelist_10blacksheep_7headers___pyx_scope_struct_1_items[8];
 static int __pyx_freecount_10blacksheep_7headers___pyx_scope_struct_1_items = 0;
 
@@ -9587,15 +9591,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10blacksheep_7headers___pyx_scope_struct_2___iter__ *__pyx_freelist_10blacksheep_7headers___pyx_scope_struct_2___iter__[8];
 static int __pyx_freecount_10blacksheep_7headers___pyx_scope_struct_2___iter__ = 0;
 
@@ -9696,15 +9700,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -12990,15 +12994,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_Generator_init(void) {
     __pyx_GeneratorType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx_GeneratorType_type.tp_iter = PyObject_SelfIter;
     __pyx_GeneratorType = __Pyx_FetchCommonType(&__pyx_GeneratorType_type);
@@ -13646,15 +13653,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -13880,15 +13887,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `blacksheep-2.0a6/blacksheep/headers.pxd` & `blacksheep-2.0a7/blacksheep/headers.pxd`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/headers.pyi` & `blacksheep-2.0a7/blacksheep/headers.pyi`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/headers.pyx` & `blacksheep-2.0a7/blacksheep/headers.pyx`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/messages.c` & `blacksheep-2.0a7/blacksheep/messages.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.35 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -74,16 +74,20 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -2264,30 +2268,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* ClassMethod.proto */
 #include "descrobject.h"
@@ -2375,15 +2379,15 @@
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* FunctionExport.proto */
 static int __Pyx_ExportFunction(const char *name, void (*f)(void), const char *sig);
 
 /* FunctionImport.proto */
-static int __Pyx_ImportFunction(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
+static int __Pyx_ImportFunction_0_29_35(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 static struct __pyx_obj_10blacksheep_8messages_Message *__pyx_f_10blacksheep_8messages_7Message_with_content(struct __pyx_obj_10blacksheep_8messages_Message *__pyx_v_self, struct __pyx_obj_10blacksheep_8contents_Content *__pyx_v_content, int __pyx_skip_dispatch); /* proto*/
 static PyObject *__pyx_f_10blacksheep_8messages_7Message_get_first_header(struct __pyx_obj_10blacksheep_8messages_Message *__pyx_v_self, PyObject *__pyx_v_key, int __pyx_skip_dispatch); /* proto*/
 static PyObject *__pyx_f_10blacksheep_8messages_7Message_get_headers(struct __pyx_obj_10blacksheep_8messages_Message *__pyx_v_self, PyObject *__pyx_v_key, int __pyx_skip_dispatch); /* proto*/
@@ -20334,15 +20338,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_10blacksheep_8messages_Request __pyx_vtable_10blacksheep_8messages_Request;
 
 static PyObject *__pyx_tp_new_10blacksheep_8messages_Request(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_10blacksheep_8messages_Request *p;
@@ -20751,15 +20755,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_10blacksheep_8messages_Response __pyx_vtable_10blacksheep_8messages_Response;
 
 static PyObject *__pyx_tp_new_10blacksheep_8messages_Response(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_10blacksheep_8messages_Response *p;
@@ -20937,15 +20941,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10blacksheep_8messages___pyx_scope_struct__read *__pyx_freelist_10blacksheep_8messages___pyx_scope_struct__read[8];
 static int __pyx_freecount_10blacksheep_8messages___pyx_scope_struct__read = 0;
 
@@ -21046,15 +21050,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10blacksheep_8messages___pyx_scope_struct_1_stream *__pyx_freelist_10blacksheep_8messages___pyx_scope_struct_1_stream[8];
 static int __pyx_freecount_10blacksheep_8messages___pyx_scope_struct_1_stream = 0;
 
@@ -21163,15 +21167,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10blacksheep_8messages___pyx_scope_struct_2_text *__pyx_freelist_10blacksheep_8messages___pyx_scope_struct_2_text[8];
 static int __pyx_freecount_10blacksheep_8messages___pyx_scope_struct_2_text = 0;
 
@@ -21276,15 +21280,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10blacksheep_8messages___pyx_scope_struct_3_form *__pyx_freelist_10blacksheep_8messages___pyx_scope_struct_3_form[8];
 static int __pyx_freecount_10blacksheep_8messages___pyx_scope_struct_3_form = 0;
 
@@ -21388,15 +21392,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10blacksheep_8messages___pyx_scope_struct_4_multipart *__pyx_freelist_10blacksheep_8messages___pyx_scope_struct_4_multipart[8];
 static int __pyx_freecount_10blacksheep_8messages___pyx_scope_struct_4_multipart = 0;
 
@@ -21500,15 +21504,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10blacksheep_8messages___pyx_scope_struct_5_files *__pyx_freelist_10blacksheep_8messages___pyx_scope_struct_5_files[8];
 static int __pyx_freecount_10blacksheep_8messages___pyx_scope_struct_5_files = 0;
 
@@ -21626,15 +21630,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10blacksheep_8messages___pyx_scope_struct_6_json *__pyx_freelist_10blacksheep_8messages___pyx_scope_struct_6_json[8];
 static int __pyx_freecount_10blacksheep_8messages___pyx_scope_struct_6_json = 0;
 
@@ -21748,15 +21752,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {"parse_charset", (PyCFunction)__pyx_pw_10blacksheep_8messages_1parse_charset, METH_O, 0},
   {"method_without_body", (PyCFunction)__pyx_pw_10blacksheep_8messages_3method_without_body, METH_O, 0},
@@ -22339,118 +22343,67 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule("blacksheep.contents"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_10blacksheep_8contents_Content = __Pyx_ImportType(__pyx_t_1, "blacksheep.contents", "Content", sizeof(struct __pyx_obj_10blacksheep_8contents_Content), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_8contents_Content),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_8contents_Content) __PYX_ERR(4, 8, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_StreamedContent = __Pyx_ImportType(__pyx_t_1, "blacksheep.contents", "StreamedContent", sizeof(struct __pyx_obj_10blacksheep_8contents_StreamedContent), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_8contents_StreamedContent),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_8contents_StreamedContent) __PYX_ERR(4, 14, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_ASGIContent = __Pyx_ImportType(__pyx_t_1, "blacksheep.contents", "ASGIContent", sizeof(struct __pyx_obj_10blacksheep_8contents_ASGIContent), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_8contents_ASGIContent),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_8contents_ASGIContent) __PYX_ERR(4, 18, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_Content = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "Content", sizeof(struct __pyx_obj_10blacksheep_8contents_Content), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_Content),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_Content) __PYX_ERR(4, 8, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_StreamedContent = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "StreamedContent", sizeof(struct __pyx_obj_10blacksheep_8contents_StreamedContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_StreamedContent),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_StreamedContent) __PYX_ERR(4, 14, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_ASGIContent = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "ASGIContent", sizeof(struct __pyx_obj_10blacksheep_8contents_ASGIContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_ASGIContent),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_ASGIContent) __PYX_ERR(4, 18, __pyx_L1_error)
   __pyx_vtabptr_10blacksheep_8contents_ASGIContent = (struct __pyx_vtabstruct_10blacksheep_8contents_ASGIContent*)__Pyx_GetVtable(__pyx_ptype_10blacksheep_8contents_ASGIContent->tp_dict); if (unlikely(!__pyx_vtabptr_10blacksheep_8contents_ASGIContent)) __PYX_ERR(4, 18, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_TextContent = __Pyx_ImportType(__pyx_t_1, "blacksheep.contents", "TextContent", sizeof(struct __pyx_obj_10blacksheep_8contents_TextContent), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_8contents_TextContent),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_8contents_TextContent) __PYX_ERR(4, 23, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_HTMLContent = __Pyx_ImportType(__pyx_t_1, "blacksheep.contents", "HTMLContent", sizeof(struct __pyx_obj_10blacksheep_8contents_HTMLContent), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_8contents_HTMLContent),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_8contents_HTMLContent) __PYX_ERR(4, 27, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_JSONContent = __Pyx_ImportType(__pyx_t_1, "blacksheep.contents", "JSONContent", sizeof(struct __pyx_obj_10blacksheep_8contents_JSONContent), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_8contents_JSONContent),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_8contents_JSONContent) __PYX_ERR(4, 31, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_FormContent = __Pyx_ImportType(__pyx_t_1, "blacksheep.contents", "FormContent", sizeof(struct __pyx_obj_10blacksheep_8contents_FormContent), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_8contents_FormContent),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_8contents_FormContent) __PYX_ERR(4, 35, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_FormPart = __Pyx_ImportType(__pyx_t_1, "blacksheep.contents", "FormPart", sizeof(struct __pyx_obj_10blacksheep_8contents_FormPart), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_8contents_FormPart),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_8contents_FormPart) __PYX_ERR(4, 39, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_MultiPartFormData = __Pyx_ImportType(__pyx_t_1, "blacksheep.contents", "MultiPartFormData", sizeof(struct __pyx_obj_10blacksheep_8contents_MultiPartFormData), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_8contents_MultiPartFormData),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_8contents_MultiPartFormData) __PYX_ERR(4, 47, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_TextContent = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "TextContent", sizeof(struct __pyx_obj_10blacksheep_8contents_TextContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_TextContent),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_TextContent) __PYX_ERR(4, 23, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_HTMLContent = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "HTMLContent", sizeof(struct __pyx_obj_10blacksheep_8contents_HTMLContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_HTMLContent),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_HTMLContent) __PYX_ERR(4, 27, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_JSONContent = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "JSONContent", sizeof(struct __pyx_obj_10blacksheep_8contents_JSONContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_JSONContent),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_JSONContent) __PYX_ERR(4, 31, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_FormContent = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "FormContent", sizeof(struct __pyx_obj_10blacksheep_8contents_FormContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_FormContent),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_FormContent) __PYX_ERR(4, 35, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_FormPart = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "FormPart", sizeof(struct __pyx_obj_10blacksheep_8contents_FormPart), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_FormPart),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_FormPart) __PYX_ERR(4, 39, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_MultiPartFormData = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "MultiPartFormData", sizeof(struct __pyx_obj_10blacksheep_8contents_MultiPartFormData), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_MultiPartFormData),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_MultiPartFormData) __PYX_ERR(4, 47, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(5, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(5, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("datetime"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_8datetime_date = __Pyx_ImportType(__pyx_t_1, "datetime", "date", sizeof(PyDateTime_Date), __PYX_GET_STRUCT_ALIGNMENT(PyDateTime_Date),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_8datetime_date) __PYX_ERR(3, 9, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_time = __Pyx_ImportType(__pyx_t_1, "datetime", "time", sizeof(PyDateTime_Time), __PYX_GET_STRUCT_ALIGNMENT(PyDateTime_Time),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_8datetime_time) __PYX_ERR(3, 12, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_datetime = __Pyx_ImportType(__pyx_t_1, "datetime", "datetime", sizeof(PyDateTime_DateTime), __PYX_GET_STRUCT_ALIGNMENT(PyDateTime_DateTime),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_8datetime_datetime) __PYX_ERR(3, 15, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_timedelta = __Pyx_ImportType(__pyx_t_1, "datetime", "timedelta", sizeof(PyDateTime_Delta), __PYX_GET_STRUCT_ALIGNMENT(PyDateTime_Delta),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_8datetime_timedelta) __PYX_ERR(3, 18, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_tzinfo = __Pyx_ImportType(__pyx_t_1, "datetime", "tzinfo", sizeof(PyDateTime_TZInfo), __PYX_GET_STRUCT_ALIGNMENT(PyDateTime_TZInfo),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_8datetime_tzinfo) __PYX_ERR(3, 21, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_date = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "date", sizeof(PyDateTime_Date), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_Date),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_date) __PYX_ERR(3, 9, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_time = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "time", sizeof(PyDateTime_Time), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_Time),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_time) __PYX_ERR(3, 12, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_datetime = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "datetime", sizeof(PyDateTime_DateTime), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_DateTime),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_datetime) __PYX_ERR(3, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_timedelta = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "timedelta", sizeof(PyDateTime_Delta), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_Delta),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_timedelta) __PYX_ERR(3, 18, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_tzinfo = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "tzinfo", sizeof(PyDateTime_TZInfo), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_TZInfo),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_tzinfo) __PYX_ERR(3, 21, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("blacksheep.cookies"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_10blacksheep_7cookies_Cookie = __Pyx_ImportType(__pyx_t_1, "blacksheep.cookies", "Cookie", sizeof(struct __pyx_obj_10blacksheep_7cookies_Cookie), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_7cookies_Cookie),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_7cookies_Cookie) __PYX_ERR(6, 17, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_7cookies_Cookie = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.cookies", "Cookie", sizeof(struct __pyx_obj_10blacksheep_7cookies_Cookie), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_7cookies_Cookie),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_7cookies_Cookie) __PYX_ERR(6, 17, __pyx_L1_error)
   __pyx_vtabptr_10blacksheep_7cookies_Cookie = (struct __pyx_vtabstruct_10blacksheep_7cookies_Cookie*)__Pyx_GetVtable(__pyx_ptype_10blacksheep_7cookies_Cookie->tp_dict); if (unlikely(!__pyx_vtabptr_10blacksheep_7cookies_Cookie)) __PYX_ERR(6, 17, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("blacksheep.exceptions"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_10blacksheep_10exceptions_MessageAborted = __Pyx_ImportType(__pyx_t_1, "blacksheep.exceptions", "MessageAborted", sizeof(struct __pyx_obj_10blacksheep_10exceptions_MessageAborted), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_10exceptions_MessageAborted),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_10exceptions_MessageAborted) __PYX_ERR(7, 4, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_HTTPException = __Pyx_ImportType(__pyx_t_1, "blacksheep.exceptions", "HTTPException", sizeof(struct __pyx_obj_10blacksheep_10exceptions_HTTPException), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_10exceptions_HTTPException),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_10exceptions_HTTPException) __PYX_ERR(7, 8, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_BadRequest = __Pyx_ImportType(__pyx_t_1, "blacksheep.exceptions", "BadRequest", sizeof(struct __pyx_obj_10blacksheep_10exceptions_BadRequest), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_10exceptions_BadRequest),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_10exceptions_BadRequest) __PYX_ERR(7, 12, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_BadRequestFormat = __Pyx_ImportType(__pyx_t_1, "blacksheep.exceptions", "BadRequestFormat", sizeof(struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_10exceptions_BadRequestFormat) __PYX_ERR(7, 16, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_NotFound = __Pyx_ImportType(__pyx_t_1, "blacksheep.exceptions", "NotFound", sizeof(struct __pyx_obj_10blacksheep_10exceptions_NotFound), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_10exceptions_NotFound),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_10exceptions_NotFound) __PYX_ERR(7, 20, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_InvalidArgument = __Pyx_ImportType(__pyx_t_1, "blacksheep.exceptions", "InvalidArgument", sizeof(struct __pyx_obj_10blacksheep_10exceptions_InvalidArgument), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_10exceptions_InvalidArgument),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_10exceptions_InvalidArgument) __PYX_ERR(7, 24, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_InvalidOperation = __Pyx_ImportType(__pyx_t_1, "blacksheep.exceptions", "InvalidOperation", sizeof(struct __pyx_obj_10blacksheep_10exceptions_InvalidOperation), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_10exceptions_InvalidOperation),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_10exceptions_InvalidOperation) __PYX_ERR(7, 28, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_MessageAborted = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "MessageAborted", sizeof(struct __pyx_obj_10blacksheep_10exceptions_MessageAborted), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_MessageAborted),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_MessageAborted) __PYX_ERR(7, 4, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_HTTPException = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "HTTPException", sizeof(struct __pyx_obj_10blacksheep_10exceptions_HTTPException), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_HTTPException),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_HTTPException) __PYX_ERR(7, 8, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_BadRequest = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "BadRequest", sizeof(struct __pyx_obj_10blacksheep_10exceptions_BadRequest), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_BadRequest),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_BadRequest) __PYX_ERR(7, 12, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_BadRequestFormat = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "BadRequestFormat", sizeof(struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_BadRequestFormat) __PYX_ERR(7, 16, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_NotFound = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "NotFound", sizeof(struct __pyx_obj_10blacksheep_10exceptions_NotFound), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_NotFound),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_NotFound) __PYX_ERR(7, 20, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_InvalidArgument = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "InvalidArgument", sizeof(struct __pyx_obj_10blacksheep_10exceptions_InvalidArgument), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_InvalidArgument),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_InvalidArgument) __PYX_ERR(7, 24, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_InvalidOperation = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "InvalidOperation", sizeof(struct __pyx_obj_10blacksheep_10exceptions_InvalidOperation), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_InvalidOperation),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_InvalidOperation) __PYX_ERR(7, 28, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("blacksheep.url"); if (unlikely(!__pyx_t_1)) __PYX_ERR(8, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_10blacksheep_3url_URL = __Pyx_ImportType(__pyx_t_1, "blacksheep.url", "URL", sizeof(struct __pyx_obj_10blacksheep_3url_URL), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_3url_URL),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_3url_URL) __PYX_ERR(8, 8, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_3url_URL = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.url", "URL", sizeof(struct __pyx_obj_10blacksheep_3url_URL), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_3url_URL),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_3url_URL) __PYX_ERR(8, 8, __pyx_L1_error)
   __pyx_vtabptr_10blacksheep_3url_URL = (struct __pyx_vtabstruct_10blacksheep_3url_URL*)__Pyx_GetVtable(__pyx_ptype_10blacksheep_3url_URL->tp_dict); if (unlikely(!__pyx_vtabptr_10blacksheep_3url_URL)) __PYX_ERR(8, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("blacksheep.headers"); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_10blacksheep_7headers_Header = __Pyx_ImportType(__pyx_t_1, "blacksheep.headers", "Header", sizeof(struct __pyx_obj_10blacksheep_7headers_Header), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_7headers_Header),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_7headers_Header) __PYX_ERR(9, 8, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_7headers_Headers = __Pyx_ImportType(__pyx_t_1, "blacksheep.headers", "Headers", sizeof(struct __pyx_obj_10blacksheep_7headers_Headers), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_7headers_Headers),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_7headers_Headers) __PYX_ERR(9, 13, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_7headers_Header = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.headers", "Header", sizeof(struct __pyx_obj_10blacksheep_7headers_Header), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_7headers_Header),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_7headers_Header) __PYX_ERR(9, 8, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_7headers_Headers = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.headers", "Headers", sizeof(struct __pyx_obj_10blacksheep_7headers_Headers), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_7headers_Headers),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_7headers_Headers) __PYX_ERR(9, 13, __pyx_L1_error)
   __pyx_vtabptr_10blacksheep_7headers_Headers = (struct __pyx_vtabstruct_10blacksheep_7headers_Headers*)__Pyx_GetVtable(__pyx_ptype_10blacksheep_7headers_Headers->tp_dict); if (unlikely(!__pyx_vtabptr_10blacksheep_7headers_Headers)) __PYX_ERR(9, 13, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -22471,27 +22424,27 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __pyx_t_1 = PyImport_ImportModule("blacksheep.contents"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportFunction(__pyx_t_1, "parse_www_form_urlencoded", (void (**)(void))&__pyx_f_10blacksheep_8contents_parse_www_form_urlencoded, "PyObject *(PyObject *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "multiparts_to_dictionary", (void (**)(void))&__pyx_f_10blacksheep_8contents_multiparts_to_dictionary, "PyObject *(PyObject *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "parse_www_form_urlencoded", (void (**)(void))&__pyx_f_10blacksheep_8contents_parse_www_form_urlencoded, "PyObject *(PyObject *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "multiparts_to_dictionary", (void (**)(void))&__pyx_f_10blacksheep_8contents_multiparts_to_dictionary, "PyObject *(PyObject *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("blacksheep.cookies"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportFunction(__pyx_t_1, "parse_cookie", (void (**)(void))&__pyx_f_10blacksheep_7cookies_parse_cookie, "struct __pyx_obj_10blacksheep_7cookies_Cookie *(PyObject *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "datetime_to_cookie_format", (void (**)(void))&__pyx_f_10blacksheep_7cookies_datetime_to_cookie_format, "PyObject *(PyDateTime_DateTime *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "write_cookie_for_response", (void (**)(void))&__pyx_f_10blacksheep_7cookies_write_cookie_for_response, "PyObject *(struct __pyx_obj_10blacksheep_7cookies_Cookie *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "split_value", (void (**)(void))&__pyx_f_10blacksheep_7cookies_split_value, "PyObject *(PyObject *, PyObject *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "parse_cookie", (void (**)(void))&__pyx_f_10blacksheep_7cookies_parse_cookie, "struct __pyx_obj_10blacksheep_7cookies_Cookie *(PyObject *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "datetime_to_cookie_format", (void (**)(void))&__pyx_f_10blacksheep_7cookies_datetime_to_cookie_format, "PyObject *(PyDateTime_DateTime *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "write_cookie_for_response", (void (**)(void))&__pyx_f_10blacksheep_7cookies_write_cookie_for_response, "PyObject *(struct __pyx_obj_10blacksheep_7cookies_Cookie *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "split_value", (void (**)(void))&__pyx_f_10blacksheep_7cookies_split_value, "PyObject *(PyObject *, PyObject *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("blacksheep.url"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportFunction(__pyx_t_1, "build_absolute_url", (void (**)(void))&__pyx_f_10blacksheep_3url_build_absolute_url, "struct __pyx_obj_10blacksheep_3url_URL *(PyObject *, PyObject *, PyObject *, PyObject *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "build_absolute_url", (void (**)(void))&__pyx_f_10blacksheep_3url_build_absolute_url, "struct __pyx_obj_10blacksheep_3url_URL *(PyObject *, PyObject *, PyObject *, PyObject *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -25344,15 +25297,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 #if PY_VERSION_HEX < 0x030500B1 || defined(__Pyx_IterableCoroutine_USED) || CYTHON_USE_ASYNC_SLOTS
 static CYTHON_INLINE PyObject *__Pyx__Coroutine_await(PyObject *coroutine) {
     __pyx_CoroutineAwaitObject *await = PyObject_GC_New(__pyx_CoroutineAwaitObject, __pyx_CoroutineAwaitType);
     if (unlikely(!await)) return NULL;
@@ -25496,15 +25452,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_Coroutine_init(void) {
     __pyx_CoroutineType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx_CoroutineType = __Pyx_FetchCommonType(&__pyx_CoroutineType_type);
     if (unlikely(!__pyx_CoroutineType))
@@ -25572,15 +25531,15 @@
 #if PY_VERSION_HEX >= 0x030500B2 || defined(PyCoro_CheckExact)
     if (PyCoro_CheckExact(obj)) {
         return __Pyx_NewRef(obj);
     } else
 #endif
 #if CYTHON_COMPILING_IN_CPYTHON && defined(CO_ITERABLE_COROUTINE)
 #if PY_VERSION_HEX >= 0x030C00A6
-    if (PyGen_CheckExact(obj) && (PyGen_GetCode(obj)->co_flags & CO_ITERABLE_COROUTINE)) {
+    if (PyGen_CheckExact(obj) && (PyGen_GetCode((PyGenObject*)obj)->co_flags & CO_ITERABLE_COROUTINE)) {
 #else
     if (PyGen_CheckExact(obj) && ((PyGenObject*)obj)->gi_code && ((PyCodeObject *)((PyGenObject*)obj)->gi_code)->co_flags & CO_ITERABLE_COROUTINE) {
 #endif
         return __Pyx_NewRef(obj);
     } else
 #endif
     {
@@ -26887,18 +26846,18 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -26944,22 +26903,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -27395,15 +27354,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -27591,15 +27550,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -28051,15 +28010,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int
 __Pyx_PyAsyncGen_ClearFreeLists(void)
 {
     int ret = __Pyx_ag_value_freelist_free + __Pyx_ag_asend_freelist_free;
@@ -28249,15 +28211,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static PyObject *
 __Pyx_async_gen_asend_new(__pyx_PyAsyncGenObject *gen, PyObject *sendval)
 {
     __pyx_PyAsyncGenASend *o;
@@ -28351,15 +28316,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static PyObject *
 __Pyx__PyAsyncGenValueWrapperNew(PyObject *val)
 {
     __pyx__PyAsyncGenWrappedValue *o;
@@ -28592,15 +28560,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static PyObject *
 __Pyx_async_gen_athrow_new(__pyx_PyAsyncGenObject *gen, PyObject *args)
 {
     __pyx_PyAsyncGenAThrow *o;
@@ -28711,17 +28682,17 @@
 bad:
     Py_XDECREF(cobj);
     Py_XDECREF(d);
     return -1;
 }
 
 /* FunctionImport */
-  #ifndef __PYX_HAVE_RT_ImportFunction
-#define __PYX_HAVE_RT_ImportFunction
-static int __Pyx_ImportFunction(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
+  #ifndef __PYX_HAVE_RT_ImportFunction_0_29_35
+#define __PYX_HAVE_RT_ImportFunction_0_29_35
+static int __Pyx_ImportFunction_0_29_35(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
     PyObject *d = 0;
     PyObject *cobj = 0;
     union {
         void (*fp)(void);
         void *p;
     } tmp;
     d = PyObject_GetAttrString(module, (char *)"__pyx_capi__");
```

### Comparing `blacksheep-2.0a6/blacksheep/messages.pxd` & `blacksheep-2.0a7/blacksheep/messages.pxd`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/messages.pyi` & `blacksheep-2.0a7/blacksheep/messages.pyi`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/messages.pyx` & `blacksheep-2.0a7/blacksheep/messages.pyx`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/middlewares.py` & `blacksheep-2.0a7/blacksheep/middlewares.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/multipart.py` & `blacksheep-2.0a7/blacksheep/multipart.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/ranges.py` & `blacksheep-2.0a7/blacksheep/ranges.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/scribe.c` & `blacksheep-2.0a7/blacksheep/scribe.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.35 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -74,16 +74,20 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -2005,30 +2009,30 @@
     PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,\
     const char* function_name);
 
 /* IncludeStringH.proto */
 #include <string.h>
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
@@ -2143,15 +2147,15 @@
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* FunctionExport.proto */
 static int __Pyx_ExportFunction(const char *name, void (*f)(void), const char *sig);
 
 /* FunctionImport.proto */
-static int __Pyx_ImportFunction(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
+static int __Pyx_ImportFunction_0_29_35(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 
 /* Module declarations from 'blacksheep.contents' */
 static PyTypeObject *__pyx_ptype_10blacksheep_8contents_Content = 0;
@@ -9188,15 +9192,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10blacksheep_6scribe___pyx_scope_struct_1_write_request_body_only *__pyx_freelist_10blacksheep_6scribe___pyx_scope_struct_1_write_request_body_only[8];
 static int __pyx_freecount_10blacksheep_6scribe___pyx_scope_struct_1_write_request_body_only = 0;
 
@@ -9307,15 +9311,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10blacksheep_6scribe___pyx_scope_struct_2_write_request *__pyx_freelist_10blacksheep_6scribe___pyx_scope_struct_2_write_request[8];
 static int __pyx_freecount_10blacksheep_6scribe___pyx_scope_struct_2_write_request = 0;
 
@@ -9426,15 +9430,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10blacksheep_6scribe___pyx_scope_struct_3_get_chunks *__pyx_freelist_10blacksheep_6scribe___pyx_scope_struct_3_get_chunks[8];
 static int __pyx_freecount_10blacksheep_6scribe___pyx_scope_struct_3_get_chunks = 0;
 
@@ -9524,15 +9528,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10blacksheep_6scribe___pyx_scope_struct_4_write_response *__pyx_freelist_10blacksheep_6scribe___pyx_scope_struct_4_write_response[8];
 static int __pyx_freecount_10blacksheep_6scribe___pyx_scope_struct_4_write_response = 0;
 
@@ -9643,15 +9647,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10blacksheep_6scribe___pyx_scope_struct_5_write_response_content *__pyx_freelist_10blacksheep_6scribe___pyx_scope_struct_5_write_response_content[8];
 static int __pyx_freecount_10blacksheep_6scribe___pyx_scope_struct_5_write_response_content = 0;
 
@@ -9762,15 +9766,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10blacksheep_6scribe___pyx_scope_struct_6_send_asgi_response *__pyx_freelist_10blacksheep_6scribe___pyx_scope_struct_6_send_asgi_response[8];
 static int __pyx_freecount_10blacksheep_6scribe___pyx_scope_struct_6_send_asgi_response = 0;
 
@@ -9884,15 +9888,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {"get_status_line", (PyCFunction)__pyx_pw_10blacksheep_6scribe_1get_status_line, METH_O, 0},
   {"write_response_cookie", (PyCFunction)__pyx_pw_10blacksheep_6scribe_3write_response_cookie, METH_O, 0},
@@ -10291,123 +10295,70 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule("blacksheep.contents"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_10blacksheep_8contents_Content = __Pyx_ImportType(__pyx_t_1, "blacksheep.contents", "Content", sizeof(struct __pyx_obj_10blacksheep_8contents_Content), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_8contents_Content),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_8contents_Content) __PYX_ERR(2, 8, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_StreamedContent = __Pyx_ImportType(__pyx_t_1, "blacksheep.contents", "StreamedContent", sizeof(struct __pyx_obj_10blacksheep_8contents_StreamedContent), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_8contents_StreamedContent),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_8contents_StreamedContent) __PYX_ERR(2, 14, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_ASGIContent = __Pyx_ImportType(__pyx_t_1, "blacksheep.contents", "ASGIContent", sizeof(struct __pyx_obj_10blacksheep_8contents_ASGIContent), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_8contents_ASGIContent),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_8contents_ASGIContent) __PYX_ERR(2, 18, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_Content = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "Content", sizeof(struct __pyx_obj_10blacksheep_8contents_Content), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_Content),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_Content) __PYX_ERR(2, 8, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_StreamedContent = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "StreamedContent", sizeof(struct __pyx_obj_10blacksheep_8contents_StreamedContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_StreamedContent),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_StreamedContent) __PYX_ERR(2, 14, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_ASGIContent = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "ASGIContent", sizeof(struct __pyx_obj_10blacksheep_8contents_ASGIContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_ASGIContent),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_ASGIContent) __PYX_ERR(2, 18, __pyx_L1_error)
   __pyx_vtabptr_10blacksheep_8contents_ASGIContent = (struct __pyx_vtabstruct_10blacksheep_8contents_ASGIContent*)__Pyx_GetVtable(__pyx_ptype_10blacksheep_8contents_ASGIContent->tp_dict); if (unlikely(!__pyx_vtabptr_10blacksheep_8contents_ASGIContent)) __PYX_ERR(2, 18, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_TextContent = __Pyx_ImportType(__pyx_t_1, "blacksheep.contents", "TextContent", sizeof(struct __pyx_obj_10blacksheep_8contents_TextContent), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_8contents_TextContent),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_8contents_TextContent) __PYX_ERR(2, 23, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_HTMLContent = __Pyx_ImportType(__pyx_t_1, "blacksheep.contents", "HTMLContent", sizeof(struct __pyx_obj_10blacksheep_8contents_HTMLContent), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_8contents_HTMLContent),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_8contents_HTMLContent) __PYX_ERR(2, 27, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_JSONContent = __Pyx_ImportType(__pyx_t_1, "blacksheep.contents", "JSONContent", sizeof(struct __pyx_obj_10blacksheep_8contents_JSONContent), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_8contents_JSONContent),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_8contents_JSONContent) __PYX_ERR(2, 31, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_FormContent = __Pyx_ImportType(__pyx_t_1, "blacksheep.contents", "FormContent", sizeof(struct __pyx_obj_10blacksheep_8contents_FormContent), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_8contents_FormContent),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_8contents_FormContent) __PYX_ERR(2, 35, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_FormPart = __Pyx_ImportType(__pyx_t_1, "blacksheep.contents", "FormPart", sizeof(struct __pyx_obj_10blacksheep_8contents_FormPart), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_8contents_FormPart),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_8contents_FormPart) __PYX_ERR(2, 39, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8contents_MultiPartFormData = __Pyx_ImportType(__pyx_t_1, "blacksheep.contents", "MultiPartFormData", sizeof(struct __pyx_obj_10blacksheep_8contents_MultiPartFormData), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_8contents_MultiPartFormData),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_8contents_MultiPartFormData) __PYX_ERR(2, 47, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_TextContent = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "TextContent", sizeof(struct __pyx_obj_10blacksheep_8contents_TextContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_TextContent),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_TextContent) __PYX_ERR(2, 23, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_HTMLContent = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "HTMLContent", sizeof(struct __pyx_obj_10blacksheep_8contents_HTMLContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_HTMLContent),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_HTMLContent) __PYX_ERR(2, 27, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_JSONContent = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "JSONContent", sizeof(struct __pyx_obj_10blacksheep_8contents_JSONContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_JSONContent),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_JSONContent) __PYX_ERR(2, 31, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_FormContent = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "FormContent", sizeof(struct __pyx_obj_10blacksheep_8contents_FormContent), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_FormContent),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_FormContent) __PYX_ERR(2, 35, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_FormPart = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "FormPart", sizeof(struct __pyx_obj_10blacksheep_8contents_FormPart), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_FormPart),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_FormPart) __PYX_ERR(2, 39, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8contents_MultiPartFormData = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.contents", "MultiPartFormData", sizeof(struct __pyx_obj_10blacksheep_8contents_MultiPartFormData), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8contents_MultiPartFormData),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8contents_MultiPartFormData) __PYX_ERR(2, 47, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("datetime"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_8datetime_date = __Pyx_ImportType(__pyx_t_1, "datetime", "date", sizeof(PyDateTime_Date), __PYX_GET_STRUCT_ALIGNMENT(PyDateTime_Date),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_8datetime_date) __PYX_ERR(1, 9, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_time = __Pyx_ImportType(__pyx_t_1, "datetime", "time", sizeof(PyDateTime_Time), __PYX_GET_STRUCT_ALIGNMENT(PyDateTime_Time),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_8datetime_time) __PYX_ERR(1, 12, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_datetime = __Pyx_ImportType(__pyx_t_1, "datetime", "datetime", sizeof(PyDateTime_DateTime), __PYX_GET_STRUCT_ALIGNMENT(PyDateTime_DateTime),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_8datetime_datetime) __PYX_ERR(1, 15, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_timedelta = __Pyx_ImportType(__pyx_t_1, "datetime", "timedelta", sizeof(PyDateTime_Delta), __PYX_GET_STRUCT_ALIGNMENT(PyDateTime_Delta),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_8datetime_timedelta) __PYX_ERR(1, 18, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_tzinfo = __Pyx_ImportType(__pyx_t_1, "datetime", "tzinfo", sizeof(PyDateTime_TZInfo), __PYX_GET_STRUCT_ALIGNMENT(PyDateTime_TZInfo),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_8datetime_tzinfo) __PYX_ERR(1, 21, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_date = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "date", sizeof(PyDateTime_Date), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_Date),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_date) __PYX_ERR(1, 9, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_time = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "time", sizeof(PyDateTime_Time), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_Time),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_time) __PYX_ERR(1, 12, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_datetime = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "datetime", sizeof(PyDateTime_DateTime), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_DateTime),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_datetime) __PYX_ERR(1, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_timedelta = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "timedelta", sizeof(PyDateTime_Delta), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_Delta),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_timedelta) __PYX_ERR(1, 18, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_tzinfo = __Pyx_ImportType_0_29_35(__pyx_t_1, "datetime", "tzinfo", sizeof(PyDateTime_TZInfo), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyDateTime_TZInfo),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_8datetime_tzinfo) __PYX_ERR(1, 21, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("blacksheep.cookies"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_10blacksheep_7cookies_Cookie = __Pyx_ImportType(__pyx_t_1, "blacksheep.cookies", "Cookie", sizeof(struct __pyx_obj_10blacksheep_7cookies_Cookie), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_7cookies_Cookie),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_7cookies_Cookie) __PYX_ERR(4, 17, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_7cookies_Cookie = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.cookies", "Cookie", sizeof(struct __pyx_obj_10blacksheep_7cookies_Cookie), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_7cookies_Cookie),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_7cookies_Cookie) __PYX_ERR(4, 17, __pyx_L1_error)
   __pyx_vtabptr_10blacksheep_7cookies_Cookie = (struct __pyx_vtabstruct_10blacksheep_7cookies_Cookie*)__Pyx_GetVtable(__pyx_ptype_10blacksheep_7cookies_Cookie->tp_dict); if (unlikely(!__pyx_vtabptr_10blacksheep_7cookies_Cookie)) __PYX_ERR(4, 17, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("blacksheep.exceptions"); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_10blacksheep_10exceptions_MessageAborted = __Pyx_ImportType(__pyx_t_1, "blacksheep.exceptions", "MessageAborted", sizeof(struct __pyx_obj_10blacksheep_10exceptions_MessageAborted), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_10exceptions_MessageAborted),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_10exceptions_MessageAborted) __PYX_ERR(5, 4, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_HTTPException = __Pyx_ImportType(__pyx_t_1, "blacksheep.exceptions", "HTTPException", sizeof(struct __pyx_obj_10blacksheep_10exceptions_HTTPException), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_10exceptions_HTTPException),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_10exceptions_HTTPException) __PYX_ERR(5, 8, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_BadRequest = __Pyx_ImportType(__pyx_t_1, "blacksheep.exceptions", "BadRequest", sizeof(struct __pyx_obj_10blacksheep_10exceptions_BadRequest), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_10exceptions_BadRequest),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_10exceptions_BadRequest) __PYX_ERR(5, 12, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_BadRequestFormat = __Pyx_ImportType(__pyx_t_1, "blacksheep.exceptions", "BadRequestFormat", sizeof(struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_10exceptions_BadRequestFormat) __PYX_ERR(5, 16, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_NotFound = __Pyx_ImportType(__pyx_t_1, "blacksheep.exceptions", "NotFound", sizeof(struct __pyx_obj_10blacksheep_10exceptions_NotFound), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_10exceptions_NotFound),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_10exceptions_NotFound) __PYX_ERR(5, 20, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_InvalidArgument = __Pyx_ImportType(__pyx_t_1, "blacksheep.exceptions", "InvalidArgument", sizeof(struct __pyx_obj_10blacksheep_10exceptions_InvalidArgument), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_10exceptions_InvalidArgument),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_10exceptions_InvalidArgument) __PYX_ERR(5, 24, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_10exceptions_InvalidOperation = __Pyx_ImportType(__pyx_t_1, "blacksheep.exceptions", "InvalidOperation", sizeof(struct __pyx_obj_10blacksheep_10exceptions_InvalidOperation), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_10exceptions_InvalidOperation),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_10exceptions_InvalidOperation) __PYX_ERR(5, 28, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_MessageAborted = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "MessageAborted", sizeof(struct __pyx_obj_10blacksheep_10exceptions_MessageAborted), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_MessageAborted),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_MessageAborted) __PYX_ERR(5, 4, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_HTTPException = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "HTTPException", sizeof(struct __pyx_obj_10blacksheep_10exceptions_HTTPException), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_HTTPException),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_HTTPException) __PYX_ERR(5, 8, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_BadRequest = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "BadRequest", sizeof(struct __pyx_obj_10blacksheep_10exceptions_BadRequest), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_BadRequest),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_BadRequest) __PYX_ERR(5, 12, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_BadRequestFormat = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "BadRequestFormat", sizeof(struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_BadRequestFormat),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_BadRequestFormat) __PYX_ERR(5, 16, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_NotFound = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "NotFound", sizeof(struct __pyx_obj_10blacksheep_10exceptions_NotFound), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_NotFound),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_NotFound) __PYX_ERR(5, 20, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_InvalidArgument = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "InvalidArgument", sizeof(struct __pyx_obj_10blacksheep_10exceptions_InvalidArgument), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_InvalidArgument),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_InvalidArgument) __PYX_ERR(5, 24, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_10exceptions_InvalidOperation = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.exceptions", "InvalidOperation", sizeof(struct __pyx_obj_10blacksheep_10exceptions_InvalidOperation), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_10exceptions_InvalidOperation),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_10exceptions_InvalidOperation) __PYX_ERR(5, 28, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("blacksheep.url"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_10blacksheep_3url_URL = __Pyx_ImportType(__pyx_t_1, "blacksheep.url", "URL", sizeof(struct __pyx_obj_10blacksheep_3url_URL), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_3url_URL),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_3url_URL) __PYX_ERR(6, 8, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_3url_URL = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.url", "URL", sizeof(struct __pyx_obj_10blacksheep_3url_URL), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_3url_URL),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_3url_URL) __PYX_ERR(6, 8, __pyx_L1_error)
   __pyx_vtabptr_10blacksheep_3url_URL = (struct __pyx_vtabstruct_10blacksheep_3url_URL*)__Pyx_GetVtable(__pyx_ptype_10blacksheep_3url_URL->tp_dict); if (unlikely(!__pyx_vtabptr_10blacksheep_3url_URL)) __PYX_ERR(6, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("blacksheep.messages"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_10blacksheep_8messages_Message = __Pyx_ImportType(__pyx_t_1, "blacksheep.messages", "Message", sizeof(struct __pyx_obj_10blacksheep_8messages_Message), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_8messages_Message),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_8messages_Message) __PYX_ERR(7, 18, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8messages_Message = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.messages", "Message", sizeof(struct __pyx_obj_10blacksheep_8messages_Message), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8messages_Message),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8messages_Message) __PYX_ERR(7, 18, __pyx_L1_error)
   __pyx_vtabptr_10blacksheep_8messages_Message = (struct __pyx_vtabstruct_10blacksheep_8messages_Message*)__Pyx_GetVtable(__pyx_ptype_10blacksheep_8messages_Message->tp_dict); if (unlikely(!__pyx_vtabptr_10blacksheep_8messages_Message)) __PYX_ERR(7, 18, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8messages_Request = __Pyx_ImportType(__pyx_t_1, "blacksheep.messages", "Request", sizeof(struct __pyx_obj_10blacksheep_8messages_Request), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_8messages_Request),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_8messages_Request) __PYX_ERR(7, 45, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8messages_Request = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.messages", "Request", sizeof(struct __pyx_obj_10blacksheep_8messages_Request), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8messages_Request),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8messages_Request) __PYX_ERR(7, 45, __pyx_L1_error)
   __pyx_vtabptr_10blacksheep_8messages_Request = (struct __pyx_vtabstruct_10blacksheep_8messages_Request*)__Pyx_GetVtable(__pyx_ptype_10blacksheep_8messages_Request->tp_dict); if (unlikely(!__pyx_vtabptr_10blacksheep_8messages_Request)) __PYX_ERR(7, 45, __pyx_L1_error)
-  __pyx_ptype_10blacksheep_8messages_Response = __Pyx_ImportType(__pyx_t_1, "blacksheep.messages", "Response", sizeof(struct __pyx_obj_10blacksheep_8messages_Response), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10blacksheep_8messages_Response),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10blacksheep_8messages_Response) __PYX_ERR(7, 58, __pyx_L1_error)
+  __pyx_ptype_10blacksheep_8messages_Response = __Pyx_ImportType_0_29_35(__pyx_t_1, "blacksheep.messages", "Response", sizeof(struct __pyx_obj_10blacksheep_8messages_Response), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10blacksheep_8messages_Response),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10blacksheep_8messages_Response) __PYX_ERR(7, 58, __pyx_L1_error)
   __pyx_vtabptr_10blacksheep_8messages_Response = (struct __pyx_vtabstruct_10blacksheep_8messages_Response*)__Pyx_GetVtable(__pyx_ptype_10blacksheep_8messages_Response->tp_dict); if (unlikely(!__pyx_vtabptr_10blacksheep_8messages_Response)) __PYX_ERR(7, 58, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -10428,21 +10379,21 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __pyx_t_1 = PyImport_ImportModule("blacksheep.contents"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportFunction(__pyx_t_1, "parse_www_form_urlencoded", (void (**)(void))&__pyx_f_10blacksheep_8contents_parse_www_form_urlencoded, "PyObject *(PyObject *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "parse_www_form_urlencoded", (void (**)(void))&__pyx_f_10blacksheep_8contents_parse_www_form_urlencoded, "PyObject *(PyObject *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("blacksheep.cookies"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportFunction(__pyx_t_1, "parse_cookie", (void (**)(void))&__pyx_f_10blacksheep_7cookies_parse_cookie, "struct __pyx_obj_10blacksheep_7cookies_Cookie *(PyObject *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "datetime_to_cookie_format", (void (**)(void))&__pyx_f_10blacksheep_7cookies_datetime_to_cookie_format, "PyObject *(PyDateTime_DateTime *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction(__pyx_t_1, "write_cookie_for_response", (void (**)(void))&__pyx_f_10blacksheep_7cookies_write_cookie_for_response, "PyObject *(struct __pyx_obj_10blacksheep_7cookies_Cookie *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "parse_cookie", (void (**)(void))&__pyx_f_10blacksheep_7cookies_parse_cookie, "struct __pyx_obj_10blacksheep_7cookies_Cookie *(PyObject *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "datetime_to_cookie_format", (void (**)(void))&__pyx_f_10blacksheep_7cookies_datetime_to_cookie_format, "PyObject *(PyDateTime_DateTime *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_0_29_35(__pyx_t_1, "write_cookie_for_response", (void (**)(void))&__pyx_f_10blacksheep_7cookies_write_cookie_for_response, "PyObject *(struct __pyx_obj_10blacksheep_7cookies_Cookie *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -11792,15 +11743,15 @@
 #if PY_VERSION_HEX >= 0x030500B2 || defined(PyCoro_CheckExact)
     if (PyCoro_CheckExact(obj)) {
         return __Pyx_NewRef(obj);
     } else
 #endif
 #if CYTHON_COMPILING_IN_CPYTHON && defined(CO_ITERABLE_COROUTINE)
 #if PY_VERSION_HEX >= 0x030C00A6
-    if (PyGen_CheckExact(obj) && (PyGen_GetCode(obj)->co_flags & CO_ITERABLE_COROUTINE)) {
+    if (PyGen_CheckExact(obj) && (PyGen_GetCode((PyGenObject*)obj)->co_flags & CO_ITERABLE_COROUTINE)) {
 #else
     if (PyGen_CheckExact(obj) && ((PyGenObject*)obj)->gi_code && ((PyCodeObject *)((PyGenObject*)obj)->gi_code)->co_flags & CO_ITERABLE_COROUTINE) {
 #endif
         return __Pyx_NewRef(obj);
     } else
 #endif
     {
@@ -13211,15 +13162,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 #if PY_VERSION_HEX < 0x030500B1 || defined(__Pyx_IterableCoroutine_USED) || CYTHON_USE_ASYNC_SLOTS
 static CYTHON_INLINE PyObject *__Pyx__Coroutine_await(PyObject *coroutine) {
     __pyx_CoroutineAwaitObject *await = PyObject_GC_New(__pyx_CoroutineAwaitObject, __pyx_CoroutineAwaitType);
     if (unlikely(!await)) return NULL;
@@ -13363,15 +13317,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_Coroutine_init(void) {
     __pyx_CoroutineType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx_CoroutineType = __Pyx_FetchCommonType(&__pyx_CoroutineType_type);
     if (unlikely(!__pyx_CoroutineType))
@@ -13777,18 +13734,18 @@
         function_name, key);
     #endif
 bad:
     return -1;
 }
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -13834,22 +13791,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -14251,15 +14208,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -14523,15 +14480,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -15087,15 +15044,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int
 __Pyx_PyAsyncGen_ClearFreeLists(void)
 {
     int ret = __Pyx_ag_value_freelist_free + __Pyx_ag_asend_freelist_free;
@@ -15285,15 +15245,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static PyObject *
 __Pyx_async_gen_asend_new(__pyx_PyAsyncGenObject *gen, PyObject *sendval)
 {
     __pyx_PyAsyncGenASend *o;
@@ -15387,15 +15350,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static PyObject *
 __Pyx__PyAsyncGenValueWrapperNew(PyObject *val)
 {
     __pyx__PyAsyncGenWrappedValue *o;
@@ -15628,15 +15594,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static PyObject *
 __Pyx_async_gen_athrow_new(__pyx_PyAsyncGenObject *gen, PyObject *args)
 {
     __pyx_PyAsyncGenAThrow *o;
@@ -15760,15 +15729,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_Generator_init(void) {
     __pyx_GeneratorType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx_GeneratorType_type.tp_iter = PyObject_SelfIter;
     __pyx_GeneratorType = __Pyx_FetchCommonType(&__pyx_GeneratorType_type);
@@ -15850,17 +15822,17 @@
 bad:
     Py_XDECREF(cobj);
     Py_XDECREF(d);
     return -1;
 }
 
 /* FunctionImport */
-  #ifndef __PYX_HAVE_RT_ImportFunction
-#define __PYX_HAVE_RT_ImportFunction
-static int __Pyx_ImportFunction(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
+  #ifndef __PYX_HAVE_RT_ImportFunction_0_29_35
+#define __PYX_HAVE_RT_ImportFunction_0_29_35
+static int __Pyx_ImportFunction_0_29_35(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
     PyObject *d = 0;
     PyObject *cobj = 0;
     union {
         void (*fp)(void);
         void *p;
     } tmp;
     d = PyObject_GetAttrString(module, (char *)"__pyx_capi__");
```

### Comparing `blacksheep-2.0a6/blacksheep/scribe.pxd` & `blacksheep-2.0a7/blacksheep/scribe.pxd`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/scribe.pyi` & `blacksheep-2.0a7/blacksheep/scribe.pyi`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/scribe.pyx` & `blacksheep-2.0a7/blacksheep/scribe.pyx`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/server/application.py` & `blacksheep-2.0a7/blacksheep/server/application.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/server/asgi.py` & `blacksheep-2.0a7/blacksheep/server/asgi.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/server/authentication/__init__.py` & `blacksheep-2.0a7/blacksheep/server/authentication/__init__.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/server/authentication/cookie.py` & `blacksheep-2.0a7/blacksheep/server/authentication/cookie.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/server/authentication/jwt.py` & `blacksheep-2.0a7/blacksheep/server/authentication/jwt.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
     def __init__(
         self,
         *,
         valid_audiences: Sequence[str],
         valid_issuers: Optional[Sequence[str]] = None,
         authority: Optional[str] = None,
+        algorithms: Optional[Sequence[str]] = None,
         require_kid: bool = True,
         keys_provider: Optional[KeysProvider] = None,
         keys_url: Optional[str] = None,
         cache_time: float = 10800,
         auth_mode: str = "JWT Bearer",
     ):
         """
@@ -77,16 +78,20 @@
             valid_issuers = [authority]
 
         if not authority and not valid_issuers:
             raise TypeError("Specify either an authority or valid issuers.")
 
         assert valid_issuers is not None
 
+        if not algorithms:
+            algorithms = ["RS256"]
+
         self._validator = JWTValidator(
             authority=authority,
+            algorithms=algorithms,
             require_kid=require_kid,
             keys_provider=keys_provider,
             keys_url=keys_url,
             valid_issuers=valid_issuers,
             valid_audiences=valid_audiences,
             cache_time=cache_time,
         )
```

### Comparing `blacksheep-2.0a6/blacksheep/server/authentication/oidc.py` & `blacksheep-2.0a7/blacksheep/server/authentication/oidc.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/server/authorization/__init__.py` & `blacksheep-2.0a7/blacksheep/server/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/server/bindings.py` & `blacksheep-2.0a7/blacksheep/server/bindings.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/server/compression.py` & `blacksheep-2.0a7/blacksheep/server/compression.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/server/controllers.py` & `blacksheep-2.0a7/blacksheep/server/controllers.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/server/cors.py` & `blacksheep-2.0a7/blacksheep/server/cors.py`

 * *Files 3% similar despite different names*

```diff
@@ -235,14 +235,25 @@
 
 
 @lru_cache(maxsize=20)
 def _get_encoded_value_for_max_age(max_age: int) -> bytes:
     return str(max_age).encode()
 
 
+def _set_cors_origin(response: Response, origin_response: bytes):
+    """
+    Sets a Access-Control-Allow-Origin to the given value, and a `Vary: Origin` header
+    if that value is not "*".
+    """
+    response.set_header(b"Access-Control-Allow-Origin", origin_response)
+
+    if origin_response != b"*":
+        response.add_header(b"Vary", b"Origin")
+
+
 def get_cors_middleware(
     app: BaseApplication,
     strategy: CORSStrategy,
 ) -> Callable[[Request, Callable[..., Any]], Awaitable[Response]]:
     async def cors_middleware(request: Request, handler):
         if isinstance(request, WebSocket):
             return await handler(request)
@@ -263,25 +274,27 @@
             next_request_method or request.method, request.url.path
         )
 
         if route is None:
             return not_found()
 
         policy = strategy.get_policy_by_route_or_default(route)
-        allowed_origins = _get_encoded_value_for_set(policy.allow_origins)
         allowed_methods = _get_encoded_value_for_set(policy.allow_methods)
         expose_headers = _get_encoded_value_for_set(policy.expose_headers)
         max_age = _get_encoded_value_for_max_age(policy.max_age)
 
         if (
             "*" not in policy.allow_origins
             and origin.decode() not in policy.allow_origins
         ):
             return _get_invalid_origin_response()
 
+        # https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Access-Control-Allow-Origin
+        origin_response = b"*" if "*" in policy.allow_origins else origin
+
         if next_request_method:
             # This is a preflight request;
             if (
                 "*" not in policy.allow_methods
                 and next_request_method.decode() not in policy.allow_methods
             ):
                 return _get_invalid_method_response()
@@ -293,16 +306,16 @@
             if next_request_headers and "*" not in policy.allow_headers:
                 for value in next_request_headers.split(b","):
                     str_value = value.strip().decode()
                     if str_value.lower() not in policy.allow_headers:
                         return _get_invalid_header_response(str_value)
 
             response = ok()
+            _set_cors_origin(response, origin_response)
             response.set_header(b"Access-Control-Allow-Methods", allowed_methods)
-            response.set_header(b"Access-Control-Allow-Origin", allowed_origins)
 
             if next_request_headers:
                 response.set_header(
                     b"Access-Control-Allow-Headers", next_request_headers
                 )
 
             if policy.allow_credentials:
@@ -325,13 +338,13 @@
         # If CORS response headers weren't set, error details wouldn't be available
         # to the client code, in such circumstances.
         try:
             response = await handler(request)
         except Exception as exc:
             response = await app.handle_request_handler_exception(request, exc)
 
-        response.set_header(b"Access-Control-Allow-Origin", allowed_origins)
+        _set_cors_origin(response, origin_response)
         response.set_header(b"Access-Control-Expose-Headers", expose_headers)
 
         return response
 
     return cors_middleware
```

### Comparing `blacksheep-2.0a6/blacksheep/server/csrf.py` & `blacksheep-2.0a7/blacksheep/server/csrf.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/server/dataprotection.py` & `blacksheep-2.0a7/blacksheep/server/dataprotection.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/server/di.py` & `blacksheep-2.0a7/blacksheep/server/di.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/server/env.py` & `blacksheep-2.0a7/blacksheep/server/env.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/server/errors.py` & `blacksheep-2.0a7/blacksheep/server/errors.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/server/files/__init__.py` & `blacksheep-2.0a7/blacksheep/server/files/__init__.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/server/files/dynamic.py` & `blacksheep-2.0a7/blacksheep/server/files/dynamic.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/server/files/static.py` & `blacksheep-2.0a7/blacksheep/server/files/static.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/server/headers/cache.py` & `blacksheep-2.0a7/blacksheep/server/headers/cache.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/server/normalization.py` & `blacksheep-2.0a7/blacksheep/server/normalization.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/server/openapi/common.py` & `blacksheep-2.0a7/blacksheep/server/openapi/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -97,14 +97,20 @@
 @dataclass
 class ResponseInfo:
     description: str
     headers: Optional[Dict[str, HeaderInfo]] = None
     content: Optional[List[ContentInfo]] = None
 
 
+@dataclass
+class SecurityInfo:
+    name: str
+    value: List[str]
+
+
 ResponseStatusType = Union[int, str, HTTPStatus]
 
 
 def response_status_to_str(value: ResponseStatusType) -> str:
     if isinstance(value, HTTPStatus):
         return str(value.value)  # type: ignore
     if isinstance(value, str):
@@ -119,14 +125,15 @@
     tags: Optional[List[str]] = None
     parameters: Optional[Mapping[str, ParameterInfo]] = None
     request_body: Optional[RequestBodyInfo] = None
     responses: Optional[Dict[ResponseStatusType, Union[str, ResponseInfo]]] = None
     ignored: Optional[bool] = None
     deprecated: Optional[bool] = None
     on_created: Optional[Callable[[Any, Any], None]] = None
+    security: Optional[List[SecurityInfo]] = None
 
 
 OpenAPIRootType = TypeVar("OpenAPIRootType", bound=OpenAPIRoot)
 
 
 class OpenAPIEndpointException(Exception):
     pass
@@ -184,14 +191,15 @@
         tags: Optional[List[str]] = None,
         parameters: Optional[Mapping[str, ParameterInfo]] = None,
         request_body: Optional[RequestBodyInfo] = None,
         responses: Optional[Dict[ResponseStatusType, Union[str, ResponseInfo]]] = None,
         ignored: Optional[bool] = None,
         deprecated: Optional[bool] = None,
         on_created: Optional[Callable[[Any, Any], None]] = None,
+        security: Optional[List[SecurityInfo]] = None,
     ) -> Any:
         def decorator(fn):
             if doc:
                 self._handlers_docs[fn] = doc
                 return fn
 
             self._handlers_docs[fn] = EndpointDocs(
@@ -200,14 +208,15 @@
                 tags=tags,
                 request_body=request_body,
                 responses=responses,
                 parameters=parameters,
                 ignored=ignored,
                 deprecated=deprecated,
                 on_created=on_created,
+                security=security,
             )
             return fn
 
         return decorator
 
     def register(self, schema) -> Any:
         """
```

### Comparing `blacksheep-2.0a6/blacksheep/server/openapi/docstrings.py` & `blacksheep-2.0a7/blacksheep/server/openapi/docstrings.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/server/openapi/exceptions.py` & `blacksheep-2.0a7/blacksheep/server/openapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/server/openapi/ui.py` & `blacksheep-2.0a7/blacksheep/server/openapi/ui.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/server/openapi/v3.py` & `blacksheep-2.0a7/blacksheep/server/openapi/v3.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,29 +8,40 @@
 from typing import Any, Dict, Iterable, List, Optional, Tuple, Type, Union
 from typing import _GenericAlias as GenericAlias
 from typing import get_type_hints
 from uuid import UUID
 
 from openapidocs.common import Format
 from openapidocs.v3 import (
+    APIKeySecurity,
     Components,
     Example,
     Header,
+    HTTPSecurity,
     Info,
     MediaType,
+    OAuth2Security,
     OpenAPI,
+    OpenIdConnectSecurity,
     Operation,
     Parameter,
     ParameterLocation,
     PathItem,
     Reference,
     RequestBody,
 )
 from openapidocs.v3 import Response as ResponseDoc
-from openapidocs.v3 import Schema, Server, Tag, ValueFormat, ValueType
+from openapidocs.v3 import (
+    Schema,
+    SecurityRequirement,
+    Server,
+    Tag,
+    ValueFormat,
+    ValueType,
+)
 
 from blacksheep.server.bindings import (
     Binder,
     BodyBinder,
     CookieBinder,
     HeaderBinder,
     QueryBinder,
@@ -258,14 +269,22 @@
                     fields_info.get(name, None), value
                 ),
             )
             for name, value in properties.items()
         ]
 
 
+SecuritySchemes = Union[
+    OAuth2Security,
+    OpenIdConnectSecurity,
+    HTTPSecurity,
+    APIKeySecurity,
+]
+
+
 class OpenAPIHandler(APIDocsHandler[OpenAPI]):
     """
     Handles the automatic generation of OpenAPI Documentation, specification v3
     for a web application, exposing methods to enrich the documentation with details
     through decorators.
     """
 
@@ -275,14 +294,20 @@
         info: Info,
         ui_path: str = "/docs",
         json_spec_path: str = "/openapi.json",
         yaml_spec_path: str = "/openapi.yaml",
         preferred_format: Format = Format.JSON,
         anonymous_access: bool = True,
         tags: Optional[List[Tag]] = None,
+        security_schemes: Optional[
+            Dict[
+                str,
+                SecuritySchemes,
+            ]
+        ] = None,
     ) -> None:
         super().__init__(
             ui_path=ui_path,
             json_spec_path=json_spec_path,
             yaml_spec_path=yaml_spec_path,
             preferred_format=preferred_format,
             anonymous_access=anonymous_access,
@@ -296,14 +321,15 @@
         self._object_types_handlers: List[ObjectTypeHandler] = [
             DataClassTypeHandler(),
             PydanticModelTypeHandler(),
         ]
         self._binder_docs: Dict[
             Type[Binder], Iterable[Union[Parameter, Reference]]
         ] = {}
+        self.security_schemes = security_schemes or {}
 
     @property
     def object_types_handlers(self) -> List[ObjectTypeHandler]:
         return self._object_types_handlers
 
     def get_ui_page_title(self) -> str:
         return self.info.title
@@ -329,14 +355,15 @@
 
     def _tags_from_paths(self, paths: Dict[str, PathItem]) -> List[Tag]:
         unique_tags = set(self._iter_tags(paths))
         return [Tag(name=name) for name in sorted(unique_tags)]
 
     def generate_documentation(self, app: Application) -> OpenAPI:
         self._optimize_binders_docs()
+        self._generate_security_schemes()
         paths = self.get_paths(app)
         return OpenAPI(
             info=self.info,
             paths=paths,
             components=self.components,
             tags=self._tags or self._tags_from_paths(paths),
         )
@@ -389,14 +416,24 @@
             return self.get_type_name_for_generic(object_type, context_type_args)
         if hasattr(object_type, "__name__"):
             return object_type.__name__
         raise ValueError(
             f"Cannot obtain a name for object_type parameter: {object_type!r}"
         )
 
+    def _generate_security_schemes(self):
+        for name, scheme in self.security_schemes.items():
+            self.register_security_scheme(name, scheme)
+
+    def register_security_scheme(self, name: str, scheme: SecuritySchemes):
+        if self.components.security_schemes is None:
+            self.components.security_schemes = {}
+
+        self.components.security_schemes[name] = scheme
+
     def register_schema_for_type(self, object_type: Type) -> Reference:
         stored_ref = self._get_stored_reference(object_type, None)
         if stored_ref:
             return stored_ref
 
         schema = self.get_schema_by_type(object_type)
         if isinstance(schema, Schema):
@@ -777,14 +814,21 @@
                     else None,
                     description=param_info.description,
                     example=param_info.example,
                 )
 
         return list(parameters.values())
 
+    def get_handler_security(self, handler: Any) -> Optional[List[SecurityRequirement]]:
+        docs = self.get_handler_docs(handler)
+        if docs and docs.security:
+            return [SecurityRequirement(s.name, s.value) for s in docs.security]
+
+        return None
+
     def _get_media_type_from_content_doc(self, content_doc: ContentInfo) -> MediaType:
         media_type = MediaType()
 
         if content_doc.type:
             media_type.schema = self.get_schema_by_type(content_doc.type)
 
         examples = content_doc.examples
@@ -990,14 +1034,15 @@
                     summary=self.get_summary(handler),
                     responses=self.get_responses(handler) or {},
                     operation_id=self.get_operation_id(docs, handler),
                     parameters=self.get_parameters(handler),
                     request_body=self.get_request_body(handler),
                     deprecated=self.is_deprecated(handler),
                     tags=self.get_handler_tags(handler),
+                    security=self.get_handler_security(handler),
                 )
                 if docs and docs.on_created:
                     docs.on_created(self, operation)
 
                 self.events.on_operation_created.fire_sync(operation)
                 setattr(path_item, method, operation)
```

### Comparing `blacksheep-2.0a6/blacksheep/server/remotes/forwarding.py` & `blacksheep-2.0a7/blacksheep/server/remotes/forwarding.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/server/remotes/hosts.py` & `blacksheep-2.0a7/blacksheep/server/remotes/hosts.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/server/rendering/abc.py` & `blacksheep-2.0a7/blacksheep/server/rendering/abc.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/server/rendering/jinja2.py` & `blacksheep-2.0a7/blacksheep/server/rendering/jinja2.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/server/res/error.css` & `blacksheep-2.0a7/blacksheep/server/res/error.css`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/server/res/error.html` & `blacksheep-2.0a7/blacksheep/server/res/error.html`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/server/res/redoc-ui.html` & `blacksheep-2.0a7/blacksheep/server/res/redoc-ui.html`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/server/res/swagger-ui.html` & `blacksheep-2.0a7/blacksheep/server/res/swagger-ui.html`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/server/responses.py` & `blacksheep-2.0a7/blacksheep/server/responses.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/server/routing.py` & `blacksheep-2.0a7/blacksheep/server/routing.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/server/security/hsts.py` & `blacksheep-2.0a7/blacksheep/server/security/hsts.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/server/websocket.py` & `blacksheep-2.0a7/blacksheep/server/websocket.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/sessions/__init__.py` & `blacksheep-2.0a7/blacksheep/sessions/__init__.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/settings/di.py` & `blacksheep-2.0a7/blacksheep/settings/di.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/settings/html.py` & `blacksheep-2.0a7/blacksheep/settings/html.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/settings/json.py` & `blacksheep-2.0a7/blacksheep/settings/json.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/testing/client.py` & `blacksheep-2.0a7/blacksheep/testing/client.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/testing/helpers.py` & `blacksheep-2.0a7/blacksheep/testing/helpers.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/testing/messages.py` & `blacksheep-2.0a7/blacksheep/testing/messages.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/testing/simulator.py` & `blacksheep-2.0a7/blacksheep/testing/simulator.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/url.c` & `blacksheep-2.0a7/blacksheep/url.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.35 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -74,16 +74,20 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -6633,15 +6637,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_10blacksheep_3url_InvalidURL(PyTypeObject *t, PyObject *a, PyObject *k) {
   PyObject *o = (&((PyTypeObject*)PyExc_Exception)[0])->tp_new(t, a, k);
   if (unlikely(!o)) return 0;
@@ -6739,15 +6743,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {"build_absolute_url", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10blacksheep_3url_3build_absolute_url, METH_VARARGS|METH_KEYWORDS, 0},
   {0, 0, 0, 0}
@@ -9409,15 +9413,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -9605,15 +9609,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `blacksheep-2.0a6/blacksheep/url.pxd` & `blacksheep-2.0a7/blacksheep/url.pxd`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/url.pyi` & `blacksheep-2.0a7/blacksheep/url.pyi`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/url.pyx` & `blacksheep-2.0a7/blacksheep/url.pyx`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/utils/__init__.py` & `blacksheep-2.0a7/blacksheep/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/utils/aio.py` & `blacksheep-2.0a7/blacksheep/utils/aio.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/blacksheep/utils/meta.py` & `blacksheep-2.0a7/blacksheep/utils/meta.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,10 +21,10 @@
     """
     path = str(root_path)
     modules = [
         os.path.basename(f)[:-3]
         for f in glob.glob(path + "/*.py")
         if not os.path.basename(f).startswith("_")
     ]
-    stripped_path = os.path.relpath(path).replace("/", ".")
+    stripped_path = os.path.relpath(path).replace("/", ".").replace("\\", ".")
     for module in modules:
         __import__(stripped_path + "." + module)
```

### Comparing `blacksheep-2.0a6/blacksheep.egg-info/PKG-INFO` & `blacksheep-2.0a7/blacksheep.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blacksheep
-Version: 2.0a6
+Version: 2.0a7
 Summary: Fast web framework for Python asyncio
 Author-email: Roberto Prevato <roberto.prevato@gmail.com>
 Project-URL: Homepage, https://github.com/Neoteroi/BlackSheep
 Project-URL: Bug Tracker, https://github.com/Neoteroi/BlackSheep/issues
 Keywords: blacksheep,web framework,asyncio
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: blacksheep Version: 2.0a6 Summary: Fast web
+Metadata-Version: 2.1 Name: blacksheep Version: 2.0a7 Summary: Fast web
 framework for Python asyncio Author-email: Roberto Prevato
 prevato@gmail.com> Project-URL: Homepage, https://github.com/Neoteroi/
 BlackSheep Project-URL: Bug Tracker, https://github.com/Neoteroi/BlackSheep/
 issues Keywords: blacksheep,web framework,asyncio Classifier: Development
 Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `blacksheep-2.0a6/blacksheep.egg-info/SOURCES.txt` & `blacksheep-2.0a7/blacksheep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/pyproject.toml` & `blacksheep-2.0a7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "blacksheep"
-version = "2.0a6"
+version = "2.0a7"
 authors = [
     { name = "Roberto Prevato", email = "roberto.prevato@gmail.com" },
 ]
 description = "Fast web framework for Python asyncio"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `blacksheep-2.0a6/setup.py` & `blacksheep-2.0a7/setup.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/tests/test_application.py` & `blacksheep-2.0a7/tests/test_application.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/tests/test_auth.py` & `blacksheep-2.0a7/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/tests/test_auth_cookie.py` & `blacksheep-2.0a7/tests/test_auth_cookie.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/tests/test_bindings.py` & `blacksheep-2.0a7/tests/test_bindings.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/tests/test_caching.py` & `blacksheep-2.0a7/tests/test_caching.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/tests/test_contents.py` & `blacksheep-2.0a7/tests/test_contents.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/tests/test_controllers.py` & `blacksheep-2.0a7/tests/test_controllers.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/tests/test_cookies.py` & `blacksheep-2.0a7/tests/test_cookies.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/tests/test_cors.py` & `blacksheep-2.0a7/tests/test_cors.py`

 * *Files 2% similar despite different names*

```diff
@@ -762,7 +762,61 @@
         ),
         MockReceive(),
         MockSend(),
     )
 
     response = app.response
     assert response.status == 404
+
+
+@pytest.mark.asyncio
+async def test_response_to_cors_request_contains_single_allow_origin(app):
+    app.use_cors(
+        allow_methods="GET POST",
+        allow_origins="https://www.neoteroi.dev https://www.neoteroi.xyz",
+    )
+
+    @app.router.post("/")
+    async def home():
+        return text("Hello, World")
+
+    await app.start()
+
+    await app(
+        get_example_scope(
+            "POST",
+            "/",
+            [
+                (b"Origin", b"https://www.neoteroi.dev"),
+            ],
+        ),
+        MockReceive(),
+        MockSend(),
+    )
+
+    response = app.response
+    assert response.status == 200
+    assert (
+        response.headers.get_single(b"Access-Control-Allow-Origin")
+        == b"https://www.neoteroi.dev"
+    )
+    assert response.headers.get_single(b"Access-Control-Expose-Headers") is not None
+
+    await app(
+        get_example_scope(
+            "POST",
+            "/",
+            [
+                (b"Origin", b"https://www.neoteroi.xyz"),
+            ],
+        ),
+        MockReceive(),
+        MockSend(),
+    )
+
+    response = app.response
+    assert response.status == 200
+    assert (
+        response.headers.get_single(b"Access-Control-Allow-Origin")
+        == b"https://www.neoteroi.xyz"
+    )
+    assert response.headers.get_single(b"Access-Control-Expose-Headers") is not None
```

### Comparing `blacksheep-2.0a6/tests/test_csrf.py` & `blacksheep-2.0a7/tests/test_csrf.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/tests/test_dataprotection.py` & `blacksheep-2.0a7/tests/test_dataprotection.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/tests/test_files_handler.py` & `blacksheep-2.0a7/tests/test_files_handler.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/tests/test_files_serving.py` & `blacksheep-2.0a7/tests/test_files_serving.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/tests/test_forwarding.py` & `blacksheep-2.0a7/tests/test_forwarding.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/tests/test_gzip.py` & `blacksheep-2.0a7/tests/test_gzip.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/tests/test_headers.py` & `blacksheep-2.0a7/tests/test_headers.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/tests/test_multipart.py` & `blacksheep-2.0a7/tests/test_multipart.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/tests/test_normalization.py` & `blacksheep-2.0a7/tests/test_normalization.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/tests/test_openapi_docstrings.py` & `blacksheep-2.0a7/tests/test_openapi_docstrings.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/tests/test_openapi_v3.py` & `blacksheep-2.0a7/tests/test_openapi_v3.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,27 +2,41 @@
 from datetime import date, datetime
 from enum import IntEnum
 from typing import Generic, List, Optional, Sequence, TypeVar, Union
 from uuid import UUID
 
 import pytest
 from openapidocs.common import Format, Serializer
-from openapidocs.v3 import Info, Reference, Schema, ValueFormat, ValueType
+from openapidocs.v3 import (
+    APIKeySecurity,
+    HTTPSecurity,
+    Info,
+    OAuth2Security,
+    OAuthFlow,
+    OAuthFlows,
+    OpenIdConnectSecurity,
+    ParameterLocation,
+    Reference,
+    Schema,
+    ValueFormat,
+    ValueType,
+)
 from pydantic import BaseModel, HttpUrl, validator
 from pydantic.generics import GenericModel
 from pydantic.types import NegativeFloat, PositiveInt, condecimal, confloat, conint
 
 from blacksheep.server.application import Application
 from blacksheep.server.bindings import FromForm
 from blacksheep.server.controllers import APIController
 from blacksheep.server.openapi.common import (
     ContentInfo,
     EndpointDocs,
     OpenAPIEndpointException,
     ResponseInfo,
+    SecurityInfo,
 )
 from blacksheep.server.openapi.exceptions import (
     DuplicatedContentTypeDocsException,
     UnsupportedUnionTypeException,
 )
 from blacksheep.server.openapi.v3 import (
     DataClassTypeHandler,
@@ -1877,14 +1891,24 @@
 
     app = get_app()
 
     @app.route("/")
     def home() -> A:
         ...
 
+    @docs(
+        security=[
+            SecurityInfo("basicAuth", []),
+            SecurityInfo("bearerAuth", ["read:home", "write:home"]),
+        ]
+    )
+    @app.route("/", methods=["POST"])
+    def auth_home() -> A:
+        ...
+
     docs.bind_app(app)
     await app.start()
 
     yaml = serializer.to_yaml(docs.generate_documentation(app))
 
     assert (
         yaml.strip()
@@ -1900,14 +1924,28 @@
                 '200':
                     description: Success response
                     content:
                         application/json:
                             schema:
                                 $ref: '#/components/schemas/A'
             operationId: home
+        post:
+            responses:
+                '200':
+                    description: Success response
+                    content:
+                        application/json:
+                            schema:
+                                $ref: '#/components/schemas/A'
+            operationId: auth_home
+            security:
+            -   basicAuth: []
+            -   bearerAuth:
+                - read:home
+                - write:home
 components:
     schemas:
         A:
             type: object
             required:
             - foo
             properties:
@@ -2606,15 +2644,53 @@
 
 @pytest.mark.asyncio
 async def test_sorting_api_controllers_tags(serializer: Serializer):
     app = get_app()
     get = app.controllers_router.get
     post = app.controllers_router.post
 
-    docs = OpenAPIHandler(info=Info(title="Example API", version="0.0.1"))
+    docs = OpenAPIHandler(
+        info=Info(
+            title="Example API",
+            version="0.0.1",
+        ),
+        security_schemes={
+            "basicAuth": HTTPSecurity(
+                scheme="basic",
+                description="Basic Auth",
+            ),
+            "bearerAuth": HTTPSecurity(
+                scheme="bearer",
+                description="Bearer Auth",
+            ),
+            "apiKeyAuth": APIKeySecurity(
+                in_=ParameterLocation.HEADER,
+                name="X-API-Key",
+                description="API Key Auth",
+            ),
+            "openID": OpenIdConnectSecurity(
+                open_id_connect_url="https://example.com",
+                description="OIDC Auth",
+            ),
+            "oauth2": OAuth2Security(
+                flows=OAuthFlows(
+                    implicit=OAuthFlow(
+                        authorization_url="https://example.com/oauth2/authorize",
+                        token_url="https://example.com/oauth2/token",
+                        refresh_url="https://example.com/oauth2/refresh",
+                        scopes={
+                            "read:cats": "Read your cats",
+                            "write:cats": "Write your cats",
+                        },
+                    )
+                ),
+                description="OAuth2 Auth",
+            ),
+        },
+    )
     docs.bind_app(app)
 
     @dataclass
     class Cat:
         pass
 
     @dataclass
@@ -2773,13 +2849,42 @@
             properties: {}
         Dog:
             type: object
             properties: {}
         Cat:
             type: object
             properties: {}
+    securitySchemes:
+        basicAuth:
+            scheme: basic
+            type: http
+            description: Basic Auth
+        bearerAuth:
+            scheme: bearer
+            type: http
+            description: Bearer Auth
+        apiKeyAuth:
+            name: X-API-Key
+            in: header
+            type: apiKey
+            description: API Key Auth
+        openID:
+            openIdConnectUrl: https://example.com
+            type: openIdConnect
+            description: OIDC Auth
+        oauth2:
+            flows:
+                implicit:
+                    scopes:
+                        read:cats: Read your cats
+                        write:cats: Write your cats
+                    authorizationUrl: https://example.com/oauth2/authorize
+                    tokenUrl: https://example.com/oauth2/token
+                    refreshUrl: https://example.com/oauth2/refresh
+            type: oauth2
+            description: OAuth2 Auth
 tags:
 -   name: Cats
 -   name: Dogs
 -   name: Parrots
 """.strip()
     )
```

### Comparing `blacksheep-2.0a6/tests/test_pathutils.py` & `blacksheep-2.0a7/tests/test_pathutils.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/tests/test_ranges.py` & `blacksheep-2.0a7/tests/test_ranges.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/tests/test_requests.py` & `blacksheep-2.0a7/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/tests/test_responses.py` & `blacksheep-2.0a7/tests/test_responses.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/tests/test_router.py` & `blacksheep-2.0a7/tests/test_router.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/tests/test_sessions.py` & `blacksheep-2.0a7/tests/test_sessions.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/tests/test_templating.py` & `blacksheep-2.0a7/tests/test_templating.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/tests/test_testing.py` & `blacksheep-2.0a7/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/tests/test_url.py` & `blacksheep-2.0a7/tests/test_url.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/tests/test_utils.py` & `blacksheep-2.0a7/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a6/tests/test_websocket.py` & `blacksheep-2.0a7/tests/test_websocket.py`

 * *Files identical despite different names*

