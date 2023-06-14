# Comparing `tmp/dyntapy-0.2.2.tar.gz` & `tmp/dyntapy-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyntapy-0.2.2.tar", last modified: Tue Jun 28 14:00:00 2022, max compression
+gzip compressed data, was "dyntapy-0.2.3.tar", last modified: Thu Sep  8 12:35:47 2022, max compression
```

## Comparing `dyntapy-0.2.2.tar` & `dyntapy-0.2.3.tar`

### file list

```diff
@@ -1,63 +1,59 @@
-drwxrwxr-x   0 portmann  (1000) portmann  (1000)        0 2022-06-28 14:00:00.529208 dyntapy-0.2.2/
--rw-rw-r--   0 portmann  (1000) portmann  (1000)    35131 2022-03-02 10:07:03.000000 dyntapy-0.2.2/LICENSE.txt
--rw-rw-r--   0 portmann  (1000) portmann  (1000)       55 2022-03-02 10:09:57.000000 dyntapy-0.2.2/MANIFEST.in
--rw-rw-r--   0 portmann  (1000) portmann  (1000)      998 2022-06-28 14:00:00.529208 dyntapy-0.2.2/PKG-INFO
-drwxrwxr-x   0 portmann  (1000) portmann  (1000)        0 2022-06-28 14:00:00.505208 dyntapy-0.2.2/dyntapy/
--rw-rw-r--   0 portmann  (1000) portmann  (1000)     1051 2022-06-28 12:40:05.000000 dyntapy-0.2.2/dyntapy/__init__.py
--rw-rw-r--   0 portmann  (1000) portmann  (1000)      506 2022-01-18 10:31:45.000000 dyntapy-0.2.2/dyntapy/_context.py
--rw-rw-r--   0 portmann  (1000) portmann  (1000)    11528 2022-04-12 11:43:15.000000 dyntapy-0.2.2/dyntapy/assignments.py
--rw-rw-r--   0 portmann  (1000) portmann  (1000)     8681 2022-03-10 12:18:14.000000 dyntapy-0.2.2/dyntapy/csr.py
--rw-rw-r--   0 portmann  (1000) portmann  (1000)    12757 2022-03-10 09:20:03.000000 dyntapy-0.2.2/dyntapy/demand.py
--rw-rw-r--   0 portmann  (1000) portmann  (1000)    29677 2022-06-27 12:52:55.000000 dyntapy-0.2.2/dyntapy/demand_data.py
-drwxrwxr-x   0 portmann  (1000) portmann  (1000)        0 2022-06-28 14:00:00.509208 dyntapy-0.2.2/dyntapy/dta/
--rw-rw-r--   0 portmann  (1000) portmann  (1000)      313 2021-10-27 20:35:36.000000 dyntapy-0.2.2/dyntapy/dta/__init__.py
--rw-rw-r--   0 portmann  (1000) portmann  (1000)     8900 2022-03-09 17:13:53.000000 dyntapy-0.2.2/dyntapy/dta/aon.py
--rw-rw-r--   0 portmann  (1000) portmann  (1000)    12276 2022-03-09 17:13:53.000000 dyntapy-0.2.2/dyntapy/dta/debugging.py
--rw-rw-r--   0 portmann  (1000) portmann  (1000)    12950 2022-03-09 16:23:31.000000 dyntapy-0.2.2/dyntapy/dta/deterministic.py
--rw-rw-r--   0 portmann  (1000) portmann  (1000)     2194 2022-01-18 10:31:45.000000 dyntapy-0.2.2/dyntapy/dta/dynamic_dijkstra.py
--rw-rw-r--   0 portmann  (1000) portmann  (1000)    33542 2022-03-09 16:23:31.000000 dyntapy-0.2.2/dyntapy/dta/i_ltm.py
--rw-rw-r--   0 portmann  (1000) portmann  (1000)     7246 2022-03-09 17:13:53.000000 dyntapy-0.2.2/dyntapy/dta/i_ltm_aon.py
--rw-rw-r--   0 portmann  (1000) portmann  (1000)     6151 2022-03-09 17:13:53.000000 dyntapy-0.2.2/dyntapy/dta/i_ltm_cls.py
--rw-rw-r--   0 portmann  (1000) portmann  (1000)     6993 2022-03-09 16:23:31.000000 dyntapy-0.2.2/dyntapy/dta/i_ltm_setup.py
--rw-rw-r--   0 portmann  (1000) portmann  (1000)     3958 2022-03-09 17:13:53.000000 dyntapy-0.2.2/dyntapy/dta/incremental_assignment.py
--rw-rw-r--   0 portmann  (1000) portmann  (1000)     8467 2022-03-09 14:50:29.000000 dyntapy-0.2.2/dyntapy/dta/orca_nodel_model.py
--rw-rw-r--   0 portmann  (1000) portmann  (1000)     8788 2022-03-09 16:23:31.000000 dyntapy-0.2.2/dyntapy/dta/qr_projection.py
--rw-rw-r--   0 portmann  (1000) portmann  (1000)     8762 2022-03-07 17:47:59.000000 dyntapy-0.2.2/dyntapy/dta/travel_times.py
--rw-rw-r--   0 portmann  (1000) portmann  (1000)    13176 2022-03-10 17:46:19.000000 dyntapy-0.2.2/dyntapy/graph_utils.py
--rw-rw-r--   0 portmann  (1000) portmann  (1000)    15795 2022-03-10 17:46:12.000000 dyntapy-0.2.2/dyntapy/results.py
--rw-rw-r--   0 portmann  (1000) portmann  (1000)     7727 2022-06-28 12:27:19.000000 dyntapy-0.2.2/dyntapy/settings.py
-drwxrwxr-x   0 portmann  (1000) portmann  (1000)        0 2022-06-28 14:00:00.513208 dyntapy-0.2.2/dyntapy/sta/
--rw-rw-r--   0 portmann  (1000) portmann  (1000)      313 2021-10-27 20:35:36.000000 dyntapy-0.2.2/dyntapy/sta/__init__.py
--rw-rw-r--   0 portmann  (1000) portmann  (1000)    14673 2022-06-28 12:28:40.000000 dyntapy-0.2.2/dyntapy/sta/dial_b.py
--rw-rw-r--   0 portmann  (1000) portmann  (1000)    18816 2022-06-28 12:28:25.000000 dyntapy-0.2.2/dyntapy/sta/equilibrate_bush.py
--rw-rw-r--   0 portmann  (1000) portmann  (1000)     1879 2022-01-18 10:31:44.000000 dyntapy-0.2.2/dyntapy/sta/gap.py
--rw-rw-r--   0 portmann  (1000) portmann  (1000)     2850 2022-03-09 16:00:37.000000 dyntapy-0.2.2/dyntapy/sta/msa.py
--rw-rw-r--   0 portmann  (1000) portmann  (1000)     6223 2022-03-10 16:07:12.000000 dyntapy-0.2.2/dyntapy/sta/uncongested_dial.py
--rw-rw-r--   0 portmann  (1000) portmann  (1000)     3268 2022-06-28 09:18:01.000000 dyntapy-0.2.2/dyntapy/sta/utilities.py
--rw-rw-r--   0 portmann  (1000) portmann  (1000)    10048 2022-03-14 14:31:09.000000 dyntapy-0.2.2/dyntapy/supply.py
--rw-rw-r--   0 portmann  (1000) portmann  (1000)    28935 2022-06-09 14:43:53.000000 dyntapy-0.2.2/dyntapy/supply_data.py
-drwxrwxr-x   0 portmann  (1000) portmann  (1000)        0 2022-06-28 14:00:00.529208 dyntapy-0.2.2/dyntapy/toy_networks/
--rw-rw-r--   0 portmann  (1000) portmann  (1000)  2130306 2022-01-18 10:31:45.000000 dyntapy-0.2.2/dyntapy/toy_networks/birmingham_net.tntp
--rw-rw-r--   0 portmann  (1000) portmann  (1000)   566619 2022-01-18 10:31:45.000000 dyntapy-0.2.2/dyntapy/toy_networks/birmingham_node.tntp
--rw-rw-r--   0 portmann  (1000) portmann  (1000)  1630299 2022-01-18 10:31:45.000000 dyntapy-0.2.2/dyntapy/toy_networks/chicagoregional_net.tntp
--rw-rw-r--   0 portmann  (1000) portmann  (1000)   261525 2022-01-18 10:31:45.000000 dyntapy-0.2.2/dyntapy/toy_networks/chicagoregional_node.tntp
--rw-rw-r--   0 portmann  (1000) portmann  (1000)   121396 2022-01-18 10:31:45.000000 dyntapy-0.2.2/dyntapy/toy_networks/chicagosketch_net.tntp
--rw-rw-r--   0 portmann  (1000) portmann  (1000)    19496 2022-01-18 10:31:45.000000 dyntapy-0.2.2/dyntapy/toy_networks/chicagosketch_node.tntp
--rw-rw-r--   0 portmann  (1000) portmann  (1000)     3136 2022-01-18 10:31:45.000000 dyntapy-0.2.2/dyntapy/toy_networks/siouxfalls_net.tntp
--rw-rw-r--   0 portmann  (1000) portmann  (1000)      719 2022-01-18 10:31:45.000000 dyntapy-0.2.2/dyntapy/toy_networks/siouxfalls_node.tntp
--rw-rw-r--   0 portmann  (1000) portmann  (1000)     4843 2022-01-18 10:31:44.000000 dyntapy-0.2.2/dyntapy/utilities.py
--rw-rw-r--   0 portmann  (1000) portmann  (1000)    31633 2022-06-15 10:56:39.000000 dyntapy-0.2.2/dyntapy/visualization.py
-drwxrwxr-x   0 portmann  (1000) portmann  (1000)        0 2022-06-28 14:00:00.505208 dyntapy-0.2.2/dyntapy.egg-info/
--rw-rw-r--   0 portmann  (1000) portmann  (1000)      998 2022-06-28 13:59:59.000000 dyntapy-0.2.2/dyntapy.egg-info/PKG-INFO
--rw-rw-r--   0 portmann  (1000) portmann  (1000)     1447 2022-06-28 14:00:00.000000 dyntapy-0.2.2/dyntapy.egg-info/SOURCES.txt
--rw-rw-r--   0 portmann  (1000) portmann  (1000)        1 2022-06-28 14:00:00.000000 dyntapy-0.2.2/dyntapy.egg-info/dependency_links.txt
--rw-rw-r--   0 portmann  (1000) portmann  (1000)      117 2022-06-28 14:00:00.000000 dyntapy-0.2.2/dyntapy.egg-info/requires.txt
--rw-rw-r--   0 portmann  (1000) portmann  (1000)        8 2022-06-28 14:00:00.000000 dyntapy-0.2.2/dyntapy.egg-info/top_level.txt
--rw-rw-r--   0 portmann  (1000) portmann  (1000)       38 2022-06-28 14:00:00.529208 dyntapy-0.2.2/setup.cfg
--rw-rw-r--   0 portmann  (1000) portmann  (1000)     2074 2022-06-28 13:56:38.000000 dyntapy-0.2.2/setup.py
-drwxrwxr-x   0 portmann  (1000) portmann  (1000)        0 2022-06-28 14:00:00.529208 dyntapy-0.2.2/tests/
--rw-rw-r--   0 portmann  (1000) portmann  (1000)      579 2022-06-24 16:48:18.000000 dyntapy-0.2.2/tests/current_tests.py
--rw-rw-r--   0 portmann  (1000) portmann  (1000)     1837 2022-03-09 13:43:35.000000 dyntapy-0.2.2/tests/simple_bottleneck.py
--rw-rw-r--   0 portmann  (1000) portmann  (1000)     1887 2022-03-09 13:43:35.000000 dyntapy-0.2.2/tests/simple_diverge.py
--rw-rw-r--   0 portmann  (1000) portmann  (1000)     1889 2022-03-09 13:43:35.000000 dyntapy-0.2.2/tests/simple_merge.py
--rw-rw-r--   0 portmann  (1000) portmann  (1000)     7999 2022-06-27 09:31:30.000000 dyntapy-0.2.2/tests/test_dyntapy.py
+drwxrwxr-x   0 portmann  (1000) portmann  (1000)        0 2022-09-08 12:35:47.355442 dyntapy-0.2.3/
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)    35131 2022-07-22 14:17:21.000000 dyntapy-0.2.3/LICENSE.txt
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)       55 2022-07-22 14:17:21.000000 dyntapy-0.2.3/MANIFEST.in
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)      998 2022-09-08 12:35:47.355442 dyntapy-0.2.3/PKG-INFO
+drwxrwxr-x   0 portmann  (1000) portmann  (1000)        0 2022-09-08 12:35:47.347442 dyntapy-0.2.3/dyntapy/
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)     1112 2022-09-08 11:05:07.000000 dyntapy-0.2.3/dyntapy/__init__.py
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)      506 2022-07-22 14:17:21.000000 dyntapy-0.2.3/dyntapy/_context.py
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)    12590 2022-08-23 12:11:02.000000 dyntapy-0.2.3/dyntapy/assignments.py
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)     8681 2022-07-22 14:17:21.000000 dyntapy-0.2.3/dyntapy/csr.py
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)    13052 2022-08-23 12:11:02.000000 dyntapy-0.2.3/dyntapy/demand.py
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)    29970 2022-08-23 12:11:02.000000 dyntapy-0.2.3/dyntapy/demand_data.py
+drwxrwxr-x   0 portmann  (1000) portmann  (1000)        0 2022-09-08 12:35:47.347442 dyntapy-0.2.3/dyntapy/dta/
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)      313 2022-07-22 14:17:21.000000 dyntapy-0.2.3/dyntapy/dta/__init__.py
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)     8900 2022-07-22 14:17:21.000000 dyntapy-0.2.3/dyntapy/dta/aon.py
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)    12276 2022-07-22 14:17:21.000000 dyntapy-0.2.3/dyntapy/dta/debugging.py
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)    12950 2022-07-22 14:17:21.000000 dyntapy-0.2.3/dyntapy/dta/deterministic.py
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)     2213 2022-08-23 12:11:02.000000 dyntapy-0.2.3/dyntapy/dta/dynamic_dijkstra.py
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)    33542 2022-07-22 14:17:21.000000 dyntapy-0.2.3/dyntapy/dta/i_ltm.py
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)     7246 2022-07-22 14:17:21.000000 dyntapy-0.2.3/dyntapy/dta/i_ltm_aon.py
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)     6151 2022-07-22 14:17:21.000000 dyntapy-0.2.3/dyntapy/dta/i_ltm_cls.py
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)     6993 2022-07-22 14:17:21.000000 dyntapy-0.2.3/dyntapy/dta/i_ltm_setup.py
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)     4755 2022-08-23 12:11:02.000000 dyntapy-0.2.3/dyntapy/dta/incremental_assignment.py
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)     8467 2022-07-22 14:17:21.000000 dyntapy-0.2.3/dyntapy/dta/orca_nodel_model.py
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)     8788 2022-07-22 14:17:21.000000 dyntapy-0.2.3/dyntapy/dta/qr_projection.py
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)     9295 2022-08-23 12:11:02.000000 dyntapy-0.2.3/dyntapy/dta/travel_times.py
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)    14507 2022-08-23 12:11:02.000000 dyntapy-0.2.3/dyntapy/graph_utils.py
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)    15795 2022-07-22 14:17:21.000000 dyntapy-0.2.3/dyntapy/results.py
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)     8034 2022-09-08 12:16:17.000000 dyntapy-0.2.3/dyntapy/settings.py
+drwxrwxr-x   0 portmann  (1000) portmann  (1000)        0 2022-09-08 12:35:47.351442 dyntapy-0.2.3/dyntapy/sta/
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)      313 2022-07-22 14:17:21.000000 dyntapy-0.2.3/dyntapy/sta/__init__.py
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)     1728 2022-09-08 11:25:38.000000 dyntapy-0.2.3/dyntapy/sta/_debugging_sta.py
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)    14673 2022-08-23 12:11:02.000000 dyntapy-0.2.3/dyntapy/sta/dial_b.py
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)     8697 2022-08-23 12:11:02.000000 dyntapy-0.2.3/dyntapy/sta/dial_stochastic_assignment.py
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)    18854 2022-08-23 12:11:02.000000 dyntapy-0.2.3/dyntapy/sta/equilibrate_bush.py
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)     1879 2022-07-22 14:17:21.000000 dyntapy-0.2.3/dyntapy/sta/gap.py
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)     2850 2022-07-22 14:17:21.000000 dyntapy-0.2.3/dyntapy/sta/msa.py
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)     5107 2022-08-23 12:11:02.000000 dyntapy-0.2.3/dyntapy/sta/uncongested_dial.py
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)     6543 2022-09-08 11:25:39.000000 dyntapy-0.2.3/dyntapy/sta/utilities.py
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)    10048 2022-07-22 14:17:21.000000 dyntapy-0.2.3/dyntapy/supply.py
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)    28984 2022-08-23 12:11:02.000000 dyntapy-0.2.3/dyntapy/supply_data.py
+drwxrwxr-x   0 portmann  (1000) portmann  (1000)        0 2022-09-08 12:35:47.355442 dyntapy-0.2.3/dyntapy/toy_networks/
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)  2130306 2022-07-22 14:17:21.000000 dyntapy-0.2.3/dyntapy/toy_networks/birmingham_net.tntp
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)   566619 2022-07-22 14:17:21.000000 dyntapy-0.2.3/dyntapy/toy_networks/birmingham_node.tntp
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)  1630299 2022-07-22 14:17:21.000000 dyntapy-0.2.3/dyntapy/toy_networks/chicagoregional_net.tntp
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)   261525 2022-07-22 14:17:21.000000 dyntapy-0.2.3/dyntapy/toy_networks/chicagoregional_node.tntp
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)   121396 2022-07-22 14:17:21.000000 dyntapy-0.2.3/dyntapy/toy_networks/chicagosketch_net.tntp
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)    19496 2022-07-22 14:17:21.000000 dyntapy-0.2.3/dyntapy/toy_networks/chicagosketch_node.tntp
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)     3136 2022-07-22 14:17:21.000000 dyntapy-0.2.3/dyntapy/toy_networks/siouxfalls_net.tntp
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)      719 2022-07-22 14:17:21.000000 dyntapy-0.2.3/dyntapy/toy_networks/siouxfalls_node.tntp
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)     4843 2022-07-22 14:17:21.000000 dyntapy-0.2.3/dyntapy/utilities.py
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)    32483 2022-09-08 12:16:48.000000 dyntapy-0.2.3/dyntapy/visualization.py
+drwxrwxr-x   0 portmann  (1000) portmann  (1000)        0 2022-09-08 12:35:47.347442 dyntapy-0.2.3/dyntapy.egg-info/
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)      998 2022-09-08 12:35:47.000000 dyntapy-0.2.3/dyntapy.egg-info/PKG-INFO
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)     1401 2022-09-08 12:35:47.000000 dyntapy-0.2.3/dyntapy.egg-info/SOURCES.txt
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)        1 2022-09-08 12:35:47.000000 dyntapy-0.2.3/dyntapy.egg-info/dependency_links.txt
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)      117 2022-09-08 12:35:47.000000 dyntapy-0.2.3/dyntapy.egg-info/requires.txt
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)        8 2022-09-08 12:35:47.000000 dyntapy-0.2.3/dyntapy.egg-info/top_level.txt
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)       38 2022-09-08 12:35:47.355442 dyntapy-0.2.3/setup.cfg
+-rw-rw-r--   0 portmann  (1000) portmann  (1000)     2074 2022-09-08 12:28:16.000000 dyntapy-0.2.3/setup.py
```

### Comparing `dyntapy-0.2.2/LICENSE.txt` & `dyntapy-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dyntapy-0.2.2/PKG-INFO` & `dyntapy-0.2.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyntapy
-Version: 0.2.2
+Version: 0.2.3
 Summary: Macroscopic Static and Dynamic Traffic Assignment in Python 
 Home-page: https://gitlab.kuleuven.be/ITSCreaLab/public-toolboxes/dyntapy
 Author: Paul Ortmann
 Author-email: itscrealab@kuleuven.be
 License: GPLv3
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyntapy-0.2.2/dyntapy/__init__.py` & `dyntapy-0.2.3/dyntapy/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,26 +3,29 @@
 #  License: GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007, see license.txt
 #  More information at: https://gitlab.mech.kuleuven.be/ITSCreaLab
 #  or contact: ITScrealab@kuleuven.be
 #
 #
 #
 
-__version__ = "0.2.2"
+__version__ = "0.2.3"
+
 # expose major functionality in dyntapy namespace such
 # that dyntapy.function() can be called directly
 from .assignments import DynamicAssignment, StaticAssignment
 from .demand_data import (
     add_centroids,
     add_connectors,
     auto_configured_centroids,
     find_nearest_centroids,
     generate_random_od_graph,
     get_centroid_grid_coords,
     _places_around_place,
+    od_graph_from_matrix,
+    od_matrix_from_dataframes,
 )
 from .graph_utils import get_shortest_paths, get_all_shortest_paths
 from .results import StaticResult, DynamicResult
 from .supply_data import relabel_graph, road_network_from_place, get_toy_network
 from .visualization import (
     show_demand,
     show_dynamic_network,
```

### Comparing `dyntapy-0.2.2/dyntapy/assignments.py` & `dyntapy-0.2.3/dyntapy/assignments.py`

 * *Files 9% similar despite different names*

```diff
@@ -81,17 +81,17 @@
 import dyntapy._context
 from dyntapy.demand import (
     InternalDynamicDemand,
     build_internal_static_demand,
     build_internal_dynamic_demand,
 )
 from dyntapy.demand_data import _check_centroid_connectivity
-from dyntapy.dta.aon import aon
 from dyntapy.dta.i_ltm_aon import i_ltm_aon
 from dyntapy.dta.incremental_assignment import incremental
+from dyntapy.sta.dial_stochastic_assignment import dial_sue
 from dyntapy.sta.dial_b import dial_b
 from dyntapy.sta.msa import msa_flow_averaging
 from dyntapy.sta.uncongested_dial import sun
 from dyntapy.supply_data import build_network
 from dyntapy.utilities import log
 from dyntapy.results import StaticResult, get_skim, DynamicResult
 
@@ -133,15 +133,15 @@
 
     def run(self, method: str = "i_ltm_aon"):
         """
 
         Parameters
         ----------
 
-        method: {'i_ltm_aon','incremental_assignment', 'aon'}
+        method: {'i_ltm_aon','incremental_assignment'}
 
         Returns
         -------
 
         dyntapy.results.DynamicResult
 
         Notes
@@ -155,15 +155,14 @@
         'i_ltm_aon' refers to a dynamic deterministic user equilibrium solution,
         note that for congested networks this is not guaranteed to converge below a
         gap of 0.01.
 
         'incremental_assignment' assigns the demands in chunks and updates the
         both costs and route choice after each DNL.
 
-        'aon' simply assigns all demand at free flow costs and executes one DNL.
 
         References
         ----------
 
         .. [1] Himpe, Willem, Ruben Corthout, and MJ Chris Tampère.
             ‘An Efficient Iterative Link Transmission Model’. Transportation Research
             Part B: Methodological 92 (2016): 170–90.
@@ -181,17 +180,19 @@
             # can be imported and used for visualization of interim computational
             # states
         )
         # TODO: add option to return iterations
         methods = {
             "i_ltm_aon": i_ltm_aon,
             "incremental_assignment": incremental,
-            "aon": aon,
         }
         if method in methods:
+            # check for turn connectors, they are required since this algorithm
+            # is defined on the line graph
+            assert _turn_connectors(self.internal_network)
             result = methods[method](
                 self.internal_network, self.internal_dynamic_demand, self.time
             )
 
         else:
             raise NotImplementedError(f"{method=} is not defined ")
         return DynamicResult(**result)
@@ -225,53 +226,51 @@
         self.od_graph = od_graph
         self.internal_demand = build_internal_static_demand(od_graph)
         self.result = None
         self.iterations = None
         log("Assignment object initialized!")
         print("init passed successfully")
 
-    def run(self, method, store_iterations=False):
+    def run(self, method, store_iterations=False, **kwargs):
         """
 
         Parameters
         ----------
 
-        method : {'dial_b','frank_wolfe', 'msa', 'sun'}
+        method : {'dial_b', 'msa', 'sun', 'sue'}
         store_iterations : bool
             set to True to get information on the individual iterations
 
         Returns
         -------
 
         dyntapy.results.StaticResult
         list of dyntapy.results.StaticResult, optional
             intermediate computation states
 
         Notes
         -----
 
-        'msa', 'frank_wolfe' and 'dial_b' all try to find the static deterministic
+        'msa' and 'dial_b' try to find the static deterministic
         user equilibrium.
 
         'msa' refers to the Method of Successive Averages, a well known method in
         Traffic Assignments that tends to zig-zag around equilibrium.
 
-        'frank_wolfe' refers to the Frank-Wolfe Algorithm.
 
         'dial_b' refers to Dial's Algorithm B, a bush-based assignment
-        algorithm. It alleviates the rather slow convergence of the Frank-Wolfe
-        algorithm close to equilibrium, see [3]_.
+        algorithm [3]_. 
 
         'sun' returns a stochastic uncongested assignment of flows on the free-flow
         travel times that are determined by the lengths and speeds of the links. It
         is based on Dial's method, see [4]_. It does not consider the whole path set
         and rests the definition of 'efficient links' to allow for computations on an
         acyclic graph.
 
-        'sun', 'frank_wolfe' and 'msa' are included for educational use.
+        'sun' and 'msa' are included for educational use.
 
         'dial_b' has been optimized and converges quickly even for
         large networks with thousands of links.
 
         References
         ----------
 
@@ -329,14 +328,42 @@
                 costs,
                 flows,
                 self.internal_demand.origins,
                 self.internal_demand.destinations,
                 skim=get_skim(costs, self.internal_demand, self.internal_network),
                 origin_flows=origin_flows,
             )
+        elif method == "sue":
+            assert not store_iterations  # not supported for SUE yet
+            # check for turn connectors, they are required since this algorithm
+            # is defined on the line graph
+            assert _turn_connectors(self.internal_network)
+            costs, flows, destination_flows = dial_sue(
+                network=self.internal_network, demand=self.internal_demand, **kwargs
+            )
+            result = StaticResult(
+                costs,
+                flows,
+                self.internal_demand.origins,
+                self.internal_demand.destinations,
+                skim=get_skim(costs, self.internal_demand, self.internal_network),
+                destination_flows=destination_flows,
+            )
 
         else:
             raise NotImplementedError(f"{method=} is not defined ")
         if not store_iterations:
             return result
         else:
             return result, dyntapy._context.iteration_states
+
+
+def _turn_connectors(network):
+    # whether the network has turn connectors
+    # just a basic check for a single centroid/ connector combo
+    origin = 0
+    link = network.nodes.out_links.get_nnz(origin)[0]
+    next_link = network.links.out_turns.get_row(link)[0]
+    if network.links.link_type[next_link] == 1:
+        return True
+    else:
+        return False
```

### Comparing `dyntapy-0.2.2/dyntapy/csr.py` & `dyntapy-0.2.3/dyntapy/csr.py`

 * *Files identical despite different names*

### Comparing `dyntapy-0.2.2/dyntapy/demand.py` & `dyntapy-0.2.3/dyntapy/demand.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,20 @@
 
     See Also
     --------
 
     dyntapy.demand.InternalStaticDemand
 
     """
-    lil_demand = nx.to_scipy_sparse_matrix(od_graph, weight="flow", format="lil")
+    try:
+        # available since networkx version 2.7.0, February 2022
+        lil_demand = nx.to_scipy_sparse_array(od_graph, weight="flow", format="lil")
+    except AttributeError:
+        # will be deprecated for networkx 3.0
+        lil_demand = nx.to_scipy_sparse_matrix(od_graph, weight="flow", format="lil")
     tot_centroids = od_graph.number_of_nodes()
     row = np.asarray(lil_demand.nonzero()[0])
     col = np.asarray(lil_demand.nonzero()[1])
     vals = np.asarray(lil_demand.tocsr().data, dtype=np.float32)
 
     intra_zonal = []
     for idx, (r, c, v) in enumerate(zip(row, col, vals)):
@@ -372,23 +377,24 @@
         dtype=np.uint32,
     )
     demand_data = [
         dynamic_demand._get_sparse_repr(t) for t in dynamic_demand.insertion_times
     ]
 
     if not np.all(
-        insertion_times[1:] - insertion_times[:-1] > simulation_time.step_size
+        dynamic_demand.insertion_times[1:] - dynamic_demand.insertion_times[:-1] >=
+        simulation_time.step_size
     ):
         raise ValueError(
             "insertion times are assumed to be monotonously increasing."
             " The minimum difference between "
             "two "
             "insertions is the internal simulation time step"
         )
-    if max(insertion_times > 24):
+    if max(dynamic_demand.insertion_times > 24):
         raise ValueError("internally time is restricted to 24 hours")
 
     static_demands = List()
     rows = [
         np.asarray(lil_demand.nonzero()[0], dtype=np.uint32)
         for lil_demand in demand_data
     ]
```

### Comparing `dyntapy-0.2.2/dyntapy/demand_data.py` & `dyntapy-0.2.3/dyntapy/demand_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,25 +74,25 @@
         containing LineStrings with a 'flow' attribute
     """
     # 4326 : WGS84
     # 3857 : web mercator
     np.random.seed(seed)
     my_gdf: gpd.geodataframe.GeoDataFrame = ox.geocode_to_gdf(name)
     tot_points = (
-        20 * tot_ods
+            20 * tot_ods
     )  # could be improved by using the area ratio between bbox and polygon for scaling
     X = (
-        np.random.random(tot_points) * (my_gdf.bbox_east[0] - my_gdf.bbox_west[0])
-        + my_gdf.bbox_west[0]
+            np.random.random(tot_points) * (my_gdf.bbox_east[0] - my_gdf.bbox_west[0])
+            + my_gdf.bbox_west[0]
     )
     # np.normal.normal means uniform distribution between 0 and 1
     # , can easily be replaced (gumbel, gaussian..)
     Y = (
-        np.random.random(tot_points) * (my_gdf.bbox_north[0] - my_gdf.bbox_south[0])
-        + my_gdf.bbox_south[0]
+            np.random.random(tot_points) * (my_gdf.bbox_north[0] - my_gdf.bbox_south[0])
+            + my_gdf.bbox_south[0]
     )
     points = [Point(x, y) for x, y in zip(X, Y)]
     my_points = gpd.geoseries.GeoSeries(points, crs=4326)
     valid_points = my_points[
         my_points.within(my_gdf.loc[0, "geometry"])
     ]  # bounding box typically doesn't align
     # with polygon extend so we ought to check which points are inside
@@ -185,38 +185,41 @@
     g.add_edges_from(edges)
     return g
 
 
 default_centroid_spacing = parameters.demand.default_centroid_spacing
 
 
-def get_centroid_grid_coords(name: str, spacing=default_centroid_spacing):
+def get_centroid_grid_coords(
+        name: str, buffer_dist=0, spacing=default_centroid_spacing
+):
     """
 
     creates centroids on a grid that overlap with the polygon
     that is associated with city or region specified
 
 
     Parameters
     ----------
     name : str,
         name of the city to be used as reference polygon
+    buffer_dist: float, optional
     spacing : float, optional
         distance between two adjacent centroids on the grid
 
     Returns
     -------
     X: numpy.ndarray
         float, 1D
         lon of centroid locations
     Y: numpy.ndarray
         float, 1D
         lat of centroid locations
     """
-    my_gdf = ox.geocode_to_gdf(name)
+    my_gdf = ox.geocode_to_gdf(name, buffer_dist=buffer_dist)
     range_ns_meters = great_circle_vec(
         my_gdf.bbox_north[0],
         my_gdf.bbox_east[0],
         my_gdf.bbox_south[0],
         my_gdf.bbox_east[0],
     )
     range_ew_meters = great_circle_vec(
@@ -339,15 +342,15 @@
     if method == "turn":
         j0 = max(new_g.nodes) + 1
         for j, (u, data) in enumerate(new_centroids):
             if euclidean:
                 delta_y = 0.1  # assuming that toy networks work with unit lengths
             else:
                 delta_y = (
-                    (100 / 6378137) * 180 / np.pi
+                        (100 / 6378137) * 180 / np.pi
                 )  # placing the artificial connecting node approx. 100 meters north
             new_g.add_node(
                 j0 + j,
                 **{"x_coord": data["x_coord"], "y_coord": data["y_coord"] + delta_y},
             )
             new_g.add_edge(
                 u,
@@ -383,18 +386,18 @@
                 euclidean,
             )
 
     return new_g
 
 
 def auto_configured_centroids(
-    place,
-    buffer_dist_close,
-    buffer_dist_extended,
-    inner_city_centroid_spacing=default_centroid_spacing,
+        place,
+        buffer_dist_close,
+        buffer_dist_extended,
+        inner_city_centroid_spacing=default_centroid_spacing,
 ):
     """
     generates centroids for the inner and extended study area from OpenStreetMap.
     The inner area is filled with a grid.
     The outer buffers are queried for settlements via OSMs 'place' tag.
 
     Parameters
@@ -438,15 +441,15 @@
         place, {"place": ["city", "town"]}, buffer_dist=buffer_dist_extended
     )
     merged_gdf = pd.concat([gdf_close, gdf_extended])
     G = merged_gdf["geometry"].apply(lambda geom: geom.wkb)
     merged_gdf = merged_gdf.loc[G.drop_duplicates().index]
     merged_gdf = merged_gdf[
         merged_gdf.geometry.type == "Point"
-    ]  # considering only points
+        ]  # considering only points
     names = merged_gdf["name"].tolist()
     x_ext, y_ext = (
         merged_gdf.geometry.apply(lambda x: x.x).to_numpy(dtype=np.float64),
         merged_gdf.geometry.apply(lambda x: x.y).to_numpy(dtype=np.float64),
     )
     place_tags = merged_gdf["place"].tolist()
     place_tags = ["-" for _ in range(len(x_inner))] + place_tags
@@ -519,21 +522,21 @@
             "link_type": np.int8(-1),
         }
         new_g.add_edge(u, v, **source_data)
         new_g.add_edge(v, u, **sink_data)
 
 
 def od_matrix_from_dataframes(
-    od_table: pd.DataFrame,
-    zoning: gpd.GeoDataFrame,
-    origin_column: str,
-    destination_column: str,
-    zone_column: str,
-    flow_column: str,
-    return_relabelling=False,
+        od_table: pd.DataFrame,
+        zoning: gpd.GeoDataFrame,
+        origin_column: str,
+        destination_column: str,
+        zone_column: str,
+        flow_column: str,
+        return_relabelling=False,
 ):
     """
 
     extracts an OD matrix and X and Y coordinates as arrays from a pandas.DataFrame and
     zoning provided as a geopandas.GeoDataFrame.
 
     It is rather common to receive OD tables in the form of .csv files
@@ -573,19 +576,22 @@
 
     """
 
     tot_zones = len(set(zoning[zone_column].to_list()))
     assert len(set(zoning[zone_column].to_list())) == len(zoning[zone_column].to_list())
     # no zone should have two conflicting geometries
     mapping = dict(zip(zoning[zone_column], np.arange(tot_zones)))
+    # the mapping will always work in string space, otherwise we need to rely on
+    # consistent types between the different columns
+    str_mapping = {str(key):item for key,item in mapping.items()}
     od_table["_origin_idx"] = od_table[origin_column].apply(
-        lambda x: mapping.get(x, -1)
+        lambda x: str_mapping.get(str(x), -1)
     )
     od_table["_destination_idx"] = od_table[destination_column].apply(
-        lambda x: mapping.get(x, -1)
+        lambda x: str_mapping.get(str(x), -1)
     )
 
     od_matrix = np.zeros((tot_zones, tot_zones), dtype=np.float64)
     try:
         assert tot_zones > len(set(od_table[origin_column].to_list()))
         assert tot_zones > len(set(od_table[destination_column].to_list()))
     except AssertionError:
@@ -613,27 +619,20 @@
 
     # extracting centroid geometries from shapefile
     zoning["centroid_x"] = zoning["geometry"].apply(lambda x: x.centroid.x)
     zoning["centroid_y"] = zoning["geometry"].apply(lambda x: x.centroid.y)
     parse(od_matrix, origins, destinations, flows)
 
     if not return_relabelling:
-        return (
-            od_matrix,
-            zoning["centroid_x"].to_numpy(),
-            zoning["centroid_y"].to_numpy(),
-        )
+        return od_matrix, zoning["centroid_x"].to_numpy(), zoning[
+            "centroid_y"].to_numpy(),
 
     else:
-        return (
-            od_matrix,
-            zoning["centroid_x"].to_numpy(),
-            zoning["centroid_y"].to_numpy(),
-            mapping,
-        )
+        return od_matrix, zoning["centroid_x"].to_numpy(), zoning[
+            "centroid_y"].to_numpy(), mapping
 
 
 def parse_demand(data: str, g):
     """
     Maps travel demand to existing closest centroids in g.
     The returned demand pattern is expressed as its own directed graph.
 
@@ -849,15 +848,15 @@
 
 default_connector_speed = parameters.demand.default_connector_speed
 default_connector_capacity = parameters.demand.default_connector_capacity
 default_connector_lanes = parameters.demand.default_connector_lanes
 
 
 def _places_around_place(
-    place, buffer_dist=default_buffer_dist, tags=["city", "town", "village"]
+        place, buffer_dist=default_buffer_dist, tags=["city", "town", "village"]
 ):
     gdf = ox.geometries_from_place(place, {"place": tags}, buffer_dist=buffer_dist)
     names = gdf["name"].tolist()
     x, y = (
         gdf.geometry.apply(lambda x: x.x).to_numpy(dtype=np.float),
         gdf.geometry.apply(lambda x: x.y).to_numpy(dtype=np.float),
     )
```

### Comparing `dyntapy-0.2.2/dyntapy/dta/aon.py` & `dyntapy-0.2.3/dyntapy/dta/aon.py`

 * *Files identical despite different names*

### Comparing `dyntapy-0.2.2/dyntapy/dta/debugging.py` & `dyntapy-0.2.3/dyntapy/dta/debugging.py`

 * *Files identical despite different names*

### Comparing `dyntapy-0.2.2/dyntapy/dta/deterministic.py` & `dyntapy-0.2.3/dyntapy/dta/deterministic.py`

 * *Files identical despite different names*

### Comparing `dyntapy-0.2.2/dyntapy/dta/dynamic_dijkstra.py` & `dyntapy-0.2.3/dyntapy/dta/dynamic_dijkstra.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,28 +13,31 @@
 
 from dyntapy.csr import UI32CSRMatrix
 
 
 @njit(cache=True)
 def dijkstra(costs, in_links: UI32CSRMatrix, target, tot_nodes, is_centroid):
     """
-    typical dijkstra_with_targets implementation with heaps, fills the distances array with the results
+    typical dijkstra_with_targets implementation with heaps, fills the distances
+    array with the results
     Parameters
     ----------
     is_centroid : bool array, dim tot_nodes, true if node is centroid, false otherwise
     tot_nodes : int, number of nodes
     costs : float32 vector
     out_links : CSR matrix, fromNode x Link
     target: integer ID of target node
     Returns
     -------
     distances: array 1D, dim tot_nodes. Distances from all nodes to the target node
     """
-    # some minor adjustments from the static version to allow for the use of the csr structures
-    # also removed conditional checks/ functionality that are not needed when this is integrated into route choice
+    # some minor adjustments from the static version to allow for the use of the csr
+    # structures
+    # also removed conditional checks/ functionality that are not needed when this is
+    # integrated into route choice
     distances = np.full(tot_nodes, np.inf, dtype=np.float32)
     seen = np.copy(distances)
     my_heap = []
     seen[target] = np.float32(0)
     heap_item = (np.float32(0), np.float32(target))
     my_heap.append(heap_item)
     while my_heap:
```

### Comparing `dyntapy-0.2.2/dyntapy/dta/i_ltm.py` & `dyntapy-0.2.3/dyntapy/dta/i_ltm.py`

 * *Files identical despite different names*

### Comparing `dyntapy-0.2.2/dyntapy/dta/i_ltm_aon.py` & `dyntapy-0.2.3/dyntapy/dta/i_ltm_aon.py`

 * *Files identical despite different names*

### Comparing `dyntapy-0.2.2/dyntapy/dta/i_ltm_cls.py` & `dyntapy-0.2.3/dyntapy/dta/i_ltm_cls.py`

 * *Files identical despite different names*

### Comparing `dyntapy-0.2.2/dyntapy/dta/i_ltm_setup.py` & `dyntapy-0.2.3/dyntapy/dta/i_ltm_setup.py`

 * *Files identical despite different names*

### Comparing `dyntapy-0.2.2/dyntapy/dta/incremental_assignment.py` & `dyntapy-0.2.3/dyntapy/dta/incremental_assignment.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,38 +10,69 @@
 from dyntapy.demand import SimulationTime
 from dyntapy.dta.travel_times import cvn_to_travel_times
 from dyntapy.results import _cvn_to_flows
 from dyntapy.supply import Network
 from dyntapy.utilities import _log
 
 
+def incremental(network, dynamic_demand, time):
+    vals = _incremental(network, dynamic_demand, time)
+    attr = [
+        "link_costs",
+        "cvn_up",
+        "cvn_down",
+        "con_up",
+        "con_down",
+        "commodity_type",
+        "turning_fractions",
+        "turn_costs",
+        "flows",
+        "origins",
+        "destinations",
+    ]
+    return {k: v for k, v in zip(attr, vals)}
+
+
 @njit(cache=True)
-def incremental(
-    network: Network, dynamic_demand: InternalDynamicDemand, time: SimulationTime
+def _incremental(
+        network: Network, dynamic_demand: InternalDynamicDemand, time: SimulationTime
 ):
     iltm_state, network = i_ltm_aon_setup(network, time, dynamic_demand)
-    incremental_loading(network, time, dynamic_demand, 20, iltm_state)
+    aon_state = incremental_loading(network, time, dynamic_demand, 20, iltm_state)
     link_costs = cvn_to_travel_times(
         cvn_up=np.sum(iltm_state.cvn_up, axis=2),
         cvn_down=np.sum(iltm_state.cvn_down, axis=2),
         time=time,
         network=network,
         con_down=iltm_state.con_down,
     )
     flows = _cvn_to_flows(iltm_state.cvn_down)
-    return flows, link_costs
+
+    return (
+        link_costs,
+        iltm_state.cvn_up,
+        iltm_state.cvn_down,
+        iltm_state.con_up,
+        iltm_state.con_down,
+        'destination',
+        iltm_state.turning_fractions,
+        aon_state.turn_costs,
+        flows,
+        dynamic_demand.all_active_origins,
+        dynamic_demand.all_active_destinations,
+    )
 
 
 @njit(cache=True)
 def incremental_loading(
-    network: Network,
-    time: SimulationTime,
-    dynamic_demand: InternalDynamicDemand,
-    K,
-    iltm_state: ILTMState,
+        network: Network,
+        time: SimulationTime,
+        dynamic_demand: InternalDynamicDemand,
+        K,
+        iltm_state: ILTMState,
 ):
     """
     Parameters
     ----------
     network :
     time :
     dynamic_demand :
@@ -59,15 +90,15 @@
         # update demand such that the current slice of demand is added.
         if k == 1:
             demand_factor = np.float32(1 / K)
         else:
             demand_factor = np.float32(k / (k - 1))
         for demand in dynamic_demand.demands:
             demand.to_destinations.values = (
-                demand.to_destinations.values * demand_factor
+                    demand.to_destinations.values * demand_factor
             )
             demand.to_origins.values = demand.to_origins.values * demand_factor
         # network loading and route choice are calculated
         i_ltm(network, dynamic_demand, iltm_state, time, aon_state.turning_fractions)
         link_costs = cvn_to_travel_times(
             cvn_up=np.sum(iltm_state.cvn_up, axis=2),
             cvn_down=np.sum(iltm_state.cvn_down, axis=2),
```

### Comparing `dyntapy-0.2.2/dyntapy/dta/orca_nodel_model.py` & `dyntapy-0.2.3/dyntapy/dta/orca_nodel_model.py`

 * *Files identical despite different names*

### Comparing `dyntapy-0.2.2/dyntapy/dta/qr_projection.py` & `dyntapy-0.2.3/dyntapy/dta/qr_projection.py`

 * *Files identical despite different names*

### Comparing `dyntapy-0.2.2/dyntapy/dta/travel_times.py` & `dyntapy-0.2.3/dyntapy/dta/travel_times.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 from dyntapy.supply import Network
 
 epsilon = parameters.dynamic_assignment.network_loading.epsilon
 
 
 @njit(cache=True, parallel=True)
 def cvn_to_travel_times(
-    cvn_up: np.ndarray,
-    cvn_down: np.ndarray,
-    con_down: np.ndarray,
-    time: SimulationTime,
-    network: Network,
+        cvn_up: np.ndarray,
+        cvn_down: np.ndarray,
+        con_down: np.ndarray,
+        time: SimulationTime,
+        network: Network,
 ):
     """
     Calculates travel times per link based on
     single commodity cumulative vehicle numbers
     follows Long, Jiancheng, Ziyou Gao, and W.Y.Szeto.
     “Discretised Link Travel Time Models Based on Cumulative
     Flows: Formulations and Properties.”
@@ -64,14 +64,21 @@
                 else:
                     last_vehicle_to_enter = cvn_up[t, link]
                     if t == 0:
                         first_vehicle_to_enter = 0
                     else:
                         first_vehicle_to_enter = cvn_up[t - 1, link]
                     delta_cvn = last_vehicle_to_enter - first_vehicle_to_enter
+                    if delta_cvn == 0:
+                        # no vehicle entered during the time period, but there was
+                        # congestion downstream
+                        # we take the solution of the last time period
+                        travel_times[t, link] = travel_times[t - 1, link]
+                        continue
+
                     last_exit_time = find_exit_time(
                         last_vehicle_to_enter, cvn_down[:, link], t, time.tot_time_steps
                     )
                     if np.uint32(last_exit_time) < last_exit_time:
                         after_last_exit_interval = np.uint32(last_exit_time) + 1
                     else:
                         after_last_exit_interval = np.uint32(last_exit_time)
@@ -81,64 +88,65 @@
                         previous_interval_vehicle_travel_time = ff_tt
                     for k in range(t, after_last_exit_interval):
                         # k is the running index for intervals
                         # in which vehicles from k left the link
                         if cvn_down[k, link] > first_vehicle_to_enter_in_k:
                             if cvn_down[k, link] > last_vehicle_to_enter:
                                 vehicles_in_flow_packet = (
-                                    last_vehicle_to_enter - first_vehicle_to_enter_in_k
+                                        last_vehicle_to_enter -
+                                        first_vehicle_to_enter_in_k
                                 )
                                 vehicle_entry = t + 1
                                 if not con_down[k, link]:
                                     # if there is no congestion downstream travel times
                                     # get overestimated dramatically due to
                                     # interpolation, we apply capacity discharge
                                     current_interval_vehicle_travel_time = max(
                                         (
-                                            k
-                                            + vehicles_in_flow_packet
-                                            / network.links.capacity[link]
-                                            - vehicle_entry
+                                                k
+                                                + vehicles_in_flow_packet
+                                                / network.links.capacity[link]
+                                                - vehicle_entry
                                         )
                                         * time.step_size,
                                         ff_tt,
                                     )
                                 else:
                                     current_interval_vehicle_travel_time = max(
                                         (
-                                            k
-                                            + vehicles_in_flow_packet
-                                            / (
-                                                cvn_down[k, link]
-                                                - cvn_down[k - 1, link]
-                                            )
-                                            - vehicle_entry
+                                                k
+                                                + vehicles_in_flow_packet
+                                                / (
+                                                        cvn_down[k, link]
+                                                        - cvn_down[k - 1, link]
+                                                )
+                                                - vehicle_entry
                                         )
                                         * time.step_size,
                                         ff_tt,
                                     )
 
                             else:
                                 vehicles_in_flow_packet = (
-                                    cvn_down[k, link] - first_vehicle_to_enter_in_k
+                                        cvn_down[k, link] - first_vehicle_to_enter_in_k
                                 )
                                 vehicle_entry = find_entry_time(
                                     cvn_down[k, link], cvn_up[:, link], k
                                 )
                                 current_interval_vehicle_travel_time = max(
                                     (k + 1 - vehicle_entry) * time.step_size, ff_tt
                                 )
                             travel_time_average += (
-                                vehicles_in_flow_packet
-                                / delta_cvn
-                                * (
-                                    current_interval_vehicle_travel_time
-                                    + previous_interval_vehicle_travel_time
-                                )
-                                / 2
+                                    vehicles_in_flow_packet
+                                    / delta_cvn
+                                    * (
+                                            current_interval_vehicle_travel_time
+                                            + previous_interval_vehicle_travel_time
+                                    )
+                                    / 2
                             )
                             first_vehicle_to_enter_in_k = cvn_down[
                                 k, link
                             ]  # first vehicle of the next period
                             previous_interval_vehicle_travel_time = (
                                 current_interval_vehicle_travel_time
                             )
@@ -159,18 +167,18 @@
     # if the condition was triggered during none of the intervals
     # the vehicle must've entered during the
     # very first interval
     if interval_before_entry == -1:
         entry_time = cvn / cvn_up[0]
     else:
         entry_time = (
-            (cvn - cvn_up[interval_before_entry])
-            / (cvn_up[interval_before_entry + 1] - cvn_up[interval_before_entry])
-            + interval_before_entry
-            + 1
+                (cvn - cvn_up[interval_before_entry])
+                / (cvn_up[interval_before_entry + 1] - cvn_up[interval_before_entry])
+                + interval_before_entry
+                + 1
         )
     return entry_time
 
 
 @njit(cache=True)
 def find_exit_time(cvn: np.float32, cvn_down: np.ndarray, k: int, T: int):
     # find the time of exit of the cumulative cvn that
@@ -185,10 +193,10 @@
     # intervals the vehicle must've exited after the
     # simulation ended
     exit_interval = np.uint32(exit_interval)
     if exit_interval == T:
         return np.float32(T)  # needs to be float, consistent return type with below
     else:
         exit_time = exit_interval + (cvn - cvn_down[exit_interval - 1]) / (
-            cvn_down[exit_interval] - cvn_down[exit_interval - 1]
+                cvn_down[exit_interval] - cvn_down[exit_interval - 1]
         )
         return exit_time
```

### Comparing `dyntapy-0.2.2/dyntapy/graph_utils.py` & `dyntapy-0.2.3/dyntapy/graph_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from numba import njit
 from numba.typed import Dict, List
 
 from dyntapy.csr import UI32CSRMatrix
 from dyntapy.supply_data import build_network
 
 
+
 # store link_ids as tuple, infer from link_ids, to_node and from_node
 @njit
 def _make_out_links(links_to_include, from_node, to_node, tot_nodes):
     """
 
     creates out_links as dictionary
 
@@ -50,17 +51,26 @@
     [node_id, link_id]
 
     """
     # creates out_links as dictionary, outlink[node] = [node_id, link_id]
     out_links = Dict()
 
     star_sizes = np.zeros(tot_nodes, dtype=np.int64)
+
+    for link, include in enumerate(links_to_include):
+        i = from_node[link]
+        j = to_node[link]
+        star_sizes[i] += 1
+
+    max_out_links = np.max(star_sizes) # getting the max out_degree of nodes to limit
+    # memory usage in creation
+    star_sizes = np.zeros(tot_nodes, dtype=np.int64)
     for i in range(tot_nodes):
         out_links[i] = np.empty(
-            (20, 2), dtype=np.int64
+            (max_out_links, 2), dtype=np.int64
         )  # In traffic networks nodes should never have more than 10 outgoing edges..
     for link, include in enumerate(links_to_include):
         if include:
             i = from_node[link]
             j = to_node[link]
             out_links[i][star_sizes[i]][0] = j
             out_links[i][star_sizes[i]][1] = link
@@ -103,19 +113,27 @@
     the resulting dictionary gives access to the graph's structure as shown below
 
     >>> in_links[node_id]
     [node_id, link_id]
 
     """
     backward_star = Dict()
-    star_sizes = np.zeros(tot_nodes, dtype=np.int64)  # , dtype=int_dtype
+    star_sizes = np.zeros(tot_nodes, dtype=np.int64)
+    for link, include in enumerate(links_to_include):
+        i = from_node[link]
+        j = to_node[link]
+        star_sizes[j] += 1
+    max_in_links = np.max(star_sizes) # getting the max in_degree of nodes to limit
+    # memory usage in creation
     for i in range(tot_nodes):
         backward_star[i] = np.empty(
-            (20, 2), dtype=np.int64
-        )  # nodes in traffic networks have less than 10 outgoing edges..
+            (max_in_links, 2), dtype=np.int64
+        )
+
+    star_sizes = np.zeros(tot_nodes, dtype=np.int64)  # , dtype=int_dtype
     for link, include in enumerate(links_to_include):
         if include:
             i = from_node[link]
             j = to_node[link]
             # print(f'i: {i} j: {j} ')
             backward_star[j][star_sizes[j]][0] = i
             backward_star[j][star_sizes[j]][1] = link
@@ -167,14 +185,45 @@
             i = predecessors[j]
             path.append(_get_link_id(i, j, out_links))
             j = predecessors[j]
         link_paths.append(path)
 
     return link_paths
 
+@njit(nogil=True)
+def pred_to_path(predecessors, source, target, out_links: UI32CSRMatrix):
+    """
+    converts optimal predecessor arrays to path between source and target
+
+    Parameters
+    ----------
+    predecessors : numpy.ndarray
+        int, 1D - predecessor of each node that is closest to `source`
+    source: int
+    target: int
+    out_links: dyntapy.csr.UI32CSRMatrix
+
+    Returns
+    -------
+
+    numba.typed.List
+
+    """
+    j =target
+    path = List()
+    i = predecessors[j]
+    path.append(_get_link_id(i, j, out_links))
+    j = predecessors[j]
+
+    while j != source:
+        i = predecessors[j]
+        path.append(_get_link_id(i, j, out_links))
+        j = predecessors[j]
+
+    return path
 
 @njit(cache=True)
 def dijkstra_all(
     costs,
     out_links: UI32CSRMatrix,
     source,
     is_centroid,
```

### Comparing `dyntapy-0.2.2/dyntapy/results.py` & `dyntapy-0.2.3/dyntapy/results.py`

 * *Files identical despite different names*

### Comparing `dyntapy-0.2.2/dyntapy/settings.py` & `dyntapy-0.2.3/dyntapy/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -171,18 +171,21 @@
         "ext_id",
         "node_type",
         "ctrl_type",
         "centroid",
         "name",
         "place",
     ]
-    link_width_scaling = 0.0025
+    link_width_scaling = 0.0025  # scales the maximum link width
+    link_width_scaling_euclidean = 0.025  # scales the maximum link width for euclidean
+    link_width_min_max_ratio = 0.15  # ratio of min/max width of the links
     link_transparency = 0.8  # 1 is opaque, 0 transparent
     node_size = 6
     link_highlight_colors = [
+        "#999999",
         "#ff6ec7",
         "#6effef",
         "#7fff6e",
         "#6e7fff",
         "#ffa66e",
         "#999999",
     ]  # neon pink, cyan, lime green
@@ -224,20 +227,23 @@
 
 @dataclass
 class _Static_Assignment:
     bpr_alpha = np.double(0.15)
     bpr_beta = np.double(4)
     msa_max_iterations = 200
     msa_delta = 0.001
+    sue_dial_max_iterations = 100
+    sue_dial_gap = 0.01
     fw_max_iterations = 50
     fw_delta = 0.001
     dial_b_max_iterations = 100
     dial_b_cost_differences = 0.001  # tested for as low as 0.00001, corresponds
     # to 0.036s error
     logit_theta = 0.1
+    mu = 0.8  # used in SUE
     gap_method = "relative"
 
 
 @dataclass
 class _Parameters:
     """container for categories of parameters"""
```

### Comparing `dyntapy-0.2.2/dyntapy/sta/dial_b.py` & `dyntapy-0.2.3/dyntapy/sta/dial_b.py`

 * *Files identical despite different names*

### Comparing `dyntapy-0.2.2/dyntapy/sta/equilibrate_bush.py` & `dyntapy-0.2.3/dyntapy/sta/equilibrate_bush.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 from numba import njit
 from numba.typed import Dict
 
 from dyntapy.settings import parameters, debugging
 from dyntapy.sta.utilities import __bpr_cost_single, __bpr_derivative_single
 from dyntapy.graph_utils import _get_link_id
 
+# sub modules for Dial's Algorithm B.
+
 epsilon = parameters.static_assignment.dial_b_cost_differences
 epsilon_2 = epsilon / 20  # Epsilon that is used on an alternatives basis, replaces
-
-
 # the expansion factor in Dial's paper.
 # needs to be lower than epsilon to achieve an epsilon compliant gap across all
-# destinations
+# destinations.
 
 
 @njit
 def __equilibrate_bush(
     costs,
     bush_flows,
     origin,
```

### Comparing `dyntapy-0.2.2/dyntapy/sta/gap.py` & `dyntapy-0.2.3/dyntapy/sta/gap.py`

 * *Files identical despite different names*

### Comparing `dyntapy-0.2.2/dyntapy/sta/msa.py` & `dyntapy-0.2.3/dyntapy/sta/msa.py`

 * *Files identical despite different names*

### Comparing `dyntapy-0.2.2/dyntapy/sta/uncongested_dial.py` & `dyntapy-0.2.3/dyntapy/sta/uncongested_dial.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,24 +4,23 @@
 #  More information at: https://gitlab.mech.kuleuven.be/ITSCreaLab
 #  or contact: ITScrealab@kuleuven.be
 #
 #
 #
 from math import exp
 
-from numba import njit
 import numpy as np
 
 from dyntapy.demand import InternalStaticDemand
 from dyntapy.graph_utils import (
-    dijkstra_all,
     _make_in_links,
     _make_out_links,
 )
 from dyntapy.settings import parameters
+from dyntapy.sta.utilities import generate_bushes
 from dyntapy.supply import Network
 
 
 # since this works with topological orders the full path set is not considered.
 def sun(network: Network, demand: InternalStaticDemand):
     theta = parameters.static_assignment.logit_theta
     ff_times = network.links.length / network.links.free_speed
@@ -86,39 +85,14 @@
             from_nodes,
             to_nodes,
         )
 
     return np.sum(bush_flows, axis=0), bush_flows
 
 
-@njit
-def generate_bushes(
-    link_ff_times, from_nodes, to_nodes, out_links, demand, tot_links, is_centroid
-):
-    tot_nodes = out_links.get_nnz_rows().size
-    tot_origins = demand.to_destinations.get_nnz_rows().size
-    topological_orders = np.empty((tot_origins, tot_nodes), dtype=np.int64)
-    distances = np.empty((tot_origins, tot_nodes), np.float64)
-    links_in_bush = np.full((tot_origins, tot_links), False)
-    assert demand.to_destinations.get_nnz_rows().size > 0
-    for origin_id, origin in enumerate(demand.to_destinations.get_nnz_rows()):
-        distances[origin_id], pred = dijkstra_all(
-            costs=link_ff_times,
-            out_links=out_links,
-            source=origin,
-            is_centroid=is_centroid,
-        )
-        topological_orders[origin_id] = np.argsort(distances[origin_id])
-        label = np.argsort(topological_orders[origin_id])
-        for link_id, (i, j) in enumerate(zip(from_nodes, to_nodes)):
-            if label[j] > label[i]:
-                links_in_bush[origin_id][link_id] = True
-    return topological_orders, links_in_bush, distances
-
-
 # @njit()
 def load_bush(
     origin,
     costs,
     destinations,
     demands,
     topological_order,
```

### Comparing `dyntapy-0.2.2/dyntapy/supply.py` & `dyntapy-0.2.3/dyntapy/supply.py`

 * *Files identical despite different names*

### Comparing `dyntapy-0.2.2/dyntapy/supply_data.py` & `dyntapy-0.2.3/dyntapy/supply_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,14 @@
         if close is not None:
             g = nx.compose(inner, close)
         if extended is not None:
             g = nx.compose(g, extended)
 
         return g
 
-    log(f"city {place} could not be found in data folder, loading from osm", level=50)
     g = acquire_graph()
 
     # osmnx generates MultiDiGraphs, meaning there can
     # be more than one edge connecting i ->j, a preliminary check on
     # them shows that these edges are mostly tagged with
     # (mildly) conflicting data, e.g. slightly different linestring
     # or length for simplification we just take all the
@@ -372,15 +371,15 @@
         ]
         if len(speed_list) > 0:
             return min(speed_list)
         else:
             return default_speed
 
 
-def build_network(g):
+def build_network(g, u_turns = False):
     """
     creates internal network representation
 
     Parameters
     ----------
     g: networkx.DiGraph
         road network graph
@@ -437,15 +436,15 @@
         x_coord,
         y_coord,
     )
     log("nodes passed")
     link_type = np.array(
         [np.int8(d.get("link_type", 0)) for (_, _, d) in sorted_edges], dtype=np.int8
     )
-    turns = _build_turns(tot_nodes, nodes, link_type)
+    turns = _build_turns(tot_nodes, nodes, link_type, u_turns = False)
     log("turns passed")
 
     link_capacity = np.array(
         [d["capacity"] for (_, _, d) in sorted_edges], dtype=np.float32
     )
     free_speed = np.array(
         [d["free_speed"] for (_, _, d) in sorted_edges], dtype=np.float32
@@ -519,15 +518,15 @@
         capacity,
         is_centroid,
         x_coord,
         y_coord,
     )
 
 
-def _build_turns(tot_nodes, nodes: Nodes, link_types):
+def _build_turns(tot_nodes, nodes: Nodes, link_types, u_turns =False):
     to_nodes = List()
     from_nodes = List()
     from_links = List()
     to_links = List()
     via_nodes = List()
     turn_counter = 0
     for via_node in np.arange(tot_nodes):
@@ -539,17 +538,19 @@
         _to_nodes = nodes.out_links.get_row(via_node)
         _from_nodes = nodes.in_links.get_row(via_node)
         _from_links = nodes.in_links.get_nnz(via_node)
         _to_links = nodes.out_links.get_nnz(via_node)
         for from_node, from_link in zip(_from_nodes, _from_links):
             for to_node, to_link in zip(_to_nodes, _to_links):
                 if not (link_types[from_link] == -1 and link_types[to_link] == 1):
-                    # u turns are allowed
-                    # excluding turns that go from sink to source connectors
+                    # always excluding turns that go from sink to source connectors
                     # and vice versa
+                    if not u_turns:
+                        if to_node==from_node:
+                            continue
                     via_nodes.append(via_node)
                     to_nodes.append(to_node)
                     from_nodes.append(from_node)
                     from_links.append(from_link)
                     to_links.append(to_link)
                     turn_counter += 1
     fw_index_array = np.column_stack((from_links, to_links))
```

### Comparing `dyntapy-0.2.2/dyntapy/toy_networks/birmingham_net.tntp` & `dyntapy-0.2.3/dyntapy/toy_networks/birmingham_net.tntp`

 * *Files identical despite different names*

### Comparing `dyntapy-0.2.2/dyntapy/toy_networks/birmingham_node.tntp` & `dyntapy-0.2.3/dyntapy/toy_networks/birmingham_node.tntp`

 * *Files identical despite different names*

### Comparing `dyntapy-0.2.2/dyntapy/toy_networks/chicagoregional_net.tntp` & `dyntapy-0.2.3/dyntapy/toy_networks/chicagoregional_net.tntp`

 * *Files identical despite different names*

### Comparing `dyntapy-0.2.2/dyntapy/toy_networks/chicagoregional_node.tntp` & `dyntapy-0.2.3/dyntapy/toy_networks/chicagoregional_node.tntp`

 * *Files identical despite different names*

### Comparing `dyntapy-0.2.2/dyntapy/toy_networks/chicagosketch_net.tntp` & `dyntapy-0.2.3/dyntapy/toy_networks/chicagosketch_net.tntp`

 * *Files identical despite different names*

### Comparing `dyntapy-0.2.2/dyntapy/toy_networks/chicagosketch_node.tntp` & `dyntapy-0.2.3/dyntapy/toy_networks/chicagosketch_node.tntp`

 * *Files identical despite different names*

### Comparing `dyntapy-0.2.2/dyntapy/toy_networks/siouxfalls_net.tntp` & `dyntapy-0.2.3/dyntapy/toy_networks/siouxfalls_net.tntp`

 * *Files identical despite different names*

### Comparing `dyntapy-0.2.2/dyntapy/toy_networks/siouxfalls_node.tntp` & `dyntapy-0.2.3/dyntapy/toy_networks/siouxfalls_node.tntp`

 * *Files identical despite different names*

### Comparing `dyntapy-0.2.2/dyntapy/utilities.py` & `dyntapy-0.2.3/dyntapy/utilities.py`

 * *Files identical despite different names*

### Comparing `dyntapy-0.2.2/dyntapy/visualization.py` & `dyntapy-0.2.3/dyntapy/visualization.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,45 +8,47 @@
 #
 #
 #
 #
 import datetime
 import os
 import warnings
+from itertools import chain
 from inspect import signature
 from warnings import warn
 
 import networkx as nx
 import numpy as np
 import osmnx as ox
 from bokeh.io import output_file, output_notebook, show
 from bokeh.layouts import Spacer, column, row
 from bokeh.models import HoverTool, OpenURL, TapTool
 from bokeh.models.callbacks import CustomJS
-from bokeh.models.glyphs import Patches
+from bokeh.models.glyphs import Patches, MultiPolygons
 from bokeh.models.markers import Circle
 from bokeh.models.widgets import Slider, TextInput
 from bokeh.plotting import ColumnDataSource, figure
 from bokeh.tile_providers import Vendors, get_provider
 from pyproj import CRS
-from shapely.geometry import LineString
+from shapely.geometry import LineString, MultiPolygon
 
-from dyntapy.demand import SimulationTime
 from dyntapy.settings import parameters
 from dyntapy.utilities import __create_green_to_red_cm
 
 traffic_cm = __create_green_to_red_cm()
 
 link_highlight_colors = parameters.visualization.link_highlight_colors
 node_highlight_color = parameters.visualization.node_highlight_color
 node_color = parameters.visualization.node_color
 centroid_color = parameters.visualization.centroid_color
 node_size = parameters.visualization.node_size
 
 
+# TODO: investigate reactions on layout width changes,
+#  https://github.com/bokeh/bokeh/pull/6021
 def _get_output_file(plot_name: str):
     dt_string = datetime.datetime.now().strftime("%d_%m_%Y_%H_%M_%S")
     return os.getcwd() + os.path.sep + f"{plot_name}_{dt_string}.html"
 
 
 def _process_plot_arguments(g, title, notebook, euclidean, link_kwargs, node_kwargs):
     # process all arguments that are shared between dynamic and static
@@ -87,15 +89,18 @@
         tile_provider = get_provider(Vendors.CARTODBPOSITRON_RETINA)
         plot.add_tile(tile_provider)
         tmp = nx.MultiDiGraph(g)
         tmp = ox.project_graph(
             tmp, CRS.from_user_input(3857)
         )  # from lan lot to web mercator
 
+        link_width_scaling = parameters.visualization.link_width_scaling
     else:
+
+        link_width_scaling = parameters.visualization.link_width_scaling_euclidean
         plot = figure(
             plot_height=parameters.visualization.plot_size,
             plot_width=parameters.visualization.plot_size,
             aspect_ratio=1,
             toolbar_location="below",
         )
         tmp = g
@@ -125,29 +130,30 @@
                 node_kwargs[key] = (
                     item.astype(np.float64)
                     .round(parameters.visualization.rounding_digits)
                     .tolist()
                 )
             else:
                 node_kwargs[key] = item.tolist()
-    return plot, tmp
+    return plot, tmp, link_width_scaling
 
 
 def show_network(
     g,
     flows=None,
     link_kwargs=dict(),
     node_kwargs=dict(),
     highlight_links=np.array([]),
     highlight_nodes=np.array([]),
     euclidean=False,
     toy_network=False,
     title=None,
     notebook=False,
     show_nodes=True,
+    return_plot=False,
 ):
     """
     Visualizing a network with static attributes in a .html.
 
     Parameters
     ----------
     g: networkx.DiGraph
@@ -159,24 +165,26 @@
         displayed
     node_kwargs: dict, optional
         key: str, value: numpy.ndarray - additional node information to be
         displayed
     highlight_links: numpy.ndarray or list, optional
         int, 1D or 2D - links to highlight
     highlight_nodes: numpy.ndarray or list, optional
-        int, 1D or 2D - links to highlight
+        int, 1D or 2D - nodes to highlight
     euclidean: bool, optional
         set to True if coordinates in graph are euclidean.
     toy_network: bool, optional
         deprecated, use euclidean instead.
     title: str, optional
     notebook: bool, optional
         set to True if the plot should be rendered in a notebook.
     show_nodes: bool, optional
         whether to render nodes
+    return_plot: bool, optional
+        set to True if the plot object should be returned instead of showing it.
 
     Examples
     --------
 
     >>> show_network(g, highlight_links=[[2,4],[3,6]])
 
     will plot the network and highlight links [2,4] in neon pink,
@@ -212,42 +220,41 @@
 
     if toy_network:
         euclidean = toy_network
         warnings.warn(
             "use of toy_network arg is deprecated, use euclidean instead",
             DeprecationWarning,
         )
-
-    plot, tmp = _process_plot_arguments(
+    plot, tmp, link_width_scaling = _process_plot_arguments(
         g, title, notebook, euclidean, link_kwargs, node_kwargs
     )
     show_flows = True
     if flows is not None:
         pass
     else:
         flows = np.zeros(g.number_of_edges())
         show_flows = False
     max_flow = max(np.max(flows), 1)
 
     max_width_bokeh, max_width_coords = get_max_edge_width(
         tmp,
-        parameters.visualization.link_width_scaling,
+        link_width_scaling,
         parameters.visualization.plot_size,
     )
 
     if type(highlight_links) not in (np.ndarray, list):
         raise ValueError
     c, x, y = _get_colors_and_coords(
         tmp,
         max_width_coords,
         max_flow,
         flows,
         time_step=1,
         highlight_links=highlight_links,
-        patch_ratio=3,
+        patch_ratio=parameters.visualization.link_width_min_max_ratio,
     )
     edge_source = _edge_cds(tmp, c, flows, x, y, **link_kwargs)
     edge_renderer = plot.add_glyph(
         edge_source,
         glyph=Patches(
             xs="x",
             ys="y",
@@ -293,15 +300,18 @@
             show_arrow=False,
             tooltips=node_tooltips,
             renderers=[node_renderer],
             description="Node Hover Tool",
         )
         plot.add_tools(node_hover)
     plot.add_tools(edge_hover)
-    show(plot)
+    if not return_plot:
+        show(plot)
+    else:
+        return plot
 
 
 def show_link_od_flows(g: nx.DiGraph, od_flows, **kwargs):
     """
     Visualizing a network with origin destination flows for each link in a .html.
 
     Parameters
@@ -344,14 +354,15 @@
     toy_network=False,
     euclidean=False,
     highlight_nodes=np.array([]),
     highlight_links=np.array([]),
     title=None,
     notebook=False,
     show_nodes=True,
+    return_plot=False,
 ):
     """
     Visualizing a network with dynamic attributes in a .html.
 
     Parameters
     ----------
     g: networkx.DiGraph
@@ -364,24 +375,26 @@
         be displayed
     node_kwargs: dict, optional
         key: str, value: np.ndarray - additional time-dependent node information to
         be displayed
     highlight_links: numpy.ndarray, optional
         int, 1D or 2D - links to highlight
     highlight_nodes: numpy.ndarray, optional
-        int, 1D or 2D - links to highlight
+        int, 1D or 2D - nodes to highlight
     euclidean: bool, optional
         set to True if coordinates in graph are euclidean.
     toy_network: bool, optional
         deprecated, use euclidean instead.
     title: str, optional
     notebook: bool, optional
         set to True if the plot should be rendered in a notebook.
     show_nodes: bool, optional
         whether to render nodes
+    return_plot: bool, optional
+        set to True if the plot object should be returned instead of showing it.
 
     Examples
     --------
     highlighting works just as in `show_network` and is not time dependent.
 
     >>> foo = np.arange((g.number_of_edges(), time.tot_time_steps))
     >>> bar = np.arange((g.number_of_edges(), time.tot_time_steps))
@@ -413,15 +426,15 @@
     if toy_network:
         euclidean = toy_network
         warnings.warn(
             "use of toy_network arg is deprecated, use euclidean instead",
             DeprecationWarning,
         )
 
-    plot, tmp = _process_plot_arguments(
+    plot, tmp, link_width_scaling = _process_plot_arguments(
         g, title, notebook, euclidean, link_kwargs, node_kwargs
     )
     if flows is None:
         if "flows" not in list(link_kwargs.keys()):
             flows = np.zeros((time.tot_time_steps, g.number_of_edges()))
         else:
             flows = link_kwargs["flows"]
@@ -463,15 +476,15 @@
         del node_kwargs[key]
 
     # adding different coordinate attribute names to comply with osmnx
 
     max_flow = min(np.max(flows), 8000)  # weeding out numerical errors
     max_width_bokeh, max_width_coords = get_max_edge_width(
         tmp,
-        parameters.visualization.link_width_scaling,
+        link_width_scaling,
         parameters.visualization.plot_size,
     )
     # calculate all colors and coordinates for the different time dependent flows
     all_colors = []
     all_x = []
     all_y = []
     for t in range(time.tot_time_steps):
@@ -615,41 +628,56 @@
             source.change.emit();
         """,
     )
     time_slider.js_on_change("value", link_call_back)
     if show_nodes:
         time_slider.js_on_change("value", node_call_back)
     layout = row(plot, column(text_input, Spacer(height=40), time_slider))
-    show(layout)
+    if return_plot:
+        return layout
+    else:
+        show(layout)
 
 
 def get_max_edge_width(g, scaling, plot_size):
     node_x = [x for _, x in g.nodes.data("x")]
     node_y = [y for _, y in g.nodes.data("y")]
     min_x, max_x, min_y, max_y = min(node_x), max(node_x), min(node_y), max(node_y)
     max_width_coords = scaling * (0.5 * (max_x - min_x) + 0.5 * (max_y - min_y))
     max_width_bokeh = plot_size * scaling
     return max_width_bokeh, max_width_coords
 
 
-def show_demand(g, title=None, notebook=False, euclidean=False, toy_network=False):
+def show_demand(
+    g,
+    title=None,
+    notebook=False,
+    euclidean=False,
+    toy_network=False,
+    highlight_nodes=[],
+    return_plot=False,
+):
     """
 
     visualize demand on a map
 
     Parameters
     ----------
     g: networkx.DiGraph
     title: str
     notebook: bool, optional
         set to True if the plot should be rendered in a notebook.
     euclidean: bool, optional
         set to True, if 'x_coord' and 'y_coord' in g are euclidean.
     toy_network: bool, optional
         deprecated, use euclidean instead
+    highlight_nodes: numpy.ndarray or list, optional
+        int, 1D - nodes to highlight
+    return_plot: bool, optional
+        set to True if the plot object should be returned instead of showing it.
 
     Examples
     --------
 
     Given an `od_matrix` and coordinates in longitude `X` and latitude `Y` it is
     straightforward to visualize the travel pattern.
 
@@ -694,55 +722,64 @@
             x_axis_type="mercator",
             y_axis_type="mercator",
             aspect_ratio=1,
             toolbar_location="below",
         )
         tile_provider = get_provider(Vendors.CARTODBPOSITRON_RETINA)
         plot.add_tile(tile_provider)
+        link_width_scaling = parameters.visualization.link_width_scaling
     else:
         tmp = (
             g  # projection not needed for toy networks, coordinates are plain
             # cartesian
         )
         plot = figure(
             plot_height=parameters.visualization.plot_size,
             plot_width=parameters.visualization.plot_size,
             aspect_ratio=1,
             toolbar_location="below",
         )
+        link_width_scaling = parameters.visualization.link_width_scaling_euclidean
     plot.title.text = title
     max_width_bokeh, max_width_coords = get_max_edge_width(
         tmp,
-        parameters.visualization.link_width_scaling,
+        link_width_scaling,
         parameters.visualization.plot_size,
     )
     min_width_coords = max_width_coords / 10
     all_flow = [flow for u, v, flow in tmp.edges.data("flow") if u != v]
     max_flow = max(all_flow)
     x_list, y_list = [], []
     for u, v, data in tmp.edges.data():
         if u != v:  # not showing intrazonal traffic
             flow = data["flow"]
             width_coords = min_width_coords + (max_width_coords - min_width_coords) * (
                 flow / max_flow
             )
-            ls, para_ls = __linestring_from_node_cords(
-                [
-                    [tmp.nodes[u]["x"], tmp.nodes[u]["y"]],
-                    [tmp.nodes[v]["x"], tmp.nodes[v]["y"]],
-                ],
+            x, y = __build_patch_buffered(
+                tmp.nodes[u]["x"],
+                tmp.nodes[u]["y"],
+                tmp.nodes[v]["x"],
+                tmp.nodes[v]["y"],
+                data,
                 width_coords,
             )
-            (x1, y1, x2, y2) = ls.xy + para_ls.xy
-            x = x2 + x1
-            y = y2 + y1
-            x_list.append(list(x))
-            y_list.append(list(y))
+            x_list.append(x)
+            y_list.append(y)
+
+    nodes_to_highlight = np.full(tmp.number_of_nodes(), False)
+    nodes_to_highlight[highlight_nodes] = True
+    node_colors = [
+        node_highlight_color if nodes_to_highlight[idx] else node_color
+        for idx in list(tmp.nodes.keys())
+    ]
+
     node_source = ColumnDataSource(
         data=dict(
+            color=node_colors,
             x=[x for _, x in tmp.nodes.data("x")],
             y=[y for _, y in tmp.nodes.data("y")],
             centroid_id=list(tmp.nodes.keys()),
         )
     )
     edge_source = ColumnDataSource(data=dict(flow=all_flow, x=x_list, y=y_list))
     # text_input = TextInput(title="Add new graph title", value='')
@@ -756,14 +793,15 @@
     edge_tooltips = [("flow", "@flow{(0.0)}")]
     node_renderer = plot.add_glyph(
         node_source,
         glyph=Circle(
             x="x",
             y="y",
             size=node_size * 2,
+            fill_color="color",
             line_color="black",
             line_alpha=0.4,
             fill_alpha=0.7,
             line_width=node_size / 10,
         ),
     )
     node_tooltips = [(item, f"@{item}") for item in ["x", "y", "centroid_id"]]
@@ -779,15 +817,18 @@
         renderers=[node_renderer],
         description="Node Hover Tool",
     )
     plot.add_tools(node_hover, edge_hover)
     text_input = TextInput(title="Add new graph title", value="")
     text_input.js_link("value", plot.title, "text")
     layout = row(plot, text_input)
-    show(layout)
+    if return_plot:
+        return plot
+    else:
+        show(layout)
 
 
 def _node_cds(g, highlight_nodes=np.array([]), **kwargs):
     visualization_keys = parameters.visualization.node_keys
     node_dict = dict()
     node_colors = [node_color for _ in range(g.number_of_nodes())]
     for _, data in sorted(g.nodes(data=True), key=lambda t: t[1]["node_id"]):
@@ -831,18 +872,18 @@
 def _get_colors_and_coords(
     g,
     max_width_coords,
     max_flow,
     flows,
     time_step,
     highlight_links: object = np.array([]),
-    patch_ratio=8,
+    patch_ratio=parameters.visualization.link_width_min_max_ratio,
 ):
     nr_of_colors = len(traffic_cm)
-    min_width_coords = max_width_coords / patch_ratio
+    min_width_coords = max_width_coords * patch_ratio
     if (
         max_flow == 0
     ):  # geometries cannot be computed, may sometimes happen in debugging.
         max_flow = 1
     colors = []
     x_list = []
     y_list = []
@@ -857,20 +898,19 @@
                         / (data["capacity"] * time_step)
                         * nr_of_colors
                     )
                 )
             ]
         except IndexError:
             color = traffic_cm[-1]  # flow larger than capacity!
-            flow = 0
+            flow = data["capacity"]
         except KeyError:  # capacity or flow not defined
             color = traffic_cm[0]
             flow = 0
         colors.append(color)
-        loaded = 0
         try:
             if flow > 0:
                 loaded = 1
                 width_coords = (
                     min_width_coords
                     + min_width_coords * loaded
                     + (max_width_coords - 2 * min_width_coords)
@@ -881,55 +921,24 @@
             # width_bokeh = min_width_bokeh + (max_width_bokeh - min_width_bokeh) * (
             # data['flow'] / max_flow)
         except KeyError or UnboundLocalError or IndexError:  # flow not defined..,
             # no width scaling possible
             width_coords = min_width_coords
             # width_bokeh = min_width_bokeh
         # edge_dict['width'].append(width_bokeh)
-        if "geometry" in data:
-            ls = data["geometry"]
-            assert isinstance(ls, LineString)
-            para_ls = ls.parallel_offset(width_coords * 1)
-        else:
-            ls, para_ls = __linestring_from_node_cords(
-                [
-                    [g.nodes[u]["x"], g.nodes[u]["y"]],
-                    [g.nodes[v]["x"], g.nodes[v]["y"]],
-                ],
-                width_coords,
-            )
 
-        try:
-            (x1, y1, x2, y2) = ls.xy + para_ls.xy
-            x = x2 + x1
-            y = y2 + y1
-        except (
-            AttributeError,
-            NotImplementedError,
-        ):  # Attributeerror: weird error due to i'll defined line
-            # string .. - dig deeper if I have more time on my hands - probably an
-            # error in osmnx line string
-            # creation
-            # Notimplemented Error - original Linestring is cut into multiple pieces
-            # by parallel offset -
-            # hence ls is MultiLineString - if the line string has very sharp corners
-            # the offset will stop working
-            # properly, we just use a straight Line connection in that case
-            ls, para_ls = __linestring_from_node_cords(
-                [
-                    [g.nodes[u]["x"], g.nodes[u]["y"]],
-                    [g.nodes[v]["x"], g.nodes[v]["y"]],
-                ],
-                width_coords,
-            )
-            (x1, y1, x2, y2) = ls.xy + para_ls.xy
-            x = x1 + x2
-            y = y1 + y2
-        x_list.append(list(x))
-        y_list.append(list(y))
+        x1, y1, x2, y2 = (
+            g.nodes[u]["x"],
+            g.nodes[u]["y"],
+            g.nodes[v]["x"],
+            g.nodes[v]["y"],
+        )
+        x, y = __build_patch_buffered(x1, y1, x2, y2, data, width_coords)
+        x_list.append(x)
+        y_list.append(y)
 
     if type(highlight_links) == np.ndarray or (
         type(highlight_links) == list
         and all(
             isinstance(x, np.integer) or isinstance(x, int) for x in highlight_links
         )
     ):
@@ -950,10 +959,24 @@
             for links, color in zip(highlight_links, link_highlight_colors):
                 for link in links:
                     colors[link] = color
 
     return colors, x_list, y_list
 
 
-def __linestring_from_node_cords(coord_list, width_coords):
-    ls = LineString(coord_list)
-    return ls, ls.parallel_offset(1 * width_coords)
+def __build_patch_buffered(x1, y1, x2, y2, data, width_coords):
+    # buffers around the line in one direction.
+    # returns a list of x and y coordinates that form the boundary of the generated
+    # polygon.
+
+    if "geometry" in data:
+        ls = data["geometry"]
+    else:
+        ls = LineString([[x1, y1], [x2, y2]])
+    poly = ls.buffer(-width_coords, single_sided=True)
+    if isinstance(poly, MultiPolygon) or len(poly.interiors) > 0:  # Lines with very
+        # steep curves or self-intersections yield either multiple polygons or
+        # polygons with holes, in either case we take the straight line instead.
+        # TODO: investigate support for MultiPolygons with holes in Bokeh
+        ls = LineString([[x1, y1], [x2, y2]])
+        poly = ls.buffer(-width_coords, single_sided=True)
+    return poly.exterior.xy[0].tolist(), poly.exterior.xy[1].tolist()
```

### Comparing `dyntapy-0.2.2/dyntapy.egg-info/PKG-INFO` & `dyntapy-0.2.3/dyntapy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyntapy
-Version: 0.2.2
+Version: 0.2.3
 Summary: Macroscopic Static and Dynamic Traffic Assignment in Python 
 Home-page: https://gitlab.kuleuven.be/ITSCreaLab/public-toolboxes/dyntapy
 Author: Paul Ortmann
 Author-email: itscrealab@kuleuven.be
 License: GPLv3
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyntapy-0.2.2/dyntapy.egg-info/SOURCES.txt` & `dyntapy-0.2.3/dyntapy.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -29,26 +29,23 @@
 dyntapy/dta/i_ltm_cls.py
 dyntapy/dta/i_ltm_setup.py
 dyntapy/dta/incremental_assignment.py
 dyntapy/dta/orca_nodel_model.py
 dyntapy/dta/qr_projection.py
 dyntapy/dta/travel_times.py
 dyntapy/sta/__init__.py
+dyntapy/sta/_debugging_sta.py
 dyntapy/sta/dial_b.py
+dyntapy/sta/dial_stochastic_assignment.py
 dyntapy/sta/equilibrate_bush.py
 dyntapy/sta/gap.py
 dyntapy/sta/msa.py
 dyntapy/sta/uncongested_dial.py
 dyntapy/sta/utilities.py
 dyntapy/toy_networks/birmingham_net.tntp
 dyntapy/toy_networks/birmingham_node.tntp
 dyntapy/toy_networks/chicagoregional_net.tntp
 dyntapy/toy_networks/chicagoregional_node.tntp
 dyntapy/toy_networks/chicagosketch_net.tntp
 dyntapy/toy_networks/chicagosketch_node.tntp
 dyntapy/toy_networks/siouxfalls_net.tntp
-dyntapy/toy_networks/siouxfalls_node.tntp
-tests/current_tests.py
-tests/simple_bottleneck.py
-tests/simple_diverge.py
-tests/simple_merge.py
-tests/test_dyntapy.py
+dyntapy/toy_networks/siouxfalls_node.tntp
```

### Comparing `dyntapy-0.2.2/setup.py` & `dyntapy-0.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     'matplotlib',
     'notebook',
     'setuptools',
 ]
 # now call setup
 setup(
     name="dyntapy",
-    version="0.2.2",
+    version="0.2.3",
     description=DESC,
     classifiers=CLASSIFIERS,
     url="https://gitlab.kuleuven.be/ITSCreaLab/public-toolboxes/dyntapy",
     author="Paul Ortmann",
     author_email="itscrealab@kuleuven.be",
     long_description=README,
     long_description_content_type="text/markdown",
```

