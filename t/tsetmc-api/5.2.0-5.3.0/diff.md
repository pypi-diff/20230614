# Comparing `tmp/tsetmc_api-5.2.0.tar.gz` & `tmp/tsetmc_api-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsetmc_api-5.2.0.tar", max compression
+gzip compressed data, was "tsetmc_api-5.3.0.tar", max compression
```

## Comparing `tsetmc_api-5.2.0.tar` & `tsetmc_api-5.3.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1098 2023-06-14 19:52:29.642076 tsetmc_api-5.2.0/LICENSE.md
--rw-r--r--   0        0        0     2858 2023-06-14 19:52:29.642076 tsetmc_api-5.2.0/README.md
--rw-r--r--   0        0        0        0 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/__init__.py
--rw-r--r--   0        0        0       36 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/day_details/__init__.py
--rw-r--r--   0        0        0     9345 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/day_details/_core.py
--rw-r--r--   0        0        0     5926 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/day_details/day_details.py
--rw-r--r--   0        0        0      438 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/day_details/orderbook.py
--rw-r--r--   0        0        0      460 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/day_details/price.py
--rw-r--r--   0        0        0     1842 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/day_details/shareholder.py
--rw-r--r--   0        0        0      231 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/day_details/threshold.py
--rw-r--r--   0        0        0      215 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/day_details/trade.py
--rw-r--r--   0        0        0      368 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/day_details/traders_type.py
--rw-r--r--   0        0        0       36 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/group/__init__.py
--rw-r--r--   0        0        0      481 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/group/_core.py
--rw-r--r--   0        0        0      739 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/group/group.py
--rw-r--r--   0        0        0       36 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/market_map/__init__.py
--rw-r--r--   0        0        0     1373 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/market_map/_core.py
--rw-r--r--   0        0        0     1628 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/market_map/map.py
--rw-r--r--   0        0        0       31 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/market_watch/__init__.py
--rw-r--r--   0        0        0    17109 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/market_watch/_core.py
--rw-r--r--   0        0        0      224 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/market_watch/daily_history.py
--rw-r--r--   0        0        0      227 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/market_watch/orderbook.py
--rw-r--r--   0        0        0      514 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/market_watch/price.py
--rw-r--r--   0        0        0      321 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/market_watch/traders_type.py
--rw-r--r--   0        0        0     5043 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/market_watch/watch.py
--rw-r--r--   0        0        0       27 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/symbol/__init__.py
--rw-r--r--   0        0        0    12706 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/symbol/_core.py
--rw-r--r--   0        0        0      164 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/symbol/group.py
--rw-r--r--   0        0        0      366 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/symbol/identification.py
--rw-r--r--   0        0        0      219 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/symbol/notification.py
--rw-r--r--   0        0        0      247 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/symbol/orderbook.py
--rw-r--r--   0        0        0     1004 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/symbol/price.py
--rw-r--r--   0        0        0     1887 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/symbol/shareholder.py
--rw-r--r--   0        0        0      221 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/symbol/state_change.py
--rw-r--r--   0        0        0      240 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/symbol/supervisor_message.py
--rw-r--r--   0        0        0     9693 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/symbol/symbol.py
--rw-r--r--   0        0        0      453 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/symbol/traders_type.py
--rw-r--r--   0        0        0      933 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/utils.py
--rw-r--r--   0        0        0       18 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/lib/tsetmc_api/version.py
--rw-r--r--   0        0        0      745 2023-06-14 19:52:29.682076 tsetmc_api-5.2.0/pyproject.toml
--rw-r--r--   0        0        0     3816 1970-01-01 00:00:00.000000 tsetmc_api-5.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-06-14 21:21:52.254227 tsetmc_api-5.3.0/LICENSE.md
+-rw-r--r--   0        0        0     3526 2023-06-14 21:21:52.254227 tsetmc_api-5.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/__init__.py
+-rw-r--r--   0        0        0       36 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/day_details/__init__.py
+-rw-r--r--   0        0        0     9346 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/day_details/_core.py
+-rw-r--r--   0        0        0     7910 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/day_details/day_details.py
+-rw-r--r--   0        0        0      438 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/day_details/orderbook.py
+-rw-r--r--   0        0        0      460 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/day_details/price.py
+-rw-r--r--   0        0        0     2473 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/day_details/shareholder.py
+-rw-r--r--   0        0        0      231 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/day_details/threshold.py
+-rw-r--r--   0        0        0      215 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/day_details/trade.py
+-rw-r--r--   0        0        0      368 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/day_details/traders_type.py
+-rw-r--r--   0        0        0       36 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/group/__init__.py
+-rw-r--r--   0        0        0      481 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/group/_core.py
+-rw-r--r--   0        0        0     1001 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/group/group.py
+-rw-r--r--   0        0        0       36 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/market_map/__init__.py
+-rw-r--r--   0        0        0     1373 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/market_map/_core.py
+-rw-r--r--   0        0        0     2103 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/market_map/map.py
+-rw-r--r--   0        0        0       31 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/market_watch/__init__.py
+-rw-r--r--   0        0        0    17110 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/market_watch/_core.py
+-rw-r--r--   0        0        0      224 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/market_watch/daily_history.py
+-rw-r--r--   0        0        0      227 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/market_watch/orderbook.py
+-rw-r--r--   0        0        0      514 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/market_watch/price.py
+-rw-r--r--   0        0        0      321 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/market_watch/traders_type.py
+-rw-r--r--   0        0        0     6442 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/market_watch/watch.py
+-rw-r--r--   0        0        0       27 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/symbol/__init__.py
+-rw-r--r--   0        0        0    12723 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/symbol/_core.py
+-rw-r--r--   0        0        0      164 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/symbol/group.py
+-rw-r--r--   0        0        0      366 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/symbol/identification.py
+-rw-r--r--   0        0        0      219 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/symbol/notification.py
+-rw-r--r--   0        0        0      247 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/symbol/orderbook.py
+-rw-r--r--   0        0        0     1004 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/symbol/price.py
+-rw-r--r--   0        0        0     2465 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/symbol/shareholder.py
+-rw-r--r--   0        0        0      221 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/symbol/state_change.py
+-rw-r--r--   0        0        0      240 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/symbol/supervisor_message.py
+-rw-r--r--   0        0        0    12214 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/symbol/symbol.py
+-rw-r--r--   0        0        0      453 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/symbol/traders_type.py
+-rw-r--r--   0        0        0     1231 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/utils.py
+-rw-r--r--   0        0        0       18 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/lib/tsetmc_api/version.py
+-rw-r--r--   0        0        0      745 2023-06-14 21:21:52.298231 tsetmc_api-5.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4484 1970-01-01 00:00:00.000000 tsetmc_api-5.3.0/PKG-INFO
```

### Comparing `tsetmc_api-5.2.0/LICENSE.md` & `tsetmc_api-5.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tsetmc_api-5.2.0/README.md` & `tsetmc_api-5.3.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 
 `pip install tsetmc-api`
 
 ## Examples
 
 You can find examples of using each component in `examples` directory.
 
-| Component    | Example File                                                |
-|--------------|-------------------------------------------------------------|
-| Symbol       | [symbol_example.py](examples/symbol_example.py)             |
-| Market Watch | [market_watch_example.py](examples/market_watch_example.py) |
-| Day Details  | [day_details_example.py](examples/day_details_example.py)   |
-| Market Map   | [market_map_example.py](examples/market_map_example.py)     |
-| Group        | [group_example.py](examples/group_example.py)               |
+| Component    | Example File                                                                                                 |
+|--------------|--------------------------------------------------------------------------------------------------------------|
+| Symbol       | [symbol_example.py](https://github.com/mahs4d/tsetmc-api/blob/master/examples/symbol_example.py)             |
+| Market Watch | [market_watch_example.py](https://github.com/mahs4d/tsetmc-api/blob/master/examples/market_watch_example.py) |
+| Day Details  | [day_details_example.py](https://github.com/mahs4d/tsetmc-api/blob/master/examples/day_details_example.py)   |
+| Market Map   | [market_map_example.py](https://github.com/mahs4d/tsetmc-api/blob/master/examples/market_map_example.py)     |
+| Group        | [group_example.py](https://github.com/mahs4d/tsetmc-api/blob/master/examples/group_example.py)               |
+| Async        | [async_example.py](https://github.com/mahs4d/tsetmc-api/blob/master/examples/async_example.py)               |
 
 ## Usage
 
 - **symbol:** working with main symbol page and live data (
   e.g. [this page](http://www.tsetmc.com/loader.aspx?ParTree=151311&i=43362635835198978))
 - **market_watch:** getting data visible from [market watch page](http://www.tsetmc.com/Loader.aspx?ParTree=15131F)
 - **day_details:** working with details of a symbol in a single day of history (
@@ -50,22 +51,27 @@
 
 Group component currently only has one function (`get_all_groups`) which returns all the symbol groups.
 
 ### Errors
 
 Tsetmc sometimes returns 403 and you should retry.
 
+### Async Support
+
+Each method in the library has an async counterpart with the same name and a `_async` suffix.
+These methods use the sync functions behind the scene in an asyncio pool executor.
+
 ### TODO
 
 - [ ] Migrate `symbol` component to use new tsetmc.
 - [ ] Migrate `market_watch` component to use new tsetmc.
 - [x] Migrate `day_details` component to use new tsetmc.
 - [x] Migrate `market_map` component to use new tsetmc.
 - [x] Migrate `group` component to use new tsetmc.
-- [ ] Support asyncio.
+- [x] Support asyncio.
 
 ## Support and Donation
 
 If this repository helped you, please support it by giving a star (:star:).
 
 For contacting me about this project please use the following email:
```

### Comparing `tsetmc_api-5.2.0/lib/tsetmc_api/day_details/_core.py` & `tsetmc_api-5.3.0/lib/tsetmc_api/day_details/_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -223,15 +223,15 @@
         sh_data = {
             'id': str(row['shareHolderID']),
             'name': row['shareHolderName'],
             'shares_count': row['numberOfShares'],
             'shares_percentage': row['perOfShares'],
         }
 
-        if row['dEven'] < it:
+        if row['dEven'] <= it:
             old_shareholders.append(sh_data)
         else:
             new_shareholders.append(sh_data)
 
     return old_shareholders, new_shareholders
```

### Comparing `tsetmc_api-5.2.0/lib/tsetmc_api/day_details/day_details.py` & `tsetmc_api-5.3.0/lib/tsetmc_api/day_details/day_details.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from . import _core
 from .orderbook import DayDetailsOrderBookDataRow, DayDetailsOrderBookRow
 from .price import DayDetailsPriceDataRow, DayDetailsPriceOverview
 from .shareholder import DayDetailsShareHolderDataRow, DayDetailsShareHolder
 from .threshold import DayDetailsThresholdsData
 from .trade import DayDetailsTradeDataRow
 from .traders_type import DayDetailsTradersTypeData, DayDetailsTradersTypeInfo, DayDetailsTradersTypeSubInfo
+from ..utils import run_sync_function
 
 
 class DayDetails:
     def __init__(self, symbol_id: str, date: jdate):
         self.symbol_id = symbol_id
         self.date = date
 
@@ -30,14 +31,23 @@
             close=raw_data['close'],
             last=raw_data['last'],
             count=raw_data['count'],
             volume=raw_data['volume'],
             value=raw_data['value'],
         )
 
+    async def get_price_overview_async(self) -> DayDetailsPriceOverview:
+        """
+        returns an overview of price information for that day
+        """
+
+        return await run_sync_function(
+            func=self.get_price_overview,
+        )
+
     def get_price_data(self) -> list[DayDetailsPriceDataRow]:
         """
         returns instant prices (for each time in that date)
         """
 
         raw_data = _core.get_day_details_price_data(symbol_id=self.symbol_id, date=self.date)
 
@@ -46,14 +56,23 @@
             close=row['close'],
             last=row['last'],
             value=row['value'],
             volume=row['volume'],
             count=row['count'],
         ) for row in raw_data]
 
+    async def get_price_data_async(self) -> list[DayDetailsPriceDataRow]:
+        """
+        returns instant prices (for each time in that date)
+        """
+
+        return await run_sync_function(
+            func=self.get_price_data,
+        )
+
     def get_orderbook_data(self) -> list[DayDetailsOrderBookDataRow]:
         """
         returns instant orderbooks (for each time in that date)
         """
 
         raw_data = _core.get_day_details_orderbook_data(symbol_id=self.symbol_id, date=self.date)
 
@@ -69,14 +88,23 @@
                 time=row['time'],
                 count=row['count'],
                 price=row['price'],
                 volume=row['volume'],
             ) for row in data['sell_rows']],
         ) for data in raw_data]
 
+    async def get_orderbook_data_async(self) -> list[DayDetailsOrderBookDataRow]:
+        """
+        returns instant orderbooks (for each time in that date)
+        """
+
+        return await run_sync_function(
+            func=self.get_orderbook_data,
+        )
+
     def get_traders_type_data(self) -> DayDetailsTradersTypeData:
         """
         returns traders type information for that day
         """
 
         raw_data = _core.get_day_details_traders_type_data(symbol_id=self.symbol_id, date=self.date)
 
@@ -103,56 +131,100 @@
                     count=raw_data['real']['sell']['count'],
                     volume=raw_data['real']['sell']['volume'],
                     value=raw_data['real']['sell']['value'],
                 ),
             ),
         )
 
+    async def get_traders_type_data_async(self) -> DayDetailsTradersTypeData:
+        """
+        returns traders type information for that day
+        """
+
+        return await run_sync_function(
+            func=self.get_traders_type_data,
+        )
+
     def get_trades_data(self, summarize: bool = False) -> list[DayDetailsTradeDataRow]:
         """
         gets all trade data
         """
 
         raw_data = _core.get_day_details_trade_data(symbol_id=self.symbol_id, date=self.date, summarize=summarize)
 
         return [DayDetailsTradeDataRow(
             time=row['time'],
             price=row['price'],
             volume=row['volume'],
         ) for row in raw_data]
 
+    async def get_trades_data_async(self, summarize: bool = False) -> list[DayDetailsTradeDataRow]:
+        """
+        gets all trade data
+        """
+
+        return await run_sync_function(
+            func=self.get_trades_data,
+            summarize=summarize,
+        )
+
     def get_thresholds_data(self) -> list[DayDetailsThresholdsData]:
+        """
+        Get allowed price window
+        """
+
         raw_data = _core.get_day_details_thresholds_data(symbol_id=self.symbol_id, date=self.date)
 
         return [DayDetailsThresholdsData(
             time=row['time'],
             range_max=row['max'],
             range_min=row['min'],
         ) for row in raw_data]
 
+    async def get_thresholds_data_async(self) -> list[DayDetailsThresholdsData]:
+        """
+        Get allowed price window
+        """
+
+        return await run_sync_function(
+            func=self.get_thresholds_data,
+        )
+
     def get_shareholders_data(self) -> tuple[list[DayDetailsShareHolderDataRow], list[DayDetailsShareHolderDataRow]]:
         """
         gets list of shareholders before and after the day
         """
 
         raw_old_shareholders, raw_new_shareholders = _core.get_day_details_shareholders_data(
             symbol_id=self.symbol_id,
             date=self.date,
         )
 
         old_shareholders = [DayDetailsShareHolderDataRow(
             symbol_id=self.symbol_id,
             date=self.date,
             shareholder=DayDetailsShareHolder(id=row['id'], name=row['name']),
-            count=row['count'],
-            percentage=row['percentage'],
+            shares_count=row['shares_count'],
+            shares_percentage=row['shares_percentage'],
         ) for row in raw_old_shareholders]
 
         new_shareholders = [DayDetailsShareHolderDataRow(
             symbol_id=self.symbol_id,
             date=self.date,
             shareholder=DayDetailsShareHolder(id=row['id'], name=row['name']),
             shares_count=row['shares_count'],
             shares_percentage=row['shares_percentage'],
         ) for row in raw_new_shareholders]
 
         return old_shareholders, new_shareholders
+
+    async def get_shareholders_data_async(self) -> tuple[
+        list[DayDetailsShareHolderDataRow],
+        list[DayDetailsShareHolderDataRow],
+    ]:
+        """
+        gets list of shareholders before and after the day
+        """
+
+        return await run_sync_function(
+            func=self.get_shareholders_data,
+        )
```

### Comparing `tsetmc_api-5.2.0/lib/tsetmc_api/day_details/shareholder.py` & `tsetmc_api-5.3.0/lib/tsetmc_api/day_details/shareholder.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from jdatetime import date as jdate
 from pydantic import BaseModel
 
 from . import _core
+from ..utils import run_sync_function
 
 
 class DayDetailsShareHolderPortfolioRow(BaseModel):
     symbol_id: str
     short_name: str
     long_name: str
     shares_count: int
@@ -27,14 +28,23 @@
             symbol_id=row['symbol_id'],
             short_name=row['short_name'],
             long_name=row['long_name'],
             shares_count=row['shares_count'],
             shares_percent=row['shares_percent'],
         ) for row in raw_data]
 
+    async def get_portfolio_data_async(self) -> list[DayDetailsShareHolderPortfolioRow]:
+        """
+        returns list of companies owned by this shareholder
+        """
+
+        return await run_sync_function(
+            func=self.get_portfolio_data,
+        )
+
 
 class DayDetailsShareHolderChartRow(BaseModel):
     date: jdate
     shares_count: int
     shares_percentage: float
 
     class Config:
@@ -61,9 +71,19 @@
 
         return [DayDetailsShareHolderChartRow(
             date=row['date'],
             shares_count=row['shares_count'],
             shares_percentage=row['shares_percentage'],
         ) for row in raw_data]
 
+    async def get_chart_data_async(self, days: int = 90) -> list[DayDetailsShareHolderChartRow]:
+        """
+        returns list of changes to shareholders share count in history of this symbol
+        """
+
+        return await run_sync_function(
+            func=self.get_chart_data_async,
+            days=days,
+        )
+
     class Config:
         arbitrary_types_allowed = True
```

### Comparing `tsetmc_api-5.2.0/lib/tsetmc_api/group/group.py` & `tsetmc_api-5.3.0/lib/tsetmc_api/group/group.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from enum import Enum
 
 from pydantic import BaseModel
 
 from . import _core
+from ..utils import run_sync_function
 
 
 class GroupType(Enum):
     PAPER = 'PAPER'
     INDUSTRIAL = 'INDUSTRIAL'
 
 
@@ -29,7 +30,17 @@
         return [Group(
             id=row['id'],
             code=row['code'],
             name=row['name'],
             description=row['description'],
             type=GroupType.PAPER if row['type'] == 'PaperType' else GroupType.INDUSTRIAL,
         ) for row in raw_data]
+
+    @staticmethod
+    async def get_all_groups_async() -> list[Group]:
+        """
+        returns list of symbol groups
+        """
+
+        return await run_sync_function(
+            func=Group.get_all_groups,
+        )
```

### Comparing `tsetmc_api-5.2.0/lib/tsetmc_api/market_map/_core.py` & `tsetmc_api-5.3.0/lib/tsetmc_api/market_map/_core.py`

 * *Files identical despite different names*

### Comparing `tsetmc_api-5.2.0/lib/tsetmc_api/market_map/map.py` & `tsetmc_api-5.3.0/lib/tsetmc_api/market_map/map.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from enum import Enum
 
 from pydantic import BaseModel
 from pydantic.utils import deep_update
 
 from . import _core
+from ..utils import run_sync_function
 
 
 class MapDataRow(BaseModel):
     symbol_id: str
     symbol_short_name: str
     symbol_long_name: str
 
@@ -60,7 +61,18 @@
 
             color=data['color'],
             price_change_percent=data['price_change_percent'],
             percent=data['percent'],
         ) for key, data in raw_data.items()}
 
         return map_data
+
+    async def get_market_map_data_async(self, map_type: MapType = MapType.MARKET_VALUE) -> dict[str, MapDataRow]:
+        """
+        returns symbol data in market map (in "naghshe bazar" page)
+        !!! webserver occasionally throws 403 error, you should retry in a few seconds when this happens
+        """
+
+        return await run_sync_function(
+            func=self.get_market_map_data,
+            map_type=map_type,
+        )
```

### Comparing `tsetmc_api-5.2.0/lib/tsetmc_api/market_watch/_core.py` & `tsetmc_api-5.3.0/lib/tsetmc_api/market_watch/_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,15 +263,15 @@
         }
 
     return watch_data
 
 
 def get_watch_daily_history_data() -> dict:
     response = requests.get(
-        url='http://members.tsetmc.com/tsev2/data/ClosingPriceAll.aspx',
+        url='https://members.tsetmc.com/tsev2/data/ClosingPriceAll.aspx',
         params={},
         verify=False,
         timeout=20,
     )
     response.raise_for_status()
     response = response.text
```

### Comparing `tsetmc_api-5.2.0/lib/tsetmc_api/market_watch/price.py` & `tsetmc_api-5.3.0/lib/tsetmc_api/market_watch/price.py`

 * *Files identical despite different names*

### Comparing `tsetmc_api-5.2.0/lib/tsetmc_api/market_watch/watch.py` & `tsetmc_api-5.3.0/lib/tsetmc_api/market_watch/watch.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from . import _core
 from .daily_history import WatchDailyHistoryDataRow
 from .orderbook import WatchOrderBook, WatchOrderBookRow
 from .price import WatchPriceDataRow
 from .traders_type import WatchTradersTypeDataRow, WatchTradersTypeInfo, WatchTradersTypeSubInfo
-from ..utils import deep_update
+from ..utils import deep_update, run_sync_function
 
 
 class MarketWatch:
     def __init__(self):
         self._heven = 0
         self._refid = 0
         self._last_price_data = {}
@@ -67,14 +67,23 @@
             )
 
         self._heven = new_heven
         self._refid = new_refid
 
         return watch_data
 
+    async def get_price_data_async(self) -> dict[str, WatchPriceDataRow]:
+        """
+        gets basic price information (in "didbane bazar" page)
+        """
+
+        return await run_sync_function(
+            func=self.get_price_data,
+        )
+
     def get_traders_type_data(self) -> dict[str, WatchTradersTypeDataRow]:
         """
         gets traders type data (in "didebane bazar" page)
         """
 
         raw_data = _core.get_watch_traders_type_data()
 
@@ -101,14 +110,23 @@
                         volume=data['real']['sell']['volume'],
                     ),
                 ),
             )
 
         return watch_data
 
+    async def get_traders_type_data_async(self) -> dict[str, WatchTradersTypeDataRow]:
+        """
+        gets traders type data (in "didebane bazar" page)
+        """
+
+        return await run_sync_function(
+            func=self.get_traders_type_data,
+        )
+
     def get_daily_history_data(self) -> dict[str, list[WatchDailyHistoryDataRow]]:
         """
         gets 30 day history of symbols (in "didbane bazar" page)
         """
 
         raw_data = _core.get_watch_daily_history_data()
 
@@ -125,18 +143,47 @@
                 low=row['low'],
                 high=row['high'],
                 yesterday=row['yesterday'],
             ) for row in raw_data[symbol_id]]
 
         return watch_data
 
+    async def get_daily_history_data_async(self) -> dict[str, list[WatchDailyHistoryDataRow]]:
+        """
+        gets 30 day history of symbols (in "didbane bazar" page)
+        """
+
+        return await run_sync_function(
+            func=self.get_daily_history_data,
+        )
+
     def get_raw_stats_data(self) -> dict[list]:
         """
         returns a list of stats for each symbol. refer to tsetmc.com for information of what each item in the list is
         """
 
+        return _core.get_watch_raw_stats_data()
+
+    async def get_raw_stats_data_async(self) -> dict[list]:
+        """
+        returns a list of stats for each symbol. refer to tsetmc.com for information of what each item in the list is
+        """
+
+        return await run_sync_function(
+            func=self.get_raw_stats_data,
+        )
+
     def get_stats_data(self) -> dict[dict]:
         """
         !!! EXPERIMENTAL: returns stats in dict, may be wrong !!!
         """
 
         return _core.get_watch_stats_data()
+
+    async def get_stats_data_async(self) -> dict[dict]:
+        """
+        !!! EXPERIMENTAL: returns stats in dict, may be wrong !!!
+        """
+
+        return await run_sync_function(
+            func=self.get_stats_data,
+        )
```

### Comparing `tsetmc_api-5.2.0/lib/tsetmc_api/symbol/_core.py` & `tsetmc_api-5.3.0/lib/tsetmc_api/symbol/_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -389,15 +389,15 @@
         tds = tr.find_all('td')
 
         shareholder_id = tr['onclick']
         shareholder_id = shareholder_id[shareholder_id.index("'") + 1: shareholder_id.index(",")]
         name = tds[0].text.strip()
         count = int(tds[1].div['title'].replace(',', ''))
         percentage = float(tds[2].text)
-        change = locale.atoi(tds[3].text.strip())
+        change = locale.atoi(tds[3].text.replace(',', '').strip())
 
         shareholders.append({
             'id': shareholder_id,
             'name': name,
             'shares_count': count,
             'shares_percentage': percentage,
             'shares_change': change,
```

### Comparing `tsetmc_api-5.2.0/lib/tsetmc_api/symbol/price.py` & `tsetmc_api-5.3.0/lib/tsetmc_api/symbol/price.py`

 * *Files identical despite different names*

### Comparing `tsetmc_api-5.2.0/lib/tsetmc_api/symbol/shareholder.py` & `tsetmc_api-5.3.0/lib/tsetmc_api/symbol/shareholder.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Any
 
 from jdatetime import date as jdate
 from pydantic import BaseModel, PrivateAttr
 
 from . import _core
+from ..utils import run_sync_function
 
 
 class SymbolShareHolderPortfolioRow(BaseModel):
     symbol_id: str
     long_name: str
     shares_count: int
     shares_percentage: float
@@ -35,14 +36,23 @@
         return [SymbolShareHolderPortfolioRow(
             symbol_id=row['symbol_id'],
             long_name=row['long_name'],
             shares_count=row['shares_count'],
             shares_percentage=row['shares_percentage'],
         ) for row in raw_data]
 
+    async def get_portfolio_data_async(self) -> list[SymbolShareHolderPortfolioRow]:
+        """
+        returns list of companies owned by this shareholder
+        """
+
+        return await run_sync_function(
+            func=self.get_portfolio_data,
+        )
+
 
 class SymbolShareHolderChartRow(BaseModel):
     date: jdate
     shares_count: int
 
     class Config:
         arbitrary_types_allowed = True
@@ -64,7 +74,16 @@
             company_isin=self.shareholder._company_isin,
         )['chart']
 
         return [SymbolShareHolderChartRow(
             date=row['date'],
             shares_count=row['shares_count'],
         ) for row in raw_data]
+
+    async def get_chart_data_async(self) -> list[SymbolShareHolderChartRow]:
+        """
+        returns list of changes to shareholders share count in history of this symbol
+        """
+
+        return await run_sync_function(
+            func=self.get_chart_data,
+        )
```

### Comparing `tsetmc_api-5.2.0/lib/tsetmc_api/symbol/symbol.py` & `tsetmc_api-5.3.0/lib/tsetmc_api/symbol/symbol.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from .notification import SymbolNotificationsDataRow
 from .orderbook import SymbolOrderBookData, SymbolOrderBookDataRow
 from .price import SymbolPriceOverview, SymbolIntraDayPriceChartDataRow, SymbolPriceData, SymbolDailyPriceDataRow
 from .shareholder import SymbolShareHolderDataRow, SymbolShareHolder
 from .state_change import SymbolStateChangeDataRow
 from .supervisor_message import SymbolSupervisorMessageDataRow
 from .traders_type import SymbolTradersTypeDataRow, SymbolTradersTypeInfo, SymbolTradersTypeSubInfo
+from ..utils import run_sync_function
 
 
 class Symbol:
     def __init__(self, symbol_id: str):
         self.symbol_id = symbol_id
 
     def get_price_overview(self) -> SymbolPriceOverview:
@@ -89,14 +90,23 @@
             datetime=raw_data['datetime'],
             price_data=tick,
             orderbook=orderbook,
             traders_type=traders_type,
             group_data=group_data,
         )
 
+    async def get_price_overview_async(self) -> SymbolPriceOverview:
+        """
+        gets the last price overview of the symbol and returns most of the information (in "dar yek negah" tab)
+        """
+
+        return await run_sync_function(
+            func=self.get_price_overview,
+        )
+
     def get_intraday_price_chart_data(self) -> list[SymbolIntraDayPriceChartDataRow]:
         """
         gets last days intraday price chart (in "dar yek negah" tab)
         """
 
         raw_data = _core.get_symbol_intraday_price_chart(symbol_id=self.symbol_id)
 
@@ -107,14 +117,23 @@
             open=row['open'],
             close=row['close'],
             volume=row['volume'],
         ) for row in raw_data]
 
         return ticks
 
+    async def get_intraday_price_chart_data_async(self) -> list[SymbolIntraDayPriceChartDataRow]:
+        """
+        gets last days intraday price chart (in "dar yek negah" tab)
+        """
+
+        return await run_sync_function(
+            func=self.get_intraday_price_chart_data,
+        )
+
     def get_supervisor_messages_data(self) -> list[SymbolSupervisorMessageDataRow]:
         """
         get list of supervisor messages (in "payame nazer" tab)
         """
 
         raw_data = _core.get_symbol_supervisor_messages(symbol_id=self.symbol_id)
 
@@ -122,42 +141,69 @@
             datetime=row['datetime'],
             title=row['title'],
             content=row['content'],
         ) for row in raw_data]
 
         return messages
 
+    async def get_supervisor_messages_data_async(self) -> list[SymbolSupervisorMessageDataRow]:
+        """
+        get list of supervisor messages (in "payame nazer" tab)
+        """
+
+        return await run_sync_function(
+            func=self.get_supervisor_messages_data,
+        )
+
     def get_notifications_data(self) -> list[SymbolNotificationsDataRow]:
         """
         get list of notifications (in "etelaiye ha" tab)
         """
 
         raw_data = _core.get_symbol_notifications(symbol_id=self.symbol_id)
 
         notifications = [SymbolNotificationsDataRow(
             datetime=row['datetime'],
             title=row['title'],
         ) for row in raw_data]
 
         return notifications
 
+    async def get_notifications_data_async(self) -> list[SymbolNotificationsDataRow]:
+        """
+        get list of notifications (in "etelaiye ha" tab)
+        """
+
+        return await run_sync_function(
+            func=self.get_notifications_data,
+        )
+
     def get_state_changes_data(self) -> list[SymbolStateChangeDataRow]:
         """
         get list of state changes (in "taghire vaziat" tab)
         """
 
         raw_data = _core.get_symbol_state_changes(symbol_id=self.symbol_id)
 
         state_changes = [SymbolStateChangeDataRow(
             datetime=row['datetime'],
             new_state=row['new_state'],
         ) for row in raw_data]
 
         return state_changes
 
+    async def get_state_changes_data_async(self) -> list[SymbolStateChangeDataRow]:
+        """
+        get list of state changes (in "taghire vaziat" tab)
+        """
+
+        return await run_sync_function(
+            func=self.get_state_changes_data,
+        )
+
     def get_daily_history(self) -> list[SymbolDailyPriceDataRow]:
         """
         get list of daily ticks history (in "sabeghe" tab)
         """
 
         raw_data = _core.get_symbol_daily_ticks_history(symbol_id=self.symbol_id)
 
@@ -172,14 +218,23 @@
             count=row['count'],
             volume=row['volume'],
             value=row['value'],
         ) for row in raw_data]
 
         return ticks
 
+    async def get_daily_history_async(self) -> list[SymbolDailyPriceDataRow]:
+        """
+        get list of daily ticks history (in "sabeghe" tab)
+        """
+
+        return await run_sync_function(
+            func=self.get_daily_history,
+        )
+
     def get_id_details(self) -> SymbolIdDetails:
         """
         gets symbol identity details and returns all the information (in "shenase" tab)
         """
 
         raw_data = _core.get_symbol_id_details(symbol_id=self.symbol_id)
 
@@ -202,14 +257,23 @@
 
             subgroup_code=raw_data['subgroup_code'],
             subgroup_name=raw_data['subgroup_name'],
         )
 
         return details
 
+    async def get_id_details_async(self) -> SymbolIdDetails:
+        """
+        gets symbol identity details and returns all the information (in "shenase" tab)
+        """
+
+        return await run_sync_function(
+            func=self.get_id_details,
+        )
+
     def get_traders_type_history(self) -> list[SymbolTradersTypeDataRow]:
         """
         returns daily traders type history (in "haghihi-hoghooghi" tab)
         """
 
         raw_data = _core.get_symbol_traders_type_history(symbol_id=self.symbol_id)
 
@@ -239,14 +303,23 @@
                     value=row['real']['sell']['value'],
                 ),
             ),
         ) for row in raw_data]
 
         return traders_type_history
 
+    async def get_traders_type_history_async(self) -> list[SymbolTradersTypeDataRow]:
+        """
+        returns daily traders type history (in "haghihi-hoghooghi" tab)
+        """
+
+        return await run_sync_function(
+            func=self.get_traders_type_history,
+        )
+
     def get_shareholders_data(self) -> list[SymbolShareHolderDataRow]:
         """
         returns list of major shareholders (in "saham daran" tab)
         """
 
         company_isin = self.get_id_details().company_isin
         raw_data = _core.get_symbol_shareholders(company_isin=company_isin)
@@ -259,7 +332,16 @@
             ),
             shares_count=row['shares_count'],
             shares_percentage=row['shares_percentage'],
             shares_change=row['shares_change'],
         ) for row in raw_data]
 
         return shareholders
+
+    async def get_shareholders_data_async(self) -> list[SymbolShareHolderDataRow]:
+        """
+        returns list of major shareholders (in "saham daran" tab)
+        """
+
+        return await run_sync_function(
+            func=self.get_shareholders_data,
+        )
```

### Comparing `tsetmc_api-5.2.0/lib/tsetmc_api/utils.py` & `tsetmc_api-5.3.0/lib/tsetmc_api/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+import asyncio
 from copy import deepcopy
+from functools import partial
+from typing import Callable, Any
 
 from jdatetime import date as jdate, time as jtime
 
 
 def deep_update(d1: dict, d2: dict) -> dict:
     ret = deepcopy(d1)
 
@@ -30,7 +33,15 @@
 def convert_deven_to_jdate(deven: int) -> jdate:
     deven = str(deven)
     return jdate.fromgregorian(
         year=int(deven[:4]),
         month=int(deven[4:6]),
         day=int(deven[6:]),
     )
+
+
+async def run_sync_function(func: Callable, *args, **kwargs) -> Any:
+    loop = asyncio.get_event_loop()
+    return await loop.run_in_executor(
+        executor=None,
+        func=partial(func, *args, **kwargs),
+    )
```

### Comparing `tsetmc_api-5.2.0/pyproject.toml` & `tsetmc_api-5.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tsetmc-api"
-version = "5.2.0"
+version = "5.3.0"
 description = "simple package to communicate and crawl data from tsetmc.com (Tehran Stock Exchange Website)"
 license = "MIT"
 repository = "https://github.com/mahs4d/tsetmc-api"
 authors = ["Mahdi Sadeghi <mahdi74sadeghi@gmail.com>"]
 packages = [
     { include = "tsetmc_api", from = "lib" },
 ]
```

### Comparing `tsetmc_api-5.2.0/PKG-INFO` & `tsetmc_api-5.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsetmc-api
-Version: 5.2.0
+Version: 5.3.0
 Summary: simple package to communicate and crawl data from tsetmc.com (Tehran Stock Exchange Website)
 Home-page: https://github.com/mahs4d/tsetmc-api
 License: MIT
 Keywords: tsetmc,stocks,tehran stock exchange
 Author: Mahdi Sadeghi
 Author-email: mahdi74sadeghi@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -32,21 +32,22 @@
 
 `pip install tsetmc-api`
 
 ## Examples
 
 You can find examples of using each component in `examples` directory.
 
-| Component    | Example File                                                |
-|--------------|-------------------------------------------------------------|
-| Symbol       | [symbol_example.py](examples/symbol_example.py)             |
-| Market Watch | [market_watch_example.py](examples/market_watch_example.py) |
-| Day Details  | [day_details_example.py](examples/day_details_example.py)   |
-| Market Map   | [market_map_example.py](examples/market_map_example.py)     |
-| Group        | [group_example.py](examples/group_example.py)               |
+| Component    | Example File                                                                                                 |
+|--------------|--------------------------------------------------------------------------------------------------------------|
+| Symbol       | [symbol_example.py](https://github.com/mahs4d/tsetmc-api/blob/master/examples/symbol_example.py)             |
+| Market Watch | [market_watch_example.py](https://github.com/mahs4d/tsetmc-api/blob/master/examples/market_watch_example.py) |
+| Day Details  | [day_details_example.py](https://github.com/mahs4d/tsetmc-api/blob/master/examples/day_details_example.py)   |
+| Market Map   | [market_map_example.py](https://github.com/mahs4d/tsetmc-api/blob/master/examples/market_map_example.py)     |
+| Group        | [group_example.py](https://github.com/mahs4d/tsetmc-api/blob/master/examples/group_example.py)               |
+| Async        | [async_example.py](https://github.com/mahs4d/tsetmc-api/blob/master/examples/async_example.py)               |
 
 ## Usage
 
 - **symbol:** working with main symbol page and live data (
   e.g. [this page](http://www.tsetmc.com/loader.aspx?ParTree=151311&i=43362635835198978))
 - **market_watch:** getting data visible from [market watch page](http://www.tsetmc.com/Loader.aspx?ParTree=15131F)
 - **day_details:** working with details of a symbol in a single day of history (
@@ -74,22 +75,27 @@
 
 Group component currently only has one function (`get_all_groups`) which returns all the symbol groups.
 
 ### Errors
 
 Tsetmc sometimes returns 403 and you should retry.
 
+### Async Support
+
+Each method in the library has an async counterpart with the same name and a `_async` suffix.
+These methods use the sync functions behind the scene in an asyncio pool executor.
+
 ### TODO
 
 - [ ] Migrate `symbol` component to use new tsetmc.
 - [ ] Migrate `market_watch` component to use new tsetmc.
 - [x] Migrate `day_details` component to use new tsetmc.
 - [x] Migrate `market_map` component to use new tsetmc.
 - [x] Migrate `group` component to use new tsetmc.
-- [ ] Support asyncio.
+- [x] Support asyncio.
 
 ## Support and Donation
 
 If this repository helped you, please support it by giving a star (:star:).
 
 For contacting me about this project please use the following email:
```

