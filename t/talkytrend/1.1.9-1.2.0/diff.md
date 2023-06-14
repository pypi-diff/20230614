# Comparing `tmp/talkytrend-1.1.9.tar.gz` & `tmp/talkytrend-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytrend-1.1.9.tar", max compression
+gzip compressed data, was "talkytrend-1.2.0.tar", max compression
```

## Comparing `talkytrend-1.1.9.tar` & `talkytrend-1.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-14 13:44:44.007210 talkytrend-1.1.9/LICENSE
--rw-r--r--   0        0        0     2058 2023-06-14 13:44:44.007210 talkytrend-1.1.9/README.md
--rw-r--r--   0        0        0     1702 2023-06-14 13:45:03.127537 talkytrend-1.1.9/pyproject.toml
--rw-r--r--   0        0        0      101 2023-06-14 13:45:03.127537 talkytrend-1.1.9/talkytrend/__init__.py
--rw-r--r--   0        0        0      628 2023-06-14 13:44:44.007210 talkytrend-1.1.9/talkytrend/config.py
--rw-r--r--   0        0        0      779 2023-06-14 13:44:44.007210 talkytrend-1.1.9/talkytrend/default_settings.toml
--rw-r--r--   0        0        0     6140 2023-06-14 13:44:44.007210 talkytrend-1.1.9/talkytrend/main.py
--rw-r--r--   0        0        0     2928 1970-01-01 00:00:00.000000 talkytrend-1.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-14 18:46:01.938655 talkytrend-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2058 2023-06-14 18:46:01.938655 talkytrend-1.2.0/README.md
+-rw-r--r--   0        0        0     1720 2023-06-14 18:46:24.999084 talkytrend-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-06-14 18:46:24.999084 talkytrend-1.2.0/talkytrend/__init__.py
+-rw-r--r--   0        0        0      628 2023-06-14 18:46:01.938655 talkytrend-1.2.0/talkytrend/config.py
+-rw-r--r--   0        0        0      843 2023-06-14 18:46:01.938655 talkytrend-1.2.0/talkytrend/default_settings.toml
+-rw-r--r--   0        0        0     6222 2023-06-14 18:46:01.938655 talkytrend-1.2.0/talkytrend/main.py
+-rw-r--r--   0        0        0     2955 1970-01-01 00:00:00.000000 talkytrend-1.2.0/PKG-INFO
```

### Comparing `talkytrend-1.1.9/LICENSE` & `talkytrend-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytrend-1.1.9/README.md` & `talkytrend-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `talkytrend-1.1.9/pyproject.toml` & `talkytrend-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talkytrend"
-version = "1.1.9"
+version = "1.2.0"
 description = "A python package to retrieve  economic data such as Trend for any financial symbol."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["finance", "crypto", "bot","trend","economic"]
 packages = [
     {include = "talkytrend"}
@@ -18,14 +18,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.10"
 asyncio = "*"
 dynaconf = "*"
 aiohttp = "*"
 tradingview_ta = "*"
+prettytable = "*"
 
 [tool.poetry.dev-dependencies]
 python-semantic-release = "*"
 pytest = "^7.0.0"
 pytest-cov = "*"
 pytest-asyncio = "*"
 pytest-mock = "*"
```

### Comparing `talkytrend-1.1.9/talkytrend/config.py` & `talkytrend-1.2.0/talkytrend/config.py`

 * *Files identical despite different names*

### Comparing `talkytrend-1.1.9/talkytrend/main.py` & `talkytrend-1.2.0/talkytrend/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
  talky trend Main
 """
 
 import asyncio
 import logging
 from datetime import date
 import aiohttp
+from prettytable import PrettyTable
 from tradingview_ta import TA_Handler
 from talkytrend import __version__
 from .config import settings
 
 class TalkyTrend:
     def __init__(self):
         self.logger = logging.getLogger("TalkyTrend")
@@ -38,14 +39,16 @@
             return analysis.summary["RECOMMENDATION"]
         except Exception as error:
             self.logger.error("event %s",error)
 
     async def check_signal(self):
         try:
             signals = []
+            table = PrettyTable()
+            table.field_names = ["Asset", "4h"]
             for asset in self.assets:
                 current_signal = await self.fetch_analysis(
                     asset_id=asset["id"],
                     exchange=asset["exchange"],
                     screener=asset["screener"],
                     interval=asset["interval"]
                 )
@@ -53,19 +56,23 @@
                 if self.is_new_signal(asset["id"], asset["interval"], current_signal):
                     signal_item = {
                         "symbol": asset["id"],
                         "interval": asset["interval"],
                         "signal": current_signal
                     }
                     self.logger.debug("signal message %s", signal_item)
+                    print(asset["id"], current_signal)
                     self.update_signal(asset["id"], asset["interval"], current_signal)
+                    table.add_row([asset["id"], current_signal])
+                    self.logger.debug("table %s", table)
                     signals.append(signal_item)
                 self.logger.debug("asset_signals %s", self.asset_signals)
                 self.logger.debug("signals %s", signals)
-            return signals
+            #return signals
+            return str(table)
         except Exception as error:
             self.logger.error("check_signal %s", error)
             return []
 
 
 
     def is_new_signal(self, asset_id, interval, current_signal):
@@ -107,52 +114,43 @@
             self.logger.error("event %s",error)
     
     async def fetch_key_news(self):
         try:
             async with aiohttp.ClientSession() as session:
                 async with session.get(self.news_url, timeout=10) as response:
                     data = await response.json()
-                    if not (articles := data.get('articles')):
-                        return None
-                    key_news = []
-                    for article in articles:
-                        news_item = {
-                            'title': article['title'],
-                            'url': article['url']
-                        }
-                        key_news.append(news_item)
-                    self.logger.debug("key_news %s",key_news)
-                    return key_news
-        except Exception as error:
-            self.logger.error("news %s",error)
+                    articles = data.get('articles', [])
+                    key_news = [{'title': article['title'], 'url': article['url']} for article in articles]
+                    self.logger.debug("key_news %s", key_news)
+                    last_item = key_news[-1]
+                    return f"{last_item['title']} {last_item['url']}"
+        except aiohttp.ClientError as error:
+            self.logger.error("news %s", error)
+            return None
+
 
     async def scanner(self):
         while True:
             try:
-                tasks = [
-                    self.fetch_key_events(),
-                    self.fetch_key_news(),
-                    self.check_signal()
-                ]
-                results = await asyncio.gather(*tasks)
-
-                if results[0] is not None:
-                    self.logger.debug("Key event %s", results[0])
-                    yield results[0]
-
-                if results[1]:
-                    if results[1][0] is not None:
-                        self.logger.debug("Key news %s", results[1][0])
-                        yield results[1][0]
-
-                if results[2]:
-                    for signal in results[2]:
+                key_events = await self.fetch_key_events()
+                if key_events is not None:
+                    self.logger.debug("Key event %s", key_events)
+                    yield key_events
+
+                key_news = await self.fetch_key_news()
+                if key_news is not None:
+                    self.logger.debug("Key news %s", key_news)
+                    yield key_news
+
+                signals = await self.check_signal()
+                if signals:
+                    for signal in signals:
                         message = f"New signal for {signal['symbol']} ({signal['interval']}): {signal['signal']}"
                         self.logger.debug("Signal message %s", message)
                         yield message
 
-
             except Exception as error:
                 self.logger.error("scanner %s", error)
 
             await asyncio.sleep(settings.scanner_frequency)
 
+
```

### Comparing `talkytrend-1.1.9/PKG-INFO` & `talkytrend-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: talkytrend
-Version: 1.1.9
+Version: 1.2.0
 Summary: A python package to retrieve  economic data such as Trend for any financial symbol.
 License: MIT
 Keywords: finance,crypto,bot,trend,economic
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp
 Requires-Dist: asyncio
 Requires-Dist: dynaconf
+Requires-Dist: prettytable
 Requires-Dist: tradingview_ta
 Project-URL: Changelog, https://github.com/mraniki/talkytrend/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/talkytrend/issues
 Project-URL: Support, https://github.com/mraniki/talkytrend/discussions
 Description-Content-Type: text/markdown
 
 # TalkyTrend
```

