# Comparing `tmp/polygon-sdk-1.0.3.tar.gz` & `tmp/polygon-sdk-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polygon-sdk-1.0.3.tar", last modified: Tue Jun 13 22:16:36 2023, max compression
+gzip compressed data, was "polygon-sdk-1.0.5.tar", last modified: Tue Jun 13 22:22:29 2023, max compression
```

## Comparing `polygon-sdk-1.0.3.tar` & `polygon-sdk-1.0.5.tar`

### file list

```diff
@@ -1,178 +1,191 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 22:16:36.656661 polygon-sdk-1.0.3/
--rw-rw-rw-   0        0        0     2507 2023-06-13 22:16:36.655661 polygon-sdk-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1929 2023-06-12 00:29:12.000000 polygon-sdk-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 22:16:36.561746 polygon-sdk-1.0.3/_discord/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 polygon-sdk-1.0.3/_discord/__init__.py
--rw-rw-rw-   0        0        0     7983 2023-06-11 21:54:23.000000 polygon-sdk-1.0.3/_discord/discord_stock_example.py
--rw-rw-rw-   0        0        0    44936 2023-06-11 21:54:23.000000 polygon-sdk-1.0.3/_discord/discord_stock_market.py
--rw-rw-rw-   0        0        0    16306 2023-06-11 21:54:23.000000 polygon-sdk-1.0.3/_discord/embeddings.py
--rw-rw-rw-   0        0        0      581 2023-06-11 21:54:23.000000 polygon-sdk-1.0.3/_discord/emojis.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:16:36.563745 polygon-sdk-1.0.3/_discord/hooks/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 polygon-sdk-1.0.3/_discord/hooks/__init__.py
--rw-rw-rw-   0        0        0     1594 2023-06-11 21:54:23.000000 polygon-sdk-1.0.3/_discord/hooks/channel_webhooks.py
--rw-rw-rw-   0        0        0    10521 2023-06-11 21:54:23.000000 polygon-sdk-1.0.3/_discord/hooks/hook_dicts.py
--rw-rw-rw-   0        0        0     5462 2023-06-11 21:54:23.000000 polygon-sdk-1.0.3/_discord/hooks/send_webhook.py
--rw-rw-rw-   0        0        0    33594 2023-06-11 21:54:23.000000 polygon-sdk-1.0.3/_discord/live_discord.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:16:36.564746 polygon-sdk-1.0.3/_discord/selectmenus/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 polygon-sdk-1.0.3/_discord/selectmenus/__init__.py
--rw-rw-rw-   0        0        0    33209 2023-06-11 22:20:44.000000 polygon-sdk-1.0.3/_discord/selectmenus/mainselect.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:16:36.566745 polygon-sdk-1.0.3/_discord/views/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 polygon-sdk-1.0.3/_discord/views/__init__.py
--rw-rw-rw-   0        0        0     1640 2023-06-11 21:54:23.000000 polygon-sdk-1.0.3/_discord/views/mainview.py
--rw-rw-rw-   0        0        0     3792 2023-06-11 21:54:23.000000 polygon-sdk-1.0.3/_discord/views/menus.py
--rw-rw-rw-   0        0        0     7502 2023-06-11 21:54:23.000000 polygon-sdk-1.0.3/_discord/webhook_creation.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:16:36.570746 polygon-sdk-1.0.3/bot/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 polygon-sdk-1.0.3/bot/__init__.py
--rw-rw-rw-   0        0        0    13209 2023-06-11 22:18:58.000000 polygon-sdk-1.0.3/bot/autocomp.py
--rw-rw-rw-   0        0        0     6919 2023-06-11 22:19:59.000000 polygon-sdk-1.0.3/bot/discord_emojis.py
--rw-rw-rw-   0        0        0        0 2023-06-11 21:54:23.000000 polygon-sdk-1.0.3/bot/helpers.py
--rw-rw-rw-   0        0        0     1279 2023-06-11 22:22:28.000000 polygon-sdk-1.0.3/bot/main.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:16:36.572745 polygon-sdk-1.0.3/bot/utils/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 polygon-sdk-1.0.3/bot/utils/__init__.py
--rw-rw-rw-   0        0        0   101924 2023-06-11 22:19:10.000000 polygon-sdk-1.0.3/bot/utils/lists_and_dicts.py
--rw-rw-rw-   0        0        0   199781 2023-06-11 22:17:58.000000 polygon-sdk-1.0.3/bot/utils/webull_tickers.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:16:36.574746 polygon-sdk-1.0.3/examples/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 polygon-sdk-1.0.3/examples/__init__.py
--rw-rw-rw-   0        0        0     5940 2023-06-11 21:54:23.000000 polygon-sdk-1.0.3/examples/all_attributes.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:16:36.578746 polygon-sdk-1.0.3/examples/realtime_markets/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 polygon-sdk-1.0.3/examples/realtime_markets/__init__.py
--rw-rw-rw-   0        0        0     2479 2023-06-11 21:54:23.000000 polygon-sdk-1.0.3/examples/realtime_markets/crypto_market.py
--rw-rw-rw-   0        0        0    44945 2023-06-11 21:54:23.000000 polygon-sdk-1.0.3/examples/realtime_markets/discord_market.py
--rw-rw-rw-   0        0        0      922 2023-06-11 21:54:23.000000 polygon-sdk-1.0.3/examples/realtime_markets/forex_market.py
--rw-rw-rw-   0        0        0      776 2023-06-11 21:54:23.000000 polygon-sdk-1.0.3/examples/realtime_markets/indices_market.py
--rw-rw-rw-   0        0        0      989 2023-06-11 21:54:23.000000 polygon-sdk-1.0.3/examples/realtime_markets/options_market.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:16:36.580745 polygon-sdk-1.0.3/examples/simulated_markets/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 polygon-sdk-1.0.3/examples/simulated_markets/__init__.py
--rw-rw-rw-   0        0        0      688 2023-06-11 21:54:23.000000 polygon-sdk-1.0.3/examples/simulated_markets/helpers.py
--rw-rw-rw-   0        0        0     5115 2023-06-11 22:19:16.000000 polygon-sdk-1.0.3/examples/simulated_markets/mock_discord.py
--rw-rw-rw-   0        0        0     1951 2023-06-12 01:17:16.000000 polygon-sdk-1.0.3/examples/simulated_markets/mock_market.py
--rw-rw-rw-   0        0        0     1551 2023-06-12 01:18:49.000000 polygon-sdk-1.0.3/examples/simulated_markets/mock_options_market.py
--rw-rw-rw-   0        0        0    14931 2023-06-11 21:54:23.000000 polygon-sdk-1.0.3/examples/webull_data.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:16:36.582746 polygon-sdk-1.0.3/funcs/
--rw-rw-rw-   0        0        0        0 2023-06-11 22:29:36.000000 polygon-sdk-1.0.3/funcs/__init__.py
--rw-rw-rw-   0        0        0    36181 2023-06-11 22:44:36.000000 polygon-sdk-1.0.3/funcs/get_data.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:16:36.589073 polygon-sdk-1.0.3/polygon_sdk.egg-info/
--rw-rw-rw-   0        0        0     2507 2023-06-13 22:16:36.000000 polygon-sdk-1.0.3/polygon_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4716 2023-06-13 22:16:36.000000 polygon-sdk-1.0.3/polygon_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 22:16:36.000000 polygon-sdk-1.0.3/polygon_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-06-13 22:16:36.000000 polygon-sdk-1.0.3/polygon_sdk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-13 22:16:36.589073 polygon-sdk-1.0.3/sdks/
--rw-rw-rw-   0        0        0        0 2023-06-11 22:15:21.000000 polygon-sdk-1.0.3/sdks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:16:36.589073 polygon-sdk-1.0.3/sdks/discord_sdk/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/discord_sdk/__init__.py
--rw-rw-rw-   0        0        0       53 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/discord_sdk/channel_ids.py
--rw-rw-rw-   0        0        0     4497 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/discord_sdk/discord_sdk.py
--rw-rw-rw-   0        0        0     2157 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/discord_sdk/searching.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:16:36.610978 polygon-sdk-1.0.3/sdks/examples/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/examples/__init__.py
--rw-rw-rw-   0        0        0     6184 2023-06-12 00:26:46.000000 polygon-sdk-1.0.3/sdks/examples/all_attributes.py
--rw-rw-rw-   0        0        0      517 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/examples/bollinger_bands.py
--rw-rw-rw-   0        0        0      706 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/examples/create_option_symbol.py
--rw-rw-rw-   0        0        0     1664 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/examples/ema.py
--rw-rw-rw-   0        0        0      910 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/examples/fetch_entire_chain.py
--rw-rw-rw-   0        0        0      649 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/examples/find_gaps.py
--rw-rw-rw-   0        0        0      823 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/examples/get_all_options_data.py
--rw-rw-rw-   0        0        0     2399 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/examples/get_ema.py
--rw-rw-rw-   0        0        0      600 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/examples/get_latest_crypto_data.py
--rw-rw-rw-   0        0        0      585 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/examples/get_latest_forex_data.py
--rw-rw-rw-   0        0        0      446 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/examples/get_latest_indices_data.py
--rw-rw-rw-   0        0        0      644 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/examples/get_latest_ticker_data.py
--rw-rw-rw-   0        0        0     3161 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/examples/get_macd.py
--rw-rw-rw-   0        0        0      582 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/examples/get_pivot_points.py
--rw-rw-rw-   0        0        0     2051 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/examples/get_rsi.py
--rw-rw-rw-   0        0        0     2172 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/examples/get_sma.py
--rw-rw-rw-   0        0        0     1796 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/examples/latest_news.py
--rw-rw-rw-   0        0        0     1625 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/examples/option_quote.py
--rw-rw-rw-   0        0        0     2408 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/examples/option_trades.py
--rw-rw-rw-   0        0        0     1408 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/examples/plot_aggs.py
--rw-rw-rw-   0        0        0      796 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/examples/plot_macd.py
--rw-rw-rw-   0        0        0     1797 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/examples/plot_option_aggs.py
--rw-rw-rw-   0        0        0      487 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/examples/rate_of_change.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:16:36.613978 polygon-sdk-1.0.3/sdks/examples/realtime_markets/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/examples/realtime_markets/__init__.py
--rw-rw-rw-   0        0        0     2479 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/examples/realtime_markets/crypto_market.py
--rw-rw-rw-   0        0        0      922 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/examples/realtime_markets/forex_market.py
--rw-rw-rw-   0        0        0      776 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/examples/realtime_markets/indices_market.py
--rw-rw-rw-   0        0        0      989 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/examples/realtime_markets/options_market.py
--rw-rw-rw-   0        0        0     4837 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/examples/scanner_example.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:16:36.615978 polygon-sdk-1.0.3/sdks/examples/simulated_markets/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/examples/simulated_markets/__init__.py
--rw-rw-rw-   0        0        0      688 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/examples/simulated_markets/helpers.py
--rw-rw-rw-   0        0        0     2606 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/examples/simulated_markets/mock_market.py
--rw-rw-rw-   0        0        0     1806 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/examples/simulated_markets/mock_options_market.py
--rw-rw-rw-   0        0        0     2116 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/examples/stock_aggregates.py
--rw-rw-rw-   0        0        0     1189 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/examples/support_resistance.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:16:36.618978 polygon-sdk-1.0.3/sdks/fudstop_sdk/
--rw-rw-rw-   0        0        0        1 2023-06-12 00:06:40.000000 polygon-sdk-1.0.3/sdks/fudstop_sdk/__init__.py
--rw-rw-rw-   0        0        0     2909 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/fudstop_sdk/fudstop_sdk.py
--rw-rw-rw-   0        0        0     1661 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/fudstop_sdk/gaps.py
--rw-rw-rw-   0        0        0      427 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/fudstop_sdk/option_vol_totals.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:16:36.621977 polygon-sdk-1.0.3/sdks/helpers/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/helpers/__init__.py
--rw-rw-rw-   0        0        0     2001 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/helpers/conditions.py
--rw-rw-rw-   0        0        0        2 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/helpers/get_cik.py
--rw-rw-rw-   0        0        0     5442 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/helpers/helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:16:36.623978 polygon-sdk-1.0.3/sdks/models/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/models/__init__.py
--rw-rw-rw-   0        0        0      488 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/models/common.py
--rw-rw-rw-   0        0        0     5097 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/models/maps.py
--rw-rw-rw-   0        0        0    13078 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/models/test_events.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:16:36.638982 polygon-sdk-1.0.3/sdks/polygon_sdk/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/polygon_sdk/__init__.py
--rw-rw-rw-   0        0        0     1265 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/polygon_sdk/aggregates.py
--rw-rw-rw-   0        0        0    29379 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/polygon_sdk/async_options_sdk.py
--rw-rw-rw-   0        0        0    52775 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/polygon_sdk/async_polygon_sdk.py
--rw-rw-rw-   0        0        0     1135 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/polygon_sdk/company_info.py
--rw-rw-rw-   0        0        0      703 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/polygon_sdk/daily_open_close.py
--rw-rw-rw-   0        0        0    15043 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/polygon_sdk/financials.py
--rw-rw-rw-   0        0        0     6644 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/polygon_sdk/forex_crypto.py
--rw-rw-rw-   0        0        0     8957 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/polygon_sdk/get_all_options.py
--rw-rw-rw-   0        0        0     1131 2023-06-11 21:54:24.000000 polygon-sdk-1.0.3/sdks/polygon_sdk/indices_snapshot.py
--rw-rw-rw-   0        0        0      823 2023-06-11 21:54:25.000000 polygon-sdk-1.0.3/sdks/polygon_sdk/logo.py
--rw-rw-rw-   0        0        0    27900 2023-06-11 21:54:25.000000 polygon-sdk-1.0.3/sdks/polygon_sdk/mapping_dicts.py
--rw-rw-rw-   0        0        0      782 2023-06-11 21:54:25.000000 polygon-sdk-1.0.3/sdks/polygon_sdk/models.py
--rw-rw-rw-   0        0        0      819 2023-06-11 21:54:25.000000 polygon-sdk-1.0.3/sdks/polygon_sdk/news.py
--rw-rw-rw-   0        0        0      820 2023-06-11 21:54:25.000000 polygon-sdk-1.0.3/sdks/polygon_sdk/option_aggs.py
--rw-rw-rw-   0        0        0     1493 2023-06-11 21:54:25.000000 polygon-sdk-1.0.3/sdks/polygon_sdk/option_quote.py
--rw-rw-rw-   0        0        0     3079 2023-06-11 21:54:25.000000 polygon-sdk-1.0.3/sdks/polygon_sdk/option_snapshot.py
--rw-rw-rw-   0        0        0      873 2023-06-11 21:54:25.000000 polygon-sdk-1.0.3/sdks/polygon_sdk/option_trades.py
--rw-rw-rw-   0        0        0      538 2023-06-11 21:54:25.000000 polygon-sdk-1.0.3/sdks/polygon_sdk/pivot_points.py
--rw-rw-rw-   0        0        0      690 2023-06-11 21:54:25.000000 polygon-sdk-1.0.3/sdks/polygon_sdk/quote.py
--rw-rw-rw-   0        0        0      151 2023-06-11 21:54:25.000000 polygon-sdk-1.0.3/sdks/polygon_sdk/sec.py
--rw-rw-rw-   0        0        0     4192 2023-06-11 21:54:25.000000 polygon-sdk-1.0.3/sdks/polygon_sdk/snapshot.py
--rw-rw-rw-   0        0        0     1313 2023-06-11 21:54:25.000000 polygon-sdk-1.0.3/sdks/polygon_sdk/technical_conditions.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:16:36.640982 polygon-sdk-1.0.3/sdks/polygon_sdk/technicals/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:25.000000 polygon-sdk-1.0.3/sdks/polygon_sdk/technicals/__init__.py
--rw-rw-rw-   0        0        0      248 2023-06-11 21:54:25.000000 polygon-sdk-1.0.3/sdks/polygon_sdk/technicals/ema.py
--rw-rw-rw-   0        0        0      229 2023-06-11 21:54:25.000000 polygon-sdk-1.0.3/sdks/polygon_sdk/technicals/macd.py
--rw-rw-rw-   0        0        0      233 2023-06-11 21:54:25.000000 polygon-sdk-1.0.3/sdks/polygon_sdk/technicals/rsi.py
--rw-rw-rw-   0        0        0      244 2023-06-11 21:54:25.000000 polygon-sdk-1.0.3/sdks/polygon_sdk/technicals/sma.py
--rw-rw-rw-   0        0        0     3361 2023-06-13 21:44:27.000000 polygon-sdk-1.0.3/sdks/polygon_sdk/tickernews.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:16:36.641982 polygon-sdk-1.0.3/sdks/terminals/
--rw-rw-rw-   0        0        0        0 2023-06-11 21:54:25.000000 polygon-sdk-1.0.3/sdks/terminals/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:16:36.642981 polygon-sdk-1.0.3/sdks/terminals/crypto/
--rw-rw-rw-   0        0        0        0 2023-06-11 21:54:25.000000 polygon-sdk-1.0.3/sdks/terminals/crypto/__init__.py
--rw-rw-rw-   0        0        0     1672 2023-06-11 21:54:25.000000 polygon-sdk-1.0.3/sdks/terminals/crypto/menu.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:16:36.654662 polygon-sdk-1.0.3/sdks/webull_sdk/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:25.000000 polygon-sdk-1.0.3/sdks/webull_sdk/__init__.py
--rw-rw-rw-   0        0        0      882 2023-06-11 22:15:21.000000 polygon-sdk-1.0.3/sdks/webull_sdk/calendar.py
--rw-rw-rw-   0        0        0     9220 2023-06-11 22:15:21.000000 polygon-sdk-1.0.3/sdks/webull_sdk/capitalflow.py
--rw-rw-rw-   0        0        0     1152 2023-06-11 21:54:25.000000 polygon-sdk-1.0.3/sdks/webull_sdk/cost_distribution.py
--rw-rw-rw-   0        0        0     2282 2023-06-11 21:54:25.000000 polygon-sdk-1.0.3/sdks/webull_sdk/derivative_query.py
--rw-rw-rw-   0        0        0     2426 2023-06-11 22:15:21.000000 polygon-sdk-1.0.3/sdks/webull_sdk/etf_finder.py
--rw-rw-rw-   0        0        0      486 2023-06-11 21:54:25.000000 polygon-sdk-1.0.3/sdks/webull_sdk/etf_holdings.py
--rw-rw-rw-   0        0        0      987 2023-06-11 21:54:25.000000 polygon-sdk-1.0.3/sdks/webull_sdk/events.py
--rw-rw-rw-   0        0        0     7818 2023-06-11 22:15:21.000000 polygon-sdk-1.0.3/sdks/webull_sdk/financial_statement.py
--rw-rw-rw-   0        0        0     3780 2023-06-11 21:54:25.000000 polygon-sdk-1.0.3/sdks/webull_sdk/forecast.py
--rw-rw-rw-   0        0        0     1033 2023-06-11 22:15:21.000000 polygon-sdk-1.0.3/sdks/webull_sdk/institutional_holdings.py
--rw-rw-rw-   0        0        0     1156 2023-06-11 22:15:21.000000 polygon-sdk-1.0.3/sdks/webull_sdk/manage.py
--rw-rw-rw-   0        0        0      617 2023-06-11 22:15:21.000000 polygon-sdk-1.0.3/sdks/webull_sdk/news.py
--rw-rw-rw-   0        0        0      307 2023-06-11 22:15:21.000000 polygon-sdk-1.0.3/sdks/webull_sdk/shortinterest.py
--rw-rw-rw-   0        0        0     2730 2023-06-11 21:54:25.000000 polygon-sdk-1.0.3/sdks/webull_sdk/top_gainers.py
--rw-rw-rw-   0        0        0    16723 2023-06-11 22:15:21.000000 polygon-sdk-1.0.3/sdks/webull_sdk/top_options.py
--rw-rw-rw-   0        0        0     5556 2023-06-11 22:15:21.000000 polygon-sdk-1.0.3/sdks/webull_sdk/webull_data.py
--rw-rw-rw-   0        0        0    43603 2023-06-13 19:11:45.000000 polygon-sdk-1.0.3/sdks/webull_sdk/webull_sdk.py
--rw-rw-rw-   0        0        0       42 2023-06-13 22:16:36.656661 polygon-sdk-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      856 2023-06-13 22:16:10.000000 polygon-sdk-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:16:36.655661 polygon-sdk-1.0.3/templates/
--rw-rw-rw-   0        0        0        0 2023-06-11 23:48:46.000000 polygon-sdk-1.0.3/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:22:29.565295 polygon-sdk-1.0.5/
+-rw-rw-rw-   0        0        0     2507 2023-06-13 22:22:29.565295 polygon-sdk-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1929 2023-06-12 00:29:12.000000 polygon-sdk-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 22:22:29.468328 polygon-sdk-1.0.5/polygon_sdk/
+-rw-rw-rw-   0        0        0        0 2023-06-11 22:28:58.000000 polygon-sdk-1.0.5/polygon_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:22:29.483326 polygon-sdk-1.0.5/polygon_sdk/_discord/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 polygon-sdk-1.0.5/polygon_sdk/_discord/__init__.py
+-rw-rw-rw-   0        0        0     7983 2023-06-11 21:54:23.000000 polygon-sdk-1.0.5/polygon_sdk/_discord/discord_stock_example.py
+-rw-rw-rw-   0        0        0    44936 2023-06-11 21:54:23.000000 polygon-sdk-1.0.5/polygon_sdk/_discord/discord_stock_market.py
+-rw-rw-rw-   0        0        0    16306 2023-06-11 21:54:23.000000 polygon-sdk-1.0.5/polygon_sdk/_discord/embeddings.py
+-rw-rw-rw-   0        0        0      581 2023-06-11 21:54:23.000000 polygon-sdk-1.0.5/polygon_sdk/_discord/emojis.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:22:29.485326 polygon-sdk-1.0.5/polygon_sdk/_discord/hooks/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 polygon-sdk-1.0.5/polygon_sdk/_discord/hooks/__init__.py
+-rw-rw-rw-   0        0        0     1594 2023-06-11 21:54:23.000000 polygon-sdk-1.0.5/polygon_sdk/_discord/hooks/channel_webhooks.py
+-rw-rw-rw-   0        0        0    10521 2023-06-11 21:54:23.000000 polygon-sdk-1.0.5/polygon_sdk/_discord/hooks/hook_dicts.py
+-rw-rw-rw-   0        0        0     5462 2023-06-11 21:54:23.000000 polygon-sdk-1.0.5/polygon_sdk/_discord/hooks/send_webhook.py
+-rw-rw-rw-   0        0        0    33594 2023-06-11 21:54:23.000000 polygon-sdk-1.0.5/polygon_sdk/_discord/live_discord.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:22:29.486326 polygon-sdk-1.0.5/polygon_sdk/_discord/selectmenus/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 polygon-sdk-1.0.5/polygon_sdk/_discord/selectmenus/__init__.py
+-rw-rw-rw-   0        0        0    33209 2023-06-11 22:20:44.000000 polygon-sdk-1.0.5/polygon_sdk/_discord/selectmenus/mainselect.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:22:29.488326 polygon-sdk-1.0.5/polygon_sdk/_discord/views/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 polygon-sdk-1.0.5/polygon_sdk/_discord/views/__init__.py
+-rw-rw-rw-   0        0        0     1640 2023-06-11 21:54:23.000000 polygon-sdk-1.0.5/polygon_sdk/_discord/views/mainview.py
+-rw-rw-rw-   0        0        0     3792 2023-06-11 21:54:23.000000 polygon-sdk-1.0.5/polygon_sdk/_discord/views/menus.py
+-rw-rw-rw-   0        0        0     7502 2023-06-11 21:54:23.000000 polygon-sdk-1.0.5/polygon_sdk/_discord/webhook_creation.py
+-rw-rw-rw-   0        0        0     3370 2023-06-13 21:55:31.000000 polygon-sdk-1.0.5/polygon_sdk/app.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:22:29.491326 polygon-sdk-1.0.5/polygon_sdk/bot/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 polygon-sdk-1.0.5/polygon_sdk/bot/__init__.py
+-rw-rw-rw-   0        0        0    13209 2023-06-11 22:18:58.000000 polygon-sdk-1.0.5/polygon_sdk/bot/autocomp.py
+-rw-rw-rw-   0        0        0     6919 2023-06-11 22:19:59.000000 polygon-sdk-1.0.5/polygon_sdk/bot/discord_emojis.py
+-rw-rw-rw-   0        0        0        0 2023-06-11 21:54:23.000000 polygon-sdk-1.0.5/polygon_sdk/bot/helpers.py
+-rw-rw-rw-   0        0        0     1279 2023-06-11 22:22:28.000000 polygon-sdk-1.0.5/polygon_sdk/bot/main.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:22:29.492545 polygon-sdk-1.0.5/polygon_sdk/bot/utils/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 polygon-sdk-1.0.5/polygon_sdk/bot/utils/__init__.py
+-rw-rw-rw-   0        0        0   101924 2023-06-11 22:19:10.000000 polygon-sdk-1.0.5/polygon_sdk/bot/utils/lists_and_dicts.py
+-rw-rw-rw-   0        0        0   199781 2023-06-11 22:17:58.000000 polygon-sdk-1.0.5/polygon_sdk/bot/utils/webull_tickers.py
+-rw-rw-rw-   0        0        0     2958 2023-06-13 13:19:27.000000 polygon-sdk-1.0.5/polygon_sdk/cfg.py
+-rw-rw-rw-   0        0        0     2264 2023-06-12 01:16:14.000000 polygon-sdk-1.0.5/polygon_sdk/example.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:22:29.492545 polygon-sdk-1.0.5/polygon_sdk/examples/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 polygon-sdk-1.0.5/polygon_sdk/examples/__init__.py
+-rw-rw-rw-   0        0        0     5940 2023-06-11 21:54:23.000000 polygon-sdk-1.0.5/polygon_sdk/examples/all_attributes.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:22:29.492545 polygon-sdk-1.0.5/polygon_sdk/examples/realtime_markets/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 polygon-sdk-1.0.5/polygon_sdk/examples/realtime_markets/__init__.py
+-rw-rw-rw-   0        0        0     2479 2023-06-11 21:54:23.000000 polygon-sdk-1.0.5/polygon_sdk/examples/realtime_markets/crypto_market.py
+-rw-rw-rw-   0        0        0    44945 2023-06-11 21:54:23.000000 polygon-sdk-1.0.5/polygon_sdk/examples/realtime_markets/discord_market.py
+-rw-rw-rw-   0        0        0      922 2023-06-11 21:54:23.000000 polygon-sdk-1.0.5/polygon_sdk/examples/realtime_markets/forex_market.py
+-rw-rw-rw-   0        0        0      776 2023-06-11 21:54:23.000000 polygon-sdk-1.0.5/polygon_sdk/examples/realtime_markets/indices_market.py
+-rw-rw-rw-   0        0        0      989 2023-06-11 21:54:23.000000 polygon-sdk-1.0.5/polygon_sdk/examples/realtime_markets/options_market.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:22:29.492545 polygon-sdk-1.0.5/polygon_sdk/examples/simulated_markets/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 polygon-sdk-1.0.5/polygon_sdk/examples/simulated_markets/__init__.py
+-rw-rw-rw-   0        0        0      688 2023-06-11 21:54:23.000000 polygon-sdk-1.0.5/polygon_sdk/examples/simulated_markets/helpers.py
+-rw-rw-rw-   0        0        0     5115 2023-06-11 22:19:16.000000 polygon-sdk-1.0.5/polygon_sdk/examples/simulated_markets/mock_discord.py
+-rw-rw-rw-   0        0        0     1951 2023-06-12 01:17:16.000000 polygon-sdk-1.0.5/polygon_sdk/examples/simulated_markets/mock_market.py
+-rw-rw-rw-   0        0        0     1551 2023-06-12 01:18:49.000000 polygon-sdk-1.0.5/polygon_sdk/examples/simulated_markets/mock_options_market.py
+-rw-rw-rw-   0        0        0    14931 2023-06-11 21:54:23.000000 polygon-sdk-1.0.5/polygon_sdk/examples/webull_data.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:22:29.492545 polygon-sdk-1.0.5/polygon_sdk/funcs/
+-rw-rw-rw-   0        0        0        0 2023-06-11 22:29:36.000000 polygon-sdk-1.0.5/polygon_sdk/funcs/__init__.py
+-rw-rw-rw-   0        0        0    36181 2023-06-11 22:44:36.000000 polygon-sdk-1.0.5/polygon_sdk/funcs/get_data.py
+-rw-rw-rw-   0        0        0      600 2023-06-11 21:54:23.000000 polygon-sdk-1.0.5/polygon_sdk/get_latest_crypto_data.py
+-rw-rw-rw-   0        0        0      585 2023-06-11 21:54:23.000000 polygon-sdk-1.0.5/polygon_sdk/get_latest_forex_data.py
+-rw-rw-rw-   0        0        0      446 2023-06-11 21:54:23.000000 polygon-sdk-1.0.5/polygon_sdk/get_latest_indices_data.py
+-rw-rw-rw-   0        0        0      762 2023-06-11 21:54:23.000000 polygon-sdk-1.0.5/polygon_sdk/get_latest_options_data.py
+-rw-rw-rw-   0        0        0      598 2023-06-12 00:39:12.000000 polygon-sdk-1.0.5/polygon_sdk/get_latest_ticker_data.py
+-rw-rw-rw-   0        0        0      235 2023-06-11 21:54:23.000000 polygon-sdk-1.0.5/polygon_sdk/get_webull_data.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:22:29.492545 polygon-sdk-1.0.5/polygon_sdk/sdks/
+-rw-rw-rw-   0        0        0        0 2023-06-11 22:15:21.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:22:29.492545 polygon-sdk-1.0.5/polygon_sdk/sdks/discord_sdk/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/discord_sdk/__init__.py
+-rw-rw-rw-   0        0        0       53 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/discord_sdk/channel_ids.py
+-rw-rw-rw-   0        0        0     4497 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/discord_sdk/discord_sdk.py
+-rw-rw-rw-   0        0        0     2157 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/discord_sdk/searching.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:22:29.521782 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/__init__.py
+-rw-rw-rw-   0        0        0     6184 2023-06-12 00:26:46.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/all_attributes.py
+-rw-rw-rw-   0        0        0      517 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/bollinger_bands.py
+-rw-rw-rw-   0        0        0      706 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/create_option_symbol.py
+-rw-rw-rw-   0        0        0     1664 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/ema.py
+-rw-rw-rw-   0        0        0      910 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/fetch_entire_chain.py
+-rw-rw-rw-   0        0        0      649 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/find_gaps.py
+-rw-rw-rw-   0        0        0      823 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/get_all_options_data.py
+-rw-rw-rw-   0        0        0     2399 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/get_ema.py
+-rw-rw-rw-   0        0        0      600 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/get_latest_crypto_data.py
+-rw-rw-rw-   0        0        0      585 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/get_latest_forex_data.py
+-rw-rw-rw-   0        0        0      446 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/get_latest_indices_data.py
+-rw-rw-rw-   0        0        0      644 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/get_latest_ticker_data.py
+-rw-rw-rw-   0        0        0     3161 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/get_macd.py
+-rw-rw-rw-   0        0        0      582 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/get_pivot_points.py
+-rw-rw-rw-   0        0        0     2051 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/get_rsi.py
+-rw-rw-rw-   0        0        0     2172 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/get_sma.py
+-rw-rw-rw-   0        0        0     1796 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/latest_news.py
+-rw-rw-rw-   0        0        0     1625 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/option_quote.py
+-rw-rw-rw-   0        0        0     2408 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/option_trades.py
+-rw-rw-rw-   0        0        0     1408 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/plot_aggs.py
+-rw-rw-rw-   0        0        0      796 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/plot_macd.py
+-rw-rw-rw-   0        0        0     1797 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/plot_option_aggs.py
+-rw-rw-rw-   0        0        0      487 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/rate_of_change.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:22:29.526786 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/realtime_markets/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/realtime_markets/__init__.py
+-rw-rw-rw-   0        0        0     2479 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/realtime_markets/crypto_market.py
+-rw-rw-rw-   0        0        0      922 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/realtime_markets/forex_market.py
+-rw-rw-rw-   0        0        0      776 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/realtime_markets/indices_market.py
+-rw-rw-rw-   0        0        0      989 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/realtime_markets/options_market.py
+-rw-rw-rw-   0        0        0     4837 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/scanner_example.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:22:29.529785 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/simulated_markets/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/simulated_markets/__init__.py
+-rw-rw-rw-   0        0        0      688 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/simulated_markets/helpers.py
+-rw-rw-rw-   0        0        0     2606 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/simulated_markets/mock_market.py
+-rw-rw-rw-   0        0        0     1806 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/simulated_markets/mock_options_market.py
+-rw-rw-rw-   0        0        0     2116 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/stock_aggregates.py
+-rw-rw-rw-   0        0        0     1189 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/examples/support_resistance.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:22:29.531786 polygon-sdk-1.0.5/polygon_sdk/sdks/fudstop_sdk/
+-rw-rw-rw-   0        0        0        1 2023-06-12 00:06:40.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/fudstop_sdk/__init__.py
+-rw-rw-rw-   0        0        0     2909 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/fudstop_sdk/fudstop_sdk.py
+-rw-rw-rw-   0        0        0     1661 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/fudstop_sdk/gaps.py
+-rw-rw-rw-   0        0        0      427 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/fudstop_sdk/option_vol_totals.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:22:29.533786 polygon-sdk-1.0.5/polygon_sdk/sdks/helpers/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/helpers/__init__.py
+-rw-rw-rw-   0        0        0     2001 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/helpers/conditions.py
+-rw-rw-rw-   0        0        0        2 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/helpers/get_cik.py
+-rw-rw-rw-   0        0        0     5442 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/helpers/helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:22:29.535786 polygon-sdk-1.0.5/polygon_sdk/sdks/models/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/models/__init__.py
+-rw-rw-rw-   0        0        0      488 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/models/common.py
+-rw-rw-rw-   0        0        0     5097 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/models/maps.py
+-rw-rw-rw-   0        0        0    13078 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/models/test_events.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:22:29.550295 polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/__init__.py
+-rw-rw-rw-   0        0        0     1265 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/aggregates.py
+-rw-rw-rw-   0        0        0    29379 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/async_options_sdk.py
+-rw-rw-rw-   0        0        0    52775 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/async_polygon_sdk.py
+-rw-rw-rw-   0        0        0     1135 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/company_info.py
+-rw-rw-rw-   0        0        0      703 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/daily_open_close.py
+-rw-rw-rw-   0        0        0    15043 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/financials.py
+-rw-rw-rw-   0        0        0     6644 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/forex_crypto.py
+-rw-rw-rw-   0        0        0     8957 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/get_all_options.py
+-rw-rw-rw-   0        0        0     1131 2023-06-11 21:54:24.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/indices_snapshot.py
+-rw-rw-rw-   0        0        0      823 2023-06-11 21:54:25.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/logo.py
+-rw-rw-rw-   0        0        0    27900 2023-06-11 21:54:25.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/mapping_dicts.py
+-rw-rw-rw-   0        0        0      782 2023-06-11 21:54:25.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/models.py
+-rw-rw-rw-   0        0        0      819 2023-06-11 21:54:25.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/news.py
+-rw-rw-rw-   0        0        0      820 2023-06-11 21:54:25.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/option_aggs.py
+-rw-rw-rw-   0        0        0     1493 2023-06-11 21:54:25.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/option_quote.py
+-rw-rw-rw-   0        0        0     3079 2023-06-11 21:54:25.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/option_snapshot.py
+-rw-rw-rw-   0        0        0      873 2023-06-11 21:54:25.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/option_trades.py
+-rw-rw-rw-   0        0        0      538 2023-06-11 21:54:25.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/pivot_points.py
+-rw-rw-rw-   0        0        0      690 2023-06-11 21:54:25.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/quote.py
+-rw-rw-rw-   0        0        0      151 2023-06-11 21:54:25.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/sec.py
+-rw-rw-rw-   0        0        0     4192 2023-06-11 21:54:25.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/snapshot.py
+-rw-rw-rw-   0        0        0     1313 2023-06-11 21:54:25.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/technical_conditions.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:22:29.552294 polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/technicals/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:25.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/technicals/__init__.py
+-rw-rw-rw-   0        0        0      248 2023-06-11 21:54:25.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/technicals/ema.py
+-rw-rw-rw-   0        0        0      229 2023-06-11 21:54:25.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/technicals/macd.py
+-rw-rw-rw-   0        0        0      233 2023-06-11 21:54:25.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/technicals/rsi.py
+-rw-rw-rw-   0        0        0      244 2023-06-11 21:54:25.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/technicals/sma.py
+-rw-rw-rw-   0        0        0     3361 2023-06-13 21:44:27.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/tickernews.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:22:29.553294 polygon-sdk-1.0.5/polygon_sdk/sdks/terminals/
+-rw-rw-rw-   0        0        0        0 2023-06-11 21:54:25.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/terminals/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:22:29.554294 polygon-sdk-1.0.5/polygon_sdk/sdks/terminals/crypto/
+-rw-rw-rw-   0        0        0        0 2023-06-11 21:54:25.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/terminals/crypto/__init__.py
+-rw-rw-rw-   0        0        0     1672 2023-06-11 21:54:25.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/terminals/crypto/menu.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:22:29.564294 polygon-sdk-1.0.5/polygon_sdk/sdks/webull_sdk/
+-rw-rw-rw-   0        0        0        1 2023-06-11 21:54:25.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/webull_sdk/__init__.py
+-rw-rw-rw-   0        0        0      882 2023-06-11 22:15:21.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/webull_sdk/calendar.py
+-rw-rw-rw-   0        0        0     9220 2023-06-11 22:15:21.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/webull_sdk/capitalflow.py
+-rw-rw-rw-   0        0        0     1152 2023-06-11 21:54:25.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/webull_sdk/cost_distribution.py
+-rw-rw-rw-   0        0        0     2282 2023-06-11 21:54:25.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/webull_sdk/derivative_query.py
+-rw-rw-rw-   0        0        0     2426 2023-06-11 22:15:21.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/webull_sdk/etf_finder.py
+-rw-rw-rw-   0        0        0      486 2023-06-11 21:54:25.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/webull_sdk/etf_holdings.py
+-rw-rw-rw-   0        0        0      987 2023-06-11 21:54:25.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/webull_sdk/events.py
+-rw-rw-rw-   0        0        0     7818 2023-06-11 22:15:21.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/webull_sdk/financial_statement.py
+-rw-rw-rw-   0        0        0     3780 2023-06-11 21:54:25.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/webull_sdk/forecast.py
+-rw-rw-rw-   0        0        0     1033 2023-06-11 22:15:21.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/webull_sdk/institutional_holdings.py
+-rw-rw-rw-   0        0        0     1156 2023-06-11 22:15:21.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/webull_sdk/manage.py
+-rw-rw-rw-   0        0        0      617 2023-06-11 22:15:21.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/webull_sdk/news.py
+-rw-rw-rw-   0        0        0      307 2023-06-11 22:15:21.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/webull_sdk/shortinterest.py
+-rw-rw-rw-   0        0        0     2730 2023-06-11 21:54:25.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/webull_sdk/top_gainers.py
+-rw-rw-rw-   0        0        0    16723 2023-06-11 22:15:21.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/webull_sdk/top_options.py
+-rw-rw-rw-   0        0        0     5556 2023-06-11 22:15:21.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/webull_sdk/webull_data.py
+-rw-rw-rw-   0        0        0    43603 2023-06-13 19:11:45.000000 polygon-sdk-1.0.5/polygon_sdk/sdks/webull_sdk/webull_sdk.py
+-rw-rw-rw-   0        0        0     1052 2023-06-12 01:22:03.000000 polygon-sdk-1.0.5/polygon_sdk/sec_filings.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:22:29.564294 polygon-sdk-1.0.5/polygon_sdk/templates/
+-rw-rw-rw-   0        0        0        0 2023-06-11 23:48:46.000000 polygon-sdk-1.0.5/polygon_sdk/templates/__init__.py
+-rw-rw-rw-   0        0        0     2265 2023-06-13 22:20:14.000000 polygon-sdk-1.0.5/polygon_sdk/test.py
+drwxrwxrwx   0        0        0        0 2023-06-13 22:22:29.478326 polygon-sdk-1.0.5/polygon_sdk.egg-info/
+-rw-rw-rw-   0        0        0     2507 2023-06-13 22:22:29.000000 polygon-sdk-1.0.5/polygon_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6798 2023-06-13 22:22:29.000000 polygon-sdk-1.0.5/polygon_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 22:22:29.000000 polygon-sdk-1.0.5/polygon_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-13 22:22:29.000000 polygon-sdk-1.0.5/polygon_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 22:22:29.565295 polygon-sdk-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      856 2023-06-13 22:19:59.000000 polygon-sdk-1.0.5/setup.py
```

### Comparing `polygon-sdk-1.0.3/PKG-INFO` & `polygon-sdk-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polygon-sdk
-Version: 1.0.3
+Version: 1.0.5
 Summary: Analyze, query, and fetch market data utilizing Polygon.io's suite of services for simulated and real-time market data analysis.
 Home-page: https://github.com/chuckdustin12/polygonsdk/
 Author: Chuck
 Author-email: chuckdustin12@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `polygon-sdk-1.0.3/README.md` & `polygon-sdk-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/_discord/discord_stock_example.py` & `polygon-sdk-1.0.5/polygon_sdk/_discord/discord_stock_example.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/_discord/discord_stock_market.py` & `polygon-sdk-1.0.5/polygon_sdk/_discord/discord_stock_market.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/_discord/embeddings.py` & `polygon-sdk-1.0.5/polygon_sdk/_discord/embeddings.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/_discord/emojis.py` & `polygon-sdk-1.0.5/polygon_sdk/_discord/emojis.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/_discord/hooks/channel_webhooks.py` & `polygon-sdk-1.0.5/polygon_sdk/_discord/hooks/channel_webhooks.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/_discord/hooks/hook_dicts.py` & `polygon-sdk-1.0.5/polygon_sdk/_discord/hooks/hook_dicts.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/_discord/hooks/send_webhook.py` & `polygon-sdk-1.0.5/polygon_sdk/_discord/hooks/send_webhook.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/_discord/live_discord.py` & `polygon-sdk-1.0.5/polygon_sdk/_discord/live_discord.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/_discord/selectmenus/mainselect.py` & `polygon-sdk-1.0.5/polygon_sdk/_discord/selectmenus/mainselect.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/_discord/views/mainview.py` & `polygon-sdk-1.0.5/polygon_sdk/_discord/views/mainview.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/_discord/views/menus.py` & `polygon-sdk-1.0.5/polygon_sdk/_discord/views/menus.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/_discord/webhook_creation.py` & `polygon-sdk-1.0.5/polygon_sdk/_discord/webhook_creation.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/bot/autocomp.py` & `polygon-sdk-1.0.5/polygon_sdk/bot/autocomp.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/bot/discord_emojis.py` & `polygon-sdk-1.0.5/polygon_sdk/bot/discord_emojis.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/bot/main.py` & `polygon-sdk-1.0.5/polygon_sdk/bot/main.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/bot/utils/lists_and_dicts.py` & `polygon-sdk-1.0.5/polygon_sdk/bot/utils/lists_and_dicts.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/bot/utils/webull_tickers.py` & `polygon-sdk-1.0.5/polygon_sdk/bot/utils/webull_tickers.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/examples/all_attributes.py` & `polygon-sdk-1.0.5/polygon_sdk/examples/all_attributes.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/examples/realtime_markets/crypto_market.py` & `polygon-sdk-1.0.5/polygon_sdk/examples/realtime_markets/crypto_market.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/examples/realtime_markets/discord_market.py` & `polygon-sdk-1.0.5/polygon_sdk/examples/realtime_markets/discord_market.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/examples/realtime_markets/forex_market.py` & `polygon-sdk-1.0.5/polygon_sdk/examples/realtime_markets/forex_market.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/examples/realtime_markets/indices_market.py` & `polygon-sdk-1.0.5/polygon_sdk/examples/realtime_markets/indices_market.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/examples/realtime_markets/options_market.py` & `polygon-sdk-1.0.5/polygon_sdk/examples/realtime_markets/options_market.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/examples/simulated_markets/helpers.py` & `polygon-sdk-1.0.5/polygon_sdk/examples/simulated_markets/helpers.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/examples/simulated_markets/mock_discord.py` & `polygon-sdk-1.0.5/polygon_sdk/examples/simulated_markets/mock_discord.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/examples/simulated_markets/mock_market.py` & `polygon-sdk-1.0.5/polygon_sdk/examples/simulated_markets/mock_market.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/examples/simulated_markets/mock_options_market.py` & `polygon-sdk-1.0.5/polygon_sdk/examples/simulated_markets/mock_options_market.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/examples/webull_data.py` & `polygon-sdk-1.0.5/polygon_sdk/examples/webull_data.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/funcs/get_data.py` & `polygon-sdk-1.0.5/polygon_sdk/funcs/get_data.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/polygon_sdk.egg-info/PKG-INFO` & `polygon-sdk-1.0.5/polygon_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polygon-sdk
-Version: 1.0.3
+Version: 1.0.5
 Summary: Analyze, query, and fetch market data utilizing Polygon.io's suite of services for simulated and real-time market data analysis.
 Home-page: https://github.com/chuckdustin12/polygonsdk/
 Author: Chuck
 Author-email: chuckdustin12@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `polygon-sdk-1.0.3/sdks/discord_sdk/discord_sdk.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/discord_sdk/discord_sdk.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/discord_sdk/searching.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/discord_sdk/searching.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/examples/all_attributes.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/examples/all_attributes.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/examples/bollinger_bands.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/examples/bollinger_bands.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/examples/create_option_symbol.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/examples/create_option_symbol.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/examples/ema.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/examples/ema.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/examples/fetch_entire_chain.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/examples/fetch_entire_chain.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/examples/find_gaps.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/examples/find_gaps.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/examples/get_all_options_data.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/examples/get_all_options_data.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/examples/get_ema.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/examples/get_ema.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/examples/get_latest_crypto_data.py` & `polygon-sdk-1.0.5/polygon_sdk/get_latest_crypto_data.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/examples/get_latest_forex_data.py` & `polygon-sdk-1.0.5/polygon_sdk/get_latest_forex_data.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/examples/get_latest_ticker_data.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/examples/get_latest_ticker_data.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/examples/get_macd.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/examples/get_macd.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/examples/get_pivot_points.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/examples/get_pivot_points.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/examples/get_rsi.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/examples/get_rsi.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/examples/get_sma.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/examples/get_sma.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/examples/latest_news.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/examples/latest_news.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/examples/option_quote.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/examples/option_quote.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/examples/option_trades.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/examples/option_trades.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/examples/plot_aggs.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/examples/plot_aggs.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/examples/plot_macd.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/examples/plot_macd.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/examples/plot_option_aggs.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/examples/plot_option_aggs.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/examples/realtime_markets/crypto_market.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/examples/realtime_markets/crypto_market.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/examples/realtime_markets/forex_market.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/examples/realtime_markets/forex_market.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/examples/realtime_markets/indices_market.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/examples/realtime_markets/indices_market.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/examples/realtime_markets/options_market.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/examples/realtime_markets/options_market.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/examples/scanner_example.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/examples/scanner_example.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/examples/simulated_markets/helpers.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/examples/simulated_markets/helpers.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/examples/simulated_markets/mock_market.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/examples/simulated_markets/mock_market.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/examples/simulated_markets/mock_options_market.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/examples/simulated_markets/mock_options_market.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/examples/stock_aggregates.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/examples/stock_aggregates.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/examples/support_resistance.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/examples/support_resistance.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/fudstop_sdk/fudstop_sdk.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/fudstop_sdk/fudstop_sdk.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/fudstop_sdk/gaps.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/fudstop_sdk/gaps.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/helpers/conditions.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/helpers/conditions.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/helpers/helpers.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/models/maps.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/models/maps.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/models/test_events.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/models/test_events.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/polygon_sdk/aggregates.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/aggregates.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/polygon_sdk/async_options_sdk.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/async_options_sdk.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/polygon_sdk/async_polygon_sdk.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/async_polygon_sdk.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/polygon_sdk/company_info.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/company_info.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/polygon_sdk/daily_open_close.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/daily_open_close.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/polygon_sdk/financials.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/financials.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/polygon_sdk/forex_crypto.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/forex_crypto.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/polygon_sdk/get_all_options.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/get_all_options.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/polygon_sdk/indices_snapshot.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/indices_snapshot.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/polygon_sdk/logo.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/logo.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/polygon_sdk/mapping_dicts.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/mapping_dicts.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/polygon_sdk/models.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/models.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/polygon_sdk/news.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/news.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/polygon_sdk/option_aggs.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/option_aggs.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/polygon_sdk/option_quote.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/option_quote.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/polygon_sdk/option_snapshot.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/option_snapshot.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/polygon_sdk/option_trades.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/option_trades.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/polygon_sdk/pivot_points.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/pivot_points.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/polygon_sdk/quote.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/quote.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/polygon_sdk/snapshot.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/snapshot.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/polygon_sdk/technical_conditions.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/technical_conditions.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/polygon_sdk/tickernews.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/polygon_sdk/tickernews.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/terminals/crypto/menu.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/terminals/crypto/menu.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/webull_sdk/calendar.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/webull_sdk/calendar.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/webull_sdk/capitalflow.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/webull_sdk/capitalflow.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/webull_sdk/cost_distribution.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/webull_sdk/cost_distribution.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/webull_sdk/derivative_query.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/webull_sdk/derivative_query.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/webull_sdk/etf_finder.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/webull_sdk/etf_finder.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/webull_sdk/events.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/webull_sdk/events.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/webull_sdk/financial_statement.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/webull_sdk/financial_statement.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/webull_sdk/forecast.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/webull_sdk/forecast.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/webull_sdk/institutional_holdings.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/webull_sdk/institutional_holdings.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/webull_sdk/manage.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/webull_sdk/manage.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/webull_sdk/news.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/webull_sdk/news.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/webull_sdk/top_gainers.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/webull_sdk/top_gainers.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/webull_sdk/top_options.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/webull_sdk/top_options.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/webull_sdk/webull_data.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/webull_sdk/webull_data.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/sdks/webull_sdk/webull_sdk.py` & `polygon-sdk-1.0.5/polygon_sdk/sdks/webull_sdk/webull_sdk.py`

 * *Files identical despite different names*

### Comparing `polygon-sdk-1.0.3/setup.py` & `polygon-sdk-1.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="polygon-sdk",
-    version="1.0.3",
+    version="1.0.5",
     author="Chuck",
     author_email="chuckdustin12@gmail.com",
     description="Analyze, query, and fetch market data utilizing Polygon.io's suite of services for simulated and real-time market data analysis.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/chuckdustin12/polygonsdk/",
     packages=setuptools.find_packages(),
```

