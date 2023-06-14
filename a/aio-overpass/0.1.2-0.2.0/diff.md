# Comparing `tmp/aio_overpass-0.1.2.tar.gz` & `tmp/aio_overpass-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_overpass-0.1.2.tar", max compression
+gzip compressed data, was "aio_overpass-0.2.0.tar", max compression
```

## Comparing `aio_overpass-0.1.2.tar` & `aio_overpass-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1069 2023-04-27 20:33:46.735549 aio_overpass-0.1.2/LICENSE
--rw-r--r--   0        0        0     8007 2023-04-27 20:33:46.735549 aio_overpass-0.1.2/README.md
--rwxr-xr-x   0        0        0      316 2023-04-27 20:33:46.735549 aio_overpass-0.1.2/aio_overpass/__init__.py
--rw-r--r--   0        0        0      977 2023-04-27 20:33:46.735549 aio_overpass-0.1.2/aio_overpass/_dist.py
--rwxr-xr-x   0        0        0      971 2023-04-27 20:33:46.735549 aio_overpass-0.1.2/aio_overpass/_ql.py
--rwxr-xr-x   0        0        0    11056 2023-04-27 20:33:46.735549 aio_overpass-0.1.2/aio_overpass/client.py
--rwxr-xr-x   0        0        0    28078 2023-04-27 20:33:46.735549 aio_overpass-0.1.2/aio_overpass/element.py
--rwxr-xr-x   0        0        0    14075 2023-04-27 20:33:46.739549 aio_overpass-0.1.2/aio_overpass/error.py
--rwxr-xr-x   0        0        0    24584 2023-04-27 20:33:46.739549 aio_overpass-0.1.2/aio_overpass/pt.py
--rwxr-xr-x   0        0        0    22350 2023-04-27 20:33:46.739549 aio_overpass-0.1.2/aio_overpass/pt_ordered.py
--rwxr-xr-x   0        0        0    14363 2023-04-27 20:33:46.739549 aio_overpass-0.1.2/aio_overpass/query.py
--rwxr-xr-x   0        0        0     2160 2023-04-27 20:33:46.739549 aio_overpass-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     9323 1970-01-01 00:00:00.000000 aio_overpass-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1536 2023-06-14 14:22:08.796390 aio_overpass-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1069 2023-06-14 14:22:08.796390 aio_overpass-0.2.0/LICENSE
+-rw-r--r--   0        0        0     8085 2023-06-14 14:22:08.796390 aio_overpass-0.2.0/README.md
+-rwxr-xr-x   0        0        0      316 2023-06-14 14:22:08.796390 aio_overpass-0.2.0/aio_overpass/__init__.py
+-rw-r--r--   0        0        0      977 2023-06-14 14:22:08.796390 aio_overpass-0.2.0/aio_overpass/_dist.py
+-rwxr-xr-x   0        0        0      971 2023-06-14 14:22:08.796390 aio_overpass-0.2.0/aio_overpass/_ql.py
+-rwxr-xr-x   0        0        0    12078 2023-06-14 14:22:08.796390 aio_overpass-0.2.0/aio_overpass/client.py
+-rwxr-xr-x   0        0        0    28970 2023-06-14 14:22:08.796390 aio_overpass-0.2.0/aio_overpass/element.py
+-rwxr-xr-x   0        0        0    14083 2023-06-14 14:22:08.796390 aio_overpass-0.2.0/aio_overpass/error.py
+-rwxr-xr-x   0        0        0    25071 2023-06-14 14:22:08.796390 aio_overpass-0.2.0/aio_overpass/pt.py
+-rwxr-xr-x   0        0        0    22491 2023-06-14 14:22:08.796390 aio_overpass-0.2.0/aio_overpass/pt_ordered.py
+-rwxr-xr-x   0        0        0    14772 2023-06-14 14:22:08.796390 aio_overpass-0.2.0/aio_overpass/query.py
+-rwxr-xr-x   0        0        0     2614 2023-06-14 14:22:08.796390 aio_overpass-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     9466 1970-01-01 00:00:00.000000 aio_overpass-0.2.0/PKG-INFO
```

### Comparing `aio_overpass-0.1.2/LICENSE` & `aio_overpass-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aio_overpass-0.1.2/README.md` & `aio_overpass-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 - [Motivation](#motivation)
 - [Related Projects](#related-projects)
 - [License](#license)
 
 #### See also
 - An overview of modules, classes and functions can be found in the [API reference](http://www.timwie.dev/aio-overpass/).
 - The version history is available in [CHANGELOG.md](https://github.com/timwie/aio-overpass/blob/main/CHANGELOG.md).
-- Contributor guide is forthcoming :construction:
+- Developers can find some instructions in [CONTRIBUTING.md](https://github.com/timwie/aio-overpass/blob/main/CONTRIBUTING.md).
 
 <br>
 
 ## Features
 - Asynchronous requests using [aiohttp]
 - Concurrent queries
 - Respects rate limits
```

### Comparing `aio_overpass-0.1.2/aio_overpass/_dist.py` & `aio_overpass-0.2.0/aio_overpass/_dist.py`

 * *Files identical despite different names*

### Comparing `aio_overpass-0.1.2/aio_overpass/_ql.py` & `aio_overpass-0.2.0/aio_overpass/_ql.py`

 * *Files identical despite different names*

### Comparing `aio_overpass-0.1.2/aio_overpass/client.py` & `aio_overpass-0.2.0/aio_overpass/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 from urllib.parse import urljoin
 
 from aio_overpass import __version__
 from aio_overpass.error import (
     CallError,
     ClientError,
     GiveupError,
-    QueryRejectCause,
-    QueryRejectError,
     RunnerError,
     _result_or_raise,
     _to_client_error,
 )
 from aio_overpass.query import DefaultQueryRunner, Query, QueryRunner
 
 import aiohttp
@@ -32,41 +30,42 @@
     "DEFAULT_USER_AGENT",
 )
 
 
 DEFAULT_INSTANCE = "https://overpass-api.de/api/"
 DEFAULT_USER_AGENT = f"aio-overpass/{__version__} (https://github.com/timwie/aio-overpass)"
 
-# TODO document and expose this limit in Status
-_DEFAULT_SLOTS = 32
-
 
 @dataclass
 class Status:
     """
     Information about the API server's rate limit.
 
     Attributes:
         slots: The maximum number of concurrent queries per IP
                (or ``None`` if there is no rate limit).
         free_slots: The number of slots open for this IP
                     (or ``None`` if there is no rate limit).
         cooldown_secs: The number of seconds until a slot opens for this IP
                        (or 0 if there is a free slot).
+        concurrency: Maximum concurrent queries configured for this client.
     """
 
     slots: Optional[int]
     free_slots: Optional[int]
     cooldown_secs: int
+    concurrency: int
 
     def __repr__(self) -> str:
+        f, s, c = self.free_slots, self.slots, self.cooldown_secs
+
         if self.slots:
-            return f"{type(self).__name__}(slots={self.free_slots}/{self.slots}, cooldown={self.cooldown_secs}s)"
+            return f"{type(self).__name__}(slots={f}/{s}, cooldown={c}s)"
 
-        return f"{type(self).__name__}(slots=∞, cooldown={self.cooldown_secs}s)"
+        return f"{type(self).__name__}(slots=∞, cooldown={c}s)"
 
 
 class Client:
     """
     A client for the Overpass API.
 
     Requests are rate-limited according to the configured number of slots per IP for the specified
@@ -75,33 +74,43 @@
 
     Args:
         url: The url of an Overpass API instance. Defaults to the main Overpass API instance.
         user_agent: A string used for the User-Agent header. It is good practice to provide a string
                     that identifies your application, and includes a way to contact you (f.e. an
                     e-mail, or a link to a repository). This is important if you make too many
                     requests, or queries that require a lot of resources.
+        concurrency: Affects the maximum number of concurrent queries. Usually, the API server
+                     status includes a number of slots it provides for each IP. If that is the
+                     case, we pick the minimum of that number of slots and ``concurrency`` as
+                     concurrency limit. If the server does not provide a limit itself,
+                     ``concurrency`` will be used as concurrency limit.
         runner: You can provide another query runner if you want to implement your own retry
                 strategy.
 
     References:
         - https://wiki.openstreetmap.org/wiki/Overpass_API#Public_Overpass_API_instances
     """
 
     def __init__(
         self,
         url: str = DEFAULT_INSTANCE,
         user_agent: str = DEFAULT_USER_AGENT,
-        runner: QueryRunner = None,
+        concurrency: int = 32,
+        runner: Optional[QueryRunner] = None,
     ) -> None:
+        if concurrency <= 0:
+            raise ValueError("'concurrency' must be > 0")
+
         self._url = url
         self._user_agent = user_agent
+        self._concurrency = concurrency
         self._runner = runner or DefaultQueryRunner()
 
-        self._maybe_session = None
-        self._maybe_sem = None
+        self._maybe_session: Optional[aiohttp.ClientSession] = None
+        self._maybe_sem: Optional[asyncio.BoundedSemaphore] = None
 
     def _session(self) -> aiohttp.ClientSession:
         """The session used for all requests of this client."""
         if not self._maybe_session or self._maybe_session.closed:
             headers = {"User-Agent": self._user_agent}
             self._maybe_session = aiohttp.ClientSession(headers=headers)
 
@@ -114,18 +123,17 @@
         This semaphore can be acquired as many times as there are query slots at the API instance.
         If all slots are acquired, further queries need to wait until a slot is released.
         """
         if self._maybe_sem:
             return self._maybe_sem
 
         session = self._session()
-
         status = await self._status(session, **kwargs)
+        self._maybe_sem = asyncio.BoundedSemaphore(status.concurrency)
 
-        self._maybe_sem = asyncio.BoundedSemaphore(status.slots or _DEFAULT_SLOTS)
         return self._maybe_sem
 
     async def close(self) -> None:
         """Cancel all running queries and close the underlying session."""
         if self._maybe_session and not self._maybe_session.closed:
             try:
                 _ = await self.cancel_queries()
@@ -138,44 +146,55 @@
                 pass  # is raised when there are still active queries. that's ok
 
     async def _status(self, session: aiohttp.ClientSession, **kwargs) -> "Status":
         try:
             async with session.get(url=urljoin(self._url, "status"), **kwargs) as response:
                 text = await response.text()
         except aiohttp.ClientError as err:
-            raise _to_client_error(err)
+            raise _to_client_error(err) from err
 
         try:
             match_slots_overall = re.findall("Rate limit: (\\d+)", text)
             match_slots_available = re.findall("(\\d+) slots available now", text)
             match_cooldowns = re.findall("Slot available after: .+, in (\\d+) seconds", text)
 
             (slots,) = match_slots_overall
             slots = int(slots) or None
-            free_slots = None
-            cooldown_secs = 0
 
             if slots:
                 cooldowns = [int(secs) for secs in match_cooldowns]
 
                 if match_slots_available:
                     free_slots = int(match_slots_available[0])
                 else:
                     free_slots = slots - len(cooldowns)
 
                 cooldown_secs = 0 if free_slots > 0 else min(cooldowns)
+
+                # pick the server's concurrent query limit if > 0 and < self._concurrency,
+                # or self._concurrency otherwise
+                concurrency = min(slots or self._concurrency, self._concurrency)
+
+                return Status(
+                    slots=slots,
+                    free_slots=free_slots,
+                    cooldown_secs=cooldown_secs,
+                    concurrency=concurrency,
+                )
+
+            return Status(
+                slots=slots,
+                free_slots=None,
+                cooldown_secs=0,
+                concurrency=self._concurrency,
+            )
+
         except ValueError as err:
             raise _to_client_error(response) from err
 
-        return Status(
-            slots=slots,
-            free_slots=free_slots,
-            cooldown_secs=cooldown_secs,
-        )
-
     async def status(self) -> Status:
         """
         Check the current API status.
 
         Raises:
             ClientError: if the status could not be looked up
         """
@@ -198,15 +217,15 @@
         endpoint = urljoin(self._url, "kill_my_queries")
         try:
             async with session.get(endpoint) as response:
                 body = await response.text()
                 killed_pids = re.findall("\\(pid (\\d+)\\)", body)
                 return len(set(killed_pids))
         except aiohttp.ClientError as err:
-            raise _to_client_error(err)
+            raise _to_client_error(err) from err
 
     async def run_query(self, query: Query) -> None:
         """
         Send a query to the API, and await its completion.
 
         "Running" the query entails acquiring a connection from the pool, waiting for a slot
         to open up, the query requests themselves (which may be retried), status requests
@@ -224,57 +243,54 @@
         """
         if query.done:
             return  # nothing to do
 
         if query.nb_tries > 0:
             query.reset()  # reset failed queries
 
-        while not query.done:
+        while True:
+            await self._invoke_runner(query)
+            if query.done:
+                return
             await self._run_query_once(query)
 
-    async def _run_query_once(self, query: Query) -> None:
-        loop = asyncio.get_event_loop()
-
+    async def _invoke_runner(self, query: Query) -> None:
         try:
             await self._runner(query)
         except ClientError:
             _logger.info("query runner raised; stop retrying")
             raise
         except BaseException as err:
-            raise RunnerError(err)
+            raise RunnerError(err) from err
 
-        # Check only after yielding to the runner, to allow caching.
+    async def _run_query_once(self, query: Query) -> None:
         if query.done:
             return
 
+        loop = asyncio.get_event_loop()
+
         if query._time_start <= 0:
             query._time_start = loop.time()
 
         query._time_start_try = 0.0
         query._time_end_try = 0.0
         query._nb_tries += 1
 
-        check_cooldown = (
-            query.error
-            and isinstance(query.error, QueryRejectError)
-            and query.error.cause == QueryRejectCause.TOO_MANY_QUERIES
-        )
-
         try:
             session = self._session()
             rate_limiter = await self._rate_limiter(timeout=_next_timeout(query))
 
-            if check_cooldown:
+            if query._has_cooldown():
                 # If this client is running too many queries, we can check the status for a
                 # cooldown period. This request failing is a bit of an edge case.
                 # 'query.error' will be overwritten, which means we will not check for a
                 # cooldown in the next iteration.
                 status = await self._status(session=session, timeout=_next_timeout(query))
 
-                if _next_timeout_secs(query) and status.cooldown_secs > _next_timeout_secs(query):
+                if (timeout := _next_timeout_secs(query)) and status.cooldown_secs > timeout:
                     raise _giveup_error(query, loop)
 
                 await asyncio.sleep(status.cooldown_secs)
 
             # Limit the concurrent query requests to the number of slots available.
             await asyncio.wait_for(
                 fut=rate_limiter.acquire(),
@@ -306,14 +322,15 @@
             query._error = err
 
 
 def _next_timeout_secs(query: Query) -> Optional[float]:
     if query.run_timeout_secs:
         # use epsilon since 0 means "no timeout"
         return max(sys.float_info.epsilon, query.run_timeout_secs - query.run_duration_secs)
+    return None
 
 
 def _next_timeout(query: Query) -> aiohttp.ClientTimeout:
     return aiohttp.ClientTimeout(total=_next_timeout_secs(query))
 
 
 def _giveup_error(query: Query, loop: asyncio.AbstractEventLoop) -> GiveupError:
```

### Comparing `aio_overpass-0.1.2/aio_overpass/element.py` & `aio_overpass-0.2.0/aio_overpass/element.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Typed result set members."""
 
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from dataclasses import dataclass
-from typing import Any, Dict, Iterable, Iterator, List, Optional, Tuple, Type, Union
+from typing import Any, Dict, Iterable, Iterator, List, Optional, Tuple, Type, Union, cast
 
 from aio_overpass import Query
 
 import shapely.geometry
 import shapely.ops
 from shapely.geometry import (
     GeometryCollection,
@@ -284,25 +284,27 @@
     elem = obj if isinstance(obj, Element) else obj.member
 
     bounds = elem._geometry.bounds
     if bounds:
         (minlat, minlon, maxlat, maxlon) = bounds
         return minlon, minlat, maxlon, maxlat
 
+    return None
+
 
 def _geojson_feature(obj: Union[Element, "Relationship"]) -> GeoJsonDict:
     feature = {
         "type": "Feature",
         "geometry": _geojson_geometry(obj),
         "properties": _geojson_properties(obj),
     }
 
     bbox = _geojson_bbox(obj)
     if bbox:
-        feature["bbox"] = bbox
+        feature["bbox"] = bbox  # type: ignore
 
     return feature
 
 
 @dataclass(repr=False, eq=False)
 class Node(Element):
     """
@@ -361,15 +363,15 @@
 
     References:
         - https://wiki.openstreetmap.org/wiki/Relation
     """
 
     members: List["Relationship"]
 
-    def __iter__(self) -> Iterator[Tuple[str, Element]]:
+    def __iter__(self) -> Iterator[Tuple[Optional[str], Element]]:
         for relship in self.members:
             yield relship.role, relship.member
 
 
 @dataclass(repr=False, eq=False)
 class AreaWay(Way):
     """
@@ -468,14 +470,29 @@
         role = f" as '{self.role}'" if self.role else " "
         return f"{type(self).__name__}({self.member}{role} in {self.relation})"
 
 
 _KNOWN_ELEMENTS = {"node", "way", "relation", "area"}
 
 
+_ElementKey = Tuple[str, int]
+"""Elements are uniquely identified by the tuple (type, id)."""
+
+_MemberKey = Tuple[_ElementKey, str]
+"""Relation members are identified by their element key and role."""
+
+
+class _ElementCollector:
+    def __init__(self) -> None:
+        self.list: List[Element] = []
+        self.typed_dict: Dict[_ElementKey, Element] = {}
+        self.untyped_dict: Dict[_ElementKey, OverpassDict] = defaultdict(dict)
+        self.member_dict: Dict[int, List[_MemberKey]] = defaultdict(list)
+
+
 def collect_elements(query: Query) -> List[Element]:
     """
     Produce typed elements from the result set of a query.
 
     This function collects elements that are of type "node", "way", "relation", or "area".
     Derived elements with other types - f.e. produced by ``make`` and ``convert`` statements
     or when using ``out count`` - are ignored. An exception is made for areas, which are so
@@ -502,41 +519,46 @@
         ValueError: If the input query is unfinished/has no result set.
         KeyError: The only times there should be missing keys is when either using ``out noids``,
                   or when building derived elements that are missing common keys.
     """
     if not query.done:
         raise ValueError("query has no result set")
 
-    # Elements are uniquely identified by a key = (type, id)
+    collector = _ElementCollector()
+    _collect_untyped(query, collector)
+    _collect_typed(collector)
+    _collect_relationships(collector)
+    return collector.list
 
-    results = []
-    elems_typed = {}  # {key: Element object}
-    elems_dict = defaultdict(dict)  # {key: element data dict}
-    members = defaultdict(list)  # {relation id: [(key, role) for each member]}
 
-    # (a) conflation
+def _collect_untyped(query: Query, collector: _ElementCollector) -> None:
+    if not query.result_set:
+        raise AssertionError
+
+    # Here we populate 'untyped_dict' with both top level elements, and
+    # relation members, while conflating their data if they appear as both.
+    # We also populate 'member_dict'.
     for elem_dict in query.result_set["elements"]:
         if elem_dict.get("type") not in _KNOWN_ELEMENTS:
             continue
 
-        key = (elem_dict["type"], elem_dict["id"])
-        elems_dict[key].update(elem_dict)
+        key: _ElementKey = (elem_dict["type"], elem_dict["id"])
+        collector.untyped_dict[key].update(elem_dict)
 
         if elem_dict["type"] != "relation":
             continue
 
         for mem in elem_dict["members"]:
             key = (mem["type"], mem["ref"])
+            collector.untyped_dict[key].update(mem)
+            collector.member_dict[elem_dict["id"]].append((key, mem.get("role")))
 
-            elems_dict[key].update(mem)
 
-            members[elem_dict["id"]].append((key, mem.get("role")))
-
-    # (b) conversion
-    for elem_key, elem_dict in elems_dict.items():
+def _collect_typed(collector: _ElementCollector) -> None:
+    for elem_key, elem_dict in collector.untyped_dict.items():
         (elem_type, elem_id) = elem_key
 
         args = dict(
             id=elem_id,
             tags=elem_dict.get("tags"),
             bounds=tuple(elem_dict["bounds"].values()) if "bounds" in elem_dict else None,
             center=Point(elem_dict["center"].values()) if "center" in elem_dict else None,
@@ -580,29 +602,28 @@
             cls = AreaWay
             args["area_id"] = elem_id % _AREA_WAY_ID_OFFSET
 
         if cls is not Relation:
             args["geometry"] = _geometry(elem_dict)
 
         elem = cls(**args)
-        results.append(elem)
-        elems_typed[elem_key] = elem
+        collector.list.append(elem)
+        collector.typed_dict[elem_key] = elem
+
 
-    # (c) linking relations & members
-    for rel_id, mem_roles in members.items():
-        rel = elems_typed[("relation", rel_id)]
+def _collect_relationships(collector: _ElementCollector) -> None:
+    for rel_id, mem_roles in collector.member_dict.items():
+        rel = cast(Relation, collector.typed_dict[("relation", rel_id)])
 
         for mem_key, mem_role in mem_roles:
-            mem = elems_typed[mem_key]
+            mem = collector.typed_dict[mem_key]
             relship = Relationship(member=mem, relation=rel, role=mem_role or None)
             mem.relations.append(relship)
             rel.members.append(relship)
 
-    return results
-
 
 # e.g. area with id 3_600_051_477 correlates with relation 51_477
 _AREA_REL_ID_OFFSET = 3_600_000_000
 _AREA_WAY_ID_OFFSET = 2_400_000_000
 
 
 def _geometry(raw_elem: OverpassDict) -> Optional[BaseGeometry]:
@@ -628,21 +649,18 @@
     if raw_elem.get("type") not in _KNOWN_ELEMENTS:
         raise ValueError("expected element of type 'node', 'way', 'relation', or 'area'")
 
     if raw_elem["type"] == "node":
         lat, lon = raw_elem.get("lat"), raw_elem.get("lon")
         if lat and lon:
             return Point(lat, lon)
-        return None
 
     if raw_elem["type"] == "way":
         ls = _line(raw_elem)
-        if not ls:
-            return None
-        if ls.is_ring and _is_area_element(raw_elem):
+        if ls and ls.is_ring and _is_area_element(raw_elem):
             return Polygon(ls)
         return ls
 
     if _is_area_element(raw_elem):
         outers = (
             ls
             for ls in (
@@ -667,14 +685,16 @@
         ]
 
         if len(polys) == 1:
             return polys[0]
 
         return MultiPolygon(polys)
 
+    return None
+
 
 def _line(way: OverpassDict) -> Union[LineString, LinearRing, None]:
     """Returns the geometry of a way in the result set."""
     if "geometry" not in way or len(way["geometry"]) < 2:
         return None
     if way["geometry"][0] == way["geometry"][-1]:
         cls = LinearRing
```

### Comparing `aio_overpass-0.1.2/aio_overpass/error.py` & `aio_overpass-0.2.0/aio_overpass/error.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """
 Error types.
 
 ```
-                             ClientError
+                            (ClientError)
                                   ╷
     ┌──────────────┬──────────────┼────────────┬────────────────┐
     ╵              ╵              ╵            ╵                ╵
-CallError    ResponseError    QueryError    GiveupError    RunnerError
-                                  ╷
-                   ┌──────────────┴──────────────┐
-                   ╵                             ╵
-          QueryLanguageError              QueryRejectError
+CallError     RunnerError   (QueryError)   GiveupError    ResponseError
+                                  ╷                             ╷
+         ┌────────────────────────┼──────────────────────┐      │
+         ╵                        ╵                      ╵      ╵
+QueryLanguageError         QueryRejectError          QueryResponseError
 ```
 """
 
 import html
 import re
 from dataclasses import dataclass
 from enum import Enum, auto
 from json import JSONDecodeError
-from typing import List, Optional, Tuple, Union
+from typing import List, Optional, Tuple, Union, no_type_check
 
 import aiohttp
 import aiohttp.typedefs
 
 
 __docformat__ = "google"
 __all__ = (
@@ -31,14 +31,15 @@
     "CallError",
     "ResponseError",
     "GiveupError",
     "QueryError",
     "QueryLanguageError",
     "QueryRejectError",
     "QueryRejectCause",
+    "QueryResponseError",
     "RunnerError",
 )
 
 
 class ClientError(Exception):
     """Base exception for failed Overpass API requests and queries."""
 
@@ -61,17 +62,14 @@
     def __post_init__(self) -> None:
         # imitate "raise QueryRunnerError(...) from cause"
         self.__cause__ = self.cause
 
     def __str__(self) -> str:
         return str(self.cause)
 
-    def __repr__(self) -> str:
-        return f"{type(self).__name__}(cause={self.cause!r})"
-
 
 @dataclass
 class CallError(ClientError):
     """
     Failed to make an API request.
 
     This error is raised when the client failed to get any response,
@@ -86,25 +84,23 @@
     def __post_init__(self) -> None:
         # imitate "raise CallError(...) from cause"
         self.__cause__ = self.cause
 
     def __str__(self) -> str:
         return str(self.cause)
 
-    def __repr__(self) -> str:
-        return f"{type(self).__name__}(cause={self.cause!r})"
-
 
 @dataclass
 class ResponseError(ClientError):
     """
     Unexpected API response.
 
-    This is usually a bug, since the client is meant to process any response of an
-    Overpass API instance.
+    This error is raised when a request fails, but we can't specifically say why.
+    This may indicate a bug on our end, since the client is meant to process almost any
+    response of an Overpass API instance.
     """
 
     request_info: aiohttp.RequestInfo
     history: Tuple[aiohttp.ClientResponse, ...]
     status: int
     message: str
     headers: Optional[aiohttp.typedefs.LooseHeaders]
@@ -114,25 +110,14 @@
         return self.history[-1]
 
     def __str__(self) -> str:
         return (
             f"unexpected response: {self.status}, {self.message!r}, {self.request_info.real_url!r}"
         )
 
-    def __repr__(self) -> str:
-        args = f"{self.request_info!r}, {self.history!r}"
-        if self.status != 0:
-            args += f", status={self.status!r}"
-        if self.message:
-            args += f", message={self.message!r}"
-        if self.headers is not None:
-            args += f", headers={self.headers!r}"
-
-        return f"{type(self).__name__}({args})"
-
 
 @dataclass
 class GiveupError(ClientError):
     """
     The client spent too long running a query, and gave up.
 
     This error is raised when the run timeout duration set by a query runner is exceeded.
@@ -149,53 +134,55 @@
         if self.kwargs:
             query = f"query {self.kwargs}"
         else:
             query = "query <no kwargs>"
 
         return f"gave up on {query} after {self.after_secs:.01f} seconds"
 
-    def __repr__(self) -> str:
-        return f"{type(self).__name__}(kwargs={self.kwargs}, after_secs={self.after_secs:.01f})"
-
 
 @dataclass
 class QueryError(ClientError):
     """
-    A query has failed at the Overpass API server.
+    Base exception for queries that failed at the Overpass API server.
 
     Attributes:
         kwargs: the query's ``kwargs``
-        messages: the error messages provided by the API
+        remarks: the error remarks provided by the API
     """
 
     kwargs: dict
-    messages: List[str]
-
-    def __post_init__(self) -> None:
-        if not self.messages:
-            raise ValueError("expected at least one message")
+    remarks: List[str]
 
     def __str__(self) -> str:
         if self.kwargs:
             query = f"query {self.kwargs}"
         else:
             query = "query <no kwargs>"
 
-        first = f"'{self.messages[0]}'"
+        first = f"'{self.remarks[0]}'"
 
-        if len(self.messages) > 1:
-            rest = f" (+{len(self.messages) - 1} more)"
+        if len(self.remarks) > 1:
+            rest = f" (+{len(self.remarks) - 1} more)"
         else:
             rest = ""
 
         return f"{query} failed: {first}{rest}"
 
-    def __repr__(self) -> str:
-        messages = ", ".join(f"'{msg}'" for msg in self.messages)
-        return f"{type(self).__name__}(kwargs={self.kwargs}, messages={messages})"
+
+@dataclass
+class QueryResponseError(ResponseError, QueryError):
+    """
+    Unexpected query response.
+
+    This error is raised when a query fails (thus extends ``QueryError``),
+    but we can't specifically say why (thus also extends ``ResponseError``).
+    """
+
+    def __str__(self) -> str:
+        return QueryError.__str__(self)
 
 
 @dataclass
 class QueryLanguageError(QueryError):
     """
     Indicates the query's QL code is not valid.
 
@@ -247,17 +234,15 @@
             return "server too busy"
         if self == QueryRejectCause.TOO_MANY_QUERIES:
             return "too many queries"
         if self == QueryRejectCause.EXCEEDED_TIMEOUT:
             return "exceeded 'timeout'"
         if self == QueryRejectCause.EXCEEDED_MAXSIZE:
             return "exceeded 'maxsize'"
-
-    def __repr__(self) -> str:
-        return f"{type(self).__name__}.{self.name}"
+        raise AssertionError()
 
 
 @dataclass
 class QueryRejectError(QueryError):
     """
     A query was rejected or cancelled by the API server.
 
@@ -271,31 +256,28 @@
         if self.cause in (QueryRejectCause.TOO_BUSY, QueryRejectCause.TOO_MANY_QUERIES):
             rejection = "query rejected"
         else:
             rejection = "query cancelled"
 
         return f"{rejection}: {self.cause}"
 
-    def __repr__(self) -> str:
-        return f"{type(self).__name__}(cause={self.cause!r})"
-
 
+@no_type_check
 def _to_client_error(
     obj: Union[aiohttp.ClientResponse, aiohttp.ClientError]
 ) -> Union[CallError, ResponseError]:
     """
     Build a ``ClientError`` from either an ``aiohttp`` client error or an unrecognized response.
 
     Returns:
-        ``CallError`` if ``obj`` is an ``aiohttp.ClientError``, but not an ``aiohttp.ClientResponseError``.
-        ``ResponseError`` if ``obj`` is a response or an ``aiohttp.ClientResponseError``.
+        - ``CallError`` if ``obj`` is an ``aiohttp.ClientError``,
+          but not an ``aiohttp.ClientResponseError``.
+        - ``ResponseError`` if ``obj`` is a response or an ``aiohttp.ClientResponseError``.
     """
-    if not isinstance(obj, aiohttp.ClientResponseError) and not isinstance(
-        obj, aiohttp.ClientResponse
-    ):
+    if not isinstance(obj, (aiohttp.ClientResponseError, aiohttp.ClientResponse)):
         return CallError(cause=obj)
 
     error = ResponseError(
         request_info=obj.request_info,
         history=obj.history,
         status=obj.status,
         message=obj.message if isinstance(obj, aiohttp.ClientResponseError) else obj.reason,
@@ -321,123 +303,114 @@
         QueryError: When there's any other JSON remark or HTML error message.
     """
     await _raise_for_html_response(response, query_kwargs)
 
     try:
         json = await response.json()
     except aiohttp.ClientResponseError as err:
-        raise _to_client_error(err)
+        raise _to_client_error(err) from err
     except JSONDecodeError as err:
         raise _response_error(response) from err
 
     if json is None:
         raise _response_error(response)
 
-    _raise_for_json_remarks(json, query_kwargs)
+    _raise_for_json_remarks(response, json, query_kwargs)
 
     _raise_for_status(response, query_kwargs)
 
     return json
 
 
-def _response_error(response: aiohttp.ClientResponse) -> ResponseError:
-    return ResponseError(
-        request_info=response.request_info,
-        history=response.history,
-        status=response.status,
-        message=response.reason,
-        headers=response.headers,
-    )
-
-
 def _raise_for_status(response: aiohttp.ClientResponse, query_kwargs: dict) -> None:
     """
     Raise a fitting exception based on the status code.
 
     Raises:
         RejectError: for status "Too Many Requests" and "Gateway Timeout"
         ResponseError: for any status >= 400
 
     References:
         - HTTP status codes: http://overpass-api.de/command_line.html
     """
     if response.status == _TOO_MANY_REQUESTS:
         raise QueryRejectError(
-            kwargs=query_kwargs, messages=[], cause=QueryRejectCause.TOO_MANY_QUERIES
+            kwargs=query_kwargs, remarks=[], cause=QueryRejectCause.TOO_MANY_QUERIES
         )
 
     if response.status == _GATEWAY_TIMEOUT:
-        raise QueryRejectError(kwargs=query_kwargs, messages=[], cause=QueryRejectCause.TOO_BUSY)
+        raise QueryRejectError(kwargs=query_kwargs, remarks=[], cause=QueryRejectCause.TOO_BUSY)
 
     if response.status >= _BAD_REQUEST:
         raise _to_client_error(response)
 
 
 _BAD_REQUEST = 400
 _TOO_MANY_REQUESTS = 429
 _GATEWAY_TIMEOUT = 504
 
 
-def _raise_for_json_remarks(json: dict, query_kwargs: dict) -> None:
+def _raise_for_json_remarks(
+    response: aiohttp.ClientResponse, json: dict, query_kwargs: dict
+) -> None:
     """
     Raise a fitting exception based on a remark in a JSON response.
 
     Raises:
         RejectError: if the API server remarked that the query was rejected or cancelled
         QueryError: if the API server remarked something else
     """
     remark = json.get("remark")
     if not remark:
         return
 
     timeout_cause = _match_reject_cause(remark)
     if timeout_cause:
-        raise QueryRejectError(kwargs=query_kwargs, messages=[remark], cause=timeout_cause)
+        raise QueryRejectError(kwargs=query_kwargs, remarks=[remark], cause=timeout_cause)
 
-    raise QueryError(kwargs=query_kwargs, messages=[remark])
+    raise _query_response_error(kwargs=query_kwargs, remarks=[remark], response=response)
 
 
 async def _raise_for_html_response(response: aiohttp.ClientResponse, query_kwargs: dict) -> None:
     """
-    Raise a fitting exception based on error messages in an HTML response.
+    Raise a fitting exception based on error remarks in an HTML response.
 
     Raises:
-        RejectError: if one of the error messages indicate that the query was rejected or cancelled
-        QueryError: when encountering other error messages
-        ResponseError: when error messages cannot be extracted from the response
+        RejectError: if one of the error remarks indicate that the query was rejected or cancelled
+        QueryError: when encountering other error remarks
+        ResponseError: when error remarks cannot be extracted from the response
     """
     if response.content_type != "text/html":
         return
 
     text = await response.text()
 
     pattern = re.compile("Error</strong>: (.+?)</p>", re.DOTALL)
     errors = [html.unescape(err.strip()) for err in pattern.findall(text)]
 
     if not errors:  # unexpected format
         raise _to_client_error(response)
 
     if any(_is_ql_error(msg) for msg in errors):
-        raise QueryLanguageError(kwargs=query_kwargs, messages=errors)
+        raise QueryLanguageError(kwargs=query_kwargs, remarks=errors)
 
-    reject_causes = (_match_reject_cause(err) for err in errors)
-    reject_causes = [cause for cause in reject_causes if cause]
+    reject_causes = [cause for err in errors if (cause := _match_reject_cause(err))]
 
     if reject_causes:
-        raise QueryRejectError(kwargs=query_kwargs, messages=errors, cause=reject_causes[0])
+        raise QueryRejectError(kwargs=query_kwargs, remarks=errors, cause=reject_causes[0])
 
-    raise QueryError(kwargs=query_kwargs, messages=errors)
+    raise _query_response_error(kwargs=query_kwargs, remarks=errors, response=response)
 
 
 def _match_reject_cause(error_msg: str) -> Optional[QueryRejectCause]:
     """
     Check if the given error message indicates that a query was rejected or cancelled.
 
     AFAIK, neither the 'remarks' in JSON responses, nor the errors listed in HTML responses
-    are neatly listed somewhere, but it seems matching a small subset of messages is enough
+    are neatly listed somewhere, but it seems matching a small subset of remarks is enough
     to identify recoverable errors.
 
     References:
         - Related: https://github.com/DinoTools/python-overpy/issues/62
         - Examples in the API source: https://github.com/drolbr/Overpass-API/search?q=runtime_error
     """
     if "Please check /api/status for the quota of your IP address" in error_msg:
@@ -452,8 +425,34 @@
     if "out of memory" in error_msg:
         return QueryRejectCause.EXCEEDED_MAXSIZE
 
     return None
 
 
 def _is_ql_error(message: str) -> bool:
-    return "parse error:" in message or "static error:" in message
+    return "encoding error:" in message or "parse error:" in message or "static error:" in message
+
+
+def _response_error(response: aiohttp.ClientResponse) -> ResponseError:
+    return ResponseError(
+        request_info=response.request_info,
+        history=response.history,
+        status=response.status,
+        message=str(response.reason) if response.reason else "",
+        headers=response.headers,
+    )
+
+
+def _query_response_error(
+    kwargs: dict,
+    remarks: List[str],
+    response: aiohttp.ClientResponse,
+) -> QueryResponseError:
+    return QueryResponseError(
+        kwargs=kwargs,
+        remarks=remarks,
+        request_info=response.request_info,
+        history=response.history,
+        status=response.status,
+        message=str(response.reason) if response.reason else "",
+        headers=response.headers,
+    )
```

### Comparing `aio_overpass-0.1.2/aio_overpass/pt.py` & `aio_overpass-0.2.0/aio_overpass/pt.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 Classes and queries specialized on public transportation routes.
 """
 
-import itertools
 from collections import Counter
 from dataclasses import dataclass
 from enum import Enum, auto
 from typing import Any, Generator, List, Optional, Set, Union, cast
 
 from aio_overpass._dist import fast_distance
 from aio_overpass._ql import one_of_filter, poly_filter
@@ -21,14 +20,15 @@
     Way,
     collect_elements,
 )
 from aio_overpass.query import Query
 
 import shapely.ops
 from shapely.geometry import GeometryCollection, Point, Polygon
+from shapely.geometry.base import BaseGeometry
 
 
 __docformat__ = "google"
 __all__ = (
     "Route",
     "Stop",
     "Connection",
@@ -117,15 +117,17 @@
                  be outside of it. This shape should be simplified, since a larger number
                  of coordinates on the exterior will slow down the query.
         vehicles: A list of transportation modes to filter by, or an empty list to include
                   routes of any type. A non-empty list will filter routes by the ``route``
                   key.
     """
 
-    def __init__(self, polygon: Polygon, vehicles: List["Vehicle"] = None, **kwargs) -> None:
+    def __init__(
+        self, polygon: Polygon, vehicles: Optional[List["Vehicle"]] = None, **kwargs
+    ) -> None:
         if not vehicles:
             vehicles = list(Vehicle)
 
         self.polygon = polygon
         self.vehicles = vehicles
 
         spatial_filter = poly_filter(self.polygon)
@@ -209,19 +211,19 @@
         """
         stop_pos_name = self.stop_position.member.tag("name") if self.stop_position else None
         platform_name = self.platform.member.tag("name") if self.platform else None
 
         if stop_pos_name == platform_name and stop_pos_name is not None:
             return stop_pos_name
 
-        names = (stop_pos_name, platform_name, *(rel.tag("name") for rel in self.stop_areas))
+        names = [stop_pos_name, platform_name, *(rel.tag("name") for rel in self.stop_areas)]
         names = [name for name in names if name]
 
         if not names:
-            return
+            return None
 
         counter = Counter(names)
         ((most_common, _),) = counter.most_common(1)
         return most_common
 
     @property
     def connection(self) -> Connection:
@@ -252,36 +254,43 @@
     @property
     def _stop_point(self) -> Optional[Point]:
         """This is set if we have a point that is on the track of the route."""
         if isinstance(self.stop_coords, Node):
             return self.stop_coords.geometry
         if isinstance(self.stop_coords, Point):
             return self.stop_coords
+        return None
 
     @property
     def _geometry(self) -> GeometryCollection:
         """Collection of ``self.platform``, ``self.stop_position`` and  ``self.stop_coords``."""
         geoms = []
 
         if self.platform:
-            geoms.append(self.platform.member.geometry)
+            # this can be None if the platform is a relation
+            geom: Optional[BaseGeometry] = getattr(self.platform.member, "geometry", None)
+            if geom:
+                geoms.append(geom)
 
         if self.stop_position:
-            geoms.append(self.stop_position.member.geometry)
+            member = cast(Node, self.stop_position.member)
+            geoms.append(member.geometry)
 
         if isinstance(self.stop_coords, Point) and self.stop_coords not in geoms:
             geoms.append(self.stop_coords)
 
         return GeometryCollection(geoms)
 
     def __repr__(self) -> str:
         if self.stop_position:
             elem = f"stop_position={self.stop_position.member}"
-        else:
+        elif self.platform:
             elem = f"platform={self.platform.member}"
+        else:
+            raise AssertionError
 
         return f"{type(self).__name__}({elem}, name='{self.name}')"
 
 
 class Vehicle(Enum):
     """
     Most common modes of public transportation.
@@ -326,17 +335,17 @@
 
     OTHER = auto()
 
     @property
     def version_number(self) -> Optional[int]:
         if self in (RouteScheme.EXPLICIT_V1, RouteScheme.ASSUME_V1):
             return 1
-
         if self in (RouteScheme.EXPLICIT_V2, RouteScheme.ASSUME_V2):
             return 2
+        return None
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}.{self.name}"
 
 
 @dataclass
 class Route(Spatial):
@@ -492,30 +501,32 @@
 
         if from_ and to and via:
             return f"{from_} => {via} => {to}"
 
         if from_ and to:
             return f"{from_} => {to}"
 
+        return None
+
     @property
     def vehicle(self) -> Vehicle:
         """
         The mode of transportation used on this route.
 
         This value corresponds with the value of the relation's ``route`` key.
         """
+        if not self.relation.tags or "route" not in self.relation.tags:
+            raise AssertionError
         return Vehicle[self.relation.tags["route"].upper()]
 
     @property
     def bounds(self) -> Optional[Bbox]:
         """The bounding box around all stops of this route."""
         geom = GeometryCollection([stop._geometry for stop in self.stops if stop._geometry])
-        bounds = geom.bounds
-        if bounds:
-            return bounds
+        return geom.bounds or None
 
     @property
     def geojson(self) -> GeoJsonDict:
         # TODO Route geojson
         raise NotImplementedError
 
     def __repr__(self) -> str:
@@ -540,25 +551,28 @@
 
 References:
     - https://wiki.openstreetmap.org/wiki/Relation:route_master 
 """
 
 
 def collect_routes(query: RouteQuery, perimeter: Optional[Polygon] = None) -> List[Route]:
+    # TODO the way 'perimeter' works might be confusing
     """
     Consumes the result set of a query and produces ``Route`` objects.
 
     The order of elements is *not* retained.
 
     The result set in the input query will be empty after calling this function.
 
     Args:
         query: The query that produced a result set of route relations.
-        perimeter: If set, ``stops`` of resulting routes will be limited to the exterior
-                   of this polygon. Any relation members in ``members`` will not be filtered.
+        perimeter: If set, ``stops`` at the end will be truncated if they are outside of this
+                   polygon. This means stops outside the polygon will still be in the list as
+                   long as there is at least one following stop that *is* inside the list.
+                   Any relation members in ``members`` will not be filtered.
 
     Raises:
         ValueError: if the input query has no result set
 
     Returns:
         all routes in the result set of the input query
     """
@@ -570,22 +584,16 @@
     for route_rel in route_rels:
         # Group route relation members per stop:
         # f.e. a platform, and a stop position at the same station.
         stops = list(_stops(route_rel))
 
         # Filter stops by perimeter: cut off at the last stop that is in the perimeter.
         if perimeter:
-            nb_last_stops_skipped = sum(
-                1
-                for _ in itertools.takewhile(
-                    lambda s: perimeter.contains(s._stop_point), reversed(stops)
-                )
-            )
-            if nb_last_stops_skipped > 0:
-                del stops[-nb_last_stops_skipped:]
+            while stops and not perimeter.contains(stops[-1]._stop_point):
+                del stops[-1]
 
         route = Route(
             relation=route_rel,
             scheme=_scheme(route_rel),
             stops=stops,
         )
 
@@ -770,16 +778,18 @@
     if _share_stop_area(a, b):
         return True
 
     # assume same stop if close together
     if not a.member._geometry or not b.member._geometry:
         return False
 
-    a, b = shapely.ops.nearest_points(a.member._geometry, b.member._geometry)  # euclidean nearest
-    distance = fast_distance(*a.coords[0], *b.coords[0])
+    pt_a, pt_b = shapely.ops.nearest_points(
+        a.member._geometry, b.member._geometry
+    )  # euclidean nearest
+    distance = fast_distance(*pt_a.coords[0], *pt_b.coords[0])
     return distance <= _MAX_DISTANCE_TO_TRACK
 
 
 _MAX_DISTANCE_TO_TRACK = 30.0  # meters
 """
 An expectation of the maximum distance between a stop position and its platform.
```

### Comparing `aio_overpass-0.1.2/aio_overpass/pt_ordered.py` & `aio_overpass-0.2.0/aio_overpass/pt_ordered.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 
     def _split(
         self, predicate: Callable[[OrderedRouteViewNode, OrderedRouteViewNode], bool]
     ) -> Generator["OrderedRouteView", None, None]:
         if len(self.ordering) < 2:
             return
 
-        ordering = []
+        ordering: List[OrderedRouteViewNode] = []
 
         for a, b in zip(self.ordering, self.ordering[1:]):
             if predicate(a, b):
                 yield replace(self, ordering=ordering)
                 ordering = [a]
             else:
                 ordering.append(a)
@@ -140,35 +140,35 @@
         """
         if first_n < 2:
             raise ValueError("cannot take less than two stops")
 
         pre_gap, *_ = self.gap_split()
 
         by_stop = itertools.groupby(pre_gap.ordering, key=lambda node: node.path_idx)
-        by_stop = itertools.islice(by_stop, first_n - 1)
+        by_stop_truncated = itertools.islice(by_stop, first_n - 1)
 
-        ordering = [node for _, nodes in by_stop for node in nodes]
+        ordering = [node for _, nodes in by_stop_truncated for node in nodes]
 
         return replace(self, ordering=ordering)
 
     def trim(self, distance: float) -> "OrderedRouteView":
         """
         Returns the continuous view that is not longer than a given distance,
         starting from the first stop.
         """
         pre_gap, *_ = self.gap_split()
 
         distance_start = pre_gap.ordering[0].distance
 
         by_stop = itertools.groupby(pre_gap.ordering, key=lambda node: node.path_idx)
 
-        ordering = []
+        ordering: List[OrderedRouteViewNode] = []
 
-        for _, nodes in by_stop:
-            nodes = list(nodes)
+        for _, nodes_iter in by_stop:
+            nodes = list(nodes_iter)
             distance_end = nodes[-1].distance
 
             if (distance_end - distance_start) > distance:
                 break
 
             ordering.extend(nodes)
 
@@ -185,16 +185,16 @@
         """
         max_nb_paths = len(self.stops) - 1
 
         grouped = itertools.groupby(iterable=self.ordering, key=lambda node: node.path_idx)
 
         lines: List[Optional[LineString]] = [None for _ in range(max_nb_paths)]
 
-        for n, nodes in grouped:
-            nodes = [(node.lat, node.lon) for node in nodes]
+        for n, nodes_iter in grouped:
+            nodes = [(node.lat, node.lon) for node in nodes_iter]
             if len(nodes) < 2:
                 continue
             line = LineString(nodes)
             lines[n] = line
 
         return lines
 
@@ -210,23 +210,23 @@
         """
         paths = self.paths
 
         if not any(ls for ls in paths):
             return MultiLineString([])
 
         # group consecutive stretches of lines or None values
-        stretches = itertools.groupby(iterable=paths, key=bool)
+        stretches_grouped = itertools.groupby(iterable=paths, key=bool)
 
         # select all sets of consecutive lines to merge them
-        stretches = (line_strings for has_track, line_strings in stretches if has_track)
+        stretches = (line_strings for has_track, line_strings in stretches_grouped if has_track)
 
         merged_lines = []
 
         for line_strings in stretches:
-            coords = []
+            coords: List[List[float]] = []
 
             for line in line_strings:
                 if not coords:
                     coords.extend(line.coords)
                 else:
                     coords.extend(
                         line.coords[1:]
@@ -448,24 +448,24 @@
 
     # (c) use a node on the graph, that is closest to one of the relation members
     station_geom = GeometryCollection(
         [relship.member._geometry for relship in (stop.stop_position, stop.platform) if relship]
     )
 
     if not track_nodes or not station_geom:
-        return
+        return None
 
     # Calculate the distance of the stop geometry to the track geometry.
     a, b = shapely.ops.nearest_points(track_ways, station_geom)  # euclidean nearest
 
     distance_to_track = fast_distance(*a.coords[0], *b.coords[0])
 
     # Idea: if the stop is too far away from the track, it cannot be representative.
     if distance_to_track > _MAX_DISTANCE_TO_TRACK:
-        return
+        return None
 
     # Find the node in the graph that is closest to the stop.
     a, _ = shapely.ops.nearest_points(track_nodes, station_geom)  # euclidean nearest
 
     # This node is *probably* representative of the actual stop position for this stop.
     # It is possible though, that the node is actually close to more than one way
     # on the route's track, and that we choose a node that could be far from the
```

### Comparing `aio_overpass-0.1.2/aio_overpass/query.py` & `aio_overpass-0.2.0/aio_overpass/query.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import asyncio
 import hashlib
 import json
 import logging
 import re
 from pathlib import Path
-from typing import Awaitable, Callable, Optional
+from typing import Optional, Protocol
 
 from aio_overpass.error import (
     ClientError,
     QueryLanguageError,
     QueryRejectCause,
     QueryRejectError,
     ResponseError,
@@ -29,15 +29,15 @@
 
 DEFAULT_MAXSIZE = 512
 """Default ``maxsize`` setting in megabytes"""
 
 DEFAULT_TIMEOUT = 180
 """Default ``timeout`` setting in seconds"""
 
-_COPYRIGHT = "The data included in this document is from www.openstreetmap.org. The data is made available under ODbL."
+_COPYRIGHT = "The data included in this document is from www.openstreetmap.org. The data is made available under ODbL."  # noqa: E501
 """This is the same copyright notice included in result sets"""
 
 _SETTING_PATTERN = re.compile(r"\[(\w+?):(.+?)]\s*;?")
 """A pattern to match setting declarations (not the entire settings statement)."""
 
 
 class Query:
@@ -74,14 +74,22 @@
         self._result_set: Optional[dict] = None
         self._result_set_bytes = 0.0
         self._time_end_try = 0.0  # time the most recent try finished
         self._time_start = 0.0  # time prior to executing the first try
         self._time_start_try = 0.0  # time prior to executing the most recent try
         self._nb_tries = 0
 
+    def _has_cooldown(self) -> bool:
+        """When ``True``, we should query the API status to retrieve our cooldown period."""
+        return (
+            self.error is not None
+            and isinstance(self.error, QueryRejectError)
+            and self.error.cause == QueryRejectCause.TOO_MANY_QUERIES
+        )
+
     def reset(self) -> None:
         """Reset the query to its initial state, ignoring previous tries."""
         Query.__init__(self, input_code=self._input_code, **self._kwargs)
 
     @property
     def input_code(self) -> str:
         """The original input Overpass QL source code."""
@@ -327,24 +335,27 @@
             details["run_duration"] = f"{self.run_duration_secs}s"
 
         details_str = ", ".join((f"{k}={v!r}" for k, v in details.items()))
 
         return f"{cls_name}({details_str})"
 
 
-QueryRunner = Callable[[Query], Awaitable[None]]
-"""
-A query runner is async function that is called before a client makes an API request.
-
-Query runners can be used to
- - retry queries when they fail
- - modify queries, f.e. to lower/increase their maxsize/timeout
- - log query results & errors
- - implement caching
-"""
+class QueryRunner(Protocol):
+    """
+    A query runner is async function that is called before a client makes an API request.
+
+    Query runners can be used to
+     - retry queries when they fail
+     - modify queries, f.e. to lower/increase their maxsize/timeout
+     - log query results & errors
+     - implement caching
+    """
+
+    async def __call__(self, query: Query) -> None:
+        pass
 
 
 class DefaultQueryRunner(QueryRunner):
     """
     A general query runner that
         - retries with an increasing back-off period in between tries if the server is too busy
         - retries and doubles timeout and maxsize settings if they were exceeded
@@ -397,15 +408,15 @@
         if query.done:
             self._cache_write(query)
             return
 
         err = query.error
 
         # Exhausted all tries; do not retry.
-        if query.nb_tries == self._max_tries:
+        if err and query.nb_tries == self._max_tries:
             raise err
 
         # Response errors usually indicate a bug in the client; do not retry.
         if isinstance(err, ResponseError):
             raise err
 
         # QL error; do not retry.
```

### Comparing `aio_overpass-0.1.2/pyproject.toml` & `aio_overpass-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "aio-overpass"
-version = "0.1.2"
+version = "0.2.0"
 description = "Async client for the Overpass API"
 authors = ["Tim Wiechers <mail@timwie.dev>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/timwie/aio-overpass"
-# TODO documentation = "https://..."
+documentation = "https://www.timwie.dev/aio-overpass/"
 packages = [{ include = "aio_overpass" }]
-include = [] # TODO "CHANGELOG.md"
+include = ["CHANGELOG.md"]
 exclude = ["test/", "tasks.py"]
 keywords = [
     "geojson",
     "geospatial",
     "gis",
     "open-street-map",
     "osm",
@@ -38,48 +38,69 @@
 shapely = { version = "~2.0.1", optional = true }
 
 [tool.poetry.extras]
 joblib = ["joblib"]
 networkx = ["networkx"]
 shapely = ["shapely"]
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 aioresponses = "^0.7.4"
 black = "^23.3.0"
 codecov = "^2.1.13"
-folium = "^0.14.0"
-invoke = "^2.0.0"
+invoke = "^2.1.2"
 isort = "^5.12.0"
-jupyterlab = "^3.6.3"
+mypy = "^1.3.0"
 pdoc = "^13.1.1"
-pytest = "^7.3.1"
+pytest = "^7.3.2"
 pytest-asyncio = "^0.21.0"
-pytest-cov = "^4.0.0"
+pytest-cov = "^4.1.0"
+ruff = "^0.0.272"
+
+[tool.poetry.group.notebooks]
+optional = true
+
+[tool.poetry.group.notebooks.dependencies]
+folium = "^0.14.0"
+jupyterlab = "^4.0.0"
 randomcolor = "^0.4.4.6"
-ruff = "^0.0.263"
 tabulate = "^0.9.0"
 
 [tool.ruff]
 # https://github.com/charliermarsh/ruff#configuration
 # https://beta.ruff.rs/docs/rules/
 line-length = 100
 target-version = "py38"
 select = ["E", "F", "N",  "UP", "ANN", "S", "B", "C4", "PL"]
 ignore = ["ANN003", "ANN101", "ANN401", "C408", "PLR2004", "PLW2901"]
 
+# Exclude a variety of commonly ignored directories.
+exclude = [
+    ".git",
+    ".ipynb_checkpoints",
+    ".mypy_cache",
+    ".pytest_cache",
+    ".ruff_cache",
+    "build",
+    "doc",
+]
+
 [tool.black]
 # https://github.com/psf/black#configuration
 line-length = 100
 
 [tool.isort]
 # https://pycqa.github.io/isort/docs/configuration/options.html
 profile = "black"
 line_length=100
 indent='    '
 multi_line_output=6
 lines_after_imports=2
 known_first_party="aio_overpass"
 sections="STDLIB,FIRSTPARTY,THIRDPARTY,LOCALFOLDER"
 
+[tool.mypy]
+# https://mypy.readthedocs.io/en/stable/running_mypy.html#missing-library-stubs-or-py-typed-marker
+ignore_missing_imports = true
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `aio_overpass-0.1.2/PKG-INFO` & `aio_overpass-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-overpass
-Version: 0.1.2
+Version: 0.2.0
 Summary: Async client for the Overpass API
 Home-page: https://github.com/timwie/aio-overpass
 License: MIT
 Keywords: geojson,geospatial,gis,open-street-map,osm,overpass-api,public-transport
 Author: Tim Wiechers
 Author-email: mail@timwie.dev
 Requires-Python: >=3.8,<4.0
@@ -24,14 +24,15 @@
 Provides-Extra: joblib
 Provides-Extra: networkx
 Provides-Extra: shapely
 Requires-Dist: aiohttp (>=3.8.4,<3.9.0)
 Requires-Dist: joblib (>=1.2.0,<1.3.0) ; extra == "joblib"
 Requires-Dist: networkx (>=3.1,<3.2) ; extra == "networkx"
 Requires-Dist: shapely (>=2.0.1,<2.1.0) ; extra == "shapely"
+Project-URL: Documentation, https://www.timwie.dev/aio-overpass/
 Project-URL: Repository, https://github.com/timwie/aio-overpass
 Description-Content-Type: text/markdown
 
 <h1 align="center">
 aio-overpass
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/timwie/aio-overpass/ci.yml)](https://github.com/timwie/aio-overpass/actions/workflows/ci.yml)
@@ -56,15 +57,15 @@
 - [Motivation](#motivation)
 - [Related Projects](#related-projects)
 - [License](#license)
 
 #### See also
 - An overview of modules, classes and functions can be found in the [API reference](http://www.timwie.dev/aio-overpass/).
 - The version history is available in [CHANGELOG.md](https://github.com/timwie/aio-overpass/blob/main/CHANGELOG.md).
-- Contributor guide is forthcoming :construction:
+- Developers can find some instructions in [CONTRIBUTING.md](https://github.com/timwie/aio-overpass/blob/main/CONTRIBUTING.md).
 
 <br>
 
 ## Features
 - Asynchronous requests using [aiohttp]
 - Concurrent queries
 - Respects rate limits
```

