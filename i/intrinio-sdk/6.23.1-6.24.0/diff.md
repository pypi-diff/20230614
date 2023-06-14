# Comparing `tmp/intrinio-sdk-6.23.1.tar.gz` & `tmp/intrinio-sdk-6.24.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/intrinio-sdk-6.23.1.tar", last modified: Tue Mar 28 02:47:26 2023, max compression
+gzip compressed data, was "dist/intrinio-sdk-6.24.0.tar", last modified: Wed Jun 14 14:28:29 2023, max compression
```

## Comparing `intrinio-sdk-6.23.1.tar` & `intrinio-sdk-6.24.0.tar`

### file list

```diff
@@ -1,590 +1,590 @@
-drwxr-xr-x   0 shawn      (503) staff       (20)        0 2023-03-28 02:47:26.000000 intrinio-sdk-6.23.1/
-drwxr-xr-x   0 shawn      (503) staff       (20)        0 2023-03-28 02:47:26.000000 intrinio-sdk-6.23.1/intrinio_sdk/
--rw-r--r--   0 shawn      (503) staff       (20)     8604 2023-03-28 00:46:17.000000 intrinio-sdk-6.23.1/intrinio_sdk/configuration.py
--rw-r--r--   0 shawn      (503) staff       (20)    13819 2023-03-28 00:46:17.000000 intrinio-sdk-6.23.1/intrinio_sdk/rest.py
--rw-r--r--   0 shawn      (503) staff       (20)    25620 2023-03-28 00:46:17.000000 intrinio-sdk-6.23.1/intrinio_sdk/__init__.py
-drwxr-xr-x   0 shawn      (503) staff       (20)        0 2023-03-28 02:47:26.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/
--rw-r--r--   0 shawn      (503) staff       (20)    26373 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/zacks_target_price_consensus.py
--rw-r--r--   0 shawn      (503) staff       (20)     9009 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_zacks_sales_surprises.py
--rw-r--r--   0 shawn      (503) staff       (20)     6524 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/detrended_price_oscillator_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)    40363 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/zacks_sales_surprise_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     6602 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_options.py
--rw-r--r--   0 shawn      (503) staff       (20)     6656 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_municipalities.py
--rw-r--r--   0 shawn      (503) staff       (20)    10646 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_williams_r.py
--rw-r--r--   0 shawn      (503) staff       (20)     7658 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/forex_currency.py
--rw-r--r--   0 shawn      (503) staff       (20)    32532 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/zacks_institutional_holding_company_detail.py
--rw-r--r--   0 shawn      (503) staff       (20)    10844 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_vortex_indicator.py
--rw-r--r--   0 shawn      (503) staff       (20)    10910 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_awesome_oscillator.py
--rw-r--r--   0 shawn      (503) staff       (20)     4570 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_securities_search.py
--rw-r--r--   0 shawn      (503) staff       (20)     8175 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_company_filings.py
--rw-r--r--   0 shawn      (503) staff       (20)     6593 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_filing_notes.py
--rw-r--r--   0 shawn      (503) staff       (20)     6229 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/williams_r_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     7946 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_options_stats_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)    22943 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/security_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)    14290 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/stock_price_adjustment.py
--rw-r--r--   0 shawn      (503) staff       (20)     4691 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_options_prices_batch_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)     4746 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_options_chain.py
--rw-r--r--   0 shawn      (503) staff       (20)     8872 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_standardized_financials.py
--rw-r--r--   0 shawn      (503) staff       (20)    19333 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/stock_market_index_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     8463 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_sic_index_historical_data.py
--rw-r--r--   0 shawn      (503) staff       (20)     8068 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_company_news.py
--rw-r--r--   0 shawn      (503) staff       (20)    24031 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/option_unusual_trade.py
--rw-r--r--   0 shawn      (503) staff       (20)     4354 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_data_tags_search.py
--rw-r--r--   0 shawn      (503) staff       (20)    32022 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/institutional_holding.py
--rw-r--r--   0 shawn      (503) staff       (20)     4539 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_company_recognize.py
--rw-r--r--   0 shawn      (503) staff       (20)     4571 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_economic_indices_search.py
--rw-r--r--   0 shawn      (503) staff       (20)    18849 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/zacks_analyst_rating_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)    79809 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/etf_stats.py
--rw-r--r--   0 shawn      (503) staff       (20)     6357 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/standardized_financials_dimension.py
--rw-r--r--   0 shawn      (503) staff       (20)    57040 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/zacks_long_term_growth_rate.py
--rw-r--r--   0 shawn      (503) staff       (20)     8325 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_company_securities.py
--rw-r--r--   0 shawn      (503) staff       (20)    70186 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/company.py
--rw-r--r--   0 shawn      (503) staff       (20)     7058 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_zacks_eps_growth_rates.py
--rw-r--r--   0 shawn      (503) staff       (20)    12984 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/company_news.py
--rw-r--r--   0 shawn      (503) staff       (20)    23120 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/etf_analytics.py
--rw-r--r--   0 shawn      (503) staff       (20)     8401 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/reported_financial.py
--rw-r--r--   0 shawn      (503) staff       (20)    37102 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/municipality.py
--rw-r--r--   0 shawn      (503) staff       (20)    21150 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/company_filing.py
--rw-r--r--   0 shawn      (503) staff       (20)    14903 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/company_shares_outstanding.py
--rw-r--r--   0 shawn      (503) staff       (20)     6794 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_zacks_analyst_ratings.py
--rw-r--r--   0 shawn      (503) staff       (20)     4642 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_filing_notes_search.py
--rw-r--r--   0 shawn      (503) staff       (20)     6244 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/force_index_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     8641 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_economic_index_historical_data.py
--rw-r--r--   0 shawn      (503) staff       (20)     6470 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/commodity_channel_index_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     9762 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_company_answers.py
--rw-r--r--   0 shawn      (503) staff       (20)     7063 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_zacks_eps_surprises.py
--rw-r--r--   0 shawn      (503) staff       (20)     8528 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_company_historical_data.py
--rw-r--r--   0 shawn      (503) staff       (20)    16762 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/option_interval_mover.py
--rw-r--r--   0 shawn      (503) staff       (20)    11274 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/moving_average_convergence_divergence_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     8244 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_forex_prices.py
--rw-r--r--   0 shawn      (503) staff       (20)     4894 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_options_chain_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)     6482 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/zacks_institutional_holding_owner_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)    14640 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/option.py
--rw-r--r--   0 shawn      (503) staff       (20)    40823 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/stock_price_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)    19534 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/filing_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)    19707 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/forex_price.py
--rw-r--r--   0 shawn      (503) staff       (20)    11154 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_volume_weighted_average_price.py
--rw-r--r--   0 shawn      (503) staff       (20)    23701 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/zacks_analyst_rating_snapshot.py
--rw-r--r--   0 shawn      (503) staff       (20)    10878 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_ichimoku_kinko_hyo.py
--rw-r--r--   0 shawn      (503) staff       (20)     6465 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/volume_weighted_average_price_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     5890 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/option_chain_eod.py
--rw-r--r--   0 shawn      (503) staff       (20)     6050 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/bulk_download_links.py
--rw-r--r--   0 shawn      (503) staff       (20)    10878 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_volume_price_trend.py
--rw-r--r--   0 shawn      (503) staff       (20)    37768 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/etf_holding.py
--rw-r--r--   0 shawn      (503) staff       (20)     6434 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/simple_moving_average_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     4823 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_options_unusual_activity.py
--rw-r--r--   0 shawn      (503) staff       (20)     8432 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/zacks_institutional_holding_company_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     9138 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_stock_exchange_securities.py
--rw-r--r--   0 shawn      (503) staff       (20)     9875 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_stock_exchange_stock_price_adjustments.py
--rw-r--r--   0 shawn      (503) staff       (20)    10811 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_keltner_channel.py
--rw-r--r--   0 shawn      (503) staff       (20)     8931 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_stock_prices.py
--rw-r--r--   0 shawn      (503) staff       (20)    11009 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_stochastic_oscillator.py
--rw-r--r--   0 shawn      (503) staff       (20)    14869 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/ichimoku_kinko_hyo_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     8723 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_stock_market_index_historical_data.py
--rw-r--r--   0 shawn      (503) staff       (20)    50532 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/company_initial_public_offering.py
--rw-r--r--   0 shawn      (503) staff       (20)    13643 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/esg_company_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)   253901 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/etf.py
--rw-r--r--   0 shawn      (503) staff       (20)    11109 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_average_directional_index.py
--rw-r--r--   0 shawn      (503) staff       (20)    10812 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_ease_of_movement.py
--rw-r--r--   0 shawn      (503) staff       (20)    41799 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/stock_price.py
--rw-r--r--   0 shawn      (503) staff       (20)     6371 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/owner_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)    15061 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/zacks_etf_holding.py
--rw-r--r--   0 shawn      (503) staff       (20)    10482 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/keltner_channel_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     8463 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/vortex_indicator_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)    16643 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/security_interval_mover.py
--rw-r--r--   0 shawn      (503) staff       (20)    16848 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/intraday_stock_price.py
--rw-r--r--   0 shawn      (503) staff       (20)    20665 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/stock_price_interval.py
--rw-r--r--   0 shawn      (503) staff       (20)    14644 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/option_stats_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)    54424 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/security.py
--rw-r--r--   0 shawn      (503) staff       (20)     6737 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_zacks_etf_holdings.py
--rw-r--r--   0 shawn      (503) staff       (20)    26231 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/filing.py
--rw-r--r--   0 shawn      (503) staff       (20)     6398 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/true_strength_index_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)    23216 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/dividend_record.py
--rw-r--r--   0 shawn      (503) staff       (20)     6570 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/average_daily_trading_volume_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)    20362 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/zacks_analyst_rating.py
--rw-r--r--   0 shawn      (503) staff       (20)     6469 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_companies.py
--rw-r--r--   0 shawn      (503) staff       (20)     5782 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/option_chain.py
--rw-r--r--   0 shawn      (503) staff       (20)    10809 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/security_intervals_movers_result.py
--rw-r--r--   0 shawn      (503) staff       (20)     6739 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/zacks_institutional_holding_historical_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     7091 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_zacks_institutional_holding_owners.py
--rw-r--r--   0 shawn      (503) staff       (20)     4530 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_companies_search.py
--rw-r--r--   0 shawn      (503) staff       (20)     8284 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/security_screen_clause.py
--rw-r--r--   0 shawn      (503) staff       (20)     8133 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/security_screen_result_data.py
--rw-r--r--   0 shawn      (503) staff       (20)     6370 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/awesome_oscillator_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)    12679 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/option_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)     9528 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/filing_note.py
--rw-r--r--   0 shawn      (503) staff       (20)    24401 2023-03-28 00:46:17.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/__init__.py
--rw-r--r--   0 shawn      (503) staff       (20)     6614 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/accumulation_distribution_index_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     6251 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_news.py
--rw-r--r--   0 shawn      (503) staff       (20)    10943 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_ultimate_oscillator.py
--rw-r--r--   0 shawn      (503) staff       (20)     4340 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/option_contracts_list.py
--rw-r--r--   0 shawn      (503) staff       (20)    22944 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/economic_index_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)    18458 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/option_interval.py
--rw-r--r--   0 shawn      (503) staff       (20)    11043 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_relative_strength_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     6533 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_esg_companies.py
--rw-r--r--   0 shawn      (503) staff       (20)     6122 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/technical_indicator.py
--rw-r--r--   0 shawn      (503) staff       (20)     7632 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/option_chain_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)    18293 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/esg_rating_with_company.py
--rw-r--r--   0 shawn      (503) staff       (20)    25762 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/owner.py
--rw-r--r--   0 shawn      (503) staff       (20)     5995 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/historical_data.py
--rw-r--r--   0 shawn      (503) staff       (20)    10988 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_insider_transaction_filings.py
--rw-r--r--   0 shawn      (503) staff       (20)    10878 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_average_true_range.py
--rw-r--r--   0 shawn      (503) staff       (20)     8711 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_esg_company_comprehensive_rating_history.py
--rw-r--r--   0 shawn      (503) staff       (20)   114262 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/esg_comprehensive_rating.py
--rw-r--r--   0 shawn      (503) staff       (20)    36893 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/zacks_eps_surprise.py
--rw-r--r--   0 shawn      (503) staff       (20)     8905 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_zacks_eps_surprises.py
--rw-r--r--   0 shawn      (503) staff       (20)     4344 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_options_tickers.py
--rw-r--r--   0 shawn      (503) staff       (20)    10320 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/filing_note_filing.py
--rw-r--r--   0 shawn      (503) staff       (20)     6233 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/standardized_financial.py
--rw-r--r--   0 shawn      (503) staff       (20)     9185 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_company_insider_transaction_filings.py
--rw-r--r--   0 shawn      (503) staff       (20)    16235 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/esg_rating.py
--rw-r--r--   0 shawn      (503) staff       (20)     8664 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_reported_financials.py
--rw-r--r--   0 shawn      (503) staff       (20)    10878 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_chaikin_money_flow.py
--rw-r--r--   0 shawn      (503) staff       (20)    34497 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/zacks_eps_estimate.py
--rw-r--r--   0 shawn      (503) staff       (20)     6075 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/option_price_batch_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)     6522 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_municipalitiy_financials.py
--rw-r--r--   0 shawn      (503) staff       (20)    14908 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/option_factors_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)     6562 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/on_balance_volume_mean_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)    11142 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_detrended_price_oscillator.py
--rw-r--r--   0 shawn      (503) staff       (20)     8400 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/thea_entity_answer.py
--rw-r--r--   0 shawn      (503) staff       (20)     6515 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_securities.py
--rw-r--r--   0 shawn      (503) staff       (20)    22029 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/data_tag.py
--rw-r--r--   0 shawn      (503) staff       (20)     6287 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_data_tags.py
--rw-r--r--   0 shawn      (503) staff       (20)    16293 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/etf_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     6694 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_historical_data.py
--rw-r--r--   0 shawn      (503) staff       (20)     7995 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_etf_holdings.py
--rw-r--r--   0 shawn      (503) staff       (20)     6344 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/money_flow_index_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)    11139 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_interval_prices.py
--rw-r--r--   0 shawn      (503) staff       (20)    11307 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_accumulation_distribution_index.py
--rw-r--r--   0 shawn      (503) staff       (20)    56139 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/zacks_eps_growth_rate.py
--rw-r--r--   0 shawn      (503) staff       (20)     9510 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_stock_price_adjustments.py
--rw-r--r--   0 shawn      (503) staff       (20)     9686 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_filing_answers.py
--rw-r--r--   0 shawn      (503) staff       (20)     8397 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_options_prices_eod.py
--rw-r--r--   0 shawn      (503) staff       (20)    20794 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/stock_market_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     6362 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/on_balance_volume_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)    43221 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/insider_transaction.py
--rw-r--r--   0 shawn      (503) staff       (20)     6470 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/relative_strength_index_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)    40407 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/option_price_eod.py
--rw-r--r--   0 shawn      (503) staff       (20)    11140 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_intraday_prices.py
--rw-r--r--   0 shawn      (503) staff       (20)    29315 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/zacks_institutional_holding.py
--rw-r--r--   0 shawn      (503) staff       (20)     6245 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_et_fs.py
--rw-r--r--   0 shawn      (503) staff       (20)     7226 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_zacks_institutional_holding_companies.py
--rw-r--r--   0 shawn      (503) staff       (20)     6380 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/volume_price_trend_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)   118624 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/esg_comprehensive_rating_with_company.py
--rw-r--r--   0 shawn      (503) staff       (20)     6688 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_stock_exchanges.py
--rw-r--r--   0 shawn      (503) staff       (20)    45403 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/zacks_institutional_holding_owner_detail.py
--rw-r--r--   0 shawn      (503) staff       (20)     8290 2023-03-28 00:46:32.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/security_screen_group.py
--rw-r--r--   0 shawn      (503) staff       (20)    10812 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_money_flow_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     4549 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_forex_currencies.py
--rw-r--r--   0 shawn      (503) staff       (20)     4355 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_forex_pairs.py
--rw-r--r--   0 shawn      (503) staff       (20)    10779 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_know_sure_thing.py
--rw-r--r--   0 shawn      (503) staff       (20)     6731 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_esg_latest_comprehensive.py
--rw-r--r--   0 shawn      (503) staff       (20)    11043 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_commodity_channel_index.py
--rw-r--r--   0 shawn      (503) staff       (20)    16239 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/insider_transaction_filing.py
--rw-r--r--   0 shawn      (503) staff       (20)     7161 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_zacks_sales_surprises.py
--rw-r--r--   0 shawn      (503) staff       (20)     6240 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/security_snapshot_group.py
--rw-r--r--   0 shawn      (503) staff       (20)     6832 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_institutional_ownership.py
--rw-r--r--   0 shawn      (503) staff       (20)     6500 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_owners.py
--rw-r--r--   0 shawn      (503) staff       (20)     8595 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/donchian_channel_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)    10977 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_simple_moving_average.py
--rw-r--r--   0 shawn      (503) staff       (20)     4617 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_stock_market_indices_search.py
--rw-r--r--   0 shawn      (503) staff       (20)     8383 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_filing_fundamentals.py
--rw-r--r--   0 shawn      (503) staff       (20)     9296 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_stock_exchange_stock_prices.py
--rw-r--r--   0 shawn      (503) staff       (20)     8094 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/forex_pair.py
--rw-r--r--   0 shawn      (503) staff       (20)     8359 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_esg_company_rating_history.py
--rw-r--r--   0 shawn      (503) staff       (20)     7447 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_zacks_target_price_consensuses.py
--rw-r--r--   0 shawn      (503) staff       (20)     6380 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/average_true_range_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)    10811 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_bollinger_bands.py
--rw-r--r--   0 shawn      (503) staff       (20)     7125 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_initial_public_offerings.py
--rw-r--r--   0 shawn      (503) staff       (20)     4453 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_sic_indices_search.py
--rw-r--r--   0 shawn      (503) staff       (20)     4754 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_options_expirations.py
--rw-r--r--   0 shawn      (503) staff       (20)     6101 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/security_screen_result.py
--rw-r--r--   0 shawn      (503) staff       (20)     6326 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/know_sure_thing_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     6380 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/chaikin_money_flow_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     8580 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_historical_data.py
--rw-r--r--   0 shawn      (503) staff       (20)     6546 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_economic_indices.py
--rw-r--r--   0 shawn      (503) staff       (20)    35692 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/zacks_eps_surprise_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)    10845 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_on_balance_volume.py
--rw-r--r--   0 shawn      (503) staff       (20)     9009 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_zacks_analyst_ratings.py
--rw-r--r--   0 shawn      (503) staff       (20)     9486 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_stock_exchange_realtime_stock_prices.py
--rw-r--r--   0 shawn      (503) staff       (20)     6344 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/ease_of_movement_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)    13776 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/bulk_download_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)    10679 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_force_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     6977 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_zacks_institutional_holdings.py
--rw-r--r--   0 shawn      (503) staff       (20)     6610 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_stock_market_indices.py
--rw-r--r--   0 shawn      (503) staff       (20)     6457 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_esg_latest.py
--rw-r--r--   0 shawn      (503) staff       (20)    11790 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/realtime_stock_price_security.py
--rw-r--r--   0 shawn      (503) staff       (20)     7884 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_options_price_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)     9075 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_owner_insider_transaction_filings.py
--rw-r--r--   0 shawn      (503) staff       (20)     6340 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_filings.py
--rw-r--r--   0 shawn      (503) staff       (20)     6434 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/negative_volume_index_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)    10907 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/sic_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     4847 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/security_snapshots_result.py
--rw-r--r--   0 shawn      (503) staff       (20)    23168 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/institutional_ownership.py
--rw-r--r--   0 shawn      (503) staff       (20)    16540 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/data_tag_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)    11361 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/company_news_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)    10743 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/option_intervals_movers_result.py
--rw-r--r--   0 shawn      (503) staff       (20)    10844 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_donchian_channel.py
--rw-r--r--   0 shawn      (503) staff       (20)     4704 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_bulk_download_links.py
--rw-r--r--   0 shawn      (503) staff       (20)     8290 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_option_prices.py
--rw-r--r--   0 shawn      (503) staff       (20)    31195 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/option_price.py
--rw-r--r--   0 shawn      (503) staff       (20)     8917 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_standardized_financials_dimensions.py
--rw-r--r--   0 shawn      (503) staff       (20)     6855 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_zacks_eps_estimates.py
--rw-r--r--   0 shawn      (503) staff       (20)     4742 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_options_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)    11092 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/company_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     4819 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_options_chain_eod.py
--rw-r--r--   0 shawn      (503) staff       (20)    11473 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_moving_average_convergence_divergence.py
--rw-r--r--   0 shawn      (503) staff       (20)    41646 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/realtime_stock_price.py
--rw-r--r--   0 shawn      (503) staff       (20)     8435 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_company_fundamentals.py
--rw-r--r--   0 shawn      (503) staff       (20)    10151 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/average_directional_index_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)    20554 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/stock_exchange.py
--rw-r--r--   0 shawn      (503) staff       (20)     6398 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_sic_indices.py
--rw-r--r--   0 shawn      (503) staff       (20)    21288 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/fundamental.py
--rw-r--r--   0 shawn      (503) staff       (20)    24303 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/economic_index.py
--rw-r--r--   0 shawn      (503) staff       (20)    10977 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_negative_volume_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     7753 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/filing_note_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)    24804 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/option_price_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)     6226 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/mass_index_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)    13209 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/option_eod.py
--rw-r--r--   0 shawn      (503) staff       (20)    10911 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_true_strength_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     6388 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/ultimate_oscillator_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     6560 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_owner_institutional_holdings.py
--rw-r--r--   0 shawn      (503) staff       (20)     6884 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_zacks_analyst_ratings_snapshot.py
--rw-r--r--   0 shawn      (503) staff       (20)    37674 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/zacks_sales_surprise.py
--rw-r--r--   0 shawn      (503) staff       (20)     4817 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/option_snapshots_result.py
--rw-r--r--   0 shawn      (503) staff       (20)     8557 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/option_intervals_result.py
--rw-r--r--   0 shawn      (503) staff       (20)    17338 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/fundamental_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)    14527 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/reported_tag.py
--rw-r--r--   0 shawn      (503) staff       (20)    11142 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_triple_exponential_average.py
--rw-r--r--   0 shawn      (503) staff       (20)     7396 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_zacks_long_term_growth_rates.py
--rw-r--r--   0 shawn      (503) staff       (20)    10662 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/bollinger_bands_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     6167 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/reported_financial_dimension.py
--rw-r--r--   0 shawn      (503) staff       (20)     6145 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/thea_source_document.py
--rw-r--r--   0 shawn      (503) staff       (20)    12624 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/stock_price_adjustment_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)   136507 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/municipality_financial.py
--rw-r--r--   0 shawn      (503) staff       (20)    10646 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_mass_index.py
--rw-r--r--   0 shawn      (503) staff       (20)    10978 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_on_balance_volume_mean.py
--rw-r--r--   0 shawn      (503) staff       (20)     6644 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_company_shares_outstanding.py
--rw-r--r--   0 shawn      (503) staff       (20)     8341 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/stochastic_oscillator_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)    52025 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/earnings_record.py
--rw-r--r--   0 shawn      (503) staff       (20)     6210 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/option_snapshot_group.py
--rw-r--r--   0 shawn      (503) staff       (20)     6549 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/triple_exponential_average_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)    11176 2023-03-28 00:46:16.000000 intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_average_daily_trading_volume.py
-drwxr-xr-x   0 shawn      (503) staff       (20)        0 2023-03-28 02:47:26.000000 intrinio-sdk-6.23.1/intrinio_sdk/api/
--rw-r--r--   0 shawn      (503) staff       (20)    10452 2023-03-28 00:46:17.000000 intrinio-sdk-6.23.1/intrinio_sdk/api/data_point_api.py
--rw-r--r--   0 shawn      (503) staff       (20)    84166 2023-03-28 00:46:17.000000 intrinio-sdk-6.23.1/intrinio_sdk/api/index_api.py
--rw-r--r--   0 shawn      (503) staff       (20)    25579 2023-03-28 00:46:17.000000 intrinio-sdk-6.23.1/intrinio_sdk/api/owners_api.py
--rw-r--r--   0 shawn      (503) staff       (20)    26157 2023-03-28 00:46:17.000000 intrinio-sdk-6.23.1/intrinio_sdk/api/et_fs_api.py
--rw-r--r--   0 shawn      (503) staff       (20)    95784 2023-03-28 00:46:17.000000 intrinio-sdk-6.23.1/intrinio_sdk/api/company_api.py
--rw-r--r--   0 shawn      (503) staff       (20)    16465 2023-03-28 00:46:17.000000 intrinio-sdk-6.23.1/intrinio_sdk/api/municipality_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1157 2023-03-28 00:46:17.000000 intrinio-sdk-6.23.1/intrinio_sdk/api/__init__.py
--rw-r--r--   0 shawn      (503) staff       (20)   342796 2023-03-28 00:46:17.000000 intrinio-sdk-6.23.1/intrinio_sdk/api/security_api.py
--rw-r--r--   0 shawn      (503) staff       (20)   213664 2023-03-28 00:46:17.000000 intrinio-sdk-6.23.1/intrinio_sdk/api/technical_api.py
--rw-r--r--   0 shawn      (503) staff       (20)   123093 2023-03-28 00:46:17.000000 intrinio-sdk-6.23.1/intrinio_sdk/api/options_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     6358 2023-03-28 00:46:17.000000 intrinio-sdk-6.23.1/intrinio_sdk/api/insider_transaction_filings_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     7996 2023-03-28 00:46:17.000000 intrinio-sdk-6.23.1/intrinio_sdk/api/historical_data_api.py
--rw-r--r--   0 shawn      (503) staff       (20)    31234 2023-03-28 00:46:17.000000 intrinio-sdk-6.23.1/intrinio_sdk/api/fundamentals_api.py
--rw-r--r--   0 shawn      (503) staff       (20)    30181 2023-03-28 00:46:17.000000 intrinio-sdk-6.23.1/intrinio_sdk/api/stock_exchange_api.py
--rw-r--r--   0 shawn      (503) staff       (20)    51756 2023-03-28 00:46:17.000000 intrinio-sdk-6.23.1/intrinio_sdk/api/filing_api.py
--rw-r--r--   0 shawn      (503) staff       (20)    14009 2023-03-28 00:46:17.000000 intrinio-sdk-6.23.1/intrinio_sdk/api/data_tag_api.py
--rw-r--r--   0 shawn      (503) staff       (20)    14832 2023-03-28 00:46:17.000000 intrinio-sdk-6.23.1/intrinio_sdk/api/forex_api.py
--rw-r--r--   0 shawn      (503) staff       (20)    74950 2023-03-28 00:46:17.000000 intrinio-sdk-6.23.1/intrinio_sdk/api/zacks_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     4435 2023-03-28 00:46:17.000000 intrinio-sdk-6.23.1/intrinio_sdk/api/bulk_downloads_api.py
--rw-r--r--   0 shawn      (503) staff       (20)    22700 2023-03-28 00:46:17.000000 intrinio-sdk-6.23.1/intrinio_sdk/api/esg_api.py
--rw-r--r--   0 shawn      (503) staff       (20)    26891 2023-03-28 00:46:17.000000 intrinio-sdk-6.23.1/intrinio_sdk/api_client.py
--rw-r--r--   0 shawn      (503) staff       (20)      776 2023-03-28 02:47:26.000000 intrinio-sdk-6.23.1/PKG-INFO
-drwxr-xr-x   0 shawn      (503) staff       (20)        0 2023-03-28 02:47:26.000000 intrinio-sdk-6.23.1/intrinio_sdk.egg-info/
--rw-r--r--   0 shawn      (503) staff       (20)      776 2023-03-28 02:47:26.000000 intrinio-sdk-6.23.1/intrinio_sdk.egg-info/PKG-INFO
--rw-r--r--   0 shawn      (503) staff       (20)    27065 2023-03-28 02:47:26.000000 intrinio-sdk-6.23.1/intrinio_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 shawn      (503) staff       (20)       64 2023-03-28 02:47:26.000000 intrinio-sdk-6.23.1/intrinio_sdk.egg-info/requires.txt
--rw-r--r--   0 shawn      (503) staff       (20)       18 2023-03-28 02:47:26.000000 intrinio-sdk-6.23.1/intrinio_sdk.egg-info/top_level.txt
--rw-r--r--   0 shawn      (503) staff       (20)        1 2023-03-28 02:47:26.000000 intrinio-sdk-6.23.1/intrinio_sdk.egg-info/dependency_links.txt
-drwxr-xr-x   0 shawn      (503) staff       (20)        0 2023-03-28 02:47:26.000000 intrinio-sdk-6.23.1/test/
--rw-r--r--   0 shawn      (503) staff       (20)     1292 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_etf_holding.py
--rw-r--r--   0 shawn      (503) staff       (20)     1540 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_commodity_channel_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     1500 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_ichimoku_kinko_hyo.py
--rw-r--r--   0 shawn      (503) staff       (20)     1458 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_zacks_analyst_ratings.py
--rw-r--r--   0 shawn      (503) staff       (20)     1546 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_institutional_ownership.py
--rw-r--r--   0 shawn      (503) staff       (20)     1440 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_company_securities.py
--rw-r--r--   0 shawn      (503) staff       (20)     1300 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_option_price.py
--rw-r--r--   0 shawn      (503) staff       (20)     1276 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_sic_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     1582 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_stock_exchange_stock_price_adjustments.py
--rw-r--r--   0 shawn      (503) staff       (20)     1234 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_etf.py
--rw-r--r--   0 shawn      (503) staff       (20)     1442 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_filing_notes_search.py
--rw-r--r--   0 shawn      (503) staff       (20)     1382 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_option_factors_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)     1460 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_zacks_eps_growth_rates.py
--rw-r--r--   0 shawn      (503) staff       (20)     1326 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_data_tag_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1426 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_options_chain_eod.py
--rw-r--r--   0 shawn      (503) staff       (20)     1266 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_company.py
--rw-r--r--   0 shawn      (503) staff       (20)     1442 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_zacks_eps_surprises.py
--rw-r--r--   0 shawn      (503) staff       (20)     1466 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_options_chain_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)     1424 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_forex_currencies.py
--rw-r--r--   0 shawn      (503) staff       (20)     1350 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_esg_company_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1384 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_sic_indices.py
--rw-r--r--   0 shawn      (503) staff       (20)     1400 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_mass_index_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1292 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_stock_price.py
--rw-r--r--   0 shawn      (503) staff       (20)     1274 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_security.py
--rw-r--r--   0 shawn      (503) staff       (20)     1540 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_stock_price_adjustments.py
--rw-r--r--   0 shawn      (503) staff       (20)     1350 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_bulk_download_links.py
--rw-r--r--   0 shawn      (503) staff       (20)     1308 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_etf_analytics.py
--rw-r--r--   0 shawn      (503) staff       (20)     1376 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_esg_rating_with_company.py
--rw-r--r--   0 shawn      (503) staff       (20)     1466 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_volume_weighted_average_price_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1358 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_filings.py
--rw-r--r--   0 shawn      (503) staff       (20)     1432 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_option_intervals_movers_result.py
--rw-r--r--   0 shawn      (503) staff       (20)     1598 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_esg_company_comprehensive_rating_history.py
--rw-r--r--   0 shawn      (503) staff       (20)     1374 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_security_screen_result.py
--rw-r--r--   0 shawn      (503) staff       (20)     1382 2023-03-17 22:19:02.000000 intrinio-sdk-6.23.1/test/test_security_interval_mover.py
--rw-r--r--   0 shawn      (503) staff       (20)     4107 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_company_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1366 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_option_snapshot_group.py
--rw-r--r--   0 shawn      (503) staff       (20)     1408 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_security_screen_result_data.py
--rw-r--r--   0 shawn      (503) staff       (20)     1488 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_stochastic_oscillator_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1292 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_filing_note.py
--rw-r--r--   0 shawn      (503) staff       (20)     1484 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_sic_index_historical_data.py
--rw-r--r--   0 shawn      (503) staff       (20)     1442 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_williams_r.py
--rw-r--r--   0 shawn      (503) staff       (20)     1508 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_zacks_eps_surprises.py
--rw-r--r--   0 shawn      (503) staff       (20)     1432 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_stock_price_adjustment_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1466 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_options_stats_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)     1564 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_detrended_price_oscillator.py
--rw-r--r--   0 shawn      (503) staff       (20)     1300 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_reported_tag.py
--rw-r--r--   0 shawn      (503) staff       (20)     1400 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_option_prices.py
--rw-r--r--   0 shawn      (503) staff       (20)     1564 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_company_insider_transaction_filings.py
--rw-r--r--   0 shawn      (503) staff       (20)     1530 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_stochastic_oscillator.py
--rw-r--r--   0 shawn      (503) staff       (20)     1316 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_economic_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     1424 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_realtime_stock_price_security.py
--rw-r--r--   0 shawn      (503) staff       (20)     1284 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_option_eod.py
--rw-r--r--   0 shawn      (503) staff       (20)     1316 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_stock_exchange.py
--rw-r--r--   0 shawn      (503) staff       (20)     1392 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_etf_holdings.py
--rw-r--r--   0 shawn      (503) staff       (20)     1356 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_technical_indicator.py
--rw-r--r--   0 shawn      (503) staff       (20)     1310 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_bulk_downloads_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1368 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_data_tags.py
--rw-r--r--   0 shawn      (503) staff       (20)     1422 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_reported_financial_dimension.py
--rw-r--r--   0 shawn      (503) staff       (20)     1506 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_awesome_oscillator.py
--rw-r--r--   0 shawn      (503) staff       (20)     1530 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_zacks_institutional_holding_company_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1424 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_economic_indices.py
--rw-r--r--   0 shawn      (503) staff       (20)     1562 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_standardized_financials_dimensions.py
--rw-r--r--   0 shawn      (503) staff       (20)     1514 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_ultimate_oscillator.py
--rw-r--r--   0 shawn      (503) staff       (20)     1366 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_option_price_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)     1408 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_option_price_batch_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)     1548 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_owner_insider_transaction_filings.py
--rw-r--r--   0 shawn      (503) staff       (20)     1490 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_vortex_indicator.py
--rw-r--r--   0 shawn      (503) staff       (20)     1500 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_chaikin_money_flow.py
--rw-r--r--   0 shawn      (503) staff       (20)     1448 2023-03-17 22:19:02.000000 intrinio-sdk-6.23.1/test/test_security_intervals_movers_result.py
--rw-r--r--   0 shawn      (503) staff       (20)     1414 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_municipalities.py
--rw-r--r--   0 shawn      (503) staff       (20)     1416 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_historical_data.py
--rw-r--r--   0 shawn      (503) staff       (20)     1366 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_security_screen_group.py
--rw-r--r--   0 shawn      (503) staff       (20)     1358 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_realtime_stock_price.py
--rw-r--r--   0 shawn      (503) staff       (20)     1590 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_zacks_analyst_ratings_snapshot.py
--rw-r--r--   0 shawn      (503) staff       (20)     1476 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_know_sure_thing.py
--rw-r--r--   0 shawn      (503) staff       (20)     1482 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_esg_latest_comprehensive.py
--rw-r--r--   0 shawn      (503) staff       (20)     1506 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_insider_transaction_filings.py
--rw-r--r--   0 shawn      (503) staff       (20)     6812 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_technical_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1482 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_intraday_prices.py
--rw-r--r--   0 shawn      (503) staff       (20)     1500 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_average_true_range.py
--rw-r--r--   0 shawn      (503) staff       (20)     1380 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_municipality_financial.py
--rw-r--r--   0 shawn      (503) staff       (20)     1484 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_on_balance_volume_mean_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1358 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_zacks_sales_surprise.py
--rw-r--r--   0 shawn      (503) staff       (20)     1482 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_esg_comprehensive_rating_with_company.py
--rw-r--r--   0 shawn      (503) staff       (20)     1400 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_zacks_eps_surprise_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1336 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_et_fs.py
--rw-r--r--   0 shawn      (503) staff       (20)     1524 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_economic_index_historical_data.py
--rw-r--r--   0 shawn      (503) staff       (20)     1464 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_awesome_oscillator_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1482 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_interval_prices.py
--rw-r--r--   0 shawn      (503) staff       (20)     1526 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_on_balance_volume_mean.py
--rw-r--r--   0 shawn      (503) staff       (20)     1424 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_options_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)     1360 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_zacks_eps_growth_rate.py
--rw-r--r--   0 shawn      (503) staff       (20)     1342 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_stock_market_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     1342 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_thea_entity_answer.py
--rw-r--r--   0 shawn      (503) staff       (20)     1416 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_stock_exchanges.py
--rw-r--r--   0 shawn      (503) staff       (20)     1462 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_standardized_financials_dimension.py
--rw-r--r--   0 shawn      (503) staff       (20)     1448 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_reported_financials.py
--rw-r--r--   0 shawn      (503) staff       (20)     1324 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_earnings_record.py
--rw-r--r--   0 shawn      (503) staff       (20)     3094 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_zacks_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1326 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_option_price_eod.py
--rw-r--r--   0 shawn      (503) staff       (20)     1358 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_thea_source_document.py
--rw-r--r--   0 shawn      (503) staff       (20)     1604 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_moving_average_convergence_divergence_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     2223 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_fundamentals_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1402 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_zacks_long_term_growth_rate.py
--rw-r--r--   0 shawn      (503) staff       (20)     1308 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_owner_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1498 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_commodity_channel_index_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1350 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_stock_price_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1406 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_insider_transaction_filing.py
--rw-r--r--   0 shawn      (503) staff       (20)     1458 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_stock_prices.py
--rw-r--r--   0 shawn      (503) staff       (20)     1482 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_negative_volume_index_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1484 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_ease_of_movement.py
--rw-r--r--   0 shawn      (503) staff       (20)     1458 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_ichimoku_kinko_hyo_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1514 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_zacks_institutional_holding_owner_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)        0 2023-03-28 00:46:17.000000 intrinio-sdk-6.23.1/test/__init__.py
--rw-r--r--   0 shawn      (503) staff       (20)     1559 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_data_tag_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1366 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_bulk_download_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1522 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_triple_exponential_average_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1358 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_company_news_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1440 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_company_initial_public_offering.py
--rw-r--r--   0 shawn      (503) staff       (20)     1482 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_historical_data.py
--rw-r--r--   0 shawn      (503) staff       (20)     1384 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_forex_pairs.py
--rw-r--r--   0 shawn      (503) staff       (20)     2673 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_filing_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1490 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_stock_exchange_securities.py
--rw-r--r--   0 shawn      (503) staff       (20)     1440 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_keltner_channel_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1398 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_security_snapshots_result.py
--rw-r--r--   0 shawn      (503) staff       (20)     2236 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_stock_exchange_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1448 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_vortex_indicator_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1408 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_force_index_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1482 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_initial_public_offerings.py
--rw-r--r--   0 shawn      (503) staff       (20)     1558 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_forex_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1500 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_volume_price_trend.py
--rw-r--r--   0 shawn      (503) staff       (20)     1292 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_forex_price.py
--rw-r--r--   0 shawn      (503) staff       (20)     1434 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_zacks_etf_holdings.py
--rw-r--r--   0 shawn      (503) staff       (20)     1324 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_company_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1284 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_forex_pair.py
--rw-r--r--   0 shawn      (503) staff       (20)     1482 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_bollinger_bands.py
--rw-r--r--   0 shawn      (503) staff       (20)     1524 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_zacks_sales_surprises.py
--rw-r--r--   0 shawn      (503) staff       (20)     1582 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_volume_weighted_average_price.py
--rw-r--r--   0 shawn      (503) staff       (20)     1466 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_true_strength_index_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1516 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_options_prices_batch_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)     1556 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_zacks_institutional_holding_owners.py
--rw-r--r--   0 shawn      (503) staff       (20)     1448 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_filing_fundamentals.py
--rw-r--r--   0 shawn      (503) staff       (20)     1448 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_donchian_channel_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1390 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_esg_comprehensive_rating.py
--rw-r--r--   0 shawn      (503) staff       (20)     1392 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_forex_prices.py
--rw-r--r--   0 shawn      (503) staff       (20)     1382 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_option_intervals_result.py
--rw-r--r--   0 shawn      (503) staff       (20)     1366 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_option_stats_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)     1562 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_accumulation_distribution_index_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1434 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_sic_indices_search.py
--rw-r--r--   0 shawn      (503) staff       (20)     1458 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_average_true_range_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1448 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_options_expirations.py
--rw-r--r--   0 shawn      (503) staff       (20)     1434 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_know_sure_thing_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1522 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_detrended_price_oscillator_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1276 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_etf_stats.py
--rw-r--r--   0 shawn      (503) staff       (20)     1418 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_data_tags_search.py
--rw-r--r--   0 shawn      (503) staff       (20)     1400 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_esg_companies.py
--rw-r--r--   0 shawn      (503) staff       (20)     1442 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_ease_of_movement_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1482 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_keltner_channel.py
--rw-r--r--   0 shawn      (503) staff       (20)     1918 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_owners_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1458 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_chaikin_money_flow_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1482 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_options_unusual_activity.py
--rw-r--r--   0 shawn      (503) staff       (20)     1482 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_simple_moving_average_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1524 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_negative_volume_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     1466 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_options_price_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)     1382 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_option_snapshots_result.py
--rw-r--r--   0 shawn      (503) staff       (20)     1522 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_zacks_institutional_holding_company_detail.py
--rw-r--r--   0 shawn      (503) staff       (20)     1500 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_stock_market_indices_search.py
--rw-r--r--   0 shawn      (503) staff       (20)     1500 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_stock_exchange_stock_prices.py
--rw-r--r--   0 shawn      (503) staff       (20)     1574 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_average_daily_trading_volume.py
--rw-r--r--   0 shawn      (503) staff       (20)     1456 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_company_fundamentals.py
--rw-r--r--   0 shawn      (503) staff       (20)     1564 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_triple_exponential_average.py
--rw-r--r--   0 shawn      (503) staff       (20)     1342 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_zacks_eps_surprise.py
--rw-r--r--   0 shawn      (503) staff       (20)     1284 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_esg_rating.py
--rw-r--r--   0 shawn      (503) staff       (20)     1342 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_filing_note_filing.py
--rw-r--r--   0 shawn      (503) staff       (20)     1488 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_municipalitiy_financials.py
--rw-r--r--   0 shawn      (503) staff       (20)     1392 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_company_news.py
--rw-r--r--   0 shawn      (503) staff       (20)     1374 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_stock_price_adjustment.py
--rw-r--r--   0 shawn      (503) staff       (20)     1342 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_zacks_eps_estimate.py
--rw-r--r--   0 shawn      (503) staff       (20)     1502 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_zacks_long_term_growth_rates.py
--rw-r--r--   0 shawn      (503) staff       (20)     1506 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_zacks_institutional_holding_owner_detail.py
--rw-r--r--   0 shawn      (503) staff       (20)     1442 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_money_flow_index_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1358 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_options.py
--rw-r--r--   0 shawn      (503) staff       (20)     1298 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_fundamental.py
--rw-r--r--   0 shawn      (503) staff       (20)     1356 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_fundamental_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1556 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_average_directional_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     1434 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_options_prices_eod.py
--rw-r--r--   0 shawn      (503) staff       (20)     1550 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_stock_market_index_historical_data.py
--rw-r--r--   0 shawn      (503) staff       (20)     1648 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_municipality_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1498 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_company_shares_outstanding.py
--rw-r--r--   0 shawn      (503) staff       (20)     1484 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_money_flow_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     1514 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_average_directional_index_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1366 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_option_chain_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)     1366 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_option_contracts_list.py
--rw-r--r--   0 shawn      (503) staff       (20)    10454 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_security_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1424 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_zacks_analyst_rating_snapshot.py
--rw-r--r--   0 shawn      (503) staff       (20)     1458 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_zacks_sales_surprises.py
--rw-r--r--   0 shawn      (503) staff       (20)     1388 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_institutional_ownership.py
--rw-r--r--   0 shawn      (503) staff       (20)     1508 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_true_strength_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     1416 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_options_tickers.py
--rw-r--r--   0 shawn      (503) staff       (20)     1514 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_owner_institutional_holdings.py
--rw-r--r--   0 shawn      (503) staff       (20)     1431 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_insider_transaction_filings_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1392 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_filing_notes.py
--rw-r--r--   0 shawn      (503) staff       (20)     1358 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_option_unusual_trade.py
--rw-r--r--   0 shawn      (503) staff       (20)     1300 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_option_chain.py
--rw-r--r--   0 shawn      (503) staff       (20)     1458 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_volume_price_trend_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1350 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_filing_note_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1258 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_option.py
--rw-r--r--   0 shawn      (503) staff       (20)     1416 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_zacks_target_price_consensus.py
--rw-r--r--   0 shawn      (503) staff       (20)     1292 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_etf_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1474 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_company_historical_data.py
--rw-r--r--   0 shawn      (503) staff       (20)     1498 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_relative_strength_index_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1416 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_zacks_sales_surprise_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1324 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_option_realtime.py
--rw-r--r--   0 shawn      (503) staff       (20)     1450 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_stock_market_indices.py
--rw-r--r--   0 shawn      (503) staff       (20)     1372 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_institutional_holding.py
--rw-r--r--   0 shawn      (503) staff       (20)     1350 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_owners.py
--rw-r--r--   0 shawn      (503) staff       (20)     1324 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_option_interval.py
--rw-r--r--   0 shawn      (503) staff       (20)     1450 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_force_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     1524 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_zacks_analyst_ratings.py
--rw-r--r--   0 shawn      (503) staff       (20)     1408 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_filing_answers.py
--rw-r--r--   0 shawn      (503) staff       (20)     1268 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_data_tag.py
--rw-r--r--   0 shawn      (503) staff       (20)     1356 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_insider_transaction.py
--rw-r--r--   0 shawn      (503) staff       (20)     1380 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_standardized_financial.py
--rw-r--r--   0 shawn      (503) staff       (20)     1566 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_stock_exchange_realtime_stock_prices.py
--rw-r--r--   0 shawn      (503) staff       (20)     5109 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_options_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1416 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_company_filings.py
--rw-r--r--   0 shawn      (503) staff       (20)     1472 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_ultimate_oscillator_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1432 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_company_recognize.py
--rw-r--r--   0 shawn      (503) staff       (20)     1376 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_esg_latest.py
--rw-r--r--   0 shawn      (503) staff       (20)     1934 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_esg_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1414 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_zacks_institutional_holding.py
--rw-r--r--   0 shawn      (503) staff       (20)     1374 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_security_screen_clause.py
--rw-r--r--   0 shawn      (503) staff       (20)     1406 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_company_shares_outstanding.py
--rw-r--r--   0 shawn      (503) staff       (20)     1440 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_bollinger_bands_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1324 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_historical_data.py
--rw-r--r--   0 shawn      (503) staff       (20)     1332 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_security_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1442 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_mass_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     1432 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_securities_search.py
--rw-r--r--   0 shawn      (503) staff       (20)     1316 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_forex_currency.py
--rw-r--r--   0 shawn      (503) staff       (20)     1374 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_economic_index_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1524 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_simple_moving_average.py
--rw-r--r--   0 shawn      (503) staff       (20)     1258 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_filing.py
--rw-r--r--   0 shawn      (503) staff       (20)     1334 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_zacks_etf_holding.py
--rw-r--r--   0 shawn      (503) staff       (20)     1524 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_zacks_target_price_consensuses.py
--rw-r--r--   0 shawn      (503) staff       (20)     1416 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_zacks_analyst_rating_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1924 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_et_fs_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1554 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_zacks_institutional_holding_historical_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1604 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_accumulation_distribution_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     1334 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_news.py
--rw-r--r--   0 shawn      (503) staff       (20)     1444 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_data_point_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1492 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_on_balance_volume.py
--rw-r--r--   0 shawn      (503) staff       (20)     1480 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_standardized_financials.py
--rw-r--r--   0 shawn      (503) staff       (20)     1400 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_stock_market_index_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1646 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_moving_average_convergence_divergence.py
--rw-r--r--   0 shawn      (503) staff       (20)     1316 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_filing_summary.py
--rw-r--r--   0 shawn      (503) staff       (20)     1514 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_zacks_institutional_holdings.py
--rw-r--r--   0 shawn      (503) staff       (20)     1382 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_security_snapshot_group.py
--rw-r--r--   0 shawn      (503) staff       (20)     1400 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_options_chain.py
--rw-r--r--   0 shawn      (503) staff       (20)     1366 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_option_interval_mover.py
--rw-r--r--   0 shawn      (503) staff       (20)     1424 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_companies_search.py
--rw-r--r--   0 shawn      (503) staff       (20)     1474 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_economic_indices_search.py
--rw-r--r--   0 shawn      (503) staff       (20)     1374 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_companies.py
--rw-r--r--   0 shawn      (503) staff       (20)     1450 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_on_balance_volume_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1492 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_esg_company_rating_history.py
--rw-r--r--   0 shawn      (503) staff       (20)     1416 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_company_answers.py
--rw-r--r--   0 shawn      (503) staff       (20)     1358 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_intraday_stock_price.py
--rw-r--r--   0 shawn      (503) staff       (20)     1348 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_reported_financial.py
--rw-r--r--   0 shawn      (503) staff       (20)     1540 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_relative_strength_index.py
--rw-r--r--   0 shawn      (503) staff       (20)     1442 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_bulk_download_links.py
--rw-r--r--   0 shawn      (503) staff       (20)     4422 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_index_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1358 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_stock_price_interval.py
--rw-r--r--   0 shawn      (503) staff       (20)     1400 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_williams_r_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1532 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_average_daily_trading_volume_technical_value.py
--rw-r--r--   0 shawn      (503) staff       (20)     1300 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_company_news.py
--rw-r--r--   0 shawn      (503) staff       (20)     1382 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_securities.py
--rw-r--r--   0 shawn      (503) staff       (20)     1326 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_option_chain_eod.py
--rw-r--r--   0 shawn      (503) staff       (20)     1580 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_zacks_institutional_holding_companies.py
--rw-r--r--   0 shawn      (503) staff       (20)     1306 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_municipality.py
--rw-r--r--   0 shawn      (503) staff       (20)     1490 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_security_donchian_channel.py
--rw-r--r--   0 shawn      (503) staff       (20)     1316 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_company_filing.py
--rw-r--r--   0 shawn      (503) staff       (20)     1314 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_historical_data_api.py
--rw-r--r--   0 shawn      (503) staff       (20)     1358 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_zacks_analyst_rating.py
--rw-r--r--   0 shawn      (503) staff       (20)     1250 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_owner.py
--rw-r--r--   0 shawn      (503) staff       (20)     1442 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_api_response_zacks_eps_estimates.py
--rw-r--r--   0 shawn      (503) staff       (20)     1324 2023-03-17 22:01:54.000000 intrinio-sdk-6.23.1/test/test_dividend_record.py
--rw-r--r--   0 shawn      (503) staff       (20)    57007 2023-03-28 00:46:17.000000 intrinio-sdk-6.23.1/README.md
--rw-r--r--   0 shawn      (503) staff       (20)     1844 2023-03-28 00:46:17.000000 intrinio-sdk-6.23.1/setup.py
--rw-r--r--   0 shawn      (503) staff       (20)       38 2023-03-28 02:47:26.000000 intrinio-sdk-6.23.1/setup.cfg
+drwxr-xr-x   0 shawn      (503) staff       (20)        0 2023-06-14 14:28:29.000000 intrinio-sdk-6.24.0/
+drwxr-xr-x   0 shawn      (503) staff       (20)        0 2023-06-14 14:28:29.000000 intrinio-sdk-6.24.0/intrinio_sdk/
+-rw-r--r--   0 shawn      (503) staff       (20)     8604 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/configuration.py
+-rw-r--r--   0 shawn      (503) staff       (20)    13819 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/rest.py
+-rw-r--r--   0 shawn      (503) staff       (20)    25620 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/__init__.py
+drwxr-xr-x   0 shawn      (503) staff       (20)        0 2023-06-14 14:28:29.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/
+-rw-r--r--   0 shawn      (503) staff       (20)    26373 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/zacks_target_price_consensus.py
+-rw-r--r--   0 shawn      (503) staff       (20)     9009 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_zacks_sales_surprises.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6524 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/detrended_price_oscillator_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)    40363 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/zacks_sales_surprise_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6602 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_options.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6656 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_municipalities.py
+-rw-r--r--   0 shawn      (503) staff       (20)    10646 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_williams_r.py
+-rw-r--r--   0 shawn      (503) staff       (20)     7658 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/forex_currency.py
+-rw-r--r--   0 shawn      (503) staff       (20)    32532 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/zacks_institutional_holding_company_detail.py
+-rw-r--r--   0 shawn      (503) staff       (20)    10844 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_vortex_indicator.py
+-rw-r--r--   0 shawn      (503) staff       (20)    10910 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_awesome_oscillator.py
+-rw-r--r--   0 shawn      (503) staff       (20)     4570 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_securities_search.py
+-rw-r--r--   0 shawn      (503) staff       (20)     8175 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_company_filings.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6593 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_filing_notes.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6229 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/williams_r_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     7946 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_options_stats_realtime.py
+-rw-r--r--   0 shawn      (503) staff       (20)    22943 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/security_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)    14290 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/stock_price_adjustment.py
+-rw-r--r--   0 shawn      (503) staff       (20)     4691 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_options_prices_batch_realtime.py
+-rw-r--r--   0 shawn      (503) staff       (20)     4746 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_options_chain.py
+-rw-r--r--   0 shawn      (503) staff       (20)     8872 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_standardized_financials.py
+-rw-r--r--   0 shawn      (503) staff       (20)    19333 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/stock_market_index_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)     8463 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_sic_index_historical_data.py
+-rw-r--r--   0 shawn      (503) staff       (20)     8068 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_company_news.py
+-rw-r--r--   0 shawn      (503) staff       (20)    24031 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/option_unusual_trade.py
+-rw-r--r--   0 shawn      (503) staff       (20)     4354 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_data_tags_search.py
+-rw-r--r--   0 shawn      (503) staff       (20)    32022 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/institutional_holding.py
+-rw-r--r--   0 shawn      (503) staff       (20)     4539 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_company_recognize.py
+-rw-r--r--   0 shawn      (503) staff       (20)     4571 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_economic_indices_search.py
+-rw-r--r--   0 shawn      (503) staff       (20)    18849 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/zacks_analyst_rating_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)    79809 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/etf_stats.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6357 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/standardized_financials_dimension.py
+-rw-r--r--   0 shawn      (503) staff       (20)    57040 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/zacks_long_term_growth_rate.py
+-rw-r--r--   0 shawn      (503) staff       (20)     8325 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_company_securities.py
+-rw-r--r--   0 shawn      (503) staff       (20)    70186 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/company.py
+-rw-r--r--   0 shawn      (503) staff       (20)     7058 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_zacks_eps_growth_rates.py
+-rw-r--r--   0 shawn      (503) staff       (20)    12984 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/company_news.py
+-rw-r--r--   0 shawn      (503) staff       (20)    23120 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/etf_analytics.py
+-rw-r--r--   0 shawn      (503) staff       (20)     8401 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/reported_financial.py
+-rw-r--r--   0 shawn      (503) staff       (20)    37102 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/municipality.py
+-rw-r--r--   0 shawn      (503) staff       (20)    21150 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/company_filing.py
+-rw-r--r--   0 shawn      (503) staff       (20)    14903 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/company_shares_outstanding.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6794 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_zacks_analyst_ratings.py
+-rw-r--r--   0 shawn      (503) staff       (20)     4642 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_filing_notes_search.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6244 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/force_index_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     8641 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_economic_index_historical_data.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6470 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/commodity_channel_index_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     9762 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_company_answers.py
+-rw-r--r--   0 shawn      (503) staff       (20)     7063 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_zacks_eps_surprises.py
+-rw-r--r--   0 shawn      (503) staff       (20)     8528 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_company_historical_data.py
+-rw-r--r--   0 shawn      (503) staff       (20)    16762 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/option_interval_mover.py
+-rw-r--r--   0 shawn      (503) staff       (20)    11274 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/moving_average_convergence_divergence_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     8244 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_forex_prices.py
+-rw-r--r--   0 shawn      (503) staff       (20)     4894 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_options_chain_realtime.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6482 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/zacks_institutional_holding_owner_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)    14640 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/option.py
+-rw-r--r--   0 shawn      (503) staff       (20)    40823 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/stock_price_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)    19534 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/filing_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)    19707 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/forex_price.py
+-rw-r--r--   0 shawn      (503) staff       (20)    11154 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_volume_weighted_average_price.py
+-rw-r--r--   0 shawn      (503) staff       (20)    23701 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/zacks_analyst_rating_snapshot.py
+-rw-r--r--   0 shawn      (503) staff       (20)    10878 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_ichimoku_kinko_hyo.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6465 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/volume_weighted_average_price_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     5890 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/option_chain_eod.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6050 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/bulk_download_links.py
+-rw-r--r--   0 shawn      (503) staff       (20)    10878 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_volume_price_trend.py
+-rw-r--r--   0 shawn      (503) staff       (20)    37768 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/etf_holding.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6434 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/simple_moving_average_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     4823 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_options_unusual_activity.py
+-rw-r--r--   0 shawn      (503) staff       (20)     8432 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/zacks_institutional_holding_company_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)     9138 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_stock_exchange_securities.py
+-rw-r--r--   0 shawn      (503) staff       (20)     9875 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_stock_exchange_stock_price_adjustments.py
+-rw-r--r--   0 shawn      (503) staff       (20)    10811 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_keltner_channel.py
+-rw-r--r--   0 shawn      (503) staff       (20)     8931 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_stock_prices.py
+-rw-r--r--   0 shawn      (503) staff       (20)    11009 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_stochastic_oscillator.py
+-rw-r--r--   0 shawn      (503) staff       (20)    14869 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/ichimoku_kinko_hyo_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     8723 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_stock_market_index_historical_data.py
+-rw-r--r--   0 shawn      (503) staff       (20)    50532 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/company_initial_public_offering.py
+-rw-r--r--   0 shawn      (503) staff       (20)    13643 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/esg_company_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)   253901 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/etf.py
+-rw-r--r--   0 shawn      (503) staff       (20)    11109 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_average_directional_index.py
+-rw-r--r--   0 shawn      (503) staff       (20)    10812 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_ease_of_movement.py
+-rw-r--r--   0 shawn      (503) staff       (20)    41799 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/stock_price.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6371 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/owner_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)    15061 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/zacks_etf_holding.py
+-rw-r--r--   0 shawn      (503) staff       (20)    10482 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/keltner_channel_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     8463 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/vortex_indicator_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)    16643 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/security_interval_mover.py
+-rw-r--r--   0 shawn      (503) staff       (20)    16848 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/intraday_stock_price.py
+-rw-r--r--   0 shawn      (503) staff       (20)    20665 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/stock_price_interval.py
+-rw-r--r--   0 shawn      (503) staff       (20)    14644 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/option_stats_realtime.py
+-rw-r--r--   0 shawn      (503) staff       (20)    54424 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/security.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6737 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_zacks_etf_holdings.py
+-rw-r--r--   0 shawn      (503) staff       (20)    26231 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/filing.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6398 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/true_strength_index_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)    23216 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/dividend_record.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6570 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/average_daily_trading_volume_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)    20362 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/zacks_analyst_rating.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6469 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_companies.py
+-rw-r--r--   0 shawn      (503) staff       (20)     5782 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/option_chain.py
+-rw-r--r--   0 shawn      (503) staff       (20)    10809 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/security_intervals_movers_result.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6739 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/zacks_institutional_holding_historical_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)     7091 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_zacks_institutional_holding_owners.py
+-rw-r--r--   0 shawn      (503) staff       (20)     4530 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_companies_search.py
+-rw-r--r--   0 shawn      (503) staff       (20)     8284 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/security_screen_clause.py
+-rw-r--r--   0 shawn      (503) staff       (20)     8133 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/security_screen_result_data.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6370 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/awesome_oscillator_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)    12679 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/option_realtime.py
+-rw-r--r--   0 shawn      (503) staff       (20)     9528 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/filing_note.py
+-rw-r--r--   0 shawn      (503) staff       (20)    24401 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/__init__.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6614 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/accumulation_distribution_index_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6251 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_news.py
+-rw-r--r--   0 shawn      (503) staff       (20)    10943 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_ultimate_oscillator.py
+-rw-r--r--   0 shawn      (503) staff       (20)     4340 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/option_contracts_list.py
+-rw-r--r--   0 shawn      (503) staff       (20)    22944 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/economic_index_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)    18458 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/option_interval.py
+-rw-r--r--   0 shawn      (503) staff       (20)    11043 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_relative_strength_index.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6533 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_esg_companies.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6122 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/technical_indicator.py
+-rw-r--r--   0 shawn      (503) staff       (20)     7632 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/option_chain_realtime.py
+-rw-r--r--   0 shawn      (503) staff       (20)    18293 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/esg_rating_with_company.py
+-rw-r--r--   0 shawn      (503) staff       (20)    25762 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/owner.py
+-rw-r--r--   0 shawn      (503) staff       (20)     5995 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/historical_data.py
+-rw-r--r--   0 shawn      (503) staff       (20)    10988 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_insider_transaction_filings.py
+-rw-r--r--   0 shawn      (503) staff       (20)    10878 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_average_true_range.py
+-rw-r--r--   0 shawn      (503) staff       (20)     8711 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_esg_company_comprehensive_rating_history.py
+-rw-r--r--   0 shawn      (503) staff       (20)   114262 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/esg_comprehensive_rating.py
+-rw-r--r--   0 shawn      (503) staff       (20)    36893 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/zacks_eps_surprise.py
+-rw-r--r--   0 shawn      (503) staff       (20)     8905 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_zacks_eps_surprises.py
+-rw-r--r--   0 shawn      (503) staff       (20)     4344 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_options_tickers.py
+-rw-r--r--   0 shawn      (503) staff       (20)    10320 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/filing_note_filing.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6233 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/standardized_financial.py
+-rw-r--r--   0 shawn      (503) staff       (20)     9185 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_company_insider_transaction_filings.py
+-rw-r--r--   0 shawn      (503) staff       (20)    16235 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/esg_rating.py
+-rw-r--r--   0 shawn      (503) staff       (20)     8664 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_reported_financials.py
+-rw-r--r--   0 shawn      (503) staff       (20)    10878 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_chaikin_money_flow.py
+-rw-r--r--   0 shawn      (503) staff       (20)    34497 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/zacks_eps_estimate.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6075 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/option_price_batch_realtime.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6522 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_municipalitiy_financials.py
+-rw-r--r--   0 shawn      (503) staff       (20)    14908 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/option_factors_realtime.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6562 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/on_balance_volume_mean_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)    11142 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_detrended_price_oscillator.py
+-rw-r--r--   0 shawn      (503) staff       (20)     8400 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/thea_entity_answer.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6515 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_securities.py
+-rw-r--r--   0 shawn      (503) staff       (20)    22029 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/data_tag.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6287 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_data_tags.py
+-rw-r--r--   0 shawn      (503) staff       (20)    16293 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/etf_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6694 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_historical_data.py
+-rw-r--r--   0 shawn      (503) staff       (20)     7995 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_etf_holdings.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6344 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/money_flow_index_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)    11139 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_interval_prices.py
+-rw-r--r--   0 shawn      (503) staff       (20)    11307 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_accumulation_distribution_index.py
+-rw-r--r--   0 shawn      (503) staff       (20)    56139 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/zacks_eps_growth_rate.py
+-rw-r--r--   0 shawn      (503) staff       (20)     9510 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_stock_price_adjustments.py
+-rw-r--r--   0 shawn      (503) staff       (20)     9686 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_filing_answers.py
+-rw-r--r--   0 shawn      (503) staff       (20)     8397 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_options_prices_eod.py
+-rw-r--r--   0 shawn      (503) staff       (20)    20794 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/stock_market_index.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6362 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/on_balance_volume_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)    43221 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/insider_transaction.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6470 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/relative_strength_index_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)    40407 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/option_price_eod.py
+-rw-r--r--   0 shawn      (503) staff       (20)    11140 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_intraday_prices.py
+-rw-r--r--   0 shawn      (503) staff       (20)    29315 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/zacks_institutional_holding.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6245 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_et_fs.py
+-rw-r--r--   0 shawn      (503) staff       (20)     7226 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_zacks_institutional_holding_companies.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6380 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/volume_price_trend_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)   118624 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/esg_comprehensive_rating_with_company.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6688 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_stock_exchanges.py
+-rw-r--r--   0 shawn      (503) staff       (20)    45403 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/zacks_institutional_holding_owner_detail.py
+-rw-r--r--   0 shawn      (503) staff       (20)     8290 2023-06-14 13:32:31.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/security_screen_group.py
+-rw-r--r--   0 shawn      (503) staff       (20)    10812 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_money_flow_index.py
+-rw-r--r--   0 shawn      (503) staff       (20)     4549 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_forex_currencies.py
+-rw-r--r--   0 shawn      (503) staff       (20)     4355 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_forex_pairs.py
+-rw-r--r--   0 shawn      (503) staff       (20)    10779 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_know_sure_thing.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6731 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_esg_latest_comprehensive.py
+-rw-r--r--   0 shawn      (503) staff       (20)    11043 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_commodity_channel_index.py
+-rw-r--r--   0 shawn      (503) staff       (20)    16239 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/insider_transaction_filing.py
+-rw-r--r--   0 shawn      (503) staff       (20)     7161 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_zacks_sales_surprises.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6240 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/security_snapshot_group.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6832 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_institutional_ownership.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6500 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_owners.py
+-rw-r--r--   0 shawn      (503) staff       (20)     8595 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/donchian_channel_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)    10977 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_simple_moving_average.py
+-rw-r--r--   0 shawn      (503) staff       (20)     4617 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_stock_market_indices_search.py
+-rw-r--r--   0 shawn      (503) staff       (20)     8383 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_filing_fundamentals.py
+-rw-r--r--   0 shawn      (503) staff       (20)     9296 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_stock_exchange_stock_prices.py
+-rw-r--r--   0 shawn      (503) staff       (20)     8094 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/forex_pair.py
+-rw-r--r--   0 shawn      (503) staff       (20)     8359 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_esg_company_rating_history.py
+-rw-r--r--   0 shawn      (503) staff       (20)     7447 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_zacks_target_price_consensuses.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6380 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/average_true_range_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)    10811 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_bollinger_bands.py
+-rw-r--r--   0 shawn      (503) staff       (20)     7125 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_initial_public_offerings.py
+-rw-r--r--   0 shawn      (503) staff       (20)     4453 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_sic_indices_search.py
+-rw-r--r--   0 shawn      (503) staff       (20)     4754 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_options_expirations.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6101 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/security_screen_result.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6326 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/know_sure_thing_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6380 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/chaikin_money_flow_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     8580 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_historical_data.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6546 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_economic_indices.py
+-rw-r--r--   0 shawn      (503) staff       (20)    35692 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/zacks_eps_surprise_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)    10845 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_on_balance_volume.py
+-rw-r--r--   0 shawn      (503) staff       (20)     9009 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_zacks_analyst_ratings.py
+-rw-r--r--   0 shawn      (503) staff       (20)     9486 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_stock_exchange_realtime_stock_prices.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6344 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/ease_of_movement_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)    13776 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/bulk_download_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)    10679 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_force_index.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6977 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_zacks_institutional_holdings.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6610 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_stock_market_indices.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6457 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_esg_latest.py
+-rw-r--r--   0 shawn      (503) staff       (20)    11790 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/realtime_stock_price_security.py
+-rw-r--r--   0 shawn      (503) staff       (20)     7884 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_options_price_realtime.py
+-rw-r--r--   0 shawn      (503) staff       (20)     9075 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_owner_insider_transaction_filings.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6340 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_filings.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6434 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/negative_volume_index_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)    10907 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/sic_index.py
+-rw-r--r--   0 shawn      (503) staff       (20)     4847 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/security_snapshots_result.py
+-rw-r--r--   0 shawn      (503) staff       (20)    23168 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/institutional_ownership.py
+-rw-r--r--   0 shawn      (503) staff       (20)    16540 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/data_tag_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)    11361 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/company_news_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)    10743 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/option_intervals_movers_result.py
+-rw-r--r--   0 shawn      (503) staff       (20)    10844 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_donchian_channel.py
+-rw-r--r--   0 shawn      (503) staff       (20)     4704 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_bulk_download_links.py
+-rw-r--r--   0 shawn      (503) staff       (20)     8290 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_option_prices.py
+-rw-r--r--   0 shawn      (503) staff       (20)    31195 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/option_price.py
+-rw-r--r--   0 shawn      (503) staff       (20)     8917 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_standardized_financials_dimensions.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6855 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_zacks_eps_estimates.py
+-rw-r--r--   0 shawn      (503) staff       (20)     4742 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_options_realtime.py
+-rw-r--r--   0 shawn      (503) staff       (20)    11092 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/company_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)     4819 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_options_chain_eod.py
+-rw-r--r--   0 shawn      (503) staff       (20)    11473 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_moving_average_convergence_divergence.py
+-rw-r--r--   0 shawn      (503) staff       (20)    50157 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/realtime_stock_price.py
+-rw-r--r--   0 shawn      (503) staff       (20)     8435 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_company_fundamentals.py
+-rw-r--r--   0 shawn      (503) staff       (20)    10151 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/average_directional_index_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)    20554 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/stock_exchange.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6398 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_sic_indices.py
+-rw-r--r--   0 shawn      (503) staff       (20)    21288 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/fundamental.py
+-rw-r--r--   0 shawn      (503) staff       (20)    24303 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/economic_index.py
+-rw-r--r--   0 shawn      (503) staff       (20)    10977 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_negative_volume_index.py
+-rw-r--r--   0 shawn      (503) staff       (20)     7753 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/filing_note_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)    24804 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/option_price_realtime.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6226 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/mass_index_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)    13209 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/option_eod.py
+-rw-r--r--   0 shawn      (503) staff       (20)    10911 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_true_strength_index.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6388 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/ultimate_oscillator_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6560 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_owner_institutional_holdings.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6884 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_zacks_analyst_ratings_snapshot.py
+-rw-r--r--   0 shawn      (503) staff       (20)    37674 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/zacks_sales_surprise.py
+-rw-r--r--   0 shawn      (503) staff       (20)     4817 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/option_snapshots_result.py
+-rw-r--r--   0 shawn      (503) staff       (20)     8557 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/option_intervals_result.py
+-rw-r--r--   0 shawn      (503) staff       (20)    17338 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/fundamental_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)    14527 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/reported_tag.py
+-rw-r--r--   0 shawn      (503) staff       (20)    11142 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_triple_exponential_average.py
+-rw-r--r--   0 shawn      (503) staff       (20)     7396 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_zacks_long_term_growth_rates.py
+-rw-r--r--   0 shawn      (503) staff       (20)    10662 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/bollinger_bands_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6167 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/reported_financial_dimension.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6145 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/thea_source_document.py
+-rw-r--r--   0 shawn      (503) staff       (20)    12624 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/stock_price_adjustment_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)   136507 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/municipality_financial.py
+-rw-r--r--   0 shawn      (503) staff       (20)    10646 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_mass_index.py
+-rw-r--r--   0 shawn      (503) staff       (20)    10978 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_on_balance_volume_mean.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6644 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_company_shares_outstanding.py
+-rw-r--r--   0 shawn      (503) staff       (20)     8341 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/stochastic_oscillator_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)    52025 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/earnings_record.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6210 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/option_snapshot_group.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6549 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/triple_exponential_average_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)    11176 2023-06-14 13:32:14.000000 intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_average_daily_trading_volume.py
+drwxr-xr-x   0 shawn      (503) staff       (20)        0 2023-06-14 14:28:29.000000 intrinio-sdk-6.24.0/intrinio_sdk/api/
+-rw-r--r--   0 shawn      (503) staff       (20)    10452 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/api/data_point_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)    84166 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/api/index_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)    25579 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/api/owners_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)    26155 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/api/et_fs_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)    95784 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/api/company_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)    16465 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/api/municipality_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1157 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/api/__init__.py
+-rw-r--r--   0 shawn      (503) staff       (20)   342796 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/api/security_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)   213664 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/api/technical_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)   127971 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/api/options_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6358 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/api/insider_transaction_filings_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)     7996 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/api/historical_data_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)    31234 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/api/fundamentals_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)    30181 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/api/stock_exchange_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)    51756 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/api/filing_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)    14009 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/api/data_tag_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)    14832 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/api/forex_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)    74950 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/api/zacks_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)     4435 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/api/bulk_downloads_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)    22700 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/api/esg_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)    26891 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/intrinio_sdk/api_client.py
+-rw-r--r--   0 shawn      (503) staff       (20)      776 2023-06-14 14:28:29.000000 intrinio-sdk-6.24.0/PKG-INFO
+drwxr-xr-x   0 shawn      (503) staff       (20)        0 2023-06-14 14:28:29.000000 intrinio-sdk-6.24.0/intrinio_sdk.egg-info/
+-rw-r--r--   0 shawn      (503) staff       (20)      776 2023-06-14 14:28:29.000000 intrinio-sdk-6.24.0/intrinio_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 shawn      (503) staff       (20)    27065 2023-06-14 14:28:29.000000 intrinio-sdk-6.24.0/intrinio_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 shawn      (503) staff       (20)       64 2023-06-14 14:28:29.000000 intrinio-sdk-6.24.0/intrinio_sdk.egg-info/requires.txt
+-rw-r--r--   0 shawn      (503) staff       (20)       18 2023-06-14 14:28:29.000000 intrinio-sdk-6.24.0/intrinio_sdk.egg-info/top_level.txt
+-rw-r--r--   0 shawn      (503) staff       (20)        1 2023-06-14 14:28:29.000000 intrinio-sdk-6.24.0/intrinio_sdk.egg-info/dependency_links.txt
+drwxr-xr-x   0 shawn      (503) staff       (20)        0 2023-06-14 14:28:29.000000 intrinio-sdk-6.24.0/test/
+-rw-r--r--   0 shawn      (503) staff       (20)     1292 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_etf_holding.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1540 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_commodity_channel_index.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1500 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_ichimoku_kinko_hyo.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1458 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_zacks_analyst_ratings.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1546 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_institutional_ownership.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1440 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_company_securities.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1300 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_option_price.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1276 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_sic_index.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1582 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_stock_exchange_stock_price_adjustments.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1234 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_etf.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1442 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_filing_notes_search.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1382 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_option_factors_realtime.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1460 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_zacks_eps_growth_rates.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1326 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_data_tag_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1426 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_options_chain_eod.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1266 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_company.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1442 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_zacks_eps_surprises.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1466 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_options_chain_realtime.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1424 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_forex_currencies.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1350 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_esg_company_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1384 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_sic_indices.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1400 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_mass_index_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1292 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_stock_price.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1274 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_security.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1540 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_stock_price_adjustments.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1350 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_bulk_download_links.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1308 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_etf_analytics.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1376 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_esg_rating_with_company.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1466 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_volume_weighted_average_price_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1358 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_filings.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1432 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_option_intervals_movers_result.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1598 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_esg_company_comprehensive_rating_history.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1374 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_security_screen_result.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1382 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_security_interval_mover.py
+-rw-r--r--   0 shawn      (503) staff       (20)     4107 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_company_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1366 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_option_snapshot_group.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1408 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_security_screen_result_data.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1488 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_stochastic_oscillator_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1292 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_filing_note.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1484 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_sic_index_historical_data.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1442 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_williams_r.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1508 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_zacks_eps_surprises.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1432 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_stock_price_adjustment_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1466 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_options_stats_realtime.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1564 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_detrended_price_oscillator.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1300 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_reported_tag.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1400 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_option_prices.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1564 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_company_insider_transaction_filings.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1530 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_stochastic_oscillator.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1316 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_economic_index.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1424 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_realtime_stock_price_security.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1284 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_option_eod.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1316 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_stock_exchange.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1392 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_etf_holdings.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1356 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_technical_indicator.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1310 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_bulk_downloads_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1368 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_data_tags.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1422 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_reported_financial_dimension.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1506 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_awesome_oscillator.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1530 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_zacks_institutional_holding_company_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1424 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_economic_indices.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1562 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_standardized_financials_dimensions.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1514 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_ultimate_oscillator.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1366 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_option_price_realtime.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1408 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_option_price_batch_realtime.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1548 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_owner_insider_transaction_filings.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1490 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_vortex_indicator.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1500 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_chaikin_money_flow.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1448 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_security_intervals_movers_result.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1414 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_municipalities.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1416 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_historical_data.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1366 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_security_screen_group.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1358 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_realtime_stock_price.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1590 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_zacks_analyst_ratings_snapshot.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1476 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_know_sure_thing.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1482 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_esg_latest_comprehensive.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1506 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_insider_transaction_filings.py
+-rw-r--r--   0 shawn      (503) staff       (20)     6812 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_technical_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1482 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_intraday_prices.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1500 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_average_true_range.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1380 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_municipality_financial.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1484 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_on_balance_volume_mean_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1358 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_zacks_sales_surprise.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1482 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_esg_comprehensive_rating_with_company.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1400 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_zacks_eps_surprise_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1336 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_et_fs.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1524 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_economic_index_historical_data.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1464 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_awesome_oscillator_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1482 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_interval_prices.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1526 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_on_balance_volume_mean.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1424 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_options_realtime.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1360 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_zacks_eps_growth_rate.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1342 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_stock_market_index.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1342 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_thea_entity_answer.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1416 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_stock_exchanges.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1462 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_standardized_financials_dimension.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1448 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_reported_financials.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1324 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_earnings_record.py
+-rw-r--r--   0 shawn      (503) staff       (20)     3094 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_zacks_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1326 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_option_price_eod.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1358 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_thea_source_document.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1604 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_moving_average_convergence_divergence_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     2223 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_fundamentals_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1402 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_zacks_long_term_growth_rate.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1308 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_owner_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1498 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_commodity_channel_index_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1350 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_stock_price_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1406 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_insider_transaction_filing.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1458 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_stock_prices.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1482 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_negative_volume_index_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1484 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_ease_of_movement.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1458 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_ichimoku_kinko_hyo_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1514 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_zacks_institutional_holding_owner_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)        0 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/test/__init__.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1559 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_data_tag_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1366 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_bulk_download_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1522 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_triple_exponential_average_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1358 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_company_news_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1440 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_company_initial_public_offering.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1482 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_historical_data.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1384 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_forex_pairs.py
+-rw-r--r--   0 shawn      (503) staff       (20)     2673 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_filing_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1490 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_stock_exchange_securities.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1440 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_keltner_channel_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1398 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_security_snapshots_result.py
+-rw-r--r--   0 shawn      (503) staff       (20)     2236 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_stock_exchange_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1448 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_vortex_indicator_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1408 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_force_index_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1482 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_initial_public_offerings.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1558 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_forex_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1500 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_volume_price_trend.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1292 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_forex_price.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1434 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_zacks_etf_holdings.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1324 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_company_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1284 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_forex_pair.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1482 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_bollinger_bands.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1524 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_zacks_sales_surprises.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1582 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_volume_weighted_average_price.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1466 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_true_strength_index_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1516 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_options_prices_batch_realtime.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1556 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_zacks_institutional_holding_owners.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1448 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_filing_fundamentals.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1448 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_donchian_channel_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1390 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_esg_comprehensive_rating.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1392 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_forex_prices.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1382 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_option_intervals_result.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1366 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_option_stats_realtime.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1562 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_accumulation_distribution_index_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1434 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_sic_indices_search.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1458 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_average_true_range_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1448 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_options_expirations.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1434 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_know_sure_thing_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1522 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_detrended_price_oscillator_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1276 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_etf_stats.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1418 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_data_tags_search.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1400 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_esg_companies.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1442 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_ease_of_movement_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1482 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_keltner_channel.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1918 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_owners_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1458 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_chaikin_money_flow_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1482 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_options_unusual_activity.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1482 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_simple_moving_average_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1524 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_negative_volume_index.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1466 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_options_price_realtime.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1382 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_option_snapshots_result.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1522 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_zacks_institutional_holding_company_detail.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1500 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_stock_market_indices_search.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1500 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_stock_exchange_stock_prices.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1574 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_average_daily_trading_volume.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1456 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_company_fundamentals.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1564 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_triple_exponential_average.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1342 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_zacks_eps_surprise.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1284 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_esg_rating.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1342 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_filing_note_filing.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1488 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_municipalitiy_financials.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1392 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_company_news.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1374 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_stock_price_adjustment.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1342 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_zacks_eps_estimate.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1502 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_zacks_long_term_growth_rates.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1506 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_zacks_institutional_holding_owner_detail.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1442 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_money_flow_index_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1358 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_options.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1298 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_fundamental.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1356 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_fundamental_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1556 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_average_directional_index.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1434 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_options_prices_eod.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1550 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_stock_market_index_historical_data.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1648 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_municipality_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1498 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_company_shares_outstanding.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1484 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_money_flow_index.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1514 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_average_directional_index_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1366 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_option_chain_realtime.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1366 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_option_contracts_list.py
+-rw-r--r--   0 shawn      (503) staff       (20)    10454 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_security_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1424 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_zacks_analyst_rating_snapshot.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1458 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_zacks_sales_surprises.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1388 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_institutional_ownership.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1508 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_true_strength_index.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1416 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_options_tickers.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1514 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_owner_institutional_holdings.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1431 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_insider_transaction_filings_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1392 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_filing_notes.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1358 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_option_unusual_trade.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1300 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_option_chain.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1458 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_volume_price_trend_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1350 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_filing_note_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1258 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_option.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1416 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_zacks_target_price_consensus.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1292 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_etf_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1474 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_company_historical_data.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1498 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_relative_strength_index_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1416 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_zacks_sales_surprise_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1324 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_option_realtime.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1450 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_stock_market_indices.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1372 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_institutional_holding.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1350 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_owners.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1324 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_option_interval.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1450 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_force_index.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1524 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_zacks_analyst_ratings.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1408 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_filing_answers.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1268 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_data_tag.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1356 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_insider_transaction.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1380 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_standardized_financial.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1566 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_stock_exchange_realtime_stock_prices.py
+-rw-r--r--   0 shawn      (503) staff       (20)     5109 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_options_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1416 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_company_filings.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1472 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_ultimate_oscillator_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1432 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_company_recognize.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1376 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_esg_latest.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1934 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_esg_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1414 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_zacks_institutional_holding.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1374 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_security_screen_clause.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1406 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_company_shares_outstanding.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1440 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_bollinger_bands_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1324 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_historical_data.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1332 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_security_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1442 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_mass_index.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1432 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_securities_search.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1316 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_forex_currency.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1374 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_economic_index_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1524 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_simple_moving_average.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1258 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_filing.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1334 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_zacks_etf_holding.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1524 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_zacks_target_price_consensuses.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1416 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_zacks_analyst_rating_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1924 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_et_fs_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1554 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_zacks_institutional_holding_historical_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1604 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_accumulation_distribution_index.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1334 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_news.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1444 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_data_point_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1492 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_on_balance_volume.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1480 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_standardized_financials.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1400 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_stock_market_index_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1646 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_moving_average_convergence_divergence.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1316 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_filing_summary.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1514 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_zacks_institutional_holdings.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1382 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_security_snapshot_group.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1400 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_options_chain.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1366 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_option_interval_mover.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1424 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_companies_search.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1474 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_economic_indices_search.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1374 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_companies.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1450 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_on_balance_volume_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1492 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_esg_company_rating_history.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1416 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_company_answers.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1358 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_intraday_stock_price.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1348 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_reported_financial.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1540 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_relative_strength_index.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1442 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_bulk_download_links.py
+-rw-r--r--   0 shawn      (503) staff       (20)     4422 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_index_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1358 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_stock_price_interval.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1400 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_williams_r_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1532 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_average_daily_trading_volume_technical_value.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1300 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_company_news.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1382 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_securities.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1326 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_option_chain_eod.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1580 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_zacks_institutional_holding_companies.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1306 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_municipality.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1490 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_security_donchian_channel.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1316 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_company_filing.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1314 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_historical_data_api.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1358 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_zacks_analyst_rating.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1250 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_owner.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1442 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_api_response_zacks_eps_estimates.py
+-rw-r--r--   0 shawn      (503) staff       (20)     1324 2023-06-08 21:57:42.000000 intrinio-sdk-6.24.0/test/test_dividend_record.py
+-rw-r--r--   0 shawn      (503) staff       (20)    57162 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/README.md
+-rw-r--r--   0 shawn      (503) staff       (20)     1844 2023-06-14 13:32:15.000000 intrinio-sdk-6.24.0/setup.py
+-rw-r--r--   0 shawn      (503) staff       (20)       38 2023-06-14 14:28:29.000000 intrinio-sdk-6.24.0/setup.cfg
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/configuration.py` & `intrinio-sdk-6.24.0/intrinio_sdk/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
@@ -241,10 +241,10 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 2.39.2\n"\
-               "SDK Package Version: 6.23.1".\
+               "Version of the API: 2.42.0\n"\
+               "SDK Package Version: 6.24.0".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/rest.py` & `intrinio-sdk-6.24.0/intrinio_sdk/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/__init__.py` & `intrinio-sdk-6.24.0/intrinio_sdk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # flake8: noqa
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/zacks_target_price_consensus.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/zacks_target_price_consensus.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_zacks_sales_surprises.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_zacks_sales_surprises.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/detrended_price_oscillator_technical_value.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/detrended_price_oscillator_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/zacks_sales_surprise_summary.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/zacks_sales_surprise_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_options.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_municipalities.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_municipalities.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_williams_r.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_williams_r.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/forex_currency.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/forex_currency.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/zacks_institutional_holding_company_detail.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/zacks_institutional_holding_company_detail.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_vortex_indicator.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_vortex_indicator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_awesome_oscillator.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_awesome_oscillator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_securities_search.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_securities_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_company_filings.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_company_filings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_filing_notes.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_filing_notes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/williams_r_technical_value.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/williams_r_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_options_stats_realtime.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_options_stats_realtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/security_summary.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/security_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/stock_price_adjustment.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/stock_price_adjustment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_options_prices_batch_realtime.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_options_prices_batch_realtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_options_chain.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_options_chain.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_standardized_financials.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_standardized_financials.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/stock_market_index_summary.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/stock_market_index_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_sic_index_historical_data.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_sic_index_historical_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_company_news.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_company_news.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/option_unusual_trade.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/option_unusual_trade.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_data_tags_search.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_data_tags_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/institutional_holding.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/institutional_holding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_company_recognize.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_company_recognize.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_economic_indices_search.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_economic_indices_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/zacks_analyst_rating_summary.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/zacks_analyst_rating_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/etf_stats.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/etf_stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/standardized_financials_dimension.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/standardized_financials_dimension.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/zacks_long_term_growth_rate.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/zacks_long_term_growth_rate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_company_securities.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_company_securities.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/company.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/company.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_zacks_eps_growth_rates.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_zacks_eps_growth_rates.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/company_news.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/company_news.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/etf_analytics.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/etf_analytics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/reported_financial.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/reported_financial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/municipality.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/municipality.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/company_filing.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/company_filing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/company_shares_outstanding.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/company_shares_outstanding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_zacks_analyst_ratings.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_zacks_analyst_ratings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_filing_notes_search.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_filing_notes_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/force_index_technical_value.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/force_index_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_economic_index_historical_data.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_economic_index_historical_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/commodity_channel_index_technical_value.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/commodity_channel_index_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_company_answers.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_company_answers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_zacks_eps_surprises.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_zacks_eps_surprises.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_company_historical_data.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_company_historical_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/option_interval_mover.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/option_interval_mover.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/moving_average_convergence_divergence_technical_value.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/moving_average_convergence_divergence_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_forex_prices.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_forex_prices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_options_chain_realtime.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_options_chain_realtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/zacks_institutional_holding_owner_summary.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/zacks_institutional_holding_owner_summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/option.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/option.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/stock_price_summary.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/stock_price_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/filing_summary.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/filing_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/forex_price.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/forex_price.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_volume_weighted_average_price.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_volume_weighted_average_price.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/zacks_analyst_rating_snapshot.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/zacks_analyst_rating_snapshot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_ichimoku_kinko_hyo.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_ichimoku_kinko_hyo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/volume_weighted_average_price_value.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/volume_weighted_average_price_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/option_chain_eod.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/option_chain_eod.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/bulk_download_links.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/bulk_download_links.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_volume_price_trend.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_volume_price_trend.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/etf_holding.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/etf_holding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/simple_moving_average_technical_value.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/simple_moving_average_technical_value.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_options_unusual_activity.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_options_unusual_activity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/zacks_institutional_holding_company_summary.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/zacks_institutional_holding_company_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_stock_exchange_securities.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_stock_exchange_securities.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_stock_exchange_stock_price_adjustments.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_stock_exchange_stock_price_adjustments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_keltner_channel.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_keltner_channel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_stock_prices.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_stock_prices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_stochastic_oscillator.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_stochastic_oscillator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/ichimoku_kinko_hyo_technical_value.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/ichimoku_kinko_hyo_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_stock_market_index_historical_data.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_stock_market_index_historical_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/company_initial_public_offering.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/company_initial_public_offering.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/esg_company_summary.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/esg_company_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/etf.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/etf.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 000001d0: 5d28 6874 7470 733a 2f2f 696e 7472 696e  ](https://intrin
 000001e0: 696f 2e63 6f6d 2920 616e 6420 636c 6963  io.com) and clic
 000001f0: 6b20 6f6e 2074 6865 2063 6861 7420 6963  k on the chat ic
 00000200: 6f6e 2069 6e20 7468 6520 6c6f 7765 7220  on in the lower 
 00000210: 7269 6768 7420 636f 726e 6572 2e20 2023  right corner.  #
 00000220: 206e 6f71 613a 2045 3530 310a 0a20 2020   noqa: E501..   
 00000230: 204f 7065 6e41 5049 2073 7065 6320 7665   OpenAPI spec ve
-00000240: 7273 696f 6e3a 2032 2e33 392e 320a 2020  rsion: 2.39.2.  
+00000240: 7273 696f 6e3a 2032 2e34 322e 300a 2020  rsion: 2.42.0.  
 00000250: 2020 0a20 2020 2047 656e 6572 6174 6564    .    Generated
 00000260: 2062 793a 2068 7474 7073 3a2f 2f67 6974   by: https://git
 00000270: 6875 622e 636f 6d2f 7377 6167 6765 722d  hub.com/swagger-
 00000280: 6170 692f 7377 6167 6765 722d 636f 6465  api/swagger-code
 00000290: 6765 6e2e 6769 740a 2222 220a 0a0a 696d  gen.git."""...im
 000002a0: 706f 7274 2070 7072 696e 740a 696d 706f  port pprint.impo
 000002b0: 7274 2072 6520 2023 206e 6f71 613a 2046  rt re  # noqa: F
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_average_directional_index.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_average_directional_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_ease_of_movement.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_ease_of_movement.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/stock_price.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/stock_price.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/owner_summary.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/owner_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/zacks_etf_holding.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/zacks_etf_holding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/keltner_channel_technical_value.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/keltner_channel_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/vortex_indicator_technical_value.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/vortex_indicator_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/security_interval_mover.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/security_interval_mover.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/intraday_stock_price.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/intraday_stock_price.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/stock_price_interval.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/stock_price_interval.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/option_stats_realtime.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/option_stats_realtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/security.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/security.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_zacks_etf_holdings.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_zacks_etf_holdings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/filing.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/filing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/true_strength_index_technical_value.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/true_strength_index_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/dividend_record.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/dividend_record.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/average_daily_trading_volume_technical_value.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/average_daily_trading_volume_technical_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/zacks_analyst_rating.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/zacks_analyst_rating.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_companies.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_companies.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/option_chain.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/option_chain.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/security_intervals_movers_result.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/security_intervals_movers_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/zacks_institutional_holding_historical_summary.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/zacks_institutional_holding_historical_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_zacks_institutional_holding_owners.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_zacks_institutional_holding_owners.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_companies_search.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_companies_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/security_screen_clause.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/security_screen_clause.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/security_screen_result_data.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/security_screen_result_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/awesome_oscillator_technical_value.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/awesome_oscillator_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/option_realtime.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/option_realtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/filing_note.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/filing_note.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/__init__.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/accumulation_distribution_index_technical_value.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/accumulation_distribution_index_technical_value.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_news.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_news.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_ultimate_oscillator.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_ultimate_oscillator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/option_contracts_list.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/option_contracts_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/economic_index_summary.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/economic_index_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/option_interval.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/option_interval.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_relative_strength_index.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_relative_strength_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_esg_companies.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_esg_companies.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/technical_indicator.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/technical_indicator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/option_chain_realtime.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/option_chain_realtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/esg_rating_with_company.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/esg_rating_with_company.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/owner.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/owner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/historical_data.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/historical_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_insider_transaction_filings.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_insider_transaction_filings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_average_true_range.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_average_true_range.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_esg_company_comprehensive_rating_history.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_esg_company_comprehensive_rating_history.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/esg_comprehensive_rating.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/esg_comprehensive_rating.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/zacks_eps_surprise.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/zacks_eps_surprise.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_zacks_eps_surprises.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_zacks_eps_surprises.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_options_tickers.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_options_tickers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/filing_note_filing.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/filing_note_filing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/standardized_financial.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/standardized_financial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_company_insider_transaction_filings.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_company_insider_transaction_filings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/esg_rating.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/esg_rating.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_reported_financials.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_reported_financials.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_chaikin_money_flow.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_chaikin_money_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/zacks_eps_estimate.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/zacks_eps_estimate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/option_price_batch_realtime.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/option_price_batch_realtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_municipalitiy_financials.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_municipalitiy_financials.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/option_factors_realtime.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/option_factors_realtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/on_balance_volume_mean_technical_value.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/on_balance_volume_mean_technical_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_detrended_price_oscillator.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_detrended_price_oscillator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/thea_entity_answer.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/thea_entity_answer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_securities.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_securities.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/data_tag.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/data_tag.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_data_tags.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_data_tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/etf_summary.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/etf_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_historical_data.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_historical_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_etf_holdings.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_etf_holdings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/money_flow_index_technical_value.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/money_flow_index_technical_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_interval_prices.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_interval_prices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_accumulation_distribution_index.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_accumulation_distribution_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/zacks_eps_growth_rate.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/zacks_eps_growth_rate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_stock_price_adjustments.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_stock_price_adjustments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_filing_answers.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_filing_answers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_options_prices_eod.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_options_prices_eod.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/stock_market_index.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/stock_market_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/on_balance_volume_technical_value.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/on_balance_volume_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/insider_transaction.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/insider_transaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/relative_strength_index_technical_value.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/relative_strength_index_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/option_price_eod.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/option_price_eod.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_intraday_prices.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_intraday_prices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/zacks_institutional_holding.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/zacks_institutional_holding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_et_fs.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_et_fs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_zacks_institutional_holding_companies.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_zacks_institutional_holding_companies.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/volume_price_trend_technical_value.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/volume_price_trend_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/esg_comprehensive_rating_with_company.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/esg_comprehensive_rating_with_company.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_stock_exchanges.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_stock_exchanges.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/zacks_institutional_holding_owner_detail.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/zacks_institutional_holding_owner_detail.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/security_screen_group.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/security_screen_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_money_flow_index.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_money_flow_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_forex_currencies.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_forex_currencies.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_forex_pairs.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_forex_pairs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_know_sure_thing.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_know_sure_thing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_esg_latest_comprehensive.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_esg_latest_comprehensive.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_commodity_channel_index.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_commodity_channel_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/insider_transaction_filing.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/insider_transaction_filing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_zacks_sales_surprises.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_zacks_sales_surprises.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/security_snapshot_group.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/security_snapshot_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_institutional_ownership.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_institutional_ownership.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_owners.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_owners.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/donchian_channel_technical_value.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/donchian_channel_technical_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_simple_moving_average.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_simple_moving_average.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_stock_market_indices_search.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_stock_market_indices_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_filing_fundamentals.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_filing_fundamentals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_stock_exchange_stock_prices.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_stock_exchange_stock_prices.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/forex_pair.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/forex_pair.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_esg_company_rating_history.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_esg_company_rating_history.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_zacks_target_price_consensuses.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_zacks_target_price_consensuses.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/average_true_range_technical_value.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/average_true_range_technical_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_bollinger_bands.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_bollinger_bands.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_initial_public_offerings.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_initial_public_offerings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_sic_indices_search.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_sic_indices_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_options_expirations.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_options_expirations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/security_screen_result.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/security_screen_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/know_sure_thing_technical_value.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/know_sure_thing_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/chaikin_money_flow_technical_value.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/chaikin_money_flow_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_historical_data.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_historical_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_economic_indices.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_economic_indices.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/zacks_eps_surprise_summary.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/zacks_eps_surprise_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_on_balance_volume.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_on_balance_volume.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_zacks_analyst_ratings.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_zacks_analyst_ratings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_stock_exchange_realtime_stock_prices.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_stock_exchange_realtime_stock_prices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/ease_of_movement_technical_value.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/ease_of_movement_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/bulk_download_summary.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/bulk_download_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_force_index.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_force_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_zacks_institutional_holdings.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_zacks_institutional_holdings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_stock_market_indices.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_stock_market_indices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_esg_latest.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_esg_latest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/realtime_stock_price_security.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/realtime_stock_price_security.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_options_price_realtime.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_options_price_realtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_owner_insider_transaction_filings.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_owner_insider_transaction_filings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_filings.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_filings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/negative_volume_index_technical_value.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/negative_volume_index_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/sic_index.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/sic_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/security_snapshots_result.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/security_snapshots_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/institutional_ownership.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/institutional_ownership.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/data_tag_summary.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/data_tag_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/company_news_summary.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/company_news_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/option_intervals_movers_result.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/option_intervals_movers_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_donchian_channel.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_donchian_channel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_bulk_download_links.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_bulk_download_links.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_option_prices.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_option_prices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/option_price.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/option_price.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_standardized_financials_dimensions.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_standardized_financials_dimensions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_zacks_eps_estimates.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_zacks_eps_estimates.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_options_realtime.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_options_realtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/company_summary.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/company_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_options_chain_eod.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_options_chain_eod.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_moving_average_convergence_divergence.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_moving_average_convergence_divergence.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_company_fundamentals.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_company_fundamentals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/average_directional_index_technical_value.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/average_directional_index_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/stock_exchange.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/stock_exchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_sic_indices.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_sic_indices.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/fundamental.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/fundamental.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/economic_index.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/economic_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_negative_volume_index.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_negative_volume_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/filing_note_summary.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/filing_note_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/option_price_realtime.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/option_price_realtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/mass_index_technical_value.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/mass_index_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/option_eod.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/option_eod.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_true_strength_index.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_true_strength_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/ultimate_oscillator_technical_value.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/ultimate_oscillator_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_owner_institutional_holdings.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_owner_institutional_holdings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_zacks_analyst_ratings_snapshot.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_zacks_analyst_ratings_snapshot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/zacks_sales_surprise.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/zacks_sales_surprise.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/option_snapshots_result.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/option_snapshots_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/option_intervals_result.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/option_intervals_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/fundamental_summary.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/fundamental_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/reported_tag.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/reported_tag.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_triple_exponential_average.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_triple_exponential_average.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_zacks_long_term_growth_rates.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_zacks_long_term_growth_rates.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/bollinger_bands_technical_value.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/bollinger_bands_technical_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/reported_financial_dimension.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/reported_financial_dimension.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/thea_source_document.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/thea_source_document.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/stock_price_adjustment_summary.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/stock_price_adjustment_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/municipality_financial.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/municipality_financial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_mass_index.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_mass_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_on_balance_volume_mean.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_on_balance_volume_mean.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_company_shares_outstanding.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_company_shares_outstanding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/stochastic_oscillator_technical_value.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/stochastic_oscillator_technical_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/earnings_record.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/earnings_record.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/option_snapshot_group.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/option_snapshot_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/triple_exponential_average_technical_value.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/triple_exponential_average_technical_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/models/api_response_security_average_daily_trading_volume.py` & `intrinio-sdk-6.24.0/intrinio_sdk/models/api_response_security_average_daily_trading_volume.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/api/data_point_api.py` & `intrinio-sdk-6.24.0/intrinio_sdk/api/data_point_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/api/index_api.py` & `intrinio-sdk-6.24.0/intrinio_sdk/api/index_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/api/owners_api.py` & `intrinio-sdk-6.24.0/intrinio_sdk/api/owners_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/api/et_fs_api.py` & `intrinio-sdk-6.24.0/intrinio_sdk/api/et_fs_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
@@ -228,15 +228,15 @@
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_etf_analytics(self, identifier, **kwargs):  # noqa: E501
         """ETF Analytics  # noqa: E501
 
-        Returns latest market analytics for a specified US ETF, including volume, trailing volumen, market cap, 52 week high, and 52 week low.  # noqa: E501
+        Returns latest market analytics for a specified US ETF, including volume, trailing volume, market cap, 52 week high, and 52 week low.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async=True
         >>> thread = api.get_etf_analytics(identifier, _async=True)
         >>> result = thread.get()
 
         :param async bool
         :param str identifier: An ETF identifier (Ticker, Figi Ticker, ISIN, RIC, Intrinio ID) (required)
@@ -250,15 +250,15 @@
         else:
             (data) = self.get_etf_analytics_with_http_info(identifier, **kwargs)  # noqa: E501
             return data
 
     def get_etf_analytics_with_http_info(self, identifier, **kwargs):  # noqa: E501
         """ETF Analytics  # noqa: E501
 
-        Returns latest market analytics for a specified US ETF, including volume, trailing volumen, market cap, 52 week high, and 52 week low.  # noqa: E501
+        Returns latest market analytics for a specified US ETF, including volume, trailing volume, market cap, 52 week high, and 52 week low.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async=True
         >>> thread = api.get_etf_analytics_with_http_info(identifier, _async=True)
         >>> result = thread.get()
 
         :param async bool
         :param str identifier: An ETF identifier (Ticker, Figi Ticker, ISIN, RIC, Intrinio ID) (required)
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/api/company_api.py` & `intrinio-sdk-6.24.0/intrinio_sdk/api/company_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/api/municipality_api.py` & `intrinio-sdk-6.24.0/intrinio_sdk/api/municipality_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/api/__init__.py` & `intrinio-sdk-6.24.0/intrinio_sdk/api/__init__.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/api/security_api.py` & `intrinio-sdk-6.24.0/intrinio_sdk/api/security_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 000001d0: 5d28 6874 7470 733a 2f2f 696e 7472 696e  ](https://intrin
 000001e0: 696f 2e63 6f6d 2920 616e 6420 636c 6963  io.com) and clic
 000001f0: 6b20 6f6e 2074 6865 2063 6861 7420 6963  k on the chat ic
 00000200: 6f6e 2069 6e20 7468 6520 6c6f 7765 7220  on in the lower 
 00000210: 7269 6768 7420 636f 726e 6572 2e20 2023  right corner.  #
 00000220: 206e 6f71 613a 2045 3530 310a 0a20 2020   noqa: E501..   
 00000230: 204f 7065 6e41 5049 2073 7065 6320 7665   OpenAPI spec ve
-00000240: 7273 696f 6e3a 2032 2e33 392e 320a 2020  rsion: 2.39.2.  
+00000240: 7273 696f 6e3a 2032 2e34 322e 300a 2020  rsion: 2.42.0.  
 00000250: 2020 0a20 2020 2047 656e 6572 6174 6564    .    Generated
 00000260: 2062 793a 2068 7474 7073 3a2f 2f67 6974   by: https://git
 00000270: 6875 622e 636f 6d2f 7377 6167 6765 722d  hub.com/swagger-
 00000280: 6170 692f 7377 6167 6765 722d 636f 6465  api/swagger-code
 00000290: 6765 6e2e 6769 740a 2222 220a 0a0a 6672  gen.git."""...fr
 000002a0: 6f6d 205f 5f66 7574 7572 655f 5f20 696d  om __future__ im
 000002b0: 706f 7274 2061 6273 6f6c 7574 655f 696d  port absolute_im
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/api/technical_api.py` & `intrinio-sdk-6.24.0/intrinio_sdk/api/technical_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/api/options_api.py` & `intrinio-sdk-6.24.0/intrinio_sdk/api/options_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
@@ -117,17 +117,17 @@
             _async=params.get('async'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_option_expirations_realtime(self, symbol, **kwargs):  # noqa: E501
-        """Option Expirations Realtime  # noqa: E501
+        """Options Expirations  # noqa: E501
 
-        Returns a list of all current and upcoming expiration dates for a particular symbol.  # noqa: E501
+        Returns a list of all current and upcoming option contract expiration dates for a particular symbol.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async=True
         >>> thread = api.get_option_expirations_realtime(symbol, _async=True)
         >>> result = thread.get()
 
         :param async bool
         :param str symbol: The option symbol, corresponding to the underlying security. (required)
@@ -142,17 +142,17 @@
         if kwargs.get('async'):
             return self.get_option_expirations_realtime_with_http_info(symbol, **kwargs)  # noqa: E501
         else:
             (data) = self.get_option_expirations_realtime_with_http_info(symbol, **kwargs)  # noqa: E501
             return data
 
     def get_option_expirations_realtime_with_http_info(self, symbol, **kwargs):  # noqa: E501
-        """Option Expirations Realtime  # noqa: E501
+        """Options Expirations  # noqa: E501
 
-        Returns a list of all current and upcoming expiration dates for a particular symbol.  # noqa: E501
+        Returns a list of all current and upcoming option contract expiration dates for a particular symbol.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async=True
         >>> thread = api.get_option_expirations_realtime_with_http_info(symbol, _async=True)
         >>> result = thread.get()
 
         :param async bool
         :param str symbol: The option symbol, corresponding to the underlying security. (required)
@@ -329,15 +329,15 @@
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_options(self, symbol, **kwargs):  # noqa: E501
         """Options  # noqa: E501
 
-        Returns a list of all securities that have options listed and are tradable on a US market exchange. Useful to retrieve the entire universe.  # noqa: E501
+        Returns a list of all securities that have options listed and are tradable on a US market exchange. Useful to retrieve the entire universe.  Available via a 3rd party, contact sales for a trial.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async=True
         >>> thread = api.get_options(symbol, _async=True)
         >>> result = thread.get()
 
         :param async bool
         :param str symbol: The option symbol, corresponding to the underlying security. (required)
@@ -360,15 +360,15 @@
         else:
             (data) = self.get_options_with_http_info(symbol, **kwargs)  # noqa: E501
             return data
 
     def get_options_with_http_info(self, symbol, **kwargs):  # noqa: E501
         """Options  # noqa: E501
 
-        Returns a list of all securities that have options listed and are tradable on a US market exchange. Useful to retrieve the entire universe.  # noqa: E501
+        Returns a list of all securities that have options listed and are tradable on a US market exchange. Useful to retrieve the entire universe.  Available via a 3rd party, contact sales for a trial.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async=True
         >>> thread = api.get_options_with_http_info(symbol, _async=True)
         >>> result = thread.get()
 
         :param async bool
         :param str symbol: The option symbol, corresponding to the underlying security. (required)
@@ -589,15 +589,15 @@
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_options_chain(self, symbol, expiration, **kwargs):  # noqa: E501
         """Options Chain  # noqa: E501
 
-        Returns a list of the historical end-of-day top of the order book size and premium (bid / ask), the latest trade size and premium as well as the greeks and implied volatility for all option contracts currently associated with the option chain.  # noqa: E501
+        Returns a list of the historical end-of-day top of the order book size and premium (bid / ask), the latest trade size and premium as well as the greeks and implied volatility for all option contracts currently associated with the option chain.  Available via a 3rd party, contact sales for a trial.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async=True
         >>> thread = api.get_options_chain(symbol, expiration, _async=True)
         >>> result = thread.get()
 
         :param async bool
         :param str symbol: The option symbol, corresponding to the underlying security. (required)
@@ -619,15 +619,15 @@
         else:
             (data) = self.get_options_chain_with_http_info(symbol, expiration, **kwargs)  # noqa: E501
             return data
 
     def get_options_chain_with_http_info(self, symbol, expiration, **kwargs):  # noqa: E501
         """Options Chain  # noqa: E501
 
-        Returns a list of the historical end-of-day top of the order book size and premium (bid / ask), the latest trade size and premium as well as the greeks and implied volatility for all option contracts currently associated with the option chain.  # noqa: E501
+        Returns a list of the historical end-of-day top of the order book size and premium (bid / ask), the latest trade size and premium as well as the greeks and implied volatility for all option contracts currently associated with the option chain.  Available via a 3rd party, contact sales for a trial.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async=True
         >>> thread = api.get_options_chain_with_http_info(symbol, expiration, _async=True)
         >>> result = thread.get()
 
         :param async bool
         :param str symbol: The option symbol, corresponding to the underlying security. (required)
@@ -988,15 +988,15 @@
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_options_expirations(self, symbol, **kwargs):  # noqa: E501
         """Options Expirations  # noqa: E501
 
-        Returns a list of all current and upcoming option contract expiration dates for a particular symbol.  # noqa: E501
+        Returns a list of all current and upcoming option contract expiration dates for a particular symbol.  Available via a 3rd party, contact sales for a trial.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async=True
         >>> thread = api.get_options_expirations(symbol, _async=True)
         >>> result = thread.get()
 
         :param async bool
         :param str symbol: The option symbol, corresponding to the underlying security. (required)
@@ -1012,15 +1012,15 @@
         else:
             (data) = self.get_options_expirations_with_http_info(symbol, **kwargs)  # noqa: E501
             return data
 
     def get_options_expirations_with_http_info(self, symbol, **kwargs):  # noqa: E501
         """Options Expirations  # noqa: E501
 
-        Returns a list of all current and upcoming option contract expiration dates for a particular symbol.  # noqa: E501
+        Returns a list of all current and upcoming option contract expiration dates for a particular symbol.  Available via a 3rd party, contact sales for a trial.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async=True
         >>> thread = api.get_options_expirations_with_http_info(symbol, _async=True)
         >>> result = thread.get()
 
         :param async bool
         :param str symbol: The option symbol, corresponding to the underlying security. (required)
@@ -1081,14 +1081,117 @@
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='ApiResponseOptionsExpirations',  # noqa: E501
+            auth_settings=auth_settings,
+            _async=params.get('async'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def get_options_expirations_eod(self, symbol, **kwargs):  # noqa: E501
+        """Options Expirations  # noqa: E501
+
+        Returns a list of all current and upcoming option contract expiration dates for a particular symbol.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async=True
+        >>> thread = api.get_options_expirations_eod(symbol, _async=True)
+        >>> result = thread.get()
+
+        :param async bool
+        :param str symbol: The option symbol, corresponding to the underlying security. (required)
+        :param str after: Return option contract expiration dates after this date.
+        :param str before: Return option contract expiration dates before this date.
+        :return: ApiResponseOptionsExpirations
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async'):
+            return self.get_options_expirations_eod_with_http_info(symbol, **kwargs)  # noqa: E501
+        else:
+            (data) = self.get_options_expirations_eod_with_http_info(symbol, **kwargs)  # noqa: E501
+            return data
+
+    def get_options_expirations_eod_with_http_info(self, symbol, **kwargs):  # noqa: E501
+        """Options Expirations  # noqa: E501
+
+        Returns a list of all current and upcoming option contract expiration dates for a particular symbol.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async=True
+        >>> thread = api.get_options_expirations_eod_with_http_info(symbol, _async=True)
+        >>> result = thread.get()
+
+        :param async bool
+        :param str symbol: The option symbol, corresponding to the underlying security. (required)
+        :param str after: Return option contract expiration dates after this date.
+        :param str before: Return option contract expiration dates before this date.
+        :return: ApiResponseOptionsExpirations
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['symbol', 'after', 'before']  # noqa: E501
+        all_params.append('async')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_options_expirations_eod" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'symbol' is set
+        if ('symbol' not in params or
+                params['symbol'] is None):
+            raise ValueError("Missing the required parameter `symbol` when calling `get_options_expirations_eod`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'symbol' in params:
+            path_params['symbol'] = params['symbol']  # noqa: E501
+
+        query_params = []
+        if 'after' in params:
+            query_params.append(('after', params['after']))  # noqa: E501
+        if 'before' in params:
+            query_params.append(('before', params['before']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['ApiKeyAuth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/options/expirations/{symbol}/eod', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='ApiResponseOptionsExpirations',  # noqa: E501
             auth_settings=auth_settings,
             _async=params.get('async'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/api/insider_transaction_filings_api.py` & `intrinio-sdk-6.24.0/intrinio_sdk/api/insider_transaction_filings_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/api/historical_data_api.py` & `intrinio-sdk-6.24.0/intrinio_sdk/api/historical_data_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/api/fundamentals_api.py` & `intrinio-sdk-6.24.0/intrinio_sdk/api/fundamentals_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/api/stock_exchange_api.py` & `intrinio-sdk-6.24.0/intrinio_sdk/api/stock_exchange_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/api/filing_api.py` & `intrinio-sdk-6.24.0/intrinio_sdk/api/filing_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/api/data_tag_api.py` & `intrinio-sdk-6.24.0/intrinio_sdk/api/data_tag_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/api/forex_api.py` & `intrinio-sdk-6.24.0/intrinio_sdk/api/forex_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/api/zacks_api.py` & `intrinio-sdk-6.24.0/intrinio_sdk/api/zacks_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/api/bulk_downloads_api.py` & `intrinio-sdk-6.24.0/intrinio_sdk/api/bulk_downloads_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/api/esg_api.py` & `intrinio-sdk-6.24.0/intrinio_sdk/api/esg_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk/api_client.py` & `intrinio-sdk-6.24.0/intrinio_sdk/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import datetime
@@ -72,15 +72,15 @@
         self.pool = ThreadPool()
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/6.23.1/python'
+        self.user_agent = 'Swagger-Codegen/6.24.0/python'
 
     def __del__(self):
         self.pool.close()
         self.pool.join()
 
     @property
     def user_agent(self):
```

### Comparing `intrinio-sdk-6.23.1/PKG-INFO` & `intrinio-sdk-6.24.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: intrinio-sdk
-Version: 6.23.1
+Version: 6.24.0
 Summary: Intrinio API
 Home-page: https://github.com/intrinio/python-sdk
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: UNKNOWN
 Description:     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk.egg-info/PKG-INFO` & `intrinio-sdk-6.24.0/intrinio_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: intrinio-sdk
-Version: 6.23.1
+Version: 6.24.0
 Summary: Intrinio API
 Home-page: https://github.com/intrinio/python-sdk
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: UNKNOWN
 Description:     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
```

### Comparing `intrinio-sdk-6.23.1/intrinio_sdk.egg-info/SOURCES.txt` & `intrinio-sdk-6.24.0/intrinio_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_etf_holding.py` & `intrinio-sdk-6.24.0/test/test_etf_holding.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_commodity_channel_index.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_commodity_channel_index.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_ichimoku_kinko_hyo.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_ichimoku_kinko_hyo.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_zacks_analyst_ratings.py` & `intrinio-sdk-6.24.0/test/test_api_response_zacks_analyst_ratings.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_institutional_ownership.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_company_securities.py` & `intrinio-sdk-6.24.0/test/test_api_response_company_securities.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_option_price.py` & `intrinio-sdk-6.24.0/test/test_option_price.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_sic_index.py` & `intrinio-sdk-6.24.0/test/test_sic_index.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_stock_exchange_stock_price_adjustments.py` & `intrinio-sdk-6.24.0/test/test_api_response_stock_exchange_stock_price_adjustments.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_etf.py` & `intrinio-sdk-6.24.0/test/test_etf.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_filing_notes_search.py` & `intrinio-sdk-6.24.0/test/test_api_response_filing_notes_search.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_option_factors_realtime.py` & `intrinio-sdk-6.24.0/test/test_option_factors_realtime.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_zacks_eps_growth_rates.py` & `intrinio-sdk-6.24.0/test/test_api_response_zacks_eps_growth_rates.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_data_tag_summary.py` & `intrinio-sdk-6.24.0/test/test_data_tag_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_options_chain_eod.py` & `intrinio-sdk-6.24.0/test/test_api_response_options_chain_eod.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_company.py` & `intrinio-sdk-6.24.0/test/test_company.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_zacks_eps_surprises.py` & `intrinio-sdk-6.24.0/test/test_api_response_zacks_eps_surprises.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_options_chain_realtime.py` & `intrinio-sdk-6.24.0/test/test_api_response_options_chain_realtime.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_forex_currencies.py` & `intrinio-sdk-6.24.0/test/test_api_response_forex_currencies.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_esg_company_summary.py` & `intrinio-sdk-6.24.0/test/test_esg_company_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_sic_indices.py` & `intrinio-sdk-6.24.0/test/test_api_response_sic_indices.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_mass_index_technical_value.py` & `intrinio-sdk-6.24.0/test/test_mass_index_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_stock_price.py` & `intrinio-sdk-6.24.0/test/test_stock_price.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_security.py` & `intrinio-sdk-6.24.0/test/test_security.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_stock_price_adjustments.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_stock_price_adjustments.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_bulk_download_links.py` & `intrinio-sdk-6.24.0/test/test_bulk_download_links.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_etf_analytics.py` & `intrinio-sdk-6.24.0/test/test_etf_analytics.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_esg_rating_with_company.py` & `intrinio-sdk-6.24.0/test/test_esg_rating_with_company.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_volume_weighted_average_price_value.py` & `intrinio-sdk-6.24.0/test/test_volume_weighted_average_price_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_filings.py` & `intrinio-sdk-6.24.0/test/test_api_response_filings.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_option_intervals_movers_result.py` & `intrinio-sdk-6.24.0/test/test_option_intervals_movers_result.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_esg_company_comprehensive_rating_history.py` & `intrinio-sdk-6.24.0/test/test_api_response_esg_company_comprehensive_rating_history.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_security_screen_result.py` & `intrinio-sdk-6.24.0/test/test_security_screen_result.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_security_interval_mover.py` & `intrinio-sdk-6.24.0/test/test_security_interval_mover.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_company_api.py` & `intrinio-sdk-6.24.0/test/test_company_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_option_snapshot_group.py` & `intrinio-sdk-6.24.0/test/test_option_snapshot_group.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_security_screen_result_data.py` & `intrinio-sdk-6.24.0/test/test_security_screen_result_data.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_stochastic_oscillator_technical_value.py` & `intrinio-sdk-6.24.0/test/test_stochastic_oscillator_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_filing_note.py` & `intrinio-sdk-6.24.0/test/test_filing_note.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_sic_index_historical_data.py` & `intrinio-sdk-6.24.0/test/test_api_response_sic_index_historical_data.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_williams_r.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_williams_r.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_zacks_eps_surprises.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_zacks_eps_surprises.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_stock_price_adjustment_summary.py` & `intrinio-sdk-6.24.0/test/test_stock_price_adjustment_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_options_stats_realtime.py` & `intrinio-sdk-6.24.0/test/test_api_response_options_stats_realtime.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_detrended_price_oscillator.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_detrended_price_oscillator.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_reported_tag.py` & `intrinio-sdk-6.24.0/test/test_reported_tag.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_option_prices.py` & `intrinio-sdk-6.24.0/test/test_api_response_option_prices.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_company_insider_transaction_filings.py` & `intrinio-sdk-6.24.0/test/test_api_response_company_insider_transaction_filings.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_stochastic_oscillator.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_stochastic_oscillator.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_economic_index.py` & `intrinio-sdk-6.24.0/test/test_economic_index.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_realtime_stock_price_security.py` & `intrinio-sdk-6.24.0/test/test_realtime_stock_price_security.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_option_eod.py` & `intrinio-sdk-6.24.0/test/test_option_eod.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_stock_exchange.py` & `intrinio-sdk-6.24.0/test/test_stock_exchange.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_etf_holdings.py` & `intrinio-sdk-6.24.0/test/test_api_response_etf_holdings.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_technical_indicator.py` & `intrinio-sdk-6.24.0/test/test_technical_indicator.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_bulk_downloads_api.py` & `intrinio-sdk-6.24.0/test/test_bulk_downloads_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_data_tags.py` & `intrinio-sdk-6.24.0/test/test_api_response_data_tags.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_reported_financial_dimension.py` & `intrinio-sdk-6.24.0/test/test_reported_financial_dimension.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_awesome_oscillator.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_awesome_oscillator.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_zacks_institutional_holding_company_summary.py` & `intrinio-sdk-6.24.0/test/test_zacks_institutional_holding_company_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_economic_indices.py` & `intrinio-sdk-6.24.0/test/test_api_response_economic_indices.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_standardized_financials_dimensions.py` & `intrinio-sdk-6.24.0/test/test_api_response_standardized_financials_dimensions.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_ultimate_oscillator.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_ultimate_oscillator.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_option_price_realtime.py` & `intrinio-sdk-6.24.0/test/test_option_price_realtime.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_option_price_batch_realtime.py` & `intrinio-sdk-6.24.0/test/test_option_price_batch_realtime.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_owner_insider_transaction_filings.py` & `intrinio-sdk-6.24.0/test/test_api_response_owner_insider_transaction_filings.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_vortex_indicator.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_vortex_indicator.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_chaikin_money_flow.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_chaikin_money_flow.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_security_intervals_movers_result.py` & `intrinio-sdk-6.24.0/test/test_security_intervals_movers_result.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_municipalities.py` & `intrinio-sdk-6.24.0/test/test_api_response_municipalities.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_historical_data.py` & `intrinio-sdk-6.24.0/test/test_api_response_historical_data.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_security_screen_group.py` & `intrinio-sdk-6.24.0/test/test_security_screen_group.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_realtime_stock_price.py` & `intrinio-sdk-6.24.0/test/test_realtime_stock_price.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_zacks_analyst_ratings_snapshot.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_zacks_analyst_ratings_snapshot.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_know_sure_thing.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_know_sure_thing.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_esg_latest_comprehensive.py` & `intrinio-sdk-6.24.0/test/test_api_response_esg_latest_comprehensive.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_insider_transaction_filings.py` & `intrinio-sdk-6.24.0/test/test_api_response_insider_transaction_filings.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_technical_api.py` & `intrinio-sdk-6.24.0/test/test_technical_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_intraday_prices.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_intraday_prices.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_average_true_range.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_average_true_range.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_municipality_financial.py` & `intrinio-sdk-6.24.0/test/test_municipality_financial.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_on_balance_volume_mean_technical_value.py` & `intrinio-sdk-6.24.0/test/test_on_balance_volume_mean_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_zacks_sales_surprise.py` & `intrinio-sdk-6.24.0/test/test_zacks_sales_surprise.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_esg_comprehensive_rating_with_company.py` & `intrinio-sdk-6.24.0/test/test_esg_comprehensive_rating_with_company.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_zacks_eps_surprise_summary.py` & `intrinio-sdk-6.24.0/test/test_zacks_eps_surprise_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_et_fs.py` & `intrinio-sdk-6.24.0/test/test_api_response_et_fs.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_economic_index_historical_data.py` & `intrinio-sdk-6.24.0/test/test_api_response_economic_index_historical_data.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_awesome_oscillator_technical_value.py` & `intrinio-sdk-6.24.0/test/test_awesome_oscillator_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_interval_prices.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_interval_prices.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_on_balance_volume_mean.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_on_balance_volume_mean.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_options_realtime.py` & `intrinio-sdk-6.24.0/test/test_api_response_options_realtime.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_zacks_eps_growth_rate.py` & `intrinio-sdk-6.24.0/test/test_zacks_eps_growth_rate.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_stock_market_index.py` & `intrinio-sdk-6.24.0/test/test_stock_market_index.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_thea_entity_answer.py` & `intrinio-sdk-6.24.0/test/test_thea_entity_answer.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_stock_exchanges.py` & `intrinio-sdk-6.24.0/test/test_api_response_stock_exchanges.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_standardized_financials_dimension.py` & `intrinio-sdk-6.24.0/test/test_standardized_financials_dimension.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_reported_financials.py` & `intrinio-sdk-6.24.0/test/test_api_response_reported_financials.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_earnings_record.py` & `intrinio-sdk-6.24.0/test/test_earnings_record.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_zacks_api.py` & `intrinio-sdk-6.24.0/test/test_zacks_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_option_price_eod.py` & `intrinio-sdk-6.24.0/test/test_option_price_eod.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_thea_source_document.py` & `intrinio-sdk-6.24.0/test/test_thea_source_document.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_moving_average_convergence_divergence_technical_value.py` & `intrinio-sdk-6.24.0/test/test_moving_average_convergence_divergence_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_fundamentals_api.py` & `intrinio-sdk-6.24.0/test/test_fundamentals_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_zacks_long_term_growth_rate.py` & `intrinio-sdk-6.24.0/test/test_zacks_long_term_growth_rate.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_owner_summary.py` & `intrinio-sdk-6.24.0/test/test_owner_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_commodity_channel_index_technical_value.py` & `intrinio-sdk-6.24.0/test/test_commodity_channel_index_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_stock_price_summary.py` & `intrinio-sdk-6.24.0/test/test_stock_price_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_insider_transaction_filing.py` & `intrinio-sdk-6.24.0/test/test_insider_transaction_filing.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_stock_prices.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_stock_prices.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_negative_volume_index_technical_value.py` & `intrinio-sdk-6.24.0/test/test_negative_volume_index_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_ease_of_movement.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_ease_of_movement.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_ichimoku_kinko_hyo_technical_value.py` & `intrinio-sdk-6.24.0/test/test_ichimoku_kinko_hyo_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_zacks_institutional_holding_owner_summary.py` & `intrinio-sdk-6.24.0/test/test_zacks_institutional_holding_owner_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_data_tag_api.py` & `intrinio-sdk-6.24.0/test/test_data_tag_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_bulk_download_summary.py` & `intrinio-sdk-6.24.0/test/test_bulk_download_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_triple_exponential_average_technical_value.py` & `intrinio-sdk-6.24.0/test/test_triple_exponential_average_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_company_news_summary.py` & `intrinio-sdk-6.24.0/test/test_company_news_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_company_initial_public_offering.py` & `intrinio-sdk-6.24.0/test/test_company_initial_public_offering.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_historical_data.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_historical_data.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_forex_pairs.py` & `intrinio-sdk-6.24.0/test/test_api_response_forex_pairs.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_filing_api.py` & `intrinio-sdk-6.24.0/test/test_filing_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_stock_exchange_securities.py` & `intrinio-sdk-6.24.0/test/test_api_response_stock_exchange_securities.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_keltner_channel_technical_value.py` & `intrinio-sdk-6.24.0/test/test_keltner_channel_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_security_snapshots_result.py` & `intrinio-sdk-6.24.0/test/test_security_snapshots_result.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_stock_exchange_api.py` & `intrinio-sdk-6.24.0/test/test_stock_exchange_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_vortex_indicator_technical_value.py` & `intrinio-sdk-6.24.0/test/test_vortex_indicator_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_force_index_technical_value.py` & `intrinio-sdk-6.24.0/test/test_force_index_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_initial_public_offerings.py` & `intrinio-sdk-6.24.0/test/test_api_response_initial_public_offerings.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_forex_api.py` & `intrinio-sdk-6.24.0/test/test_forex_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_volume_price_trend.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_volume_price_trend.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_forex_price.py` & `intrinio-sdk-6.24.0/test/test_forex_price.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_zacks_etf_holdings.py` & `intrinio-sdk-6.24.0/test/test_api_response_zacks_etf_holdings.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_company_summary.py` & `intrinio-sdk-6.24.0/test/test_company_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_forex_pair.py` & `intrinio-sdk-6.24.0/test/test_forex_pair.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_bollinger_bands.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_bollinger_bands.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_zacks_sales_surprises.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_zacks_sales_surprises.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_volume_weighted_average_price.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_volume_weighted_average_price.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_true_strength_index_technical_value.py` & `intrinio-sdk-6.24.0/test/test_true_strength_index_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_options_prices_batch_realtime.py` & `intrinio-sdk-6.24.0/test/test_api_response_options_prices_batch_realtime.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_zacks_institutional_holding_owners.py` & `intrinio-sdk-6.24.0/test/test_api_response_zacks_institutional_holding_owners.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_filing_fundamentals.py` & `intrinio-sdk-6.24.0/test/test_api_response_filing_fundamentals.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_donchian_channel_technical_value.py` & `intrinio-sdk-6.24.0/test/test_donchian_channel_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_esg_comprehensive_rating.py` & `intrinio-sdk-6.24.0/test/test_esg_comprehensive_rating.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_forex_prices.py` & `intrinio-sdk-6.24.0/test/test_api_response_forex_prices.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_option_intervals_result.py` & `intrinio-sdk-6.24.0/test/test_option_intervals_result.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_option_stats_realtime.py` & `intrinio-sdk-6.24.0/test/test_option_stats_realtime.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_accumulation_distribution_index_technical_value.py` & `intrinio-sdk-6.24.0/test/test_accumulation_distribution_index_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_sic_indices_search.py` & `intrinio-sdk-6.24.0/test/test_api_response_sic_indices_search.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_average_true_range_technical_value.py` & `intrinio-sdk-6.24.0/test/test_average_true_range_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_options_expirations.py` & `intrinio-sdk-6.24.0/test/test_api_response_options_expirations.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_know_sure_thing_technical_value.py` & `intrinio-sdk-6.24.0/test/test_know_sure_thing_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_detrended_price_oscillator_technical_value.py` & `intrinio-sdk-6.24.0/test/test_detrended_price_oscillator_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_etf_stats.py` & `intrinio-sdk-6.24.0/test/test_etf_stats.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_data_tags_search.py` & `intrinio-sdk-6.24.0/test/test_api_response_data_tags_search.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_esg_companies.py` & `intrinio-sdk-6.24.0/test/test_api_response_esg_companies.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_ease_of_movement_technical_value.py` & `intrinio-sdk-6.24.0/test/test_ease_of_movement_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_keltner_channel.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_keltner_channel.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_owners_api.py` & `intrinio-sdk-6.24.0/test/test_owners_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_chaikin_money_flow_technical_value.py` & `intrinio-sdk-6.24.0/test/test_chaikin_money_flow_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_options_unusual_activity.py` & `intrinio-sdk-6.24.0/test/test_api_response_options_unusual_activity.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_simple_moving_average_technical_value.py` & `intrinio-sdk-6.24.0/test/test_simple_moving_average_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_negative_volume_index.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_negative_volume_index.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_options_price_realtime.py` & `intrinio-sdk-6.24.0/test/test_api_response_options_price_realtime.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_option_snapshots_result.py` & `intrinio-sdk-6.24.0/test/test_option_snapshots_result.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_zacks_institutional_holding_company_detail.py` & `intrinio-sdk-6.24.0/test/test_zacks_institutional_holding_company_detail.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_stock_market_indices_search.py` & `intrinio-sdk-6.24.0/test/test_api_response_stock_market_indices_search.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_stock_exchange_stock_prices.py` & `intrinio-sdk-6.24.0/test/test_api_response_stock_exchange_stock_prices.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_average_daily_trading_volume.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_average_daily_trading_volume.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_company_fundamentals.py` & `intrinio-sdk-6.24.0/test/test_api_response_company_fundamentals.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_triple_exponential_average.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_triple_exponential_average.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_zacks_eps_surprise.py` & `intrinio-sdk-6.24.0/test/test_zacks_eps_surprise.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_esg_rating.py` & `intrinio-sdk-6.24.0/test/test_esg_rating.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_filing_note_filing.py` & `intrinio-sdk-6.24.0/test/test_filing_note_filing.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_municipalitiy_financials.py` & `intrinio-sdk-6.24.0/test/test_api_response_municipalitiy_financials.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_company_news.py` & `intrinio-sdk-6.24.0/test/test_api_response_company_news.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_stock_price_adjustment.py` & `intrinio-sdk-6.24.0/test/test_stock_price_adjustment.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_zacks_eps_estimate.py` & `intrinio-sdk-6.24.0/test/test_zacks_eps_estimate.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_zacks_long_term_growth_rates.py` & `intrinio-sdk-6.24.0/test/test_api_response_zacks_long_term_growth_rates.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_zacks_institutional_holding_owner_detail.py` & `intrinio-sdk-6.24.0/test/test_zacks_institutional_holding_owner_detail.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_money_flow_index_technical_value.py` & `intrinio-sdk-6.24.0/test/test_money_flow_index_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_options.py` & `intrinio-sdk-6.24.0/test/test_api_response_options.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_fundamental.py` & `intrinio-sdk-6.24.0/test/test_fundamental.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_fundamental_summary.py` & `intrinio-sdk-6.24.0/test/test_fundamental_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_average_directional_index.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_average_directional_index.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_options_prices_eod.py` & `intrinio-sdk-6.24.0/test/test_api_response_options_prices_eod.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_stock_market_index_historical_data.py` & `intrinio-sdk-6.24.0/test/test_api_response_stock_market_index_historical_data.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_municipality_api.py` & `intrinio-sdk-6.24.0/test/test_municipality_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_company_shares_outstanding.py` & `intrinio-sdk-6.24.0/test/test_api_response_company_shares_outstanding.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_money_flow_index.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_money_flow_index.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_average_directional_index_technical_value.py` & `intrinio-sdk-6.24.0/test/test_average_directional_index_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_option_chain_realtime.py` & `intrinio-sdk-6.24.0/test/test_option_chain_realtime.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_option_contracts_list.py` & `intrinio-sdk-6.24.0/test/test_option_contracts_list.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_security_api.py` & `intrinio-sdk-6.24.0/test/test_security_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_zacks_analyst_rating_snapshot.py` & `intrinio-sdk-6.24.0/test/test_zacks_analyst_rating_snapshot.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_zacks_sales_surprises.py` & `intrinio-sdk-6.24.0/test/test_api_response_zacks_sales_surprises.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_institutional_ownership.py` & `intrinio-sdk-6.24.0/test/test_institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_true_strength_index.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_true_strength_index.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_options_tickers.py` & `intrinio-sdk-6.24.0/test/test_api_response_options_tickers.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_owner_institutional_holdings.py` & `intrinio-sdk-6.24.0/test/test_api_response_owner_institutional_holdings.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_insider_transaction_filings_api.py` & `intrinio-sdk-6.24.0/test/test_insider_transaction_filings_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_filing_notes.py` & `intrinio-sdk-6.24.0/test/test_api_response_filing_notes.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_option_unusual_trade.py` & `intrinio-sdk-6.24.0/test/test_option_unusual_trade.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_option_chain.py` & `intrinio-sdk-6.24.0/test/test_option_chain.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_volume_price_trend_technical_value.py` & `intrinio-sdk-6.24.0/test/test_volume_price_trend_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_filing_note_summary.py` & `intrinio-sdk-6.24.0/test/test_filing_note_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_option.py` & `intrinio-sdk-6.24.0/test/test_option.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_zacks_target_price_consensus.py` & `intrinio-sdk-6.24.0/test/test_zacks_target_price_consensus.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_etf_summary.py` & `intrinio-sdk-6.24.0/test/test_etf_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_company_historical_data.py` & `intrinio-sdk-6.24.0/test/test_api_response_company_historical_data.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_relative_strength_index_technical_value.py` & `intrinio-sdk-6.24.0/test/test_relative_strength_index_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_zacks_sales_surprise_summary.py` & `intrinio-sdk-6.24.0/test/test_zacks_sales_surprise_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_option_realtime.py` & `intrinio-sdk-6.24.0/test/test_option_realtime.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_stock_market_indices.py` & `intrinio-sdk-6.24.0/test/test_api_response_stock_market_indices.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_institutional_holding.py` & `intrinio-sdk-6.24.0/test/test_institutional_holding.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_owners.py` & `intrinio-sdk-6.24.0/test/test_api_response_owners.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_option_interval.py` & `intrinio-sdk-6.24.0/test/test_option_interval.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_force_index.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_force_index.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_zacks_analyst_ratings.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_zacks_analyst_ratings.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_filing_answers.py` & `intrinio-sdk-6.24.0/test/test_api_response_filing_answers.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_data_tag.py` & `intrinio-sdk-6.24.0/test/test_data_tag.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_insider_transaction.py` & `intrinio-sdk-6.24.0/test/test_insider_transaction.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_standardized_financial.py` & `intrinio-sdk-6.24.0/test/test_standardized_financial.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_stock_exchange_realtime_stock_prices.py` & `intrinio-sdk-6.24.0/test/test_api_response_stock_exchange_realtime_stock_prices.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_options_api.py` & `intrinio-sdk-6.24.0/test/test_options_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_company_filings.py` & `intrinio-sdk-6.24.0/test/test_api_response_company_filings.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_ultimate_oscillator_technical_value.py` & `intrinio-sdk-6.24.0/test/test_ultimate_oscillator_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_company_recognize.py` & `intrinio-sdk-6.24.0/test/test_api_response_company_recognize.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_esg_latest.py` & `intrinio-sdk-6.24.0/test/test_api_response_esg_latest.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_esg_api.py` & `intrinio-sdk-6.24.0/test/test_esg_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_zacks_institutional_holding.py` & `intrinio-sdk-6.24.0/test/test_zacks_institutional_holding.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_security_screen_clause.py` & `intrinio-sdk-6.24.0/test/test_security_screen_clause.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_company_shares_outstanding.py` & `intrinio-sdk-6.24.0/test/test_company_shares_outstanding.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_bollinger_bands_technical_value.py` & `intrinio-sdk-6.24.0/test/test_bollinger_bands_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_historical_data.py` & `intrinio-sdk-6.24.0/test/test_historical_data.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_security_summary.py` & `intrinio-sdk-6.24.0/test/test_security_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_mass_index.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_mass_index.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_securities_search.py` & `intrinio-sdk-6.24.0/test/test_api_response_securities_search.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_forex_currency.py` & `intrinio-sdk-6.24.0/test/test_forex_currency.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_economic_index_summary.py` & `intrinio-sdk-6.24.0/test/test_economic_index_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_simple_moving_average.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_simple_moving_average.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_filing.py` & `intrinio-sdk-6.24.0/test/test_filing.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_zacks_etf_holding.py` & `intrinio-sdk-6.24.0/test/test_zacks_etf_holding.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_zacks_target_price_consensuses.py` & `intrinio-sdk-6.24.0/test/test_api_response_zacks_target_price_consensuses.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_zacks_analyst_rating_summary.py` & `intrinio-sdk-6.24.0/test/test_zacks_analyst_rating_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_et_fs_api.py` & `intrinio-sdk-6.24.0/test/test_et_fs_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_zacks_institutional_holding_historical_summary.py` & `intrinio-sdk-6.24.0/test/test_zacks_institutional_holding_historical_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_accumulation_distribution_index.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_accumulation_distribution_index.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_news.py` & `intrinio-sdk-6.24.0/test/test_api_response_news.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_data_point_api.py` & `intrinio-sdk-6.24.0/test/test_data_point_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_on_balance_volume.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_on_balance_volume.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_standardized_financials.py` & `intrinio-sdk-6.24.0/test/test_api_response_standardized_financials.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_stock_market_index_summary.py` & `intrinio-sdk-6.24.0/test/test_stock_market_index_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_moving_average_convergence_divergence.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_moving_average_convergence_divergence.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_filing_summary.py` & `intrinio-sdk-6.24.0/test/test_filing_summary.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_zacks_institutional_holdings.py` & `intrinio-sdk-6.24.0/test/test_api_response_zacks_institutional_holdings.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_security_snapshot_group.py` & `intrinio-sdk-6.24.0/test/test_security_snapshot_group.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_options_chain.py` & `intrinio-sdk-6.24.0/test/test_api_response_options_chain.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_option_interval_mover.py` & `intrinio-sdk-6.24.0/test/test_option_interval_mover.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_companies_search.py` & `intrinio-sdk-6.24.0/test/test_api_response_companies_search.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_economic_indices_search.py` & `intrinio-sdk-6.24.0/test/test_api_response_economic_indices_search.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_companies.py` & `intrinio-sdk-6.24.0/test/test_api_response_companies.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_on_balance_volume_technical_value.py` & `intrinio-sdk-6.24.0/test/test_on_balance_volume_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_esg_company_rating_history.py` & `intrinio-sdk-6.24.0/test/test_api_response_esg_company_rating_history.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_company_answers.py` & `intrinio-sdk-6.24.0/test/test_api_response_company_answers.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_intraday_stock_price.py` & `intrinio-sdk-6.24.0/test/test_intraday_stock_price.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_reported_financial.py` & `intrinio-sdk-6.24.0/test/test_reported_financial.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_relative_strength_index.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_relative_strength_index.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_bulk_download_links.py` & `intrinio-sdk-6.24.0/test/test_api_response_bulk_download_links.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_index_api.py` & `intrinio-sdk-6.24.0/test/test_index_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_stock_price_interval.py` & `intrinio-sdk-6.24.0/test/test_stock_price_interval.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_williams_r_technical_value.py` & `intrinio-sdk-6.24.0/test/test_williams_r_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_average_daily_trading_volume_technical_value.py` & `intrinio-sdk-6.24.0/test/test_average_daily_trading_volume_technical_value.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_company_news.py` & `intrinio-sdk-6.24.0/test/test_company_news.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_securities.py` & `intrinio-sdk-6.24.0/test/test_api_response_securities.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_option_chain_eod.py` & `intrinio-sdk-6.24.0/test/test_option_chain_eod.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_zacks_institutional_holding_companies.py` & `intrinio-sdk-6.24.0/test/test_api_response_zacks_institutional_holding_companies.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_municipality.py` & `intrinio-sdk-6.24.0/test/test_municipality.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_security_donchian_channel.py` & `intrinio-sdk-6.24.0/test/test_api_response_security_donchian_channel.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_company_filing.py` & `intrinio-sdk-6.24.0/test/test_company_filing.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_historical_data_api.py` & `intrinio-sdk-6.24.0/test/test_historical_data_api.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_zacks_analyst_rating.py` & `intrinio-sdk-6.24.0/test/test_zacks_analyst_rating.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_owner.py` & `intrinio-sdk-6.24.0/test/test_owner.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_api_response_zacks_eps_estimates.py` & `intrinio-sdk-6.24.0/test/test_api_response_zacks_eps_estimates.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/test/test_dividend_record.py` & `intrinio-sdk-6.24.0/test/test_dividend_record.py`

 * *Files identical despite different names*

### Comparing `intrinio-sdk-6.23.1/README.md` & `intrinio-sdk-6.24.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Intrinio Python SDK
 
 To get an API key, [sign up here](https://intrinio.com/).
 
 Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.
 
-- API version: 2.39.2
-- Package version: 6.23.1
+- API version: 2.42.0
+- Package version: 6.24.0
 
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation
@@ -173,22 +173,23 @@
 *IndexApi* | [**search_sic_indices**](docs/IndexApi.md#search_sic_indices) | **GET** /indices/sic/search | Search SIC Indices
 *IndexApi* | [**search_stock_markets_indices**](docs/IndexApi.md#search_stock_markets_indices) | **GET** /indices/stock_market/search | Search Stock Market Indices
 *InsiderTransactionFilingsApi* | [**get_all_insider_transaction_filings**](docs/InsiderTransactionFilingsApi.md#get_all_insider_transaction_filings) | **GET** /insider_transaction_filings | All Insider Transactions Filings
 *MunicipalityApi* | [**get_all_municipalities**](docs/MunicipalityApi.md#get_all_municipalities) | **GET** /municipalities | All Municipalities
 *MunicipalityApi* | [**get_municipality_by_id**](docs/MunicipalityApi.md#get_municipality_by_id) | **GET** /municipalities/{id} | Municipality by ID
 *MunicipalityApi* | [**get_municipality_financials**](docs/MunicipalityApi.md#get_municipality_financials) | **GET** /municipalities/{id}/financials | Financials for a Municipality
 *OptionsApi* | [**get_all_options_tickers**](docs/OptionsApi.md#get_all_options_tickers) | **GET** /options/tickers | Options Tickers
-*OptionsApi* | [**get_option_expirations_realtime**](docs/OptionsApi.md#get_option_expirations_realtime) | **GET** /options/expirations/{symbol}/realtime | Option Expirations Realtime
+*OptionsApi* | [**get_option_expirations_realtime**](docs/OptionsApi.md#get_option_expirations_realtime) | **GET** /options/expirations/{symbol}/realtime | Options Expirations
 *OptionsApi* | [**get_option_strikes_realtime**](docs/OptionsApi.md#get_option_strikes_realtime) | **GET** /options/strikes/{symbol}/{strike}/realtime | Option Strikes Realtime
 *OptionsApi* | [**get_options**](docs/OptionsApi.md#get_options) | **GET** /options/{symbol} | Options
 *OptionsApi* | [**get_options_by_symbol_realtime**](docs/OptionsApi.md#get_options_by_symbol_realtime) | **GET** /options/{symbol}/realtime | Options by Symbol Realtime
 *OptionsApi* | [**get_options_chain**](docs/OptionsApi.md#get_options_chain) | **GET** /options/chain/{symbol}/{expiration} | Options Chain
 *OptionsApi* | [**get_options_chain_eod**](docs/OptionsApi.md#get_options_chain_eod) | **GET** /options/chain/{symbol}/{expiration}/eod | Options Chain EOD
 *OptionsApi* | [**get_options_chain_realtime**](docs/OptionsApi.md#get_options_chain_realtime) | **GET** /options/chain/{symbol}/{expiration}/realtime | Options Chain Realtime
 *OptionsApi* | [**get_options_expirations**](docs/OptionsApi.md#get_options_expirations) | **GET** /options/expirations/{symbol} | Options Expirations
+*OptionsApi* | [**get_options_expirations_eod**](docs/OptionsApi.md#get_options_expirations_eod) | **GET** /options/expirations/{symbol}/eod | Options Expirations
 *OptionsApi* | [**get_options_interval_by_contract**](docs/OptionsApi.md#get_options_interval_by_contract) | **GET** /options/interval/{identifier} | Options Intervals By Contract
 *OptionsApi* | [**get_options_interval_movers**](docs/OptionsApi.md#get_options_interval_movers) | **GET** /options/interval/movers | Options Intervals Movers
 *OptionsApi* | [**get_options_interval_movers_change**](docs/OptionsApi.md#get_options_interval_movers_change) | **GET** /options/interval/movers/change | Options Intervals Movers By Change
 *OptionsApi* | [**get_options_interval_movers_volume**](docs/OptionsApi.md#get_options_interval_movers_volume) | **GET** /options/interval/movers/volume | Options Intervals Movers By Volume
 *OptionsApi* | [**get_options_prices**](docs/OptionsApi.md#get_options_prices) | **GET** /options/prices/{identifier} | Option Prices
 *OptionsApi* | [**get_options_prices_batch_realtime**](docs/OptionsApi.md#get_options_prices_batch_realtime) | **POST** /options/prices/realtime/batch | Option Prices Batch Realtime
 *OptionsApi* | [**get_options_prices_eod**](docs/OptionsApi.md#get_options_prices_eod) | **GET** /options/prices/{identifier}/eod | Option Prices EOD
```

### Comparing `intrinio-sdk-6.23.1/setup.py` & `intrinio-sdk-6.24.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # coding: utf-8
 
 """
     Intrinio API
 
     Welcome to the Intrinio API! Through our Financial Data Marketplace, we offer a wide selection of financial data feed APIs sourced by our own proprietary processes as well as from many data vendors. For a complete API request / response reference please view the [Intrinio API documentation](https://docs.intrinio.com/documentation/api_v2). If you need additional help in using the API, please visit the [Intrinio website](https://intrinio.com) and click on the chat icon in the lower right corner.  # noqa: E501
 
-    OpenAPI spec version: 2.39.2
+    OpenAPI spec version: 2.42.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "intrinio-sdk"
-VERSION = "6.23.1"
+VERSION = "6.24.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

