# Comparing `tmp/i8-terminal-0.2.84.tar.gz` & `tmp/i8-terminal-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i8-terminal-0.2.84.tar", last modified: Wed Jun 14 20:15:18 2023, max compression
+gzip compressed data, was "i8-terminal-0.2.9.tar", last modified: Sat Jun 18 08:33:09 2022, max compression
```

## Comparing `i8-terminal-0.2.84.tar` & `i8-terminal-0.2.9.tar`

### file list

```diff
@@ -1,145 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:15:18.300191 i8-terminal-0.2.84/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-06-14 20:15:18.300191 i8-terminal-0.2.84/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:15:18.288190 i8-terminal-0.2.84/i8_terminal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:15:18.288190 i8-terminal-0.2.84/i8_terminal/api/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:15:18.288190 i8-terminal-0.2.84/i8_terminal/api/earnings/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/api/earnings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:15:18.288190 i8-terminal-0.2.84/i8_terminal/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/app/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/app/plot_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:15:18.288190 i8-terminal-0.2.84/i8_terminal/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/assets/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    10071 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/assets/i8t_chart_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    49202 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/assets/i8t_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    76185 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/assets/loading.gif
--rw-r--r--   0 runner    (1001) docker     (123)    13983 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/assets/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:15:18.288190 i8-terminal-0.2.84/i8_terminal/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:15:18.288190 i8-terminal-0.2.84/i8_terminal/commands/company/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/company/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/company/company_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/company/company_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/company/compnay_details.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:15:18.292190 i8-terminal-0.2.84/i8_terminal/commands/earnings/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/earnings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/earnings/earnings_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/earnings/earnings_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/earnings/earnings_recent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/earnings/earnings_upcoming.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:15:18.292190 i8-terminal-0.2.84/i8_terminal/commands/financials/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/financials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/financials/financials_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/financials/financials_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/financials/financials_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     8509 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/financials/financials_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:15:18.292190 i8-terminal-0.2.84/i8_terminal/commands/market/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/market/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/market/market_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:15:18.292190 i8-terminal-0.2.84/i8_terminal/commands/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/metrics/metrics_current.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/metrics/metrics_describe.py
--rw-r--r--   0 runner    (1001) docker     (123)    14560 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/metrics/metrics_historical.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/metrics/metrics_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:15:18.292190 i8-terminal-0.2.84/i8_terminal/commands/news/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/news/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/news/news_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:15:18.292190 i8-terminal-0.2.84/i8_terminal/commands/notebook/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/notebook/notebook_launch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:15:18.292190 i8-terminal-0.2.84/i8_terminal/commands/price/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/price/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/price/price_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/price/price_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/price/price_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:15:18.292190 i8-terminal-0.2.84/i8_terminal/commands/screen/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/screen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/screen/screen_gainers.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/screen/screen_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/screen/screen_losers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/screen/screen_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:15:18.292190 i8-terminal-0.2.84/i8_terminal/commands/user/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/user/user_login.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/user/user_logout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/user/webserver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:15:18.292190 i8-terminal-0.2.84/i8_terminal/commands/watchlist/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/watchlist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/watchlist/watchlist_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/watchlist/watchlist_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/watchlist/watchlist_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/watchlist/watchlist_financials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/watchlist/watchlist_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/watchlist/watchlist_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/watchlist/watchlist_rm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/commands/watchlist/watchlist_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:15:18.296190 i8-terminal-0.2.84/i8_terminal/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/common/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11927 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/common/financials.py
--rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/common/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/common/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/common/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/common/price.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/common/screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/common/stock_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/i8_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:15:18.296190 i8-terminal-0.2.84/i8_terminal/i8_terminal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-06-14 20:15:18.000000 i8-terminal-0.2.84/i8_terminal/i8_terminal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-06-14 20:15:18.000000 i8-terminal-0.2.84/i8_terminal/i8_terminal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 20:15:18.000000 i8-terminal-0.2.84/i8_terminal/i8_terminal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-14 20:15:18.000000 i8-terminal-0.2.84/i8_terminal/i8_terminal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-14 20:15:18.000000 i8-terminal-0.2.84/i8_terminal/i8_terminal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 20:15:18.000000 i8-terminal-0.2.84/i8_terminal/i8_terminal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:15:18.296190 i8-terminal-0.2.84/i8_terminal/service_result/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/service_result/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/service_result/column_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/service_result/columns_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/service_result/earning_list_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/service_result/service_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:15:18.296190 i8-terminal-0.2.84/i8_terminal/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/services/earnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:15:18.300191 i8-terminal-0.2.84/i8_terminal/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/types/auto_complete_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/types/chart_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/types/command_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/types/condition_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/types/fin_identifier_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/types/fin_period_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/types/fin_statement_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/types/i8_auto_suggest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10920 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/types/i8_completer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/types/indicator_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/types/market_indice_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/types/metric_identifier_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/types/metric_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/types/metric_view_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/types/output_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/types/period_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/types/period_type_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/types/price_period_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/types/screening_condition_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/types/screening_operator_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/types/screening_value_field_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/types/sort_order_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/types/ticker_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/types/user_watchlist_tickers_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/types/user_watchlists_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/utils_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/i8_terminal/version.txt
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 20:15:18.300191 i8-terminal-0.2.84/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-14 20:14:13.000000 i8-terminal-0.2.84/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 08:33:09.160778 i8-terminal-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      112 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3196 2022-06-18 08:33:09.160778 i8-terminal-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2639 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 08:33:09.148778 i8-terminal-0.2.9/i8_terminal/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 08:33:09.148778 i8-terminal-0.2.9/i8_terminal/app/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6618 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/app/layout.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5098 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/app/plot_server.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 08:33:09.148778 i8-terminal-0.2.9/i8_terminal/assets/
+-rw-r--r--   0 runner    (1001) docker     (121)     2653 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/assets/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)    10071 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/assets/i8t_chart_logo.png
+-rw-r--r--   0 runner    (1001) docker     (121)    49202 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/assets/i8t_logo.png
+-rw-r--r--   0 runner    (1001) docker     (121)    76185 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/assets/loading.gif
+-rw-r--r--   0 runner    (1001) docker     (121)    13983 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/assets/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 08:33:09.148778 i8-terminal-0.2.9/i8_terminal/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)      426 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 08:33:09.148778 i8-terminal-0.2.9/i8_terminal/commands/company/
+-rw-r--r--   0 runner    (1001) docker     (121)      185 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/company/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9590 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/company/company_compare.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1279 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/company/company_search.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2776 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/company/compnay_details.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 08:33:09.152778 i8-terminal-0.2.9/i8_terminal/commands/earnings/
+-rw-r--r--   0 runner    (1001) docker     (121)      135 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/earnings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1967 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/earnings/earnings_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3533 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/earnings/earnings_plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1910 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/earnings/earnings_recent.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2739 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/earnings/earnings_upcoming.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 08:33:09.152778 i8-terminal-0.2.9/i8_terminal/commands/financials/
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/financials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7407 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/financials/financials_compare.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/financials/financials_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4459 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/financials/financials_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8262 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/financials/financials_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 08:33:09.152778 i8-terminal-0.2.9/i8_terminal/commands/market/
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/market/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10108 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/market/market_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 08:33:09.152778 i8-terminal-0.2.9/i8_terminal/commands/metrics/
+-rw-r--r--   0 runner    (1001) docker     (121)      133 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1204 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/metrics/metrics_describe.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2096 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/metrics/metrics_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8560 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/metrics/metrics_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 08:33:09.152778 i8-terminal-0.2.9/i8_terminal/commands/news/
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/news/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2407 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/news/news_list.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 08:33:09.152778 i8-terminal-0.2.9/i8_terminal/commands/price/
+-rw-r--r--   0 runner    (1001) docker     (121)      149 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/price/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5130 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/price/price_compare.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2803 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/price/price_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10367 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/price/price_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 08:33:09.152778 i8-terminal-0.2.9/i8_terminal/commands/screen/
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/screen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      292 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/screen/screen_list.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 08:33:09.152778 i8-terminal-0.2.9/i8_terminal/commands/user/
+-rw-r--r--   0 runner    (1001) docker     (121)      107 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1717 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/user/user_login.py
+-rw-r--r--   0 runner    (1001) docker     (121)      428 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/user/user_logout.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1843 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/user/webserver.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 08:33:09.156778 i8-terminal-0.2.9/i8_terminal/commands/watchlist/
+-rw-r--r--   0 runner    (1001) docker     (121)      135 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/watchlist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1688 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/watchlist/watchlist_add.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/watchlist/watchlist_create.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2241 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/watchlist/watchlist_financials.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1330 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/watchlist/watchlist_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2536 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/watchlist/watchlist_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1799 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/watchlist/watchlist_rm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2207 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/commands/watchlist/watchlist_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 08:33:09.156778 i8-terminal-0.2.9/i8_terminal/common/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1729 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/common/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11753 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/common/financials.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4117 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/common/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1740 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/common/layout.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4998 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/common/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3654 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/common/price.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1288 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/common/stock_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2885 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4564 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      966 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/config.yml
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/i8_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 08:33:09.156778 i8-terminal-0.2.9/i8_terminal/i8_terminal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3196 2022-06-18 08:33:09.000000 i8-terminal-0.2.9/i8_terminal/i8_terminal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3553 2022-06-18 08:33:09.000000 i8-terminal-0.2.9/i8_terminal/i8_terminal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-18 08:33:09.000000 i8-terminal-0.2.9/i8_terminal/i8_terminal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-06-18 08:33:09.000000 i8-terminal-0.2.9/i8_terminal/i8_terminal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      242 2022-06-18 08:33:09.000000 i8-terminal-0.2.9/i8_terminal/i8_terminal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-06-18 08:33:09.000000 i8-terminal-0.2.9/i8_terminal/i8_terminal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5468 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/main.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 08:33:09.160778 i8-terminal-0.2.9/i8_terminal/types/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2138 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/types/auto_complete_choice.py
+-rw-r--r--   0 runner    (1001) docker     (121)      705 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/types/chart_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1917 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/types/command_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1137 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/types/fin_identifier_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)      914 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/types/fin_period_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)      782 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/types/fin_statement_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2222 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/types/i8_auto_suggest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6929 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/types/i8_completer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1909 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/types/indicator_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)      750 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/types/metric_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)      685 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/types/period_type_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)      810 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/types/price_period_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)      592 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/types/ticker_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1049 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/types/user_watchlist_tickers_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1024 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/types/user_watchlists_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1030 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/i8_terminal/version.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      174 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      241 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-18 08:33:09.160778 i8-terminal-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1380 2022-06-18 08:32:34.000000 i8-terminal-0.2.9/setup.py
```

### Comparing `i8-terminal-0.2.84/LICENSE` & `i8-terminal-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.84/PKG-INFO` & `i8-terminal-0.2.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,100 +1,92 @@
 Metadata-Version: 2.1
 Name: i8-terminal
-Version: 0.2.84
+Version: 0.2.9
 Summary: Investor8 CLI
 Home-page: UNKNOWN
 Author: investoreight
 Author-email: info@investoreight.com
 License: MIT
 Project-URL: Homepage, https://i8terminal.io/
 Project-URL: Documentation, https://docs.i8terminal.io/
 Project-URL: Download, https://i8terminal.io/download
 Project-URL: Source Code, https://github.com/investoreight/i8-terminal
 Project-URL: Bug Tracker, https://github.com/investoreight/i8-terminal/issues
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# i8 Terminal: Modern Market Research powered by the Command-Line
+# i8 Terminal: Modern Market Research with the Power of Command-Line
 
-[i8 terminal](https://www.i8terminal.io) is a modern python-based terminal application that gives you superior power and flexibility to understand and analyze the market. The interface is simple, efficient, and powerful: it's command-line!
+[i8 terminal](https://www.i8terminal.io) is a modern python-based terminal application that gives you a superior power and flexibility to understand and analyze the market. The interface is simple, efficient, and powerful: it's command-line!
 
 i8 Terminal is backed by the [Investoreight Platform](https://www.investoreight.com) and currently covers major U.S. exchanges.
 
 ## Features and Highlights
 - Prompt Market Insights and Analysis
 - Custom Charting, Reporting, and Visualizations
 - Powerful and Customizable Screening
 - Easy-to-Use and Extendable
 - Backed by the [Investoreight Platform](https://www.investoreight.com)
 
 ![i8 Terminal Features](https://www.i8terminal.io/img/gif/i8-terminal-demo.gif)
 
 ## i8 Terminal Commands
-i8 Terminal offers some built-in commands to analyze and research the market. You can also create your own custom commands or extend the existing command. Find an overview of commands [here](https://i8terminal.io/#commands).
+i8 Terminal offer some built-in commands to analyze and research the market. You can also create your own custom commands or extend the existing command. Find an overview of commands [here](https://i8terminal.io/#commands).
 
-Check out the following video to see some more commands from i8 Terminal:
+Checkout the following video to see some more commands from i8 Terminal:
 
 [![i8 Terminal Sample Commands](https://img.youtube.com/vi/NpOCqcb-RxY/0.jpg)](https://www.youtube.com/watch?v=NpOCqcb-RxY)
 
 
 ## Installing i8 Terminal
-**Note**: i8 Terminal currently only supports Python 3.9+
+**Note**: i8 Terminal currenly only supports Python 3.9+
 
 If you have Python 3 installed, you can simply install the tool with Python pip:
 
 ```
 pip install i8-terminal
 ```
 
-We recommend installing i8 terminal in an isolated virtual environment. This can be done as follows:
+We recommend to install i8 terminal in an isolated virtual environment. This can be done as follows:
 
 #### On Mac OS or Linux:
 
 ```
-python3 -m venv .venv
-source .venv/bin/activate
+python3 -m venv .venv 
+source .venv/bin/activate 
 pip install i8-terminal
 ```
 
 #### On Windows:
 
 ```
-python3 -m venv .venv
-source .venv/Script/activate
+python3 -m venv .venv 
+source .venv/Script/activate 
 pip install i8-terminal
 ```
 
 ### Install i8 Terminal using the Windows Installer
-On Windows, you can also install i8 Terminal using the Windows executable. Check [here](https://i8terminal.io/download) if you want to download the windows executable.
+On Windows you can also install i8 Terminal using the windows executable. Check [here](https://i8terminal.io/download) if you want to download the windows executable.
 
 
-## How to Contribute i8 Terminal
-The preferred workflow for contributing to i8 Terminal is to clone the
-[GitHub repository](https://github.com/investoreight/i8-terminal), develop on a branch and make a Pull Request.
-
-See [here](https://github.com/investoreight/i8-terminal/blob/main/CONTRIBUTING.md) for guidelines for contributors.
-
-i8 Terminal is built on top of the [Investoreight Core API](https://github.com/investoreight/investor8-sdk).
-
 ## How to Run i8 Terminal
-You can verify whether i8 Terminal is installed successfully by running i8 script:
+You can verify whether i8 Terminal is installed succefully by running i8 script:
 
 ```
 i8
 ```
 
-If you are using the application for the first time, you should first sign in. Run the following command, which will open a browser and redirect you to the investoreight platform to sign in (or sign up):
+If you are using the application for the first time, you should first sign in. Run the following command, which will open a browser and redirects you to the investoreight platform to sing in (or sign up):
 
 ```
 i8 user login
 ```
 
-After a successful login, the most convenient way to use i8 terminal is to use its own shell:
+After a succesful login, the most convenient way to use i8 terminal is to use its own shell:
 
 ```
 i8 shell
 ```
 
 You should now be able to run i8 commands. Check our [documentation](https://docs.i8terminal.io/) for more details.
```

### Comparing `i8-terminal-0.2.84/README.md` & `i8-terminal-0.2.9/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,83 +1,75 @@
-# i8 Terminal: Modern Market Research powered by the Command-Line
+# i8 Terminal: Modern Market Research with the Power of Command-Line
 
-[i8 terminal](https://www.i8terminal.io) is a modern python-based terminal application that gives you superior power and flexibility to understand and analyze the market. The interface is simple, efficient, and powerful: it's command-line!
+[i8 terminal](https://www.i8terminal.io) is a modern python-based terminal application that gives you a superior power and flexibility to understand and analyze the market. The interface is simple, efficient, and powerful: it's command-line!
 
 i8 Terminal is backed by the [Investoreight Platform](https://www.investoreight.com) and currently covers major U.S. exchanges.
 
 ## Features and Highlights
 - Prompt Market Insights and Analysis
 - Custom Charting, Reporting, and Visualizations
 - Powerful and Customizable Screening
 - Easy-to-Use and Extendable
 - Backed by the [Investoreight Platform](https://www.investoreight.com)
 
 ![i8 Terminal Features](https://www.i8terminal.io/img/gif/i8-terminal-demo.gif)
 
 ## i8 Terminal Commands
-i8 Terminal offers some built-in commands to analyze and research the market. You can also create your own custom commands or extend the existing command. Find an overview of commands [here](https://i8terminal.io/#commands).
+i8 Terminal offer some built-in commands to analyze and research the market. You can also create your own custom commands or extend the existing command. Find an overview of commands [here](https://i8terminal.io/#commands).
 
-Check out the following video to see some more commands from i8 Terminal:
+Checkout the following video to see some more commands from i8 Terminal:
 
 [![i8 Terminal Sample Commands](https://img.youtube.com/vi/NpOCqcb-RxY/0.jpg)](https://www.youtube.com/watch?v=NpOCqcb-RxY)
 
 
 ## Installing i8 Terminal
-**Note**: i8 Terminal currently only supports Python 3.9+
+**Note**: i8 Terminal currenly only supports Python 3.9+
 
 If you have Python 3 installed, you can simply install the tool with Python pip:
 
 ```
 pip install i8-terminal
 ```
 
-We recommend installing i8 terminal in an isolated virtual environment. This can be done as follows:
+We recommend to install i8 terminal in an isolated virtual environment. This can be done as follows:
 
 #### On Mac OS or Linux:
 
 ```
-python3 -m venv .venv
-source .venv/bin/activate
+python3 -m venv .venv 
+source .venv/bin/activate 
 pip install i8-terminal
 ```
 
 #### On Windows:
 
 ```
-python3 -m venv .venv
-source .venv/Script/activate
+python3 -m venv .venv 
+source .venv/Script/activate 
 pip install i8-terminal
 ```
 
 ### Install i8 Terminal using the Windows Installer
-On Windows, you can also install i8 Terminal using the Windows executable. Check [here](https://i8terminal.io/download) if you want to download the windows executable.
+On Windows you can also install i8 Terminal using the windows executable. Check [here](https://i8terminal.io/download) if you want to download the windows executable.
 
 
-## How to Contribute i8 Terminal
-The preferred workflow for contributing to i8 Terminal is to clone the
-[GitHub repository](https://github.com/investoreight/i8-terminal), develop on a branch and make a Pull Request.
-
-See [here](https://github.com/investoreight/i8-terminal/blob/main/CONTRIBUTING.md) for guidelines for contributors.
-
-i8 Terminal is built on top of the [Investoreight Core API](https://github.com/investoreight/investor8-sdk).
-
 ## How to Run i8 Terminal
-You can verify whether i8 Terminal is installed successfully by running i8 script:
+You can verify whether i8 Terminal is installed succefully by running i8 script:
 
 ```
 i8
 ```
 
-If you are using the application for the first time, you should first sign in. Run the following command, which will open a browser and redirect you to the investoreight platform to sign in (or sign up):
+If you are using the application for the first time, you should first sign in. Run the following command, which will open a browser and redirects you to the investoreight platform to sing in (or sign up):
 
 ```
 i8 user login
 ```
 
-After a successful login, the most convenient way to use i8 terminal is to use its own shell:
+After a succesful login, the most convenient way to use i8 terminal is to use its own shell:
 
 ```
 i8 shell
 ```
 
 You should now be able to run i8 commands. Check our [documentation](https://docs.i8terminal.io/) for more details.
```

### Comparing `i8-terminal-0.2.84/i8_terminal/app/layout.py` & `i8-terminal-0.2.9/i8_terminal/app/layout.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.84/i8_terminal/app/plot_server.py` & `i8-terminal-0.2.9/i8_terminal/app/plot_server.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import contextlib
 import logging
 import os
-import socket
 import sys
 import webbrowser
 from threading import Timer
 from typing import Any, Dict, List, Tuple
 
 import dash
 import dash_bootstrap_components as dbc
@@ -145,23 +144,14 @@
 def serve_plot(fig: go.Figure, cmd_context: Dict[str, Any]) -> None:
     _configure_dash()
 
     APP.layout = create_plot_layout(fig, cmd_context)
     APP.title = f"i8 Terminal: {cmd_context['plot_title']}"
     app_url = f"http://localhost:{APP_SETTINGS['app']['port']}/"
     console = Console()
-    with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
-        is_port_in_use = s.connect_ex(("localhost", APP_SETTINGS["app"]["port"])) == 0
-    if is_port_in_use:
-        console.print(
-            f"Port number {APP_SETTINGS['app']['port']} is already in use. Please make sure that only one instance of \
-                i8-terminal runs at a time!",
-            style="yellow",
-        )
-        return
     with open(os.devnull, "w") as f, contextlib.redirect_stderr(f):
         Timer(2, lambda: webbrowser.open_new(app_url)).start()
         console.print(
             f'[bold green]Your plot is serving on http://127.0.0.1:{APP_SETTINGS["app"]["port"]}/[/bold green]'
         )
         console.print("Press `Ctrl + C` to stop the webserver.")
         if APP.logger.hasHandlers():
```

### Comparing `i8-terminal-0.2.84/i8_terminal/assets/favicon.ico` & `i8-terminal-0.2.9/i8_terminal/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.84/i8_terminal/assets/i8t_chart_logo.png` & `i8-terminal-0.2.9/i8_terminal/assets/i8t_chart_logo.png`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.84/i8_terminal/assets/i8t_logo.png` & `i8-terminal-0.2.9/i8_terminal/assets/i8t_logo.png`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.84/i8_terminal/assets/loading.gif` & `i8-terminal-0.2.9/i8_terminal/assets/loading.gif`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.84/i8_terminal/assets/styles.css` & `i8-terminal-0.2.9/i8_terminal/assets/styles.css`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.84/i8_terminal/commands/company/company_compare.py` & `i8-terminal-0.2.9/i8_terminal/commands/financials/financials_compare.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,176 +1,193 @@
-from typing import Dict, Optional
+from typing import Any, Dict, List, Optional
 
 import click
+import investor8_sdk
 import numpy as np
-import pandas as pd
-from pandas import DataFrame
+import plotly.graph_objects as go
+from pandas.core.frame import DataFrame
 from rich.console import Console
-from rich.panel import Panel
-from rich.table import Table
-from rich.tree import Tree
-
-from i8_terminal.commands.company import company
-from i8_terminal.common.cli import pass_command
-from i8_terminal.common.layout import format_metrics_df
-from i8_terminal.common.metrics import get_current_metrics_df
-from i8_terminal.common.stock_info import validate_tickers
-from i8_terminal.common.utils import export_to_html
-from i8_terminal.config import APP_SETTINGS, get_table_style
-from i8_terminal.types.ticker_param_type import TickerParamType
-
-
-def get_section_stock_infos_df(tickers: str, target: str, section: Dict[str, str]) -> Optional[DataFrame]:
-    df = get_current_metrics_df(tickers, section["metrics"])
-    if df is None:
+
+from i8_terminal.app.layout import get_plot_default_layout
+from i8_terminal.app.plot_server import serve_plot
+from i8_terminal.commands.financials import financials
+from i8_terminal.common.cli import get_click_command_path, pass_command
+from i8_terminal.common.metrics import get_all_metrics_df
+from i8_terminal.common.utils import PlotType, export_data
+from i8_terminal.config import APP_SETTINGS
+from i8_terminal.types.period_type_param_type import PeriodTypeParamType
+
+from i8_terminal.types.fin_statement_param_type import FinancialStatementParamType  # isort:skip
+
+from i8_terminal.types.fin_identifier_param_type import FinancialsIdentifierParamType  # isort:skip
+
+from i8_terminal.common.financials import (  # isort:skip
+    find_similar_statement,
+    get_statements_codes,
+    get_statements_disp_name,
+    fin_df2export_df,
+    fin_df2Tree,
+    parse_identifier,
+    prepare_financials_df,
+)
+
+
+def get_standardized_financials(
+    identifiers_list: List[Dict[str, str]],
+    statement: str,
+    period_type: str,
+    period_size: int = 4,
+    exportize: Optional[bool] = False,
+) -> Optional[Dict[str, Any]]:
+    fins = []
+    for idf in identifiers_list:
+        resp = None
+        try:
+            if idf.get("fiscal_year"):
+                resp = investor8_sdk.FinancialsApi().get_financials_single(
+                    ticker=idf["ticker"],
+                    stat_code=statement,
+                    fiscal_year=idf.get("fiscal_year"),
+                    fiscal_period=idf.get("fiscal_period"),
+                )
+            else:
+                if not period_type:
+                    period_type = "Q" if statement == "balance_sheet_statement" else "FY"
+                resp = investor8_sdk.FinancialsApi().get_latest_standardized_financials(
+                    ticker=idf["ticker"], stat_code=statement
+                )[period_type]
+            if resp:
+                fins.append(resp)
+        except Exception:
+            continue
+    if not fins:
         return None
-    if section["name"] == "Financials":
-        fyq_rows = []
-        for ticker, ticker_df in df.groupby("Ticker"):
-            fyq_rows.append(
-                {
-                    "Ticker": ticker,
-                    "metric_name": "fyq",
-                    "value": ticker_df["period"].values[0],
-                    "display_name": "FYQ",
-                    "data_format": "str",
-                    "display_format": "str",
-                }
-            )
-        df = pd.concat([pd.DataFrame(fyq_rows), df], ignore_index=True, axis=0)
-    formatted_df = format_metrics_df(df, target)
-    formatted_df = formatted_df.pivot(index="display_name", columns="Ticker", values="value").reset_index(level=0)
-    formatted_df["Section"] = section["name"]
-    sorter = df["display_name"].unique()
-    sorter_index = dict(zip(sorter, range(len(sorter))))
-    formatted_df["Rank"] = formatted_df["display_name"].map(sorter_index)
-    formatted_df.sort_values("Rank", inplace=True)
-    formatted_df.drop("Rank", axis=1, inplace=True)
-    return formatted_df
-
-
-def get_stock_infos_df(tickers: str, target: str) -> Optional[DataFrame]:
-    return (
-        pd.concat(
-            [
-                get_section_stock_infos_df(tickers, target, section)
-                for section in APP_SETTINGS["commands"]["company_compare"]["metric_groups"]
-            ]
-        )
-        .rename(columns={"display_name": "Name"})
-        .astype(object)
-        .replace(np.nan, "N/A")
-    )
+    return prepare_financials_df(fins, period_size, include_ticker=True, exportize=exportize)
 
 
-def companies_df2tree(df: DataFrame, tickers: str) -> Tree:
-    tickers_list = tickers.replace(" ", "").upper().split(",")
-    col_width = 40
-    plot_title = f"Comparison of {', '.join(tickers_list)}"
-    plot_title = " and ".join(plot_title.rsplit(", ", 1))
-    tree = Tree(Panel(plot_title, width=50))
-    # Add header table to tree
-    header_table = Table(
-        width=50 + (col_width * (len(tickers_list) - 1)), show_lines=False, show_header=False, box=None
-    )
-    header_table.add_column(width=35, style="magenta")
-    for p in tickers_list:
-        header_table.add_column(width=col_width, justify="right", style="magenta")
-    header_table.add_row("Ticker", *tickers_list)
-    tree.add(header_table)
-
-    table_style = get_table_style("company_compare")
-
-    for sec_name, sec_values in df.groupby("Section", sort=False):
-        sec_branch = tree.add(f"[magenta]{sec_name}")
-        for i, r in sec_values.reset_index().iterrows():
-            t = Table(
-                width=46 + (col_width * (len(tickers_list) - 1)),
-                show_lines=False,
-                show_header=False,
-                box=None,
-                row_styles=[table_style["row_styles"][i % 2]],
+def create_fig(df: DataFrame, header_dict: Dict[str, List[str]], cmd_context: Dict[str, Any]) -> go.Figure:
+    cells_fill_color = [["rgb(200, 212, 227)", "rgb(235, 240, 248)"]] * len(df.columns)
+    cells_data = list(df.to_dict("list").values())
+    # Add end_date row to cells data
+    cells_data = [[(["End Date"] + header_dict["end_date"])[idx]] + d for idx, d in enumerate(cells_data)]
+    fig = go.Figure(
+        data=[
+            go.Table(
+                columnwidth=[58, 25],
+                header=dict(
+                    values=[""] + ["<b>" + p.replace("\n", " ") + "</b>" for p in header_dict["period"]],
+                    align=["left", "center"],
+                    height=32,
+                    font_size=14,
+                ),
+                cells=dict(
+                    fill_color=cells_fill_color, values=cells_data, align=["left", "right"], height=28, font_size=14
+                ),
             )
-            t.add_column(width=31)
-            for tk in tickers_list:
-                t.add_column(width=col_width, justify="right")
-            t.add_row(r["Name"], *[f"{d}" for d in r[tickers_list].values])
-            sec_branch.add(t)
-
-    return tree
+        ]
+    )
+    fig.update_layout(
+        title=cmd_context["plot_title"],
+        margin=dict(b=15, l=25, r=25),
+        **get_plot_default_layout(),
+    )
 
+    return fig
 
-def export_companies_data(
-    export_df: pd.DataFrame,
-    export_path: str,
-) -> None:
-    console = Console()
-    extension = export_path.split(".")[-1]
-    if extension == "csv":
-        export_df.drop(columns=["Section"], inplace=True)  # type: ignore
-        export_df.to_csv(export_path, index=False)
-        console.print(f"Data is saved on: {export_path}")
-    elif extension == "xlsx":
-        writer = pd.ExcelWriter(export_path, engine="xlsxwriter")
-        for sec_name, sec_values in export_df.groupby("Section", sort=False):
-            sec_values.drop(columns=["Section"], inplace=True)  # type: ignore
-            sec_values.rename(columns={"Name": ""}, inplace=True)
-            sec_values.to_excel(writer, sheet_name=sec_name, startrow=1, header=False, index=False)
-            workbook = writer.book
-            column_width = 18
-            header_format = workbook.add_format(APP_SETTINGS["styles"]["xlsx"]["default"]["header"])
-            metric_format = workbook.add_format(APP_SETTINGS["styles"]["xlsx"]["default"]["metric"])
-            column_format = workbook.add_format(APP_SETTINGS["styles"]["xlsx"]["company"]["column"])
-            worksheet = writer.sheets[sec_name]
-            headers = sec_values.columns.tolist()
-            for col_num, value in enumerate(headers):
-                if type(value) is tuple:
-                    worksheet.merge_range(0, col_num, len(value) - 1, col_num, " ".join(reversed(value)), header_format)
-                else:
-                    worksheet.write(0, col_num, value, header_format)
-            worksheet.set_column(0, 0, 20, metric_format)
-            worksheet.set_column(1, len(sec_values.columns) - 1, column_width, column_format)
-        writer.save()
-        console.print(f"Data is saved on: {export_path}")
-    else:
-        console.print("export_path is not valid")
 
-
-@company.command()
+@financials.command()
+@click.pass_context
 @click.option(
-    "--tickers",
-    "-k",
-    type=TickerParamType(),
+    "--identifiers",
+    "-i",
+    type=FinancialsIdentifierParamType(),
     required=True,
-    callback=validate_tickers,
-    help="Comma-separated list of tickers.",
+    help="Comma-separated list of identifiers.",
+)
+@click.option(
+    "--statement",
+    "-s",
+    type=FinancialStatementParamType(),
+    default="income",
+    help="Type of financial statement.",
 )
+@click.option(
+    "--period_type",
+    "-m",
+    type=PeriodTypeParamType(),
+    help="Period by which you want to view the report. Possible values are `FY` for yearly, `Q` for quarterly, and `TTM` for TTM reports.",
+)
+@click.option("--plot", is_flag=True, default=False, help="Plot results on the browser.")
 @click.option("--export", "export_path", "-e", help="Filename to export the output to.")
 @pass_command
-def compare(tickers: str, export_path: Optional[str]) -> None:
-    """
-    Compare details of the given companies. TICKERS is a comma-separated list of tickers.
-
-    Examples:
-
-    `i8 company compare --tickers MSFT,AAPL`
-
-    """
+def compare(
+    ctx: click.Context,
+    identifiers: str,
+    statement: str,
+    period_type: str,
+    plot: bool,
+    export_path: Optional[str],
+) -> None:
+    matched_statement = find_similar_statement(statement)
+    if not matched_statement:
+        click.echo(
+            f"`{statement}` is not a valid statement code. \nValid statement codes: {', '.join(get_statements_codes())}"
+        )
+        return
+    identifiers_list = identifiers.replace(" ", "").upper().split(",")
+    parsed_identifiers_list = [parse_identifier(i, period_type) for i in identifiers_list]
+    # Remove duplicates identifiers
+    parsed_identifiers_list = [dict(t) for t in {tuple(d.items()) for d in parsed_identifiers_list}]
+    tickers_list = list(set([d["ticker"] for d in parsed_identifiers_list]))
+    plot_title = f"Comparison of {', '.join(tickers_list)} {get_statements_disp_name(matched_statement)}s"
+    plot_title = " and ".join(plot_title.rsplit(", ", 1))
     console = Console()
     with console.status("Fetching data...", spinner="material") as status:
-        stock_infos_df = get_stock_infos_df(tickers, target="store" if export_path else "console")
-        if stock_infos_df is None:
+        fins = get_standardized_financials(
+            parsed_identifiers_list,
+            matched_statement,
+            period_type,
+            period_size=4,
+            exportize=True if export_path else False,
+        )
+        if fins is None:
             status.stop()
             click.echo("No data found!")
             return
-    if export_path:
-        if export_path.split(".")[-1] == "html":
-            tree = companies_df2tree(stock_infos_df, tickers)
-            export_to_html(tree, export_path)
-            return
-        export_companies_data(
-            stock_infos_df,
+        periods_list = fins["data"].columns[1:].to_list()
+        df_metrics = get_all_metrics_df()
+        df = fins["data"].merge(df_metrics, on="tag_fullname", how="left")
+        df["section_name"] = df["section_name"].apply(lambda x: "Others" if not x or x == "-" else x)
+        df = df.astype(object).replace(np.nan, None)  # Replace nan with None
+        if plot:
+            cmd_context = {
+                "plot_title": plot_title,
+                "command_path": get_click_command_path(ctx, {"--statement": matched_statement}),
+                "tickers": tickers_list,
+                "plot_type": PlotType.TABLE.value,
+            }
+            df = df[df["is_significant"] != False]
+            df = df[["name", *fins["data"].columns[1:]]]
+            df.rename(columns={"name": ""}, inplace=True)
+            fig = create_fig(df, fins["header"], cmd_context)
+
+    missing_tickers = set(tickers_list) - set(fins["header"].get("ticker", set()))
+    if missing_tickers:
+        missing_tickers_str = " and ".join(", ".join(missing_tickers).rsplit(", ", 1))
+        console.print(f'The specified financials for ticker(s) "{missing_tickers_str}" are not available.')
+        console.print("To see the covered financials check the [magenta]financials coverage[magenta] command.")
+
+    if plot and export_path:
+        console.print("The plot and export options are not compatible to use together")
+    elif plot:
+        serve_plot(fig, cmd_context)
+    elif export_path:
+        export_df = fin_df2export_df(df, periods_list)
+        export_data(
+            export_df,
             export_path,
+            column_width=22,
+            column_format=APP_SETTINGS["styles"]["xlsx"]["financials"]["column"],
         )
     else:
-        tree = companies_df2tree(stock_infos_df, tickers)
+        tree = fin_df2Tree(df, fins["header"], periods_list, title=plot_title)
         console.print(tree)
```

### Comparing `i8-terminal-0.2.84/i8_terminal/commands/company/company_search.py` & `i8-terminal-0.2.9/i8_terminal/commands/company/company_search.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,37 +9,34 @@
 from i8_terminal.common.cli import pass_command
 from i8_terminal.common.layout import df2Table, format_df
 
 
 def search_stocks_df(keyword: str) -> DataFrame:
     results = investor8_sdk.SearchApi().search_stocks(keyword, 8)
     df = DataFrame([d.to_dict() for d in results])
-    return df[["ticker", "name"]]
+    return df[["ticker", "name", "exchange", "sector"]]
 
 
 def format_stocks_df(df: DataFrame, target: str) -> DataFrame:
     formatters: Dict[str, Any] = {}
     col_names = {
         "ticker": "Ticker",
         "name": "Name",
+        "exchange": "Exchange",
+        "sector": "Sector",
     }
     return format_df(df, col_names, formatters)
 
 
 @company.command()
 @click.option("--keyword", "-k", required=True, help="Keyword can be ticker or company name.")
 @pass_command
 def search(keyword: str) -> None:
     """
-    Searches and shows all securities that match with the given KEYWORD.
-
-    Examples:
-
-    `i8 company search --keyword apl`
-
+    Searches and all securities that matches with the given KEYWORD.
     """
     console = Console()
     with console.status("Fetching data...", spinner="material"):
         df = search_stocks_df(keyword)
     df_formatted = format_stocks_df(df, "console")
     table = df2Table(df_formatted)
     console.print(table)
```

### Comparing `i8-terminal-0.2.84/i8_terminal/commands/company/compnay_details.py` & `i8-terminal-0.2.9/i8_terminal/commands/company/compnay_details.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from rich.panel import Panel
 from rich.table import Table
 from rich.text import Text
 
 from i8_terminal.commands.company import company
 from i8_terminal.common.cli import pass_command
 from i8_terminal.common.formatting import format_number
-from i8_terminal.common.stock_info import validate_ticker
+from i8_terminal.common.utils import validate_ticker
 from i8_terminal.types.ticker_param_type import TickerParamType
 
 
 def make_layout() -> Layout:
     """Define the layout."""
     layout = Layout(name="root")
 
@@ -53,16 +53,15 @@
 
 @company.command()
 @click.option(
     "--ticker", "-k", type=TickerParamType(), required=True, callback=validate_ticker, help="Ticker or company name."
 )
 @pass_command
 def details(ticker: str) -> None:
-    """
-    Get details for a given company.
+    """Get details for a given company.
 
     Examples:
 
     `i8 company details --ticker MSFT`
 
     """
     template = """
```

### Comparing `i8-terminal-0.2.84/i8_terminal/commands/earnings/earnings_list.py` & `i8-terminal-0.2.9/i8_terminal/commands/watchlist/watchlist_summary.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,56 @@
-from typing import Optional
+from typing import Any, Dict, Optional
 
 import click
+import investor8_sdk
+import pandas as pd
 from rich.console import Console
 
-import i8_terminal.api.earnings as earnings_api
-from i8_terminal.commands.earnings import earnings
+from i8_terminal.commands.watchlist import watchlist
 from i8_terminal.common.cli import pass_command
 from i8_terminal.common.layout import df2Table
-from i8_terminal.common.stock_info import validate_ticker
-from i8_terminal.common.utils import export_data, export_to_html
-from i8_terminal.config import APP_SETTINGS
-from i8_terminal.service_result.earning_list_result import EarningsListResult
-from i8_terminal.types.ticker_param_type import TickerParamType
+from i8_terminal.common.utils import export_data
+from i8_terminal.config import APP_SETTINGS, USER_SETTINGS
 
+from i8_terminal.common.metrics import get_current_metrics_df, prepare_current_metrics_formatted_df  # isort:skip
 
-@earnings.command()
-@click.option("--ticker", "-k", type=TickerParamType(), required=True, callback=validate_ticker, help="Company ticker.")
-@click.option("--export", "export_path", "-e", help="Filename to export the output to.")
-@pass_command
-def list(ticker: str, export_path: Optional[str]) -> None:
-    """
-    Lists upcoming company earnings.
-
-    Examples:
+from i8_terminal.types.user_watchlists_param_type import UserWatchlistsParamType  # isort:skip
 
-    `i8 earnings list --ticker AAPL`
 
-    """
-    earnings_list: EarningsListResult = earnings_api.list(ticker, 10)
+def prepare_watchlist_stocks_df(name: str) -> Optional[pd.DataFrame]:
+    watchlist = investor8_sdk.UserApi().get_watchlist_by_name_user_id(name=name, user_id=USER_SETTINGS.get("user_id"))
+    watchlist_stocks_df = get_current_metrics_df(
+        ",".join(watchlist.tickers), "company_name,stock_exchange,52_week_low,52_week_high,price.r,change,market_cap"
+    )
+    return watchlist_stocks_df
+
+
+@watchlist.command()
+@click.option(
+    "--name",
+    "-n",
+    type=UserWatchlistsParamType(),
+    required=True,
+    help="Name of the watchlist.",
+)
+@click.option("--export", "export_path", "-e", help="Filename to export the output to.")
+@pass_command
+def summary(name: str, export_path: Optional[str]) -> None:
+    console = Console()
+    with console.status("Fetching data...", spinner="material"):
+        df = prepare_watchlist_stocks_df(name)
+    if df is None:
+        console.print("No data found for metrics with selected tickers", style="yellow")
+        return
     if export_path:
-        if export_path.split(".")[-1] == "html":
-            df = earnings_list.to_df()
-            table = df2Table(df)
-            export_to_html(table, export_path)
-        else:
-            export_data(
-                earnings_list.to_df("raw"),
-                export_path,
-                column_width=18,
-                column_format=APP_SETTINGS["styles"]["xlsx"]["financials"]["column"],
-            )
+        export_data(
+            prepare_current_metrics_formatted_df(df, "store"),
+            export_path,
+            column_width=18,
+            column_format=APP_SETTINGS["styles"]["xlsx"]["financials"]["column"],
+        )
     else:
-        df = earnings_list.to_df()
-        console = Console()
-        console.print(earnings_list._to_rich_table("humanize", "default"))
+        columns_justify: Dict[str, Any] = {}
+        for metric_display_name, metric_df in df.groupby("display_name"):
+            columns_justify[metric_display_name] = "left" if metric_df["display_format"].values[0] == "str" else "right"
+        table = df2Table(prepare_current_metrics_formatted_df(df, "console"), columns_justify=columns_justify)
+        console.print(table)
```

### Comparing `i8-terminal-0.2.84/i8_terminal/commands/earnings/earnings_plot.py` & `i8-terminal-0.2.9/i8_terminal/commands/earnings/earnings_plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from rich.console import Console
 
 from i8_terminal.app.layout import get_plot_default_layout
 from i8_terminal.app.plot_server import serve_plot
 from i8_terminal.commands.earnings import earnings
 from i8_terminal.common.cli import get_click_command_path, pass_command
 from i8_terminal.common.formatting import format_number
-from i8_terminal.common.stock_info import validate_tickers
 from i8_terminal.common.utils import PlotType
 from i8_terminal.types.metric_param_type import MetricParamType
 from i8_terminal.types.ticker_param_type import TickerParamType
 
 
 def get_historical_earnings_df(tickers: List[str], size: int) -> DataFrame:
     hist_earnings = []
@@ -68,26 +67,18 @@
 
     return fig
 
 
 @earnings.command()
 @click.pass_context
 @click.option("--metric", "-m", type=MetricParamType(), default="basiceps", help="Metric name.")
-@click.option(
-    "--tickers",
-    "-k",
-    type=TickerParamType(),
-    required=True,
-    callback=validate_tickers,
-    help="Comma-separated list of tickers.",
-)
+@click.option("--tickers", "-k", type=TickerParamType(), required=True, help="Comma-separated list of tickers.")
 @pass_command
 def plot(ctx: click.Context, metric: str, tickers: str) -> None:
-    """
-    Compare and plot earning metrics of given companies. TICKERS is a comma-separated list of tickers.
+    """Compare and plot earning metrics of given companies. TICKERS is a comma seperated list of tickers.
 
     Examples:
 
     `i8 earnings plot --metric net_ppe --tickers AMD,INTC,QCOM`
     """
     metric = metric.replace(" ", "").upper()
     tickers_list = tickers.replace(" ", "").upper().split(",")
```

### Comparing `i8-terminal-0.2.84/i8_terminal/commands/earnings/earnings_recent.py` & `i8-terminal-0.2.9/i8_terminal/commands/price/price_list.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,81 +1,75 @@
-from typing import Optional
+from typing import Optional, cast
 
 import click
-import investor8_sdk
-import pandas as pd
+from click.types import DateTime
+from pandas import DataFrame
 from rich.console import Console
 
-from i8_terminal.commands.earnings import earnings
+from i8_terminal.commands.price import price
 from i8_terminal.common.cli import pass_command
 from i8_terminal.common.formatting import get_formatter
 from i8_terminal.common.layout import df2Table, format_df
-from i8_terminal.common.stock_info import get_stocks_df
-from i8_terminal.common.utils import export_data, export_to_html
+from i8_terminal.common.price import get_historical_price_list_df
 from i8_terminal.config import APP_SETTINGS
+from i8_terminal.types.price_period_param_type import PricePeriodParamType
+from i8_terminal.types.ticker_param_type import TickerParamType
 
+from i8_terminal.common.utils import export_data, get_period_code, validate_ticker  # isort:skip
 
-def get_recent_earnings_df(size: int) -> pd.DataFrame:
-    earnings = investor8_sdk.EarningsApi().get_recent_earnings(size=size)
-    earnings = [d.to_dict() for d in earnings]
-    df = pd.DataFrame(earnings)
-    stocks_df = get_stocks_df()
-    return pd.merge(df, stocks_df, on="ticker")
 
-
-def format_recent_earnings_df(df: pd.DataFrame, target: str) -> pd.DataFrame:
+def format_hist_price_df(df: DataFrame, target: str) -> DataFrame:
     formatters = {
-        "latest_price": get_formatter("price", target),
-        "change": get_formatter("perc", target),
-        "fyq": get_formatter("fyq", target),
-        "eps_ws": get_formatter("number", target),
-        "eps_actual": get_formatter("number", target),
-        "revenue_ws": get_formatter("financial", target),
-        "revenue_actual": get_formatter("financial", target),
+        "Date": get_formatter("date", target),
+        "open": get_formatter("price", target),
+        "close": get_formatter("price", target),
+        "low": get_formatter("price", target),
+        "high": get_formatter("price", target),
+        "volume": get_formatter("number_int", target),
+        "change_perc": get_formatter("perc", target),
     }
     col_names = {
-        "ticker": "Ticker",
-        "name": "Name",
-        "latest_price": "Price",
-        "change": "Change",
-        "actual_report_date": "Report Date",
-        "fyq": "Period",
-        "call_time": "Call Time",
-        "eps_ws": "EPS Estimate",
-        "eps_actual": "EPS Actual",
-        "revenue_ws": "Revenue Estimate",
-        "revenue_actual": "Revenue Actual",
+        "Date": "Date",
+        "open": "Open",
+        "close": "Close",
+        "low": "Low",
+        "high": "High",
+        "volume": "Volume",
+        "change_perc": "Change (%)",
     }
     return format_df(df, col_names, formatters)
 
 
-@earnings.command()
+@price.command()
+@click.option("--ticker", "-k", type=TickerParamType(), required=True, callback=validate_ticker, help="Company ticker.")
+@click.option(
+    "--period",
+    "-p",
+    type=PricePeriodParamType(),
+    default="1M",
+    help="Historical price period.",
+)
+@click.option("--from_date", "-f", type=DateTime(), help="Histotical price from date.")
+@click.option("--to_date", "-t", type=DateTime(), help="Histotical price to date.")
 @click.option("--export", "export_path", "-e", help="Filename to export the output to.")
 @pass_command
-def recent(export_path: Optional[str]) -> None:
-    """
-    Lists recent company earnings.
-
-    Examples:
-
-    `i8 earnings recent`
-
-    """
+def list(
+    ticker: str, period: str, from_date: Optional[DateTime], to_date: Optional[DateTime], export_path: Optional[str]
+) -> None:
+    """Lists historical prices for the given TICKER."""
+    period_code = get_period_code(period.replace(" ", "").upper())
     console = Console()
     with console.status("Fetching data...", spinner="material"):
-        df = get_recent_earnings_df(size=20)
+        df = get_historical_price_list_df([ticker], period_code, cast(str, from_date), cast(str, to_date))
+
     if export_path:
-        if export_path.split(".")[-1] == "html":
-            df_formatted = format_recent_earnings_df(df, "console")
-            table = df2Table(df_formatted)
-            export_to_html(table, export_path)
-            return
+        df_formatted = format_hist_price_df(df, "store")
         export_data(
-            format_recent_earnings_df(df, "store"),
+            df_formatted,
             export_path,
-            column_width=18,
-            column_format=APP_SETTINGS["styles"]["xlsx"]["financials"]["column"],
+            column_width=14,
+            column_format=APP_SETTINGS["styles"]["xlsx"]["price"]["column"],
         )
-        return
-    df_formatted = format_recent_earnings_df(df, "console")
-    table = df2Table(df_formatted)
-    console.print(table)
+    else:
+        df_formatted = format_hist_price_df(df, "console")
+        table = df2Table(df_formatted)
+        console.print(table)
```

### Comparing `i8-terminal-0.2.84/i8_terminal/commands/financials/financials_compare.py` & `i8-terminal-0.2.9/i8_terminal/commands/financials/financials_plot.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,203 +1,218 @@
-from typing import Any, Dict, List, Optional
+from datetime import datetime
+from typing import Any, Dict, List, Optional, Tuple, cast
 
+import arrow
 import click
 import investor8_sdk
 import numpy as np
+import pandas as pd
+import plotly.express as px
 import plotly.graph_objects as go
-from pandas.core.frame import DataFrame
+from click.types import DateTime
+from plotly.subplots import make_subplots
 from rich.console import Console
 
 from i8_terminal.app.layout import get_plot_default_layout
 from i8_terminal.app.plot_server import serve_plot
 from i8_terminal.commands.financials import financials
 from i8_terminal.common.cli import get_click_command_path, pass_command
-from i8_terminal.common.financials import (
-    fin_df2export_df,
-    fin_df2Tree,
-    find_similar_statement,
-    get_statements_codes,
-    get_statements_disp_name,
-    parse_identifier,
-    prepare_financials_df,
-)
-from i8_terminal.common.metrics import get_all_financial_metrics_df
-from i8_terminal.common.utils import PlotType, export_data, export_to_html
-from i8_terminal.config import APP_SETTINGS
-from i8_terminal.types.fin_identifier_param_type import FinancialsIdentifierParamType
-from i8_terminal.types.fin_statement_param_type import FinancialStatementParamType
+from i8_terminal.common.utils import PlotType
+from i8_terminal.types.metric_param_type import MetricParamType
 from i8_terminal.types.period_type_param_type import PeriodTypeParamType
+from i8_terminal.types.ticker_param_type import TickerParamType
 
+from i8_terminal.common.metrics import find_similar_fin_metric  # isort:skip
+from i8_terminal.types.chart_param_type import ChartParamType, get_chart_param_types  # isort:skip
 
-def get_standardized_financials(
-    identifiers_list: List[Dict[str, str]],
-    statement: str,
-    period_type: str,
-    period_size: int = 4,
-    exportize: Optional[bool] = False,
-) -> Optional[Dict[str, Any]]:
-    fins = []
-    for idf in identifiers_list:
-        resp = None
-        try:
-            if idf.get("fiscal_year"):
-                resp = investor8_sdk.FinancialsApi().get_financials_single(
-                    ticker=idf["ticker"],
-                    stat_code=statement,
-                    fiscal_year=idf.get("fiscal_year"),
-                    fiscal_period=idf.get("fiscal_period"),
+
+def get_historical_financials_df(
+    tickers: List[str], metrics: List[str], period_type: str, from_date: Optional[str], to_date: Optional[str]
+) -> Tuple[pd.DataFrame, List[str]]:
+    if not to_date:
+        to_date = arrow.now().datetime.strftime("%Y-%m-%d")
+    if not from_date:
+        from_date = arrow.now().shift(years=-8 if period_type == "FY" else -4).datetime.strftime("%Y-%m-%d")
+    hist_financials = investor8_sdk.MetricsApi().get_historical_metrics(
+        symbols=",".join(tickers),
+        metrics=",".join([f"{metric}.{period_type}" for metric in metrics]),
+        from_date=from_date,
+        to_date=to_date,
+    )
+    df = pd.DataFrame.from_records(
+        [
+            (ticker, metric, period_value.period, period_value.value)
+            for ticker, metric_dict in hist_financials.data.items()
+            for metric, period_value_list in metric_dict.items()
+            for period_value in period_value_list
+        ],
+        columns=["Ticker", "metric_name", "Period", "Value"],
+    )
+    metadata_df = pd.DataFrame([h.to_dict() for h in hist_financials.metadata])
+    df = pd.merge(df, metadata_df, on="metric_name")
+    df.rename(columns={"display_name": "Metric"}, inplace=True)
+    df = pd.pivot_table(df, index="Period", columns=["Ticker", "Metric"], values=["Value"]).reset_index(level=0)
+    df = df.dropna()
+    metric_display_names = list(set(metadata_df[metadata_df.metric_name.isin(metrics)]["display_name"]))
+    df.index.name = f"Historical {' and '.join(metric_display_names)}"
+    return df, metric_display_names
+
+
+def create_fig(
+    df: pd.DataFrame, cmd_context: Dict[str, Any], matched_metrics: List[str], tickers: List[str], chart_type: str
+) -> go.Figure:
+    vertical_spacing = 0.02
+    layout = dict(
+        title=cmd_context["plot_title"],
+        autosize=True,
+        hovermode="closest",
+        legend=dict(font=dict(size=11), orientation="v"),
+        margin=dict(b=20, l=50, r=65),
+    )
+    rows_num = len(matched_metrics)
+
+    if rows_num == 2:
+        row_width = [0.5, 0.5]
+    else:
+        row_width = [1]
+
+    fig = make_subplots(
+        rows=rows_num, cols=1, shared_xaxes=True, vertical_spacing=vertical_spacing, row_width=row_width
+    )
+
+    for m in matched_metrics:
+        for tk in tickers:
+            idx = tickers.index(tk)
+            if chart_type == "bar":
+                fig.add_trace(
+                    go.Bar(
+                        x=df["Period"],
+                        y=df["Value"][tk][m],
+                        name=tk,
+                        marker=dict(color=px.colors.qualitative.Plotly[idx]),
+                        legendgroup=f"group{idx}",
+                        showlegend=True if matched_metrics.index(m) == 0 else False,
+                    ),
+                    row=matched_metrics.index(m) + 1,
+                    col=1,
                 )
             else:
-                if not period_type:
-                    period_type = "Q" if statement == "balance_sheet_statement" else "FY"
-                resp = investor8_sdk.FinancialsApi().get_latest_standardized_financials(
-                    ticker=idf["ticker"], stat_code=statement
-                )[period_type]
-            if resp:
-                fins.append(resp)
-        except Exception:
-            continue
-    if not fins:
-        return None
-    return prepare_financials_df(fins, period_size, include_ticker=True, exportize=exportize)
-
-
-def create_fig(df: DataFrame, header_dict: Dict[str, List[str]], cmd_context: Dict[str, Any]) -> go.Figure:
-    cells_fill_color = [["rgb(200, 212, 227)", "rgb(235, 240, 248)"]] * len(df.columns)
-    cells_data = list(df.to_dict("list").values())
-    # Add end_date row to cells data
-    cells_data = [[(["End Date"] + header_dict["end_date"])[idx]] + d for idx, d in enumerate(cells_data)]
-    fig = go.Figure(
-        data=[
-            go.Table(
-                columnwidth=[58, 25],
-                header=dict(
-                    values=[""] + ["<b>" + p.replace("\n", " ") + "</b>" for p in header_dict["period"]],
-                    align=["left", "center"],
-                    height=32,
-                    font_size=14,
-                ),
-                cells=dict(
-                    fill_color=cells_fill_color, values=cells_data, align=["left", "right"], height=28, font_size=14
-                ),
-            )
-        ]
+                fig.add_trace(
+                    go.Scatter(
+                        x=df["Period"],
+                        y=df["Value"][tk][m],
+                        name=tk,
+                        marker=dict(color=px.colors.qualitative.Plotly[idx]),
+                        legendgroup=f"group{idx}",
+                        showlegend=True if matched_metrics.index(m) == 0 else False,
+                    ),
+                    row=matched_metrics.index(m) + 1,
+                    col=1,
+                )
+
+    fig.update_traces(hovertemplate="%{y} %{x}")
+    fig.update_xaxes(
+        rangeslider_visible=False,
+        spikemode="across",
+        spikesnap="cursor",
     )
+
     fig.update_layout(
-        title=cmd_context["plot_title"],
-        margin=dict(b=15, l=25, r=25),
+        **layout,
         **get_plot_default_layout(),
+        legend_title_text=None,
+        xaxis_title=None,
+        yaxis_title=None,
+    )
+
+    # Add yaxis titles
+    for idx, r in enumerate(np.cumsum(row_width)[::-1]):
+        fig["layout"][f"yaxis{idx+1}"]["title"] = matched_metrics[idx]
+
+    fig.update_annotations(
+        dict(
+            font_size=10,
+            font_color="#525252",
+        )
+    )
+    fig.update_yaxes(
+        title_font_size=10,
     )
 
     return fig
 
 
 @financials.command()
 @click.pass_context
-@click.option(
-    "--identifiers",
-    "-i",
-    type=FinancialsIdentifierParamType(),
-    required=True,
-    help="Comma-separated list of identifiers.",
-)
-@click.option(
-    "--statement",
-    "-s",
-    type=FinancialStatementParamType(),
-    default="income",
-    help="Type of financial statement.",
-)
+@click.option("--tickers", "-k", type=TickerParamType(), required=True, help="Comma-separated list of tickers.")
 @click.option(
     "--period_type",
     "-m",
     type=PeriodTypeParamType(),
-    help="Period by which you want to view the report. Possible values are `FY` for yearly, \
-        `Q` for quarterly, and `TTM` for TTM reports.",
+    default="FY",
+    help="Period by which you want to view the report. Possible values are `FY` for yearly, `Q` for quarterly, and `TTM` for TTM reports.",
+)
+@click.option("--metrics", "-m", type=MetricParamType(), default="basic_eps", help="Comma-separated list of metrics.")
+@click.option("--from_date", "-f", type=DateTime(), help="Histotical financials from date.")
+@click.option("--to_date", "-t", type=DateTime(), help="Histotical financials to date.")
+@click.option(
+    "--chart_type",
+    "-c",
+    type=ChartParamType([("bar", "Bar chart"), ("line", "Line chart")]),
+    default="bar",
+    help="Chart can be bar or line chart.",
 )
-@click.option("--plot", is_flag=True, default=False, help="Plot results on the browser.")
-@click.option("--export", "export_path", "-e", help="Filename to export the output to.")
 @pass_command
-def compare(
+def plot(
     ctx: click.Context,
-    identifiers: str,
-    statement: str,
+    tickers: str,
     period_type: str,
-    plot: bool,
-    export_path: Optional[str],
+    metrics: str,
+    chart_type: str,
+    from_date: Optional[datetime],
+    to_date: Optional[datetime],
 ) -> None:
-    """
-    Compare financial metrics of given companies. IDENTIFIERS is a comma-separated list of identifiers.
+    """Compare and plot financials metrics of given companies. TICKERS is a comma seperated list of tickers.
 
     Examples:
 
-    `i8 financials compare --period_type FY --statement income --identifiers AAPL-2020-FY,MSFT-2020-FY`
-
+    `i8 financials plot --period_type Q --metrics net_ppe --from_date 2020-05-01 --to_date 2022-05-01 --tickers AMD,INTC,QCOM --chart_type line`
     """
-    matched_statement = find_similar_statement(statement)
-    if not matched_statement:
+    metrics_list = metrics.replace(" ", "").split(",")
+    matched_metrics = [find_similar_fin_metric(metric.replace("_", "")) for metric in metrics_list]
+    if not matched_metrics:
         click.echo(
-            f"`{statement}` is not a valid statement code. \nValid statement codes: {', '.join(get_statements_codes())}"
+            f"`{metrics}` is not valid metrics name. See the list of valid financial metrics with the following command:\n`i8 metrics`"
         )
         return
-    identifiers_list = identifiers.replace(" ", "").upper().split(",")
-    parsed_identifiers_list = [parse_identifier(i, period_type) for i in identifiers_list]
-    # Remove duplicates identifiers
-    parsed_identifiers_list = [dict(t) for t in {tuple(d.items()) for d in parsed_identifiers_list}]
-    tickers_list = list(set([d["ticker"] for d in parsed_identifiers_list]))
-    plot_title = f"Comparison of {', '.join(tickers_list)} {get_statements_disp_name(matched_statement)}s"
-    plot_title = " and ".join(plot_title.rsplit(", ", 1))
+    if len(matched_metrics) > 2:
+        click.echo("You can enter up to 2 metrics.")
+        return
+    if not chart_type in [t[0] for t in get_chart_param_types()]:
+        click.echo(f"`{chart_type}` is not valid chart type.")
+        return
+    command_path_parsed_options_dict = {"--metrics": ",".join(matched_metrics)}  # type: ignore
+    if from_date:
+        command_path_parsed_options_dict["--from_date"] = from_date.strftime("%Y-%m-%d")
+    if to_date:
+        command_path_parsed_options_dict["--to_date"] = to_date.strftime("%Y-%m-%d")
+    command_path = get_click_command_path(ctx, command_path_parsed_options_dict)
+    tickers_list = tickers.replace(" ", "").upper().split(",")
+    if len(tickers_list) > 5:
+        click.echo("You can enter up to 5 tickers.")
+        return
+    cmd_context = {
+        "command_path": command_path,
+        "tickers": tickers_list,
+        "plot_type": PlotType.CHART.value,
+    }
+
     console = Console()
     with console.status("Fetching data...", spinner="material") as status:
-        fins = get_standardized_financials(
-            parsed_identifiers_list,
-            matched_statement,
-            period_type,
-            period_size=4,
-            exportize=True if export_path else False,
-        )
-        if fins is None:
-            status.stop()
-            click.echo("No data found!")
-            return
-        periods_list = fins["data"].columns[1:].to_list()
-        df_metrics = get_all_financial_metrics_df()
-        df = fins["data"].merge(df_metrics, on="tag", how="left")
-        df["section_name"] = df["section_name"].apply(lambda x: "Others" if not x or x == "-" else x)
-        df = df.astype(object).replace(np.nan, None)  # Replace nan with None
-        if plot:
-            cmd_context = {
-                "plot_title": plot_title,
-                "command_path": get_click_command_path(ctx, {"--statement": matched_statement}),
-                "tickers": tickers_list,
-                "plot_type": PlotType.TABLE.value,
-            }
-            df = df[df["is_significant"] is not False]
-            df = df[["name", *fins["data"].columns[1:]]]
-            df.rename(columns={"name": ""}, inplace=True)
-            fig = create_fig(df, fins["header"], cmd_context)
-
-    missing_tickers = set(tickers_list) - set(fins["header"].get("ticker", set()))
-    if missing_tickers:
-        missing_tickers_str = " and ".join(", ".join(missing_tickers).rsplit(", ", 1))
-        console.print(f'The specified financials for ticker(s) "{missing_tickers_str}" are not available.')
-        console.print("To see the covered financials check the [magenta]financials coverage[magenta] command.")
-
-    if plot and export_path:
-        console.print("The plot and export options are not compatible to use together")
-    elif plot:
-        serve_plot(fig, cmd_context)
-    elif export_path:
-        if export_path.split(".")[-1] == "html":
-            tree = fin_df2Tree(df, fins["header"], periods_list, title=plot_title)
-            export_to_html(tree, export_path)
-            return
-        export_df = fin_df2export_df(df, periods_list)
-        export_data(
-            export_df,
-            export_path,
-            column_width=22,
-            column_format=APP_SETTINGS["styles"]["xlsx"]["financials"]["column"],
+        df, metric_display_names = get_historical_financials_df(
+            tickers_list, matched_metrics, period_type, cast(str, from_date), cast(str, to_date)  # type: ignore
         )
-    else:
-        tree = fin_df2Tree(df, fins["header"], periods_list, title=plot_title)
-        console.print(tree)
+        cmd_context["plot_title"] = df.index.name
+        status.update("Generating plot...")
+        fig = create_fig(df, cmd_context, metric_display_names, tickers_list, chart_type)  # type: ignore
+
+    serve_plot(fig, cmd_context)
```

### Comparing `i8-terminal-0.2.84/i8_terminal/commands/financials/financials_coverage.py` & `i8-terminal-0.2.9/i8_terminal/commands/financials/financials_coverage.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,33 +2,25 @@
 import investor8_sdk
 from pandas import DataFrame
 from rich.console import Console
 
 from i8_terminal.commands.financials import financials
 from i8_terminal.common.cli import pass_command
 from i8_terminal.common.financials import available_fin_df2tree
-from i8_terminal.common.stock_info import validate_ticker
+from i8_terminal.common.utils import validate_ticker
 from i8_terminal.types.ticker_param_type import TickerParamType
 
 
 def get_available_financials_df(ticker: str) -> DataFrame:
     available_fins = investor8_sdk.FinancialsApi().get_list_available_standardized_financials(ticker=ticker)
     return DataFrame([d.to_dict() for d in available_fins])
 
 
 @financials.command()
 @click.option("--ticker", "-k", type=TickerParamType(), required=True, callback=validate_ticker, help="Company ticker.")
 @pass_command
 def coverage(ticker: str) -> None:
-    """
-    Shows available financial statements of the given company.
-
-    Examples:
-
-    `i8 financials coverage --ticker AAPL`
-
-    """
     console = Console()
     with console.status("Fetching data...", spinner="material"):
         available_fin_df = get_available_financials_df(ticker)
         available_fins_tree = available_fin_df2tree(available_fin_df, ticker)
     console.print(available_fins_tree)
```

### Comparing `i8-terminal-0.2.84/i8_terminal/commands/financials/financials_list.py` & `i8-terminal-0.2.9/i8_terminal/commands/financials/financials_list.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,56 +3,62 @@
 import click
 import investor8_sdk
 import numpy as np
 from rich.console import Console
 
 from i8_terminal.commands.financials import financials
 from i8_terminal.common.cli import pass_command
-from i8_terminal.common.financials import (
-    fin_df2export_df,
-    fin_df2Tree,
+from i8_terminal.common.metrics import get_all_metrics_df
+from i8_terminal.common.utils import export_data
+from i8_terminal.config import APP_SETTINGS
+from i8_terminal.types.period_type_param_type import PeriodTypeParamType
+
+from i8_terminal.types.fin_statement_param_type import FinancialStatementParamType  # isort:skip
+
+from i8_terminal.types.fin_identifier_param_type import FinancialsIdentifierParamType  # isort:skip
+
+from i8_terminal.common.financials import (  # isort:skip
     find_similar_statement,
     get_statements_codes,
     get_statements_disp_name,
+    fin_df2export_df,
+    fin_df2Tree,
     parse_identifier,
     prepare_financials_df,
 )
-from i8_terminal.common.metrics import get_all_financial_metrics_df
-from i8_terminal.common.utils import export_data, export_to_html
-from i8_terminal.config import APP_SETTINGS
-from i8_terminal.types.fin_identifier_param_type import FinancialsIdentifierParamType
-from i8_terminal.types.fin_statement_param_type import FinancialStatementParamType
-from i8_terminal.types.period_type_param_type import PeriodTypeParamType
 
 
 def get_standardized_financials(
     identifiers_dict: Dict[str, str],
     statement: str,
     period_type: Optional[str],
     period_size: int = 4,
     exportize: Optional[bool] = False,
 ) -> Optional[Dict[str, Any]]:
     fins = []
-    if identifiers_dict.get("fiscal_period"):
-        fins = [
-            investor8_sdk.FinancialsApi().get_financials_single(
+    try:
+        if identifiers_dict.get("fiscal_period"):
+            fins = [
+                investor8_sdk.FinancialsApi().get_financials_single(
+                    ticker=identifiers_dict["ticker"],
+                    stat_code=statement,
+                    fiscal_year=identifiers_dict.get("fiscal_year"),
+                    fiscal_period=identifiers_dict.get("fiscal_period"),
+                )
+            ]
+        else:
+            period_type = "FY" if not period_type else period_type
+            fins = investor8_sdk.FinancialsApi().get_list_standardized_financials(
                 ticker=identifiers_dict["ticker"],
                 stat_code=statement,
-                fiscal_year=identifiers_dict.get("fiscal_year"),
-                fiscal_period=identifiers_dict.get("fiscal_period"),
+                period_type=period_type,
+                end_year=identifiers_dict.get("fiscal_year", ""),
             )
-        ]
-    else:
-        period_type = "FY" if not period_type else period_type
-        fins = investor8_sdk.FinancialsApi().get_list_standardized_financials(
-            ticker=identifiers_dict["ticker"],
-            stat_code=statement,
-            period_type=period_type,
-            end_year=identifiers_dict.get("fiscal_year", ""),
-        )
+    except Exception:
+        pass
     if not fins:
         return None
     return prepare_financials_df(fins, period_size, include_ticker=False, exportize=exportize)
 
 
 @financials.command()
 @click.option(
@@ -69,28 +75,19 @@
     default="income",
     help="Type of financial statement.",
 )
 @click.option(
     "--period_type",
     "-m",
     type=PeriodTypeParamType(),
-    help="Period by which you want to view the report. Possible values are `FY` for yearly, \
-        `Q` for quarterly, and `TTM` for TTM reports.",
+    help="Period by which you want to view the report. Possible values are `FY` for yearly, `Q` for quarterly, and `TTM` for TTM reports.",
 )
 @click.option("--export", "export_path", "-e", help="Filename to export the output to.")
 @pass_command
 def list(identifier: str, statement: str, period_type: Optional[str], export_path: Optional[str]) -> None:
-    """
-    Lists financial metrics of a given company.
-
-    Examples:
-
-    `i8 financials list --period_type FY --statement income --identifier AAPL-2020-FY`
-
-    """
     matched_statement = find_similar_statement(statement)
     if not matched_statement:
         click.echo(
             f"`{statement}` is not a valid statement code. \nValid statement codes: {', '.join(get_statements_codes())}"
         )
         click.echo("Unknown Statement Code!")
         return
@@ -101,29 +98,20 @@
             identifiers_dict, matched_statement, period_type, period_size=4, exportize=True if export_path else False
         )
         if fins is None:
             status.stop()
             click.echo("No data found!")
             return
         periods_list = fins["data"].columns[1:].to_list()
-        df_metrics = get_all_financial_metrics_df()
-        df = fins["data"].merge(df_metrics, on="tag", how="left")
+        df_metrics = get_all_metrics_df()
+        df = fins["data"].merge(df_metrics, on="tag_fullname", how="left")
         df["section_name"] = df["section_name"].apply(lambda x: "Others" if not x or x == "-" else x)
         df = df.astype(object).replace(np.nan, None)  # Replace nan with None
 
     if export_path:
-        if export_path.split(".")[-1] == "html":
-            tree = fin_df2Tree(
-                df,
-                fins["header"],
-                periods_list,
-                title=f"{identifiers_dict['ticker'].upper()} {get_statements_disp_name(matched_statement)}",
-            )
-            export_to_html(tree, export_path)
-            return
         export_df = fin_df2export_df(df, periods_list)
         export_data(
             export_df,
             export_path,
             column_width=18,
             column_format=APP_SETTINGS["styles"]["xlsx"]["financials"]["column"],
         )
```

### Comparing `i8-terminal-0.2.84/i8_terminal/commands/financials/financials_plot.py` & `i8-terminal-0.2.9/i8_terminal/commands/metrics/metrics_plot.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,120 +1,143 @@
 from datetime import datetime
-from typing import Any, Dict, List, Optional, Tuple, cast
+from typing import Any, Dict, List, Optional, cast
 
-import arrow
 import click
 import investor8_sdk
 import numpy as np
 import pandas as pd
 import plotly.express as px
 import plotly.graph_objects as go
 from click.types import DateTime
+from pandas import DataFrame
 from plotly.subplots import make_subplots
 from rich.console import Console
 
 from i8_terminal.app.layout import get_plot_default_layout
 from i8_terminal.app.plot_server import serve_plot
-from i8_terminal.commands.financials import financials
+from i8_terminal.commands.metrics import metrics
 from i8_terminal.common.cli import get_click_command_path, pass_command
-from i8_terminal.common.metrics import find_similar_fin_metric
-from i8_terminal.common.stock_info import validate_tickers
-from i8_terminal.common.utils import PlotType, reverse_period
-from i8_terminal.types.chart_param_type import ChartParamType, get_chart_param_types
+from i8_terminal.common.metrics import get_period_start_date
+from i8_terminal.common.utils import PlotType
+from i8_terminal.types.chart_param_type import ChartParamType
 from i8_terminal.types.metric_param_type import MetricParamType
 from i8_terminal.types.period_type_param_type import PeriodTypeParamType
+from i8_terminal.types.price_period_param_type import PricePeriodParamType
 from i8_terminal.types.ticker_param_type import TickerParamType
 
 
-def get_historical_financials_df(
-    tickers: List[str], metrics: List[str], period_type: str, from_date: Optional[str], to_date: Optional[str]
-) -> Tuple[pd.DataFrame, List[str]]:
-    if not to_date:
-        to_date = arrow.now().datetime.strftime("%Y-%m-%d")
-    if not from_date:
-        from_date = arrow.now().shift(years=-8 if period_type == "FY" else -4).datetime.strftime("%Y-%m-%d")
-    hist_financials = investor8_sdk.MetricsApi().get_historical_metrics(
-        symbols=",".join(tickers),
-        metrics=",".join([f"{metric}.{period_type}" for metric in metrics]),
-        from_date=from_date,
-        to_date=to_date,
+def get_historical_metrics_df(
+    tickers: List[str],
+    metrics: List[str],
+    period: str,
+    period_type: str,
+    from_date: Optional[str],
+    to_date: Optional[str],
+) -> DataFrame:
+    metrics_period_type = (
+        [f"{metric}.{period_type}" for metric in metrics] if period_type else [metric for metric in metrics]
     )
+    if from_date:
+        if not to_date:
+            to_date = datetime.now().strftime("%Y-%m-%d")
+        historical_metrics = investor8_sdk.MetricsApi().get_historical_metrics(
+            symbols=",".join(tickers),
+            metrics=",".join(metrics_period_type),
+            from_date=from_date,
+            to_date=to_date,
+        )
+    else:
+        from_date = get_period_start_date(period)
+        to_date = datetime.now().strftime("%Y-%m-%d")
+        historical_metrics = investor8_sdk.MetricsApi().get_historical_metrics(
+            symbols=",".join(tickers),
+            metrics=",".join(metrics_period_type),
+            from_date=from_date,
+            to_date=to_date,
+        )
     df = pd.DataFrame.from_records(
         [
-            (ticker, metric, period_value.period, period_value.value)
-            for ticker, metric_dict in hist_financials.data.items()
+            (ticker, metric, period_value.period, period_value.period_date_time, period_value.value)
+            for ticker, metric_dict in historical_metrics.data.items()
             for metric, period_value_list in metric_dict.items()
             for period_value in period_value_list
         ],
-        columns=["Ticker", "metric_name", "Period", "Value"],
+        columns=["Ticker", "metric_name", "Period", "PeriodDateTime", "Value"],
     )
-    metadata_df = pd.DataFrame([h.to_dict() for h in hist_financials.metadata])
+    metadata_df = pd.DataFrame([h.to_dict() for h in historical_metrics.metadata])
     df = pd.merge(df, metadata_df, on="metric_name")
     df.rename(columns={"display_name": "Metric"}, inplace=True)
-    df = pd.pivot_table(df, index="Period", columns=["Ticker", "Metric"], values=["Value"]).reset_index(level=0)
-    df["ReversedPeriod"] = df["Period"].apply(lambda x: reverse_period(x))
-    df = df.sort_values("ReversedPeriod").dropna()
-    metric_display_names = list(set(metadata_df[metadata_df.metric_name.isin(metrics)]["display_name"]))
-    df.index.name = f"Historical {' and '.join(metric_display_names)}"
-    return df, metric_display_names
+    df["Value"] = df["Value"].astype(df["data_format"].values[0])
+    return df
 
 
 def create_fig(
-    df: pd.DataFrame, cmd_context: Dict[str, Any], matched_metrics: List[str], tickers: List[str], chart_type: str
+    df: DataFrame,
+    cmd_context: Dict[str, Any],
+    tickers: List[str],
+    chart_type: str,
 ) -> go.Figure:
     vertical_spacing = 0.02
     layout = dict(
         title=cmd_context["plot_title"],
         autosize=True,
         hovermode="closest",
         legend=dict(font=dict(size=11), orientation="v"),
         margin=dict(b=20, l=50, r=65),
     )
-    rows_num = len(matched_metrics)
+    metrics = list(set(df["Metric"]))
+    rows_num = len(metrics)
 
     if rows_num == 2:
         row_width = [0.5, 0.5]
     else:
         row_width = [1]
 
     fig = make_subplots(
-        rows=rows_num, cols=1, shared_xaxes=True, vertical_spacing=vertical_spacing, row_width=row_width
+        rows=rows_num,
+        cols=1,
+        shared_xaxes=False if len(list(set(df["default_period_type"]))) > 1 else True,
+        vertical_spacing=vertical_spacing,
+        row_width=row_width,
     )
 
-    for m in matched_metrics:
-        for tk in tickers:
-            idx = tickers.index(tk)
+    for metric, metric_df in df.groupby("Metric"):
+        metric_idx = metrics.index(metric)
+        for ticker, ticker_df in metric_df.sort_values(["PeriodDateTime"]).groupby("Ticker"):
+            idx = tickers.index(ticker)
             if chart_type == "bar":
                 fig.add_trace(
                     go.Bar(
-                        x=df["Period"],
-                        y=df["Value"][tk][m],
-                        name=tk,
+                        x=ticker_df["Period"],
+                        y=ticker_df["Value"],
+                        name=ticker,
                         marker=dict(color=px.colors.qualitative.Plotly[idx]),
                         legendgroup=f"group{idx}",
-                        showlegend=True if matched_metrics.index(m) == 0 else False,
+                        showlegend=True if metrics.index(metric) == 0 else False,
                     ),
-                    row=matched_metrics.index(m) + 1,
+                    row=metrics.index(metric) + 1,
                     col=1,
                 )
             else:
                 fig.add_trace(
                     go.Scatter(
-                        x=df["Period"],
-                        y=df["Value"][tk][m],
-                        name=tk,
+                        x=ticker_df["Period"],
+                        y=ticker_df["Value"],
+                        name=ticker,
                         marker=dict(color=px.colors.qualitative.Plotly[idx]),
                         legendgroup=f"group{idx}",
-                        showlegend=True if matched_metrics.index(m) == 0 else False,
+                        showlegend=True if metrics.index(metric) == 0 else False,
                     ),
-                    row=matched_metrics.index(m) + 1,
+                    row=metrics.index(metric) + 1,
                     col=1,
                 )
+        if len(metrics) > 1:
+            fig["layout"][f"xaxis{metric_idx+1}"]["dtick"] = round(len(metric_df["Period"]) / 10)
 
-    fig.update_traces(hovertemplate="%{y} %{x}")
+    fig.update_traces(hovertemplate="%{y:.2f} %{x}")
     fig.update_xaxes(
         rangeslider_visible=False,
         spikemode="across",
         spikesnap="cursor",
     )
 
     fig.update_layout(
@@ -123,108 +146,105 @@
         legend_title_text=None,
         xaxis_title=None,
         yaxis_title=None,
     )
 
     # Add yaxis titles
     for idx, r in enumerate(np.cumsum(row_width)[::-1]):
-        fig["layout"][f"yaxis{idx+1}"]["title"] = matched_metrics[idx]
+        fig["layout"][f"yaxis{idx+1}"]["title"] = metrics[idx]
 
     fig.update_annotations(
         dict(
             font_size=10,
             font_color="#525252",
         )
     )
     fig.update_yaxes(
         title_font_size=10,
     )
 
     return fig
 
 
-@financials.command()
+@metrics.command()
 @click.pass_context
+@click.option("--tickers", "-k", type=TickerParamType(), required=True, help="Comma-separated list of tickers.")
+@click.option(
+    "--metrics",
+    "-m",
+    type=MetricParamType(),
+    default="pe_ratio_ttm",
+    help="Comma-separated list of daily metrics.",
+)
 @click.option(
-    "--tickers",
-    "-k",
-    type=TickerParamType(),
-    required=True,
-    callback=validate_tickers,
-    help="Comma-separated list of tickers.",
+    "--period",
+    "-p",
+    type=PricePeriodParamType(),
+    default="1Y",
+    help="Historical price period.",
 )
 @click.option(
     "--period_type",
     "-m",
     type=PeriodTypeParamType(),
-    default="FY",
-    help="Period by which you want to view the report. Possible values are `FY` for yearly, \
-        `Q` for quarterly, and `TTM` for TTM reports.",
+    help="Period by which you want to view the report. Possible values are `FY` for yearly, `Q` for quarterly, and `TTM` for TTM reports.",
 )
-@click.option("--metrics", "-m", type=MetricParamType(), default="basic_eps", help="Comma-separated list of metrics.")
 @click.option("--from_date", "-f", type=DateTime(), help="Histotical financials from date.")
 @click.option("--to_date", "-t", type=DateTime(), help="Histotical financials to date.")
 @click.option(
     "--chart_type",
     "-c",
     type=ChartParamType([("bar", "Bar chart"), ("line", "Line chart")]),
-    default="bar",
+    default="line",
     help="Chart can be bar or line chart.",
 )
 @pass_command
 def plot(
     ctx: click.Context,
     tickers: str,
-    period_type: str,
     metrics: str,
     chart_type: str,
+    period: str,
+    period_type: str,
     from_date: Optional[datetime],
     to_date: Optional[datetime],
 ) -> None:
-    """
-    Compare and plot financial metrics of given companies. TICKERS is a comma-separated list of tickers.
+    """Compare and plot daily metrics of given companies. TICKERS is a comma seperated list of tickers.
 
     Examples:
 
-    `i8 financials plot --period_type Q --metrics net_ppe --from_date 2020-05-01 --to_date 2022-05-01 \
-        --tickers AMD,INTC,QCOM --chart_type line`
+    `i8 metrics plot --metrics pe_ratio_fy --period 5Y --tickers AMD,INTC,QCOM`
     """
+    period = period.replace(" ", "").upper()
     metrics_list = metrics.replace(" ", "").split(",")
-    matched_metrics = [find_similar_fin_metric(metric.replace("_", "")) for metric in metrics_list]
-    if not matched_metrics:
-        click.echo(
-            f"`{metrics}` is not valid metrics name. See the list of valid financial metrics with the \
-                following command:\n`i8 metrics`"
-        )
-        return
-    if len(matched_metrics) > 2:
-        click.echo("You can enter up to 2 metrics.")
+    if len(metrics_list) > 2:
+        click.echo("You can enter up to 2 daily metrics.")
         return
-    if chart_type not in [t[0] for t in get_chart_param_types()]:
-        click.echo(f"`{chart_type}` is not valid chart type.")
-        return
-    command_path_parsed_options_dict = {"--metrics": ",".join(matched_metrics)}  # type: ignore
+    command_path_parsed_options_dict = {}
     if from_date:
         command_path_parsed_options_dict["--from_date"] = from_date.strftime("%Y-%m-%d")
     if to_date:
         command_path_parsed_options_dict["--to_date"] = to_date.strftime("%Y-%m-%d")
     command_path = get_click_command_path(ctx, command_path_parsed_options_dict)
     tickers_list = tickers.replace(" ", "").upper().split(",")
     if len(tickers_list) > 5:
         click.echo("You can enter up to 5 tickers.")
         return
+    if not chart_type in ["bar", "line"]:
+        click.echo(f"`{chart_type}` is not valid chart type.")
+        return
     cmd_context = {
         "command_path": command_path,
         "tickers": tickers_list,
         "plot_type": PlotType.CHART.value,
     }
 
     console = Console()
     with console.status("Fetching data...", spinner="material") as status:
-        df, metric_display_names = get_historical_financials_df(
-            tickers_list, matched_metrics, period_type, cast(str, from_date), cast(str, to_date)  # type: ignore
+        df = get_historical_metrics_df(
+            tickers_list, metrics_list, period, period_type, cast(str, from_date), cast(str, to_date)
         )
-        cmd_context["plot_title"] = df.index.name
+        cmd_context["plot_title"] = f"Historical {' and '.join(list(set(df['Metric'])))}"
         status.update("Generating plot...")
-        fig = create_fig(df, cmd_context, metric_display_names, tickers_list, chart_type)  # type: ignore
+        fig = create_fig(df, cmd_context, tickers_list, chart_type)
 
     serve_plot(fig, cmd_context)
```

### Comparing `i8-terminal-0.2.84/i8_terminal/commands/market/market_summary.py` & `i8-terminal-0.2.9/i8_terminal/commands/market/market_summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,22 +160,14 @@
     }[name]
 
 
 @market.command()
 @click.option("--live", is_flag=True, default=False, help="Print live results of market summary on terminal.")
 @pass_command
 def summary(live: bool) -> None:
-    """
-    Shows a summary of the market information.
-
-    Examples:
-
-    `i8 market summary`
-
-    """
     console = Console()
     price_size = 10
     with console.status("Fetching data...", spinner="material") as status:
         sectors_df = get_sector_returns_df()
         major_indices_df = get_major_indices_df()
         today_winners_df = get_today_top_stocks_df("winners")
         today_losers_df = get_today_top_stocks_df("losers")
```

### Comparing `i8-terminal-0.2.84/i8_terminal/commands/metrics/metrics_current.py` & `i8-terminal-0.2.9/i8_terminal/commands/watchlist/watchlist_metrics.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,89 +1,64 @@
 from typing import Any, Dict, Optional
 
 import click
+import investor8_sdk
+import pandas as pd
 from rich.console import Console
 
-from i8_terminal.commands.metrics import metrics
+from i8_terminal.commands.watchlist import watchlist
 from i8_terminal.common.cli import pass_command
 from i8_terminal.common.layout import df2Table
-from i8_terminal.common.metrics import (
-    get_current_metrics_df,
-    prepare_current_metrics_formatted_df,
-)
-from i8_terminal.common.stock_info import validate_tickers
-from i8_terminal.common.utils import export_data, export_to_html
-from i8_terminal.config import APP_SETTINGS
-from i8_terminal.types.metric_identifier_param_type import MetricIdentifierParamType
-from i8_terminal.types.ticker_param_type import TickerParamType
+from i8_terminal.common.utils import export_data
+from i8_terminal.config import APP_SETTINGS, USER_SETTINGS
+from i8_terminal.types.metric_param_type import MetricParamType
+
+from i8_terminal.common.metrics import get_current_metrics_df, prepare_current_metrics_formatted_df  # isort:skip
+
+from i8_terminal.types.user_watchlists_param_type import UserWatchlistsParamType  # isort:skip
 
 
-@metrics.command()
+def prepare_watchlist_stocks_df(name: str, metrics: str) -> Optional[pd.DataFrame]:
+    watchlist = investor8_sdk.UserApi().get_watchlist_by_name_user_id(name=name, user_id=USER_SETTINGS.get("user_id"))
+    watchlist_stocks_df = get_current_metrics_df(",".join(watchlist.tickers), metrics)
+    return watchlist_stocks_df
+
+
+@watchlist.command()
 @click.option(
-    "--tickers",
-    "-k",
-    type=TickerParamType(),
+    "--name",
+    "-n",
+    type=UserWatchlistsParamType(),
     required=True,
-    callback=validate_tickers,
-    help="Comma-separated list of tickers.",
+    help="Name of the watchlist.",
 )
 @click.option(
     "--metrics",
     "-m",
-    type=MetricIdentifierParamType(),
+    type=MetricParamType(),
     default="pe_ratio_ttm",
     help="Comma-separated list of daily metrics.",
 )
 @click.option("--export", "export_path", "-e", help="Filename to export the output to.")
 @pass_command
-def current(tickers: str, metrics: str, export_path: Optional[str]) -> None:
-    """
-    Lists the given metrics for a given list of companies. TICKERS is a comma-separated list of tickers.
-    METRICS can be in the below format:
-    {metric}.{optional period}
-
-    Available periods:
-        q = most recent quarter,
-        fy = most recent fiscal year,
-        ttm = trailing 12 months,
-        ytd = year to date,
-        p = default period type
-
-    Examples:
-
-    `i8 metrics current --metrics total_revenue.q,net_income.fy,close.d,total_revenue \
-        --tickers AMD,INTC,QCOM`
-    """
+def metrics(name: str, metrics: str, export_path: Optional[str]) -> None:
     console = Console()
     with console.status("Fetching data...", spinner="material"):
-        df = get_current_metrics_df(tickers, metrics.replace(".p", ""))
+        df = prepare_watchlist_stocks_df(name, metrics)
     if df is None:
         console.print("No data found for metrics with selected tickers", style="yellow")
         return
-    for m in [*set(metric.split(".")[0] for metric in set(metrics.split(","))) - set(df["metric_name"])]:
+    for m in list(set(metrics.split(",")) - set(df["metric_name"])):
         console.print(f"\nNo data found for metric {m} with selected tickers", style="yellow")
-    columns_justify: Dict[str, Any] = {}
     if export_path:
-        if export_path.split(".")[-1] == "html":
-            for metric_display_name, metric_df in df.groupby("display_name"):
-                columns_justify[metric_display_name] = (
-                    "left" if metric_df["display_format"].values[0] == "str" else "right"
-                )
-            table = df2Table(
-                prepare_current_metrics_formatted_df(df, "console", include_period=True),
-                columns_justify=columns_justify,
-            )
-            export_to_html(table, export_path)
-            return
         export_data(
-            prepare_current_metrics_formatted_df(df, "store", include_period=True),
+            prepare_current_metrics_formatted_df(df, "store"),
             export_path,
             column_width=18,
             column_format=APP_SETTINGS["styles"]["xlsx"]["financials"]["column"],
         )
     else:
+        columns_justify: Dict[str, Any] = {}
         for metric_display_name, metric_df in df.groupby("display_name"):
             columns_justify[metric_display_name] = "left" if metric_df["display_format"].values[0] == "str" else "right"
-        table = df2Table(
-            prepare_current_metrics_formatted_df(df, "console", include_period=True), columns_justify=columns_justify
-        )
+        table = df2Table(prepare_current_metrics_formatted_df(df, "console"), columns_justify=columns_justify)
         console.print(table)
```

### Comparing `i8-terminal-0.2.84/i8_terminal/commands/metrics/metrics_search.py` & `i8-terminal-0.2.9/i8_terminal/types/fin_identifier_param_type.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,59 +1,30 @@
-from typing import Any, Dict, Optional
+from datetime import datetime
+from typing import List, Tuple
 
-import click
-from pandas import DataFrame
-from rich.console import Console
-
-from i8_terminal.commands.metrics import metrics
-from i8_terminal.common.cli import pass_command
-from i8_terminal.common.layout import df2Table, format_df
-from i8_terminal.common.metrics import get_all_metrics_df
-
-
-def search_metrics_df(keyword: str) -> Optional[DataFrame]:
-    keyword = keyword.lower()
-    metrics_df = get_all_metrics_df()
-    metrics_df["lower_display_name"] = metrics_df["display_name"].str.lower()
-    result = metrics_df[
-        metrics_df["metric_name"].str.contains(keyword) | metrics_df["lower_display_name"].str.contains(keyword)
-    ]
-    if result.empty:
-        return None
-    return result
-
-
-def format_metrics_df(df: DataFrame) -> DataFrame:
-    formatters: Dict[str, Any] = {}
-    col_names = {
-        "metric_name": "Metric Name",
-        "display_name": "Display Name",
-        "unit": "Unit",
-        "type": "Type",
-        "display_format": "Display Format",
-        "data_format": "Data Format",
-        "period_type_default": "Default Period Type",
-    }
-    return format_df(df, col_names, formatters)
-
-
-@metrics.command()
-@click.option("--keyword", "-k", required=True, help="Keyword can be metric name.")
-@pass_command
-def search(keyword: str) -> None:
-    """
-    Searches and shows all metrics that match with the given KEYWORD.
-
-    Examples:
-
-    `i8 metrics search --keyword return`
-
-    """
-    console = Console()
-    with console.status("Fetching data...", spinner="material"):
-        df = search_metrics_df(keyword)
-    if df is None:
-        console.print(f"No metrics found for keyword '{keyword}'", style="yellow")
-        return
-    df_formatted = format_metrics_df(df)
-    table = df2Table(df_formatted)
-    console.print(table)
+from i8_terminal.types.auto_complete_choice import AutoCompleteChoice
+from i8_terminal.types.fin_period_param_type import FinancialsPeriodParamType
+from i8_terminal.types.ticker_param_type import TickerParamType
+
+
+class FinancialsIdentifierParamType(AutoCompleteChoice):
+    name = "financials"
+
+    def __init__(self) -> None:
+        self._ticker_auto_comp = TickerParamType()
+        self._period_auto_comp = FinancialsPeriodParamType()
+
+    def get_suggestions(
+        self, keyword: str, pre_populate: bool = False, param_type: str = None
+    ) -> List[Tuple[str, str]]:
+        if param_type == "ticker":
+            return self._ticker_auto_comp.get_suggestions(keyword)
+        elif param_type == "year":
+            years = [(str(i), "") for i in range(datetime.now().year, 2008, -1)]
+            if keyword.strip() == "":
+                return years
+            return [y for y in years if y[0].startswith(keyword)]
+        else:
+            return self._period_auto_comp.get_suggestions(keyword, True)
+
+    def __repr__(self) -> str:
+        return "FINANCIALS"
```

### Comparing `i8-terminal-0.2.84/i8_terminal/commands/news/news_list.py` & `i8-terminal-0.2.9/i8_terminal/commands/news/news_list.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pandas import DataFrame
 from rich.console import Console
 
 from i8_terminal.commands.news import news
 from i8_terminal.common.cli import pass_command
 from i8_terminal.common.formatting import format_number, get_formatter
 from i8_terminal.common.layout import df2Table, format_df
-from i8_terminal.common.stock_info import validate_ticker
+from i8_terminal.common.utils import validate_ticker
 from i8_terminal.types.ticker_param_type import TickerParamType
 
 
 def get_news_df(identifier: str, page_size: int) -> DataFrame:
     if identifier:
         news = investor8_sdk.NewsApi().get_ticker_news(identifier)
     else:
@@ -59,21 +59,14 @@
 
 @news.command()
 @click.option(
     "--ticker", "-k", type=TickerParamType(), required=True, callback=validate_ticker, help="Ticker or company name."
 )
 @pass_command
 def list(ticker: str) -> None:
-    """
-    Lists the latest market news for a given ticker.
-
-    Examples:
-
-    `i8 news list --ticker AAPL`
-
-    """
+    """Lists the latest market news. If ticker is provided, the news are filtered based on the give ticker."""
     console = Console()
     with console.status("Fetching data...", spinner="material"):
         df = get_news_df(ticker, page_size=10)
     df_formatted = format_news_df(df, "console")
     table = df2Table(df_formatted)
     console.print(table)
```

### Comparing `i8-terminal-0.2.84/i8_terminal/commands/price/price_compare.py` & `i8-terminal-0.2.9/i8_terminal/commands/price/price_compare.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,34 +3,26 @@
 import click
 import plotly.express as px
 from click.types import DateTime
 from pandas.core.frame import DataFrame
 from plotly.graph_objects import Figure
 from rich.console import Console
 
-from i8_terminal.app.layout import get_date_range, get_plot_default_layout
 from i8_terminal.app.plot_server import serve_plot
 from i8_terminal.commands.price import price
 from i8_terminal.common.cli import get_click_command_path, pass_command
-from i8_terminal.common.layout import df2Table
-from i8_terminal.common.price import (
-    get_historical_price_df,
-    get_historical_price_export_df,
-)
-from i8_terminal.common.stock_info import validate_tickers
-from i8_terminal.common.utils import (
-    PlotType,
-    export_data,
-    export_to_html,
-    get_period_code,
-)
+from i8_terminal.common.utils import PlotType, export_data, get_period_code
 from i8_terminal.config import APP_SETTINGS
 from i8_terminal.types.price_period_param_type import PricePeriodParamType
 from i8_terminal.types.ticker_param_type import TickerParamType
 
+from i8_terminal.common.price import get_historical_price_df, get_historical_price_export_df  # isort:skip
+
+from i8_terminal.app.layout import get_date_range, get_plot_default_layout  # isort:skip
+
 
 def get_price_data(
     tickers: List[str], period_code: int, from_date: Optional[str], to_date: Optional[str]
 ) -> Optional[DataFrame]:
     hist_price_df = get_historical_price_df(tickers, period_code, from_date, to_date, pivot_value="change_perc")
     # FIXME: use realtime price in future
     # realtime_price_df = get_historical_price_df(tickers, 1)
@@ -92,34 +84,26 @@
     "-p",
     type=PricePeriodParamType(),
     default="1M",
     help="Historical price period.",
 )
 @click.option("--from_date", "-f", type=DateTime(), help="Histotical price from date.")
 @click.option("--to_date", "-t", type=DateTime(), help="Histotical price to date.")
-@click.option(
-    "--tickers",
-    "-k",
-    type=TickerParamType(),
-    required=True,
-    callback=validate_tickers,
-    help="Comma-separated list of tickers.",
-)
+@click.option("--tickers", "-k", type=TickerParamType(), required=True, help="Comma-separated list of tickers.")
 @click.option("--export", "export_path", "-e", help="Filename to export the output to.")
 @pass_command
 def compare(
     ctx: click.Context,
     period: str,
     from_date: Optional[DateTime],
     to_date: Optional[DateTime],
     tickers: str,
     export_path: Optional[str],
 ) -> None:
-    """
-    Compares historical prices of given companies. TICKERS is a comma-separated list of tickers.
+    """Compare historical prices of given companies. TICKERS is a comma seperated list of tickers.
 
     Examples:
 
     `i8 price compare --period 3Y --tickers AMD,INTC,QCOM`
     """
     command_path = get_click_command_path(ctx)
     period = period.replace(" ", "").upper()
@@ -149,18 +133,14 @@
                 status.stop()
                 console.print("No data found!")
                 return
             status.update("Generating plot...")
             fig = create_fig(df, period_code, cmd_context)
 
     if export_path:
-        if export_path.split(".")[-1] == "html":
-            table = df2Table(df)
-            export_to_html(table, export_path)
-            return
         export_data(
             df,
             export_path,
             index=True,
             column_width=20,
             column_format=APP_SETTINGS["styles"]["xlsx"]["price"]["column"],
         )
```

### Comparing `i8-terminal-0.2.84/i8_terminal/commands/price/price_list.py` & `i8-terminal-0.2.9/i8_terminal/commands/metrics/metrics_list.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,87 +1,49 @@
-from typing import Optional, cast
+from typing import Any, Dict, Optional
 
 import click
-from click.types import DateTime
-from pandas import DataFrame
 from rich.console import Console
 
-from i8_terminal.commands.price import price
+from i8_terminal.commands.metrics import metrics
 from i8_terminal.common.cli import pass_command
-from i8_terminal.common.formatting import get_formatter
-from i8_terminal.common.layout import df2Table, format_df
-from i8_terminal.common.price import get_historical_price_list_df
-from i8_terminal.common.stock_info import validate_ticker
-from i8_terminal.common.utils import export_data, export_to_html, get_period_code
+from i8_terminal.common.layout import df2Table
+from i8_terminal.common.utils import export_data
 from i8_terminal.config import APP_SETTINGS
-from i8_terminal.types.price_period_param_type import PricePeriodParamType
+from i8_terminal.types.metric_param_type import MetricParamType
 from i8_terminal.types.ticker_param_type import TickerParamType
 
+from i8_terminal.common.metrics import get_current_metrics_df, prepare_current_metrics_formatted_df  # isort:skip
 
-def format_hist_price_df(df: DataFrame, target: str) -> DataFrame:
-    formatters = {
-        "Date": get_formatter("date", target),
-        "open": get_formatter("price", target),
-        "close": get_formatter("price", target),
-        "low": get_formatter("price", target),
-        "high": get_formatter("price", target),
-        "volume": get_formatter("number_int", target),
-        "change_perc": get_formatter("perc", target),
-    }
-    col_names = {
-        "Date": "Date",
-        "open": "Open",
-        "close": "Close",
-        "low": "Low",
-        "high": "High",
-        "volume": "Volume",
-        "change_perc": "Change (%)",
-    }
-    return format_df(df, col_names, formatters)
 
-
-@price.command()
-@click.option("--ticker", "-k", type=TickerParamType(), required=True, callback=validate_ticker, help="Company ticker.")
+@metrics.command()
+@click.option("--tickers", "-k", type=TickerParamType(), required=True, help="Comma-separated list of tickers.")
 @click.option(
-    "--period",
-    "-p",
-    type=PricePeriodParamType(),
-    default="1M",
-    help="Historical price period.",
+    "--metrics",
+    "-m",
+    type=MetricParamType(),
+    default="pe_ratio_ttm",
+    help="Comma-separated list of daily metrics.",
 )
-@click.option("--from_date", "-f", type=DateTime(), help="Histotical price from date.")
-@click.option("--to_date", "-t", type=DateTime(), help="Histotical price to date.")
 @click.option("--export", "export_path", "-e", help="Filename to export the output to.")
 @pass_command
-def list(
-    ticker: str, period: str, from_date: Optional[DateTime], to_date: Optional[DateTime], export_path: Optional[str]
-) -> None:
-    """
-    Lists historical prices for a given TICKER.
-
-    Examples:
-
-    `i8 price list --period 3M --ticker AAPL`
-
-    """
-    period_code = get_period_code(period.replace(" ", "").upper())
+def list(tickers: str, metrics: str, export_path: Optional[str]) -> None:
     console = Console()
     with console.status("Fetching data...", spinner="material"):
-        df = get_historical_price_list_df([ticker], period_code, cast(str, from_date), cast(str, to_date))
-
+        df = get_current_metrics_df(tickers, metrics)
+    if df is None:
+        console.print("No data found for metrics with selected tickers", style="yellow")
+        return
+    for m in [*set(metrics.split(",")) - set(df["metric_name"])]:
+        console.print(f"\nNo data found for metric {m} with selected tickers", style="yellow")
     if export_path:
-        if export_path.split(".")[-1] == "html":
-            df_formatted = format_hist_price_df(df, "console")
-            table = df2Table(df_formatted)
-            export_to_html(table, export_path)
-            return
-        df_formatted = format_hist_price_df(df, "store")
         export_data(
-            df_formatted,
+            prepare_current_metrics_formatted_df(df, "store"),
             export_path,
-            column_width=14,
-            column_format=APP_SETTINGS["styles"]["xlsx"]["price"]["column"],
+            column_width=18,
+            column_format=APP_SETTINGS["styles"]["xlsx"]["financials"]["column"],
         )
     else:
-        df_formatted = format_hist_price_df(df, "console")
-        table = df2Table(df_formatted)
+        columns_justify: Dict[str, Any] = {}
+        for metric_display_name, metric_df in df.groupby("display_name"):
+            columns_justify[metric_display_name] = "left" if metric_df["display_format"].values[0] == "str" else "right"
+        table = df2Table(prepare_current_metrics_formatted_df(df, "console"), columns_justify=columns_justify)
         console.print(table)
```

### Comparing `i8-terminal-0.2.84/i8_terminal/commands/price/price_plot.py` & `i8-terminal-0.2.9/i8_terminal/commands/price/price_plot.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,31 +8,28 @@
 import pandas as pd
 import plotly.graph_objects as go
 from click.types import DateTime
 from pandas.core.frame import DataFrame
 from plotly.subplots import make_subplots
 from rich.console import Console
 
-from i8_terminal.app.layout import get_date_range, get_plot_default_layout
 from i8_terminal.app.plot_server import serve_plot
 from i8_terminal.commands.price import price
 from i8_terminal.common.cli import get_click_command_path, pass_command
-from i8_terminal.common.metrics import (
-    find_similar_indicator,
-    get_indicators_list,
-    get_metrics_display_names,
-    get_period_start_date,
-)
-from i8_terminal.common.stock_info import validate_ticker
-from i8_terminal.common.utils import PlotType, get_period_code, get_period_days
-from i8_terminal.types.chart_param_type import ChartParamType, get_chart_param_types
+from i8_terminal.common.price import get_historical_price_df
 from i8_terminal.types.indicator_param_type import IndicatorParamType
 from i8_terminal.types.price_period_param_type import PricePeriodParamType
 from i8_terminal.types.ticker_param_type import TickerParamType
 
+from i8_terminal.common.utils import PlotType, get_period_code, get_period_days, validate_ticker  # isort:skip
+
+from i8_terminal.app.layout import get_date_range, get_plot_default_layout  # isort:skip
+from i8_terminal.common.metrics import find_similar_indicator, get_indicators_list  # isort:skip
+from i8_terminal.types.chart_param_type import ChartParamType, get_chart_param_types  # isort:skip
+
 
 def get_matched_indicators(indicators_list: List[str]) -> List[str]:
     matched_indicators = []
     if indicators_list:
         for i in indicators_list:
             similar_indicator = find_similar_indicator(i)
             if similar_indicator:
@@ -81,42 +78,30 @@
 
     return indicator_categories
 
 
 def get_data_df(
     tickers: List[str], period: str, indicators: List[str], from_date: Optional[str], to_date: Optional[str]
 ) -> Optional[DataFrame]:
-    indicators.append("close,open,low,high")
-    if from_date:
-        if not to_date:
-            to_date = datetime.now().strftime("%Y-%m-%d")
+    period_code = get_period_code(period)
+    hist_price_df = get_historical_price_df(tickers, period_code, from_date, to_date)
+    if hist_price_df is None:
+        return None
+    hist_price_df = hist_price_df[["Ticker", "Date", "close", "open", "high", "low", "volume"]]
+    rename_cols = {"close": "Close", "open": "Open", "high": "High", "low": "Low"}
+    hist_price_df.rename(columns=rename_cols, inplace=True)
+    if indicators:
+        indicators_df = get_indicators_df(tickers, ",".join(indicators), period, from_date, to_date)
+        merged_df = pd.merge(hist_price_df, indicators_df, on=["Ticker", "Date"])
+        merged_df = merged_df.set_index("Date")
+        merged_df.rename(columns={"ma12": "MA12", "ma26": "MA26", "ma52": "MA52", "rsi14_d": "RSI"}, inplace=True)
+        return merged_df[list(rename_cols.values()) + indicators]
     else:
-        from_date = get_period_start_date(period)
-        to_date = datetime.now().strftime("%Y-%m-%d")
-    historical_prices = investor8_sdk.MetricsApi().get_historical_metrics(
-        symbols=",".join(tickers),
-        metrics=",".join(indicators),
-        from_date=from_date,
-        to_date=to_date,
-    )
-    df = pd.DataFrame.from_records(
-        [
-            (ticker, metric, period_value.period, period_value.period_date_time, period_value.value)
-            for ticker, metric_dict in historical_prices.data.items()
-            for metric, period_value_list in metric_dict.items()
-            for period_value in period_value_list
-        ],
-        columns=["ticker", "metric_name", "period", "period_datetime", "value"],
-    )
-    metadata_df = pd.DataFrame([h.to_dict() for h in historical_prices.metadata])
-    df = pd.merge(df, metadata_df, on="metric_name")
-    df = df.pivot(index="period_datetime", columns="display_name", values="value")
-    df = df[df.columns].astype(float)
-    df.index.name = "Date"
-    return df
+        hist_price_df = hist_price_df.set_index("Date")
+        return hist_price_df[list(rename_cols.values())]
 
 
 def create_fig(
     df: DataFrame,
     period: str,
     indicator_categories: Dict[str, List[str]],
     cmd_context: Dict[str, Any],
@@ -149,44 +134,38 @@
         vertical_spacing=vertical_spacing,
         row_width=row_width,
     )
     if chart_type == "candlestick":
         fig.add_trace(
             go.Candlestick(
                 x=df.index,
-                open=df["Open Price"],
-                high=df["High Price"],
-                low=df["Low Price"],
-                close=df["Close Price"],
+                open=df["Open"],
+                high=df["High"],
+                low=df["Low"],
+                close=df["Close"],
                 name="Price",
                 showlegend=False,
             ),
             row=1,
             col=1,
         )
     else:
-        fig.add_trace(go.Scatter(x=df.index, y=df["Close Price"], name="Close"), row=1, col=1)
+        fig.add_trace(go.Scatter(x=df.index, y=df["Close"], name="Close"), row=1, col=1)
         fig.update_traces(hovertemplate="%{y:$.2f} %{x}")
 
     for idx, (k, ind) in enumerate(indicator_categories.items()):
         for m in ind:
             if m == "volume":
-                fig.add_trace(
-                    go.Bar(x=df.index, y=df[get_metrics_display_names([m])[0]], name="Volume", showlegend=False),
-                    row=idx + 1,
-                    col=1,
-                )
+                fig.add_trace(go.Bar(x=df.index, y=df[m], name="Volume", showlegend=False), row=idx + 1, col=1)
             else:
-                fig.add_trace(
-                    go.Scatter(x=df.index, y=df[get_metrics_display_names([m])[0]], name=m), row=idx + 1, col=1
-                )
+                fig.add_trace(go.Scatter(x=df.index, y=df[m], name=m), row=idx + 1, col=1)
 
     dt_all = pd.date_range(start=df.index[-1], end=df.index[0])
     dt_obs = [d.strftime("%Y-%m-%d") for d in df.index]
-    dt_breaks = [d for d in dt_all.strftime("%Y-%m-%d").tolist() if d not in dt_obs]
+    dt_breaks = [d for d in dt_all.strftime("%Y-%m-%d").tolist() if not d in dt_obs]
 
     fig.update_xaxes(
         rangeslider_visible=False, spikemode="across", spikesnap="cursor", rangebreaks=[dict(values=dt_breaks)]
     )
     if range_selector:
         fig.update_xaxes(rangeselector=get_date_range(get_period_code(period)))
     fig.update_layout(
@@ -255,26 +234,25 @@
     ticker: str,
     period: str,
     indicators: str,
     from_date: Optional[datetime],
     to_date: Optional[datetime],
     chart_type: str,
 ) -> None:
-    """
-    Plots historical prices of a given company.
+    """Plot historical prices of given company.
 
     Examples:
 
     `i8 price plot --period 1M --indicators volume --ticker MSFT --chart_type candlestick`
     """
-    if chart_type not in [t[0] for t in get_chart_param_types()]:
+    if not chart_type in [t[0] for t in get_chart_param_types()]:
         click.echo(f"`{chart_type}` is not valid chart type.")
         return
     period = period.replace(" ", "").upper()
-    indicators_list = indicators.replace(" ", "").split(",") if indicators else []
+    indicators_list = indicators.replace(" ", "").upper().split(",") if indicators else []
     indicators_list = get_matched_indicators(indicators_list)
     indicator_categories = get_indicator_categories(indicators_list)
     ticker = ticker.upper()
     plot_title = f"{ticker} historical prices"
     command_path_parsed_options_dict = {"--indicators": ",".join(indicators_list)}
     if from_date:
         command_path_parsed_options_dict["--from_date"] = from_date.strftime("%Y-%m-%d")
```

### Comparing `i8-terminal-0.2.84/i8_terminal/commands/screen/screen_gainers.py` & `i8-terminal-0.2.9/i8_terminal/commands/watchlist/watchlist_add.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from typing import Optional
+from typing import List
 
 import click
+import investor8_sdk
 from rich.console import Console
+from rich.style import Style
 
-from i8_terminal.commands.screen import screen
+from i8_terminal.app.layout import get_terminal_command_layout
+from i8_terminal.commands.watchlist import watchlist
 from i8_terminal.common.cli import pass_command
-from i8_terminal.common.screen import get_top_stocks_df, render_top_stocks
-from i8_terminal.types.market_indice_param_type import MarketIndiceParamType
-from i8_terminal.types.metric_view_param_type import MetricViewParamType
+from i8_terminal.config import USER_SETTINGS
+from i8_terminal.types.ticker_param_type import TickerParamType
 
+from i8_terminal.types.user_watchlists_param_type import UserWatchlistsParamType  # isort:skip
 
-@screen.command()
-@click.option(
-    "--index",
-    "-i",
-    type=MarketIndiceParamType(),
-    default="$SPX",
-    help="Index of market.",
-)
-@click.option(
-    "--view_name", "view_name", "-v", type=MetricViewParamType(), help="Metric view name in configuration file."
-)
-@click.option("--export", "export_path", "-e", help="Filename to export the output to.")
-@pass_command
-def gainers(index: str, view_name: Optional[str], export_path: Optional[str]) -> None:
-    """
-    Lists today winner companies.
 
-    Examples:
+def add_tickers_to_watchlist(name: str, tickers: List[str]) -> None:
+    wl = investor8_sdk.UserApi().get_watchlist_by_name_user_id(name=name, user_id=USER_SETTINGS.get("user_id"))
+    investor8_sdk.UserApi().add_to_watchlist(body={"Id": wl.id, "Tickers": tickers})
 
-    `i8 screen gainers --index $SPX`
 
-    """
+@watchlist.command()
+@click.option(
+    "--name",
+    "-n",
+    type=UserWatchlistsParamType(),
+    required=True,
+    help="Name of the watchlist.",
+)
+@click.option("--tickers", "-k", type=TickerParamType(), required=True, help="Comma-separated list of tickers.")
+@pass_command
+def add(name: str, tickers: str) -> None:
     console = Console()
-    with console.status("Fetching data...", spinner="material"):
-        df = get_top_stocks_df("winners", index, view_name)
-    if df is None:
-        console.print("No data found for today winners", style="yellow")
-        return
-    table = render_top_stocks(df, export_path=export_path, ascending=False)
-    if table:
-        console.print(table)
+    tickers_list = tickers.replace(" ", "").upper().split(",")
+    with console.status("Updating Watchlist...", spinner="material"):
+        add_tickers_to_watchlist(name, tickers_list)
+    console.print(
+        f"✅ Ticker{'s' if len(tickers_list) > 1 else ''} [cyan]{', '.join(tickers_list)}[/cyan] added to watchlist [cyan]{name}[/cyan] successfully!"
+    )
+    terminal_command_style = Style(**get_terminal_command_layout())
+    console.print(
+        f'Try `[{terminal_command_style}]watchlist details --name "{name}"[/{terminal_command_style}]` to see the watchlist.'
+    )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `i8-terminal-0.2.84/i8_terminal/commands/user/user_login.py` & `i8-terminal-0.2.9/i8_terminal/commands/user/user_login.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 def get_login_authentication_request_id() -> str:
     resp = investor8_sdk.UserApi().create_login_authentication_request(body={"ReqType": 3})
     return str(resp.request_id)
 
 
 def open_browser(request_id: str) -> None:
-    url = f"https://www.investoreight.com/account/authorize?reqId={request_id}&redirectUrl=http://localhost:{APP_SETTINGS['app']['port']}"  # noqa: E501
+    url = f"https://www.investoreight.com/account/authorize?reqId={request_id}&redirectUrl=http://localhost:{APP_SETTINGS['app']['port']}"
     webbrowser.open(url)
 
 
 def login_within_terminal() -> None:
     email = click.prompt("Email", show_default=False, type=str)
     password = click.prompt("Password", hide_input=True, show_default=False, type=str)
     body = {"Email": email, "Password": password}
@@ -27,17 +27,14 @@
         api_response = investor8_sdk.UserApi().login_user(body=body)
         user_setting = {
             "user_id": api_response.user_id,
             "i8_core_token": api_response.token,
             "i8_core_api_key": api_response.api_key,
         }
         save_user_settings(user_setting)
-        investor8_sdk.ApiClient().configuration.api_key["apiKey"] = api_response.api_key
-        investor8_sdk.ApiClient().configuration.api_key["Authorization"] = api_response.token
-        investor8_sdk.ApiClient().configuration.api_key_prefix["Authorization"] = "Bearer"
         click.echo("User logged in successfully!")
     except Exception as e:
         click.echo(e)
 
 
 @user.command()
 @click.option(
```

### Comparing `i8-terminal-0.2.84/i8_terminal/commands/user/webserver.py` & `i8-terminal-0.2.9/i8_terminal/commands/user/webserver.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.84/i8_terminal/commands/watchlist/watchlist_add.py` & `i8-terminal-0.2.9/i8_terminal/commands/watchlist/watchlist_rm.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,57 +4,43 @@
 import investor8_sdk
 from rich.console import Console
 from rich.style import Style
 
 from i8_terminal.app.layout import get_terminal_command_layout
 from i8_terminal.commands.watchlist import watchlist
 from i8_terminal.common.cli import pass_command
-from i8_terminal.common.stock_info import validate_tickers
 from i8_terminal.config import USER_SETTINGS
-from i8_terminal.types.ticker_param_type import TickerParamType
-from i8_terminal.types.user_watchlists_param_type import UserWatchlistsParamType
 
+from i8_terminal.types.user_watchlist_tickers_param_type import UserWatchlistTickersParamType  # isort:skip
+from i8_terminal.types.user_watchlists_param_type import UserWatchlistsParamType  # isort:skip
 
-def add_tickers_to_watchlist(name: str, tickers: List[str]) -> None:
+
+def remove_tickers_from_watchlist(name: str, tickers: List[str]) -> None:
     wl = investor8_sdk.UserApi().get_watchlist_by_name_user_id(name=name, user_id=USER_SETTINGS.get("user_id"))
-    investor8_sdk.UserApi().add_to_watchlist(body={"Id": wl.id, "Tickers": tickers})
+    for ticker in tickers:
+        investor8_sdk.UserApi().remove_from_watchlist(body={"Id": wl.id, "Ticker": ticker})
 
 
 @watchlist.command()
 @click.option(
     "--name",
     "-n",
     type=UserWatchlistsParamType(),
     required=True,
     help="Name of the watchlist.",
 )
 @click.option(
-    "--tickers",
-    "-k",
-    type=TickerParamType(),
-    required=True,
-    callback=validate_tickers,
-    help="Comma-separated list of tickers.",
+    "--tickers", "-k", type=UserWatchlistTickersParamType(), required=True, help="Comma-separated list of tickers."
 )
 @pass_command
-def add(name: str, tickers: str) -> None:
-    """
-    Adds given tickers to a given watchlist.
-
-    Examples:
-
-    `i8 watchlist add --name MyWatchlist --tickers AAPL,MSFT`
-
-    """
+def rm(name: str, tickers: str) -> None:
     console = Console()
     tickers_list = tickers.replace(" ", "").upper().split(",")
     with console.status("Updating Watchlist...", spinner="material"):
-        add_tickers_to_watchlist(name, tickers_list)
+        remove_tickers_from_watchlist(name, tickers_list)
     console.print(
-        f"✅ Ticker{'s' if len(tickers_list) > 1 else ''} [cyan]{', '.join(tickers_list)}\
-            [/cyan] added to watchlist [cyan]{name}[/cyan] successfully!"
+        f"✅ Ticker{'s' if len(tickers_list) > 1 else ''} [cyan]{', '.join(tickers_list)}[/cyan] removed from watchlist [cyan]{name}[/cyan] successfully!"
     )
     terminal_command_style = Style(**get_terminal_command_layout())
     console.print(
-        f'Try `[{terminal_command_style}]watchlist summary --name "{name}"[/{terminal_command_style}]`\
-             to see the watchlist.'
+        f'Try `[{terminal_command_style}]watchlist details --name "{name}"[/{terminal_command_style}]` to see the watchlist.'
     )
```

### Comparing `i8-terminal-0.2.84/i8_terminal/commands/watchlist/watchlist_create.py` & `i8-terminal-0.2.9/i8_terminal/commands/watchlist/watchlist_create.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import click
 import investor8_sdk
 from rich.console import Console
 
 from i8_terminal.commands.watchlist import watchlist
 from i8_terminal.common.cli import pass_command
-from i8_terminal.common.stock_info import validate_tickers
 from i8_terminal.config import USER_SETTINGS
 from i8_terminal.types.ticker_param_type import TickerParamType
 
 
 def create_watchlist(name: str, tickers: List[str]) -> None:
     investor8_sdk.UserApi().create_watchlist(
         body={"UserId": USER_SETTINGS.get("user_id"), "Name": name, "Tickers": tickers}
@@ -19,30 +18,15 @@
 
 @watchlist.command()
 @click.option(
     "--name",
     "-n",
     help="Name of the watchlist you want to create.",
 )
-@click.option(
-    "--tickers",
-    "-k",
-    type=TickerParamType(),
-    required=True,
-    callback=validate_tickers,
-    help="Comma-separated list of tickers.",
-)
+@click.option("--tickers", "-k", type=TickerParamType(), required=True, help="Comma-separated list of tickers.")
 @pass_command
 def create(name: str, tickers: str) -> None:
-    """
-    Creates new watchlist with given name and tickers.
-
-    Examples:
-
-    `i8 watchlist create --name MyWatchlist --tickers AAPL,MSFT`
-
-    """
     console = Console()
     tickers_list = tickers.replace(" ", "").upper().split(",")
     with console.status("Creating Watchlist...", spinner="material"):
         create_watchlist(name, tickers_list)
     console.print(f"✅ Watchlist [cyan]{name}[/cyan] is created successfully!")
```

### Comparing `i8-terminal-0.2.84/i8_terminal/commands/watchlist/watchlist_financials.py` & `i8-terminal-0.2.9/i8_terminal/commands/watchlist/watchlist_financials.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,28 +4,27 @@
 import investor8_sdk
 import pandas as pd
 from rich.console import Console
 
 from i8_terminal.commands.watchlist import watchlist
 from i8_terminal.common.cli import pass_command
 from i8_terminal.common.layout import df2Table
-from i8_terminal.common.metrics import (
-    get_current_metrics_df,
-    prepare_current_metrics_formatted_df,
-)
-from i8_terminal.common.utils import export_data, export_to_html
+from i8_terminal.common.utils import export_data
 from i8_terminal.config import APP_SETTINGS, USER_SETTINGS
-from i8_terminal.types.user_watchlists_param_type import UserWatchlistsParamType
+
+from i8_terminal.common.metrics import get_current_metrics_df, prepare_current_metrics_formatted_df  # isort:skip
+
+from i8_terminal.types.user_watchlists_param_type import UserWatchlistsParamType  # isort:skip
 
 
 def prepare_watchlist_stocks_df(name: str) -> Optional[pd.DataFrame]:
     watchlist = investor8_sdk.UserApi().get_watchlist_by_name_user_id(name=name, user_id=USER_SETTINGS.get("user_id"))
     watchlist_stocks_df = get_current_metrics_df(
         ",".join(watchlist.tickers),
-        APP_SETTINGS["metric_view"]["watchlist_financials"]["metrics"],
+        "total_revenue,net_income,basic_eps,net_cash_from_operating_activities,total_assets,total_liabilities",
     )
     return watchlist_stocks_df
 
 
 @watchlist.command()
 @click.option(
     "--name",
@@ -33,55 +32,26 @@
     type=UserWatchlistsParamType(),
     required=True,
     help="Name of the watchlist.",
 )
 @click.option("--export", "export_path", "-e", help="Filename to export the output to.")
 @pass_command
 def financials(name: str, export_path: Optional[str]) -> None:
-    """
-    Lists financial metrics for a given watchlist.
-
-    Examples:
-
-    `i8 watchlist financials --name MyWatchlist`
-
-    """
     console = Console()
     with console.status("Fetching data...", spinner="material"):
         df = prepare_watchlist_stocks_df(name)
     if df is None:
         console.print("No data found for metrics with selected tickers", style="yellow")
         return
-    period_rows = []
-    for ticker, ticker_df in df.groupby("Ticker"):
-        period_rows.append(
-            {
-                "Ticker": ticker,
-                "metric_name": "period",
-                "value": ticker_df["period"].values[0],
-                "display_name": "Period",
-                "data_format": "str",
-                "display_format": "str",
-            }
-        )
-    df = pd.concat([pd.DataFrame(period_rows), df], ignore_index=True, axis=0)
-    columns_justify: Dict[str, Any] = {}
     if export_path:
-        if export_path.split(".")[-1] == "html":
-            for metric_display_name, metric_df in df.groupby("display_name"):
-                columns_justify[metric_display_name] = (
-                    "left" if metric_df["display_format"].values[0] == "str" else "right"
-                )
-            table = df2Table(prepare_current_metrics_formatted_df(df, "console"), columns_justify=columns_justify)
-            export_to_html(table, export_path)
-            return
         export_data(
             prepare_current_metrics_formatted_df(df, "store"),
             export_path,
             column_width=18,
             column_format=APP_SETTINGS["styles"]["xlsx"]["financials"]["column"],
         )
     else:
+        columns_justify: Dict[str, Any] = {}
         for metric_display_name, metric_df in df.groupby("display_name"):
             columns_justify[metric_display_name] = "left" if metric_df["display_format"].values[0] == "str" else "right"
         table = df2Table(prepare_current_metrics_formatted_df(df, "console"), columns_justify=columns_justify)
         console.print(table)
```

### Comparing `i8-terminal-0.2.84/i8_terminal/commands/watchlist/watchlist_list.py` & `i8-terminal-0.2.9/i8_terminal/commands/watchlist/watchlist_list.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,35 +18,26 @@
 
 def prepare_watchlists_df(watchlists: List[WatchlistDto]) -> DataFrame:
     wls: List[Dict[str, str]] = []
     for wl in watchlists:
         wls.append(
             {
                 "name": wl.name,
-                "tickers": f"{', '.join(str(ticker) for ticker in wl.tickers[:5])} \
-                    {f'and {len(wl.tickers)-5} more' if len(wl.tickers) > 5 else ''}",
+                "tickers": f"{', '.join(str(ticker) for ticker in wl.tickers[:5])} {f'and {len(wl.tickers)-5} more' if len(wl.tickers) > 5 else ''}",
             }
         )
     watchlists_df = DataFrame(wls)
     col_names = {
         "name": "Name",
         "tickers": "Tickers",
     }
     return format_df(watchlists_df, col_names, {})
 
 
 @watchlist.command()
 @pass_command
 def list() -> None:
-    """
-    Lists user watchlists.
-
-    Examples:
-
-    `i8 watchlist list`
-
-    """
     console = Console()
     with console.status("Fetching data...", spinner="material"):
         df = get_user_watchlists()
     table = df2Table(df)
     console.print(table)
```

### Comparing `i8-terminal-0.2.84/i8_terminal/common/cli.py` & `i8-terminal-0.2.9/i8_terminal/common/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from functools import update_wrapper
 from typing import Any, Dict, Optional
 
 import click
 import investor8_sdk
 
 from i8_terminal.config import USER_SETTINGS
-from i8_terminal.utils_setup import get_version
+from i8_terminal.utils import get_version
 
 
 def get_click_command_path(ctx: Any, parsed_options_dict: Optional[Dict[str, str]] = None) -> str:
     command_path = ctx.command_path.replace("  ", " ")
     cm_path = f"i8 {' '.join(command_path.split(' ')[1:])}"
     params = ctx.params
     args = []
```

### Comparing `i8-terminal-0.2.84/i8_terminal/common/financials.py` & `i8-terminal-0.2.9/i8_terminal/common/financials.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,17 +170,16 @@
         for tag in fin.financial_tags:
             fins_dict[idf][tag["tag_name"]] = format_number(
                 tag["value"], tag["unit"], humanize=True, exportize=exportize
             )
 
     df_rows = DataFrame(fins_dict.values(), index=fins_dict.keys()).T
     df_rows = df_rows.where(pd.notnull(df_rows), "-")  # Fill nan with `-`
-    df_rows.index = df_rows.index.set_names(["tag"])
+    df_rows.index = df_rows.index.set_names(["tag_fullname"])
     df_rows = df_rows.reset_index()
-    df_rows["tag"] = df_rows["tag"].apply(lambda x: x.split("_")[0])
 
     return {"header": header_dict, "data": df_rows}
 
 
 def fin_df2export_df(df: pd.DataFrame, periods_list: List[str]) -> pd.DataFrame:
     col_names = {
         "name": "",
@@ -221,15 +220,15 @@
             )
             period_type_disp_name = f" {get_period_type_disp_name(period_type)}"
             t = Table(
                 width=46 + (col_width * (len(statement_codes) - 1)),
                 show_lines=False,
                 show_header=False,
                 box=None,
-                style="cyan" if period_type == "FY" or period_type == "TTM" else None,  # type: ignore
+                style="cyan" if period_type == "FY" or period_type == "TTM" else None,
             )
             t.add_column(width=16)
             for st in statement_codes:
                 t.add_column(width=col_width, justify="center")
             if period_type_df.empty:
                 t.add_row(period_type_disp_name, *["❌", "❌", "❌"])
             else:
@@ -251,30 +250,28 @@
                         if pd.isnull(
                             fiscal_period_df.get_group(statement_code)["fiscal_period"].reset_index(drop=True)[0]
                         ):
                             row_text.append(
                                 "NA"
                                 if (
                                     statement_code == "balance_sheet_statement"
-                                    and (period_type == "TTM" or period_type == "YTD")  # noqa: W503
+                                    and (period_type == "TTM" or period_type == "YTD")
                                 )
                                 else "❌"
                             )
                         else:
                             available_fiscal_periods = []
                             for fiscal_period in fiscal_period_df.get_group(statement_code)["fiscal_period"]:
                                 available_fiscal_periods.append(f"{fiscal_period[0:2]}")
                             available_fiscal_periods = list(dict.fromkeys(available_fiscal_periods))
                             available_fiscal_periods.sort()
                             row_text.append(
                                 "Q1-Q4"
                                 if available_fiscal_periods == ["Q1", "Q2", "Q3", "Q4"]
-                                or (  # noqa: W503
-                                    period_type == "TTM" and available_fiscal_periods == ["Q1", "Q2", "Q3"] and has_fy
-                                )
+                                or (period_type == "TTM" and available_fiscal_periods == ["Q1", "Q2", "Q3"] and has_fy)
                                 else ",".join(available_fiscal_periods)
                             )
                 t.add_row(period_type_disp_name, *row_text)
 
             year_branch.add(t)
 
     return tree
```

### Comparing `i8-terminal-0.2.84/i8_terminal/common/formatting.py` & `i8-terminal-0.2.9/i8_terminal/common/formatting.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,15 @@
 import re
 from datetime import date
-from enum import Enum
 from typing import Any, Optional, Union
 
 import arrow
 import numpy as np
 
 
-class color(Enum):
-    i8_dark = "#015560"
-    i8_light = "#00b08f"
-    i8_red = "#ef553b"
-    i8_green = "#00cc96"
-
-
 def make_svg_responsive(svg_str: str) -> str:
     svg_str = re.sub(r'width=".+?"', "", svg_str, 1)
     svg_str = re.sub(r'height=".+?"', "", svg_str, 1)
     svg_str = re.sub(r'style=""', r'style="fill: rgba(0, 0, 0, 0);"', svg_str, 1)  # Make svg transparent
 
     return svg_str
 
@@ -70,56 +62,14 @@
     if colorize:
         color = "red" if m <= 0 else "green"
         res = f"[{color}]{res}[/{color}]"
 
     return res
 
 
-def format_number_v2(
-    m: int,
-    percision: int = 2,
-    unit: Optional[str] = None,
-    humanize: bool = False,
-    in_millions: bool = False,
-) -> Optional[Union[str, int]]:
-    res: Optional[Union[str, int]] = None
-    if m is None or np.isnan(m):
-        return "-"
-
-    if in_millions:
-        number = abs(m)
-        if m < 0:
-            res = f"({number // 1e6:,.1f})"
-        else:
-            res = f"{number // 1e6:,.1f}"
-
-    elif humanize:
-        number = abs(m)
-        if number < 1e3:
-            res = f"{m:,.{percision}f}"
-        if number >= 1e3 and number < 1e6:
-            res = f"{m / 1e3:,.{percision}f} K"
-        if number >= 1e6 and number < 1e9:
-            res = f"{m / 1e6:,.{percision}f} M"
-        if number >= 1e9 and number < 1e12:
-            res = f"{m / 1e9:,.{percision}f} B"
-        if number >= 1e12:
-            res = f"{m / 1e12:,.{percision}f} T"
-    else:
-        res = f"{m:,.{percision}f}"
-
-    if unit == "percentage":
-        res = f"{res}%" if m <= 0 else f"+{res}%"
-
-    if unit in ["usd", "usdpershare"]:
-        res = f"${res}"
-
-    return res
-
-
 def format_date(date: date, use_elapsed_format: bool = False, use_precise_format: bool = False) -> Any:
     if use_elapsed_format:
         time_span = arrow.utcnow() - arrow.get(date)
         days = time_span.days
         if days >= 2:
             return arrow.get(date, tzinfo="US/Eastern").strftime("%b %d, %Y %I:%M %p ET")
         hours, remainder = divmod(time_span.seconds, 3600)
@@ -154,34 +104,25 @@
     return f"{fyq[-2:]} {fyq[2:-2]}"
 
 
 _formatters_map = {
     ("fyq", "console"): lambda x: format_fyq(x),
     ("fyq", "store"): lambda x: format_fyq(x),
     ("number", "console"): lambda x: format_number(x),
-    ("number", "store"): lambda x: format_number(x, exportize=True),
-    ("colorize_number", "console"): lambda x: format_number(x, colorize=True),
+    ("number", "store"): lambda x: format_number(x),
     ("price", "console"): lambda x: format_number(x, unit="usd"),
     ("price", "store"): lambda x: round(x, 2),
     ("financial", "console"): lambda x: format_number(x, unit="usd", humanize=True),
-    ("financial", "store"): lambda x: format_number(x, exportize=True),
-    ("colorize_financial", "console"): lambda x: format_number(x, unit="usd", humanize=True, colorize=True),
+    ("financial", "store"): lambda x: format_number(x),
     ("number_int", "console"): lambda x: format_number(x, decimal=0),
     ("number_int", "store"): lambda x: int(x),
     ("perc", "console"): lambda x: format_number(x, decimal=2, unit="percentage", colorize=True),
-    ("perc", "store"): lambda x: format_number(x, exportize=True),
-    ("number_perc", "console"): lambda x: format_number(x, decimal=2, unit="percentage"),
+    ("perc", "store"): lambda x: format_number(x, decimal=2),
     ("date", "console"): lambda x: format_date(x),
     ("date", "store"): lambda x: format_date(x),
     ("str", "store"): lambda x: x,
     ("str", "console"): lambda x: x,
 }
 
 
 def get_formatter(name: str, target: str) -> Any:
     return _formatters_map[(name, target)]
-
-
-def styling_markdown_text(text: str) -> str:
-    text = text.replace("#", "")  # Ignore headings
-    text = re.sub("```\n([^`]*)\n```", "[magenta]\\1[/magenta]", text)
-    return re.sub("`([^`]*)`", "[magenta]\\1[/magenta]", text)
```

### Comparing `i8-terminal-0.2.84/i8_terminal/common/layout.py` & `i8-terminal-0.2.9/i8_terminal/common/layout.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,29 +13,20 @@
     for c, f in cols_formatters.items():
         df[c] = df[c].map(f)
     return df[cols_map.keys()].rename(columns=cols_map)
 
 
 def format_metrics_df(df: DataFrame, target: str) -> DataFrame:
     df["value"] = df.apply(
-        lambda metric: get_formatter(
-            "number_int"
-            if metric.data_format == "int" and metric.display_format == "number"
-            else metric.display_format,
-            target,
-        )(
-            locate("int" if metric.data_format == "unsigned_int" else metric.data_format)(locate("float")(metric.value) if metric.data_format == "int" or metric.data_format == "unsigned_int" else metric.value)  # type: ignore # noqa: E501
-        ),
-        axis=1,
+        lambda metric: get_formatter("number_int" if metric.data_format == "int" and metric.display_format == "number" else metric.display_format, target)(locate(metric.data_format)(locate("float")(metric.value) if metric.data_format == "int" else metric.value)), axis=1  # type: ignore
     )
     return df
 
 
 def df2Table(df: DataFrame, style_profile: str = "default", columns_justify: Dict[str, Any] = {}) -> Table:
-    MIN_COL_LENGTH = 13
     style = get_table_style(style_profile)
     table = Table(**style)
     default_justify = {
         "Price": "right",
         "Open": "right",
         "Close": "right",
         "Low": "right",
@@ -45,27 +36,14 @@
         "Change (%)": "right",
         "Market Cap": "right",
         "EPS Cons.": "right",
         "EPS Actual": "right",
         "Revenue Cons.": "right",
         "Revenue Actual": "right",
         "Level": "right",
-        "EPS Estimate": "right",
-        "Revenue Estimate": "right",
-        "EPS Beat Rate": "right",
-        "Revenue Beat Rate": "right",
-        "EPS Surprise": "right",
-        "Revenue Surprise": "right",
-        "EPS Consensus": "right",
-        "Revenue Consensus": "right",
-        "Eps Surprise": "right",
     }
     for c in df.columns:
-        table.add_column(
-            c,
-            justify=columns_justify.get(c, default_justify.get(c, "left")),
-            min_width=min(max(df[c].str.len().max(), len(df[c].name)), MIN_COL_LENGTH),
-        )
+        table.add_column(c, justify=columns_justify.get(c, default_justify.get(c, "left")))
     for _, r in df.iterrows():
-        row = [r[c] if r[c] is not np.nan and r[c] is not None else "-" for c in df.columns]
+        row = [r[c] if r[c] is not np.nan else "-" for c in df.columns]
         table.add_row(*row)
     return table
```

### Comparing `i8-terminal-0.2.84/i8_terminal/common/price.py` & `i8-terminal-0.2.9/i8_terminal/common/price.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.84/i8_terminal/config.py` & `i8-terminal-0.2.9/i8_terminal/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,59 @@
 import logging
 import os
 import shutil
 import sys
 import uuid
 from typing import Any, Dict
 
-import investor8_sdk
 import yaml
-from mergedeep import merge
 from rich.style import Style
 
 from i8_terminal.i8_exception import I8Exception
+from i8_terminal.utils import find_dicts_diff
 
 PACKAGE_PATH = os.path.dirname(__file__)
 EXECUTABLE_APP_DIR = os.path.join(os.path.dirname(sys.executable))
 OS_HOME_PATH = os.path.expanduser("~")
 SETTINGS_FOLDER = os.path.join(OS_HOME_PATH, ".i8_terminal")
-METRICS_METADATA_PATH = os.path.join(SETTINGS_FOLDER, "metrics_metadata.csv")
 USER_SETTINGS_PATH = os.path.join(SETTINGS_FOLDER, "user.yml")
 APP_SETTINGS_PATH = os.path.join(SETTINGS_FOLDER, "config.yml")
 ASSETS_PATH = os.path.join(PACKAGE_PATH, "assets")
 I8_TERMINAL_LOGO_URL = "https://www.investoreight.com/media/i8t-chart-logo.png"
 
 
 def init_settings() -> None:
     if not os.path.exists(SETTINGS_FOLDER):
         try:
             os.mkdir(SETTINGS_FOLDER)
-        except Exception:
+        except:
             logging.error(
-                f"Cannot initialize app. Application needs write access to create app directory in the following path: \
-                    '{OS_HOME_PATH}'"
+                f"Cannot initialize app. Application needs write access to create app directory in the following path: '{OS_HOME_PATH}'"
             )
 
     if not os.path.exists(USER_SETTINGS_PATH):
         try:
             user_setting = {"app_instance_id": uuid.uuid4().hex}
             with open(USER_SETTINGS_PATH, "w") as f:
                 yaml.dump(user_setting, f)
-        except Exception:
+        except:
             logging.error(
                 f"Cannot initalize user settings. Make sure you have write access to the path: '{USER_SETTINGS_PATH}'"
             )
 
     if not os.path.exists(APP_SETTINGS_PATH):
         try:
             app_settings_src_path = os.path.join(PACKAGE_PATH, "config.yml")
             if os.path.exists(app_settings_src_path):
                 shutil.copyfile(app_settings_src_path, APP_SETTINGS_PATH)
             else:
                 shutil.copyfile(f"{EXECUTABLE_APP_DIR}/config.yml", APP_SETTINGS_PATH)
         except Exception as e:
             logging.error(
-                f"Cannot initalize app settings. Make sure you have write access to the path: \
-                    '{APP_SETTINGS_PATH}'\n {e}"
+                f"Cannot initalize app settings. Make sure you have write access to the path: '{APP_SETTINGS_PATH}'\n {e}"
             )
 
 
 def load_user_settings() -> Any:
     if not os.path.exists(USER_SETTINGS_PATH):
         return {}
     with open(USER_SETTINGS_PATH, "r") as f:
@@ -92,79 +88,47 @@
 def restore_user_settings() -> None:
     current_user_settings = load_user_settings()
     restored_user_setting = {"app_instance_id": current_user_settings.get("app_instance_id")}
     with open(USER_SETTINGS_PATH, "w") as f:
         yaml.dump(restored_user_setting, f)
 
 
-def find_dicts_diff(dict1: Dict[str, Any], dict2: Dict[str, Any]) -> Dict[str, Any]:
-    result = {}
-    for k in dict1:
-        if k in dict2:
-            if type(dict1[k]) is dict:
-                res = find_dicts_diff(dict1[k], dict2[k])
-                if res:
-                    result[k] = res
-            if dict1[k] != dict2[k]:
-                result[k] = dict1[k]
-        else:
-            result[k] = dict1[k]
-    for k in dict2:
-        if k not in dict1:
-            result[k] = dict2[k]
-    return result
-
-
 def update_settings() -> None:
     current_app_settings = load_app_settings()
     latest_app_settings = load_latest_app_settings()
-    app_new_settings = find_dicts_diff(latest_app_settings, current_app_settings)
-    user_new_settings = find_dicts_diff(current_app_settings, latest_app_settings)
-    if app_new_settings or user_new_settings:
-        new_settings = merge({}, latest_app_settings, current_app_settings)
+    new_settings = find_dicts_diff(latest_app_settings, current_app_settings)
+    if new_settings:
+        new_app_settings = {**current_app_settings, **new_settings}
         with open(APP_SETTINGS_PATH, "w") as f:
-            yaml.dump(new_settings, f)
+            yaml.dump(new_app_settings, f)
 
 
 def get_table_style(profile_name: str = "default") -> Dict[str, Any]:
     styles = APP_SETTINGS["styles"]["table"][profile_name]
     try:
         return {
             "header_style": Style(**styles["header"]),
             "row_styles": [Style(**styles["row"]), Style(**styles["alternate_row"])],
             "show_lines": styles.get("show_lines", False),
         }
-    except Exception:
+    except:
         raise I8Exception(
-            "Cannot parse table style settings from the configuration file! \
-                Check to see if the configuration file is formatted correctly!"
+            "Cannot parse table style settings from the configuration file! Check to see if the configuration file is formatted correctly!"
         )
 
 
 def is_user_logged_in() -> bool:
     if not USER_SETTINGS.get("i8_core_api_key") or not USER_SETTINGS.get("i8_core_token"):
         return False
     return True
 
 
-def init_api_configs() -> None:
-    investor8_sdk.ApiClient().configuration.api_key["apiKey"] = USER_SETTINGS.get("i8_core_api_key")
-    investor8_sdk.ApiClient().configuration.api_key["Authorization"] = USER_SETTINGS.get("i8_core_token")
-    investor8_sdk.ApiClient().configuration.api_key_prefix["Authorization"] = "Bearer"
-
-
-def init_notebook() -> None:
-    if is_user_logged_in():
-        init_api_configs()
-    else:
-        print("You are not logged in. Please login to i8 Terminal using 'user login' command.")
-
-
 if "USER_SETTINGS" not in globals():
     init_settings()
-    update_settings()
     USER_SETTINGS = load_user_settings()
     APP_SETTINGS = load_app_settings()
 
 if not USER_SETTINGS.get("app_instance_id"):
     user_setting = {"app_instance_id": uuid.uuid4().hex}
     save_user_settings(user_setting)
+
+update_settings()
```

### Comparing `i8-terminal-0.2.84/i8_terminal/i8_terminal.egg-info/PKG-INFO` & `i8-terminal-0.2.9/i8_terminal/i8_terminal.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,100 +1,92 @@
 Metadata-Version: 2.1
 Name: i8-terminal
-Version: 0.2.84
+Version: 0.2.9
 Summary: Investor8 CLI
 Home-page: UNKNOWN
 Author: investoreight
 Author-email: info@investoreight.com
 License: MIT
 Project-URL: Homepage, https://i8terminal.io/
 Project-URL: Documentation, https://docs.i8terminal.io/
 Project-URL: Download, https://i8terminal.io/download
 Project-URL: Source Code, https://github.com/investoreight/i8-terminal
 Project-URL: Bug Tracker, https://github.com/investoreight/i8-terminal/issues
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# i8 Terminal: Modern Market Research powered by the Command-Line
+# i8 Terminal: Modern Market Research with the Power of Command-Line
 
-[i8 terminal](https://www.i8terminal.io) is a modern python-based terminal application that gives you superior power and flexibility to understand and analyze the market. The interface is simple, efficient, and powerful: it's command-line!
+[i8 terminal](https://www.i8terminal.io) is a modern python-based terminal application that gives you a superior power and flexibility to understand and analyze the market. The interface is simple, efficient, and powerful: it's command-line!
 
 i8 Terminal is backed by the [Investoreight Platform](https://www.investoreight.com) and currently covers major U.S. exchanges.
 
 ## Features and Highlights
 - Prompt Market Insights and Analysis
 - Custom Charting, Reporting, and Visualizations
 - Powerful and Customizable Screening
 - Easy-to-Use and Extendable
 - Backed by the [Investoreight Platform](https://www.investoreight.com)
 
 ![i8 Terminal Features](https://www.i8terminal.io/img/gif/i8-terminal-demo.gif)
 
 ## i8 Terminal Commands
-i8 Terminal offers some built-in commands to analyze and research the market. You can also create your own custom commands or extend the existing command. Find an overview of commands [here](https://i8terminal.io/#commands).
+i8 Terminal offer some built-in commands to analyze and research the market. You can also create your own custom commands or extend the existing command. Find an overview of commands [here](https://i8terminal.io/#commands).
 
-Check out the following video to see some more commands from i8 Terminal:
+Checkout the following video to see some more commands from i8 Terminal:
 
 [![i8 Terminal Sample Commands](https://img.youtube.com/vi/NpOCqcb-RxY/0.jpg)](https://www.youtube.com/watch?v=NpOCqcb-RxY)
 
 
 ## Installing i8 Terminal
-**Note**: i8 Terminal currently only supports Python 3.9+
+**Note**: i8 Terminal currenly only supports Python 3.9+
 
 If you have Python 3 installed, you can simply install the tool with Python pip:
 
 ```
 pip install i8-terminal
 ```
 
-We recommend installing i8 terminal in an isolated virtual environment. This can be done as follows:
+We recommend to install i8 terminal in an isolated virtual environment. This can be done as follows:
 
 #### On Mac OS or Linux:
 
 ```
-python3 -m venv .venv
-source .venv/bin/activate
+python3 -m venv .venv 
+source .venv/bin/activate 
 pip install i8-terminal
 ```
 
 #### On Windows:
 
 ```
-python3 -m venv .venv
-source .venv/Script/activate
+python3 -m venv .venv 
+source .venv/Script/activate 
 pip install i8-terminal
 ```
 
 ### Install i8 Terminal using the Windows Installer
-On Windows, you can also install i8 Terminal using the Windows executable. Check [here](https://i8terminal.io/download) if you want to download the windows executable.
+On Windows you can also install i8 Terminal using the windows executable. Check [here](https://i8terminal.io/download) if you want to download the windows executable.
 
 
-## How to Contribute i8 Terminal
-The preferred workflow for contributing to i8 Terminal is to clone the
-[GitHub repository](https://github.com/investoreight/i8-terminal), develop on a branch and make a Pull Request.
-
-See [here](https://github.com/investoreight/i8-terminal/blob/main/CONTRIBUTING.md) for guidelines for contributors.
-
-i8 Terminal is built on top of the [Investoreight Core API](https://github.com/investoreight/investor8-sdk).
-
 ## How to Run i8 Terminal
-You can verify whether i8 Terminal is installed successfully by running i8 script:
+You can verify whether i8 Terminal is installed succefully by running i8 script:
 
 ```
 i8
 ```
 
-If you are using the application for the first time, you should first sign in. Run the following command, which will open a browser and redirect you to the investoreight platform to sign in (or sign up):
+If you are using the application for the first time, you should first sign in. Run the following command, which will open a browser and redirects you to the investoreight platform to sing in (or sign up):
 
 ```
 i8 user login
 ```
 
-After a successful login, the most convenient way to use i8 terminal is to use its own shell:
+After a succesful login, the most convenient way to use i8 terminal is to use its own shell:
 
 ```
 i8 shell
 ```
 
 You should now be able to run i8 commands. Check our [documentation](https://docs.i8terminal.io/) for more details.
```

### Comparing `i8-terminal-0.2.84/i8_terminal/i8_terminal.egg-info/SOURCES.txt` & `i8-terminal-0.2.9/i8_terminal/i8_terminal.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -5,18 +5,16 @@
 requirements.txt
 setup.py
 i8_terminal/__init__.py
 i8_terminal/config.py
 i8_terminal/config.yml
 i8_terminal/i8_exception.py
 i8_terminal/main.py
-i8_terminal/utils_setup.py
+i8_terminal/utils.py
 i8_terminal/version.txt
-i8_terminal/api/__init__.py
-i8_terminal/api/earnings/__init__.py
 i8_terminal/app/__init__.py
 i8_terminal/app/layout.py
 i8_terminal/app/plot_server.py
 i8_terminal/assets/favicon.ico
 i8_terminal/assets/i8t_chart_logo.png
 i8_terminal/assets/i8t_logo.png
 i8_terminal/assets/loading.gif
@@ -35,86 +33,61 @@
 i8_terminal/commands/financials/financials_compare.py
 i8_terminal/commands/financials/financials_coverage.py
 i8_terminal/commands/financials/financials_list.py
 i8_terminal/commands/financials/financials_plot.py
 i8_terminal/commands/market/__init__.py
 i8_terminal/commands/market/market_summary.py
 i8_terminal/commands/metrics/__init__.py
-i8_terminal/commands/metrics/metrics_current.py
 i8_terminal/commands/metrics/metrics_describe.py
-i8_terminal/commands/metrics/metrics_historical.py
-i8_terminal/commands/metrics/metrics_search.py
+i8_terminal/commands/metrics/metrics_list.py
+i8_terminal/commands/metrics/metrics_plot.py
 i8_terminal/commands/news/__init__.py
 i8_terminal/commands/news/news_list.py
-i8_terminal/commands/notebook/__init__.py
-i8_terminal/commands/notebook/notebook_launch.py
 i8_terminal/commands/price/__init__.py
 i8_terminal/commands/price/price_compare.py
 i8_terminal/commands/price/price_list.py
 i8_terminal/commands/price/price_plot.py
 i8_terminal/commands/screen/__init__.py
-i8_terminal/commands/screen/screen_gainers.py
 i8_terminal/commands/screen/screen_list.py
-i8_terminal/commands/screen/screen_losers.py
-i8_terminal/commands/screen/screen_search.py
 i8_terminal/commands/user/__init__.py
 i8_terminal/commands/user/user_login.py
 i8_terminal/commands/user/user_logout.py
 i8_terminal/commands/user/webserver.py
 i8_terminal/commands/watchlist/__init__.py
 i8_terminal/commands/watchlist/watchlist_add.py
 i8_terminal/commands/watchlist/watchlist_create.py
-i8_terminal/commands/watchlist/watchlist_export.py
 i8_terminal/commands/watchlist/watchlist_financials.py
 i8_terminal/commands/watchlist/watchlist_list.py
 i8_terminal/commands/watchlist/watchlist_metrics.py
 i8_terminal/commands/watchlist/watchlist_rm.py
 i8_terminal/commands/watchlist/watchlist_summary.py
 i8_terminal/common/__init__.py
 i8_terminal/common/cli.py
 i8_terminal/common/financials.py
 i8_terminal/common/formatting.py
 i8_terminal/common/layout.py
 i8_terminal/common/metrics.py
 i8_terminal/common/price.py
-i8_terminal/common/screen.py
 i8_terminal/common/stock_info.py
 i8_terminal/common/utils.py
 i8_terminal/i8_terminal.egg-info/PKG-INFO
 i8_terminal/i8_terminal.egg-info/SOURCES.txt
 i8_terminal/i8_terminal.egg-info/dependency_links.txt
 i8_terminal/i8_terminal.egg-info/entry_points.txt
 i8_terminal/i8_terminal.egg-info/requires.txt
 i8_terminal/i8_terminal.egg-info/top_level.txt
-i8_terminal/service_result/__init__.py
-i8_terminal/service_result/column_info.py
-i8_terminal/service_result/columns_context.py
-i8_terminal/service_result/earning_list_result.py
-i8_terminal/service_result/service_result.py
-i8_terminal/services/__init__.py
-i8_terminal/services/earnings.py
 i8_terminal/types/__init__.py
 i8_terminal/types/auto_complete_choice.py
 i8_terminal/types/chart_param_type.py
 i8_terminal/types/command_parser.py
-i8_terminal/types/condition_param_type.py
 i8_terminal/types/fin_identifier_param_type.py
 i8_terminal/types/fin_period_param_type.py
 i8_terminal/types/fin_statement_param_type.py
 i8_terminal/types/i8_auto_suggest.py
 i8_terminal/types/i8_completer.py
 i8_terminal/types/indicator_param_type.py
-i8_terminal/types/market_indice_param_type.py
-i8_terminal/types/metric_identifier_param_type.py
 i8_terminal/types/metric_param_type.py
-i8_terminal/types/metric_view_param_type.py
-i8_terminal/types/output_param_type.py
-i8_terminal/types/period_param_type.py
 i8_terminal/types/period_type_param_type.py
 i8_terminal/types/price_period_param_type.py
-i8_terminal/types/screening_condition_param_type.py
-i8_terminal/types/screening_operator_param_type.py
-i8_terminal/types/screening_value_field_param_type.py
-i8_terminal/types/sort_order_param_type.py
 i8_terminal/types/ticker_param_type.py
 i8_terminal/types/user_watchlist_tickers_param_type.py
 i8_terminal/types/user_watchlists_param_type.py
```

### Comparing `i8-terminal-0.2.84/i8_terminal/main.py` & `i8-terminal-0.2.9/i8_terminal/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 import os
 import sys
 
 from rich.console import Console
 
 from i8_terminal.common.cli import log_terminal_usage, pass_command
-from i8_terminal.config import USER_SETTINGS, init_api_configs, is_user_logged_in
-from i8_terminal.utils_setup import get_version
+from i8_terminal.config import USER_SETTINGS, is_user_logged_in
+from i8_terminal.utils import get_version
 
 console = Console(force_terminal=True, color_system="truecolor")
 if set(["i8"]) == set(sys.argv[1:]):
     console.print(f"\n👋 Welcome to i8 Terminal! Version: {get_version()}", style="yellow")
     console.print("Copyright © 2020-2022 Investoreight | https://www.i8terminal.io/\n")
     console.print("- Enter [magenta]i8 shell[/magenta] to run i8 Terminal shell.")
     os._exit(0)
 if set(["i8", "version"]) == set(sys.argv[1:]):
     console.print(f"Version: {get_version()}", style="yellow")
     os._exit(0)
 status = console.status("Starting Up...", spinner="material")
 status.start()
 
 
-import webbrowser
-
 import click
 import investor8_sdk
 from click_repl import repl
 from investor8_sdk.rest import ApiException
 
 from i8_terminal.commands import cli
-from i8_terminal.common.stock_info import validate_ticker
 from i8_terminal.types.i8_auto_suggest import I8AutoSuggest
 from i8_terminal.types.i8_completer import I8Completer
-from i8_terminal.types.ticker_param_type import TickerParamType
 
 
 def init_commands() -> None:
     status.start()
     app_dir = os.path.join(os.path.join(os.path.dirname(sys.executable), "lib"), "i8_terminal")
     sys.path.append(app_dir)
     commands_dir = os.path.join(os.path.dirname(os.path.abspath(__file__)), "commands")
@@ -57,16 +53,15 @@
 
         while True:
             try:
                 repl(click.get_current_context(), prompt_kwargs=prompt_kwargs)
             except ApiException as e:
                 if "apiKey" in e.body.decode("utf-8"):
                     console.print(
-                        "You need to login before using i8 Terminal. Please login to i8 Terminal using \
-                            [magenta]user login[/magenta] command."
+                        "You need to login before using i8 Terminal. Please login to i8 Terminal using [magenta]user login[/magenta] command."
                     )
                 else:
                     console.print(f"⚠ Error: {e.body.decode('utf-8')}", style="yellow")
                 log_terminal_usage(click.get_current_context(), e.body.decode("utf-8"))
             except Exception as e:
                 display_error = f"- Type: {type(e).__name__}\n- Message: {e}"
                 log_terminal_usage(click.get_current_context(), display_error)
@@ -88,39 +83,17 @@
     @pass_command
     def clear(all: bool) -> None:
         """Clear the console screen."""
         cls_screen()
         if not all:
             print_welcome_msg()
 
-    @cli.command()
-    @click.option(
-        "--ticker",
-        "-k",
-        type=TickerParamType(),
-        required=True,
-        callback=validate_ticker,
-        help="Ticker or company name.",
-    )
-    @pass_command
-    def browse(ticker: str) -> None:
-        """
-        Open company detail page in investoreight.com
-
-        Examples:
-
-        `i8 browse --ticker MSFT`
-        """
-        url = f"https://www.investoreight.com/stock/{ticker}"
-        webbrowser.open(url)
-        console.print(f"[blue]{url}[/blue]")
-
 
 def print_welcome_msg() -> None:
-    console.print(f"\n👋 Welcome to i8 Terminal! Version:  {get_version()}", style="yellow")
+    console.print(f"\n👋 Welcome to i8 Terminal! Version: {get_version()}", style="yellow")
     console.print("Copyright © 2020-2022 Investoreight | https://www.i8terminal.io/")
     console.print("- Enter [magenta]?[/magenta] to get the list of commands.")
     console.print("- Enter [magenta]exit[/magenta] to exit the shell.\n")
     if is_user_logged_in():
         console.print(f'Logged in as "{USER_SETTINGS["user_id"]}".\n')
     else:
         console.print(
@@ -132,46 +105,37 @@
     os.system("cls" if os.name == "nt" else "clear")
 
 
 def check_version() -> None:
     resp = None
     try:
         resp = investor8_sdk.SettingsApi().check_i8t_version(get_version())
-    except Exception:
+    except:
         pass
     if not resp or not resp.to_dict().get("version_supported"):
         status.stop()
         console.print(
             "[yellow]You are using an old version of i8 Terminal that is not supported anymore.[/yellow]",
-            "[yellow]Please update i8 Terminal with the following command to be able to use the application.[/yellow]",
-            "\n[magenta]i8update[/magenta]\n",
+            "[yellow]Please update i8 Terminal with the following command to be able to use the application.[/yellow]\n",
+            "[magenta]i8update[/magenta]\n",
             "If you are using Python pip, you can run the following command to update i8 Terminal:\n",
             "[magenta]pip install --upgrade i8-terminal[/magenta]",
         )
         os._exit(0)
 
 
 def main() -> None:
     check_version()
     init_commands()
+
     if is_user_logged_in():
-        init_api_configs()
+        investor8_sdk.ApiClient().configuration.api_key["apiKey"] = USER_SETTINGS.get("i8_core_api_key")
+        investor8_sdk.ApiClient().configuration.api_key["Authorization"] = USER_SETTINGS.get("i8_core_token")
+        investor8_sdk.ApiClient().configuration.api_key_prefix["Authorization"] = "Bearer"
 
-    try:
-        cli(obj={})
-    except ApiException as e:
-        if "apiKey" in e.body.decode("utf-8"):
-            console.print(
-                "You need to login before using i8 Terminal. Please login to i8 Terminal \
-                    using [magenta]user login[/magenta] command."
-            )
-        else:
-            console.print(f"⚠ Error: {e.body.decode('utf-8')}", style="yellow")
-    except Exception as e:
-        display_error = f"- Type: {type(e).__name__}\n- Message: {e}"
-        console.print(f"⚠ Error:\n{display_error}", style="yellow")
+    cli(obj={})
 
 
 if __name__ == "__main__":
     main()
 else:
     init_commands()
```

### Comparing `i8-terminal-0.2.84/i8_terminal/types/auto_complete_choice.py` & `i8-terminal-0.2.9/i8_terminal/types/auto_complete_choice.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.84/i8_terminal/types/chart_param_type.py` & `i8-terminal-0.2.9/i8_terminal/types/chart_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.84/i8_terminal/types/command_parser.py` & `i8-terminal-0.2.9/i8_terminal/types/command_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 class CommandParser:
     def __init__(self, cli: Callable[[F], Group]) -> None:
         self.cli = cast(Group, cli)
 
     def parse(self, document: Document) -> Union[CompleterContext, None]:
         tokens = document.text.split(" ")
         used_options = [p for p in tokens if p.startswith("-")]
-        last_option = tokens[-2] if len(tokens) > 2 and tokens[-2].startswith("-") else None
+        last_option = tokens[-2] if len(tokens) > 3 and tokens[-2].startswith("-") else None
 
         try:
             args = shlex.split(document.text_before_cursor)
         except ValueError:
             # Invalid command, perhaps caused by missing closing quotation.
             return None
```

### Comparing `i8-terminal-0.2.84/i8_terminal/types/fin_identifier_param_type.py` & `i8-terminal-0.2.9/i8_terminal/types/user_watchlist_tickers_param_type.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from datetime import datetime
 from typing import List, Tuple
 
+import investor8_sdk
+
+from i8_terminal.common.stock_info import get_stocks
+from i8_terminal.config import USER_SETTINGS
 from i8_terminal.types.auto_complete_choice import AutoCompleteChoice
-from i8_terminal.types.fin_period_param_type import FinancialsPeriodParamType
-from i8_terminal.types.ticker_param_type import TickerParamType
 
 
-class FinancialsIdentifierParamType(AutoCompleteChoice):
-    name = "financials"
+def get_user_watchlist_tickers() -> List[Tuple[str, str]]:
+    results = investor8_sdk.UserApi().get_watchlists_by_user(user_id=USER_SETTINGS.get("user_id"))
+    tickers = set(ticker for wl in results.watchlists for ticker in wl.tickers)
+    stocks = get_stocks()
+    return [(tk, name) for (tk, name) in stocks if tk in tickers]
+
+
+class UserWatchlistTickersParamType(AutoCompleteChoice):
+    name = "userwatchlisttickers"
+
+    def get_suggestions(self, keyword: str, pre_populate: bool = False) -> List[Tuple[str, str]]:
+        if not self.is_loaded:
+            self.set_choices(get_user_watchlist_tickers())
+
+        if pre_populate and keyword.strip() == "":
+            return self._choices[: self.size]
 
-    def __init__(self) -> None:
-        self._ticker_auto_comp = TickerParamType()
-        self._period_auto_comp = FinancialsPeriodParamType()
-
-    def get_suggestions(
-        self, keyword: str, pre_populate: bool = False, param_type: str = None
-    ) -> List[Tuple[str, str]]:
-        if param_type == "ticker":
-            return self._ticker_auto_comp.get_suggestions(keyword)
-        elif param_type == "year":
-            years = [(str(i), "") for i in range(datetime.now().year, 2008, -1)]
-            if keyword.strip() == "":
-                return years
-            return [y for y in years if y[0].startswith(keyword)]
-        else:
-            return self._period_auto_comp.get_suggestions(keyword, True)
+        return self.search_keyword(keyword)
 
     def __repr__(self) -> str:
-        return "FINANCIALS"
+        return "USERWATCHLISTTICKERS"
```

### Comparing `i8-terminal-0.2.84/i8_terminal/types/fin_period_param_type.py` & `i8-terminal-0.2.9/i8_terminal/types/fin_period_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.84/i8_terminal/types/fin_statement_param_type.py` & `i8-terminal-0.2.9/i8_terminal/types/fin_statement_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.84/i8_terminal/types/i8_auto_suggest.py` & `i8-terminal-0.2.9/i8_terminal/types/i8_auto_suggest.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from click import Group
 from click.decorators import F
 from prompt_toolkit.auto_suggest import AutoSuggest, Suggestion
 from prompt_toolkit.buffer import Buffer
 from prompt_toolkit.document import Document
 
 from i8_terminal.types.command_parser import CommandParser
-from i8_terminal.types.fin_identifier_param_type import FinancialsIdentifierParamType
-from i8_terminal.types.metric_identifier_param_type import MetricIdentifierParamType
+
+from i8_terminal.types.fin_identifier_param_type import FinancialsIdentifierParamType  # isort:skip
 
 
 class I8AutoSuggest(AutoSuggest):
     """
     Give suggestions based on click option types.
     """
 
@@ -28,15 +28,15 @@
         command = ctx.click_ctx.command
 
         if ctx.last_option:
             matched_params = [p for p in command.params if isinstance(p, click.Option) and ctx.last_option in p.opts]
             if len(matched_params) > 0:
                 matched_param = matched_params[0]
                 if type(matched_param.type) is click.types.DateTime:
-                    return Suggestion("YYYY-MM-DD"[len(ctx.incomplete) :])  # noqa: E203
+                    return Suggestion("YYYY-MM-DD"[len(ctx.incomplete) :])
                 elif type(matched_param.type) is FinancialsIdentifierParamType:
                     parts_num = 3
                     parts = ctx.incomplete.split(",")
                     incomplete = parts[-1] if len(parts) > 0 else " "
                     sub_parts = incomplete.split("-")
                     if len(sub_parts) > 2:
                         parts_num = 1
@@ -47,25 +47,10 @@
                         return Suggestion("Ticker-[Fiscal Year]-[Fiscal Period]")
                     elif parts_num == 3:
                         return Suggestion("-[Fiscal Year]-[Fiscal Period]")
                     elif parts_num == 2:
                         return Suggestion("-[Fiscal Period]")
                 elif matched_param.name == "export_path":
                     if len(ctx.incomplete) < 1:
-                        return Suggestion("[path]/[filename].[csv|xlsx|pdf|html]")
-                elif matched_param.name == "path":
-                    if len(ctx.incomplete) < 1:
-                        return Suggestion("[path]/[filename].[xlsx]")
-                elif type(matched_param.type) is MetricIdentifierParamType:
-                    parts_num = 2
-                    parts = ctx.incomplete.split(",")
-                    incomplete = parts[-1] if len(parts) > 0 else " "
-                    sub_parts = incomplete.split(".")
-                    if len(sub_parts) > 1:
-                        parts_num = 1
-
-                    if len(incomplete) < 1:
-                        return Suggestion("Metric.[Optional Period]")
-                    elif parts_num == 2:
-                        return Suggestion(".[Optional Period]")
+                        return Suggestion("[path]/[filename].[csv|xlsx|pdf]")
 
         return None
```

### Comparing `i8-terminal-0.2.84/i8_terminal/types/indicator_param_type.py` & `i8-terminal-0.2.9/i8_terminal/types/indicator_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.84/i8_terminal/types/market_indice_param_type.py` & `i8-terminal-0.2.9/i8_terminal/types/price_period_param_type.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 from typing import List, Tuple
 
 from i8_terminal.types.auto_complete_choice import AutoCompleteChoice
 
 
-def get_market_indice_types() -> List[Tuple[str, str]]:
-    return [("$DJI", "Dow 30"), ("$SPX", "S&P 500"), ("$NDX", "NASDAQ 100")]
+def get_price_periods() -> List[Tuple[str, str]]:
+    return [
+        ("1M", "One Month"),
+        ("3M", "Three Months"),
+        ("6M", "Six Months"),
+        ("1Y", "One Year"),
+        ("3Y", "Three Years"),
+        ("5Y", "Five Years"),
+    ]
 
 
-class MarketIndiceParamType(AutoCompleteChoice):
-    name = "marketindice"
+class PricePeriodParamType(AutoCompleteChoice):
+    name = "priceperiod"
 
     def get_suggestions(self, keyword: str, pre_populate: bool = True) -> List[Tuple[str, str]]:
         if not self.is_loaded:
-            self.set_choices(get_market_indice_types())
+            self.set_choices(get_price_periods())
 
         if pre_populate and keyword.strip() == "":
             return self._choices[: self.size]
         return self.search_keyword(keyword)
 
     def __repr__(self) -> str:
-        return "MARKETINDICE"
+        return "PRICEPERIOD"
```

### Comparing `i8-terminal-0.2.84/i8_terminal/types/metric_identifier_param_type.py` & `i8-terminal-0.2.9/i8_terminal/types/metric_param_type.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from typing import List, Tuple
 
+from i8_terminal.common.metrics import get_all_metrics_df
 from i8_terminal.types.auto_complete_choice import AutoCompleteChoice
-from i8_terminal.types.metric_param_type import MetricParamType
-from i8_terminal.types.period_param_type import PeriodParamType
 
 
-class MetricIdentifierParamType(AutoCompleteChoice):
-    name = "metricidentifier"
+def get_metrics() -> List[Tuple[str, str]]:
+    df = get_all_metrics_df()[["metric_name", "display_name"]]
+    return list(df.to_records(index=False))
 
-    def __init__(self) -> None:
-        self._metric_auto_comp = MetricParamType()
-        self._period_auto_comp = PeriodParamType()
-
-    def get_suggestions(
-        self, keyword: str, pre_populate: bool = True, param_type: str = None, metric: str = None
-    ) -> List[Tuple[str, str]]:
-        if param_type == "metric":
-            return self._metric_auto_comp.get_suggestions(keyword)
-        else:
-            return self._period_auto_comp.get_suggestions(keyword, metric=metric)  # type: ignore
+
+class MetricParamType(AutoCompleteChoice):
+    name = "metric"
+
+    def get_suggestions(self, keyword: str, pre_populate: bool = True) -> List[Tuple[str, str]]:
+        if not self.is_loaded:
+            self.set_choices(get_metrics())
+
+        if pre_populate and keyword.strip() == "":
+            return self._choices[: self.size]
+
+        return self.search_keyword(keyword)
 
     def __repr__(self) -> str:
-        return "METRICIDENTIFIER"
+        return "METRIC"
```

### Comparing `i8-terminal-0.2.84/i8_terminal/types/metric_param_type.py` & `i8-terminal-0.2.9/i8_terminal/types/user_watchlists_param_type.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 from typing import List, Tuple
 
-from i8_terminal.common.metrics import get_all_metrics_df
+import investor8_sdk
+import pandas as pd
+
+from i8_terminal.config import USER_SETTINGS
 from i8_terminal.types.auto_complete_choice import AutoCompleteChoice
 
 
-def get_metrics() -> List[Tuple[str, str]]:
-    df = get_all_metrics_df()[["metric_name", "display_name"]]
+def get_user_watchlists() -> List[Tuple[str, str]]:
+    results = investor8_sdk.UserApi().get_watchlists_by_user(user_id=USER_SETTINGS.get("user_id"))
+    df = pd.DataFrame([d.to_dict() for d in results.watchlists])[["name"]]
+    df["name"] = df["name"].apply(lambda x: f'"{x}"' if " " in x else x)
+    df["desc"] = ""
     return list(df.to_records(index=False))
 
 
-class MetricParamType(AutoCompleteChoice):
-    name = "metric"
+class UserWatchlistsParamType(AutoCompleteChoice):
+    name = "userwatchlists"
 
-    def get_suggestions(self, keyword: str, pre_populate: bool = True) -> List[Tuple[str, str]]:
+    def get_suggestions(self, keyword: str, pre_populate: bool = False) -> List[Tuple[str, str]]:
         if not self.is_loaded:
-            self.set_choices(get_metrics())
+            self.set_choices(get_user_watchlists())
 
         if pre_populate and keyword.strip() == "":
             return self._choices[: self.size]
 
         return self.search_keyword(keyword)
 
     def __repr__(self) -> str:
-        return "METRIC"
+        return "USERWATCHLISTS"
```

### Comparing `i8-terminal-0.2.84/i8_terminal/types/metric_view_param_type.py` & `i8-terminal-0.2.9/i8_terminal/types/period_type_param_type.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from typing import List, Tuple
 
-from i8_terminal.config import APP_SETTINGS
 from i8_terminal.types.auto_complete_choice import AutoCompleteChoice
 
 
-def get_metric_view_names() -> List[Tuple[str, str]]:
-    return [(view_name, "") for view_name in APP_SETTINGS["metric_view"]]
+def get_period_types() -> List[Tuple[str, str]]:
+    return [("Q", "Quarterly"), ("FY", "Anual"), ("TTM", "Trailing 12-month")]
 
 
-class MetricViewParamType(AutoCompleteChoice):
-    name = "metricview"
+class PeriodTypeParamType(AutoCompleteChoice):
+    name = "periodtype"
 
     def get_suggestions(self, keyword: str, pre_populate: bool = True) -> List[Tuple[str, str]]:
         if not self.is_loaded:
-            self.set_choices(get_metric_view_names())
+            self.set_choices(get_period_types())
 
         if pre_populate and keyword.strip() == "":
             return self._choices[: self.size]
         return self.search_keyword(keyword)
 
     def __repr__(self) -> str:
-        return "METRICVIEW"
+        return "PERIODTYPE"
```

### Comparing `i8-terminal-0.2.84/i8_terminal/types/ticker_param_type.py` & `i8-terminal-0.2.9/i8_terminal/types/ticker_param_type.py`

 * *Files identical despite different names*

### Comparing `i8-terminal-0.2.84/setup.py` & `i8-terminal-0.2.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List
 
 from setuptools import find_packages, setup
 
-from i8_terminal.utils_setup import get_version
+from i8_terminal.utils import get_version
 
 PACKAGE_NAME = "i8_terminal"
 
 
 def get_long_description() -> str:
     with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
```

