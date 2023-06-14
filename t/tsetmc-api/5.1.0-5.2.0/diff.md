# Comparing `tmp/tsetmc_api-5.1.0.tar.gz` & `tmp/tsetmc_api-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsetmc_api-5.1.0.tar", max compression
+gzip compressed data, was "tsetmc_api-5.2.0.tar", max compression
```

## Comparing `tsetmc_api-5.1.0.tar` & `tsetmc_api-5.2.0.tar`

### file list

```diff
@@ -1,40 +1,41 @@
--rw-r--r--   0        0        0     1098 2023-06-13 09:21:30.533244 tsetmc_api-5.1.0/LICENSE.md
--rw-r--r--   0        0        0     2705 2023-06-13 09:21:30.533244 tsetmc_api-5.1.0/README.md
--rw-r--r--   0        0        0       18 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/__init__.py
--rw-r--r--   0        0        0       36 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/day_details/__init__.py
--rw-r--r--   0        0        0     9279 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/day_details/_core.py
--rw-r--r--   0        0        0     5877 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/day_details/day_details.py
--rw-r--r--   0        0        0      438 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/day_details/orderbook.py
--rw-r--r--   0        0        0      460 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/day_details/price.py
--rw-r--r--   0        0        0     1842 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/day_details/shareholder.py
--rw-r--r--   0        0        0      114 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/day_details/threshold.py
--rw-r--r--   0        0        0      215 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/day_details/trade.py
--rw-r--r--   0        0        0      368 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/day_details/traders_type.py
--rw-r--r--   0        0        0       36 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/group/__init__.py
--rw-r--r--   0        0        0      481 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/group/_core.py
--rw-r--r--   0        0        0      739 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/group/group.py
--rw-r--r--   0        0        0       36 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/market_map/__init__.py
--rw-r--r--   0        0        0     1373 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/market_map/_core.py
--rw-r--r--   0        0        0     1628 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/market_map/map.py
--rw-r--r--   0        0        0       31 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/market_watch/__init__.py
--rw-r--r--   0        0        0    17109 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/market_watch/_core.py
--rw-r--r--   0        0        0      224 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/market_watch/daily_history.py
--rw-r--r--   0        0        0      227 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/market_watch/orderbook.py
--rw-r--r--   0        0        0      514 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/market_watch/price.py
--rw-r--r--   0        0        0      321 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/market_watch/traders_type.py
--rw-r--r--   0        0        0     5043 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/market_watch/watch.py
--rw-r--r--   0        0        0       27 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/symbol/__init__.py
--rw-r--r--   0        0        0    12706 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/symbol/_core.py
--rw-r--r--   0        0        0      164 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/symbol/group.py
--rw-r--r--   0        0        0      366 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/symbol/identification.py
--rw-r--r--   0        0        0      219 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/symbol/notification.py
--rw-r--r--   0        0        0      247 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/symbol/orderbook.py
--rw-r--r--   0        0        0     1004 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/symbol/price.py
--rw-r--r--   0        0        0     1887 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/symbol/shareholder.py
--rw-r--r--   0        0        0      221 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/symbol/state_change.py
--rw-r--r--   0        0        0      240 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/symbol/supervisor_message.py
--rw-r--r--   0        0        0     9693 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/symbol/symbol.py
--rw-r--r--   0        0        0      453 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/symbol/traders_type.py
--rw-r--r--   0        0        0      874 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/lib/tsetmc_api/utils.py
--rw-r--r--   0        0        0      745 2023-06-13 09:21:30.573244 tsetmc_api-5.1.0/pyproject.toml
--rw-r--r--   0        0        0     3663 1970-01-01 00:00:00.000000 tsetmc_api-5.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-06-14 19:52:29.642076 tsetmc_api-5.2.0/LICENSE.md
+-rw-r--r--   0        0        0     2858 2023-06-14 19:52:29.642076 tsetmc_api-5.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/__init__.py
+-rw-r--r--   0        0        0       36 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/day_details/__init__.py
+-rw-r--r--   0        0        0     9345 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/day_details/_core.py
+-rw-r--r--   0        0        0     5926 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/day_details/day_details.py
+-rw-r--r--   0        0        0      438 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/day_details/orderbook.py
+-rw-r--r--   0        0        0      460 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/day_details/price.py
+-rw-r--r--   0        0        0     1842 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/day_details/shareholder.py
+-rw-r--r--   0        0        0      231 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/day_details/threshold.py
+-rw-r--r--   0        0        0      215 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/day_details/trade.py
+-rw-r--r--   0        0        0      368 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/day_details/traders_type.py
+-rw-r--r--   0        0        0       36 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/group/__init__.py
+-rw-r--r--   0        0        0      481 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/group/_core.py
+-rw-r--r--   0        0        0      739 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/group/group.py
+-rw-r--r--   0        0        0       36 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/market_map/__init__.py
+-rw-r--r--   0        0        0     1373 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/market_map/_core.py
+-rw-r--r--   0        0        0     1628 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/market_map/map.py
+-rw-r--r--   0        0        0       31 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/market_watch/__init__.py
+-rw-r--r--   0        0        0    17109 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/market_watch/_core.py
+-rw-r--r--   0        0        0      224 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/market_watch/daily_history.py
+-rw-r--r--   0        0        0      227 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/market_watch/orderbook.py
+-rw-r--r--   0        0        0      514 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/market_watch/price.py
+-rw-r--r--   0        0        0      321 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/market_watch/traders_type.py
+-rw-r--r--   0        0        0     5043 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/market_watch/watch.py
+-rw-r--r--   0        0        0       27 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/symbol/__init__.py
+-rw-r--r--   0        0        0    12706 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/symbol/_core.py
+-rw-r--r--   0        0        0      164 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/symbol/group.py
+-rw-r--r--   0        0        0      366 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/symbol/identification.py
+-rw-r--r--   0        0        0      219 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/symbol/notification.py
+-rw-r--r--   0        0        0      247 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/symbol/orderbook.py
+-rw-r--r--   0        0        0     1004 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/symbol/price.py
+-rw-r--r--   0        0        0     1887 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/symbol/shareholder.py
+-rw-r--r--   0        0        0      221 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/symbol/state_change.py
+-rw-r--r--   0        0        0      240 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/symbol/supervisor_message.py
+-rw-r--r--   0        0        0     9693 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/symbol/symbol.py
+-rw-r--r--   0        0        0      453 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/symbol/traders_type.py
+-rw-r--r--   0        0        0      933 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/utils.py
+-rw-r--r--   0        0        0       18 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/version.py
+-rw-r--r--   0        0        0      745 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3816 1970-01-01 00:00:00.000000 tsetmc_api-5.2.0/PKG-INFO
```

### Comparing `tsetmc_api-5.1.0/LICENSE.md` & `tsetmc_api-5.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tsetmc_api-5.1.0/README.md` & `tsetmc_api-5.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -62,7 +62,11 @@
 - [x] Migrate `market_map` component to use new tsetmc.
 - [x] Migrate `group` component to use new tsetmc.
 - [ ] Support asyncio.
 
 ## Support and Donation
 
 If this repository helped you, please support it by giving a star (:star:).
+
+For contacting me about this project please use the following email:
+
+[mahdi74sadeghi+tsetmc_api@gmail.com](mailto:mahdi74sadeghi+tsetmc_api@gmail.com)
```

### Comparing `tsetmc_api-5.1.0/lib/tsetmc_api/day_details/_core.py` & `tsetmc_api-5.2.0/lib/tsetmc_api/day_details/_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -177,32 +177,33 @@
                 'value': response['sell_I_Value'],
                 'count': response['sell_I_Count'],
             }
         },
     }
 
 
-def get_day_details_thresholds_data(symbol_id: str, date: jdate) -> dict:
+def get_day_details_thresholds_data(symbol_id: str, date: jdate) -> list[dict]:
     t = date.togregorian().strftime('%Y%m%d')
     response = requests.get(
         url=f'http://cdn.tsetmc.com/api/MarketData/GetStaticThreshold/{symbol_id}/{t}',
         params={},
         headers={
             'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36',
         },
         verify=False,
         timeout=20,
     )
     response.raise_for_status()
     response = response.json()['staticThreshold']
 
-    return {
-        'max': response[1]['psGelStaMax'],
-        'min': response[1]['psGelStaMin'],
-    }
+    return [{
+        'time': convert_heven_to_jtime(rsp['hEven']),
+        'max': rsp['psGelStaMax'],
+        'min': rsp['psGelStaMin'],
+    } for rsp in response]
 
 
 def get_day_details_shareholders_data(symbol_id: str, date: jdate) -> tuple[list[dict], list[dict]]:
     t = date.togregorian().strftime('%Y%m%d')
     response = requests.get(
         url=f'http://cdn.tsetmc.com/api/Shareholder/{symbol_id}/{t}',
         params={},
```

### Comparing `tsetmc_api-5.1.0/lib/tsetmc_api/day_details/day_details.py` & `tsetmc_api-5.2.0/lib/tsetmc_api/day_details/day_details.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,20 +116,22 @@
 
         return [DayDetailsTradeDataRow(
             time=row['time'],
             price=row['price'],
             volume=row['volume'],
         ) for row in raw_data]
 
-    def get_thresholds_data(self) -> DayDetailsThresholdsData:
+    def get_thresholds_data(self) -> list[DayDetailsThresholdsData]:
         raw_data = _core.get_day_details_thresholds_data(symbol_id=self.symbol_id, date=self.date)
-        return DayDetailsThresholdsData(
-            range_max=raw_data['max'],
-            range_min=raw_data['min'],
-        )
+
+        return [DayDetailsThresholdsData(
+            time=row['time'],
+            range_max=row['max'],
+            range_min=row['min'],
+        ) for row in raw_data]
 
     def get_shareholders_data(self) -> tuple[list[DayDetailsShareHolderDataRow], list[DayDetailsShareHolderDataRow]]:
         """
         gets list of shareholders before and after the day
         """
 
         raw_old_shareholders, raw_new_shareholders = _core.get_day_details_shareholders_data(
```

### Comparing `tsetmc_api-5.1.0/lib/tsetmc_api/day_details/shareholder.py` & `tsetmc_api-5.2.0/lib/tsetmc_api/day_details/shareholder.py`

 * *Files identical despite different names*

### Comparing `tsetmc_api-5.1.0/lib/tsetmc_api/group/group.py` & `tsetmc_api-5.2.0/lib/tsetmc_api/group/group.py`

 * *Files identical despite different names*

### Comparing `tsetmc_api-5.1.0/lib/tsetmc_api/market_map/_core.py` & `tsetmc_api-5.2.0/lib/tsetmc_api/market_map/_core.py`

 * *Files identical despite different names*

### Comparing `tsetmc_api-5.1.0/lib/tsetmc_api/market_map/map.py` & `tsetmc_api-5.2.0/lib/tsetmc_api/market_map/map.py`

 * *Files identical despite different names*

### Comparing `tsetmc_api-5.1.0/lib/tsetmc_api/market_watch/_core.py` & `tsetmc_api-5.2.0/lib/tsetmc_api/market_watch/_core.py`

 * *Files identical despite different names*

### Comparing `tsetmc_api-5.1.0/lib/tsetmc_api/market_watch/price.py` & `tsetmc_api-5.2.0/lib/tsetmc_api/market_watch/price.py`

 * *Files identical despite different names*

### Comparing `tsetmc_api-5.1.0/lib/tsetmc_api/market_watch/watch.py` & `tsetmc_api-5.2.0/lib/tsetmc_api/market_watch/watch.py`

 * *Files identical despite different names*

### Comparing `tsetmc_api-5.1.0/lib/tsetmc_api/symbol/_core.py` & `tsetmc_api-5.2.0/lib/tsetmc_api/symbol/_core.py`

 * *Files identical despite different names*

### Comparing `tsetmc_api-5.1.0/lib/tsetmc_api/symbol/price.py` & `tsetmc_api-5.2.0/lib/tsetmc_api/symbol/price.py`

 * *Files identical despite different names*

### Comparing `tsetmc_api-5.1.0/lib/tsetmc_api/symbol/shareholder.py` & `tsetmc_api-5.2.0/lib/tsetmc_api/symbol/shareholder.py`

 * *Files identical despite different names*

### Comparing `tsetmc_api-5.1.0/lib/tsetmc_api/symbol/symbol.py` & `tsetmc_api-5.2.0/lib/tsetmc_api/symbol/symbol.py`

 * *Files identical despite different names*

### Comparing `tsetmc_api-5.1.0/lib/tsetmc_api/utils.py` & `tsetmc_api-5.2.0/lib/tsetmc_api/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,20 +13,22 @@
             ret[key] = deep_update(d1=d1[key], d2=value)
         else:
             ret[key] = value
 
     return ret
 
 
-def convert_heven_to_jtime(heven: int) -> jtime:
+def convert_heven_to_jtime(heven: int | str) -> jtime | None:
     heven = str(heven)
     if len(heven) == 6:
         return jtime(hour=int(heven[:2]), minute=int(heven[2:4]), second=int(heven[4:]))
-    else:
+    elif len(heven) == 5:
         return jtime(hour=int(heven[:1]), minute=int(heven[1:3]), second=int(heven[3:]))
+    else:
+        return None
 
 
 def convert_deven_to_jdate(deven: int) -> jdate:
     deven = str(deven)
     return jdate.fromgregorian(
         year=int(deven[:4]),
         month=int(deven[4:6]),
```

### Comparing `tsetmc_api-5.1.0/pyproject.toml` & `tsetmc_api-5.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tsetmc-api"
-version = "5.1.0"
+version = "5.2.0"
 description = "simple package to communicate and crawl data from tsetmc.com (Tehran Stock Exchange Website)"
 license = "MIT"
 repository = "https://github.com/mahs4d/tsetmc-api"
 authors = ["Mahdi Sadeghi <mahdi74sadeghi@gmail.com>"]
 packages = [
     { include = "tsetmc_api", from = "lib" },
 ]
```

### Comparing `tsetmc_api-5.1.0/PKG-INFO` & `tsetmc_api-5.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsetmc-api
-Version: 5.1.0
+Version: 5.2.0
 Summary: simple package to communicate and crawl data from tsetmc.com (Tehran Stock Exchange Website)
 Home-page: https://github.com/mahs4d/tsetmc-api
 License: MIT
 Keywords: tsetmc,stocks,tehran stock exchange
 Author: Mahdi Sadeghi
 Author-email: mahdi74sadeghi@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -87,7 +87,11 @@
 - [x] Migrate `group` component to use new tsetmc.
 - [ ] Support asyncio.
 
 ## Support and Donation
 
 If this repository helped you, please support it by giving a star (:star:).
 
+For contacting me about this project please use the following email:
+
+[mahdi74sadeghi+tsetmc_api@gmail.com](mailto:mahdi74sadeghi+tsetmc_api@gmail.com)
+
```

