# Comparing `tmp/srsinst.rga-0.3.0.tar.gz` & `tmp/srsinst.rga-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\PyPI\instrument drivers to GIT\rga100\dist\.tmp-ejzn8mjc\srsinst.rga-0.3.0.tar", last modified: Wed May 24 20:43:46 2023, max compression
+gzip compressed data, was "C:\PyPI\instrument_library\rga100\dist\.tmp-msw7v9pn\srsinst.rga-0.3.1.tar", last modified: Wed Jun 14 00:00:45 2023, max compression
```

## Comparing `srsinst.rga-0.3.0.tar` & `srsinst.rga-0.3.1.tar`

### file list

```diff
@@ -1,56 +1,72 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 20:43:46.766221 srsinst.rga-0.3.0/
--rw-rw-rw-   0        0        0     1356 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/.gitignore
--rw-rw-rw-   0        0        0     1113 2023-05-19 17:56:22.000000 srsinst.rga-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     6402 2023-05-24 20:43:46.766221 srsinst.rga-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     5623 2023-05-19 18:09:46.000000 srsinst.rga-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 20:43:46.702127 srsinst.rga-0.3.0/docs/
-drwxrwxrwx   0        0        0        0 2023-05-24 20:43:46.702127 srsinst.rga-0.3.0/docs/_static/
-drwxrwxrwx   0        0        0        0 2023-05-24 20:43:46.736271 srsinst.rga-0.3.0/docs/_static/image/
--rw-rw-rw-   0        0        0   115947 2023-05-19 17:56:22.000000 srsinst.rga-0.3.0/docs/_static/image/derived-pvst-plot-screenshot.png
--rw-rw-rw-   0        0        0     1164 2023-05-16 00:38:30.000000 srsinst.rga-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-24 20:43:46.766221 srsinst.rga-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-05-19 17:56:22.000000 srsinst.rga-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 20:43:46.712095 srsinst.rga-0.3.0/srsinst/
-drwxrwxrwx   0        0        0        0 2023-05-24 20:43:46.746266 srsinst.rga-0.3.0/srsinst/rga/
--rw-rw-rw-   0        0        0      345 2023-05-24 20:36:23.000000 srsinst.rga-0.3.0/srsinst/rga/__init__.py
--rw-rw-rw-   0        0        0      483 2023-05-19 21:11:26.000000 srsinst.rga-0.3.0/srsinst/rga/__main__.py
--rw-rw-rw-   0        0        0    10600 2023-05-19 21:11:26.000000 srsinst.rga-0.3.0/srsinst/rga/gaslib.dat
-drwxrwxrwx   0        0        0        0 2023-05-24 20:43:46.746266 srsinst.rga-0.3.0/srsinst/rga/instruments/
--rw-rw-rw-   0        0        0       38 2023-05-19 21:11:26.000000 srsinst.rga-0.3.0/srsinst/rga/instruments/__init__.py
--rw-rw-rw-   0        0        0      872 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/instruments/get_instruments.py
-drwxrwxrwx   0        0        0        0 2023-05-24 20:43:46.756254 srsinst.rga-0.3.0/srsinst/rga/instruments/rga100/
--rw-rw-rw-   0        0        0        0 2023-05-19 21:11:26.000000 srsinst.rga-0.3.0/srsinst/rga/instruments/rga100/__init__.py
--rw-rw-rw-   0        0        0     5249 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/instruments/rga100/commands.py
--rw-rw-rw-   0        0        0     7009 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/instruments/rga100/components.py
--rw-rw-rw-   0        0        0     4510 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/instruments/rga100/errors.py
--rw-rw-rw-   0        0        0     8589 2023-05-23 22:01:40.000000 srsinst.rga-0.3.0/srsinst/rga/instruments/rga100/rga.py
--rw-rw-rw-   0        0        0    18656 2023-05-19 21:11:26.000000 srsinst.rga-0.3.0/srsinst/rga/instruments/rga100/rga_commands.json
--rw-rw-rw-   0        0        0    11501 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/instruments/rga100/scans.py
--rw-rw-rw-   0        0        0     9872 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/instruments/rga100/sicp.py
-drwxrwxrwx   0        0        0        0 2023-05-24 20:43:46.756254 srsinst.rga-0.3.0/srsinst/rga/plots/
--rw-rw-rw-   0        0        0        0 2023-05-19 21:11:26.000000 srsinst.rga-0.3.0/srsinst/rga/plots/__init__.py
--rw-rw-rw-   0        0        0     3611 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/plots/analogscanplot.py
--rw-rw-rw-   0        0        0     3443 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/plots/analysis.py
--rw-rw-rw-   0        0        0     3234 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/plots/basescanplot.py
--rw-rw-rw-   0        0        0     3279 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/plots/histogramscanplot.py
--rw-rw-rw-   0        0        0     8102 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/plots/timeplot.py
--rw-rw-rw-   0        0        0     2228 2023-05-22 17:53:19.000000 srsinst.rga-0.3.0/srsinst/rga/rga.taskconfig
-drwxrwxrwx   0        0        0        0 2023-05-24 20:43:46.766221 srsinst.rga-0.3.0/srsinst/rga/tasks/
--rw-rw-rw-   0        0        0        0 2023-05-19 21:11:26.000000 srsinst.rga-0.3.0/srsinst/rga/tasks/__init__.py
--rw-rw-rw-   0        0        0     3999 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/tasks/analogscantask.py
--rw-rw-rw-   0        0        0     2543 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/tasks/cemcontroltask.py
--rw-rw-rw-   0        0        0     9319 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/tasks/cemgaintask.py
--rw-rw-rw-   0        0        0     9586 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/tasks/compositionanalysistask.py
--rw-rw-rw-   0        0        0     5243 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/tasks/derivedpvstscantask.py
--rw-rw-rw-   0        0        0     2751 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/tasks/filamentcontroltask.py
--rw-rw-rw-   0        0        0     3685 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/tasks/histogramscantask.py
--rw-rw-rw-   0        0        0    11440 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/tasks/peaktuningtask.py
--rw-rw-rw-   0        0        0     2557 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/tasks/pvstscantask.py
--rw-rw-rw-   0        0        0     2087 2023-05-19 21:13:35.000000 srsinst.rga-0.3.0/srsinst/rga/tasks/searchlan.py
-drwxrwxrwx   0        0        0        0 2023-05-24 20:43:46.746266 srsinst.rga-0.3.0/srsinst.rga.egg-info/
--rw-rw-rw-   0        0        0     6402 2023-05-24 20:43:46.000000 srsinst.rga-0.3.0/srsinst.rga.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1432 2023-05-24 20:43:46.000000 srsinst.rga-0.3.0/srsinst.rga.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 20:43:46.000000 srsinst.rga-0.3.0/srsinst.rga.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-24 20:43:46.000000 srsinst.rga-0.3.0/srsinst.rga.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       68 2023-05-24 20:43:46.000000 srsinst.rga-0.3.0/srsinst.rga.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-24 20:43:46.000000 srsinst.rga-0.3.0/srsinst.rga.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 00:00:45.750303 srsinst.rga-0.3.1/
+-rw-rw-rw-   0        0        0     1113 2023-05-16 22:11:28.000000 srsinst.rga-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0     6863 2023-06-14 00:00:45.750303 srsinst.rga-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5860 2023-06-13 00:01:09.000000 srsinst.rga-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 00:00:45.714113 srsinst.rga-0.3.1/docs/
+-rw-rw-rw-   0        0        0      654 2023-05-19 21:28:01.000000 srsinst.rga-0.3.1/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-06-14 00:00:45.694113 srsinst.rga-0.3.1/docs/_static/
+drwxrwxrwx   0        0        0        0 2023-06-14 00:00:45.714113 srsinst.rga-0.3.1/docs/_static/image/
+-rw-rw-rw-   0        0        0   174977 2023-06-09 18:18:12.000000 srsinst.rga-0.3.1/docs/_static/image/comp-analysis-screenshot.png
+-rw-rw-rw-   0        0        0   115947 2023-05-19 17:56:22.000000 srsinst.rga-0.3.1/docs/_static/image/derived-pvst-plot-screenshot.png
+-rw-rw-rw-   0        0        0    51322 2023-06-09 22:02:41.000000 srsinst.rga-0.3.1/docs/_static/image/initial-screen-capture.png
+-rw-rw-rw-   0        0        0    27661 2023-05-25 23:24:03.000000 srsinst.rga-0.3.1/docs/_static/image/simple-analog-scan-screenshot.png
+-rw-rw-rw-   0        0        0     1970 2023-06-13 20:55:52.000000 srsinst.rga-0.3.1/docs/conf.py
+-rw-rw-rw-   0        0        0      356 2023-06-01 23:58:11.000000 srsinst.rga-0.3.1/docs/custom_tasks.rst
+-rw-rw-rw-   0        0        0     6252 2023-06-12 22:33:57.000000 srsinst.rga-0.3.1/docs/gui_application.rst
+-rw-rw-rw-   0        0        0     2584 2023-06-12 23:28:46.000000 srsinst.rga-0.3.1/docs/index.rst
+-rw-rw-rw-   0        0        0     4199 2023-06-12 17:15:20.000000 srsinst.rga-0.3.1/docs/installation.rst
+-rw-rw-rw-   0        0        0    16282 2023-06-12 20:44:51.000000 srsinst.rga-0.3.1/docs/instrument_driver.rst
+-rwxrwxrwx   0        0        0      802 2023-05-19 21:28:01.000000 srsinst.rga-0.3.1/docs/make.bat
+-rw-rw-rw-   0        0        0       32 2023-05-19 21:28:01.000000 srsinst.rga-0.3.1/docs/requirements.txt
+-rw-rw-rw-   0        0        0     1332 2023-05-31 23:18:38.000000 srsinst.rga-0.3.1/docs/srsinst.rga.instruments.rga100.rst
+-rw-rw-rw-   0        0        0      358 2023-05-19 21:28:01.000000 srsinst.rga-0.3.1/docs/srsinst.rga.instruments.rst
+-rw-rw-rw-   0        0        0     1049 2023-06-09 19:15:10.000000 srsinst.rga-0.3.1/docs/srsinst.rga.plots.rst
+-rw-rw-rw-   0        0        0      148 2023-05-31 23:17:11.000000 srsinst.rga-0.3.1/docs/srsinst.rga.rst
+-rw-rw-rw-   0        0        0     2095 2023-06-06 22:33:30.000000 srsinst.rga-0.3.1/docs/srsinst.rga.tasks.rst
+-rw-rw-rw-   0        0        0     1488 2023-06-13 21:05:18.000000 srsinst.rga-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-14 00:00:45.750303 srsinst.rga-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsinst.rga-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 00:00:45.694113 srsinst.rga-0.3.1/srsinst/
+drwxrwxrwx   0        0        0        0 2023-06-14 00:00:45.724115 srsinst.rga-0.3.1/srsinst/rga/
+-rw-rw-rw-   0        0        0      349 2023-06-14 00:00:17.000000 srsinst.rga-0.3.1/srsinst/rga/__init__.py
+-rw-rw-rw-   0        0        0      483 2023-05-19 21:11:26.000000 srsinst.rga-0.3.1/srsinst/rga/__main__.py
+-rw-rw-rw-   0        0        0    10675 2023-06-01 21:25:29.000000 srsinst.rga-0.3.1/srsinst/rga/gaslib.dat
+drwxrwxrwx   0        0        0        0 2023-06-14 00:00:45.724115 srsinst.rga-0.3.1/srsinst/rga/instruments/
+-rw-rw-rw-   0        0        0        0 2023-06-13 23:56:14.000000 srsinst.rga-0.3.1/srsinst/rga/instruments/__init__.py
+-rw-rw-rw-   0        0        0      872 2023-05-19 21:13:35.000000 srsinst.rga-0.3.1/srsinst/rga/instruments/get_instruments.py
+drwxrwxrwx   0        0        0        0 2023-06-14 00:00:45.739268 srsinst.rga-0.3.1/srsinst/rga/instruments/rga100/
+-rw-rw-rw-   0        0        0        0 2023-05-19 21:11:26.000000 srsinst.rga-0.3.1/srsinst/rga/instruments/rga100/__init__.py
+-rw-rw-rw-   0        0        0     5249 2023-05-19 21:13:35.000000 srsinst.rga-0.3.1/srsinst/rga/instruments/rga100/commands.py
+-rw-rw-rw-   0        0        0     7355 2023-05-25 20:26:25.000000 srsinst.rga-0.3.1/srsinst/rga/instruments/rga100/components.py
+-rw-rw-rw-   0        0        0     4510 2023-05-19 21:13:35.000000 srsinst.rga-0.3.1/srsinst/rga/instruments/rga100/errors.py
+-rw-rw-rw-   0        0        0     8719 2023-06-13 23:56:14.000000 srsinst.rga-0.3.1/srsinst/rga/instruments/rga100/rga.py
+-rw-rw-rw-   0        0        0    18656 2023-05-19 21:11:26.000000 srsinst.rga-0.3.1/srsinst/rga/instruments/rga100/rga_commands.json
+-rw-rw-rw-   0        0        0    11740 2023-05-31 21:39:25.000000 srsinst.rga-0.3.1/srsinst/rga/instruments/rga100/scans.py
+-rw-rw-rw-   0        0        0     9870 2023-06-06 21:51:12.000000 srsinst.rga-0.3.1/srsinst/rga/instruments/rga100/sicp.py
+drwxrwxrwx   0        0        0        0 2023-06-14 00:00:45.740273 srsinst.rga-0.3.1/srsinst/rga/plots/
+-rw-rw-rw-   0        0        0        0 2023-05-19 21:11:26.000000 srsinst.rga-0.3.1/srsinst/rga/plots/__init__.py
+-rw-rw-rw-   0        0        0     4122 2023-06-09 19:33:09.000000 srsinst.rga-0.3.1/srsinst/rga/plots/analogscanplot.py
+-rw-rw-rw-   0        0        0     3448 2023-06-09 18:23:15.000000 srsinst.rga-0.3.1/srsinst/rga/plots/analysis.py
+-rw-rw-rw-   0        0        0     3287 2023-06-09 19:32:57.000000 srsinst.rga-0.3.1/srsinst/rga/plots/basescanplot.py
+-rw-rw-rw-   0        0        0     3792 2023-06-09 19:32:57.000000 srsinst.rga-0.3.1/srsinst/rga/plots/histogramscanplot.py
+-rw-rw-rw-   0        0        0     9182 2023-06-09 19:33:28.000000 srsinst.rga-0.3.1/srsinst/rga/plots/timeplot.py
+-rw-rw-rw-   0        0        0     2226 2023-06-01 00:10:48.000000 srsinst.rga-0.3.1/srsinst/rga/rga.taskconfig
+drwxrwxrwx   0        0        0        0 2023-06-14 00:00:45.750303 srsinst.rga-0.3.1/srsinst/rga/tasks/
+-rw-rw-rw-   0        0        0        0 2023-05-19 21:11:26.000000 srsinst.rga-0.3.1/srsinst/rga/tasks/__init__.py
+-rw-rw-rw-   0        0        0     4001 2023-05-31 18:21:03.000000 srsinst.rga-0.3.1/srsinst/rga/tasks/analogscantask.py
+-rw-rw-rw-   0        0        0     2543 2023-05-19 21:13:35.000000 srsinst.rga-0.3.1/srsinst/rga/tasks/cemcontroltask.py
+-rw-rw-rw-   0        0        0     9379 2023-06-02 18:26:25.000000 srsinst.rga-0.3.1/srsinst/rga/tasks/cemgaintask.py
+-rw-rw-rw-   0        0        0     9586 2023-05-19 21:13:35.000000 srsinst.rga-0.3.1/srsinst/rga/tasks/compositionanalysistask.py
+-rw-rw-rw-   0        0        0     5243 2023-05-19 21:13:35.000000 srsinst.rga-0.3.1/srsinst/rga/tasks/derivedpvstscantask.py
+-rw-rw-rw-   0        0        0     2751 2023-05-19 21:13:35.000000 srsinst.rga-0.3.1/srsinst/rga/tasks/filamentcontroltask.py
+-rw-rw-rw-   0        0        0     3685 2023-05-19 21:13:35.000000 srsinst.rga-0.3.1/srsinst/rga/tasks/histogramscantask.py
+-rw-rw-rw-   0        0        0    11440 2023-05-19 21:13:35.000000 srsinst.rga-0.3.1/srsinst/rga/tasks/peaktuningtask.py
+-rw-rw-rw-   0        0        0     2557 2023-05-19 21:13:35.000000 srsinst.rga-0.3.1/srsinst/rga/tasks/pvstscantask.py
+-rw-rw-rw-   0        0        0     2591 2023-06-06 22:11:10.000000 srsinst.rga-0.3.1/srsinst/rga/tasks/searchlan.py
+drwxrwxrwx   0        0        0        0 2023-06-14 00:00:45.724115 srsinst.rga-0.3.1/srsinst.rga.egg-info/
+-rw-rw-rw-   0        0        0     6863 2023-06-14 00:00:45.000000 srsinst.rga-0.3.1/srsinst.rga.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1890 2023-06-14 00:00:45.000000 srsinst.rga-0.3.1/srsinst.rga.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 00:00:45.000000 srsinst.rga-0.3.1/srsinst.rga.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-14 00:00:45.000000 srsinst.rga-0.3.1/srsinst.rga.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      132 2023-06-14 00:00:45.000000 srsinst.rga-0.3.1/srsinst.rga.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-14 00:00:45.000000 srsinst.rga-0.3.1/srsinst.rga.egg-info/top_level.txt
```

### Comparing `srsinst.rga-0.3.0/LICENSE` & `srsinst.rga-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.0/PKG-INFO` & `srsinst.rga-0.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,68 @@
 Metadata-Version: 2.1
 Name: srsinst.rga
-Version: 0.3.0
+Version: 0.3.1
 Summary: Instrument driver package for Residual Gas Analyzers (RGA) from Stanford Research Systems
 Author: Chulhoon Kim
 License: MIT license
+Project-URL: homepage, https://github.com/thinkSRS/srsinst.rga
+Project-URL: repository, https://github.com/thinkSRS/srsinst.rga.git
+Project-URL: documentation, https://thinksrs.github.io/srsinst.rga
 Keywords: RGA,residual gas analyzer,SRS,Stanford Research Systems
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: full
+Provides-Extra: docs
 License-File: LICENSE
 
 # `srsinst.rga`
 
 `srsinst.rga` provides Python instrument classes to control and acquire mass spectra from 
 [Stanford Research Systems (SRS) Residual Gas Analyzers (RGA)](https://thinksrs.com/products/rga.html).
 It also provides tasks running in GUI environment based on 
 [srsgui](https://thinksrs.github.io/srsgui/).  
-To operate SRS RGA with this package safely, you need to be familiar with SRS RGA. 
+To operate an SRS RGA with this package safely, you need to be familiar with SRS RGAs. 
 For detailed information, refer to the 
 [manual](https://thinksrs.com/downloads/pdfs/manuals/RGAm.pdf).
 
-![screenshot](https://github.com/thinkSRS/srsinst.rga/blob/main/docs/_static/image/derived-pvst-plot-screenshot.png " ")
+![screenshot](https://github.com/thinkSRS/srsinst.rga/blob/main/docs/_static/image/comp-analysis-screenshot.png " ")
 
 ## Installation
-You need a working Python with `pip` (Python package installer) installed. If you don't,
-[install Python 3](https://realpython.com/installing-python/) to your system.
-
-To install `srsinst.rga` as an instrument driver only, use Python package installer `pip` 
-from the command line.
-
-    python -m pip install srsinst.rga
+You need a working Python version 3.7 or later with `pip` (Python package installer) installed. 
+If you don't, [install Python 3](https://www.python.org/) to your system.
 
 To use its full GUI application, create a virtual environment, if necessary,
-and install with *[full]* option:
+and rub Python package installer `pip` with *[full]* option from the command prompt.
+
+    # To create a simple virtual environment (Optional) 
+    # The activate command may differ depending on your computer operating systems.
+    # Following is for Windows.
 
-    # To create a simple virtual environment (Optional)
     python -m venv venv
     venv\scripts\activate
 
-    # To install full GUI application 
+    # To install full GUI application
+
     python -m pip install srsinst.rga[full]
 
 
+To install `srsinst.rga` as an instrument driver only, install WITHOUT the *[full]* option. 
+Installation will be faster, because it does NOT install GUI related packages.
+
+    python -m pip install srsinst.rga
+
+
 ## Run `srsinst.rga` as GUI application
 If the Python Scripts directory is in PATH environment variable,
 Start the application by typing from the command line:
 
     rga
 
 If not,
```

### Comparing `srsinst.rga-0.3.0/README.md` & `srsinst.rga-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 # `srsinst.rga`
 
 `srsinst.rga` provides Python instrument classes to control and acquire mass spectra from 
 [Stanford Research Systems (SRS) Residual Gas Analyzers (RGA)](https://thinksrs.com/products/rga.html).
 It also provides tasks running in GUI environment based on 
 [srsgui](https://thinksrs.github.io/srsgui/).  
-To operate SRS RGA with this package safely, you need to be familiar with SRS RGA. 
+To operate an SRS RGA with this package safely, you need to be familiar with SRS RGAs. 
 For detailed information, refer to the 
 [manual](https://thinksrs.com/downloads/pdfs/manuals/RGAm.pdf).
 
-![screenshot](https://github.com/thinkSRS/srsinst.rga/blob/main/docs/_static/image/derived-pvst-plot-screenshot.png " ")
+![screenshot](https://github.com/thinkSRS/srsinst.rga/blob/main/docs/_static/image/comp-analysis-screenshot.png " ")
 
 ## Installation
-You need a working Python with `pip` (Python package installer) installed. If you don't,
-[install Python 3](https://realpython.com/installing-python/) to your system.
-
-To install `srsinst.rga` as an instrument driver only, use Python package installer `pip` 
-from the command line.
-
-    python -m pip install srsinst.rga
+You need a working Python version 3.7 or later with `pip` (Python package installer) installed. 
+If you don't, [install Python 3](https://www.python.org/) to your system.
 
 To use its full GUI application, create a virtual environment, if necessary,
-and install with *[full]* option:
+and rub Python package installer `pip` with *[full]* option from the command prompt.
+
+    # To create a simple virtual environment (Optional) 
+    # The activate command may differ depending on your computer operating systems.
+    # Following is for Windows.
 
-    # To create a simple virtual environment (Optional)
     python -m venv venv
     venv\scripts\activate
 
-    # To install full GUI application 
+    # To install full GUI application
+
     python -m pip install srsinst.rga[full]
 
 
+To install `srsinst.rga` as an instrument driver only, install WITHOUT the *[full]* option. 
+Installation will be faster, because it does NOT install GUI related packages.
+
+    python -m pip install srsinst.rga
+
+
 ## Run `srsinst.rga` as GUI application
 If the Python Scripts directory is in PATH environment variable,
 Start the application by typing from the command line:
 
     rga
 
 If not,
```

### Comparing `srsinst.rga-0.3.0/docs/_static/image/derived-pvst-plot-screenshot.png` & `srsinst.rga-0.3.1/docs/_static/image/derived-pvst-plot-screenshot.png`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.0/srsinst/rga/gaslib.dat` & `srsinst.rga-0.3.1/srsinst/rga/gaslib.dat`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 
 # Gas Library for composition analysis
+
 # Fragmentation ratio of a gas in this library is just for reference.
-# The real ratio obtained from you mass spectrometer may be different.
+# The real ratio obtained from your mass spectrometer may be different.
 # Usually the higher mass, the lower intensity than the ones on this library.
 # Adjust the peak intensities in the library to fit spectra you acquire,
-# if you know what you are doing.
+# if you know what you are doing (Make a backup before changing the values in the library).
 
 # Adjust the sensitivity factor, if you know the real partial pressure of the gas,
 # to match the principal peak intensity of the gas to the partial pressure of the gas
 
-# Reduction ratio is for UGA system which samples atmospheric pressure gas.
-# sampling partial pressure is reduced to the vacuum chamber partial pressure to operate
+# Reduction ratio is for UGA systems which samples gases in the atmospheric pressure.
+# The sampling partial pressure is reduced to the vacuum chamber partial pressure to operate
 # the mass spectrometer safely.
 
 # Each gas consists of 3 lines
 # "Name of gas" "Sensitivity factor" "Reduction factor"
 # Peak positions (AMU)
 # Percent peak intensities with respect to the principal peak
```

### Comparing `srsinst.rga-0.3.0/srsinst/rga/instruments/get_instruments.py` & `srsinst.rga-0.3.1/srsinst/rga/instruments/get_instruments.py`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.0/srsinst/rga/instruments/rga100/commands.py` & `srsinst.rga-0.3.1/srsinst/rga/instruments/rga100/commands.py`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.0/srsinst/rga/instruments/rga100/components.py` & `srsinst.rga-0.3.1/srsinst/rga/instruments/rga100/components.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,26 @@
 from .commands import FloatNSCommand, BoolSetNSCommand,\
                       RgaIntCommand, RgaFloatCommand, \
                       RgaIonEnergyCommand, RgaTotalPressureCommand, \
                       RgaStoredCEMGainCommand
 from .errors import query_errors, fetch_error_descriptions
 
 
+class Defaults:
+    """
+    SRS RGA default values after reset
+    """
+    ElectronEnergy = 70
+    IonEnergy = 12
+    FocusVoltage = 90
+    InitialMass = 1
+    ScanSpeed = 4
+    StepsPerAmu = 10
+
+
 class Ionizer(Component):
     electron_energy = RgaIntCommand('EE', 'eV', 25, 105, 1, 70)
     ion_energy = RgaIonEnergyCommand('IE', 'eV', 8, 12, 4, 12)
     focus_voltage = RgaIntCommand('VF', 'V', 0, 150, 1, 90)
     emission_current = RgaFloatCommand('FL', 'mA', 0.0, 3.5, 0.01, 2, 1.0)
     """
     For typical operation, set emission current to 1 (mA).
@@ -38,15 +50,18 @@
         --------
             tuple
                 (electron_energy, ion_energy, focus_voltage)
         """
 
         return self.electron_energy, self.ion_energy, self.focus_voltage
 
-    def set_parameters(self, electron_energy, ion_energy, focus_voltage):
+    def set_parameters(self,
+                       electron_energy=Defaults.ElectronEnergy,
+                       ion_energy=Defaults.IonEnergy,
+                       focus_voltage=Defaults.FocusVoltage):
         """
         Set electron energy, ion energy and focus voltage
 
         Parameters
         -----------
             electron_energy : int
                 electron energy electron impact ionization
```

### Comparing `srsinst.rga-0.3.0/srsinst/rga/instruments/rga100/errors.py` & `srsinst.rga-0.3.1/srsinst/rga/instruments/rga100/errors.py`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.0/srsinst/rga/instruments/rga100/rga.py` & `srsinst.rga-0.3.1/srsinst/rga/instruments/rga100/rga.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,26 +15,14 @@
 from srsgui import SerialInterface, TcpipInterface
 from srsgui import FindListInput, Ip4Input, StringInput, PasswordInput, IntegerInput
 
 from .scans import Scans, Scans200, Scans300
 from .components import QMF, Ionizer, Filament, CEM, Pressure, Status
 
 
-class Defaults:
-    """
-    SRS RGA default values after reset
-    """
-    ElectronEnergy = 70
-    IonEnergy = 12
-    FocusVoltage = 90
-    InitialMass = 1
-    ScanSpeed = 4
-    StepsPerAmu = 10
-
-
 class RGA100(Instrument):
     """
     Class to control and acquire data with
     `SRS RGA100, 200, 300 series <https://www.thinksrs.com/products/rga.html>`_.
 
     A native SRS RGA has a RS232 serial port that connects with
     baud rate of 28800, one stop bit, no parity, with RTS/CTS flow control.
@@ -51,24 +39,24 @@
 
         from srsinst.rga import RGA100
         r1 = RGA100('serial', 'COM3', 28800)
 
         # if Ethernet connection is used,
         # r1 = RGA100('tcpip', '192.168.1.100', 'userid', 'password')
 
-        r1.set_emission_current(1.0)
-        r1.set_scan_parameters()
+        r1.filament.turn_on()
+        r1.set_scan_parameters() # Set to defaults
 
-        xs = r1.get_mass_axis()
-        ys = r1.get_analog_scan()
+        xs = r1.scan.get_mass_axis()
+        ys = r1.scan.get_analog_scan()
 
         for x, y in zip(xs, ys):
             print(x, y)
 
-        r1.set_emission_current(0.0)
+        r1.filament.turn_off()
         r1.disconnect()
 
     """
 
     _IdString = 'SRSRGA'
     _term_char = b'\r'
 
@@ -87,15 +75,14 @@
                 'password': PasswordInput('admin'),
                 'port': 818
             }
         ],
     ]
 
     def __init__(self, interface_type=None, *args):
-
         super().__init__(interface_type, *args)
         self.set_term_char(b'\r')
         self._m_max = Scans.MaxMass
 
         # Add components
         self.ionizer = Ionizer(self)
         self.filament = Filament(self)
@@ -114,41 +101,49 @@
         Parameters
         -----------
             interface_type: str
                 Use **'serial'** for serial communication
             port : string
                 serial port,  such as 'COM3' or '/dev/ttyUSB0'
             baud_rate : int, optional
-                baud rate of the serial port, default is 114200, and SRS RGA uses 28800.
+                baud rate of the serial port, the Instrument class default is 114200, but RGA100 uses **28800** only.
             hardware_flow_control: bool, optional
-                RTS/CTS setting. The default is False, SRS RGA requires **True**.
+                RTS/CTS setting. The Instrument class default is False, however, RGA100 requires **True**.
 
         If interface_type is 'tcpip',
 
         Parameters
         -----------
             interface_type: str
                 Use **'tcpip'** for Ethernet communication
             ip_address: str
                 IP address of a instrument
             user_id: str
                 user name for login.
             password : str
                 password for login.
             port : int, optional
-                TCP port number. The default is 818, which SRS RGA uses
+                TCP port number. The default is 818.
 
         """
         super().connect(interface_type, *args)
         if type(self.comm) == SerialInterface:
             # Make sure the hardware flow control is set
             self.comm._serial.rtscts = True
 
     def check_id(self):
+        """
+        Check if the connected instrument returns the right ID string
+        and adjust the maximum mass depending on the ID string.
 
+        returns
+        --------
+            tuple
+                (model_name, serial_number, firmware_version)
+        """
         self._m_max = 100
         if not self.is_connected():
             return None, None, None
 
         reply = self.query_text('ID?').strip()
 
         if len(reply) < 20:
@@ -170,23 +165,23 @@
 
         self._model_name = model_name
         self._serial_number = serial_number
         self._firmware_version = firmware_version
 
         if self._m_max >= 300:
             self._m_max = 300
-            if type(self.scan) is not Scans300:
+            if not isinstance(self.scan, Scans300):
                 self.scan = Scans300(self)
         elif self._m_max >= 200:
             self._m_max = 200
-            if type(self.scan) is not Scans200:
+            if not isinstance(self.scan, Scans200):
                 self.scan = Scans200(self)
         elif self._m_max >= 100:
             self._m_max = 100
-            if type(self.scan) is not Scans:
+            if not isinstance(self.scan, Scans):
                 self.scan = Scans(self)
         return self._model_name, self._serial_number, self._firmware_version
 
     def get_status(self):
         status_string = 'Emission current: {:.2f} mA\n'.format(self.ionizer.emission_current)
         status_string += 'CEM HV: {:.0f} V\n'.format(self.cem.voltage)
         status_string += self.status.get_error_text()
```

### Comparing `srsinst.rga-0.3.0/srsinst/rga/instruments/rga100/rga_commands.json` & `srsinst.rga-0.3.1/srsinst/rga/instruments/rga100/rga_commands.json`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.0/srsinst/rga/instruments/rga100/scans.py` & `srsinst.rga-0.3.1/srsinst/rga/instruments/rga100/scans.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,22 +7,24 @@
 import numpy as np
 
 from srsgui.inst.communications import Interface, SerialInterface, TcpipInterface
 from srsgui.inst.component import Component
 from srsgui.inst.commands import IntGetCommand
 
 from .commands import IntNSCommand
+from .components import Defaults
 
 
 class Scans(Component):
-    MaxMass = 100
     """
-    Component for scan setup and data acquisition from SRS RGAs
+    Component for scan setup and data acquisition for RGA100 class
     """
 
+    MaxMass = 100
+
     initial_mass = IntNSCommand('MI', 'AMU', 1, MaxMass, 1, 1)
     final_mass = IntNSCommand('MF', 'AMU', 1, MaxMass, 1, MaxMass)
     speed = IntNSCommand('NF', '', 0, 7, 1, 4)
     resolution = IntNSCommand('SA', 'points/AMU', 10, 25, 1, 10)
     total_points_analog = IntGetCommand('AP', 'points')
     total_points_histogram = IntGetCommand('HP', 'points')
 
@@ -109,15 +111,19 @@
         Returns
         ---------
             (int, int, int, int)
                 tuple of (initial_mass, final_mass, scan_speed, steps_per_amu)
         """
         return self.initial_mass, self.final_mass, self.speed, self.resolution
 
-    def set_parameters(self, initial_mass=1, final_mass=65, scan_speed=4, steps_per_amu=10):
+    def set_parameters(self,
+                       initial_mass=Defaults.InitialMass,
+                       final_mass=65,
+                       scan_speed=Defaults.ScanSpeed,
+                       steps_per_amu=Defaults.StepsPerAmu):
         """
         Set scan parameters
 
         Parameters
         -------------
             initial_mass: int, optional
                 the initial mass of an analog or histogram scan. The default is 1 AMU
@@ -129,14 +135,15 @@
                 steps for 1 AMU in analog scan, between 10 and 25. The default is 10.
                 For a histogram scan, it is 1
         """
 
         self.final_mass = self.get_max_mass()
         self.initial_mass = initial_mass
         self.final_mass = final_mass
+        temp = self.final_mass  # To add a pause
         self.speed = scan_speed
         self.resolution = steps_per_amu
 
     def read_long(self):
         data = self.comm._read_binary(4)
         intensity = self.convert_to_long(data)
         return intensity
```

### Comparing `srsinst.rga-0.3.0/srsinst/rga/instruments/rga100/sicp.py` & `srsinst.rga-0.3.1/srsinst/rga/instruments/rga100/sicp.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ##! Subject to the MIT License
 ##! 
 
 """
 SRS Internet Configuration Protocol (SICP) class
 
 The RGA120 series and RGA Ethernet Adapter (REA) use the IP configuration over UDP broadcasting, SRS IP Configuration protocol (SICP). When a search
-packet is broadcasted, all SICP enabled devices on the Local Area Network (LAN)
+packet is broadcast, all SICP enabled devices on the Local Area Network (LAN)
 will respond with a packet. From those packets, you can find available devices
 on the network.
 
 If an instrument is waiting for IP configuration, you can change
 the IP settings by broadcasting another packet. For REAs, the IP setting is only
 available by power-cycle with a hardware button pressed. For RGA120s, the IP setting is available when the ECU is powered while unplugged
 from the probe.
```

### Comparing `srsinst.rga-0.3.0/srsinst/rga/plots/analogscanplot.py` & `srsinst.rga-0.3.1/srsinst/rga/plots/analogscanplot.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,33 @@
 from srsinst.rga.plots.analysis import calculate_baseline
 from srsinst.rga.instruments.rga100.scans import Scans
 
 logger = logging.getLogger(__name__)
 
 
 class AnalogScanPlot(BaseScanPlot):
+    """
+    Class to manage an analog scan plot with data generated from the parent task
+
+    parameters
+    -----------
+
+        parent: Task
+            It uses resources from the parent task
+
+        scan: Scans
+            an instance of Scans class in an instance of RGA100 class
+
+        plot_name: str
+            name of the plot used as title of the plot and name of the dict for scan data saving
+
+        save_to_file: bool
+            to create a table in the data file
+    """
+
     def __init__(self, parent: Task, ax: Axes, scan: Scans, plot_name='', save_to_file=True):
         if not issubclass(type(parent), Task):
             raise TypeError('Invalid parent {} is not a Task subclass'.format(type(parent)))
         if not hasattr(ax, 'figure'):
             raise TypeError('ax has no figure attribute. type: "{}"'.format(type(ax)))
 
         super().__init__(parent, ax, plot_name, save_to_file)
@@ -36,14 +55,15 @@
         self.prev_baseline, = self.ax.plot(self.data['x'], self.data['y'], label='Prev. baseline')
 
         self.ax.set_ylim(1, 10000)
 
         self.reset()
 
     def reset(self):
+
         self.first_scan = True
         self.initial_mass = self.scan.initial_mass
         self.final_mass = self.scan.final_mass
         self.resolution = self.scan.resolution
         self.set_x_axis(self.scan.get_mass_axis(True))
 
         self.ax.set_xlim(self.initial_mass, self.final_mass, auto=False)
```

### Comparing `srsinst.rga-0.3.0/srsinst/rga/plots/analysis.py` & `srsinst.rga-0.3.1/srsinst/rga/plots/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         return z, d, info
     else:
         return z
 
 
 def get_peak_from_analog_scan(x, y, mass, fit=False):
     """
-    Calculate a peak intensity from an analog scan spectrum
+    Calculate the intensity of a peak in an analog scan spectrum
 
     Parameters
     -----------
         x: Numpy array
             mass axis values
         y: Numpy array
             intensity array
```

### Comparing `srsinst.rga-0.3.0/srsinst/rga/plots/basescanplot.py` & `srsinst.rga-0.3.1/srsinst/rga/plots/basescanplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,19 @@
 from matplotlib.axes import Axes
 from srsgui import Task
 
 logger = logging.getLogger(__name__)
 
 
 class BaseScanPlot:
+    """
+    Base class for scan plots
+
+    """
+
     def __init__(self, parent: Task, ax: Axes, plot_name='', save_to_file=False):
         self.type = self.__class__.__name__
         self.parent = parent
         self.ax = ax
         self.name = plot_name.strip()
 
         self.conversion_factor = 1
```

### Comparing `srsinst.rga-0.3.0/srsinst/rga/plots/histogramscanplot.py` & `srsinst.rga-0.3.1/srsinst/rga/plots/histogramscanplot.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,20 +7,37 @@
 import numpy
 from matplotlib.axes import Axes
 from srsgui import Task
 from srsinst.rga.plots.basescanplot import BaseScanPlot
 
 from srsinst.rga.instruments.rga100.scans import Scans
 
-
-
 logger = logging.getLogger(__name__)
 
 
 class HistogramScanPlot(BaseScanPlot):
+    """
+    Class to manage an histogram scan bar graph with data generated from the parent task
+
+    parameters
+    -----------
+
+        parent: Task
+            It uses resources from the parent task
+
+        scan: Scans
+            an instance of Scans class in an instance of RGA100 class
+
+        plot_name: str
+            name of the plot used as title of the plot and name of the dict for scan data saving
+
+        save_to_file: bool
+            to create a table in the data file
+    """
+
     def __init__(self, parent: Task, ax: Axes, scan: Scans, plot_name='', save_to_file=True):
         if not issubclass(type(parent), Task):
             raise TypeError('Invalid parent {} is not a Task subclass'.format(type(parent)))
         if not hasattr(ax, 'figure'):
             raise TypeError('ax has no figure attribute. type: "{}"'.format(type(ax)))
         super().__init__(parent, ax, plot_name, save_to_file)
```

### Comparing `srsinst.rga-0.3.0/srsinst/rga/plots/timeplot.py` & `srsinst.rga-0.3.1/srsinst/rga/plots/timeplot.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,18 +10,46 @@
 from matplotlib.axes import Axes
 from srsgui import Task
 
 logger = logging.getLogger(__name__)
 
 
 class TimePlot:
+    """
+    Class to manage a plot for multiple time-series data generated in the parent task
+
+    parameters
+    -----------
+
+        parent: Task
+            It uses resources from the parent task
+
+        ax: Axes
+            Matplotlib Axes on which it makes a plot
+
+        data_names: tuple or list
+            list of names of time series data. It specifies the number of data sets, too.
+
+        save_to_file: bool
+            Allow To create a table in the data file
+
+        use_datetime: bool
+            To use datetime format for x axis, otherwise it uses the elapsed time in seconds
+
+        plot_options: list of dict
+            each element of the list with the matching element in data_names
+            will be passed to Matplotlib Axes.plot as **kwarg, if exists.
+    """
+
     def __init__(self, parent: Task, ax: Axes, plot_name='', data_names=('Y',), save_to_file=True,
                  use_datetime=True, plot_options=None):
+
         if plot_options is None:
-            plot_options = {}
+            plot_options = []
+
         if not issubclass(type(parent), Task):
             raise TypeError('Invalid parent {} is not a Task subclass'.format(type(parent)))
         # if type(ax) is not Axes or AxesSubplot:
         #    raise TypeError('ax is not a Matplotlib Axes class, but "{}"'.format(type(ax)))
 
         self.type = self.__class__.__name__
         self.parent = parent
@@ -51,17 +79,24 @@
         self.max_points_in_plot = 10000  # Maximum point to plot
 
         if self.use_datetime:
             self.time = np.zeros(self._data_buffer_size).astype('datetime64[ms]')
         else:
             self.time = np.zeros(self._data_buffer_size, dtype=np.float64)
 
-        for key in self.data_keys:
+        for index, key in enumerate(self.data_keys):
+            try:
+                options = plot_options[index]
+                if type(options) is not dict:
+                    raise TypeError
+            except (IndexError, TypeError):
+                options = {}
+
             self.data[key] = np.zeros(self._data_buffer_size)
-            self.lines[key], = self.ax.plot([1.0], [1.0], label=key)
+            self.lines[key], = self.ax.plot([1.0], [1.0], label=key, **options)
 
         # significant digits in a number in text
         self.round_float_resolution = 4
         self.header_saved = False
 
         self.ax.set_title(self.name)
 
@@ -85,14 +120,15 @@
 
     def on_xlim_changed(self, event_ax):
         self.update_plot()
 
     def on_pick(self, event):
         """
         Toggle a line from the line corresponding in the legend
+
         https://matplotlib.org/stable/gallery/event_handling/legend_picking.html
         """
         legline = event.artist
         origline = self.lined[legline]
         visible = not origline.get_visible()
         origline.set_visible(visible)
         legline.set_alpha(1.0 if visible else 0.3)
```

### Comparing `srsinst.rga-0.3.0/srsinst/rga/rga.taskconfig` & `srsinst.rga-0.3.1/srsinst/rga/rga.taskconfig`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Line that starts with '#' is a comment line
 # RGA Task list for srsgui
 
 # The name is used for the main window title
 
 Name: RGA Tasks
 
-
 # Specify Instruments used in the task suite
 # A line that starts with 'inst' adds an instrument to be used in the following tasks.
 # An instrument is a subclass derived from Instrument class in 'srsgui' package
 # The second column is the name of the Python module or package that contains the instrument class.
 # The third column is a instrument class in the module
 # The fourth column is connection parameters.
 # If the fourth item is given, the instrument will be connected using the parameters
```

### Comparing `srsinst.rga-0.3.0/srsinst/rga/tasks/analogscantask.py` & `srsinst.rga-0.3.1/srsinst/rga/tasks/analogscantask.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,18 @@
         IntensityUnit: ListInput(['Ion current (fA)', 'Partial Pressure (Torr)']),
     }
 
     def setup(self):
         # Get values to use for task  from input_parameters in GUI
         self.params = self.get_all_input_parameters()
 
+        # Get the instrument to use
+        self.rga = get_rga(self, self.params[self.InstrumentName])
+        self.id_string = self.rga.status.id_string
+
         # Get logger to use
         self.logger = self.get_logger(__name__)
 
         self.init_scan()
 
         # Set up an analog scan plot
         self.ax = self.get_figure().add_subplot(111)
@@ -50,22 +54,19 @@
             self.conversion_factor = 0.1
             self.plot.set_conversion_factor(self.conversion_factor, 'fA')
         else:
             self.conversion_factor = self.rga.pressure.get_partial_pressure_sensitivity_in_torr()
             self.plot.set_conversion_factor(self.conversion_factor, 'Torr')
 
     def init_scan(self):
-        # Get the instrument to use
-        self.rga = get_rga(self, self.params[self.InstrumentName])
-        self.id_string = self.rga.status.id_string
-
         emission_current = self.rga.ionizer.emission_current
         cem_voltage = self.rga.cem.voltage
 
         self.logger.info('Emission current: {:.2f} mA CEM HV: {} V'.format(emission_current, cem_voltage))
+
         self.rga.scan.set_parameters(self.params[self.StartMass],
                                      self.params[self.StopMass],
                                      self.params[self.ScanSpeed],
                                      self.params[self.StepSize])
 
     def test(self):
         self.set_task_passed(True)
```

### Comparing `srsinst.rga-0.3.0/srsinst/rga/tasks/cemcontroltask.py` & `srsinst.rga-0.3.1/srsinst/rga/tasks/cemcontroltask.py`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.0/srsinst/rga/tasks/cemgaintask.py` & `srsinst.rga-0.3.1/srsinst/rga/tasks/cemgaintask.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,14 +169,15 @@
         self.logger.info(f'Measured gain at HV {hv_to_set:.0f} V : {measured_gain:.0f}')
 
         # If the gain error is larger than 10 %, set it to fail
         error = abs(measured_gain - self.params[self.GainToSet]) / self.params[self.GainToSet]
         if error <= 0.10:
             self.rga.cem.voltage = hv_to_set
             self.rga.cem.stored_gain = round(measured_gain, 1)
+            self.rga.cem.stored_voltage = round(hv_to_set)
             self.set_task_passed(True)
             self.add_details(f'Gain at {hv_to_set:.0f} V : {measured_gain:.0f}')
         else:
             self.set_task_passed(False)
 
     def update(self, data_dict):
         """
```

### Comparing `srsinst.rga-0.3.0/srsinst/rga/tasks/compositionanalysistask.py` & `srsinst.rga-0.3.1/srsinst/rga/tasks/compositionanalysistask.py`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.0/srsinst/rga/tasks/derivedpvstscantask.py` & `srsinst.rga-0.3.1/srsinst/rga/tasks/derivedpvstscantask.py`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.0/srsinst/rga/tasks/filamentcontroltask.py` & `srsinst.rga-0.3.1/srsinst/rga/tasks/filamentcontroltask.py`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.0/srsinst/rga/tasks/histogramscantask.py` & `srsinst.rga-0.3.1/srsinst/rga/tasks/histogramscantask.py`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.0/srsinst/rga/tasks/peaktuningtask.py` & `srsinst.rga-0.3.1/srsinst/rga/tasks/peaktuningtask.py`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.0/srsinst/rga/tasks/pvstscantask.py` & `srsinst.rga-0.3.1/srsinst/rga/tasks/pvstscantask.py`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.0/srsinst/rga/tasks/searchlan.py` & `srsinst.rga-0.3.1/srsinst/rga/tasks/searchlan.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,24 +5,39 @@
 
 from srsgui import Task
 from srsgui.task.inputs import ListInput
 from srsinst.rga import SICP
 
 
 class SearchLanTask(Task):
-    """Search for RGAs on the local area network (LAN) using SICP.
-It may not work if a computer firewall blocks UDP port 818 used for broadcast.
+    """
+Search for RGAs on the local area network (LAN) using :mod:`SICP<srsinst.rga.instruments.rga100.sicp>`.
+
+The information on the all RGAs found displayed in the console with the display option.
+Available RGAs are displayed in the task result panel.
+
+It does not ot work if the computer firewall blocks communication on the UDP port 818 used for broadcast.
+
+    parameters
+    -----------
+
+        display option:
+            The format of output display in the console: Short or Full
+
     """
 
     # Input parameter name
     DisplayOption = 'display option'
 
+    OptionShort = 'Short'
+    OptionFull = 'Full'
+
     # input_parameters values are used to change interactively from GUI
     input_parameters = {
-        DisplayOption: ListInput(['Short', 'Full']),
+        DisplayOption: ListInput([OptionShort, OptionFull]),
     }
 
     def setup(self):
         # Get the logger to use
         self.logger = self.get_logger(__name__)
 
         # Get the input parameters from GUI
@@ -36,16 +51,17 @@
         if len(sicp.packet_list) == 0:
             self.logger.info('No RGAs found')
             self.set_task_passed(True)
             return
 
         self.display_result('\nAvailable RGAs')
         self.display_result('================')
+        print('Option: {}'.format(self.params[self.DisplayOption]))
         for p in sicp.packet_list:
-            if self.params[self.DisplayOption] == 0:
+            if self.params[self.DisplayOption] == self.OptionShort:
                 self.logger.info('Name: {:20s}, SN: {}, IP: {}, Status: {}'
                                  .format(p.device_name, p.serial_number,
                                          p.convert_to_ip_format(p.ip_address),
                                          p.get_short_status_from_packet()))
             else:
                 p.print_info()
```

### Comparing `srsinst.rga-0.3.0/srsinst.rga.egg-info/PKG-INFO` & `srsinst.rga-0.3.1/srsinst.rga.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,68 @@
 Metadata-Version: 2.1
 Name: srsinst.rga
-Version: 0.3.0
+Version: 0.3.1
 Summary: Instrument driver package for Residual Gas Analyzers (RGA) from Stanford Research Systems
 Author: Chulhoon Kim
 License: MIT license
+Project-URL: homepage, https://github.com/thinkSRS/srsinst.rga
+Project-URL: repository, https://github.com/thinkSRS/srsinst.rga.git
+Project-URL: documentation, https://thinksrs.github.io/srsinst.rga
 Keywords: RGA,residual gas analyzer,SRS,Stanford Research Systems
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: full
+Provides-Extra: docs
 License-File: LICENSE
 
 # `srsinst.rga`
 
 `srsinst.rga` provides Python instrument classes to control and acquire mass spectra from 
 [Stanford Research Systems (SRS) Residual Gas Analyzers (RGA)](https://thinksrs.com/products/rga.html).
 It also provides tasks running in GUI environment based on 
 [srsgui](https://thinksrs.github.io/srsgui/).  
-To operate SRS RGA with this package safely, you need to be familiar with SRS RGA. 
+To operate an SRS RGA with this package safely, you need to be familiar with SRS RGAs. 
 For detailed information, refer to the 
 [manual](https://thinksrs.com/downloads/pdfs/manuals/RGAm.pdf).
 
-![screenshot](https://github.com/thinkSRS/srsinst.rga/blob/main/docs/_static/image/derived-pvst-plot-screenshot.png " ")
+![screenshot](https://github.com/thinkSRS/srsinst.rga/blob/main/docs/_static/image/comp-analysis-screenshot.png " ")
 
 ## Installation
-You need a working Python with `pip` (Python package installer) installed. If you don't,
-[install Python 3](https://realpython.com/installing-python/) to your system.
-
-To install `srsinst.rga` as an instrument driver only, use Python package installer `pip` 
-from the command line.
-
-    python -m pip install srsinst.rga
+You need a working Python version 3.7 or later with `pip` (Python package installer) installed. 
+If you don't, [install Python 3](https://www.python.org/) to your system.
 
 To use its full GUI application, create a virtual environment, if necessary,
-and install with *[full]* option:
+and rub Python package installer `pip` with *[full]* option from the command prompt.
+
+    # To create a simple virtual environment (Optional) 
+    # The activate command may differ depending on your computer operating systems.
+    # Following is for Windows.
 
-    # To create a simple virtual environment (Optional)
     python -m venv venv
     venv\scripts\activate
 
-    # To install full GUI application 
+    # To install full GUI application
+
     python -m pip install srsinst.rga[full]
 
 
+To install `srsinst.rga` as an instrument driver only, install WITHOUT the *[full]* option. 
+Installation will be faster, because it does NOT install GUI related packages.
+
+    python -m pip install srsinst.rga
+
+
 ## Run `srsinst.rga` as GUI application
 If the Python Scripts directory is in PATH environment variable,
 Start the application by typing from the command line:
 
     rga
 
 If not,
```

