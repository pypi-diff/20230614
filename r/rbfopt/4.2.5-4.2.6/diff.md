# Comparing `tmp/rbfopt-4.2.5.tar.gz` & `tmp/rbfopt-4.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rbfopt-4.2.5.tar", last modified: Sun Nov 20 21:02:36 2022, max compression
+gzip compressed data, was "rbfopt-4.2.6.tar", last modified: Wed Jun 14 17:57:45 2023, max compression
```

## Comparing `rbfopt-4.2.5.tar` & `rbfopt-4.2.6.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 nannicini  (1000) nannicini  (1000)        0 2022-11-20 21:02:36.501338 rbfopt-4.2.5/
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)      233 2022-11-17 01:27:23.000000 rbfopt-4.2.5/AUTHORS
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)    18898 2022-11-20 18:08:54.000000 rbfopt-4.2.5/CHANGELOG
--rw-------   0 nannicini  (1000) nannicini  (1000)     1681 2019-03-14 19:18:42.000000 rbfopt-4.2.5/LICENSE
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)       37 2018-05-29 13:05:01.000000 rbfopt-4.2.5/MANIFEST.in
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)    15567 2022-11-20 21:02:36.502338 rbfopt-4.2.5/PKG-INFO
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)    14999 2022-11-20 18:11:01.000000 rbfopt-4.2.5/README.rst
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)       21 2022-11-18 04:37:41.000000 rbfopt-4.2.5/VERSION
-drwxr-xr-x   0 nannicini  (1000) nannicini  (1000)        0 2022-11-20 21:02:36.498338 rbfopt-4.2.5/bin/
--rw-rw-r--   0 nannicini  (1000) nannicini  (1000)    10262 2020-06-26 22:34:46.000000 rbfopt-4.2.5/bin/rbfopt_cl_interface.py
--rw-rw-r--   0 nannicini  (1000) nannicini  (1000)     6374 2020-06-26 22:34:46.000000 rbfopt-4.2.5/bin/rbfopt_test_interface.py
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)   283616 2022-11-17 01:27:23.000000 rbfopt-4.2.5/manual.pdf
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)       61 2017-03-15 15:10:41.000000 rbfopt-4.2.5/requirements.txt
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)       67 2022-11-20 21:02:36.502338 rbfopt-4.2.5/setup.cfg
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)     1989 2022-11-17 01:27:23.000000 rbfopt-4.2.5/setup.py
-drwxr-xr-x   0 nannicini  (1000) nannicini  (1000)        0 2022-11-20 21:02:36.496338 rbfopt-4.2.5/src/
-drwxr-xr-x   0 nannicini  (1000) nannicini  (1000)        0 2022-11-20 21:02:36.499338 rbfopt-4.2.5/src/rbfopt/
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)      765 2022-11-18 04:36:00.000000 rbfopt-4.2.5/src/rbfopt/__init__.py
-drwxr-xr-x   0 nannicini  (1000) nannicini  (1000)        0 2022-11-20 21:02:36.500338 rbfopt-4.2.5/src/rbfopt/doc/
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)     7409 2017-09-04 22:11:30.000000 rbfopt-4.2.5/src/rbfopt/doc/Makefile
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)    12653 2022-11-17 01:27:23.000000 rbfopt-4.2.5/src/rbfopt/doc/conf.py
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)      550 2017-09-04 22:11:30.000000 rbfopt-4.2.5/src/rbfopt/doc/index.rst
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)     7244 2017-09-04 22:11:30.000000 rbfopt-4.2.5/src/rbfopt/doc/make.bat
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)      139 2017-09-04 22:11:30.000000 rbfopt-4.2.5/src/rbfopt/doc/rbfopt_algorithm.rst
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)      148 2017-09-04 22:11:30.000000 rbfopt-4.2.5/src/rbfopt/doc/rbfopt_aux_problems.rst
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)      139 2017-09-04 22:11:30.000000 rbfopt-4.2.5/src/rbfopt/doc/rbfopt_black_box.rst
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)      154 2017-09-04 22:11:30.000000 rbfopt-4.2.5/src/rbfopt/doc/rbfopt_degree0_models.rst
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)      154 2017-09-04 22:11:30.000000 rbfopt-4.2.5/src/rbfopt/doc/rbfopt_degree1_models.rst
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)      157 2017-09-04 22:11:30.000000 rbfopt-4.2.5/src/rbfopt/doc/rbfopt_degreem1_models.rst
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)      142 2017-09-04 22:11:30.000000 rbfopt-4.2.5/src/rbfopt/doc/rbfopt_refinement.rst
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)      136 2017-09-04 22:11:30.000000 rbfopt-4.2.5/src/rbfopt/doc/rbfopt_settings.rst
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)      154 2017-09-04 22:11:30.000000 rbfopt-4.2.5/src/rbfopt/doc/rbfopt_test_functions.rst
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)      154 2017-09-04 22:11:30.000000 rbfopt-4.2.5/src/rbfopt/doc/rbfopt_user_black_box.rst
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)      127 2017-09-04 22:11:30.000000 rbfopt-4.2.5/src/rbfopt/doc/rbfopt_utils.rst
-drwxr-xr-x   0 nannicini  (1000) nannicini  (1000)        0 2022-11-20 21:02:36.500338 rbfopt-4.2.5/src/rbfopt/examples/
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)     6024 2022-11-17 01:27:23.000000 rbfopt-4.2.5/src/rbfopt/examples/rbfopt_black_box_example.py
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)   133694 2022-11-18 20:08:49.000000 rbfopt-4.2.5/src/rbfopt/rbfopt_algorithm.py
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)    61159 2022-11-17 01:27:23.000000 rbfopt-4.2.5/src/rbfopt/rbfopt_aux_problems.py
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)     4352 2022-11-17 01:27:23.000000 rbfopt-4.2.5/src/rbfopt/rbfopt_black_box.py
--rw-rw-r--   0 nannicini  (1000) nannicini  (1000)    39709 2020-06-26 22:34:46.000000 rbfopt-4.2.5/src/rbfopt/rbfopt_degree0_models.py
--rw-rw-r--   0 nannicini  (1000) nannicini  (1000)    42746 2020-06-26 22:34:46.000000 rbfopt-4.2.5/src/rbfopt/rbfopt_degree1_models.py
--rw-rw-r--   0 nannicini  (1000) nannicini  (1000)    33837 2020-06-26 22:34:46.000000 rbfopt-4.2.5/src/rbfopt/rbfopt_degreem1_models.py
--rw-rw-r--   0 nannicini  (1000) nannicini  (1000)    18570 2020-06-26 22:34:46.000000 rbfopt-4.2.5/src/rbfopt/rbfopt_refinement.py
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)    29030 2022-11-18 04:44:20.000000 rbfopt-4.2.5/src/rbfopt/rbfopt_settings.py
--rw-rw-r--   0 nannicini  (1000) nannicini  (1000)   116828 2022-11-15 04:56:38.000000 rbfopt-4.2.5/src/rbfopt/rbfopt_test_functions.py
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)     6690 2022-11-17 01:27:23.000000 rbfopt-4.2.5/src/rbfopt/rbfopt_user_black_box.py
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)    76345 2022-11-18 02:27:20.000000 rbfopt-4.2.5/src/rbfopt/rbfopt_utils.py
-drwxr-xr-x   0 nannicini  (1000) nannicini  (1000)        0 2022-11-20 21:02:36.499338 rbfopt-4.2.5/src/rbfopt.egg-info/
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)    15567 2022-11-20 21:02:36.000000 rbfopt-4.2.5/src/rbfopt.egg-info/PKG-INFO
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)     1710 2022-11-20 21:02:36.000000 rbfopt-4.2.5/src/rbfopt.egg-info/SOURCES.txt
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)        1 2022-11-20 21:02:36.000000 rbfopt-4.2.5/src/rbfopt.egg-info/dependency_links.txt
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)        1 2017-08-22 13:23:44.000000 rbfopt-4.2.5/src/rbfopt.egg-info/not-zip-safe
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)       18 2022-11-20 21:02:36.000000 rbfopt-4.2.5/src/rbfopt.egg-info/requires.txt
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)        7 2022-11-20 21:02:36.000000 rbfopt-4.2.5/src/rbfopt.egg-info/top_level.txt
-drwxr-xr-x   0 nannicini  (1000) nannicini  (1000)        0 2022-11-20 21:02:36.501338 rbfopt-4.2.5/tests/
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)        0 2017-09-04 22:11:30.000000 rbfopt-4.2.5/tests/__init__.py
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)      109 2017-09-04 22:11:30.000000 rbfopt-4.2.5/tests/context.py
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)    29576 2022-11-18 20:09:19.000000 rbfopt-4.2.5/tests/slow_test_rbfopt_algorithm.py
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)    22288 2022-11-20 01:50:02.000000 rbfopt-4.2.5/tests/test_rbfopt_algorithm.py
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)    24590 2022-11-17 01:27:23.000000 rbfopt-4.2.5/tests/test_rbfopt_aux_problems.py
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)    12439 2022-11-17 01:27:23.000000 rbfopt-4.2.5/tests/test_rbfopt_degree0_models.py
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)    13223 2022-11-17 01:27:23.000000 rbfopt-4.2.5/tests/test_rbfopt_degree1_models.py
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)     6575 2022-11-17 01:27:23.000000 rbfopt-4.2.5/tests/test_rbfopt_degreem1_models.py
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)     1786 2022-11-17 01:27:23.000000 rbfopt-4.2.5/tests/test_rbfopt_mwe.py
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)     9732 2022-11-17 01:27:23.000000 rbfopt-4.2.5/tests/test_rbfopt_refinement.py
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)     4836 2022-11-18 01:30:07.000000 rbfopt-4.2.5/tests/test_rbfopt_settings.py
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)     3196 2022-11-17 01:27:23.000000 rbfopt-4.2.5/tests/test_rbfopt_test_functions.py
--rw-r--r--   0 nannicini  (1000) nannicini  (1000)    38393 2022-11-18 02:28:47.000000 rbfopt-4.2.5/tests/test_rbfopt_utils.py
+drwxr-xr-x   0 nannicini  (1000) nannicini  (1000)        0 2023-06-14 17:57:45.585514 rbfopt-4.2.6/
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)      233 2022-11-17 01:27:23.000000 rbfopt-4.2.6/AUTHORS
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)    18898 2022-11-20 18:08:54.000000 rbfopt-4.2.6/CHANGELOG
+-rw-------   0 nannicini  (1000) nannicini  (1000)     1681 2019-03-14 19:18:42.000000 rbfopt-4.2.6/LICENSE
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)       37 2018-05-29 13:05:01.000000 rbfopt-4.2.6/MANIFEST.in
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)    15547 2023-06-14 17:57:45.585514 rbfopt-4.2.6/PKG-INFO
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)    14999 2022-11-20 18:11:01.000000 rbfopt-4.2.6/README.rst
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)       21 2023-06-14 17:55:26.000000 rbfopt-4.2.6/VERSION
+drwxr-xr-x   0 nannicini  (1000) nannicini  (1000)        0 2023-06-14 17:57:45.576514 rbfopt-4.2.6/bin/
+-rw-rw-r--   0 nannicini  (1000) nannicini  (1000)    10262 2020-06-26 22:34:46.000000 rbfopt-4.2.6/bin/rbfopt_cl_interface.py
+-rw-rw-r--   0 nannicini  (1000) nannicini  (1000)     6374 2020-06-26 22:34:46.000000 rbfopt-4.2.6/bin/rbfopt_test_interface.py
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)   283616 2022-11-17 01:27:23.000000 rbfopt-4.2.6/manual.pdf
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)       61 2017-03-15 15:10:41.000000 rbfopt-4.2.6/requirements.txt
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)       67 2023-06-14 17:57:45.586514 rbfopt-4.2.6/setup.cfg
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)     1989 2022-11-17 01:27:23.000000 rbfopt-4.2.6/setup.py
+drwxr-xr-x   0 nannicini  (1000) nannicini  (1000)        0 2023-06-14 17:57:45.571514 rbfopt-4.2.6/src/
+drwxr-xr-x   0 nannicini  (1000) nannicini  (1000)        0 2023-06-14 17:57:45.577514 rbfopt-4.2.6/src/rbfopt/
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)      765 2023-06-14 17:57:03.000000 rbfopt-4.2.6/src/rbfopt/__init__.py
+drwxr-xr-x   0 nannicini  (1000) nannicini  (1000)        0 2023-06-14 17:57:45.580514 rbfopt-4.2.6/src/rbfopt/doc/
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)     7409 2017-09-04 22:11:30.000000 rbfopt-4.2.6/src/rbfopt/doc/Makefile
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)    12662 2023-06-14 17:38:18.000000 rbfopt-4.2.6/src/rbfopt/doc/conf.py
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)      550 2017-09-04 22:11:30.000000 rbfopt-4.2.6/src/rbfopt/doc/index.rst
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)     7244 2017-09-04 22:11:30.000000 rbfopt-4.2.6/src/rbfopt/doc/make.bat
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)      139 2017-09-04 22:11:30.000000 rbfopt-4.2.6/src/rbfopt/doc/rbfopt_algorithm.rst
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)      148 2017-09-04 22:11:30.000000 rbfopt-4.2.6/src/rbfopt/doc/rbfopt_aux_problems.rst
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)      139 2017-09-04 22:11:30.000000 rbfopt-4.2.6/src/rbfopt/doc/rbfopt_black_box.rst
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)      154 2017-09-04 22:11:30.000000 rbfopt-4.2.6/src/rbfopt/doc/rbfopt_degree0_models.rst
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)      154 2017-09-04 22:11:30.000000 rbfopt-4.2.6/src/rbfopt/doc/rbfopt_degree1_models.rst
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)      157 2017-09-04 22:11:30.000000 rbfopt-4.2.6/src/rbfopt/doc/rbfopt_degreem1_models.rst
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)      142 2017-09-04 22:11:30.000000 rbfopt-4.2.6/src/rbfopt/doc/rbfopt_refinement.rst
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)      136 2017-09-04 22:11:30.000000 rbfopt-4.2.6/src/rbfopt/doc/rbfopt_settings.rst
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)      154 2017-09-04 22:11:30.000000 rbfopt-4.2.6/src/rbfopt/doc/rbfopt_test_functions.rst
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)      154 2017-09-04 22:11:30.000000 rbfopt-4.2.6/src/rbfopt/doc/rbfopt_user_black_box.rst
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)      127 2017-09-04 22:11:30.000000 rbfopt-4.2.6/src/rbfopt/doc/rbfopt_utils.rst
+drwxr-xr-x   0 nannicini  (1000) nannicini  (1000)        0 2023-06-14 17:57:45.580514 rbfopt-4.2.6/src/rbfopt/examples/
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)     6024 2022-11-17 01:27:23.000000 rbfopt-4.2.6/src/rbfopt/examples/rbfopt_black_box_example.py
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)   133694 2022-11-18 20:08:49.000000 rbfopt-4.2.6/src/rbfopt/rbfopt_algorithm.py
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)    61159 2022-11-17 01:27:23.000000 rbfopt-4.2.6/src/rbfopt/rbfopt_aux_problems.py
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)     4352 2022-11-17 01:27:23.000000 rbfopt-4.2.6/src/rbfopt/rbfopt_black_box.py
+-rw-rw-r--   0 nannicini  (1000) nannicini  (1000)    39709 2020-06-26 22:34:46.000000 rbfopt-4.2.6/src/rbfopt/rbfopt_degree0_models.py
+-rw-rw-r--   0 nannicini  (1000) nannicini  (1000)    42746 2020-06-26 22:34:46.000000 rbfopt-4.2.6/src/rbfopt/rbfopt_degree1_models.py
+-rw-rw-r--   0 nannicini  (1000) nannicini  (1000)    33837 2020-06-26 22:34:46.000000 rbfopt-4.2.6/src/rbfopt/rbfopt_degreem1_models.py
+-rw-rw-r--   0 nannicini  (1000) nannicini  (1000)    18570 2020-06-26 22:34:46.000000 rbfopt-4.2.6/src/rbfopt/rbfopt_refinement.py
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)    29030 2022-11-18 04:44:20.000000 rbfopt-4.2.6/src/rbfopt/rbfopt_settings.py
+-rw-rw-r--   0 nannicini  (1000) nannicini  (1000)   116828 2022-11-15 04:56:38.000000 rbfopt-4.2.6/src/rbfopt/rbfopt_test_functions.py
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)     6690 2022-11-17 01:27:23.000000 rbfopt-4.2.6/src/rbfopt/rbfopt_user_black_box.py
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)    76345 2022-11-18 02:27:20.000000 rbfopt-4.2.6/src/rbfopt/rbfopt_utils.py
+drwxr-xr-x   0 nannicini  (1000) nannicini  (1000)        0 2023-06-14 17:57:45.578514 rbfopt-4.2.6/src/rbfopt.egg-info/
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)    15547 2023-06-14 17:57:45.000000 rbfopt-4.2.6/src/rbfopt.egg-info/PKG-INFO
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)     1710 2023-06-14 17:57:45.000000 rbfopt-4.2.6/src/rbfopt.egg-info/SOURCES.txt
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)        1 2023-06-14 17:57:45.000000 rbfopt-4.2.6/src/rbfopt.egg-info/dependency_links.txt
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)        1 2017-08-22 13:23:44.000000 rbfopt-4.2.6/src/rbfopt.egg-info/not-zip-safe
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)       18 2023-06-14 17:57:45.000000 rbfopt-4.2.6/src/rbfopt.egg-info/requires.txt
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)        7 2023-06-14 17:57:45.000000 rbfopt-4.2.6/src/rbfopt.egg-info/top_level.txt
+drwxr-xr-x   0 nannicini  (1000) nannicini  (1000)        0 2023-06-14 17:57:45.584514 rbfopt-4.2.6/tests/
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)        0 2017-09-04 22:11:30.000000 rbfopt-4.2.6/tests/__init__.py
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)      109 2017-09-04 22:11:30.000000 rbfopt-4.2.6/tests/context.py
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)    29576 2022-11-18 20:09:19.000000 rbfopt-4.2.6/tests/slow_test_rbfopt_algorithm.py
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)    22288 2022-11-20 01:50:02.000000 rbfopt-4.2.6/tests/test_rbfopt_algorithm.py
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)    24590 2022-11-17 01:27:23.000000 rbfopt-4.2.6/tests/test_rbfopt_aux_problems.py
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)    12439 2022-11-17 01:27:23.000000 rbfopt-4.2.6/tests/test_rbfopt_degree0_models.py
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)    13223 2022-11-17 01:27:23.000000 rbfopt-4.2.6/tests/test_rbfopt_degree1_models.py
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)     6575 2022-11-17 01:27:23.000000 rbfopt-4.2.6/tests/test_rbfopt_degreem1_models.py
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)     1786 2022-11-17 01:27:23.000000 rbfopt-4.2.6/tests/test_rbfopt_mwe.py
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)     9732 2022-11-17 01:27:23.000000 rbfopt-4.2.6/tests/test_rbfopt_refinement.py
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)     4836 2022-11-18 01:30:07.000000 rbfopt-4.2.6/tests/test_rbfopt_settings.py
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)     3196 2022-11-17 01:27:23.000000 rbfopt-4.2.6/tests/test_rbfopt_test_functions.py
+-rw-r--r--   0 nannicini  (1000) nannicini  (1000)    38393 2022-11-18 02:28:47.000000 rbfopt-4.2.6/tests/test_rbfopt_utils.py
```

### Comparing `rbfopt-4.2.5/CHANGELOG` & `rbfopt-4.2.6/CHANGELOG`

 * *Files identical despite different names*

### Comparing `rbfopt-4.2.5/LICENSE` & `rbfopt-4.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rbfopt-4.2.5/PKG-INFO` & `rbfopt-4.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: rbfopt
-Version: 4.2.5
+Version: 4.2.6
 Summary: Library for black-box (derivative-free) optimization
 Home-page: https://github.com/coin-or/rbfopt
 Author: Giacomo Nannicini
 Author-email: nannicini@us.ibm.com
 License: Revised BSD
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 License-File: LICENSE
 License-File: AUTHORS
@@ -398,9 +397,7 @@
 =======
 Support
 =======
 
 If you believe there is a bug or an issue, please open an issue on
 GitHub.  If you have a general question, please use GitHub's
 "Discussions" feature (the tab can be opened at the top of the page).
-
-
```

### Comparing `rbfopt-4.2.5/README.rst` & `rbfopt-4.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `rbfopt-4.2.5/bin/rbfopt_cl_interface.py` & `rbfopt-4.2.6/bin/rbfopt_cl_interface.py`

 * *Files identical despite different names*

### Comparing `rbfopt-4.2.5/bin/rbfopt_test_interface.py` & `rbfopt-4.2.6/bin/rbfopt_test_interface.py`

 * *Files identical despite different names*

### Comparing `rbfopt-4.2.5/manual.pdf` & `rbfopt-4.2.6/manual.pdf`

 * *Files identical despite different names*

### Comparing `rbfopt-4.2.5/setup.py` & `rbfopt-4.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `rbfopt-4.2.5/src/rbfopt/__init__.py` & `rbfopt-4.2.6/src/rbfopt/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # there might be issues when running several processes in parallel.
 os.environ['OMP_NUM_THREADS'] = '1'
 from .rbfopt_settings import RbfoptSettings
 from .rbfopt_algorithm import RbfoptAlgorithm
 from .rbfopt_black_box import RbfoptBlackBox
 from .rbfopt_user_black_box import RbfoptUserBlackBox
 
-__version__ = '4.2.5'
+__version__ = '4.2.6'
 
 __all__ = ['rbfopt_algorithm',
            'rbfopt_aux_problems',
            'rbfopt_black_box_example',
            'rbfopt_black_box',
            'rbfopt_degree0_models',
            'rbfopt_degree1_models',
```

### Comparing `rbfopt-4.2.5/src/rbfopt/doc/Makefile` & `rbfopt-4.2.6/src/rbfopt/doc/Makefile`

 * *Files identical despite different names*

### Comparing `rbfopt-4.2.5/src/rbfopt/doc/conf.py` & `rbfopt-4.2.6/src/rbfopt/doc/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 sys.path.insert(0, os.path.abspath('../..'))
 sys.path.insert(1, os.path.abspath('..'))
 
 # -- Mock modules for autodoc
 
 MOCK_MODULES = ['argparse', 'numpy', 'scipy', 'scipy.spatial', 
                 'scipy.linalg', 'scipy.special', 'pyomo.opt',
-                'pyomo.environ']
+                'pyomo.environ', 'pyomo']
 sys.modules.update((mod_name, Mock()) for mod_name in MOCK_MODULES)
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #needs_sphinx = '1.0'
```

### Comparing `rbfopt-4.2.5/src/rbfopt/doc/index.rst` & `rbfopt-4.2.6/src/rbfopt/doc/index.rst`

 * *Files identical despite different names*

### Comparing `rbfopt-4.2.5/src/rbfopt/doc/make.bat` & `rbfopt-4.2.6/src/rbfopt/doc/make.bat`

 * *Files identical despite different names*

### Comparing `rbfopt-4.2.5/src/rbfopt/examples/rbfopt_black_box_example.py` & `rbfopt-4.2.6/src/rbfopt/examples/rbfopt_black_box_example.py`

 * *Files identical despite different names*

### Comparing `rbfopt-4.2.5/src/rbfopt/rbfopt_algorithm.py` & `rbfopt-4.2.6/src/rbfopt/rbfopt_algorithm.py`

 * *Files identical despite different names*

### Comparing `rbfopt-4.2.5/src/rbfopt/rbfopt_aux_problems.py` & `rbfopt-4.2.6/src/rbfopt/rbfopt_aux_problems.py`

 * *Files identical despite different names*

### Comparing `rbfopt-4.2.5/src/rbfopt/rbfopt_black_box.py` & `rbfopt-4.2.6/src/rbfopt/rbfopt_black_box.py`

 * *Files identical despite different names*

### Comparing `rbfopt-4.2.5/src/rbfopt/rbfopt_degree0_models.py` & `rbfopt-4.2.6/src/rbfopt/rbfopt_degree0_models.py`

 * *Files identical despite different names*

### Comparing `rbfopt-4.2.5/src/rbfopt/rbfopt_degree1_models.py` & `rbfopt-4.2.6/src/rbfopt/rbfopt_degree1_models.py`

 * *Files identical despite different names*

### Comparing `rbfopt-4.2.5/src/rbfopt/rbfopt_degreem1_models.py` & `rbfopt-4.2.6/src/rbfopt/rbfopt_degreem1_models.py`

 * *Files identical despite different names*

### Comparing `rbfopt-4.2.5/src/rbfopt/rbfopt_refinement.py` & `rbfopt-4.2.6/src/rbfopt/rbfopt_refinement.py`

 * *Files identical despite different names*

### Comparing `rbfopt-4.2.5/src/rbfopt/rbfopt_settings.py` & `rbfopt-4.2.6/src/rbfopt/rbfopt_settings.py`

 * *Files identical despite different names*

### Comparing `rbfopt-4.2.5/src/rbfopt/rbfopt_test_functions.py` & `rbfopt-4.2.6/src/rbfopt/rbfopt_test_functions.py`

 * *Files identical despite different names*

### Comparing `rbfopt-4.2.5/src/rbfopt/rbfopt_user_black_box.py` & `rbfopt-4.2.6/src/rbfopt/rbfopt_user_black_box.py`

 * *Files identical despite different names*

### Comparing `rbfopt-4.2.5/src/rbfopt/rbfopt_utils.py` & `rbfopt-4.2.6/src/rbfopt/rbfopt_utils.py`

 * *Files identical despite different names*

### Comparing `rbfopt-4.2.5/src/rbfopt.egg-info/PKG-INFO` & `rbfopt-4.2.6/src/rbfopt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: rbfopt
-Version: 4.2.5
+Version: 4.2.6
 Summary: Library for black-box (derivative-free) optimization
 Home-page: https://github.com/coin-or/rbfopt
 Author: Giacomo Nannicini
 Author-email: nannicini@us.ibm.com
 License: Revised BSD
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 License-File: LICENSE
 License-File: AUTHORS
@@ -398,9 +397,7 @@
 =======
 Support
 =======
 
 If you believe there is a bug or an issue, please open an issue on
 GitHub.  If you have a general question, please use GitHub's
 "Discussions" feature (the tab can be opened at the top of the page).
-
-
```

### Comparing `rbfopt-4.2.5/src/rbfopt.egg-info/SOURCES.txt` & `rbfopt-4.2.6/src/rbfopt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rbfopt-4.2.5/tests/slow_test_rbfopt_algorithm.py` & `rbfopt-4.2.6/tests/slow_test_rbfopt_algorithm.py`

 * *Files identical despite different names*

### Comparing `rbfopt-4.2.5/tests/test_rbfopt_algorithm.py` & `rbfopt-4.2.6/tests/test_rbfopt_algorithm.py`

 * *Files identical despite different names*

### Comparing `rbfopt-4.2.5/tests/test_rbfopt_aux_problems.py` & `rbfopt-4.2.6/tests/test_rbfopt_aux_problems.py`

 * *Files identical despite different names*

### Comparing `rbfopt-4.2.5/tests/test_rbfopt_degree0_models.py` & `rbfopt-4.2.6/tests/test_rbfopt_degree0_models.py`

 * *Files identical despite different names*

### Comparing `rbfopt-4.2.5/tests/test_rbfopt_degree1_models.py` & `rbfopt-4.2.6/tests/test_rbfopt_degree1_models.py`

 * *Files identical despite different names*

### Comparing `rbfopt-4.2.5/tests/test_rbfopt_degreem1_models.py` & `rbfopt-4.2.6/tests/test_rbfopt_degreem1_models.py`

 * *Files identical despite different names*

### Comparing `rbfopt-4.2.5/tests/test_rbfopt_mwe.py` & `rbfopt-4.2.6/tests/test_rbfopt_mwe.py`

 * *Files identical despite different names*

### Comparing `rbfopt-4.2.5/tests/test_rbfopt_refinement.py` & `rbfopt-4.2.6/tests/test_rbfopt_refinement.py`

 * *Files identical despite different names*

### Comparing `rbfopt-4.2.5/tests/test_rbfopt_settings.py` & `rbfopt-4.2.6/tests/test_rbfopt_settings.py`

 * *Files identical despite different names*

### Comparing `rbfopt-4.2.5/tests/test_rbfopt_test_functions.py` & `rbfopt-4.2.6/tests/test_rbfopt_test_functions.py`

 * *Files identical despite different names*

### Comparing `rbfopt-4.2.5/tests/test_rbfopt_utils.py` & `rbfopt-4.2.6/tests/test_rbfopt_utils.py`

 * *Files identical despite different names*

