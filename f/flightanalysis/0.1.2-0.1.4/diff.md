# Comparing `tmp/flightanalysis-0.1.2.tar.gz` & `tmp/flightanalysis-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flightanalysis-0.1.2.tar", last modified: Wed Jun 14 11:11:33 2023, max compression
+gzip compressed data, was "flightanalysis-0.1.4.tar", last modified: Wed Jun 14 12:08:46 2023, max compression
```

## Comparing `flightanalysis-0.1.2.tar` & `flightanalysis-0.1.4.tar`

### file list

```diff
@@ -1,93 +1,90 @@
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 11:11:33.663910 flightanalysis-0.1.2/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)    35149 2023-03-28 15:54:19.000000 flightanalysis-0.1.2/LICENSE
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      111 2023-06-14 11:06:49.000000 flightanalysis-0.1.2/MANIFEST.in
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1443 2023-06-14 11:11:33.663910 flightanalysis-0.1.2/PKG-INFO
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1160 2023-03-28 15:54:19.000000 flightanalysis-0.1.2/README.md
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 11:11:33.659910 flightanalysis-0.1.2/flightanalysis/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      261 2023-03-28 15:54:19.000000 flightanalysis-0.1.2/flightanalysis/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     3609 2023-03-28 15:54:19.000000 flightanalysis-0.1.2/flightanalysis/aircraft_analysis.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 11:11:33.659910 flightanalysis-0.1.2/flightanalysis/base/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       65 2023-03-28 15:54:19.000000 flightanalysis-0.1.2/flightanalysis/base/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2565 2023-06-05 21:18:21.000000 flightanalysis-0.1.2/flightanalysis/base/collection.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2178 2023-06-13 10:36:02.000000 flightanalysis-0.1.2/flightanalysis/base/constructs.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      221 2023-03-28 15:54:19.000000 flightanalysis-0.1.2/flightanalysis/base/numpy_encoder.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     5286 2023-06-13 11:47:30.000000 flightanalysis-0.1.2/flightanalysis/base/table.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1693 2023-06-05 21:18:21.000000 flightanalysis-0.1.2/flightanalysis/controls.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 11:11:33.659910 flightanalysis-0.1.2/flightanalysis/criteria/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1454 2023-03-28 15:54:19.000000 flightanalysis-0.1.2/flightanalysis/criteria/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2350 2023-03-28 15:54:19.000000 flightanalysis-0.1.2/flightanalysis/criteria/combination.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1324 2023-03-28 15:54:19.000000 flightanalysis-0.1.2/flightanalysis/criteria/comparison.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2013 2023-03-28 15:54:19.000000 flightanalysis-0.1.2/flightanalysis/criteria/continuous.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      925 2023-03-28 15:54:19.000000 flightanalysis-0.1.2/flightanalysis/criteria/results.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1341 2023-06-05 21:18:21.000000 flightanalysis-0.1.2/flightanalysis/criteria/single.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 11:11:33.659910 flightanalysis-0.1.2/flightanalysis/data/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      279 2023-06-05 21:18:21.000000 flightanalysis-0.1.2/flightanalysis/data/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)    79839 2023-06-14 11:06:35.000000 flightanalysis-0.1.2/flightanalysis/data/f25.json
--rw-rw-r--   0 td6834    (1001) td6834    (1001)    10240 2023-06-14 11:06:29.000000 flightanalysis-0.1.2/flightanalysis/data/f25.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)    70673 2023-06-14 11:05:48.000000 flightanalysis-0.1.2/flightanalysis/data/p23.json
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     8236 2023-06-14 11:05:42.000000 flightanalysis-0.1.2/flightanalysis/data/p23.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)    73755 2023-06-14 11:05:11.000000 flightanalysis-0.1.2/flightanalysis/data/p25.json
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     8437 2023-06-14 11:05:32.000000 flightanalysis-0.1.2/flightanalysis/data/p25.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 11:11:33.659910 flightanalysis-0.1.2/flightanalysis/environment/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       91 2023-03-28 15:54:19.000000 flightanalysis-0.1.2/flightanalysis/environment/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1393 2023-06-05 21:18:21.000000 flightanalysis-0.1.2/flightanalysis/environment/environment.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4345 2023-03-28 15:54:19.000000 flightanalysis-0.1.2/flightanalysis/environment/wind.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      466 2023-06-13 14:30:47.000000 flightanalysis-0.1.2/flightanalysis/fc_json.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4174 2023-06-14 09:43:36.000000 flightanalysis-0.1.2/flightanalysis/fc_score.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     7725 2023-06-05 21:18:18.000000 flightanalysis-0.1.2/flightanalysis/flightline.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 11:11:33.659910 flightanalysis-0.1.2/flightanalysis/model/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      108 2023-03-28 15:54:19.000000 flightanalysis-0.1.2/flightanalysis/model/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1179 2023-06-05 21:18:21.000000 flightanalysis-0.1.2/flightanalysis/model/coefficients.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      405 2023-03-28 15:54:19.000000 flightanalysis-0.1.2/flightanalysis/model/constants.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1377 2023-06-05 21:18:21.000000 flightanalysis-0.1.2/flightanalysis/model/flow.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      675 2023-03-28 15:54:19.000000 flightanalysis-0.1.2/flightanalysis/model/model.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 11:11:33.663910 flightanalysis-0.1.2/flightanalysis/schedule/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2888 2023-06-13 12:22:27.000000 flightanalysis-0.1.2/flightanalysis/schedule/__init__.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 11:11:33.663910 flightanalysis-0.1.2/flightanalysis/schedule/definition/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      695 2023-06-05 21:18:21.000000 flightanalysis-0.1.2/flightanalysis/schedule/definition/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1482 2023-06-06 05:23:48.000000 flightanalysis-0.1.2/flightanalysis/schedule/definition/collectors.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     6382 2023-06-13 08:53:43.000000 flightanalysis-0.1.2/flightanalysis/schedule/definition/element_builders.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4907 2023-06-05 21:18:21.000000 flightanalysis-0.1.2/flightanalysis/schedule/definition/element_definition.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4658 2023-06-14 07:40:53.000000 flightanalysis-0.1.2/flightanalysis/schedule/definition/manoeuvre_builder.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     5202 2023-06-13 12:23:31.000000 flightanalysis-0.1.2/flightanalysis/schedule/definition/manoeuvre_definition.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4126 2023-06-05 21:18:21.000000 flightanalysis-0.1.2/flightanalysis/schedule/definition/manoeuvre_info.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     6220 2023-06-13 12:59:23.000000 flightanalysis-0.1.2/flightanalysis/schedule/definition/manoeuvre_parameters.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     7430 2023-06-06 05:26:36.000000 flightanalysis-0.1.2/flightanalysis/schedule/definition/operation.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1959 2023-06-14 11:04:57.000000 flightanalysis-0.1.2/flightanalysis/schedule/definition/schedule_definition.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 11:11:33.663910 flightanalysis-0.1.2/flightanalysis/schedule/elements/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     7335 2023-06-13 12:21:00.000000 flightanalysis-0.1.2/flightanalysis/schedule/elements/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1749 2023-06-13 12:17:45.000000 flightanalysis-0.1.2/flightanalysis/schedule/elements/autorotation.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     3397 2023-06-13 12:16:23.000000 flightanalysis-0.1.2/flightanalysis/schedule/elements/line.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     6341 2023-06-13 12:18:07.000000 flightanalysis-0.1.2/flightanalysis/schedule/elements/loop.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1844 2023-06-13 12:18:45.000000 flightanalysis-0.1.2/flightanalysis/schedule/elements/nose_drop.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1357 2023-06-13 12:19:01.000000 flightanalysis-0.1.2/flightanalysis/schedule/elements/pitch_break.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1109 2023-06-13 12:19:11.000000 flightanalysis-0.1.2/flightanalysis/schedule/elements/recovery.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1685 2023-06-13 12:21:37.000000 flightanalysis-0.1.2/flightanalysis/schedule/elements/stall_turn.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     3929 2023-06-13 12:27:56.000000 flightanalysis-0.1.2/flightanalysis/schedule/manoeuvre.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4507 2023-06-05 21:18:21.000000 flightanalysis-0.1.2/flightanalysis/schedule/schedule.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      891 2023-03-28 15:54:19.000000 flightanalysis-0.1.2/flightanalysis/simulation.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 11:11:33.663910 flightanalysis-0.1.2/flightanalysis/state/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1689 2023-06-14 08:27:10.000000 flightanalysis-0.1.2/flightanalysis/state/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2611 2023-06-05 21:18:21.000000 flightanalysis-0.1.2/flightanalysis/state/state.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 11:11:33.663910 flightanalysis-0.1.2/flightanalysis/state/tools/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)        1 2023-03-28 15:54:19.000000 flightanalysis-0.1.2/flightanalysis/state/tools/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4570 2023-06-14 09:02:25.000000 flightanalysis-0.1.2/flightanalysis/state/tools/alignment.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4450 2023-06-05 21:18:21.000000 flightanalysis-0.1.2/flightanalysis/state/tools/builders.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2722 2023-03-28 15:54:19.000000 flightanalysis-0.1.2/flightanalysis/state/tools/conversions.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     3635 2023-06-05 21:18:21.000000 flightanalysis-0.1.2/flightanalysis/state/tools/dumpers.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      931 2023-06-05 21:18:21.000000 flightanalysis-0.1.2/flightanalysis/state/tools/measurements.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2966 2023-06-05 21:18:21.000000 flightanalysis-0.1.2/flightanalysis/state/tools/transformers.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 11:11:33.659910 flightanalysis-0.1.2/flightanalysis.egg-info/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1443 2023-06-14 11:11:33.000000 flightanalysis-0.1.2/flightanalysis.egg-info/PKG-INFO
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2774 2023-06-14 11:11:33.000000 flightanalysis-0.1.2/flightanalysis.egg-info/SOURCES.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)        1 2023-06-14 11:11:33.000000 flightanalysis-0.1.2/flightanalysis.egg-info/dependency_links.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       49 2023-06-14 11:11:33.000000 flightanalysis-0.1.2/flightanalysis.egg-info/requires.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       15 2023-06-14 11:11:33.000000 flightanalysis-0.1.2/flightanalysis.egg-info/top_level.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      418 2023-06-14 11:11:33.663910 flightanalysis-0.1.2/setup.cfg
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      672 2023-03-28 15:54:19.000000 flightanalysis-0.1.2/setup.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 11:11:33.663910 flightanalysis-0.1.2/tests/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      215 2023-03-28 15:54:19.000000 flightanalysis-0.1.2/tests/test_analysis.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      402 2023-03-28 15:54:19.000000 flightanalysis-0.1.2/tests/test_controls.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      206 2023-03-28 15:54:19.000000 flightanalysis-0.1.2/tests/test_data.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2268 2023-03-28 15:54:19.000000 flightanalysis-0.1.2/tests/test_fc_json.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     6855 2023-06-05 21:18:18.000000 flightanalysis-0.1.2/tests/test_flightline.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 12:08:46.372161 flightanalysis-0.1.4/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)    35149 2023-03-28 15:54:19.000000 flightanalysis-0.1.4/LICENSE
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       34 2023-06-14 11:48:20.000000 flightanalysis-0.1.4/MANIFEST.in
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1443 2023-06-14 12:08:46.372161 flightanalysis-0.1.4/PKG-INFO
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1160 2023-03-28 15:54:19.000000 flightanalysis-0.1.4/README.md
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 12:08:46.368161 flightanalysis-0.1.4/flightanalysis/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      261 2023-03-28 15:54:19.000000 flightanalysis-0.1.4/flightanalysis/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     3609 2023-03-28 15:54:19.000000 flightanalysis-0.1.4/flightanalysis/aircraft_analysis.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 12:08:46.368161 flightanalysis-0.1.4/flightanalysis/base/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       65 2023-03-28 15:54:19.000000 flightanalysis-0.1.4/flightanalysis/base/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2565 2023-06-05 21:18:21.000000 flightanalysis-0.1.4/flightanalysis/base/collection.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2178 2023-06-13 10:36:02.000000 flightanalysis-0.1.4/flightanalysis/base/constructs.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      221 2023-03-28 15:54:19.000000 flightanalysis-0.1.4/flightanalysis/base/numpy_encoder.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     5286 2023-06-13 11:47:30.000000 flightanalysis-0.1.4/flightanalysis/base/table.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1693 2023-06-05 21:18:21.000000 flightanalysis-0.1.4/flightanalysis/controls.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 12:08:46.368161 flightanalysis-0.1.4/flightanalysis/criteria/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1454 2023-03-28 15:54:19.000000 flightanalysis-0.1.4/flightanalysis/criteria/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2350 2023-03-28 15:54:19.000000 flightanalysis-0.1.4/flightanalysis/criteria/combination.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1324 2023-03-28 15:54:19.000000 flightanalysis-0.1.4/flightanalysis/criteria/comparison.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2013 2023-03-28 15:54:19.000000 flightanalysis-0.1.4/flightanalysis/criteria/continuous.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      925 2023-03-28 15:54:19.000000 flightanalysis-0.1.4/flightanalysis/criteria/results.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1341 2023-06-05 21:18:21.000000 flightanalysis-0.1.4/flightanalysis/criteria/single.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 12:08:46.368161 flightanalysis-0.1.4/flightanalysis/data/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      293 2023-06-14 12:08:11.000000 flightanalysis-0.1.4/flightanalysis/data/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)    79839 2023-06-14 11:06:35.000000 flightanalysis-0.1.4/flightanalysis/data/f25.json
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)    70673 2023-06-14 11:05:48.000000 flightanalysis-0.1.4/flightanalysis/data/p23.json
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)    73755 2023-06-14 11:05:11.000000 flightanalysis-0.1.4/flightanalysis/data/p25.json
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 12:08:46.368161 flightanalysis-0.1.4/flightanalysis/environment/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       91 2023-03-28 15:54:19.000000 flightanalysis-0.1.4/flightanalysis/environment/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1393 2023-06-05 21:18:21.000000 flightanalysis-0.1.4/flightanalysis/environment/environment.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4345 2023-03-28 15:54:19.000000 flightanalysis-0.1.4/flightanalysis/environment/wind.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      466 2023-06-13 14:30:47.000000 flightanalysis-0.1.4/flightanalysis/fc_json.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4174 2023-06-14 09:43:36.000000 flightanalysis-0.1.4/flightanalysis/fc_score.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     7725 2023-06-05 21:18:18.000000 flightanalysis-0.1.4/flightanalysis/flightline.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 12:08:46.368161 flightanalysis-0.1.4/flightanalysis/model/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      108 2023-03-28 15:54:19.000000 flightanalysis-0.1.4/flightanalysis/model/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1179 2023-06-05 21:18:21.000000 flightanalysis-0.1.4/flightanalysis/model/coefficients.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      405 2023-03-28 15:54:19.000000 flightanalysis-0.1.4/flightanalysis/model/constants.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1377 2023-06-05 21:18:21.000000 flightanalysis-0.1.4/flightanalysis/model/flow.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      675 2023-03-28 15:54:19.000000 flightanalysis-0.1.4/flightanalysis/model/model.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 12:08:46.368161 flightanalysis-0.1.4/flightanalysis/schedule/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2888 2023-06-13 12:22:27.000000 flightanalysis-0.1.4/flightanalysis/schedule/__init__.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 12:08:46.368161 flightanalysis-0.1.4/flightanalysis/schedule/definition/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      695 2023-06-05 21:18:21.000000 flightanalysis-0.1.4/flightanalysis/schedule/definition/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1482 2023-06-06 05:23:48.000000 flightanalysis-0.1.4/flightanalysis/schedule/definition/collectors.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     6382 2023-06-13 08:53:43.000000 flightanalysis-0.1.4/flightanalysis/schedule/definition/element_builders.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4907 2023-06-05 21:18:21.000000 flightanalysis-0.1.4/flightanalysis/schedule/definition/element_definition.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4658 2023-06-14 07:40:53.000000 flightanalysis-0.1.4/flightanalysis/schedule/definition/manoeuvre_builder.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     5202 2023-06-13 12:23:31.000000 flightanalysis-0.1.4/flightanalysis/schedule/definition/manoeuvre_definition.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4126 2023-06-05 21:18:21.000000 flightanalysis-0.1.4/flightanalysis/schedule/definition/manoeuvre_info.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     6220 2023-06-13 12:59:23.000000 flightanalysis-0.1.4/flightanalysis/schedule/definition/manoeuvre_parameters.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     7430 2023-06-06 05:26:36.000000 flightanalysis-0.1.4/flightanalysis/schedule/definition/operation.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1959 2023-06-14 11:04:57.000000 flightanalysis-0.1.4/flightanalysis/schedule/definition/schedule_definition.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 12:08:46.372161 flightanalysis-0.1.4/flightanalysis/schedule/elements/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     7335 2023-06-13 12:21:00.000000 flightanalysis-0.1.4/flightanalysis/schedule/elements/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1749 2023-06-13 12:17:45.000000 flightanalysis-0.1.4/flightanalysis/schedule/elements/autorotation.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     3397 2023-06-13 12:16:23.000000 flightanalysis-0.1.4/flightanalysis/schedule/elements/line.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     6341 2023-06-13 12:18:07.000000 flightanalysis-0.1.4/flightanalysis/schedule/elements/loop.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1844 2023-06-13 12:18:45.000000 flightanalysis-0.1.4/flightanalysis/schedule/elements/nose_drop.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1357 2023-06-13 12:19:01.000000 flightanalysis-0.1.4/flightanalysis/schedule/elements/pitch_break.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1109 2023-06-13 12:19:11.000000 flightanalysis-0.1.4/flightanalysis/schedule/elements/recovery.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1685 2023-06-13 12:21:37.000000 flightanalysis-0.1.4/flightanalysis/schedule/elements/stall_turn.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     3929 2023-06-13 12:27:56.000000 flightanalysis-0.1.4/flightanalysis/schedule/manoeuvre.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4507 2023-06-05 21:18:21.000000 flightanalysis-0.1.4/flightanalysis/schedule/schedule.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      891 2023-03-28 15:54:19.000000 flightanalysis-0.1.4/flightanalysis/simulation.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 12:08:46.372161 flightanalysis-0.1.4/flightanalysis/state/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1689 2023-06-14 08:27:10.000000 flightanalysis-0.1.4/flightanalysis/state/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2611 2023-06-05 21:18:21.000000 flightanalysis-0.1.4/flightanalysis/state/state.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 12:08:46.372161 flightanalysis-0.1.4/flightanalysis/state/tools/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)        1 2023-03-28 15:54:19.000000 flightanalysis-0.1.4/flightanalysis/state/tools/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4570 2023-06-14 09:02:25.000000 flightanalysis-0.1.4/flightanalysis/state/tools/alignment.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4450 2023-06-05 21:18:21.000000 flightanalysis-0.1.4/flightanalysis/state/tools/builders.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2722 2023-03-28 15:54:19.000000 flightanalysis-0.1.4/flightanalysis/state/tools/conversions.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     3635 2023-06-05 21:18:21.000000 flightanalysis-0.1.4/flightanalysis/state/tools/dumpers.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      931 2023-06-05 21:18:21.000000 flightanalysis-0.1.4/flightanalysis/state/tools/measurements.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2966 2023-06-05 21:18:21.000000 flightanalysis-0.1.4/flightanalysis/state/tools/transformers.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 12:08:46.368161 flightanalysis-0.1.4/flightanalysis.egg-info/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1443 2023-06-14 12:08:46.000000 flightanalysis-0.1.4/flightanalysis.egg-info/PKG-INFO
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2693 2023-06-14 12:08:46.000000 flightanalysis-0.1.4/flightanalysis.egg-info/SOURCES.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)        1 2023-06-14 12:08:46.000000 flightanalysis-0.1.4/flightanalysis.egg-info/dependency_links.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       49 2023-06-14 12:08:46.000000 flightanalysis-0.1.4/flightanalysis.egg-info/requires.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       15 2023-06-14 12:08:46.000000 flightanalysis-0.1.4/flightanalysis.egg-info/top_level.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      446 2023-06-14 12:08:46.372161 flightanalysis-0.1.4/setup.cfg
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      687 2023-06-14 11:51:46.000000 flightanalysis-0.1.4/setup.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 12:08:46.372161 flightanalysis-0.1.4/tests/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      215 2023-03-28 15:54:19.000000 flightanalysis-0.1.4/tests/test_analysis.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      402 2023-03-28 15:54:19.000000 flightanalysis-0.1.4/tests/test_controls.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      206 2023-03-28 15:54:19.000000 flightanalysis-0.1.4/tests/test_data.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2268 2023-03-28 15:54:19.000000 flightanalysis-0.1.4/tests/test_fc_json.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     6855 2023-06-05 21:18:18.000000 flightanalysis-0.1.4/tests/test_flightline.py
```

### Comparing `flightanalysis-0.1.2/LICENSE` & `flightanalysis-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/PKG-INFO` & `flightanalysis-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flightanalysis
-Version: 0.1.2
+Version: 0.1.4
 Summary: A package for analysing flight data
 Home-page: https://github.com/PyFlightCoach/FlightAnalysis
 Author: Thomas David
 Author-email: thomasdavid0@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `flightanalysis-0.1.2/README.md` & `flightanalysis-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/aircraft_analysis.py` & `flightanalysis-0.1.4/flightanalysis/aircraft_analysis.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/base/collection.py` & `flightanalysis-0.1.4/flightanalysis/base/collection.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/base/constructs.py` & `flightanalysis-0.1.4/flightanalysis/base/constructs.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/base/table.py` & `flightanalysis-0.1.4/flightanalysis/base/table.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/controls.py` & `flightanalysis-0.1.4/flightanalysis/controls.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/criteria/__init__.py` & `flightanalysis-0.1.4/flightanalysis/criteria/__init__.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/criteria/combination.py` & `flightanalysis-0.1.4/flightanalysis/criteria/combination.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/criteria/comparison.py` & `flightanalysis-0.1.4/flightanalysis/criteria/comparison.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/criteria/continuous.py` & `flightanalysis-0.1.4/flightanalysis/criteria/continuous.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/criteria/results.py` & `flightanalysis-0.1.4/flightanalysis/criteria/results.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/criteria/single.py` & `flightanalysis-0.1.4/flightanalysis/criteria/single.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/data/f25.json` & `flightanalysis-0.1.4/flightanalysis/data/f25.json`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/data/p23.json` & `flightanalysis-0.1.4/flightanalysis/data/p23.json`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/data/p25.json` & `flightanalysis-0.1.4/flightanalysis/data/p25.json`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/environment/environment.py` & `flightanalysis-0.1.4/flightanalysis/environment/environment.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/environment/wind.py` & `flightanalysis-0.1.4/flightanalysis/environment/wind.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/fc_score.py` & `flightanalysis-0.1.4/flightanalysis/fc_score.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/flightline.py` & `flightanalysis-0.1.4/flightanalysis/flightline.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/model/coefficients.py` & `flightanalysis-0.1.4/flightanalysis/model/coefficients.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/model/flow.py` & `flightanalysis-0.1.4/flightanalysis/model/flow.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/model/model.py` & `flightanalysis-0.1.4/flightanalysis/model/model.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/schedule/__init__.py` & `flightanalysis-0.1.4/flightanalysis/schedule/__init__.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/schedule/definition/__init__.py` & `flightanalysis-0.1.4/flightanalysis/schedule/definition/__init__.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/schedule/definition/collectors.py` & `flightanalysis-0.1.4/flightanalysis/schedule/definition/collectors.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/schedule/definition/element_builders.py` & `flightanalysis-0.1.4/flightanalysis/schedule/definition/element_builders.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/schedule/definition/element_definition.py` & `flightanalysis-0.1.4/flightanalysis/schedule/definition/element_definition.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/schedule/definition/manoeuvre_builder.py` & `flightanalysis-0.1.4/flightanalysis/schedule/definition/manoeuvre_builder.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/schedule/definition/manoeuvre_definition.py` & `flightanalysis-0.1.4/flightanalysis/schedule/definition/manoeuvre_definition.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/schedule/definition/manoeuvre_info.py` & `flightanalysis-0.1.4/flightanalysis/schedule/definition/manoeuvre_info.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/schedule/definition/manoeuvre_parameters.py` & `flightanalysis-0.1.4/flightanalysis/schedule/definition/manoeuvre_parameters.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/schedule/definition/operation.py` & `flightanalysis-0.1.4/flightanalysis/schedule/definition/operation.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/schedule/definition/schedule_definition.py` & `flightanalysis-0.1.4/flightanalysis/schedule/definition/schedule_definition.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/schedule/elements/__init__.py` & `flightanalysis-0.1.4/flightanalysis/schedule/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/schedule/elements/autorotation.py` & `flightanalysis-0.1.4/flightanalysis/schedule/elements/autorotation.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/schedule/elements/line.py` & `flightanalysis-0.1.4/flightanalysis/schedule/elements/line.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/schedule/elements/loop.py` & `flightanalysis-0.1.4/flightanalysis/schedule/elements/loop.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/schedule/elements/nose_drop.py` & `flightanalysis-0.1.4/flightanalysis/schedule/elements/nose_drop.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/schedule/elements/pitch_break.py` & `flightanalysis-0.1.4/flightanalysis/schedule/elements/pitch_break.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/schedule/elements/recovery.py` & `flightanalysis-0.1.4/flightanalysis/schedule/elements/recovery.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/schedule/elements/stall_turn.py` & `flightanalysis-0.1.4/flightanalysis/schedule/elements/stall_turn.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/schedule/manoeuvre.py` & `flightanalysis-0.1.4/flightanalysis/schedule/manoeuvre.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/schedule/schedule.py` & `flightanalysis-0.1.4/flightanalysis/schedule/schedule.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/simulation.py` & `flightanalysis-0.1.4/flightanalysis/simulation.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/state/__init__.py` & `flightanalysis-0.1.4/flightanalysis/state/__init__.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/state/state.py` & `flightanalysis-0.1.4/flightanalysis/state/state.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/state/tools/alignment.py` & `flightanalysis-0.1.4/flightanalysis/state/tools/alignment.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/state/tools/builders.py` & `flightanalysis-0.1.4/flightanalysis/state/tools/builders.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/state/tools/conversions.py` & `flightanalysis-0.1.4/flightanalysis/state/tools/conversions.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/state/tools/dumpers.py` & `flightanalysis-0.1.4/flightanalysis/state/tools/dumpers.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/state/tools/measurements.py` & `flightanalysis-0.1.4/flightanalysis/state/tools/measurements.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis/state/tools/transformers.py` & `flightanalysis-0.1.4/flightanalysis/state/tools/transformers.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/flightanalysis.egg-info/PKG-INFO` & `flightanalysis-0.1.4/flightanalysis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flightanalysis
-Version: 0.1.2
+Version: 0.1.4
 Summary: A package for analysing flight data
 Home-page: https://github.com/PyFlightCoach/FlightAnalysis
 Author: Thomas David
 Author-email: thomasdavid0@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `flightanalysis-0.1.2/flightanalysis.egg-info/SOURCES.txt` & `flightanalysis-0.1.4/flightanalysis.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -24,19 +24,16 @@
 flightanalysis/criteria/combination.py
 flightanalysis/criteria/comparison.py
 flightanalysis/criteria/continuous.py
 flightanalysis/criteria/results.py
 flightanalysis/criteria/single.py
 flightanalysis/data/__init__.py
 flightanalysis/data/f25.json
-flightanalysis/data/f25.py
 flightanalysis/data/p23.json
-flightanalysis/data/p23.py
 flightanalysis/data/p25.json
-flightanalysis/data/p25.py
 flightanalysis/environment/__init__.py
 flightanalysis/environment/environment.py
 flightanalysis/environment/wind.py
 flightanalysis/model/__init__.py
 flightanalysis/model/coefficients.py
 flightanalysis/model/constants.py
 flightanalysis/model/flow.py
```

### Comparing `flightanalysis-0.1.2/setup.py` & `flightanalysis-0.1.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,10 +7,10 @@
 ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 You should have received a copy of the GNU General Public License along with
 this program. If not, see <http://www.gnu.org/licenses/>.
 """
 
 
-from setuptools import setup
+from setuptools import setup, find_packages
 
 setup()
```

### Comparing `flightanalysis-0.1.2/tests/test_fc_json.py` & `flightanalysis-0.1.4/tests/test_fc_json.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.1.2/tests/test_flightline.py` & `flightanalysis-0.1.4/tests/test_flightline.py`

 * *Files identical despite different names*

