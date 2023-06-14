# Comparing `tmp/volstreet-0.9.8.tar.gz` & `tmp/volstreet-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volstreet-0.9.8.tar", last modified: Tue Jun 13 08:25:51 2023, max compression
+gzip compressed data, was "volstreet-0.9.9.tar", last modified: Wed Jun 14 06:56:50 2023, max compression
```

## Comparing `volstreet-0.9.8.tar` & `volstreet-0.9.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 08:25:51.362784 volstreet-0.9.8/
--rw-rw-rw-   0        0        0      497 2023-06-13 08:25:51.362784 volstreet-0.9.8/PKG-INFO
--rw-rw-rw-   0        0        0      124 2023-06-07 14:47:58.000000 volstreet-0.9.8/README.md
--rw-rw-rw-   0        0        0       91 2023-05-24 02:09:11.000000 volstreet-0.9.8/pyproject.toml
--rw-rw-rw-   0        0        0     1375 2023-06-13 08:25:51.364780 volstreet-0.9.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-13 08:25:51.355502 volstreet-0.9.8/volstreet/
--rw-rw-rw-   0        0        0    16121 2023-05-24 02:09:11.000000 volstreet-0.9.8/volstreet/SmartWebSocketV2.py
--rw-rw-rw-   0        0        0       37 2023-06-07 15:08:38.000000 volstreet-0.9.8/volstreet/__init__.py
--rw-rw-rw-   0        0        0     8133 2023-06-07 07:39:33.000000 volstreet-0.9.8/volstreet/blackscholes.py
--rw-rw-rw-   0        0        0     2694 2023-06-07 14:47:58.000000 volstreet-0.9.8/volstreet/constants.py
--rw-rw-rw-   0        0        0    25475 2023-06-12 13:04:14.000000 volstreet-0.9.8/volstreet/datamodule.py
--rw-rw-rw-   0        0        0   167555 2023-06-13 08:04:56.000000 volstreet-0.9.8/volstreet/dealingroom.py
--rw-rw-rw-   0        0        0     1683 2023-05-24 02:09:11.000000 volstreet-0.9.8/volstreet/discord_bot.py
--rw-rw-rw-   0        0        0      209 2023-06-06 15:42:44.000000 volstreet-0.9.8/volstreet/exceptions.py
--rw-rw-rw-   0        0        0    39664 2023-05-24 02:09:11.000000 volstreet-0.9.8/volstreet/nsefunctions.py
--rw-rw-rw-   0        0        0    14536 2023-06-07 14:47:58.000000 volstreet-0.9.8/volstreet/strategies.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:25:51.362784 volstreet-0.9.8/volstreet.egg-info/
--rw-rw-rw-   0        0        0      497 2023-06-13 08:25:51.000000 volstreet-0.9.8/volstreet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      447 2023-06-13 08:25:51.000000 volstreet-0.9.8/volstreet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 08:25:51.000000 volstreet-0.9.8/volstreet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      787 2023-06-13 08:25:51.000000 volstreet-0.9.8/volstreet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-13 08:25:51.000000 volstreet-0.9.8/volstreet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 06:56:50.886340 volstreet-0.9.9/
+-rw-rw-rw-   0        0        0      497 2023-06-14 06:56:50.887338 volstreet-0.9.9/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2023-06-07 14:47:58.000000 volstreet-0.9.9/README.md
+-rw-rw-rw-   0        0        0       91 2023-05-24 02:09:11.000000 volstreet-0.9.9/pyproject.toml
+-rw-rw-rw-   0        0        0     1375 2023-06-14 06:56:50.888334 volstreet-0.9.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-14 06:56:50.879365 volstreet-0.9.9/volstreet/
+-rw-rw-rw-   0        0        0    16121 2023-05-24 02:09:11.000000 volstreet-0.9.9/volstreet/SmartWebSocketV2.py
+-rw-rw-rw-   0        0        0       37 2023-06-07 15:08:38.000000 volstreet-0.9.9/volstreet/__init__.py
+-rw-rw-rw-   0        0        0     8765 2023-06-13 13:36:04.000000 volstreet-0.9.9/volstreet/blackscholes.py
+-rw-rw-rw-   0        0        0     2694 2023-06-07 14:47:58.000000 volstreet-0.9.9/volstreet/constants.py
+-rw-rw-rw-   0        0        0    25475 2023-06-12 13:04:14.000000 volstreet-0.9.9/volstreet/datamodule.py
+-rw-rw-rw-   0        0        0   168512 2023-06-14 04:51:09.000000 volstreet-0.9.9/volstreet/dealingroom.py
+-rw-rw-rw-   0        0        0     1683 2023-05-24 02:09:11.000000 volstreet-0.9.9/volstreet/discord_bot.py
+-rw-rw-rw-   0        0        0      209 2023-06-06 15:42:44.000000 volstreet-0.9.9/volstreet/exceptions.py
+-rw-rw-rw-   0        0        0    39664 2023-05-24 02:09:11.000000 volstreet-0.9.9/volstreet/nsefunctions.py
+-rw-rw-rw-   0        0        0    14536 2023-06-07 14:47:58.000000 volstreet-0.9.9/volstreet/strategies.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:56:50.885343 volstreet-0.9.9/volstreet.egg-info/
+-rw-rw-rw-   0        0        0      497 2023-06-14 06:56:50.000000 volstreet-0.9.9/volstreet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      447 2023-06-14 06:56:50.000000 volstreet-0.9.9/volstreet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 06:56:50.000000 volstreet-0.9.9/volstreet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      787 2023-06-14 06:56:50.000000 volstreet-0.9.9/volstreet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-14 06:56:50.000000 volstreet-0.9.9/volstreet.egg-info/top_level.txt
```

### Comparing `volstreet-0.9.8/setup.cfg` & `volstreet-0.9.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6f6c 7374 7265 6574 0d0a 7665   = volstreet..ve
-00000020: 7273 696f 6e20 3d20 302e 392e 380d 0a61  rsion = 0.9.8..a
+00000020: 7273 696f 6e20 3d20 302e 392e 390d 0a61  rsion = 0.9.9..a
 00000030: 7574 686f 7220 3d20 5261 6875 6c20 5468  uthor = Rahul Th
 00000040: 616b 6b61 720d 0a61 7574 686f 725f 656d  akkar..author_em
 00000050: 6169 6c20 3d20 722e 7468 616b 6b61 7231  ail = r.thakkar1
 00000060: 3540 676d 6169 6c2e 636f 6d0d 0a64 6573  5@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2056 6f6c 5374  cription = VolSt
 00000080: 7265 6574 2069 7320 6120 5079 7468 6f6e  reet is a Python
 00000090: 206c 6962 7261 7279 2066 6f72 2061 7574   library for aut
```

### Comparing `volstreet-0.9.8/volstreet/SmartWebSocketV2.py` & `volstreet-0.9.9/volstreet/SmartWebSocketV2.py`

 * *Files identical despite different names*

### Comparing `volstreet-0.9.8/volstreet/blackscholes.py` & `volstreet-0.9.9/volstreet/blackscholes.py`

 * *Files 13% similar despite different names*

```diff
@@ -165,38 +165,63 @@
             "theta": thetas,
             "vega": vegas,
             "implied_volatility": ivs,
         }
     )
 
 
-def iv_curve_adjustor(movement, time_to_expiry, iv=1, spot=100, strike=100, _print_details=False):
+def iv_transformer_coeffs(tte):
+    adjuster = 3 if tte < (0.8 / 365) else 1
+    dfs2 = 1 / ((tte ** 1.2) * adjuster)
+    dfs2 = min(dfs2, 20000)
+
+    dfs = 1 / ((tte ** 0.45) * 5)
+    dfs = min(dfs, 5)
+    dfs = -6 + dfs
+    return dfs2, dfs, .97
+
+
+def iv_transformer_coeffs_wip(tte):
+
+    # distance squared coefficient
+    dfs2 = 3270.27*np.exp(-384.38*tte) + 100
+    dfs2 = min(dfs2, 20000)
+
+    # distance coefficient
+    if tte < 0.26/365:
+        dfs = 1
+    else:
+        dfs = 1 / ((tte ** 0.45) * 5)
+        dfs = min(dfs, 5)
+        dfs = -6 + dfs
+
+    # intercept
+    if tte < 3/(24*365):
+        intercept = 1.07
+    elif tte < 0.27/365:
+        intercept = 1
+    else:
+        intercept = 0.98
+    return dfs2, dfs, intercept
+
+
+def iv_curve_adjustor(movement, time_to_expiry, iv: int | tuple = 1, spot=100, strike=100, _print_details=False):
 
     """
     This function returns the adjusted implied volatility accounting for the curve effect.
     :param movement: movement of the underlying in percentage with sign
     :param time_to_expiry: time to expiry in years
     :param iv: implied volatility of the strike
     :param spot: spot price
     :param strike: strike price
     :param _print_details: print details of the adjustment
     :return: adjusted implied volatility for the strike after the movement
     """
 
-    def iv_transformer_coeffs(tte):
-        adjuster = 3 if tte < (0.8 / 365) else 1
-        dfs2 = 1 / ((tte ** 1.2) * adjuster)
-        dfs2 = min(dfs2, 20000)
-
-        dfs = 1 / ((tte ** 0.45) * 5)
-        dfs = min(dfs, 5)
-        dfs = -6 + dfs
-        return dfs2, dfs, .97
-
-    coefs = iv_transformer_coeffs(time_to_expiry)
+    coefs = iv_transformer_coeffs_wip(time_to_expiry)
     current_diff = (strike/spot - 1)
     current_iv_multiple = coefs[0] * current_diff ** 2 + coefs[1] * current_diff + coefs[2]
     atm_iv = iv / current_iv_multiple
 
     new_spot = spot * (1 + movement)
     total_displacement = (strike / new_spot - 1)
     premium_to_atm_iv = coefs[0] * total_displacement ** 2 + coefs[1] * total_displacement + coefs[2]
@@ -229,14 +254,17 @@
     flag = flag.lower()[0]
     price_func = call if flag == 'c' else put
     vol = implied_volatility(current_price, current_spot, strike, timeleft, 0.06, flag)
     delta_ = delta(current_spot, strike, timeleft, 0.06, vol, flag)
     estimated_movement_points = (target_price - current_price) / delta_
     estimated_movement = estimated_movement_points / current_spot
     timeleft = timeleft - (time_delta / 525600) if time_delta else timeleft
+    if timeleft < 0.0008:  # On expiry day
+        vol_multiple = 2 - (1401.74 * timeleft)
+        vol = vol * vol_multiple
     modified_vol = iv_curve_adjustor(estimated_movement, timeleft, iv=vol, spot=current_spot, strike=strike)
 
     if _print_details:
         print(f'estimated movement: {estimated_movement}, vol: {vol}, modified vol: {modified_vol}')
 
     f = lambda s1: price_func(s1, strike, timeleft, 0.06, modified_vol) - target_price
```

### Comparing `volstreet-0.9.8/volstreet/constants.py` & `volstreet-0.9.9/volstreet/constants.py`

 * *Files identical despite different names*

### Comparing `volstreet-0.9.8/volstreet/datamodule.py` & `volstreet-0.9.9/volstreet/datamodule.py`

 * *Files identical despite different names*

### Comparing `volstreet-0.9.8/volstreet/dealingroom.py` & `volstreet-0.9.9/volstreet/dealingroom.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from smartapi import SmartConnect
 from smartapi.smartExceptions import DataException
 import pyotp
 from threading import Thread
 from volstreet.SmartWebSocketV2 import SmartWebSocketV2
 from volstreet.constants import scrips, holidays, symbol_df, logger
 from volstreet import blackscholes as bs, datamodule as dm
-from collections import defaultdict
+from collections import defaultdict, deque
 import yfinance as yf
 from fuzzywuzzy import process
 import re
 import logging
 import functools
 import itertools
 import traceback
@@ -2614,15 +2614,15 @@
         call_stop_loss : float, optional
             Call stop loss percentage, by default None. If None then stop loss is same as stop_loss.
         put_stop_loss : float, optional
             Put stop loss percentage, by default None. If None then stop loss is same as stop_loss.
         exit_time : tuple, optional
             Exit time, by default (15, 29)
         sleep_time : int, optional
-            Sleep time in seconds for updating prices, by default 60
+            Sleep time in seconds for updating prices, by default 5
         catch_trend : bool, optional
             Catch trend or not, by default False
         trend_qty_ratio : int, optional
             Ratio of trend quantity to strangle quantity, by default 1
         trend_strike_offset : float, optional
             Strike offset for trend order in percentage terms, by default 0
         trend_sl : float, optional
@@ -2634,26 +2634,41 @@
         @log_errors
         def position_monitor(info_dict):
 
             c_avg_price = info_dict["call_avg_price"]
             p_avg_price = info_dict["put_avg_price"]
             traded_strangle = info_dict["traded_strangle"]
 
+            # Price deque
+            n_prices = max(int(30/sleep_time), 1)  # Hard coded 30-second price window for now
+            last_n_prices = {"call": deque(maxlen=n_prices), "put": deque(maxlen=n_prices)}
+
             last_print_time = currenttime()
             last_log_time = currenttime()
             last_notify_time = currenttime()
             print_interval = timedelta(seconds=5)
-            log_interval = timedelta(minutes=5)
-            notify_interval = timedelta(minutes=60)
+            log_interval = timedelta(minutes=60)
+            notify_interval = timedelta(minutes=180)
+
             while not info_dict["exit_triggers"]["trade_complete"]:
+
+                # Fetching prices
                 spot_price = self.fetch_ltp()
                 c_ltp, p_ltp = traded_strangle.fetch_ltp()
                 info_dict["underlying_ltp"] = spot_price
                 info_dict["call_ltp"] = c_ltp
                 info_dict["put_ltp"] = p_ltp
+                last_n_prices["call"].append(c_ltp)
+                last_n_prices["put"].append(p_ltp)
+                c_ltp_avg = sum(last_n_prices["call"])/len(last_n_prices["call"]) if last_n_prices["call"] else c_ltp
+                p_ltp_avg = sum(last_n_prices["put"])/len(last_n_prices["put"]) if last_n_prices["put"] else p_ltp
+                info_dict["call_ltp_avg"] = c_ltp_avg
+                info_dict["put_ltp_avg"] = p_ltp_avg
+
+                # Calculate IV
                 call_iv, put_iv, avg_iv = strangle_iv(
                     callprice=c_ltp,
                     putprice=p_ltp,
                     callstrike=call_strike,
                     putstrike=put_strike,
                     spot=spot_price,
                     timeleft=timetoexpiry(expiry)
@@ -2678,14 +2693,16 @@
                     f"Time: {currenttime():%d-%m-%Y %H:%M:%S}\n"
                     f"Underlying LTP: {spot_price}\n"
                     f"Call Strike: {call_strike}\n"
                     f"Put Strike: {put_strike}\n"
                     f"Call Price: {c_ltp}\n"
                     f"Put Price: {p_ltp}\n"
                     f"MTM Price: {mtm_price}\n"
+                    f"Call last n avg: {c_ltp_avg}\n"
+                    f"Put last n avg: {p_ltp_avg}\n"
                     f"IVs: {call_iv}, {put_iv}, {avg_iv}\n"
                     f"Call SL: {info_dict['call_sl']}\n"
                     f"Put SL: {info_dict['put_sl']}\n"
                     f"Profit Pts: {info_dict['profit_in_pts']:.2f}\n"
                     f"Profit: {info_dict['profit_in_rs']:.2f}\n"
                 )
                 if currenttime() - last_print_time > print_interval:
@@ -2759,15 +2776,15 @@
             place_option_order_and_notify(
                 trend_option, "BUY", qty_in_lots, "LIMIT", "Intraday Strangle Trend Catcher", self.webhook_url
             )
 
         def check_for_stop_loss(info_dict, side, sl_order_ids=None):
 
             if sl_order_ids is None:  # Not using SL orders
-                sl = info_dict[f"{side}_ltp"] > info_dict[f"{side}_stop_loss_price"]
+                sl = info_dict[f"{side}_ltp_avg"] > info_dict[f"{side}_stop_loss_price"]
 
             else:  # Using SL orders
                 sl = False
                 pass  # TODO: Implement fetching order status and checking for SL
 
             info_dict[f"{side}_sl"] = sl
 
@@ -2801,15 +2818,15 @@
                     other_sl_option = traded_strangle.put_option if sl_type == "call" else traded_strangle.call_option
                     notifier(f'{self.name} strangle {other_sl_type} stop loss hit.', self.webhook_url)
                     other_exit_price = place_option_order_and_notify(
                         other_sl_option, "BUY", quantity_in_lots, "LIMIT", order_tag, self.webhook_url
                     )
                     info_dict[f'{other_sl_type}_exit_price'] = other_exit_price
                     break
-                sleep(sleep_time)
+                sleep(1)
 
         # Setting strikes and expiry
         order_tag = "Intraday Strangle"
         underlying_ltp = self.fetch_ltp()
         call_strike = underlying_ltp * (1 + call_strike_offset)
         put_strike = underlying_ltp * (1 - put_strike_offset)
         call_strike = findstrike(call_strike, self.base)
@@ -2918,26 +2935,27 @@
             "call_sl": False,
             "put_sl": False,
             "exit_triggers": {"trade_complete": False}
         }
 
         position_monitor_thread = Thread(target=position_monitor, args=(shared_info_dict,))
         position_monitor_thread.start()
+        sleep(3)  # To ensure that the position monitor thread has started
 
         # Wait for exit time or both stop losses to hit (Main Loop)
         while all([currenttime().time() < time(*exit_time)]):
             check_for_stop_loss(shared_info_dict, 'call')
             if shared_info_dict["call_sl"]:
                 process_stop_loss(shared_info_dict, "call")
                 break
             check_for_stop_loss(shared_info_dict, 'put')
             if shared_info_dict["put_sl"]:
                 process_stop_loss(shared_info_dict, "put")
                 break
-            sleep(sleep_time)
+            sleep(1)
 
         # Out of the while loop, so exit time reached or both stop losses hit
 
         call_sl = shared_info_dict["call_sl"]
         put_sl = shared_info_dict["put_sl"]
 
         if not call_sl and not put_sl:
@@ -3876,14 +3894,18 @@
 # Finding ATM strike
 def findstrike(x, base):
     number = base * round(x / base)
     return int(number)
 
 
 def custom_round(x, base=0.05):
+
+    if x == 0:
+        return 0
+
     num = base * round(x / base)
     if num == 0:
         num = base
     return round(num, 2)
 
 
 def splice_orders(quantity_in_lots, freeze_qty):
```

### Comparing `volstreet-0.9.8/volstreet/discord_bot.py` & `volstreet-0.9.9/volstreet/discord_bot.py`

 * *Files identical despite different names*

### Comparing `volstreet-0.9.8/volstreet/nsefunctions.py` & `volstreet-0.9.9/volstreet/nsefunctions.py`

 * *Files identical despite different names*

### Comparing `volstreet-0.9.8/volstreet/strategies.py` & `volstreet-0.9.9/volstreet/strategies.py`

 * *Files identical despite different names*

### Comparing `volstreet-0.9.8/volstreet.egg-info/requires.txt` & `volstreet-0.9.9/volstreet.egg-info/requires.txt`

 * *Files identical despite different names*

