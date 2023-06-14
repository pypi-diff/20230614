# Comparing `tmp/ase-cogef-23.2.1.tar.gz` & `tmp/ase-cogef-23.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ase-cogef-23.2.1.tar", last modified: Thu Feb  9 13:27:17 2023, max compression
+gzip compressed data, was "ase-cogef-23.6.1.tar", last modified: Wed Jun 14 14:24:54 2023, max compression
```

## Comparing `ase-cogef-23.2.1.tar` & `ase-cogef-23.6.1.tar`

### file list

```diff
@@ -1,76 +1,81 @@
-drwxrwxr-x   0 mw        (1000) mw        (1000)        0 2023-02-09 13:27:17.026764 ase-cogef-23.2.1/
--rw-rw-r--   0 mw        (1000) mw        (1000)    18092 2021-02-08 17:21:22.000000 ase-cogef-23.2.1/COPYING
--rw-rw-r--   0 mw        (1000) mw        (1000)    26530 2021-02-08 17:21:22.000000 ase-cogef-23.2.1/COPYING.LESSER
--rw-rw-r--   0 mw        (1000) mw        (1000)      614 2021-02-08 17:21:22.000000 ase-cogef-23.2.1/LICENSE
--rw-rw-r--   0 mw        (1000) mw        (1000)       74 2021-02-08 17:21:22.000000 ase-cogef-23.2.1/MANIFEST.in
--rw-rw-r--   0 mw        (1000) mw        (1000)     2648 2023-02-09 13:27:17.026764 ase-cogef-23.2.1/PKG-INFO
--rw-rw-r--   0 mw        (1000) mw        (1000)     1973 2023-01-26 10:31:57.000000 ase-cogef-23.2.1/README.rst
-drwxrwxr-x   0 mw        (1000) mw        (1000)        0 2023-02-09 13:27:17.022763 ase-cogef-23.2.1/ase_cogef.egg-info/
--rw-rw-r--   0 mw        (1000) mw        (1000)     2648 2023-02-09 13:27:17.000000 ase-cogef-23.2.1/ase_cogef.egg-info/PKG-INFO
--rw-rw-r--   0 mw        (1000) mw        (1000)     1671 2023-02-09 13:27:17.000000 ase-cogef-23.2.1/ase_cogef.egg-info/SOURCES.txt
--rw-rw-r--   0 mw        (1000) mw        (1000)        1 2023-02-09 13:27:17.000000 ase-cogef-23.2.1/ase_cogef.egg-info/dependency_links.txt
--rw-rw-r--   0 mw        (1000) mw        (1000)       46 2023-02-09 13:27:17.000000 ase-cogef-23.2.1/ase_cogef.egg-info/entry_points.txt
--rw-rw-r--   0 mw        (1000) mw        (1000)       53 2023-02-09 13:27:17.000000 ase-cogef-23.2.1/ase_cogef.egg-info/requires.txt
--rw-rw-r--   0 mw        (1000) mw        (1000)        6 2023-02-09 13:27:17.000000 ase-cogef-23.2.1/ase_cogef.egg-info/top_level.txt
-drwxrwxr-x   0 mw        (1000) mw        (1000)        0 2023-02-09 13:27:17.022763 ase-cogef-23.2.1/bin/
--rwxrwxr-x   0 mw        (1000) mw        (1000)       62 2021-02-08 17:21:22.000000 ase-cogef-23.2.1/bin/cogef
-drwxrwxr-x   0 mw        (1000) mw        (1000)        0 2023-02-09 13:27:17.022763 ase-cogef-23.2.1/cogef/
--rw-rw-r--   0 mw        (1000) mw        (1000)     1553 2023-02-09 13:26:21.000000 ase-cogef-23.2.1/cogef/__init__.py
-drwxrwxr-x   0 mw        (1000) mw        (1000)        0 2023-02-09 13:27:17.022763 ase-cogef-23.2.1/cogef/cli/
--rw-rw-r--   0 mw        (1000) mw        (1000)        0 2021-02-08 17:21:22.000000 ase-cogef-23.2.1/cogef/cli/__init__.py
--rw-rw-r--   0 mw        (1000) mw        (1000)     1727 2021-02-08 17:21:22.000000 ase-cogef-23.2.1/cogef/cli/main.py
--rw-rw-r--   0 mw        (1000) mw        (1000)    29946 2023-02-09 13:22:16.000000 ase-cogef-23.2.1/cogef/cogef1d.py
-drwxrwxr-x   0 mw        (1000) mw        (1000)        0 2023-02-09 13:27:17.022763 ase-cogef-23.2.1/cogef/cogef2d/
--rw-rw-r--   0 mw        (1000) mw        (1000)      252 2023-02-09 13:22:16.000000 ase-cogef-23.2.1/cogef/cogef2d/__init__.py
--rw-rw-r--   0 mw        (1000) mw        (1000)    29150 2023-02-09 13:22:16.000000 ase-cogef-23.2.1/cogef/cogef2d/cogef2d.py
--rw-rw-r--   0 mw        (1000) mw        (1000)    27966 2023-02-09 13:22:16.000000 ase-cogef-23.2.1/cogef/cogef2d/cogef2in1.py
--rw-rw-r--   0 mw        (1000) mw        (1000)    57166 2023-02-09 13:22:16.000000 ase-cogef-23.2.1/cogef/cogef2d/dissociation2d.py
--rw-rw-r--   0 mw        (1000) mw        (1000)     8000 2023-02-09 13:22:16.000000 ase-cogef-23.2.1/cogef/cogef2d/fixed2d.py
--rw-rw-r--   0 mw        (1000) mw        (1000)     5051 2023-02-09 13:22:16.000000 ase-cogef-23.2.1/cogef/cogef2d/neb.py
--rw-rw-r--   0 mw        (1000) mw        (1000)    22066 2023-01-26 10:31:57.000000 ase-cogef-23.2.1/cogef/dcogef.py
-drwxrwxr-x   0 mw        (1000) mw        (1000)        0 2023-02-09 13:27:17.022763 ase-cogef-23.2.1/cogef/dissociation/
--rw-rw-r--   0 mw        (1000) mw        (1000)      115 2023-02-09 13:22:16.000000 ase-cogef-23.2.1/cogef/dissociation/__init__.py
--rw-rw-r--   0 mw        (1000) mw        (1000)    18471 2023-02-09 13:22:16.000000 ase-cogef-23.2.1/cogef/dissociation/barrier.py
--rw-rw-r--   0 mw        (1000) mw        (1000)    38535 2023-02-09 13:22:16.000000 ase-cogef-23.2.1/cogef/dissociation/diss_old.py
--rw-rw-r--   0 mw        (1000) mw        (1000)    30158 2023-02-09 13:22:16.000000 ase-cogef-23.2.1/cogef/dissociation/dissociation.py
--rw-rw-r--   0 mw        (1000) mw        (1000)      947 2023-02-09 13:22:16.000000 ase-cogef-23.2.1/cogef/dissociation/tabulated_barrier.py
--rw-rw-r--   0 mw        (1000) mw        (1000)     7156 2023-02-09 13:22:16.000000 ase-cogef-23.2.1/cogef/generalized.py
--rw-rw-r--   0 mw        (1000) mw        (1000)     5061 2023-02-09 13:22:16.000000 ase-cogef-23.2.1/cogef/minmax.py
--rw-rw-r--   0 mw        (1000) mw        (1000)     6535 2023-02-09 13:22:16.000000 ase-cogef-23.2.1/cogef/mpf.py
--rw-rw-r--   0 mw        (1000) mw        (1000)     1494 2023-02-09 13:22:16.000000 ase-cogef-23.2.1/cogef/potentials.py
--rw-rw-r--   0 mw        (1000) mw        (1000)    39550 2021-02-08 17:21:22.000000 ase-cogef-23.2.1/cogef/probability.py
--rw-rw-r--   0 mw        (1000) mw        (1000)     1148 2023-02-09 13:22:16.000000 ase-cogef-23.2.1/cogef/spring_constant.py
-drwxrwxr-x   0 mw        (1000) mw        (1000)        0 2023-02-09 13:27:17.026764 ase-cogef-23.2.1/cogef/test/
--rw-rw-r--   0 mw        (1000) mw        (1000)        0 2021-02-08 17:21:22.000000 ase-cogef-23.2.1/cogef/test/__init__.py
--rw-rw-r--   0 mw        (1000) mw        (1000)     1820 2023-01-26 10:31:57.000000 ase-cogef-23.2.1/cogef/test/au6harmonic.py
--rw-rw-r--   0 mw        (1000) mw        (1000)     1224 2023-02-09 13:22:16.000000 ase-cogef-23.2.1/cogef/test/conftest.py
-drwxrwxr-x   0 mw        (1000) mw        (1000)        0 2023-02-09 13:27:17.026764 ase-cogef-23.2.1/cogef/test/dissociate/
--rw-rw-r--   0 mw        (1000) mw        (1000)        0 2023-02-09 13:22:16.000000 ase-cogef-23.2.1/cogef/test/dissociate/__init__.py
--rw-rw-r--   0 mw        (1000) mw        (1000)     6006 2023-02-09 13:22:16.000000 ase-cogef-23.2.1/cogef/test/dissociate/test_barrier_unit.py
--rw-rw-r--   0 mw        (1000) mw        (1000)     4476 2023-02-09 13:22:16.000000 ase-cogef-23.2.1/cogef/test/dissociate/test_dissociate_integration.py
--rw-rw-r--   0 mw        (1000) mw        (1000)     1593 2023-02-09 13:22:16.000000 ase-cogef-23.2.1/cogef/test/dissociate/test_tabulated_barrier.py
--rw-rw-r--   0 mw        (1000) mw        (1000)     8610 2021-02-08 17:21:22.000000 ase-cogef-23.2.1/cogef/test/rate_0_1.dat
--rw-rw-r--   0 mw        (1000) mw        (1000)     8471 2021-02-08 17:21:22.000000 ase-cogef-23.2.1/cogef/test/rate_0_8.dat
--rw-rw-r--   0 mw        (1000) mw        (1000)     8547 2021-02-08 17:21:22.000000 ase-cogef-23.2.1/cogef/test/rate_1_2.dat
--rw-rw-r--   0 mw        (1000) mw        (1000)    48156 2021-02-08 17:21:22.000000 ase-cogef-23.2.1/cogef/test/rate_29_11.dat
--rw-rw-r--   0 mw        (1000) mw        (1000)    45834 2021-02-08 17:21:22.000000 ase-cogef-23.2.1/cogef/test/rate_8_12.dat
--rw-rw-r--   0 mw        (1000) mw        (1000)     2297 2021-02-08 17:21:22.000000 ase-cogef-23.2.1/cogef/test/rate_CTC-CCC.dat
--rw-rw-r--   0 mw        (1000) mw        (1000)     2279 2021-02-08 17:21:22.000000 ase-cogef-23.2.1/cogef/test/rate_CTC-TTC.dat
--rw-rw-r--   0 mw        (1000) mw        (1000)     2347 2021-02-08 17:21:22.000000 ase-cogef-23.2.1/cogef/test/rate_INTER-CTC.dat
--rw-rw-r--   0 mw        (1000) mw        (1000)     2435 2021-02-08 17:21:22.000000 ase-cogef-23.2.1/cogef/test/rate_INTER-TTC.dat
--rw-rw-r--   0 mw        (1000) mw        (1000)     2192 2021-02-08 17:21:22.000000 ase-cogef-23.2.1/cogef/test/rate_SP-INTER.dat
--rw-rw-r--   0 mw        (1000) mw        (1000)     1411 2023-02-09 13:22:16.000000 ase-cogef-23.2.1/cogef/test/test_MPF.py
--rw-rw-r--   0 mw        (1000) mw        (1000)     6433 2023-02-09 13:22:16.000000 ase-cogef-23.2.1/cogef/test/test_cogef1d.py
--rw-rw-r--   0 mw        (1000) mw        (1000)     3301 2023-02-09 13:22:16.000000 ase-cogef-23.2.1/cogef/test/test_cogef1d_generalized.py
--rw-rw-r--   0 mw        (1000) mw        (1000)      520 2023-02-09 13:22:16.000000 ase-cogef-23.2.1/cogef/test/test_concerted.py
--rw-rw-r--   0 mw        (1000) mw        (1000)      711 2023-02-09 13:22:16.000000 ase-cogef-23.2.1/cogef/test/test_hocut.py
--rw-rw-r--   0 mw        (1000) mw        (1000)     3480 2023-01-26 10:31:57.000000 ase-cogef-23.2.1/cogef/test/test_minmax.py
--rw-rw-r--   0 mw        (1000) mw        (1000)     5069 2023-01-26 10:31:57.000000 ase-cogef-23.2.1/cogef/test/test_probability.py
--rw-rw-r--   0 mw        (1000) mw        (1000)     1246 2023-02-09 13:22:16.000000 ase-cogef-23.2.1/cogef/test/test_spring_constant.py
--rw-rw-r--   0 mw        (1000) mw        (1000)     1168 2023-02-09 13:22:16.000000 ase-cogef-23.2.1/cogef/test/test_spring_vibrations.py
--rw-rw-r--   0 mw        (1000) mw        (1000)      192 2023-01-26 10:31:57.000000 ase-cogef-23.2.1/cogef/test/test_units.py
--rw-rw-r--   0 mw        (1000) mw        (1000)      105 2023-01-26 10:31:57.000000 ase-cogef-23.2.1/cogef/units.py
--rw-rw-r--   0 mw        (1000) mw        (1000)      534 2023-01-26 10:31:57.000000 ase-cogef-23.2.1/cogef/utilities.py
--rw-rw-r--   0 mw        (1000) mw        (1000)     9754 2023-01-26 10:31:57.000000 ase-cogef-23.2.1/cogef/vibrations.py
--rw-rw-r--   0 mw        (1000) mw        (1000)       38 2023-02-09 13:27:17.026764 ase-cogef-23.2.1/setup.cfg
--rw-rw-r--   0 mw        (1000) mw        (1000)     1606 2023-01-26 10:31:57.000000 ase-cogef-23.2.1/setup.py
+drwxrwxr-x   0 mw        (1000) mw        (1000)        0 2023-06-14 14:24:54.120657 ase-cogef-23.6.1/
+-rw-rw-r--   0 mw        (1000) mw        (1000)    18092 2021-02-08 17:21:22.000000 ase-cogef-23.6.1/COPYING
+-rw-rw-r--   0 mw        (1000) mw        (1000)    26530 2021-02-08 17:21:22.000000 ase-cogef-23.6.1/COPYING.LESSER
+-rw-rw-r--   0 mw        (1000) mw        (1000)      614 2021-02-08 17:21:22.000000 ase-cogef-23.6.1/LICENSE
+-rw-rw-r--   0 mw        (1000) mw        (1000)       74 2021-02-08 17:21:22.000000 ase-cogef-23.6.1/MANIFEST.in
+-rw-rw-r--   0 mw        (1000) mw        (1000)     2648 2023-06-14 14:24:54.120657 ase-cogef-23.6.1/PKG-INFO
+-rw-rw-r--   0 mw        (1000) mw        (1000)     1973 2023-01-26 10:31:57.000000 ase-cogef-23.6.1/README.rst
+drwxrwxr-x   0 mw        (1000) mw        (1000)        0 2023-06-14 14:24:54.116657 ase-cogef-23.6.1/ase_cogef.egg-info/
+-rw-rw-r--   0 mw        (1000) mw        (1000)     2648 2023-06-14 14:24:54.000000 ase-cogef-23.6.1/ase_cogef.egg-info/PKG-INFO
+-rw-rw-r--   0 mw        (1000) mw        (1000)     1776 2023-06-14 14:24:54.000000 ase-cogef-23.6.1/ase_cogef.egg-info/SOURCES.txt
+-rw-rw-r--   0 mw        (1000) mw        (1000)        1 2023-06-14 14:24:54.000000 ase-cogef-23.6.1/ase_cogef.egg-info/dependency_links.txt
+-rw-rw-r--   0 mw        (1000) mw        (1000)       46 2023-06-14 14:24:54.000000 ase-cogef-23.6.1/ase_cogef.egg-info/entry_points.txt
+-rw-rw-r--   0 mw        (1000) mw        (1000)       53 2023-06-14 14:24:54.000000 ase-cogef-23.6.1/ase_cogef.egg-info/requires.txt
+-rw-rw-r--   0 mw        (1000) mw        (1000)        6 2023-06-14 14:24:54.000000 ase-cogef-23.6.1/ase_cogef.egg-info/top_level.txt
+drwxrwxr-x   0 mw        (1000) mw        (1000)        0 2023-06-14 14:24:54.116657 ase-cogef-23.6.1/bin/
+-rwxrwxr-x   0 mw        (1000) mw        (1000)       62 2021-02-08 17:21:22.000000 ase-cogef-23.6.1/bin/cogef
+drwxrwxr-x   0 mw        (1000) mw        (1000)        0 2023-06-14 14:24:54.116657 ase-cogef-23.6.1/cogef/
+-rw-rw-r--   0 mw        (1000) mw        (1000)     1553 2023-06-14 14:24:09.000000 ase-cogef-23.6.1/cogef/__init__.py
+drwxrwxr-x   0 mw        (1000) mw        (1000)        0 2023-06-14 14:24:54.116657 ase-cogef-23.6.1/cogef/cli/
+-rw-rw-r--   0 mw        (1000) mw        (1000)        0 2021-02-08 17:21:22.000000 ase-cogef-23.6.1/cogef/cli/__init__.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)     1727 2021-02-08 17:21:22.000000 ase-cogef-23.6.1/cogef/cli/main.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)    29475 2023-06-14 10:51:50.000000 ase-cogef-23.6.1/cogef/cogef1d.py
+drwxrwxr-x   0 mw        (1000) mw        (1000)        0 2023-06-14 14:24:54.116657 ase-cogef-23.6.1/cogef/cogef2d/
+-rw-rw-r--   0 mw        (1000) mw        (1000)      252 2023-02-09 13:22:16.000000 ase-cogef-23.6.1/cogef/cogef2d/__init__.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)    29150 2023-03-30 11:21:17.000000 ase-cogef-23.6.1/cogef/cogef2d/cogef2d.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)    27966 2023-06-14 10:40:19.000000 ase-cogef-23.6.1/cogef/cogef2d/cogef2in1.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)    57166 2023-06-14 10:40:19.000000 ase-cogef-23.6.1/cogef/cogef2d/dissociation2d.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)     8000 2023-06-14 10:40:19.000000 ase-cogef-23.6.1/cogef/cogef2d/fixed2d.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)     5000 2023-06-14 10:40:19.000000 ase-cogef-23.6.1/cogef/cogef2d/neb.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)    20280 2023-06-14 10:51:50.000000 ase-cogef-23.6.1/cogef/dcogef.py
+drwxrwxr-x   0 mw        (1000) mw        (1000)        0 2023-06-14 14:24:54.120657 ase-cogef-23.6.1/cogef/dissociation/
+-rw-rw-r--   0 mw        (1000) mw        (1000)      115 2023-03-30 11:21:17.000000 ase-cogef-23.6.1/cogef/dissociation/__init__.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)    18471 2023-06-14 10:40:19.000000 ase-cogef-23.6.1/cogef/dissociation/barrier.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)    38535 2023-06-14 10:40:19.000000 ase-cogef-23.6.1/cogef/dissociation/diss_old.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)    30158 2023-06-14 10:40:19.000000 ase-cogef-23.6.1/cogef/dissociation/dissociation.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)      947 2023-06-14 10:40:19.000000 ase-cogef-23.6.1/cogef/dissociation/tabulated_barrier.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)     2090 2023-06-14 10:40:19.000000 ase-cogef-23.6.1/cogef/efei.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)     8262 2023-06-14 10:40:19.000000 ase-cogef-23.6.1/cogef/generalized.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)     5061 2023-03-30 11:21:17.000000 ase-cogef-23.6.1/cogef/minmax.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)     6535 2023-03-30 11:21:17.000000 ase-cogef-23.6.1/cogef/mpf.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)     1156 2023-06-14 10:40:19.000000 ase-cogef-23.6.1/cogef/neb.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)     1494 2023-02-09 13:22:16.000000 ase-cogef-23.6.1/cogef/potentials.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)    39550 2021-02-08 17:21:22.000000 ase-cogef-23.6.1/cogef/probability.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)     1148 2023-02-09 13:22:16.000000 ase-cogef-23.6.1/cogef/spring_constant.py
+drwxrwxr-x   0 mw        (1000) mw        (1000)        0 2023-06-14 14:24:54.120657 ase-cogef-23.6.1/cogef/test/
+-rw-rw-r--   0 mw        (1000) mw        (1000)        0 2021-02-08 17:21:22.000000 ase-cogef-23.6.1/cogef/test/__init__.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)     1820 2023-01-26 10:31:57.000000 ase-cogef-23.6.1/cogef/test/au6harmonic.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)     1498 2023-06-14 10:40:19.000000 ase-cogef-23.6.1/cogef/test/conftest.py
+drwxrwxr-x   0 mw        (1000) mw        (1000)        0 2023-06-14 14:24:54.120657 ase-cogef-23.6.1/cogef/test/dissociate/
+-rw-rw-r--   0 mw        (1000) mw        (1000)        0 2023-03-30 11:21:17.000000 ase-cogef-23.6.1/cogef/test/dissociate/__init__.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)     6006 2023-06-14 10:40:19.000000 ase-cogef-23.6.1/cogef/test/dissociate/test_barrier_unit.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)     4476 2023-06-14 10:40:19.000000 ase-cogef-23.6.1/cogef/test/dissociate/test_dissociate_integration.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)     1659 2023-06-14 10:40:19.000000 ase-cogef-23.6.1/cogef/test/dissociate/test_tabulated_barrier.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)     8610 2021-02-08 17:21:22.000000 ase-cogef-23.6.1/cogef/test/rate_0_1.dat
+-rw-rw-r--   0 mw        (1000) mw        (1000)     8471 2021-02-08 17:21:22.000000 ase-cogef-23.6.1/cogef/test/rate_0_8.dat
+-rw-rw-r--   0 mw        (1000) mw        (1000)     8547 2021-02-08 17:21:22.000000 ase-cogef-23.6.1/cogef/test/rate_1_2.dat
+-rw-rw-r--   0 mw        (1000) mw        (1000)    48156 2021-02-08 17:21:22.000000 ase-cogef-23.6.1/cogef/test/rate_29_11.dat
+-rw-rw-r--   0 mw        (1000) mw        (1000)    45834 2021-02-08 17:21:22.000000 ase-cogef-23.6.1/cogef/test/rate_8_12.dat
+-rw-rw-r--   0 mw        (1000) mw        (1000)     2297 2021-02-08 17:21:22.000000 ase-cogef-23.6.1/cogef/test/rate_CTC-CCC.dat
+-rw-rw-r--   0 mw        (1000) mw        (1000)     2279 2021-02-08 17:21:22.000000 ase-cogef-23.6.1/cogef/test/rate_CTC-TTC.dat
+-rw-rw-r--   0 mw        (1000) mw        (1000)     2347 2021-02-08 17:21:22.000000 ase-cogef-23.6.1/cogef/test/rate_INTER-CTC.dat
+-rw-rw-r--   0 mw        (1000) mw        (1000)     2435 2021-02-08 17:21:22.000000 ase-cogef-23.6.1/cogef/test/rate_INTER-TTC.dat
+-rw-rw-r--   0 mw        (1000) mw        (1000)     2192 2021-02-08 17:21:22.000000 ase-cogef-23.6.1/cogef/test/rate_SP-INTER.dat
+-rw-rw-r--   0 mw        (1000) mw        (1000)     1411 2023-03-30 11:21:17.000000 ase-cogef-23.6.1/cogef/test/test_MPF.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)     6433 2023-06-14 10:40:19.000000 ase-cogef-23.6.1/cogef/test/test_cogef1d.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)     2939 2023-06-14 10:40:19.000000 ase-cogef-23.6.1/cogef/test/test_cogef1d_generalized.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)      938 2023-06-14 10:40:19.000000 ase-cogef-23.6.1/cogef/test/test_concerted.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)     1615 2023-06-14 10:51:50.000000 ase-cogef-23.6.1/cogef/test/test_dcogef.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)      665 2023-06-14 10:40:19.000000 ase-cogef-23.6.1/cogef/test/test_efei_pair.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)      711 2023-02-09 13:22:16.000000 ase-cogef-23.6.1/cogef/test/test_hocut.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)     3480 2023-01-26 10:31:57.000000 ase-cogef-23.6.1/cogef/test/test_minmax.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)     1080 2023-06-14 10:40:19.000000 ase-cogef-23.6.1/cogef/test/test_neb.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)     5153 2023-06-14 10:40:19.000000 ase-cogef-23.6.1/cogef/test/test_probability.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)     1246 2023-02-09 13:22:16.000000 ase-cogef-23.6.1/cogef/test/test_spring_constant.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)     1168 2023-02-09 13:22:16.000000 ase-cogef-23.6.1/cogef/test/test_spring_vibrations.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)      192 2023-01-26 10:31:57.000000 ase-cogef-23.6.1/cogef/test/test_units.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)      105 2023-01-26 10:31:57.000000 ase-cogef-23.6.1/cogef/units.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)      534 2023-01-26 10:31:57.000000 ase-cogef-23.6.1/cogef/utilities.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)     9754 2023-01-26 10:31:57.000000 ase-cogef-23.6.1/cogef/vibrations.py
+-rw-rw-r--   0 mw        (1000) mw        (1000)       38 2023-06-14 14:24:54.120657 ase-cogef-23.6.1/setup.cfg
+-rw-rw-r--   0 mw        (1000) mw        (1000)     1606 2023-01-26 10:31:57.000000 ase-cogef-23.6.1/setup.py
```

### Comparing `ase-cogef-23.2.1/COPYING` & `ase-cogef-23.6.1/COPYING`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/COPYING.LESSER` & `ase-cogef-23.6.1/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/LICENSE` & `ase-cogef-23.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/PKG-INFO` & `ase-cogef-23.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ase-cogef
-Version: 23.2.1
+Version: 23.6.1
 Summary: COnstrained Geometries simulate External Force
 Home-page: https://gitedit.gitlab.io/cogef
 Maintainer: Michael Walter
 Maintainer-email: mcoywalter@gmail.com
 License: LGPLv2.1+
 Platform: unix
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ase-cogef-23.2.1/README.rst` & `ase-cogef-23.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/ase_cogef.egg-info/PKG-INFO` & `ase-cogef-23.6.1/ase_cogef.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ase-cogef
-Version: 23.2.1
+Version: 23.6.1
 Summary: COnstrained Geometries simulate External Force
 Home-page: https://gitedit.gitlab.io/cogef
 Maintainer: Michael Walter
 Maintainer-email: mcoywalter@gmail.com
 License: LGPLv2.1+
 Platform: unix
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ase-cogef-23.2.1/ase_cogef.egg-info/SOURCES.txt` & `ase-cogef-23.6.1/ase_cogef.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -10,17 +10,19 @@
 ase_cogef.egg-info/entry_points.txt
 ase_cogef.egg-info/requires.txt
 ase_cogef.egg-info/top_level.txt
 bin/cogef
 cogef/__init__.py
 cogef/cogef1d.py
 cogef/dcogef.py
+cogef/efei.py
 cogef/generalized.py
 cogef/minmax.py
 cogef/mpf.py
+cogef/neb.py
 cogef/potentials.py
 cogef/probability.py
 cogef/spring_constant.py
 cogef/units.py
 cogef/utilities.py
 cogef/vibrations.py
 cogef/cli/__init__.py
@@ -49,16 +51,19 @@
 cogef/test/rate_INTER-CTC.dat
 cogef/test/rate_INTER-TTC.dat
 cogef/test/rate_SP-INTER.dat
 cogef/test/test_MPF.py
 cogef/test/test_cogef1d.py
 cogef/test/test_cogef1d_generalized.py
 cogef/test/test_concerted.py
+cogef/test/test_dcogef.py
+cogef/test/test_efei_pair.py
 cogef/test/test_hocut.py
 cogef/test/test_minmax.py
+cogef/test/test_neb.py
 cogef/test/test_probability.py
 cogef/test/test_spring_constant.py
 cogef/test/test_spring_vibrations.py
 cogef/test/test_units.py
 cogef/test/dissociate/__init__.py
 cogef/test/dissociate/test_barrier_unit.py
 cogef/test/dissociate/test_dissociate_integration.py
```

### Comparing `ase-cogef-23.2.1/cogef/__init__.py` & `ase-cogef-23.6.1/cogef/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from cogef.probability import probability_density_polymer2
 from cogef.cogef1d import COGEF, do_nothing
 from cogef.generalized import COGEF1D
 from cogef.dissociation import Dissociation, estimate_force_change
 from cogef.dcogef import DCOGEF
 from cogef.mpf import MPF
 
-__version__ = '23.2.1'
+__version__ = '23.6.1'
 
 __all__ = ['SpringVib', 'SpringInf', 'load_rate_constants',
            'load_all_rate_constants', 'load_external_forces',
            'load_all_external_forces',
            'load_mean_distances_intact', 'load_mean_distances', 'Minima',
            'probability_density', 'rupture_force_from_dpdf',
            'rupture_force_and_uncertainty_from_dpdf', 'constant_velocity',
```

### Comparing `ase-cogef-23.2.1/cogef/cli/main.py` & `ase-cogef-23.6.1/cogef/cli/main.py`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/cogef/cogef1d.py` & `ase-cogef-23.6.1/cogef/cogef1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,41 +7,25 @@
 from pathlib import Path
 import numpy as np
 from numpy import array, polyfit
 import matplotlib.pyplot as plt
 
 from ase.constraints import dict2constraint, FixBondLength
 from ase.optimize import FIRE
-from ase import io
+from ase import Atoms, io
 from ase.io.trajectory import Trajectory
 from ase.parallel import parprint
 from ase.calculators.calculator import PropertyNotImplementedError
 from ase.io.formats import UnknownFileTypeError
 
 from cogef.utilities import mkparent
 
 
 # XXX this example seems to be outdated
-def do_nothing(image):
-    """Explanation of the initialization function needed for methods *pull*
-    and *insert* in class *COGEF*.
-
-    This function can be used to set a cell, to set a calculator and to
-    return the name of the trajectory file for the optimization.
-    Do not remove accidently *FixBondLength* with *set_constraint(...)*.
-
-    Parameters
-    ----------
-    image: Atoms object
-        Configuration which has to be optimized.
-
-    Returns
-    -------
-    image: Atoms object or similar
-    """
+def do_nothing(image: Atoms) -> Atoms:
     return image
 
 
 class COGEF(object):
     """COnstraint GEometry to simulate Forces (COGEF).
 
     Pull two atoms apart or press two atoms together by applying the COGEF
```

### Comparing `ase-cogef-23.2.1/cogef/cogef2d/cogef2d.py` & `ase-cogef-23.6.1/cogef/cogef2d/cogef2d.py`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/cogef/cogef2d/cogef2in1.py` & `ase-cogef-23.6.1/cogef/cogef2d/cogef2in1.py`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/cogef/cogef2d/dissociation2d.py` & `ase-cogef-23.6.1/cogef/cogef2d/dissociation2d.py`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/cogef/cogef2d/fixed2d.py` & `ase-cogef-23.6.1/cogef/cogef2d/fixed2d.py`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/cogef/cogef2d/neb.py` & `ase-cogef-23.6.1/cogef/cogef2d/neb.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 from ase.neb import NEB, interpolate
 from ase import io
 from ase.autoneb import AutoNEB
 from ase.optimize import BFGS
 from ase.parallel import world
 
+from cogef.neb import write_trajectory
+
 
 class Fixed2DNEB:
     """NEB class for Fixed2D"""
     def __init__(self, propagator, nebcls=NEB, nebkwargs={}):
         self.prop = propagator
         self.nebcls = nebcls
         self.nebkwargs = nebkwargs
@@ -40,17 +42,15 @@
                     images[j] = self.prop.initialize(image)
 
                     # XXX NEB does not like changing unit cells
                     # -> fix there ?
                     images[j].cell = cell
 
             def write_restart_file(images):
-                with io.Trajectory(self.frestart, 'w') as traj:
-                    for image in images:
-                        traj.write(image)
+                write_trajectory(self.frestart, images)
 
             if self.nebcls == AutoNEB:
                 prefix = Path(self.prop.name) / 'autoneb' / 'neb'
                 prefix.parent.mkdir(exist_ok=True)
 
                 additional = self.nebkwargs.pop('additional', 5)
```

### Comparing `ase-cogef-23.2.1/cogef/dcogef.py` & `ase-cogef-23.6.1/cogef/dcogef.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,18 +3,21 @@
 
 """Similar to class COGEF in cogef.py but changing a dihedral angle instead
 of a distance.
 
 """
 
 from numpy import dot, pi, sin, cos, arccos, sqrt, array
+from typing import List, Tuple
 
+from ase import Atoms
 from ase.constraints import FixInternals, FixBondLengths, ExternalForce
 from ase.constraints import MirrorTorque
 from ase.optimize import FIRE
+from ase.build.connected import connected_indices
 
 from cogef import COGEF, do_nothing
 from cogef.cogef2d import COGEF2D
 from cogef.cogef2d.cogef2d import do_nothing2d
 from cogef.cogef2d.cogef2in1 import COGEF2IN1
 
 
@@ -103,14 +106,25 @@
                      [sinphi * costheta,
                       cosphi * cospsi - sinphi * sintheta * sinpsi,
                       -cosphi * sinpsi - sinphi * sintheta * cospsi],
                      [sintheta, costheta * sinpsi, costheta * cospsi]])
     return dot(rot_mat, vector)
 
 
+def splitted_indices(atoms: Atoms,
+                     index1: int, index2: int,
+                     **kwargs) -> Tuple[List[int], List[int]]:
+    def connected(i1, i2):
+        atoms_copy = atoms.copy()
+        atoms_copy[i1].symbol = 'X'
+        return connected_indices(atoms_copy, i2, **kwargs)
+
+    return connected(index2, index1), connected(index1, index2)
+
+
 class DCOGEF(COGEF):
     """COGEF method based on the dihedral angle.
 
     Parameters
     ----------
     images: str or list of Atoms objects
         Initial trajectory or its filename.
@@ -128,27 +142,31 @@
         and during optimization,
         e.g. *fixed_atom_pairs=[(1, 3), (4, 2), (10, 11)]*.
 
     """
     def __init__(self, images, dihedral_indices, optimizer=FIRE, fmax=0.1,
                  optimizer_logfile='-',
                  fixed_atom_pairs=None):
-        COGEF.__init__(self, images, dihedral_indices[0], dihedral_indices[1],
+        COGEF.__init__(self, dihedral_indices[1], dihedral_indices[2],
+                       'dcogef', 'dcogef.traj',
                        optimizer, fmax, optimizer_logfile,
                        fixed_atom_pairs)  # TODO: dihedral_indices[1] -> [3] ?
+        self.images = images
         self.dihedral_indices = dihedral_indices
 
-    def pull(self, stepangle, steps, initialize=do_nothing,
-             trajectory='pull.traj'):
+        _, self.rotated_indices = splitted_indices(images[0],
+                                                   *dihedral_indices[1:3])
+
+    def pull(self, stepangle, steps, initialize=do_nothing):
         """Obtain the COGEF path by rotating the dihedral angle.
         See also class COGEF.
 
         """
         return COGEF.pull(self, stepsize=stepangle, steps=steps,
-                          initialize=initialize, trajectory=trajectory)
+                          initialize=initialize)
 
     def insert(self, imagenum, steps=1, initialize=do_nothing,
                trajectory='pull.traj'):
         raise NotImplementedError('The method "insert" is not ' +
                                   'implemented, yet.')
 
     def log(self, step, steps, atoms, logfile):
@@ -161,87 +179,26 @@
         logfile.write('\n%s: step %d/%d, dihedral angle %15.6f degrees\n\n'
                       % (name, step + 1, steps,
                          atoms.get_dihedral(self.dihedral_indices[0],
                                             self.dihedral_indices[1],
                                             self.dihedral_indices[2],
                                             self.dihedral_indices[3])))
 
-    def shift_atoms(self, atoms, stepangle):
-        """Increase the dihedral angle.
-
-        Move atoms with indices *self.dihedral_indices[0]* and
-        *self.dihedral_indices[3]* to change the dihedral angle by
-        stepangle, then fix the dihedral angle. Set stepangle to None if
-        you want an optimization without fixed dihedral angle.
-
-        Parameters
-        ----------
-        atoms: Atoms object
-            Configuration used for modification.
-        stepangle: float
-            Total increase of dihedral angle.
-            Set *stepangle* to *None* in order to only fix bond defined in
-            *self.fixed_atom_pairs*.
-
-        Returns
-        -------
-        result: tuple of two floats or tuple of two numpy arrays
-            The shift angle of both atoms.
-
-        """
-        if stepangle is None:
-            if self.fixed_atom_pairs:
-                con = FixBondLengths(self.fixed_atom_pairs)
-            else:
-                con = []
-            atoms.set_constraint(con)
-            return 0., 0.  # TODO: why not two times *zeros(3)*?
-        atom1 = self.dihedral_indices[0]
-        atom2 = self.dihedral_indices[1]
-        atom3 = self.dihedral_indices[2]
-        atom4 = self.dihedral_indices[3]
-        vec = atoms[atom3].position - atoms[atom2].position
-        stepangle -= int(stepangle / (2 * pi)) * 2 * pi
-        value1 = stepangle / 2.
-        value2 = stepangle / 2.
-        if self.fixed_atom_pairs:
-            atom1in = False
-            atom2in = False
-            for pair in self.fixed_atom_pairs:
-                if self.atom1 in pair:
-                    atom1in = True
-                if self.atom2 in pair:
-                    atom2in = True
-            if atom1in:
-                value2 = value1 + value2
-                value1 = 0
-            elif atom2in:
-                value1 = value1 + value2
-                value2 = 0
-            bonds = []
-            for pair in self.fixed_atom_pairs:
-                bonds.append([atoms.get_distance(pair[0], pair[1]), pair])
-        else:
-            bonds = None
-        pos1 = atoms[atom1].position
-        pos2 = atoms[atom2].position
-        atoms[atom1].position = rotate_around_axis(vec, pos1 - pos2,
-                                                   -value1) + pos2
-        pos3 = atoms[atom3].position
-        pos4 = atoms[atom4].position
-        atoms[atom4].position = rotate_around_axis(vec, pos4 - pos3,
-                                                   value2) + pos3
-        dihedral = [atoms.get_dihedral(self.dihedral_indices[0],
-                                       self.dihedral_indices[1],
-                                       self.dihedral_indices[2],
-                                       self.dihedral_indices[3]) * pi / 180.,
-                    self.dihedral_indices]
-        con = FixInternals(bonds=bonds, dihedrals=[dihedral])
-        atoms.set_constraint(con)
-        return -value1, value2
+    def shift_atoms(self, atoms: Atoms, stepangle: float):
+        pos0 = atoms[self.dihedral_indices[1]].position
+        axis = atoms[self.dihedral_indices[2]].position - pos0
+
+        for ia in self.rotated_indices:
+            atoms[ia].position = (
+                pos0 + rotate_around_axis(
+                    axis, atoms[ia].position - pos0, stepangle))
+
+        dihedral_deg = atoms.get_dihedral(*self.dihedral_indices)
+        atoms.constaint = FixInternals(
+            dihedrals_deg=[[dihedral_deg, self.dihedral_indices]])
 
 
 class DCOGEF2D(COGEF2D):
     """Like class COGEF2D but the second constraint parameter is a
     dihedral angle instead of a bond length.
 
     Parameters
```

### Comparing `ase-cogef-23.2.1/cogef/dissociation/barrier.py` & `ase-cogef-23.6.1/cogef/dissociation/barrier.py`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/cogef/dissociation/diss_old.py` & `ase-cogef-23.6.1/cogef/dissociation/diss_old.py`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/cogef/dissociation/dissociation.py` & `ase-cogef-23.6.1/cogef/dissociation/dissociation.py`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/cogef/dissociation/tabulated_barrier.py` & `ase-cogef-23.6.1/cogef/dissociation/tabulated_barrier.py`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/cogef/generalized.py` & `ase-cogef-23.6.1/cogef/generalized.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,82 @@
 from pathlib import Path
 import numpy as np
+from typing import Union, List
+from collections.abc import Iterable
 
-from ase import io
+from ase import io, Atoms
 from ase.constraints import FixBondLength, FixBondLengths
 from ase.parallel import parprint, world
 from ase.utils import deprecated, IOContext
+from ase.optimize.optimize import Optimizer
+from ase.optimize import FIRE
 
 from cogef import COGEF
 from cogef.utilities import mkparent
 
 
+def shift_atoms_mass_weighted(
+        atoms: Atoms, i1: int, i2: int, stepsize: float):
+    a1 = atoms[i1]
+    a2 = atoms[i2]
+    nvec12 = a2.position - a1.position
+    nvec12 /= np.linalg.norm(nvec12)
+    # shift mass weighted
+    a1.position -= stepsize * a2.mass / (a1.mass + a2.mass) * nvec12
+    a2.position += stepsize * a1.mass / (a1.mass + a2.mass) * nvec12
+
+
+def pair_extended_name(cls, pair: List[int], value: str = None) -> str:
+    if value is None:
+        name = str(cls.__class__.__name__).lower()
+    else:
+        name = str(value)
+
+    # add pull positions as extension if not already there
+    ext = '_{0}_{1}'.format(*pair)
+    if ext not in name:
+        name += ext
+
+    return name
+
+
 class COGEF1D(COGEF, IOContext):
-    def __init__(self, atom1, atom2, initialize=None,
-                 txt='-', comm=world, **kwargs):
-        self.initialize = initialize
+    def __init__(self, atom1: int, atom2: int, initialize=None,
+                 name=None,
+                 optimizer: Optimizer = FIRE,
+                 fmax: float = 0.1,
+                 trajname: str = 'cogef.traj',
+                 txt='-',
+                 comm=world,
+                 optimizer_logfile='-'):
+        self.trajname = trajname
         self.txt = self.openfile(txt, comm)
-        COGEF.__init__(self, atom1, atom2, **kwargs)
+
+        self.atom1 = atom1
+        self.atom2 = atom2
+        # XXX remove
+        self.constdict = FixBondLength(atom1, atom2).todict()
+
+        self._initialize = initialize
+        self.name = name
+        self.optimizer = optimizer
+        self.fmax = fmax
+
+        # XXX is this needed?
+        self.optimizer_logfile = optimizer_logfile
+        self.last_intact_bond_image = float("inf")
 
     @property
     def name(self):
         return self._name
 
     @name.setter
     def name(self, value):
-        if value is None:
-            self._name = str(self.__class__.__name__).lower()
-        else:
-            self._name = str(value)
-
-        # add pull positions as extension if not already there
-        ext = '_{0}_{1}'.format(self.atom1, self.atom2)
-        if ext not in self._name:
-            self._name += ext
+        self._name = pair_extended_name(
+            self, [self.atom1, self.atom2], value)
 
         # name change => remove images
         self._images = []
         self.look_for_images()
 
     def shift_and_optimize(self, mother, dstep, index):
         """Shift atoms by dstep and optimze
@@ -62,45 +103,55 @@
             mkparent(optimizer_traj)
             atoms = mother.copy()
             self.shift_atoms(atoms, dstep)
 
         # make sure my constraint is there before initialize
         self.add_my_constraint(atoms)
 
-        if self.initialize is None:
-            atoms.calc = self.images[-1].calc
-        else:
-            # let the user provided function take care about the image
-            atoms = self.initialize(atoms)
+        atoms = self.initialize(atoms)
 
         # make sure, my constraint is not accidently removed
         self.add_my_constraint(atoms)
 
         return self._optimize(atoms)
 
+    def initialize(self, atoms):
+        if self._initialize is None:
+            atoms.calc = self.images[-1].calc
+        else:
+            # let the user provided function take care about the image
+            atoms = self._initialize(atoms)
+        return atoms
+
     def _optimize(self, atoms):
         opt = self.optimizer(atoms, logfile=self.txt)
         opt.run(fmax=self.fmax)
         return atoms
 
-    def move(self, dstep, steps):
-        if len(self.images) == 1:
-            # make sure first image is relaxed
-            self.images[0] = self._optimize(self.images[0])
+    def update_trajectory(self, name: str) -> io.Trajectory:
+        filename = Path(name)
 
-        filename = Path(self.trajname)
         if filename.is_file():
             trajectory = io.Trajectory(filename, 'a')
             assert len(trajectory) == len(self.images)
         else:
             mkparent(filename)
             trajectory = io.Trajectory(filename, 'w')
             for image in self.images:
                 trajectory.write(image)
 
+        return trajectory
+
+    def move(self, dstep, steps):
+        if len(self.images) == 1:
+            # make sure first image is relaxed
+            self.images[0] = self._optimize(self.images[0])
+
+        trajectory = self.update_trajectory(self.trajname)
+
         for i in range(steps):
             parprint(self.__class__.__name__, f'step {i + 1}/{steps}',
                      file=self.txt)
             self.images.append(
                 self.shift_and_optimize(
                     self.images[-1], dstep=dstep, index=len(self.images)))
             trajectory.write(self.images[-1])
@@ -108,23 +159,17 @@
     @deprecated(DeprecationWarning('Please use move'))
     def pull(self, dstep, steps, initialize=None):
         self.move(dstep, steps)
 
     def __len__(self):
         return len(self.images)
 
-    def shift_atoms(self, atoms, stepsize):
+    def shift_atoms(self, atoms: Atoms, stepsize: float) -> None:
         """Shift atoms by stepsize"""
-        a1 = atoms[self.atom1]
-        a2 = atoms[self.atom2]
-        nvec12 = a2.position - a1.position
-        nvec12 /= np.linalg.norm(nvec12)
-        # shift mass weighted
-        a1.position -= stepsize * a2.mass / (a1.mass + a2.mass) * nvec12
-        a2.position += stepsize * a1.mass / (a1.mass + a2.mass) * nvec12
+        shift_atoms_mass_weighted(atoms, self.atom1, self.atom2, stepsize)
 
     def add_my_constraint(self, atoms):
         """make sure my constraint is present"""
         self.remove_my_constraint(atoms)
         atoms.constraints.append(self.get_constraint())
 
     def remove_my_constraint(self, atoms):
@@ -146,75 +191,68 @@
 
     def get_energies(self):
         return np.array([img.get_potential_energy()
                          for img in self.images])
 
     def get_forces(self):
         """Return forces due to constraint"""
-        # XXX implement yourself?
-        forces, distances = self.get_force_curve('use_forces')
-        return forces
 
-    def forces_from_energies(self):
-        """Forces from energy derivatives
+        def constraint_force(image):
+            vec = image[self.atom2].position - image[self.atom1].position
+            vec /= np.linalg.norm(vec)
+            forces = image.get_forces(apply_constraint=False)
+            delta_f = forces[self.atom1] - forces[self.atom2]
+            return np.dot(delta_f, vec) / 2.
 
-        returns: distances and corresponding forces
-        """
-        # XXX implement yourself?
-        forces, distances = self.get_force_curve('use_energies')
-        return distances, forces
+        return np.array([constraint_force(img)
+                         for img in self.images])
 
     def look_for_images(self):
-        """Check whether there are images already based on the name"""
-        try:
-            self.images = io.Trajectory(self.trajname)
+        """Read images if the Trajectory-file exists already"""
+        if Path(self.trajname).exists():
+            with io.Trajectory(self.trajname) as traj:
+                self.images = [img for img in traj]
             parprint(self.__class__.__name__ + ': read', len(self.images),
                      'images from', self.trajname, file=self.txt)
-        except FileNotFoundError:
-            pass
 
 
 class Concerted(COGEF1D):
     """COGEF1D for concerted variation of two bonds"""
     def __init__(self, pairs, *args, **kwargs):
         """
         pair1: indices of first bond
         pair2: indices of second bond
         """
         self.pairs = pairs
         COGEF1D.__init__(self, *pairs[0], *args, **kwargs)
 
-    def shift_atoms(self, atoms, stepsize):
-        """Shift atoms by stepsize"""
-        for i1, i2 in self.pairs:
-            a1 = atoms[i1]
-            a2 = atoms[i2]
-            nvec12 = a2.position - a1.position
-            nvec12 /= np.linalg.norm(nvec12)
-            # shift mass weighted
-            a1.position -= stepsize * a2.mass / (a1.mass + a2.mass) * nvec12
-            a2.position += stepsize * a1.mass / (a1.mass + a2.mass) * nvec12
+    def move(self, dstep: Union[float, Iterable], steps: int):
+        """Move pairs by dstep for given number of steps"""
+        if isinstance(dstep, Iterable):
+            assert len(dstep) == 2  # 2 pairs up to now
+        else:
+            dstep = [dstep] * 2
+        super().move(dstep, steps)
+
+    def shift_atoms(self, atoms: Atoms, stepsize: List[float]):
+        for dx, (i1, i2) in zip(stepsize, self.pairs):
+            shift_atoms_mass_weighted(atoms, i1, i2, dx)
 
     def get_constraint(self):
         # we need to create a new constraint for every image
         return FixBondLengths(self.pairs)
 
     @property
     def name(self):
         return self._name
 
     @name.setter
     def name(self, value):
-        if value is None:
-            self._name = str(self.__class__.__name__).lower()
-        else:
-            self._name = str(value)
-
-        # add pull positions as extension if not already there
-        for pair in self.pairs:
-            ext = '_{0}_{1}'.format(*pair)
-            if ext not in self._name:
-                self._name += ext
+        name = pair_extended_name(
+            self, self.pairs[0], value)
+        for pair in self.pairs[1:]:
+            name = pair_extended_name(self, pair, name)
+        self._name = name
 
         # name change => remove images
         self._images = []
         self.look_for_images()
```

### Comparing `ase-cogef-23.2.1/cogef/minmax.py` & `ase-cogef-23.6.1/cogef/minmax.py`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/cogef/mpf.py` & `ase-cogef-23.6.1/cogef/mpf.py`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/cogef/potentials.py` & `ase-cogef-23.6.1/cogef/potentials.py`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/cogef/probability.py` & `ase-cogef-23.6.1/cogef/probability.py`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/cogef/spring_constant.py` & `ase-cogef-23.6.1/cogef/spring_constant.py`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/cogef/test/au6harmonic.py` & `ase-cogef-23.6.1/cogef/test/au6harmonic.py`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/cogef/test/conftest.py` & `ase-cogef-23.6.1/cogef/test/conftest.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from pathlib import Path
 import pytest
 from ase import Atoms
 from ase.utils import workdir
 from ase.calculators.morse import MorsePotential
 from ase.optimize import FIRE
+from ase.calculators.emt import EMT
 
 from cogef import COGEF1D
 
 
 @pytest.fixture(autouse=True)
 def use_tmp_workdir(tmp_path):
     # Pytest can on some systems provide a Path from pathlib2.  Normalize:
@@ -15,14 +16,24 @@
     with workdir(path, mkdir=True):
         yield tmp_path
     # We print the path so user can see where test failed, if it failed.
     print(f'Testpath: {path}')
 
 
 @pytest.fixture
+def H3():
+    """create H3 optimized in EMT"""
+    image = Atoms('H3', positions=[(0, 0, 0), (0.751, 0, 0), (0, 1., 0)])
+    image.calc = EMT()
+    opt = FIRE(image, logfile=None)
+    opt.run(fmax=0.05)
+    return image
+
+
+@pytest.fixture
 def H4():
     """Linear H4 with Morse potential"""
     image = Atoms('H4', positions=[(i, 0, 0) for i in range(4)])
     image.calc = MorsePotential()
     return image
```

### Comparing `ase-cogef-23.2.1/cogef/test/dissociate/test_barrier_unit.py` & `ase-cogef-23.6.1/cogef/test/dissociate/test_barrier_unit.py`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/cogef/test/dissociate/test_dissociate_integration.py` & `ase-cogef-23.6.1/cogef/test/dissociate/test_dissociate_integration.py`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/cogef/test/dissociate/test_tabulated_barrier.py` & `ase-cogef-23.6.1/cogef/test/dissociate/test_tabulated_barrier.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         F_ana = Fmax * mpf.general(T_K=T, alpha_nNs=alpha_nNs)
         F_rup, F_err = diss.rupture_force_and_uncertainty(
             T, alpha_nNs * nN, Fmax, 0.0, 0.001)
         assert F_rup == pytest.approx(F_ana, 0.01)
 
 
 def test_tabulated():
+    """Compare a tabulated barrier against an analytic barrier"""
     Fmax = 5
     De = 3
 
     T = 300
     alpha_nNs = 1
 
     bexact = Quadratic(De, Fmax)
```

### Comparing `ase-cogef-23.2.1/cogef/test/rate_0_1.dat` & `ase-cogef-23.6.1/cogef/test/rate_0_1.dat`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/cogef/test/rate_0_8.dat` & `ase-cogef-23.6.1/cogef/test/rate_0_8.dat`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/cogef/test/rate_1_2.dat` & `ase-cogef-23.6.1/cogef/test/rate_1_2.dat`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/cogef/test/rate_29_11.dat` & `ase-cogef-23.6.1/cogef/test/rate_29_11.dat`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/cogef/test/rate_8_12.dat` & `ase-cogef-23.6.1/cogef/test/rate_8_12.dat`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/cogef/test/rate_CTC-CCC.dat` & `ase-cogef-23.6.1/cogef/test/rate_CTC-CCC.dat`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/cogef/test/rate_CTC-TTC.dat` & `ase-cogef-23.6.1/cogef/test/rate_CTC-TTC.dat`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/cogef/test/rate_INTER-CTC.dat` & `ase-cogef-23.6.1/cogef/test/rate_INTER-CTC.dat`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/cogef/test/rate_INTER-TTC.dat` & `ase-cogef-23.6.1/cogef/test/rate_INTER-TTC.dat`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/cogef/test/rate_SP-INTER.dat` & `ase-cogef-23.6.1/cogef/test/rate_SP-INTER.dat`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/cogef/test/test_MPF.py` & `ase-cogef-23.6.1/cogef/test/test_MPF.py`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/cogef/test/test_cogef1d.py` & `ase-cogef-23.6.1/cogef/test/test_cogef1d.py`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/cogef/test/test_cogef1d_generalized.py` & `ase-cogef-23.6.1/cogef/test/test_cogef1d_generalized.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,15 @@
 import pytest
 from ase import Atoms
 from ase.calculators.emt import EMT
-from ase.optimize import FIRE
 from ase.constraints import FixBondLength
 
 from cogef import COGEF1D
 
 
-@pytest.fixture
-def H3():
-    """create H3 optimized in EMT"""
-    image = Atoms('H3', positions=[(0, 0, 0), (0.751, 0, 0), (0, 1., 0)])
-    image.calc = EMT()
-    opt = FIRE(image, logfile=None)
-    opt.run(fmax=0.05)
-    return image
-
-
 def test_unrelaxed(H3):
     """First [0] image should be relaxed without constraints"""
     image = Atoms('H3', positions=[(0, 0, 0), (0.751, 0, 0), (0, 1., 0)])
     image.calc = EMT()
 
     cogef1d = COGEF1D(0, 1, fmax=0.05)
     cogef1d.images = [image]
@@ -90,15 +79,16 @@
     constraint = FixBondLength(1, 2)
 
     def initialize(atoms):
         atoms.set_constraint(constraint)
         atoms.calc = EMT()
         return atoms
 
-    cogefH6.initialize = initialize
+    # XXX too much couplig XXX
+    cogefH6._initialize = initialize
     cogefH6.move(0.2, 1)
     image = cogefH6.images[-1]
     assert len(image.constraints) == 2   # cogef adds one
 
     hascons = False
     for cons in image.constraints:
         if cons.todict() == constraint.todict():
@@ -108,11 +98,7 @@
 
 def test_distances_energies_forces(cogefH6):
     """Assure basic functions to exist and give correct result size"""
     cogefH6.move(0.2, 4)
     assert len(cogefH6.get_distances()) == len(cogefH6.images)
     assert len(cogefH6.get_energies()) == len(cogefH6.images)
     assert len(cogefH6.get_forces()) == len(cogefH6.images)
-
-    d_i, f_i = cogefH6.forces_from_energies()
-    assert len(d_i) == len(cogefH6.images) - 2
-    assert len(d_i) == len(f_i)
```

### Comparing `ase-cogef-23.2.1/cogef/test/test_hocut.py` & `ase-cogef-23.6.1/cogef/test/test_hocut.py`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/cogef/test/test_minmax.py` & `ase-cogef-23.6.1/cogef/test/test_minmax.py`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/cogef/test/test_probability.py` & `ase-cogef-23.6.1/cogef/test/test_probability.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # Copyright (C) 2016-2019
 # See accompanying license files for details.
 
 """Tests for cogef/probability.py
 
 """
-from os.path import join
+import os.path
 from numpy import array
 
 from cogef import __path__
 from cogef import load_rate_constants, load_all_rate_constants, Minima
 from cogef import probability_density
 from cogef import rupture_force_and_uncertainty_from_dpdf
 
 
 def test_minima(tmpdir):
     # Class Minima
-
     loading_rate = 10.
-    path = join(__path__[0], 'test')
+    path = os.path.join(__path__[0], 'test')
 
     print('\n' +
           '1) C6H14: 5 CC bonds, 3 different forward rates')
     rates08, forces08 = load_rate_constants(
-        join(path, 'rate_0_8.dat'))  # outer bond
-    rates01, forces01 = load_rate_constants(join(path, 'rate_0_1.dat'))
+        os.path.join(path, 'rate_0_8.dat'))  # outer bond
+    rates01, forces01 = load_rate_constants(os.path.join(path, 'rate_0_1.dat'))
     rates12, forces12 = load_rate_constants(
-        join(path, 'rate_1_2.dat'))  # middle bond
+        os.path.join(path, 'rate_1_2.dat'))  # middle bond
     forces = forces08
-    assert forces == forces01 and forces == forces12
+    assert forces == forces01
+    assert forces == forces12
     # R -> P1
     #   -> P2
     #   -> P3
     #   -> P4
     #   -> P5
     minima = Minima()
     minima.add_destination(rates08)
@@ -56,17 +56,17 @@
 
     # ------------------------------------
 
     print('\n' +
           '2) Spiropyran: two transitions with forward and backward rates ' +
           'respectively')
     rates8_12, backrates8_12, forces8_12 = \
-        load_all_rate_constants(join(path, 'rate_8_12.dat'))
+        load_all_rate_constants(os.path.join(path, 'rate_8_12.dat'))
     rates29_11, backrates29_11, forces29_11 = \
-        load_all_rate_constants(join(path, 'rate_29_11.dat'))
+        load_all_rate_constants(os.path.join(path, 'rate_29_11.dat'))
     forces = forces8_12
     assert forces == forces29_11
     # R <-> I <-> P
     minima = Minima()
     minima.set_position(minima.add_destination(rates8_12, backrates8_12))
     minima.add_destination(rates29_11, backrates29_11)
     dpdf = probability_density(minima, forces, loading_rate)
@@ -79,23 +79,23 @@
     print('(' + str(round(f_rup, 2)) + ' +- ' + str(round(f_err, 2)) + ') nN')
 
     # ------------------------------------
 
     print('\n' +
           '3) More complex spiropyran system')
     rates_sp_inter, backrates_sp_inter, forces_sp_inter = \
-        load_all_rate_constants(join(path, 'rate_SP-INTER.dat'))
+        load_all_rate_constants(os.path.join(path, 'rate_SP-INTER.dat'))
     rates_inter_ctc, backrates_inter_ctc, forces_inter_ctc \
-        = load_all_rate_constants(join(path, 'rate_INTER-CTC.dat'))
+        = load_all_rate_constants(os.path.join(path, 'rate_INTER-CTC.dat'))
     rates_inter_ttc, backrates_inter_ttc, forces_inter_ttc \
-        = load_all_rate_constants(join(path, 'rate_INTER-TTC.dat'))
+        = load_all_rate_constants(os.path.join(path, 'rate_INTER-TTC.dat'))
     rates_ctc_ttc, backrates_ctc_ttc, forces_ctc_ttc \
-        = load_all_rate_constants(join(path, 'rate_CTC-TTC.dat'))
+        = load_all_rate_constants(os.path.join(path, 'rate_CTC-TTC.dat'))
     rates_ctc_ccc, backrates_ctc_ccc, forces_ctc_ccc \
-        = load_all_rate_constants(join(path, 'rate_CTC-CCC.dat'))
+        = load_all_rate_constants(os.path.join(path, 'rate_CTC-CCC.dat'))
     forces = forces_sp_inter
     assert forces == forces_inter_ctc and \
         forces == forces_inter_ttc and \
         forces == forces_ctc_ttc and \
         forces == forces_ctc_ccc
     # SP <-> inter. <-> CTC <-> CCC
     #                    ^
```

### Comparing `ase-cogef-23.2.1/cogef/test/test_spring_constant.py` & `ase-cogef-23.6.1/cogef/test/test_spring_constant.py`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/cogef/test/test_spring_vibrations.py` & `ase-cogef-23.6.1/cogef/test/test_spring_vibrations.py`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/cogef/utilities.py` & `ase-cogef-23.6.1/cogef/utilities.py`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/cogef/vibrations.py` & `ase-cogef-23.6.1/cogef/vibrations.py`

 * *Files identical despite different names*

### Comparing `ase-cogef-23.2.1/setup.py` & `ase-cogef-23.6.1/setup.py`

 * *Files identical despite different names*

