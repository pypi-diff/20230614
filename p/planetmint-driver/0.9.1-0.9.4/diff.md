# Comparing `tmp/planetmint_driver-0.9.1.tar.gz` & `tmp/planetmint_driver-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planetmint_driver-0.9.1.tar", last modified: Mon Jan 31 22:37:53 2022, max compression
+gzip compressed data, was "planetmint_driver-0.9.4.tar", last modified: Mon Mar 28 21:00:21 2022, max compression
```

## Comparing `planetmint_driver-0.9.1.tar` & `planetmint_driver-0.9.4.tar`

### file list

```diff
@@ -1,88 +1,66 @@
-drwxrwxr-x   0 juergen   (1000) juergen   (1000)        0 2022-01-31 22:37:53.373532 planetmint_driver-0.9.1/
--rw-rw-r--   0 juergen   (1000) juergen   (1000)      235 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/AUTHORS.rst
--rw-rw-r--   0 juergen   (1000) juergen   (1000)     5535 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/CHANGELOG.rst
--rw-rw-r--   0 juergen   (1000) juergen   (1000)     5748 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/CONTRIBUTING.rst
--rw-rw-r--   0 juergen   (1000) juergen   (1000)    34523 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/LICENSE
--rw-rw-r--   0 juergen   (1000) juergen   (1000)      285 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/MANIFEST.in
--rw-rw-r--   0 juergen   (1000) juergen   (1000)    17069 2022-01-31 22:37:53.373532 planetmint_driver-0.9.1/PKG-INFO
--rw-rw-r--   0 juergen   (1000) juergen   (1000)     7729 2022-01-31 19:57:32.000000 planetmint_driver-0.9.1/README.rst
-drwxrwxr-x   0 juergen   (1000) juergen   (1000)        0 2022-01-31 22:37:53.369532 planetmint_driver-0.9.1/docs/
--rw-rw-r--   0 juergen   (1000) juergen   (1000)     6806 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/docs/Makefile
-drwxrwxr-x   0 juergen   (1000) juergen   (1000)        0 2022-01-31 22:37:53.369532 planetmint_driver-0.9.1/docs/_static/
--rw-rw-r--   0 juergen   (1000) juergen   (1000)    53825 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/docs/_static/cc_escrow_execute_abort.png
--rw-rw-r--   0 juergen   (1000) juergen   (1000)    61740 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/docs/_static/tx_escrow_execute_abort.png
--rw-rw-r--   0 juergen   (1000) juergen   (1000)    27597 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/docs/_static/tx_multi_condition_multi_fulfillment_v1.png
--rw-rw-r--   0 juergen   (1000) juergen   (1000)    11955 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/docs/_static/tx_single_condition_single_fulfillment_v1.png
--rw-rw-r--   0 juergen   (1000) juergen   (1000)     1423 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/docs/aboutthedocs.rst
--rw-rw-r--   0 juergen   (1000) juergen   (1000)      947 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/docs/advanced-installation.rst
--rw-rw-r--   0 juergen   (1000) juergen   (1000)    44159 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/docs/advanced-usage.rst
--rw-rw-r--   0 juergen   (1000) juergen   (1000)      187 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/docs/authors.rst
--rw-rw-r--   0 juergen   (1000) juergen   (1000)      189 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/docs/changelog.rst
--rwxrwxr-x   0 juergen   (1000) juergen   (1000)     2174 2022-01-31 22:15:50.000000 planetmint_driver-0.9.1/docs/conf.py
--rw-rw-r--   0 juergen   (1000) juergen   (1000)     2408 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/docs/connect.rst
--rw-rw-r--   0 juergen   (1000) juergen   (1000)      192 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/docs/contributing.rst
--rw-rw-r--   0 juergen   (1000) juergen   (1000)    67499 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/docs/handcraft.rst
--rw-rw-r--   0 juergen   (1000) juergen   (1000)      821 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/docs/index.rst
--rw-rw-r--   0 juergen   (1000) juergen   (1000)     1929 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/docs/libref.rst
--rw-rw-r--   0 juergen   (1000) juergen   (1000)     6481 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/docs/make.bat
-drwxrwxr-x   0 juergen   (1000) juergen   (1000)        0 2022-01-31 22:37:53.369532 planetmint_driver-0.9.1/docs/out/
-drwxrwxr-x   0 juergen   (1000) juergen   (1000)        0 2022-01-31 22:37:53.369532 planetmint_driver-0.9.1/docs/out/html/
-drwxrwxr-x   0 juergen   (1000) juergen   (1000)        0 2022-01-31 22:37:53.369532 planetmint_driver-0.9.1/docs/out/html/_images/
--rw-rw-r--   0 juergen   (1000) juergen   (1000)    53825 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/docs/out/html/_images/cc_escrow_execute_abort.png
--rw-rw-r--   0 juergen   (1000) juergen   (1000)    61740 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/docs/out/html/_images/tx_escrow_execute_abort.png
--rw-rw-r--   0 juergen   (1000) juergen   (1000)    11955 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/docs/out/html/_images/tx_single_condition_single_fulfillment_v1.png
-drwxrwxr-x   0 juergen   (1000) juergen   (1000)        0 2022-01-31 22:37:53.373532 planetmint_driver-0.9.1/docs/out/html/_static/
--rw-rw-r--   0 juergen   (1000) juergen   (1000)      673 2022-01-31 20:26:51.000000 planetmint_driver-0.9.1/docs/out/html/_static/ajax-loader.gif
--rw-rw-r--   0 juergen   (1000) juergen   (1000)    53825 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/docs/out/html/_static/cc_escrow_execute_abort.png
--rw-rw-r--   0 juergen   (1000) juergen   (1000)      756 2022-01-31 20:26:51.000000 planetmint_driver-0.9.1/docs/out/html/_static/comment-bright.png
--rw-rw-r--   0 juergen   (1000) juergen   (1000)      829 2022-01-31 20:26:51.000000 planetmint_driver-0.9.1/docs/out/html/_static/comment-close.png
--rw-rw-r--   0 juergen   (1000) juergen   (1000)      641 2022-01-31 20:26:51.000000 planetmint_driver-0.9.1/docs/out/html/_static/comment.png
--rw-rw-r--   0 juergen   (1000) juergen   (1000)      222 2022-01-31 20:26:51.000000 planetmint_driver-0.9.1/docs/out/html/_static/down-pressed.png
--rw-rw-r--   0 juergen   (1000) juergen   (1000)      202 2022-01-31 20:26:51.000000 planetmint_driver-0.9.1/docs/out/html/_static/down.png
--rw-rw-r--   0 juergen   (1000) juergen   (1000)      286 2022-01-31 20:26:51.000000 planetmint_driver-0.9.1/docs/out/html/_static/file.png
--rw-rw-r--   0 juergen   (1000) juergen   (1000)       90 2022-01-31 20:26:51.000000 planetmint_driver-0.9.1/docs/out/html/_static/minus.png
--rw-rw-r--   0 juergen   (1000) juergen   (1000)       90 2022-01-31 20:26:51.000000 planetmint_driver-0.9.1/docs/out/html/_static/plus.png
--rw-rw-r--   0 juergen   (1000) juergen   (1000)    61740 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/docs/out/html/_static/tx_escrow_execute_abort.png
--rw-rw-r--   0 juergen   (1000) juergen   (1000)    27597 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/docs/out/html/_static/tx_multi_condition_multi_fulfillment_v1.png
--rw-rw-r--   0 juergen   (1000) juergen   (1000)    11955 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/docs/out/html/_static/tx_single_condition_single_fulfillment_v1.png
--rw-rw-r--   0 juergen   (1000) juergen   (1000)      214 2022-01-31 20:26:51.000000 planetmint_driver-0.9.1/docs/out/html/_static/up-pressed.png
--rw-rw-r--   0 juergen   (1000) juergen   (1000)      203 2022-01-31 20:26:51.000000 planetmint_driver-0.9.1/docs/out/html/_static/up.png
--rw-rw-r--   0 juergen   (1000) juergen   (1000)     6074 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/docs/quickstart.rst
--rw-rw-r--   0 juergen   (1000) juergen   (1000)      439 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/docs/upgrading.rst
--rw-rw-r--   0 juergen   (1000) juergen   (1000)    25017 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/docs/usage.rst
-drwxrwxr-x   0 juergen   (1000) juergen   (1000)        0 2022-01-31 22:37:53.373532 planetmint_driver-0.9.1/planetmint_driver/
--rw-rw-r--   0 juergen   (1000) juergen   (1000)      279 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/planetmint_driver/__init__.py
-drwxrwxr-x   0 juergen   (1000) juergen   (1000)        0 2022-01-31 22:37:53.373532 planetmint_driver-0.9.1/planetmint_driver/common/
--rw-rw-r--   0 juergen   (1000) juergen   (1000)     1035 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/planetmint_driver/common/__init__.py
--rw-rw-r--   0 juergen   (1000) juergen   (1000)     1997 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/planetmint_driver/common/crypto.py
--rw-rw-r--   0 juergen   (1000) juergen   (1000)     4060 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/planetmint_driver/common/exceptions.py
--rw-rw-r--   0 juergen   (1000) juergen   (1000)    46789 2022-01-31 22:10:10.000000 planetmint_driver-0.9.1/planetmint_driver/common/transaction.py
--rw-rw-r--   0 juergen   (1000) juergen   (1000)     5039 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/planetmint_driver/common/utils.py
--rw-rw-r--   0 juergen   (1000) juergen   (1000)     4695 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/planetmint_driver/connection.py
--rw-rw-r--   0 juergen   (1000) juergen   (1000)      875 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/planetmint_driver/crypto.py
--rw-rw-r--   0 juergen   (1000) juergen   (1000)    18244 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/planetmint_driver/driver.py
--rw-rw-r--   0 juergen   (1000) juergen   (1000)     2108 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/planetmint_driver/exceptions.py
--rw-rw-r--   0 juergen   (1000) juergen   (1000)    12426 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/planetmint_driver/offchain.py
--rw-rw-r--   0 juergen   (1000) juergen   (1000)     2300 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/planetmint_driver/pool.py
--rw-rw-r--   0 juergen   (1000) juergen   (1000)     3163 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/planetmint_driver/transport.py
--rw-rw-r--   0 juergen   (1000) juergen   (1000)     2828 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/planetmint_driver/utils.py
-drwxrwxr-x   0 juergen   (1000) juergen   (1000)        0 2022-01-31 22:37:53.373532 planetmint_driver-0.9.1/planetmint_driver.egg-info/
--rw-rw-r--   0 juergen   (1000) juergen   (1000)    17069 2022-01-31 22:37:52.000000 planetmint_driver-0.9.1/planetmint_driver.egg-info/PKG-INFO
--rw-rw-r--   0 juergen   (1000) juergen   (1000)     2269 2022-01-31 22:37:53.000000 planetmint_driver-0.9.1/planetmint_driver.egg-info/SOURCES.txt
--rw-rw-r--   0 juergen   (1000) juergen   (1000)        1 2022-01-31 22:37:52.000000 planetmint_driver-0.9.1/planetmint_driver.egg-info/dependency_links.txt
--rw-rw-r--   0 juergen   (1000) juergen   (1000)        1 2022-01-31 22:37:52.000000 planetmint_driver-0.9.1/planetmint_driver.egg-info/not-zip-safe
--rw-rw-r--   0 juergen   (1000) juergen   (1000)      672 2022-01-31 22:37:52.000000 planetmint_driver-0.9.1/planetmint_driver.egg-info/requires.txt
--rw-rw-r--   0 juergen   (1000) juergen   (1000)       18 2022-01-31 22:37:52.000000 planetmint_driver-0.9.1/planetmint_driver.egg-info/top_level.txt
--rw-rw-r--   0 juergen   (1000) juergen   (1000)       38 2022-01-31 22:37:53.373532 planetmint_driver-0.9.1/setup.cfg
--rw-rw-r--   0 juergen   (1000) juergen   (1000)     2124 2022-01-31 22:32:48.000000 planetmint_driver-0.9.1/setup.py
-drwxrwxr-x   0 juergen   (1000) juergen   (1000)        0 2022-01-31 22:37:53.373532 planetmint_driver-0.9.1/tests/
--rw-rw-r--   0 juergen   (1000) juergen   (1000)        0 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/tests/__init__.py
--rw-rw-r--   0 juergen   (1000) juergen   (1000)    16146 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/tests/conftest.py
--rw-rw-r--   0 juergen   (1000) juergen   (1000)     1963 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/tests/test_connection.py
--rw-rw-r--   0 juergen   (1000) juergen   (1000)      461 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/tests/test_crypto.py
--rw-rw-r--   0 juergen   (1000) juergen   (1000)    12239 2022-01-31 20:36:55.000000 planetmint_driver-0.9.1/tests/test_driver.py
--rw-rw-r--   0 juergen   (1000) juergen   (1000)      767 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/tests/test_exceptions.py
--rw-rw-r--   0 juergen   (1000) juergen   (1000)     5399 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/tests/test_offchain.py
--rw-rw-r--   0 juergen   (1000) juergen   (1000)     1226 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/tests/test_pool.py
--rw-rw-r--   0 juergen   (1000) juergen   (1000)     3514 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/tests/test_transport.py
--rw-rw-r--   0 juergen   (1000) juergen   (1000)     1475 2022-01-31 13:14:04.000000 planetmint_driver-0.9.1/tests/test_utils.py
+drwxrwxr-x   0 juergen   (1000) juergen   (1000)        0 2022-03-28 21:00:21.338145 planetmint_driver-0.9.4/
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)      235 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/AUTHORS.rst
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)     5535 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/CHANGELOG.rst
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)     5748 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/CONTRIBUTING.rst
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)    34523 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/LICENSE
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)      285 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/MANIFEST.in
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)    17069 2022-03-28 21:00:21.338145 planetmint_driver-0.9.4/PKG-INFO
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)     7729 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/README.rst
+drwxrwxr-x   0 juergen   (1000) juergen   (1000)        0 2022-03-28 21:00:21.338145 planetmint_driver-0.9.4/docs/
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)     6806 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/docs/Makefile
+drwxrwxr-x   0 juergen   (1000) juergen   (1000)        0 2022-03-28 21:00:21.338145 planetmint_driver-0.9.4/docs/_static/
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)    53825 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/docs/_static/cc_escrow_execute_abort.png
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)    61740 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/docs/_static/tx_escrow_execute_abort.png
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)    27597 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/docs/_static/tx_multi_condition_multi_fulfillment_v1.png
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)    11955 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/docs/_static/tx_single_condition_single_fulfillment_v1.png
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)     1423 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/docs/aboutthedocs.rst
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)      947 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/docs/advanced-installation.rst
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)    44159 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/docs/advanced-usage.rst
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)      187 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/docs/authors.rst
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)      189 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/docs/changelog.rst
+-rwxrwxr-x   0 juergen   (1000) juergen   (1000)     2174 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/docs/conf.py
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)     2408 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/docs/connect.rst
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)      192 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/docs/contributing.rst
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)    67499 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/docs/handcraft.rst
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)      821 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/docs/index.rst
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)     1929 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/docs/libref.rst
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)     6481 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/docs/make.bat
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)     6074 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/docs/quickstart.rst
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)      439 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/docs/upgrading.rst
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)    25017 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/docs/usage.rst
+drwxrwxr-x   0 juergen   (1000) juergen   (1000)        0 2022-03-28 21:00:21.338145 planetmint_driver-0.9.4/planetmint_driver/
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)      279 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/planetmint_driver/__init__.py
+drwxrwxr-x   0 juergen   (1000) juergen   (1000)        0 2022-03-28 21:00:21.338145 planetmint_driver-0.9.4/planetmint_driver/common/
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)     1035 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/planetmint_driver/common/__init__.py
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)     1997 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/planetmint_driver/common/crypto.py
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)     4060 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/planetmint_driver/common/exceptions.py
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)    47933 2022-03-28 20:56:59.000000 planetmint_driver-0.9.4/planetmint_driver/common/transaction.py
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)     5039 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/planetmint_driver/common/utils.py
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)     4695 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/planetmint_driver/connection.py
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)      875 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/planetmint_driver/crypto.py
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)    18244 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/planetmint_driver/driver.py
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)     2108 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/planetmint_driver/exceptions.py
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)    13091 2022-03-28 20:56:59.000000 planetmint_driver-0.9.4/planetmint_driver/offchain.py
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)     2300 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/planetmint_driver/pool.py
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)     3163 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/planetmint_driver/transport.py
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)     2828 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/planetmint_driver/utils.py
+drwxrwxr-x   0 juergen   (1000) juergen   (1000)        0 2022-03-28 21:00:21.338145 planetmint_driver-0.9.4/planetmint_driver.egg-info/
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)    17069 2022-03-28 21:00:21.000000 planetmint_driver-0.9.4/planetmint_driver.egg-info/PKG-INFO
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)     1484 2022-03-28 21:00:21.000000 planetmint_driver-0.9.4/planetmint_driver.egg-info/SOURCES.txt
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)        1 2022-03-28 21:00:21.000000 planetmint_driver-0.9.4/planetmint_driver.egg-info/dependency_links.txt
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)        1 2022-03-28 21:00:21.000000 planetmint_driver-0.9.4/planetmint_driver.egg-info/not-zip-safe
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)      672 2022-03-28 21:00:21.000000 planetmint_driver-0.9.4/planetmint_driver.egg-info/requires.txt
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)       18 2022-03-28 21:00:21.000000 planetmint_driver-0.9.4/planetmint_driver.egg-info/top_level.txt
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)       38 2022-03-28 21:00:21.338145 planetmint_driver-0.9.4/setup.cfg
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)     2124 2022-03-28 20:58:15.000000 planetmint_driver-0.9.4/setup.py
+drwxrwxr-x   0 juergen   (1000) juergen   (1000)        0 2022-03-28 21:00:21.338145 planetmint_driver-0.9.4/tests/
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)        0 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/tests/__init__.py
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)    16328 2022-03-28 20:56:59.000000 planetmint_driver-0.9.4/tests/conftest.py
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)     1963 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/tests/test_connection.py
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)      461 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/tests/test_crypto.py
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)    12239 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/tests/test_driver.py
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)      767 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/tests/test_exceptions.py
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)     6010 2022-03-28 20:56:59.000000 planetmint_driver-0.9.4/tests/test_offchain.py
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)     1226 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/tests/test_pool.py
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)     3514 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/tests/test_transport.py
+-rw-rw-r--   0 juergen   (1000) juergen   (1000)     1475 2022-02-15 15:30:26.000000 planetmint_driver-0.9.4/tests/test_utils.py
```

### Comparing `planetmint_driver-0.9.1/CHANGELOG.rst` & `planetmint_driver-0.9.4/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/CONTRIBUTING.rst` & `planetmint_driver-0.9.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/LICENSE` & `planetmint_driver-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/PKG-INFO` & `planetmint_driver-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetmint_driver
-Version: 0.9.1
+Version: 0.9.4
 Summary: Python driver for Planetmint
 Home-page: https://github.com/planetmint/planetmint-driver
 Author: Planetmint
 Author-email: contact@ipdb.global
 License: Apache Software License 2.0
 Description: 
         .. Copyright Planetmint GmbH and Planetmint contributors
```

### Comparing `planetmint_driver-0.9.1/README.rst` & `planetmint_driver-0.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/docs/Makefile` & `planetmint_driver-0.9.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/docs/_static/cc_escrow_execute_abort.png` & `planetmint_driver-0.9.4/docs/_static/cc_escrow_execute_abort.png`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/docs/_static/tx_escrow_execute_abort.png` & `planetmint_driver-0.9.4/docs/_static/tx_escrow_execute_abort.png`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/docs/_static/tx_multi_condition_multi_fulfillment_v1.png` & `planetmint_driver-0.9.4/docs/_static/tx_multi_condition_multi_fulfillment_v1.png`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/docs/_static/tx_single_condition_single_fulfillment_v1.png` & `planetmint_driver-0.9.4/docs/_static/tx_single_condition_single_fulfillment_v1.png`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/docs/aboutthedocs.rst` & `planetmint_driver-0.9.4/docs/aboutthedocs.rst`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/docs/advanced-installation.rst` & `planetmint_driver-0.9.4/docs/advanced-installation.rst`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/docs/advanced-usage.rst` & `planetmint_driver-0.9.4/docs/advanced-usage.rst`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/docs/conf.py` & `planetmint_driver-0.9.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/docs/connect.rst` & `planetmint_driver-0.9.4/docs/connect.rst`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/docs/handcraft.rst` & `planetmint_driver-0.9.4/docs/handcraft.rst`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/docs/index.rst` & `planetmint_driver-0.9.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/docs/libref.rst` & `planetmint_driver-0.9.4/docs/libref.rst`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/docs/make.bat` & `planetmint_driver-0.9.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/docs/quickstart.rst` & `planetmint_driver-0.9.4/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/docs/usage.rst` & `planetmint_driver-0.9.4/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/planetmint_driver/common/__init__.py` & `planetmint_driver-0.9.4/planetmint_driver/common/__init__.py`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/planetmint_driver/common/crypto.py` & `planetmint_driver-0.9.4/planetmint_driver/common/crypto.py`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/planetmint_driver/common/exceptions.py` & `planetmint_driver-0.9.4/planetmint_driver/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/planetmint_driver/common/transaction.py` & `planetmint_driver-0.9.4/planetmint_driver/common/transaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -539,22 +539,21 @@
 
         # Asset payloads for 'CREATE' operations must be None or
         # dicts holding a `data` property. Asset payloads for 'TRANSFER'
         # operations must be dicts holding an `id` property.
         if (operation == Transaction.CREATE and
                 asset is not None and
                 not (isinstance(asset, dict) and 'data' in asset)):
-            raise TypeError(('`asset` must be None or a dict holding a `data`'
-                             " property instance for '{}' "
-                             "Transactions".format(operation)))
+            raise TypeError('`asset` must be None or a dict holding a `data` '
+                            ' property instance for \'{}\' '
+                            'Transactions'.format(operation))
         elif (operation == Transaction.TRANSFER and
-                not (isinstance(asset, dict) and 'id' in asset)):
-            raise TypeError(('`asset` must be a dict holding an `id` property '
-                             "for 'TRANSFER' Transactions"))
-
+              not (isinstance(asset, dict) and 'id' in asset)):
+            raise TypeError('`asset` must be a dict holding an `id` property '
+                            'for {} Transactions'.format(operation))
         if outputs and not isinstance(outputs, list):
             raise TypeError('`outputs` must be a list instance or None')
 
         if inputs and not isinstance(inputs, list):
             raise TypeError('`inputs` must be a list instance or None')
 
         if metadata is not None and not isinstance(metadata, dict):
@@ -832,14 +831,41 @@
         for i, input_ in enumerate(self.inputs):
             self.inputs[i] = self._sign_input(input_, tx_serialized, key_pairs)
 
         self._hash()
 
         return self
 
+    def delegate_signing(self, callback):
+        """Fulfills a previous Transaction's Output by signing Inputs using callback.
+
+            Note:
+                This method works only for the following Cryptoconditions
+                currently:
+                    - Ed25519Fulfillment
+            Args:
+                callback (function): A callback used to sign inputs. Callback
+                    takes input dict and message to sign as arguments
+                    and returns signature (bytes).
+            Returns:
+                :class:`~planetmint.common.transaction.Transaction`
+        """
+        tx_dict = self.to_dict()
+        tx_dict = self._remove_signatures(tx_dict)
+        tx_serialized = self._to_str(tx_dict)
+        message = sha3_256(tx_serialized.encode())
+        for input_ in self.inputs:
+            if input_.fulfills:
+                message.update('{}{}'.format(
+                    input_.fulfills.txid, input_.fulfills.output).encode())
+            signature = callback(input_.to_dict(), message.digest())
+            input_.fulfillment.signature = signature
+        self._hash()
+        return self
+
     @classmethod
     def _sign_input(cls, input_, message, key_pairs):
         """Signs a single Input.
 
             Note:
                 This method works only for the following Cryptoconditions
                 currently:
```

### Comparing `planetmint_driver-0.9.1/planetmint_driver/common/utils.py` & `planetmint_driver-0.9.4/planetmint_driver/common/utils.py`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/planetmint_driver/connection.py` & `planetmint_driver-0.9.4/planetmint_driver/connection.py`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/planetmint_driver/crypto.py` & `planetmint_driver-0.9.4/planetmint_driver/crypto.py`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/planetmint_driver/driver.py` & `planetmint_driver-0.9.4/planetmint_driver/driver.py`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/planetmint_driver/exceptions.py` & `planetmint_driver-0.9.4/planetmint_driver/exceptions.py`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/planetmint_driver/offchain.py` & `planetmint_driver-0.9.4/planetmint_driver/offchain.py`

 * *Files 6% similar despite different names*

```diff
@@ -348,7 +348,25 @@
     transaction_obj = Transaction.from_dict(transaction)
     try:
         signed_transaction = transaction_obj.sign(private_keys)
     except KeypairMismatchException as exc:
         raise MissingPrivateKeyError('A private key is missing!') from exc
 
     return signed_transaction.to_dict()
+
+
+def fulfill_with_signing_delegation(transaction, signing_callback):
+    """Fulfills the given transction with signing delegated to
+    `signing_callback`.
+
+    Args:
+        transaction (dict): The transaction to be fulfilled.
+        signing_callback (function): Callback taking `input` and
+            `message` to sign and returning signature.  This signature is
+            further used to construct fulfillment.
+    Returns:
+        dict: The fulfilled transaction payload, ready to be sent to a
+            Planetmint federation.
+    """
+    return (Transaction.from_dict(transaction)
+            .delegate_signing(signing_callback)
+            .to_dict())
```

### Comparing `planetmint_driver-0.9.1/planetmint_driver/pool.py` & `planetmint_driver-0.9.4/planetmint_driver/pool.py`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/planetmint_driver/transport.py` & `planetmint_driver-0.9.4/planetmint_driver/transport.py`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/planetmint_driver/utils.py` & `planetmint_driver-0.9.4/planetmint_driver/utils.py`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/planetmint_driver.egg-info/PKG-INFO` & `planetmint_driver-0.9.4/planetmint_driver.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetmint-driver
-Version: 0.9.1
+Version: 0.9.4
 Summary: Python driver for Planetmint
 Home-page: https://github.com/planetmint/planetmint-driver
 Author: Planetmint
 Author-email: contact@ipdb.global
 License: Apache Software License 2.0
 Description: 
         .. Copyright Planetmint GmbH and Planetmint contributors
```

### Comparing `planetmint_driver-0.9.1/planetmint_driver.egg-info/requires.txt` & `planetmint_driver-0.9.4/planetmint_driver.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/setup.py` & `planetmint_driver-0.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     'sphinx_rtd_theme',
     'sphinxcontrib-httpdomain',
     'matplotlib',
 ]
 
 setup(
     name='planetmint_driver',
-    version='0.9.1',
+    version='0.9.4',
     description="Python driver for Planetmint",
     long_description=readme + '\n\n' + changelog,
     long_description_content_type='text/x-rst',
     author="Planetmint",
     author_email='contact@ipdb.global',
     url='https://github.com/planetmint/planetmint-driver',
     packages=find_packages(exclude=['tests*']),
```

### Comparing `planetmint_driver-0.9.1/tests/conftest.py` & `planetmint_driver-0.9.4/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,14 +240,21 @@
 @fixture
 def signed_alice_transaction(alice_privkey, alice_transaction_obj):
     signed_transaction = alice_transaction_obj.sign([alice_privkey])
     return signed_transaction.to_dict()
 
 
 @fixture
+def alice_transaction_signature(signed_alice_transaction):
+    return Ed25519Sha256.from_uri(
+        signed_alice_transaction['inputs'][0]['fulfillment']
+    ).signature
+
+
+@fixture
 def persisted_alice_transaction(signed_alice_transaction,
                                 transactions_api_full_url):
     response = requests.post(transactions_api_full_url,
                              json=signed_alice_transaction)
     return response.json()
```

### Comparing `planetmint_driver-0.9.1/tests/test_connection.py` & `planetmint_driver-0.9.4/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/tests/test_driver.py` & `planetmint_driver-0.9.4/tests/test_driver.py`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/tests/test_exceptions.py` & `planetmint_driver-0.9.4/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/tests/test_offchain.py` & `planetmint_driver-0.9.4/tests/test_offchain.py`

 * *Files 14% similar despite different names*

```diff
@@ -129,7 +129,27 @@
 
 
 def test_fulfill_transaction_raises(alice_transaction, bob_privkey):
     from planetmint_driver.offchain import fulfill_transaction
     from planetmint_driver.exceptions import MissingPrivateKeyError
     with raises(MissingPrivateKeyError):
         fulfill_transaction(alice_transaction, private_keys=bob_privkey)
+
+
+def test_transaction_fulfill_with_signingning_delegation(
+        alice_privkey,
+        alice_transaction,
+        alice_transaction_signature):
+    from planetmint_driver.offchain import (
+        fulfill_transaction,
+        fulfill_with_signing_delegation
+    )
+
+    fulfilled_transaction = fulfill_transaction(
+        alice_transaction,
+        private_keys=alice_privkey)
+
+    fulfilled_transaction_with_delegation = fulfill_with_signing_delegation(
+        alice_transaction,
+        lambda x, y: alice_transaction_signature)
+
+    assert fulfilled_transaction == fulfilled_transaction_with_delegation
```

### Comparing `planetmint_driver-0.9.1/tests/test_pool.py` & `planetmint_driver-0.9.4/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/tests/test_transport.py` & `planetmint_driver-0.9.4/tests/test_transport.py`

 * *Files identical despite different names*

### Comparing `planetmint_driver-0.9.1/tests/test_utils.py` & `planetmint_driver-0.9.4/tests/test_utils.py`

 * *Files identical despite different names*

