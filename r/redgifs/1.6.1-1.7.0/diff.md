# Comparing `tmp/redgifs-1.6.1.tar.gz` & `tmp/redgifs-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redgifs-1.6.1.tar", last modified: Wed May 24 17:14:58 2023, max compression
+gzip compressed data, was "redgifs-1.7.0.tar", last modified: Wed Jun 14 09:14:55 2023, max compression
```

## Comparing `redgifs-1.6.1.tar` & `redgifs-1.7.0.tar`

### file list

```diff
@@ -1,32 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 17:14:58.376152 redgifs-1.6.1/
--rw-rw-rw-   0        0        0     1081 2023-05-02 03:05:42.000000 redgifs-1.6.1/LICENSE
--rw-rw-rw-   0        0        0       25 2023-05-02 03:05:42.000000 redgifs-1.6.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2040 2023-05-24 17:14:58.374154 redgifs-1.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     1513 2023-05-03 09:52:15.000000 redgifs-1.6.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 17:14:58.230999 redgifs-1.6.1/redgifs/
--rw-rw-rw-   0        0        0     1622 2023-05-24 17:03:51.000000 redgifs-1.6.1/redgifs/__init__.py
--rw-rw-rw-   0        0        0     7140 2023-05-10 15:25:07.000000 redgifs-1.6.1/redgifs/__main__.py
--rw-rw-rw-   0        0        0     5406 2023-05-10 14:59:39.000000 redgifs-1.6.1/redgifs/aio.py
--rw-rw-rw-   0        0        0    10605 2023-05-03 09:47:21.000000 redgifs-1.6.1/redgifs/api.py
--rw-rw-rw-   0        0        0     1234 2023-05-02 03:05:42.000000 redgifs-1.6.1/redgifs/const.py
--rw-rw-rw-   0        0        0   153021 2023-05-03 03:37:37.000000 redgifs-1.6.1/redgifs/enums.py
--rw-rw-rw-   0        0        0     2661 2023-05-02 03:05:42.000000 redgifs-1.6.1/redgifs/errors.py
--rw-rw-rw-   0        0        0    11849 2023-05-03 03:42:33.000000 redgifs-1.6.1/redgifs/http.py
--rw-rw-rw-   0        0        0     9027 2023-05-03 04:35:11.000000 redgifs-1.6.1/redgifs/models.py
--rw-rw-rw-   0        0        0     9954 2023-05-03 04:07:51.000000 redgifs-1.6.1/redgifs/parser.py
--rw-rw-rw-   0        0        0     1665 2023-05-02 03:05:42.000000 redgifs-1.6.1/redgifs/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-24 17:14:58.287062 redgifs-1.6.1/redgifs.egg-info/
--rw-rw-rw-   0        0        0     2040 2023-05-24 17:14:57.000000 redgifs-1.6.1/redgifs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      530 2023-05-24 17:14:57.000000 redgifs-1.6.1/redgifs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 17:14:57.000000 redgifs-1.6.1/redgifs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-24 17:14:57.000000 redgifs-1.6.1/redgifs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       95 2023-05-24 17:14:57.000000 redgifs-1.6.1/redgifs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-24 17:14:57.000000 redgifs-1.6.1/redgifs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       34 2023-05-02 03:05:42.000000 redgifs-1.6.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 17:14:58.377153 redgifs-1.6.1/setup.cfg
--rw-rw-rw-   0        0        0     1179 2023-05-06 13:55:09.000000 redgifs-1.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 17:14:58.369152 redgifs-1.6.1/tests/
--rw-rw-rw-   0        0        0      134 2023-05-02 03:05:42.000000 redgifs-1.6.1/tests/test_invalid_search.py
--rw-rw-rw-   0        0        0      425 2023-05-02 03:05:42.000000 redgifs-1.6.1/tests/test_result_attrs.py
--rw-rw-rw-   0        0        0      873 2023-05-02 03:05:42.000000 redgifs-1.6.1/tests/test_search.py
--rw-rw-rw-   0        0        0      697 2023-05-02 03:05:42.000000 redgifs-1.6.1/tests/test_tags.py
+drwxr-xr-x   0 scruz     (1000) scruz     (1000)        0 2023-06-14 09:14:55.774782 redgifs-1.7.0/
+-rw-r--r--   0 scruz     (1000) scruz     (1000)     1081 2023-05-27 17:52:04.000000 redgifs-1.7.0/LICENSE
+-rw-r--r--   0 scruz     (1000) scruz     (1000)       51 2023-06-08 17:16:32.000000 redgifs-1.7.0/MANIFEST.in
+-rw-r--r--   0 scruz     (1000) scruz     (1000)     2068 2023-06-14 09:14:55.774782 redgifs-1.7.0/PKG-INFO
+-rw-r--r--   0 scruz     (1000) scruz     (1000)     1630 2023-06-13 04:20:23.000000 redgifs-1.7.0/README.md
+drwxr-xr-x   0 scruz     (1000) scruz     (1000)        0 2023-06-14 09:14:55.764782 redgifs-1.7.0/redgifs/
+-rw-r--r--   0 scruz     (1000) scruz     (1000)     1639 2023-06-14 09:08:09.000000 redgifs-1.7.0/redgifs/__init__.py
+-rw-r--r--   0 scruz     (1000) scruz     (1000)     7194 2023-06-13 04:21:15.000000 redgifs-1.7.0/redgifs/__main__.py
+-rw-r--r--   0 scruz     (1000) scruz     (1000)     5351 2023-06-02 00:11:47.000000 redgifs-1.7.0/redgifs/aio.py
+-rw-r--r--   0 scruz     (1000) scruz     (1000)    10426 2023-06-02 00:32:47.000000 redgifs-1.7.0/redgifs/api.py
+-rw-r--r--   0 scruz     (1000) scruz     (1000)     1234 2023-06-01 10:27:52.000000 redgifs-1.7.0/redgifs/const.py
+-rw-r--r--   0 scruz     (1000) scruz     (1000)     1306 2023-06-02 00:13:19.000000 redgifs-1.7.0/redgifs/enums.py
+-rw-r--r--   0 scruz     (1000) scruz     (1000)     2661 2023-06-01 10:27:53.000000 redgifs-1.7.0/redgifs/errors.py
+-rw-r--r--   0 scruz     (1000) scruz     (1000)    11717 2023-05-31 19:16:35.000000 redgifs-1.7.0/redgifs/http.py
+-rw-r--r--   0 scruz     (1000) scruz     (1000)     9031 2023-06-02 00:32:25.000000 redgifs-1.7.0/redgifs/models.py
+-rw-r--r--   0 scruz     (1000) scruz     (1000)     9954 2023-06-01 10:28:00.000000 redgifs-1.7.0/redgifs/parser.py
+-rw-r--r--   0 scruz     (1000) scruz     (1000)   203632 2023-05-31 11:42:30.000000 redgifs-1.7.0/redgifs/tags.json
+-rw-r--r--   0 scruz     (1000) scruz     (1000)     2724 2023-06-08 17:57:53.000000 redgifs-1.7.0/redgifs/tags.py
+-rw-r--r--   0 scruz     (1000) scruz     (1000)     2084 2023-06-07 20:09:42.000000 redgifs-1.7.0/redgifs/utils.py
+drwxr-xr-x   0 scruz     (1000) scruz     (1000)        0 2023-06-14 09:14:55.764782 redgifs-1.7.0/redgifs.egg-info/
+-rw-r--r--   0 scruz     (1000) scruz     (1000)     2068 2023-06-14 09:14:55.000000 redgifs-1.7.0/redgifs.egg-info/PKG-INFO
+-rw-r--r--   0 scruz     (1000) scruz     (1000)      585 2023-06-14 09:14:55.000000 redgifs-1.7.0/redgifs.egg-info/SOURCES.txt
+-rw-r--r--   0 scruz     (1000) scruz     (1000)        1 2023-06-14 09:14:55.000000 redgifs-1.7.0/redgifs.egg-info/dependency_links.txt
+-rw-r--r--   0 scruz     (1000) scruz     (1000)       50 2023-06-14 09:14:55.000000 redgifs-1.7.0/redgifs.egg-info/entry_points.txt
+-rw-r--r--   0 scruz     (1000) scruz     (1000)       95 2023-06-14 09:14:55.000000 redgifs-1.7.0/redgifs.egg-info/requires.txt
+-rw-r--r--   0 scruz     (1000) scruz     (1000)        8 2023-06-14 09:14:55.000000 redgifs-1.7.0/redgifs.egg-info/top_level.txt
+-rw-r--r--   0 scruz     (1000) scruz     (1000)       34 2023-05-27 17:52:04.000000 redgifs-1.7.0/requirements.txt
+-rw-r--r--   0 scruz     (1000) scruz     (1000)       38 2023-06-14 09:14:55.774782 redgifs-1.7.0/setup.cfg
+-rw-r--r--   0 scruz     (1000) scruz     (1000)     1179 2023-05-31 11:07:41.000000 redgifs-1.7.0/setup.py
+drwxr-xr-x   0 scruz     (1000) scruz     (1000)        0 2023-06-14 09:14:55.774782 redgifs-1.7.0/tests/
+-rw-r--r--   0 scruz     (1000) scruz     (1000)      298 2023-06-01 10:50:33.000000 redgifs-1.7.0/tests/test_images.py
+-rw-r--r--   0 scruz     (1000) scruz     (1000)      134 2023-05-27 17:52:04.000000 redgifs-1.7.0/tests/test_invalid_search.py
+-rw-r--r--   0 scruz     (1000) scruz     (1000)      465 2023-06-01 09:42:26.000000 redgifs-1.7.0/tests/test_result_attrs.py
+-rw-r--r--   0 scruz     (1000) scruz     (1000)      901 2023-05-31 11:09:33.000000 redgifs-1.7.0/tests/test_search.py
+-rw-r--r--   0 scruz     (1000) scruz     (1000)      561 2023-06-01 10:03:17.000000 redgifs-1.7.0/tests/test_tags.py
```

### Comparing `redgifs-1.6.1/LICENSE` & `redgifs-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `redgifs-1.6.1/PKG-INFO` & `redgifs-1.7.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,89 +1,93 @@
-Metadata-Version: 2.1
-Name: redgifs
-Version: 1.6.1
-Summary: Async and Sync Python Wrapper for the RedGIFs API.
-Home-page: https://github.com/scrazzz/redgifs
-Author: scrazzz
-License: MIT
-Project-URL: Documentation, https://redgifs.rtfd.io
-Project-URL: Issue tracker, https://github.com/scrazzz/redgifs/issues
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: test
-License-File: LICENSE
-
-<h1 align="center"> <code>redgifs</code> </h1>
-
-<div align="center">
-    <a href="https://pypi.org/project/redgifs">
-        <img src="https://img.shields.io/pypi/v/redgifs.svg" alt="pypi">
-    </a>
-    <a href="https://github.com/scrazzz/redgifs/actions/workflows/test.yml">
-        <img src="https://github.com/scrazzz/redgifs/actions/workflows/test.yml/badge.svg" alt="pytest">
-    </a>
-</div>
-
-<p align="center"> Async and Sync Python Wrapper for the RedGIFs API. </p>
-
------
-
-> ⭐ _Please star this repo to support the developer and to encourage the development of this project!_
-
------
-
-### Installation
-```
-pip install -U redgifs
-```
-
-#### Development version
-```
-pip install -U git+https://github.com/scrazzz/redgifs
-```
-
-`redgifs` works on Python versions 3.8 and above.
-
------
-
-### Quickstart
-Command Line usage:
-```console
-redgifs [url]
-```
-See `redgifs -h` for help.
-
-Synchronous usage:
-```py
-import redgifs
-
-api = redgifs.API()
-api.login() # Login with temporary token
-response = api.search('3D')
-print(response)
-api.close()
-```
-
-Asynchronous usage:
-```py
-import asyncio
-from redgifs.aio import API
-
-async def main():
-    api = API()
-    await api.login() # Login with teporary token
-    response = await api.search('3D')
-    print(response)
-    await api.close()
-
-loop = asyncio.get_event_loop()
-loop.run_until_complete(main())
-```
-
-More examples can be found in the examples directory.
-
------
-
-### Links
-- [Documentation](https://redgifs.readthedocs.io)
-- [Discord](https://discord.gg/yNsUTuXvzn)
+Metadata-Version: 2.1
+Name: redgifs
+Version: 1.7.0
+Summary: Async and Sync Python Wrapper for the RedGIFs API.
+Home-page: https://github.com/scrazzz/redgifs
+Author: scrazzz
+License: MIT
+Project-URL: Documentation, https://redgifs.rtfd.io
+Project-URL: Issue tracker, https://github.com/scrazzz/redgifs/issues
+Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown
+Provides-Extra: docs
+Provides-Extra: test
+License-File: LICENSE
+
+<!-- <h1 align="center"> <code>redgifs</code> </h1> -->
+
+<h1 align="center">
+    <img src="https://bigbits.eu.org/cdn/i/vyyv" alt="redgifspy-logo" width=200>
+</h1>
+
+<div align="center">
+    <a href="https://pypi.org/project/redgifs">
+        <img src="https://img.shields.io/pypi/v/redgifs.svg" alt="pypi">
+    </a>
+    <a href="https://github.com/scrazzz/redgifs/actions/workflows/test.yml">
+        <img src="https://github.com/scrazzz/redgifs/actions/workflows/test.yml/badge.svg" alt="pytest">
+    </a>
+</div>
+
+<p align="center"> Async and Sync Python Wrapper for the RedGIFs API. </p>
+
+-----
+
+> ⭐ _Please star this repo to support the developer and to encourage the development of this project!_
+
+-----
+
+### Installation
+```
+pip install -U redgifs
+```
+
+#### Development version
+```
+pip install -U git+https://github.com/scrazzz/redgifs
+```
+
+`redgifs` works on Python versions 3.8 and above.
+
+-----
+
+### Quickstart
+Command Line usage:
+```console
+redgifs [url]
+```
+See `redgifs -h` for help.
+
+Synchronous usage:
+```py
+import redgifs
+
+api = redgifs.API()
+api.login() # Login with temporary token
+response = api.search('3D')
+print(response)
+api.close()
+```
+
+Asynchronous usage:
+```py
+import asyncio
+from redgifs.aio import API
+
+async def main():
+    api = API()
+    await api.login() # Login with teporary token
+    response = await api.search('3D')
+    print(response)
+    await api.close()
+
+loop = asyncio.get_event_loop()
+loop.run_until_complete(main())
+```
+
+More examples can be found in the examples directory.
+
+-----
+
+### Links
+- [Documentation](https://redgifs.readthedocs.io)
+- [Discord](https://discord.gg/yNsUTuXvzn)
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: redgifs Version: 1.6.1 Summary: Async and Sync
+Metadata-Version: 2.1 Name: redgifs Version: 1.7.0 Summary: Async and Sync
 Python Wrapper for the RedGIFs API. Home-page: https://github.com/scrazzz/
 redgifs Author: scrazzz License: MIT Project-URL: Documentation, https://
 redgifs.rtfd.io Project-URL: Issue tracker, https://github.com/scrazzz/redgifs/
 issues Requires-Python: >=3.8.0 Description-Content-Type: text/markdown
 Provides-Extra: docs Provides-Extra: test License-File: LICENSE
-                             ****** redgifs ******
+                        ****** [redgifspy-logo] ******
                                 [pypi] [pytest]
               Async and Sync Python Wrapper for the RedGIFs API.
 ----- > â­ _Please star this repo to support the developer and to encourage
 the development of this project!_ ----- ### Installation ``` pip install -
 U redgifs ``` #### Development version ``` pip install -U git+https://
 github.com/scrazzz/redgifs ``` `redgifs` works on Python versions 3.8 and
 above. ----- ### Quickstart Command Line usage: ```console redgifs [url] ```
```

### Comparing `redgifs-1.6.1/README.md` & `redgifs-1.7.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-<h1 align="center"> <code>redgifs</code> </h1>
+<!-- <h1 align="center"> <code>redgifs</code> </h1> -->
+
+<h1 align="center">
+    <img src="https://bigbits.eu.org/cdn/i/vyyv" alt="redgifspy-logo" width=200>
+</h1>
 
 <div align="center">
     <a href="https://pypi.org/project/redgifs">
         <img src="https://img.shields.io/pypi/v/redgifs.svg" alt="pypi">
     </a>
     <a href="https://github.com/scrazzz/redgifs/actions/workflows/test.yml">
         <img src="https://github.com/scrazzz/redgifs/actions/workflows/test.yml/badge.svg" alt="pytest">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-                             ****** redgifs ******
+                        ****** [redgifspy-logo] ******
                                 [pypi] [pytest]
               Async and Sync Python Wrapper for the RedGIFs API.
 ----- > â­ _Please star this repo to support the developer and to encourage
 the development of this project!_ ----- ### Installation ``` pip install -
 U redgifs ``` #### Development version ``` pip install -U git+https://
 github.com/scrazzz/redgifs ``` `redgifs` works on Python versions 3.8 and
 above. ----- ### Quickstart Command Line usage: ```console redgifs [url] ```
```

### Comparing `redgifs-1.6.1/redgifs/__init__.py` & `redgifs-1.7.0/redgifs/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,25 +22,26 @@
 DEALINGS IN THE SOFTWARE.
 """
 
 __title__ = 'redgifs'
 __author__ = 'scrazzz'
 __license__ = 'MIT'
 __copyright__ = 'Copyright (c) 2022-present scrazzz'
-__version__ = '1.6.1'
+__version__ = '1.7.0'
 
 from typing import Literal, NamedTuple
 
 from .api import API
 from .http import ProxyAuth
-from .enums import Order, Tags
+from .enums import Order
+from .tags import Tags
 from .errors import *
 
 class VersionInfo(NamedTuple):
     major: int
     minor: int
     micro: int
     releaselevel: Literal['alpha', 'beta', 'final']
 
-version_info: VersionInfo = VersionInfo(major=1, minor=6, micro=1, releaselevel='final')
+version_info: VersionInfo = VersionInfo(major=1, minor=7, micro=0, releaselevel='final')
 
 del NamedTuple, VersionInfo
```

### Comparing `redgifs-1.6.1/redgifs/__main__.py` & `redgifs-1.7.0/redgifs/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,16 @@
         gif = get_quality(quality, gif)
         filename = f'{gif.split("/")[3].split(".")[0]}.mp4'
         print(f'Downloading {id}...')
         if folder:
             client.download(gif, f'{folder}/{filename}')
         else:
             client.download(gif, f'{filename}')
+        print('Download complete.\n')
+        exit(0)
 
     # Handle /users/ URLs (eg: https://redgifs.com/users/redgifs)
     if '/users/' in yarl_url.path:
         match = re.match(USERNAME_RE, str(yarl_url))
         if not match:
             raise TypeError(f'Not a valid /users/ URL: {yarl_url}')
         user = match.groupdict()['username']
```

### Comparing `redgifs-1.6.1/redgifs/aio.py` & `redgifs-1.7.0/redgifs/aio.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,28 +27,30 @@
 import io
 import os
 from typing import Any, Dict, List, Optional, Union
 
 import aiohttp
 
 from .http import AsyncHttp, ProxyAuth
-from .enums import Tags, Order
-from .utils import _to_web_url
+from .tags import Tags
+from .enums import Order
+from .utils import _to_web_url, _async_read_tags_json
 from .parser import parse_search, parse_creator, parse_creators, parse_search_image
 from .models import GIF, URL, CreatorResult, SearchResult, CreatorsResult
 
 class API:
     def __init__(
         self,
         session: Optional[aiohttp.ClientSession] = None,
         *,
         proxy: Optional[str] = None,
         proxy_auth: Optional[ProxyAuth] = None
     ) -> None:
         self.http: AsyncHttp = AsyncHttp(session, proxy=proxy, proxy_auth=proxy_auth)
+        self._tags = Tags()
 
     async def login(self, username: Optional[str] = None, password: Optional[str] = None) -> bool:
         return (await self.http.login(username, password))
 
     async def get_tags(self) -> List[Dict[str, Union[str, int]]]:
         resp = await self.http.get_tags()
         return resp['tags']
@@ -84,31 +86,39 @@
         result = (await self.http.get_trending_tags())['tags']
         return result
 
     async def fetch_tag_suggestions(self, query: str) -> List[str]:
         result = await self.http.get_tag_suggestions(query)
         return [d['text'] for d in result]
 
-    async def search(self, search_text: Union[str, Tags], *, order: Order = Order.trending, count: int = 80, page: int = 1) -> SearchResult:
-        if isinstance(search_text, str):
-            st = Tags.search(search_text)[0]
-        elif isinstance(search_text, Tags):
-            st = search_text.value
+    async def search(
+        self,
+        search_text: str,
+        *,
+        order: Order = Order.trending,
+        count: int = 80,
+        page: int = 1
+    ) -> SearchResult:
+        if len(self._tags.tags_mapping) == 0:
+            tags = await _async_read_tags_json()
+            self._tags._set(tags)
+
+        st = self._tags.search(search_text)[0]
         resp = await self.http.search(st, order, count, page)
         return parse_search(st, resp)
 
     search_gif = search
 
     async def search_creators(
         self,
         *,
         page: int = 1,
         order: Order = Order.recent,
         verified: bool = False,
-        tags: Optional[Union[List[Tags], List[str]]] = None
+        tags: Optional[List[str]] = None
     ) -> CreatorsResult:
         resp = await self.http.search_creators(page=page, order=order, verified=verified, tags=tags)
         return parse_creators(resp)
 
     async def search_creator(
         self,
         username: str,
@@ -120,27 +130,23 @@
         resp = await self.http.search_creator(username=username, page=page, count=count, order=order)
         return parse_creator(resp)
 
     search_user = search_creator
 
     async def search_image(
         self,
-        search_text: Union[str, Tags],
+        search_text: str,
         *,
-        order: Order = Order.trending,
+        order: Order = Order.new,
         count: int = 80,
         page: int = 1
     ) -> SearchResult:
-        if isinstance(search_text, str):
-            # We are not going to use Tags.search() here because it doesn't matter
-            # whatever the search_text is, this API endpoints provides images nonetheless.
-            st = search_text
-        elif isinstance(search_text, Tags):
-            st = search_text.value
-        resp = await self.http.search_image(st, order, count, page)
-        return parse_search_image(st, resp)
+        # We are not going to use Tags.search() here because it doesn't matter
+        # whatever the search_text is, this API endpoints provides images nonetheless.
+        resp = await self.http.search_image(search_text, order, count, page)
+        return parse_search_image(search_text, resp)
 
     async def download(self, url: str, fp: Union[str, bytes, os.PathLike[Any], io.BufferedIOBase]) -> int:
         return (await self.http.download(url, fp))
 
     async def close(self) -> None:
         return (await self.http.close())
```

### Comparing `redgifs-1.6.1/redgifs/api.py` & `redgifs-1.7.0/redgifs/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,17 +26,18 @@
 
 import io
 import os
 from typing import Any, Dict, List, Optional, Union
 
 import requests
 
+from .tags import Tags
+from .enums import Order
 from .http import HTTP, ProxyAuth
-from .enums import Order, Tags
-from .utils import _to_web_url
+from .utils import _to_web_url, _read_tags_json
 from .parser import parse_creator, parse_search, parse_creators, parse_search_image
 from .models import URL, GIF, CreatorResult, SearchResult, CreatorsResult
 
 class API:
     """The API Instance to get information from the RedGifs API.
 
     .. note::
@@ -61,14 +62,15 @@
         self,
         session: Optional[requests.Session] = None,
         *,
         proxy: Optional[str] = None,
         proxy_auth: Optional[ProxyAuth] = None
     ) -> None:
         self.http: HTTP = HTTP(session, proxy=proxy, proxy_auth=proxy_auth)
+        self._tags = Tags()
 
     def login(self, username: Optional[str] = None, password: Optional[str] = None) -> bool:
         return self.http.login(username, password)
 
     def get_tags(self) -> List[Dict[str, Union[str, int]]]:
         """Get all available RedGifs Tags.
         
@@ -142,16 +144,16 @@
         return resp
 
     def fetch_tag_suggestions(self, query: str) -> List[str]:
         """Get tag suggestions from RedGifs.
 
         .. note::
 
-            This is an API call. See :func:`~redgifs.Tags.search` for an internal lookup
-            of available tags.
+            This is an API call. See :func:`Tags.search() <redgifs.Tags.search()>` for an internal lookup
+            of all available tags.
 
         Parameters
         ----------
         query: :class:`str`
             The tag name to look for.
 
         Returns
@@ -160,68 +162,68 @@
             A list of tag names.
         """
         result = self.http.get_tag_suggestions(query)
         return [d['text'] for d in result]
 
     def search(
         self,
-        search_text: Union[str, Tags],
+        search_text: str,
         *,
         order: Order = Order.trending,
         count: int = 80,
         page: int = 1
     ) -> SearchResult:
         """
         Search for a GIF.
 
         Parameters
         ----------
-        search_text: Union[:class:`str`, :class:`Tags`]
+        search_text: :class:`str`
             The GIFs to search for. Can be a string or an instance of :class:`Tags`.
         order: Optional[:class:`Order`]
             The order of the GIFs to return.
         count: Optional[:class:`int`]
             The amount of GIFs to return.
         page: Optional[:class:`int`]
             The page number of the GIFs to return.
 
         Returns
         -------
         :py:class:`SearchResult <redgifs.models.SearchResult>` - The search result.
         """
+        if len(self._tags.tags_mapping) == 0:
+            tags = _read_tags_json()
+            self._tags._set(tags)
 
-        if isinstance(search_text, str):
-            st = Tags.search(search_text)[0]
-        elif isinstance(search_text, Tags):
-            st = search_text.value
+        st = self._tags.search(search_text)[0]
         resp = self.http.search(st, order, count, page)
         return parse_search(st, resp)
 
     search_gif = search
 
     def search_creators(
         self,
         *,
         page: int = 1,
         order: Order = Order.recent,
         verified: bool = False,
-        tags: Optional[Union[List[Tags], List[str]]] = None
+        tags: Optional[List[str]] = None
     ) -> CreatorsResult:
         """
         Search for RedGifs Creators.
 
         Parameters
         ----------
         page: Optional[:class:`int`]
             The number of page to return.
         order: Optional[:class:`Order`]
             The order of the creators to return.
         verified: Optional[:class:`bool`]
             Wheather to only return verified creators.
-        tags: Optional[Union[List[:class:`Tags`], List[:class:`str`]]]
+        tags: Optional[List[:class:`str`]]
             A list of tags to look for.
             Narrows down the results to content creators that have contents with all the given tags.
 
         Returns
         -------
         :py:class:`CreatorsResult <redgifs.models.CreatorsResult>` - The search result.
         """
@@ -250,46 +252,42 @@
         resp = self.http.search_creator(username, page=page, count=count, order=order)
         return parse_creator(resp)
 
     search_user = search_creator
 
     def search_image(
         self,
-        search_text: Union[str, Tags],
+        search_text: str,
         *,
-        order: Order = Order.trending,
+        order: Order = Order.new,
         count: int = 80,
         page: int = 1
     ) -> SearchResult:
         """
         Search for images on Redgifs.
 
         Parameters
         ----------
-        search_text: Union[:class:`str`, :class:`Tags`]
+        search_text: :class:`str`
             The images to search for. Can be a string or an instance of :class:`Tags`.
         order: Optional[:class:`Order`]
             The order of the images to return.
         count: Optional[:class:`int`]
             The amount of images to return.
         page: Optional[:class:`int`]
             The page number of the images to return.
 
         Returns
         -------
         :py:class:`SearchResult <redgifs.models.SearchResult>` - The search result.
         """
-        if isinstance(search_text, str):
-            # We are not going to use Tags.search() here because it doesn't matter
-            # whatever the search_text is, this API endpoints provides images nonetheless.
-            st = search_text
-        elif isinstance(search_text, Tags):
-            st = search_text.value
-        resp = self.http.search_image(st, order, count, page)
-        return parse_search_image(st, resp)
+        # We are not going to use Tags.search() here because it doesn't matter
+        # whatever the search_text is, this API endpoints provides images nonetheless.
+        resp = self.http.search_image(search_text, order, count, page)
+        return parse_search_image(search_text, resp)
 
     def download(self, url: str, fp: Union[str, bytes, os.PathLike[Any], io.BufferedIOBase]):
         """
         A friendly method to download a RedGifs media.
 
         Example:
```

### Comparing `redgifs-1.6.1/redgifs/const.py` & `redgifs-1.7.0/redgifs/const.py`

 * *Files identical despite different names*

### Comparing `redgifs-1.6.1/redgifs/errors.py` & `redgifs-1.7.0/redgifs/errors.py`

 * *Files identical despite different names*

### Comparing `redgifs-1.6.1/redgifs/http.py` & `redgifs-1.7.0/redgifs/http.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 import requests
 import aiohttp
 import yarl
 
 from . import __version__
 from .errors import HTTPException
-from .enums import Tags, Order
+from .enums import Order
 from .const import REDGIFS_THUMBS_RE
 from .utils import strip_ip
 
 _log = logging.getLogger(__name__)
 
 class Route:
     BASE: ClassVar[str] = "https://api.redgifs.com"
@@ -130,40 +130,40 @@
 
     def get_tags(self, **params: Any):
         return self.request(Route('GET', '/v1/tags'), **params)
 
     def get_gif(self, id: str, **params: Any):
         return self.request(Route('GET', '/v2/gifs/{id}', id=id), **params)
 
-    def search(self, search_text: Union[str, Tags], order: Order, count: int, page: int, **params: Any):
+    def search(self, search_text: str, order: Order, count: int, page: int, **params: Any):
         r = Route(
             'GET', '/v2/gifs/search?search_text={search_text}&order={order}&count={count}&page={page}',
             search_text=search_text, order=order.value, count=count, page=page
         )
         return self.request(r, **params)
     
     # User/Creator methods
 
     def search_creators(
         self,
         page: int,
         order: Order,
         verified: bool,
-        tags: Optional[Union[List[Tags], List[str]]],
+        tags: Optional[List[str]],
         **params: Any
     ):
         url = '/v1/creators/search?page={page}&order={order}'
         if verified:
             url += '&verified={verified}'
         if tags:
             url += '&tags={tags}'
             r = Route(
                 'GET', url,
                 page=page, order=order.value, verified='y' if verified else 'n',
-                tags=','.join(t.value for t in tags) if isinstance(tags[0], Tags) else ','.join(t for t in tags) # type: ignore
+                tags=','.join(t for t in tags)
             )
             return self.request(r, **params)
         else:
             r = Route(
                 'GET', url,
                 page=page, order=order.value, verified='y' if verified else 'n'
             )
@@ -174,15 +174,15 @@
             'GET', '/v2/users/{username}/search?page={page}&count={count}&order={order}',
             username=username, page=page, count=count, order=order.value
         )
         return self.request(r, **params)
 
     # Pic methods
 
-    def search_image(self, search_text: Union[str, Tags], order: Order, count: int, page: int, **params: Any):
+    def search_image(self, search_text: str, order: Order, count: int, page: int, **params: Any):
         r = Route(
             'GET', '/v2/gifs/search?search_text={search_text}&order={order}&count={count}&page={page}&type=i',
             search_text=search_text, order=order.value, count=count, page=page
         )
         return self.request(r, **params)
 
     # Tag methods
```

### Comparing `redgifs-1.6.1/redgifs/models.py` & `redgifs-1.7.0/redgifs/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,15 +246,15 @@
     poster: Optional[str]
     preview: Optional[str]
     thumbnail: Optional[str]
 
 @dataclass
 class SearchResult:
     # TODO: Document "users"
-    """The result you have searched. This is returned in :py:meth:`search() <redgifs.API.search()>`.
+    """The result you have searched. This is returned in :py:meth:`API.search() <redgifs.API.search()>`.
 
     Attributes
     ----------
     searched_for: :class:`str`
         The result of what you have searched for.
         This may differ from what you have provided for ``query`` in :py:meth:`API.search() <redgifs.API.search()>`.
     page: :class:`int`
```

### Comparing `redgifs-1.6.1/redgifs/parser.py` & `redgifs-1.7.0/redgifs/parser.py`

 * *Files identical despite different names*

### Comparing `redgifs-1.6.1/redgifs/utils.py` & `redgifs-1.7.0/redgifs/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,19 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 import re
+import json
+import pkgutil
+import asyncio
+from typing import Dict
+
 import yarl
 
 from .const import REDGIFS_THUMBS_RE
 
 def _to_web_url(id_or_url: str, use_regex: bool = False) -> str:
     if not use_regex:
         return f'https://redgifs.com/watch/{id_or_url.lower()}'
@@ -40,9 +45,17 @@
         return f'https://redgifs.com/watch/{id.lower()}'
     except IndexError:
         return ''
 
 def strip_ip(url: str) -> str:
     u = yarl.URL(url)
     if u.query.get('for'):
-        return u % {'for': 'REDACTED'}
+        return str(u % {'for': 'REDACTED'})
     return url
+
+def _read_tags_json() -> Dict[str, str]:
+    file_ = pkgutil.get_data(__name__, 'tags.json') # type: ignore - We know this won't be None
+    return json.loads(file_) # type: ignore - same reason above
+
+async def _async_read_tags_json() -> Dict[str, str]:
+    r = await asyncio.get_event_loop().run_in_executor(None, _read_tags_json)
+    return r
```

### Comparing `redgifs-1.6.1/redgifs.egg-info/PKG-INFO` & `redgifs-1.7.0/redgifs.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,89 +1,93 @@
-Metadata-Version: 2.1
-Name: redgifs
-Version: 1.6.1
-Summary: Async and Sync Python Wrapper for the RedGIFs API.
-Home-page: https://github.com/scrazzz/redgifs
-Author: scrazzz
-License: MIT
-Project-URL: Documentation, https://redgifs.rtfd.io
-Project-URL: Issue tracker, https://github.com/scrazzz/redgifs/issues
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: test
-License-File: LICENSE
-
-<h1 align="center"> <code>redgifs</code> </h1>
-
-<div align="center">
-    <a href="https://pypi.org/project/redgifs">
-        <img src="https://img.shields.io/pypi/v/redgifs.svg" alt="pypi">
-    </a>
-    <a href="https://github.com/scrazzz/redgifs/actions/workflows/test.yml">
-        <img src="https://github.com/scrazzz/redgifs/actions/workflows/test.yml/badge.svg" alt="pytest">
-    </a>
-</div>
-
-<p align="center"> Async and Sync Python Wrapper for the RedGIFs API. </p>
-
------
-
-> ⭐ _Please star this repo to support the developer and to encourage the development of this project!_
-
------
-
-### Installation
-```
-pip install -U redgifs
-```
-
-#### Development version
-```
-pip install -U git+https://github.com/scrazzz/redgifs
-```
-
-`redgifs` works on Python versions 3.8 and above.
-
------
-
-### Quickstart
-Command Line usage:
-```console
-redgifs [url]
-```
-See `redgifs -h` for help.
-
-Synchronous usage:
-```py
-import redgifs
-
-api = redgifs.API()
-api.login() # Login with temporary token
-response = api.search('3D')
-print(response)
-api.close()
-```
-
-Asynchronous usage:
-```py
-import asyncio
-from redgifs.aio import API
-
-async def main():
-    api = API()
-    await api.login() # Login with teporary token
-    response = await api.search('3D')
-    print(response)
-    await api.close()
-
-loop = asyncio.get_event_loop()
-loop.run_until_complete(main())
-```
-
-More examples can be found in the examples directory.
-
------
-
-### Links
-- [Documentation](https://redgifs.readthedocs.io)
-- [Discord](https://discord.gg/yNsUTuXvzn)
+Metadata-Version: 2.1
+Name: redgifs
+Version: 1.7.0
+Summary: Async and Sync Python Wrapper for the RedGIFs API.
+Home-page: https://github.com/scrazzz/redgifs
+Author: scrazzz
+License: MIT
+Project-URL: Documentation, https://redgifs.rtfd.io
+Project-URL: Issue tracker, https://github.com/scrazzz/redgifs/issues
+Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown
+Provides-Extra: docs
+Provides-Extra: test
+License-File: LICENSE
+
+<!-- <h1 align="center"> <code>redgifs</code> </h1> -->
+
+<h1 align="center">
+    <img src="https://bigbits.eu.org/cdn/i/vyyv" alt="redgifspy-logo" width=200>
+</h1>
+
+<div align="center">
+    <a href="https://pypi.org/project/redgifs">
+        <img src="https://img.shields.io/pypi/v/redgifs.svg" alt="pypi">
+    </a>
+    <a href="https://github.com/scrazzz/redgifs/actions/workflows/test.yml">
+        <img src="https://github.com/scrazzz/redgifs/actions/workflows/test.yml/badge.svg" alt="pytest">
+    </a>
+</div>
+
+<p align="center"> Async and Sync Python Wrapper for the RedGIFs API. </p>
+
+-----
+
+> ⭐ _Please star this repo to support the developer and to encourage the development of this project!_
+
+-----
+
+### Installation
+```
+pip install -U redgifs
+```
+
+#### Development version
+```
+pip install -U git+https://github.com/scrazzz/redgifs
+```
+
+`redgifs` works on Python versions 3.8 and above.
+
+-----
+
+### Quickstart
+Command Line usage:
+```console
+redgifs [url]
+```
+See `redgifs -h` for help.
+
+Synchronous usage:
+```py
+import redgifs
+
+api = redgifs.API()
+api.login() # Login with temporary token
+response = api.search('3D')
+print(response)
+api.close()
+```
+
+Asynchronous usage:
+```py
+import asyncio
+from redgifs.aio import API
+
+async def main():
+    api = API()
+    await api.login() # Login with teporary token
+    response = await api.search('3D')
+    print(response)
+    await api.close()
+
+loop = asyncio.get_event_loop()
+loop.run_until_complete(main())
+```
+
+More examples can be found in the examples directory.
+
+-----
+
+### Links
+- [Documentation](https://redgifs.readthedocs.io)
+- [Discord](https://discord.gg/yNsUTuXvzn)
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: redgifs Version: 1.6.1 Summary: Async and Sync
+Metadata-Version: 2.1 Name: redgifs Version: 1.7.0 Summary: Async and Sync
 Python Wrapper for the RedGIFs API. Home-page: https://github.com/scrazzz/
 redgifs Author: scrazzz License: MIT Project-URL: Documentation, https://
 redgifs.rtfd.io Project-URL: Issue tracker, https://github.com/scrazzz/redgifs/
 issues Requires-Python: >=3.8.0 Description-Content-Type: text/markdown
 Provides-Extra: docs Provides-Extra: test License-File: LICENSE
-                             ****** redgifs ******
+                        ****** [redgifspy-logo] ******
                                 [pypi] [pytest]
               Async and Sync Python Wrapper for the RedGIFs API.
 ----- > â­ _Please star this repo to support the developer and to encourage
 the development of this project!_ ----- ### Installation ``` pip install -
 U redgifs ``` #### Development version ``` pip install -U git+https://
 github.com/scrazzz/redgifs ``` `redgifs` works on Python versions 3.8 and
 above. ----- ### Quickstart Command Line usage: ```console redgifs [url] ```
```

### Comparing `redgifs-1.6.1/redgifs.egg-info/SOURCES.txt` & `redgifs-1.7.0/redgifs.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -9,18 +9,21 @@
 redgifs/api.py
 redgifs/const.py
 redgifs/enums.py
 redgifs/errors.py
 redgifs/http.py
 redgifs/models.py
 redgifs/parser.py
+redgifs/tags.json
+redgifs/tags.py
 redgifs/utils.py
 redgifs.egg-info/PKG-INFO
 redgifs.egg-info/SOURCES.txt
 redgifs.egg-info/dependency_links.txt
 redgifs.egg-info/entry_points.txt
 redgifs.egg-info/requires.txt
 redgifs.egg-info/top_level.txt
+tests/test_images.py
 tests/test_invalid_search.py
 tests/test_result_attrs.py
 tests/test_search.py
 tests/test_tags.py
```

### Comparing `redgifs-1.6.1/setup.py` & `redgifs-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 extras_require = {
     'docs': [
         'Sphinx==4.4.0',
         'furo==2022.2.23'
     ],
     'test': [
-        'pytest==7.1.1'
+        'pytest==7.3.1'
     ],
 }
 
 setup(
     name='redgifs',
     author='scrazzz',
     url='https://github.com/scrazzz/redgifs',
```

### Comparing `redgifs-1.6.1/tests/test_search.py` & `redgifs-1.7.0/tests/test_search.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 @pytest.mark.parametrize(
     "count, expected_count",
     [ (10, 10), (20, 20), (40, 40) ]
 )
 def test_search_with_count(count, expected_count):
     result = api.search('hitomi tanaka', count=count)
-    assert len(result.gifs) == expected_count
+    assert result.gifs is not None and len(result.gifs) == expected_count
 
 
 @pytest.mark.parametrize(
     "page, expected_page",
     [ (2, 2), (3, 3), (6, 6) ]
 )
 def test_search_with_page(page, expected_page):
```

