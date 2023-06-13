# Comparing `tmp/aiomql-1.tar.gz` & `tmp/aiomql-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiomql-1.tar", last modified: Thu Feb 23 16:00:25 2023, max compression
+gzip compressed data, was "aiomql-2.0.0.tar", last modified: Tue Jun 13 22:50:09 2023, max compression
```

## Comparing `aiomql-1.tar` & `aiomql-2.0.0.tar`

### file list

```diff
@@ -1,54 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-02-23 16:00:25.348288 aiomql-1/
--rw-rw-rw-   0        0        0     1092 2023-02-23 15:40:36.000000 aiomql-1/LICENSE
--rw-rw-rw-   0        0        0     3261 2023-02-23 16:00:25.341291 aiomql-1/PKG-INFO
--rw-rw-rw-   0        0        0     2649 2023-02-23 15:40:36.000000 aiomql-1/README.md
--rw-rw-rw-   0        0        0      803 2023-02-23 15:59:03.000000 aiomql-1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-23 16:00:25.350291 aiomql-1/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-02-23 15:40:36.000000 aiomql-1/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-23 16:00:21.978362 aiomql-1/src/
-drwxrwxrwx   0        0        0        0 2023-02-23 16:00:24.372289 aiomql-1/src/aiomql/
--rw-rw-rw-   0        0        0      615 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/__init__.py
--rw-rw-rw-   0        0        0     1907 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/account.py
--rw-rw-rw-   0        0        0     4370 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/bot_builder.py
--rw-rw-rw-   0        0        0     3331 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/candle.py
--rw-rw-rw-   0        0        0     4106 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/config.py
-drwxrwxrwx   0        0        0        0 2023-02-23 16:00:24.704292 aiomql-1/src/aiomql/core/
--rw-rw-rw-   0        0        0     3683 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/core/__init__.py
--rw-rw-rw-   0        0        0    37666 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/core/constants.py
--rw-rw-rw-   0        0        0     6686 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/core/meta_trader.py
--rw-rw-rw-   0        0        0    15918 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/core/models.py
--rw-rw-rw-   0        0        0     2221 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/executor.py
--rw-rw-rw-   0        0        0     4542 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/history.py
-drwxrwxrwx   0        0        0        0 2023-02-23 16:00:23.719453 aiomql-1/src/aiomql/lib/
-drwxrwxrwx   0        0        0        0 2023-02-23 16:00:24.829289 aiomql-1/src/aiomql/lib/markets/
--rw-rw-rw-   0        0        0      442 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/lib/markets/forex_market.py
--rw-rw-rw-   0        0        0      500 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/lib/markets/synthetic_market.py
-drwxrwxrwx   0        0        0        0 2023-02-23 16:00:24.923290 aiomql-1/src/aiomql/lib/strategies/
--rw-rw-rw-   0        0        0     5433 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/lib/strategies/finger_trap.py
-drwxrwxrwx   0        0        0        0 2023-02-23 16:00:24.946292 aiomql-1/src/aiomql/lib/symbols/
--rw-rw-rw-   0        0        0     1166 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/lib/symbols/forex_symbol.py
--rw-rw-rw-   0        0        0      767 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/lib/symbols/synthetic_symbol.py
-drwxrwxrwx   0        0        0        0 2023-02-23 16:00:25.035291 aiomql-1/src/aiomql/lib/traders/
--rw-rw-rw-   0        0        0     2715 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/lib/traders/simple_deal_trader.py
--rw-rw-rw-   0        0        0     4261 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/market.py
--rw-rw-rw-   0        0        0     3915 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/order.py
--rw-rw-rw-   0        0        0     2885 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/positions.py
--rw-rw-rw-   0        0        0     3436 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/records.py
--rw-rw-rw-   0        0        0     3344 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/result.py
--rw-rw-rw-   0        0        0     3161 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/strategy.py
--rw-rw-rw-   0        0        0     8748 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/symbol.py
--rw-rw-rw-   0        0        0     5865 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/terminal.py
--rw-rw-rw-   0        0        0     1617 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/ticks.py
--rw-rw-rw-   0        0        0     1286 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/trader.py
--rw-rw-rw-   0        0        0      111 2023-02-23 15:40:36.000000 aiomql-1/src/aiomql/utils.py
-drwxrwxrwx   0        0        0        0 2023-02-23 16:00:24.585287 aiomql-1/src/aiomql.egg-info/
--rw-rw-rw-   0        0        0     3261 2023-02-23 16:00:21.000000 aiomql-1/src/aiomql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1057 2023-02-23 16:00:21.000000 aiomql-1/src/aiomql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-23 16:00:21.000000 aiomql-1/src/aiomql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-02-23 16:00:21.000000 aiomql-1/src/aiomql.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-02-23 16:00:21.000000 aiomql-1/src/aiomql.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-23 16:00:25.288289 aiomql-1/tests/
--rw-rw-rw-   0        0        0      331 2023-02-23 15:40:36.000000 aiomql-1/tests/test_config.py
--rw-rw-rw-   0        0        0      132 2023-02-23 15:40:36.000000 aiomql-1/tests/test_constants.py
--rw-rw-rw-   0        0        0      224 2023-02-23 15:40:36.000000 aiomql-1/tests/test_symbol.py
--rw-rw-rw-   0        0        0      602 2023-02-23 15:40:36.000000 aiomql-1/tests/test_terminal.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:50:09.756431 aiomql-2.0.0/
+-rw-rw-rw-   0        0        0     1092 2023-04-10 06:55:09.000000 aiomql-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0     2284 2023-06-13 22:50:09.754411 aiomql-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1668 2023-06-13 22:43:24.000000 aiomql-2.0.0/README.md
+-rw-rw-rw-   0        0        0      807 2023-06-13 22:43:24.000000 aiomql-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-13 22:50:09.756431 aiomql-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-04-10 06:55:09.000000 aiomql-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:50:09.587355 aiomql-2.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-13 22:50:09.676005 aiomql-2.0.0/src/aiomql/
+-rw-rw-rw-   0        0        0      606 2023-06-13 22:43:24.000000 aiomql-2.0.0/src/aiomql/__init__.py
+-rw-rw-rw-   0        0        0     2960 2023-06-13 22:43:24.000000 aiomql-2.0.0/src/aiomql/account.py
+-rw-rw-rw-   0        0        0     3203 2023-06-13 22:43:24.000000 aiomql-2.0.0/src/aiomql/bot_builder.py
+-rw-rw-rw-   0        0        0     6195 2023-06-13 22:43:24.000000 aiomql-2.0.0/src/aiomql/candle.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:50:09.717242 aiomql-2.0.0/src/aiomql/core/
+-rw-rw-rw-   0        0        0       63 2023-06-13 22:43:24.000000 aiomql-2.0.0/src/aiomql/core/__init__.py
+-rw-rw-rw-   0        0        0     4675 2023-06-13 22:43:24.000000 aiomql-2.0.0/src/aiomql/core/base.py
+-rw-rw-rw-   0        0        0     3787 2023-06-13 22:43:24.000000 aiomql-2.0.0/src/aiomql/core/config.py
+-rw-rw-rw-   0        0        0    38122 2023-06-13 22:43:24.000000 aiomql-2.0.0/src/aiomql/core/constants.py
+-rw-rw-rw-   0        0        0     6783 2023-06-13 22:43:24.000000 aiomql-2.0.0/src/aiomql/core/meta_trader.py
+-rw-rw-rw-   0        0        0    16658 2023-06-13 22:43:24.000000 aiomql-2.0.0/src/aiomql/core/models.py
+-rw-rw-rw-   0        0        0     2183 2023-06-13 22:43:24.000000 aiomql-2.0.0/src/aiomql/executor.py
+-rw-rw-rw-   0        0        0     4683 2023-06-13 22:43:24.000000 aiomql-2.0.0/src/aiomql/history.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:50:09.719454 aiomql-2.0.0/src/aiomql/lib/
+-rw-rw-rw-   0        0        0      198 2023-06-13 22:14:26.000000 aiomql-2.0.0/src/aiomql/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:50:09.727329 aiomql-2.0.0/src/aiomql/lib/strategies/
+-rw-rw-rw-   0        0        0        0 2023-05-06 20:55:40.000000 aiomql-2.0.0/src/aiomql/lib/strategies/__init__.py
+-rw-rw-rw-   0        0        0     7214 2023-06-13 22:43:24.000000 aiomql-2.0.0/src/aiomql/lib/strategies/finger_trap.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:50:09.734770 aiomql-2.0.0/src/aiomql/lib/symbols/
+-rw-rw-rw-   0        0        0       86 2023-06-10 11:42:24.000000 aiomql-2.0.0/src/aiomql/lib/symbols/__init__.py
+-rw-rw-rw-   0        0        0     1137 2023-06-13 22:43:24.000000 aiomql-2.0.0/src/aiomql/lib/symbols/forex_symbol.py
+-rw-rw-rw-   0        0        0      965 2023-06-13 22:43:24.000000 aiomql-2.0.0/src/aiomql/lib/symbols/synthetic_symbol.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:50:09.740645 aiomql-2.0.0/src/aiomql/lib/traders/
+-rw-rw-rw-   0        0        0     2653 2023-06-13 22:43:24.000000 aiomql-2.0.0/src/aiomql/lib/traders/simple_deal_trader.py
+-rw-rw-rw-   0        0        0      979 2023-06-11 16:02:42.000000 aiomql-2.0.0/src/aiomql/lib/traders/trade_result.py
+-rw-rw-rw-   0        0        0     3651 2023-06-13 22:43:24.000000 aiomql-2.0.0/src/aiomql/order.py
+-rw-rw-rw-   0        0        0     2777 2023-06-13 22:43:24.000000 aiomql-2.0.0/src/aiomql/positions.py
+-rw-rw-rw-   0        0        0     2720 2023-06-13 22:43:24.000000 aiomql-2.0.0/src/aiomql/records.py
+-rw-rw-rw-   0        0        0     1992 2023-06-13 22:43:24.000000 aiomql-2.0.0/src/aiomql/result.py
+-rw-rw-rw-   0        0        0     2655 2023-06-13 22:43:24.000000 aiomql-2.0.0/src/aiomql/strategy.py
+-rw-rw-rw-   0        0        0    11560 2023-06-13 22:43:24.000000 aiomql-2.0.0/src/aiomql/symbol.py
+-rw-rw-rw-   0        0        0     4604 2023-06-13 22:43:24.000000 aiomql-2.0.0/src/aiomql/terminal.py
+-rw-rw-rw-   0        0        0     2581 2023-06-13 22:43:24.000000 aiomql-2.0.0/src/aiomql/ticks.py
+-rw-rw-rw-   0        0        0     1200 2023-06-13 22:43:24.000000 aiomql-2.0.0/src/aiomql/trader.py
+-rw-rw-rw-   0        0        0      208 2023-06-13 22:43:24.000000 aiomql-2.0.0/src/aiomql/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:50:09.694761 aiomql-2.0.0/src/aiomql.egg-info/
+-rw-rw-rw-   0        0        0     2284 2023-06-13 22:50:09.000000 aiomql-2.0.0/src/aiomql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1033 2023-06-13 22:50:09.000000 aiomql-2.0.0/src/aiomql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 22:50:09.000000 aiomql-2.0.0/src/aiomql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-06-13 22:50:09.000000 aiomql-2.0.0/src/aiomql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-13 22:50:09.000000 aiomql-2.0.0/src/aiomql.egg-info/top_level.txt
```

### Comparing `aiomql-1/LICENSE` & `aiomql-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiomql-1/PKG-INFO` & `aiomql-2.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiomql
-Version: 1
+Version: 2.0.0
 Summary: Asynchronous MetaTrader5 library and Bot Builder
 Author-email: Ichinga Samuel <ichingasamuel@gmail.com>
 Project-URL: Homepage, https://github.com/Ichinga-Samuel/aiomql
 Project-URL: Bug Tracker, https://github.com/Ichinga-Samuel/aiomql/issues
 Keywords: MetaTrader5,Asynchronous,Algorithmic Trading,Trading Bot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,86 +13,65 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # aiomql
 ![GitHub](https://img.shields.io/github/license/ichinga-samuel/aiomql?style=plastic)
 ![GitHub issues](https://img.shields.io/github/issues/ichinga-samuel/aiomql?style=plastic)
 ![PyPI](https://img.shields.io/pypi/v/aiomql)
-![GitHub Workflow Status](https://img.shields.io/github/workflow/status/ichinga-samuel/aiomql/Push)
-![Libraries.io dependency status for GitHub repo](https://img.shields.io/librariesio/github/ichinga-samuel/aiomql)
+
 
 ## Installation
 ```bash
 pip install aiomql
 ```
 
 ## Key Features
 - Asynchronous Python Library For MetaTrader 5
 - Build bots for trading in different financial markets using a bot factory
-- Use threadpool or proccesspool executors to run multiple strategies on multiple instruments concurrently
+- Use threadpool executors to run multiple strategies on multiple instruments concurrently
 - Record and keep track of trades and strategies in csv files.
 - Utility classes for using the MetaTrader 5 Library
 - Sample Pre-Built strategies
 
-## Simple Usage as an Async MetaTrader5 Libray
+## Simple Usage as an asynchronous MetaTrader5 Libray
 ```python
 import asyncio
 
 # import the class
-from aiomql import MetaTrader
-from aiomql import Account, Terminal
-from aiomql import TimeFrame, OrderType
+from aiomql import MetaTrader, Account, TimeFrame, OrderType
 
 
 async def main():
-    # Initialize Terminal
-    terminal = Terminal()
-    mt5 = MetaTrader()
-    await mt5.initialize()
-
-    # create Account
-    account = Account(account_number=30371334, password="nwa0#anaEze", server="Deriv-Demo")
-
-    # login with account
-    await account.login()
-
-    # connection status with the account.connected property
-    res = "Login Successful" if account.connected else "Unable to login into account"
-    print(res)
-
-    # set account properties
-    account.risk = 0.10  # percentage of account equity to risk i.e 10%
-    account.risk_to_reward = 3
-
-    # get symbols available for the account if login was successful
-    if account.connected:
-        symbols = await mt5.symbols_get()
-        print(symbols)
-
-    # print timeframe constant for five minutes
-    print(TimeFrame.M5)
-    await terminal.shutdown()
-
+    # Assuming your login details are already defined in the aiomql.json somewhere in your project directory. 
+    acc = Account()
+    
+    # if this is unsuccessful the program exits
+    await acc.initialize()
+    
+    # print all available symbols
+    print(acc.symbols)
 
 asyncio.run(main())
 ```
-## As a Bot Building FrameWork using a Prebuilt Strategy
+## As a Bot Building FrameWork using a Sample Strategy
 ```python
-import logging
-
 from aiomql import Bot
-from aiomql.lib import ForexMarket, FingerTrap
+from aiomql import ForexSymbol
+from aiomql.lib import FingerTrap
+
+# Create a bot instance
+bot = Bot()
 
-fmt = "%(asctime)s : %(message)s"
+# Choose a Symbol to trade
+symbol = ForexSymbol(name='EURUSD')
 
-logging.basicConfig(filename='example.log', format=fmt, level=logging.DEBUG)
+# Create a strategy
+ft_eur_usd = FingerTrap(symbol=symbol)
 
-market = ForexMarket()
-bot = Bot(market=market)
+# Add strategy to Bot
+bot.add_strategy(ft_eur_usd)
 
-# Finger strategy on all instruments in the forex markets
-bot.add_strategy_all(strategy=FingerTrap)
+# run the bot
 bot.execute()
-# This assumes that a mt5.json config file with account_number, password and server keys is available
 ```
 
 see [docs](https://github.com/Ichinga-Samuel/aiomql/tree/master/docs)
```

### Comparing `aiomql-1/README.md` & `aiomql-2.0.0/src/aiomql.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,83 +1,77 @@
+Metadata-Version: 2.1
+Name: aiomql
+Version: 2.0.0
+Summary: Asynchronous MetaTrader5 library and Bot Builder
+Author-email: Ichinga Samuel <ichingasamuel@gmail.com>
+Project-URL: Homepage, https://github.com/Ichinga-Samuel/aiomql
+Project-URL: Bug Tracker, https://github.com/Ichinga-Samuel/aiomql/issues
+Keywords: MetaTrader5,Asynchronous,Algorithmic Trading,Trading Bot
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # aiomql
 ![GitHub](https://img.shields.io/github/license/ichinga-samuel/aiomql?style=plastic)
 ![GitHub issues](https://img.shields.io/github/issues/ichinga-samuel/aiomql?style=plastic)
 ![PyPI](https://img.shields.io/pypi/v/aiomql)
-![GitHub Workflow Status](https://img.shields.io/github/workflow/status/ichinga-samuel/aiomql/Push)
-![Libraries.io dependency status for GitHub repo](https://img.shields.io/librariesio/github/ichinga-samuel/aiomql)
+
 
 ## Installation
 ```bash
 pip install aiomql
 ```
 
 ## Key Features
 - Asynchronous Python Library For MetaTrader 5
 - Build bots for trading in different financial markets using a bot factory
-- Use threadpool or proccesspool executors to run multiple strategies on multiple instruments concurrently
+- Use threadpool executors to run multiple strategies on multiple instruments concurrently
 - Record and keep track of trades and strategies in csv files.
 - Utility classes for using the MetaTrader 5 Library
 - Sample Pre-Built strategies
 
-## Simple Usage as an Async MetaTrader5 Libray
+## Simple Usage as an asynchronous MetaTrader5 Libray
 ```python
 import asyncio
 
 # import the class
-from aiomql import MetaTrader
-from aiomql import Account, Terminal
-from aiomql import TimeFrame, OrderType
+from aiomql import MetaTrader, Account, TimeFrame, OrderType
 
 
 async def main():
-    # Initialize Terminal
-    terminal = Terminal()
-    mt5 = MetaTrader()
-    await mt5.initialize()
-
-    # create Account
-    account = Account(account_number=30371334, password="nwa0#anaEze", server="Deriv-Demo")
-
-    # login with account
-    await account.login()
-
-    # connection status with the account.connected property
-    res = "Login Successful" if account.connected else "Unable to login into account"
-    print(res)
-
-    # set account properties
-    account.risk = 0.10  # percentage of account equity to risk i.e 10%
-    account.risk_to_reward = 3
-
-    # get symbols available for the account if login was successful
-    if account.connected:
-        symbols = await mt5.symbols_get()
-        print(symbols)
-
-    # print timeframe constant for five minutes
-    print(TimeFrame.M5)
-    await terminal.shutdown()
-
+    # Assuming your login details are already defined in the aiomql.json somewhere in your project directory. 
+    acc = Account()
+    
+    # if this is unsuccessful the program exits
+    await acc.initialize()
+    
+    # print all available symbols
+    print(acc.symbols)
 
 asyncio.run(main())
 ```
-## As a Bot Building FrameWork using a Prebuilt Strategy
+## As a Bot Building FrameWork using a Sample Strategy
 ```python
-import logging
-
 from aiomql import Bot
-from aiomql.lib import ForexMarket, FingerTrap
+from aiomql import ForexSymbol
+from aiomql.lib import FingerTrap
+
+# Create a bot instance
+bot = Bot()
 
-fmt = "%(asctime)s : %(message)s"
+# Choose a Symbol to trade
+symbol = ForexSymbol(name='EURUSD')
 
-logging.basicConfig(filename='example.log', format=fmt, level=logging.DEBUG)
+# Create a strategy
+ft_eur_usd = FingerTrap(symbol=symbol)
 
-market = ForexMarket()
-bot = Bot(market=market)
+# Add strategy to Bot
+bot.add_strategy(ft_eur_usd)
 
-# Finger strategy on all instruments in the forex markets
-bot.add_strategy_all(strategy=FingerTrap)
+# run the bot
 bot.execute()
-# This assumes that a mt5.json config file with account_number, password and server keys is available
 ```
 
 see [docs](https://github.com/Ichinga-Samuel/aiomql/tree/master/docs)
```

### Comparing `aiomql-1/pyproject.toml` & `aiomql-2.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aiomql"
-version = "1"
+version = "2.0.0"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `aiomql-1/src/aiomql/__init__.py` & `aiomql-2.0.0/src/aiomql/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from .account import Account, account
+from .account import Account
 from .symbol import Symbol
-from .strategy import Strategy, Entry
+from .strategy import Strategy
 from .bot_builder import Bot
-from .result import TradeResult
+from .result import Result
 from .records import Records
 from .candle import Candle, Candles
 from .positions import Positions
 from .executor import Executor
 from .order import Order
-from .ticks import Tick
+from .ticks import Tick, Ticks
 from .history import History
 from .trader import Trader
-from .market import Market
 from .terminal import Terminal, terminal
-from .config import Config
 
+from .core.config import Config
 from .core .constants import *
 from .core .meta_trader import MetaTrader
 from .core .models import *
+from .lib.symbols import *
```

### Comparing `aiomql-1/src/aiomql/candle.py` & `aiomql-2.0.0/src/aiomql/ticks.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,113 +1,85 @@
-from typing import Union, Type
+from typing import Union, TypeVar
 
-from pandas import DataFrame
+from pandas import DataFrame, Series
 
-from .core import Base
+from .core.constants import TickFlag
 
 
-class Candle(Base):
-    """
-    A class representing rates from the charts as Japanese Candlesticks.
-    Subclass this class to add needed properties.
-    Attributes:
-        Index (int): Position of the candle in the chart. Zero represents the most recent
-        time (int): Period start time.
-        open (int): Open price
-        high (float): The highest price of the period
-        low (float): The lowest price of the period
-        close (float): Close price
-        tick_volume (float): Tick volume
-        real_volume (float): Trade volume
-        spread (float): Spread
-        ema (float, optional): ema
-    """
-    Index: int
-    time: int
-    open: float
-    high: float
-    low: float
-    close: float
-    tick_volume: float
-    real_volume: float
-    spread: float
-    ema: float
-
-    def __lt__(self, other: 'Candle'):
-        return self.Index < other.Index
-
-    # def __hash__(self):
-    #     return hash(self.time)
-
-    @property
-    def mid(self) -> float:
-        """
-        The mid of open and close
-        Returns: mid
-
-        """
-        return (self.open + self.close) / 2
+Self = TypeVar('Self', bound='Ticks')
 
-    def is_bullish(self) -> bool:
-        """
-        Returns: True or Fasle
 
-        """
-        return self.close > self.open
-
-    def is_bearish(self) -> bool:
-        """
-
-        Returns: True or False
-
-        """
-        return self.open > self.close
-
-    def is_hanging_man(self, ratio=1.5):
-        return max((self.open - self.low), (self.high - self.close)) / (self.close - self.open) >= ratio
+class Tick:
+    """
+    Price Tick of a Financial Instrument or symbol.
 
-    def is_bullish_hammer(self, ratio=1.5):
-        return max((self.close - self.low), (self.high - self.open)) / (self.open - self.close) >= ratio
+    Notes: All initialization arguments are assumed to be class attributes.
+    """
+    def __init__(self, *, time: int, bid: float, ask: float, last: float, volume: float, time_msc: int, flags: TickFlag,
+                 volume_real: float, Index: int = 0, **kwargs):
+        self.time = time
+        self.bid = bid
+        self.ask = ask
+        self.last = last
+        self.volume = volume
+        self.time_msc = time_msc
+        self.flags = flags
+        self.volume_real = volume_real
+        self.Index = Index
+        [setattr(self, key, value) for key, value in kwargs.items()]
 
 
-class Candles:
+class Ticks:
     """
-    A class representing a collection of rates as Candle Objects, Arranged chronologically.
-    Class is an iterable container
+    Container data class for price ticks. Arrange in chronological order.
+    Supports iteration, slicing and assignment
 
     Args:
-        data (DataFrame, tuple[tuple]): A pandas dataframe or a tuple of tuple as returned from the terminal
+        data (DataFrame | tuple[tuple]): Dataframe of price ticks or a tuple of tuples
 
     Keyword Args:
-        candle (Type(Candle)): Type of Candle object represented by the class.
         flip (bool): If flip is True reverse data argument.
 
     Attributes:
-        _data: Dataframe Object holding the rates
-        Candle: Candle class for individual objects
+        data: Dataframe Object holding the ticks
     """
-    def __init__(self, *, data: DataFrame | tuple[tuple], candle: Type[Candle] = Candle, flip=True):
-        data = DataFrame(data) if not isinstance(data, DataFrame) else data
+    time: Series
+    bid: Series
+    ask: Series
+    last: Series
+    volume: Series
+    time_msc: Series
+    flags: Series
+    volume_real: Series
+    Index: Series
+
+    def __init__(self, *, data: DataFrame | tuple[tuple], flip=False):
+        data: DataFrame = DataFrame(data) if not isinstance(data, DataFrame) else data
         self._data = data.iloc[::-1] if flip else data
-        self.Candle = candle
 
     def __len__(self):
         return self._data.shape[0]
 
-    def __contains__(self, item: Candle):
-        return item.time == self[item.Index].time
+    def __contains__(self, item: Tick) -> bool:
+        return item.time_msc == self[item.Index].time_msc
+
+    def __getattribute__(self, item):
+        if item in {'time', 'bid', 'ask', 'last', 'volume', 'time_msc', 'flags', 'volume_real', 'Index'}:
+            return self._data[item]
+        return super(Ticks, self).__getattribute__(item)
 
-    def __getitem__(self, index) -> Union[type(Candle), "Candles"]:
+    def __getitem__(self, index) -> Tick | Self:
         if isinstance(index, slice):
             cls = self.__class__
             data = self._data.iloc[index]
-            return cls(data=data, candle=self.Candle, flip=False)
+            data.reset_index(drop=True, inplace=True)
+            return cls(data=data)
 
         item = self._data.iloc[index]
-        return self.Candle(Index=index, **item)
+        return Tick(Index=index, **item)
 
     def __iter__(self):
-        return (self.Candle(**row._asdict()) for row in self._data.itertuples())
+        return (Tick(**row._asdict()) for row in self._data.itertuples())
 
     @property
-    def data(self):
+    def data(self) -> DataFrame:
         return self._data
```

### Comparing `aiomql-1/src/aiomql/config.py` & `aiomql-2.0.0/src/aiomql/core/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,121 +1,113 @@
 import os
 from pathlib import Path
 from sys import _getframe
-from typing import Iterator, Literal
+from typing import Iterator
 import json
-from functools import cache
+from logging import getLogger
+
+logger = getLogger()
 
 
 class Config:
     """
     Set config variables for your bot
-
     Keyword Args:
         file (str): config file
         record_trades (bool): If true record trade in a csv file defaults to True
         filename (str): Name of config file, defaults to "mt5.json"
-        executor: Type of pool executor, can be thread or process defaults to thread
         records_dir(str): Name of directory for saving trades, defaults to trade records
         win_percentage (float): Percentage of expected profit that counts as a win
         base_dir (str | Path): Base directory for saving outputs.
 
     Attributes:
         file (str):
         record_trades (bool):
         filename (str):
-        executor (str):
         records_dir (str):
         win_percentage (float):
         base_dir (str | Path):
         account_number (int): Broker account number for
         password (str): Broker password
         server (str): Broker server
         path (str): Path to terminal file
     """
-    account_number: int
-    password: str
-    server: str
-    path: str
-
+    login: int = 0
+    password: str = ""
+    server: str = ""
+    path: str = ""
+    timeout: int = 60000
+    record_trades: bool = True
+    filename: str = "aiomql.json"
+    file = None
+    win_percentage: float = 0.85
+    
     def __new__(cls, *args, **kwargs):
         if not hasattr(cls, '_instance'):
             cls._instance = super().__new__(cls)
         return cls._instance
-
-    def __init__(self, *, file: str = "", record_trades: bool = True, filename: str = "mt5.json",
-                 executor: Literal['thread', 'process'] = "thread", base_dir: str | Path = "", win_percentage: float = 0.85,
-                 records_dir: str = "trade_records", **kwargs):
-        self.record_trades = record_trades
-        self.executor = executor
-        self.filename = filename
-        self.win_percentage = win_percentage
-        self.file = file
-        self.base_dir = base_dir or Path.cwd()
-        self.records_dir = self.base_dir / records_dir
+    
+    def __init__(self, **kwargs):
         self.set_attributes(**kwargs)
-        self.load_json()
-
-    def __setattr__(self, key, value):
-        if key == 'base_dir' or key == 'records_dir' and isinstance(value, str):
-            super().__setattr__(key, Path(value))
-            return
-        super().__setattr__(key, value)
-
+        self.records_dir = Path.home() / 'Documents' / 'Aiomql' / 'Trade Records'
+        self.records_dir.mkdir(parents=True, exist_ok=True)
+        self.load_config()
+    
+    @staticmethod
+    def walk_to_root(path: str) -> Iterator[str]:
+        
+        if not os.path.exists(path):
+            raise IOError('Starting path not found')
+        
+        if os.path.isfile(path):
+            path = os.path.dirname(path)
+        
+        last_dir = None
+        current_dir = os.path.abspath(path)
+        while last_dir != current_dir:
+            yield current_dir
+            parent_dir = os.path.abspath(os.path.join(current_dir, os.path.pardir))
+            last_dir, current_dir = current_dir, parent_dir
+    
     def find_config(self):
         current_file = __file__
         frame = _getframe()
         while frame.f_code.co_filename == current_file:
             if frame.f_back is None:
-                return False
+                return None
             frame = frame.f_back
         frame_filename = frame.f_code.co_filename
         path = os.path.dirname(os.path.abspath(frame_filename))
-
+        
         for dirname in self.walk_to_root(path):
             check_path = os.path.join(dirname, self.filename)
             if os.path.isfile(check_path):
-                self.file = check_path
-                return True
-        return False
-
-    def load_json(self):
-        res = self.file or self.find_config()
-        if not res:
+                return check_path
+        return None
+    
+    def load_config(self, file: str = None):
+        if (file := (file or self.find_config())) is None:
+            logger.warning('No Config File Found')
             return
-        fh = open(self.file, mode='r')
+        fh = open(file, mode='r')
         data = json.load(fh)
         fh.close()
         [setattr(self, key, value) for key, value in data.items()]
 
-    @cache
-    def load(self, file: str):
-        fh = open(file, mode='r')
-        data = json.load(fh)
-        self.set_attributes(**data)
+    def account_info(self) -> dict['login', 'password', 'server']:
+        """
+           Returns Account Info as found in the config object if available
 
+           Returns (dict): A dictionary of account properties
+        """
+        return {'login': self.login, 'password': self.password, 'server': self.server}
+    
     def set_attributes(self, **kwargs):
         """
         Add attributes to the config object
         Args:
             **kwargs: Set attributes as keyword arguments
 
         Returns:
 
         """
         [setattr(self, i, j) for i, j in kwargs.items()]
-
-    @staticmethod
-    def walk_to_root(path: str) -> Iterator[str]:
-
-        if not os.path.exists(path):
-            raise IOError('Starting path not found')
-
-        if os.path.isfile(path):
-            path = os.path.dirname(path)
-
-        last_dir = None
-        current_dir = os.path.abspath(path)
-        while last_dir != current_dir:
-            yield current_dir
-            parent_dir = os.path.abspath(os.path.join(current_dir, os.path.pardir))
-            last_dir, current_dir = current_dir, parent_dir
```

### Comparing `aiomql-1/src/aiomql/core/__init__.py` & `aiomql-2.0.0/src/aiomql/core/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,85 +1,122 @@
-from typing import Iterable, Mapping
 from functools import cache
+from typing import Mapping, Iterable
+from logging import getLogger
 
-import MetaTrader5
+from .config import Config
+from .meta_trader import MetaTrader
+
+logger = getLogger()
 
 
 class Base:
     """
-    Sets all arguments as class properties
+    Base class for data model with setup and data accessing functionalities.
+    Attributes defined on the class body with type annotations help with type hinting and initializing the attribute.
 
     Args:
         **kwargs: Object attributes and values as keyword arguments
+
+    Attributes:
+        mt5 (ClassVar, MetaTrader): The MetaTrader Instance
+
+        config (ClassVar, Config): Singleton class Variable
     """
+    mt5: MetaTrader = MetaTrader()
+    config = Config()
+
     def __init__(self, **kwargs):
         self.set_attributes(**kwargs)
 
     def __repr__(self):
         values = ', '.join(f"{name}={value!r}" for name, value in self.__dict__.items())
         return f"{self.__class__.__name__}({values})"
 
     def set_attributes(self, **kwargs):
         """
         Set keyword arguments as object attributes
+        
         Args:
             **kwargs: Object attributes and values as keyword arguments
-        Returns:
 
         Raises:
             AttributeError: When assigning an attribute that does not belong to the class or any parent class
+
+        Notes:
+            Only sets attributes that have been annotated on the class body.
         """
         for i, j in kwargs.items():
             try:
                 setattr(self, i, self.annotations[i](j))
             except KeyError:
-                raise AttributeError(f"Attribute {i} does not belong to class {self.__class__.__name__}")
+                logger.warning(f"Attribute {i} does not belong to class {self.__class__.__name__}")
+                continue
+            except Exception as exe:
+                logger.warning(f'Did not set attribute {i} on class {self.__class__.__name__} due to {exe}')
+                continue
 
     @property
     @cache
     def annotations(self) -> dict:
-        init = {}
+        """
+        Returns annotations defined on the class body and it's parent classes as dictionary
+
+        Returns:
+            annotations (dict): dictionary of annotations
+
+        """
+        annots = {}
         for base in self.__class__.__mro__[-3::-1]:
-            init |= getattr(base, '__annotations__', {})
-        return init
+            annots |= getattr(base, '__annotations__', {})
+        return annots
 
     def get_dict(self, exclude: set = None, include: set = None) -> dict:
         """
-        Returns class attributes as a dict
+        Returns class attributes as a dict, with the ability to filter
+
         Keyword Args:
             exclude: A set of attributes to be excluded
             include: Specific attributes to be returned
 
         Returns:
              dict: A dictionary of specified class attributes
 
-
         Notes:
             You can only set either of include or exclude.
-            If you set both, the values of include will take precedence
+            If you set both, include will take precedence
 
         """
         exclude, include = exclude or set(), include or set()
-        filter = include or set(self.dict.keys()).difference(exclude)
-        return {key: value for key, value in self.dict.items() if key in filter}
+        filter_ = include or set(self.dict.keys()).difference(exclude)
+        return {key: value for key, value in self.dict.items() if key in filter_}
 
     @property
     @cache
     def class_vars(self):
+        """
+        Annotated class attributes
+
+        Returns:
+            A dictionary of available class attributes
+
+        """
         return {key: value for key, value in self.__class__.__dict__.items() if key in self.__class__.__annotations__}
 
     @property
     def dict(self) -> dict:
         """
-        All class attributes as a dictionary, except those in the "Config.except" set
-        Returns:
-            dict: A dictionary of class attributes
+        All instance and class attributes as a dictionary, except those in the "Config.except" set
 
+        Returns:
+            dict: A dictionary of instance and class attributes
         """
-        return {key: value for key, value in self.__dict__.items() | self.class_vars.items() if key not in self.Config.exclude}
+        try:
+            return {key: value for key, value in (self.__dict__ | self.class_vars).items() if key not in self.Config.filter}
+        except Exception as err:
+            logger.warning(err)
 
     @dict.setter
     def dict(self, value: Mapping | Iterable[Iterable]):
         """
         Update the dict property
         Args:
             value (Mapping | Iterable[Iterable]): Value should be a mapping or iterable of key value pairs
@@ -90,23 +127,22 @@
         self.dict.update(value)
 
     class Config:
         """
         Config Object of the class
 
         Attributes:
-            exclude (set): A set of class attributes that will be excluded from the dict property
+            exclude (set): A set of default attributes that will be excluded from the dict property
+            include (set): A set of default attributes that should always be include
         """
-        exclude = {'retcode', 'comment', 'request', 'mt5', 'retcode_external', "Config", "request_id"}
-
-
-class BaseMeta(type):
-    def __new__(mcs, cls_name, bases, cls_dict):
-        platform = cls_dict.get('platform')
-        defaults = {} if platform is None else platform.__dict__
-        defaults = {f'_{key}': value for key, value in defaults.items() if not key.startswith('_')}
-        cls_dict |= defaults
-        return super().__new__(mcs, cls_name, bases, cls_dict)
-
-
-class Platform(metaclass=BaseMeta):
-    platform: MetaTrader5 = MetaTrader5
+        exclude = {'mt5', "Config"}
+        include = set()
+        
+        @classmethod
+        @property
+        def filter(cls) -> set:
+            """
+            Returns:
+
+            """
+            return cls.exclude.difference(cls.include)
+
```

### Comparing `aiomql-1/src/aiomql/core/constants.py` & `aiomql-2.0.0/src/aiomql/core/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 """
 
 
 class Repr:
     __enum_name__ = ""
 
     def __str__(self):
-        return f"{self.__class__.__enum_name__}_{self.name}"
+        return f"{self.__enum_name__}_{self.name}"
 
 
 class TradeAction(Repr, IntEnum):
     """
     TRADE_REQUEST_ACTIONS
     
     Attributes:
@@ -222,14 +222,18 @@
 
         MN1 (int): One Month
 
     Methods:
         time: return the value of the timeframe object in seconds. Used as a property
     """
     __enum_name__ = "TIMEFRAME"
+
+    def __str__(self):
+        return self.name
+
     M1 = mt5.TIMEFRAME_M1
     M2 = mt5.TIMEFRAME_M2
     M3 = mt5.TIMEFRAME_M3
     M4 = mt5.TIMEFRAME_M4
     M5 = mt5.TIMEFRAME_M5
     M6 = mt5.TIMEFRAME_M6
     M10 = mt5.TIMEFRAME_M10
@@ -237,35 +241,43 @@
     M20 = mt5.TIMEFRAME_M20
     M30 = mt5.TIMEFRAME_M30
     H1 = mt5.TIMEFRAME_H1
     H2 = mt5.TIMEFRAME_H2
     H3 = mt5.TIMEFRAME_H3
     H4 = mt5.TIMEFRAME_H4
     H6 = mt5.TIMEFRAME_H6
-    H8 = mt5.TIMEFRAME_H1
+    H8 = mt5.TIMEFRAME_H8
+    H12 = mt5.TIMEFRAME_H12
     D1 = mt5.TIMEFRAME_D1
     W1 = mt5.TIMEFRAME_W1
     MN1 = mt5.TIMEFRAME_MN1
 
     @property
     def time(self):
         """
 
         Returns:
             int: The number of seconds in a TIMEFRAME
 
         Examples:
             >>> t = TimeFrame.H1
             >>> print(t.time)
-            3600
         """
-        times = {1: 60, 2: 120, 3: 180, 4: 240, 5: 300, 6: 360, 10: 600, 15: 900, 20: 1200, 30: 1800, 16385: 3600, 16386: 7200,
-                 16387: 10800, 16388: 14400, 16390: 21600, 16392: 21800, 16408: 86400, 32769: 604800, 49153: 2592000}
+        times = {1: 60, 2: 120, 3: 180, 4: 240, 5: 300, 6: 360, 10: 600, 15: 900, 20: 1200, 30: 1800, 16385: 3600,
+                 16386: 7200, 16387: 10800, 16388: 14400, 16390: 21600, 16392: 28800, 16396: 43200, 16408: 86400,
+                 32769: 604800, 49153: 2592000}
         return times[self]
 
+    @classmethod
+    def get(cls, time):
+        times = {60: 1, 120: 2, 180: 3, 240: 4, 300: 5, 360: 6, 600: 10, 900: 15, 1200: 20, 1800: 30, 3600: 16385,
+                 7200: 16386, 10800: 16387, 14400: 16388, 21600: 16390, 28800: 16392, 43200: 16396, 86400: 16408,
+                 604800: 32769, 2592000: 49153}
+        return TimeFrame(times[int(time)])
+
 
 class CopyTicks(Repr, IntEnum):
     """
     COPY_TICKS defines the types of ticks that can be requested using the copy_ticks_from() and copy_ticks_range() functions.
     Attributes:
         ALL (int): All ticks
```

### Comparing `aiomql-1/src/aiomql/core/meta_trader.py` & `aiomql-2.0.0/src/aiomql/core/meta_trader.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 from datetime import datetime
 import asyncio
 
-from . import Platform
+import MetaTrader5
+
 from .constants import TimeFrame, CopyTicks, OrderType
 
 
-class MetaTrader(Platform):
+class BaseMeta(type):
+    def __new__(mcs, cls_name, bases, cls_dict):
+        defaults = MetaTrader5.__dict__
+        defaults = {f'_{key}': value for key, value in defaults.items() if not key.startswith('_')}
+        cls_dict |= defaults
+        return super().__new__(mcs, cls_name, bases, cls_dict)
+
+
+class MetaTrader(metaclass=BaseMeta):
 
     async def login(self, login: int, password: str, server: str, timeout: int = 60000) -> bool:
         """"""
         return await asyncio.to_thread(self._login, login, password=password, server=server, timeout=timeout)
 
     async def initialize(self, path: str = "", login: int = 0, password: str = "", server: str = "", timeout: int = 60000, portable=False) -> bool:
         """"""
@@ -25,41 +34,41 @@
     async def last_error(self) -> tuple[int, str]:
         return await asyncio.to_thread(self._last_error)
 
     async def version(self) -> tuple[int, int, str] | None:
         """"""
         return await asyncio.to_thread(self._version)
 
-    async def account_info(self) -> Platform.platform.AccountInfo:
+    async def account_info(self) -> "AccountInfo":
         """"""
         return await asyncio.to_thread(self._account_info)
 
-    async def terminal_info(self) -> Platform.platform.TerminalInfo:
+    async def terminal_info(self) -> "TerminalInfo":
         return await asyncio.to_thread(self._terminal_info)
 
     async def symbols_total(self) -> int:
         return await asyncio.to_thread(self._symbols_total)
 
-    async def symbols_get(self, group: str = "") -> tuple[Platform.platform.SymbolInfo]:
+    async def symbols_get(self, group: str = "") -> tuple["SymbolInfo"]:
         kwargs = {'group': group} if group else {}
         return await asyncio.to_thread(self._symbols_get, **kwargs)
 
-    async def symbol_info(self, symbol: str) -> Platform.platform.SymbolInfo:
+    async def symbol_info(self, symbol: str) -> "SymbolInfo":
         return await asyncio.to_thread(self._symbol_info, symbol)
 
-    async def symbol_info_tick(self, symbol: str) -> Platform.platform.Tick:
+    async def symbol_info_tick(self, symbol: str) -> "Tick":
         return await asyncio.to_thread(self._symbol_info_tick, symbol)
 
     async def symbol_select(self, symbol: str, enable: bool) -> bool:
         return await asyncio.to_thread(self._symbol_select, symbol, enable)
 
     async def market_book_add(self, symbol: str) -> bool:
         return await asyncio.to_thread(self._market_book_add, symbol)
 
-    async def market_book_get(self, symbol: str) -> Platform.platform.BookInfo:
+    async def market_book_get(self, symbol: str) -> "BookInfo":
         return await asyncio.to_thread(self._market_book_get, symbol)
 
     async def market_book_release(self, symbol: str) -> bool:
         return await asyncio.to_thread(self._market_book_release, symbol)
 
     async def copy_rates_from(self, symbol: str, timeframe: TimeFrame, date_from: datetime | int, count: int):
         return await asyncio.to_thread(self._copy_rates_from, symbol, timeframe, date_from, count)
@@ -75,45 +84,45 @@
 
     async def copy_ticks_range(self, symbol: str, date_from: datetime | int, date_to: datetime | int, flags: CopyTicks):
         return await asyncio.to_thread(self._copy_ticks_range, symbol, date_from, date_to, flags)
 
     async def orders_total(self) -> int:
         return await asyncio.to_thread(self._orders_total)
 
-    async def orders_get(self, group: str = "", ticket: int = 0, symbol: str = "") -> tuple[Platform.platform.TradeOrder]:
+    async def orders_get(self, group: str = "", ticket: int = 0, symbol: str = "") -> tuple["TradeOrder"]:
         kwargs = {key: value for key, value in (('group', group), ('ticket', ticket), ('symbol', symbol)) if value}
         return await asyncio.to_thread(self._orders_get, **kwargs)
 
     async def order_calc_margin(self, action: OrderType, symbol: str, volume: float, price: float) -> float:
         return await asyncio.to_thread(self._order_calc_margin, action, symbol, volume, price)
 
     async def order_calc_profit(self, action: OrderType, symbol: str, volume: float, price_open: float, price_close: float) -> float:
         return await asyncio.to_thread(self._order_calc_profit, action, symbol, volume, price_open, price_close)
 
-    async def order_check(self, request: Platform.platform.TradeRequest) -> Platform.platform.OrderCheckResult:
+    async def order_check(self, request: "TradeRequest") -> "OrderCheckResult":
         return await asyncio.to_thread(self._order_check, request)
 
-    async def order_send(self, request: Platform.platform.TradeRequest) -> Platform.platform.OrderSendResult:
+    async def order_send(self, request: "TradeRequest") -> "OrderSendResult":
         return await asyncio.to_thread(self._order_send, request)
 
     async def positions_total(self) -> int:
         return await asyncio.to_thread(self._positions_total)
 
-    async def positions_get(self, group: str = "", ticket: int = 0, symbol: str = "") -> tuple[Platform.platform.TradePosition]:
+    async def positions_get(self, group: str = "", ticket: int = 0, symbol: str = "") -> tuple["TradePosition"]:
         kwargs = {key: value for key, value in (('group', group), ('ticket', ticket), ('symbol', symbol)) if value}
         return await asyncio.to_thread(self._positions_get, **kwargs)
 
     async def history_orders_total(self, date_from: datetime | int, date_to: datetime | int) -> int:
         return await asyncio.to_thread(self._history_orders_total, date_from, date_to)
 
     async def history_orders_get(self, date_from: datetime | int, date_to: datetime | int, group: str = "", ticket: int = 0, position: int = 0) -> \
-            tuple[Platform.platform.TradeOrder]:
+            tuple["TradeOrder"]:
         kwargs = {key: value for key, value in (('group', group), ('ticket', ticket), ('position', position)) if value}
         return await asyncio.to_thread(self._history_orders_get, date_from, date_to, **kwargs)
 
     async def history_deals_total(self, date_from: datetime | int, date_to: datetime | int) -> int:
         return await asyncio.to_thread(self._history_deals_total, date_from, date_to)
 
     async def history_deals_get(self, date_from: datetime | int, date_to: datetime | int, group: str = "", ticket: int = 0, position: int = 0) -> \
-            tuple[Platform.platform.TradeDeal]:
+            tuple["TradeDeal"]:
         kwargs = {key: value for key, value in (('group', group), ('ticket', ticket), ('position', position)) if value}
         return await asyncio.to_thread(self._history_deals_get, date_from, date_to, **kwargs)
```

### Comparing `aiomql-1/src/aiomql/core/models.py` & `aiomql-2.0.0/src/aiomql/core/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import MetaTrader5 as mt5
 
 from .constants import BookType, TradeAction, OrderType, OrderTime, OrderFilling, PositionType, PositionReason, DealType, DealEntry, DealReason, \
     SymbolChartMode, SymbolTradeMode, SymbolCalcMode, SymbolOptionMode, SymbolOrderGTCMode, SymbolOptionRight, SymbolTradeExecution, SymbolSwapMode, \
-    DayOfWeek, ErrorCode, AccountTradeMode, AccountStopoutMode, AccountMarginMode
+    DayOfWeek, ErrorCode, AccountTradeMode, AccountStopoutMode, AccountMarginMode, OrderReason
 
 from . import Base
 
 """
-This module hold data structures used in this library
+This module contains data structures used in this library.
+They are used as base classes to other classes having the same properties but with more methods.
 """
 
 
 class AccountInfo(Base):
     """
     Information about account.
 
     Attributes:
-        account_number: int
+        login: int
         password: str
         server: str
         trade_mode: AccountTradeMode
         balance: float
         leverage: float
         profit: float
         point: float
@@ -44,17 +45,17 @@
         currency_digits: int
         assets: float
         liabilities: float
         commission_blocked: float
         name: str
         company: str
     """
-    account_number: int
-    password: str
-    server: str
+    login: int = 0
+    password: str = ''
+    server: str = ''
     trade_mode: AccountTradeMode
     balance: float
     leverage: float
     profit: float
     point: float
     amount: float = 0
     equity: float
@@ -329,14 +330,29 @@
     exchange: str
     formula: str
     isin: str
     name: str
     page: str
     path: str
 
+    def __init__(self, **kwargs):
+        if 'name' not in kwargs:
+            raise AttributeError('Symbol Object Must be initialized with a name')
+        self.name = kwargs.pop('name')
+        super().__init__(**kwargs)
+
+    def __repr__(self):
+        return self.name
+
+    def __eq__(self, other: "SymbolInfo"):
+        return self.name == other.name
+
+    def __hash__(self):
+        return hash(self.name)
+
 
 class BookInfo(Base):
     """
     Book Info
 
     Attributes:
         type: BookType
@@ -355,59 +371,66 @@
     Trade Order
 
     Attributes:
         ticket: int
         time_setup: int
         time_setup_msc: int
         time_expiration: int
-        type: int
-        type_time: int
-        type_filling: int
+        time_done: int
+        time_done_msc: int
+        type: OrderType
+        type_time: OrderTime
+        type_filling: OrderFilling
         state: int
         magic: int
+        position_id: int
+        position_by_id: int
+        reason: OrderReason
         volume_current: float
         volume_initial: float
         price_open: float
         sl: float
         tp: float
         price_current: float
-        price_open: float
-        price_stop_limit: float
-        position_id: int
-        position_by_id: int
-        reason: str
+        price_stoplimit: float
         symbol: str
+        comment: str
+        external_id: str
     """
     ticket: int
     time_setup: int
     time_setup_msc: int
     time_expiration: int
-    type: int
-    type_time: int
-    type_filling: int
+    time_done: int
+    time_done_msc: int
+    type: OrderType
+    type_time: OrderTime
+    type_filling: OrderFilling
     state: int
     magic: int
+    position_id: int
+    position_by_id: int
+    reason: OrderReason
     volume_current: float
     volume_initial: float
     price_open: float
     sl: float
     tp: float
     price_current: float
-    price_open: float
-    price_stop_limit: float
-    position_id: int
-    position_by_id: int
-    reason: str
+    price_stoplimit: float
     symbol: str
+    comment: str
+    external_id: str
 
 
 class TradeRequest(Base):
     """
+    
     Trade Request
-
+    
     Attributes:
         action: TradeAction
         type: OrderType
         order: int
         symbol: str
         volume: float
         sl: float
```

### Comparing `aiomql-1/src/aiomql/executor.py` & `aiomql-2.0.0/src/aiomql/executor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 import asyncio
-from concurrent.futures import ThreadPoolExecutor, ProcessPoolExecutor
+from concurrent.futures import ThreadPoolExecutor
 from typing import Sequence
 
 from .strategy import Strategy
 from .symbol import Symbol
-from .config import Config
 
 
 class Executor:
     """
     Executor class for running multiple strategies and instruments concurrently.
 
     Attributes:
-        executor (ThreadPoolExecutor, ProcessPoolExecutor): Executor object.
+        executor (ThreadPoolExecutor): Executor object.
         workers (list): List of strategies.
 
     """
     def __init__(self):
-        self.config = Config()
-        self.executor = ThreadPoolExecutor if self.config.executor == 'thread' else ProcessPoolExecutor
+        self.executor = ThreadPoolExecutor
         self.workers: list[type(Strategy)] = []
 
     def add_workers(self, strategies: Sequence[type(Strategy)]):
         """
         Add multiple strategies at once
 
         Args:
@@ -30,16 +28,21 @@
 
         Returns:
         """
         self.workers.extend(strategies)
 
     def remove_workers(self, *symbols: Sequence[Symbol]):
         """
-        Remove worker if the symbol of the strategy did not initialize successfully
+        Removes any worker running on a symbol not successfully initialized.
+        
+        Args:
+            *symbols: Successfully initialized symbols
+
         Returns:
+
         """
         for strategy in self.workers:
             if strategy.symbol not in symbols:
                 self.workers.remove(strategy)
 
     def add_worker(self, strategy: type(Strategy)):
         """
@@ -60,20 +63,22 @@
             strategy (Strategy): A strategy object
 
         Returns:
 
         """
         asyncio.run(strategy.trade())
 
-    def execute(self, workers: int = 0):
+    def execute(self, workers: int | None = None):
         """
         Add workers to pool executors.
 
         Args:
-            workers: Number of workers to use in executor pool. Defaults to zero
+            workers: Number of workers to use in executor pool. Defaults to None
 
         Returns:
 
         """
         workers = workers or len(self.workers)
+        workers = max(workers, 5)
         with self.executor(max_workers=workers) as executor:
             executor.map(self.run, self.workers)
+
```

### Comparing `aiomql-1/src/aiomql/history.py` & `aiomql-2.0.0/src/aiomql/history.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 import asyncio
 from datetime import datetime
+from logging import getLogger
 
-from .config import Config
+from .core.config import Config
 
 from .core.meta_trader import MetaTrader
 from .core.models import TradeDeal, TradeOrder
-from .terminal import terminal
+
+logger = getLogger()
 
 
 class History:
     """
     The history class handles trade deals and trade orders in the trading history.
 
-    Args:
-        mt5 (MetaTrader): The Meta trader object for connecting to the terminal. Default Keyword Argument.
-
+    Args: date_from (datetime, float): Date the orders are requested from. Set by the 'datetime' object or as a
+    number of seconds elapsed since 1970.01.01. Defaults to the current time in "utc"
 
-        date_from (datetime, float): Date the orders are requested from. Set by the 'datetime' object or as a number of seconds elapsed since
-            1970.01.01. Defaults to the current time in "utc"
 
+    date_to (datetime, float): Date up to which the orders are requested. Set by the 'datetime' object or as a number of
+    seconds elapsed since 1970.01.01. Defaults to the current time in "utc"
 
-        date_to (datetime, float): Date, up to which the orders are requested. Set by the 'datetime' object or as a number of
-            seconds elapsed since 1970.01.01. Defaults to the current time in "utc"
 
-
-        group (str): Filter for selecting history by symbols.
+    group (str): Filter for selecting history by symbols.
 
 
-        ticket (int): Filter for selecting history by ticket number
+    ticket (int): Filter for selecting history by ticket number
 
 
-        position (int): Filter for selecting history deals by position
+    position (int): Filter for selecting history deals by position
 
     Attributes:
         deals (Iterable[TradeDeal]): Iterable of trade deals
         orders (Iterable[TradeOrder]): Iterable of trade orders
         total_deals: Total number of deals
         total_orders (int): Total number orders
         group (str): Filter for selecting history by symbols.
@@ -42,29 +40,31 @@
         position (int): Filter for selecting history deals by position
         initialized (bool): check if initial request has been sent to the terminal to get history.
     """
     deals: list[TradeDeal] = []
     orders: list[TradeOrder] = []
     total_deals: int = 0
     total_orders: int = 0
+    mt5: MetaTrader = MetaTrader()
+    config: Config = Config()
+    initialized = False
 
-    def __init__(self, *, mt5=MetaTrader(), date_from: datetime | float = datetime.utcnow(), date_to: datetime | float = datetime.utcnow(),
+    def __init__(self, *, date_from: datetime | float = 0, date_to: datetime | float = 0,
                  group: str = "", ticket: int = 0, position: int = 0):
-        self.config = Config()
-        self.mt5 = mt5
-        self.date_from = date_from
-        self.date_to = date_to
+        now = datetime.utcnow()
+        self.date_from = date_from or now
+        self.date_to = date_to or now
         self.group = group
         self.ticket = ticket
         self.position = position
-        self.initialized = False
 
     async def init(self, deals=True, orders=True) -> bool:
         """
         Get history deals and orders
+
         Keyword Args:
             deals (bool): If true get history deals during initial request to terminal
             orders (bool): If true get history orders during initial request to terminal
 
         Returns:
             bool: True if all requests were successful else False
 
@@ -81,17 +81,21 @@
         Get trade deals
         Returns:
             list[TradeDeal]: Iterable of trade deals
 
         """
         deals = await self.mt5.history_deals_get(date_from=self.date_from, date_to=self.date_to, group=self.group, ticket=self.ticket,
                                                  position=self.position)
+        if deals is not None:
+            self.deals = [TradeDeal(**deal._asdict()) for deal in deals] if deals else []
+            self.total_deals = len(self.deals)
+            return self.deals
 
-        self.deals = [TradeDeal(**deal._asdict()) for deal in deals] if deals else []
-        self.total_deals = len(self.deals)
+        err = await self.mt5.last_error()
+        logger.warning(err)
         return self.deals
 
     async def deals_total(self) -> int:
         """
         Get total number of deals
         Returns (int): Number of Deals
         """
@@ -101,17 +105,22 @@
     async def get_orders(self) -> list[TradeOrder]:
         """
         Get trade orders
         Returns:
             list[TradeOrder]): Iterable of trade orders
         """
 
-        orders = await self.mt5.history_orders_get(date_from=self.date_from, date_to=self.date_to, group=self.group, ticket=self.ticket,
-                                                   position=self.position)
-        self.orders = [TradeOrder(**order._asdict()) for order in orders] if orders else []
+        orders = await self.mt5.history_orders_get(date_from=self.date_from, date_to=self.date_to, group=self.group,
+                                                   ticket=self.ticket, position=self.position)
+        if orders is None:
+            err = await self.mt5.last_error()
+            logger.warning(err)
+            return self.orders
+
+        self.orders = [TradeOrder(**order._asdict()) for order in orders]
         self.total_orders = len(self.orders)
         return self.orders
 
     async def orders_total(self) -> int:
         """
         Get total number of orders
         Returns (int): Number of orders
```

### Comparing `aiomql-1/src/aiomql/lib/traders/simple_deal_trader.py` & `aiomql-2.0.0/src/aiomql/lib/traders/simple_deal_trader.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,67 +1,65 @@
 import logging
+from datetime import datetime
 
 from ...utils import dict_to_string
-from ...result import TradeResult
-from ...symbol import Symbol
 from ...trader import Trader
 from ...core.constants import OrderType
 
-from ..symbols import ForexSymbol, SyntheticSymbol
+from .trade_result import TradeResult
 
 logger = logging.getLogger()
 
 
 class DealTrader(Trader):
 
-    def __init__(self, *, symbol: ForexSymbol | SyntheticSymbol):
-        super().__init__(symbol=symbol)
-
     async def create_order(self, order: OrderType, points: float):
         """
-        Using the amount of points i.e pips/10 determine the volume, stop_loss and take_profit.
-        Use equity and risk value on account to determine amount
+        Using the number of target pips determines the lot size
         Args:
             order (OrderType): Type of order
-            points (float): Number of points
+            points (float): Number of pips
 
         Returns:
 
         """
         await self.account.refresh()
-        amount = self.account.equity * self.account.risk
-        sl, tp, volume = await self.symbol.get_sl_tp_volume(amount=amount, risk_to_reward=self.account.risk_to_reward, points=points)
+        amount = self.account.margin_free * self.account.risk
+        sl, tp, volume = await self.symbol.get_sl_tp_volume(amount=amount, risk_to_reward=self.account.risk_to_reward,
+                                                            points=points)
         self.order.volume = volume
         self.order.type = order
         await self.set_order_limits(sl, tp)
 
     async def set_order_limits(self, sl, tp):
         tick = await self.symbol.info_tick()
         if self.order.type == OrderType.BUY:
             self.order.sl, self.order.tp = tick.ask - sl, tick.ask + tp
             self.order.price = tick.ask
         else:
             self.order.sl, self.order.tp = tick.bid + sl, tick.bid - tp
             self.order.price = tick.bid
 
-    async def place_trade(self, order: OrderType, points: float, params: dict = None):
+    async def place_trade(self, order: OrderType, points: float, params):
         try:
-            params = params or {}
             await self.create_order(order=order, points=points)
-
             check = await self.order.check()
             if check.retcode != 0:
-                logger.warning(f"Comment: {check.comment}\tParameters: {dict_to_string(params)}\tsymbol: {self.order.symbol}")
+                logger.warning(f"Symbol: {self.order.symbol}\nResult:\n{dict_to_string(check.get_dict(include={'comment', 'retcode'}), multi=True)}")
                 return
 
             result = await self.order.send()
             if result.retcode != 10009:
-                logger.warning(f"Comment: {result.comment}\tParameters: {dict_to_string(params)}\tsymbol: {self.order.symbol}")
+                logger.warning(f"Symbol: {self.order.symbol}\nResult:\n{dict_to_string(result.get_dict(include={'comment', 'retcode'}), multi=True)}")
                 return
 
-            logger.info(f"{result.comment}\tparameters: {dict_to_string(params)}\tsymbol: {self.order.symbol}")
+            params['date'] = (date := datetime.utcnow())
+            params['time'] = date.timestamp()
+            logger.info(f"Symbol: {self.order.symbol}\nOrder: {dict_to_string(result.dict, multi=True)}\n")
             self.order.set_attributes(**result.get_dict(include={'price', 'volume'}))
             result.profit = await self.order.calc_profit()
-            TradeResult(parameters=params, request=self.order, result=result)
+            await TradeResult(result=result, parameters=params).save()
+            # await results.save()
             return
+
         except Exception as err:
-            logger.error(f"{err}\tparameters: {dict_to_string(params)}\tsymbol: {self.order.symbol}")
+            logger.error(f"{err}. Symbol: {self.order.symbol}\n {self.__class__.__name__}place trade")
```

### Comparing `aiomql-1/src/aiomql/order.py` & `aiomql-2.0.0/src/aiomql/order.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-from .core.meta_trader import MetaTrader
 from .core.models import TradeRequest, OrderSendResult, OrderCheckResult, TradeOrder
 from .core.constants import TradeAction, OrderTime, OrderFilling
 
 
 class Order(TradeRequest):
     """
     Trade order related functions and properties. Subclass of TradeRequest.
 
     Keyword Args:
-        mt5 (MetaTrader): The Meta trader object for connecting to the terminal. Default Keyword Argument
         kwargs: Arguments for initializing the order object
 
     Attributes:
         action (TradeAction): Trading operation type from TradeAction Enum
 
         type_time (OrderTime):  Order type by expiration from OrderTime
 
@@ -23,18 +21,14 @@
     """
     action: TradeAction = TradeAction.DEAL
     type_time: OrderTime = OrderTime.SPECIFIED_DAY
     type_filling: OrderFilling = OrderFilling.FOK
     total: int = 0
     orders: list[TradeOrder]
 
-    def __init__(self, mt5=MetaTrader(), **kwargs):
-        self.mt5 = mt5
-        super().__init__(**kwargs)
-
     async def orders_total(self):
         """
         Get the number of active orders. Update the total property
 
         Returns:
             int: Number of active orders
         """
```

### Comparing `aiomql-1/src/aiomql/positions.py` & `aiomql-2.0.0/src/aiomql/positions.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 
 class Positions:
     """
     Hold open positions related properties and objects
 
     Keyword Args:
-        mt5 (MetaTrader): The Meta trader object for connecting to the terminal. Default Keyword Argument
         symbol (str): Financial instrument name
         group (str): The filter for arranging a group of necessary symbols. Optional named parameter. If the group is specified, the function returns
                      only positions meeting a specified criteria for a symbol name.
         ticket (int): Position ticket
 
     Attributes:
         symbol (str): Financial instrument name
@@ -25,49 +24,52 @@
 
         ticket (int): Position ticket
 
         positions (list[TradePosition]): A list of trade positions
 
         total_positions (int):
     """
-    def __init__(self, *, symbol: str = "", group: str = "", ticket: int = 0, mt5=MetaTrader()):
-        self.mt5 = mt5
+    mt5: MetaTrader = MetaTrader()
+    total_positions: int = 0
+    positions: list[TradePosition] = []
+    
+    def __init__(self, *, symbol: str = "", group: str = "", ticket: int = 0):
         self.symbol = symbol
         self.group = group
         self.ticket = ticket
-        self.total_positions: int = 0
-        self.positions: list[TradePosition] = []
 
     async def positions_total(self) -> int:
         """
         Get open positions with the ability to filter by symbol or ticket.
+        
         Returns (int): Return integer value
 
         """
         self.total_positions = await self.mt5.positions_total()
         return self.total_positions
 
     async def positions_get(self):
         """
         Get open positions with the ability to filter by symbol or ticket.
+        
         Returns:
             list[TradePosition]: A list of open trade positions
 
         """
         positions = await self.mt5.positions_get(group=self.group, symbol=self.symbol, ticket=self.ticket)
         self.positions = [TradePosition(**pos._asdict()) for pos in positions]
         return self.positions
 
     async def close_all(self) -> int:
         """
         Close all open positions
-        Returns (int): Return number of open positions
-
+        
+        Returns (int): Return number of positions closed.
         """
-        orders = [Order(mt5=self.mt5, action=TradeAction.DEAL, price=pos.price_current, position=pos.ticket,
+        orders = [Order(action=TradeAction.DEAL, price=pos.price_current, position=pos.ticket,
                         type=OrderType(pos.type).opposite,
                         **pos.get_dict(include={'symbol', 'volume'})) for pos in (await self.positions_get())]
 
         results = await asyncio.gather(*[order.send() for order in orders])
         amount_closed = len([res for res in results if res.retcode == 10009])
         await self.positions_total()
         return amount_closed
```

### Comparing `aiomql-1/src/aiomql/records.py` & `aiomql-2.0.0/src/aiomql/records.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,106 +1,91 @@
 import asyncio
 from datetime import datetime
-from typing import Iterable
 from pathlib import Path
 import csv
 
 from .history import History
-from .config import Config
+from .core.config import Config
 
 
 class Records:
     """
     This utility class read trade records from csv files, and update them based on their closing positions
 
     Keyword Args:
         records_dir (Path): Path to directory containing record of placed trades.
 
     Attributes:
         config: Config object
 
         records_dir(Path): Path to directory containing record of placed trades, If not given takes the default from the config
     """
-
-    def __init__(self, records_dir: Path = None):
-        self.config = Config()
+    config: Config = Config()
+    
+    def __init__(self, records_dir: Path = ''):
         self.records_dir = records_dir or self.config.records_dir
 
     async def get_records(self):
         """
         get trade records from records_dir folder
         Returns:
 
         """
         for file in self.records_dir.iterdir():
             if file.is_file() and file.name.endswith('.csv'):
                 yield file
 
-    async def read_record(self, file: Path):
+    async def read_update(self, file: Path):
         """
         Read and update trade records
 
         Args:
             file: Trade record file
 
         Returns:
 
         """
-        with open(file, newline='') as fr:
-            reader = csv.DictReader(fr)
-            rows = (row for row in reader)
-            rows = await self.update_record(rows)
-            fr.close()
-            if not all(rows):
-                return
-            fw = open(file, newline='', mode='w')
-            writer = csv.DictWriter(fw, fieldnames=list(rows[0].keys()))
-            writer.writeheader()
-            writer.writerows(rows)
-            fw.close()
+        fr = open(file, mode='r', newline='')
+        reader = csv.DictReader(fr)
+        rows = [row for row in reader]
+        rows = await self.update_rows(rows)
+        fr.close()
+        fw = open(file, mode='w', newline='')
+        writer = csv.DictWriter(fw, fieldnames=reader.fieldnames)
+        writer.writeheader()
+        writer.writerows(rows)
+        fw.close()
 
-    async def update_record(self, rows: Iterable) -> Iterable[dict]:
+    async def update_rows(self, rows: list[dict]) -> list[dict]:
         """
-        Get update of trades in the record file.
+        Update the trade records with historical records
         Args:
-            rows: rows of recorded trade in a particular file
+            rows: A list of dictionaries from the dictionary writer object of the csv file.
 
-        Returns: return rows of updated trades as an iterable of dicts
+        Returns:
 
         """
-        rows = {row['deal']: row for row in sorted((row for row in rows), key=lambda row: float(row['time']))}
-        open_rows = [(key, value) for key, value in rows.items() if value.get('closed').title() == "False"]
-        if len(open_rows) == 0:
-            return [{}]
-
-        start, end = datetime.fromtimestamp(float(open_rows[0][1]['time'])).replace(hour=0, minute=0, second=0), datetime.now()\
-            .replace(hour=23, minute=59, second=59)
-
-        history = History(date_from=start, date_to=end)
-        await history.init(orders=False)
-        deals = {str(deal.position_id): deal.profit for deal in history.deals}
-
-        for el in open_rows:
-            row = el[1]
-            if row['order'] not in deals:
-                continue
-            profit = float(row['profit'])
-            actual_profit = deals[row['order']]
-            win = actual_profit / profit > self.config.win_percentage
-            row.update(actual_profit=actual_profit, closed=True, win=win)
-        return list(rows.values())
+        start = float(min(rows, key=lambda r: r['time'])['time'])
+        end = datetime.utcnow().timestamp()
+        his = History(date_from=start, date_to=end)
+        await his.init(orders=False)
+        deals = {str(deal.position_id): deal.profit for deal in his.deals}
+        for row in rows:
+            if (deal := row['order']) in deals:
+                profit = deals[deal]
+                row.update(actual_profit=profit, win=profit > 0)
+        return rows
 
-    async def update_trade_records(self):
+    async def update_records(self):
         """
         Update trade records
         Returns:
         """
-        records = [self.read_record(record) async for record in self.get_records()]
+        records = [self.read_update(record) async for record in self.get_records()]
         await asyncio.gather(*records)
 
-    async def update_trade_record(self, file: Path | str):
+    async def update_record(self, file: Path | str):
         """
-
         Returns:
 
         """
-        await self.read_record(file)
+        await self.read_update(file)
```

### Comparing `aiomql-1/src/aiomql/result.py` & `aiomql-2.0.0/src/aiomql/result.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,77 +1,56 @@
-import datetime
-from functools import cache
-import csv
 import asyncio
+from abc import ABC, abstractmethod
+import csv
 from logging import getLogger
 
-from .core.models import OrderSendResult
-from .order import Order
-from .config import Config
+from .core.config import Config
 
 logger = getLogger()
 
 
-class TradeResult:
+class Result(ABC):
     """
-    Save result of trades made by a strategy to a csv file.
-    Args:
+    An abstract base Class for handling trade results and strategy parameters for record keeping and reference purpose
         result (OrderSendResult): OrderSendResult object of an executed trade
         request (Order | dict): Order object or a dict of trade order request properties
         parameters (dict): The parameters of the strategy placing the trade
         time (float): Timestamp of when order was placed
         name: Name  of strategy or any desired name for the result csv file
     Attributes:
         config: The configuration object
-        result (dict): Trade result as a dict
-        request (dict): Trade order as a dict
-        parameters (dict): The parameters of the strategy placing the trade
-        time: Timestamp
-        time (float): Timestamp of when order was placed
-        name: Name  of strategy or any desired name for the result csv file
+        name: Any desired name for the result csv file
 
     Notes:
         To enable saving trades as csv file. Make sure that config.record_trades is True
     """
-    def __init__(self, *, result: OrderSendResult | dict, request: Order | dict, parameters: dict, time: float = datetime.datetime.utcnow().timestamp(),
-                 name: str = ""):
-        self.config = Config()
-        self.result: dict = result.dict if not isinstance(request, dict) else request
-        self.request: dict = request.get_dict(include={'action', 'symbol', 'sl', 'tp', 'type'}) if not isinstance(request, dict) else request
-        self.parameters = parameters
-        self.time = time
-        self.name = name or self.parameters.get('name', datetime.datetime.today().strftime('%a %M %b %Y'))
-
-        if self.config.record_trades:
-            loop = asyncio.get_running_loop()
-            asyncio.run_coroutine_threadsafe(self.to_csv(), loop)
+    config = Config()
+
+    def __init__(self, name: str):
+        self.name = name
 
     @property
-    @cache
+    @abstractmethod
     def data(self) -> dict:
         """
-        A dict representing data to be saved in the csv file. It is a combination of the strategy parameters, the order result properties, the trade
-        request properties, actual profit made from trade, timestamp of when trade was placed, closed to indicate if trade has been closed and win to
-        indicate if trade was successful or not
+        A dict representing data to be saved in the csv file.
         Returns (dict): A dict of data to be saved
         """
-        data = self.parameters | self.result | self.request | {'actual_profit': 0, 'time': self.time, 'closed': False, 'win': False}
-        return data
 
     async def to_csv(self):
         """
-        Saves to csv file format
-        Returns:
-
+        Record trade results and associated parameters as a csv file
         """
         try:
             file = self.config.records_dir / f"{self.name}.csv"
             exists = file.exists()
-            self.data.pop('name')
-            self.data['date'] = datetime.datetime.utcnow().strftime("%d/%m/%Y %H:%M")
             with open(file, 'a', newline='') as fh:
                 writer = csv.DictWriter(fh, fieldnames=sorted(list(self.data.keys())), extrasaction='ignore', restval=None)
                 if not exists:
                     writer.writeheader()
                 writer.writerow(self.data)
         except Exception as err:
-            logger.error(err)
+            logger.error(f'Error: {err}. Unable to save trade results')
+
+    async def save(self):
+        loop = asyncio.get_running_loop()
+        asyncio.run_coroutine_threadsafe(self.to_csv(), loop)
```

### Comparing `aiomql-1/src/aiomql/strategy.py` & `aiomql-2.0.0/src/aiomql/strategy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,50 @@
 import asyncio
 import time
-from dataclasses import dataclass
-from typing import Literal, Type
+from typing import Type, TypeVar
 from abc import ABC, abstractmethod
 
 import pandas_ta as ta
-from pandas import DataFrame
 
-from .core.constants import TimeFrame, OrderType
+from .core.constants import TimeFrame
 from .candle import Candles, Candle
-from .symbol import Symbol
+from .symbol import Symbol as _Symbol
+from .account import Account
 
 
-@dataclass
-class Entry:
-    """
-    A helper class for capturing entry positions.
-
-    Attributes:
-        time (float): Time of the bar
-
-        trend (str): The trend of the chart. Can be either of "notrend", "uptrend", "downtrend".
-
-        new (bool): Shows if an entry position has been seen before.
-
-        type (OrderType): OrderType for placing trade order
-
-        points (float): points to trade.
-    """
-    time: float = 0
-    trend: Literal["notrend", "uptrend", "downtrend"] = "notrend"
-    current: float = 0
-    new: bool = True
-    type: OrderType | None = None
-    points: float = 0
+Symbol = TypeVar('Symbol', bound=_Symbol)
 
 
 class Strategy(ABC):
     """
     The base class for creating strategies.
 
     Keyword Args:
         symbol (Symbol): The Financial Instrument as a Symbol Object
-        **kwargs: Optional Keyword Arguments
+
+        params (dict): Configurable parameters for running the strategy
 
     Attributes:
         Candle (Type[Candle]): Can be a subclass of the Candle class specific to the strategy and analysis carried out on it.
 
         Candles (Type[Candles]): Candles class for the strategy can be the same or a subclass of the "candle.Candles" class.
 
-        name (str): A name for the strategy. You can initialize a new name for the strategy that will replace the one defined as class parameter
+        name (str): A name for the strategy.
+
+        symbol (Symbol): The Financial Instrument as a Symbol Object
     """
     Candle: Type[Candle] = Candle
     Candles: Type[Candles] = Candles
     name:  str = ""
+    account = Account()
 
-    def __init__(self, *, symbol: type(Symbol), **kwargs):
+    def __init__(self, *, symbol: Symbol, params: dict = None):
         self.symbol = symbol
-        self.name = kwargs.get('name') or self.name
+        self.parameters = params or {}
+        self.parameters['symbol'] = symbol.name
 
     def __repr__(self):
         return f"{self.name}({self.symbol!r})"
 
     async def get_ema(self, *, time_frame: TimeFrame, period: int, count: int = 500) -> type(Candles):
         """
         Helper method that gets the ema of the bars.
@@ -71,30 +54,32 @@
 
             period (int): Period of the ema
 
             count (int): Number of objects to be returned
 
         Returns: A Candles Object
         """
-        data: DataFrame = await self.symbol.copy_rates_from_pos(timeframe=time_frame, count=count)
-        await asyncio.to_thread(data.ta.ema, length=period, append=True)
-        data.rename(columns={f"EMA_{period}": 'ema'}, inplace=True)
-        return self.Candles(data=data, candle=self.Candle)
+        rates = await self.symbol.copy_rates_from_pos(timeframe=time_frame, count=count)
+        await asyncio.to_thread(rates.data.ta.ema, length=period, append=True)
+        rates.data.rename(columns={f"EMA_{period}": 'ema'}, inplace=True)
+        return self.Candles(data=rates.data)
 
     @staticmethod
     async def sleep(secs: float):
         """
         Sleep for the needed amount of seconds between requests to the terminal
         Args:
             secs (float): The time period of the requests, eg. when trading on the 5 minute time frame the value will be 300 secs
 
         Returns: None.
 
         """
-        await asyncio.sleep(secs - (time.time() % secs) + 1)
+        mod = time.time() % secs
+        secs = secs - mod if mod != 0 else mod
+        await asyncio.sleep(secs)
 
     @abstractmethod
     async def trade(self):
         """
         Place trades using this method
         Returns:
```

### Comparing `aiomql-1/src/aiomql/trader.py` & `aiomql-2.0.0/src/aiomql/trader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 from abc import ABC, abstractmethod
+from typing import TypeVar
 
-from .account import Account, account
 from .order import Order
-from .result import TradeResult
-from .symbol import Symbol
+from .symbol import Symbol as _Symbol
+from .account import Account
+
+Symbol = TypeVar('Symbol', bound=_Symbol)
 
 
 class Trader(ABC):
     """
     Helper class for creating a Trader object. Handles the initializing of an order and the placing of trades
     Args:
         symbol (Symbol): Financial instrument
 
-        account (Account): Trading account
-
     Attributes:
 
-        symbol (Symbol): Financial instrument class Symbol class or a subclass of it.
+        symbol (Symbol): Financial instrument class Symbol class or any subclass of it.
 
         account (Account): Trading account
 
         order (Order): Trade order
     """
-    def __init__(self, *, symbol: type(Symbol), account: Account = account):
-        self.account = account
+
+    def __init__(self, *, symbol: Symbol):
         self.symbol = symbol
-        self.order = Order(symbol=symbol.name)
+        self.order = Order(symbol=symbol)
+        self.account = Account()
 
+    @abstractmethod
     async def create_order(self, *args, **kwargs):
         """
         Create an order, and update the order object initialized
         Args:
             *args:
             **kwargs:
 
         Returns:
 
         """
 
     @abstractmethod
-    async def place_trade(self, *args, **kwargs) -> TradeResult | None:
+    async def place_trade(self, *args, **kwargs):
         """
         Send trade to server
         Args:
             *args:
             **kwargs:
-
-        Returns: TradeResult if successful
-
         """
```

### Comparing `aiomql-1/src/aiomql.egg-info/SOURCES.txt` & `aiomql-2.0.0/src/aiomql.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -2,18 +2,16 @@
 README.md
 pyproject.toml
 setup.py
 src/aiomql/__init__.py
 src/aiomql/account.py
 src/aiomql/bot_builder.py
 src/aiomql/candle.py
-src/aiomql/config.py
 src/aiomql/executor.py
 src/aiomql/history.py
-src/aiomql/market.py
 src/aiomql/order.py
 src/aiomql/positions.py
 src/aiomql/records.py
 src/aiomql/result.py
 src/aiomql/strategy.py
 src/aiomql/symbol.py
 src/aiomql/terminal.py
@@ -22,20 +20,20 @@
 src/aiomql/utils.py
 src/aiomql.egg-info/PKG-INFO
 src/aiomql.egg-info/SOURCES.txt
 src/aiomql.egg-info/dependency_links.txt
 src/aiomql.egg-info/requires.txt
 src/aiomql.egg-info/top_level.txt
 src/aiomql/core/__init__.py
+src/aiomql/core/base.py
+src/aiomql/core/config.py
 src/aiomql/core/constants.py
 src/aiomql/core/meta_trader.py
 src/aiomql/core/models.py
-src/aiomql/lib/markets/forex_market.py
-src/aiomql/lib/markets/synthetic_market.py
+src/aiomql/lib/__init__.py
+src/aiomql/lib/strategies/__init__.py
 src/aiomql/lib/strategies/finger_trap.py
+src/aiomql/lib/symbols/__init__.py
 src/aiomql/lib/symbols/forex_symbol.py
 src/aiomql/lib/symbols/synthetic_symbol.py
 src/aiomql/lib/traders/simple_deal_trader.py
-tests/test_config.py
-tests/test_constants.py
-tests/test_symbol.py
-tests/test_terminal.py
+src/aiomql/lib/traders/trade_result.py
```

