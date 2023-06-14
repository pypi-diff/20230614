# Comparing `tmp/srsinst.rga-0.3.2.tar.gz` & `tmp/srsinst.rga-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\PyPI\instrument_library\rga100\dist\.tmp-x4sk8_99\srsinst.rga-0.3.2.tar", last modified: Wed Jun 14 00:11:01 2023, max compression
+gzip compressed data, was "C:\PyPI\instrument_library\rga100\dist\.tmp-2q4_xfpq\srsinst.rga-0.3.3.tar", last modified: Wed Jun 14 20:09:00 2023, max compression
```

## Comparing `srsinst.rga-0.3.2.tar` & `srsinst.rga-0.3.3.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 00:11:01.680223 srsinst.rga-0.3.2/
--rw-rw-rw-   0        0        0     1113 2023-05-16 22:11:28.000000 srsinst.rga-0.3.2/LICENSE
--rw-rw-rw-   0        0        0     6841 2023-06-14 00:11:01.680223 srsinst.rga-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     5838 2023-06-14 00:09:13.000000 srsinst.rga-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 00:11:01.638137 srsinst.rga-0.3.2/docs/
--rw-rw-rw-   0        0        0      654 2023-05-19 21:28:01.000000 srsinst.rga-0.3.2/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-06-14 00:11:01.622069 srsinst.rga-0.3.2/docs/_static/
-drwxrwxrwx   0        0        0        0 2023-06-14 00:11:01.638137 srsinst.rga-0.3.2/docs/_static/image/
--rw-rw-rw-   0        0        0   174977 2023-06-09 18:18:12.000000 srsinst.rga-0.3.2/docs/_static/image/comp-analysis-screenshot.png
--rw-rw-rw-   0        0        0   115947 2023-05-19 17:56:22.000000 srsinst.rga-0.3.2/docs/_static/image/derived-pvst-plot-screenshot.png
--rw-rw-rw-   0        0        0    51322 2023-06-09 22:02:41.000000 srsinst.rga-0.3.2/docs/_static/image/initial-screen-capture.png
--rw-rw-rw-   0        0        0    27661 2023-05-25 23:24:03.000000 srsinst.rga-0.3.2/docs/_static/image/simple-analog-scan-screenshot.png
--rw-rw-rw-   0        0        0     1970 2023-06-13 20:55:52.000000 srsinst.rga-0.3.2/docs/conf.py
--rw-rw-rw-   0        0        0      356 2023-06-01 23:58:11.000000 srsinst.rga-0.3.2/docs/custom_tasks.rst
--rw-rw-rw-   0        0        0     6252 2023-06-12 22:33:57.000000 srsinst.rga-0.3.2/docs/gui_application.rst
--rw-rw-rw-   0        0        0     2584 2023-06-12 23:28:46.000000 srsinst.rga-0.3.2/docs/index.rst
--rw-rw-rw-   0        0        0     4199 2023-06-12 17:15:20.000000 srsinst.rga-0.3.2/docs/installation.rst
--rw-rw-rw-   0        0        0    16282 2023-06-12 20:44:51.000000 srsinst.rga-0.3.2/docs/instrument_driver.rst
--rwxrwxrwx   0        0        0      802 2023-05-19 21:28:01.000000 srsinst.rga-0.3.2/docs/make.bat
--rw-rw-rw-   0        0        0       32 2023-05-19 21:28:01.000000 srsinst.rga-0.3.2/docs/requirements.txt
--rw-rw-rw-   0        0        0     1332 2023-05-31 23:18:38.000000 srsinst.rga-0.3.2/docs/srsinst.rga.instruments.rga100.rst
--rw-rw-rw-   0        0        0      358 2023-05-19 21:28:01.000000 srsinst.rga-0.3.2/docs/srsinst.rga.instruments.rst
--rw-rw-rw-   0        0        0     1049 2023-06-09 19:15:10.000000 srsinst.rga-0.3.2/docs/srsinst.rga.plots.rst
--rw-rw-rw-   0        0        0      148 2023-05-31 23:17:11.000000 srsinst.rga-0.3.2/docs/srsinst.rga.rst
--rw-rw-rw-   0        0        0     2095 2023-06-06 22:33:30.000000 srsinst.rga-0.3.2/docs/srsinst.rga.tasks.rst
--rw-rw-rw-   0        0        0     1488 2023-06-13 21:05:18.000000 srsinst.rga-0.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-14 00:11:01.680223 srsinst.rga-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsinst.rga-0.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 00:11:01.622069 srsinst.rga-0.3.2/srsinst/
-drwxrwxrwx   0        0        0        0 2023-06-14 00:11:01.650220 srsinst.rga-0.3.2/srsinst/rga/
--rw-rw-rw-   0        0        0      349 2023-06-14 00:10:36.000000 srsinst.rga-0.3.2/srsinst/rga/__init__.py
--rw-rw-rw-   0        0        0      483 2023-05-19 21:11:26.000000 srsinst.rga-0.3.2/srsinst/rga/__main__.py
--rw-rw-rw-   0        0        0    10675 2023-06-01 21:25:29.000000 srsinst.rga-0.3.2/srsinst/rga/gaslib.dat
-drwxrwxrwx   0        0        0        0 2023-06-14 00:11:01.650220 srsinst.rga-0.3.2/srsinst/rga/instruments/
--rw-rw-rw-   0        0        0        0 2023-06-13 23:56:14.000000 srsinst.rga-0.3.2/srsinst/rga/instruments/__init__.py
--rw-rw-rw-   0        0        0      872 2023-05-19 21:13:35.000000 srsinst.rga-0.3.2/srsinst/rga/instruments/get_instruments.py
-drwxrwxrwx   0        0        0        0 2023-06-14 00:11:01.660223 srsinst.rga-0.3.2/srsinst/rga/instruments/rga100/
--rw-rw-rw-   0        0        0        0 2023-05-19 21:11:26.000000 srsinst.rga-0.3.2/srsinst/rga/instruments/rga100/__init__.py
--rw-rw-rw-   0        0        0     5249 2023-05-19 21:13:35.000000 srsinst.rga-0.3.2/srsinst/rga/instruments/rga100/commands.py
--rw-rw-rw-   0        0        0     7355 2023-05-25 20:26:25.000000 srsinst.rga-0.3.2/srsinst/rga/instruments/rga100/components.py
--rw-rw-rw-   0        0        0     4510 2023-05-19 21:13:35.000000 srsinst.rga-0.3.2/srsinst/rga/instruments/rga100/errors.py
--rw-rw-rw-   0        0        0     8719 2023-06-13 23:56:14.000000 srsinst.rga-0.3.2/srsinst/rga/instruments/rga100/rga.py
--rw-rw-rw-   0        0        0    18656 2023-05-19 21:11:26.000000 srsinst.rga-0.3.2/srsinst/rga/instruments/rga100/rga_commands.json
--rw-rw-rw-   0        0        0    11740 2023-05-31 21:39:25.000000 srsinst.rga-0.3.2/srsinst/rga/instruments/rga100/scans.py
--rw-rw-rw-   0        0        0     9870 2023-06-06 21:51:12.000000 srsinst.rga-0.3.2/srsinst/rga/instruments/rga100/sicp.py
-drwxrwxrwx   0        0        0        0 2023-06-14 00:11:01.670223 srsinst.rga-0.3.2/srsinst/rga/plots/
--rw-rw-rw-   0        0        0        0 2023-05-19 21:11:26.000000 srsinst.rga-0.3.2/srsinst/rga/plots/__init__.py
--rw-rw-rw-   0        0        0     4122 2023-06-09 19:33:09.000000 srsinst.rga-0.3.2/srsinst/rga/plots/analogscanplot.py
--rw-rw-rw-   0        0        0     3448 2023-06-09 18:23:15.000000 srsinst.rga-0.3.2/srsinst/rga/plots/analysis.py
--rw-rw-rw-   0        0        0     3287 2023-06-09 19:32:57.000000 srsinst.rga-0.3.2/srsinst/rga/plots/basescanplot.py
--rw-rw-rw-   0        0        0     3792 2023-06-09 19:32:57.000000 srsinst.rga-0.3.2/srsinst/rga/plots/histogramscanplot.py
--rw-rw-rw-   0        0        0     9182 2023-06-09 19:33:28.000000 srsinst.rga-0.3.2/srsinst/rga/plots/timeplot.py
--rw-rw-rw-   0        0        0     2226 2023-06-01 00:10:48.000000 srsinst.rga-0.3.2/srsinst/rga/rga.taskconfig
-drwxrwxrwx   0        0        0        0 2023-06-14 00:11:01.670223 srsinst.rga-0.3.2/srsinst/rga/tasks/
--rw-rw-rw-   0        0        0        0 2023-05-19 21:11:26.000000 srsinst.rga-0.3.2/srsinst/rga/tasks/__init__.py
--rw-rw-rw-   0        0        0     4001 2023-05-31 18:21:03.000000 srsinst.rga-0.3.2/srsinst/rga/tasks/analogscantask.py
--rw-rw-rw-   0        0        0     2543 2023-05-19 21:13:35.000000 srsinst.rga-0.3.2/srsinst/rga/tasks/cemcontroltask.py
--rw-rw-rw-   0        0        0     9379 2023-06-02 18:26:25.000000 srsinst.rga-0.3.2/srsinst/rga/tasks/cemgaintask.py
--rw-rw-rw-   0        0        0     9586 2023-05-19 21:13:35.000000 srsinst.rga-0.3.2/srsinst/rga/tasks/compositionanalysistask.py
--rw-rw-rw-   0        0        0     5243 2023-05-19 21:13:35.000000 srsinst.rga-0.3.2/srsinst/rga/tasks/derivedpvstscantask.py
--rw-rw-rw-   0        0        0     2751 2023-05-19 21:13:35.000000 srsinst.rga-0.3.2/srsinst/rga/tasks/filamentcontroltask.py
--rw-rw-rw-   0        0        0     3685 2023-05-19 21:13:35.000000 srsinst.rga-0.3.2/srsinst/rga/tasks/histogramscantask.py
--rw-rw-rw-   0        0        0    11440 2023-05-19 21:13:35.000000 srsinst.rga-0.3.2/srsinst/rga/tasks/peaktuningtask.py
--rw-rw-rw-   0        0        0     2557 2023-05-19 21:13:35.000000 srsinst.rga-0.3.2/srsinst/rga/tasks/pvstscantask.py
--rw-rw-rw-   0        0        0     2591 2023-06-06 22:11:10.000000 srsinst.rga-0.3.2/srsinst/rga/tasks/searchlan.py
-drwxrwxrwx   0        0        0        0 2023-06-14 00:11:01.650220 srsinst.rga-0.3.2/srsinst.rga.egg-info/
--rw-rw-rw-   0        0        0     6841 2023-06-14 00:11:01.000000 srsinst.rga-0.3.2/srsinst.rga.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1890 2023-06-14 00:11:01.000000 srsinst.rga-0.3.2/srsinst.rga.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 00:11:01.000000 srsinst.rga-0.3.2/srsinst.rga.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-14 00:11:01.000000 srsinst.rga-0.3.2/srsinst.rga.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      132 2023-06-14 00:11:01.000000 srsinst.rga-0.3.2/srsinst.rga.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-14 00:11:01.000000 srsinst.rga-0.3.2/srsinst.rga.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 20:09:00.852535 srsinst.rga-0.3.3/
+-rw-rw-rw-   0        0        0     1113 2023-05-16 22:11:28.000000 srsinst.rga-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0     6841 2023-06-14 20:09:00.852535 srsinst.rga-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5838 2023-06-14 00:09:13.000000 srsinst.rga-0.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 20:09:00.794016 srsinst.rga-0.3.3/docs/
+-rw-rw-rw-   0        0        0      654 2023-05-19 21:28:01.000000 srsinst.rga-0.3.3/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-06-14 20:09:00.756685 srsinst.rga-0.3.3/docs/_static/
+drwxrwxrwx   0        0        0        0 2023-06-14 20:09:00.804015 srsinst.rga-0.3.3/docs/_static/image/
+-rw-rw-rw-   0        0        0   174977 2023-06-09 18:18:12.000000 srsinst.rga-0.3.3/docs/_static/image/comp-analysis-screenshot.png
+-rw-rw-rw-   0        0        0   115947 2023-05-19 17:56:22.000000 srsinst.rga-0.3.3/docs/_static/image/derived-pvst-plot-screenshot.png
+-rw-rw-rw-   0        0        0    51322 2023-06-09 22:02:41.000000 srsinst.rga-0.3.3/docs/_static/image/initial-screen-capture.png
+-rw-rw-rw-   0        0        0    27661 2023-05-25 23:24:03.000000 srsinst.rga-0.3.3/docs/_static/image/simple-analog-scan-screenshot.png
+-rw-rw-rw-   0        0        0     1970 2023-06-13 20:55:52.000000 srsinst.rga-0.3.3/docs/conf.py
+-rw-rw-rw-   0        0        0      356 2023-06-01 23:58:11.000000 srsinst.rga-0.3.3/docs/custom_tasks.rst
+-rw-rw-rw-   0        0        0     6252 2023-06-12 22:33:57.000000 srsinst.rga-0.3.3/docs/gui_application.rst
+-rw-rw-rw-   0        0        0     2584 2023-06-12 23:28:46.000000 srsinst.rga-0.3.3/docs/index.rst
+-rw-rw-rw-   0        0        0     4199 2023-06-12 17:15:20.000000 srsinst.rga-0.3.3/docs/installation.rst
+-rw-rw-rw-   0        0        0    16282 2023-06-12 20:44:51.000000 srsinst.rga-0.3.3/docs/instrument_driver.rst
+-rwxrwxrwx   0        0        0      802 2023-05-19 21:28:01.000000 srsinst.rga-0.3.3/docs/make.bat
+-rw-rw-rw-   0        0        0       32 2023-05-19 21:28:01.000000 srsinst.rga-0.3.3/docs/requirements.txt
+-rw-rw-rw-   0        0        0     1332 2023-05-31 23:18:38.000000 srsinst.rga-0.3.3/docs/srsinst.rga.instruments.rga100.rst
+-rw-rw-rw-   0        0        0      358 2023-05-19 21:28:01.000000 srsinst.rga-0.3.3/docs/srsinst.rga.instruments.rst
+-rw-rw-rw-   0        0        0     1049 2023-06-09 19:15:10.000000 srsinst.rga-0.3.3/docs/srsinst.rga.plots.rst
+-rw-rw-rw-   0        0        0      148 2023-05-31 23:17:11.000000 srsinst.rga-0.3.3/docs/srsinst.rga.rst
+-rw-rw-rw-   0        0        0     2098 2023-06-14 18:25:03.000000 srsinst.rga-0.3.3/docs/srsinst.rga.tasks.rst
+-rw-rw-rw-   0        0        0     1471 2023-06-14 20:02:52.000000 srsinst.rga-0.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-14 20:09:00.852535 srsinst.rga-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsinst.rga-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 20:09:00.756685 srsinst.rga-0.3.3/srsinst/
+drwxrwxrwx   0        0        0        0 2023-06-14 20:09:00.814047 srsinst.rga-0.3.3/srsinst/rga/
+-rw-rw-rw-   0        0        0      349 2023-06-14 20:05:00.000000 srsinst.rga-0.3.3/srsinst/rga/__init__.py
+-rw-rw-rw-   0        0        0      483 2023-05-19 21:11:26.000000 srsinst.rga-0.3.3/srsinst/rga/__main__.py
+-rw-rw-rw-   0        0        0    10675 2023-06-01 21:25:29.000000 srsinst.rga-0.3.3/srsinst/rga/gaslib.dat
+drwxrwxrwx   0        0        0        0 2023-06-14 20:09:00.814047 srsinst.rga-0.3.3/srsinst/rga/instruments/
+-rw-rw-rw-   0        0        0       38 2023-06-14 18:20:37.000000 srsinst.rga-0.3.3/srsinst/rga/instruments/__init__.py
+-rw-rw-rw-   0        0        0      872 2023-05-19 21:13:35.000000 srsinst.rga-0.3.3/srsinst/rga/instruments/get_instruments.py
+drwxrwxrwx   0        0        0        0 2023-06-14 20:09:00.824015 srsinst.rga-0.3.3/srsinst/rga/instruments/rga100/
+-rw-rw-rw-   0        0        0        0 2023-05-19 21:11:26.000000 srsinst.rga-0.3.3/srsinst/rga/instruments/rga100/__init__.py
+-rw-rw-rw-   0        0        0     5249 2023-05-19 21:13:35.000000 srsinst.rga-0.3.3/srsinst/rga/instruments/rga100/commands.py
+-rw-rw-rw-   0        0        0     7355 2023-05-25 20:26:25.000000 srsinst.rga-0.3.3/srsinst/rga/instruments/rga100/components.py
+-rw-rw-rw-   0        0        0     4510 2023-05-19 21:13:35.000000 srsinst.rga-0.3.3/srsinst/rga/instruments/rga100/errors.py
+-rw-rw-rw-   0        0        0     8719 2023-06-13 23:56:14.000000 srsinst.rga-0.3.3/srsinst/rga/instruments/rga100/rga.py
+-rw-rw-rw-   0        0        0    18656 2023-05-19 21:11:26.000000 srsinst.rga-0.3.3/srsinst/rga/instruments/rga100/rga_commands.json
+-rw-rw-rw-   0        0        0    11740 2023-05-31 21:39:25.000000 srsinst.rga-0.3.3/srsinst/rga/instruments/rga100/scans.py
+-rw-rw-rw-   0        0        0     9870 2023-06-06 21:51:12.000000 srsinst.rga-0.3.3/srsinst/rga/instruments/rga100/sicp.py
+drwxrwxrwx   0        0        0        0 2023-06-14 20:09:00.832502 srsinst.rga-0.3.3/srsinst/rga/plots/
+-rw-rw-rw-   0        0        0        0 2023-05-19 21:11:26.000000 srsinst.rga-0.3.3/srsinst/rga/plots/__init__.py
+-rw-rw-rw-   0        0        0     4122 2023-06-09 19:33:09.000000 srsinst.rga-0.3.3/srsinst/rga/plots/analogscanplot.py
+-rw-rw-rw-   0        0        0     3448 2023-06-09 18:23:15.000000 srsinst.rga-0.3.3/srsinst/rga/plots/analysis.py
+-rw-rw-rw-   0        0        0     3287 2023-06-09 19:32:57.000000 srsinst.rga-0.3.3/srsinst/rga/plots/basescanplot.py
+-rw-rw-rw-   0        0        0     3792 2023-06-09 19:32:57.000000 srsinst.rga-0.3.3/srsinst/rga/plots/histogramscanplot.py
+-rw-rw-rw-   0        0        0     9182 2023-06-09 19:33:28.000000 srsinst.rga-0.3.3/srsinst/rga/plots/timeplot.py
+-rw-rw-rw-   0        0        0     2226 2023-06-01 00:10:48.000000 srsinst.rga-0.3.3/srsinst/rga/rga.taskconfig
+drwxrwxrwx   0        0        0        0 2023-06-14 20:09:00.842505 srsinst.rga-0.3.3/srsinst/rga/tasks/
+-rw-rw-rw-   0        0        0        0 2023-05-19 21:11:26.000000 srsinst.rga-0.3.3/srsinst/rga/tasks/__init__.py
+-rw-rw-rw-   0        0        0     4001 2023-05-31 18:21:03.000000 srsinst.rga-0.3.3/srsinst/rga/tasks/analogscantask.py
+-rw-rw-rw-   0        0        0     2543 2023-05-19 21:13:35.000000 srsinst.rga-0.3.3/srsinst/rga/tasks/cemcontroltask.py
+-rw-rw-rw-   0        0        0     9379 2023-06-02 18:26:25.000000 srsinst.rga-0.3.3/srsinst/rga/tasks/cemgaintask.py
+-rw-rw-rw-   0        0        0     9586 2023-05-19 21:13:35.000000 srsinst.rga-0.3.3/srsinst/rga/tasks/compositionanalysistask.py
+-rw-rw-rw-   0        0        0     5243 2023-05-19 21:13:35.000000 srsinst.rga-0.3.3/srsinst/rga/tasks/derivedpvstscantask.py
+-rw-rw-rw-   0        0        0     2751 2023-05-19 21:13:35.000000 srsinst.rga-0.3.3/srsinst/rga/tasks/filamentcontroltask.py
+-rw-rw-rw-   0        0        0     3685 2023-05-19 21:13:35.000000 srsinst.rga-0.3.3/srsinst/rga/tasks/histogramscantask.py
+-rw-rw-rw-   0        0        0    11440 2023-05-19 21:13:35.000000 srsinst.rga-0.3.3/srsinst/rga/tasks/peaktuningtask.py
+-rw-rw-rw-   0        0        0     2557 2023-05-19 21:13:35.000000 srsinst.rga-0.3.3/srsinst/rga/tasks/pvstscantask.py
+-rw-rw-rw-   0        0        0     2591 2023-06-06 22:11:10.000000 srsinst.rga-0.3.3/srsinst/rga/tasks/searchlan.py
+drwxrwxrwx   0        0        0        0 2023-06-14 20:09:00.804015 srsinst.rga-0.3.3/srsinst.rga.egg-info/
+-rw-rw-rw-   0        0        0     6841 2023-06-14 20:09:00.000000 srsinst.rga-0.3.3/srsinst.rga.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1890 2023-06-14 20:09:00.000000 srsinst.rga-0.3.3/srsinst.rga.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 20:09:00.000000 srsinst.rga-0.3.3/srsinst.rga.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-14 20:09:00.000000 srsinst.rga-0.3.3/srsinst.rga.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      117 2023-06-14 20:09:00.000000 srsinst.rga-0.3.3/srsinst.rga.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-14 20:09:00.000000 srsinst.rga-0.3.3/srsinst.rga.egg-info/top_level.txt
```

### Comparing `srsinst.rga-0.3.2/LICENSE` & `srsinst.rga-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/PKG-INFO` & `srsinst.rga-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsinst.rga
-Version: 0.3.2
+Version: 0.3.3
 Summary: Instrument driver package for Residual Gas Analyzers (RGA) from Stanford Research Systems
 Author: Chulhoon Kim
 License: MIT license
 Project-URL: homepage, https://github.com/thinkSRS/srsinst.rga
 Project-URL: repository, https://github.com/thinkSRS/srsinst.rga.git
 Project-URL: documentation, https://thinksrs.github.io/srsinst.rga
 Keywords: RGA,residual gas analyzer,SRS,Stanford Research Systems
```

### Comparing `srsinst.rga-0.3.2/README.md` & `srsinst.rga-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/docs/Makefile` & `srsinst.rga-0.3.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/docs/_static/image/comp-analysis-screenshot.png` & `srsinst.rga-0.3.3/docs/_static/image/comp-analysis-screenshot.png`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/docs/_static/image/derived-pvst-plot-screenshot.png` & `srsinst.rga-0.3.3/docs/_static/image/derived-pvst-plot-screenshot.png`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/docs/_static/image/initial-screen-capture.png` & `srsinst.rga-0.3.3/docs/_static/image/initial-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/docs/_static/image/simple-analog-scan-screenshot.png` & `srsinst.rga-0.3.3/docs/_static/image/simple-analog-scan-screenshot.png`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/docs/conf.py` & `srsinst.rga-0.3.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/docs/gui_application.rst` & `srsinst.rga-0.3.3/docs/gui_application.rst`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/docs/index.rst` & `srsinst.rga-0.3.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/docs/installation.rst` & `srsinst.rga-0.3.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/docs/instrument_driver.rst` & `srsinst.rga-0.3.3/docs/instrument_driver.rst`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/docs/make.bat` & `srsinst.rga-0.3.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/docs/srsinst.rga.instruments.rga100.rst` & `srsinst.rga-0.3.3/docs/srsinst.rga.instruments.rga100.rst`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/docs/srsinst.rga.plots.rst` & `srsinst.rga-0.3.3/docs/srsinst.rga.plots.rst`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/docs/srsinst.rga.tasks.rst` & `srsinst.rga-0.3.3/docs/srsinst.rga.tasks.rst`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
    :no-inherited-members:
 
 srsinst.rga.tasks.filamentcontroltask module
 --------------------------------------------
 
 .. automodule:: srsinst.rga.tasks.filamentcontroltask
    :members:
-   :undoc-members:
+   :no-undoc-members:
    :show-inheritance:
    :no-inherited-members:
 
 srsinst.rga.tasks.analogscantask module
 ---------------------------------------
 
 .. automodule:: srsinst.rga.tasks.analogscantask
```

### Comparing `srsinst.rga-0.3.2/pyproject.toml` & `srsinst.rga-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 ]
 dynamic = ["version"]
 
 [tool.setuptools.dynamic]
 version = {attr = "srsinst.rga.__version__"}
 
 [project.optional-dependencies]
-full = ['matplotlib >= 3.6.2', 'pyside6 <=6.4.3, >=6.5.1']
+full = ['matplotlib >= 3.6.2', 'pyside6']
 docs = ['matplotlib', 'pyside6', 'sphinx>=5', 'sphinx-rtd-theme>=1']
 # For Dependency specification, Refer to PEP 631
 
 [project.urls]
 homepage = "https://github.com/thinkSRS/srsinst.rga"
 repository = "https://github.com/thinkSRS/srsinst.rga.git"
 documentation = "https://thinksrs.github.io/srsinst.rga"
```

### Comparing `srsinst.rga-0.3.2/srsinst/rga/gaslib.dat` & `srsinst.rga-0.3.3/srsinst/rga/gaslib.dat`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/srsinst/rga/instruments/get_instruments.py` & `srsinst.rga-0.3.3/srsinst/rga/instruments/get_instruments.py`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/srsinst/rga/instruments/rga100/commands.py` & `srsinst.rga-0.3.3/srsinst/rga/instruments/rga100/commands.py`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/srsinst/rga/instruments/rga100/components.py` & `srsinst.rga-0.3.3/srsinst/rga/instruments/rga100/components.py`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/srsinst/rga/instruments/rga100/errors.py` & `srsinst.rga-0.3.3/srsinst/rga/instruments/rga100/errors.py`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/srsinst/rga/instruments/rga100/rga.py` & `srsinst.rga-0.3.3/srsinst/rga/instruments/rga100/rga.py`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/srsinst/rga/instruments/rga100/rga_commands.json` & `srsinst.rga-0.3.3/srsinst/rga/instruments/rga100/rga_commands.json`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/srsinst/rga/instruments/rga100/scans.py` & `srsinst.rga-0.3.3/srsinst/rga/instruments/rga100/scans.py`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/srsinst/rga/instruments/rga100/sicp.py` & `srsinst.rga-0.3.3/srsinst/rga/instruments/rga100/sicp.py`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/srsinst/rga/plots/analogscanplot.py` & `srsinst.rga-0.3.3/srsinst/rga/plots/analogscanplot.py`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/srsinst/rga/plots/analysis.py` & `srsinst.rga-0.3.3/srsinst/rga/plots/analysis.py`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/srsinst/rga/plots/basescanplot.py` & `srsinst.rga-0.3.3/srsinst/rga/plots/basescanplot.py`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/srsinst/rga/plots/histogramscanplot.py` & `srsinst.rga-0.3.3/srsinst/rga/plots/histogramscanplot.py`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/srsinst/rga/plots/timeplot.py` & `srsinst.rga-0.3.3/srsinst/rga/plots/timeplot.py`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/srsinst/rga/rga.taskconfig` & `srsinst.rga-0.3.3/srsinst/rga/rga.taskconfig`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/srsinst/rga/tasks/analogscantask.py` & `srsinst.rga-0.3.3/srsinst/rga/tasks/analogscantask.py`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/srsinst/rga/tasks/cemcontroltask.py` & `srsinst.rga-0.3.3/srsinst/rga/tasks/cemcontroltask.py`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/srsinst/rga/tasks/cemgaintask.py` & `srsinst.rga-0.3.3/srsinst/rga/tasks/cemgaintask.py`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/srsinst/rga/tasks/compositionanalysistask.py` & `srsinst.rga-0.3.3/srsinst/rga/tasks/compositionanalysistask.py`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/srsinst/rga/tasks/derivedpvstscantask.py` & `srsinst.rga-0.3.3/srsinst/rga/tasks/derivedpvstscantask.py`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/srsinst/rga/tasks/filamentcontroltask.py` & `srsinst.rga-0.3.3/srsinst/rga/tasks/filamentcontroltask.py`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/srsinst/rga/tasks/histogramscantask.py` & `srsinst.rga-0.3.3/srsinst/rga/tasks/histogramscantask.py`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/srsinst/rga/tasks/peaktuningtask.py` & `srsinst.rga-0.3.3/srsinst/rga/tasks/peaktuningtask.py`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/srsinst/rga/tasks/pvstscantask.py` & `srsinst.rga-0.3.3/srsinst/rga/tasks/pvstscantask.py`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/srsinst/rga/tasks/searchlan.py` & `srsinst.rga-0.3.3/srsinst/rga/tasks/searchlan.py`

 * *Files identical despite different names*

### Comparing `srsinst.rga-0.3.2/srsinst.rga.egg-info/PKG-INFO` & `srsinst.rga-0.3.3/srsinst.rga.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsinst.rga
-Version: 0.3.2
+Version: 0.3.3
 Summary: Instrument driver package for Residual Gas Analyzers (RGA) from Stanford Research Systems
 Author: Chulhoon Kim
 License: MIT license
 Project-URL: homepage, https://github.com/thinkSRS/srsinst.rga
 Project-URL: repository, https://github.com/thinkSRS/srsinst.rga.git
 Project-URL: documentation, https://thinksrs.github.io/srsinst.rga
 Keywords: RGA,residual gas analyzer,SRS,Stanford Research Systems
```

### Comparing `srsinst.rga-0.3.2/srsinst.rga.egg-info/SOURCES.txt` & `srsinst.rga-0.3.3/srsinst.rga.egg-info/SOURCES.txt`

 * *Files identical despite different names*

