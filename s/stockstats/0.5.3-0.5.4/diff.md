# Comparing `tmp/stockstats-0.5.3.tar.gz` & `tmp/stockstats-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stockstats-0.5.3.tar", last modified: Mon Jun 12 15:56:09 2023, max compression
+gzip compressed data, was "stockstats-0.5.4.tar", last modified: Wed Jun 14 15:41:15 2023, max compression
```

## Comparing `stockstats-0.5.3.tar` & `stockstats-0.5.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:56:09.599066 stockstats-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-12 15:55:43.000000 stockstats-0.5.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-12 15:55:43.000000 stockstats-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    25456 2023-06-12 15:56:09.599066 stockstats-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24525 2023-06-12 15:55:43.000000 stockstats-0.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-12 15:55:43.000000 stockstats-0.5.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-12 15:56:09.599066 stockstats-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-06-12 15:55:43.000000 stockstats-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:56:09.599066 stockstats-0.5.3/stockstats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25456 2023-06-12 15:56:09.000000 stockstats-0.5.3/stockstats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-12 15:56:09.000000 stockstats-0.5.3/stockstats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:56:09.000000 stockstats-0.5.3/stockstats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-12 15:56:09.000000 stockstats-0.5.3/stockstats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 15:56:09.000000 stockstats-0.5.3/stockstats.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    48422 2023-06-12 15:55:43.000000 stockstats-0.5.3/stockstats.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 15:55:43.000000 stockstats-0.5.3/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:41:15.825227 stockstats-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-14 15:41:05.000000 stockstats-0.5.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-14 15:41:05.000000 stockstats-0.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    26076 2023-06-14 15:41:15.825227 stockstats-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25144 2023-06-14 15:41:05.000000 stockstats-0.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-14 15:41:05.000000 stockstats-0.5.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-14 15:41:15.825227 stockstats-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-06-14 15:41:05.000000 stockstats-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:41:15.825227 stockstats-0.5.4/stockstats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26076 2023-06-14 15:41:15.000000 stockstats-0.5.4/stockstats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-14 15:41:15.000000 stockstats-0.5.4/stockstats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 15:41:15.000000 stockstats-0.5.4/stockstats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-14 15:41:15.000000 stockstats-0.5.4/stockstats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-14 15:41:15.000000 stockstats-0.5.4/stockstats.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    49577 2023-06-14 15:41:05.000000 stockstats-0.5.4/stockstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-14 15:41:05.000000 stockstats-0.5.4/test-requirements.txt
```

### Comparing `stockstats-0.5.3/LICENSE.txt` & `stockstats-0.5.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stockstats-0.5.3/PKG-INFO` & `stockstats-0.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: stockstats
-Version: 0.5.3
+Version: 0.5.4
 Summary: DataFrame with inline stock statistics support.
 Home-page: https://github.com/jealous/stockstats
 Author: Cedric Zhuang
 Author-email: jealous@163.com
 License: BSD
 Keywords: stock statistics indicator
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities
@@ -25,15 +25,15 @@
 
 # Stock Statistics/Indicators Calculation Helper
 
 [![build & test](https://github.com/jealous/stockstats/actions/workflows/build-test.yml/badge.svg)](https://github.com/jealous/stockstats/actions/workflows/build-test.yml)
 [![codecov](https://codecov.io/gh/jealous/stockstats/branch/master/graph/badge.svg?token=IFMD1pVJ7T)](https://codecov.io/gh/jealous/stockstats)
 [![pypi](https://img.shields.io/pypi/v/stockstats.svg)](https://pypi.python.org/pypi/stockstats)
 
-VERSION: 0.5.3
+VERSION: 0.5.4
 
 ## Introduction
 
 Supply a wrapper ``StockDataFrame`` for ``pandas.DataFrame`` with inline stock
 statistics/indicators support.
 
 Supported statistics/indicators are:
@@ -77,14 +77,15 @@
 * KAMA: Kaufman's Adaptive Moving Average
 * PPO: Percentage Price Oscillator
 * StochRSI: Stochastic RSI
 * WT: LazyBear's Wave Trend
 * Supertrend: with the Upper Band and Lower Band
 * Aroon: Aroon Oscillator
 * Z: Z-Score
+* AO: Awesome Oscillator
 
 ## Installation
 
 ```pip install stockstats```
 
 ## Compatibility
 
@@ -714,14 +715,30 @@
 * `x` = the value being evaluated
 * `μ` = the mean
 * `σ` = the standard deviation
 
 Examples:
 * `df['close_75_z']` returns the Z-Score of close price with a window of 75
 
+#### [Awesome Oscillator](https://www.ifcm.co.uk/ntx-indicators/awesome-oscillator)
+
+The AO indicator is a good indicator for measuring the market dynamics,
+it reflects specific changes in the driving force of the market, which
+helps to identify the strength of the trend, including the points of
+its formation and reversal.
+
+Awesome Oscillator Formula
+
+* MEDIAN PRICE = (HIGH+LOW)/2
+* AO = SMA(MEDIAN PRICE, 5)-SMA(MEDIAN PRICE, 34)
+
+Examples:
+* `df['ao']` returns the Awesome Oscillator with default windows (5, 34)
+* `df['ao_3,10']` returns the Awesome Oscillator with a window of 3 and 10
+
 ## Issues
 
 We use [Github Issues](https://github.com/jealous/stockstats/issues) to track
 the issues or bugs.
 
 ## Others
```

### Comparing `stockstats-0.5.3/README.md` & `stockstats-0.5.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Stock Statistics/Indicators Calculation Helper
 
 [![build & test](https://github.com/jealous/stockstats/actions/workflows/build-test.yml/badge.svg)](https://github.com/jealous/stockstats/actions/workflows/build-test.yml)
 [![codecov](https://codecov.io/gh/jealous/stockstats/branch/master/graph/badge.svg?token=IFMD1pVJ7T)](https://codecov.io/gh/jealous/stockstats)
 [![pypi](https://img.shields.io/pypi/v/stockstats.svg)](https://pypi.python.org/pypi/stockstats)
 
-VERSION: 0.5.3
+VERSION: 0.5.4
 
 ## Introduction
 
 Supply a wrapper ``StockDataFrame`` for ``pandas.DataFrame`` with inline stock
 statistics/indicators support.
 
 Supported statistics/indicators are:
@@ -52,14 +52,15 @@
 * KAMA: Kaufman's Adaptive Moving Average
 * PPO: Percentage Price Oscillator
 * StochRSI: Stochastic RSI
 * WT: LazyBear's Wave Trend
 * Supertrend: with the Upper Band and Lower Band
 * Aroon: Aroon Oscillator
 * Z: Z-Score
+* AO: Awesome Oscillator
 
 ## Installation
 
 ```pip install stockstats```
 
 ## Compatibility
 
@@ -689,14 +690,30 @@
 * `x` = the value being evaluated
 * `μ` = the mean
 * `σ` = the standard deviation
 
 Examples:
 * `df['close_75_z']` returns the Z-Score of close price with a window of 75
 
+#### [Awesome Oscillator](https://www.ifcm.co.uk/ntx-indicators/awesome-oscillator)
+
+The AO indicator is a good indicator for measuring the market dynamics,
+it reflects specific changes in the driving force of the market, which
+helps to identify the strength of the trend, including the points of
+its formation and reversal.
+
+Awesome Oscillator Formula
+
+* MEDIAN PRICE = (HIGH+LOW)/2
+* AO = SMA(MEDIAN PRICE, 5)-SMA(MEDIAN PRICE, 34)
+
+Examples:
+* `df['ao']` returns the Awesome Oscillator with default windows (5, 34)
+* `df['ao_3,10']` returns the Awesome Oscillator with a window of 3 and 10
+
 ## Issues
 
 We use [Github Issues](https://github.com/jealous/stockstats/issues) to track
 the issues or bugs.
 
 ## Others
```

### Comparing `stockstats-0.5.3/setup.py` & `stockstats-0.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,16 +76,16 @@
     url="https://github.com/jealous/stockstats",
     py_modules=['stockstats'],
     platforms=['any'],
     long_description=get_long_description(),
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 2.7",
-        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Natural Language :: English",
         "Intended Audience :: Developers",
         "Intended Audience :: Financial and Insurance Industry",
         "Operating System :: OS Independent",
         "Development Status :: 4 - Beta",
         "Topic :: Utilities",
```

### Comparing `stockstats-0.5.3/stockstats.egg-info/PKG-INFO` & `stockstats-0.5.4/stockstats.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: stockstats
-Version: 0.5.3
+Version: 0.5.4
 Summary: DataFrame with inline stock statistics support.
 Home-page: https://github.com/jealous/stockstats
 Author: Cedric Zhuang
 Author-email: jealous@163.com
 License: BSD
 Keywords: stock statistics indicator
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities
@@ -25,15 +25,15 @@
 
 # Stock Statistics/Indicators Calculation Helper
 
 [![build & test](https://github.com/jealous/stockstats/actions/workflows/build-test.yml/badge.svg)](https://github.com/jealous/stockstats/actions/workflows/build-test.yml)
 [![codecov](https://codecov.io/gh/jealous/stockstats/branch/master/graph/badge.svg?token=IFMD1pVJ7T)](https://codecov.io/gh/jealous/stockstats)
 [![pypi](https://img.shields.io/pypi/v/stockstats.svg)](https://pypi.python.org/pypi/stockstats)
 
-VERSION: 0.5.3
+VERSION: 0.5.4
 
 ## Introduction
 
 Supply a wrapper ``StockDataFrame`` for ``pandas.DataFrame`` with inline stock
 statistics/indicators support.
 
 Supported statistics/indicators are:
@@ -77,14 +77,15 @@
 * KAMA: Kaufman's Adaptive Moving Average
 * PPO: Percentage Price Oscillator
 * StochRSI: Stochastic RSI
 * WT: LazyBear's Wave Trend
 * Supertrend: with the Upper Band and Lower Band
 * Aroon: Aroon Oscillator
 * Z: Z-Score
+* AO: Awesome Oscillator
 
 ## Installation
 
 ```pip install stockstats```
 
 ## Compatibility
 
@@ -714,14 +715,30 @@
 * `x` = the value being evaluated
 * `μ` = the mean
 * `σ` = the standard deviation
 
 Examples:
 * `df['close_75_z']` returns the Z-Score of close price with a window of 75
 
+#### [Awesome Oscillator](https://www.ifcm.co.uk/ntx-indicators/awesome-oscillator)
+
+The AO indicator is a good indicator for measuring the market dynamics,
+it reflects specific changes in the driving force of the market, which
+helps to identify the strength of the trend, including the points of
+its formation and reversal.
+
+Awesome Oscillator Formula
+
+* MEDIAN PRICE = (HIGH+LOW)/2
+* AO = SMA(MEDIAN PRICE, 5)-SMA(MEDIAN PRICE, 34)
+
+Examples:
+* `df['ao']` returns the Awesome Oscillator with default windows (5, 34)
+* `df['ao_3,10']` returns the Awesome Oscillator with a window of 3 and 10
+
 ## Issues
 
 We use [Github Issues](https://github.com/jealous/stockstats/issues) to track
 the issues or bugs.
 
 ## Others
```

### Comparing `stockstats-0.5.3/stockstats.py` & `stockstats-0.5.4/stockstats.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,14 +101,17 @@
 
     WAVE_TREND_1 = 10
     WAVE_TREND_2 = 21
 
     KAMA_SLOW = 34
     KAMA_FAST = 5
 
+    AO_SLOW = 34
+    AO_FAST = 5
+
     MULTI_SPLIT_INDICATORS = ("kama",)
 
     # End of options
 
     @staticmethod
     def _change(series, window):
         return series.pct_change(periods=-window).fillna(0.0) * 100
@@ -544,40 +547,41 @@
 
         high = self['high']
         low = self['low']
         close = self['close']
         m_atr = self.SUPERTREND_MUL * self._atr(window)
         hl_avg = (high + low) / 2.0
         # basic upper band
-        b_ub = hl_avg + m_atr
+        b_ub = list(hl_avg + m_atr)
         # basic lower band
-        b_lb = hl_avg - m_atr
+        b_lb = list(hl_avg - m_atr)
 
         size = len(close)
         ub = np.empty(size, dtype=np.float64)
         lb = np.empty(size, dtype=np.float64)
         st = np.empty(size, dtype=np.float64)
+        close = list(close)
 
         for i in range(size):
             if i == 0:
-                ub[i] = b_ub.iloc[i]
-                lb[i] = b_lb.iloc[i]
-                if close.iloc[i] <= ub[i]:
+                ub[i] = b_ub[i]
+                lb[i] = b_lb[i]
+                if close[i] <= ub[i]:
                     st[i] = ub[i]
                 else:
                     st[i] = lb[i]
                 continue
 
-            last_close = close.iloc[i - 1]
-            curr_close = close.iloc[i]
+            last_close = close[i - 1]
+            curr_close = close[i]
             last_ub = ub[i - 1]
             last_lb = lb[i - 1]
             last_st = st[i - 1]
-            curr_b_ub = b_ub.iloc[i]
-            curr_b_lb = b_lb.iloc[i]
+            curr_b_ub = b_ub[i]
+            curr_b_lb = b_lb[i]
 
             # calculate current upper band
             if curr_b_ub < last_ub or last_close > last_ub:
                 ub[i] = curr_b_ub
             else:
                 ub[i] = last_ub
 
@@ -1166,14 +1170,43 @@
         rolling_pos_flow = self._mov_sum(pos_flow, window)
         rolling_neg_flow = self._mov_sum(neg_flow, window)
         money_flow_ratio = rolling_pos_flow / (rolling_neg_flow + 1e-12)
         mfi = (1.0 - 1.0 / (1 + money_flow_ratio))
         mfi.iloc[:window] = 0.5
         self[column_name] = mfi
 
+    def _get_ao(self, windows=None):
+        """ get awesome oscillator
+
+        The AO indicator is a good indicator for measuring the market dynamics,
+        it reflects specific changes in the driving force of the market, which
+        helps to identify the strength of the trend, including the points of
+        its formation and reversal.
+
+
+        Awesome Oscillator Formula
+        * MEDIAN PRICE = (HIGH+LOW)/2
+        * AO = SMA(MEDIAN PRICE, 5)-SMA(MEDIAN PRICE, 34)
+
+        https://www.ifcm.co.uk/ntx-indicators/awesome-oscillator
+        """
+        if windows is None:
+            fast = self.AO_FAST
+            slow = self.AO_SLOW
+            column_name = 'ao'
+        else:
+            n0, n1 = self.to_ints(windows)
+            fast = min(n0, n1)
+            slow = max(n0, n1)
+            column_name = 'ao_{},{}'.format(fast, slow)
+
+        median_price = (self['high'] + self['low']) * 0.5
+        ao = self._sma(median_price, fast) - self._sma(median_price, slow)
+        self[column_name] = ao
+
     def _get_kama(self, column, windows, fasts=None, slows=None):
         """ get Kaufman's Adaptive Moving Average.
         Implemented after
         https://school.stockcharts.com/doku.php?id=technical_indicators:kaufman_s_adaptive_moving_average
 
         :param column: column to calculate
         :param windows: collection of window of exponential moving average
@@ -1196,25 +1229,26 @@
         change = (col - col_window_s).abs()
         volatility = self._mov_sum((col - col_last).abs(), window)
         efficiency_ratio = change / volatility
         fast_ema_smoothing = 2.0 / (fast + 1)
         slow_ema_smoothing = 2.0 / (slow + 1)
         smoothing_2 = fast_ema_smoothing - slow_ema_smoothing
         efficient_smoothing = efficiency_ratio * smoothing_2
-        smoothing = 2 * (efficient_smoothing + slow_ema_smoothing)
+        smoothing = list(2 * (efficient_smoothing + slow_ema_smoothing))
 
         # start with simple moving average
-        kama = self._sma(col, window)
+        kama = list(self._sma(col, window))
+        col_list = list(col)
         if len(kama) >= window:
-            last_kama = kama.iloc[window - 1]
+            last_kama = kama[window - 1]
         else:
             last_kama = 0.0
         for i in range(window, len(kama)):
-            cur = smoothing.iloc[i] * (col.iloc[i] - last_kama) + last_kama
-            kama.iloc[i] = cur
+            cur = smoothing[i] * (col_list[i] - last_kama) + last_kama
+            kama[i] = cur
             last_kama = cur
         self[column_name] = kama
 
     @staticmethod
     def parse_column_name(name):
         m = re.match(r'(.*)_([\d\-+~,.]+)_(\w+)', name)
         ret = (None,)
@@ -1343,14 +1377,15 @@
             ('mfi',): self._get_mfi,
             ('wt1', 'wt2'): self._get_wave_trend,
             ('wr',): self._get_wr,
             ('supertrend',
              'supertrend_lb',
              'supertrend_ub'): self._get_supertrend,
             ('aroon',): self._get_aroon,
+            ('ao',): self._get_ao,
         }
 
     def __init_not_exist_column(self, key):
         for names, handler in self.handler.items():
             if key in names:
                 handler()
                 return
```

