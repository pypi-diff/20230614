# Comparing `tmp/flightanalysis-0.1.0.tar.gz` & `tmp/flightanalysis-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flightanalysis-0.1.0.tar", last modified: Wed Mar  1 19:17:55 2023, max compression
+gzip compressed data, was "flightanalysis-0.1.1.tar", last modified: Wed Jun 14 09:41:56 2023, max compression
```

## Comparing `flightanalysis-0.1.0.tar` & `flightanalysis-0.1.1.tar`

### file list

```diff
@@ -1,76 +1,89 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-03-01 19:17:55.829802 flightanalysis-0.1.0/
--rw-r--r--   0 tom       (1000) tom       (1000)    35149 2022-12-20 14:21:12.000000 flightanalysis-0.1.0/LICENSE
--rw-r--r--   0 tom       (1000) tom       (1000)     1976 2023-03-01 19:17:55.829802 flightanalysis-0.1.0/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     1693 2022-12-20 14:21:12.000000 flightanalysis-0.1.0/README.md
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-03-01 19:17:55.819802 flightanalysis-0.1.0/flightanalysis/
--rw-r--r--   0 tom       (1000) tom       (1000)      219 2022-12-20 14:21:12.000000 flightanalysis-0.1.0/flightanalysis/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3609 2022-12-20 14:21:12.000000 flightanalysis-0.1.0/flightanalysis/aircraft_analysis.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-03-01 19:17:55.819802 flightanalysis-0.1.0/flightanalysis/base/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2022-12-20 14:21:12.000000 flightanalysis-0.1.0/flightanalysis/base/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1755 2023-03-01 19:12:41.000000 flightanalysis-0.1.0/flightanalysis/base/collection.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2175 2023-03-01 19:12:41.000000 flightanalysis-0.1.0/flightanalysis/base/constructs.py
--rw-r--r--   0 tom       (1000) tom       (1000)      221 2022-12-20 14:21:12.000000 flightanalysis-0.1.0/flightanalysis/base/numpy_encoder.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3810 2023-03-01 19:12:41.000000 flightanalysis-0.1.0/flightanalysis/base/table.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1695 2023-03-01 19:12:41.000000 flightanalysis-0.1.0/flightanalysis/controls.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-03-01 19:17:55.819802 flightanalysis-0.1.0/flightanalysis/criteria/
--rw-r--r--   0 tom       (1000) tom       (1000)     1454 2022-12-20 18:43:19.000000 flightanalysis-0.1.0/flightanalysis/criteria/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2350 2022-12-20 14:21:12.000000 flightanalysis-0.1.0/flightanalysis/criteria/combination.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1324 2022-12-20 14:21:12.000000 flightanalysis-0.1.0/flightanalysis/criteria/comparison.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2013 2022-12-20 18:43:19.000000 flightanalysis-0.1.0/flightanalysis/criteria/continuous.py
--rw-r--r--   0 tom       (1000) tom       (1000)      925 2022-12-20 14:21:12.000000 flightanalysis-0.1.0/flightanalysis/criteria/results.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1331 2023-03-01 19:12:41.000000 flightanalysis-0.1.0/flightanalysis/criteria/single.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-03-01 19:17:55.819802 flightanalysis-0.1.0/flightanalysis/data/
--rw-r--r--   0 tom       (1000) tom       (1000)      296 2023-01-28 21:30:38.000000 flightanalysis-0.1.0/flightanalysis/data/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)    10931 2023-03-01 19:12:41.000000 flightanalysis-0.1.0/flightanalysis/data/p23.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-03-01 19:17:55.819802 flightanalysis-0.1.0/flightanalysis/environment/
--rw-r--r--   0 tom       (1000) tom       (1000)       91 2022-12-20 14:21:12.000000 flightanalysis-0.1.0/flightanalysis/environment/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1395 2023-03-01 19:12:41.000000 flightanalysis-0.1.0/flightanalysis/environment/environment.py
--rw-r--r--   0 tom       (1000) tom       (1000)     4345 2022-12-20 14:21:12.000000 flightanalysis-0.1.0/flightanalysis/environment/wind.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6335 2023-01-28 21:30:38.000000 flightanalysis-0.1.0/flightanalysis/fc_json.py
--rw-r--r--   0 tom       (1000) tom       (1000)     7236 2022-12-20 14:21:12.000000 flightanalysis-0.1.0/flightanalysis/flightline.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-03-01 19:17:55.819802 flightanalysis-0.1.0/flightanalysis/model/
--rw-r--r--   0 tom       (1000) tom       (1000)      108 2022-12-20 14:21:12.000000 flightanalysis-0.1.0/flightanalysis/model/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1181 2023-03-01 19:12:41.000000 flightanalysis-0.1.0/flightanalysis/model/coefficients.py
--rw-r--r--   0 tom       (1000) tom       (1000)      405 2022-12-20 14:21:12.000000 flightanalysis-0.1.0/flightanalysis/model/constants.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1379 2023-03-01 19:12:41.000000 flightanalysis-0.1.0/flightanalysis/model/flow.py
--rw-r--r--   0 tom       (1000) tom       (1000)      675 2022-12-20 14:21:12.000000 flightanalysis-0.1.0/flightanalysis/model/model.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-03-01 19:17:55.819802 flightanalysis-0.1.0/flightanalysis/schedule/
--rw-r--r--   0 tom       (1000) tom       (1000)     2854 2022-12-20 14:21:12.000000 flightanalysis-0.1.0/flightanalysis/schedule/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-03-01 19:17:55.829802 flightanalysis-0.1.0/flightanalysis/schedule/definition/
--rw-r--r--   0 tom       (1000) tom       (1000)      641 2023-03-01 19:12:41.000000 flightanalysis-0.1.0/flightanalysis/schedule/definition/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1442 2023-03-01 19:12:41.000000 flightanalysis-0.1.0/flightanalysis/schedule/definition/collectors.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6720 2023-03-01 19:12:41.000000 flightanalysis-0.1.0/flightanalysis/schedule/definition/element_definition.py
--rw-r--r--   0 tom       (1000) tom       (1000)    13176 2023-03-01 19:12:41.000000 flightanalysis-0.1.0/flightanalysis/schedule/definition/manoeuvre_definition.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3994 2022-12-20 14:21:12.000000 flightanalysis-0.1.0/flightanalysis/schedule/definition/manoeuvre_info.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6781 2023-03-01 19:12:41.000000 flightanalysis-0.1.0/flightanalysis/schedule/definition/manoeuvre_parameters.py
--rw-r--r--   0 tom       (1000) tom       (1000)     5146 2022-12-20 14:21:12.000000 flightanalysis-0.1.0/flightanalysis/schedule/definition/operation.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1978 2022-12-20 14:21:12.000000 flightanalysis-0.1.0/flightanalysis/schedule/definition/schedule_definition.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-03-01 19:17:55.829802 flightanalysis-0.1.0/flightanalysis/schedule/elements/
--rw-r--r--   0 tom       (1000) tom       (1000)     6662 2023-03-01 19:12:41.000000 flightanalysis-0.1.0/flightanalysis/schedule/elements/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3389 2023-03-01 19:12:41.000000 flightanalysis-0.1.0/flightanalysis/schedule/elements/line.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6406 2023-03-01 19:12:41.000000 flightanalysis-0.1.0/flightanalysis/schedule/elements/loop.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3461 2023-03-01 19:12:41.000000 flightanalysis-0.1.0/flightanalysis/schedule/elements/snap.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3747 2023-03-01 19:12:41.000000 flightanalysis-0.1.0/flightanalysis/schedule/elements/spin.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1674 2023-03-01 19:12:41.000000 flightanalysis-0.1.0/flightanalysis/schedule/elements/stall_turn.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3182 2023-03-01 19:12:41.000000 flightanalysis-0.1.0/flightanalysis/schedule/manoeuvre.py
--rw-r--r--   0 tom       (1000) tom       (1000)     4367 2022-12-20 14:21:12.000000 flightanalysis-0.1.0/flightanalysis/schedule/schedule.py
--rw-r--r--   0 tom       (1000) tom       (1000)      891 2022-12-20 14:21:12.000000 flightanalysis-0.1.0/flightanalysis/simulation.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-03-01 19:17:55.829802 flightanalysis-0.1.0/flightanalysis/state/
--rw-r--r--   0 tom       (1000) tom       (1000)     1554 2023-03-01 19:12:41.000000 flightanalysis-0.1.0/flightanalysis/state/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2175 2023-03-01 19:12:41.000000 flightanalysis-0.1.0/flightanalysis/state/state.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-03-01 19:17:55.829802 flightanalysis-0.1.0/flightanalysis/state/tools/
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2022-12-20 14:21:12.000000 flightanalysis-0.1.0/flightanalysis/state/tools/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3461 2023-03-01 19:12:41.000000 flightanalysis-0.1.0/flightanalysis/state/tools/alignment.py
--rw-r--r--   0 tom       (1000) tom       (1000)     4315 2023-03-01 19:12:41.000000 flightanalysis-0.1.0/flightanalysis/state/tools/builders.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2722 2022-12-20 14:21:12.000000 flightanalysis-0.1.0/flightanalysis/state/tools/conversions.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3691 2022-12-20 14:21:12.000000 flightanalysis-0.1.0/flightanalysis/state/tools/dumpers.py
--rw-r--r--   0 tom       (1000) tom       (1000)      934 2023-03-01 19:12:41.000000 flightanalysis-0.1.0/flightanalysis/state/tools/measurements.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2883 2023-03-01 19:12:41.000000 flightanalysis-0.1.0/flightanalysis/state/tools/transformers.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-03-01 19:17:55.819802 flightanalysis-0.1.0/flightanalysis.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)     1976 2023-03-01 19:17:55.000000 flightanalysis-0.1.0/flightanalysis.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     2265 2023-03-01 19:17:55.000000 flightanalysis-0.1.0/flightanalysis.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-03-01 19:17:55.000000 flightanalysis-0.1.0/flightanalysis.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       49 2023-03-01 19:17:55.000000 flightanalysis-0.1.0/flightanalysis.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       15 2023-03-01 19:17:55.000000 flightanalysis-0.1.0/flightanalysis.egg-info/top_level.txt
--rw-r--r--   0 tom       (1000) tom       (1000)      418 2023-03-01 19:17:55.829802 flightanalysis-0.1.0/setup.cfg
--rw-r--r--   0 tom       (1000) tom       (1000)      672 2023-03-01 19:15:51.000000 flightanalysis-0.1.0/setup.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:41:56.971436 flightanalysis-0.1.1/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)    35149 2023-03-28 15:54:19.000000 flightanalysis-0.1.1/LICENSE
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1443 2023-06-14 09:41:56.971436 flightanalysis-0.1.1/PKG-INFO
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1160 2023-03-28 15:54:19.000000 flightanalysis-0.1.1/README.md
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:41:56.959435 flightanalysis-0.1.1/flightanalysis/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      261 2023-03-28 15:54:19.000000 flightanalysis-0.1.1/flightanalysis/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     3609 2023-03-28 15:54:19.000000 flightanalysis-0.1.1/flightanalysis/aircraft_analysis.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:41:56.959435 flightanalysis-0.1.1/flightanalysis/base/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       65 2023-03-28 15:54:19.000000 flightanalysis-0.1.1/flightanalysis/base/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2565 2023-06-05 21:18:21.000000 flightanalysis-0.1.1/flightanalysis/base/collection.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2178 2023-06-13 10:36:02.000000 flightanalysis-0.1.1/flightanalysis/base/constructs.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      221 2023-03-28 15:54:19.000000 flightanalysis-0.1.1/flightanalysis/base/numpy_encoder.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     5286 2023-06-13 11:47:30.000000 flightanalysis-0.1.1/flightanalysis/base/table.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1693 2023-06-05 21:18:21.000000 flightanalysis-0.1.1/flightanalysis/controls.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:41:56.963435 flightanalysis-0.1.1/flightanalysis/criteria/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1454 2023-03-28 15:54:19.000000 flightanalysis-0.1.1/flightanalysis/criteria/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2350 2023-03-28 15:54:19.000000 flightanalysis-0.1.1/flightanalysis/criteria/combination.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1324 2023-03-28 15:54:19.000000 flightanalysis-0.1.1/flightanalysis/criteria/comparison.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2013 2023-03-28 15:54:19.000000 flightanalysis-0.1.1/flightanalysis/criteria/continuous.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      925 2023-03-28 15:54:19.000000 flightanalysis-0.1.1/flightanalysis/criteria/results.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1341 2023-06-05 21:18:21.000000 flightanalysis-0.1.1/flightanalysis/criteria/single.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:41:56.963435 flightanalysis-0.1.1/flightanalysis/data/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      279 2023-06-05 21:18:21.000000 flightanalysis-0.1.1/flightanalysis/data/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)    10183 2023-06-05 21:18:21.000000 flightanalysis-0.1.1/flightanalysis/data/f25.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     8236 2023-06-06 04:46:01.000000 flightanalysis-0.1.1/flightanalysis/data/p23.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     8471 2023-06-05 21:18:21.000000 flightanalysis-0.1.1/flightanalysis/data/p25.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:41:56.963435 flightanalysis-0.1.1/flightanalysis/environment/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       91 2023-03-28 15:54:19.000000 flightanalysis-0.1.1/flightanalysis/environment/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1393 2023-06-05 21:18:21.000000 flightanalysis-0.1.1/flightanalysis/environment/environment.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4345 2023-03-28 15:54:19.000000 flightanalysis-0.1.1/flightanalysis/environment/wind.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      466 2023-06-13 14:30:47.000000 flightanalysis-0.1.1/flightanalysis/fc_json.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4167 2023-06-14 09:22:45.000000 flightanalysis-0.1.1/flightanalysis/fc_score.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     7725 2023-06-05 21:18:18.000000 flightanalysis-0.1.1/flightanalysis/flightline.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:41:56.963435 flightanalysis-0.1.1/flightanalysis/model/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      108 2023-03-28 15:54:19.000000 flightanalysis-0.1.1/flightanalysis/model/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1179 2023-06-05 21:18:21.000000 flightanalysis-0.1.1/flightanalysis/model/coefficients.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      405 2023-03-28 15:54:19.000000 flightanalysis-0.1.1/flightanalysis/model/constants.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1377 2023-06-05 21:18:21.000000 flightanalysis-0.1.1/flightanalysis/model/flow.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      675 2023-03-28 15:54:19.000000 flightanalysis-0.1.1/flightanalysis/model/model.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:41:56.963435 flightanalysis-0.1.1/flightanalysis/schedule/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2888 2023-06-13 12:22:27.000000 flightanalysis-0.1.1/flightanalysis/schedule/__init__.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:41:56.967435 flightanalysis-0.1.1/flightanalysis/schedule/definition/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      695 2023-06-05 21:18:21.000000 flightanalysis-0.1.1/flightanalysis/schedule/definition/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1482 2023-06-06 05:23:48.000000 flightanalysis-0.1.1/flightanalysis/schedule/definition/collectors.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     6382 2023-06-13 08:53:43.000000 flightanalysis-0.1.1/flightanalysis/schedule/definition/element_builders.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4907 2023-06-05 21:18:21.000000 flightanalysis-0.1.1/flightanalysis/schedule/definition/element_definition.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4658 2023-06-14 07:40:53.000000 flightanalysis-0.1.1/flightanalysis/schedule/definition/manoeuvre_builder.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     5202 2023-06-13 12:23:31.000000 flightanalysis-0.1.1/flightanalysis/schedule/definition/manoeuvre_definition.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4126 2023-06-05 21:18:21.000000 flightanalysis-0.1.1/flightanalysis/schedule/definition/manoeuvre_info.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     6220 2023-06-13 12:59:23.000000 flightanalysis-0.1.1/flightanalysis/schedule/definition/manoeuvre_parameters.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     7430 2023-06-06 05:26:36.000000 flightanalysis-0.1.1/flightanalysis/schedule/definition/operation.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1949 2023-06-13 12:24:01.000000 flightanalysis-0.1.1/flightanalysis/schedule/definition/schedule_definition.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:41:56.967435 flightanalysis-0.1.1/flightanalysis/schedule/elements/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     7335 2023-06-13 12:21:00.000000 flightanalysis-0.1.1/flightanalysis/schedule/elements/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1749 2023-06-13 12:17:45.000000 flightanalysis-0.1.1/flightanalysis/schedule/elements/autorotation.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     3397 2023-06-13 12:16:23.000000 flightanalysis-0.1.1/flightanalysis/schedule/elements/line.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     6341 2023-06-13 12:18:07.000000 flightanalysis-0.1.1/flightanalysis/schedule/elements/loop.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1844 2023-06-13 12:18:45.000000 flightanalysis-0.1.1/flightanalysis/schedule/elements/nose_drop.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1357 2023-06-13 12:19:01.000000 flightanalysis-0.1.1/flightanalysis/schedule/elements/pitch_break.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1109 2023-06-13 12:19:11.000000 flightanalysis-0.1.1/flightanalysis/schedule/elements/recovery.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1685 2023-06-13 12:21:37.000000 flightanalysis-0.1.1/flightanalysis/schedule/elements/stall_turn.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     3929 2023-06-13 12:27:56.000000 flightanalysis-0.1.1/flightanalysis/schedule/manoeuvre.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4507 2023-06-05 21:18:21.000000 flightanalysis-0.1.1/flightanalysis/schedule/schedule.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      891 2023-03-28 15:54:19.000000 flightanalysis-0.1.1/flightanalysis/simulation.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:41:56.967435 flightanalysis-0.1.1/flightanalysis/state/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1689 2023-06-14 08:27:10.000000 flightanalysis-0.1.1/flightanalysis/state/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2611 2023-06-05 21:18:21.000000 flightanalysis-0.1.1/flightanalysis/state/state.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:41:56.967435 flightanalysis-0.1.1/flightanalysis/state/tools/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)        1 2023-03-28 15:54:19.000000 flightanalysis-0.1.1/flightanalysis/state/tools/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4570 2023-06-14 09:02:25.000000 flightanalysis-0.1.1/flightanalysis/state/tools/alignment.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4450 2023-06-05 21:18:21.000000 flightanalysis-0.1.1/flightanalysis/state/tools/builders.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2722 2023-03-28 15:54:19.000000 flightanalysis-0.1.1/flightanalysis/state/tools/conversions.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     3635 2023-06-05 21:18:21.000000 flightanalysis-0.1.1/flightanalysis/state/tools/dumpers.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      931 2023-06-05 21:18:21.000000 flightanalysis-0.1.1/flightanalysis/state/tools/measurements.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2966 2023-06-05 21:18:21.000000 flightanalysis-0.1.1/flightanalysis/state/tools/transformers.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:41:56.959435 flightanalysis-0.1.1/flightanalysis.egg-info/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1443 2023-06-14 09:41:56.000000 flightanalysis-0.1.1/flightanalysis.egg-info/PKG-INFO
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2675 2023-06-14 09:41:56.000000 flightanalysis-0.1.1/flightanalysis.egg-info/SOURCES.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)        1 2023-06-14 09:41:56.000000 flightanalysis-0.1.1/flightanalysis.egg-info/dependency_links.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       49 2023-06-14 09:41:56.000000 flightanalysis-0.1.1/flightanalysis.egg-info/requires.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       15 2023-06-14 09:41:56.000000 flightanalysis-0.1.1/flightanalysis.egg-info/top_level.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      418 2023-06-14 09:41:56.971436 flightanalysis-0.1.1/setup.cfg
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      672 2023-03-28 15:54:19.000000 flightanalysis-0.1.1/setup.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:41:56.971436 flightanalysis-0.1.1/tests/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      215 2023-03-28 15:54:19.000000 flightanalysis-0.1.1/tests/test_analysis.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      402 2023-03-28 15:54:19.000000 flightanalysis-0.1.1/tests/test_controls.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      206 2023-03-28 15:54:19.000000 flightanalysis-0.1.1/tests/test_data.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2268 2023-03-28 15:54:19.000000 flightanalysis-0.1.1/tests/test_fc_json.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     6855 2023-06-05 21:18:18.000000 flightanalysis-0.1.1/tests/test_flightline.py
```

### Comparing `flightanalysis-0.1.0/LICENSE` & `flightanalysis-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.0/PKG-INFO` & `flightanalysis-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: flightanalysis
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for analysing flight data
 Home-page: https://github.com/PyFlightCoach/FlightAnalysis
 Author: Thomas David
 Author-email: thomasdavid0@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FlightAnalysis
 
-This package contains tools for analysing flight log data. It is based around the State and Section objects, which handle state information for an instant and a section of time. It also contains tools for constructing template Section and State instances based on serialised aerobatic manoeuvre definitions. Temporal alignments can be performed to automatically label flight data based on these templates. New scaled templates can then be constructed based on measurements taken of the labelled elements. 
+This package contains tools for analysing flight log data. 
 
 The Main Idea
 1. Read the sequence defintion from the serialisation of it (currently schedule/p_21.py)
 2. Read, trim and rotate flight recorded flight data
 3. generate a roughly scaled template sequence
 4. run a dynamic time warping algorithm to align the flight to the template
 5. generate scaled templates based on the rules and the flown manoeuvre
@@ -24,17 +24,12 @@
 - Estimate winds from flight data without airspeed sensor. see examples/wind.ipynb
 - Construct a FD model from the flight data with MLP regression or something.
 - The templates are constructed in some kind of 'Judging' axis, similar to the aircraft wind axis but with atmospheric wind removed. Consider accounting for some aerodynamic characteristics here and constructing templates at some alpha and beta.
 - Compare logged control inputs to ideal control inputs calculated using the templates and the FDmodel.
 
 
 # External Dependencies:
-python (3.6+?)
-numpy
-pandas
 scipy
 fastdtw
-
-## This package also depends on other PyFlightCoach packages:
 ardupilot_log_reader
 flightdata
-geometry
+pfc-geometry
```

### Comparing `flightanalysis-0.1.0/README.md` & `flightanalysis-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # FlightAnalysis
 
-This package contains tools for analysing flight log data. It is based around the State and Section objects, which handle state information for an instant and a section of time. It also contains tools for constructing template Section and State instances based on serialised aerobatic manoeuvre definitions. Temporal alignments can be performed to automatically label flight data based on these templates. New scaled templates can then be constructed based on measurements taken of the labelled elements. 
+This package contains tools for analysing flight log data. 
 
 The Main Idea
 1. Read the sequence defintion from the serialisation of it (currently schedule/p_21.py)
 2. Read, trim and rotate flight recorded flight data
 3. generate a roughly scaled template sequence
 4. run a dynamic time warping algorithm to align the flight to the template
 5. generate scaled templates based on the rules and the flown manoeuvre
@@ -14,17 +14,12 @@
 - Estimate winds from flight data without airspeed sensor. see examples/wind.ipynb
 - Construct a FD model from the flight data with MLP regression or something.
 - The templates are constructed in some kind of 'Judging' axis, similar to the aircraft wind axis but with atmospheric wind removed. Consider accounting for some aerodynamic characteristics here and constructing templates at some alpha and beta.
 - Compare logged control inputs to ideal control inputs calculated using the templates and the FDmodel.
 
 
 # External Dependencies:
-python (3.6+?)
-numpy
-pandas
 scipy
 fastdtw
-
-## This package also depends on other PyFlightCoach packages:
 ardupilot_log_reader
 flightdata
-geometry
+pfc-geometry
```

### Comparing `flightanalysis-0.1.0/flightanalysis/aircraft_analysis.py` & `flightanalysis-0.1.1/flightanalysis/aircraft_analysis.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.0/flightanalysis/base/collection.py` & `flightanalysis-0.1.1/flightanalysis/base/collection.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from typing import Dict, List, Union, Any
+import numpy as np
+import pandas as pd
 
 
 class Collection:
     VType = None
     uid = "uid"
     def __init__(self, data: Union[Dict[str,Any], List[Any]]=None):
         if data is None:
@@ -14,18 +16,21 @@
     def __getattr__(self, name):
         if name in self.data:
             return self.data[name]
 
     def __getitem__(self, key: Union[int, str]):
         if isinstance(key, int): 
             return list(self.data.values())[key]
+        elif isinstance(key, slice):
+            return self.__class__(list(self.data.values())[key])
         elif isinstance(key, str):
             return self.data[key]
         elif isinstance(key, self.__class__.VType):
             return self.data[getattr(key, self.__class__.uid)]
+        raise ValueError(f"Invalid Key or Indexer {key}")
 
     def __iter__(self):
         for v in self.data.values():
             yield v
 
     def to_list(self):
         return list(self.data.values())
@@ -41,18 +46,34 @@
         return cls([cls.VType.from_dict(**v) for v in vals])    
 
     @classmethod
     def from_dict(cls, vals: Dict[str, dict]):
         return cls([cls.VType.from_dict(v) for v in vals.values()])
     
     def add(self, v):
-        self.data[getattr(v, self.uid)] = v
+        if v is None:
+            return self
+        elif isinstance(v, self.VType):
+            self.data[getattr(v, self.uid)] = v
+        elif isinstance(v, self.__class__):
+            return self.__class__(dict(**self.data, **v.data))
         return v
 
     def next_free_name(self, prefix: str):
         i=0
         while f"{prefix}{i}" in self.data:
             i+=1
         else:
             return f"{prefix}{i}"
 
-    
+    def copy(self):
+        return self.__class__([v.copy() for v in self])
+    
+    def __str__(self) -> str:
+        return str(pd.Series({k: str(v) for k, v in self.data.items()}))
+    
+    def __repr__(self) -> str:
+        contents = str(pd.Series({k: repr(v) for k, v in self.data.items()}))
+        return f"{self.__class__.__name__}\n{contents}"
+    
+    def __len__(self) -> int:
+        return len(self.data)
```

### Comparing `flightanalysis-0.1.0/flightanalysis/base/constructs.py` & `flightanalysis-0.1.1/flightanalysis/base/constructs.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,28 +7,27 @@
     bvel = velocity in (body frame)
     rvel = rotational velocity (body axis rates)
 
     """
 import numpy as np
 import pandas as pd
 from typing import List, Dict, Union
-
-
+from .collection import Collection
+from itertools import chain
 class SVar:
-    def __init__(self, obj, keys=None, builder=None):
+    def __init__(self, name, obj, keys=None, builder=None):
+        self.name = name
         self.obj = obj
         self.keys = obj.cols if keys is None else keys
         self.builder = builder
 
 
-class Constructs:
-    def __init__(self, data: Dict[str, SVar]):
-        self.data = data
-        self.cols = [name for sv in self.data.values() for name in sv.keys]
-
+class Constructs(Collection):
+    VType=SVar
+    uid = "name"
     def subset(self, names: List[str]):
         """get a subset of the constructs"""
         return Constructs({key: value for key, value in self.data.items() if key in names})
 
     def existing(self, vars: List[str]):
         """return a subset that is fully populated by the list of keys input"""
         return self.subset([
@@ -39,17 +38,14 @@
     def missing(self, vars: List[str]):
         """return a subset that has not been populated by the list of vars"""
         return self.subset([
             key for key, value in self.data.items() 
             if not all(val in vars for val in value.keys)
         ])
 
-    def to_list(self):
-        return list(self.data.values())
-
     def contains(self, names: Union[list, str]) -> bool:
         _names = [names] if isinstance(names, str) else names
         
         keys = self.data.keys()
         res = [name in keys for name in _names]
         return res[0] if isinstance(names, str) else res
 
@@ -58,7 +54,10 @@
 
     def __add__(self, other):
         return Constructs(dict(**self.data, **other.data))
 
     def __iter__(self):
         for val in self.data.values():
             yield val
+
+    def cols(self):
+        return chain(*[c.keys for c in self.data.values()])
```

### Comparing `flightanalysis-0.1.0/flightanalysis/base/table.py` & `flightanalysis-0.1.1/flightanalysis/base/table.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,54 @@
+from __future__ import annotations
 import numpy as np
 import pandas as pd
 
 from geometry import Base,  Point, Quaternion, Transformation
 from typing import Union, Dict
 from .constructs import SVar, Constructs
 from numbers import Number
-
+from time import time
 
 class Time(Base):
     cols=["t", "dt"]
     
     @staticmethod
     def from_t(t: np.ndarray):
         if isinstance(t, Number):
             return Time(t, 1/30)
         else:
             dt = np.array([1/30]) if len(t) == 1 else np.gradient(t)
             return Time(t, dt)
 
+    def scale(self, duration):
+        old_duration = self.t[-1] - self.t[0]
+        sfac = duration / old_duration
+        return Time(
+            self.t[0] + (self.t - self.t[0]) * sfac,
+            self.dt * sfac
+        )
+
+    def reset_zero(self):
+        return Time(self.t - self.t[0], self.dt)
+
+    @staticmethod
+    def now():
+        return Time.from_t(time())
+
+    def extend(self):
+        return Time.concatenate([self, Time(self.t[-1] + self.dt[-1], self.dt[-1])])
+
 
 def make_time(tab):
     return Time.from_t(tab.t)
     
 class Table:
-    constructs = Constructs(dict(
-        time = SVar(Time,        ["t", "dt"]               , make_time )
-    ))
+    constructs = Constructs([
+         SVar("time", Time,        ["t", "dt"]               , make_time )
+    ])
 
     def __init__(self, data: pd.DataFrame, fill=True):
         if len(data) == 0:
             raise Exception("Created with empty dataframe")
             
         self.data = data
 
@@ -75,39 +94,44 @@
 
             return self.__class__(
                 self.data.iloc[self.data.index.get_indexer([sli], method="nearest"), :]
             )
         
         return self.__class__(self.data.loc[sli])
 
+    def slice_raw_t(self, sli):
+        inds = self.data.reset_index().set_index("t")["index"].loc[sli].to_numpy()#set_index("t", drop=False).columns
 
+        return self.__class__(self.data.loc[inds])
+        
     def __iter__(self):
         for ind in list(self.data.index):
             yield self[ind]
 
     @classmethod
     def from_constructs(cls, *args,**kwargs):
         kwargs = dict(
             **{list(cls.constructs.data.keys())[i]: arg for i, arg in enumerate(args)},
             **kwargs
         )
 
         df = pd.concat(
             [
                 x.to_pandas(
-                    columns=cls.constructs.data[key].keys, 
+                    columns=cls.constructs[key].keys, 
                     index=kwargs["time"].t
                 ) for key, x in kwargs.items() if not x is None
             ],
             axis=1
         )
 
         return cls(df)
 
-
+    def __repr__(self):
+        return f"{self.__class__.__name__} Table, duration = {self.duration}\n{self.data}"
 
 
     def copy(self, *args,**kwargs):
         kwargs = dict(kwargs, **{list(self.constructs.data.keys())[i]: arg for i, arg in enumerate(args)}) # add the args to the kwargs
 
         old_constructs = {key: self.__getattr__(key) for key in self.constructs.existing(self.data.columns).data if not key in kwargs}
         
@@ -118,14 +142,33 @@
 
     def label(self, **kwargs):
         return self.__class__(self.data.assign(**kwargs))
 
     def remove_labels(self):
         return self.__class__(
             self.data.drop(
-                [c for c in self.data.columns if not c in self.constructs.cols], 
-                1, 
+                [c for c in self.data.columns if not c in self.constructs.cols()], 
+                axis=1, 
                 errors="ignore"
             )
         )
     
 
+    def append(self, other, timeoption:str="dt"):
+
+        if timeoption in ["now", "t"]:
+            t = np.array([time()]) if timeoption == "now" else other.t
+            dt = other.dt
+            dt[0] = t[0] - self.t[-1]
+            new_time = Time(t, dt)
+        elif timeoption == "dt":
+            new_time = Time(other.t + self[-1].t - other[0].t + other[0].dt, other.dt)
+
+        return self.__class__(pd.concat(
+            [
+                self.data, 
+                other.copy(new_time).data
+            ], 
+            axis=0, 
+            ignore_index=True
+        ).set_index("t", drop=False))
+
```

### Comparing `flightanalysis-0.1.0/flightanalysis/controls.py` & `flightanalysis-0.1.1/flightanalysis/controls.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,18 +24,18 @@
             chans.e,
             chans.r,
             np.mean([chans.a1, chans.a2]),
         )
 
 
 class Controls(Table):
-    constructs = Table.constructs + Constructs(dict(
-        surfaces = SVar(Surfaces),
-        channels = SVar(Channels)
-    ))
+    constructs = Table.constructs + Constructs([
+        SVar("surfaces", Surfaces),
+        SVar("channels", Channels)
+    ])
 
 
     def build(flight: Union[Flight, str], conversion):
         if isinstance(flight, str):
             flight = {
                 ".csv": Flight.from_csv,
                 ".BIN": Flight.from_log
```

### Comparing `flightanalysis-0.1.0/flightanalysis/criteria/__init__.py` & `flightanalysis-0.1.1/flightanalysis/criteria/__init__.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.0/flightanalysis/criteria/combination.py` & `flightanalysis-0.1.1/flightanalysis/criteria/combination.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.0/flightanalysis/criteria/comparison.py` & `flightanalysis-0.1.1/flightanalysis/criteria/comparison.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.0/flightanalysis/criteria/continuous.py` & `flightanalysis-0.1.1/flightanalysis/criteria/continuous.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.0/flightanalysis/criteria/results.py` & `flightanalysis-0.1.1/flightanalysis/criteria/results.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.0/flightanalysis/criteria/single.py` & `flightanalysis-0.1.1/flightanalysis/criteria/single.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,8 +30,10 @@
             kind = self.__class__.__name__,
             lookup = inspect.getsourcelines(self.criteria)[0][0].split("=")[1].strip(),
             preprocess = inspect.getsourcelines(self.criteria)[0][0].split("=")[1].strip()
         )
 
     @staticmethod
     def from_dict(data:dict):
-        return Single(eval(data["lookup"]),eval(data["preprocess"]))
+        return Single(eval(data["lookup"]),eval(data["preprocess"]))
+    
+
```

### Comparing `flightanalysis-0.1.0/flightanalysis/environment/environment.py` & `flightanalysis-0.1.1/flightanalysis/environment/environment.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,18 +26,18 @@
     @staticmethod
     def iso_sea_level(length: int):
         return Air(101325, 288.15, get_rho(101325, 288.15)).tile(length)
 
 
 
 class Environment(Table):
-    constructs = Table.constructs + Constructs(dict(
-        atm = SVar(Air, ["P", "T", "rho"], lambda tab: Air.iso_sea_level(len(tab))),
-        wind = SVar(Point, ["wvx", "wvy", "wvz"], lambda tab: P0(len(tab)))
-    ))
+    constructs = Table.constructs + Constructs([
+        SVar("atm", Air, ["P", "T", "rho"], lambda tab: Air.iso_sea_level(len(tab))),
+        SVar("wind", Point, ["wvx", "wvy", "wvz"], lambda tab: P0(len(tab)))
+    ])
 
     @staticmethod
     def build(flight: Flight, sec: State, wmodel: WindModel):
 
         df = flight.read_fields(Fields.PRESSURE)
         df = df.assign(temperature_0=291.15)
         df = df.assign(rho=get_rho(df["pressure_0"], df["temperature_0"]))
```

### Comparing `flightanalysis-0.1.0/flightanalysis/environment/wind.py` & `flightanalysis-0.1.1/flightanalysis/environment/wind.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.0/flightanalysis/flightline.py` & `flightanalysis-0.1.1/flightanalysis/flightline.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 This program is distributed in the hope that it will be useful, but WITHOUT
 ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 You should have received a copy of the GNU General Public License along with
 this program. If not, see <http://www.gnu.org/licenses/>.
 """
 
-from geometry import GPS, Coord, Point, Transformation, Quaternion, PX, PY, PZ, P0
+from geometry import GPS, Coord, Point, Transformation, Quaternion, PX, PY, PZ, P0, Euler
 from typing import Union
 from flightdata import Flight, Fields
 import numpy as np
 from json import load, dump
 
 
 class Box(object):
@@ -23,16 +23,15 @@
 
     def __init__(self, name, pilot_position: GPS, heading: float, club:str=None, country:str=None):
         self.name = name
         self.club=club
         self.country=country
         self.pilot_position = pilot_position
         self.heading = heading
-
-
+        self.rotation = Euler(0, 0, -self.heading)
 
     def to_dict(self) -> dict:
         temp = self.__dict__.copy()
         temp["pilot_position"] = self.pilot_position.to_dict()
         return temp
 
     @staticmethod
@@ -61,19 +60,18 @@
     def from_initial(flight: Flight):
         '''Generate a box based on the initial position and heading of the model at the start of the log. 
         This is a convenient, but not very accurate way to setup the box. 
         '''
         imu_ready_data = flight.data.loc[flight.imu_ready_time()]
 
         position = GPS(*imu_ready_data[Fields.GLOBALPOSITION.names])
-        heading = Quaternion(
-            *imu_ready_data[Fields.QUATERNION.names]
+        heading = Euler(
+            *imu_ready_data[Fields.ATTITUDE.names]
         ).transform_point(PX())
-        
-        
+
         return Box('origin', position[0], np.arctan2(heading.y, heading.x)[0], "unknown", "unknown")
 
     @staticmethod
     def from_points(name, pilot: GPS, centre: GPS):
         direction = centre - pilot
         return Box(
             name,
@@ -118,14 +116,23 @@
         return Box.from_points(
             "FCJ_box",
             GPS(float(data['pilotLat']), float(data['pilotLng'])),
             GPS(float(data['centerLat']), float(data['centerLng']))
         )
 
 
+    def gps_to_point(self, gps: GPS) -> Point:
+        pned = gps - self.pilot_position
+        return self.rotation.transform_point(Point(pned.y, pned.x, -pned.z ))
+
+
+#    def point_to_gps(self, pos: Point) -> GPS:
+ #       return self.pilot_position + self.rotation.inverse().transform_point(pos)
+    
+
 class FlightLine(object):
     '''class to define where the flight line is in relation to the raw input data
     It contains two coordinate frames (generally used for reference / debugging only) and two transformations, 
     which will take geometry to and from these reference frames.  
 
     '''
 
@@ -143,14 +150,19 @@
         self.world = world
         self.contest = contest
         self.transform_to = Transformation.from_coords(contest, world)
         self.transform_from = Transformation.build(-self.transform_to.translation,
                                              self.transform_to.rotation.conjugate())
 
     @staticmethod
+    def home():
+        """Default home is NWU"""
+        return FlightLine(Coord.from_nothing(), Coord.from_zx(P0(), PZ(-1), PX()))
+
+    @staticmethod
     def from_box(box: Box, world_home: GPS):
         """Constructor from a Box instance. This method assumes the input data is in the 
         Ardupilot default World frame (NED). It creates the contest frame from the box as described in __init__, 
         ie z up, y in the box heading direction. 
 
         Args:
             box (Box): box defining the contest coord
```

### Comparing `flightanalysis-0.1.0/flightanalysis/model/coefficients.py` & `flightanalysis-0.1.1/flightanalysis/model/coefficients.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 import numpy as np
 from flightanalysis.state import State
 from flightanalysis.model.flow import Flow
 from flightanalysis.model.constants import ACConstants
 
 
 class Coefficients(Table):
-    constructs = Table.constructs + Constructs(dict(
-        force = SVar(Point, ["cx", "cy", "cz"], None),
-        moment = SVar(Point, ["cl", "cm", "cn"], None)
-    ))
+    constructs = Table.constructs + Constructs([
+        SVar("force", Point, ["cx", "cy", "cz"], None),
+        SVar("moment", Point, ["cl", "cm", "cn"], None)
+    ])
 
     @staticmethod
     def build(sec: State, flow: Flow, consts: ACConstants):
         I = consts.inertia
         u = sec.vel
         du = sec.acc
         w = sec.rvel
```

### Comparing `flightanalysis-0.1.0/flightanalysis/model/flow.py` & `flightanalysis-0.1.1/flightanalysis/model/flow.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 
 
 class Attack(Base):
     cols = ['alpha', 'beta', 'q']
 
 
 class Flow(Table):
-    constructs = Table.constructs + Constructs(dict(
-        aspd = SVar(Point, ["asx", "asy", "asz"], None),
-        flow = SVar(Point, ["alpha", "beta", "q"], None)
-    ))
+    constructs = Table.constructs + Constructs([
+        SVar("aspd", Point, ["asx", "asy", "asz"], None),
+        SVar("flow", Point, ["alpha", "beta", "q"], None)
+    ])
 
     @staticmethod
     def build(body: State, env: Environment):
 #        wind = judge.judging_to_wind(env.wind)
         airspeed = body.vel - body.att.inverse().transform_point(env.wind)
 
         np.seterr(invalid='ignore')
```

### Comparing `flightanalysis-0.1.0/flightanalysis/model/model.py` & `flightanalysis-0.1.1/flightanalysis/model/model.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.0/flightanalysis/schedule/__init__.py` & `flightanalysis-0.1.1/flightanalysis/schedule/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,11 +57,11 @@
 Inter Element Judging Process
 To be described later but it is already implemented in the ManDef
 
 """
 
 
 
-from .elements import Loop, Line, Snap, Spin, StallTurn
+from .elements import Loop, Line, StallTurn, NoseDrop, PitchBreak, Recovery, Autorotation
 from .manoeuvre import Manoeuvre
 from .schedule import Schedule
 from .definition import *
```

### Comparing `flightanalysis-0.1.0/flightanalysis/schedule/definition/__init__.py` & `flightanalysis-0.1.1/flightanalysis/schedule/definition/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Callable
 from numbers import Number
 
 from .operation import Opp, MathOpp, FunOpp, ItemOpp
 from .manoeuvre_info import ManInfo, BoxLocation, Orientation, Direction, Height, Position
 from .collectors import Collector, Collectors
 
-from .manoeuvre_parameters import ManParm, ManParms, MPValue
+from .manoeuvre_parameters import ManParm, ManParms
 
 def _a(arg):
     if isinstance(arg, ManParm):
         return arg.valuefunc()
     elif isinstance(arg, Number):
         return lambda mps: arg
     elif isinstance(arg, Opp):
@@ -20,7 +20,8 @@
 from .element_definition import ElDef, ElDefs
 
 from .manoeuvre_definition import ManDef
 
 from .schedule_definition import SchedDef
 
 
+from .manoeuvre_builder import ManoeuvreBuilder, f3amb, MBTags
```

### Comparing `flightanalysis-0.1.0/flightanalysis/schedule/definition/collectors.py` & `flightanalysis-0.1.1/flightanalysis/schedule/definition/collectors.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,28 +14,33 @@
         """return the value"""
         return els.get_parameter_from_element(self.elname, self.pname)
 
     def __str__(self):
         return self.name
 
     @staticmethod
-    def parse(ins, coll: Collection):
-        try:
-            return Opp.parse(ins, coll)
-        except KeyError:
-            return Collector(*ins.strip(" ").split("."))
+    def parse(ins):
+        return Opp.parse_f(
+            ins, 
+            lambda ins : Collector(*ins.strip(" ").split("."))
+        )
+        
 
     def to_dict(self):
         return dict(
             elname=self.elname,
             pname=self.pname
         )
 
+    def copy(self):
+        return Collector(self.elname, self.pname)
+
+
 class Collectors(Collection):
-    VType=Collector
+    VType=Opp
     uid="name"
 
     def __str__(self):
         return str([str(v) for v in self])
     
     @staticmethod
     def parse(ins: str):
@@ -48,9 +53,10 @@
     def to_list(self):
         return [str(v) for v in self]
     
     @staticmethod
     def from_list(data):
         coll = Collectors()
         for d in data:
-            coll.add(Collector.parse(d, coll))
-        return coll
+            coll.add(Collector.parse(d))
+        return coll
+
```

### Comparing `flightanalysis-0.1.0/flightanalysis/schedule/definition/manoeuvre_info.py` & `flightanalysis-0.1.1/flightanalysis/schedule/definition/manoeuvre_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,22 +97,24 @@
         self, 
         name:str, 
         short_name:str, 
         k:float, 
         position: Position,
         start: BoxLocation, 
         end: BoxLocation,
+        centre_loc: int = -1, # -1 for standard definitino, >=0 for the start of an element ID
     ):
 
         self.name = name
         self.short_name = short_name
         self.k = k
         self.position=position
         self.start = start
         self.end = end
+        self.centre_loc = centre_loc
 
 
     def initial_position(self, depth: float, wind: int) -> Transformation: 
         return Point(
             {
                 Position.CENTRE: wind * {
                     Direction.UPWIND: depth * np.tan(np.radians(60)),
```

### Comparing `flightanalysis-0.1.0/flightanalysis/schedule/definition/manoeuvre_parameters.py` & `flightanalysis-0.1.1/flightanalysis/schedule/definition/manoeuvre_parameters.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import enum
 from typing import List, Dict, Callable, Union
 import numpy as np
 import pandas as pd
 from numbers import Number
-from flightanalysis.schedule.elements import Loop, Line, Snap, Spin, StallTurn, El, Elements
 from flightanalysis.schedule.manoeuvre import Manoeuvre
 from flightanalysis.criteria import *
 from flightanalysis import State
 from functools import partial
 from flightanalysis.base.collection import Collection
 from numbers import Number
 from . import Collector, Collectors, MathOpp, FunOpp, ItemOpp, Opp
 
 
 
 class ManParm(Opp):
     """This class represents a parameter that can be used to characterise the geometry of a manoeuvre.
     For example, the loop diameters, line lengths, roll direction. 
+    
+    TODO: I think the way this uses the base class is nonsensical - ManParm.parse returns an Opp, not a ManParm.
+    perhaps a manparm should parse args and kwargs to the opp, or something like that.
     """
     def __init__(
         self, 
         name:str, 
         criteria: Union[Single, Comparison, Combination], 
         default=None, 
         collectors:Collectors=None
@@ -31,22 +33,22 @@
             name (str): a short name, must work as an attribute so no spaces or funny characters
             criteria (Comparison): The comparison criteria function to be used when judging this parameter
             default (float): A default value (or default option if specified in criteria)
             collectors (Callable): a list of functions that will pull values for this parameter from an Elements 
                 collection. If the manoeuvre was flown correctly these should all be the same. The resulting list 
                 can be passed through the criteria (Comparison callable) to calculate a downgrade.
         """
-        self.name=name
         self.criteria = criteria
         self.default = default
-        
-        self.collectors = Collectors() if collectors is None else collectors
-        assert isinstance(self.collectors,Collectors)
+        self.collectors = collectors
+        if self.collectors is None:
+            self.collectors = Collectors()
         self.n = len(self.criteria.desired[0]) if isinstance(self.criteria, Combination) else None
-
+        super().__init__(name)
+        
     def to_dict(self):
         return dict(
             name = self.name,
             criteria = self.criteria.to_dict(),
             default = self.default,
             collectors = self.collectors.to_list()
         )
@@ -65,14 +67,17 @@
             self.collectors.add(collector)    
         elif isinstance(collector, Collectors):
             for coll in collector:
                 self.append(coll)
         else:
             raise ValueError(f"expected a Collector or Collectors not {collector.__class__.__name__}")
 
+    def assign(self, id, collector):
+        self.collectors.data[id] = collector
+
     def collect(self, els):
         return np.array([collector(els) for collector in self.collectors])
 
     def get_downgrades(self, els):
         return self.criteria(self.name, self.collect(els))
 
     @property
@@ -101,14 +106,19 @@
             return lambda mps: mps.data[self.name].value[id] 
         else:
             raise Exception("Cant create a valuefunc in this case")
     
     def __getitem__(self, i):
         return ItemOpp(self, i)
 
+    def copy(self):
+        return ManParm(self.name, self.criteria, self.default, self.collectors.copy())
+
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}({str(self)} = {self.value})"
 
 
 class ManParms(Collection):
     VType=ManParm
     uid="name"
 
     def collect(self, manoeuvre: Manoeuvre) -> Dict[str, float]:
@@ -127,55 +137,28 @@
 
         Args:
             colls (Dict[str, Callable]): dict of parmname: collector method
         """
         for mp, col in colls.items():
             self.data[mp].append(col)
 
-    @staticmethod
-    def create_defaults_f3a(**kwargs):
-        mps = ManParms([
-            ManParm("speed", inter_f3a_speed, 30.0),
-            ManParm("loop_radius", inter_f3a_radius, 55.0),
-            ManParm("line_length", inter_f3a_length, 130.0),
-            ManParm("point_length", inter_f3a_length, 10.0),
-            ManParm("continuous_roll_rate", inter_f3a_roll_rate, np.pi/2),
-            ManParm("partial_roll_rate", inter_f3a_roll_rate, np.pi/2),
-            ManParm("snap_rate", inter_f3a_roll_rate, 4*np.pi),
-            ManParm("stallturn_rate", inter_f3a_roll_rate, 2*np.pi),
-            ManParm("spin_rate", inter_f3a_roll_rate, 2*np.pi),
-        ])
-        for k,v in kwargs.items():
-            if isinstance(v, Number):
-                mps.data[k].default = v
-            elif isinstance(v, ManParm):
-                mps.data[k] = v
-        return mps
 
     def update_defaults(self, intended: Manoeuvre):
         """Pull the parameters from a manoeuvre object and update the defaults of self based on the result of 
         the collectors.
 
         Args:
-            intended (Manoeuvre): Usually a Manoeuvre that has been resized based on an alingned state
+            intended (Manoeuvre): Usually a Manoeuvre that has been resized based on an alinged state
         """
 
         for mp in self:
-            flown_parm = mp.collect(intended.all_elements)
+            flown_parm = mp.collect(intended.all_elements())
             if len(flown_parm) >0:
                 if isinstance(mp.criteria, Combination):
                     default = mp.criteria.check_option(flown_parm)
                 else:
-                    default = np.mean(flown_parm)
+                    default = np.mean(np.abs(flown_parm)) * np.sign(mp.default)
                 mp.default = default
-            
-                
-
-class MPValue:
-    def __init__(self, value, minval, maxval, slope):
-        self.value = value
-        self.minval = minval
-        self.maxval = maxval
-        self.slope = slope
-
 
+    def remove_unused(self):
+        return ManParms([mp for mp in self if len(mp.collectors) > 0])
```

### Comparing `flightanalysis-0.1.0/flightanalysis/schedule/definition/schedule_definition.py` & `flightanalysis-0.1.1/flightanalysis/schedule/definition/schedule_definition.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from . import ManDef, ManInfo, ManParms
 from flightanalysis import State
 from typing import Dict, Tuple
 from geometry import Transformation
 from flightanalysis.schedule.schedule import Schedule
-from flightanalysis.schedule.elements import Line, Loop, Snap, Spin, StallTurn
+from flightanalysis.schedule.elements import Line
 from flightanalysis.base.collection import Collection
 from json import dump, load
 from flightanalysis.base.numpy_encoder import NumpyEncoder
 
 
 class SchedDef(Collection):
     VType=ManDef
```

### Comparing `flightanalysis-0.1.0/flightanalysis/schedule/elements/__init__.py` & `flightanalysis-0.1.1/flightanalysis/schedule/elements/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from telnetlib import DO
 import numpy as np
 import pandas as pd
 from flightanalysis.state import State
 from geometry import Transformation, PX, PY, PZ, Point, angle_diff, Coord
-from json import load
+from json import load, dumps
 from flightanalysis.criteria import *
 from flightanalysis.base.collection import Collection
-
+from flightanalysis.base.table import Time
+from typing import Union
 
 class DownGrade:
     def __init__(self, name, measurement, criteria):
         self.name = name
         self.measurement = measurement
         self.criteria = criteria
 
@@ -27,44 +27,51 @@
 
     def apply(self, el, fl, tp):
         return Results([es.criteria(es.name, es.measure(el, fl, tp), False) for es in self])
        
 
 class El:   
     parameters = ["speed"]
-    
+
     def __init__(self, uid: str, speed: float):        
         self.uid = uid
         if speed < 0:
             raise ValueError("negative speeds are not allowed")
         self.speed = speed
 
     def get_data(self, st: State):
         return st.get_element(self.uid)
 
     def _add_rolls(self, el: State, roll: float) -> State:
         if not roll == 0:
-            el = el.superimpose_roll(roll)
+            el = el.superimpose_rotation(PX(), roll)
         return el.label(element=self.uid)
 
     def __eq__(self, other):
         if not self.__class__ == other.__class__:
             return False
         if not self.uid == other.uid:
             return False
-        return np.all([getattr(parm, self) == other.getattr(parm, other) for parm in self.__class__.parameters])
+        return np.all([np.isclose(getattr(self, p), getattr(other, p), 0.01) for p in self.__class__.parameters])
+
+    def __repr__(self):
+        return dumps(self.to_dict(), indent=2)
 
     def to_dict(self):
         return dict(type=self.__class__.__name__, **self.__dict__)
 
     def set_parms(self, **parms):
-        new_inst = self.__class__(**self.__dict__)
+        kwargs = {k:v for k, v in self.__dict__.items() if not k[0] == "_"}
+
         for key, value in parms.items():
-            setattr(new_inst, key, value)
-        return new_inst
+            if key in kwargs:
+                kwargs[key] = value
+        
+        return self.__class__(**kwargs)
+
 
     def setup_analysis_state(self, flown: State, template:State):
         """Change the reference coordinate frame for a flown element to the
         elements coord"""   
         return flown.move_back(Transformation.from_coord(self.coord(template)))
 
     def measure_end_roll_angle(self, flown: State, template:State):
@@ -129,47 +136,35 @@
         if the x_vector is in the xz plane then the z vector is world y,
         #otherwise the Z vector is world X
         """
         x_vector = template[0].att.transform_point(PX(1))
         z_vector = PY(1.0) if abs(x_vector.y[0]) < 0.1 else PX(1.0)
         return Coord.from_zx(template[0].pos, z_vector, x_vector)
 
+    @staticmethod
+    def create_time(duration: float, time: Time=None):
+        if time is None:
+            n = int(np.ceil(duration * State._construct_freq))
+            return Time.from_t(
+                np.linspace(0, duration, n if n > 1 else n+1))
+        else:
+            #probably want to extend by one timestep
+            return time.reset_zero().scale(duration)
+
     @property
     def exit_scoring(self):
         return DownGrades([
             DownGrade("ip_track", "measure_end_ip_track", basic_angle_f3a),
             DownGrade("op_track", "measure_end_op_track", basic_angle_f3a),
             DownGrade("roll_angle", "measure_end_roll_angle", basic_angle_f3a),
         ])
 
-from .line import Line
-from .loop import Loop
-from .snap import Snap
-from .spin import Spin
-from .stall_turn import StallTurn
-
-els = {c.__name__.lower(): c for c in El.__subclasses__()}
-
-El.from_name = lambda name: els[name.lower()]
-
-def from_dict(data):
-    kind = data.pop("kind")
-    return els[kind](**data)
-
-El.from_dict = staticmethod(from_dict)
-
-def from_json(file):
-    with open(file, "r") as f:
-        return El.from_dict(load(f))
-
-El.from_json = from_json
 
 from flightanalysis.base.collection import Collection
 
-
 class Elements(Collection):
     VType=El
     def get_parameter_from_element(self, element_name: str, parameter_name: str):
         return getattr(self.data[element_name], parameter_name)  
     
     @staticmethod
     def from_dicts(data):
@@ -193,9 +188,33 @@
     def downgrade(self):
         return sum(er.results.downgrade() for er in self)
     
     def downgrade_list(self):
         return [er.results.downgrade() for er in self]
     
 
+from .line import Line
+from .loop import Loop
+from .stall_turn import StallTurn
+from .nose_drop import NoseDrop
+from .pitch_break import PitchBreak
+from .recovery import Recovery
+from .autorotation import Autorotation
+
+els = {c.__name__.lower(): c for c in El.__subclasses__()}
+
+El.from_name = lambda name: els[name.lower()]
+
+def from_dict(data):
+    kind = data.pop("kind")
+    return els[kind](**data)
+
+El.from_dict = staticmethod(from_dict)
+
+def from_json(file):
+    with open(file, "r") as f:
+        return El.from_dict(load(f))
+
+El.from_json = from_json
+
```

### Comparing `flightanalysis-0.1.0/flightanalysis/schedule/elements/line.py` & `flightanalysis-0.1.1/flightanalysis/schedule/elements/line.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 
 import numpy as np
-from geometry import Transformation, Point, PX, PY, PZ, Coord
+from geometry import Transformation, Point, P0, PX, PY, PZ, Coord
 from flightanalysis.base.table import Time
 from flightanalysis.state import State
 from enum import Enum
 from . import El, DownGrades, DownGrade
 from flightanalysis.criteria import *
+from typing import Union
 
 
 class Line(El):
     parameters = El.parameters + "length,roll,rate".split(",")
 
     def __init__(self, speed, length, roll=0, uid:str=None):
         super().__init__(uid, speed)
-        if length < 0:
-            raise ValueError("Cannot create line with negative length")
+#        if length < 0:
+ #           raise ValueError("Cannot create line with negative length")
         self.length = length
         self.roll = roll
     
     @property
     def intra_scoring(self):
         _intra_scoring = DownGrades([
             DownGrade("speed", "measure_speed", intra_f3a_speed),
@@ -41,57 +42,56 @@
 
     def to_dict(self):
         return dict(
             kind=self.__class__.__name__,
             length=self.length,
             roll=self.roll,
             speed=self.speed,
+            rate=self.rate,
             uid=self.uid
         )
 
-    def scale(self, factor):
-        return self.set_parms(length=self.length * factor)
-
     @property
     def rate(self):
-        return abs(self.roll) * self.speed / self.length
+        return self.roll * self.speed / self.length
 
-    def create_template(self, transform: Transformation) -> State:
-        """contstruct a State representing the judging frame for this line element
+    def create_template(self, istate: State, time: Time=None) -> State:
+        """construct a State representing the judging frame for this line element
 
         Args:
-            transform (Transformation): initial position and orientation
+            istate (Transformation): initial position and orientation
             speed (float): speed in judging frame X axis
             simple (bool, optional): just create the first and last points of the section. Defaults to False.
 
         Returns:
             State: [description]
         """
-        sec= State.from_transform(
-            transform, 
-            time = Time(0, 1/State._construct_freq),
-            vel=PX(self.speed)
-        ).extrapolate(duration=self.length / self.speed)
-
-        return self._add_rolls(sec, self.roll)
+        v = PX(self.speed) if istate.vel == 0 else istate.vel.scale(self.speed)
+             
+        return self._add_rolls(
+            istate.copy(vel=v, rvel=P0()).fill(
+                El.create_time(self.length / self.speed, time)
+            ), 
+            self.roll
+        )
 
     def match_axis_rate(self, roll_rate: float):
         # roll rate in radians per second
         if not self.roll == 0.0:
             return self.set_parms(
                 length=abs(self.roll) * self.speed / roll_rate)
         else:
             return self.set_parms()
 
     def match_intention(self, transform: Transformation, flown: State):
         jit = flown.judging_itrans(transform)
         return self.set_parms(
             length=jit.att.inverse().transform_point(flown.pos - jit.pos).x[-1],
             roll=np.sign(np.mean(flown.p)) * abs(self.roll),
-            speed=np.mean(flown.u)
+            speed=abs(flown.vel).mean()
         )
 
     @staticmethod
     def from_roll(speed: float, rate: float, angle: float):
         return Line(speed, rate * angle * speed, angle )
 
     def copy_direction(self, other):
```

### Comparing `flightanalysis-0.1.0/flightanalysis/schedule/elements/loop.py` & `flightanalysis-0.1.1/flightanalysis/schedule/elements/loop.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import pandas as pd
 from geometry import Transformation, Coord, Point, Quaternion, PX, PY, PZ
 from flightanalysis.state import State
 from flightanalysis.base.table import Time
 from scipy import optimize
 from flightanalysis.criteria import *
 from . import El, DownGrades, DownGrade
+from typing import Union
 
 
 class Loop(El):
     parameters = El.parameters + "radius,angle,roll,ke,rate".split(",")
 
     def __init__(self, speed: float, radius: float, angle: float, roll:float=0.0, ke: bool = False, uid: str=None):
         super().__init__(uid, speed)
@@ -55,40 +56,39 @@
     def diameter(self):
         return self.radius * 2
 
     @property
     def rate(self):
         return self.roll * self.speed / (self.angle * self.radius)
 
-    def create_template(self, transform: Transformation) -> State:
-        """generate a template loop State 
+    def create_template(self, istate: State, time: Time=None) -> State:
+        """Generate a template loop. 
 
         Args:
-            transform (Transformation): initial pos and attitude
+            istate (State): initial state
 
         Returns:
             [State]: flight data representing the loop
         """
-
         duration = self.radius * abs(self.angle) / self.speed
-        axis_rate = self.angle / duration
         
-        if axis_rate == 0:
-            raise NotImplementedError()
-
-        state = State.from_transform(
-            transform, 
-            vel=PX(self.speed),
-            rvel=PZ(self.angle / duration) if self.ke else PY(self.angle / duration)
-        ).extrapolate(duration)
+        if self.angle == 0:
+            raise NotImplementedError()      
         
-        return self._add_rolls(state, self.roll)
-
-    def corresponding_template(self, itrans: Transformation, aligned: State):
-        c = self.centre(itrans)
+        v = PX(self.speed) if istate.vel == 0 else istate.vel.scale(self.speed)
+        
+        return self._add_rolls(
+            istate.copy(
+                vel=v,
+                rvel=PZ(self.angle / duration) if self.ke else PY(self.angle / duration)
+            ).fill(
+                El.create_time(duration, time)
+            ), 
+            self.roll
+        )
 
     @property
     def centre_vector(self) -> Point:
         """Return the body frame vector from the start of the loop to the centre"""
         cv= PY if self.ke else PZ
         return cv(self.radius * np.sign(self.angle))
 
@@ -127,43 +127,39 @@
         return rpos / rpos[-1]
 
     def measure_radius(self, flown:State, template:State):
         """The radius in m given a state in the loop coordinate frame"""
         return abs(flown.pos * Point(1,1,0))
    
     def measure_end_angle(self, flown: State, template:State):
-        
         template_vels = template.att.transform_point(template.vel) * Point(1,1,0)
         flown_vels = flown.att.transform_point(flown.vel) * Point(1,1,0)
         return Point.angle_between(template_vels[-1], flown_vels[-1])
 
     def match_axis_rate(self, pitch_rate: float):
         return self.set_parms(radius=self.speed / pitch_rate)
 
-    def match_intention(self, itrans: Transformation, flown: State):      
+    def match_intention(self, itrans: Transformation, flown: State):
         jit = flown.judging_itrans(itrans)
         pos = jit.att.transform_point(flown.pos - jit.pos)
 
-        if self.ke:
-            x, y = pos.x, pos.y
-        else:
-            x, y = pos.x, pos.z
+        x, y = (pos.x, pos.y) if self.ke else (pos.x, pos.z)
             
         calc_R = lambda x, y, xc, yc: np.sqrt((x-xc)**2 + (y-yc)**2)
 
         def f_2(c):
             return calc_R(x, y, *c) - calc_R(x[0], y[0], *c)
 
         center, ier = optimize.leastsq(f_2, (np.mean(x), np.mean(y)))
 
         return self.set_parms(
             radius=calc_R(x[0], y[0],*center).mean(),
             roll=abs(self.roll) * np.sign(np.mean(flown.rvel.x)),
-            angle=abs(self.angle) * np.sign(np.sign(np.mean(flown.rvel.y))),
-            speed=np.mean(flown.u)
+            angle=abs(self.angle) * np.sign(flown.r.mean() if self.ke else flown.q.mean()),
+            speed=abs(flown.vel).mean()
         )
     
 
     def segment(self, transform:Transformation, flown: State, partitions=10):
         subsections = flown.segment(partitions)
         elms = [ self.match_intention( transform,sec) for sec in subsections ]
```

### Comparing `flightanalysis-0.1.0/flightanalysis/schedule/elements/stall_turn.py` & `flightanalysis-0.1.1/flightanalysis/schedule/elements/stall_turn.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import pandas as pd
-from geometry import Transformation, Point, PX, PY, PZ
+from geometry import Transformation, Point, PX, PY, PZ, P0
 from flightanalysis.state import State
-    
+from flightanalysis.base import Time
 from . import El, DownGrades, DownGrade
 from flightanalysis.criteria import *
 
 
 class StallTurn(El):
     parameters = El.parameters + ["yaw_rate"]
     def __init__(self, speed:float, yaw_rate:float=3.0, uid: str=None):
@@ -26,33 +26,30 @@
             speed=self.speed,
             uid=self.uid
         )
 
     def describe(self):
         return f"stallturn, yaw rate = {self.yaw_rate}"
 
-    def scale(self, factor):
-        return self.set_parms()
-
-    def create_template(self, transform: Transformation):
+    def create_template(self, istate: State, time: Time=None) -> State:
         return self._add_rolls(
-            State.from_transform(transform, vel=Point.zeros()).extrapolate( 
-                np.pi / abs(self.yaw_rate)
+            istate.copy(rvel=P0() ,vel=P0()).fill( 
+                El.create_time(np.pi / abs(self.yaw_rate), time)
             ).superimpose_rotation(
                 PZ(), 
                 np.sign(self.yaw_rate) * np.pi
             ), 
             0.0
         )
 
     def match_axis_rate(self, yaw_rate: float):
         return self.set_parms(yaw_rate=yaw_rate)
 
     def match_intention(self, transform: Transformation, flown: State):
         return self.set_parms(
-            yaw_rate=flown.r.max(), 
+            yaw_rate=flown.data.r[flown.data.r.abs().idxmax()]
         )
 
     def copy_direction(self, other):
         return self.set_parms(
             yaw_rate=abs(self.yaw_rate) * np.sign(other.yaw_rate)
         )
```

### Comparing `flightanalysis-0.1.0/flightanalysis/schedule/manoeuvre.py` & `flightanalysis-0.1.1/flightanalysis/schedule/manoeuvre.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,52 +23,73 @@
             data["uid"]
         )
 
     @staticmethod
     def from_all_elements(uid:str, els: List[El]):
         return Manoeuvre(els[0], els[1:], uid)
 
-    @property
-    def all_elements(self):
-        return Elements([self.entry_line, *self.elements.to_list()]) if not self.entry_line is None else self.elements
+    def all_elements(self, exit_line=False):
+        els = []
 
-    def create_template(self, transform: Transformation) -> State:
-        itrans = transform
+        if not self.entry_line is None:
+            els.append(self.entry_line)
+        else:
+            els.append(Line(self.elements[0].speed, 30, 0, "entry_line"))
+
+        for el in self.elements:
+            els.append(el)
+
+        if exit_line:
+            els.append(Line(els[-1].speed, 30, 0, "exit_line"))
+        
+        return Elements(els)
+
+
+    def create_template(self, initial: Union[Transformation, State], flown:State=None) -> State:
+        
+        istate = State.from_transform(initial, vel=PX()) if isinstance(initial, Transformation) else initial
+        
         templates = []
-        for i, element in enumerate(self.all_elements):
-            templates.append(element.create_template(itrans))
-            itrans = templates[-1][-1].transform
+        els = self.all_elements()
+        for i, element in enumerate(els):
+            time = element.get_data(flown).time if not flown is None else None
+            if i < len(els)-1 and not time is None:
+                time = time.extend()
+            templates.append(element.create_template(istate, time))
+            istate = templates[-1][-1]
         
         return State.stack(templates).label(manoeuvre=self.uid)
 
     def get_data(self, st: State):
         return st.get_manoeuvre(self.uid)
 
-    def match_intention(self, transform: Transformation, flown: State):
+    def match_intention(self, istate: State, flown: State):
         """Create a new manoeuvre with all the elements scaled to match the corresponding 
         flown element"""
 
         elms = []
         flown = self.get_data(flown)
 
-        for elm in self.all_elements:
+        for elm in self.all_elements():
+            st = elm.get_data(flown)
             elms.append(elm.match_intention(
-                transform, 
-                elm.get_data(flown)
+                istate.transform, 
+                st
             ))
-            try:
-                transform = elms[-1].create_template(
-                    transform
-                )[-1].transform
-            except Exception as ex:
-                print(f"Error creating template for {elm.__class__.__name__}, {elm.__dict__}")
-                print(str(ex))
-                raise Exception("Error Creating Template")
 
-        return Manoeuvre(elms[0], Elements(elms[1:]), self.uid), transform
+            if isinstance(elms[-1], Autorotation):
+                #copy the autorotation pitch offset back to the preceding pitch departure
+                angles = np.arctan2(st.vel.z, st.vel.x)
+                pos_break = max(angles)
+                neg_break = min(angles)
+                elms[-2].break_angle = pos_break if pos_break > -neg_break else neg_break
+
+            istate = elms[-1].create_template(istate)[-1]
+        
+        return Manoeuvre(elms[0], Elements(elms[1:]), self.uid), istate
 
     def match_rates(self, rates):
         new_elms = [elm.match_axis_rate(rates[elm.__class__], rates["speed"]) for elm in self.elements]
         return self.replace_elms(new_elms)
 
     def copy_directions(self, other):
         return Manoeuvre.from_all_elements(
@@ -84,7 +105,10 @@
         ers = [ElResults(self.entry_line, self.entry_line.analyse_exit(fl, tp))]
 
         for el in self.elements:
             fl = el.get_data(flown)
             tp = el.get_data(template).relocate(fl.pos[0])
             ers.append(ElResults(el, el.analyse(fl, tp)))
         return ElementsResults(ers)
+
+    def descriptions(self):
+        return [e.describe() for e in self.elements]
```

### Comparing `flightanalysis-0.1.0/flightanalysis/schedule/schedule.py` & `flightanalysis-0.1.1/flightanalysis/schedule/schedule.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from . import Manoeuvre
-from geometry import Transformation
+from geometry import Transformation, PX
 from flightanalysis.state import State
 import numpy as np
 from flightanalysis.base.collection import Collection
 
 # TODO it would be better if the list index of each manoeuvre corresponded with the uid. This is not possible because takeoff is not included as a manoeuvre. 
 # TODO perhaps include takeoff in the list as manoeuvre 0 and add it when reading from the json, use a constructor rather than __init__ when creating from python
 # TODO this will cause a problem when creating templates, as some data must (probably) be created for the takeoff, which will bugger up the entry_x_offset and dtw alignment (if its a straight line)
@@ -27,23 +27,25 @@
             
         return State.stack(templates)
 
     def match_intention(self, itrans:Transformation, alinged: State):
         """resize every element of the schedule to best fit the corresponding element in a labelled State
 
         Args:
+            itrans (Transformation): Transformation to first point of template 
             alinged (State): labelled flight data
 
         Returns:
             Schedule: new schedule with all the elements resized
         """
         _mans = []
+        istate = State.from_transform(Transformation(alinged[0].pos,itrans.att), vel=PX(self[0].elements[0].speed))
         for i, man in enumerate(self):
-            man, transform = man.match_intention(
-                transform if i>0 else Transformation(alinged[0].pos,itrans.att), 
+            man, istate = man.match_intention(
+                istate, 
                 man.get_data(alinged)
             )
             _mans.append(man)
 
         return Schedule(_mans)
 
     def correct_intention(self):
```

### Comparing `flightanalysis-0.1.0/flightanalysis/simulation.py` & `flightanalysis-0.1.1/flightanalysis/simulation.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.0/flightanalysis/state/__init__.py` & `flightanalysis-0.1.1/flightanalysis/state/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 
 
 
 from .state import State
 
 #
 from .tools.builders import (
+    fill,
     extrapolate, 
     from_csv, 
     from_flight, 
     stack
 )
 #
+State.fill = fill
 State.extrapolate = extrapolate
 State.from_csv = staticmethod(from_csv)
 State.from_flight = staticmethod(from_flight)
 State.stack = staticmethod(stack)
 #
 from .tools.transformers import (
     superimpose_angles, 
@@ -31,30 +33,43 @@
 State.move_back = move_back
 State.relocate = relocate
 State.superimpose_angles = superimpose_angles
 State.superimpose_rotation = superimpose_rotation
 State.superimpose_roll = superimpose_roll
 State.smooth_rotation = smooth_rotation
 #
-from .tools.alignment import align, copy_labels, splitter_labels, get_manoeuvre, get_element, get_element_from_manoeuvre
+from .tools.alignment import (
+    align, 
+    copy_labels, 
+    splitter_labels, 
+    get_manoeuvre, 
+    get_element, 
+    get_meid,
+    get_subset
+)
 #
 State.align = staticmethod(align)
 State.copy_labels = staticmethod(copy_labels)
 State.splitter_labels = splitter_labels
 State.get_manoeuvre = get_manoeuvre
 State.get_element = get_element
-State.get_element_from_manoeuvre = get_element_from_manoeuvre
+State.get_meid = get_meid
+State.get_subset = get_subset
 #
 from .tools.conversions import convert_state, to_judging, body_to_wind, judging_to_wind, wind_to_body
 #
 State.body_rotate = convert_state
 State.to_judging = to_judging
 State.body_to_wind = body_to_wind
 State.judging_to_wind = judging_to_wind
 State.wind_to_body = wind_to_body
 #
 from .tools.measurements import direction, inverted, upright, judging_itrans
 #
 State.direction = direction
 State.inverted = inverted
 State.upright = upright
-State.judging_itrans = judging_itrans
+State.judging_itrans = judging_itrans
+
+
+from .tools.dumpers import create_fc_json
+State.create_fc_json = create_fc_json
```

### Comparing `flightanalysis-0.1.0/flightanalysis/state/state.py` & `flightanalysis-0.1.1/flightanalysis/state/state.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from geometry import Point, Quaternion, Transformation, PX, PY, PZ, P0
+from geometry import Point, Quaternion, Transformation, PX, PY, PZ, P0, Q0
 
 import numpy as np
 import pandas as pd
 from typing import Union
 
 from flightanalysis.base.table import Table, Constructs, SVar, Time
 
@@ -29,42 +29,52 @@
 
 def make_racc(sec) -> Point:
     if len(sec) > 1:
         return sec.rvel.diff(sec.dt)
     else:
         return P0()
 
+
 class State(Table):
-    constructs = Table.constructs + Constructs(dict(
-        pos  = SVar(Point,       ["x", "y", "z"]           , None       ), 
-        att  = SVar(Quaternion,  ["rw", "rx", "ry", "rz"]  , None       ),
-        vel  = SVar(Point,       ["u", "v", "w"]           , make_bvel  ),
-        rvel = SVar(Point,       ["p", "q", "r"]           , make_rvel ),
-        acc  = SVar(Point,       ["du", "dv", "dw"]        , make_bacc  ),
-        racc = SVar(Point,       ["dp", "dq", "dr"]        , make_racc ),
-    ))
+    constructs = Table.constructs + Constructs([
+        SVar("pos", Point,       ["x", "y", "z"]           , lambda self: P0(len(self))       ), 
+        SVar("att", Quaternion,  ["rw", "rx", "ry", "rz"]  , lambda self : Q0(len(self))       ),
+        SVar("vel", Point,       ["u", "v", "w"]           , make_bvel  ),
+        SVar("rvel", Point,       ["p", "q", "r"]           , make_rvel ),
+        SVar("acc", Point,       ["du", "dv", "dw"]        , make_bacc  ),
+        SVar("racc", Point,       ["dp", "dq", "dr"]        , make_racc ),
+    ])
     _construct_freq = 30
 
     @property
     def transform(self):
         return Transformation.build(self.pos, self.att)
     
     @property
     def back_transform(self):
         return Transformation(-self.pos, self.att.inverse())
      
-
-    def from_transform(transform: Transformation, **kwargs): 
-        kwargs["time"] = Time.from_t(np.linspace(0, 30*len(transform), len(transform)))
+    @staticmethod
+    def from_transform(transform: Transformation, **kwargs):
+        if not "time" in kwargs: 
+            kwargs["time"] = Time.from_t(np.linspace(0, State._construct_freq*len(transform), len(transform)))
         return State.from_constructs(pos=transform.p, att=transform.q, **kwargs)
 
-    def body_to_world(self, pin: Point) -> Point:
+    def body_to_world(self, pin: Point, rotation_only=False) -> Point:
         """Rotate a point in the body frame to a point in the data frame
 
         Args:
             pin (Point): Point on the aircraft
 
         Returns:
             Point: Point in the world
         """
-        return self.transform.point(pin)
-
+        if rotation_only:
+            return self.transform.rotate(pin)
+        else:
+            return self.transform.point(pin)
+
+    def world_to_body(self, pin: Point, rotation_only=False) -> Point:
+        if rotation_only:
+            self.back_transform.rotate(pin)
+        else:
+            return self.back_transform.point(pin)
```

### Comparing `flightanalysis-0.1.0/flightanalysis/state/tools/alignment.py` & `flightanalysis-0.1.1/flightanalysis/state/tools/alignment.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from geometry import Point
 from fastdtw import fastdtw
 import warnings
 from scipy.spatial.distance import euclidean
 from flightanalysis.state import State
 import numpy as np
 import pandas as pd
-from typing import List
+from typing import List, Union
+from pandas.api.types import is_list_like
 
 
 def align(flown, template, radius=5, mirror=True, white=False, weights = Point(1,1,1)) -> State:
     """Perform a temporal alignment between two sections. return the flown section with labels 
     copied from the template along the warped path
 
     Args:
@@ -42,30 +43,42 @@
         radius=radius,
         dist=euclidean
     )
 
     return distance, copy_labels(template, flown, path)
 
 
-def copy_labels(template, flown, path) -> State:
+def copy_labels(template, flown, path=None) -> State:
     """Copy the labels from a template section to a flown section along the index warping path
 
     Args:
         template (Section): A labelled section
         flown (Section): An unlabelled section
         path (List): A list of lists containing index pairs from template to flown
 
     Returns:
         Section: a labelled section
     """
-    mans = pd.DataFrame(path, columns=["template", "flight"]).set_index("template").join(
-            template.data.reset_index(drop=True).loc[:, ["manoeuvre", "element"]]
-        ).groupby(['flight']).last().reset_index().set_index("flight")
 
-    return State(flown.data.reset_index(drop=True).join(mans).set_index("t", drop=False))
+    flown = flown.remove_labels()
+
+    keys = [k for k in ["manoeuvre", "element", "sub_element"] if k in template.data.columns]
+    if path is None:
+        return State(
+            pd.concat(
+                [flown.data.reset_index(drop=True), template.data.loc[:,keys].reset_index(drop=True)], 
+                axis=1
+            ).set_index("t", drop=False)
+        )
+    else:
+        mans = pd.DataFrame(path, columns=["template", "flight"]).set_index("template").join(
+                template.data.reset_index(drop=True).loc[:, keys]
+            ).groupby(['flight']).last().reset_index().set_index("flight")
+
+        return State(flown.data.reset_index(drop=True).join(mans).set_index("t", drop=False))
 
 
 def splitter_labels(self: State, mans: List[dict]) -> State:
         """label the manoeuvres in a State based on the flight coach splitter information
 
         TODO this assumes the state only contains the dataset contained in the json
 
@@ -92,16 +105,37 @@
                 ).label(manoeuvre=split_man["name"])
             )
             labels.append(split_man["name"])
 
         return State.stack(labelled)
 
 
-def get_manoeuvre(self: State, manoeuvre_name: str):
-    return State(self.data.loc[self.data.manoeuvre == manoeuvre_name])
 
-def get_element(self: State, element_name: str):
-    return State(self.data.loc[self.data.element == element_name]) 
+def get_subset(self: State, mans: Union[list, slice], col="manoeuvre"):
+    selectors = self.data.loc[:,col].unique()
+    if isinstance(mans, slice):
+        mans = selectors[mans]
+
+    if not is_list_like(mans):
+        mans = [mans]
+    
+    if not all(isinstance(m, str) for m in mans):
+        mans = [m.uid if m.__class__.__name__ == "Manoeuvre" else m for m in mans]
+        mans = [m.uid if m.__class__.__bases__[0].__name__ == "El" else m for m in mans]    
+        mans = [selectors[m] if isinstance(m, int) else m for m in mans]
+        
+    assert all(isinstance(m, str) for m in mans)
+
+    return State(self.data.loc[self.data.loc[:, col].isin(mans)])
 
-def get_element_from_manoeuvre(self: State, manoeuvre_name: str, element_name: str):
-    return self.get_manoeuvre(manoeuvre_name).get_element(element_name)
+def get_manoeuvre(self: State, manoeuvre: Union[str, list, int]):
+    return get_subset(self, manoeuvre, "manoeuvre")
 
+def get_element(self: State, element: Union[str, list, int]):
+    return get_subset(self, element, "element") 
+
+def get_meid(self: State, manid: int, elid: int=None):
+    st = self.get_manoeuvre(manid)
+    if not elid is None:
+        return st.get_element(elid)
+    else:
+        return st
```

### Comparing `flightanalysis-0.1.0/flightanalysis/state/tools/builders.py` & `flightanalysis-0.1.1/flightanalysis/state/tools/builders.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,23 @@
 from geometry import Point, Quaternion, PX, P0
 from typing import Union
 from flightanalysis.flightline import FlightLine, Box
 from flightdata import Flight, Fields
 from pathlib import Path
 
 
+def fill(istate: State, time: Time) -> State:
+    vel = istate.vel.tile(len(time))   
+    rvel = istate.rvel.tile(len(time))
+    att = istate.att.body_rotate(rvel * time.t)
+    #pos = Point.concatenate([P0(), (att[1:].transform_point(vel[1:]) * time.dt[1:]).cumsum()]) + istate.pos
+    #TODO improve the position accuracy by extrapolating the points round a circle
+    pos = (att.transform_point(vel) * time.dt).cumsum() + istate.pos
+    return State.from_constructs(time,pos, att, vel, rvel)
+
 
 def extrapolate(istate: State, duration: float) -> State:
     """extrapolate the input state, currently ignores input accelerations
 
     Args:
         istate (State): initial state of length 1
         duration (float): duration of extrapolation in seconds
@@ -20,21 +29,16 @@
     Returns:
         State: state projected forwards
     """
 
     npoints = np.max([int(np.ceil(duration / istate.dt[0])), 3])
 
     time = Time.from_t(np.linspace(0,duration, npoints))
-    vel = istate.vel.tile(len(time))   
-    rvel = istate.rvel.tile(len(time))
-    att = istate.att.body_rotate(rvel * time.t)
-    #pos = Point.concatenate([P0(), (att[1:].transform_point(vel[1:]) * time.dt[1:]).cumsum()]) + istate.pos
-    #TODO improve the position accuracy by extrapolating the points round a circle
-    pos = (att.transform_point(vel) * time.dt).cumsum() + istate.pos
-    return State.from_constructs(time,pos, att, vel, rvel)
+
+    return istate.fill(time)
 
 
 def from_csv(filename) -> State:
     df = pd.read_csv(filename)
 
     if "time_index" in df.columns: # This is for back compatability with old csv files where time column was labelled differently
         if "t" in df.columns:
@@ -46,15 +50,16 @@
 
 def from_flight(flight: Union[Flight, str], box:Union[FlightLine, Box, str]) -> State:
     if isinstance(flight, str):
         flight = {
             ".csv": Flight.from_csv,
             ".BIN": Flight.from_log
         }[Path(flight).suffix](flight)
-
+    if box is None:
+        box = Box.from_initial(flight)
     if isinstance(box, FlightLine):
         return _from_flight(flight, box)
     if isinstance(box, Box):
         return _from_flight(flight, FlightLine.from_box(box, flight.origin))
     if isinstance(box, str):
         box = Box.from_json(box)
         return _from_flight(flight, FlightLine.from_box(box, flight.origin))
```

### Comparing `flightanalysis-0.1.0/flightanalysis/state/tools/conversions.py` & `flightanalysis-0.1.1/flightanalysis/state/tools/conversions.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.0/flightanalysis/state/tools/dumpers.py` & `flightanalysis-0.1.1/flightanalysis/state/tools/dumpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from geometry import Transformation, Coord, Quaternion, Point
 from flightanalysis.state import State
-from flightanalysis.schedule import Schedule, SchedDef
 import numpy as np
 import pandas as pd
 
 
 
 def _create_json_data(self: State) -> pd.DataFrame:
     fcd = pd.DataFrame(columns=["N", "E", "D", "VN", "VE", "VD", "r", "p", "yw", "wN", "wE", "roll", "pitch", "yaw"])
     fcd["N"], fcd["E"], fcd["D"] = self.x, -self.y, -self.z
-    wvels = self.body_to_world(Point(self.bvel))
+    wvels = self.body_to_world(Point(self.vel))
     fcd["VN"], fcd["VE"], fcd["VD"] = wvels.x, -wvels.y, -wvels.z
 
     transform = Transformation.from_coords(
         Coord.from_xy(Point(0, 0, 0), Point(1, 0, 0), Point(0, 1, 0)),
         Coord.from_xy(Point(0, 0, 0), Point(1, 0, 0), Point(0, -1, 0))
     )
     eul = transform.rotate(Quaternion(self.att)).to_euler()
@@ -29,47 +28,47 @@
 
     fcd = fcd.reset_index()
     fcd.columns = ["time", "N", "E", "D", "VN", "VE", "VD", "r", "p", "yw", "wN", "wE", "roll", "pitch", "yaw"]
     fcd["time"] = np.int64(fcd["time"] * 1e6)
     return fcd
 
 
-def _create_json_mans(self: State, sdef: SchedDef) -> pd.DataFrame:
+def _create_json_mans(self: State, sdef) -> pd.DataFrame:
     mans = pd.DataFrame(columns=["name", "id", "sp", "wd", "start", "stop", "sel", "background", "k"])
 
     mans["name"] = ["tkoff"] + [man.info.short_name for man in sdef]
     mans["k"] = [0] + [man.info.k for man in sdef]
-    mans["id"] = ["sp_{}".format(i) for i in range(len(sdef) + 1)]
+    mans["id"] = ["sp_{}".format(i) for i in range(len(sdef.data)+1)]
 
     mans["sp"] = list(range(len(sdef.data) + 1))
     
     itsecs = [self.get_manoeuvre(m.info.short_name) for m in sdef] 
 
-    mans["wd"] = [100 * st.duration / self.duration for st in itsecs]
+    mans["wd"] = [0.0] + [100 * st.duration / self.duration for st in itsecs]
     
     dat = self.data.reset_index(drop=True)
 
     mans["start"] = [0] + [dat.loc[dat.manoeuvre==man.info.short_name].index[0] for man in sdef]
 
     mans["stop"] = [mans["start"][1] + 1] + [dat.loc[dat.manoeuvre==man.info.short_name].index[-1] + 1 for man in sdef]
         
-    mans["sel"] = np.full(len(sdef) + 1, False)
+    mans["sel"] = np.full(len(sdef.data) + 1, False)
     mans.loc[1,"sel"] = True
-    mans["background"] = np.full(len(sdef) + 1, "")
+    mans["background"] = np.full(len(sdef.data) + 1, "")
 
     return mans
 
 
-def create_fc_json(self: State, sdef: SchedDef, schedule_name: str, schedule_category: str="F3A"):
+def create_fc_json(self: State, sdef, schedule_name: str, schedule_category: str="F3A"):
     fcdata = _create_json_data(self)
     fcmans = _create_json_mans(self, sdef)
     return {
         "version": "1.3",
         "comments": "DO NOT EDIT\n",
-        "name": sdef.info.name,
+        "name": schedule_name,
         "view": {
             "position": {
                 "x": -120,
                 "y": 130.50000000000003,
                 "z": 264.99999999999983
             },
             "target": {
```

### Comparing `flightanalysis-0.1.0/flightanalysis/state/tools/measurements.py` & `flightanalysis-0.1.1/flightanalysis/state/tools/measurements.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 from flightanalysis.state import State
 import numpy as np
 from geometry import Transformation, Quaternion, Coord, P0, PX, PY, PZ, Point
 
 
-
-
-
 def direction(self):
     """returns 1 for going right, -1 for going left"""
     return np.sign(self.att.transform_point(Point(1, 0, 0)).x)
     
 
 def inverted(self):
     return np.sign(self.att.transform_point(Point(0, 0, 1)).z) > 0
```

### Comparing `flightanalysis-0.1.0/flightanalysis/state/tools/transformers.py` & `flightanalysis-0.1.1/flightanalysis/state/tools/transformers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 import numpy as np
 import pandas as pd
 from flightanalysis.state import State
 from geometry import Point, Quaternion, Transformation, PX, Q0, P0
 
 
-
 def move(st: State, transform: Transformation) -> State:
-    return State.from_constructs(
+    return State.copy_labels(st, State.from_constructs(
         time=st.time,
         pos=transform.point(st.pos),
         att=transform.rotate(st.att),
         vel=st.vel,
         rvel=st.rvel,
         acc=st.acc,
         racc=st.racc,
-    )
+    ))
 
 def move_back(st:State, transform:Transformation) -> State:
     st = move(st, Transformation(-transform.pos, Q0()))
     return move(st, Transformation(P0(), transform.att.inverse()))
 
 
 def relocate(st:State, start_pos: Point) -> State:
     offset = start_pos - st.pos[0]
     return st.move(Transformation(offset, Q0()))
 
 def superimpose_angles(st: State, angles: Point, reference:str="body"): 
     assert reference in ["body", "world"]
-    sec =  State.from_constructs(
-        st.time,
-        st.pos,
-        st.att.rotate(angles) if reference=="world" else st.att.body_rotate(angles)
-    )
+    sec = State.copy_labels(
+        st, 
+        State.from_constructs(
+            st.time,
+            st.pos,
+            st.att.rotate(angles) if reference=="world" else st.att.body_rotate(angles)
+        )
+    ) 
 
     #if "sub_element" in st.data.columns:
      #   sec = sec.append_columns(st.data["sub_element"])
     return sec
 
 
 def superimpose_rotation(st: State, axis: Point, angle: float, reference:str="body"):
@@ -56,15 +58,14 @@
 
     Args:
         angle (float): the amount of roll to integrate
     """
     return st.superimpose_rotation(PX(), angle)
 
 
-
 def smooth_rotation(st: State, axis: Point, angle: float, reference:str="body", w: float=0.25, w2=0.1):
     """Accelerate for acc_prop * t, flat rate for middle, slow down for acc_prop * t.
 
     Args:
         axis (Point): Axis to rotate around.
         angle (float): angle to rotate.
         reference (str, optional): rotate about body or world. Defaults to "body".
```

### Comparing `flightanalysis-0.1.0/flightanalysis.egg-info/PKG-INFO` & `flightanalysis-0.1.1/flightanalysis.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: flightanalysis
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for analysing flight data
 Home-page: https://github.com/PyFlightCoach/FlightAnalysis
 Author: Thomas David
 Author-email: thomasdavid0@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FlightAnalysis
 
-This package contains tools for analysing flight log data. It is based around the State and Section objects, which handle state information for an instant and a section of time. It also contains tools for constructing template Section and State instances based on serialised aerobatic manoeuvre definitions. Temporal alignments can be performed to automatically label flight data based on these templates. New scaled templates can then be constructed based on measurements taken of the labelled elements. 
+This package contains tools for analysing flight log data. 
 
 The Main Idea
 1. Read the sequence defintion from the serialisation of it (currently schedule/p_21.py)
 2. Read, trim and rotate flight recorded flight data
 3. generate a roughly scaled template sequence
 4. run a dynamic time warping algorithm to align the flight to the template
 5. generate scaled templates based on the rules and the flown manoeuvre
@@ -24,17 +24,12 @@
 - Estimate winds from flight data without airspeed sensor. see examples/wind.ipynb
 - Construct a FD model from the flight data with MLP regression or something.
 - The templates are constructed in some kind of 'Judging' axis, similar to the aircraft wind axis but with atmospheric wind removed. Consider accounting for some aerodynamic characteristics here and constructing templates at some alpha and beta.
 - Compare logged control inputs to ideal control inputs calculated using the templates and the FDmodel.
 
 
 # External Dependencies:
-python (3.6+?)
-numpy
-pandas
 scipy
 fastdtw
-
-## This package also depends on other PyFlightCoach packages:
 ardupilot_log_reader
 flightdata
-geometry
+pfc-geometry
```

### Comparing `flightanalysis-0.1.0/flightanalysis.egg-info/SOURCES.txt` & `flightanalysis-0.1.1/flightanalysis.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 setup.cfg
 setup.py
 flightanalysis/__init__.py
 flightanalysis/aircraft_analysis.py
 flightanalysis/controls.py
 flightanalysis/fc_json.py
+flightanalysis/fc_score.py
 flightanalysis/flightline.py
 flightanalysis/simulation.py
 flightanalysis.egg-info/PKG-INFO
 flightanalysis.egg-info/SOURCES.txt
 flightanalysis.egg-info/dependency_links.txt
 flightanalysis.egg-info/requires.txt
 flightanalysis.egg-info/top_level.txt
@@ -21,42 +22,53 @@
 flightanalysis/criteria/__init__.py
 flightanalysis/criteria/combination.py
 flightanalysis/criteria/comparison.py
 flightanalysis/criteria/continuous.py
 flightanalysis/criteria/results.py
 flightanalysis/criteria/single.py
 flightanalysis/data/__init__.py
+flightanalysis/data/f25.py
 flightanalysis/data/p23.py
+flightanalysis/data/p25.py
 flightanalysis/environment/__init__.py
 flightanalysis/environment/environment.py
 flightanalysis/environment/wind.py
 flightanalysis/model/__init__.py
 flightanalysis/model/coefficients.py
 flightanalysis/model/constants.py
 flightanalysis/model/flow.py
 flightanalysis/model/model.py
 flightanalysis/schedule/__init__.py
 flightanalysis/schedule/manoeuvre.py
 flightanalysis/schedule/schedule.py
 flightanalysis/schedule/definition/__init__.py
 flightanalysis/schedule/definition/collectors.py
+flightanalysis/schedule/definition/element_builders.py
 flightanalysis/schedule/definition/element_definition.py
+flightanalysis/schedule/definition/manoeuvre_builder.py
 flightanalysis/schedule/definition/manoeuvre_definition.py
 flightanalysis/schedule/definition/manoeuvre_info.py
 flightanalysis/schedule/definition/manoeuvre_parameters.py
 flightanalysis/schedule/definition/operation.py
 flightanalysis/schedule/definition/schedule_definition.py
 flightanalysis/schedule/elements/__init__.py
+flightanalysis/schedule/elements/autorotation.py
 flightanalysis/schedule/elements/line.py
 flightanalysis/schedule/elements/loop.py
-flightanalysis/schedule/elements/snap.py
-flightanalysis/schedule/elements/spin.py
+flightanalysis/schedule/elements/nose_drop.py
+flightanalysis/schedule/elements/pitch_break.py
+flightanalysis/schedule/elements/recovery.py
 flightanalysis/schedule/elements/stall_turn.py
 flightanalysis/state/__init__.py
 flightanalysis/state/state.py
 flightanalysis/state/tools/__init__.py
 flightanalysis/state/tools/alignment.py
 flightanalysis/state/tools/builders.py
 flightanalysis/state/tools/conversions.py
 flightanalysis/state/tools/dumpers.py
 flightanalysis/state/tools/measurements.py
-flightanalysis/state/tools/transformers.py
+flightanalysis/state/tools/transformers.py
+tests/test_analysis.py
+tests/test_controls.py
+tests/test_data.py
+tests/test_fc_json.py
+tests/test_flightline.py
```

### Comparing `flightanalysis-0.1.0/setup.py` & `flightanalysis-0.1.1/setup.py`

 * *Files identical despite different names*

