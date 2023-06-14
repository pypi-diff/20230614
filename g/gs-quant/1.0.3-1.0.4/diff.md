# Comparing `tmp/gs_quant-1.0.3.tar.gz` & `tmp/gs_quant-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gs_quant-1.0.3.tar", last modified: Thu Jun  1 08:43:30 2023, max compression
+gzip compressed data, was "dist/gs_quant-1.0.4.tar", last modified: Thu Jun  1 14:54:56 2023, max compression
```

## Comparing `gs_quant-1.0.3.tar` & `gs_quant-1.0.4.tar`

### file list

```diff
@@ -1,421 +1,421 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-01 08:43:11.000000 gs_quant-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-01 08:43:30.000000 gs_quant-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-01 08:43:11.000000 gs_quant-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/analytics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/analytics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/analytics/common/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/analytics/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/analytics/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/analytics/common/enumerators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/analytics/common/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/analytics/core/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/analytics/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18717 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/analytics/core/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/analytics/core/processor_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/analytics/core/query_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/analytics/datagrid/
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/analytics/datagrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/analytics/datagrid/data_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/analytics/datagrid/data_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/analytics/datagrid/data_row.py
--rw-r--r--   0 runner    (1001) docker     (123)    31289 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/analytics/datagrid/datagrid.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/analytics/datagrid/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/analytics/datagrid/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/analytics/processors/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/analytics/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/analytics/processors/analysis_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/analytics/processors/econometrics_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/analytics/processors/scale_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/analytics/processors/special_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)    21852 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/analytics/processors/statistics_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)    16176 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/analytics/processors/utility_processors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/analytics/workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/analytics/workspaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25146 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/analytics/workspaces/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    24692 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/analytics/workspaces/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/api/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/api/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/api/fred/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/api/fred/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/api/fred/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/api/fred/fred_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/api/gs/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/api/gs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16576 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/api/gs/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/api/gs/backtests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/api/gs/base_screener.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/api/gs/carbon.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/api/gs/content.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/api/gs/countries.py
--rw-r--r--   0 runner    (1001) docker     (123)    38345 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/api/gs/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/api/gs/data_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/api/gs/datagrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/api/gs/esg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/api/gs/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/api/gs/hedges.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/api/gs/indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/api/gs/monitors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/api/gs/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/api/gs/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    14693 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/api/gs/portfolios.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/api/gs/price.py
--rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/api/gs/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)    11988 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/api/gs/risk.py
--rw-r--r--   0 runner    (1001) docker     (123)     8390 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/api/gs/risk_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/api/gs/screens.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/api/gs/thematics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/api/gs/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/api/gs/workspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    12505 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/api/risk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/backtests/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/backtests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/backtests/action_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9891 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/backtests/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/backtests/backtest_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    16840 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/backtests/backtest_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/backtests/backtest_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/backtests/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/backtests/data_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/backtests/data_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/backtests/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14179 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/backtests/equity_vol_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/backtests/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/backtests/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    39790 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/backtests/generic_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/backtests/order.py
--rw-r--r--   0 runner    (1001) docker     (123)    10071 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/backtests/predefined_asset_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/backtests/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/backtests/strategy_systematic.py
--rw-r--r--   0 runner    (1001) docker     (123)    18765 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/backtests/triggers.py
--rw-r--r--   0 runner    (1001) docker     (123)    19105 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/config/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/config/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/config.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/content/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/content/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/content/reports_and_screens/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/content/reports_and_screens/00_fx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/content/reports_and_screens/00_fx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/content/reports_and_screens/00_fx/vol_screen_app.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/content/reports_and_screens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/context_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/data/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/data/coordinate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/data/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    16613 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/data/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/data/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/data/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/data/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/datetime/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/datetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10979 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/datetime/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/datetime/gscalendar.py
--rw-r--r--   0 runner    (1001) docker     (123)    11678 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/datetime/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/datetime/relative_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/datetime/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/datetime/time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.datetime.date.business_day_count.html
--rw-r--r--   0 runner    (1001) docker     (123)    11059 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.datetime.date.business_day_offset.html
--rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.datetime.date.date_range.html
--rw-r--r--   0 runner    (1001) docker     (123)    10403 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.datetime.date.is_business_day.html
--rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.datetime.date.prev_business_date.html
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.datetime.point.point_sort_order.html
--rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.abs_.html
--rw-r--r--   0 runner    (1001) docker     (123)    14066 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.add.html
--rw-r--r--   0 runner    (1001) docker     (123)    10248 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.and_.html
--rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.ceil.html
--rw-r--r--   0 runner    (1001) docker     (123)    14106 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.divide.html
--rw-r--r--   0 runner    (1001) docker     (123)    11393 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.exp.html
--rw-r--r--   0 runner    (1001) docker     (123)    13221 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.filter_.html
--rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.floor.html
--rw-r--r--   0 runner    (1001) docker     (123)    13898 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.floordiv.html
--rw-r--r--   0 runner    (1001) docker     (123)    11096 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.if_.html
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.log.html
--rw-r--r--   0 runner    (1001) docker     (123)    14126 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.multiply.html
--rw-r--r--   0 runner    (1001) docker     (123)    10247 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.not_.html
--rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.or_.html
--rw-r--r--   0 runner    (1001) docker     (123)    11654 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.power.html
--rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.repeat.html
--rw-r--r--   0 runner    (1001) docker     (123)    11620 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.smooth_spikes.html
--rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.sqrt.html
--rw-r--r--   0 runner    (1001) docker     (123)    14183 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.subtract.html
--rw-r--r--   0 runner    (1001) docker     (123)    11852 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.weighted_sum.html
--rw-r--r--   0 runner    (1001) docker     (123)     9329 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.analysis.count.html
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.analysis.diff.html
--rw-r--r--   0 runner    (1001) docker     (123)     9322 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.analysis.first.html
--rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.analysis.lag.html
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.analysis.last.html
--rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.analysis.last_value.html
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.analysis.weighted_sum.html
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.backtesting.basket.html
--rw-r--r--   0 runner    (1001) docker     (123)    13116 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.datetime.align.html
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.datetime.date_range.html
--rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.datetime.day.html
--rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.datetime.interpolate.html
--rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.datetime.month.html
--rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.datetime.prepend.html
--rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.datetime.quarter.html
--rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.datetime.union.html
--rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.datetime.value.html
--rw-r--r--   0 runner    (1001) docker     (123)    10532 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.datetime.weekday.html
--rw-r--r--   0 runner    (1001) docker     (123)    10483 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.datetime.year.html
--rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.econometrics.annualize.html
--rw-r--r--   0 runner    (1001) docker     (123)    13874 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.econometrics.beta.html
--rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.econometrics.change.html
--rw-r--r--   0 runner    (1001) docker     (123)    13613 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.econometrics.correlation.html
--rw-r--r--   0 runner    (1001) docker     (123)    10460 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.econometrics.excess_returns_.html
--rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.econometrics.index.html
--rw-r--r--   0 runner    (1001) docker     (123)    10995 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.econometrics.max_drawdown.html
--rw-r--r--   0 runner    (1001) docker     (123)    12717 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.econometrics.prices.html
--rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.econometrics.returns.html
--rw-r--r--   0 runner    (1001) docker     (123)    12191 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.econometrics.sharpe_ratio.html
--rw-r--r--   0 runner    (1001) docker     (123)    14325 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.econometrics.volatility.html
--rw-r--r--   0 runner    (1001) docker     (123)    14645 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.statistics.cov.html
--rw-r--r--   0 runner    (1001) docker     (123)    14370 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.statistics.exponential_std.html
--rw-r--r--   0 runner    (1001) docker     (123)    12083 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.statistics.generate_series.html
--rw-r--r--   0 runner    (1001) docker     (123)    13669 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.statistics.max_.html
--rw-r--r--   0 runner    (1001) docker     (123)    14083 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.statistics.mean.html
--rw-r--r--   0 runner    (1001) docker     (123)    13491 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.statistics.median.html
--rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.statistics.min_.html
--rw-r--r--   0 runner    (1001) docker     (123)    13107 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.statistics.mode.html
--rw-r--r--   0 runner    (1001) docker     (123)    12906 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.statistics.percentile.html
--rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.statistics.percentiles.html
--rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.statistics.product.html
--rw-r--r--   0 runner    (1001) docker     (123)    13118 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.statistics.range_.html
--rw-r--r--   0 runner    (1001) docker     (123)    13766 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.statistics.std.html
--rw-r--r--   0 runner    (1001) docker     (123)    13622 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.statistics.sum_.html
--rw-r--r--   0 runner    (1001) docker     (123)    13834 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.statistics.var.html
--rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.statistics.winsorize.html
--rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.statistics.zscores.html
--rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.technicals.bollinger_bands.html
--rw-r--r--   0 runner    (1001) docker     (123)    11628 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.technicals.exponential_moving_average.html
--rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.technicals.exponential_spread_volatility.html
--rw-r--r--   0 runner    (1001) docker     (123)    11474 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.technicals.exponential_volatility.html
--rw-r--r--   0 runner    (1001) docker     (123)    11114 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.technicals.moving_average.html
--rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.technicals.relative_strength_index.html
--rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.technicals.smoothed_moving_average.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/entities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21932 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/entities/entitlements.py
--rw-r--r--   0 runner    (1001) docker     (123)    42358 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/entities/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/entities/tree_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/instrument/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/instrument/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13457 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/instrument/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/instrument/overrides.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/json_convertors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/json_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/markets/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/markets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39088 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/markets/baskets.py
--rw-r--r--   0 runner    (1001) docker     (123)    26457 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/markets/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/markets/factor.py
--rw-r--r--   0 runner    (1001) docker     (123)    41479 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/markets/hedge.py
--rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/markets/historical.py
--rw-r--r--   0 runner    (1001) docker     (123)    21287 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/markets/index.py
--rw-r--r--   0 runner    (1001) docker     (123)    20792 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/markets/indices_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/markets/markets.py
--rw-r--r--   0 runner    (1001) docker     (123)    30382 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/markets/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    25417 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/markets/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)    24832 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/markets/portfolio_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/markets/portfolio_manager_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    29040 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/markets/position_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    62817 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/markets/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/markets/report_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16415 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/markets/screens.py
--rw-r--r--   0 runner    (1001) docker     (123)    69212 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/markets/securities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/models/
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29649 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/models/epidemiology.py
--rw-r--r--   0 runner    (1001) docker     (123)    96299 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/models/risk_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16981 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/models/risk_model_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/priceable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/quote_reports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/quote_reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/quote_reports/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/risk/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/risk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19996 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/risk/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/risk/measures.py
--rw-r--r--   0 runner    (1001) docker     (123)    16256 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/risk/result_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    39862 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/risk/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/risk/scenario_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/risk/scenarios.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/risk/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    28088 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/target/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/target/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30269 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/target/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11832 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/target/assets_screener.py
--rw-r--r--   0 runner    (1001) docker     (123)    30119 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/target/backtests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/target/base_screener.py
--rw-r--r--   0 runner    (1001) docker     (123)    16824 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/target/charts.py
--rw-r--r--   0 runner    (1001) docker     (123)   241626 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/target/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    15206 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/target/content.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/target/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/target/countries.py
--rw-r--r--   0 runner    (1001) docker     (123)    36383 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/target/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/target/data_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/target/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    23131 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/target/hedge.py
--rw-r--r--   0 runner    (1001) docker     (123)    28594 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/target/indices.py
--rw-r--r--   0 runner    (1001) docker     (123)   158854 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/target/instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)    26039 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/target/measures.py
--rw-r--r--   0 runner    (1001) docker     (123)    15365 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/target/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10446 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/target/portfolios.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/target/price.py
--rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/target/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)    37770 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/target/risk.py
--rw-r--r--   0 runner    (1001) docker     (123)    13042 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/target/risk_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/target/screens.py
--rw-r--r--   0 runner    (1001) docker     (123)    17024 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/target/secmaster.py
--rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/target/trades.py
--rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/target/workflow_quote.py
--rw-r--r--   0 runner    (1001) docker     (123)    19404 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/target/workspaces_markets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/test/analytics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/analytics/test_datagrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/analytics/test_sorting_and_filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/analytics/test_workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/test/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/api/test_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/api/test_backtests.py
--rw-r--r--   0 runner    (1001) docker     (123)     7969 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/api/test_base_screener.py
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/api/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/api/test_carbon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/api/test_content.py
--rw-r--r--   0 runner    (1001) docker     (123)    19594 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/api/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/api/test_data_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/api/test_esg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/api/test_fred.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/api/test_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/api/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/api/test_instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/api/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/api/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/api/test_portfolios.py
--rw-r--r--   0 runner    (1001) docker     (123)    12054 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/api/test_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     8938 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/api/test_risk.py
--rw-r--r--   0 runner    (1001) docker     (123)    30272 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/api/test_risk_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/api/test_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/api/test_thread_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/api/test_users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/test/backtest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/backtest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34874 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/backtest/test_backtest_eq_vol_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/backtest/test_backtest_flow_vol.py
--rw-r--r--   0 runner    (1001) docker     (123)     8314 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/backtest/test_backtest_predefined.py
--rw-r--r--   0 runner    (1001) docker     (123)    20499 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/backtest/test_generic_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/backtest/test_triggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/data/test_data_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10512 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/data/test_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/test/datetime_/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/datetime_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/datetime_/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/datetime_/test_gscalendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/datetime_/test_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/datetime_/test_relative_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/datetime_/test_time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/test/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/fixtures/content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/test/markets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/markets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12018 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/markets/test_baskets.py
--rw-r--r--   0 runner    (1001) docker     (123)   180924 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/markets/test_hedger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/markets/test_instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)    17017 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/markets/test_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)    59098 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/markets/test_portfolio_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    14328 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/markets/test_pricing_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    20426 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/markets/test_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    62477 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/markets/test_securities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/test/models/
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/models/test_epidemiology.py
--rw-r--r--   0 runner    (1001) docker     (123)    30540 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/models/test_risk_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/test/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/test/timeseries/multi_measure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/timeseries/multi_measure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/timeseries/multi_measure/test_commod.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/timeseries/multi_measure/test_measure_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    19175 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/timeseries/test_algebra.py
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/timeseries/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    19817 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/timeseries/test_backtesting.py
--rw-r--r--   0 runner    (1001) docker     (123)    17659 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/timeseries/test_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)    17631 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/timeseries/test_econometrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/timeseries/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)   238697 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/timeseries/test_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/timeseries/test_measures_countries.py
--rw-r--r--   0 runner    (1001) docker     (123)    22551 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/timeseries/test_measures_fx_vol.py
--rw-r--r--   0 runner    (1001) docker     (123)    14577 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/timeseries/test_measures_inflation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/timeseries/test_measures_portfolios.py
--rw-r--r--   0 runner    (1001) docker     (123)    58767 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/timeseries/test_measures_rates.py
--rw-r--r--   0 runner    (1001) docker     (123)    36565 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/timeseries/test_measures_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)    10574 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/timeseries/test_measures_risk_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    14552 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/timeseries/test_measures_xccy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/timeseries/test_rolling.py
--rw-r--r--   0 runner    (1001) docker     (123)    29280 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/timeseries/test_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/timeseries/test_tca.py
--rw-r--r--   0 runner    (1001) docker     (123)    10202 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/timeseries/test_technicals.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/timeseries/test_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/timeseries/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/test/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/utils/datagrid_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/utils/mock_calc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/utils/mock_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/utils/mock_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/test/utils/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23911 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/timeseries/algebra.py
--rw-r--r--   0 runner    (1001) docker     (123)    10377 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/timeseries/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    19824 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/timeseries/backtesting.py
--rw-r--r--   0 runner    (1001) docker     (123)    21728 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/timeseries/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)    27160 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/timeseries/econometrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/timeseries/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/timeseries/measure_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)   227438 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/timeseries/measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/timeseries/measures_countries.py
--rw-r--r--   0 runner    (1001) docker     (123)    31461 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/timeseries/measures_fx_vol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/timeseries/measures_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    16985 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/timeseries/measures_inflation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/timeseries/measures_portfolios.py
--rw-r--r--   0 runner    (1001) docker     (123)   100015 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/timeseries/measures_rates.py
--rw-r--r--   0 runner    (1001) docker     (123)    16529 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/timeseries/measures_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/timeseries/measures_risk_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    20096 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/timeseries/measures_xccy.py
--rw-r--r--   0 runner    (1001) docker     (123)    54899 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/timeseries/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/timeseries/tca.py
--rw-r--r--   0 runner    (1001) docker     (123)    20055 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/timeseries/technicals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant/tracing/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/tracing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-06-01 08:43:11.000000 gs_quant-1.0.3/gs_quant/tracing/tracing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:43:30.000000 gs_quant-1.0.3/gs_quant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-01 08:43:29.000000 gs_quant-1.0.3/gs_quant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14744 2023-06-01 08:43:29.000000 gs_quant-1.0.3/gs_quant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 08:43:29.000000 gs_quant-1.0.3/gs_quant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-01 08:43:29.000000 gs_quant-1.0.3/gs_quant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-01 08:43:29.000000 gs_quant-1.0.3/gs_quant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-01 08:43:30.000000 gs_quant-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-06-01 08:43:11.000000 gs_quant-1.0.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83669 2023-06-01 08:43:11.000000 gs_quant-1.0.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-01 14:54:39.000000 gs_quant-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-01 14:54:56.000000 gs_quant-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-01 14:54:39.000000 gs_quant-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/analytics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/analytics/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/analytics/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/analytics/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/analytics/common/enumerators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/analytics/common/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/analytics/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/analytics/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18717 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/analytics/core/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/analytics/core/processor_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/analytics/core/query_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/analytics/datagrid/
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/analytics/datagrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/analytics/datagrid/data_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/analytics/datagrid/data_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/analytics/datagrid/data_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31289 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/analytics/datagrid/datagrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/analytics/datagrid/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/analytics/datagrid/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/analytics/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/analytics/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/analytics/processors/analysis_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/analytics/processors/econometrics_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/analytics/processors/scale_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/analytics/processors/special_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21852 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/analytics/processors/statistics_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16176 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/analytics/processors/utility_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/analytics/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/analytics/workspaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25146 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/analytics/workspaces/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24692 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/analytics/workspaces/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/api/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/api/fred/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/api/fred/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/api/fred/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/api/fred/fred_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/api/gs/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/api/gs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16576 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/api/gs/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/api/gs/backtests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/api/gs/base_screener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/api/gs/carbon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/api/gs/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/api/gs/countries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38389 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/api/gs/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/api/gs/data_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/api/gs/datagrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/api/gs/esg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/api/gs/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/api/gs/hedges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/api/gs/indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/api/gs/monitors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/api/gs/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/api/gs/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14693 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/api/gs/portfolios.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/api/gs/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/api/gs/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11988 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/api/gs/risk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8390 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/api/gs/risk_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/api/gs/screens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/api/gs/thematics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/api/gs/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/api/gs/workspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12505 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/api/risk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/backtests/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/backtests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/backtests/action_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9891 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/backtests/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/backtests/backtest_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16840 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/backtests/backtest_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/backtests/backtest_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/backtests/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/backtests/data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/backtests/data_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/backtests/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14179 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/backtests/equity_vol_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/backtests/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/backtests/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39790 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/backtests/generic_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/backtests/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10071 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/backtests/predefined_asset_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/backtests/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/backtests/strategy_systematic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18765 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/backtests/triggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19105 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/config/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/config.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/content/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/content/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/content/reports_and_screens/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/content/reports_and_screens/00_fx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/content/reports_and_screens/00_fx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/content/reports_and_screens/00_fx/vol_screen_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/content/reports_and_screens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/context_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/data/coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/data/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16777 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/data/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/data/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/data/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/data/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/datetime/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/datetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10979 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/datetime/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/datetime/gscalendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11678 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/datetime/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/datetime/relative_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/datetime/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/datetime/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.datetime.date.business_day_count.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11059 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.datetime.date.business_day_offset.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.datetime.date.date_range.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10403 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.datetime.date.is_business_day.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.datetime.date.prev_business_date.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.datetime.point.point_sort_order.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.abs_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14066 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.add.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10248 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.and_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.ceil.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14106 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.divide.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11393 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.exp.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13221 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.filter_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.floor.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13898 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.floordiv.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11096 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.if_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.log.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14126 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.multiply.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10247 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.not_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.or_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11654 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.power.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.repeat.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11620 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.smooth_spikes.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.sqrt.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14183 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.subtract.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11852 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.weighted_sum.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9329 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.analysis.count.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.analysis.diff.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9322 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.analysis.first.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.analysis.lag.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.analysis.last.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.analysis.last_value.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.analysis.weighted_sum.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.backtesting.basket.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13116 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.datetime.align.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.datetime.date_range.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.datetime.day.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.datetime.interpolate.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.datetime.month.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.datetime.prepend.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.datetime.quarter.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.datetime.union.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.datetime.value.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10532 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.datetime.weekday.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10483 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.datetime.year.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.econometrics.annualize.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13874 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.econometrics.beta.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.econometrics.change.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13613 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.econometrics.correlation.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10460 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.econometrics.excess_returns_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.econometrics.index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10995 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.econometrics.max_drawdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12717 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.econometrics.prices.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.econometrics.returns.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12191 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.econometrics.sharpe_ratio.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14325 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.econometrics.volatility.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14645 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.statistics.cov.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14370 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.statistics.exponential_std.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12083 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.statistics.generate_series.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13669 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.statistics.max_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14083 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.statistics.mean.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13491 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.statistics.median.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.statistics.min_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13107 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.statistics.mode.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12906 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.statistics.percentile.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.statistics.percentiles.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.statistics.product.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13118 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.statistics.range_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13766 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.statistics.std.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13622 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.statistics.sum_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13834 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.statistics.var.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.statistics.winsorize.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.statistics.zscores.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.technicals.bollinger_bands.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11628 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.technicals.exponential_moving_average.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.technicals.exponential_spread_volatility.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11474 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.technicals.exponential_volatility.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11114 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.technicals.moving_average.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.technicals.relative_strength_index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.technicals.smoothed_moving_average.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21932 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/entities/entitlements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42358 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/entities/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/entities/tree_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/instrument/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/instrument/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13457 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/instrument/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/instrument/overrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/json_convertors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/json_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/markets/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/markets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39088 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/markets/baskets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26457 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/markets/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/markets/factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41479 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/markets/hedge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/markets/historical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21287 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/markets/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20792 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/markets/indices_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/markets/markets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30382 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/markets/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25417 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/markets/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24832 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/markets/portfolio_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/markets/portfolio_manager_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29040 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/markets/position_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62817 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/markets/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/markets/report_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16415 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/markets/screens.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69212 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/markets/securities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29649 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/models/epidemiology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96299 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/models/risk_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16981 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/models/risk_model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/priceable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/quote_reports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/quote_reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/quote_reports/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/risk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/risk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19996 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/risk/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/risk/measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16256 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/risk/result_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39862 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/risk/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/risk/scenario_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/risk/scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/risk/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28088 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/target/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/target/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30269 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/target/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11832 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/target/assets_screener.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30119 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/target/backtests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/target/base_screener.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16824 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/target/charts.py
+-rw-r--r--   0 runner    (1001) docker     (123)   241626 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/target/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15206 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/target/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/target/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/target/countries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36466 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/target/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/target/data_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/target/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23131 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/target/hedge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28594 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/target/indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)   158854 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/target/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26039 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/target/measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15365 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/target/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10446 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/target/portfolios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/target/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/target/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37770 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/target/risk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13042 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/target/risk_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/target/screens.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17024 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/target/secmaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/target/trades.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/target/workflow_quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19404 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/target/workspaces_markets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/test/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/analytics/test_datagrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/analytics/test_sorting_and_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/analytics/test_workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/test/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/api/test_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/api/test_backtests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7969 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/api/test_base_screener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/api/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/api/test_carbon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/api/test_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19594 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/api/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/api/test_data_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/api/test_esg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/api/test_fred.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/api/test_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/api/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/api/test_instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/api/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/api/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/api/test_portfolios.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12054 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/api/test_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8938 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/api/test_risk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30272 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/api/test_risk_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/api/test_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/api/test_thread_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/api/test_users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/test/backtest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/backtest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34874 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/backtest/test_backtest_eq_vol_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/backtest/test_backtest_flow_vol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8314 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/backtest/test_backtest_predefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20499 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/backtest/test_generic_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/backtest/test_triggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/data/test_data_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13830 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/data/test_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/test/datetime_/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/datetime_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/datetime_/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/datetime_/test_gscalendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/datetime_/test_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/datetime_/test_relative_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/datetime_/test_time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/test/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/fixtures/content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/test/markets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/markets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12018 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/markets/test_baskets.py
+-rw-r--r--   0 runner    (1001) docker     (123)   180924 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/markets/test_hedger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/markets/test_instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17017 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/markets/test_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59098 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/markets/test_portfolio_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14328 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/markets/test_pricing_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20426 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/markets/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62477 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/markets/test_securities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/test/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/models/test_epidemiology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30540 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/models/test_risk_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/test/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/test/timeseries/multi_measure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/timeseries/multi_measure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/timeseries/multi_measure/test_commod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/timeseries/multi_measure/test_measure_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19175 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/timeseries/test_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/timeseries/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19817 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/timeseries/test_backtesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17659 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/timeseries/test_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17631 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/timeseries/test_econometrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/timeseries/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)   238697 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/timeseries/test_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/timeseries/test_measures_countries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22551 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/timeseries/test_measures_fx_vol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14577 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/timeseries/test_measures_inflation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/timeseries/test_measures_portfolios.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58767 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/timeseries/test_measures_rates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36565 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/timeseries/test_measures_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10574 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/timeseries/test_measures_risk_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14552 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/timeseries/test_measures_xccy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/timeseries/test_rolling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29280 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/timeseries/test_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/timeseries/test_tca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10202 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/timeseries/test_technicals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/timeseries/test_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/timeseries/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/utils/datagrid_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/utils/mock_calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/utils/mock_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/utils/mock_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/test/utils/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23911 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/timeseries/algebra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10377 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/timeseries/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19824 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/timeseries/backtesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21728 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/timeseries/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27160 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/timeseries/econometrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/timeseries/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/timeseries/measure_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)   227438 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/timeseries/measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/timeseries/measures_countries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31461 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/timeseries/measures_fx_vol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/timeseries/measures_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16985 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/timeseries/measures_inflation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/timeseries/measures_portfolios.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100015 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/timeseries/measures_rates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16529 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/timeseries/measures_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/timeseries/measures_risk_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20096 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/timeseries/measures_xccy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54899 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/timeseries/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/timeseries/tca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20055 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/timeseries/technicals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant/tracing/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/tracing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-06-01 14:54:39.000000 gs_quant-1.0.4/gs_quant/tracing/tracing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14744 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-01 14:54:56.000000 gs_quant-1.0.4/gs_quant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-01 14:54:56.000000 gs_quant-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-06-01 14:54:39.000000 gs_quant-1.0.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83669 2023-06-01 14:54:39.000000 gs_quant-1.0.4/versioneer.py
```

### Comparing `gs_quant-1.0.3/PKG-INFO` & `gs_quant-1.0.4/gs_quant.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gs_quant
-Version: 1.0.3
+Name: gs-quant
+Version: 1.0.4
 Summary: Goldman Sachs Quant
 Home-page: https://marquee.gs.com
 Author: Goldman Sachs
 Author-email: developer@gs.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Description: # GS Quant
```

### Comparing `gs_quant-1.0.3/README.md` & `gs_quant-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/__init__.py` & `gs_quant-1.0.4/gs_quant/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/analytics/common/__init__.py` & `gs_quant-1.0.4/gs_quant/analytics/common/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/analytics/common/constants.py` & `gs_quant-1.0.4/gs_quant/analytics/common/constants.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/analytics/common/enumerators.py` & `gs_quant-1.0.4/gs_quant/analytics/common/enumerators.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/analytics/common/helpers.py` & `gs_quant-1.0.4/gs_quant/analytics/common/helpers.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/analytics/core/__init__.py` & `gs_quant-1.0.4/gs_quant/analytics/core/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/analytics/core/processor.py` & `gs_quant-1.0.4/gs_quant/analytics/core/processor.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/analytics/core/processor_result.py` & `gs_quant-1.0.4/gs_quant/analytics/core/processor_result.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/analytics/core/query_helpers.py` & `gs_quant-1.0.4/gs_quant/analytics/core/query_helpers.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/analytics/datagrid/__init__.py` & `gs_quant-1.0.4/gs_quant/analytics/datagrid/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/analytics/datagrid/data_cell.py` & `gs_quant-1.0.4/gs_quant/analytics/datagrid/data_cell.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/analytics/datagrid/data_column.py` & `gs_quant-1.0.4/gs_quant/analytics/datagrid/data_column.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/analytics/datagrid/data_row.py` & `gs_quant-1.0.4/gs_quant/analytics/datagrid/data_row.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/analytics/datagrid/datagrid.py` & `gs_quant-1.0.4/gs_quant/analytics/datagrid/datagrid.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/analytics/datagrid/serializers.py` & `gs_quant-1.0.4/gs_quant/analytics/datagrid/serializers.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/analytics/datagrid/utils.py` & `gs_quant-1.0.4/gs_quant/analytics/datagrid/utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/analytics/processors/__init__.py` & `gs_quant-1.0.4/gs_quant/analytics/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/analytics/processors/analysis_processors.py` & `gs_quant-1.0.4/gs_quant/analytics/processors/analysis_processors.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/analytics/processors/econometrics_processors.py` & `gs_quant-1.0.4/gs_quant/analytics/processors/econometrics_processors.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/analytics/processors/scale_processors.py` & `gs_quant-1.0.4/gs_quant/analytics/processors/scale_processors.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/analytics/processors/special_processors.py` & `gs_quant-1.0.4/gs_quant/analytics/processors/special_processors.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/analytics/processors/statistics_processors.py` & `gs_quant-1.0.4/gs_quant/analytics/processors/statistics_processors.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/analytics/processors/utility_processors.py` & `gs_quant-1.0.4/gs_quant/analytics/processors/utility_processors.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/analytics/workspaces/__init__.py` & `gs_quant-1.0.4/gs_quant/analytics/workspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/analytics/workspaces/components.py` & `gs_quant-1.0.4/gs_quant/analytics/workspaces/components.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/analytics/workspaces/workspace.py` & `gs_quant-1.0.4/gs_quant/analytics/workspaces/workspace.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/api/__init__.py` & `gs_quant-1.0.4/gs_quant/api/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/api/data.py` & `gs_quant-1.0.4/gs_quant/api/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,14 +56,15 @@
             start: Optional[Union[dt.date, dt.datetime]] = None,
             end: Optional[Union[dt.date, dt.datetime]] = None,
             as_of: Optional[dt.datetime] = None,
             since: Optional[dt.datetime] = None,
             restrict_fields: bool = False,
             format: str = 'MessagePack',
             dates: List[dt.date] = None,
+            empty_intervals: Optional[bool] = None,
             **kwargs
     ):
         end_is_time = isinstance(end, dt.datetime)
         start_is_time = isinstance(start, dt.datetime)
 
         if kwargs.get('market_data_coordinates'):
             real_time = ((start is None or start_is_time) and (end is None or end_is_time))
@@ -87,15 +88,16 @@
                 start_date=start if not start_is_time else None,
                 start_time=start if start_is_time else None,
                 end_date=end if not end_is_time else None,
                 end_time=end if end_is_time else None,
                 as_of_time=as_of,
                 since=since,
                 format=format,
-                dates=dates
+                dates=dates,
+                empty_intervals=empty_intervals
             )
 
         query_properties = query.properties()
         query.where = dict()
         for field, value in kwargs.items():
             snake_case_field = inflection.underscore(field)
             if snake_case_field in query_properties and snake_case_field not in ('name',):
```

### Comparing `gs_quant-1.0.3/gs_quant/api/fred/__init__.py` & `gs_quant-1.0.4/gs_quant/api/fred/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/api/fred/data.py` & `gs_quant-1.0.4/gs_quant/api/fred/data.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/api/fred/fred_query.py` & `gs_quant-1.0.4/gs_quant/api/fred/fred_query.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/api/gs/__init__.py` & `gs_quant-1.0.4/gs_quant/api/gs/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/api/gs/assets.py` & `gs_quant-1.0.4/gs_quant/api/gs/assets.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/api/gs/backtests.py` & `gs_quant-1.0.4/gs_quant/api/gs/backtests.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/api/gs/base_screener.py` & `gs_quant-1.0.4/gs_quant/api/gs/base_screener.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/api/gs/carbon.py` & `gs_quant-1.0.4/gs_quant/api/gs/carbon.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/api/gs/content.py` & `gs_quant-1.0.4/gs_quant/api/gs/content.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/api/gs/countries.py` & `gs_quant-1.0.4/gs_quant/api/gs/countries.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/api/gs/data.py` & `gs_quant-1.0.4/gs_quant/api/gs/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -812,15 +812,15 @@
             incoming_data_data_types = pd.DataFrame(sample).dtypes.to_dict()
 
             df = pd.DataFrame(data, columns={**dataset_types, **incoming_data_data_types})
 
             for field_name, type_name in dataset_types.items():
                 if df.get(field_name) is not None and type_name in ('date', 'date-time') and \
                         len(df.get(field_name).value_counts()) > 0:
-                    df[field_name] = pd.to_datetime(df[field_name])
+                    df[field_name] = pd.to_datetime(df[field_name], format='mixed', infer_datetime_format=True)
 
             field_names = dataset_types.keys()
 
             if 'date' in field_names:
                 df = df.set_index('date')
             elif 'time' in field_names:
                 df = df.set_index('time')
```

### Comparing `gs_quant-1.0.3/gs_quant/api/gs/data_screen.py` & `gs_quant-1.0.4/gs_quant/api/gs/data_screen.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/api/gs/datagrid.py` & `gs_quant-1.0.4/gs_quant/api/gs/datagrid.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/api/gs/esg.py` & `gs_quant-1.0.4/gs_quant/api/gs/esg.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/api/gs/groups.py` & `gs_quant-1.0.4/gs_quant/api/gs/groups.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/api/gs/hedges.py` & `gs_quant-1.0.4/gs_quant/api/gs/hedges.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/api/gs/indices.py` & `gs_quant-1.0.4/gs_quant/api/gs/indices.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/api/gs/monitors.py` & `gs_quant-1.0.4/gs_quant/api/gs/monitors.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/api/gs/parser.py` & `gs_quant-1.0.4/gs_quant/api/gs/parser.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/api/gs/plots.py` & `gs_quant-1.0.4/gs_quant/api/gs/plots.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/api/gs/portfolios.py` & `gs_quant-1.0.4/gs_quant/api/gs/portfolios.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/api/gs/price.py` & `gs_quant-1.0.4/gs_quant/api/gs/price.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/api/gs/reports.py` & `gs_quant-1.0.4/gs_quant/api/gs/reports.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/api/gs/risk.py` & `gs_quant-1.0.4/gs_quant/api/gs/risk.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/api/gs/risk_models.py` & `gs_quant-1.0.4/gs_quant/api/gs/risk_models.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/api/gs/screens.py` & `gs_quant-1.0.4/gs_quant/api/gs/screens.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/api/gs/thematics.py` & `gs_quant-1.0.4/gs_quant/api/gs/thematics.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/api/gs/users.py` & `gs_quant-1.0.4/gs_quant/api/gs/users.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/api/gs/workspaces.py` & `gs_quant-1.0.4/gs_quant/api/gs/workspaces.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/api/risk.py` & `gs_quant-1.0.4/gs_quant/api/risk.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/api/utils.py` & `gs_quant-1.0.4/gs_quant/api/utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/backtests/__init__.py` & `gs_quant-1.0.4/gs_quant/backtests/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/backtests/action_handler.py` & `gs_quant-1.0.4/gs_quant/backtests/action_handler.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/backtests/actions.py` & `gs_quant-1.0.4/gs_quant/backtests/actions.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/backtests/backtest_engine.py` & `gs_quant-1.0.4/gs_quant/backtests/backtest_engine.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/backtests/backtest_objects.py` & `gs_quant-1.0.4/gs_quant/backtests/backtest_objects.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/backtests/backtest_utils.py` & `gs_quant-1.0.4/gs_quant/backtests/backtest_utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/backtests/core.py` & `gs_quant-1.0.4/gs_quant/backtests/core.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/backtests/data_handler.py` & `gs_quant-1.0.4/gs_quant/backtests/data_handler.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/backtests/data_sources.py` & `gs_quant-1.0.4/gs_quant/backtests/data_sources.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/backtests/decorator.py` & `gs_quant-1.0.4/gs_quant/backtests/decorator.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/backtests/equity_vol_engine.py` & `gs_quant-1.0.4/gs_quant/backtests/equity_vol_engine.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/backtests/event.py` & `gs_quant-1.0.4/gs_quant/backtests/event.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/backtests/execution_engine.py` & `gs_quant-1.0.4/gs_quant/backtests/execution_engine.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/backtests/generic_engine.py` & `gs_quant-1.0.4/gs_quant/backtests/generic_engine.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/backtests/order.py` & `gs_quant-1.0.4/gs_quant/backtests/order.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/backtests/predefined_asset_engine.py` & `gs_quant-1.0.4/gs_quant/backtests/predefined_asset_engine.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/backtests/strategy.py` & `gs_quant-1.0.4/gs_quant/backtests/strategy.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/backtests/strategy_systematic.py` & `gs_quant-1.0.4/gs_quant/backtests/strategy_systematic.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/backtests/triggers.py` & `gs_quant-1.0.4/gs_quant/backtests/triggers.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/base.py` & `gs_quant-1.0.4/gs_quant/base.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/common.py` & `gs_quant-1.0.4/gs_quant/common.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/config/__init__.py` & `gs_quant-1.0.4/gs_quant/config/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/config/options.py` & `gs_quant-1.0.4/gs_quant/config/options.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/config.ini` & `gs_quant-1.0.4/gs_quant/config.ini`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/content/reports_and_screens/00_fx/vol_screen_app.py` & `gs_quant-1.0.4/gs_quant/content/reports_and_screens/00_fx/vol_screen_app.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/context_base.py` & `gs_quant-1.0.4/gs_quant/context_base.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/data/__init__.py` & `gs_quant-1.0.4/gs_quant/data/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/data/coordinate.py` & `gs_quant-1.0.4/gs_quant/data/coordinate.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/data/core.py` & `gs_quant-1.0.4/gs_quant/data/core.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/data/dataset.py` & `gs_quant-1.0.4/gs_quant/data/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,24 +109,26 @@
             self,
             start: Optional[Union[dt.date, dt.datetime]] = None,
             end: Optional[Union[dt.date, dt.datetime]] = None,
             as_of: Optional[dt.datetime] = None,
             since: Optional[dt.datetime] = None,
             fields: Optional[Iterable[Union[str, Fields]]] = None,
             asset_id_type: Optional[str] = None,
+            empty_intervals: Optional[bool] = None,
             **kwargs
     ) -> pd.DataFrame:
         """
         Get data for the given range and parameters
 
         :param start: Requested start date/datetime for data
         :param end: Requested end date/datetime for data
         :param as_of: Request data as_of
         :param since: Request data since
         :param fields: DataSet fields to include
+        :param empty_intervals: whether to request empty intervals
         :param kwargs: Extra query arguments, e.g. ticker='EDZ19'
         :return: A Dataframe of the requested data
 
         **Examples**
 
         >>> from gs_quant.data import Dataset
         >>> import datetime as dt
@@ -141,14 +143,15 @@
 
         query = self.provider.build_query(
             start=start,
             end=end,
             as_of=as_of,
             since=since,
             fields=field_names,
+            empty_intervals=empty_intervals,
             **kwargs
         )
         data = self.provider.query_data(query, self.id, asset_id_type=asset_id_type)
         if type(data) is tuple:
             df = self.provider.construct_dataframe_with_types(self.id, data[0], schema_varies)
             return df.groupby(data[1], group_keys=True).apply(lambda x: x)
         else:
```

### Comparing `gs_quant-1.0.3/gs_quant/data/fields.py` & `gs_quant-1.0.4/gs_quant/data/fields.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/data/log.py` & `gs_quant-1.0.4/gs_quant/data/log.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/data/query.py` & `gs_quant-1.0.4/gs_quant/data/query.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/data/stream.py` & `gs_quant-1.0.4/gs_quant/data/stream.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/datetime/__init__.py` & `gs_quant-1.0.4/gs_quant/datetime/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/datetime/date.py` & `gs_quant-1.0.4/gs_quant/datetime/date.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/datetime/gscalendar.py` & `gs_quant-1.0.4/gs_quant/datetime/gscalendar.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/datetime/point.py` & `gs_quant-1.0.4/gs_quant/datetime/point.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/datetime/relative_date.py` & `gs_quant-1.0.4/gs_quant/datetime/relative_date.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/datetime/rules.py` & `gs_quant-1.0.4/gs_quant/datetime/rules.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/datetime/time.py` & `gs_quant-1.0.4/gs_quant/datetime/time.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.datetime.date.business_day_count.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.datetime.date.business_day_count.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.datetime.date.business_day_offset.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.datetime.date.business_day_offset.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.datetime.date.date_range.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.datetime.date.date_range.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.datetime.date.is_business_day.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.datetime.date.is_business_day.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.datetime.date.prev_business_date.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.datetime.date.prev_business_date.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.datetime.point.point_sort_order.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.datetime.point.point_sort_order.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.abs_.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.abs_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.add.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.add.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.and_.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.and_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.ceil.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.ceil.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.divide.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.divide.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.exp.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.exp.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.filter_.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.filter_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.floor.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.floor.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.floordiv.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.floordiv.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.if_.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.if_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.log.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.log.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.multiply.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.multiply.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.not_.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.not_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.or_.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.or_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.power.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.power.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.repeat.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.repeat.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.smooth_spikes.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.smooth_spikes.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.sqrt.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.sqrt.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.subtract.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.subtract.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.algebra.weighted_sum.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.algebra.weighted_sum.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.analysis.count.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.analysis.count.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.analysis.diff.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.analysis.diff.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.analysis.first.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.analysis.first.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.analysis.lag.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.analysis.lag.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.analysis.last.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.analysis.last.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.analysis.last_value.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.analysis.last_value.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.analysis.weighted_sum.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.analysis.weighted_sum.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.backtesting.basket.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.backtesting.basket.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.datetime.align.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.datetime.align.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.datetime.date_range.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.datetime.date_range.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.datetime.day.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.datetime.day.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.datetime.interpolate.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.datetime.interpolate.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.datetime.month.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.datetime.month.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.datetime.prepend.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.datetime.prepend.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.datetime.quarter.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.datetime.quarter.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.datetime.union.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.datetime.union.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.datetime.value.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.datetime.value.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.datetime.weekday.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.datetime.weekday.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.datetime.year.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.datetime.year.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.econometrics.annualize.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.econometrics.annualize.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.econometrics.beta.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.econometrics.beta.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.econometrics.change.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.econometrics.change.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.econometrics.correlation.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.econometrics.correlation.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.econometrics.excess_returns_.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.econometrics.excess_returns_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.econometrics.index.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.econometrics.index.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.econometrics.max_drawdown.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.econometrics.max_drawdown.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.econometrics.prices.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.econometrics.prices.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.econometrics.returns.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.econometrics.returns.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.econometrics.sharpe_ratio.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.econometrics.sharpe_ratio.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.econometrics.volatility.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.econometrics.volatility.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.statistics.cov.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.statistics.cov.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.statistics.exponential_std.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.statistics.exponential_std.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.statistics.generate_series.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.statistics.generate_series.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.statistics.max_.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.statistics.max_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.statistics.mean.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.statistics.mean.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.statistics.median.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.statistics.median.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.statistics.min_.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.statistics.min_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.statistics.mode.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.statistics.mode.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.statistics.percentile.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.statistics.percentile.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.statistics.percentiles.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.statistics.percentiles.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.statistics.product.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.statistics.product.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.statistics.range_.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.statistics.range_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.statistics.std.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.statistics.std.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.statistics.sum_.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.statistics.sum_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.statistics.var.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.statistics.var.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.statistics.winsorize.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.statistics.winsorize.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.statistics.zscores.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.statistics.zscores.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.technicals.bollinger_bands.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.technicals.bollinger_bands.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.technicals.exponential_moving_average.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.technicals.exponential_moving_average.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.technicals.exponential_spread_volatility.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.technicals.exponential_spread_volatility.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.technicals.exponential_volatility.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.technicals.exponential_volatility.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.technicals.moving_average.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.technicals.moving_average.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.technicals.relative_strength_index.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.technicals.relative_strength_index.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/docs/gs_quant.timeseries.technicals.smoothed_moving_average.html` & `gs_quant-1.0.4/gs_quant/docs/gs_quant.timeseries.technicals.smoothed_moving_average.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/entities/entitlements.py` & `gs_quant-1.0.4/gs_quant/entities/entitlements.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/entities/entity.py` & `gs_quant-1.0.4/gs_quant/entities/entity.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/entities/tree_entity.py` & `gs_quant-1.0.4/gs_quant/entities/tree_entity.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/errors.py` & `gs_quant-1.0.4/gs_quant/errors.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/instrument/__init__.py` & `gs_quant-1.0.4/gs_quant/instrument/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/instrument/core.py` & `gs_quant-1.0.4/gs_quant/instrument/core.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/instrument/overrides.py` & `gs_quant-1.0.4/gs_quant/instrument/overrides.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/json_convertors.py` & `gs_quant-1.0.4/gs_quant/json_convertors.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/json_encoder.py` & `gs_quant-1.0.4/gs_quant/json_encoder.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/markets/__init__.py` & `gs_quant-1.0.4/gs_quant/markets/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/markets/baskets.py` & `gs_quant-1.0.4/gs_quant/markets/baskets.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/markets/core.py` & `gs_quant-1.0.4/gs_quant/markets/core.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/markets/factor.py` & `gs_quant-1.0.4/gs_quant/markets/factor.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/markets/hedge.py` & `gs_quant-1.0.4/gs_quant/markets/hedge.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/markets/historical.py` & `gs_quant-1.0.4/gs_quant/markets/historical.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/markets/index.py` & `gs_quant-1.0.4/gs_quant/markets/index.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/markets/indices_utils.py` & `gs_quant-1.0.4/gs_quant/markets/indices_utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/markets/markets.py` & `gs_quant-1.0.4/gs_quant/markets/markets.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/markets/optimizer.py` & `gs_quant-1.0.4/gs_quant/markets/optimizer.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/markets/portfolio.py` & `gs_quant-1.0.4/gs_quant/markets/portfolio.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/markets/portfolio_manager.py` & `gs_quant-1.0.4/gs_quant/markets/portfolio_manager.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/markets/portfolio_manager_utils.py` & `gs_quant-1.0.4/gs_quant/markets/portfolio_manager_utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/markets/position_set.py` & `gs_quant-1.0.4/gs_quant/markets/position_set.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/markets/report.py` & `gs_quant-1.0.4/gs_quant/markets/report.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/markets/report_utils.py` & `gs_quant-1.0.4/gs_quant/markets/report_utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/markets/screens.py` & `gs_quant-1.0.4/gs_quant/markets/screens.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/markets/securities.py` & `gs_quant-1.0.4/gs_quant/markets/securities.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/models/__init__.py` & `gs_quant-1.0.4/gs_quant/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/models/epidemiology.py` & `gs_quant-1.0.4/gs_quant/models/epidemiology.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/models/risk_model.py` & `gs_quant-1.0.4/gs_quant/models/risk_model.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/models/risk_model_utils.py` & `gs_quant-1.0.4/gs_quant/models/risk_model_utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/priceable.py` & `gs_quant-1.0.4/gs_quant/priceable.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/quote_reports/core.py` & `gs_quant-1.0.4/gs_quant/quote_reports/core.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/risk/__init__.py` & `gs_quant-1.0.4/gs_quant/risk/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/risk/core.py` & `gs_quant-1.0.4/gs_quant/risk/core.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/risk/measures.py` & `gs_quant-1.0.4/gs_quant/risk/measures.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/risk/result_handlers.py` & `gs_quant-1.0.4/gs_quant/risk/result_handlers.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/risk/results.py` & `gs_quant-1.0.4/gs_quant/risk/results.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/risk/scenario_utils.py` & `gs_quant-1.0.4/gs_quant/risk/scenario_utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/risk/scenarios.py` & `gs_quant-1.0.4/gs_quant/risk/scenarios.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/risk/transform.py` & `gs_quant-1.0.4/gs_quant/risk/transform.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/session.py` & `gs_quant-1.0.4/gs_quant/session.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/target/__init__.py` & `gs_quant-1.0.4/gs_quant/target/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/target/assets.py` & `gs_quant-1.0.4/gs_quant/target/assets.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/target/assets_screener.py` & `gs_quant-1.0.4/gs_quant/target/assets_screener.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/target/backtests.py` & `gs_quant-1.0.4/gs_quant/target/backtests.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/target/base_screener.py` & `gs_quant-1.0.4/gs_quant/target/base_screener.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/target/charts.py` & `gs_quant-1.0.4/gs_quant/target/charts.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/target/common.py` & `gs_quant-1.0.4/gs_quant/target/common.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/target/content.py` & `gs_quant-1.0.4/gs_quant/target/content.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/target/coordinates.py` & `gs_quant-1.0.4/gs_quant/target/coordinates.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/target/countries.py` & `gs_quant-1.0.4/gs_quant/target/countries.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/target/data.py` & `gs_quant-1.0.4/gs_quant/target/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -491,14 +491,15 @@
     offset_to_exchange_close: Optional[str] = field(default=None, metadata=field_metadata)
     multi_trading_session: Optional[bool] = field(default=None, metadata=field_metadata)
     multi_session: Optional[bool] = field(default=None, metadata=field_metadata)
     quote_consolidation: Optional[bool] = field(default=None, metadata=field_metadata)
     time_index: Optional[str] = field(default=None, metadata=field_metadata)
     name: Optional[str] = field(default=None, metadata=name_metadata)
     adjust_as_of: Optional[datetime.datetime] = field(default=None, metadata=field_metadata)
+    empty_intervals: Optional[bool] = field(default=None, metadata=field_metadata)
 
 
 @handle_camel_case_args
 @dataclass_json(letter_case=LetterCase.CAMEL)
 @dataclass(unsafe_hash=True, repr=False)
 class DataSetCatalogEntry(Base):
     id_: str = field(default=None, metadata=config(field_name='id', exclude=exclude_none))
```

### Comparing `gs_quant-1.0.3/gs_quant/target/data_screen.py` & `gs_quant-1.0.4/gs_quant/target/data_screen.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/target/groups.py` & `gs_quant-1.0.4/gs_quant/target/groups.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/target/hedge.py` & `gs_quant-1.0.4/gs_quant/target/hedge.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/target/indices.py` & `gs_quant-1.0.4/gs_quant/target/indices.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/target/instrument.py` & `gs_quant-1.0.4/gs_quant/target/instrument.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/target/measures.py` & `gs_quant-1.0.4/gs_quant/target/measures.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/target/monitor.py` & `gs_quant-1.0.4/gs_quant/target/monitor.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/target/portfolios.py` & `gs_quant-1.0.4/gs_quant/target/portfolios.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/target/price.py` & `gs_quant-1.0.4/gs_quant/target/price.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/target/reports.py` & `gs_quant-1.0.4/gs_quant/target/reports.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/target/risk.py` & `gs_quant-1.0.4/gs_quant/target/risk.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/target/risk_models.py` & `gs_quant-1.0.4/gs_quant/target/risk_models.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/target/screens.py` & `gs_quant-1.0.4/gs_quant/target/screens.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/target/secmaster.py` & `gs_quant-1.0.4/gs_quant/target/secmaster.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/target/trades.py` & `gs_quant-1.0.4/gs_quant/target/trades.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/target/workflow_quote.py` & `gs_quant-1.0.4/gs_quant/target/workflow_quote.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/target/workspaces_markets.py` & `gs_quant-1.0.4/gs_quant/target/workspaces_markets.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/analytics/test_datagrid.py` & `gs_quant-1.0.4/gs_quant/test/analytics/test_datagrid.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/analytics/test_sorting_and_filtering.py` & `gs_quant-1.0.4/gs_quant/test/analytics/test_sorting_and_filtering.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/analytics/test_workspace.py` & `gs_quant-1.0.4/gs_quant/test/analytics/test_workspace.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/api/test_assets.py` & `gs_quant-1.0.4/gs_quant/test/api/test_assets.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/api/test_backtests.py` & `gs_quant-1.0.4/gs_quant/test/api/test_backtests.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/api/test_base_screener.py` & `gs_quant-1.0.4/gs_quant/test/api/test_base_screener.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/api/test_cache.py` & `gs_quant-1.0.4/gs_quant/test/api/test_cache.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/api/test_carbon.py` & `gs_quant-1.0.4/gs_quant/test/api/test_carbon.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/api/test_content.py` & `gs_quant-1.0.4/gs_quant/test/api/test_content.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/api/test_data.py` & `gs_quant-1.0.4/gs_quant/test/api/test_data.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/api/test_data_screen.py` & `gs_quant-1.0.4/gs_quant/test/api/test_data_screen.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/api/test_esg.py` & `gs_quant-1.0.4/gs_quant/test/api/test_esg.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/api/test_fred.py` & `gs_quant-1.0.4/gs_quant/test/api/test_fred.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/api/test_groups.py` & `gs_quant-1.0.4/gs_quant/test/api/test_groups.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/api/test_index.py` & `gs_quant-1.0.4/gs_quant/test/api/test_index.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/api/test_instruments.py` & `gs_quant-1.0.4/gs_quant/test/api/test_instruments.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/api/test_json.py` & `gs_quant-1.0.4/gs_quant/test/api/test_json.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/api/test_monitor.py` & `gs_quant-1.0.4/gs_quant/test/api/test_monitor.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/api/test_portfolios.py` & `gs_quant-1.0.4/gs_quant/test/api/test_portfolios.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/api/test_reports.py` & `gs_quant-1.0.4/gs_quant/test/api/test_reports.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/api/test_risk.py` & `gs_quant-1.0.4/gs_quant/test/api/test_risk.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/api/test_risk_models.py` & `gs_quant-1.0.4/gs_quant/test/api/test_risk_models.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/api/test_target.py` & `gs_quant-1.0.4/gs_quant/test/api/test_target.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/api/test_thread_manager.py` & `gs_quant-1.0.4/gs_quant/test/api/test_thread_manager.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/api/test_users.py` & `gs_quant-1.0.4/gs_quant/test/api/test_users.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/backtest/test_backtest_eq_vol_engine.py` & `gs_quant-1.0.4/gs_quant/test/backtest/test_backtest_eq_vol_engine.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/backtest/test_backtest_flow_vol.py` & `gs_quant-1.0.4/gs_quant/test/backtest/test_backtest_flow_vol.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/backtest/test_backtest_predefined.py` & `gs_quant-1.0.4/gs_quant/test/backtest/test_backtest_predefined.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/backtest/test_generic_engine.py` & `gs_quant-1.0.4/gs_quant/test/backtest/test_generic_engine.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/backtest/test_triggers.py` & `gs_quant-1.0.4/gs_quant/test/backtest/test_triggers.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/data/test_data_coordinate.py` & `gs_quant-1.0.4/gs_quant/test/data/test_data_coordinate.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/data/test_dataset.py` & `gs_quant-1.0.4/gs_quant/test/data/test_dataset.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 specific language governing permissions and limitations
 under the License.
 """
 import copy
 import datetime as dt
 
 import numpy as np
-from numpy import int64, float64, datetime64
 import pandas as pd
 import pytest
+from numpy import int64, float64, datetime64
 
 from gs_quant.api.gs.data import GsDataApi
 from gs_quant.data import Dataset
 from gs_quant.session import GsSession, Environment
-from gs_quant.target.data import Format
+from gs_quant.target.data import Format, DataQuery
 
 test_types = {
     'date': 'date',
     'assetId': 'string',
     'askPrice': 'number',
     'adjustedAskPrice': 'number',
     'bidPrice': 'number',
@@ -144,24 +144,114 @@
         'lowPrice': 2568.89,
         'adjustedHighPrice': 2595.32,
         'adjustedLowPrice': 2568.89,
         'updateTime': dt.datetime.strptime('2019-01-10T00:44:00Z', '%Y-%m-%dT%H:%M:%SZ')
     }
 ]
 
+tr_types = {
+    'time': 'date-time',
+    'assetId': 'string',
+    'askPrice': 'number',
+    'adjustedAskPrice': 'number',
+    'bidPrice': 'number',
+    'adjustedBidPrice': 'number',
+    'tradePrice': 'number',
+    'adjustedTradePrice': 'number',
+    'openPrice': 'number',
+    'adjustedOpenPrice': 'number',
+    'highPrice': 'number',
+    'adjustedLowPrice': 'number',
+    'lowPrice': 'number',
+    'adjustedHighPrice': 'number'
+}
+tr_data = [
+    {
+        'time': dt.datetime(2023, 5, 31, 14),
+        'assetId': 'MA4B66MW5E27U8P32SB',
+        'askPrice': 2529,
+        'adjustedAskPrice': 2529,
+        'bidPrice': 2442.55,
+        'adjustedBidPrice': 2442.55,
+        'tradePrice': 2510.03,
+        'adjustedTradePrice': 2510.03,
+        'openPrice': 2476.96,
+        'adjustedOpenPrice': 2476.96,
+        'highPrice': 2519.49,
+        'lowPrice': 2467.47,
+        'adjustedHighPrice': 2519.49,
+        'adjustedLowPrice': 2467.47
+    },
+    {
+        'time': dt.datetime(2023, 5, 31, 15),
+        'assetId': 'MA4B66MW5E27U8P32SB',
+        'askPrice': 2502.34,
+        'adjustedAskPrice': 2502.34,
+        'bidPrice': 2418.09,
+        'adjustedBidPrice': 2418.09,
+        'tradePrice': 2447.89,
+        'adjustedTradePrice': 2447.89,
+        'openPrice': 2491.92,
+        'adjustedOpenPrice': 2491.92,
+        'highPrice': 2493.14,
+        'lowPrice': 2443.96,
+        'adjustedHighPrice': 2493.14,
+        'adjustedLowPrice': 2443.96
+    },
+    {
+        'time': dt.datetime(2023, 5, 31, 16),
+        'assetId': 'MA4B66MW5E27U8P32SB'
+    },
+    {
+        'time': dt.datetime(2023, 5, 31, 17),
+        'assetId': 'MA4B66MW5E27U8P32SB',
+        'askPrice': 2566.52,
+        'adjustedAskPrice': 2566.52,
+        'bidPrice': 2487.8,
+        'adjustedBidPrice': 2487.8,
+        'tradePrice': 2531.94,
+        'adjustedTradePrice': 2531.94,
+        'openPrice': 2474.33,
+        'adjustedOpenPrice': 2474.33,
+        'highPrice': 2538.07,
+        'lowPrice': 2474.33,
+        'adjustedHighPrice': 2538.07,
+        'adjustedLowPrice': 2474.33
+    }
+]
+
 test_coverage_data = {'results': [{'gsid': 'gsid1'}]}
 
 
 def test_query_data(mocker):
-    mocker.patch("gs_quant.api.gs.data.GsDataApi.query_data", return_value=test_data)
+    mock = mocker.patch("gs_quant.api.gs.data.GsDataApi.query_data", return_value=test_data)
     mocker.patch("gs_quant.api.gs.data.GsDataApi.get_types", return_value=test_types)
     dataset = Dataset(Dataset.TR.TREOD)
     data = dataset.get_data(dt.date(2019, 1, 2), dt.date(2019, 1, 9), assetId='MA4B66MW5E27U8P32SB')
     assert data.equals(GsDataApi.construct_dataframe_with_types(str(Dataset.TR.TREOD), test_data))
 
+    assert mock.call_count == 1
+    query = mock.call_args[0][0]
+    assert type(query) == DataQuery
+    assert query.empty_intervals is None
+
+
+def test_query_data_intervals(mocker):
+    mock = mocker.patch("gs_quant.api.gs.data.GsDataApi.query_data", return_value=tr_data)
+    mocker.patch("gs_quant.api.gs.data.GsDataApi.get_types", return_value=tr_types)
+    dataset = Dataset(Dataset.TR.TREOD)
+    data = dataset.get_data(dt.datetime(2023, 5, 31, 13), dt.datetime(2023, 5, 31, 17), assetId='MA4B66MW5E27U8P32SB',
+                            intervals=4, empty_intervals=True)
+    assert data.equals(GsDataApi.construct_dataframe_with_types(str(Dataset.TR.TR), tr_data))
+
+    assert mock.call_count == 1
+    query = mock.call_args[0][0]
+    assert type(query) == DataQuery
+    assert query.empty_intervals is True
+
 
 def test_query_data_types(mocker):
     mocker.patch("gs_quant.api.gs.data.GsDataApi.query_data", return_value=test_data)
     mocker.patch("gs_quant.api.gs.data.GsDataApi.get_types", return_value=test_types)
     dataset = Dataset(Dataset.TR.TREOD)
     data = dataset.get_data(dt.date(2019, 1, 2), dt.date(2019, 1, 9), assetId='MA4B66MW5E27U8P32SB')
     assert data.equals(GsDataApi.construct_dataframe_with_types(str(Dataset.TR.TREOD), test_data))
@@ -221,14 +311,24 @@
             curr = var_schema[i]
             curr['difference_tradePrice'] = curr['tradePrice'] - prev['tradePrice']
 
     df = GsDataApi.construct_dataframe_with_types(str(Dataset.TR.TREOD), var_schema, True)
     assert np.issubdtype(df['difference_tradePrice'].dtype, np.floating)
 
 
+def test_dataframe_with_mixed_date_type(mocker):
+    mocker.patch.object(GsDataApi, 'get_types', return_value={'updateTime': 'date-time'})
+
+    df = GsDataApi.construct_dataframe_with_types('BBG_PER_SECURITY',
+                                                  [{'updateTime': '2022-02-24T19:25:28Z'},
+                                                   {'updateTime': '2022-11-10T17:18:23.021494Z'}])
+
+    assert df.empty is False
+
+
 def test_data_series_format(mocker):
     start = dt.date(2019, 1, 2)
     end = dt.datetime(2019, 1, 9)
     df = pd.DataFrame(test_data)
     index = pd.to_datetime(df.loc[:, 'date'].values)
     expected = pd.Series(index=index, data=df.loc[:, 'tradePrice'].values)
     expected = expected.rename_axis('date')
```

### Comparing `gs_quant-1.0.3/gs_quant/test/datetime_/test_date.py` & `gs_quant-1.0.4/gs_quant/test/datetime_/test_date.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/datetime_/test_gscalendar.py` & `gs_quant-1.0.4/gs_quant/test/datetime_/test_gscalendar.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/datetime_/test_point.py` & `gs_quant-1.0.4/gs_quant/test/datetime_/test_point.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/datetime_/test_relative_date.py` & `gs_quant-1.0.4/gs_quant/test/datetime_/test_relative_date.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/datetime_/test_time.py` & `gs_quant-1.0.4/gs_quant/test/datetime_/test_time.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/fixtures/content.py` & `gs_quant-1.0.4/gs_quant/test/fixtures/content.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/markets/test_baskets.py` & `gs_quant-1.0.4/gs_quant/test/markets/test_baskets.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/markets/test_hedger.py` & `gs_quant-1.0.4/gs_quant/test/markets/test_hedger.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/markets/test_instrument.py` & `gs_quant-1.0.4/gs_quant/test/markets/test_instrument.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/markets/test_portfolio.py` & `gs_quant-1.0.4/gs_quant/test/markets/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/markets/test_portfolio_manager.py` & `gs_quant-1.0.4/gs_quant/test/markets/test_portfolio_manager.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/markets/test_pricing_context.py` & `gs_quant-1.0.4/gs_quant/test/markets/test_pricing_context.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/markets/test_report.py` & `gs_quant-1.0.4/gs_quant/test/markets/test_report.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/markets/test_securities.py` & `gs_quant-1.0.4/gs_quant/test/markets/test_securities.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/models/__init__.py` & `gs_quant-1.0.4/gs_quant/test/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/models/test_epidemiology.py` & `gs_quant-1.0.4/gs_quant/test/models/test_epidemiology.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/models/test_risk_model.py` & `gs_quant-1.0.4/gs_quant/test/models/test_risk_model.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/test_base.py` & `gs_quant-1.0.4/gs_quant/test/test_base.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/timeseries/multi_measure/test_commod.py` & `gs_quant-1.0.4/gs_quant/test/timeseries/multi_measure/test_commod.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/timeseries/multi_measure/test_measure_registry.py` & `gs_quant-1.0.4/gs_quant/test/timeseries/multi_measure/test_measure_registry.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/timeseries/test_algebra.py` & `gs_quant-1.0.4/gs_quant/test/timeseries/test_algebra.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/timeseries/test_analysis.py` & `gs_quant-1.0.4/gs_quant/test/timeseries/test_analysis.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/timeseries/test_backtesting.py` & `gs_quant-1.0.4/gs_quant/test/timeseries/test_backtesting.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/timeseries/test_datetime.py` & `gs_quant-1.0.4/gs_quant/test/timeseries/test_datetime.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/timeseries/test_econometrics.py` & `gs_quant-1.0.4/gs_quant/test/timeseries/test_econometrics.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/timeseries/test_helper.py` & `gs_quant-1.0.4/gs_quant/test/timeseries/test_helper.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/timeseries/test_measures.py` & `gs_quant-1.0.4/gs_quant/test/timeseries/test_measures.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/timeseries/test_measures_countries.py` & `gs_quant-1.0.4/gs_quant/test/timeseries/test_measures_countries.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/timeseries/test_measures_fx_vol.py` & `gs_quant-1.0.4/gs_quant/test/timeseries/test_measures_fx_vol.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/timeseries/test_measures_inflation.py` & `gs_quant-1.0.4/gs_quant/test/timeseries/test_measures_inflation.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/timeseries/test_measures_portfolios.py` & `gs_quant-1.0.4/gs_quant/test/timeseries/test_measures_portfolios.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/timeseries/test_measures_rates.py` & `gs_quant-1.0.4/gs_quant/test/timeseries/test_measures_rates.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/timeseries/test_measures_reports.py` & `gs_quant-1.0.4/gs_quant/test/timeseries/test_measures_reports.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/timeseries/test_measures_risk_models.py` & `gs_quant-1.0.4/gs_quant/test/timeseries/test_measures_risk_models.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/timeseries/test_measures_xccy.py` & `gs_quant-1.0.4/gs_quant/test/timeseries/test_measures_xccy.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/timeseries/test_rolling.py` & `gs_quant-1.0.4/gs_quant/test/timeseries/test_rolling.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/timeseries/test_statistics.py` & `gs_quant-1.0.4/gs_quant/test/timeseries/test_statistics.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/timeseries/test_tca.py` & `gs_quant-1.0.4/gs_quant/test/timeseries/test_tca.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/timeseries/test_technicals.py` & `gs_quant-1.0.4/gs_quant/test/timeseries/test_technicals.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/timeseries/test_timeseries.py` & `gs_quant-1.0.4/gs_quant/test/timeseries/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/timeseries/utils.py` & `gs_quant-1.0.4/gs_quant/test/timeseries/utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/utils/datagrid_test_utils.py` & `gs_quant-1.0.4/gs_quant/test/utils/datagrid_test_utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/utils/mock_calc.py` & `gs_quant-1.0.4/gs_quant/test/utils/mock_calc.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/utils/mock_data.py` & `gs_quant-1.0.4/gs_quant/test/utils/mock_data.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/utils/mock_request.py` & `gs_quant-1.0.4/gs_quant/test/utils/mock_request.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/test/utils/test_utils.py` & `gs_quant-1.0.4/gs_quant/test/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/timeseries/__init__.py` & `gs_quant-1.0.4/gs_quant/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/timeseries/algebra.py` & `gs_quant-1.0.4/gs_quant/timeseries/algebra.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/timeseries/analysis.py` & `gs_quant-1.0.4/gs_quant/timeseries/analysis.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/timeseries/backtesting.py` & `gs_quant-1.0.4/gs_quant/timeseries/backtesting.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/timeseries/datetime.py` & `gs_quant-1.0.4/gs_quant/timeseries/datetime.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/timeseries/econometrics.py` & `gs_quant-1.0.4/gs_quant/timeseries/econometrics.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/timeseries/helper.py` & `gs_quant-1.0.4/gs_quant/timeseries/helper.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/timeseries/measure_registry.py` & `gs_quant-1.0.4/gs_quant/timeseries/measure_registry.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/timeseries/measures.py` & `gs_quant-1.0.4/gs_quant/timeseries/measures.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/timeseries/measures_countries.py` & `gs_quant-1.0.4/gs_quant/timeseries/measures_countries.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/timeseries/measures_fx_vol.py` & `gs_quant-1.0.4/gs_quant/timeseries/measures_fx_vol.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/timeseries/measures_helper.py` & `gs_quant-1.0.4/gs_quant/timeseries/measures_helper.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/timeseries/measures_inflation.py` & `gs_quant-1.0.4/gs_quant/timeseries/measures_inflation.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/timeseries/measures_portfolios.py` & `gs_quant-1.0.4/gs_quant/timeseries/measures_portfolios.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/timeseries/measures_rates.py` & `gs_quant-1.0.4/gs_quant/timeseries/measures_rates.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/timeseries/measures_reports.py` & `gs_quant-1.0.4/gs_quant/timeseries/measures_reports.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/timeseries/measures_risk_models.py` & `gs_quant-1.0.4/gs_quant/timeseries/measures_risk_models.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/timeseries/measures_xccy.py` & `gs_quant-1.0.4/gs_quant/timeseries/measures_xccy.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/timeseries/statistics.py` & `gs_quant-1.0.4/gs_quant/timeseries/statistics.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/timeseries/tca.py` & `gs_quant-1.0.4/gs_quant/timeseries/tca.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/timeseries/technicals.py` & `gs_quant-1.0.4/gs_quant/timeseries/technicals.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/tracing/__init__.py` & `gs_quant-1.0.4/gs_quant/tracing/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant/tracing/tracing.py` & `gs_quant-1.0.4/gs_quant/tracing/tracing.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant.egg-info/PKG-INFO` & `gs_quant-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gs-quant
-Version: 1.0.3
+Name: gs_quant
+Version: 1.0.4
 Summary: Goldman Sachs Quant
 Home-page: https://marquee.gs.com
 Author: Goldman Sachs
 Author-email: developer@gs.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Description: # GS Quant
```

### Comparing `gs_quant-1.0.3/gs_quant.egg-info/SOURCES.txt` & `gs_quant-1.0.4/gs_quant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/gs_quant.egg-info/requires.txt` & `gs_quant-1.0.4/gs_quant.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/setup.py` & `gs_quant-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.3/versioneer.py` & `gs_quant-1.0.4/versioneer.py`

 * *Files identical despite different names*

