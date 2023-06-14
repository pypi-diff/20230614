# Comparing `tmp/polygon_api_client-1.8.6.tar.gz` & `tmp/polygon_api_client-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polygon_api_client-1.8.6.tar", max compression
+gzip compressed data, was "polygon_api_client-1.9.tar", max compression
```

## Comparing `polygon_api_client-1.8.6.tar` & `polygon_api_client-1.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1074 2023-05-17 15:05:24.035156 polygon_api_client-1.8.6/LICENSE
--rw-r--r--   0        0        0      148 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/__init__.py
--rw-r--r--   0        0        0      256 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/exceptions.py
--rw-r--r--   0        0        0      329 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/logging.py
--rw-r--r--   0        0        0      561 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/modelclass.py
--rw-r--r--   0        0        0     1713 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/__init__.py
--rw-r--r--   0        0        0     8840 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/aggs.py
--rw-r--r--   0        0        0     6705 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/base.py
--rw-r--r--   0        0        0    12601 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/indicators.py
--rw-r--r--   0        0        0      356 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/models/__init__.py
--rw-r--r--   0        0        0     3408 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/models/aggs.py
--rw-r--r--   0        0        0     1530 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/models/common.py
--rw-r--r--   0        0        0     2755 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/models/conditions.py
--rw-r--r--   0        0        0     1784 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/models/contracts.py
--rw-r--r--   0        0        0      645 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/models/dividends.py
--rw-r--r--   0        0        0      569 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/models/exchanges.py
--rw-r--r--   0        0        0    10103 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/models/financials.py
--rw-r--r--   0        0        0     2399 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/models/indicators.py
--rw-r--r--   0        0        0     2499 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/models/markets.py
--rw-r--r--   0        0        0     3434 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/models/quotes.py
--rw-r--r--   0        0        0     3687 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/models/request.py
--rw-r--r--   0        0        0     8754 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/models/snapshot.py
--rw-r--r--   0        0        0      446 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/models/splits.py
--rw-r--r--   0        0        0     2269 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/models/summaries.py
--rw-r--r--   0        0        0     6892 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/models/tickers.py
--rw-r--r--   0        0        0     2051 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/models/trades.py
--rw-r--r--   0        0        0     5129 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/quotes.py
--rw-r--r--   0        0        0    23756 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/reference.py
--rw-r--r--   0        0        0     7816 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/snapshot.py
--rw-r--r--   0        0        0     1201 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/summaries.py
--rw-r--r--   0        0        0     4127 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/trades.py
--rw-r--r--   0        0        0     3799 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/rest/vX.py
--rw-r--r--   0        0        0     9678 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/websocket/__init__.py
--rw-r--r--   0        0        0     1612 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/websocket/models/__init__.py
--rw-r--r--   0        0        0      719 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/websocket/models/common.py
--rw-r--r--   0        0        0     9844 2023-05-17 15:05:24.043156 polygon_api_client-1.8.6/polygon/websocket/models/models.py
--rw-r--r--   0        0        0     1005 2023-05-17 15:05:49.435358 polygon_api_client-1.8.6/pyproject.toml
--rw-r--r--   0        0        0      837 1970-01-01 00:00:00.000000 polygon_api_client-1.8.6/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-20 19:46:59.600176 polygon_api_client-1.9/LICENSE
+-rw-r--r--   0        0        0      148 2023-05-20 19:46:59.604176 polygon_api_client-1.9/polygon/__init__.py
+-rw-r--r--   0        0        0      256 2023-05-20 19:46:59.604176 polygon_api_client-1.9/polygon/exceptions.py
+-rw-r--r--   0        0        0      329 2023-05-20 19:46:59.604176 polygon_api_client-1.9/polygon/logging.py
+-rw-r--r--   0        0        0      561 2023-05-20 19:46:59.604176 polygon_api_client-1.9/polygon/modelclass.py
+-rw-r--r--   0        0        0     1791 2023-05-20 19:46:59.604176 polygon_api_client-1.9/polygon/rest/__init__.py
+-rw-r--r--   0        0        0     8840 2023-05-20 19:46:59.604176 polygon_api_client-1.9/polygon/rest/aggs.py
+-rw-r--r--   0        0        0     7446 2023-05-20 19:46:59.604176 polygon_api_client-1.9/polygon/rest/base.py
+-rw-r--r--   0        0        0    12601 2023-05-20 19:46:59.604176 polygon_api_client-1.9/polygon/rest/indicators.py
+-rw-r--r--   0        0        0      356 2023-05-20 19:46:59.604176 polygon_api_client-1.9/polygon/rest/models/__init__.py
+-rw-r--r--   0        0        0     3408 2023-05-20 19:46:59.604176 polygon_api_client-1.9/polygon/rest/models/aggs.py
+-rw-r--r--   0        0        0     1530 2023-05-20 19:46:59.604176 polygon_api_client-1.9/polygon/rest/models/common.py
+-rw-r--r--   0        0        0     2755 2023-05-20 19:46:59.604176 polygon_api_client-1.9/polygon/rest/models/conditions.py
+-rw-r--r--   0        0        0     1784 2023-05-20 19:46:59.604176 polygon_api_client-1.9/polygon/rest/models/contracts.py
+-rw-r--r--   0        0        0      645 2023-05-20 19:46:59.604176 polygon_api_client-1.9/polygon/rest/models/dividends.py
+-rw-r--r--   0        0        0      569 2023-05-20 19:46:59.604176 polygon_api_client-1.9/polygon/rest/models/exchanges.py
+-rw-r--r--   0        0        0    10103 2023-05-20 19:46:59.604176 polygon_api_client-1.9/polygon/rest/models/financials.py
+-rw-r--r--   0        0        0     2399 2023-05-20 19:46:59.604176 polygon_api_client-1.9/polygon/rest/models/indicators.py
+-rw-r--r--   0        0        0     2499 2023-05-20 19:46:59.604176 polygon_api_client-1.9/polygon/rest/models/markets.py
+-rw-r--r--   0        0        0     3434 2023-05-20 19:46:59.604176 polygon_api_client-1.9/polygon/rest/models/quotes.py
+-rw-r--r--   0        0        0     3687 2023-05-20 19:46:59.604176 polygon_api_client-1.9/polygon/rest/models/request.py
+-rw-r--r--   0        0        0    13533 2023-05-20 19:46:59.604176 polygon_api_client-1.9/polygon/rest/models/snapshot.py
+-rw-r--r--   0        0        0      446 2023-05-20 19:46:59.604176 polygon_api_client-1.9/polygon/rest/models/splits.py
+-rw-r--r--   0        0        0     2269 2023-05-20 19:46:59.604176 polygon_api_client-1.9/polygon/rest/models/summaries.py
+-rw-r--r--   0        0        0     6892 2023-05-20 19:46:59.604176 polygon_api_client-1.9/polygon/rest/models/tickers.py
+-rw-r--r--   0        0        0     2051 2023-05-20 19:46:59.604176 polygon_api_client-1.9/polygon/rest/models/trades.py
+-rw-r--r--   0        0        0     5129 2023-05-20 19:46:59.604176 polygon_api_client-1.9/polygon/rest/quotes.py
+-rw-r--r--   0        0        0    23756 2023-05-20 19:46:59.604176 polygon_api_client-1.9/polygon/rest/reference.py
+-rw-r--r--   0        0        0     9805 2023-05-20 19:46:59.604176 polygon_api_client-1.9/polygon/rest/snapshot.py
+-rw-r--r--   0        0        0     1201 2023-05-20 19:46:59.604176 polygon_api_client-1.9/polygon/rest/summaries.py
+-rw-r--r--   0        0        0     4127 2023-05-20 19:46:59.604176 polygon_api_client-1.9/polygon/rest/trades.py
+-rw-r--r--   0        0        0     3799 2023-05-20 19:46:59.604176 polygon_api_client-1.9/polygon/rest/vX.py
+-rw-r--r--   0        0        0     9678 2023-05-20 19:46:59.604176 polygon_api_client-1.9/polygon/websocket/__init__.py
+-rw-r--r--   0        0        0     1612 2023-05-20 19:46:59.604176 polygon_api_client-1.9/polygon/websocket/models/__init__.py
+-rw-r--r--   0        0        0      719 2023-05-20 19:46:59.604176 polygon_api_client-1.9/polygon/websocket/models/common.py
+-rw-r--r--   0        0        0     9844 2023-05-20 19:46:59.604176 polygon_api_client-1.9/polygon/websocket/models/models.py
+-rw-r--r--   0        0        0     1003 2023-05-20 19:47:17.868298 polygon_api_client-1.9/pyproject.toml
+-rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 polygon_api_client-1.9/PKG-INFO
```

### Comparing `polygon_api_client-1.8.6/LICENSE` & `polygon_api_client-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.6/polygon/modelclass.py` & `polygon_api_client-1.9/polygon/modelclass.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.6/polygon/rest/__init__.py` & `polygon_api_client-1.9/polygon/rest/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     ExchangesClient,
     ContractsClient,
 )
 from .vX import VXClient
 from typing import Optional, Any
 import os
 
-
 BASE = "https://api.polygon.io"
 ENV_KEY = "POLYGON_API_KEY"
 
 
 class RESTClient(
     AggsClient,
     TradesClient,
@@ -42,29 +41,32 @@
         api_key: Optional[str] = os.getenv(ENV_KEY),
         connect_timeout: float = 10.0,
         read_timeout: float = 10.0,
         num_pools: int = 10,
         retries: int = 3,
         base: str = BASE,
         verbose: bool = False,
+        trace: bool = False,
         custom_json: Optional[Any] = None,
     ):
         super().__init__(
             api_key=api_key,
             connect_timeout=connect_timeout,
             read_timeout=read_timeout,
             num_pools=num_pools,
             retries=retries,
             base=base,
             verbose=verbose,
+            trace=trace,
             custom_json=custom_json,
         )
         self.vx = VXClient(
             api_key=api_key,
             connect_timeout=connect_timeout,
             read_timeout=read_timeout,
             num_pools=num_pools,
             retries=retries,
             base=base,
             verbose=verbose,
+            trace=trace,
             custom_json=custom_json,
         )
```

### Comparing `polygon_api_client-1.8.6/polygon/rest/aggs.py` & `polygon_api_client-1.9/polygon/rest/aggs.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.6/polygon/rest/base.py` & `polygon_api_client-1.9/polygon/rest/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from enum import Enum
 from typing import Optional, Any, Dict
 from datetime import datetime
 import pkg_resources  # part of setuptools
 from .models.request import RequestOptionBuilder
 from ..logging import get_logger
 import logging
+from urllib.parse import urlencode
 from ..exceptions import AuthError, BadResponse, NoResultsError
 
 logger = get_logger("RESTClient")
 version = "unknown"
 try:
     version = pkg_resources.require("polygon-api-client")[0].version
 except:
@@ -25,14 +26,15 @@
         api_key: Optional[str],
         connect_timeout: float,
         read_timeout: float,
         num_pools: int,
         retries: int,
         base: str,
         verbose: bool,
+        trace: bool,
         custom_json: Optional[Any] = None,
     ):
         if api_key is None:
             raise AuthError(
                 f"Must specify env var POLYGON_API_KEY or pass api_key in constructor"
             )
 
@@ -54,14 +56,15 @@
             cert_reqs="CERT_REQUIRED",
         )
 
         self.timeout = urllib3.Timeout(connect=connect_timeout, read=read_timeout)
         self.retries = retries
         if verbose:
             logger.setLevel(logging.DEBUG)
+        self.trace = trace
         if custom_json:
             self.json = custom_json
         else:
             self.json = json
 
     def _decode(self, resp):
         return self.json.loads(resp.data.decode("utf-8"))
@@ -73,22 +76,40 @@
         result_key: Optional[str] = None,
         deserializer=None,
         raw: bool = False,
         options: Optional[RequestOptionBuilder] = None,
     ) -> Any:
         option = options if options is not None else RequestOptionBuilder()
 
+        headers = self._concat_headers(option.headers)
+
+        if self.trace:
+            full_url = f"{self.BASE}{path}"
+            if params:
+                full_url += f"?{urlencode(params)}"
+            print_headers = headers.copy()
+            if "Authorization" in print_headers:
+                print_headers["Authorization"] = print_headers["Authorization"].replace(
+                    self.API_KEY, "REDACTED"
+                )
+            print(f"Request URL: {full_url}")
+            print(f"Request Headers: {print_headers}")
+
         resp = self.client.request(
             "GET",
             self.BASE + path,
             fields=params,
             retries=self.retries,
-            headers=self._concat_headers(option.headers),
+            headers=headers,
         )
 
+        if self.trace:
+            resp_headers_dict = dict(resp.headers.items())
+            print(f"Response Headers: {resp_headers_dict}")
+
         if resp.status != 200:
             raise BadResponse(resp.data.decode("utf-8"))
 
         if raw:
             return resp
 
         obj = self._decode(resp)
```

### Comparing `polygon_api_client-1.8.6/polygon/rest/indicators.py` & `polygon_api_client-1.9/polygon/rest/indicators.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.6/polygon/rest/models/aggs.py` & `polygon_api_client-1.9/polygon/rest/models/aggs.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.6/polygon/rest/models/common.py` & `polygon_api_client-1.9/polygon/rest/models/common.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.6/polygon/rest/models/conditions.py` & `polygon_api_client-1.9/polygon/rest/models/conditions.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.6/polygon/rest/models/contracts.py` & `polygon_api_client-1.9/polygon/rest/models/contracts.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.6/polygon/rest/models/dividends.py` & `polygon_api_client-1.9/polygon/rest/models/dividends.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.6/polygon/rest/models/exchanges.py` & `polygon_api_client-1.9/polygon/rest/models/exchanges.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.6/polygon/rest/models/financials.py` & `polygon_api_client-1.9/polygon/rest/models/financials.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.6/polygon/rest/models/indicators.py` & `polygon_api_client-1.9/polygon/rest/models/indicators.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.6/polygon/rest/models/markets.py` & `polygon_api_client-1.9/polygon/rest/models/markets.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.6/polygon/rest/models/quotes.py` & `polygon_api_client-1.9/polygon/rest/models/quotes.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.6/polygon/rest/models/request.py` & `polygon_api_client-1.9/polygon/rest/models/request.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.6/polygon/rest/models/snapshot.py` & `polygon_api_client-1.9/polygon/websocket/models/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,279 +1,345 @@
-from typing import Optional, List, Dict
-from .aggs import Agg
-from .quotes import LastQuote
-from .trades import LastTrade
+from typing import Optional, List, Union, NewType
+from .common import EventType
 from ...modelclass import modelclass
 
 
 @modelclass
-class MinuteSnapshot:
-    "Most recent minute bar."
+class EquityAgg:
+    """EquityAgg contains aggregate data for either stock tickers, option contracts or index tickers."""
+
+    event_type: Optional[Union[str, EventType]] = None
+    symbol: Optional[str] = None
+    volume: Optional[float] = None
     accumulated_volume: Optional[float] = None
+    official_open_price: Optional[float] = None
+    vwap: Optional[float] = None
     open: Optional[float] = None
+    close: Optional[float] = None
     high: Optional[float] = None
     low: Optional[float] = None
-    close: Optional[float] = None
-    volume: Optional[float] = None
-    vwap: Optional[float] = None
+    aggregate_vwap: Optional[float] = None
+    average_size: Optional[float] = None
+    start_timestamp: Optional[int] = None
+    end_timestamp: Optional[int] = None
     otc: Optional[bool] = None
 
     @staticmethod
     def from_dict(d):
-        return MinuteSnapshot(
+        return EquityAgg(
+            d.get("ev", None),
+            d.get("sym", None),
+            d.get("v", None),
             d.get("av", None),
+            d.get("op", None),
+            d.get("vw", None),
             d.get("o", None),
+            d.get("c", None),
             d.get("h", None),
             d.get("l", None),
-            d.get("c", None),
-            d.get("v", None),
-            d.get("vw", None),
+            d.get("a", None),
+            d.get("z", None),
+            d.get("s", None),
+            d.get("e", None),
             d.get("otc", None),
         )
 
 
 @modelclass
-class IndicesSession:
-    "Contains data for the most recent daily bar in an options contract."
-    change: Optional[float] = None
-    change_percent: Optional[float] = None
+class CurrencyAgg:
+    "CurrencyAgg contains aggregate data for either forex currency pairs or crypto pairs."
+    event_type: Optional[Union[str, EventType]] = None
+    pair: Optional[str] = None
+    open: Optional[float] = None
     close: Optional[float] = None
     high: Optional[float] = None
     low: Optional[float] = None
-    open: Optional[float] = None
-    previous_close: Optional[float] = None
+    volume: Optional[float] = None
+    vwap: Optional[float] = None
+    start_timestamp: Optional[int] = None
+    end_timestamp: Optional[int] = None
+    avg_trade_size: Optional[float] = None
 
     @staticmethod
     def from_dict(d):
-        return IndicesSession(**d)
+        return CurrencyAgg(
+            d.get("ev", None),
+            d.get("pair", None),
+            d.get("o", None),
+            d.get("c", None),
+            d.get("h", None),
+            d.get("l", None),
+            d.get("v", None),
+            d.get("vw", None),
+            d.get("s", None),
+            d.get("e", None),
+            d.get("z", None),
+        )
 
 
 @modelclass
-class IndicesSnapshot:
-    value: Optional[float] = None
-    name: Optional[str] = None
-    type: Optional[str] = None
-    ticker: Optional[str] = None
-    market_status: Optional[str] = None
-    session: Optional[IndicesSession] = None
-    error: Optional[str] = None
-    message: Optional[str] = None
+class EquityTrade:
+    "EquityTrade contains trade data for either stock tickers or option contracts."
+    event_type: Optional[Union[str, EventType]] = None
+    symbol: Optional[str] = None
+    exchange: Optional[int] = None
+    id: Optional[str] = None
+    tape: Optional[int] = None
+    price: Optional[float] = None
+    size: Optional[int] = None
+    conditions: Optional[List[int]] = None
+    timestamp: Optional[int] = None
+    sequence_number: Optional[int] = None
+    trf_id: Optional[int] = None
+    trf_timestamp: Optional[int] = None
 
     @staticmethod
     def from_dict(d):
-        return IndicesSnapshot(
-            value=d.get("value", None),
-            name=d.get("name", None),
-            type=d.get("type", None),
-            ticker=d.get("ticker", None),
-            market_status=d.get("market_status", None),
-            session=None
-            if "session" not in d
-            else IndicesSession.from_dict(d["session"]),
-            error=d.get("error", None),
-            message=d.get("message", None),
+        return EquityTrade(
+            d.get("ev", None),
+            d.get("sym", None),
+            d.get("x", None),
+            d.get("i", None),
+            d.get("z", None),
+            d.get("p", None),
+            d.get("s", None),
+            d.get("c", None),
+            d.get("t", None),
+            d.get("q", None),
+            d.get("trfi", None),
+            d.get("trft", None),
         )
 
 
 @modelclass
-class TickerSnapshot:
-    "Contains the most up-to-date market data for all traded ticker symbols."
-    day: Optional[Agg] = None
-    last_quote: Optional[LastQuote] = None
-    last_trade: Optional[LastTrade] = None
-    min: Optional[MinuteSnapshot] = None
-    prev_day: Optional[Agg] = None
-    ticker: Optional[str] = None
-    todays_change: Optional[float] = None
-    todays_change_percent: Optional[float] = None
-    updated: Optional[int] = None
+class CryptoTrade:
+    "CryptoTrade contains trade data for a crypto pair."
+    event_type: Optional[Union[str, EventType]] = None
+    pair: Optional[str] = None
+    exchange: Optional[int] = None
+    id: Optional[str] = None
+    price: Optional[float] = None
+    size: Optional[float] = None
+    conditions: Optional[List[int]] = None
+    timestamp: Optional[int] = None
+    received_timestamp: Optional[int] = None
 
     @staticmethod
     def from_dict(d):
-        return TickerSnapshot(
-            day=None if "day" not in d else Agg.from_dict(d["day"]),
-            last_quote=None
-            if "lastQuote" not in d
-            else LastQuote.from_dict(d["lastQuote"]),
-            last_trade=None
-            if "lastTrade" not in d
-            else LastTrade.from_dict(d["lastTrade"]),
-            min=None if "min" not in d else MinuteSnapshot.from_dict(d["min"]),
-            prev_day=None if "prevDay" not in d else Agg.from_dict(d["prevDay"]),
-            ticker=d.get("ticker", None),
-            todays_change=d.get("todaysChange", None),
-            todays_change_percent=d.get("todaysChangePerc", None),
-            updated=d.get("updated", None),
+        return CryptoTrade(
+            d.get("ev", None),
+            d.get("pair", None),
+            d.get("x", None),
+            d.get("i", None),
+            d.get("p", None),
+            d.get("s", None),
+            d.get("c", None),
+            d.get("t", None),
+            d.get("r", None),
         )
 
 
 @modelclass
-class DayOptionContractSnapshot:
-    "Contains data for the most recent daily bar in an options contract."
-    change: Optional[float] = None
-    change_percent: Optional[float] = None
-    close: Optional[float] = None
-    high: Optional[float] = None
-    last_updated: Optional[int] = None
-    low: Optional[float] = None
-    open: Optional[float] = None
-    previous_close: Optional[float] = None
-    volume: Optional[float] = None
-    vwap: Optional[float] = None
+class EquityQuote:
+    "EquityQuote contains quote data for either stock tickers or option contracts."
+    event_type: Optional[Union[str, EventType]] = None
+    symbol: Optional[str] = None
+    bid_exchange_id: Optional[int] = None
+    bid_price: Optional[float] = None
+    bid_size: Optional[int] = None
+    ask_exchange_id: Optional[int] = None
+    ask_price: Optional[float] = None
+    ask_size: Optional[int] = None
+    condition: Optional[int] = None
+    indicators: Optional[List[int]] = None
+    timestamp: Optional[int] = None
+    tape: Optional[int] = None
+    sequence_number: Optional[int] = None
+    trf_id: Optional[int] = None
+    trf_timestamp: Optional[int] = None
 
     @staticmethod
     def from_dict(d):
-        return DayOptionContractSnapshot(**d)
+        return EquityQuote(
+            d.get("ev", None),
+            d.get("sym", None),
+            d.get("bx", None),
+            d.get("bp", None),
+            d.get("bs", None),
+            d.get("ax", None),
+            d.get("ap", None),
+            d.get("as", None),
+            d.get("c", None),
+            d.get("i", None),
+            d.get("t", None),
+            d.get("z", None),
+            d.get("q", None),
+            d.get("trfi", None),
+            d.get("trft", None),
+        )
 
 
 @modelclass
-class OptionDetails:
-    "Contains details for an options contract."
-    contract_type: Optional[str] = None
-    exercise_style: Optional[str] = None
-    expiration_date: Optional[str] = None
-    shares_per_contract: Optional[float] = None
-    strike_price: Optional[float] = None
-    ticker: Optional[str] = None
+class ForexQuote:
+    "ForexQuote contains quote data for a forex currency pair."
+    event_type: Optional[Union[str, EventType]] = None
+    pair: Optional[str] = None
+    exchange_id: Optional[int] = None
+    ask_price: Optional[float] = None
+    bid_price: Optional[float] = None
+    timestamp: Optional[int] = None
 
     @staticmethod
     def from_dict(d):
-        return OptionDetails(**d)
+        return ForexQuote(
+            d.get("ev", None),
+            d.get("p", None),
+            d.get("x", None),
+            d.get("a", None),
+            d.get("b", None),
+            d.get("t", None),
+        )
 
 
 @modelclass
-class LastQuoteOptionContractSnapshot:
-    "Contains data for the most recent quote in an options contract."
-    ask: Optional[float] = None
-    ask_size: Optional[float] = None
-    bid: Optional[float] = None
+class CryptoQuote:
+    "CryptoQuote contains quote data for a crypto pair."
+    event_type: Optional[Union[str, EventType]] = None
+    pair: Optional[str] = None
+    bid_price: Optional[int] = None
     bid_size: Optional[float] = None
-    last_updated: Optional[int] = None
-    midpoint: Optional[float] = None
-    timeframe: Optional[str] = None
-
-    @staticmethod
-    def from_dict(d):
-        return LastQuoteOptionContractSnapshot(**d)
-
-
-@modelclass
-class LastTradeOptionContractSnapshot:
-    "Contains data for the most recent trade for an options contract."
-    price: Optional[float] = None
-    sip_timestamp: Optional[int] = None
-    size: Optional[int] = None
-    conditions: Optional[List[int]] = None
-    exchange: Optional[int] = None
-    timeframe: Optional[str] = None
-
-    @staticmethod
-    def from_dict(d):
-        return LastTradeOptionContractSnapshot(**d)
-
-
-@modelclass
-class Greeks:
-    "Contains data for the greeks in an options contract."
-    delta: Optional[float] = None
-    gamma: Optional[float] = None
-    theta: Optional[float] = None
-    vega: Optional[float] = None
+    ask_price: Optional[int] = None
+    ask_size: Optional[int] = None
+    timestamp: Optional[float] = None
+    exchange_id: Optional[int] = None
+    received_timestamp: Optional[int] = None
 
     @staticmethod
     def from_dict(d):
-        return Greeks(**d)
+        return CryptoQuote(
+            d.get("ev", None),
+            d.get("pair", None),
+            d.get("bp", None),
+            d.get("bs", None),
+            d.get("ap", None),
+            d.get("as", None),
+            d.get("t", None),
+            d.get("x", None),
+            d.get("r", None),
+        )
 
 
 @modelclass
-class UnderlyingAsset:
-    "Contains data for the underlying stock in an options contract."
-    change_to_break_even: Optional[float] = None
-    last_updated: Optional[int] = None
-    price: Optional[float] = None
-    value: Optional[float] = None
-    ticker: Optional[str] = None
-    timeframe: Optional[str] = None
+class Imbalance:
+    "Imbalance contains imbalance event data for a given stock ticker symbol."
+    event_type: Optional[Union[str, EventType]] = None
+    symbol: Optional[str] = None
+    time_stamp: Optional[int] = None
+    auction_time: Optional[int] = None
+    auction_type: Optional[str] = None
+    symbol_sequence: Optional[int] = None
+    exchange_id: Optional[int] = None
+    imbalance_quantity: Optional[int] = None
+    paired_quantity: Optional[int] = None
+    book_clearing_price: Optional[float] = None
 
     @staticmethod
     def from_dict(d):
-        return UnderlyingAsset(**d)
+        return Imbalance(
+            d.get("ev", None),
+            d.get("T", None),
+            d.get("t", None),
+            d.get("at", None),
+            d.get("a", None),
+            d.get("i", None),
+            d.get("x", None),
+            d.get("o", None),
+            d.get("p", None),
+            d.get("b", None),
+        )
 
 
 @modelclass
-class OptionContractSnapshot:
-    "Contains data for the snapshot of an option contract of a stock equity."
-    break_even_price: Optional[float] = None
-    day: Optional[DayOptionContractSnapshot] = None
-    details: Optional[OptionDetails] = None
-    greeks: Optional[Greeks] = None
-    implied_volatility: Optional[float] = None
-    last_quote: Optional[LastQuoteOptionContractSnapshot] = None
-    last_trade: Optional[LastTradeOptionContractSnapshot] = None
-    open_interest: Optional[float] = None
-    underlying_asset: Optional[UnderlyingAsset] = None
+class LimitUpLimitDown:
+    "LimitUpLimitDown contains LULD event data for a given stock ticker symbol."
+    event_type: Optional[Union[str, EventType]] = None
+    symbol: Optional[str] = None
+    high_price: Optional[float] = None
+    low_price: Optional[float] = None
+    indicators: Optional[List[int]] = None
+    tape: Optional[int] = None
+    timestamp: Optional[int] = None
+    sequence_number: Optional[int] = None
 
     @staticmethod
     def from_dict(d):
-        return OptionContractSnapshot(
-            break_even_price=d.get("break_even_price", None),
-            day=None
-            if "day" not in d
-            else DayOptionContractSnapshot.from_dict(d["day"]),
-            details=None
-            if "details" not in d
-            else OptionDetails.from_dict(d["details"]),
-            greeks=None if "greeks" not in d else Greeks.from_dict(d["greeks"]),
-            implied_volatility=d.get("implied_volatility", None),
-            last_quote=None
-            if "last_quote" not in d
-            else LastQuoteOptionContractSnapshot.from_dict(d["last_quote"]),
-            last_trade=None
-            if "last_trade" not in d
-            else LastTradeOptionContractSnapshot.from_dict(d["last_trade"]),
-            open_interest=d.get("open_interest", None),
-            underlying_asset=None
-            if "underlying_asset" not in d
-            else UnderlyingAsset.from_dict(d["underlying_asset"]),
+        return LimitUpLimitDown(
+            d.get("ev", None),
+            d.get("T", None),
+            d.get("h", None),
+            d.get("l", None),
+            d.get("i", None),
+            d.get("z", None),
+            d.get("t", None),
+            d.get("q", None),
         )
 
 
 @modelclass
-class OrderBookQuote:
-    "Contains data for a book bid or ask."
-    price: Optional[float] = None
-    exchange_shares: Optional[Dict[str, float]] = None
+class Level2Book:
+    "Level2Book contains level 2 book data for a given crypto pair."
+    event_type: Optional[Union[str, EventType]] = None
+    pair: Optional[str] = None
+    bid_prices: Optional[float] = None
+    ask_prices: Optional[float] = None
+    timestamp: Optional[int] = None
+    exchange_id: Optional[int] = None
+    received_timestamp: Optional[int] = None
 
     @staticmethod
     def from_dict(d):
-        return OrderBookQuote(
-            d.get("p", None),
+        return Level2Book(
+            d.get("ev", None),
+            d.get("pair", None),
+            d.get("b", None),
+            d.get("a", None),
+            d.get("t", None),
             d.get("x", None),
+            d.get("r", None),
         )
 
 
 @modelclass
-class SnapshotTickerFullBook:
-    "Contains the current level 2 book of a single ticker. This is the combined book from all of the exchanges."
+class IndexValue:
+    event_type: Optional[Union[str, EventType]] = None
+    value: Optional[float] = None
     ticker: Optional[str] = None
-    bids: Optional[List[OrderBookQuote]] = None
-    asks: Optional[List[OrderBookQuote]] = None
-    bid_count: Optional[float] = None
-    ask_count: Optional[float] = None
-    spread: Optional[float] = None
-    updated: Optional[int] = None
+    timestamp: Optional[str] = None
 
     @staticmethod
     def from_dict(d):
-        return SnapshotTickerFullBook(
-            ticker=d.get("ticker", None),
-            bids=None
-            if "bids" not in d
-            else [OrderBookQuote.from_dict(o) for o in d["bids"]],
-            asks=None
-            if "asks" not in d
-            else [OrderBookQuote.from_dict(o) for o in d["asks"]],
-            bid_count=d.get("bidCount", None),
-            ask_count=d.get("askCount", None),
-            spread=d.get("spread", None),
-            updated=d.get("updated", None),
+        return IndexValue(
+            d.get("ev", None),
+            d.get("val", None),
+            d.get("T", None),
+            d.get("t", None),
         )
+
+
+WebSocketMessage = NewType(
+    "WebSocketMessage",
+    List[
+        Union[
+            EquityAgg,
+            CurrencyAgg,
+            EquityTrade,
+            CryptoTrade,
+            EquityQuote,
+            ForexQuote,
+            CryptoQuote,
+            Imbalance,
+            LimitUpLimitDown,
+            Level2Book,
+            IndexValue,
+        ]
+    ],
+)
```

### Comparing `polygon_api_client-1.8.6/polygon/rest/models/summaries.py` & `polygon_api_client-1.9/polygon/rest/models/summaries.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.6/polygon/rest/models/tickers.py` & `polygon_api_client-1.9/polygon/rest/models/tickers.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.6/polygon/rest/models/trades.py` & `polygon_api_client-1.9/polygon/rest/models/trades.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.6/polygon/rest/quotes.py` & `polygon_api_client-1.9/polygon/rest/quotes.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.6/polygon/rest/reference.py` & `polygon_api_client-1.9/polygon/rest/reference.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.6/polygon/rest/snapshot.py` & `polygon_api_client-1.9/polygon/rest/snapshot.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Optional, Any, Dict, List, Union, Iterator
 from .models import (
     TickerSnapshot,
     Direction,
     OptionContractSnapshot,
     SnapshotMarketType,
     SnapshotTickerFullBook,
+    UniversalSnapshot,
     IndicesSnapshot,
 )
 from urllib3 import HTTPResponse
 
 from .models.request import RequestOptionBuilder
 
 
@@ -17,14 +18,56 @@
     if market_type == SnapshotMarketType.STOCKS.value:
         return "us"
 
     return "global"
 
 
 class SnapshotClient(BaseClient):
+    def list_universal_snapshots(
+        self,
+        market_type: Optional[Union[str, SnapshotMarketType]] = None,
+        ticker_any_of: Optional[List[str]] = None,
+        ticker_lt: Optional[str] = None,
+        ticker_lte: Optional[str] = None,
+        ticker_gt: Optional[str] = None,
+        ticker_gte: Optional[str] = None,
+        params: Optional[Dict[str, Any]] = None,
+        raw: bool = False,
+        options: Optional[RequestOptionBuilder] = None,
+    ) -> Union[Iterator[UniversalSnapshot], HTTPResponse]:
+        """
+        Get snapshots for assets of all types
+        - https://polygon.io/docs/stocks/get_v3_snapshot
+        - https://polygon.io/docs/options/get_v3_snapshot
+        - https://polygon.io/docs/indices/get_v3_snapshot
+        - https://polygon.io/docs/forex/get_v3_snapshot
+        - https://polygon.io/docs/crypto/get_v3_snapshot
+
+        :param market_type: the type of the asset
+        :param ticker_any_of: Comma-separated list of tickers, up to a maximum of 250. If no tickers are passed then all
+        results will be returned in a paginated manner. Warning: The maximum number of characters allowed in a URL
+        are subject to your technology stack.
+        :param ticker_lt search for tickers less than
+        :param ticker_lte search for tickers less than or equal to
+        :param ticker_gt search for tickers greater than
+        :param ticker_gte search for tickers greater than or equal to
+        :param raw: returns the raw HTTP response if true, else the response is deserialized into a structured object
+        :param options: request options
+        :return: list of Snapshots
+        """
+        url = f"/v3/snapshot"
+        return self._paginate(
+            path=url,
+            params=self._get_params(self.list_universal_snapshots, locals()),
+            result_key="results",
+            deserializer=UniversalSnapshot.from_dict,
+            raw=raw,
+            options=options,
+        )
+
     def get_snapshot_all(
         self,
         market_type: Union[str, SnapshotMarketType],
         tickers: Optional[Union[str, List[str]]] = None,
         params: Optional[Dict[str, Any]] = None,
         raw: bool = False,
         include_otc: Optional[bool] = False,
```

### Comparing `polygon_api_client-1.8.6/polygon/rest/summaries.py` & `polygon_api_client-1.9/polygon/rest/summaries.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.6/polygon/rest/trades.py` & `polygon_api_client-1.9/polygon/rest/trades.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.6/polygon/rest/vX.py` & `polygon_api_client-1.9/polygon/rest/vX.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.6/polygon/websocket/__init__.py` & `polygon_api_client-1.9/polygon/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.6/polygon/websocket/models/__init__.py` & `polygon_api_client-1.9/polygon/websocket/models/__init__.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.6/polygon/websocket/models/common.py` & `polygon_api_client-1.9/polygon/websocket/models/common.py`

 * *Files identical despite different names*

### Comparing `polygon_api_client-1.8.6/pyproject.toml` & `polygon_api_client-1.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polygon-api-client"
-version = "v1.8.6"
+version = "v1.9"
 description = "Official Polygon.io REST and Websocket client."
 authors = ["polygon.io"]
 license = "MIT"
 homepage = "https://polygon.io"
 repository = "https://github.com/polygon-io/client-python"
 documentation = "https://polygon.io/docs"
 keywords = [
@@ -32,16 +32,16 @@
 [tool.poetry.dev-dependencies]
 black = "^22.12.0"
 mypy = "^1.0"
 types-urllib3 = "^1.26.25"
 Sphinx = "^5.3.0"
 sphinx-rtd-theme = "^1.0.0"
 # keep this in sync with docs/requirements.txt for readthedocs.org
-sphinx-autodoc-typehints = "^1.19.2"
+sphinx-autodoc-typehints = "^1.23.0"
 types-certifi = "^2021.10.8"
 types-setuptools = "^67.4.0"
-pook = "^1.0.2"
+pook = "^1.1.1"
 orjson = "^3.8.7"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `polygon_api_client-1.8.6/PKG-INFO` & `polygon_api_client-1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polygon-api-client
-Version: 1.8.6
+Version: 1.9
 Summary: Official Polygon.io REST and Websocket client.
 Home-page: https://polygon.io
 License: MIT
 Keywords: polygon,free,rest,stock,market,data,api,polygon.io,websocket,client
 Author: polygon.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

