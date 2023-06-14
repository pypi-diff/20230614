# Comparing `tmp/py-algorand-sdk-2.2.0.tar.gz` & `tmp/py-algorand-sdk-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-algorand-sdk-2.2.0.tar", last modified: Mon May  8 14:09:50 2023, max compression
+gzip compressed data, was "py-algorand-sdk-2.3.0.tar", last modified: Wed Jun 14 18:51:17 2023, max compression
```

## Comparing `py-algorand-sdk-2.2.0.tar` & `py-algorand-sdk-2.3.0.tar`

### file list

```diff
@@ -1,90 +1,74 @@
-drwxr-xr-x   0 barbara    (502) staff       (20)        0 2023-05-08 14:09:50.463777 py-algorand-sdk-2.2.0/
--rw-r--r--   0 barbara    (502) staff       (20)     1065 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/LICENSE
--rw-r--r--   0 barbara    (502) staff       (20)       44 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/MANIFEST.in
--rw-r--r--   0 barbara    (502) staff       (20)     4289 2023-05-08 14:09:50.463379 py-algorand-sdk-2.2.0/PKG-INFO
--rw-r--r--   0 barbara    (502) staff       (20)     3923 2023-03-14 19:29:33.000000 py-algorand-sdk-2.2.0/README.md
-drwxr-xr-x   0 barbara    (502) staff       (20)        0 2023-05-08 14:09:50.422193 py-algorand-sdk-2.2.0/algosdk/
--rw-r--r--   0 barbara    (502) staff       (20)      745 2023-03-14 19:29:33.000000 py-algorand-sdk-2.2.0/algosdk/__init__.py
--rw-r--r--   0 barbara    (502) staff       (20)     1115 2023-03-14 19:29:33.000000 py-algorand-sdk-2.2.0/algosdk/__init__.pyi
-drwxr-xr-x   0 barbara    (502) staff       (20)        0 2023-05-08 14:09:50.432890 py-algorand-sdk-2.2.0/algosdk/abi/
--rw-r--r--   0 barbara    (502) staff       (20)     1284 2023-03-14 19:29:33.000000 py-algorand-sdk-2.2.0/algosdk/abi/__init__.py
--rw-r--r--   0 barbara    (502) staff       (20)     2711 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/algosdk/abi/address_type.py
--rw-r--r--   0 barbara    (502) staff       (20)     3243 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/algosdk/abi/array_dynamic_type.py
--rw-r--r--   0 barbara    (502) staff       (20)     3675 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/algosdk/abi/array_static_type.py
--rw-r--r--   0 barbara    (502) staff       (20)     4709 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/algosdk/abi/base_type.py
--rw-r--r--   0 barbara    (502) staff       (20)     1936 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/algosdk/abi/bool_type.py
--rw-r--r--   0 barbara    (502) staff       (20)     1651 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/algosdk/abi/byte_type.py
--rw-r--r--   0 barbara    (502) staff       (20)     3072 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/algosdk/abi/contract.py
--rw-r--r--   0 barbara    (502) staff       (20)     1845 2023-03-14 19:29:33.000000 py-algorand-sdk-2.2.0/algosdk/abi/interface.py
--rw-r--r--   0 barbara    (502) staff       (20)     7715 2023-03-14 19:29:33.000000 py-algorand-sdk-2.2.0/algosdk/abi/method.py
--rw-r--r--   0 barbara    (502) staff       (20)      389 2022-01-14 15:35:40.000000 py-algorand-sdk-2.2.0/algosdk/abi/reference.py
--rw-r--r--   0 barbara    (502) staff       (20)     2251 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/algosdk/abi/string_type.py
--rw-r--r--   0 barbara    (502) staff       (20)     1076 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/algosdk/abi/transaction.py
--rw-r--r--   0 barbara    (502) staff       (20)    12075 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/algosdk/abi/tuple_type.py
--rw-r--r--   0 barbara    (502) staff       (20)     3165 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/algosdk/abi/ufixed_type.py
--rw-r--r--   0 barbara    (502) staff       (20)     2510 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/algosdk/abi/uint_type.py
--rw-r--r--   0 barbara    (502) staff       (20)      767 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/algosdk/account.py
--rw-r--r--   0 barbara    (502) staff       (20)    36921 2023-05-08 14:08:12.000000 py-algorand-sdk-2.2.0/algosdk/atomic_transaction_composer.py
--rw-r--r--   0 barbara    (502) staff       (20)     4291 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/algosdk/auction.py
--rw-r--r--   0 barbara    (502) staff       (20)     3289 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/algosdk/box_reference.py
--rw-r--r--   0 barbara    (502) staff       (20)     4705 2023-05-08 14:08:12.000000 py-algorand-sdk-2.2.0/algosdk/constants.py
--rw-r--r--   0 barbara    (502) staff       (20)     6981 2023-03-14 19:29:33.000000 py-algorand-sdk-2.2.0/algosdk/dryrun_results.py
--rw-r--r--   0 barbara    (502) staff       (20)     5880 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/algosdk/encoding.py
--rw-r--r--   0 barbara    (502) staff       (20)     5623 2023-03-14 19:29:33.000000 py-algorand-sdk-2.2.0/algosdk/error.py
--rw-r--r--   0 barbara    (502) staff       (20)    13562 2023-05-08 14:08:12.000000 py-algorand-sdk-2.2.0/algosdk/kmd.py
--rw-r--r--   0 barbara    (502) staff       (20)     2061 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/algosdk/logic.py
--rw-r--r--   0 barbara    (502) staff       (20)     5033 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/algosdk/mnemonic.py
--rw-r--r--   0 barbara    (502) staff       (20)        0 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/algosdk/py.typed
--rw-r--r--   0 barbara    (502) staff       (20)     2803 2023-03-14 19:29:33.000000 py-algorand-sdk-2.2.0/algosdk/source_map.py
-drwxr-xr-x   0 barbara    (502) staff       (20)        0 2023-05-08 14:09:50.433963 py-algorand-sdk-2.2.0/algosdk/testing/
--rw-r--r--   0 barbara    (502) staff       (20)        0 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/algosdk/testing/__init__.py
--rw-r--r--   0 barbara    (502) staff       (20)    27818 2023-03-14 19:29:33.000000 py-algorand-sdk-2.2.0/algosdk/testing/dryrun.py
--rw-r--r--   0 barbara    (502) staff       (20)   109053 2023-05-08 14:08:12.000000 py-algorand-sdk-2.2.0/algosdk/transaction.py
--rw-r--r--   0 barbara    (502) staff       (20)     2543 2022-08-18 18:15:50.000000 py-algorand-sdk-2.2.0/algosdk/util.py
-drwxr-xr-x   0 barbara    (502) staff       (20)        0 2023-05-08 14:09:50.436761 py-algorand-sdk-2.2.0/algosdk/v2client/
--rw-r--r--   0 barbara    (502) staff       (20)       93 2023-03-14 19:29:33.000000 py-algorand-sdk-2.2.0/algosdk/v2client/__init__.py
--rw-r--r--   0 barbara    (502) staff       (20)    24540 2023-05-08 14:08:12.000000 py-algorand-sdk-2.2.0/algosdk/v2client/algod.py
--rw-r--r--   0 barbara    (502) staff       (20)    36632 2023-03-14 19:29:33.000000 py-algorand-sdk-2.2.0/algosdk/v2client/indexer.py
-drwxr-xr-x   0 barbara    (502) staff       (20)        0 2023-05-08 14:09:50.448548 py-algorand-sdk-2.2.0/algosdk/v2client/models/
--rw-r--r--   0 barbara    (502) staff       (20)     1612 2023-05-08 14:08:12.000000 py-algorand-sdk-2.2.0/algosdk/v2client/models/__init__.py
--rw-r--r--   0 barbara    (502) staff       (20)    17792 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/algosdk/v2client/models/account.py
--rw-r--r--   0 barbara    (502) staff       (20)     8562 2022-02-15 21:52:01.000000 py-algorand-sdk-2.2.0/algosdk/v2client/models/account_participation.py
--rw-r--r--   0 barbara    (502) staff       (20)     3301 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/algosdk/v2client/models/application.py
--rw-r--r--   0 barbara    (502) staff       (20)     4367 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/algosdk/v2client/models/application_local_state.py
--rw-r--r--   0 barbara    (502) staff       (20)     7927 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/algosdk/v2client/models/application_params.py
--rw-r--r--   0 barbara    (502) staff       (20)     3782 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/algosdk/v2client/models/application_state_schema.py
--rw-r--r--   0 barbara    (502) staff       (20)     3255 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/algosdk/v2client/models/asset.py
--rw-r--r--   0 barbara    (502) staff       (20)     5346 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/algosdk/v2client/models/asset_holding.py
--rw-r--r--   0 barbara    (502) staff       (20)    12993 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/algosdk/v2client/models/asset_params.py
--rw-r--r--   0 barbara    (502) staff       (20)     7734 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/algosdk/v2client/models/dryrun_request.py
--rw-r--r--   0 barbara    (502) staff       (20)     5163 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/algosdk/v2client/models/dryrun_source.py
--rw-r--r--   0 barbara    (502) staff       (20)     1238 2023-05-08 14:08:12.000000 py-algorand-sdk-2.2.0/algosdk/v2client/models/simulate_request.py
--rw-r--r--   0 barbara    (502) staff       (20)     3181 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/algosdk/v2client/models/teal_key_value.py
--rw-r--r--   0 barbara    (502) staff       (20)     3928 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/algosdk/v2client/models/teal_value.py
--rw-r--r--   0 barbara    (502) staff       (20)     7486 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/algosdk/wallet.py
--rw-r--r--   0 barbara    (502) staff       (20)    13267 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/algosdk/wordlist.py
-drwxr-xr-x   0 barbara    (502) staff       (20)        0 2023-05-08 14:09:50.452674 py-algorand-sdk-2.2.0/py_algorand_sdk.egg-info/
--rw-r--r--   0 barbara    (502) staff       (20)     4289 2023-05-08 14:09:50.000000 py-algorand-sdk-2.2.0/py_algorand_sdk.egg-info/PKG-INFO
--rw-r--r--   0 barbara    (502) staff       (20)     2204 2023-05-08 14:09:50.000000 py-algorand-sdk-2.2.0/py_algorand_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 barbara    (502) staff       (20)        1 2023-05-08 14:09:50.000000 py-algorand-sdk-2.2.0/py_algorand_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 barbara    (502) staff       (20)       59 2023-05-08 14:09:50.000000 py-algorand-sdk-2.2.0/py_algorand_sdk.egg-info/requires.txt
--rw-r--r--   0 barbara    (502) staff       (20)        8 2023-05-08 14:09:50.000000 py-algorand-sdk-2.2.0/py_algorand_sdk.egg-info/top_level.txt
--rw-r--r--   0 barbara    (502) staff       (20)       30 2021-09-22 13:48:08.000000 py-algorand-sdk-2.2.0/pyproject.toml
--rw-r--r--   0 barbara    (502) staff       (20)       38 2023-05-08 14:09:50.463880 py-algorand-sdk-2.2.0/setup.cfg
--rw-r--r--   0 barbara    (502) staff       (20)      871 2023-05-08 14:08:22.000000 py-algorand-sdk-2.2.0/setup.py
-drwxr-xr-x   0 barbara    (502) staff       (20)        0 2023-05-08 14:09:50.453833 py-algorand-sdk-2.2.0/tests/
--rw-r--r--   0 barbara    (502) staff       (20)        0 2022-08-18 18:15:50.000000 py-algorand-sdk-2.2.0/tests/__init__.py
--rw-r--r--   0 barbara    (502) staff       (20)     4770 2023-05-08 14:08:12.000000 py-algorand-sdk-2.2.0/tests/environment.py
-drwxr-xr-x   0 barbara    (502) staff       (20)        0 2023-05-08 14:09:50.457853 py-algorand-sdk-2.2.0/tests/steps/
--rw-r--r--   0 barbara    (502) staff       (20)        0 2022-08-18 18:15:50.000000 py-algorand-sdk-2.2.0/tests/steps/__init__.py
--rw-r--r--   0 barbara    (502) staff       (20)     9561 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/tests/steps/account_v2_steps.py
--rw-r--r--   0 barbara    (502) staff       (20)    44018 2023-05-05 20:18:25.000000 py-algorand-sdk-2.2.0/tests/steps/application_v2_steps.py
--rw-r--r--   0 barbara    (502) staff       (20)    49356 2023-05-08 14:08:12.000000 py-algorand-sdk-2.2.0/tests/steps/other_v2_steps.py
--rw-r--r--   0 barbara    (502) staff       (20)    26804 2023-05-08 14:08:12.000000 py-algorand-sdk-2.2.0/tests/steps/steps.py
-drwxr-xr-x   0 barbara    (502) staff       (20)        0 2023-05-08 14:09:50.462402 py-algorand-sdk-2.2.0/tests/unit_tests/
--rw-r--r--   0 barbara    (502) staff       (20)        0 2022-08-18 18:15:50.000000 py-algorand-sdk-2.2.0/tests/unit_tests/__init__.py
--rw-r--r--   0 barbara    (502) staff       (20)    26719 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/tests/unit_tests/test_abi.py
--rw-r--r--   0 barbara    (502) staff       (20)    19987 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/tests/unit_tests/test_dryrun.py
--rw-r--r--   0 barbara    (502) staff       (20)    40826 2023-03-14 19:29:33.000000 py-algorand-sdk-2.2.0/tests/unit_tests/test_logicsig.py
--rw-r--r--   0 barbara    (502) staff       (20)    30241 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/tests/unit_tests/test_other.py
--rw-r--r--   0 barbara    (502) staff       (20)    59966 2023-03-14 18:07:29.000000 py-algorand-sdk-2.2.0/tests/unit_tests/test_transaction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 18:51:17.544038 py-algorand-sdk-2.3.0/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       44 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4728 2023-06-14 18:51:17.544038 py-algorand-sdk-2.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4342 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 18:51:17.540038 py-algorand-sdk-2.3.0/algosdk/
+-rw-r--r--   0 root         (0) root         (0)      745 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1115 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 18:51:17.544038 py-algorand-sdk-2.3.0/algosdk/abi/
+-rw-r--r--   0 root         (0) root         (0)     1284 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/abi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2711 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/abi/address_type.py
+-rw-r--r--   0 root         (0) root         (0)     3243 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/abi/array_dynamic_type.py
+-rw-r--r--   0 root         (0) root         (0)     3675 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/abi/array_static_type.py
+-rw-r--r--   0 root         (0) root         (0)     4709 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/abi/base_type.py
+-rw-r--r--   0 root         (0) root         (0)     1936 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/abi/bool_type.py
+-rw-r--r--   0 root         (0) root         (0)     1651 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/abi/byte_type.py
+-rw-r--r--   0 root         (0) root         (0)     3072 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/abi/contract.py
+-rw-r--r--   0 root         (0) root         (0)     1845 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/abi/interface.py
+-rw-r--r--   0 root         (0) root         (0)     7715 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/abi/method.py
+-rw-r--r--   0 root         (0) root         (0)      389 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/abi/reference.py
+-rw-r--r--   0 root         (0) root         (0)     2251 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/abi/string_type.py
+-rw-r--r--   0 root         (0) root         (0)     1076 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/abi/transaction.py
+-rw-r--r--   0 root         (0) root         (0)    12075 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/abi/tuple_type.py
+-rw-r--r--   0 root         (0) root         (0)     3165 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/abi/ufixed_type.py
+-rw-r--r--   0 root         (0) root         (0)     2510 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/abi/uint_type.py
+-rw-r--r--   0 root         (0) root         (0)      767 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/account.py
+-rw-r--r--   0 root         (0) root         (0)    37203 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/atomic_transaction_composer.py
+-rw-r--r--   0 root         (0) root         (0)     4291 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/auction.py
+-rw-r--r--   0 root         (0) root         (0)     3289 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/box_reference.py
+-rw-r--r--   0 root         (0) root         (0)     4705 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/constants.py
+-rw-r--r--   0 root         (0) root         (0)     6981 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/dryrun_results.py
+-rw-r--r--   0 root         (0) root         (0)     5880 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/encoding.py
+-rw-r--r--   0 root         (0) root         (0)     5623 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/error.py
+-rw-r--r--   0 root         (0) root         (0)    13562 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/kmd.py
+-rw-r--r--   0 root         (0) root         (0)     2061 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/logic.py
+-rw-r--r--   0 root         (0) root         (0)     5033 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/mnemonic.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/py.typed
+-rw-r--r--   0 root         (0) root         (0)     2803 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/source_map.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 18:51:17.544038 py-algorand-sdk-2.3.0/algosdk/testing/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/testing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27818 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/testing/dryrun.py
+-rw-r--r--   0 root         (0) root         (0)   109051 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/transaction.py
+-rw-r--r--   0 root         (0) root         (0)     2543 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 18:51:17.544038 py-algorand-sdk-2.3.0/algosdk/v2client/
+-rw-r--r--   0 root         (0) root         (0)       93 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/v2client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26714 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/v2client/algod.py
+-rw-r--r--   0 root         (0) root         (0)    37764 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/v2client/indexer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 18:51:17.544038 py-algorand-sdk-2.3.0/algosdk/v2client/models/
+-rw-r--r--   0 root         (0) root         (0)     1612 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/v2client/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17792 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/v2client/models/account.py
+-rw-r--r--   0 root         (0) root         (0)     8562 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/v2client/models/account_participation.py
+-rw-r--r--   0 root         (0) root         (0)     3301 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/v2client/models/application.py
+-rw-r--r--   0 root         (0) root         (0)     4367 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/v2client/models/application_local_state.py
+-rw-r--r--   0 root         (0) root         (0)     7927 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/v2client/models/application_params.py
+-rw-r--r--   0 root         (0) root         (0)     3782 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/v2client/models/application_state_schema.py
+-rw-r--r--   0 root         (0) root         (0)     3255 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/v2client/models/asset.py
+-rw-r--r--   0 root         (0) root         (0)     5346 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/v2client/models/asset_holding.py
+-rw-r--r--   0 root         (0) root         (0)    12993 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/v2client/models/asset_params.py
+-rw-r--r--   0 root         (0) root         (0)     7734 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/v2client/models/dryrun_request.py
+-rw-r--r--   0 root         (0) root         (0)     5163 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/v2client/models/dryrun_source.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/v2client/models/simulate_request.py
+-rw-r--r--   0 root         (0) root         (0)     3181 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/v2client/models/teal_key_value.py
+-rw-r--r--   0 root         (0) root         (0)     3928 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/v2client/models/teal_value.py
+-rw-r--r--   0 root         (0) root         (0)     7486 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/wallet.py
+-rw-r--r--   0 root         (0) root         (0)    13267 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/algosdk/wordlist.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 18:51:17.544038 py-algorand-sdk-2.3.0/py_algorand_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4728 2023-06-14 18:51:17.000000 py-algorand-sdk-2.3.0/py_algorand_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1830 2023-06-14 18:51:17.000000 py-algorand-sdk-2.3.0/py_algorand_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 18:51:17.000000 py-algorand-sdk-2.3.0/py_algorand_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-06-14 18:51:17.000000 py-algorand-sdk-2.3.0/py_algorand_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-14 18:51:17.000000 py-algorand-sdk-2.3.0/py_algorand_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-14 18:51:04.000000 py-algorand-sdk-2.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 18:51:17.544038 py-algorand-sdk-2.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      871 2023-06-14 18:51:08.000000 py-algorand-sdk-2.3.0/setup.py
```

### Comparing `py-algorand-sdk-2.2.0/LICENSE` & `py-algorand-sdk-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/PKG-INFO` & `py-algorand-sdk-2.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: py-algorand-sdk
-Version: 2.2.0
+Version: 2.3.0
 Summary: Algorand SDK in Python
 Home-page: https://github.com/algorand/py-algorand-sdk
 Author: Algorand
 Author-email: pypiservice@algorand.com
 License: MIT
 Project-URL: Source, https://github.com/algorand/py-algorand-sdk
+Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # py-algorand-sdk
 
 [![PyPI version](https://badge.fury.io/py/py-algorand-sdk.svg)](https://badge.fury.io/py/py-algorand-sdk)
@@ -70,14 +71,16 @@
 
 * `make lint`
 
 Run non-test-harness related unit tests
 
 * `make pytest-unit`
 
+We use cucumber testing for all of our SDKs, including this one. Please refer to [algorand-sdk-testing](https://github.com/algorand/algorand-sdk-testing#readme) for guidance and existing tests that you may need to update. Depending on the type of update you wish to contribute, you may also need to have corresponding updates in the other SDKs (Go, JS, and Java). Feel welcome to ask for collaboration on that front. 
+
 ## Quick start
 
 Here's a simple example you can run without a node.
 
 ```python
 from algosdk import account, encoding
 
@@ -125,7 +128,9 @@
 ## Documentation
 
 Documentation for the Python SDK is available at [py-algorand-sdk.readthedocs.io](https://py-algorand-sdk.readthedocs.io/en/latest/).
 
 ## License
 
 py-algorand-sdk is licensed under an MIT license. See the [LICENSE](https://github.com/algorand/py-algorand-sdk/blob/master/LICENSE) file for details.
+
+
```

### Comparing `py-algorand-sdk-2.2.0/README.md` & `py-algorand-sdk-2.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -57,14 +57,16 @@
 
 * `make lint`
 
 Run non-test-harness related unit tests
 
 * `make pytest-unit`
 
+We use cucumber testing for all of our SDKs, including this one. Please refer to [algorand-sdk-testing](https://github.com/algorand/algorand-sdk-testing#readme) for guidance and existing tests that you may need to update. Depending on the type of update you wish to contribute, you may also need to have corresponding updates in the other SDKs (Go, JS, and Java). Feel welcome to ask for collaboration on that front. 
+
 ## Quick start
 
 Here's a simple example you can run without a node.
 
 ```python
 from algosdk import account, encoding
```

### Comparing `py-algorand-sdk-2.2.0/algosdk/__init__.py` & `py-algorand-sdk-2.3.0/algosdk/__init__.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/__init__.pyi` & `py-algorand-sdk-2.3.0/algosdk/__init__.pyi`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/abi/__init__.py` & `py-algorand-sdk-2.3.0/algosdk/abi/__init__.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/abi/address_type.py` & `py-algorand-sdk-2.3.0/algosdk/abi/address_type.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/abi/array_dynamic_type.py` & `py-algorand-sdk-2.3.0/algosdk/abi/array_dynamic_type.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/abi/array_static_type.py` & `py-algorand-sdk-2.3.0/algosdk/abi/array_static_type.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/abi/base_type.py` & `py-algorand-sdk-2.3.0/algosdk/abi/base_type.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/abi/bool_type.py` & `py-algorand-sdk-2.3.0/algosdk/abi/bool_type.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/abi/byte_type.py` & `py-algorand-sdk-2.3.0/algosdk/abi/byte_type.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/abi/contract.py` & `py-algorand-sdk-2.3.0/algosdk/abi/contract.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/abi/interface.py` & `py-algorand-sdk-2.3.0/algosdk/abi/interface.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/abi/method.py` & `py-algorand-sdk-2.3.0/algosdk/abi/method.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/abi/string_type.py` & `py-algorand-sdk-2.3.0/algosdk/abi/string_type.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/abi/transaction.py` & `py-algorand-sdk-2.3.0/algosdk/abi/transaction.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/abi/tuple_type.py` & `py-algorand-sdk-2.3.0/algosdk/abi/tuple_type.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/abi/ufixed_type.py` & `py-algorand-sdk-2.3.0/algosdk/abi/ufixed_type.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/abi/uint_type.py` & `py-algorand-sdk-2.3.0/algosdk/abi/uint_type.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/account.py` & `py-algorand-sdk-2.3.0/algosdk/account.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/atomic_transaction_composer.py` & `py-algorand-sdk-2.3.0/algosdk/atomic_transaction_composer.py`

 * *Files 2% similar despite different names*

```diff
@@ -268,18 +268,20 @@
 class SimulateEvalOverrides:
     def __init__(
         self,
         *,
         max_log_calls: Optional[int] = None,
         max_log_size: Optional[int] = None,
         allow_empty_signatures: Optional[bool] = None,
+        extra_opcode_budget: Optional[int] = None,
     ) -> None:
         self.max_log_calls = max_log_calls
         self.max_log_size = max_log_size
         self.allow_empty_signatures = allow_empty_signatures
+        self.extra_opcode_budget = extra_opcode_budget
 
     @staticmethod
     def from_simulation_result(
         simulation_result: Dict[str, Any]
     ) -> Optional["SimulateEvalOverrides"]:
         if "eval-overrides" not in simulation_result:
             return None
@@ -291,14 +293,18 @@
             eval_override.max_log_calls = eval_override_dict["max-log-calls"]
         if "max-log-size" in eval_override_dict:
             eval_override.max_log_size = eval_override_dict["max-log-size"]
         if "allow-empty-signatures" in eval_override_dict:
             eval_override.allow_empty_signatures = eval_override_dict[
                 "allow-empty-signatures"
             ]
+        if "extra-opcode-budget" in eval_override_dict:
+            eval_override.extra_opcode_budget = eval_override_dict[
+                "extra-opcode-budget"
+            ]
 
         return eval_override
 
 
 class SimulateAtomicTransactionResponse:
     def __init__(
         self,
```

### Comparing `py-algorand-sdk-2.2.0/algosdk/auction.py` & `py-algorand-sdk-2.3.0/algosdk/auction.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/box_reference.py` & `py-algorand-sdk-2.3.0/algosdk/box_reference.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/constants.py` & `py-algorand-sdk-2.3.0/algosdk/constants.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/dryrun_results.py` & `py-algorand-sdk-2.3.0/algosdk/dryrun_results.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/encoding.py` & `py-algorand-sdk-2.3.0/algosdk/encoding.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/error.py` & `py-algorand-sdk-2.3.0/algosdk/error.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/kmd.py` & `py-algorand-sdk-2.3.0/algosdk/kmd.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/logic.py` & `py-algorand-sdk-2.3.0/algosdk/logic.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/mnemonic.py` & `py-algorand-sdk-2.3.0/algosdk/mnemonic.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/source_map.py` & `py-algorand-sdk-2.3.0/algosdk/source_map.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/testing/dryrun.py` & `py-algorand-sdk-2.3.0/algosdk/testing/dryrun.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/transaction.py` & `py-algorand-sdk-2.3.0/algosdk/transaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -3032,14 +3032,21 @@
             and self.sprf == other.sprf
             and self.sprfmsg == other.sprfmsg
         )
 
         return False
 
 
+GenericSignedTransaction = Union[
+    SignedTransaction,
+    LogicSigTransaction,
+    MultisigTransaction,
+]
+
+
 def write_to_file(txns, path, overwrite=True):
     """
     Write signed or unsigned transactions to a file.
 
     Args:
         txns (Transaction[], SignedTransaction[], or MultisigTransaction[]):\
             can be a mix of the three
@@ -3229,15 +3236,15 @@
 
 
 defaultAppId = 1380011588
 
 
 def create_dryrun(
     client: algod.AlgodClient,
-    txns: List["GenericSignedTransaction"],
+    txns: List[GenericSignedTransaction],
     protocol_version=None,
     latest_timestamp=None,
     round=None,
 ) -> models.DryrunRequest:
     """
     Create DryrunRequest object from a client and list of signed transactions
 
@@ -3357,14 +3364,7 @@
     app["params"]["approval-program"] = base64.b64decode(
         app["params"]["approval-program"]
     )
     app["params"]["clear-state-program"] = base64.b64decode(
         app["params"]["clear-state-program"]
     )
     return app
-
-
-GenericSignedTransaction = Union[
-    SignedTransaction,
-    LogicSigTransaction,
-    MultisigTransaction,
-]
```

### Comparing `py-algorand-sdk-2.2.0/algosdk/util.py` & `py-algorand-sdk-2.3.0/algosdk/util.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/v2client/algod.py` & `py-algorand-sdk-2.3.0/algosdk/v2client/algod.py`

 * *Files 3% similar despite different names*

```diff
@@ -714,14 +714,75 @@
 
         Returns:
             Dict[str, Any]: Response from algod
         """
         req = f"/devmode/blocks/offset/{offset}"
         return self.algod_request("POST", req, **kwargs)
 
+    def get_ledger_state_delta(
+        self, round: int, response_format: str = "json", **kwargs: Any
+    ) -> AlgodResponseType:
+        """
+        Get the ledger state delta for a round.
+
+        Args:
+            round (int): The round for the desired state delta
+            response_format (str): The format in which the response is returned: either
+                "json" or "msgpack"
+
+        Returns:
+            Dict[str, Any]: Response from algod
+        """
+        query = {"format": response_format}
+        req = f"/deltas/{round}"
+        return self.algod_request(
+            "GET", req, params=query, response_format=response_format, **kwargs
+        )
+
+    def get_transaction_group_ledger_state_deltas_for_round(
+        self, round: int, response_format: str = "json", **kwargs: Any
+    ) -> AlgodResponseType:
+        """
+        Get the ledger state deltas for all transaction groups in a given round.
+
+        Args:
+            round (int): The round for the desired state delta
+            response_format (str): The format in which the response is returned: either
+                "json" or "msgpack"
+
+        Returns:
+            Dict[str, Any]: Response from algod
+        """
+        query = {"format": response_format}
+        req = f"/deltas/{round}/txn/group"
+        return self.algod_request(
+            "GET", req, params=query, response_format=response_format, **kwargs
+        )
+
+    def get_ledger_state_delta_for_transaction_group(
+        self, id: str, response_format: str = "json", **kwargs: Any
+    ) -> AlgodResponseType:
+        """
+        Get the ledger state delta for a transaction group given the
+        transaction or group ID.
+
+        Args:
+            id (str): A transaction ID or transaction group ID
+            response_format (str): The format in which the response is returned: either
+                "json" or "msgpack"
+
+        Returns:
+            Dict[str, Any]: Response from algod
+        """
+        query = {"format": response_format}
+        req = f"/deltas/txn/group/{id}"
+        return self.algod_request(
+            "GET", req, params=query, response_format=response_format, **kwargs
+        )
+
 
 def _specify_round_string(
     block: Union[int, None], round_num: Union[int, None]
 ) -> str:
     """
     Return the round number specified in either 'block' or 'round_num'.
```

### Comparing `py-algorand-sdk-2.2.0/algosdk/v2client/indexer.py` & `py-algorand-sdk-2.3.0/algosdk/v2client/indexer.py`

 * *Files 5% similar despite different names*

```diff
@@ -119,27 +119,34 @@
                 token provided by the previous results
             min_balance (int, optional): results should have an amount greater
                 than this value (results with an amount equal to this value
                 are excluded)
             max_balance (int, optional): results should have an amount less
                 than this value (results with an amount equal to this value
                 are excluded)
-            block (int, optional): include results for the specified round;
-                for performance reasons, this parameter may be disabled on
-                some configurations
+            block (int, optional): this is a synonym for round_num. Do not
+                include both.
             auth_addr (str, optional): Include accounts configured to use
                 this spending key.
             application_id (int, optional): results should filter on this
                 application
-            round_num (int, optional): alias for block; only specify one of
-                these
+            round_num (int, optional): Include results for the specified round.
+                For performance reasons, this parameter may be disabled on some configurations.
+                Using application-id or asset-id filters will return both creator and opt-in accounts.
+                Filtering by include-all will return creator and opt-in accounts for deleted assets and accounts.
+                Non-opt-in managers are not included in the results when asset-id is used.
+                If specified, do not include block
             include_all (bool, optional): include all items including closed
                 accounts, deleted applications, destroyed assets, opted-out
                 asset holdings, and closed-out application localstates. Defaults
                 to false.
+            exclude (str optional): Exclude additional items such as asset holdings,
+                application local data stored for this account,
+                asset parameters created by this account,
+                and application parameters created by this account.
         """
         req = "/accounts"
         query = dict()
         if asset_id:
             query["asset-id"] = asset_id
         if limit:
             query["limit"] = limit
@@ -182,19 +189,14 @@
                 token provided by the previous results
             min_balance (int, optional): results should have an amount greater
                 than this value (results with an amount equal to this value
                 are excluded)
             max_balance (int, optional): results should have an amount less
                 than this value (results with an amount equal to this value
                 are excluded)
-            block (int, optional): include results for the specified round;
-                for performance reasons, this parameter may be disabled on
-                some configurations
-            round_num (int, optional): alias for block; only specify one of
-                these
             include_all (bool, optional): include all items including closed
                 accounts, deleted applications, destroyed assets, opted-out
                 asset holdings, and closed-out application localstates. Defaults
                 to false.
         """
         req = "/assets/" + str(asset_id) + "/balances"
         query = dict()
@@ -239,21 +241,24 @@
         **kwargs
     ):
         """
         Return account information.
 
         Args:
             address (str): account public key
-            block (int, optional): use results from the specified round
-            round_num (int, optional): alias for block; only specify one of
-                these
-            include_all (bool, optional): include all items including closed
-                accounts, deleted applications, destroyed assets, opted-out
-                asset holdings, and closed-out application localstates. Defaults
-                to false.
+            block (int, optional): this is a synonym for round_num. Do not
+                include both.
+            round_num (int, optional): Include results for the specified round.
+                If specified, do not include block
+            include_all (bool, optional): Include all items including closed accounts, deleted applications,
+                destroyed assets, opted-out asset holdings, and closed-out application localstates.
+                Defaults to false.
+            exclude (str optional): Exclude additional items such as asset holdings,
+                application local data stored for this account, asset parameters created by this account,
+                and application parameters created by this account.
         """
         req = "/accounts/" + address
         query = dict()
         _specify_round(query, block, round_num)
         if include_all:
             query["include-all"] = include_all
         if exclude:
@@ -278,17 +283,18 @@
         Args:
             address (str): account public key
             limit (int, optional): maximum number of results to return
             next_page (str, optional): the next page of results; use the next
                 token provided by the previous results
             asset_id (int): include transactions for the specified
                 asset
-            block (int, optional): use results from the specified round
-            round_num (int, optional): alias for block; only specify one of
-                these
+            block (int, optional): this is a synonym for round_num. Do not
+                include both.
+            round_num (int, optional): Include results for the specified round.
+                If specified, do not include block
             include_all (bool, optional): include all items including closed
                 accounts, deleted applications, destroyed assets, opted-out
                 asset holdings, and closed-out application localstates. Defaults
                 to false.
         """
         req = "/accounts/" + address + "/assets"
         query = dict()
@@ -321,17 +327,18 @@
         Args:
             address (str): account public key
             limit (int, optional): maximum number of results to return
             next_page (str, optional): the next page of results; use the next
                 token provided by the previous results
             asset_id (int): include transactions for the specified
                 asset
-            block (int, optional): use results from the specified round
-            round_num (int, optional): alias for block; only specify one of
-                these
+            block (int, optional): this is a synonym for round_num. Do not
+                include both.
+            round_num (int, optional): Include results for the specified round.
+                If specified, do not include block
             include_all (bool, optional): include all items including closed
                 accounts, deleted applications, destroyed assets, opted-out
                 asset holdings, and closed-out application localstates. Defaults
                 to false.
         """
         req = "/accounts/" + address + "/created-assets"
         query = dict()
@@ -363,17 +370,18 @@
 
         Args:
             address (str): account public key
             limit (int, optional): maximum number of results to return
             next_page (str, optional): the next page of results; use the next
                 token provided by the previous results
             application_id (int, optional): restrict search to application index
-            block (int, optional): use results from the specified round
-            round_num (int, optional): alias for block; only specify one of
-                these
+            block (int, optional): this is a synonym for round_num. Do not
+                include both.
+            round_num (int, optional): Include results for the specified round.
+                If specified, do not include block
             include_all (bool, optional): include all items including closed
                 accounts, deleted applications, destroyed assets, opted-out
                 asset holdings, and closed-out application localstates. Defaults
                 to false.
         """
         req = "/accounts/" + address + "/apps-local-state"
         query = dict()
@@ -405,17 +413,18 @@
 
         Args:
             address (str): account public key
             limit (int, optional): maximum number of results to return
             next_page (str, optional): the next page of results; use the next
                 token provided by the previous results
             application_id (int, optional): restrict search to application index
-            block (int, optional): use results from the specified round
-            round_num (int, optional): alias for block; only specify one of
-                these
+            block (int, optional): this is a synonym for round_num. Do not
+                include both.
+            round_num (int, optional): Include results for the specified round.
+                If specified, do not include block
             include_all (bool, optional): include all items including closed
                 accounts, deleted applications, destroyed assets, opted-out
                 asset holdings, and closed-out application localstates. Defaults
                 to false.
         """
         req = "/accounts/" + address + "/created-applications"
         query = dict()
@@ -483,18 +492,18 @@
             block (int, optional): include results for the specified round
             min_round (int, optional): include results at or after the
                 specified round
             max_round (int, optional): include results at or before the
                 specified round
             asset_id (int, optional): include transactions for the specified
                 asset
-            end_time (str, optional): include results before the given time;
-                must be an RFC 3339 formatted string
             start_time (str, optional): include results after the given time;
                 must be an RFC 3339 formatted string
+            end_time (str, optional): include results before the given time;
+                must be an RFC 3339 formatted string
             min_amount (int, optional): results should have an amount greater
                 than this value; microalgos are the default currency unless an
                 asset-id is provided, in which case the asset will be used
             max_amount (int, optional): results should have an amount less
                 than this value, microalgos are the default currency unless an
                 asset-id is provided, in which case the asset will be used
             address (str, optional): only include transactions with this
@@ -589,35 +598,36 @@
             note_prefix (bytes, optional): specifies a prefix which must be
                 contained in the note field
             txn_type (str, optional): type of transaction; one of "pay",
                 "keyreg", "acfg", "axfer", "afrz"
             sig_type (str, optional): type of signature; one of "sig", "msig",
                 "lsig"
             txid (str, optional): lookup a specific transaction by ID
-            block (int, optional): include results for the specified round
+            block (int, optional): this is a synonym for round_num. Do not
+                include both.
             min_round (int, optional): include results at or after the
                 specified round
             max_round (int, optional): include results at or before the
                 specified round
             asset_id (int, optional): include transactions for the specified
                 asset
-            end_time (str, optional): include results before the given time;
-                must be an RFC 3339 formatted string
             start_time (str, optional): include results after the given time;
                 must be an RFC 3339 formatted string
+            end_time (str, optional): include results before the given time;
+                must be an RFC 3339 formatted string
             min_amount (int, optional): results should have an amount greater
                 than this value; microalgos are the default currency unless an
                 asset-id is provided, in which case the asset will be used
             max_amount (int, optional): results should have an amount less
                 than this value, microalgos are the default currency unless an
                 asset-id is provided, in which case the asset will be used
             rekey_to (bool, optional): include results which include the
                 rekey-to field
-            round_num (int, optional): alias for block; only specify one of
-                these
+            round_num (int, optional): Include results for the specified round.
+                If specified, do not include block
         """
         req = "/accounts/" + address + "/transactions"
         query = dict()
         if limit:
             query["limit"] = limit
         if next_page:
             query["next"] = next_page
@@ -684,25 +694,26 @@
             note_prefix (bytes, optional): specifies a prefix which must be
                 contained in the note field
             txn_type (str, optional): type of transaction; one of "pay",
                 "keyreg", "acfg", "axfer", "afrz"
             sig_type (str, optional): type of signature; one of "sig", "msig",
                 "lsig"
             txid (str, optional): lookup a specific transaction by ID
-            block (int, optional): include results for the specified round
+            block (int, optional): this is a synonym for round_num. Do not
+                include both.
             min_round (int, optional): include results at or after the
                 specified round
             max_round (int, optional): include results at or before the
                 specified round
             address (str, optional): only include transactions with this
                 address in one of the transaction fields
-            end_time (str, optional): include results before the given time;
-                must be an RFC 3339 formatted string
             start_time (str, optional): include results after the given time;
                 must be an RFC 3339 formatted string
+            end_time (str, optional): include results before the given time;
+                must be an RFC 3339 formatted string
             min_amount (int, optional): results should have an amount greater
                 than this value; microalgos are the default currency unless an
                 asset-id is provided, in which case the asset will be used
             max_amount (int, optional): results should have an amount less
                 than this value, microalgos are the default currency unless an
                 asset-id is provided, in which case the asset will be used
             address_role (str, optional): one of "sender" or "receiver";
@@ -711,16 +722,16 @@
             exclude_close_to (bool, optional): combine with address and
                 address_role parameters to define what type of address to
                 search for; the close to fields are normally treated as a
                 receiver, if you would like to exclude them set this parameter
                 to true
             rekey_to (bool, optional): include results which include the
                 rekey-to field
-            round_num (int, optional): alias for block; only specify one of
-                these
+            round_num (int, optional): Include results for the specified round.
+                If specified, do not include block
         """
         req = "/assets/" + str(asset_id) + "/transactions"
         query = dict()
         if limit:
             query["limit"] = limit
         if next_page:
             query["next"] = next_page
@@ -860,17 +871,19 @@
         **kwargs
     ):
         """
         Return applications that satisfy the conditions.
 
         Args:
             application_id (int, optional): restrict search to application index
+            creator (str, optional): filter just assets with the given creator
+                address
             round (int, optional): not supported, DO NOT USE!
             limit (int, optional): restrict number of results to limit
-            next_page (string, optional): used for pagination
+            next_page (str, optional): used for pagination
             round_num (int, optional): not supported, DO NOT USE!
             include_all (bool, optional): include all items including closed
                 accounts, deleted applications, destroyed assets, opted-out
                 asset holdings, and closed-out application localstates. Defaults
                 to false.
         """
         req = "/applications"
@@ -904,17 +917,17 @@
         Return log messages generated by the passed in application.
 
         Args:
             application_id (int): application index
             limit (int, optional): limit maximum number of results to return
             min_round (int, optional): only include results at or after the specified round
             max_round (int, optional): only include results at or before the specified round
-            next_page (string, optional): used for pagination
-            sender_addr (string, optional): only include transactions with this sender address
-            txid (string, optional): only include results with this transaction ID
+            next_page (str, optional): used for pagination
+            sender_addr (str, optional): only include transactions with this sender address
+            txid (str, optional): only include results with this transaction ID
         """
         req = "/applications/{}/logs".format(application_id)
         query = dict()
         if limit:
             query["limit"] = limit
         if max_round:
             query["max-round"] = max_round
@@ -956,15 +969,15 @@
 
         NOTE: box names are returned as base64-encoded strings.
 
         Args:
             application_id (int): The ID of the application to look up.
             limit (int, optional): Max number of box names to return.
                 If max is not set, or max == 0, returns all box-names up to queried indexer's `defaultBoxesLimit`.
-            next_page (string, optional): used for pagination
+            next_page (str, optional): used for pagination
         """
         req = "/applications/" + str(application_id) + "/boxes"
         params = {}
         if limit:
             params["limit"] = limit
         if next_page:
             params["next"] = next_page
```

### Comparing `py-algorand-sdk-2.2.0/algosdk/v2client/models/__init__.py` & `py-algorand-sdk-2.3.0/algosdk/v2client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/v2client/models/account.py` & `py-algorand-sdk-2.3.0/algosdk/v2client/models/account.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/v2client/models/account_participation.py` & `py-algorand-sdk-2.3.0/algosdk/v2client/models/account_participation.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/v2client/models/application.py` & `py-algorand-sdk-2.3.0/algosdk/v2client/models/application.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/v2client/models/application_local_state.py` & `py-algorand-sdk-2.3.0/algosdk/v2client/models/application_local_state.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/v2client/models/application_params.py` & `py-algorand-sdk-2.3.0/algosdk/v2client/models/application_params.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/v2client/models/application_state_schema.py` & `py-algorand-sdk-2.3.0/algosdk/v2client/models/application_state_schema.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/v2client/models/asset.py` & `py-algorand-sdk-2.3.0/algosdk/v2client/models/asset.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/v2client/models/asset_holding.py` & `py-algorand-sdk-2.3.0/algosdk/v2client/models/asset_holding.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/v2client/models/asset_params.py` & `py-algorand-sdk-2.3.0/algosdk/v2client/models/asset_params.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/v2client/models/dryrun_request.py` & `py-algorand-sdk-2.3.0/algosdk/v2client/models/dryrun_request.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/v2client/models/dryrun_source.py` & `py-algorand-sdk-2.3.0/algosdk/v2client/models/dryrun_source.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/v2client/models/simulate_request.py` & `py-algorand-sdk-2.3.0/algosdk/v2client/models/simulate_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,27 +16,31 @@
         return {"txns": [txn.dictify() for txn in self.txns]}
 
 
 class SimulateRequest(object):
     txn_groups: List[SimulateRequestTransactionGroup]
     allow_more_logs: bool
     allow_empty_signatures: bool
+    extra_opcode_budget: int
 
     def __init__(
         self,
         *,
         txn_groups: List[SimulateRequestTransactionGroup],
         allow_more_logs: bool = False,
         allow_empty_signatures: bool = False,
+        extra_opcode_budget: int = 0,
     ) -> None:
         self.txn_groups = txn_groups
         self.allow_more_logs = allow_more_logs
         self.allow_empty_signatures = allow_empty_signatures
+        self.extra_opcode_budget = extra_opcode_budget
 
     def dictify(self) -> Dict[str, Any]:
         return {
             "txn-groups": [
                 txn_group.dictify() for txn_group in self.txn_groups
             ],
             "allow-more-logging": self.allow_more_logs,
             "allow-empty-signatures": self.allow_empty_signatures,
+            "extra-opcode-budget": self.extra_opcode_budget,
         }
```

### Comparing `py-algorand-sdk-2.2.0/algosdk/v2client/models/teal_key_value.py` & `py-algorand-sdk-2.3.0/algosdk/v2client/models/teal_key_value.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/v2client/models/teal_value.py` & `py-algorand-sdk-2.3.0/algosdk/v2client/models/teal_value.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/wallet.py` & `py-algorand-sdk-2.3.0/algosdk/wallet.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/algosdk/wordlist.py` & `py-algorand-sdk-2.3.0/algosdk/wordlist.py`

 * *Files identical despite different names*

### Comparing `py-algorand-sdk-2.2.0/py_algorand_sdk.egg-info/PKG-INFO` & `py-algorand-sdk-2.3.0/py_algorand_sdk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: py-algorand-sdk
-Version: 2.2.0
+Version: 2.3.0
 Summary: Algorand SDK in Python
 Home-page: https://github.com/algorand/py-algorand-sdk
 Author: Algorand
 Author-email: pypiservice@algorand.com
 License: MIT
 Project-URL: Source, https://github.com/algorand/py-algorand-sdk
+Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # py-algorand-sdk
 
 [![PyPI version](https://badge.fury.io/py/py-algorand-sdk.svg)](https://badge.fury.io/py/py-algorand-sdk)
@@ -70,14 +71,16 @@
 
 * `make lint`
 
 Run non-test-harness related unit tests
 
 * `make pytest-unit`
 
+We use cucumber testing for all of our SDKs, including this one. Please refer to [algorand-sdk-testing](https://github.com/algorand/algorand-sdk-testing#readme) for guidance and existing tests that you may need to update. Depending on the type of update you wish to contribute, you may also need to have corresponding updates in the other SDKs (Go, JS, and Java). Feel welcome to ask for collaboration on that front. 
+
 ## Quick start
 
 Here's a simple example you can run without a node.
 
 ```python
 from algosdk import account, encoding
 
@@ -125,7 +128,9 @@
 ## Documentation
 
 Documentation for the Python SDK is available at [py-algorand-sdk.readthedocs.io](https://py-algorand-sdk.readthedocs.io/en/latest/).
 
 ## License
 
 py-algorand-sdk is licensed under an MIT license. See the [LICENSE](https://github.com/algorand/py-algorand-sdk/blob/master/LICENSE) file for details.
+
+
```

### Comparing `py-algorand-sdk-2.2.0/py_algorand_sdk.egg-info/SOURCES.txt` & `py-algorand-sdk-2.3.0/py_algorand_sdk.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -58,21 +58,8 @@
 algosdk/v2client/models/simulate_request.py
 algosdk/v2client/models/teal_key_value.py
 algosdk/v2client/models/teal_value.py
 py_algorand_sdk.egg-info/PKG-INFO
 py_algorand_sdk.egg-info/SOURCES.txt
 py_algorand_sdk.egg-info/dependency_links.txt
 py_algorand_sdk.egg-info/requires.txt
-py_algorand_sdk.egg-info/top_level.txt
-tests/__init__.py
-tests/environment.py
-tests/steps/__init__.py
-tests/steps/account_v2_steps.py
-tests/steps/application_v2_steps.py
-tests/steps/other_v2_steps.py
-tests/steps/steps.py
-tests/unit_tests/__init__.py
-tests/unit_tests/test_abi.py
-tests/unit_tests/test_dryrun.py
-tests/unit_tests/test_logicsig.py
-tests/unit_tests/test_other.py
-tests/unit_tests/test_transaction.py
+py_algorand_sdk.egg-info/top_level.txt
```

### Comparing `py-algorand-sdk-2.2.0/setup.py` & `py-algorand-sdk-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = f.read()
 
 setuptools.setup(
     name="py-algorand-sdk",
     description="Algorand SDK in Python",
     author="Algorand",
     author_email="pypiservice@algorand.com",
-    version="2.2.0",
+    version="2.3.0",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/algorand/py-algorand-sdk",
     license="MIT",
     project_urls={
         "Source": "https://github.com/algorand/py-algorand-sdk",
     },
```

