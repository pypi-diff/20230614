# Comparing `tmp/flightanalysis-0.1.5.tar.gz` & `tmp/flightanalysis-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flightanalysis-0.1.5.tar", last modified: Wed Jun 14 12:27:56 2023, max compression
+gzip compressed data, was "flightanalysis-0.1.6.tar", last modified: Wed Jun 14 17:43:24 2023, max compression
```

## Comparing `flightanalysis-0.1.5.tar` & `flightanalysis-0.1.6.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 12:27:56.461065 flightanalysis-0.1.5/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)    35149 2023-03-28 15:54:19.000000 flightanalysis-0.1.5/LICENSE
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       34 2023-06-14 11:48:20.000000 flightanalysis-0.1.5/MANIFEST.in
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1443 2023-06-14 12:27:56.461065 flightanalysis-0.1.5/PKG-INFO
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1160 2023-03-28 15:54:19.000000 flightanalysis-0.1.5/README.md
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 12:27:56.457065 flightanalysis-0.1.5/flightanalysis/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      261 2023-03-28 15:54:19.000000 flightanalysis-0.1.5/flightanalysis/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     3609 2023-03-28 15:54:19.000000 flightanalysis-0.1.5/flightanalysis/aircraft_analysis.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 12:27:56.457065 flightanalysis-0.1.5/flightanalysis/base/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       65 2023-03-28 15:54:19.000000 flightanalysis-0.1.5/flightanalysis/base/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2565 2023-06-05 21:18:21.000000 flightanalysis-0.1.5/flightanalysis/base/collection.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2178 2023-06-13 10:36:02.000000 flightanalysis-0.1.5/flightanalysis/base/constructs.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      221 2023-03-28 15:54:19.000000 flightanalysis-0.1.5/flightanalysis/base/numpy_encoder.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     5286 2023-06-13 11:47:30.000000 flightanalysis-0.1.5/flightanalysis/base/table.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1693 2023-06-05 21:18:21.000000 flightanalysis-0.1.5/flightanalysis/controls.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 12:27:56.457065 flightanalysis-0.1.5/flightanalysis/criteria/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1454 2023-03-28 15:54:19.000000 flightanalysis-0.1.5/flightanalysis/criteria/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2350 2023-03-28 15:54:19.000000 flightanalysis-0.1.5/flightanalysis/criteria/combination.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1324 2023-03-28 15:54:19.000000 flightanalysis-0.1.5/flightanalysis/criteria/comparison.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2013 2023-03-28 15:54:19.000000 flightanalysis-0.1.5/flightanalysis/criteria/continuous.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      925 2023-03-28 15:54:19.000000 flightanalysis-0.1.5/flightanalysis/criteria/results.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1341 2023-06-05 21:18:21.000000 flightanalysis-0.1.5/flightanalysis/criteria/single.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 12:27:56.457065 flightanalysis-0.1.5/flightanalysis/data/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      293 2023-06-14 12:08:11.000000 flightanalysis-0.1.5/flightanalysis/data/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)    79839 2023-06-14 11:06:35.000000 flightanalysis-0.1.5/flightanalysis/data/f25.json
--rw-rw-r--   0 td6834    (1001) td6834    (1001)    70673 2023-06-14 11:05:48.000000 flightanalysis-0.1.5/flightanalysis/data/p23.json
--rw-rw-r--   0 td6834    (1001) td6834    (1001)    73755 2023-06-14 11:05:11.000000 flightanalysis-0.1.5/flightanalysis/data/p25.json
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 12:27:56.457065 flightanalysis-0.1.5/flightanalysis/environment/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       91 2023-03-28 15:54:19.000000 flightanalysis-0.1.5/flightanalysis/environment/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1393 2023-06-05 21:18:21.000000 flightanalysis-0.1.5/flightanalysis/environment/environment.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4345 2023-03-28 15:54:19.000000 flightanalysis-0.1.5/flightanalysis/environment/wind.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      466 2023-06-13 14:30:47.000000 flightanalysis-0.1.5/flightanalysis/fc_json.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4174 2023-06-14 09:43:36.000000 flightanalysis-0.1.5/flightanalysis/fc_score.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     7725 2023-06-05 21:18:18.000000 flightanalysis-0.1.5/flightanalysis/flightline.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 12:27:56.457065 flightanalysis-0.1.5/flightanalysis/model/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      108 2023-03-28 15:54:19.000000 flightanalysis-0.1.5/flightanalysis/model/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1179 2023-06-05 21:18:21.000000 flightanalysis-0.1.5/flightanalysis/model/coefficients.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      405 2023-03-28 15:54:19.000000 flightanalysis-0.1.5/flightanalysis/model/constants.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1377 2023-06-05 21:18:21.000000 flightanalysis-0.1.5/flightanalysis/model/flow.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      675 2023-03-28 15:54:19.000000 flightanalysis-0.1.5/flightanalysis/model/model.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 12:27:56.457065 flightanalysis-0.1.5/flightanalysis/schedule/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2888 2023-06-13 12:22:27.000000 flightanalysis-0.1.5/flightanalysis/schedule/__init__.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 12:27:56.461065 flightanalysis-0.1.5/flightanalysis/schedule/definition/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      695 2023-06-05 21:18:21.000000 flightanalysis-0.1.5/flightanalysis/schedule/definition/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1482 2023-06-06 05:23:48.000000 flightanalysis-0.1.5/flightanalysis/schedule/definition/collectors.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     6382 2023-06-13 08:53:43.000000 flightanalysis-0.1.5/flightanalysis/schedule/definition/element_builders.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4907 2023-06-05 21:18:21.000000 flightanalysis-0.1.5/flightanalysis/schedule/definition/element_definition.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4658 2023-06-14 07:40:53.000000 flightanalysis-0.1.5/flightanalysis/schedule/definition/manoeuvre_builder.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     5202 2023-06-13 12:23:31.000000 flightanalysis-0.1.5/flightanalysis/schedule/definition/manoeuvre_definition.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4126 2023-06-05 21:18:21.000000 flightanalysis-0.1.5/flightanalysis/schedule/definition/manoeuvre_info.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     6220 2023-06-13 12:59:23.000000 flightanalysis-0.1.5/flightanalysis/schedule/definition/manoeuvre_parameters.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     7430 2023-06-06 05:26:36.000000 flightanalysis-0.1.5/flightanalysis/schedule/definition/operation.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1959 2023-06-14 11:04:57.000000 flightanalysis-0.1.5/flightanalysis/schedule/definition/schedule_definition.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 12:27:56.461065 flightanalysis-0.1.5/flightanalysis/schedule/elements/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     7335 2023-06-13 12:21:00.000000 flightanalysis-0.1.5/flightanalysis/schedule/elements/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1749 2023-06-13 12:17:45.000000 flightanalysis-0.1.5/flightanalysis/schedule/elements/autorotation.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     3397 2023-06-13 12:16:23.000000 flightanalysis-0.1.5/flightanalysis/schedule/elements/line.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     6341 2023-06-13 12:18:07.000000 flightanalysis-0.1.5/flightanalysis/schedule/elements/loop.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1844 2023-06-13 12:18:45.000000 flightanalysis-0.1.5/flightanalysis/schedule/elements/nose_drop.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1357 2023-06-13 12:19:01.000000 flightanalysis-0.1.5/flightanalysis/schedule/elements/pitch_break.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1109 2023-06-13 12:19:11.000000 flightanalysis-0.1.5/flightanalysis/schedule/elements/recovery.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1685 2023-06-13 12:21:37.000000 flightanalysis-0.1.5/flightanalysis/schedule/elements/stall_turn.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     3929 2023-06-13 12:27:56.000000 flightanalysis-0.1.5/flightanalysis/schedule/manoeuvre.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4507 2023-06-05 21:18:21.000000 flightanalysis-0.1.5/flightanalysis/schedule/schedule.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      891 2023-03-28 15:54:19.000000 flightanalysis-0.1.5/flightanalysis/simulation.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 12:27:56.461065 flightanalysis-0.1.5/flightanalysis/state/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1689 2023-06-14 08:27:10.000000 flightanalysis-0.1.5/flightanalysis/state/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2611 2023-06-05 21:18:21.000000 flightanalysis-0.1.5/flightanalysis/state/state.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 12:27:56.461065 flightanalysis-0.1.5/flightanalysis/state/tools/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)        1 2023-03-28 15:54:19.000000 flightanalysis-0.1.5/flightanalysis/state/tools/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4570 2023-06-14 09:02:25.000000 flightanalysis-0.1.5/flightanalysis/state/tools/alignment.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4450 2023-06-05 21:18:21.000000 flightanalysis-0.1.5/flightanalysis/state/tools/builders.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2722 2023-03-28 15:54:19.000000 flightanalysis-0.1.5/flightanalysis/state/tools/conversions.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     3635 2023-06-05 21:18:21.000000 flightanalysis-0.1.5/flightanalysis/state/tools/dumpers.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      931 2023-06-05 21:18:21.000000 flightanalysis-0.1.5/flightanalysis/state/tools/measurements.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2966 2023-06-05 21:18:21.000000 flightanalysis-0.1.5/flightanalysis/state/tools/transformers.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 12:27:56.457065 flightanalysis-0.1.5/flightanalysis.egg-info/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1443 2023-06-14 12:27:56.000000 flightanalysis-0.1.5/flightanalysis.egg-info/PKG-INFO
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2693 2023-06-14 12:27:56.000000 flightanalysis-0.1.5/flightanalysis.egg-info/SOURCES.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)        1 2023-06-14 12:27:56.000000 flightanalysis-0.1.5/flightanalysis.egg-info/dependency_links.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       49 2023-06-14 12:27:56.000000 flightanalysis-0.1.5/flightanalysis.egg-info/requires.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       15 2023-06-14 12:27:56.000000 flightanalysis-0.1.5/flightanalysis.egg-info/top_level.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      446 2023-06-14 12:27:56.461065 flightanalysis-0.1.5/setup.cfg
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      687 2023-06-14 11:51:46.000000 flightanalysis-0.1.5/setup.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 12:27:56.461065 flightanalysis-0.1.5/tests/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      215 2023-03-28 15:54:19.000000 flightanalysis-0.1.5/tests/test_analysis.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      402 2023-03-28 15:54:19.000000 flightanalysis-0.1.5/tests/test_controls.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      206 2023-03-28 15:54:19.000000 flightanalysis-0.1.5/tests/test_data.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2268 2023-03-28 15:54:19.000000 flightanalysis-0.1.5/tests/test_fc_json.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     6855 2023-06-05 21:18:18.000000 flightanalysis-0.1.5/tests/test_flightline.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 17:43:24.274142 flightanalysis-0.1.6/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)    35149 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/LICENSE
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       34 2023-06-14 11:48:20.000000 flightanalysis-0.1.6/MANIFEST.in
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1443 2023-06-14 17:43:24.274142 flightanalysis-0.1.6/PKG-INFO
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1160 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/README.md
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 17:43:24.270142 flightanalysis-0.1.6/flightanalysis/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      261 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/flightanalysis/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     3609 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/flightanalysis/aircraft_analysis.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 17:43:24.270142 flightanalysis-0.1.6/flightanalysis/base/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       65 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/flightanalysis/base/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2574 2023-06-14 16:19:59.000000 flightanalysis-0.1.6/flightanalysis/base/collection.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2178 2023-06-13 10:36:02.000000 flightanalysis-0.1.6/flightanalysis/base/constructs.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      221 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/flightanalysis/base/numpy_encoder.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     5436 2023-06-14 15:42:22.000000 flightanalysis-0.1.6/flightanalysis/base/table.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1693 2023-06-05 21:18:21.000000 flightanalysis-0.1.6/flightanalysis/controls.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 17:43:24.270142 flightanalysis-0.1.6/flightanalysis/criteria/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1454 2023-06-14 16:19:04.000000 flightanalysis-0.1.6/flightanalysis/criteria/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2434 2023-06-14 16:18:29.000000 flightanalysis-0.1.6/flightanalysis/criteria/combination.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1417 2023-06-14 16:16:38.000000 flightanalysis-0.1.6/flightanalysis/criteria/comparison.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2228 2023-06-14 16:17:13.000000 flightanalysis-0.1.6/flightanalysis/criteria/continuous.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      925 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/flightanalysis/criteria/results.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1532 2023-06-14 16:16:58.000000 flightanalysis-0.1.6/flightanalysis/criteria/single.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 17:43:24.270142 flightanalysis-0.1.6/flightanalysis/data/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      293 2023-06-14 12:08:11.000000 flightanalysis-0.1.6/flightanalysis/data/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)    79839 2023-06-14 11:06:35.000000 flightanalysis-0.1.6/flightanalysis/data/f25.json
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)    70673 2023-06-14 11:05:48.000000 flightanalysis-0.1.6/flightanalysis/data/p23.json
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)    73755 2023-06-14 11:05:11.000000 flightanalysis-0.1.6/flightanalysis/data/p25.json
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 17:43:24.270142 flightanalysis-0.1.6/flightanalysis/environment/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       91 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/flightanalysis/environment/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1393 2023-06-05 21:18:21.000000 flightanalysis-0.1.6/flightanalysis/environment/environment.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4345 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/flightanalysis/environment/wind.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      466 2023-06-13 14:30:47.000000 flightanalysis-0.1.6/flightanalysis/fc_json.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     5479 2023-06-14 17:31:54.000000 flightanalysis-0.1.6/flightanalysis/fc_score.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     7725 2023-06-05 21:18:18.000000 flightanalysis-0.1.6/flightanalysis/flightline.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 17:43:24.274142 flightanalysis-0.1.6/flightanalysis/model/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      108 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/flightanalysis/model/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1179 2023-06-05 21:18:21.000000 flightanalysis-0.1.6/flightanalysis/model/coefficients.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      405 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/flightanalysis/model/constants.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1377 2023-06-05 21:18:21.000000 flightanalysis-0.1.6/flightanalysis/model/flow.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      675 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/flightanalysis/model/model.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 17:43:24.274142 flightanalysis-0.1.6/flightanalysis/schedule/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2888 2023-06-13 12:22:27.000000 flightanalysis-0.1.6/flightanalysis/schedule/__init__.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 17:43:24.274142 flightanalysis-0.1.6/flightanalysis/schedule/definition/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      695 2023-06-05 21:18:21.000000 flightanalysis-0.1.6/flightanalysis/schedule/definition/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1482 2023-06-06 05:23:48.000000 flightanalysis-0.1.6/flightanalysis/schedule/definition/collectors.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     6382 2023-06-13 08:53:43.000000 flightanalysis-0.1.6/flightanalysis/schedule/definition/element_builders.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4907 2023-06-05 21:18:21.000000 flightanalysis-0.1.6/flightanalysis/schedule/definition/element_definition.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4658 2023-06-14 07:40:53.000000 flightanalysis-0.1.6/flightanalysis/schedule/definition/manoeuvre_builder.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     5202 2023-06-13 12:23:31.000000 flightanalysis-0.1.6/flightanalysis/schedule/definition/manoeuvre_definition.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4126 2023-06-05 21:18:21.000000 flightanalysis-0.1.6/flightanalysis/schedule/definition/manoeuvre_info.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     6220 2023-06-13 12:59:23.000000 flightanalysis-0.1.6/flightanalysis/schedule/definition/manoeuvre_parameters.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     7430 2023-06-06 05:26:36.000000 flightanalysis-0.1.6/flightanalysis/schedule/definition/operation.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1959 2023-06-14 11:04:57.000000 flightanalysis-0.1.6/flightanalysis/schedule/definition/schedule_definition.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 17:43:24.274142 flightanalysis-0.1.6/flightanalysis/schedule/elements/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     7343 2023-06-14 17:36:12.000000 flightanalysis-0.1.6/flightanalysis/schedule/elements/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1965 2023-06-14 17:38:48.000000 flightanalysis-0.1.6/flightanalysis/schedule/elements/autorotation.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     3369 2023-06-14 16:25:15.000000 flightanalysis-0.1.6/flightanalysis/schedule/elements/line.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     6341 2023-06-13 12:18:07.000000 flightanalysis-0.1.6/flightanalysis/schedule/elements/loop.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2069 2023-06-14 17:37:45.000000 flightanalysis-0.1.6/flightanalysis/schedule/elements/nose_drop.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1584 2023-06-14 17:38:08.000000 flightanalysis-0.1.6/flightanalysis/schedule/elements/pitch_break.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1282 2023-06-14 17:38:30.000000 flightanalysis-0.1.6/flightanalysis/schedule/elements/recovery.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1685 2023-06-13 12:21:37.000000 flightanalysis-0.1.6/flightanalysis/schedule/elements/stall_turn.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4106 2023-06-14 15:44:45.000000 flightanalysis-0.1.6/flightanalysis/schedule/manoeuvre.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4507 2023-06-05 21:18:21.000000 flightanalysis-0.1.6/flightanalysis/schedule/schedule.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      891 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/flightanalysis/simulation.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 17:43:24.274142 flightanalysis-0.1.6/flightanalysis/state/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1689 2023-06-14 08:27:10.000000 flightanalysis-0.1.6/flightanalysis/state/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2611 2023-06-05 21:18:21.000000 flightanalysis-0.1.6/flightanalysis/state/state.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 17:43:24.274142 flightanalysis-0.1.6/flightanalysis/state/tools/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)        1 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/flightanalysis/state/tools/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4570 2023-06-14 09:02:25.000000 flightanalysis-0.1.6/flightanalysis/state/tools/alignment.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4450 2023-06-05 21:18:21.000000 flightanalysis-0.1.6/flightanalysis/state/tools/builders.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2722 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/flightanalysis/state/tools/conversions.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     3635 2023-06-14 15:40:09.000000 flightanalysis-0.1.6/flightanalysis/state/tools/dumpers.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      931 2023-06-05 21:18:21.000000 flightanalysis-0.1.6/flightanalysis/state/tools/measurements.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2966 2023-06-05 21:18:21.000000 flightanalysis-0.1.6/flightanalysis/state/tools/transformers.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 17:43:24.270142 flightanalysis-0.1.6/flightanalysis.egg-info/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1443 2023-06-14 17:43:24.000000 flightanalysis-0.1.6/flightanalysis.egg-info/PKG-INFO
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2693 2023-06-14 17:43:24.000000 flightanalysis-0.1.6/flightanalysis.egg-info/SOURCES.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)        1 2023-06-14 17:43:24.000000 flightanalysis-0.1.6/flightanalysis.egg-info/dependency_links.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       49 2023-06-14 17:43:24.000000 flightanalysis-0.1.6/flightanalysis.egg-info/requires.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       15 2023-06-14 17:43:24.000000 flightanalysis-0.1.6/flightanalysis.egg-info/top_level.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      446 2023-06-14 17:43:24.274142 flightanalysis-0.1.6/setup.cfg
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      687 2023-06-14 11:51:46.000000 flightanalysis-0.1.6/setup.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 17:43:24.274142 flightanalysis-0.1.6/tests/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      215 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/tests/test_analysis.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      402 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/tests/test_controls.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      206 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/tests/test_data.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2268 2023-03-28 15:54:19.000000 flightanalysis-0.1.6/tests/test_fc_json.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     6855 2023-06-05 21:18:18.000000 flightanalysis-0.1.6/tests/test_flightline.py
```

### Comparing `flightanalysis-0.1.5/LICENSE` & `flightanalysis-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/PKG-INFO` & `flightanalysis-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flightanalysis
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package for analysing flight data
 Home-page: https://github.com/PyFlightCoach/FlightAnalysis
 Author: Thomas David
 Author-email: thomasdavid0@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `flightanalysis-0.1.5/README.md` & `flightanalysis-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/aircraft_analysis.py` & `flightanalysis-0.1.6/flightanalysis/aircraft_analysis.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/base/collection.py` & `flightanalysis-0.1.6/flightanalysis/base/collection.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         for v in self.data.values():
             yield v
 
     def to_list(self):
         return list(self.data.values())
     
     def to_dicts(self) -> List[dict]:
-        return [v.to_dict() for v in self.data]
+        return [v.to_dict() for v in self.data.values()]
 
     def to_dict(self) -> Dict[str, dict]:
         return {k: v.to_dict() for k, v in self.data.items()}
 
     @classmethod
     def from_dicts(cls, vals: List[dict]):
         return cls([cls.VType.from_dict(**v) for v in vals])
```

### Comparing `flightanalysis-0.1.5/flightanalysis/base/constructs.py` & `flightanalysis-0.1.6/flightanalysis/base/constructs.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/base/table.py` & `flightanalysis-0.1.6/flightanalysis/base/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,21 @@
         else:
             raise AttributeError(f"Unknown column or construct {name}")
 
     def to_csv(self, filename):
         self.data.to_csv(filename)
         return filename
 
+    def to_dict(self):
+        return self.data.to_dict()
+    
+    @classmethod
+    def from_dict(Cls, data):
+        return Cls(pd.DataFrame(data))
+
     def __len__(self):
         return len(self.data)
 
 
     @property
     def duration(self):
         return self.data.index[-1] - self.data.index[0]
```

### Comparing `flightanalysis-0.1.5/flightanalysis/controls.py` & `flightanalysis-0.1.6/flightanalysis/controls.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/criteria/__init__.py` & `flightanalysis-0.1.6/flightanalysis/criteria/__init__.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/criteria/combination.py` & `flightanalysis-0.1.6/flightanalysis/criteria/combination.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 import inspect
 
 
 class Combination:
     """Handles a series of criteria assessments.
     for example a number of rolls in an element. 
     """
-    def __init__(self, desired: List[List[Number]], criteria=None):
+    def __init__(self, desired: List[List[Number]], criteria=None, scr:str=None):
         self.desired = np.array(desired)
         self.criteria = lambda x : 0.0 if criteria is None else criteria
-        
+        self.scr = scr if scr else inspect.getsourcelines(self.criteria)[0][0].split("=")[1].strip()
+
     def __getitem__(self, value: int):
         return self.desired[value]
 
     def get_errors(self, values: np.ndarray):
         """get the error between values and desired for all the options"""
         return self.desired - np.array(values)
 
@@ -33,22 +34,23 @@
         dgs = self.criteria(self.get_option_error(self.check_option(values), values))
         return Result(name, values, dgs)
 
     def to_dict(self):
         return dict(
             kind = self.__class__.__name__,
             desired = list(self.desired),
-            criteria = inspect.getsourcelines(self.criteria)[0][0].split("=")[1].strip()
+            criteria = self.scr
         )
 
     @staticmethod
     def from_dict(data:dict):
         return Combination(
             desired = np.array(data["desired"]),
-            criteria = eval(data["criteria"])
+            criteria = eval(data["criteria"]),
+            scr=data["criteria"]
         )
 
     @staticmethod
     def rolllist(rolls, reversable=True):
         rolls = [rolls, [-r for r in rolls]] if reversable else [rolls]
         return Combination(rolls)
```

### Comparing `flightanalysis-0.1.5/flightanalysis/criteria/comparison.py` & `flightanalysis-0.1.6/flightanalysis/criteria/comparison.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 import numpy as np
 import pandas as pd
 from . import Result
 from typing import Callable
 import inspect
 
 class Comparison:
-    def __init__(self, criteria: Callable, initial_value=None):
+    def __init__(self, criteria: Callable, initial_value=None, scr: str=None):
         self.criteria = criteria
         self.initial_value = initial_value
+        self.scr = scr if scr else inspect.getsourcelines(self.criteria)[0][0].split("=")[1].strip()
 
     def lookup(self,value):
         try:
             return self.criteria(value)
         except IndexError:
             raise ValueError(f"The requested ratio of {value} is not present in levels {self.levels}")
             
@@ -28,19 +29,20 @@
             ratios,
             self.lookup(np.abs(ratios))
         )
 
     def to_dict(self):
         return dict(
             kind = self.__class__.__name__,
-            criteria = inspect.getsourcelines(self.criteria)[0][0].split("=")[1].strip(),
+            criteria = self.scr,
             initial_value = self.initial_value
         )
 
     @staticmethod
     def from_dict(data:dict):
         return Comparison(
             eval(data["criteria"]),
-            initial_value = data["initial_value"]
+            initial_value = data["initial_value"],
+            scr=data["criteria"]
         )
```

### Comparing `flightanalysis-0.1.5/flightanalysis/criteria/continuous.py` & `flightanalysis-0.1.6/flightanalysis/criteria/continuous.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,21 +19,23 @@
         arr = arr.to_numpy()
     peaks = arr[get_peak_locs(arr)]
     troughs = arr[get_peak_locs(arr, True)]
     return np.abs(peaks) - np.abs(troughs)
 
 
 class Continuous:
-    def __init__(self,  lookup: Callable, preprocess: Callable=None): 
+    def __init__(self,  lookup: Callable, preprocess: Callable=None, slu:str=None, spp:str=None): 
         self.lookup = lookup
+        self.slu=slu if slu else inspect.getsourcelines(self.lookup)[0][0].split("=")[1].strip()
         if preprocess is None:
             self.preprocess = lambda x: x
         else:
             self.preprocess = preprocess
-
+        self.spp=spp if spp else inspect.getsourcelines(self.preprocess)[0][0].split("=")[1].strip()
+        
     def __call__(self, name, data: pd.Series, pp: bool=True):
         pdata = self.preprocess(data) if pp else data
         peak_locs = get_peak_locs(pdata)
         trough_locs = get_peak_locs(pdata, True)
 
         mistakes = pdata[peak_locs] - pdata[trough_locs]
 
@@ -45,14 +47,19 @@
             errors,  
             downgrades 
         )
 
     def to_dict(self):
         return dict(
             kind = self.__class__.__name__,
-            lookup = inspect.getsourcelines(self.criteria)[0][0].split("=")[1].strip(),
-            preprocess = inspect.getsourcelines(self.criteria)[0][0].split("=")[1].strip()
+            lookup = self.slu,
+            preprocess = self.spp
         )
 
     @staticmethod
     def from_dict(data:dict):
-        return Continuous(eval(data["lookup"]),eval(data["preprocess"]))
+        return Continuous(
+            eval(data["lookup"]),
+            eval(data["preprocess"]),
+            data["lookup"],
+            data["preprocess"]
+        )
```

### Comparing `flightanalysis-0.1.5/flightanalysis/criteria/results.py` & `flightanalysis-0.1.6/flightanalysis/criteria/results.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/criteria/single.py` & `flightanalysis-0.1.6/flightanalysis/criteria/single.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,36 +4,43 @@
 from .results import Result, Results
 import inspect
 
 
 class Single:
     """This class creates a function to return a result for a set of errors. 
     """
-    def __init__(self, lookup: Callable, preprocess: Callable=None):
+    def __init__(self, lookup: Callable, preprocess: Callable=None, slu=None, spp=None):
         """
         Args:
             lookup (Callable): a function that returns a score for a given error
             preprocess (Callable, optional): A function to apply to the input value to return the error.
         """
         self.lookup = lookup        
+        self.slu=slu if slu else inspect.getsourcelines(self.lookup)[0][0].split("=")[1].strip()
+
         if preprocess is None:
             self.preprocess = lambda x: x
         else:
             self.preprocess = preprocess
-    
+        self.spp=spp if spp else inspect.getsourcelines(self.preprocess)[0][0].split("=")[1].strip()
+
     def __call__(self, name: str, data: np.ndarray, pp = True) -> List[float]:
         """get a Result object for a set of errors."""
         pdata = self.preprocess(data) if pp else data
         return Result(name,data,self.lookup(pdata))
 
     def to_dict(self):
         return dict(
             kind = self.__class__.__name__,
-            lookup = inspect.getsourcelines(self.criteria)[0][0].split("=")[1].strip(),
-            preprocess = inspect.getsourcelines(self.criteria)[0][0].split("=")[1].strip()
+            lookup = self.slu,
+            preprocess = self.spp
         )
 
     @staticmethod
     def from_dict(data:dict):
-        return Single(eval(data["lookup"]),eval(data["preprocess"]))
-    
+        return Single(
+            eval(data["lookup"]),
+            eval(data["preprocess"]),
+            data["lookup"],
+            data["preprocess"]
+        )
```

### Comparing `flightanalysis-0.1.5/flightanalysis/data/f25.json` & `flightanalysis-0.1.6/flightanalysis/data/f25.json`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/data/p23.json` & `flightanalysis-0.1.6/flightanalysis/data/p23.json`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/data/p25.json` & `flightanalysis-0.1.6/flightanalysis/data/p25.json`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/environment/environment.py` & `flightanalysis-0.1.6/flightanalysis/environment/environment.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/environment/wind.py` & `flightanalysis-0.1.6/flightanalysis/environment/wind.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/fc_score.py` & `flightanalysis-0.1.6/flightanalysis/fc_score.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from json import load
+from flightanalysis.base import Collection
 from flightanalysis.state import State
 from flightanalysis.flightline import Box
 from flightanalysis.data import get_schedule_definition
 from flightanalysis.schedule import *
 from flightdata import Flight
 from geometry import Transformation, Quaternion, Q0
 import numpy as np
@@ -25,14 +26,39 @@
 
         #TODO factor by visibility, replace abs here with something cleverer. Add some logic to the arbitrary fudge factors
         self.pos_dg = np.cumsum(abs(self.pos_error) * self.aligned.dt / 500)
         self.roll_dg = np.cumsum(np.abs(self.roll_error) * self.aligned.dt / 40)
 
         self.score = 10 - self.pos_dg[-1] - self.roll_dg[-1]
     
+    def to_dict(self):
+        return dict(
+            mdef = self.mdef.to_dict(),
+            aligned = self.aligned.to_dict(),
+            intended = self.intended.to_dict(),
+            intended_template = self.intended_template.to_dict(),
+            corrected = self.corrected.to_dict(),
+            corrected_template = self.corrected_template.to_dict(),
+        )
+
+    @staticmethod
+    def from_dict(data:dict):
+        return ManoeuvreAnalysis(
+            ManDef.from_dict(data["mdef"]),
+            State.from_dict(data["aligned"]),
+            Manoeuvre.from_dict(data["intended"]),
+            State.from_dict(data["intended_template"]),
+            Manoeuvre.from_dict(data["corrected"]),
+            State.from_dict(data["corrected_template"]),
+        )
+
+    @property
+    def uid(self):
+        return self.mdef.uid
+
     @staticmethod
     def build(mdef: ManDef, flown: State):
 
         itrans = Transformation(
             flown[0].pos,
             mdef.info.start.initial_rotation(
                 mdef.info.start.d.get_wind(flown.direction()[0])
@@ -59,15 +85,15 @@
         mdef.mps.update_defaults(intended)       
 
         corr = Manoeuvre(intended.entry_line, mdef._create().elements, mdef.info.short_name)
         corr_tp = corr.create_template(itrans, aligned)
         
         return ManoeuvreAnalysis(mdef, aligned, intended, int_tp, corr, corr_tp)
 
-    
+
 
 
     def plot_3d(self, **kwargs):
         fig = plotsec(self.aligned, color="red", **kwargs)
         return plotsec(self.corrected_template, color="green", fig=fig, **kwargs)
 
     def plot_dg(self):
@@ -83,14 +109,29 @@
             ), 
             yaxis2=dict(title="roll error",
                 overlaying="y",
                 side="right",)
         )
         fig.show()
 
+class ScheduleAnalysis(Collection):
+    VType=ManoeuvreAnalysis
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+    def summary_df(self):
+        return pd.DataFrame(
+            [[an.mdef.info.short_name, an.mdef.info.k, an.score] for an in self], 
+            columns=["name", "k", "score"]
+        )
+
+    def total_score(self):
+        df = self.summary_df()
+        return sum(df.k * df.score)
 
 
 if __name__ == "__main__":
     with open("examples/data/manual_F3A_P23_22_05_31_00000350.json", "r") as f:
         data = load(f)
 
 
@@ -99,15 +140,15 @@
     state = State.from_flight(flight, box).splitter_labels(data["mans"])
     sdef = get_schedule_definition(data["parameters"]["schedule"][1])
 
     analyses: List[ManoeuvreAnalysis] = []
 
     for mid in range(17):
         analyses.append(ManoeuvreAnalysis.build(sdef[mid], state.get_meid(mid+1)))
-    
+
     df = pd.DataFrame([[an.mdef.info.short_name, an.score, an.mdef.info.k] for an in analyses], columns=["name", "score", "k"])
     if "scores" in data:
         df["manual_scores"] = data["scores"][1:-1]
         
     print(df)
     print(f"total = {sum(df.score * df.k)}")
     pass
```

### Comparing `flightanalysis-0.1.5/flightanalysis/flightline.py` & `flightanalysis-0.1.6/flightanalysis/flightline.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/model/coefficients.py` & `flightanalysis-0.1.6/flightanalysis/model/coefficients.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/model/flow.py` & `flightanalysis-0.1.6/flightanalysis/model/flow.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/model/model.py` & `flightanalysis-0.1.6/flightanalysis/model/model.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/schedule/__init__.py` & `flightanalysis-0.1.6/flightanalysis/schedule/__init__.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/schedule/definition/__init__.py` & `flightanalysis-0.1.6/flightanalysis/schedule/definition/__init__.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/schedule/definition/collectors.py` & `flightanalysis-0.1.6/flightanalysis/schedule/definition/collectors.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/schedule/definition/element_builders.py` & `flightanalysis-0.1.6/flightanalysis/schedule/definition/element_builders.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/schedule/definition/element_definition.py` & `flightanalysis-0.1.6/flightanalysis/schedule/definition/element_definition.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/schedule/definition/manoeuvre_builder.py` & `flightanalysis-0.1.6/flightanalysis/schedule/definition/manoeuvre_builder.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/schedule/definition/manoeuvre_definition.py` & `flightanalysis-0.1.6/flightanalysis/schedule/definition/manoeuvre_definition.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/schedule/definition/manoeuvre_info.py` & `flightanalysis-0.1.6/flightanalysis/schedule/definition/manoeuvre_info.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/schedule/definition/manoeuvre_parameters.py` & `flightanalysis-0.1.6/flightanalysis/schedule/definition/manoeuvre_parameters.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/schedule/definition/operation.py` & `flightanalysis-0.1.6/flightanalysis/schedule/definition/operation.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/schedule/definition/schedule_definition.py` & `flightanalysis-0.1.6/flightanalysis/schedule/definition/schedule_definition.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/schedule/elements/__init__.py` & `flightanalysis-0.1.6/flightanalysis/schedule/elements/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
             return False
         return np.all([np.isclose(getattr(self, p), getattr(other, p), 0.01) for p in self.__class__.parameters])
 
     def __repr__(self):
         return dumps(self.to_dict(), indent=2)
 
     def to_dict(self):
-        return dict(type=self.__class__.__name__, **self.__dict__)
+        return dict(kind=self.__class__.__name__, **self.__dict__)
 
     def set_parms(self, **parms):
         kwargs = {k:v for k, v in self.__dict__.items() if not k[0] == "_"}
 
         for key, value in parms.items():
             if key in kwargs:
                 kwargs[key] = value
@@ -201,15 +201,15 @@
 from .autorotation import Autorotation
 
 els = {c.__name__.lower(): c for c in El.__subclasses__()}
 
 El.from_name = lambda name: els[name.lower()]
 
 def from_dict(data):
-    kind = data.pop("kind")
+    kind = data.pop("kind").lower()
     return els[kind](**data)
 
 El.from_dict = staticmethod(from_dict)
 
 def from_json(file):
     with open(file, "r") as f:
         return El.from_dict(load(f))
```

### Comparing `flightanalysis-0.1.5/flightanalysis/schedule/elements/autorotation.py` & `flightanalysis-0.1.6/flightanalysis/schedule/elements/autorotation.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,23 @@
     rather than the body x axis"""
     parameters = El.parameters + "length,roll,rate,angle".split(",")
     def __init__(self, speed: float, length: float, roll: float, uid: str):
         super().__init__(uid, speed)
         self.length = length
         self.roll = roll
     
+    def to_dict(self):
+        return dict(
+            kind=self.__class__.__name__,
+            speed=self.speed,
+            length=self.length,
+            roll=self.roll,
+            uid=self.uid
+        )
+    
     @property
     def angle(self):
         return 2 * np.pi * self.roll
 
     @property
     def rate(self):
         return self.angle * self.speed / self.length
```

### Comparing `flightanalysis-0.1.5/flightanalysis/schedule/elements/line.py` & `flightanalysis-0.1.6/flightanalysis/schedule/elements/line.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 
     def to_dict(self):
         return dict(
             kind=self.__class__.__name__,
             length=self.length,
             roll=self.roll,
             speed=self.speed,
-            rate=self.rate,
             uid=self.uid
         )
 
     @property
     def rate(self):
         return self.roll * self.speed / self.length
```

### Comparing `flightanalysis-0.1.5/flightanalysis/schedule/elements/loop.py` & `flightanalysis-0.1.6/flightanalysis/schedule/elements/loop.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/schedule/elements/nose_drop.py` & `flightanalysis-0.1.6/flightanalysis/schedule/elements/nose_drop.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,22 @@
     break_angle off the vertical line"""
     parameters = El.parameters + "radius,break_angle".split(",")
     def __init__(self, speed: float, radius: float, break_angle: float, uid: str=None):
         super().__init__(uid, speed)
         self.radius=radius
         self.break_angle = break_angle
 
+    def to_dict(self):
+        return dict(
+            kind=self.__class__.__name__,
+            speed=self.speed,
+            radius=self.radius,
+            break_angle=self.break_angle,
+            uid=self.uid
+        )
 
     def create_template(self, istate: State, time: Time=None):
         _inverted = 1 if istate.transform.rotation.is_inverted()[0] else -1
         
         alpha =  np.arctan2(istate.vel.z, istate.vel.x)[0]
 
         return Loop(self.speed, self.radius, 0.5*np.pi*_inverted).create_template(
```

### Comparing `flightanalysis-0.1.5/flightanalysis/schedule/elements/pitch_break.py` & `flightanalysis-0.1.6/flightanalysis/schedule/elements/pitch_break.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,24 @@
 class PitchBreak(El):
     parameters = El.parameters + "length,break_angle".split(",")
     def __init__(self, speed: float, length: float, break_angle: float, uid: str=None):
         super().__init__(uid, speed)
         self.length=length
         self.break_angle = break_angle
 
+    def to_dict(self):
+        return dict(
+            kind=self.__class__.__name__,
+            speed=self.speed,
+            length=self.length,
+            break_angle=self.break_angle,
+            uid=self.uid
+        )
+
+
     def create_template(self, istate: State, time: Time=None):
 
         return Line(self.speed, self.length).create_template(
             istate, 
             time
         ).superimpose_rotation(
             PY(),
```

### Comparing `flightanalysis-0.1.5/flightanalysis/schedule/elements/recovery.py` & `flightanalysis-0.1.6/flightanalysis/schedule/elements/recovery.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,18 +9,23 @@
 
 class Recovery(El):
     parameters = El.parameters + ["length"]
     def __init__(self, speed, length, uid: str=None):
         super().__init__(uid, speed)
         self.length = length
 
-    def create_template(self, istate: State, time: Time=None):
-        
-
+    def to_dict(self):
+        return dict(
+            kind=self.__class__.__name__,
+            speed=self.speed,
+            length=self.length,
+            uid=self.uid
+        )
 
+    def create_template(self, istate: State, time: Time=None):
         return Line(self.speed, self.length).create_template(
             istate, 
             time
         ).superimpose_rotation(
             PY(),
             -np.arctan2(istate.vel.z, istate.vel.x)[-1]
         ).label(element=self.uid)
```

### Comparing `flightanalysis-0.1.5/flightanalysis/schedule/elements/stall_turn.py` & `flightanalysis-0.1.6/flightanalysis/schedule/elements/stall_turn.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/schedule/manoeuvre.py` & `flightanalysis-0.1.6/flightanalysis/schedule/manoeuvre.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,21 @@
     def from_dict(data):
         return Manoeuvre(
             Line.from_dict(data["entry_line"]),
             Elements.from_dicts(data["elements"]),
             data["uid"]
         )
 
+    def to_dict(self):
+        return dict(
+            entry_line=self.entry_line.to_dict(),
+            elements=self.elements.to_dicts(),
+            uid=self.uid
+        )
+
     @staticmethod
     def from_all_elements(uid:str, els: List[El]):
         return Manoeuvre(els[0], els[1:], uid)
 
     def all_elements(self, exit_line=False):
         els = []
```

### Comparing `flightanalysis-0.1.5/flightanalysis/schedule/schedule.py` & `flightanalysis-0.1.6/flightanalysis/schedule/schedule.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/simulation.py` & `flightanalysis-0.1.6/flightanalysis/simulation.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/state/__init__.py` & `flightanalysis-0.1.6/flightanalysis/state/__init__.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/state/state.py` & `flightanalysis-0.1.6/flightanalysis/state/state.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/state/tools/alignment.py` & `flightanalysis-0.1.6/flightanalysis/state/tools/alignment.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/state/tools/builders.py` & `flightanalysis-0.1.6/flightanalysis/state/tools/builders.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/state/tools/conversions.py` & `flightanalysis-0.1.6/flightanalysis/state/tools/conversions.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/state/tools/dumpers.py` & `flightanalysis-0.1.6/flightanalysis/state/tools/dumpers.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/state/tools/measurements.py` & `flightanalysis-0.1.6/flightanalysis/state/tools/measurements.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis/state/tools/transformers.py` & `flightanalysis-0.1.6/flightanalysis/state/tools/transformers.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/flightanalysis.egg-info/PKG-INFO` & `flightanalysis-0.1.6/flightanalysis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flightanalysis
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package for analysing flight data
 Home-page: https://github.com/PyFlightCoach/FlightAnalysis
 Author: Thomas David
 Author-email: thomasdavid0@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `flightanalysis-0.1.5/flightanalysis.egg-info/SOURCES.txt` & `flightanalysis-0.1.6/flightanalysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/setup.py` & `flightanalysis-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/tests/test_fc_json.py` & `flightanalysis-0.1.6/tests/test_fc_json.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.5/tests/test_flightline.py` & `flightanalysis-0.1.6/tests/test_flightline.py`

 * *Files identical despite different names*

