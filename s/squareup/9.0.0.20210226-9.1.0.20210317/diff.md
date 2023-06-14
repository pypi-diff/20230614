# Comparing `tmp/squareup-9.0.0.20210226.tar.gz` & `tmp/squareup-9.1.0.20210317.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/squareup-9.0.0.20210226.tar", last modified: Fri Feb 26 19:02:10 2021, max compression
+gzip compressed data, was "dist/squareup-9.1.0.20210317.tar", last modified: Wed Mar 17 21:59:34 2021, max compression
```

## Comparing `squareup-9.0.0.20210226.tar` & `squareup-9.1.0.20210317.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-26 19:02:10.731701 squareup-9.0.0.20210226/
--rw-r--r--   0 root         (0) root         (0)      550 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/LICENSE
--rw-r--r--   0 root         (0) root         (0)       34 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    19640 2021-02-26 19:02:10.731701 squareup-9.0.0.20210226/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    16009 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2021-02-26 19:02:10.731701 squareup-9.0.0.20210226/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1016 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-26 19:02:10.723701 squareup-9.0.0.20210226/square/
--rw-r--r--   0 root         (0) root         (0)      109 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-26 19:02:10.727701 squareup-9.0.0.20210226/square/api/
--rw-r--r--   0 root         (0) root         (0)      658 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2689 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/api/apple_pay_api.py
--rw-r--r--   0 root         (0) root         (0)     7100 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/api/bank_accounts_api.py
--rw-r--r--   0 root         (0) root         (0)     2659 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/api/base_api.py
--rw-r--r--   0 root         (0) root         (0)    15557 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/api/bookings_api.py
--rw-r--r--   0 root         (0) root         (0)     8101 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/api/cash_drawers_api.py
--rw-r--r--   0 root         (0) root         (0)    32627 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/api/catalog_api.py
--rw-r--r--   0 root         (0) root         (0)     2655 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/api/checkout_api.py
--rw-r--r--   0 root         (0) root         (0)     9840 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/api/customer_groups_api.py
--rw-r--r--   0 root         (0) root         (0)     4244 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/api/customer_segments_api.py
--rw-r--r--   0 root         (0) root         (0)    22286 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/api/customers_api.py
--rw-r--r--   0 root         (0) root         (0)     6694 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/api/devices_api.py
--rw-r--r--   0 root         (0) root         (0)    20282 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/api/disputes_api.py
--rw-r--r--   0 root         (0) root         (0)     4333 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/api/employees_api.py
--rw-r--r--   0 root         (0) root         (0)    16784 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/api/inventory_api.py
--rw-r--r--   0 root         (0) root         (0)    18697 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/api/invoices_api.py
--rw-r--r--   0 root         (0) root         (0)    32472 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/api/labor_api.py
--rw-r--r--   0 root         (0) root         (0)     7621 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/api/locations_api.py
--rw-r--r--   0 root         (0) root         (0)    27999 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/api/loyalty_api.py
--rw-r--r--   0 root         (0) root         (0)     4509 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/api/merchants_api.py
--rw-r--r--   0 root         (0) root         (0)     2735 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/api/mobile_authorization_api.py
--rw-r--r--   0 root         (0) root         (0)     8358 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/api/o_auth_api.py
--rw-r--r--   0 root         (0) root         (0)    16219 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/api/orders_api.py
--rw-r--r--   0 root         (0) root         (0)    14901 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/api/payments_api.py
--rw-r--r--   0 root         (0) root         (0)     8275 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/api/refunds_api.py
--rw-r--r--   0 root         (0) root         (0)    13727 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/api/subscriptions_api.py
--rw-r--r--   0 root         (0) root         (0)    17739 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/api/team_api.py
--rw-r--r--   0 root         (0) root         (0)    15018 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/api/terminal_api.py
--rw-r--r--   0 root         (0) root         (0)    20030 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/api/transactions_api.py
--rw-r--r--   0 root         (0) root         (0)    18679 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/api/v1_employees_api.py
--rw-r--r--   0 root         (0) root         (0)    27232 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/api/v1_transactions_api.py
--rw-r--r--   0 root         (0) root         (0)    13419 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/api_helper.py
--rw-r--r--   0 root         (0) root         (0)     5203 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/client.py
--rw-r--r--   0 root         (0) root         (0)     4452 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/configuration.py
--rw-r--r--   0 root         (0) root         (0)      381 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/decorators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-26 19:02:10.727701 squareup-9.0.0.20210226/square/exceptions/
--rw-r--r--   0 root         (0) root         (0)       35 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      751 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/exceptions/api_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-26 19:02:10.727701 squareup-9.0.0.20210226/square/http/
--rw-r--r--   0 root         (0) root         (0)      155 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1772 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/http/api_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-26 19:02:10.727701 squareup-9.0.0.20210226/square/http/auth/
--rw-r--r--   0 root         (0) root         (0)       30 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/http/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      534 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/http/auth/o_auth_2.py
--rw-r--r--   0 root         (0) root         (0)      987 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/http/http_call_back.py
--rw-r--r--   0 root         (0) root         (0)     6940 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/http/http_client.py
--rw-r--r--   0 root         (0) root         (0)      766 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/http/http_method_enum.py
--rw-r--r--   0 root         (0) root         (0)     2636 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/http/http_request.py
--rw-r--r--   0 root         (0) root         (0)     1349 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/http/http_response.py
--rw-r--r--   0 root         (0) root         (0)     3449 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/http/requests_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-26 19:02:10.727701 squareup-9.0.0.20210226/square/utilities/
--rw-r--r--   0 root         (0) root         (0)       37 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      418 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/square/utilities/file_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-26 19:02:10.727701 squareup-9.0.0.20210226/squareup.egg-info/
--rw-r--r--   0 root         (0) root         (0)    19640 2021-02-26 19:02:10.000000 squareup-9.0.0.20210226/squareup.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1988 2021-02-26 19:02:10.000000 squareup-9.0.0.20210226/squareup.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-02-26 19:02:10.000000 squareup-9.0.0.20210226/squareup.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      117 2021-02-26 19:02:10.000000 squareup-9.0.0.20210226/squareup.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2021-02-26 19:02:10.000000 squareup-9.0.0.20210226/squareup.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-26 19:02:10.727701 squareup-9.0.0.20210226/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-26 19:02:10.731701 squareup-9.0.0.20210226/tests/api/
--rw-r--r--   0 root         (0) root         (0)        0 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/tests/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      764 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/tests/api/api_test_base.py
--rw-r--r--   0 root         (0) root         (0)     2415 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/tests/api/test_catalog_api.py
--rw-r--r--   0 root         (0) root         (0)     1757 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/tests/api/test_customers_api.py
--rw-r--r--   0 root         (0) root         (0)     1304 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/tests/api/test_employees_api.py
--rw-r--r--   0 root         (0) root         (0)     2568 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/tests/api/test_labor_api.py
--rw-r--r--   0 root         (0) root         (0)     1078 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/tests/api/test_locations_api.py
--rw-r--r--   0 root         (0) root         (0)     1634 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/tests/api/test_merchants_api.py
--rw-r--r--   0 root         (0) root         (0)     1508 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/tests/api/test_payments_api.py
--rw-r--r--   0 root         (0) root         (0)     1484 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/tests/api/test_refunds_api.py
--rw-r--r--   0 root         (0) root         (0)     3175 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/tests/api/v2_endpoints_tests.py
--rw-r--r--   0 root         (0) root         (0)      525 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/tests/http_response_catcher.py
--rw-r--r--   0 root         (0) root         (0)     4887 2021-02-26 19:02:08.000000 squareup-9.0.0.20210226/tests/test_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-17 21:59:34.905271 squareup-9.1.0.20210317/
+-rw-r--r--   0 root         (0) root         (0)      550 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       34 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    19640 2021-03-17 21:59:34.905271 squareup-9.1.0.20210317/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    16009 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2021-03-17 21:59:34.905271 squareup-9.1.0.20210317/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1016 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-17 21:59:34.897271 squareup-9.1.0.20210317/square/
+-rw-r--r--   0 root         (0) root         (0)      109 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-17 21:59:34.901271 squareup-9.1.0.20210317/square/api/
+-rw-r--r--   0 root         (0) root         (0)      658 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2681 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/api/apple_pay_api.py
+-rw-r--r--   0 root         (0) root         (0)     7100 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/api/bank_accounts_api.py
+-rw-r--r--   0 root         (0) root         (0)     2659 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/api/base_api.py
+-rw-r--r--   0 root         (0) root         (0)    15557 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/api/bookings_api.py
+-rw-r--r--   0 root         (0) root         (0)     8101 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/api/cash_drawers_api.py
+-rw-r--r--   0 root         (0) root         (0)    32626 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/api/catalog_api.py
+-rw-r--r--   0 root         (0) root         (0)     2651 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/api/checkout_api.py
+-rw-r--r--   0 root         (0) root         (0)     9840 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/api/customer_groups_api.py
+-rw-r--r--   0 root         (0) root         (0)     4244 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/api/customer_segments_api.py
+-rw-r--r--   0 root         (0) root         (0)    22286 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/api/customers_api.py
+-rw-r--r--   0 root         (0) root         (0)     6694 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/api/devices_api.py
+-rw-r--r--   0 root         (0) root         (0)    20282 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/api/disputes_api.py
+-rw-r--r--   0 root         (0) root         (0)     4333 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/api/employees_api.py
+-rw-r--r--   0 root         (0) root         (0)    16784 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/api/inventory_api.py
+-rw-r--r--   0 root         (0) root         (0)    18697 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/api/invoices_api.py
+-rw-r--r--   0 root         (0) root         (0)    32472 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/api/labor_api.py
+-rw-r--r--   0 root         (0) root         (0)     7621 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/api/locations_api.py
+-rw-r--r--   0 root         (0) root         (0)    27999 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/api/loyalty_api.py
+-rw-r--r--   0 root         (0) root         (0)     4509 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/api/merchants_api.py
+-rw-r--r--   0 root         (0) root         (0)     2735 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/api/mobile_authorization_api.py
+-rw-r--r--   0 root         (0) root         (0)     8358 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/api/o_auth_api.py
+-rw-r--r--   0 root         (0) root         (0)    16219 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/api/orders_api.py
+-rw-r--r--   0 root         (0) root         (0)    16696 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/api/payments_api.py
+-rw-r--r--   0 root         (0) root         (0)     8527 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/api/refunds_api.py
+-rw-r--r--   0 root         (0) root         (0)    13727 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/api/subscriptions_api.py
+-rw-r--r--   0 root         (0) root         (0)    17739 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/api/team_api.py
+-rw-r--r--   0 root         (0) root         (0)    15044 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/api/terminal_api.py
+-rw-r--r--   0 root         (0) root         (0)    20030 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/api/transactions_api.py
+-rw-r--r--   0 root         (0) root         (0)    18679 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/api/v1_employees_api.py
+-rw-r--r--   0 root         (0) root         (0)    27232 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/api/v1_transactions_api.py
+-rw-r--r--   0 root         (0) root         (0)    13528 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/api_helper.py
+-rw-r--r--   0 root         (0) root         (0)     5203 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/client.py
+-rw-r--r--   0 root         (0) root         (0)     4452 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/configuration.py
+-rw-r--r--   0 root         (0) root         (0)      381 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/decorators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-17 21:59:34.901271 squareup-9.1.0.20210317/square/exceptions/
+-rw-r--r--   0 root         (0) root         (0)       35 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      751 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/exceptions/api_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-17 21:59:34.901271 squareup-9.1.0.20210317/square/http/
+-rw-r--r--   0 root         (0) root         (0)      155 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/http/api_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-17 21:59:34.901271 squareup-9.1.0.20210317/square/http/auth/
+-rw-r--r--   0 root         (0) root         (0)       30 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/http/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      534 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/http/auth/o_auth_2.py
+-rw-r--r--   0 root         (0) root         (0)      987 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/http/http_call_back.py
+-rw-r--r--   0 root         (0) root         (0)     6940 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/http/http_client.py
+-rw-r--r--   0 root         (0) root         (0)      766 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/http/http_method_enum.py
+-rw-r--r--   0 root         (0) root         (0)     2636 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/http/http_request.py
+-rw-r--r--   0 root         (0) root         (0)     1349 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/http/http_response.py
+-rw-r--r--   0 root         (0) root         (0)     3449 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/http/requests_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-17 21:59:34.901271 squareup-9.1.0.20210317/square/utilities/
+-rw-r--r--   0 root         (0) root         (0)       37 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      418 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/square/utilities/file_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-17 21:59:34.901271 squareup-9.1.0.20210317/squareup.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    19640 2021-03-17 21:59:34.000000 squareup-9.1.0.20210317/squareup.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1988 2021-03-17 21:59:34.000000 squareup-9.1.0.20210317/squareup.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-03-17 21:59:34.000000 squareup-9.1.0.20210317/squareup.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      117 2021-03-17 21:59:34.000000 squareup-9.1.0.20210317/squareup.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2021-03-17 21:59:34.000000 squareup-9.1.0.20210317/squareup.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-17 21:59:34.905271 squareup-9.1.0.20210317/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-17 21:59:34.905271 squareup-9.1.0.20210317/tests/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/tests/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      764 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/tests/api/api_test_base.py
+-rw-r--r--   0 root         (0) root         (0)     2415 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/tests/api/test_catalog_api.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/tests/api/test_customers_api.py
+-rw-r--r--   0 root         (0) root         (0)     1304 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/tests/api/test_employees_api.py
+-rw-r--r--   0 root         (0) root         (0)     2568 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/tests/api/test_labor_api.py
+-rw-r--r--   0 root         (0) root         (0)     1078 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/tests/api/test_locations_api.py
+-rw-r--r--   0 root         (0) root         (0)     1634 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/tests/api/test_merchants_api.py
+-rw-r--r--   0 root         (0) root         (0)     1508 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/tests/api/test_payments_api.py
+-rw-r--r--   0 root         (0) root         (0)     1484 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/tests/api/test_refunds_api.py
+-rw-r--r--   0 root         (0) root         (0)     3175 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/tests/api/v2_endpoints_tests.py
+-rw-r--r--   0 root         (0) root         (0)      525 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/tests/http_response_catcher.py
+-rw-r--r--   0 root         (0) root         (0)     4887 2021-03-17 21:59:33.000000 squareup-9.1.0.20210317/tests/test_helper.py
```

### Comparing `squareup-9.0.0.20210226/LICENSE` & `squareup-9.1.0.20210317/LICENSE`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/PKG-INFO` & `squareup-9.1.0.20210317/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squareup
-Version: 9.0.0.20210226
+Version: 9.1.0.20210317
 Summary: Use Square APIs to manage and run business including payment, customer, product, inventory, and employee management.
 Home-page: https://squareup.com/developers
 Author: Square Developer Platform
 Author-email: developers@squareup.com
 License: UNKNOWN
 Description: ![Square logo]
```

### Comparing `squareup-9.0.0.20210226/README.md` & `squareup-9.1.0.20210317/README.md`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/setup.py` & `squareup-9.1.0.20210317/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         long_description = fh.read()
 else:
     with open('README.md', 'r', encoding='utf-8') as fh:
         long_description = fh.read()
 
 setup(
     name='squareup',
-    version='9.0.0.20210226',
+    version='9.1.0.20210317',
     description='Use Square APIs to manage and run business including payment, customer, product, inventory, and employee management.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Square Developer Platform',
     author_email='developers@squareup.com',
     url='https://squareup.com/developers',
     packages=find_packages(),
```

### Comparing `squareup-9.0.0.20210226/square/api/__init__.py` & `squareup-9.1.0.20210317/square/api/__init__.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/square/api/apple_pay_api.py` & `squareup-9.1.0.20210317/square/api/apple_pay_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,26 +13,26 @@
     def __init__(self, config, call_back=None):
         super(ApplePayApi, self).__init__(config, call_back)
 
     def register_domain(self,
                         body):
         """Does a POST request to /v2/apple-pay/domains.
 
-        Activates a domain for use with Web Apple Pay and Square. A
+        Activates a domain for use with Apple Pay on the Web and Square. A
         validation
-        will be performed on this domain by Apple to ensure is it properly set
+        is performed on this domain by Apple to ensure that it is properly set
         up as
         an Apple Pay enabled domain.
         This endpoint provides an easy way for platform developers to bulk
         activate
-        Web Apple Pay with Square for merchants using their platform.
-        To learn more about Apple Pay on Web see the Apple Pay section in the
-        [Square Payment Form
-        Walkthrough](https://developer.squareup.com/docs/payment-form/payment-f
-        orm-walkthrough).
+        Apple Pay on the Web with Square for merchants using their platform.
+        To learn more about Web Apple Pay, see
+        [Add the Apple Pay on the Web
+        Button](https://developer.squareup.com/docs/payment-form/add-digital-wa
+        llets/apple-pay).
 
         Args:
             body (RegisterDomainRequest): An object containing the fields to
                 POST for the request.  See the corresponding object definition
                 for field details.
 
         Returns:
```

### Comparing `squareup-9.0.0.20210226/square/api/bank_accounts_api.py` & `squareup-9.1.0.20210317/square/api/bank_accounts_api.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/square/api/base_api.py` & `squareup-9.1.0.20210317/square/api/base_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         global_headers (dict): The global headers of the API which are sent with
             every request.
 
     """
 
     def global_headers(self):
         return {
-            'user-agent': 'Square-Python-SDK/9.0.0.20210226',
+            'user-agent': 'Square-Python-SDK/9.1.0.20210317',
             'Square-Version': self.config.square_version
         }
 
     def __init__(self, config, call_back=None):
         self._config = config
         self._http_call_back = call_back
```

### Comparing `squareup-9.0.0.20210226/square/api/bookings_api.py` & `squareup-9.1.0.20210317/square/api/bookings_api.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/square/api/cash_drawers_api.py` & `squareup-9.1.0.20210317/square/api/cash_drawers_api.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/square/api/catalog_api.py` & `squareup-9.1.0.20210317/square/api/catalog_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,15 +320,15 @@
         is specified as a comma-separated list of valid
         [CatalogObject](#type-catalogobject) types:
         `ITEM`, `ITEM_VARIATION`, `MODIFIER`, `MODIFIER_LIST`, `CATEGORY`,
         `DISCOUNT`, `TAX`, `IMAGE`.
         __Important:__ ListCatalog does not return deleted catalog items. To
         retrieve
         deleted catalog items, use
-        [SearchCatalogObjects](#endpoint-Catalog-SearchCatalogObjects) 
+        [SearchCatalogObjects](#endpoint-Catalog-SearchCatalogObjects)
         and set the `include_deleted_objects` attribute value to `true`.
 
         Args:
             cursor (string, optional): The pagination cursor returned in the
                 previous response. Leave unset for an initial request. See
                 [Pagination](https://developer.squareup.com/docs/basics/api101/
                 pagination) for more information.
```

### Comparing `squareup-9.0.0.20210226/square/api/checkout_api.py` & `squareup-9.1.0.20210317/square/api/checkout_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
         super(CheckoutApi, self).__init__(config, call_back)
 
     def create_checkout(self,
                         location_id,
                         body):
         """Does a POST request to /v2/locations/{location_id}/checkouts.
 
-        Links a `checkoutId` to a `checkout_page_url` that customers will
-        be directed to in order to provide their payment information using a
+        Links a `checkoutId` to a `checkout_page_url` that customers are
+        directed to in order to provide their payment information using a
         payment processing workflow hosted on connect.squareup.com.
 
         Args:
             location_id (string): The ID of the business location to associate
                 the checkout with.
             body (CreateCheckoutRequest): An object containing the fields to
                 POST for the request.  See the corresponding object definition
```

### Comparing `squareup-9.0.0.20210226/square/api/customer_groups_api.py` & `squareup-9.1.0.20210317/square/api/customer_groups_api.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/square/api/customer_segments_api.py` & `squareup-9.1.0.20210317/square/api/customer_segments_api.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/square/api/customers_api.py` & `squareup-9.1.0.20210317/square/api/customers_api.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/square/api/devices_api.py` & `squareup-9.1.0.20210317/square/api/devices_api.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/square/api/disputes_api.py` & `squareup-9.1.0.20210317/square/api/disputes_api.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/square/api/employees_api.py` & `squareup-9.1.0.20210317/square/api/employees_api.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/square/api/inventory_api.py` & `squareup-9.1.0.20210317/square/api/inventory_api.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/square/api/invoices_api.py` & `squareup-9.1.0.20210317/square/api/invoices_api.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/square/api/labor_api.py` & `squareup-9.1.0.20210317/square/api/labor_api.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/square/api/locations_api.py` & `squareup-9.1.0.20210317/square/api/locations_api.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/square/api/loyalty_api.py` & `squareup-9.1.0.20210317/square/api/loyalty_api.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/square/api/merchants_api.py` & `squareup-9.1.0.20210317/square/api/merchants_api.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/square/api/mobile_authorization_api.py` & `squareup-9.1.0.20210317/square/api/mobile_authorization_api.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/square/api/o_auth_api.py` & `squareup-9.1.0.20210317/square/api/o_auth_api.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/square/api/orders_api.py` & `squareup-9.1.0.20210317/square/api/orders_api.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/square/api/payments_api.py` & `squareup-9.1.0.20210317/square/api/payments_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,26 +111,22 @@
         _result = ApiResponse(_response, body=decoded, errors=_errors)
         return _result
 
     def create_payment(self,
                        body):
         """Does a POST request to /v2/payments.
 
-        Charges a payment source (for example, a card 
-        represented by customer's card on file or a card nonce). In addition 
-        to the payment source, the request must include the 
-        amount to accept for the payment.
-        There are several optional parameters that you can include in the
-        request 
-        (for example, tip money, whether to autocomplete the payment, or a
-        reference ID 
-        to correlate this payment with another system). 
-        The `PAYMENTS_WRITE_ADDITIONAL_RECIPIENTS` OAuth permission is
-        required
-        to enable application fees.
+        Creates a payment using the provided source. You can use this endpoint
+                to charge a card (credit/debit card or    
+        Square gift card) or record a payment that the seller received outside
+        of Square 
+        (cash payment from a buyer or a payment that an external entity 
+        procesed on behalf of the seller).
+        The endpoint creates a 
+        `Payment` object and returns it in the response.
 
         Args:
             body (CreatePaymentRequest): An object containing the fields to
                 POST for the request.  See the corresponding object definition
                 for field details.
 
         Returns:
@@ -184,15 +180,15 @@
         direct Square to cancel the payment using this endpoint. In the
         request, you provide the same
         idempotency key that you provided in your `CreatePayment` request that
         you want to cancel. After
         canceling the payment, you can submit your `CreatePayment` request
         again.
         Note that if no payment with the specified idempotency key is found,
-        no action is taken and the endpoint 
+        no action is taken and the endpoint
         returns successfully.
 
         Args:
             body (CancelPaymentByIdempotencyKeyRequest): An object containing
                 the fields to POST for the request.  See the corresponding
                 object definition for field details.
 
@@ -277,25 +273,79 @@
         if type(decoded) is dict:
             _errors = decoded.get('errors')
         else:
             _errors = None
         _result = ApiResponse(_response, body=decoded, errors=_errors)
         return _result
 
+    def update_payment(self,
+                       payment_id,
+                       body):
+        """Does a PUT request to /v2/payments/{payment_id}.
+
+        Updates a payment with the APPROVED status.
+        You can update the `amount_money` and `tip_money` using this
+        endpoint.
+
+        Args:
+            payment_id (string): The ID of the payment to update.
+            body (UpdatePaymentRequest): An object containing the fields to
+                POST for the request.  See the corresponding object definition
+                for field details.
+
+        Returns:
+            ApiResponse: An object with the response value as well as other
+                useful information such as status codes and headers. Success
+
+        Raises:
+            APIException: When an error occurs while fetching the data from
+                the remote API. This exception includes the HTTP Response
+                code, an error message, and the HTTP body that was received in
+                the request.
+
+        """
+
+        # Prepare query URL
+        _url_path = '/v2/payments/{payment_id}'
+        _url_path = APIHelper.append_url_with_template_parameters(_url_path, {
+            'payment_id': {'value': payment_id, 'encode': True}
+        })
+        _query_builder = self.config.get_base_uri()
+        _query_builder += _url_path
+        _query_url = APIHelper.clean_url(_query_builder)
+
+        # Prepare headers
+        _headers = {
+            'accept': 'application/json',
+            'content-type': 'application/json; charset=utf-8'
+        }
+
+        # Prepare and execute request
+        _request = self.config.http_client.put(_query_url, headers=_headers, parameters=APIHelper.json_serialize(body))
+        OAuth2.apply(self.config, _request)
+        _response = self.execute_request(_request)
+
+        decoded = APIHelper.json_deserialize(_response.text)
+        if type(decoded) is dict:
+            _errors = decoded.get('errors')
+        else:
+            _errors = None
+        _result = ApiResponse(_response, body=decoded, errors=_errors)
+        return _result
+
     def cancel_payment(self,
                        payment_id):
         """Does a POST request to /v2/payments/{payment_id}/cancel.
 
-        Cancels (voids) a payment. If you set `autocomplete` to `false` when
-        creating a payment, 
-        you can cancel the payment using this endpoint.
+        Cancels (voids) a payment. You can use this endpoint to cancel a
+        payment with 
+        the APPROVED `status`.
 
         Args:
-            payment_id (string): The `payment_id` identifying the payment to
-                be canceled.
+            payment_id (string): The ID of the payment to cancel.
 
         Returns:
             ApiResponse: An object with the response value as well as other
                 useful information such as status codes and headers. Success
 
         Raises:
             APIException: When an error occurs while fetching the data from
@@ -334,18 +384,17 @@
 
     def complete_payment(self,
                          payment_id):
         """Does a POST request to /v2/payments/{payment_id}/complete.
 
         Completes (captures) a payment.
         By default, payments are set to complete immediately after they are
-        created. 
-        If you set `autocomplete` to `false` when creating a payment, you can
-        complete (capture) 
-        the payment using this endpoint.
+        created.
+        You can use this endpoint to complete a payment with the APPROVED
+        `status`.
 
         Args:
             payment_id (string): The unique ID identifying the payment to be
                 completed.
 
         Returns:
             ApiResponse: An object with the response value as well as other
```

### Comparing `squareup-9.0.0.20210226/square/api/refunds_api.py` & `squareup-9.1.0.20210317/square/api/refunds_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -111,16 +111,21 @@
         _result = ApiResponse(_response, body=decoded, errors=_errors)
         return _result
 
     def refund_payment(self,
                        body):
         """Does a POST request to /v2/refunds.
 
-        Refunds a payment. You can refund the entire payment amount or a 
-        portion of it.
+        Refunds a payment. You can refund the entire payment amount or a
+        portion of it. You can use this endpoint to refund a card payment or
+        record a 
+        refund of a cash or external payment. For more information, see
+        [Refund
+        Payment](https://developer.squareup.com/docs/payments-api/refund-paymen
+        ts).
 
         Args:
             body (RefundPaymentRequest): An object containing the fields to
                 POST for the request.  See the corresponding object definition
                 for field details.
 
         Returns:
```

### Comparing `squareup-9.0.0.20210226/square/api/subscriptions_api.py` & `squareup-9.1.0.20210317/square/api/subscriptions_api.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/square/api/team_api.py` & `squareup-9.1.0.20210317/square/api/team_api.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/square/api/terminal_api.py` & `squareup-9.1.0.20210317/square/api/terminal_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,17 @@
     def __init__(self, config, call_back=None):
         super(TerminalApi, self).__init__(config, call_back)
 
     def create_terminal_checkout(self,
                                  body):
         """Does a POST request to /v2/terminals/checkouts.
 
-        Creates a new Terminal checkout request and sends it to the specified
-        device to take a payment for the requested amount.
+        Creates a Terminal checkout request and sends it to the specified
+        device to take a payment
+        for the requested amount.
 
         Args:
             body (CreateTerminalCheckoutRequest): An object containing the
                 fields to POST for the request.  See the corresponding object
                 definition for field details.
 
         Returns:
@@ -111,19 +112,19 @@
         _result = ApiResponse(_response, body=decoded, errors=_errors)
         return _result
 
     def get_terminal_checkout(self,
                               checkout_id):
         """Does a GET request to /v2/terminals/checkouts/{checkout_id}.
 
-        Retrieves a Terminal checkout request by checkout_id.
+        Retrieves a Terminal checkout request by `checkout_id`.
 
         Args:
-            checkout_id (string): Unique ID for the desired
-                `TerminalCheckout`
+            checkout_id (string): The unique ID for the desired
+                `TerminalCheckout`.
 
         Returns:
             ApiResponse: An object with the response value as well as other
                 useful information such as status codes and headers. Success
 
         Raises:
             APIException: When an error occurs while fetching the data from
@@ -164,16 +165,16 @@
                                  checkout_id):
         """Does a POST request to /v2/terminals/checkouts/{checkout_id}/cancel.
 
         Cancels a Terminal checkout request if the status of the request
         permits it.
 
         Args:
-            checkout_id (string): Unique ID for the desired
-                `TerminalCheckout`
+            checkout_id (string): The unique ID for the desired
+                `TerminalCheckout`.
 
         Returns:
             ApiResponse: An object with the response value as well as other
                 useful information such as status codes and headers. Success
 
         Raises:
             APIException: When an error occurs while fetching the data from
@@ -259,15 +260,15 @@
         _result = ApiResponse(_response, body=decoded, errors=_errors)
         return _result
 
     def search_terminal_refunds(self,
                                 body):
         """Does a POST request to /v2/terminals/refunds/search.
 
-        Retrieves a filtered list of Terminal Interac refund requests created
+        Retrieves a filtered list of Interac Terminal refund requests created
         by the seller making the request.
 
         Args:
             body (SearchTerminalRefundsRequest): An object containing the
                 fields to POST for the request.  See the corresponding object
                 definition for field details.
 
@@ -308,19 +309,19 @@
         _result = ApiResponse(_response, body=decoded, errors=_errors)
         return _result
 
     def get_terminal_refund(self,
                             terminal_refund_id):
         """Does a GET request to /v2/terminals/refunds/{terminal_refund_id}.
 
-        Retrieves an Interac terminal refund object by ID.
+        Retrieves an Interac Terminal refund object by ID.
 
         Args:
-            terminal_refund_id (string): Unique ID for the desired
-                `TerminalRefund`
+            terminal_refund_id (string): The unique ID for the desired
+                `TerminalRefund`.
 
         Returns:
             ApiResponse: An object with the response value as well as other
                 useful information such as status codes and headers. Success
 
         Raises:
             APIException: When an error occurs while fetching the data from
@@ -357,20 +358,20 @@
         _result = ApiResponse(_response, body=decoded, errors=_errors)
         return _result
 
     def cancel_terminal_refund(self,
                                terminal_refund_id):
         """Does a POST request to /v2/terminals/refunds/{terminal_refund_id}/cancel.
 
-        Cancels an Interac terminal refund request by refund request ID if the
+        Cancels an Interac Terminal refund request by refund request ID if the
         status of the request permits it.
 
         Args:
-            terminal_refund_id (string): Unique ID for the desired
-                `TerminalRefund`
+            terminal_refund_id (string): The unique ID for the desired
+                `TerminalRefund`.
 
         Returns:
             ApiResponse: An object with the response value as well as other
                 useful information such as status codes and headers. Success
 
         Raises:
             APIException: When an error occurs while fetching the data from
```

### Comparing `squareup-9.0.0.20210226/square/api/transactions_api.py` & `squareup-9.1.0.20210317/square/api/transactions_api.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/square/api/v1_employees_api.py` & `squareup-9.1.0.20210317/square/api/v1_employees_api.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/square/api/v1_transactions_api.py` & `squareup-9.1.0.20210317/square/api/v1_transactions_api.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/square/api_helper.py` & `squareup-9.1.0.20210317/square/api_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         else:
             if hasattr(obj, "_names"):
                 obj = APIHelper.to_dictionary(obj)
 
         return jsonpickle.encode(obj, False)
 
     @staticmethod
-    def json_deserialize(json, unboxing_function=None):
+    def json_deserialize(json, unboxing_function=None, as_dict=False):
         """JSON Deserialization of a given string.
 
         Args:
             json (str): The JSON serialized string to deserialize.
 
         Returns:
             dict: A dictionary representing the data contained in the
@@ -89,14 +89,17 @@
         try:
             decoded = jsonpickle.decode(json)
         except ValueError:
             return json
 
         if unboxing_function is None:
             return decoded
+
+        if as_dict:
+            return {k: unboxing_function(v) for k, v in decoded.items()}
         elif isinstance(decoded, list):
             return [unboxing_function(element) for element in decoded]
         else:
             return unboxing_function(decoded)
 
     @staticmethod
     def serialize_array(key, array, formatting="indexed"):
```

### Comparing `squareup-9.0.0.20210226/square/client.py` & `squareup-9.1.0.20210317/square/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,19 +33,19 @@
 from square.api.terminal_api import TerminalApi
 
 
 class Client(object):
 
     @staticmethod
     def sdk_version():
-        return '9.0.0.20210226'
+        return '9.1.0.20210317'
 
     @staticmethod
     def square_version():
-        return '2021-02-26'
+        return '2021-03-17'
 
     @lazy_property
     def mobile_authorization(self):
         return MobileAuthorizationApi(self.config)
 
     @lazy_property
     def o_auth(self):
@@ -158,15 +158,15 @@
     @lazy_property
     def terminal(self):
         return TerminalApi(self.config)
 
     def __init__(self, timeout=60, max_retries=3, backoff_factor=0,
                  environment='production',
                  custom_url='https://connect.squareup.com',
-                 square_version='2021-02-26', access_token='TODO: Replace',
+                 square_version='2021-03-17', access_token='TODO: Replace',
                  additional_headers={}, config=None):
         if config is None:
             self.config = Configuration(timeout=timeout,
                                         max_retries=max_retries,
                                         backoff_factor=backoff_factor,
                                         environment=environment,
                                         custom_url=custom_url,
```

### Comparing `squareup-9.0.0.20210226/square/configuration.py` & `squareup-9.1.0.20210317/square/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     @property
     def additional_headers(self):
         return deepcopy(self._additional_headers)
 
     def __init__(self, timeout=60, max_retries=3, backoff_factor=0,
                  environment='production',
                  custom_url='https://connect.squareup.com',
-                 square_version='2021-02-26', access_token='TODO: Replace',
+                 square_version='2021-03-17', access_token='TODO: Replace',
                  additional_headers={}):
         # The value to use for connection timeout
         self._timeout = timeout
 
         # The number of times to retry an endpoint call if it fails
         self._max_retries = max_retries
```

### Comparing `squareup-9.0.0.20210226/square/exceptions/api_exception.py` & `squareup-9.1.0.20210317/square/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/square/http/api_response.py` & `squareup-9.1.0.20210317/square/http/api_response.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/square/http/auth/o_auth_2.py` & `squareup-9.1.0.20210317/square/http/auth/o_auth_2.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/square/http/http_call_back.py` & `squareup-9.1.0.20210317/square/http/http_call_back.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/square/http/http_client.py` & `squareup-9.1.0.20210317/square/http/http_client.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/square/http/http_method_enum.py` & `squareup-9.1.0.20210317/square/http/http_method_enum.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/square/http/http_request.py` & `squareup-9.1.0.20210317/square/http/http_request.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/square/http/http_response.py` & `squareup-9.1.0.20210317/square/http/http_response.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/square/http/requests_client.py` & `squareup-9.1.0.20210317/square/http/requests_client.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/squareup.egg-info/PKG-INFO` & `squareup-9.1.0.20210317/squareup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squareup
-Version: 9.0.0.20210226
+Version: 9.1.0.20210317
 Summary: Use Square APIs to manage and run business including payment, customer, product, inventory, and employee management.
 Home-page: https://squareup.com/developers
 Author: Square Developer Platform
 Author-email: developers@squareup.com
 License: UNKNOWN
 Description: ![Square logo]
```

### Comparing `squareup-9.0.0.20210226/squareup.egg-info/SOURCES.txt` & `squareup-9.1.0.20210317/squareup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/tests/api/api_test_base.py` & `squareup-9.1.0.20210317/tests/api/api_test_base.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/tests/api/test_catalog_api.py` & `squareup-9.1.0.20210317/tests/api/test_catalog_api.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/tests/api/test_customers_api.py` & `squareup-9.1.0.20210317/tests/api/test_customers_api.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/tests/api/test_employees_api.py` & `squareup-9.1.0.20210317/tests/api/test_employees_api.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/tests/api/test_labor_api.py` & `squareup-9.1.0.20210317/tests/api/test_labor_api.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/tests/api/test_locations_api.py` & `squareup-9.1.0.20210317/tests/api/test_locations_api.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/tests/api/test_merchants_api.py` & `squareup-9.1.0.20210317/tests/api/test_merchants_api.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/tests/api/test_payments_api.py` & `squareup-9.1.0.20210317/tests/api/test_payments_api.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/tests/api/test_refunds_api.py` & `squareup-9.1.0.20210317/tests/api/test_refunds_api.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/tests/api/v2_endpoints_tests.py` & `squareup-9.1.0.20210317/tests/api/v2_endpoints_tests.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/tests/http_response_catcher.py` & `squareup-9.1.0.20210317/tests/http_response_catcher.py`

 * *Files identical despite different names*

### Comparing `squareup-9.0.0.20210226/tests/test_helper.py` & `squareup-9.1.0.20210317/tests/test_helper.py`

 * *Files identical despite different names*

