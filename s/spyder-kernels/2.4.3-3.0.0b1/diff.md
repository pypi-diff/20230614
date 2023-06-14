# Comparing `tmp/spyder-kernels-2.4.3.tar.gz` & `tmp/spyder-kernels-3.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyder-kernels-2.4.3.tar", last modified: Sun Apr  2 18:29:38 2023, max compression
+gzip compressed data, was "spyder-kernels-3.0.0b1.tar", last modified: Wed Jun 14 03:22:05 2023, max compression
```

## Comparing `spyder-kernels-2.4.3.tar` & `spyder-kernels-3.0.0b1.tar`

### file list

```diff
@@ -1,84 +1,85 @@
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-02 18:29:38.190342 spyder-kernels-2.4.3/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      314 2019-12-29 23:57:49.000000 spyder-kernels-2.4.3/.codecov.yml
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      269 2019-02-03 15:33:04.000000 spyder-kernels-2.4.3/.coveragerc
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4930 2018-08-07 19:28:05.000000 spyder-kernels-2.4.3/.gitattributes
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-02 18:29:38.178341 spyder-kernels-2.4.3/.github/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       24 2021-04-02 18:19:53.000000 spyder-kernels-2.4.3/.github/FUNDING.yml
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-02 18:29:38.178341 spyder-kernels-2.4.3/.github/workflows/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1865 2023-04-02 18:24:49.000000 spyder-kernels-2.4.3/.github/workflows/linux-pip-tests.yml
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2203 2023-04-02 18:24:49.000000 spyder-kernels-2.4.3/.github/workflows/linux-tests.yml
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1799 2023-04-02 18:24:49.000000 spyder-kernels-2.4.3/.github/workflows/macos-tests.yml
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1694 2023-02-20 16:51:15.000000 spyder-kernels-2.4.3/.github/workflows/windows-tests.yml
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      363 2019-12-29 23:57:49.000000 spyder-kernels-2.4.3/.gitignore
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      891 2018-08-07 19:28:05.000000 spyder-kernels-2.4.3/AUTHORS.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    61395 2023-04-02 18:27:42.000000 spyder-kernels-2.4.3/CHANGELOG.md
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1103 2018-08-07 19:28:05.000000 spyder-kernels-2.4.3/LICENSE.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       79 2019-07-11 12:23:54.000000 spyder-kernels-2.4.3/MANIFEST.in
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3960 2023-04-02 18:29:38.190342 spyder-kernels-2.4.3/PKG-INFO
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2827 2023-04-02 18:24:49.000000 spyder-kernels-2.4.3/README.md
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      727 2021-06-12 22:37:24.000000 spyder-kernels-2.4.3/RELEASE.md
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-02 18:29:38.178341 spyder-kernels-2.4.3/requirements/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      108 2023-04-02 18:24:49.000000 spyder-kernels-2.4.3/requirements/posix.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      211 2023-04-02 18:24:49.000000 spyder-kernels-2.4.3/requirements/python-27.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      100 2022-10-03 09:12:17.000000 spyder-kernels-2.4.3/requirements/tests.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       91 2023-03-28 21:53:50.000000 spyder-kernels-2.4.3/requirements/windows.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       67 2023-04-02 18:29:38.190342 spyder-kernels-2.4.3/setup.cfg
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3208 2023-04-02 18:24:49.000000 spyder-kernels-2.4.3/setup.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-02 18:29:38.178341 spyder-kernels-2.4.3/spyder_kernels/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1476 2018-08-07 19:28:05.000000 spyder-kernels-2.4.3/spyder_kernels/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      401 2023-04-02 18:28:50.000000 spyder-kernels-2.4.3/spyder_kernels/_version.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-02 18:29:38.182341 spyder-kernels-2.4.3/spyder_kernels/comms/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1540 2019-12-29 23:57:49.000000 spyder-kernels-2.4.3/spyder_kernels/comms/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    18501 2023-04-02 18:24:49.000000 spyder-kernels-2.4.3/spyder_kernels/comms/commbase.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    11098 2023-04-02 18:24:49.000000 spyder-kernels-2.4.3/spyder_kernels/comms/frontendcomm.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-02 18:29:38.182341 spyder-kernels-2.4.3/spyder_kernels/console/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      353 2018-08-07 19:28:05.000000 spyder-kernels-2.4.3/spyder_kernels/console/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1023 2021-11-22 19:09:05.000000 spyder-kernels-2.4.3/spyder_kernels/console/__main__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    30967 2023-04-02 18:24:49.000000 spyder-kernels-2.4.3/spyder_kernels/console/kernel.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      731 2021-07-28 17:22:20.000000 spyder-kernels-2.4.3/spyder_kernels/console/outstream.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3389 2023-04-02 18:24:49.000000 spyder-kernels-2.4.3/spyder_kernels/console/shell.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    10967 2023-04-02 18:24:49.000000 spyder-kernels-2.4.3/spyder_kernels/console/start.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-02 18:29:38.182341 spyder-kernels-2.4.3/spyder_kernels/console/tests/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2018-08-23 02:20:23.000000 spyder-kernels-2.4.3/spyder_kernels/console/tests/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      270 2020-02-28 19:57:03.000000 spyder-kernels-2.4.3/spyder_kernels/console/tests/load_data.npz
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    10240 2019-01-26 09:49:54.000000 spyder-kernels-2.4.3/spyder_kernels/console/tests/load_data.spydata
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    40006 2023-04-02 18:24:49.000000 spyder-kernels-2.4.3/spyder_kernels/console/tests/test_console_kernel.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-02 18:29:38.186342 spyder-kernels-2.4.3/spyder_kernels/customize/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      511 2018-08-07 19:28:05.000000 spyder-kernels-2.4.3/spyder_kernels/customize/__init__.py
--rwxrwxr-x   0 carlos    (1000) carlos    (1000)     4657 2023-04-02 18:24:49.000000 spyder-kernels-2.4.3/spyder_kernels/customize/namespace_manager.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    28522 2023-04-02 18:24:49.000000 spyder-kernels-2.4.3/spyder_kernels/customize/spydercustomize.py
--rwxrwxr-x   0 carlos    (1000) carlos    (1000)    34926 2023-04-02 18:24:49.000000 spyder-kernels-2.4.3/spyder_kernels/customize/spyderpdb.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-02 18:29:38.186342 spyder-kernels-2.4.3/spyder_kernels/customize/tests/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      363 2019-02-03 15:33:04.000000 spyder-kernels-2.4.3/spyder_kernels/customize/tests/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3074 2023-04-02 18:24:49.000000 spyder-kernels-2.4.3/spyder_kernels/customize/tests/test_umr.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      820 2023-02-20 16:51:15.000000 spyder-kernels-2.4.3/spyder_kernels/customize/tests/test_utils.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4901 2023-04-02 18:24:49.000000 spyder-kernels-2.4.3/spyder_kernels/customize/umr.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4514 2023-04-02 18:24:49.000000 spyder-kernels-2.4.3/spyder_kernels/customize/utils.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     9786 2023-04-02 18:24:49.000000 spyder-kernels-2.4.3/spyder_kernels/py3compat.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-02 18:29:38.186342 spyder-kernels-2.4.3/spyder_kernels/utils/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      348 2018-08-07 19:28:05.000000 spyder-kernels-2.4.3/spyder_kernels/utils/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    11924 2023-04-02 18:24:49.000000 spyder-kernels-2.4.3/spyder_kernels/utils/dochelpers.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    19217 2023-04-02 18:24:49.000000 spyder-kernels-2.4.3/spyder_kernels/utils/iofuncs.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2110 2023-04-02 18:24:49.000000 spyder-kernels-2.4.3/spyder_kernels/utils/lazymodules.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1579 2023-04-02 18:24:49.000000 spyder-kernels-2.4.3/spyder_kernels/utils/misc.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1351 2022-03-30 02:02:02.000000 spyder-kernels-2.4.3/spyder_kernels/utils/mpl.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    25417 2023-04-02 18:24:49.000000 spyder-kernels-2.4.3/spyder_kernels/utils/nsview.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1425 2019-08-05 17:14:47.000000 spyder-kernels-2.4.3/spyder_kernels/utils/test_utils.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-02 18:29:38.190342 spyder-kernels-2.4.3/spyder_kernels/utils/tests/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      343 2018-08-07 19:28:05.000000 spyder-kernels-2.4.3/spyder_kernels/utils/tests/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      482 2018-06-18 15:46:26.000000 spyder-kernels-2.4.3/spyder_kernels/utils/tests/data.mat
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    20480 2023-02-20 16:51:47.000000 spyder-kernels-2.4.3/spyder_kernels/utils/tests/export_data.spydata
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    20480 2023-02-20 16:51:47.000000 spyder-kernels-2.4.3/spyder_kernels/utils/tests/export_data_renamed.spydata
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    10240 2019-01-26 09:50:47.000000 spyder-kernels-2.4.3/spyder_kernels/utils/tests/export_data_withfunction.spydata
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      270 2020-02-28 19:57:03.000000 spyder-kernels-2.4.3/spyder_kernels/utils/tests/import_data.npz
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1301 2018-06-18 15:46:26.000000 spyder-kernels-2.4.3/spyder_kernels/utils/tests/numpy_data.npz
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1930 2023-04-02 18:24:49.000000 spyder-kernels-2.4.3/spyder_kernels/utils/tests/test_dochelpers.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    11525 2023-04-02 18:24:49.000000 spyder-kernels-2.4.3/spyder_kernels/utils/tests/test_iofuncs.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1257 2021-07-28 13:28:52.000000 spyder-kernels-2.4.3/spyder_kernels/utils/tests/test_lazymodules.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    14130 2023-04-02 18:24:49.000000 spyder-kernels-2.4.3/spyder_kernels/utils/tests/test_nsview.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-02 18:29:38.178341 spyder-kernels-2.4.3/spyder_kernels.egg-info/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3960 2023-04-02 18:29:38.000000 spyder-kernels-2.4.3/spyder_kernels.egg-info/PKG-INFO
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2280 2023-04-02 18:29:38.000000 spyder-kernels-2.4.3/spyder_kernels.egg-info/SOURCES.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2023-04-02 18:29:38.000000 spyder-kernels-2.4.3/spyder_kernels.egg-info/dependency_links.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      447 2023-04-02 18:29:38.000000 spyder-kernels-2.4.3/spyder_kernels.egg-info/requires.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       15 2023-04-02 18:29:38.000000 spyder-kernels-2.4.3/spyder_kernels.egg-info/top_level.txt
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-06-14 03:22:05.381071 spyder-kernels-3.0.0b1/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      314 2019-12-29 23:57:49.000000 spyder-kernels-3.0.0b1/.codecov.yml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      269 2019-02-03 15:33:04.000000 spyder-kernels-3.0.0b1/.coveragerc
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4930 2018-08-07 19:28:05.000000 spyder-kernels-3.0.0b1/.gitattributes
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-06-14 03:22:05.365071 spyder-kernels-3.0.0b1/.github/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       24 2021-04-02 18:19:53.000000 spyder-kernels-3.0.0b1/.github/FUNDING.yml
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-06-14 03:22:05.365071 spyder-kernels-3.0.0b1/.github/workflows/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1856 2023-06-14 03:07:28.000000 spyder-kernels-3.0.0b1/.github/workflows/linux-pip-tests.yml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2071 2023-06-14 03:07:28.000000 spyder-kernels-3.0.0b1/.github/workflows/linux-tests.yml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1863 2023-06-14 03:07:28.000000 spyder-kernels-3.0.0b1/.github/workflows/macos-tests.yml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1862 2023-04-15 18:12:27.000000 spyder-kernels-3.0.0b1/.github/workflows/windows-tests.yml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      363 2019-12-29 23:57:49.000000 spyder-kernels-3.0.0b1/.gitignore
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      891 2018-08-07 19:28:05.000000 spyder-kernels-3.0.0b1/AUTHORS.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    66257 2023-06-14 03:14:39.000000 spyder-kernels-3.0.0b1/CHANGELOG.md
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1103 2018-08-07 19:28:05.000000 spyder-kernels-3.0.0b1/LICENSE.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       79 2019-07-11 12:23:54.000000 spyder-kernels-3.0.0b1/MANIFEST.in
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3891 2023-06-14 03:22:05.381071 spyder-kernels-3.0.0b1/PKG-INFO
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2830 2023-06-14 03:07:28.000000 spyder-kernels-3.0.0b1/README.md
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      727 2021-06-12 22:37:24.000000 spyder-kernels-3.0.0b1/RELEASE.md
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-06-14 03:22:05.365071 spyder-kernels-3.0.0b1/requirements/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      120 2023-06-14 03:07:28.000000 spyder-kernels-3.0.0b1/requirements/posix.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      105 2023-06-14 03:07:28.000000 spyder-kernels-3.0.0b1/requirements/tests.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       91 2023-06-14 03:07:28.000000 spyder-kernels-3.0.0b1/requirements/windows.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       38 2023-06-14 03:22:05.381071 spyder-kernels-3.0.0b1/setup.cfg
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2869 2023-06-14 03:07:28.000000 spyder-kernels-3.0.0b1/setup.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-06-14 03:22:05.369071 spyder-kernels-3.0.0b1/spyder_kernels/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1476 2018-08-07 19:28:05.000000 spyder-kernels-3.0.0b1/spyder_kernels/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      405 2023-06-14 03:19:15.000000 spyder-kernels-3.0.0b1/spyder_kernels/_version.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-06-14 03:22:05.369071 spyder-kernels-3.0.0b1/spyder_kernels/comms/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1540 2019-12-29 23:57:49.000000 spyder-kernels-3.0.0b1/spyder_kernels/comms/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    17579 2023-06-14 03:07:28.000000 spyder-kernels-3.0.0b1/spyder_kernels/comms/commbase.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     7462 2023-06-14 03:07:28.000000 spyder-kernels-3.0.0b1/spyder_kernels/comms/frontendcomm.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2513 2023-06-14 03:07:28.000000 spyder-kernels-3.0.0b1/spyder_kernels/comms/utils.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-06-14 03:22:05.369071 spyder-kernels-3.0.0b1/spyder_kernels/console/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      353 2018-08-07 19:28:05.000000 spyder-kernels-3.0.0b1/spyder_kernels/console/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1023 2021-11-22 19:09:05.000000 spyder-kernels-3.0.0b1/spyder_kernels/console/__main__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    34596 2023-06-14 03:07:28.000000 spyder-kernels-3.0.0b1/spyder_kernels/console/kernel.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      731 2021-07-28 17:22:20.000000 spyder-kernels-3.0.0b1/spyder_kernels/console/outstream.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    13159 2023-06-14 03:07:28.000000 spyder-kernels-3.0.0b1/spyder_kernels/console/shell.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    10827 2023-06-14 03:07:28.000000 spyder-kernels-3.0.0b1/spyder_kernels/console/start.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-06-14 03:22:05.369071 spyder-kernels-3.0.0b1/spyder_kernels/console/tests/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2018-08-23 02:20:23.000000 spyder-kernels-3.0.0b1/spyder_kernels/console/tests/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      270 2020-02-28 19:57:03.000000 spyder-kernels-3.0.0b1/spyder_kernels/console/tests/load_data.npz
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    10240 2019-01-26 09:49:54.000000 spyder-kernels-3.0.0b1/spyder_kernels/console/tests/load_data.spydata
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    45052 2023-06-14 03:07:28.000000 spyder-kernels-3.0.0b1/spyder_kernels/console/tests/test_console_kernel.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-06-14 03:22:05.373071 spyder-kernels-3.0.0b1/spyder_kernels/customize/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      511 2018-08-07 19:28:05.000000 spyder-kernels-3.0.0b1/spyder_kernels/customize/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    20441 2023-06-14 03:07:28.000000 spyder-kernels-3.0.0b1/spyder_kernels/customize/code_runner.py
+-rwxrwxr-x   0 carlos    (1000) carlos    (1000)     4195 2023-06-14 03:07:28.000000 spyder-kernels-3.0.0b1/spyder_kernels/customize/namespace_manager.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     9773 2023-06-14 03:07:28.000000 spyder-kernels-3.0.0b1/spyder_kernels/customize/spydercustomize.py
+-rwxrwxr-x   0 carlos    (1000) carlos    (1000)    32111 2023-06-14 03:07:28.000000 spyder-kernels-3.0.0b1/spyder_kernels/customize/spyderpdb.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-06-14 03:22:05.373071 spyder-kernels-3.0.0b1/spyder_kernels/customize/tests/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      363 2019-02-03 15:33:04.000000 spyder-kernels-3.0.0b1/spyder_kernels/customize/tests/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3000 2023-06-14 03:07:28.000000 spyder-kernels-3.0.0b1/spyder_kernels/customize/tests/test_umr.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      820 2023-02-20 16:51:15.000000 spyder-kernels-3.0.0b1/spyder_kernels/customize/tests/test_utils.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4722 2023-06-14 03:07:28.000000 spyder-kernels-3.0.0b1/spyder_kernels/customize/umr.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4664 2023-06-14 03:07:28.000000 spyder-kernels-3.0.0b1/spyder_kernels/customize/utils.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-06-14 03:22:05.377071 spyder-kernels-3.0.0b1/spyder_kernels/utils/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      348 2018-08-07 19:28:05.000000 spyder-kernels-3.0.0b1/spyder_kernels/utils/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    11290 2023-06-14 03:07:28.000000 spyder-kernels-3.0.0b1/spyder_kernels/utils/dochelpers.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    21324 2023-06-14 03:07:28.000000 spyder-kernels-3.0.0b1/spyder_kernels/utils/iofuncs.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2094 2023-06-14 03:07:28.000000 spyder-kernels-3.0.0b1/spyder_kernels/utils/lazymodules.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1564 2023-06-14 03:07:28.000000 spyder-kernels-3.0.0b1/spyder_kernels/utils/misc.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1351 2022-03-30 02:02:02.000000 spyder-kernels-3.0.0b1/spyder_kernels/utils/mpl.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    24326 2023-06-14 03:07:28.000000 spyder-kernels-3.0.0b1/spyder_kernels/utils/nsview.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1425 2019-08-05 17:14:47.000000 spyder-kernels-3.0.0b1/spyder_kernels/utils/test_utils.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-06-14 03:22:05.381071 spyder-kernels-3.0.0b1/spyder_kernels/utils/tests/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      343 2018-08-07 19:28:05.000000 spyder-kernels-3.0.0b1/spyder_kernels/utils/tests/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)   138515 2023-06-14 03:07:28.000000 spyder-kernels-3.0.0b1/spyder_kernels/utils/tests/data.dcm
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      482 2018-06-18 15:46:26.000000 spyder-kernels-3.0.0b1/spyder_kernels/utils/tests/data.mat
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    20480 2023-02-20 16:51:47.000000 spyder-kernels-3.0.0b1/spyder_kernels/utils/tests/export_data.spydata
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    20480 2023-02-20 16:51:47.000000 spyder-kernels-3.0.0b1/spyder_kernels/utils/tests/export_data_renamed.spydata
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    10240 2019-01-26 09:50:47.000000 spyder-kernels-3.0.0b1/spyder_kernels/utils/tests/export_data_withfunction.spydata
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      270 2020-02-28 19:57:03.000000 spyder-kernels-3.0.0b1/spyder_kernels/utils/tests/import_data.npz
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1301 2018-06-18 15:46:26.000000 spyder-kernels-3.0.0b1/spyder_kernels/utils/tests/numpy_data.npz
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1877 2023-06-14 03:07:28.000000 spyder-kernels-3.0.0b1/spyder_kernels/utils/tests/test_dochelpers.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    12120 2023-06-14 03:07:28.000000 spyder-kernels-3.0.0b1/spyder_kernels/utils/tests/test_iofuncs.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1257 2021-07-28 13:28:52.000000 spyder-kernels-3.0.0b1/spyder_kernels/utils/tests/test_lazymodules.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    13727 2023-06-14 03:07:28.000000 spyder-kernels-3.0.0b1/spyder_kernels/utils/tests/test_nsview.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-06-14 03:22:05.369071 spyder-kernels-3.0.0b1/spyder_kernels.egg-info/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3891 2023-06-14 03:22:05.000000 spyder-kernels-3.0.0b1/spyder_kernels.egg-info/PKG-INFO
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2321 2023-06-14 03:22:05.000000 spyder-kernels-3.0.0b1/spyder_kernels.egg-info/SOURCES.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2023-06-14 03:22:05.000000 spyder-kernels-3.0.0b1/spyder_kernels.egg-info/dependency_links.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      362 2023-06-14 03:22:05.000000 spyder-kernels-3.0.0b1/spyder_kernels.egg-info/requires.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       15 2023-06-14 03:22:05.000000 spyder-kernels-3.0.0b1/spyder_kernels.egg-info/top_level.txt
```

### Comparing `spyder-kernels-2.4.3/.gitattributes` & `spyder-kernels-3.0.0b1/.gitattributes`

 * *Files identical despite different names*

### Comparing `spyder-kernels-2.4.3/.github/workflows/linux-pip-tests.yml` & `spyder-kernels-3.0.0b1/.github/workflows/linux-tests.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,72 @@
-name: Linux pip tests
+name: Linux tests
 
 on:
   push:
     branches:
     - master
     - 2.*
   pull_request:
     branches:
     - master
     - 2.*
 
 concurrency:
-  group: linux-pip-tests-${{ github.ref }}
+  group: linux-tests-${{ github.ref }}
   cancel-in-progress: true
 
 jobs:
   linux:
     name: Py${{ matrix.PYTHON_VERSION }}
     runs-on: ubuntu-latest
     env:
       CI: True
       PYTHON_VERSION: ${{ matrix.PYTHON_VERSION }}
       RUNNER_OS: 'ubuntu'
+      USE_CONDA: 'true'
     strategy:
       fail-fast: false 
       matrix:
-        PYTHON_VERSION: ['2.7', '3.7', '3.8', '3.9']
+        PYTHON_VERSION: ['3.8', '3.9', '3.10']
     timeout-minutes: 20
     steps:
       - name: Checkout branch
         uses: actions/checkout@v1
       - name: Install System Packages
         run: | 
           sudo apt-get update
           sudo apt-get install libegl1-mesa
       - name: Install Conda
         uses: conda-incubator/setup-miniconda@v2
         with:
            activate-environment: test
-           auto-update-conda: false
+           auto-update-conda: true
            auto-activate-base: false
+           channels: conda-forge
+           miniforge-variant: Mambaforge
            python-version: ${{ matrix.PYTHON_VERSION }} 
-      - name: Install package and dependencies
+      - name: Install package dependencies
         shell: bash -l {0}
         run: |
-          pip install -e .[test]
-          # Zict 2.1.0 is not compatible with Python 3
-          pip install zict==2.0.0
+          mamba install --file requirements/posix.txt -y -q
+      - name: Install test dependencies
+        shell: bash -l {0}
+        run: mamba install --file requirements/tests.txt -y -q
+      - name: Install Package
+        shell: bash -l {0}
+        run: pip install -e .
       - name: Show environment information
         shell: bash -l {0}
         run: |
           conda info
           conda list
       - name: Run tests
         shell: bash -l {0}
         run: |
-          xvfb-run --auto-servernum pytest spyder_kernels --color=yes --cov=spyder_kernels -x -vv || \
-          xvfb-run --auto-servernum pytest spyder_kernels --color=yes --cov=spyder_kernels -x -vv || \
-          xvfb-run --auto-servernum pytest spyder_kernels --color=yes --cov=spyder_kernels -x -vv
+          xvfb-run --auto-servernum pytest spyder_kernels --color=yes --cov=spyder_kernels -vv || \
+          xvfb-run --auto-servernum pytest spyder_kernels --color=yes --cov=spyder_kernels -vv || \
+          xvfb-run --auto-servernum pytest spyder_kernels --color=yes --cov=spyder_kernels -vv
       - name: Upload coverage to Codecov
-        if: matrix.PYTHON_VERSION == '3.8'
-        shell: bash -l {0}
-        run: codecov -t 02fa9892-fa7f-4cf8-ac3c-d54143ddc933
+        uses: codecov/codecov-action@v3
+        with:
+          fail_ci_if_error: false
+          verbose: true
```

### Comparing `spyder-kernels-2.4.3/.github/workflows/linux-tests.yml` & `spyder-kernels-3.0.0b1/.github/workflows/macos-tests.yml`

 * *Files 25% similar despite different names*

```diff
@@ -1,71 +1,68 @@
-name: Linux tests
+name: Macos tests
 
 on:
   push:
     branches:
     - master
     - 2.*
   pull_request:
     branches:
     - master
     - 2.*
 
 concurrency:
-  group: linux-tests-${{ github.ref }}
+  group: macos-tests-${{ github.ref }}
   cancel-in-progress: true
 
 jobs:
-  linux:
+  macos:
     name: Py${{ matrix.PYTHON_VERSION }}
-    runs-on: ubuntu-latest
+    runs-on: macos-latest
     env:
       CI: True
       PYTHON_VERSION: ${{ matrix.PYTHON_VERSION }}
-      RUNNER_OS: 'ubuntu'
+      RUNNER_OS: 'macos'
       USE_CONDA: 'true'
     strategy:
       fail-fast: false 
       matrix:
         PYTHON_VERSION: ['3.8', '3.9', '3.10']
-    timeout-minutes: 20
+    timeout-minutes: 25
     steps:
       - name: Checkout branch
         uses: actions/checkout@v1
-      - name: Install System Packages
-        run: | 
-          sudo apt-get update
-          sudo apt-get install libegl1-mesa
       - name: Install Conda
         uses: conda-incubator/setup-miniconda@v2
         with:
            activate-environment: test
            auto-update-conda: true
            auto-activate-base: false
            channels: conda-forge
            miniforge-variant: Mambaforge
            python-version: ${{ matrix.PYTHON_VERSION }} 
       - name: Install package dependencies
         shell: bash -l {0}
         run: |
-          if [ "$PYTHON_VERSION" != "2.7" ]; then mamba install --file requirements/posix.txt -y -q; else mamba install --file requirements/python-27.txt -y -q; fi
+          mamba install --file requirements/posix.txt -y -q
       - name: Install test dependencies
         shell: bash -l {0}
         run: mamba install --file requirements/tests.txt -y -q
       - name: Install Package
         shell: bash -l {0}
         run: pip install -e .
       - name: Show environment information
         shell: bash -l {0}
         run: |
           conda info
           conda list
       - name: Run tests
         shell: bash -l {0}
         run: |
-          xvfb-run --auto-servernum pytest spyder_kernels --color=yes --cov=spyder_kernels -x -vv || \
-          xvfb-run --auto-servernum pytest spyder_kernels --color=yes --cov=spyder_kernels -x -vv || \
-          xvfb-run --auto-servernum pytest spyder_kernels --color=yes --cov=spyder_kernels -x -vv
+          pytest spyder_kernels --color=yes --cov=spyder_kernels -vv || \
+          pytest spyder_kernels --color=yes --cov=spyder_kernels -vv || \
+          pytest spyder_kernels --color=yes --cov=spyder_kernels -vv
       - name: Upload coverage to Codecov
-        if: matrix.PYTHON_VERSION == '3.8'
-        shell: bash -l {0}
-        run: codecov -t 02fa9892-fa7f-4cf8-ac3c-d54143ddc933
+        uses: codecov/codecov-action@v3
+        with:
+          fail_ci_if_error: false
+          verbose: true
```

### Comparing `spyder-kernels-2.4.3/.github/workflows/macos-tests.yml` & `spyder-kernels-3.0.0b1/.github/workflows/linux-pip-tests.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,66 @@
-name: Macos tests
+name: Linux pip tests
 
 on:
   push:
     branches:
     - master
     - 2.*
   pull_request:
     branches:
     - master
     - 2.*
 
 concurrency:
-  group: macos-tests-${{ github.ref }}
+  group: linux-pip-tests-${{ github.ref }}
   cancel-in-progress: true
 
 jobs:
-  macos:
+  linux:
     name: Py${{ matrix.PYTHON_VERSION }}
-    runs-on: macos-latest
+    runs-on: ubuntu-latest
     env:
       CI: True
       PYTHON_VERSION: ${{ matrix.PYTHON_VERSION }}
-      RUNNER_OS: 'macos'
+      RUNNER_OS: 'ubuntu'
+      USE_CONDA: 'false'
     strategy:
       fail-fast: false 
       matrix:
         PYTHON_VERSION: ['3.8', '3.9', '3.10']
-    timeout-minutes: 25
+    timeout-minutes: 20
     steps:
       - name: Checkout branch
         uses: actions/checkout@v1
+      - name: Install System Packages
+        run: | 
+          sudo apt-get update
+          sudo apt-get install libegl1-mesa
       - name: Install Conda
         uses: conda-incubator/setup-miniconda@v2
         with:
            activate-environment: test
-           auto-update-conda: true
+           auto-update-conda: false
            auto-activate-base: false
-           channels: conda-forge
-           miniforge-variant: Mambaforge
            python-version: ${{ matrix.PYTHON_VERSION }} 
-      - name: Install package dependencies
+      - name: Install package and dependencies
         shell: bash -l {0}
         run: |
-          if [ "$PYTHON_VERSION" != "2.7" ]; then mamba install --file requirements/posix.txt -y -q; else mamba install --file requirements/python-27.txt -y -q; fi
-      - name: Install test dependencies
-        shell: bash -l {0}
-        run: mamba install --file requirements/tests.txt -y -q
-      - name: Install Package
-        shell: bash -l {0}
-        run: pip install -e .
+          pip install -e .[test]
+          # Zict 2.1.0 is not compatible with Python 3
+          pip install zict==2.0.0
       - name: Show environment information
         shell: bash -l {0}
         run: |
           conda info
           conda list
       - name: Run tests
         shell: bash -l {0}
         run: |
-          pytest spyder_kernels --color=yes --cov=spyder_kernels -x -vv || \
-          pytest spyder_kernels --color=yes --cov=spyder_kernels -x -vv || \
-          pytest spyder_kernels --color=yes --cov=spyder_kernels -x -vv
+          xvfb-run --auto-servernum pytest spyder_kernels --color=yes --cov=spyder_kernels -vv || \
+          xvfb-run --auto-servernum pytest spyder_kernels --color=yes --cov=spyder_kernels -vv || \
+          xvfb-run --auto-servernum pytest spyder_kernels --color=yes --cov=spyder_kernels -vv
+      - name: Upload coverage to Codecov
+        uses: codecov/codecov-action@v3
+        with:
+          fail_ci_if_error: false
+          verbose: true
```

### Comparing `spyder-kernels-2.4.3/.github/workflows/windows-tests.yml` & `spyder-kernels-3.0.0b1/.github/workflows/windows-tests.yml`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
   windows:
     name: Py${{ matrix.PYTHON_VERSION }}
     runs-on: windows-latest
     env:
       CI: True
       PYTHON_VERSION: ${{ matrix.PYTHON_VERSION }}
       RUNNER_OS: 'windows'
+      USE_CONDA: 'true'
     strategy:
       fail-fast: false 
       matrix:
         PYTHON_VERSION: ['3.8', '3.9', '3.10']
     timeout-minutes: 25
     steps:
       - name: Checkout branch
@@ -53,10 +54,15 @@
         shell: bash -l {0}
         run: |
           conda info
           conda list
       - name: Run tests
         shell: bash -l {0}
         run: |
-          pytest spyder_kernels --color=yes --cov=spyder_kernels -x -vv || \
-          pytest spyder_kernels --color=yes --cov=spyder_kernels -x -vv || \
-          pytest spyder_kernels --cov=spyder_kernels -x -vv
+          pytest spyder_kernels --color=yes --cov=spyder_kernels -vv || \
+          pytest spyder_kernels --color=yes --cov=spyder_kernels -vv || \
+          pytest spyder_kernels --cov=spyder_kernels -vv
+      - name: Upload coverage to Codecov
+        uses: codecov/codecov-action@v3
+        with:
+          fail_ci_if_error: false
+          verbose: true
```

### Comparing `spyder-kernels-2.4.3/AUTHORS.txt` & `spyder-kernels-3.0.0b1/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `spyder-kernels-2.4.3/CHANGELOG.md` & `spyder-kernels-3.0.0b1/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,52 @@
 # History of changes
 
+## Version 3.0.0b1 (2023-06-14)
+
+### Issues Closed
+
+* [Issue 425](https://github.com/spyder-ide/spyder-kernels/issues/425) - Possible minor issues related to post mortem debugging ([PR 444](https://github.com/spyder-ide/spyder-kernels/pull/444) by [@impact27](https://github.com/impact27))
+* [Issue 340](https://github.com/spyder-ide/spyder-kernels/issues/340) - Drop support for Python 2 ([PR 341](https://github.com/spyder-ide/spyder-kernels/pull/341) by [@impact27](https://github.com/impact27))
+
+In this release 2 issues were closed.
+
+### Pull Requests Merged
+
+* [PR 456](https://github.com/spyder-ide/spyder-kernels/pull/456) - PR: Remove unnecessary code for old IPykernel versions in our tests, by [@ccordoba12](https://github.com/ccordoba12)
+* [PR 453](https://github.com/spyder-ide/spyder-kernels/pull/453) - PR: Move code that loads and saves HDF5 and DICOM files from Spyder, by [@ccordoba12](https://github.com/ccordoba12)
+* [PR 447](https://github.com/spyder-ide/spyder-kernels/pull/447) - PR: Create magics for run|debug file|cell, by [@impact27](https://github.com/impact27)
+* [PR 446](https://github.com/spyder-ide/spyder-kernels/pull/446) - PR: Make call to interrupt children processes work for IPykernel greater than 6.21.2, by [@ccordoba12](https://github.com/ccordoba12)
+* [PR 444](https://github.com/spyder-ide/spyder-kernels/pull/444) - PR: Fix post mortem for debugging, by [@impact27](https://github.com/impact27) ([425](https://github.com/spyder-ide/spyder-kernels/issues/425))
+* [PR 443](https://github.com/spyder-ide/spyder-kernels/pull/443) - PR: Fix small typo in Readme, by [@davidbrochart](https://github.com/davidbrochart)
+* [PR 437](https://github.com/spyder-ide/spyder-kernels/pull/437) - PR: Remove imports from __future__, by [@oscargus](https://github.com/oscargus)
+* [PR 421](https://github.com/spyder-ide/spyder-kernels/pull/421) - PR: Update variable explorer from the kernel, by [@impact27](https://github.com/impact27)
+* [PR 417](https://github.com/spyder-ide/spyder-kernels/pull/417) - PR: Fix error in `globalsfilter`, by [@ccordoba12](https://github.com/ccordoba12)
+* [PR 412](https://github.com/spyder-ide/spyder-kernels/pull/412) - PR: Use temporary file for faulthandler and make sure iopub is open for comms, by [@impact27](https://github.com/impact27)
+* [PR 409](https://github.com/spyder-ide/spyder-kernels/pull/409) - PR: Add Python executable as part of kernel info, by [@impact27](https://github.com/impact27)
+* [PR 408](https://github.com/spyder-ide/spyder-kernels/pull/408) - PR: Expose package version in SpyderShell, by [@impact27](https://github.com/impact27)
+* [PR 403](https://github.com/spyder-ide/spyder-kernels/pull/403) - PR: Make debugger faster by avoiding unnecessary comm messages, by [@impact27](https://github.com/impact27)
+* [PR 401](https://github.com/spyder-ide/spyder-kernels/pull/401) - PR: Wait for connection file to be written, by [@impact27](https://github.com/impact27)
+* [PR 400](https://github.com/spyder-ide/spyder-kernels/pull/400) - PR: Use `execute_interactive` to print errors during tests, by [@impact27](https://github.com/impact27)
+* [PR 397](https://github.com/spyder-ide/spyder-kernels/pull/397) - PR: Remove Python 2 code introduced when merging PR #395, by [@impact27](https://github.com/impact27)
+* [PR 396](https://github.com/spyder-ide/spyder-kernels/pull/396) - PR: Add handlers to interrupt executions and enter the debugger after that, by [@impact27](https://github.com/impact27)
+* [PR 390](https://github.com/spyder-ide/spyder-kernels/pull/390) - PR: Filter comm socket thread, by [@impact27](https://github.com/impact27)
+* [PR 387](https://github.com/spyder-ide/spyder-kernels/pull/387) - PR: Minor changes to finish the migration to Python 3, by [@ccordoba12](https://github.com/ccordoba12)
+* [PR 366](https://github.com/spyder-ide/spyder-kernels/pull/366) - PR: Print warning when using `global` in an empty namespace, by [@impact27](https://github.com/impact27)
+* [PR 341](https://github.com/spyder-ide/spyder-kernels/pull/341) - PR: Drop support for Python 2, by [@impact27](https://github.com/impact27) ([340](https://github.com/spyder-ide/spyder-kernels/issues/340))
+* [PR 339](https://github.com/spyder-ide/spyder-kernels/pull/339) - PR: Use control channel for comms, by [@impact27](https://github.com/impact27)
+* [PR 286](https://github.com/spyder-ide/spyder-kernels/pull/286) - PR: Improve and refactor the way we run and debug code, by [@impact27](https://github.com/impact27)
+* [PR 257](https://github.com/spyder-ide/spyder-kernels/pull/257) - PR: Notify frontend of Matplotlib backend change, by [@impact27](https://github.com/impact27)
+* [PR 171](https://github.com/spyder-ide/spyder-kernels/pull/171) - PR: Publish Pdb stack frames to Spyder, by [@impact27](https://github.com/impact27)
+
+In this release 25 pull requests were closed.
+
+
+----
+
+
 ## Version 2.4.3 (2023-04-02)
 
 ### Issues Closed
 
 * [Issue 440](https://github.com/spyder-ide/spyder-kernels/issues/440) - distutils and LooseVersion deprecation ([PR 450](https://github.com/spyder-ide/spyder-kernels/pull/450) by [@ccordoba12](https://github.com/ccordoba12))
 
 In this release 1 issue was closed.
```

### Comparing `spyder-kernels-2.4.3/LICENSE.txt` & `spyder-kernels-3.0.0b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spyder-kernels-2.4.3/PKG-INFO` & `spyder-kernels-3.0.0b1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: spyder-kernels
-Version: 2.4.3
+Version: 3.0.0b1
 Summary: Jupyter kernels for Spyder's console
 Home-page: https://github.com/spyder-ide/spyder-kernels
 Download-URL: https://www.spyder-ide.org/#fh5co-download
 Author: Spyder Development Team
 Author-email: spyderlib@googlegroups.com
 License: MIT
 Keywords: spyder jupyter kernel ipython console
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Jupyter
 Classifier: Framework :: IPython
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Interpreters
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.txt
 License-File: AUTHORS.txt
 
 # Jupyter kernels for the Spyder console
 
@@ -33,15 +32,15 @@
 [![Linux status](https://github.com/spyder-ide/spyder-kernels/workflows/Linux%20tests/badge.svg)](https://github.com/spyder-ide/spyder-kernels/actions?query=workflow%3A%22Linux+tests%22)
 [![Macos status](https://github.com/spyder-ide/spyder-kernels/workflows/Macos%20tests/badge.svg)](https://github.com/spyder-ide/spyder-kernels/actions?query=workflow%3A%22Macos+tests%22)
 [![codecov](https://codecov.io/gh/spyder-ide/spyder-kernels/branch/master/graph/badge.svg)](https://codecov.io/gh/spyder-ide/spyder-kernels/branch/master)
 
 Package that provides Jupyter kernels for use with the consoles of Spyder, the
 Scientific Python Development Environment.
 
-These kernels can launched either through Spyder itself or in an independent
+These kernels can be launched either through Spyder itself or in an independent
 Python session, and allow for interactive or file-based execution of Python
 code inside Spyder.
 
 To learn about creating, connecting to and using these kernels with the Spyder
 console, please read our [documentation](https://docs.spyder-ide.org/current/panes/ipythonconsole.html).
 
 For advice on managing packages and environments with `spyder-kernels`, please read this
```

### Comparing `spyder-kernels-2.4.3/README.md` & `spyder-kernels-3.0.0b1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![Linux status](https://github.com/spyder-ide/spyder-kernels/workflows/Linux%20tests/badge.svg)](https://github.com/spyder-ide/spyder-kernels/actions?query=workflow%3A%22Linux+tests%22)
 [![Macos status](https://github.com/spyder-ide/spyder-kernels/workflows/Macos%20tests/badge.svg)](https://github.com/spyder-ide/spyder-kernels/actions?query=workflow%3A%22Macos+tests%22)
 [![codecov](https://codecov.io/gh/spyder-ide/spyder-kernels/branch/master/graph/badge.svg)](https://codecov.io/gh/spyder-ide/spyder-kernels/branch/master)
 
 Package that provides Jupyter kernels for use with the consoles of Spyder, the
 Scientific Python Development Environment.
 
-These kernels can launched either through Spyder itself or in an independent
+These kernels can be launched either through Spyder itself or in an independent
 Python session, and allow for interactive or file-based execution of Python
 code inside Spyder.
 
 To learn about creating, connecting to and using these kernels with the Spyder
 console, please read our [documentation](https://docs.spyder-ide.org/current/panes/ipythonconsole.html).
 
 For advice on managing packages and environments with `spyder-kernels`, please read this
```

### Comparing `spyder-kernels-2.4.3/RELEASE.md` & `spyder-kernels-3.0.0b1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `spyder-kernels-2.4.3/spyder_kernels/__init__.py` & `spyder-kernels-3.0.0b1/spyder_kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-2.4.3/spyder_kernels/comms/__init__.py` & `spyder-kernels-3.0.0b1/spyder_kernels/comms/__init__.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-2.4.3/spyder_kernels/comms/commbase.py` & `spyder-kernels-3.0.0b1/spyder_kernels/comms/commbase.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,30 +46,25 @@
         - The 'content' is a dict with: {
                 'is_error': a boolean indicating if the return value is an
                             exception to be raised.
                 'call_id': The uuid from above,
                 'call_name': The function name (mostly for debugging)
                 }
 """
-from __future__ import print_function
-
 import cloudpickle
 import pickle
 import logging
 import sys
 import uuid
 import traceback
 
-from spyder_kernels.py3compat import PY2, PY3
-
 
 logger = logging.getLogger(__name__)
 
-# To be able to get and set variables between Python 2 and 3
-DEFAULT_PICKLE_PROTOCOL = 2
+DEFAULT_PICKLE_PROTOCOL = 4
 
 # Max timeout (in secs) for blocking calls
 TIMEOUT = 3
 
 
 class CommError(RuntimeError):
     pass
@@ -128,15 +123,15 @@
         return
     sys_excepthook(type, value, tb)
 
 
 sys.excepthook = comm_excepthook
 
 
-class CommBase(object):
+class CommBase:
     """
     Class with the necessary attributes and methods to handle
     communications between a kernel and a frontend.
     Subclasses must open a comm and register it with `self._register_comm`.
     """
 
     def __init__(self):
@@ -150,16 +145,14 @@
         self._reply_inbox = {}
         self._reply_waitlist = {}
 
         self._register_message_handler(
             'remote_call', self._handle_remote_call)
         self._register_message_handler(
             'remote_call_reply', self._handle_remote_call_reply)
-        self.register_call_handler('_set_pickle_protocol',
-                                   self._set_pickle_protocol)
 
     def get_comm_id_list(self, comm_id=None):
         """Get a list of comms id."""
         if comm_id is None:
             id_list = list(self._comms.keys())
         else:
             id_list = [comm_id]
@@ -178,44 +171,38 @@
 
     def is_open(self, comm_id=None):
         """Check to see if the comm is open."""
         if comm_id is None:
             return len(self._comms) > 0
         return comm_id in self._comms
 
-    def is_ready(self, comm_id=None):
-        """
-        Check to see if the other side replied.
-
-        The check is made with _set_pickle_protocol as this is the first call
-        made. If comm_id is not specified, check all comms.
-        """
-        id_list = self.get_comm_id_list(comm_id)
-        if len(id_list) == 0:
-            return False
-        return all([self._comms[cid]['status'] == 'ready' for cid in id_list])
-
     def register_call_handler(self, call_name, handler):
         """
         Register a remote call handler.
 
         Parameters
         ----------
         call_name : str
             The name of the called function.
         handler : callback
-            A function to handle the request, or `None` to unregister
-            `call_name`.
+            A function to handle the request.
         """
-        if not handler:
-            self._remote_call_handlers.pop(call_name, None)
-            return
-
         self._remote_call_handlers[call_name] = handler
 
+    def unregister_call_handler(self, call_name):
+        """
+        Unegister a remote call handler.
+
+        Parameters
+        ----------
+        call_name : str
+            The name of the called function.
+        """
+        self._remote_call_handlers.pop(call_name, None)
+
     def remote_call(self, comm_id=None, callback=None, **settings):
         """Get a handler for remote calls."""
         return RemoteCallFactory(self, comm_id, callback, **settings)
 
     # ---- Private -----
     def _send_message(self, spyder_msg_type, content=None, data=None,
                       comm_id=None):
@@ -248,15 +235,14 @@
                 data, protocol=self._comms[comm_id]['pickle_protocol'])]
             self._comms[comm_id]['comm'].send(msg_dict, buffers=buffers)
 
     def _set_pickle_protocol(self, protocol):
         """Set the pickle protocol used to send data."""
         protocol = min(protocol, pickle.HIGHEST_PROTOCOL)
         self._comms[self.calling_comm_id]['pickle_protocol'] = protocol
-        self._comms[self.calling_comm_id]['status'] = 'ready'
 
     @property
     def _comm_name(self):
         """
         Get the name used for the underlying comms.
         """
         return 'spyder_api'
@@ -305,23 +291,15 @@
         self.calling_comm_id = msg['content']['comm_id']
 
         # Get message dict
         msg_dict = msg['content']['data']
 
         # Load the buffer. Only one is supported.
         try:
-            if PY3:
-                # https://docs.python.org/3/library/pickle.html#pickle.loads
-                # Using encoding='latin1' is required for unpickling
-                # NumPy arrays and instances of datetime, date and time
-                # pickled by Python 2.
-                buffer = cloudpickle.loads(msg['buffers'][0],
-                                           encoding='latin-1')
-            else:
-                buffer = cloudpickle.loads(msg['buffers'][0])
+            buffer = cloudpickle.loads(msg['buffers'][0])
         except Exception as e:
             logger.debug(
                 "Exception in cloudpickle.loads : %s" % str(e))
             buffer = CommsErrorWrapper(
                 msg_dict['content']['call_name'],
                 msg_dict['content']['call_id'])
 
@@ -400,26 +378,28 @@
         return call_dict
 
     def on_incoming_call(self, call_dict):
         """A call was received"""
         if "pickle_highest_protocol" in call_dict:
             self._set_pickle_protocol(call_dict["pickle_highest_protocol"])
 
-    def _get_call_return_value(self, call_dict, call_data, comm_id):
+    def _send_call(self, call_dict, call_data, comm_id):
+        """Send call."""
+        call_dict = self.on_outgoing_call(call_dict)
+        self._send_message(
+            'remote_call', content=call_dict, data=call_data,
+            comm_id=comm_id)
+
+    def _get_call_return_value(self, call_dict, comm_id):
         """
         Send a remote call and return the reply.
 
         If settings['blocking'] == True, this will wait for a reply and return
         the replied value.
         """
-        call_dict = self.on_outgoing_call(call_dict)
-        self._send_message(
-            'remote_call', content=call_dict, data=call_data,
-            comm_id=comm_id)
-
         settings = call_dict['settings']
 
         blocking = 'blocking' in settings and settings['blocking']
 
         if not blocking:
             return
 
@@ -428,24 +408,24 @@
 
         # Wait for the blocking call
         if 'timeout' in settings and settings['timeout'] is not None:
             timeout = settings['timeout']
         else:
             timeout = TIMEOUT
 
-        self._wait_reply(call_id, call_name, timeout)
+        self._wait_reply(comm_id, call_id, call_name, timeout)
 
         reply = self._reply_inbox.pop(call_id)
 
         if reply['is_error']:
             return self._sync_error(reply['value'])
 
         return reply['value']
 
-    def _wait_reply(self, call_id, call_name, timeout):
+    def _wait_reply(self, comm_id, call_id, call_name, timeout):
         """
         Wait for the other side reply.
         """
         raise NotImplementedError
 
     def _handle_remote_call_reply(self, msg_dict, buffer):
         """
@@ -492,15 +472,15 @@
     def _sync_error(self, error_wrapper):
         """
         Handle an error that was raised on the other side syncronously.
         """
         error_wrapper.raise_error()
 
 
-class RemoteCallFactory(object):
+class RemoteCallFactory:
     """Class to create `RemoteCall`s."""
 
     def __init__(self, comms_wrapper, comm_id, callback, **settings):
         # Avoid setting attributes
         super(RemoteCallFactory, self).__setattr__(
             '_comms_wrapper', comms_wrapper)
         super(RemoteCallFactory, self).__setattr__('_comm_id', comm_id)
@@ -550,9 +530,10 @@
         if not self._comms_wrapper.is_open(self._comm_id):
             # Only an error if the call is blocking.
             if blocking:
                 raise CommError("The comm is not connected.")
             logger.debug("Call to unconnected comm: %s" % self._name)
             return
         self._comms_wrapper._register_call(call_dict, self._callback)
+        self._comms_wrapper._send_call(call_dict, call_data, self._comm_id)
         return self._comms_wrapper._get_call_return_value(
-            call_dict, call_data, self._comm_id)
+            call_dict, self._comm_id)
```

### Comparing `spyder-kernels-2.4.3/spyder_kernels/console/__main__.py` & `spyder-kernels-3.0.0b1/spyder_kernels/console/__main__.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-2.4.3/spyder_kernels/console/kernel.py` & `spyder-kernels-3.0.0b1/spyder_kernels/console/kernel.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,37 +7,41 @@
 # -----------------------------------------------------------------------------
 
 """
 Spyder kernel for Jupyter.
 """
 
 # Standard library imports
+import faulthandler
+import json
 import logging
 import os
+import re
 import sys
+import traceback
+import tempfile
 import threading
 
 # Third-party imports
 from ipykernel.ipkernel import IPythonKernel
-from ipykernel import eventloops
+from ipykernel import eventloops, get_connection_info
 from traitlets.config.loader import LazyConfigValue
+import zmq
+from zmq.utils.garbage import gc
 
 # Local imports
-from spyder_kernels.py3compat import (
-    TEXT_TYPES, to_text_string, PY3)
 from spyder_kernels.comms.frontendcomm import FrontendComm
 from spyder_kernels.utils.iofuncs import iofunctions
 from spyder_kernels.utils.mpl import (
     MPL_BACKENDS_FROM_SPYDER, MPL_BACKENDS_TO_SPYDER, INLINE_FIGURE_FORMATS)
 from spyder_kernels.utils.nsview import (
     get_remote_data, make_remote_view, get_size)
 from spyder_kernels.console.shell import SpyderShell
+from spyder_kernels.comms.utils import WriteContext
 
-if PY3:
-    import faulthandler
 
 
 logger = logging.getLogger(__name__)
 
 
 # Excluded variables from the Variable Explorer (i.e. they are not
 # shown at all there)
@@ -53,112 +57,250 @@
         super(SpyderKernel, self).__init__(*args, **kwargs)
 
         self.comm_manager.get_comm = self._get_comm
         self.frontend_comm = FrontendComm(self)
 
         # All functions that can be called through the comm
         handlers = {
-            'set_breakpoints': self.set_spyder_breakpoints,
-            'set_pdb_ignore_lib': self.set_pdb_ignore_lib,
-            'set_pdb_execute_events': self.set_pdb_execute_events,
-            'set_pdb_use_exclamation_mark': self.set_pdb_use_exclamation_mark,
+            'set_pdb_configuration': self.shell.set_pdb_configuration,
             'get_value': self.get_value,
             'load_data': self.load_data,
             'save_namespace': self.save_namespace,
             'is_defined': self.is_defined,
             'get_doc': self.get_doc,
             'get_source': self.get_source,
             'set_value': self.set_value,
             'remove_value': self.remove_value,
             'copy_value': self.copy_value,
             'set_cwd': self.set_cwd,
-            'get_cwd': self.get_cwd,
             'get_syspath': self.get_syspath,
             'get_env': self.get_env,
             'close_all_mpl_figures': self.close_all_mpl_figures,
             'show_mpl_backend_errors': self.show_mpl_backend_errors,
             'get_namespace_view': self.get_namespace_view,
             'set_namespace_view_settings': self.set_namespace_view_settings,
             'get_var_properties': self.get_var_properties,
             'set_sympy_forecolor': self.set_sympy_forecolor,
             'update_syspath': self.update_syspath,
             'is_special_kernel_valid': self.is_special_kernel_valid,
             'get_matplotlib_backend': self.get_matplotlib_backend,
             'get_mpl_interactive_backend': self.get_mpl_interactive_backend,
-            'pdb_input_reply': self.pdb_input_reply,
-            '_interrupt_eventloop': self._interrupt_eventloop,
+            'pdb_input_reply': self.shell.pdb_input_reply,
             'enable_faulthandler': self.enable_faulthandler,
-            }
+            'get_current_frames': self.get_current_frames,
+            'request_pdb_stop': self.shell.request_pdb_stop,
+            'raise_interrupt_signal': self.shell.raise_interrupt_signal,
+            'get_fault_text': self.get_fault_text,
+        }
         for call_id in handlers:
             self.frontend_comm.register_call_handler(
                 call_id, handlers[call_id])
 
         self.namespace_view_settings = {}
         self._mpl_backend_error = None
-        self._running_namespace = None
         self.faulthandler_handle = None
+        self._cwd_initialised = False
 
-    # -- Public API -----------------------------------------------------------
-    def do_shutdown(self, restart):
-        """Disable faulthandler if enabled before proceeding."""
-        self.disable_faulthandler()
-        super(SpyderKernel, self).do_shutdown(restart)
+        # Add handlers to control to process messages while debugging
+        self.control_handlers['comm_msg'] = self.control_comm_msg
+        self.control_handlers['complete_request'] = self.shell_handlers[
+            'complete_request']
 
+        # Socket to signal shell_stream locally
+        self.loopback_socket = None
+
+    # -- Public API -----------------------------------------------------------
     def frontend_call(self, blocking=False, broadcast=True,
-                      timeout=None, callback=None):
+                      timeout=None, callback=None, display_error=False):
         """Call the frontend."""
         # If not broadcast, send only to the calling comm
         if broadcast:
             comm_id = None
         else:
             comm_id = self.frontend_comm.calling_comm_id
 
         return self.frontend_comm.remote_call(
             blocking=blocking,
             comm_id=comm_id,
             callback=callback,
-            timeout=timeout)
+            timeout=timeout,
+            display_error=display_error)
+
+    def get_state(self):
+        """"get current state to send to the frontend"""
+        state = {}
+        with WriteContext("get_state"):
+            if self._cwd_initialised:
+                state["cwd"] = self.get_cwd()
+            state["namespace_view"] = self.get_namespace_view()
+            state["var_properties"] = self.get_var_properties()
+        return state
+
+    def publish_state(self):
+        """Publish the current kernel state"""
+        if not self.frontend_comm.is_open():
+            # No one to send to
+            return
+        try:
+            self.frontend_call(blocking=False).update_state(self.get_state())
+        except Exception:
+            pass
 
-    def enable_faulthandler(self, fn):
+    def enable_faulthandler(self):
         """
         Open a file to save the faulthandling and identifiers for
         internal threads.
         """
-        if not PY3:
-            # Not implemented
+        fault_dir = None
+        if sys.platform.startswith('linux'):
+            # Do not use /tmp for temporary files
+            try:
+                from xdg.BaseDirectory import xdg_data_home
+                fault_dir = xdg_data_home
+                os.makedirs(fault_dir, exist_ok=True)
+            except Exception:
+                fault_dir = None
+
+        self.faulthandler_handle = tempfile.NamedTemporaryFile(
+            'wt', suffix='.fault', dir=fault_dir)
+        main_id = threading.main_thread().ident
+        system_ids = [
+            thread.ident for thread in threading.enumerate()
+            if thread is not threading.main_thread()
+        ]
+        faulthandler.enable(self.faulthandler_handle)
+        return self.faulthandler_handle.name, main_id, system_ids
+
+    def get_fault_text(self, fault_filename, main_id, ignore_ids):
+        """Get fault text from old run."""
+        # Read file
+        try:
+            with open(fault_filename, 'r') as f:
+                fault = f.read()
+        except FileNotFoundError:
             return
-        self.disable_faulthandler()
-        f = open(fn, 'w')
-        self.faulthandler_handle = f
-        f.write("Main thread id:\n")
-        f.write(hex(threading.main_thread().ident))
-        f.write('\nSystem threads ids:\n')
-        f.write(" ".join([hex(thread.ident) for thread in threading.enumerate()
-                          if thread is not threading.main_thread()]))
-        f.write('\n')
-        faulthandler.enable(f)
+        except UnicodeDecodeError as e:
+            return (
+                "Can not read fault file!\n"
+                + "UnicodeDecodeError: " + str(e))
 
-    def disable_faulthandler(self):
-        """
-        Cancel the faulthandling, close the file handle and remove the file.
-        """
-        if not PY3:
-            # Not implemented
+        # Remove file
+        try:
+            os.remove(fault_filename)
+        except FileNotFoundError:
+            pass
+        except PermissionError:
+            pass
+
+        # Process file
+        if not fault:
             return
-        if self.faulthandler_handle:
-            faulthandler.disable()
-            self.faulthandler_handle.close()
-            self.faulthandler_handle = None
+
+        thread_regex = (
+            r"(Current thread|Thread) "
+            r"(0x[\da-f]+) \(most recent call first\):"
+            r"(?:.|\r\n|\r|\n)+?(?=Current thread|Thread|\Z)")
+        # Keep line for future improvements
+        # files_regex = r"File \"([^\"]+)\", line (\d+) in (\S+)"
+
+        text = ""
+        start_idx = 0
+        for idx, match in enumerate(re.finditer(thread_regex, fault)):
+            # Add anything non-matched
+            text += fault[start_idx:match.span()[0]]
+            start_idx = match.span()[1]
+            thread_id = int(match.group(2), base=16)
+            if thread_id != main_id:
+                if thread_id in ignore_ids:
+                    continue
+                if "wurlitzer.py" in match.group(0):
+                    # Wurlitzer threads are launched later
+                    continue
+                text += "\n" + match.group(0) + "\n"
+            else:
+                try:
+                    pattern = (r".*(?:/IPython/core/interactiveshell\.py|"
+                               r"\\IPython\\core\\interactiveshell\.py).*")
+                    match_internal = next(re.finditer(pattern, match.group(0)))
+                    end_idx = match_internal.span()[0]
+                except StopIteration:
+                    end_idx = None
+                text += "\nMain thread:\n" + match.group(0)[:end_idx] + "\n"
+
+        # Add anything after match
+        text += fault[start_idx:]
+        return text
+
+    def get_system_threads_id(self):
+        """Return the list of system threads id."""
+        ignore_threads = [
+            self.parent.poller,  # Parent poller
+            self.shell.history_manager.save_thread,  # history
+            self.parent.heartbeat,  # heartbeat
+            self.parent.iopub_thread.thread,  # iopub
+            gc.thread,  # ZMQ garbage collector thread
+            self.parent.control_thread,  # control
+        ]
+        return [
+            thread.ident for thread in ignore_threads if thread is not None]
+
+    def filter_stack(self, stack, is_main):
+        """Return the part of the stack the user needs to see."""
+        # Remove wurlitzer frames
+        for frame_summary in stack:
+            if "wurlitzer.py" in frame_summary.filename:
+                return
+        # Cleanup main thread
+        if is_main:
+            start_idx = -1
+            for idx in range(len(stack)):
+                if stack[idx].filename.endswith(
+                        ("IPython/core/interactiveshell.py",
+                         "IPython\\core\\interactiveshell.py")):
+                    start_idx = idx + 1
+            if start_idx != -1:
+                stack = stack[start_idx:]
+            else:
+                stack = []
+        return stack
+
+    def get_current_frames(self, ignore_internal_threads=True,
+                           capture_locals=False):
+        """Get the current frames."""
+        ignore_list = self.get_system_threads_id()
+        main_id = threading.main_thread().ident
+        frames = {}
+        thread_names = {thread.ident: thread.name
+                        for thread in threading.enumerate()}
+
+        for thread_id, frame in sys._current_frames().items():
+            stack = traceback.StackSummary.extract(
+                traceback.walk_stack(frame))
+            if capture_locals:
+                for f_summary, f in zip(stack, traceback.walk_stack(frame)):
+                    f_summary.locals = self.get_namespace_view(frame=f[0])
+            stack.reverse()
+            if ignore_internal_threads:
+                if thread_id in ignore_list:
+                    continue
+                stack = self.filter_stack(stack, main_id == thread_id)
+            if stack is not None:
+                if thread_id in thread_names:
+                    thread_name = thread_names[thread_id]
+                else:
+                    thread_name = str(thread_id)
+                frames[thread_name] = stack
+        return frames
 
     # --- For the Variable Explorer
     def set_namespace_view_settings(self, settings):
         """Set namespace_view_settings."""
         self.namespace_view_settings = settings
 
-    def get_namespace_view(self):
+    def get_namespace_view(self, frame=None):
         """
         Return the namespace view
 
         This is a dictionary with the following structure
 
         {'a':
             {
@@ -179,28 +321,28 @@
           `get_type_string`.
         * 'numpy_type' is its Numpy type (if any) computed with
           `get_numpy_type_string`.
         """
 
         settings = self.namespace_view_settings
         if settings:
-            ns = self._get_current_namespace()
+            ns = self.shell._get_current_namespace(frame=frame)
             view = make_remote_view(ns, settings, EXCLUDED_NAMES)
             return view
         else:
             return None
 
     def get_var_properties(self):
         """
         Get some properties of the variables in the current
         namespace
         """
         settings = self.namespace_view_settings
         if settings:
-            ns = self._get_current_namespace()
+            ns = self.shell._get_current_namespace()
             data = get_remote_data(ns, settings, mode='editable',
                                    more_excluded_names=EXCLUDED_NAMES)
 
             properties = {}
             for name, value in list(data.items()):
                 properties[name] = {
                     'is_list':  self._is_list(value),
@@ -217,31 +359,31 @@
 
             return properties
         else:
             return None
 
     def get_value(self, name):
         """Get the value of a variable"""
-        ns = self._get_current_namespace()
+        ns = self.shell._get_current_namespace()
         return ns[name]
 
     def set_value(self, name, value):
         """Set the value of a variable"""
-        ns = self._get_reference_namespace(name)
+        ns = self.shell._get_reference_namespace(name)
         ns[name] = value
         self.log.debug(ns)
 
     def remove_value(self, name):
         """Remove a variable"""
-        ns = self._get_reference_namespace(name)
+        ns = self.shell._get_reference_namespace(name)
         ns.pop(name)
 
     def copy_value(self, orig_name, new_name):
         """Copy a variable"""
-        ns = self._get_reference_namespace(orig_name)
+        ns = self.shell._get_reference_namespace(orig_name)
         ns[new_name] = ns[orig_name]
 
     def load_data(self, filename, ext, overwrite=False):
         """
         Load data from filename.
 
         Use 'overwrite' to determine if conflicts between variable names need
@@ -274,15 +416,15 @@
         except Exception as error:
             return str(error)
 
         return None
 
     def save_namespace(self, filename):
         """Save namespace into filename"""
-        ns = self._get_current_namespace()
+        ns = self.shell._get_current_namespace()
         settings = self.namespace_view_settings
         data = get_remote_data(ns, settings, mode='picklable',
                                more_excluded_names=EXCLUDED_NAMES).copy()
         return iofunctions.save(data, filename)
 
     # --- For Pdb
     def _do_complete(self, code, cursor_pos):
@@ -295,69 +437,49 @@
 
         Public method of ipykernel overwritten for debugging.
         """
         if self.shell.is_debugging():
             return self.shell.pdb_session.do_complete(code, cursor_pos)
         return self._do_complete(code, cursor_pos)
 
-    def set_spyder_breakpoints(self, breakpoints):
-        """
-        Handle a message from the frontend
-        """
-        if self.shell.pdb_session:
-            self.shell.pdb_session.set_spyder_breakpoints(breakpoints)
-
-    def set_pdb_ignore_lib(self, state):
-        """
-        Change the "Ignore libraries while stepping" debugger setting.
+    def interrupt_eventloop(self):
         """
-        if self.shell.pdb_session:
-            self.shell.pdb_session.pdb_ignore_lib = state
+        Interrupts the eventloop.
 
-    def set_pdb_execute_events(self, state):
-        """
-        Handle a message from the frontend
-        """
-        if self.shell.pdb_session:
-            self.shell.pdb_session.pdb_execute_events = state
+        To be used when the main thread is blocked by a call to self.eventloop.
+        This can be called from another thread, e.g. the control thread.
 
-    def set_pdb_use_exclamation_mark(self, state):
-        """
-        Set an option on the current debugging session to decide wether
-        the Pdb commands needs to be prefixed by '!'
+        note:
+        Interrupting the eventloop is only implemented when a message is
+        received on the shell channel, but this message is queued and
+        won't be processed because an `execute` message is being
+        processed.
         """
-        if self.shell.pdb_session:
-            self.shell.pdb_session.pdb_use_exclamation_mark = state
+        if not self.eventloop:
+            return
 
-    def pdb_input_reply(self, line, echo_stack_entry=True):
-        """Get a pdb command from the frontend."""
-        debugger = self.shell.pdb_session
-        if debugger:
-            debugger._disable_next_stack_entry = not echo_stack_entry
-            debugger._cmd_input_line = line
-        if self.eventloop:
-            # Interrupting the eventloop is only implemented when a message is
-            # received on the shell channel, but this message is queued and
-            # won't be processed because an `execute` message is being
-            # processed. Therefore we process the message here (control chan.)
-            # and request a dummy message to be sent on the shell channel to
-            # stop the eventloop. This will call back `_interrupt_eventloop`.
-            self.frontend_call().request_interrupt_eventloop()
+        if self.loopback_socket is None:
+            # Add socket to signal shell_stream locally
+            self.loopback_socket = self.shell_stream.socket.context.socket(
+                zmq.DEALER)
+            port = json.loads(get_connection_info())['shell_port']
+            self.loopback_socket.connect("tcp://127.0.0.1:%i" % port)
+            # Add dummy handler
+            self.shell_handlers["interrupt_eventloop"] = (
+                lambda stream, ident, parent: None)
 
-    def _interrupt_eventloop(self):
-        """Interrupts the eventloop."""
-        # Receiving the request is enough to stop the eventloop.
-        pass
+        self.session.send(
+            self.loopback_socket, self.session.msg("interrupt_eventloop"))
 
     # --- For the Help plugin
     def is_defined(self, obj, force_import=False):
         """Return True if object is defined in current namespace"""
         from spyder_kernels.utils.dochelpers import isdefined
 
-        ns = self._get_current_namespace(with_magics=True)
+        ns = self.shell._get_current_namespace(with_magics=True)
         return isdefined(obj, force_import=force_import, namespace=ns)
 
     def get_doc(self, objtxt):
         """Get object documentation dictionary"""
         try:
             import matplotlib
             matplotlib.rcParams['docstring.hardcopy'] = True
@@ -404,16 +526,15 @@
 
         # --- Get interactive framework
         framework = None
 
         # Detect if there is a graphical framework running by checking the
         # eventloop function attached to the kernel.eventloop attribute (see
         # `ipykernel.eventloops.enable_gui` for context).
-        from IPython.core.getipython import get_ipython
-        loop_func = get_ipython().kernel.eventloop
+        loop_func = self.eventloop
 
         if loop_func is not None:
             if loop_func == eventloops.loop_tk:
                 framework = 'tk'
             elif loop_func == eventloops.loop_qt5:
                 framework = 'qt'
             elif loop_func == eventloops.loop_cocoa:
@@ -433,15 +554,15 @@
             # This covers the case of other backends (e.g. Wx or Gtk)
             # which users can set interactively with the %matplotlib
             # magic but not through our Preferences.
             return -1
 
     def set_matplotlib_backend(self, backend, pylab=False):
         """Set matplotlib backend given a Spyder backend option."""
-        mpl_backend = MPL_BACKENDS_FROM_SPYDER[to_text_string(backend)]
+        mpl_backend = MPL_BACKENDS_FROM_SPYDER[str(backend)]
         self._set_mpl_backend(mpl_backend, pylab=pylab)
 
     def set_mpl_inline_figure_format(self, figure_format):
         """Set the inline figure format to use with matplotlib."""
         mpl_figure_format = INLINE_FIGURE_FORMATS[figure_format]
         self._set_config_option(
             'InlineBackend.figure_format', mpl_figure_format)
@@ -457,16 +578,15 @@
 
     def set_mpl_inline_bbox_inches(self, bbox_inches):
         """
         Set inline print figure bbox inches.
 
         The change is done by updating the 'print_figure_kwargs' config dict.
         """
-        from IPython.core.getipython import get_ipython
-        config = get_ipython().kernel.config
+        config = self.config
         inline_config = (
             config['InlineBackend'] if 'InlineBackend' in config else {})
         print_figure_kwargs = (
             inline_config['print_figure_kwargs']
             if 'print_figure_kwargs' in inline_config else {})
         bbox_inches_dict = {
             'bbox_inches': 'tight' if bbox_inches else None}
@@ -494,15 +614,17 @@
     def set_autocall(self, autocall):
         """Enable/Disable autocall funtionality."""
         self._set_config_option('ZMQInteractiveShell.autocall', autocall)
 
     # --- Additional methods
     def set_cwd(self, dirname):
         """Set current working directory."""
+        self._cwd_initialised = True
         os.chdir(dirname)
+        self.publish_state()
 
     def get_cwd(self):
         """Get current working directory."""
         try:
             return os.getcwd()
         except (IOError, OSError):
             pass
@@ -566,57 +688,14 @@
             sys.path.extend(pypath)
             os.environ.update({'PYTHONPATH': os.pathsep.join(pypath)})
         else:
             os.environ.pop('PYTHONPATH', None)
 
     # -- Private API ---------------------------------------------------
     # --- For the Variable Explorer
-    def _get_current_namespace(self, with_magics=False):
-        """
-        Return current namespace
-
-        This is globals() if not debugging, or a dictionary containing
-        both locals() and globals() for current frame when debugging
-        """
-        ns = {}
-        if self.shell.is_debugging() and self.shell.pdb_session.curframe:
-            # Stopped at a pdb prompt
-            ns.update(self.shell.user_ns)
-            ns.update(self.shell._pdb_locals)
-        else:
-            # Give access to the running namespace if there is one
-            if self._running_namespace is None:
-                ns.update(self.shell.user_ns)
-            else:
-                # This is true when a file is executing.
-                running_globals, running_locals = self._running_namespace
-                ns.update(running_globals)
-                if running_locals is not None:
-                    ns.update(running_locals)
-
-        # Add magics to ns so we can show help about them on the Help
-        # plugin
-        if with_magics:
-            line_magics = self.shell.magics_manager.magics['line']
-            cell_magics = self.shell.magics_manager.magics['cell']
-            ns.update(line_magics)
-            ns.update(cell_magics)
-        return ns
-
-    def _get_reference_namespace(self, name):
-        """
-        Return namespace where reference name is defined
-
-        It returns the globals() if reference has not yet been defined
-        """
-        lcls = self.shell._pdb_locals
-        if name in lcls:
-            return lcls
-        return self.shell.user_ns
-
     def _get_len(self, var):
         """Return sequence length"""
         try:
             return get_size(var)
         except:
             return None
 
@@ -699,18 +778,17 @@
     # --- For the Help plugin
     def _eval(self, text):
         """
         Evaluate text and return (obj, valid)
         where *obj* is the object represented by *text*
         and *valid* is True if object evaluation did not raise any exception
         """
-        from spyder_kernels.py3compat import is_text_string
 
-        assert is_text_string(text)
-        ns = self._get_current_namespace(with_magics=True)
+        assert isinstance(text, str)
+        ns = self.shell._get_current_namespace(with_magics=True)
         try:
             return eval(text, ns), True
         except:
             return None, False
 
     # --- For Matplotlib
     def _set_mpl_backend(self, backend, pylab=False):
@@ -719,15 +797,14 @@
 
         backend: A parameter that can be passed to %matplotlib
                  (e.g. 'inline' or 'tk').
         pylab: Is the pylab magic should be used in order to populate the
                namespace from numpy and matplotlib
         """
         import traceback
-        from IPython.core.getipython import get_ipython
 
         # Don't proceed further if there's any error while importing Matplotlib
         try:
             import matplotlib
         except Exception:
             return
 
@@ -743,15 +820,15 @@
         error = None
         try:
             # This prevents Matplotlib to automatically set the backend, which
             # overrides our own mechanism.
             matplotlib.rcParams['backend'] = 'Agg'
 
             # Set the backend
-            get_ipython().run_line_magic(magic, backend)
+            self.shell.run_line_magic(magic, backend)
         except RuntimeError as err:
             # This catches errors generated by ipykernel when
             # trying to set a backend. See issue 5541
             if "GUI eventloops" in str(err):
                 previous_backend = matplotlib.get_backend()
                 if not backend in previous_backend.lower():
                     # Only inform about an error if the user selected backend
@@ -785,21 +862,20 @@
         """
         Set config options using the %config magic.
 
         As parameters:
             option: config option, for example 'InlineBackend.figure_format'.
             value: value of the option, for example 'SVG', 'Retina', etc.
         """
-        from IPython.core.getipython import get_ipython
         try:
             base_config = "{option} = "
             value_line = (
-                "'{value}'" if isinstance(value, TEXT_TYPES) else "{value}")
+                "'{value}'" if isinstance(value, str) else "{value}")
             config_line = base_config + value_line
-            get_ipython().run_line_magic(
+            self.shell.run_line_magic(
                 'config',
                 config_line.format(option=option, value=value))
         except Exception:
             pass
 
     def _set_mpl_inline_rc_config(self, option, value):
         """
@@ -818,42 +894,39 @@
             print(self._mpl_backend_error)  # spyder: test-skip
 
     def set_sympy_forecolor(self, background_color='dark'):
         """Set SymPy forecolor depending on console background."""
         if os.environ.get('SPY_SYMPY_O') == 'True':
             try:
                 from sympy import init_printing
-                from IPython.core.getipython import get_ipython
                 if background_color == 'dark':
-                    init_printing(forecolor='White', ip=get_ipython())
+                    init_printing(forecolor='White', ip=self.shell)
                 elif background_color == 'light':
-                    init_printing(forecolor='Black', ip=get_ipython())
+                    init_printing(forecolor='Black', ip=self.shell)
             except Exception:
                 pass
 
     # --- Others
     def _load_autoreload_magic(self):
         """Load %autoreload magic."""
-        from IPython.core.getipython import get_ipython
         try:
-            get_ipython().run_line_magic('reload_ext', 'autoreload')
-            get_ipython().run_line_magic('autoreload', '2')
+            self.shell.run_line_magic('reload_ext', 'autoreload')
+            self.shell.run_line_magic('autoreload', '2')
         except Exception:
             pass
 
     def _load_wurlitzer(self):
         """Load wurlitzer extension."""
         # Wurlitzer has no effect on Windows
         if not os.name == 'nt':
-            from IPython.core.getipython import get_ipython
             # Enclose this in a try/except because if it fails the
             # console will be totally unusable.
             # Fixes spyder-ide/spyder#8668
             try:
-                get_ipython().run_line_magic('reload_ext', 'wurlitzer')
+                self.shell.run_line_magic('reload_ext', 'wurlitzer')
             except Exception:
                 pass
 
     def _get_comm(self, comm_id):
         """
         We need to redefine this method from ipykernel.comm_manager to
         avoid showing a warning when the comm corresponding to comm_id
@@ -861,7 +934,36 @@
 
         Fixes spyder-ide/spyder#15498
         """
         try:
             return self.comm_manager.comms[comm_id]
         except KeyError:
             pass
+
+    def control_comm_msg(self, stream, ident, msg):
+        """
+        Handler for comm_msg messages from control channel.
+
+        If comm is not open yet, cache message.
+        """
+        content = msg['content']
+        comm_id = content['comm_id']
+        comm = self.comm_manager.get_comm(comm_id)
+        if comm is None:
+            self.frontend_comm.cache_message(comm_id, msg)
+            return
+        try:
+            comm.handle_msg(msg)
+        except Exception:
+            self.comm_manager.log.error(
+                'Exception in comm_msg for %s', comm_id, exc_info=True)
+
+    def pre_handler_hook(self):
+        """Hook to execute before calling message handler"""
+        pass
+
+    def post_handler_hook(self):
+        """Hook to execute after calling message handler"""
+        # keep ipykernel behavior of resetting sigint every call
+        self.shell.register_debugger_sigint()
+        # Reset tracing function so that pdb.set_trace works
+        sys.settrace(None)
```

### Comparing `spyder-kernels-2.4.3/spyder_kernels/console/outstream.py` & `spyder-kernels-3.0.0b1/spyder_kernels/console/outstream.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-2.4.3/spyder_kernels/console/start.py` & `spyder-kernels-3.0.0b1/spyder_kernels/console/start.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,27 +12,23 @@
 
 # Standard library imports
 import os
 import os.path as osp
 import sys
 import site
 
+# Third-party imports
 from traitlets import DottedObjectName
-import ipykernel
 
 # Local imports
 from spyder_kernels.utils.misc import is_module_installed
 from spyder_kernels.utils.mpl import (
     MPL_BACKENDS_FROM_SPYDER, INLINE_FIGURE_FORMATS)
 
 
-PY2 = sys.version[0] == '2'
-IPYKERNEL_6 = ipykernel.__version__[0] >= '6'
-
-
 def import_spydercustomize():
     """Import our customizations into the kernel."""
     here = osp.dirname(__file__)
     parent = osp.dirname(here)
     customize_dir = osp.join(parent, 'customize')
 
     # Remove current directory from sys.path to prevent kernel
@@ -92,36 +88,26 @@
     if testing:
         # Don't load nor save history in our IPython consoles.
         spy_cfg.HistoryAccessor.enabled = False
 
     # Until we implement Issue 1052
     spy_cfg.InteractiveShell.xmode = 'Plain'
 
-    # Jedi completer. It's only available in Python 3
+    # Jedi completer.
     jedi_o = os.environ.get('SPY_JEDI_O') == 'True'
-    if not PY2:
-        spy_cfg.IPCompleter.use_jedi = jedi_o
+    spy_cfg.IPCompleter.use_jedi = jedi_o
 
     # Clear terminal arguments input.
     # This needs to be done before adding the exec_lines that come from
     # Spyder, to avoid deleting the sys module if users want to import
     # it through them.
     # See spyder-ide/spyder#15788
     clear_argv = "import sys; sys.argv = ['']; del sys"
     spy_cfg.IPKernelApp.exec_lines = [clear_argv]
 
-    # Set our runfile in builtins here to prevent other packages shadowing it.
-    # This started to be a problem since IPykernel 6.3.0.
-    if not PY2:
-        spy_cfg.IPKernelApp.exec_lines.append(
-            "import builtins; "
-            "builtins.runfile = builtins.spyder_runfile; "
-            "del builtins.spyder_runfile; del builtins"
-        )
-
     # Prevent other libraries to change the breakpoint builtin.
     # This started to be a problem since IPykernel 6.3.0.
     if sys.version_info[0:2] >= (3, 7):
         spy_cfg.IPKernelApp.exec_lines.append(
             "import sys; import pdb; "
             "sys.breakpointhook = pdb.set_trace; "
             "del sys; del pdb"
@@ -138,20 +124,23 @@
     spy_cfg.IPKernelApp.exec_lines.append(
         "get_ipython().kernel._load_autoreload_magic()")
 
     # Load wurlitzer extension
     spy_cfg.IPKernelApp.exec_lines.append(
         "get_ipython().kernel._load_wurlitzer()")
 
-    # Default inline backend configuration
+    # Default inline backend configuration.
     # This is useful to have when people doesn't
     # use our config system to configure the
     # inline backend but want to use
     # '%matplotlib inline' at runtime
     spy_cfg.InlineBackend.rc = {
+        # The typical default figure size is too large for inline use,
+        # so we shrink the figure size to 6x4, and tweak fonts to
+        # make that fit.
         'figure.figsize': (6.0, 4.0),
         # 72 dpi matches SVG/qtconsole.
         # This only affects PNG export, as SVG has no dpi setting.
         'figure.dpi': 72,
         # 12pt labels get cutoff on 6x4 logplots, so use 10pt.
         'font.size': 10,
         # 10pt still needs a little more room on the xlabel
@@ -220,15 +209,15 @@
             spy_cfg.IPKernelApp.file_to_run = run_file_o
 
     # Autocall
     autocall_o = os.environ.get('SPY_AUTOCALL_O')
     if autocall_o is not None:
         spy_cfg.ZMQInteractiveShell.autocall = int(autocall_o)
 
-    # To handle the banner by ourselves in IPython 3+
+    # To handle the banner by ourselves
     spy_cfg.ZMQInteractiveShell.banner1 = ''
 
     # Greedy completer
     greedy_o = os.environ.get('SPY_GREEDY_O') == 'True'
     spy_cfg.IPCompleter.greedy = greedy_o
 
     # Sympy loading
@@ -257,15 +246,15 @@
     ip = get_ipython()       #analysis:ignore
     funcname, name = line.split()
     try:
         import guiqwt.pyplot as pyplot
     except:
         import matplotlib.pyplot as pyplot
     pyplot.figure();
-    getattr(pyplot, funcname[2:])(ip.kernel._get_current_namespace()[name])
+    getattr(pyplot, funcname[2:])(ip._get_current_namespace()[name])
     pyplot.show()
 
 
 def main():
     # Remove this module's path from sys.path:
     try:
         sys.path.remove(osp.dirname(__file__))
@@ -291,27 +280,33 @@
 
     # Main imports
     from ipykernel.kernelapp import IPKernelApp
     from spyder_kernels.console.kernel import SpyderKernel
 
     class SpyderKernelApp(IPKernelApp):
 
-        if IPYKERNEL_6:
-            outstream_class = DottedObjectName(
-                'spyder_kernels.console.outstream.TTYOutStream')
+        outstream_class = DottedObjectName(
+            'spyder_kernels.console.outstream.TTYOutStream')
 
         def init_pdb(self):
             """
             This method was added in IPykernel 5.3.1 and it replaces
             the debugger used by the kernel with a new class
             introduced in IPython 7.15 during kernel's initialization.
             Therefore, it doesn't allow us to use our debugger.
             """
             pass
 
+        def close(self):
+            """Close the loopback socket."""
+            socket = self.kernel.loopback_socket
+            if socket and not socket.closed:
+                socket.close()
+            return super().close()
+
     # Fire up the kernel instance.
     kernel = SpyderKernelApp.instance()
     kernel.kernel_class = SpyderKernel
     try:
         kernel.config = kernel_config()
     except:
         pass
```

### Comparing `spyder-kernels-2.4.3/spyder_kernels/console/tests/load_data.spydata` & `spyder-kernels-3.0.0b1/spyder_kernels/console/tests/load_data.spydata`

 * *Files identical despite different names*

### Comparing `spyder-kernels-2.4.3/spyder_kernels/console/tests/test_console_kernel.py` & `spyder-kernels-3.0.0b1/spyder_kernels/console/tests/test_console_kernel.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,50 +7,44 @@
 
 """
 Tests for the console kernel.
 """
 
 # Standard library imports
 import ast
+import asyncio
 import os
 import os.path as osp
 from textwrap import dedent
 from contextlib import contextmanager
 import time
 from subprocess import Popen, PIPE
 import sys
 import inspect
+import uuid
 from collections import namedtuple
 
 # Test imports
-import ipykernel
 import pytest
 from flaky import flaky
 from jupyter_core import paths
 from jupyter_client import BlockingKernelClient
 import numpy as np
 
 # Local imports
-from spyder_kernels.py3compat import PY2, PY3, to_text_string
 from spyder_kernels.utils.iofuncs import iofunctions
 from spyder_kernels.utils.mpl import MPL_BACKENDS_FROM_SPYDER
 from spyder_kernels.utils.test_utils import get_kernel, get_log_text
 from spyder_kernels.customize.spyderpdb import SpyderPdb
-
-# For ipykernel 6
-try:
-    import asyncio
-except ImportError:
-    pass
+from spyder_kernels.comms.commbase import CommBase
 
 # =============================================================================
 # Constants and utility functions
 # =============================================================================
 FILES_PATH = os.path.dirname(os.path.realpath(__file__))
-IPYKERNEL_6 = ipykernel.__version__[0] >= '6'
 TIMEOUT = 15
 SETUP_TIMEOUT = 60
 
 # We declare this constant immediately before the test, as determining
 # that TURTLE_ACTIVE is True will briefly pop up a window, similar to the
 # windows that will pop up during the test itself.
 TURTLE_ACTIVE = False
@@ -64,15 +58,15 @@
 
 
 @contextmanager
 def setup_kernel(cmd):
     """start an embedded kernel in a subprocess, and wait for it to be ready
 
     This function was taken from the ipykernel project.
-    We plan to remove it when dropping support for python 2.
+    We plan to remove it.
 
     Yields
     -------
     client: jupyter_client.BlockingKernelClient connected to the kernel
     """
     kernel = Popen([sys.executable, '-c', cmd], stdout=PIPE, stderr=PIPE)
     try:
@@ -85,34 +79,120 @@
         while not os.path.exists(connection_file) \
             and kernel.poll() is None \
             and time.time() < tic + SETUP_TIMEOUT:
             time.sleep(0.1)
 
         if kernel.poll() is not None:
             o,e = kernel.communicate()
-            if not PY3 and isinstance(e, bytes):
-                e = e.decode()
             raise IOError("Kernel failed to start:\n%s" % e)
 
         if not os.path.exists(connection_file):
             if kernel.poll() is None:
                 kernel.terminate()
             raise IOError("Connection file %r never arrived" % connection_file)
 
         client = BlockingKernelClient(connection_file=connection_file)
-        client.load_connection_file()
+        tic = time.time()
+        while True:
+            try:
+                client.load_connection_file()
+                break
+            except ValueError:
+                # The file is not written yet
+                if time.time() > tic + SETUP_TIMEOUT:
+                    # Give up after 5s
+                    raise IOError("Kernel failed to write connection file")
         client.start_channels()
         client.wait_for_ready()
         try:
             yield client
         finally:
             client.stop_channels()
     finally:
-        if not PY2:
-            kernel.terminate()
+        kernel.terminate()
+
+
+class Comm():
+    """
+    Comm base class, copied from qtconsole without the qt stuff
+    """
+
+    def __init__(self, target_name, kernel_client,
+                 msg_callback=None, close_callback=None):
+        """
+        Create a new comm. Must call open to use.
+        """
+        self.target_name = target_name
+        self.kernel_client = kernel_client
+        self.comm_id = uuid.uuid1().hex
+        self._msg_callback = msg_callback
+        self._close_callback = close_callback
+        self._send_channel = self.kernel_client.shell_channel
+
+    def _send_msg(self, msg_type, content, data, metadata, buffers):
+        """
+        Send a message on the shell channel.
+        """
+        if data is None:
+            data = {}
+        if content is None:
+            content = {}
+        content['comm_id'] = self.comm_id
+        content['data'] = data
+        msg = self.kernel_client.session.msg(
+            msg_type, content, metadata=metadata)
+        if buffers:
+            msg['buffers'] = buffers
+        return self._send_channel.send(msg)
+
+    # methods for sending messages
+    def open(self, data=None, metadata=None, buffers=None):
+        """Open the kernel-side version of this comm"""
+        return self._send_msg(
+            'comm_open', {'target_name': self.target_name},
+            data, metadata, buffers)
+
+    def send(self, data=None, metadata=None, buffers=None):
+        """Send a message to the kernel-side version of this comm"""
+        return self._send_msg(
+            'comm_msg', {}, data, metadata, buffers)
+
+    def close(self, data=None, metadata=None, buffers=None):
+        """Close the kernel-side version of this comm"""
+        return self._send_msg(
+            'comm_close', {}, data, metadata, buffers)
+
+    def on_msg(self, callback):
+        """Register a callback for comm_msg
+
+        Will be called with the `data` of any comm_msg messages.
+
+        Call `on_msg(None)` to disable an existing callback.
+        """
+        self._msg_callback = callback
+
+    def on_close(self, callback):
+        """Register a callback for comm_close
+
+        Will be called with the `data` of the close message.
+
+        Call `on_close(None)` to disable an existing callback.
+        """
+        self._close_callback = callback
+
+    # methods for handling incoming messages
+    def handle_msg(self, msg):
+        """Handle a comm_msg message"""
+        if self._msg_callback:
+            return self._msg_callback(msg)
+
+    def handle_close(self, msg):
+        """Handle a comm_close message"""
+        if self._close_callback:
+            return self._close_callback(msg)
 
 
 # =============================================================================
 # Fixtures
 # =============================================================================
 @pytest.fixture
 def kernel(request):
@@ -148,18 +228,15 @@
             'True_'
         ],
         'minmax': False
     }
 
     # Teardown
     def reset_kernel():
-        if IPYKERNEL_6:
-            asyncio.run(kernel.do_execute('reset -f', True))
-        else:
-            kernel.do_execute('reset -f', True)
+        asyncio.run(kernel.do_execute('reset -f', True))
     request.addfinalizer(reset_kernel)
 
     return kernel
 
 
 # =============================================================================
 # Tests
@@ -196,40 +273,30 @@
 
 
 # --- For the Variable Explorer
 def test_get_namespace_view(kernel):
     """
     Test the namespace view of the kernel.
     """
-    if IPYKERNEL_6:
-        execute = asyncio.run(kernel.do_execute('a = 1', True))
-    else:
-        execute = kernel.do_execute('a = 1', True)
+    execute = asyncio.run(kernel.do_execute('a = 1', True))
 
     nsview = repr(kernel.get_namespace_view())
     assert "'a':" in nsview
     assert "'type': 'int'" in nsview or "'type': u'int'" in nsview
     assert "'size': 1" in nsview
     assert "'view': '1'" in nsview
     assert "'numpy_type': 'Unknown'" in nsview
-
-    if PY3:
-        assert "'python_type': 'int'" in nsview
-    else:
-        assert "'python_type': u'int'" in nsview
+    assert "'python_type': 'int'" in nsview
 
 
 def test_get_var_properties(kernel):
     """
     Test the properties fo the variables in the namespace.
     """
-    if IPYKERNEL_6:
-        asyncio.run(kernel.do_execute('a = 1', True))
-    else:
-        kernel.do_execute('a = 1', True)
+    asyncio.run(kernel.do_execute('a = 1', True))
 
     var_properties = repr(kernel.get_var_properties())
     assert "'a'" in var_properties
     assert "'is_list': False" in var_properties
     assert "'is_dict': False" in var_properties
     assert "'len': 1" in var_properties
     assert "'is_array': False" in var_properties
@@ -239,47 +306,38 @@
     assert "'array_shape': None" in var_properties
     assert "'array_ndim': None" in var_properties
 
 
 def test_get_value(kernel):
     """Test getting the value of a variable."""
     name = 'a'
-    if IPYKERNEL_6:
-        asyncio.run(kernel.do_execute("a = 124", True))
-    else:
-        kernel.do_execute("a = 124", True)
+    asyncio.run(kernel.do_execute("a = 124", True))
 
     # Check data type send
     assert kernel.get_value(name) == 124
 
 
 def test_set_value(kernel):
     """Test setting the value of a variable."""
     name = 'a'
-    if IPYKERNEL_6:
-         asyncio.run(kernel.do_execute('a = 0', True))
-    else:
-        kernel.do_execute('a = 0', True)
+    asyncio.run(kernel.do_execute('a = 0', True))
     value = 10
     kernel.set_value(name, value)
     log_text = get_log_text(kernel)
     assert "'__builtin__': <module " in log_text
     assert "'__builtins__': <module " in log_text
     assert "'_ih': ['']" in log_text
     assert "'_oh': {}" in log_text
     assert "'a': 10" in log_text
 
 
 def test_remove_value(kernel):
     """Test the removal of a variable."""
     name = 'a'
-    if IPYKERNEL_6:
-        asyncio.run(kernel.do_execute('a = 1', True))
-    else:
-        kernel.do_execute('a = 1', True)
+    asyncio.run(kernel.do_execute('a = 1', True))
 
     var_properties = repr(kernel.get_var_properties())
     assert "'a'" in var_properties
     assert "'is_list': False" in var_properties
     assert "'is_dict': False" in var_properties
     assert "'len': 1" in var_properties
     assert "'is_array': False" in var_properties
@@ -293,18 +351,15 @@
     assert var_properties == '{}'
 
 
 def test_copy_value(kernel):
     """Test the copy of a variable."""
     orig_name = 'a'
     new_name = 'b'
-    if IPYKERNEL_6:
-         asyncio.run(kernel.do_execute('a = 1', True))
-    else:
-        kernel.do_execute('a = 1', True)
+    asyncio.run(kernel.do_execute('a = 1', True))
 
     var_properties = repr(kernel.get_var_properties())
     assert "'a'" in var_properties
     assert "'is_list': False" in var_properties
     assert "'is_dict': False" in var_properties
     assert "'len': 1" in var_properties
     assert "'is_array': False" in var_properties
@@ -332,19 +387,15 @@
     "load", [(True, "val1 = 0", {"val1": np.array(1)}),
              (False, "val1 = 0", {"val1": 0, "val1_000": np.array(1)})])
 def test_load_npz_data(kernel, load):
     """Test loading data from npz filename."""
     namespace_file = osp.join(FILES_PATH, 'load_data.npz')
     extention = '.npz'
     overwrite, execute, variables = load
-
-    if IPYKERNEL_6:
-        asyncio.run(kernel.do_execute(execute, True))
-    else:
-        kernel.do_execute(execute, True)
+    asyncio.run(kernel.do_execute(execute, True))
 
     kernel.load_data(namespace_file, extention, overwrite=overwrite)
     for var, value in variables.items():
         assert value == kernel.get_value(var)
 
 
 def test_load_data(kernel):
@@ -364,19 +415,15 @@
     assert "'array_shape': None" in var_properties
     assert "'array_ndim': None" in var_properties
 
 
 def test_save_namespace(kernel):
     """Test saving the namespace into filename."""
     namespace_file = osp.join(FILES_PATH, 'save_data.spydata')
-
-    if IPYKERNEL_6:
-        asyncio.run(kernel.do_execute('b = 1', True))
-    else:
-        kernel.do_execute('b = 1', True)
+    asyncio.run(kernel.do_execute('b = 1', True))
 
     kernel.save_namespace(namespace_file)
     assert osp.isfile(namespace_file)
     load_func = iofunctions.load_funcs['.spydata']
     data, error_message = load_func(namespace_file)
     assert data == {'b': 1}
     assert not error_message
@@ -396,15 +443,15 @@
     objtxt = 'help'
     assert ("Define the builtin 'help'" in kernel.get_doc(objtxt)['docstring'] or
             "Define the built-in 'help'" in kernel.get_doc(objtxt)['docstring'])
 
 def test_get_source(kernel):
     """Test to get object source."""
     objtxt = 'help'
-    assert 'class _Helper(object):' in kernel.get_source(objtxt)
+    assert 'class _Helper' in kernel.get_source(objtxt)
 
 
 # --- Other stuff
 @pytest.mark.skipif(os.name == 'nt', reason="Doesn't work on Windows")
 def test_output_from_c_libraries(kernel, capsys):
     """Test that the wurlitzer extension is working."""
     # This code was taken from the Wurlitzer demo
@@ -412,62 +459,53 @@
 import ctypes
 libc = ctypes.CDLL(None)
 libc.printf(('Hello from C\\n').encode('utf8'))
 """
 
     # With Wurlitzer we have the expected output
     kernel._load_wurlitzer()
-
-    if IPYKERNEL_6:
-        asyncio.run(kernel.do_execute(code, True))
-    else:
-        kernel.do_execute(code, True)
+    asyncio.run(kernel.do_execute(code, True))
     captured = capsys.readouterr()
     assert captured.out == "Hello from C\n"
 
 
 @flaky(max_runs=3)
 def test_cwd_in_sys_path():
     """
     Test that cwd stays as the first element in sys.path after the
     kernel has started.
     """
     # Command to start the kernel
     cmd = "from spyder_kernels.console import start; start.main()"
 
     with setup_kernel(cmd) as client:
-        msg_id = client.execute("import sys; sys_path = sys.path",
-                                user_expressions={'output':'sys_path'})
-        reply = client.get_shell_msg(timeout=TIMEOUT)
-        while 'user_expressions' not in reply['content']:
-            reply = client.get_shell_msg(timeout=TIMEOUT)
+        reply = client.execute_interactive(
+            "import sys; sys_path = sys.path",
+            user_expressions={'output':'sys_path'}, timeout=TIMEOUT)
 
         # Transform value obtained through user_expressions
         user_expressions = reply['content']['user_expressions']
         str_value = user_expressions['output']['data']['text/plain']
         value = ast.literal_eval(str_value)
 
         # Assert the first value of sys_path is an empty string
         assert '' in value
 
 
 @flaky(max_runs=3)
-@pytest.mark.skipif(not PY3,
-                    reason="Only meant for Python 3")
 def test_multiprocessing(tmpdir):
     """
-    Test that multiprocessing works on Python 3.
+    Test that multiprocessing works.
     """
     # Command to start the kernel
     cmd = "from spyder_kernels.console import start; start.main()"
 
     with setup_kernel(cmd) as client:
         # Remove all variables
-        client.execute("%reset -f")
-        client.get_shell_msg(timeout=TIMEOUT)
+        client.execute_interactive("%reset -f", timeout=TIMEOUT)
 
         # Write multiprocessing code to a file
         code = """
 from multiprocessing import Pool
 
 def f(x):
     return x*x
@@ -476,40 +514,37 @@
     with Pool(5) as p:
         result = p.map(f, [1, 2, 3])
 """
         p = tmpdir.join("mp-test.py")
         p.write(code)
 
         # Run code
-        client.execute("runfile(r'{}')".format(to_text_string(p)))
-        client.get_shell_msg(timeout=TIMEOUT)
+        client.execute_interactive(
+            "%runfile {}".format(repr(str(p))), timeout=TIMEOUT)
 
         # Verify that the `result` variable is defined
         client.inspect('result')
         msg = client.get_shell_msg(timeout=TIMEOUT)
         while "found" not in msg['content']:
             msg = client.get_shell_msg(timeout=TIMEOUT)
         content = msg['content']
         assert content['found']
 
 
 @flaky(max_runs=3)
-@pytest.mark.skipif(not PY3,
-                    reason="Only meant for Python 3")
 def test_multiprocessing_2(tmpdir):
     """
-    Test that multiprocessing works on Python 3.
+    Test that multiprocessing works.
     """
     # Command to start the kernel
     cmd = "from spyder_kernels.console import start; start.main()"
 
     with setup_kernel(cmd) as client:
         # Remove all variables
-        client.execute("%reset -f")
-        client.get_shell_msg(timeout=TIMEOUT)
+        client.execute_interactive("%reset -f", timeout=TIMEOUT)
 
         # Write multiprocessing code to a file
         code = """
 from multiprocessing import Pool
 
 class myClass():
     def __init__(self, i):
@@ -523,44 +558,44 @@
         result = p.map(myFunc, [1, 2, 3])
     result = [r.i for r in result]
 """
         p = tmpdir.join("mp-test.py")
         p.write(code)
 
         # Run code
-        client.execute("runfile(r'{}')".format(to_text_string(p)))
-        client.get_shell_msg(timeout=TIMEOUT)
+        client.execute_interactive(
+            "%runfile {}".format(repr(str(p))), timeout=TIMEOUT)
 
         # Verify that the `result` variable is defined
         client.inspect('result')
         msg = client.get_shell_msg(timeout=TIMEOUT)
         while "found" not in msg['content']:
             msg = client.get_shell_msg(timeout=TIMEOUT)
         content = msg['content']
         assert content['found']
         assert "[11, 12, 13]" in content['data']['text/plain']
 
 
 @flaky(max_runs=3)
 @pytest.mark.skipif(
-    not PY3, reason="Only meant for Python 3")
-@pytest.mark.skipif(
     sys.platform == 'darwin' and sys.version_info[:2] == (3, 8),
     reason="Fails on Mac with Python 3.8")
+@pytest.mark.skipif(
+    os.environ.get('USE_CONDA') != 'true',
+    reason="Doesn't work with pip packages")
 def test_dask_multiprocessing(tmpdir):
     """
-    Test that dask multiprocessing works on Python 3.
+    Test that dask multiprocessing works.
     """
     # Command to start the kernel
     cmd = "from spyder_kernels.console import start; start.main()"
 
     with setup_kernel(cmd) as client:
         # Remove all variables
-        client.execute("%reset -f")
-        client.get_shell_msg(timeout=TIMEOUT)
+        client.execute_interactive("%reset -f")
 
         # Write multiprocessing code to a file
         # Runs two times to verify that in the second case it doesn't break
         code = """
 from dask.distributed import Client
 
 if __name__=='__main__':
@@ -568,19 +603,19 @@
     client.close()
     x = 'hello'
 """
         p = tmpdir.join("mp-test.py")
         p.write(code)
 
         # Run code two times
-        client.execute("runfile(r'{}')".format(to_text_string(p)))
-        client.get_shell_msg(timeout=TIMEOUT)
+        client.execute_interactive(
+            "%runfile {}".format(repr(str(p))), timeout=TIMEOUT)
 
-        client.execute("runfile(r'{}')".format(to_text_string(p)))
-        client.get_shell_msg(timeout=TIMEOUT)
+        client.execute_interactive(
+            "%runfile {}".format(repr(str(p))), timeout=TIMEOUT)
 
         # Verify that the `x` variable is defined
         client.inspect('x')
         msg = client.get_shell_msg(timeout=TIMEOUT)
         while "found" not in msg['content']:
             msg = client.get_shell_msg(timeout=TIMEOUT)
         content = msg['content']
@@ -593,62 +628,58 @@
     Test that runfile uses the proper name space for execution.
     """
     # Command to start the kernel
     cmd = "from spyder_kernels.console import start; start.main()"
 
     with setup_kernel(cmd) as client:
         # Remove all variables
-        client.execute("%reset -f")
-        client.get_shell_msg(timeout=TIMEOUT)
+        client.execute_interactive("%reset -f", timeout=TIMEOUT)
 
         # Write defined variable code to a file
-        code = u"result = 'hello world'; error # make an error"
+        code = "result = 'hello world'; error # make an error"
         d = tmpdir.join("defined-test.py")
         d.write(code)
 
         # Write undefined variable code to a file
-        code = dedent(u"""
+        code = dedent("""
         try:
             result3 = result
         except NameError:
             result2 = 'hello world'
         """)
         u = tmpdir.join("undefined-test.py")
         u.write(code)
 
         # Run code file `d` to define `result` even after an error
-        client.execute("runfile(r'{}', current_namespace=False)"
-                       .format(to_text_string(d)))
-        client.get_shell_msg(timeout=TIMEOUT)
+        client.execute_interactive(
+            "%runfile {}".format(repr(str(d))), timeout=TIMEOUT)
 
         # Verify that `result` is defined in the current namespace
         client.inspect('result')
         msg = client.get_shell_msg(timeout=TIMEOUT)
         while "found" not in msg['content']:
             msg = client.get_shell_msg(timeout=TIMEOUT)
         content = msg['content']
         assert content['found']
 
         # Run code file `u` without current namespace
-        client.execute("runfile(r'{}', current_namespace=False)"
-                       .format(to_text_string(u)))
-        client.get_shell_msg(timeout=TIMEOUT)
+        client.execute_interactive(
+            "%runfile {}".format(repr(str(u))), timeout=TIMEOUT)
 
         # Verify that the variable `result2` is defined
         client.inspect('result2')
         msg = client.get_shell_msg(timeout=TIMEOUT)
         while "found" not in msg['content']:
             msg = client.get_shell_msg(timeout=TIMEOUT)
         content = msg['content']
         assert content['found']
 
         # Run code file `u` with current namespace
-        client.execute("runfile(r'{}', current_namespace=True)"
-                       .format(to_text_string(u)))
-        msg = client.get_shell_msg(timeout=TIMEOUT)
+        msg = client.execute_interactive("%runfile {} --current-namespace"
+                                        .format(repr(str(u))), timeout=TIMEOUT)
         content = msg['content']
 
         # Verify that the variable `result3` is defined
         client.inspect('result3')
         msg = client.get_shell_msg(timeout=TIMEOUT)
         while "found" not in msg['content']:
             msg = client.get_shell_msg(timeout=TIMEOUT)
@@ -672,38 +703,35 @@
     """Test that setting Numpy threshold doesn't make the Variable Explorer slow."""
 
     cmd = "from spyder_kernels.console import start; start.main()"
 
     with setup_kernel(cmd) as client:
 
         # Set Numpy threshold, suppress and formatter
-        client.execute("""
+        client.execute_interactive("""
 import numpy as np;
 np.set_printoptions(
     threshold=np.inf,
     suppress=True,
     formatter={'float_kind':'{:0.2f}'.format})
-    """)
-        client.get_shell_msg(timeout=TIMEOUT)
+    """, timeout=TIMEOUT)
 
         # Create a big Numpy array and an array to check decimal format
-        client.execute("""
+        client.execute_interactive("""
 x = np.random.rand(75000,5);
 a = np.array([123412341234.123412341234])
-""")
-        client.get_shell_msg(timeout=TIMEOUT)
+""", timeout=TIMEOUT)
 
         # Assert that NumPy threshold, suppress and formatter
         # are the same as the ones set by the user
-        client.execute("""
+        client.execute_interactive("""
 t = np.get_printoptions()['threshold'];
 s = np.get_printoptions()['suppress'];
 f = np.get_printoptions()['formatter']
-""")
-        client.get_shell_msg(timeout=TIMEOUT)
+""", timeout=TIMEOUT)
 
         # Check correct decimal format
         client.inspect('a')
         msg = client.get_shell_msg(timeout=TIMEOUT)
         while "data" not in msg['content']:
             msg = client.get_shell_msg(timeout=TIMEOUT)
         content = msg['content']['data']['text/plain']
@@ -741,16 +769,15 @@
 def test_turtle_launch(tmpdir):
     """Test turtle scripts running in the same kernel."""
     # Command to start the kernel
     cmd = "from spyder_kernels.console import start; start.main()"
 
     with setup_kernel(cmd) as client:
         # Remove all variables
-        client.execute("%reset -f")
-        client.get_shell_msg(timeout=TIMEOUT)
+        client.execute_interactive("%reset -f", timeout=TIMEOUT)
 
         # Write turtle code to a file
         code = """
 import turtle
 wn=turtle.Screen()
 wn.bgcolor("lightgreen")
 tess = turtle.Turtle() # Create tess and set some attributes
@@ -766,16 +793,16 @@
 
 turtle.bye()
 """
         p = tmpdir.join("turtle-test.py")
         p.write(code)
 
         # Run code
-        client.execute("runfile(r'{}')".format(to_text_string(p)))
-        client.get_shell_msg(timeout=TIMEOUT)
+        client.execute_interactive(
+            "%runfile {}".format(repr(str(p))), timeout=TIMEOUT)
 
         # Verify that the `tess` variable is defined
         client.inspect('tess')
         msg = client.get_shell_msg(timeout=TIMEOUT)
         while "found" not in msg['content']:
             msg = client.get_shell_msg(timeout=TIMEOUT)
         content = msg['content']
@@ -784,16 +811,16 @@
         # Write turtle code to a file
         code = code + "a = 10"
 
         p = tmpdir.join("turtle-test1.py")
         p.write(code)
 
         # Run code again
-        client.execute("runfile(r'{}')".format(to_text_string(p)))
-        client.get_shell_msg(timeout=TIMEOUT)
+        client.execute_interactive(
+            "%runfile {}".format(repr(str(p))), timeout=TIMEOUT)
 
         # Verify that the `a` variable is defined
         client.inspect('a')
         msg = client.get_shell_msg(timeout=TIMEOUT)
         while "found" not in msg['content']:
             msg = client.get_shell_msg(timeout=TIMEOUT)
         content = msg['content']
@@ -805,69 +832,58 @@
     """Test that the default backend for our kernels is 'inline'."""
     # Command to start the kernel
     cmd = "from spyder_kernels.console import start; start.main()"
 
     with setup_kernel(cmd) as client:
         # Get current backend
         code = "import matplotlib; backend = matplotlib.get_backend()"
-        client.execute(code, user_expressions={'output': 'backend'})
-        reply = client.get_shell_msg(timeout=TIMEOUT)
-        while 'user_expressions' not in reply['content']:
-            reply = client.get_shell_msg(timeout=TIMEOUT)
+        reply = client.execute_interactive(
+            code, user_expressions={'output': 'backend'}, timeout=TIMEOUT)
 
         # Transform value obtained through user_expressions
         user_expressions = reply['content']['user_expressions']
         str_value = user_expressions['output']['data']['text/plain']
         value = ast.literal_eval(str_value)
 
         # Assert backend is inline
         assert 'inline' in value
 
 
 def test_do_complete(kernel):
     """
     Check do complete works in normal and debugging mode.
     """
-    if IPYKERNEL_6:
-        asyncio.run(kernel.do_execute('abba = 1', True))
-    else:
-        kernel.do_execute('abba = 1', True)
+    asyncio.run(kernel.do_execute('abba = 1', True))
     assert kernel.get_value('abba') == 1
     match = kernel.do_complete('ab', 2)
     assert 'abba' in match['matches']
 
     # test pdb
     pdb_obj = SpyderPdb()
     pdb_obj.curframe = inspect.currentframe()
     pdb_obj.completenames = lambda *ignore: ['baba']
-    kernel.shell.pdb_session = pdb_obj
+    kernel.shell._namespace_stack = [pdb_obj]
     match = kernel.do_complete('ba', 2)
     assert 'baba' in match['matches']
     pdb_obj.curframe = None
 
 
 @pytest.mark.parametrize("exclude_callables_and_modules", [True, False])
 @pytest.mark.parametrize("exclude_unsupported", [True, False])
 def test_callables_and_modules(kernel, exclude_callables_and_modules,
                                exclude_unsupported):
     """
     Tests that callables and modules are in the namespace view only
     when the right options are passed to the kernel.
     """
-    if IPYKERNEL_6:
-        asyncio.run(kernel.do_execute('import numpy', True))
-        asyncio.run(kernel.do_execute('a = 10', True))
-        asyncio.run(kernel.do_execute('def f(x): return x', True))
-    else:
-        kernel.do_execute('import numpy', True)
-        kernel.do_execute('a = 10', True)
-        kernel.do_execute('def f(x): return x', True)
+    asyncio.run(kernel.do_execute('import numpy', True))
+    asyncio.run(kernel.do_execute('a = 10', True))
+    asyncio.run(kernel.do_execute('def f(x): return x', True))
 
     settings = kernel.namespace_view_settings
-
     settings['exclude_callables_and_modules'] = exclude_callables_and_modules
     settings['exclude_unsupported'] = exclude_unsupported
     nsview = kernel.get_namespace_view()
 
     # Callables and modules should always be in nsview when the option
     # is active.
     if not exclude_callables_and_modules:
@@ -893,15 +909,15 @@
     wants to work with them.
 
     This is a regression test for spyder-ide/spyder#13909.
     """
     pdb_obj = SpyderPdb()
     pdb_obj.curframe = inspect.currentframe()
     pdb_obj.curframe_locals = pdb_obj.curframe.f_locals
-    kernel.shell.pdb_session = pdb_obj
+    kernel.shell._namespace_stack = [pdb_obj]
 
     # Create a local variable.
     kernel.shell.pdb_session.default('zz = 10')
     assert kernel.get_value('zz') == 10
 
     # Run a list comprehension with this variable.
     kernel.shell.pdb_session.default("compr = [zz * i for i in [1, 2, 3]]")
@@ -919,15 +935,15 @@
     Test that evaluating comprehensions with locals works in Pdb.
 
     This is a regression test for spyder-ide/spyder#16790.
     """
     pdb_obj = SpyderPdb()
     pdb_obj.curframe = inspect.currentframe()
     pdb_obj.curframe_locals = pdb_obj.curframe.f_locals
-    kernel.shell.pdb_session = pdb_obj
+    kernel.shell._namespace_stack = [pdb_obj]
 
     # Create a local variable.
     kernel.shell.pdb_session.default('aa = [1, 2]')
     kernel.shell.pdb_session.default('bb = [3, 4]')
     kernel.shell.pdb_session.default('res = []')
 
     # Run a list comprehension with this variable.
@@ -945,26 +961,20 @@
     """
     # Define get_ipython for timeit
     get_ipython = lambda: kernel.shell
     kernel.shell.user_ns["test"] = 0
     pdb_obj = SpyderPdb()
     pdb_obj.curframe = inspect.currentframe()
     pdb_obj.curframe_locals = pdb_obj.curframe.f_locals
-    kernel.shell.pdb_session = pdb_obj
+    kernel.shell._namespace_stack = [pdb_obj]
 
     # Check adding something to globals works
     pdb_obj.default("globals()['test2'] = 0")
     assert pdb_obj.curframe.f_globals["test2"] == 0
 
-    if PY2:
-        # no error method in py2
-        pdb_obj.curframe = None
-        pdb_obj.curframe_locals = None
-        return
-
     # Create wrapper to check for errors
     old_error = pdb_obj.error
     pdb_obj._error_occured = False
     def error_wrapper(*args, **kwargs):
         print(args, kwargs)
         pdb_obj._error_occured = True
         return old_error(*args, **kwargs)
@@ -994,15 +1004,15 @@
 
     This is a regression test for spyder-ide/spyder-kernels#345
     """
     pdb_obj = SpyderPdb()
     Frame = namedtuple("Frame", ["f_globals"])
     pdb_obj.curframe = Frame(f_globals=kernel.shell.user_ns)
     pdb_obj.curframe_locals = kernel.shell.user_ns
-    kernel.shell.pdb_session = pdb_obj
+    kernel.shell._namespace_stack = [pdb_obj]
 
     # Create a local function.
     kernel.shell.pdb_session.default(
         'def fun_a(): return [i for i in range(1)]')
     kernel.shell.pdb_session.default(
         'zz = fun_a()')
     assert kernel.get_value('zz') == [0]
@@ -1026,15 +1036,15 @@
 
     This is another regression test for spyder-ide/spyder-kernels#345
     """
     baba = 1
     pdb_obj = SpyderPdb()
     pdb_obj.curframe = inspect.currentframe()
     pdb_obj.curframe_locals = pdb_obj.curframe.f_locals
-    kernel.shell.pdb_session = pdb_obj
+    kernel.shell._namespace_stack = [pdb_obj]
 
     # Create a local function.
     kernel.shell.pdb_session.default(
         'def fun_a(): return [i for i in range(1)]')
     kernel.shell.pdb_session.default(
         'zz = fun_a()')
     assert kernel.get_value('zz') == [0]
@@ -1063,15 +1073,15 @@
     """
     Test thal locals and globals work properly in Pdb.
     """
     a = 1
     pdb_obj = SpyderPdb()
     pdb_obj.curframe = inspect.currentframe()
     pdb_obj.curframe_locals = pdb_obj.curframe.f_locals
-    kernel.shell.pdb_session = pdb_obj
+    kernel.shell._namespace_stack = [pdb_obj]
 
     assert kernel.get_value('a') == 1
 
     kernel.shell.pdb_session.default(
         'test = "a" in globals()')
     assert kernel.get_value('test') == False
 
@@ -1100,72 +1110,110 @@
     pdb_obj.curframe = None
     pdb_obj.curframe_locals = None
 
 
 @flaky(max_runs=3)
 @pytest.mark.parametrize("backend", [None, 'inline', 'tk', 'qt5'])
 @pytest.mark.skipif(
-    not sys.platform.startswith('linux'),
-    reason="Doesn't work reliably on Windows and Mac")
-@pytest.mark.skipif(
-    not bool(os.environ.get('USE_CONDA')),
+    os.environ.get('USE_CONDA') != 'true',
     reason="Doesn't work with pip packages")
 @pytest.mark.skipif(
-    sys.version_info[:2] < (3, 8),
-    reason="Too flaky in Python 3.7 and doesn't work in older versions")
+    sys.version_info[:2] < (3, 9),
+    reason="Too flaky in Python 3.7/8 and doesn't work in older versions")
+@pytest.mark.skipif(sys.platform == 'darwin', reason="Fails on Mac")
 def test_get_interactive_backend(backend):
     """
     Test that we correctly get the interactive backend set in the kernel.
     """
     cmd = "from spyder_kernels.console import start; start.main()"
 
     with setup_kernel(cmd) as client:
         # Set backend
         if backend is not None:
-            client.execute("%matplotlib {}".format(backend))
-            client.get_shell_msg(timeout=TIMEOUT)
-            client.execute("import time; time.sleep(.1)")
-            client.get_shell_msg(timeout=TIMEOUT)
+            client.execute_interactive(
+                "%matplotlib {}".format(backend), timeout=TIMEOUT)
+            client.execute_interactive(
+                "import time; time.sleep(.1)", timeout=TIMEOUT)
 
         # Get backend
         code = "backend = get_ipython().kernel.get_mpl_interactive_backend()"
-        client.execute(code, user_expressions={'output': 'backend'})
-        reply = client.get_shell_msg(timeout=TIMEOUT)
-        while 'user_expressions' not in reply['content']:
-            reply = client.get_shell_msg(timeout=TIMEOUT)
+        reply = client.execute_interactive(
+            code, user_expressions={'output': 'backend'}, timeout=TIMEOUT)
 
         # Get value obtained through user_expressions
         user_expressions = reply['content']['user_expressions']
         value = user_expressions['output']['data']['text/plain']
 
         # Assert we got the right interactive backend
         if backend is not None:
             assert MPL_BACKENDS_FROM_SPYDER[value] == backend
         else:
             assert value == '0'
 
 
+def test_global_message(tmpdir):
+    """
+    Test that using `global` triggers a warning.
+    """
+    # Command to start the kernel
+    cmd = "from spyder_kernels.console import start; start.main()"
+
+    with setup_kernel(cmd) as client:
+        # Remove all variables
+        client.execute_interactive("%reset -f", timeout=TIMEOUT)
+
+        # Write code with a global to a file
+        code = (
+            "def foo1():\n"
+            "    global x\n"
+            "    x = 2\n"
+            "x = 1\n"
+            "print(x)\n"
+        )
+
+        p = tmpdir.join("test.py")
+        p.write(code)
+        global found
+        found = False
+
+        def check_found(msg):
+            if "text" in msg["content"]:
+                if ("WARNING: This file contains a global statement"  in
+                        msg["content"]["text"]):
+                    global found
+                    found = True
+
+        # Run code in current namespace
+        client.execute_interactive("%runfile {} --current-namespace".format(
+            repr(str(p))), timeout=TIMEOUT, output_hook=check_found)
+        assert not found
+
+        # Run code in empty namespace
+        client.execute_interactive(
+            "%runfile {}".format(repr(str(p))), timeout=TIMEOUT,
+            output_hook=check_found)
+
+        assert found
+
+
 @flaky(max_runs=3)
-@pytest.mark.skipif(
-    sys.version_info[0] < 3,
-    reason="Fails with python 2")
 def test_debug_namespace(tmpdir):
     """
     Test that the kernel uses the proper namespace while debugging.
     """
     # Command to start the kernel
     cmd = "from spyder_kernels.console import start; start.main()"
 
     with setup_kernel(cmd) as client:
         # Write code to a file
         d = tmpdir.join("pdb-ns-test.py")
         d.write('def func():\n    bb = "hello"\n    breakpoint()\nfunc()')
 
         # Run code file `d`
-        msg_id = client.execute("runfile(r'{}')".format(to_text_string(d)))
+        msg_id = client.execute("%runfile {}".format(repr(str(d))))
 
         # make sure that 'bb' returns 'hello'
         client.get_stdin_msg(timeout=TIMEOUT)
         client.input('bb')
 
         t0 = time.time()
         while True:
@@ -1184,33 +1232,126 @@
             assert time.time() - t0 < 5
             msg = client.get_iopub_msg(timeout=TIMEOUT)
             if msg.get('msg_type') == 'stream':
                 if 'hello' in msg["content"].get("text"):
                     break
 
 
+def test_interrupt():
+    """
+    Test that the kernel can be interrupted by calling a comm handler.
+    """
+    # Command to start the kernel
+    cmd = "from spyder_kernels.console import start; start.main()"
+    import pickle
+    with setup_kernel(cmd) as client:
+        kernel_comm = CommBase()
+
+        # Create new comm and send the highest protocol
+        comm = Comm(kernel_comm._comm_name, client)
+        comm.open(data={'pickle_highest_protocol': pickle.HIGHEST_PROTOCOL})
+        comm._send_channel = client.control_channel
+        kernel_comm._register_comm(comm)
+
+        client.execute_interactive("import time", timeout=TIMEOUT)
+
+        # Try interrupting loop
+        t0 = time.time()
+        msg_id = client.execute("for i in range(100): time.sleep(.1)")
+        time.sleep(.2)
+        # Raise interrupt on control_channel
+        kernel_comm.remote_call().raise_interrupt_signal()
+        # Wait for shell message
+        while True:
+            assert time.time() - t0 < 5
+            msg = client.get_shell_msg(timeout=TIMEOUT)
+            if msg["parent_header"].get("msg_id") != msg_id:
+                # not from my request
+                continue
+            break
+        assert time.time() - t0 < 5
+
+        if os.name == 'nt':
+            # Windows doesn't do "interrupting sleep"
+            return
+
+        # Try interrupting sleep
+        t0 = time.time()
+        msg_id = client.execute("time.sleep(10)")
+        time.sleep(.2)
+        # Raise interrupt on control_channel
+        kernel_comm.remote_call().raise_interrupt_signal()
+        # Wait for shell message
+        while True:
+            assert time.time() - t0 < 5
+            msg = client.get_shell_msg(timeout=TIMEOUT)
+            if msg["parent_header"].get("msg_id") != msg_id:
+                # not from my request
+                continue
+            break
+        assert time.time() - t0 < 5
+
+
+def test_enter_debug_after_interruption():
+    """
+    Test that we can enter the debugger after interrupting the current
+    execution.
+    """
+    # Command to start the kernel
+    cmd = "from spyder_kernels.console import start; start.main()"
+    import pickle
+    with setup_kernel(cmd) as client:
+        kernel_comm = CommBase()
+
+        # Create new comm and send the highest protocol
+        comm = Comm(kernel_comm._comm_name, client)
+        comm.open(data={'pickle_highest_protocol': pickle.HIGHEST_PROTOCOL})
+        comm._send_channel = client.control_channel
+        kernel_comm._register_comm(comm)
+
+        client.execute_interactive("import time", timeout=TIMEOUT)
+
+        # Try interrupting loop
+        t0 = time.time()
+        msg_id = client.execute("for i in range(100): time.sleep(.1)")
+        time.sleep(.2)
+        # Request to enter the debugger
+        kernel_comm.remote_call().request_pdb_stop()
+        # Wait for debug message
+        while True:
+            assert time.time() - t0 < 5
+            msg = client.get_iopub_msg(timeout=TIMEOUT)
+            if msg.get('msg_type') == 'stream':
+                print(msg["content"].get("text"))
+            if msg["parent_header"].get("msg_id") != msg_id:
+                # not from my request
+                continue
+            if msg.get('msg_type') == 'comm_msg':
+                if msg["content"].get("data", {}).get("content", {}).get(
+                        'call_name') == 'pdb_input':
+                    # pdb entered
+                    break
+                comm.handle_msg(msg)
+
+        assert time.time() - t0 < 5
+
+
 def test_non_strings_in_locals(kernel):
     """
     Test that we can hande non-string entries in `locals` when bulding the
     namespace view.
 
     This is a regression test for issue spyder-ide/spyder#19145
     """
-    if IPYKERNEL_6:
-        execute = asyncio.run(kernel.do_execute(
-            'locals().update({1:2})', True))
-    else:
-        execute = kernel.do_execute('locals().update({1:2})', True)
+    execute = asyncio.run(kernel.do_execute('locals().update({1:2})', True))
 
     nsview = repr(kernel.get_namespace_view())
     assert "1:" in nsview
 
 
-@pytest.mark.skipif(
-    sys.version_info[0] < 3, reason="Doesn't work with Python 2")
 def test_django_settings(kernel):
     """
     Test that we don't generate errors when importing `django.conf.settings`.
 
     This is a regression test for issue spyder-ide/spyder#19516
     """
     execute = asyncio.run(kernel.do_execute(
```

### Comparing `spyder-kernels-2.4.3/spyder_kernels/customize/spyderpdb.py` & `spyder-kernels-3.0.0b1/spyder_kernels/customize/spyderpdb.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,114 +5,117 @@
 # Licensed under the terms of the MIT License
 # (see spyder_kernels/__init__.py for details)
 
 """Spyder debugger."""
 
 import ast
 import bdb
+import builtins
+from contextlib import contextmanager
 import logging
 import os
 import sys
 import traceback
 import threading
 from collections import namedtuple
 
 from IPython.core.autocall import ZMQExitAutocall
 from IPython.core.debugger import Pdb as ipyPdb
-from IPython.core.getipython import get_ipython
+from IPython.core.inputtransformer2 import TransformerManager
 
+import spyder_kernels
 from spyder_kernels.comms.frontendcomm import CommError, frontend_request
 from spyder_kernels.customize.utils import path_is_library, capture_last_Expr
-from spyder_kernels.py3compat import (
-    TimeoutError, PY2, _print, isidentifier, PY3, input)
-
-if not PY2:
-    from IPython.core.inputtransformer2 import TransformerManager
-    import builtins
-    basestring = (str,)
-else:
-    import __builtin__ as builtins
-    from IPython.core.inputsplitter import IPythonInputSplitter as TransformerManager
 
 
 logger = logging.getLogger(__name__)
 
 
-class DebugWrapper(object):
+class DebugWrapper:
     """
     Notifies the frontend when debugging starts/stops
     """
     def __init__(self, pdb_obj):
         self.pdb_obj = pdb_obj
+        self._cleanup = True
 
     def __enter__(self):
         """
         Debugging starts.
         """
-        self.pdb_obj._frontend_notified = True
-        try:
-            frontend_request(blocking=True).set_debug_state(True)
-        except (CommError, TimeoutError):
-            logger.debug("Could not send debugging state to the frontend.")
+        shell = self.pdb_obj.shell
+        if shell.pdb_session == self.pdb_obj:
+            self._cleanup = False
+        else:
+            shell.add_pdb_session(self.pdb_obj)
+            self._cleanup = True
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         """
         Debugging ends.
         """
-        self.pdb_obj._frontend_notified = False
-        try:
-            frontend_request(blocking=True).set_debug_state(False)
-        except (CommError, TimeoutError):
-            logger.debug("Could not send debugging state to the frontend.")
+        if self._cleanup:
+            self.pdb_obj.shell.remove_pdb_session(self.pdb_obj)
 
 
-class SpyderPdb(ipyPdb, object):  # Inherits `object` to call super() in PY2
+class SpyderPdb(ipyPdb):
     """
     Extends Pdb to add features:
 
      - Process IPython magics.
      - Accepts multiline input.
      - Better interrupt signal handling.
      - Option to skip libraries while stepping.
      - Add completion to non-command code.
     """
 
-    send_initial_notification = True
-    starting = True
-
     def __init__(self, completekey='tab', stdin=None, stdout=None,
                  skip=None, nosigint=False):
         """Init Pdb."""
         self.curframe_locals = None
         # Only set to true when calling debugfile
         self.continue_if_has_breakpoints = False
         self.pdb_ignore_lib = False
         self.pdb_execute_events = False
         self.pdb_use_exclamation_mark = False
+        self.pdb_publish_stack = False
         self._exclamation_warning_printed = False
         self.pdb_stop_first_line = True
         self._disable_next_stack_entry = False
         super(SpyderPdb, self).__init__()
-        self._pdb_breaking = False
-        self._frontend_notified = False
 
         # content of tuple: (filename, line number)
         self._previous_step = None
 
         # Don't report hidden frames for IPython 7.24+. This attribute
         # has no effect in previous versions.
         self.report_skipped = False
 
-
         # Keep track of remote filename
         self.remote_filename = None
 
+        # Needed to know which namespace to show (user or current frame)
         # Line received from the frontend
         self._cmd_input_line = None
 
+        # Disable sigint so we can do it ourselves
+        self.nosigint = True
+
+        # Keep track of interrupting state to avoid several interruptions
+        self.interrupting = False
+
+        # Turn off IPython's debugger skip funcionality by default because
+        # it makes our debugger quite slow. It's also important to remark
+        # that this functionality doesn't do anything on its own. Users
+        # need to mark what frames they want to skip for it to be useful.
+        # So, we hope that knowledgeable users will find that they need to
+        # enable it in Spyder.
+        # Fixes spyder-ide/spyder#20639.
+        self._predicates["debuggerskip"] = False
+
     # --- Methods overriden for code execution
     def print_exclamation_warning(self):
         """Print pdb warning for exclamation mark."""
         if not self._exclamation_warning_printed:
             print("Warning: The exclamation mark option is enabled. "
                   "Please use '!' as a prefix for Pdb commands.")
             self._exclamation_warning_printed = True
@@ -124,20 +127,21 @@
         execute_events = self.pdb_execute_events
         if line[:1] == '!':
             line = line[1:]
         elif self.pdb_use_exclamation_mark:
             self.print_exclamation_warning()
             self.error("Unknown command '" + line.split()[0] + "'")
             return
-        # Disallow the use of %debug magic in the debugger
-        if line.startswith("%debug"):
-            self.error("Please don't use '%debug' in the debugger.\n"
-                       "For a recursive debugger, use the pdb 'debug'"
-                       " command instead")
-            return
+
+        # Replace %debug magic in the debugger
+        if line.startswith("%debug") or line.startswith("%%debug"):
+            cmd, arg, _ = self.parseline(line.lstrip("%"))
+            if cmd == "debug":
+                return self.do_debug(arg)
+
         locals = self.curframe_locals
         globals = self.curframe.f_globals
 
         if self.pdb_use_exclamation_mark:
             # Find pdb commands executed without !
             cmd, arg, line = self.parseline(line)
             if cmd:
@@ -178,25 +182,27 @@
             save_stdin = sys.stdin
             save_displayhook = sys.displayhook
             try:
                 sys.stdin = self.stdin
                 sys.stdout = self.stdout
                 sys.displayhook = self.displayhook
                 if execute_events:
-                     get_ipython().events.trigger('pre_execute')
+                     self.shell.events.trigger('pre_execute')
 
                 code_ast = ast.parse(line)
 
                 if line.rstrip()[-1:] == ";":
                     # Supress output with ;
                     capture_last_expression = False
                 else:
                     code_ast, capture_last_expression = capture_last_Expr(
                         code_ast, "_spyderpdb_out")
 
+                globals["__spyder_builtins__"] = builtins
+
                 if locals is not globals:
                     # Mitigates a behaviour of CPython that makes it difficult
                     # to work with exec and the local namespace
                     # See:
                     #  - https://bugs.python.org/issue41918
                     #  - https://bugs.python.org/issue46153
                     #  - https://bugs.python.org/issue21161
@@ -213,52 +219,59 @@
                     # a copy of the curframe locals. This means that closures
                     # for example are early binding instead of late binding.
 
                     # Create a function
                     indent = "    "
                     code = ["def _spyderpdb_code():"]
 
-                    # Load the locals
-                    globals["_spyderpdb_builtins_locals"] = builtins.locals
-
-                    # Save builtins locals in case it is shadowed
-                    globals["_spyderpdb_locals"] = locals
+                    # Add locals in globals
+                    # If the debugger is recursive, the globals could already
+                    # have a _spyderpdb_locals as it might be shared between
+                    # levels
+                    if "_spyderpdb_locals" in globals:
+                        globals["_spyderpdb_locals"].append(locals)
+                    else:
+                        globals["_spyderpdb_locals"] = [locals]
 
                     # Load locals if they have a valid name
                     # In comprehensions, locals could contain ".0" for example
-                    code += [indent + "{k} = _spyderpdb_locals['{k}']".format(
-                        k=k) for k in locals if isidentifier(k)]
+                    code += [indent + "{k} = _spyderpdb_locals[-1]['{k}']".format(
+                        k=k) for k in locals if k.isidentifier()]
 
+                    # The code comes here
 
                     # Update the locals
-                    code += [indent + "_spyderpdb_locals.update("
-                             "_spyderpdb_builtins_locals())"]
+                    code += [indent + "_spyderpdb_locals[-1].update("
+                             "__spyder_builtins__.locals())"]
 
                     # Run the function
                     code += ["_spyderpdb_code()"]
 
-                    # Cleanup
-                    code += [
-                        "del _spyderpdb_code",
-                        "del _spyderpdb_locals",
-                        "del _spyderpdb_builtins_locals"
-                    ]
-
                     # Parse the function
                     fun_ast = ast.parse('\n'.join(code) + '\n')
 
                     # Inject code_ast in the function before the locals update
                     fun_ast.body[0].body = (
                         fun_ast.body[0].body[:-1]  # The locals
                         + code_ast.body  # Code to run
                         + fun_ast.body[0].body[-1:]  # Locals update
                     )
                     code_ast = fun_ast
 
-                exec(compile(code_ast, "<stdin>", "exec"), globals)
+                try:
+                    exec(compile(code_ast, "<stdin>", "exec"), globals)
+                finally:
+                    if locals is not globals:
+                        # CLeanup code
+                        globals.pop("_spyderpdb_code", None)
+                        if len(globals["_spyderpdb_locals"]) > 1:
+                            del globals["_spyderpdb_locals"][-1]
+                        else:
+                            del globals["_spyderpdb_locals"]
+                        
 
                 if capture_last_expression:
                     out = globals.pop("_spyderpdb_out", None)
                     if out is not None:
                         sys.stdout.flush()
                         sys.stderr.flush()
                         try:
@@ -266,96 +279,116 @@
                                 repr(out))
                         except (CommError, TimeoutError):
                             # Fallback
                             print("pdb out> ", repr(out))
 
             finally:
                 if execute_events:
-                     get_ipython().events.trigger('post_execute')
+                     self.shell.events.trigger('post_execute')
                 sys.stdout = save_stdout
                 sys.stdin = save_stdin
                 sys.displayhook = save_displayhook
         except BaseException:
-            if PY2:
-                t, v = sys.exc_info()[:2]
-                if type(t) == type(''):
-                    exc_type_name = t
-                else: exc_type_name = t.__name__
-                print >>self.stdout, '***', exc_type_name + ':', v
-            else:
-                exc_info = sys.exc_info()[:2]
-                self.error(
-                    traceback.format_exception_only(*exc_info)[-1].strip())
+            exc_info = sys.exc_info()[:2]
+            self.error(
+                traceback.format_exception_only(*exc_info)[-1].strip())
 
     # --- Methods overriden for signal handling
-    def sigint_handler(self, signum, frame):
-        """
-        Handle a sigint signal. Break on the frame above this one.
-
-        This method is not present in python2 so this won't be called there.
-        """
-        if self.allow_kbdint:
-            raise KeyboardInterrupt
+    def interrupt(self):
+        """Stop debugger on next instruction."""
+        self.interrupting = True
         self.message("\nProgram interrupted. (Use 'cont' to resume).")
-        # avoid stopping in set_trace
-        sys.settrace(None)
-        self._pdb_breaking = True
         self.set_step()
-        self.set_trace(sys._getframe())
+
+    def set_trace(self, frame=None):
+        """Register that debugger is tracing."""
+        self.shell.add_pdb_session(self)
+        super(SpyderPdb, self).set_trace(frame)
+
+    def set_quit(self):
+        """Register that debugger is not tracing."""
+        self.shell.remove_pdb_session(self)
+        super(SpyderPdb, self).set_quit()
 
     def interaction(self, frame, traceback):
         """
         Called when a user interaction is required.
-
-        If this is from sigint, break on the upper frame.
-        If the frame is in spydercustomize.py, quit.
-        Notifies spyder and print current code.
-
         """
-        if self._pdb_breaking:
-            self._pdb_breaking = False
-            if frame and frame.f_back:
-                return self.interaction(frame.f_back, traceback)
-
-        self.setup(frame, traceback)
-        self.print_stack_entry(self.stack[self.curindex])
-        if self._frontend_notified:
-            self._cmdloop()
-        else:
-            with DebugWrapper(self):
-                self._cmdloop()
-        self.forget()
+        with DebugWrapper(self):
+            # Wrapp in case the frontend was not notified, e.g. postmortem
+            return super(SpyderPdb, self).interaction(
+                frame, traceback)
 
-    def print_stack_entry(self, frame_lineno, prompt_prefix='\n-> ',
-                          context=None):
+    def print_stack_entry(self, *args, **kwargs):
         """Disable printing stack entry if requested."""
         if self._disable_next_stack_entry:
             self._disable_next_stack_entry = False
             return
-        return super(SpyderPdb, self).print_stack_entry(
-            frame_lineno, prompt_prefix, context)
+        return super().print_stack_entry(*args, **kwargs)
 
     # --- Methods overriden for skipping libraries
     def stop_here(self, frame):
         """Check if pdb should stop here."""
-        if (frame is not None
-                and "__tracebackhide__" in frame.f_locals
-                and frame.f_locals["__tracebackhide__"] == "__pdb_exit__"):
+        # Never stop if we are continuing unless there is a breakpoint
+        if self.stopframe == self.botframe and self.stoplineno == -1:
+            return False
+        if self.continue_if_has_breakpoints and self.should_continue(frame):
+            self.set_continue()
+            return False
+        if (
+            frame is not None
+            and "__tracebackhide__" in frame.f_locals
+            and frame.f_locals["__tracebackhide__"] == "__pdb_exit__"
+        ):
             self.onecmd('exit')
             return False
 
-        if not super(SpyderPdb, self).stop_here(frame):
+        if not super().stop_here(frame):
             return False
+        if frame is self.stopframe:
+            return True
         filename = frame.f_code.co_filename
         if filename.startswith('<'):
             # This is not a file
             return True
         if self.pdb_ignore_lib and path_is_library(filename):
             return False
+        if self.skip_hidden and os.path.dirname(spyder_kernels.__file__) in filename:
+            # This is spyder-kernels internals
+            return False
         return True
+    
+    def should_continue(self, frame):
+        """
+        Jump to first breakpoint if needed.
+
+        Fixes spyder-ide/spyder#2034
+        """
+
+        if not self.continue_if_has_breakpoints:
+            # This was disabled
+            return False
+        self.continue_if_has_breakpoints = False
+
+        # Get all breakpoints for the file we're going to debug
+        if not frame:
+            # We are not debugging, return. Solves spyder-ide/spyder#10290
+            return False
+
+        lineno = frame.f_lineno
+        breaks = self.get_file_breaks(frame.f_code.co_filename)
+
+        # Do 'continue' if the first breakpoint is *not* placed
+        # where the debugger is going to land.
+        # Fixes spyder-ide/spyder#4681
+        if self.pdb_stop_first_line:
+            return breaks and lineno < breaks[0]
+
+        # The breakpoint could be in another file.
+        return not (breaks and lineno >= breaks[0])
 
     def do_where(self, arg):
         """w(here)
         Print a stack trace, with the most recent frame at the bottom.
         An arrow indicates the "current frame", which determines the
         context of most commands. 'bt' is an alias for this command.
 
@@ -417,40 +450,39 @@
             # This could be a Pdb command
             compfunc = self.completenames
 
         def is_name_or_composed(text):
             if not text or text[0] == '.':
                 return False
             # We want to keep value.subvalue
-            return isidentifier(text.replace('.', ''))
+            return text.replace('.', '').isidentifier()
 
         while text and not is_name_or_composed(text):
             text = text[1:]
             begidx += 1
 
         matches = []
         if compfunc:
             matches = compfunc(text, line, begidx, endidx)
 
         cursor_start = cursor_pos - len(text)
 
         if ipython_do_complete:
-            kernel = get_ipython().kernel
             # Make complete call with current frame
             if self.curframe:
                 if self.curframe_locals:
                     Frame = namedtuple("Frame", ["f_locals", "f_globals"])
                     frame = Frame(self.curframe_locals,
                                   self.curframe.f_globals)
                 else:
                     frame = self.curframe
-                kernel.shell.set_completer_frame(frame)
-            result = kernel._do_complete(code, cursor_pos)
+                self.shell.set_completer_frame(frame)
+            result = self.shell.kernel._do_complete(code, cursor_pos)
             # Reset frame
-            kernel.shell.set_completer_frame()
+            self.shell.set_completer_frame()
             # If there is no Pdb results to merge, return the result
             if not compfunc:
                 return result
 
             ipy_matches = result['matches']
             # Make sure both match lists start at the same place
             if cursor_start < result['cursor_start']:
@@ -520,15 +552,15 @@
 
         if not is_pdb_command_name:
             # Remove eg. leading opening parenthesis
             def is_name_or_composed(text):
                 if not text or text[0] == '.':
                     return False
                 # We want to keep value.subvalue
-                return isidentifier(text.replace('.', ''))
+                return text.replace('.', '').isidentifier()
 
             while text and not is_name_or_composed(text):
                 text = text[1:]
                 begidx += 1
 
         cursor_start = cursor_pos - len(text)
         matches = []
@@ -538,119 +570,117 @@
                 'matches': matches,
                 'cursor_end': cursor_pos,
                 'cursor_start': cursor_start,
                 'metadata': {},
                 'status': 'ok'
                 }
 
-        kernel = get_ipython().kernel
         # Make complete call with current frame
         if self.curframe:
             if self.curframe_locals:
                 Frame = namedtuple("Frame", ["f_locals", "f_globals"])
                 frame = Frame(self.curframe_locals,
                               self.curframe.f_globals)
             else:
                 frame = self.curframe
-            kernel.shell.set_completer_frame(frame)
-        result = kernel._do_complete(code, cursor_pos)
+            self.shell.set_completer_frame(frame)
+        result = self.shell.kernel._do_complete(code, cursor_pos)
         # Reset frame
-        kernel.shell.set_completer_frame()
+        self.shell.set_completer_frame()
         return result
 
     # --- Methods overriden by us for Spyder integration
     def postloop(self):
         # postloop() is called when the debugger’s input prompt exists. Reset
-        # _previous_step so that publish_pdb_state() actually notifies Spyder
+        # _previous_step so that get_pdb_state() actually notifies Spyder
         # about a changed frame the next the input prompt is entered again.
         self._previous_step = None
 
-    def preloop(self):
-        """Ask Spyder for breakpoints before the first prompt is created."""
-        try:
-            pdb_settings = frontend_request(blocking=True).get_pdb_settings()
-            self.pdb_ignore_lib = pdb_settings['pdb_ignore_lib']
-            self.pdb_execute_events = pdb_settings['pdb_execute_events']
-            self.pdb_use_exclamation_mark = pdb_settings[
-                'pdb_use_exclamation_mark']
-            self.pdb_stop_first_line = pdb_settings['pdb_stop_first_line']
-            if self.starting:
-                self.set_spyder_breakpoints(pdb_settings['breakpoints'])
-            if self.send_initial_notification:
-                self.publish_pdb_state()
-        except (CommError, TimeoutError):
-            logger.debug("Could not get breakpoints from the frontend.")
-        super(SpyderPdb, self).preloop()
-
     def set_continue(self):
         """
         Stop only at breakpoints or when finished.
 
         Reimplemented to avoid stepping out of debugging if there are no
         breakpoints. We could add more later.
         """
         # Don't stop except at breakpoints or when finished
         self._set_stopinfo(self.botframe, None, -1)
 
-    def reset(self):
-        """
-        Register Pdb session after reset.
-        """
-        super(SpyderPdb, self).reset()
-        get_ipython().pdb_session = self
-
     def do_debug(self, arg):
         """
         Debug code
 
         Enter a recursive debugger that steps through the code
         argument (which is an arbitrary expression or statement to be
         executed in the current environment).
         """
-        try:
-            super(SpyderPdb, self).do_debug(arg)
-        except Exception:
-            if PY2:
-                t, v = sys.exc_info()[:2]
-                if type(t) == type(''):
-                    exc_type_name = t
-                else: exc_type_name = t.__name__
-                print >>self.stdout, '***', exc_type_name + ':', v
-            else:
+        with self.recursive_debugger() as debugger:
+            self.message("Entering recursive debugger")
+            try:
+                globals = self.curframe.f_globals
+                locals = self.curframe_locals
+                return sys.call_tracing(debugger.run, (arg, globals, locals))
+            except Exception:
                 exc_info = sys.exc_info()[:2]
                 self.error(
                     traceback.format_exception_only(*exc_info)[-1].strip())
-        get_ipython().pdb_session = self
+            finally:
+                self.message("Leaving recursive debugger")
+
+    @contextmanager
+    def recursive_debugger(self):
+        """Get a recursive debugger."""
+        # Save and restore tracing function
+        trace_function = sys.gettrace()
+        sys.settrace(None)
+
+        # Create child debugger
+        debugger = self.__class__(
+            completekey=self.completekey,
+            stdin=self.stdin, stdout=self.stdout)
+        debugger.prompt = "(%s) " % self.prompt.strip()
+        try:
+            yield debugger
+        finally:
+            # Reset parent debugger
+            sys.settrace(trace_function)
+            self.lastcmd = debugger.lastcmd
+
+            # Reset _previous_step so that get_pdb_state() notifies Spyder about
+            # a changed debugger position. The reset is required because the
+            # recursive debugger might change the position, but the parent
+            # debugger (self) is not aware of this.
+            self._previous_step = None
 
     def user_return(self, frame, return_value):
         """This function is called when a return trap is set here."""
         # This is useful when debugging in an active interpreter (otherwise,
         # the debugger will stop before reaching the target file)
         if self._wait_for_mainpyfile:
             if (self.mainpyfile != self.canonic(frame.f_code.co_filename)
                     or frame.f_lineno <= 0):
                 return
             self._wait_for_mainpyfile = False
         super(SpyderPdb, self).user_return(frame, return_value)
 
     def _cmdloop(self):
         """Modifies the error text."""
+        self.interrupting = False
         while True:
             try:
                 # keyboard interrupts allow for an easy way to cancel
                 # the current command, so allow them during interactive input
                 self.allow_kbdint = True
                 self.cmdloop()
                 self.allow_kbdint = False
                 break
             except KeyboardInterrupt:
-                _print("--KeyboardInterrupt--\n"
-                       "For copying text while debugging, use Ctrl+Shift+C",
-                       file=self.stdout)
-
+                print("--KeyboardInterrupt--\n"
+                      "For copying text while debugging, use Ctrl+Shift+C",
+                      file=self.stdout)
 
     def cmdloop(self, intro=None):
         """
         Repeatedly issue a prompt, accept input, parse an initial prefix
         off the received input, and dispatch to action methods, passing them
         the remainder of the line as argument.
         """
@@ -673,36 +703,33 @@
             stop = self.postcmd(stop, line)
         self.postloop()
 
     def cmd_input(self, prompt=''):
         """
         Get input from frontend. Blocks until return
         """
-        kernel = get_ipython().kernel
+        kernel = self.shell.kernel
         # Only works if the comm is open
         if not kernel.frontend_comm.is_open():
             return input(prompt)
 
         # Flush output before making the request.
         sys.stderr.flush()
         sys.stdout.flush()
         sys.__stderr__.flush()
         sys.__stdout__.flush()
 
         # Send the input request.
         self._cmd_input_line = None
-        kernel.frontend_call().pdb_input(prompt)
+        kernel.frontend_call(display_error=True).pdb_input(
+            prompt, state=self.get_pdb_state())
 
         # Allow GUI event loop to update
-        if PY3:
-            is_main_thread = (
-                threading.current_thread() is threading.main_thread())
-        else:
-            is_main_thread = isinstance(
-                threading.current_thread(), threading._MainThread)
+        is_main_thread = (
+            threading.current_thread() is threading.main_thread())
 
         # Get input by running eventloop
         if is_main_thread and kernel.eventloop:
             while self._cmd_input_line is None:
                 eventloop = kernel.eventloop
                 # Check if the current backend is Tk on Windows
                 # to let GUI update.
@@ -740,49 +767,15 @@
         return line
 
     def postcmd(self, stop, line):
         """Hook method executed just after a command dispatch is finished."""
         # Flush in case the command produced output on underlying outputs
         sys.__stderr__.flush()
         sys.__stdout__.flush()
-        self.publish_pdb_state()
-        return super(SpyderPdb, self).postcmd(stop, line)
-
-    if PY2:
-        def break_here(self, frame):
-            """
-            Breakpoints don't work for files with non-ascii chars in Python 2
-
-            Fixes Issue 1484
-            """
-            from bdb import effective
-            filename = self.canonic(frame.f_code.co_filename)
-            try:
-                filename = unicode(filename, "utf-8")
-            except TypeError:
-                pass
-            if filename not in self.breaks:
-                return False
-            lineno = frame.f_lineno
-            if lineno not in self.breaks[filename]:
-                # The line itself has no breakpoint, but maybe the line is the
-                # first line of a function with breakpoint set by function name
-                lineno = frame.f_code.co_firstlineno
-                if lineno not in self.breaks[filename]:
-                    return False
-
-            # flag says ok to delete temp. bp
-            (bp, flag) = effective(filename, lineno, frame)
-            if bp:
-                self.currentbp = bp.number
-                if (flag and bp.temporary):
-                    self.do_clear(str(bp.number))
-                return True
-            else:
-                return False
+        return stop
 
     # --- Methods defined by us for Spyder integration
     def set_spyder_breakpoints(self, breakpoints):
         """Set Spyder breakpoints."""
         self.clear_all_breaks()
         # -----Really deleting all breakpoints:
         for bp in bdb.Breakpoint.bpbynumber:
@@ -798,155 +791,88 @@
                     self.set_break(self.canonic(fname), linenumber,
                                    cond=condition)
                 except ValueError:
                     # Fixes spyder/issues/15546
                     # The file is not readable
                     pass
 
-        # Jump to first breakpoint.
-        # Fixes issue 2034
-        if self.starting:
-            # Only run this after a Pdb session is created
-            self.starting = False
-
-            # Get all breakpoints for the file we're going to debug
-            frame = self.curframe
-            if not frame:
-                # We are not debugging, return. Solves #10290
-                return
-            lineno = frame.f_lineno
-            breaks = self.get_file_breaks(frame.f_code.co_filename)
-
-            # Do 'continue' if the first breakpoint is *not* placed
-            # where the debugger is going to land.
-            # Fixes issue 4681
-            if self.pdb_stop_first_line:
-                do_continue = (
-                    self.continue_if_has_breakpoints
-                    and breaks
-                    and lineno < breaks[0])
-            else:
-                # The breakpoint could be in another file.
-                do_continue = (
-                    self.continue_if_has_breakpoints
-                    and not (breaks and lineno >= breaks[0]))
-
-            if do_continue:
-                try:
-                    if self.pdb_use_exclamation_mark:
-                        cont_cmd = '!continue'
-                    else:
-                        cont_cmd = 'continue'
-                    frontend_request(blocking=False).pdb_execute(cont_cmd)
-                except (CommError, TimeoutError):
-                    logger.debug(
-                        "Could not send a Pdb continue call to the frontend.")
+    breakpoints = property(fset=set_spyder_breakpoints)
 
-    def publish_pdb_state(self):
+    def get_pdb_state(self):
         """
         Send debugger state (frame position) to the frontend.
 
         The state is only sent if it has changed since the last update.
         """
+        state = self.shell.kernel.get_state()
 
         frame = self.curframe
         if frame is None:
             self._previous_step = None
-            return
+            return state
 
         # Get filename and line number of the current frame
         fname = self.canonic(frame.f_code.co_filename)
-        if PY2:
-            try:
-                fname = unicode(fname, "utf-8")
-            except TypeError:
-                pass
         if fname == self.mainpyfile and self.remote_filename is not None:
             fname = self.remote_filename
         lineno = frame.f_lineno
 
         if self._previous_step == (fname, lineno):
-            return
+            # Do not update state if not needed
+            return state
 
         # Set step of the current frame (if any)
         step = {}
         self._previous_step = None
-        if isinstance(fname, basestring) and isinstance(lineno, int):
+        if isinstance(fname, str) and isinstance(lineno, int):
             step = dict(fname=fname, lineno=lineno)
             self._previous_step = (fname, lineno)
 
-        try:
-            frontend_request(blocking=False).pdb_state(dict(step=step))
-        except (CommError, TimeoutError):
-            logger.debug("Could not send Pdb state to the frontend.")
+        state['step'] = step
+
+        if self.pdb_publish_stack:
+            # Publish Pdb stack so we can update the Debugger plugin on Spyder
+            pdb_stack = traceback.StackSummary.extract(self.stack)
+            pdb_index = self.curindex
+
+            skip_hidden = getattr(self, 'skip_hidden', False)
+
+            if skip_hidden:
+                # Filter out the hidden frames
+                hidden = self.hidden_frames(self.stack)
+                pdb_stack = [f for f, h in zip(pdb_stack, hidden) if not h]
+                # Adjust the index
+                pdb_index -= sum(hidden[:pdb_index])
+
+            state['stack'] = (pdb_stack, pdb_index)
+
+        return state
 
     def run(self, cmd, globals=None, locals=None):
         """Debug a statement executed via the exec() function.
 
         globals defaults to __main__.dict; locals defaults to globals.
         """
-        self.starting = True
         with DebugWrapper(self):
             super(SpyderPdb, self).run(cmd, globals, locals)
 
     def runeval(self, expr, globals=None, locals=None):
         """Debug an expression executed via the eval() function.
 
         globals defaults to __main__.dict; locals defaults to globals.
         """
-        self.starting = True
         with DebugWrapper(self):
             super(SpyderPdb, self).runeval(expr, globals, locals)
 
     def runcall(self, *args, **kwds):
         """Debug a single function call.
 
         Return the result of the function call.
         """
-        self.starting = True
         with DebugWrapper(self):
             super(SpyderPdb, self).runcall(*args, **kwds)
 
-    def enter_recursive_debugger(self, code, filename,
-                                 continue_if_has_breakpoints):
-        """
-        Enter debugger recursively.
-        """
-        sys.settrace(None)
-        globals = self.curframe.f_globals
-        locals = self.curframe_locals
-        # Create child debugger
-        debugger = SpyderPdb(
-            completekey=self.completekey,
-            stdin=self.stdin, stdout=self.stdout)
-        debugger.use_rawinput = self.use_rawinput
-        debugger.prompt = "(%s) " % self.prompt.strip()
-
-        debugger.set_remote_filename(filename)
-        debugger.continue_if_has_breakpoints = continue_if_has_breakpoints
-
-        # Enter recursive debugger
-        sys.call_tracing(debugger.run, (code, globals, locals))
-        # Reset parent debugger
-        sys.settrace(self.trace_dispatch)
-        self.lastcmd = debugger.lastcmd
-        get_ipython().pdb_session = self
-
-        # Reset _previous_step so that publish_pdb_state() called from within
-        # postcmd() notifies Spyder about a changed debugger position. The reset
-        # is required because the recursive debugger might change the position,
-        # but the parent debugger (self) is not aware of this.
-        self._previous_step = None
-
     def set_remote_filename(self, filename):
         """Set remote filename to signal Spyder on mainpyfile."""
         self.remote_filename = filename
         self.mainpyfile = self.canonic(filename)
         self._wait_for_mainpyfile = True
-
-
-def get_new_debugger(filename, continue_if_has_breakpoints):
-    """Get a new debugger."""
-    debugger = SpyderPdb()
-    debugger.set_remote_filename(filename)
-    debugger.continue_if_has_breakpoints = continue_if_has_breakpoints
-    return debugger
```

### Comparing `spyder-kernels-2.4.3/spyder_kernels/customize/tests/test_umr.py` & `spyder-kernels-3.0.0b1/spyder_kernels/customize/tests/test_umr.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,23 +12,22 @@
 import os
 import sys
 
 # Third party imports
 import pytest
 
 # Local imports
-from spyder_kernels.py3compat import to_text_string
 from spyder_kernels.customize.umr import UserModuleReloader
 
 
 @pytest.fixture
 def user_module(tmpdir):
     """Create a simple module in tmpdir as an example of a user module."""
-    if to_text_string(tmpdir) not in sys.path:
-        sys.path.append(to_text_string(tmpdir))
+    if str(tmpdir) not in sys.path:
+        sys.path.append(str(tmpdir))
 
     def create_module(modname):
         modfile = tmpdir.mkdir(modname).join('bar.py')
         code = """
 def square(x):
     return x**2
         """
```

### Comparing `spyder-kernels-2.4.3/spyder_kernels/customize/tests/test_utils.py` & `spyder-kernels-3.0.0b1/spyder_kernels/customize/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-2.4.3/spyder_kernels/customize/umr.py` & `spyder-kernels-3.0.0b1/spyder_kernels/customize/umr.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,17 @@
 
 """User module reloader."""
 
 import os
 import sys
 
 from spyder_kernels.customize.utils import path_is_library
-from spyder_kernels.py3compat import PY2, _print
 
 
-class UserModuleReloader(object):
+class UserModuleReloader:
     """
     User Module Reloader (UMR) aims at deleting user modules
     to force Python to deeply reload them during import
 
     pathlist [list]: blacklist in terms of module path
     namelist [list]: blacklist in terms of module name
     """
@@ -39,17 +38,14 @@
         # Add other, necessary modules to the UMR blacklist
         # astropy: See spyder-ide/spyder#6962
         # pytorch: See spyder-ide/spyder#7041
         # fastmat: See spyder-ide/spyder#7190
         # pythoncom: See spyder-ide/spyder#7190
         # tensorflow: See spyder-ide/spyder#8697
         other_modules = ['pytorch', 'pythoncom', 'tensorflow']
-        if PY2:
-            py2_modules = ['astropy', 'fastmat']
-            other_modules = other_modules + py2_modules
         self.namelist = namelist + spy_modules + mpl_modules + other_modules
 
         self.pathlist = pathlist
 
         # List of previously loaded modules
         self.previous_modules = list(sys.modules.keys())
 
@@ -135,9 +131,9 @@
                     del sys.modules[modname]
                 else:
                     continue
 
         # Report reloaded modules
         if self.verbose and self.modnames_to_reload:
             modnames = self.modnames_to_reload
-            _print("\x1b[4;33m%s\x1b[24m%s\x1b[0m"
-                   % ("Reloaded modules", ": "+", ".join(modnames)))
+            print("\x1b[4;33m%s\x1b[24m%s\x1b[0m"
+                  % ("Reloaded modules", ": "+", ".join(modnames)))
```

### Comparing `spyder-kernels-2.4.3/spyder_kernels/customize/utils.py` & `spyder-kernels-3.0.0b1/spyder_kernels/customize/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,36 +93,41 @@
         else:
             return False
     else:
         return False
 
 
 def capture_last_Expr(code_ast, out_varname):
-    """Parse line and modify code to capture in globals the last expression."""
+    """
+    Parse line and modify code to capture in globals the last expression.
+
+    The namespace must contain __spyder_builtins__, which is the builtins module.
+    """
     # Modify ast code to capture the last expression
     capture_last_expression = False
     if (
         len(code_ast.body)
         and isinstance(code_ast.body[-1], ast.Expr)
     ):
         capture_last_expression = True
         expr_node = code_ast.body[-1]
         # Create new assign node
         assign_node = ast.parse(
-            'globals()[{}] = None'.format(repr(out_varname))).body[0]
+            '__spyder_builtins__.globals()[{}] = None'.format(
+                repr(out_varname))).body[0]
         # Replace None by the value
         assign_node.value = expr_node.value
         # Fix line number and column offset
         assign_node.lineno = expr_node.lineno
         assign_node.col_offset = expr_node.col_offset
         if sys.version_info[:2] >= (3, 8):
             # Exists from 3.8, necessary from 3.11
             assign_node.end_lineno = expr_node.end_lineno
             if assign_node.lineno == assign_node.end_lineno:
-                # Add 'globals()[{}] = ' and remove 'None'
+                # Add '__spyder_builtins__.globals()[{}] = ' and remove 'None'
                 assign_node.end_col_offset += expr_node.end_col_offset - 4
             else:
                 assign_node.end_col_offset = expr_node.end_col_offset
         code_ast.body[-1] = assign_node
     return code_ast, capture_last_expression
```

### Comparing `spyder-kernels-2.4.3/spyder_kernels/utils/dochelpers.py` & `spyder-kernels-3.0.0b1/spyder_kernels/utils/dochelpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,18 @@
 # Copyright (c) 2009- Spyder Kernels Contributors
 #
 # Licensed under the terms of the MIT License
 # (see spyder_kernels/__init__.py for details)
 # -----------------------------------------------------------------------------
 
 """Utilities and wrappers around inspect module"""
-
-from __future__ import print_function
-
+import builtins
 import inspect
 import re
 
-# Local imports:
-from spyder_kernels.py3compat import (is_text_string, builtins, get_meth_func,
-                                      get_meth_class_inst, get_meth_class,
-                                      get_func_defaults, to_text_string, PY2)
-
 
 SYMBOLS = r"[^\'\"a-zA-Z0-9_.]"
 
 
 def getobj(txt, last=False):
     """Return the last valid object name in string"""
     txt_end = ""
@@ -53,15 +46,15 @@
 
 def getobjdir(obj):
     """
     For standard objects, will simply return dir(obj)
     In special cases (e.g. WrapITK package), will return only string elements
     of result returned by dir(obj)
     """
-    return [item for item in dir(obj) if is_text_string(item)]
+    return [item for item in dir(obj) if isinstance(item, str)]
 
 
 def getdoc(obj):
     """
     Return text documentation from an object. This comes in a form of
     dictionary with four keys:
 
@@ -80,15 +73,15 @@
     
     # Most of the time doc will only contain ascii characters, but there are
     # some docstrings that contain non-ascii characters. Not all source files
     # declare their encoding in the first line, so querying for that might not
     # yield anything, either. So assume the most commonly used
     # multi-byte file encoding (which also covers ascii). 
     try:
-        docstring = to_text_string(docstring)
+        docstring = str(docstring)
     except:
         pass
     
     # Doc dict keys
     doc = {'name': '',
            'argspec': '',
            'note': '',
@@ -97,35 +90,29 @@
     if callable(obj):
         try:
             name = obj.__name__
         except AttributeError:
             doc['docstring'] = docstring
             return doc
         if inspect.ismethod(obj):
-            imclass = get_meth_class(obj)
-            if get_meth_class_inst(obj) is not None:
+            imclass = obj.__self__.__class__
+            if obj.__self__ is not None:
                 doc['note'] = 'Method of %s instance' \
-                              % get_meth_class_inst(obj).__class__.__name__
+                              % obj.__self__.__class__.__name__
             else:
                 doc['note'] = 'Unbound %s method' % imclass.__name__
-            obj = get_meth_func(obj)
+            obj = obj.__func__
         elif hasattr(obj, '__module__'):
             doc['note'] = 'Function of %s module' % obj.__module__
         else:
             doc['note'] = 'Function'
         doc['name'] = obj.__name__
         if inspect.isfunction(obj):
-            if PY2:
-                args, varargs, varkw, defaults = inspect.getargspec(obj)
-                doc['argspec'] = inspect.formatargspec(
-                    args, varargs, varkw, defaults,
-                    formatvalue=lambda o:'='+repr(o))
-            else:
-                sig = inspect.signature(obj)
-                doc['argspec'] = str(sig)
+            sig = inspect.signature(obj)
+            doc['argspec'] = str(sig)
             if name == '<lambda>':
                 doc['name'] = name + ' lambda '
                 doc['argspec'] = doc['argspec'][1:-1] # remove parentheses
         else:
             argspec = getargspecfromtext(doc['docstring'])
             if argspec:
                 doc['argspec'] = argspec
@@ -154,18 +141,18 @@
     return doc
 
 
 def getsource(obj):
     """Wrapper around inspect.getsource"""
     try:
         try:
-            src = to_text_string(inspect.getsource(obj))
+            src = str(inspect.getsource(obj))
         except TypeError:
             if hasattr(obj, '__class__'):
-                src = to_text_string(inspect.getsource(obj.__class__))
+                src = str(inspect.getsource(obj.__class__))
             else:
                 # Bindings like VTK or ITK require this case
                 src = getdoc(obj)
         return src
     except (TypeError, IOError):
         return
 
@@ -226,15 +213,15 @@
 
 
 def getargs(obj):
     """Get the names and default values of a function's arguments"""
     if inspect.isfunction(obj) or inspect.isbuiltin(obj):
         func_obj = obj
     elif inspect.ismethod(obj):
-        func_obj = get_meth_func(obj)
+        func_obj = obj.__func__
     elif inspect.isclass(obj) and hasattr(obj, '__init__'):
         func_obj = getattr(obj, '__init__')
     else:
         return []
 
     if not hasattr(func_obj, '__code__'):
         # Builtin: try to extract info from doc
@@ -250,15 +237,15 @@
         return getargsfromdoc(obj)
 
     # Supporting tuple arguments in def statement:
     for i_arg, arg in enumerate(args):
         if isinstance(arg, list):
             args[i_arg] = "(%s)" % ", ".join(arg)
 
-    defaults = get_func_defaults(func_obj)
+    defaults = func_obj.__defaults__
     if defaults is not None:
         for index, default in enumerate(defaults):
             args[index + len(args) - len(defaults)] += '=' + repr(default)
 
     if inspect.isclass(obj) or inspect.ismethod(obj):
         if len(args) == 1:
             return None
@@ -329,15 +316,15 @@
             else:
                 return False
         base += '.'+attr
     return True
     
 
 if __name__ == "__main__":
-    class Test(object):
+    class Test:
         def method(self, x, y=2):
             pass
     print(getargtxt(Test.__init__))  # spyder: test-skip
     print(getargtxt(Test.method))  # spyder: test-skip
     print(isdefined('numpy.take', force_import=True))  # spyder: test-skip
     print(isdefined('__import__'))  # spyder: test-skip
     print(isdefined('.keys', force_import=True))  # spyder: test-skip
```

### Comparing `spyder-kernels-2.4.3/spyder_kernels/utils/iofuncs.py` & `spyder-kernels-3.0.0b1/spyder_kernels/utils/iofuncs.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,47 +8,46 @@
 
 """
 Input/Output Utilities
 
 Note: 'load' functions has to return a dictionary from which a globals()
       namespace may be updated
 """
-
-from __future__ import print_function
-
 # Standard library imports
 import sys
 import os
 import os.path as osp
 import tarfile
 import tempfile
 import shutil
 import types
 import json
 import inspect
 import dis
 import copy
 import glob
+import pickle
 
 # Local imports
-from spyder_kernels.py3compat import getcwd, pickle, PY2, to_text_string
 from spyder_kernels.utils.lazymodules import (
     FakeObject, numpy as np, pandas as pd, PIL, scipy as sp)
 
 
+# ---- For Matlab files
+# -----------------------------------------------------------------------------
 class MatlabStruct(dict):
     """
     Matlab style struct, enhanced.
 
     Supports dictionary and attribute style access.  Can be pickled,
     and supports code completion in a REPL.
 
     Examples
     ========
-    >>> from spyder.utils.iofuncs import MatlabStruct
+    >>> from spyder_kernels.utils.iofuncs import MatlabStruct
     >>> a = MatlabStruct()
     >>> a.b = 'spam'  # a["b"] == 'spam'
     >>> a.c["d"] = 'eggs'  # a.c.d == 'eggs'
     >>> print(a)
     {'c': {'d': 'eggs'}, 'b': 'spam'}
 
     """
@@ -78,15 +77,14 @@
 
     def _is_allowed(self, frame):
         """Check for allowed op code in the calling frame"""
         allowed = [dis.opmap['STORE_ATTR'], dis.opmap['LOAD_CONST'],
                    dis.opmap.get('STOP_CODE', 0)]
         bytecode = frame.f_code.co_code
         instruction = bytecode[frame.f_lasti + 3]
-        instruction = ord(instruction) if PY2 else instruction
         return instruction in allowed
 
     __setattr__ = dict.__setitem__
     __delattr__ = dict.__delitem__
 
     @property
     def __dict__(self):
@@ -165,14 +163,16 @@
 
     try:
         sp.io.savemat(filename, data, oned_as='row')
     except Exception as error:
         return str(error)
 
 
+# ---- For arrays
+# -----------------------------------------------------------------------------
 def load_array(filename):
     if np.load is FakeObject:
         return None, ''
 
     try:
         name = osp.splitext(osp.basename(filename))[0]
         data = np.load(filename)
@@ -189,14 +189,16 @@
 def __save_array(data, basename, index):
     """Save numpy array"""
     fname = basename + '_%04d.npy' % index
     np.save(fname, data)
     return fname
 
 
+# ---- For PIL images
+# -----------------------------------------------------------------------------
 if sys.byteorder == 'little':
     _ENDIAN = '<'
 else:
     _ENDIAN = '>'
 
 DTYPES = {
     "1": ('|b1', None),
@@ -233,14 +235,16 @@
     try:
         name = osp.splitext(osp.basename(filename))[0]
         return {name: __image_to_array(filename)}, None
     except Exception as error:
         return None, str(error)
 
 
+# ---- For misc formats
+# -----------------------------------------------------------------------------
 def load_pickle(filename):
     """Load a pickle file as a dictionary"""
     try:
         if pd.read_pickle is not FakeObject:
             return pd.read_pickle(filename), None
         else:
             with open(filename, 'rb') as fid:
@@ -249,29 +253,27 @@
     except Exception as err:
         return None, str(err)
 
 
 def load_json(filename):
     """Load a json file as a dictionary"""
     try:
-        if PY2:
-            args = 'rb'
-        else:
-            args = 'r'
-        with open(filename, args) as fid:
+        with open(filename, 'r') as fid:
             data = json.load(fid)
         return data, None
     except Exception as err:
         return None, str(err)
 
 
+# ---- For Spydata files
+# -----------------------------------------------------------------------------
 def save_dictionary(data, filename):
     """Save dictionary in a single file .spydata file"""
     filename = osp.abspath(filename)
-    old_cwd = getcwd()
+    old_cwd = os.getcwd()
     os.chdir(osp.dirname(filename))
     error_message = None
     skipped_keys = []
     data_copy = {}
 
     try:
         # Copy dictionary before modifying it to fix #6689
@@ -354,15 +356,15 @@
         # This improves interoperability and UTF-8/long variable name support.
         with tarfile.open(filename, "w", format=tarfile.PAX_FORMAT) as tar:
             for fname in ([pickle_filename]
                           + [fn for fn in list(saved_arrays.values())]):
                 tar.add(osp.basename(fname))
                 os.remove(fname)
     except (RuntimeError, pickle.PicklingError, TypeError) as error:
-        error_message = to_text_string(error)
+        error_message = str(error)
     else:
         if skipped_keys:
             skipped_keys.sort()
             error_message = ('Some objects could not be saved: '
                              + ', '.join(skipped_keys))
     finally:
         os.chdir(old_cwd)
@@ -373,44 +375,39 @@
     """Check if a file is within a directory."""
     abs_directory = os.path.abspath(directory)
     abs_target = os.path.abspath(target)
     prefix = os.path.commonprefix([abs_directory, abs_target])
     return prefix == abs_directory
 
 
-def safe_extract(tar, path=".", members=None, numeric_owner=False):
+def safe_extract(tar, path=".", members=None, *, numeric_owner=False):
     """Safely extract a tar file."""
     for member in tar.getmembers():
         member_path = os.path.join(path, member.name)
         if not is_within_directory(path, member_path):
             raise Exception(
-                "Attempted path traversal in tar file {}".format(
-                    repr(tar.name)
-                )
+                f"Attempted path traversal in tar file {tar.name!r}"
             )
     tar.extractall(path, members, numeric_owner=numeric_owner)
 
 
 def load_dictionary(filename):
     """Load dictionary from .spydata file"""
     filename = osp.abspath(filename)
-    old_cwd = getcwd()
+    old_cwd = os.getcwd()
     tmp_folder = tempfile.mkdtemp()
     os.chdir(tmp_folder)
     data = None
     error_message = None
     try:
         with tarfile.open(filename, "r") as tar:
-            if PY2:
-                tar.extractall()
-            else:
-                safe_extract(tar)
+            safe_extract(tar)
 
         pickle_filename = glob.glob('*.pickle')[0]
-        # 'New' format (Spyder >=2.2 for Python 2 and Python 3)
+        # 'New' format (Spyder >=2.2)
         with open(pickle_filename, 'rb') as fdesc:
             data = pickle.loads(fdesc.read())
         saved_arrays = {}
         if np.load is not FakeObject:
             # Loading numpy arrays saved with np.save
             try:
                 saved_arrays = data.pop('__saved_arrays__')
@@ -422,95 +419,169 @@
                         data[name][index] = arr
                     else:
                         data[name].insert(index, arr)
             except KeyError:
                 pass
     # Except AttributeError from e.g. trying to load function no longer present
     except (AttributeError, EOFError, ValueError) as error:
-        error_message = to_text_string(error)
+        error_message = str(error)
     # To ensure working dir gets changed back and temp dir wiped no matter what
     finally:
         os.chdir(old_cwd)
         try:
             shutil.rmtree(tmp_folder)
         except OSError as error:
-            error_message = to_text_string(error)
+            error_message = str(error)
     return data, error_message
 
 
-class IOFunctions(object):
+# ---- For HDF5 files
+# -----------------------------------------------------------------------------
+def load_hdf5(filename):
+    """
+    Load an hdf5 file.
+
+    Notes
+    -----
+    - This is a fairly dumb implementation which reads the whole HDF5 file into
+      Spyder's variable explorer.  Since HDF5 files are designed for storing
+      very large data-sets, it may be much better to work directly with the
+      HDF5 objects, thus keeping the data on disk. Nonetheless, this gives
+      quick and dirty but convenient access to them.
+    - There is no support for creating files with compression, chunking etc,
+      although these can be read without problem.
+    - When reading an HDF5 file with sub-groups, groups in the file will
+      correspond to dictionaries with the same layout.
+    """
+    def get_group(group):
+        contents = {}
+        for name, obj in list(group.items()):
+            if isinstance(obj, h5py.Dataset):
+                contents[name] = np.array(obj)
+            elif isinstance(obj, h5py.Group):
+                # it is a group, so call self recursively
+                contents[name] = get_group(obj)
+            # other objects such as links are ignored
+        return contents
+
+    try:
+        import h5py
+
+        f = h5py.File(filename, 'r')
+        contents = get_group(f)
+        f.close()
+        return contents, None
+    except Exception as error:
+        return None, str(error)
+
+
+def save_hdf5(data, filename):
+    """
+    Save an hdf5 file.
+
+    Notes
+    -----
+    - All datatypes to be saved must be convertible to a numpy array, otherwise
+      an exception will be raised.
+    - Data attributes are currently ignored.
+    - When saving data after reading it with load_hdf5, dictionaries are not
+      turned into HDF5 groups.
+    """
+    try:
+        import h5py
+
+        f = h5py.File(filename, 'w')
+        for key, value in list(data.items()):
+            f[key] = np.array(value)
+        f.close()
+    except Exception as error:
+        return str(error)
+
+
+# ---- For DICOM files
+# -----------------------------------------------------------------------------
+def load_dicom(filename):
+    """Load a DICOM files."""
+    try:
+        from pydicom import dicomio
+
+        name = osp.splitext(osp.basename(filename))[0]
+        try:
+            data = dicomio.read_file(filename, force=True)
+        except TypeError:
+            data = dicomio.read_file(filename)
+        arr = data.pixel_array
+        return {name: arr}, None
+    except Exception as error:
+        return None, str(error)
+
+
+# ---- Class to group all IO functionality
+# -----------------------------------------------------------------------------
+class IOFunctions:
     def __init__(self):
         self.load_extensions = None
         self.save_extensions = None
         self.load_filters = None
         self.save_filters = None
         self.load_funcs = None
         self.save_funcs = None
 
     def setup(self):
-        iofuncs = self.get_internal_funcs()+self.get_3rd_party_funcs()
+        iofuncs = self.get_internal_funcs()
         load_extensions = {}
         save_extensions = {}
         load_funcs = {}
         save_funcs = {}
         load_filters = []
         save_filters = []
         load_ext = []
+
         for ext, name, loadfunc, savefunc in iofuncs:
-            filter_str = to_text_string(name + " (*%s)" % ext)
+            filter_str = str(name + " (*%s)" % ext)
             if loadfunc is not None:
                 load_filters.append(filter_str)
                 load_extensions[filter_str] = ext
                 load_funcs[ext] = loadfunc
                 load_ext.append(ext)
             if savefunc is not None:
                 save_extensions[filter_str] = ext
                 save_filters.append(filter_str)
                 save_funcs[ext] = savefunc
-        load_filters.insert(0, to_text_string("Supported files"+" (*"+\
-                                              " *".join(load_ext)+")"))
-        load_filters.append(to_text_string("All files (*.*)"))
+
+        load_filters.insert(
+            0, str("Supported files" + " (*" + " *".join(load_ext) + ")")
+        )
+        load_filters.append(str("All files (*.*)"))
+
         self.load_filters = "\n".join(load_filters)
         self.save_filters = "\n".join(save_filters)
         self.load_funcs = load_funcs
         self.save_funcs = save_funcs
         self.load_extensions = load_extensions
         self.save_extensions = save_extensions
 
     def get_internal_funcs(self):
         return [
-                ('.spydata', "Spyder data files",
-                             load_dictionary, save_dictionary),
-                ('.npy', "NumPy arrays", load_array, None),
-                ('.npz', "NumPy zip arrays", load_array, None),
-                ('.mat', "Matlab files", load_matlab, save_matlab),
-                ('.csv', "CSV text files", 'import_wizard', None),
-                ('.txt', "Text files", 'import_wizard', None),
-                ('.jpg', "JPEG images", load_image, None),
-                ('.png', "PNG images", load_image, None),
-                ('.gif', "GIF images", load_image, None),
-                ('.tif', "TIFF images", load_image, None),
-                ('.pkl', "Pickle files", load_pickle, None),
-                ('.pickle', "Pickle files", load_pickle, None),
-                ('.json', "JSON files", load_json, None),
-                ]
-
-    def get_3rd_party_funcs(self):
-        other_funcs = []
-        try:
-            from spyder.otherplugins import get_spyderplugins_mods
-            for mod in get_spyderplugins_mods(io=True):
-                try:
-                    other_funcs.append((mod.FORMAT_EXT, mod.FORMAT_NAME,
-                                        mod.FORMAT_LOAD, mod.FORMAT_SAVE))
-                except AttributeError as error:
-                    print("%s: %s" % (mod, str(error)), file=sys.stderr)
-        except ImportError:
-            pass
-        return other_funcs
+            ('.spydata', "Spyder data files", load_dictionary, save_dictionary),
+            ('.npy', "NumPy arrays", load_array, None),
+            ('.npz', "NumPy zip arrays", load_array, None),
+            ('.mat', "Matlab files", load_matlab, save_matlab),
+            ('.csv', "CSV text files", 'import_wizard', None),
+            ('.txt', "Text files", 'import_wizard', None),
+            ('.jpg', "JPEG images", load_image, None),
+            ('.png', "PNG images", load_image, None),
+            ('.gif', "GIF images", load_image, None),
+            ('.tif', "TIFF images", load_image, None),
+            ('.pkl', "Pickle files", load_pickle, None),
+            ('.pickle', "Pickle files", load_pickle, None),
+            ('.json', "JSON files", load_json, None),
+            ('.h5', "HDF5 files", load_hdf5, save_hdf5),
+            ('.dcm', "DICOM images", load_dicom, None),
+        ]
 
     def save(self, data, filename):
         ext = osp.splitext(filename)[1].lower()
         if ext in self.save_funcs:
             return self.save_funcs[ext](data, filename)
         else:
             return "<b>Unsupported file type '%s'</b>" % ext
@@ -522,19 +593,16 @@
         else:
             return None, "<b>Unsupported file type '%s'</b>" % ext
 
 iofunctions = IOFunctions()
 iofunctions.setup()
 
 
-def save_auto(data, filename):
-    """Save data into filename, depending on file extension"""
-    pass
-
-
+# ---- Test
+# -----------------------------------------------------------------------------
 if __name__ == "__main__":
     import datetime
     testdict = {'d': 1, 'a': np.random.rand(10, 10), 'b': [1, 2]}
     testdate = datetime.date(1945, 5, 8)
     example = {'str': 'kjkj kj k j j kj k jkj',
                'unicode': u'éù',
                'list': [1, 3, [4, 5, 6], 'kjkj', None],
@@ -545,13 +613,13 @@
                'empty_array': np.array([]),
                'date': testdate,
                'datetime': datetime.datetime(1945, 5, 8),
                }
     import time
     t0 = time.time()
     save_dictionary(example, "test.spydata")
-    print(" Data saved in %.3f seconds" % (time.time()-t0))  # spyder: test-skip
+    print(" Data saved in %.3f seconds" % (time.time()-t0))
     t0 = time.time()
     example2, ok = load_dictionary("test.spydata")
     os.remove("test.spydata")
 
-    print("Data loaded in %.3f seconds" % (time.time()-t0))  # spyder: test-skip
+    print("Data loaded in %.3f seconds" % (time.time()-t0))
```

### Comparing `spyder-kernels-2.4.3/spyder_kernels/utils/lazymodules.py` & `spyder-kernels-3.0.0b1/spyder_kernels/utils/lazymodules.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 
 from spyder_kernels.utils.misc import is_module_installed
 
 
 # =============================================================================
 # Auxiliary classes
 # =============================================================================
-class FakeObject(object):
+class FakeObject:
     """Fake class used in replacement of missing objects"""
     pass
 
 
-class LazyModule(object):
+class LazyModule:
     """Lazy module loader class."""
 
     def __init__(self, modname, second_level_attrs=None):
         """
         Lazy module loader class.
 
         Parameters
```

### Comparing `spyder-kernels-2.4.3/spyder_kernels/utils/misc.py` & `spyder-kernels-3.0.0b1/spyder_kernels/utils/misc.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # (see spyder_kernels/__init__.py for details)
 # -----------------------------------------------------------------------------
 
 """Miscellaneous utilities"""
 
 import re
 
-from spyder_kernels.py3compat import lru_cache
+from functools import lru_cache
 
 
 @lru_cache(maxsize=100)
 def is_module_installed(module_name):
     """
     Simpler version of spyder.utils.programs.is_module_installed.
     """
```

### Comparing `spyder-kernels-2.4.3/spyder_kernels/utils/mpl.py` & `spyder-kernels-3.0.0b1/spyder_kernels/utils/mpl.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-2.4.3/spyder_kernels/utils/nsview.py` & `spyder-kernels-3.0.0b1/spyder_kernels/utils/nsview.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,27 +5,18 @@
 # Licensed under the terms of the MIT License
 # (see spyder_kernels/__init__.py for details)
 # -----------------------------------------------------------------------------
 
 """
 Utilities to build a namespace view.
 """
-
-from __future__ import print_function
-
 from itertools import islice
 import inspect
 import re
 
-# Local imports
-from spyder_kernels.py3compat import (NUMERIC_TYPES, INT_TYPES, TEXT_TYPES,
-                                      to_text_string, is_text_string,
-                                      is_type_text_string,
-                                      is_binary_string, PY2,
-                                      to_binary_string, iteritems)
 from spyder_kernels.utils.lazymodules import (
     bs4, FakeObject, numpy as np, pandas as pd, PIL)
 
 
 #==============================================================================
 # Numpy support
 #==============================================================================
@@ -270,26 +261,26 @@
             if name == 'module':
                 return value.__name__ + ' module'
             if module == 'builtins':
                 return name + ' object'
             return name + ' object of ' + module + ' module'
         return name
     except Exception:
-        type_str = to_text_string(object_type)
+        type_str = str(object_type)
         return type_str[1:-1]
 
 
 def collections_display(value, level):
     """Display for collections (i.e. list, set, tuple and dict)."""
     is_dict = isinstance(value, dict)
     is_set = isinstance(value, set)
 
     # Get elements
     if is_dict:
-        elements = iteritems(value)
+        elements = iter(value.items())
     else:
         elements = value
 
     # Truncate values
     truncate = False
     if level == 1 and len(value) > 10:
         elements = islice(elements, 10) if is_dict or is_set else value[:10]
@@ -369,119 +360,108 @@
             if level == 0:
                 display = '%s  Mode: %s' % (address(value), value.mode)
             else:
                 display = 'Image'
         elif isinstance(value, pd.DataFrame):
             if level == 0:
                 cols = value.columns
-                if PY2 and len(cols) > 0:
-                    # Get rid of possible BOM utf-8 data present at the
-                    # beginning of a file, which gets attached to the first
-                    # column header when headers are present in the first
-                    # row.
-                    # Fixes Issue 2514
-                    try:
-                        ini_col = to_text_string(cols[0], encoding='utf-8-sig')
-                    except:
-                        ini_col = to_text_string(cols[0])
-                    cols = [ini_col] + [to_text_string(c) for c in cols[1:]]
-                else:
-                    cols = [to_text_string(c) for c in cols]
+                cols = [str(c) for c in cols]
                 display = 'Column names: ' + ', '.join(list(cols))
             else:
                 display = 'Dataframe'
         elif isinstance(value, bs4.element.NavigableString):
             # Fixes Issue 2448
-            display = to_text_string(value)
+            display = str(value)
             if level > 0:
-                display = u"'" + display + u"'"
+                display = "'" + display + "'"
         elif isinstance(value, pd.Index):
             if level == 0:
                 try:
                     display = value._summary()
                 except AttributeError:
                     display = value.summary()
             else:
                 display = 'Index'
-        elif is_binary_string(value):
+        elif isinstance(value, bytes):
             # We don't apply this to classes that extend string types
             # See issue 5636
-            if is_type_text_string(value):
+            if type(value) in [str, bytes]:
                 try:
-                    display = to_text_string(value, 'utf8')
+                    display = str(value, 'utf8')
                     if level > 0:
-                        display = u"'" + display + u"'"
+                        display = "'" + display + "'"
                 except:
                     display = value
                     if level > 0:
                         display = b"'" + display + b"'"
             else:
                 display = default_display(value)
-        elif is_text_string(value):
+        elif isinstance(value, str):
             # We don't apply this to classes that extend string types
             # See issue 5636
-            if is_type_text_string(value):
+            if type(value) in [str, bytes]:
                 display = value
                 if level > 0:
-                    display = u"'" + display + u"'"
+                    display = "'" + display + "'"
             else:
                 display = default_display(value)
+
         elif (isinstance(value, datetime.date) or
               isinstance(value, datetime.timedelta)):
             display = str(value)
-        elif (isinstance(value, NUMERIC_TYPES) or
+        elif (isinstance(value, (int, float, complex)) or
               isinstance(value, bool) or
               isinstance(value, numeric_numpy_types)):
             display = repr(value)
         else:
             if level == 0:
                 display = default_display(value)
             else:
                 display = default_display(value, with_module=False)
     except Exception:
         display = default_display(value)
 
     # Truncate display at 70 chars to avoid freezing Spyder
     # because of large displays
     if len(display) > 70:
-        if is_binary_string(display):
+        if isinstance(display, bytes):
             ellipses = b' ...'
         else:
-            ellipses = u' ...'
+            ellipses = ' ...'
         display = display[:70].rstrip() + ellipses
 
     # Restore Numpy printoptions
     if np_printoptions is not FakeObject:
         np.set_printoptions(**np_printoptions)
 
     return display
 
 
 def display_to_value(value, default_value, ignore_errors=True):
     """Convert back to value"""
     from qtpy.compat import from_qvariant
-    value = from_qvariant(value, to_text_string)
+    value = from_qvariant(value, str)
     try:
         np_dtype = get_numpy_dtype(default_value)
         if isinstance(default_value, bool):
             # We must test for boolean before NumPy data types
             # because `bool` class derives from `int` class
             try:
                 value = bool(float(value))
             except ValueError:
                 value = value.lower() == "true"
         elif np_dtype is not None:
             if 'complex' in str(type(default_value)):
                 value = np_dtype(complex(value))
             else:
                 value = np_dtype(value)
-        elif is_binary_string(default_value):
-            value = to_binary_string(value, 'utf8')
-        elif is_text_string(default_value):
-            value = to_text_string(value)
+        elif isinstance(default_value, bytes):
+            value = bytes(value, 'utf-8')
+        elif isinstance(default_value, str):
+            value = str(value)
         elif isinstance(default_value, complex):
             value = complex(value)
         elif isinstance(default_value, float):
             value = float(value)
         elif isinstance(default_value, int):
             try:
                 value = int(value)
@@ -527,15 +507,15 @@
             return type(item).__name__
         if isinstance(item, pd.Series):
             return "Series"
     except Exception:
         pass
 
     found = re.findall(r"<(?:type|class) '(\S*)'>",
-                       to_text_string(type(item)))
+                       str(type(item)))
     if found:
         if found[0] == 'type':
             return 'class'
         return found[0]
     else:
         return 'Unknown'
 
@@ -608,15 +588,16 @@
 
 def globalsfilter(input_dict, check_all=False, filters=None,
                   exclude_private=None, exclude_capitalized=None,
                   exclude_uppercase=None, exclude_unsupported=None,
                   excluded_names=None, exclude_callables_and_modules=None):
     """Keep objects in namespace view according to different criteria."""
     output_dict = {}
-    _is_string = is_type_text_string
+    def _is_string(obj):
+        return type(obj) in [str, bytes]
 
     for key, value in list(input_dict.items()):
         excluded = (
             (exclude_private and _is_string(key) and key.startswith('_')) or
             (exclude_capitalized and _is_string(key) and key[0].isupper()) or
             (exclude_uppercase and _is_string(key) and key.isupper() and
              len(key) > 1 and not key[1:].isdigit()) or
@@ -646,15 +627,15 @@
 
     Note:
     If you update this list, don't forget to update variablexplorer.rst
     in spyder-docs
     """
     from datetime import date, timedelta
     editable_types = [int, float, complex, list, set, dict, tuple, date,
-                      timedelta] + list(TEXT_TYPES) + list(INT_TYPES)
+                      timedelta, str]
     try:
         from numpy import ndarray, matrix, generic
         editable_types += [ndarray, matrix, generic]
     except:
         pass
     try:
         from pandas import DataFrame, Series, Index
```

### Comparing `spyder-kernels-2.4.3/spyder_kernels/utils/test_utils.py` & `spyder-kernels-3.0.0b1/spyder_kernels/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-2.4.3/spyder_kernels/utils/tests/export_data.spydata` & `spyder-kernels-3.0.0b1/spyder_kernels/utils/tests/export_data.spydata`

 * *Files identical despite different names*

### Comparing `spyder-kernels-2.4.3/spyder_kernels/utils/tests/export_data_renamed.spydata` & `spyder-kernels-3.0.0b1/spyder_kernels/utils/tests/export_data_renamed.spydata`

 * *Files identical despite different names*

### Comparing `spyder-kernels-2.4.3/spyder_kernels/utils/tests/export_data_withfunction.spydata` & `spyder-kernels-3.0.0b1/spyder_kernels/utils/tests/export_data_withfunction.spydata`

 * *Files identical despite different names*

### Comparing `spyder-kernels-2.4.3/spyder_kernels/utils/tests/numpy_data.npz` & `spyder-kernels-3.0.0b1/spyder_kernels/utils/tests/numpy_data.npz`

 * *Files identical despite different names*

### Comparing `spyder-kernels-2.4.3/spyder_kernels/utils/tests/test_dochelpers.py` & `spyder-kernels-3.0.0b1/spyder_kernels/utils/tests/test_dochelpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,24 +16,22 @@
 
 # Test library imports
 import pytest
 
 # Local imports
 from spyder_kernels.utils.dochelpers import (getargtxt, getdoc, getobj,
                                              isdefined)
-from spyder_kernels.py3compat import PY2
 
 
 class Test(object):
     def method(self, x, y=2):
         pass
 
 
-@pytest.mark.skipif(
-    PY2 or os.name == 'nt', reason="Only works on Linux and Mac")
+@pytest.mark.skipif(os.name == 'nt', reason="Only works on Linux and Mac")
 @pytest.mark.skipif(
     sys.platform == 'darwin' and sys.version_info[:2] == (3, 8),
     reason="Fails on Mac with Python 3.8")
 def test_dochelpers():
     """Test dochelpers."""
     assert getargtxt(Test.method) == ['x, ', 'y=2']
     assert not getargtxt(Test.__init__)
```

### Comparing `spyder-kernels-2.4.3/spyder_kernels/utils/tests/test_iofuncs.py` & `spyder-kernels-3.0.0b1/spyder_kernels/utils/tests/test_iofuncs.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,25 +12,26 @@
 
 # Standard library imports
 import io
 import os
 import copy
 
 # Third party imports
+from PIL import ImageFile
 import pytest
 import numpy as np
 
 # Local imports
 import spyder_kernels.utils.iofuncs as iofuncs
-from spyder_kernels.py3compat import is_text_string, PY2
 
 
 # Full path to this file's parent directory for loading data
-LOCATION = os.path.realpath(os.path.join(os.getcwd(),
-                                         os.path.dirname(__file__)))
+LOCATION = os.path.realpath(
+    os.path.join(os.getcwd(), os.path.dirname(__file__))
+)
 
 
 # =============================================================================
 # ---- Helper functions and classes
 # =============================================================================
 def are_namespaces_equal(actual, expected):
     if actual is None and expected is None:
@@ -44,15 +45,15 @@
             are_equal = are_equal and all(
                 [np.all(obj1 == obj2) for obj1, obj2 in zip(expected[var],
                                                             actual[var])])
         print(str(var) + ": " + str(are_equal))
     return are_equal
 
 
-class CustomObj(object):
+class CustomObj:
     """A custom class of objects for testing."""
     def __init__(self, data):
         self.data = None
         if data:
             self.data = data
 
     def __eq__(self, other):
@@ -223,15 +224,14 @@
     inf, _ = iofuncs.load_matlab(path)
     valid = True
     for var in sorted(real_values.keys()):
         valid = valid and bool(np.mean(real_values[var] == inf[var]))
     assert valid
 
 
-@pytest.mark.skipif(PY2, reason="Fails on Python 2")
 @pytest.mark.parametrize('spydata_file_name', ['export_data.spydata',
                                                'export_data_renamed.spydata'])
 def test_spydata_import(spydata_file_name, spydata_values):
     """
     Test spydata handling and variable importing.
 
     This test loads all the variables contained inside a spydata tar
@@ -251,15 +251,15 @@
 
     Checks that the error is caught, the message is passed back,
     and the current working directory is restored afterwards.
     """
     original_cwd = os.getcwd()
     path = os.path.join(LOCATION, 'export_data_withfunction.spydata')
     data, error = iofuncs.load_dictionary(path)
-    assert error and is_text_string(error)
+    assert error and isinstance(error, str)
     assert data is None
     assert os.getcwd() == original_cwd
 
 
 def test_spydata_import_missing_file():
     """
     Test that import fails properly when file is missing, and resets the cwd.
@@ -336,9 +336,29 @@
         if os.path.isfile(path):
             try:
                 os.remove(path)
             except (IOError, OSError, PermissionError):
                 pass
 
 
+def test_save_load_hdf5_files():
+    """Simple test to check that we can save and load HDF5 files."""
+    data = {'a' : [1, 2, 3, 4], 'b' : 4.5}
+    iofuncs.save_hdf5(data, "test.h5")
+
+    expected = ({'a': np.array([1, 2, 3, 4]), 'b': np.array(4.5)}, None)
+    assert repr(iofuncs.load_hdf5("test.h5")) == repr(expected)
+
+
+def test_load_dicom_files():
+    """Check that we can load DICOM files."""
+    # This test pass locally but we need to set the variable below for it to
+    # pass on CIs.
+    # See https://stackoverflow.com/a/47958486/438386 for context.
+    ImageFile.LOAD_TRUNCATED_IMAGES = True
+
+    data = iofuncs.load_dicom(os.path.join(LOCATION, 'data.dcm'))
+    assert data[0]['data'].shape == (512, 512)
+
+
 if __name__ == "__main__":
     pytest.main()
```

### Comparing `spyder-kernels-2.4.3/spyder_kernels/utils/tests/test_lazymodules.py` & `spyder-kernels-3.0.0b1/spyder_kernels/utils/tests/test_lazymodules.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-2.4.3/spyder_kernels/utils/tests/test_nsview.py` & `spyder-kernels-3.0.0b1/spyder_kernels/utils/tests/test_nsview.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 import numpy as np
 import pandas as pd
 import pytest
 import xarray as xr
 import PIL.Image
 
 # Local imports
-from spyder_kernels.py3compat import PY2
 from spyder_kernels.utils.nsview import (
     sort_against, is_supported, value_to_display, get_size,
     get_supported_types, get_type_string, get_numpy_type_string,
     is_editable_type)
 
 
 def generate_complex_object():
@@ -106,15 +105,15 @@
     assert is_supported(none_var, filters=tuple(supported_types[mode]))
     assert is_supported(none_list, filters=tuple(supported_types[mode]))
     assert is_supported(none_dict, filters=tuple(supported_types[mode]))
     assert is_supported(none_tuple, filters=tuple(supported_types[mode]))
 
 
 def test_str_subclass_display():
-    """Test for value_to_display of subclasses of str/basestring."""
+    """Test for value_to_display of subclasses of str."""
     class Test(str):
         def __repr__(self):
             return 'test'
     value = Test()
     value_display = value_to_display(value)
     assert 'Test object' in value_display
 
@@ -280,20 +279,14 @@
 
 
 def test_str_in_container_display():
     """Test that strings are displayed correctly inside lists or dicts."""
     # Assert that both bytes and unicode return the right display
     assert value_to_display([b'a', u'b']) == "['a', 'b']"
 
-    # Encoded unicode gives bytes and it can't be transformed to
-    # unicode again. So this test the except part of
-    # is_binary_string(value) in value_to_display
-    if PY2:
-        assert value_to_display([u'Э'.encode('cp1251')]) == "['\xdd']"
-
 
 def test_ellipses(tmpdir):
     """
     Test that we're adding a binary ellipses when value_to_display of
     a collection is too long and binary.
 
     For issue 6942
@@ -310,35 +303,32 @@
 
 
 def test_get_type_string():
     """Test for get_type_string."""
     # Bools
     assert get_type_string(True) == 'bool'
 
-    # Numeric types (PY2 has long, which disappeared in PY3)
-    if not PY2:
-        expected = ['int', 'float', 'complex']
-        numeric_types = [1, 1.5, 1 + 2j]
-        assert [get_type_string(t) for t in numeric_types] == expected
+    expected = ['int', 'float', 'complex']
+    numeric_types = [1, 1.5, 1 + 2j]
+    assert [get_type_string(t) for t in numeric_types] == expected
 
     # Lists
     assert get_type_string([1, 2, 3]) == 'list'
 
     # Sets
     assert get_type_string({1, 2, 3}) == 'set'
 
     # Dictionaries
     assert get_type_string({'a': 1, 'b': 2}) == 'dict'
 
     # Tuples
     assert get_type_string((1, 2, 3)) == 'tuple'
 
     # Strings
-    if not PY2:
-        assert get_type_string('foo') == 'str'
+    assert get_type_string('foo') == 'str'
 
     # Numpy objects
     assert get_type_string(np.array([1, 2, 3])) == 'NDArray'
 
     masked_array = np.ma.MaskedArray([1, 2, 3], mask=[True, False, True])
     assert get_type_string(masked_array) == 'MaskedArray'
 
@@ -349,15 +339,15 @@
     df = pd.DataFrame([1, 2, 3])
     assert get_type_string(df) == 'DataFrame'
 
     series = pd.Series([1, 2, 3])
     assert get_type_string(series) == 'Series'
 
     index = pd.Index([1, 2, 3])
-    assert get_type_string(index) == 'Int64Index'
+    assert get_type_string(index) in ['Int64Index', 'Index']
 
     # PIL images
     img = PIL.Image.new('RGB', (256,256))
     assert get_type_string(img) == 'PIL.Image.Image'
 
     # Datetime objects
     date = datetime.date(2010, 10, 1)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `spyder-kernels-2.4.3/spyder_kernels.egg-info/PKG-INFO` & `spyder-kernels-3.0.0b1/spyder_kernels.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: spyder-kernels
-Version: 2.4.3
+Version: 3.0.0b1
 Summary: Jupyter kernels for Spyder's console
 Home-page: https://github.com/spyder-ide/spyder-kernels
 Download-URL: https://www.spyder-ide.org/#fh5co-download
 Author: Spyder Development Team
 Author-email: spyderlib@googlegroups.com
 License: MIT
 Keywords: spyder jupyter kernel ipython console
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Jupyter
 Classifier: Framework :: IPython
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Interpreters
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.txt
 License-File: AUTHORS.txt
 
 # Jupyter kernels for the Spyder console
 
@@ -33,15 +32,15 @@
 [![Linux status](https://github.com/spyder-ide/spyder-kernels/workflows/Linux%20tests/badge.svg)](https://github.com/spyder-ide/spyder-kernels/actions?query=workflow%3A%22Linux+tests%22)
 [![Macos status](https://github.com/spyder-ide/spyder-kernels/workflows/Macos%20tests/badge.svg)](https://github.com/spyder-ide/spyder-kernels/actions?query=workflow%3A%22Macos+tests%22)
 [![codecov](https://codecov.io/gh/spyder-ide/spyder-kernels/branch/master/graph/badge.svg)](https://codecov.io/gh/spyder-ide/spyder-kernels/branch/master)
 
 Package that provides Jupyter kernels for use with the consoles of Spyder, the
 Scientific Python Development Environment.
 
-These kernels can launched either through Spyder itself or in an independent
+These kernels can be launched either through Spyder itself or in an independent
 Python session, and allow for interactive or file-based execution of Python
 code inside Spyder.
 
 To learn about creating, connecting to and using these kernels with the Spyder
 console, please read our [documentation](https://docs.spyder-ide.org/current/panes/ipythonconsole.html).
 
 For advice on managing packages and environments with `spyder-kernels`, please read this
```

### Comparing `spyder-kernels-2.4.3/spyder_kernels.egg-info/SOURCES.txt` & `spyder-kernels-3.0.0b1/spyder_kernels.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,47 +4,46 @@
 .gitignore
 AUTHORS.txt
 CHANGELOG.md
 LICENSE.txt
 MANIFEST.in
 README.md
 RELEASE.md
-setup.cfg
 setup.py
 .github/FUNDING.yml
 .github/workflows/linux-pip-tests.yml
 .github/workflows/linux-tests.yml
 .github/workflows/macos-tests.yml
 .github/workflows/windows-tests.yml
 requirements/posix.txt
-requirements/python-27.txt
 requirements/tests.txt
 requirements/windows.txt
 spyder_kernels/__init__.py
 spyder_kernels/_version.py
-spyder_kernels/py3compat.py
 spyder_kernels.egg-info/PKG-INFO
 spyder_kernels.egg-info/SOURCES.txt
 spyder_kernels.egg-info/dependency_links.txt
 spyder_kernels.egg-info/requires.txt
 spyder_kernels.egg-info/top_level.txt
 spyder_kernels/comms/__init__.py
 spyder_kernels/comms/commbase.py
 spyder_kernels/comms/frontendcomm.py
+spyder_kernels/comms/utils.py
 spyder_kernels/console/__init__.py
 spyder_kernels/console/__main__.py
 spyder_kernels/console/kernel.py
 spyder_kernels/console/outstream.py
 spyder_kernels/console/shell.py
 spyder_kernels/console/start.py
 spyder_kernels/console/tests/__init__.py
 spyder_kernels/console/tests/load_data.npz
 spyder_kernels/console/tests/load_data.spydata
 spyder_kernels/console/tests/test_console_kernel.py
 spyder_kernels/customize/__init__.py
+spyder_kernels/customize/code_runner.py
 spyder_kernels/customize/namespace_manager.py
 spyder_kernels/customize/spydercustomize.py
 spyder_kernels/customize/spyderpdb.py
 spyder_kernels/customize/umr.py
 spyder_kernels/customize/utils.py
 spyder_kernels/customize/tests/__init__.py
 spyder_kernels/customize/tests/test_umr.py
@@ -54,14 +53,15 @@
 spyder_kernels/utils/iofuncs.py
 spyder_kernels/utils/lazymodules.py
 spyder_kernels/utils/misc.py
 spyder_kernels/utils/mpl.py
 spyder_kernels/utils/nsview.py
 spyder_kernels/utils/test_utils.py
 spyder_kernels/utils/tests/__init__.py
+spyder_kernels/utils/tests/data.dcm
 spyder_kernels/utils/tests/data.mat
 spyder_kernels/utils/tests/export_data.spydata
 spyder_kernels/utils/tests/export_data_renamed.spydata
 spyder_kernels/utils/tests/export_data_withfunction.spydata
 spyder_kernels/utils/tests/import_data.npz
 spyder_kernels/utils/tests/numpy_data.npz
 spyder_kernels/utils/tests/test_dochelpers.py
```

