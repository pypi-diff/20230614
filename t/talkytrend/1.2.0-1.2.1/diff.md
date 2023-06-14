# Comparing `tmp/talkytrend-1.2.0.tar.gz` & `tmp/talkytrend-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytrend-1.2.0.tar", max compression
+gzip compressed data, was "talkytrend-1.2.1.tar", max compression
```

## Comparing `talkytrend-1.2.0.tar` & `talkytrend-1.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-14 18:46:01.938655 talkytrend-1.2.0/LICENSE
--rw-r--r--   0        0        0     2058 2023-06-14 18:46:01.938655 talkytrend-1.2.0/README.md
--rw-r--r--   0        0        0     1720 2023-06-14 18:46:24.999084 talkytrend-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      101 2023-06-14 18:46:24.999084 talkytrend-1.2.0/talkytrend/__init__.py
--rw-r--r--   0        0        0      628 2023-06-14 18:46:01.938655 talkytrend-1.2.0/talkytrend/config.py
--rw-r--r--   0        0        0      843 2023-06-14 18:46:01.938655 talkytrend-1.2.0/talkytrend/default_settings.toml
--rw-r--r--   0        0        0     6222 2023-06-14 18:46:01.938655 talkytrend-1.2.0/talkytrend/main.py
--rw-r--r--   0        0        0     2955 1970-01-01 00:00:00.000000 talkytrend-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-14 19:23:58.809130 talkytrend-1.2.1/LICENSE
+-rw-r--r--   0        0        0     2058 2023-06-14 19:23:58.809130 talkytrend-1.2.1/README.md
+-rw-r--r--   0        0        0     1720 2023-06-14 19:24:17.305615 talkytrend-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-06-14 19:24:17.305615 talkytrend-1.2.1/talkytrend/__init__.py
+-rw-r--r--   0        0        0      628 2023-06-14 19:23:58.813130 talkytrend-1.2.1/talkytrend/config.py
+-rw-r--r--   0        0        0      842 2023-06-14 19:23:58.813130 talkytrend-1.2.1/talkytrend/default_settings.toml
+-rw-r--r--   0        0        0     6295 2023-06-14 19:23:58.813130 talkytrend-1.2.1/talkytrend/main.py
+-rw-r--r--   0        0        0     2955 1970-01-01 00:00:00.000000 talkytrend-1.2.1/PKG-INFO
```

### Comparing `talkytrend-1.2.0/LICENSE` & `talkytrend-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytrend-1.2.0/README.md` & `talkytrend-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `talkytrend-1.2.0/pyproject.toml` & `talkytrend-1.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talkytrend"
-version = "1.2.0"
+version = "1.2.1"
 description = "A python package to retrieve  economic data such as Trend for any financial symbol."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["finance", "crypto", "bot","trend","economic"]
 packages = [
     {include = "talkytrend"}
```

### Comparing `talkytrend-1.2.0/talkytrend/config.py` & `talkytrend-1.2.1/talkytrend/config.py`

 * *Files identical despite different names*

### Comparing `talkytrend-1.2.0/talkytrend/default_settings.toml` & `talkytrend-1.2.1/talkytrend/default_settings.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [default]
 talkytrend_enabled = true
 scanner_frequency = 7200
-enable_signals = false
+enable_signals = true
 assets = [
     { id ="EURUSD", exchange='FX_IDC',screener="forex", interval = "4h" },
     { id ="BTCUSD",exchange="BINANCE",screener="crypto", interval = "4h"},
     #use https://tvdb.brianthe.dev/ to get details
     # { id ="GOLD",exchange="TVC",screener="cfd", interval = "4h"},
     # { id ="USOIL",exchange="FX",screener="cfd", interval = "4h"},
     # { id ="ETHUSD",exchange="BINANCE",screener="crypto", interval = "4h"},
```

### Comparing `talkytrend-1.2.0/talkytrend/main.py` & `talkytrend-1.2.1/talkytrend/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 import asyncio
 import logging
 from datetime import date
 import aiohttp
 from prettytable import PrettyTable
 from tradingview_ta import TA_Handler
 from talkytrend import __version__
-from .config import settings
+from talkytrend.config import settings
 
 class TalkyTrend:
     def __init__(self):
         self.logger = logging.getLogger("TalkyTrend")
         self.enabled = settings.talkytrend_enabled
+        if not self.enabled:
+            return
         self.assets = settings.assets
         self.asset_signals = {}
         self.economic_calendar = settings.economic_calendar
         self.news_url = f"{settings.news_url}{settings.news_api_key}" if settings.news_api_key else None
         self.live_tv = settings.live_tv_url
 
     async def fetch_analysis(
@@ -127,30 +129,30 @@
             self.logger.error("news %s", error)
             return None
 
 
     async def scanner(self):
         while True:
             try:
-                key_events = await self.fetch_key_events()
-                if key_events is not None:
-                    self.logger.debug("Key event %s", key_events)
-                    yield key_events
-
-                key_news = await self.fetch_key_news()
-                if key_news is not None:
-                    self.logger.debug("Key news %s", key_news)
-                    yield key_news
-
-                signals = await self.check_signal()
-                if signals:
-                    for signal in signals:
-                        message = f"New signal for {signal['symbol']} ({signal['interval']}): {signal['signal']}"
-                        self.logger.debug("Signal message %s", message)
-                        yield message
+                if settings.enable_events:
+                    key_events = await self.fetch_key_events()
+                    if key_events is not None:
+                        self.logger.debug("Key event %s", key_events)
+                        yield key_events
+                if settings.enable_news:
+                    key_news = await self.fetch_key_news()
+                    if key_news is not None:
+                        self.logger.debug("Key news %s", key_news)
+                        yield key_news
+
+                if settings.enable_signals:
+                    signals = await self.check_signal()
+                    if signals is not None:
+                        self.logger.debug("Signals %s", signals)
+                        yield signals
 
             except Exception as error:
                 self.logger.error("scanner %s", error)
 
             await asyncio.sleep(settings.scanner_frequency)
```

### Comparing `talkytrend-1.2.0/PKG-INFO` & `talkytrend-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talkytrend
-Version: 1.2.0
+Version: 1.2.1
 Summary: A python package to retrieve  economic data such as Trend for any financial symbol.
 License: MIT
 Keywords: finance,crypto,bot,trend,economic
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

