# Comparing `tmp/solox-2.6.4.tar.gz` & `tmp/solox-2.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/SoloX/SoloX/dist/.tmp-mq4e96qp/solox-2.6.4.tar", last modified: Mon May 29 08:34:00 2023, max compression
+gzip compressed data, was "/home/runner/work/SoloX/SoloX/dist/.tmp-mpi62pce/solox-2.6.5.tar", last modified: Wed Jun 14 02:48:32 2023, max compression
```

## Comparing `solox-2.6.4.tar` & `solox-2.6.5.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-29 08:33:51.000000 solox-2.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-29 08:33:51.000000 solox-2.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-05-29 08:34:00.000000 solox-2.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-05-29 08:33:51.000000 solox-2.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-29 08:34:00.000000 solox-2.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-29 08:33:51.000000 solox-2.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/solox/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-29 08:33:51.000000 solox-2.6.4/solox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-29 08:33:51.000000 solox-2.6.4/solox/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-05-29 08:33:51.000000 solox-2.6.4/solox/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/solox/public/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12374 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/_iosPerf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/solox/public/adb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/solox/public/adb/linux/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/adb/linux/adb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/solox/public/adb/linux_arm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/adb/linux_arm/adb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/solox/public/adb/mac/
--rwxr-xr-x   0 runner    (1001) docker     (123)  7328624 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/adb/mac/adb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/solox/public/adb/windows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/adb/windows/AdbWinApi.dll
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/adb/windows/AdbWinUsbApi.dll
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/adb/windows/adb.exe
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/adb.py
--rw-r--r--   0 runner    (1001) docker     (123)    22010 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/apm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/apm_pk.py
--rw-r--r--   0 runner    (1001) docker     (123)    31724 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    20468 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/fps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/solox/public/iosperf/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30884 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_crash.py
--rw-r--r--   0 runner    (1001) docker     (123)    41300 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_hexdump.py
--rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_imagemounter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_installation.py
--rw-r--r--   0 runner    (1001) docker     (123)    39237 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_ipautil.py
--rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_perf.py
--rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_proto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_relay.py
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_safe_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_usbmux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/_wdaproxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    18789 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/bplist.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    31289 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/plistlib2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/requests_usbmux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/iosperf/struct2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/solox/public/report_template/
--rw-r--r--   0 runner    (1001) docker     (123)    29240 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/report_template/android.html
--rw-r--r--   0 runner    (1001) docker     (123)    29276 2023-05-29 08:33:51.000000 solox-2.6.4/solox/public/report_template/ios.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/solox/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/solox/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/css/highlight.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    28641 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/css/select2-bootstrap-5-theme.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    28632 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/css/select2-bootstrap-5-theme.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/css/select2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    24260 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/css/sweetalert2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/css/tabler.demo.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   297299 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/css/tabler.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/solox/static/image/
--rw-r--r--   0 runner    (1001) docker     (123)   144017 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/image/404.png
--rw-r--r--   0 runner    (1001) docker     (123)    47566 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/image/500.png
--rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/image/avatar.png
--rw-r--r--   0 runner    (1001) docker     (123)   136870 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/image/coffee.png
--rw-r--r--   0 runner    (1001) docker     (123)   219538 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/image/empty.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/solox/static/image/readme/
--rw-r--r--   0 runner    (1001) docker     (123)   796212 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/image/readme/home.png
--rw-r--r--   0 runner    (1001) docker     (123)   699302 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/image/readme/pk.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/solox/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   493603 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/js/apexcharts.js
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/js/gray.js
--rw-r--r--   0 runner    (1001) docker     (123)   117604 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/js/highlight.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   406552 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/js/highstock.js
--rw-r--r--   0 runner    (1001) docker     (123)   198689 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/js/html2canvas.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    73170 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/js/select2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   173966 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/js/socket.io.js
--rw-r--r--   0 runner    (1001) docker     (123)    43109 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/js/sweetalert2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/js/tabler.demo.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   143123 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/js/tabler.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/solox/static/logo/
--rw-r--r--   0 runner    (1001) docker     (123)    23002 2023-05-29 08:33:51.000000 solox-2.6.4/solox/static/logo/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/solox/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-05-29 08:33:51.000000 solox-2.6.4/solox/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-05-29 08:33:51.000000 solox-2.6.4/solox/templates/500.html
--rw-r--r--   0 runner    (1001) docker     (123)    65740 2023-05-29 08:33:51.000000 solox-2.6.4/solox/templates/analysis.html
--rw-r--r--   0 runner    (1001) docker     (123)    43308 2023-05-29 08:33:51.000000 solox-2.6.4/solox/templates/analysis_compare.html
--rw-r--r--   0 runner    (1001) docker     (123)    38287 2023-05-29 08:33:51.000000 solox-2.6.4/solox/templates/analysis_pk.html
--rw-r--r--   0 runner    (1001) docker     (123)    33714 2023-05-29 08:33:51.000000 solox-2.6.4/solox/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)   101171 2023-05-29 08:33:51.000000 solox-2.6.4/solox/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    55676 2023-05-29 08:33:51.000000 solox-2.6.4/solox/templates/pk.html
--rw-r--r--   0 runner    (1001) docker     (123)    34893 2023-05-29 08:33:51.000000 solox-2.6.4/solox/templates/report.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/solox/view/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-29 08:33:51.000000 solox-2.6.4/solox/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30353 2023-05-29 08:33:51.000000 solox-2.6.4/solox/view/apis.py
--rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-05-29 08:33:51.000000 solox-2.6.4/solox/view/pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-29 08:33:51.000000 solox-2.6.4/solox/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:34:00.000000 solox-2.6.4/solox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-05-29 08:34:00.000000 solox-2.6.4/solox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-29 08:34:00.000000 solox-2.6.4/solox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 08:34:00.000000 solox-2.6.4/solox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-29 08:34:00.000000 solox-2.6.4/solox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-29 08:34:00.000000 solox-2.6.4/solox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:48:32.000000 solox-2.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-14 02:48:22.000000 solox-2.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-14 02:48:22.000000 solox-2.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-06-14 02:48:32.000000 solox-2.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-06-14 02:48:22.000000 solox-2.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-14 02:48:32.000000 solox-2.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-14 02:48:22.000000 solox-2.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:48:32.000000 solox-2.6.5/solox/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-14 02:48:22.000000 solox-2.6.5/solox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-14 02:48:22.000000 solox-2.6.5/solox/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-06-14 02:48:22.000000 solox-2.6.5/solox/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:48:32.000000 solox-2.6.5/solox/public/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12374 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/_iosPerf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:48:32.000000 solox-2.6.5/solox/public/adb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:48:32.000000 solox-2.6.5/solox/public/adb/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/adb/linux/adb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:48:32.000000 solox-2.6.5/solox/public/adb/linux_arm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/adb/linux_arm/adb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:48:32.000000 solox-2.6.5/solox/public/adb/mac/
+-rwxr-xr-x   0 runner    (1001) docker     (123)  7328624 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/adb/mac/adb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:48:32.000000 solox-2.6.5/solox/public/adb/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/adb/windows/AdbWinApi.dll
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/adb/windows/AdbWinUsbApi.dll
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/adb/windows/adb.exe
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/adb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21834 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/apm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/apm_pk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32904 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20987 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/fps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:48:32.000000 solox-2.6.5/solox/public/iosperf/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/iosperf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30884 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/iosperf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/iosperf/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/iosperf/_crash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41300 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/iosperf/_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/iosperf/_hexdump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/iosperf/_imagemounter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/iosperf/_installation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39237 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/iosperf/_instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/iosperf/_ipautil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/iosperf/_perf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/iosperf/_proto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/iosperf/_relay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/iosperf/_safe_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/iosperf/_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/iosperf/_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/iosperf/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/iosperf/_usbmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/iosperf/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/iosperf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/iosperf/_wdaproxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18789 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/iosperf/bplist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/iosperf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31289 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/iosperf/plistlib2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/iosperf/requests_usbmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/iosperf/struct2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:48:32.000000 solox-2.6.5/solox/public/report_template/
+-rw-r--r--   0 runner    (1001) docker     (123)    29240 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/report_template/android.html
+-rw-r--r--   0 runner    (1001) docker     (123)    29276 2023-06-14 02:48:22.000000 solox-2.6.5/solox/public/report_template/ios.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:48:32.000000 solox-2.6.5/solox/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:48:32.000000 solox-2.6.5/solox/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-14 02:48:22.000000 solox-2.6.5/solox/static/css/highlight.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    28641 2023-06-14 02:48:22.000000 solox-2.6.5/solox/static/css/select2-bootstrap-5-theme.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    28632 2023-06-14 02:48:22.000000 solox-2.6.5/solox/static/css/select2-bootstrap-5-theme.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-06-14 02:48:22.000000 solox-2.6.5/solox/static/css/select2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    24260 2023-06-14 02:48:22.000000 solox-2.6.5/solox/static/css/sweetalert2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-06-14 02:48:22.000000 solox-2.6.5/solox/static/css/tabler.demo.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   297299 2023-06-14 02:48:22.000000 solox-2.6.5/solox/static/css/tabler.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:48:32.000000 solox-2.6.5/solox/static/image/
+-rw-r--r--   0 runner    (1001) docker     (123)   144017 2023-06-14 02:48:22.000000 solox-2.6.5/solox/static/image/404.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47566 2023-06-14 02:48:22.000000 solox-2.6.5/solox/static/image/500.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-06-14 02:48:22.000000 solox-2.6.5/solox/static/image/avatar.png
+-rw-r--r--   0 runner    (1001) docker     (123)   136870 2023-06-14 02:48:22.000000 solox-2.6.5/solox/static/image/coffee.png
+-rw-r--r--   0 runner    (1001) docker     (123)   219538 2023-06-14 02:48:22.000000 solox-2.6.5/solox/static/image/empty.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:48:32.000000 solox-2.6.5/solox/static/image/readme/
+-rw-r--r--   0 runner    (1001) docker     (123)   796212 2023-06-14 02:48:22.000000 solox-2.6.5/solox/static/image/readme/home.png
+-rw-r--r--   0 runner    (1001) docker     (123)   699302 2023-06-14 02:48:22.000000 solox-2.6.5/solox/static/image/readme/pk.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:48:32.000000 solox-2.6.5/solox/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   493603 2023-06-14 02:48:22.000000 solox-2.6.5/solox/static/js/apexcharts.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-06-14 02:48:22.000000 solox-2.6.5/solox/static/js/gray.js
+-rw-r--r--   0 runner    (1001) docker     (123)   117604 2023-06-14 02:48:22.000000 solox-2.6.5/solox/static/js/highlight.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   406552 2023-06-14 02:48:22.000000 solox-2.6.5/solox/static/js/highstock.js
+-rw-r--r--   0 runner    (1001) docker     (123)   198689 2023-06-14 02:48:22.000000 solox-2.6.5/solox/static/js/html2canvas.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-06-14 02:48:22.000000 solox-2.6.5/solox/static/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    73170 2023-06-14 02:48:22.000000 solox-2.6.5/solox/static/js/select2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   173966 2023-06-14 02:48:22.000000 solox-2.6.5/solox/static/js/socket.io.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43109 2023-06-14 02:48:22.000000 solox-2.6.5/solox/static/js/sweetalert2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-14 02:48:22.000000 solox-2.6.5/solox/static/js/tabler.demo.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   143123 2023-06-14 02:48:22.000000 solox-2.6.5/solox/static/js/tabler.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:48:32.000000 solox-2.6.5/solox/static/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)    23002 2023-06-14 02:48:22.000000 solox-2.6.5/solox/static/logo/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:48:32.000000 solox-2.6.5/solox/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-06-14 02:48:22.000000 solox-2.6.5/solox/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-06-14 02:48:22.000000 solox-2.6.5/solox/templates/500.html
+-rw-r--r--   0 runner    (1001) docker     (123)    65911 2023-06-14 02:48:22.000000 solox-2.6.5/solox/templates/analysis.html
+-rw-r--r--   0 runner    (1001) docker     (123)    43308 2023-06-14 02:48:22.000000 solox-2.6.5/solox/templates/analysis_compare.html
+-rw-r--r--   0 runner    (1001) docker     (123)    38458 2023-06-14 02:48:22.000000 solox-2.6.5/solox/templates/analysis_pk.html
+-rw-r--r--   0 runner    (1001) docker     (123)    35262 2023-06-14 02:48:22.000000 solox-2.6.5/solox/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)   101321 2023-06-14 02:48:22.000000 solox-2.6.5/solox/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    55677 2023-06-14 02:48:22.000000 solox-2.6.5/solox/templates/pk.html
+-rw-r--r--   0 runner    (1001) docker     (123)    34893 2023-06-14 02:48:22.000000 solox-2.6.5/solox/templates/report.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:48:32.000000 solox-2.6.5/solox/view/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-14 02:48:22.000000 solox-2.6.5/solox/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30915 2023-06-14 02:48:22.000000 solox-2.6.5/solox/view/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-06-14 02:48:22.000000 solox-2.6.5/solox/view/pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-06-14 02:48:22.000000 solox-2.6.5/solox/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:48:32.000000 solox-2.6.5/solox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-06-14 02:48:32.000000 solox-2.6.5/solox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-14 02:48:32.000000 solox-2.6.5/solox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 02:48:32.000000 solox-2.6.5/solox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-14 02:48:32.000000 solox-2.6.5/solox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-14 02:48:32.000000 solox-2.6.5/solox.egg-info/top_level.txt
```

### Comparing `solox-2.6.4/LICENSE` & `solox-2.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/PKG-INFO` & `solox-2.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solox
-Version: 2.6.4
+Version: 2.6.5
 Summary: SoloX - Real-time collection tool for Android/iOS performance data.
 Home-page: https://github.com/smart-test-ti/SoloX
 Author: Rafa Chen
 Author-email: rafacheninc@gamil.com
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -49,15 +49,15 @@
 💡 If Windows users need to test ios, install and start Itunes. [**Documentation**](https://github.com/alibaba/taobao-iphone-device)
 
 ## 📥Installation
 
 ### default
 
 ```shell
-pip install -U solox  (pip install solox==2.6.2)
+pip install -U solox  (pip install solox==2.6.4)
 ```
 
 ### mirrors
 
 ```shell
 pip install -i  https://mirrors.ustc.edu.cn/pypi/web/simple -U solox
 ```
@@ -81,16 +81,14 @@
 ## 🏴󠁣󠁩󠁣󠁭󠁿Collect in python
 
 ```python
 
 from solox.public.apm import APM
 from solox.public.common import Devices
 
-# solox version >= 2.1.2
-
 d = Devices()
 pids = d.getPid(deviceId='ca6bd5a5', pkgName='com.bilibili.app.in') # for android
 
 apm = APM(pkgName='com.bilibili.app.in',platform='Android', deviceId='ca6bd5a5', 
           surfaceview=True, noLog=True, pid=None)
 # apm = APM(pkgName='com.bilibili.app.in', platform='iOS') only supports one device
 # surfaceview： False = gfxinfo (Developer - GPU rendering mode - adb shell dumpsys gfxinfo)
@@ -105,15 +103,15 @@
 gpu = apm.collectGpu() # % only supports ios
 
 # ************* Collect all performance parameter ************* #
 apm = APM(pkgName='com.bilibili.app.in',platform='Android', deviceId='ca6bd5a5', 
           surfaceview=True, noLog=False, pid=None, duration=20) # duration : second
 # apm = APM(pkgName='com.bilibili.app.in', platform='iOS',  noLog=False, duration=20)
 if __name__ == '__main__':
-     apm.collectAll()
+     apm.collectAll() # will generate HTML report
 ```
 
 ## 🏴󠁣󠁩󠁣󠁭󠁿Collect in API
 
 ### Start the service in the background
 
 ```
```

### Comparing `solox-2.6.4/README.md` & `solox-2.6.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 💡 If Windows users need to test ios, install and start Itunes. [**Documentation**](https://github.com/alibaba/taobao-iphone-device)
 
 ## 📥Installation
 
 ### default
 
 ```shell
-pip install -U solox  (pip install solox==2.6.2)
+pip install -U solox  (pip install solox==2.6.4)
 ```
 
 ### mirrors
 
 ```shell
 pip install -i  https://mirrors.ustc.edu.cn/pypi/web/simple -U solox
 ```
@@ -66,16 +66,14 @@
 ## 🏴󠁣󠁩󠁣󠁭󠁿Collect in python
 
 ```python
 
 from solox.public.apm import APM
 from solox.public.common import Devices
 
-# solox version >= 2.1.2
-
 d = Devices()
 pids = d.getPid(deviceId='ca6bd5a5', pkgName='com.bilibili.app.in') # for android
 
 apm = APM(pkgName='com.bilibili.app.in',platform='Android', deviceId='ca6bd5a5', 
           surfaceview=True, noLog=True, pid=None)
 # apm = APM(pkgName='com.bilibili.app.in', platform='iOS') only supports one device
 # surfaceview： False = gfxinfo (Developer - GPU rendering mode - adb shell dumpsys gfxinfo)
@@ -90,15 +88,15 @@
 gpu = apm.collectGpu() # % only supports ios
 
 # ************* Collect all performance parameter ************* #
 apm = APM(pkgName='com.bilibili.app.in',platform='Android', deviceId='ca6bd5a5', 
           surfaceview=True, noLog=False, pid=None, duration=20) # duration : second
 # apm = APM(pkgName='com.bilibili.app.in', platform='iOS',  noLog=False, duration=20)
 if __name__ == '__main__':
-     apm.collectAll()
+     apm.collectAll() # will generate HTML report
 ```
 
 ## 🏴󠁣󠁩󠁣󠁭󠁿Collect in API
 
 ### Start the service in the background
 
 ```
```

### Comparing `solox-2.6.4/setup.py` & `solox-2.6.5/setup.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/__main__.py` & `solox-2.6.5/solox/__main__.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/debug.py` & `solox-2.6.5/solox/debug.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,17 +41,17 @@
         if thread:
             thread = socketio.start_background_task(target=backgroundThread)
 
 
 def backgroundThread():
     global thread
     try:
-        logger.info('Initializing adb environment ...')
-        os.system('adb kill-server')
-        os.system('adb start-server')
+        # logger.info('Initializing adb environment ...')
+        # os.system('adb kill-server')
+        # os.system('adb start-server')
         current_time = time.strftime("%Y%m%d%H", time.localtime())
         logPath = os.path.join(os.getcwd(),'adblog',f'{current_time}.log')
         logcat = subprocess.Popen(f'adb logcat *:E > {logPath}', stdout=subprocess.PIPE,
                                   shell=True)
         
         with open(logPath, "r") as f:
             while thread:
@@ -145,15 +145,15 @@
     Listen and open the url after solox is started
     :param host:
     :param port:
     :return:
     """
     flag = True
     while flag:
-        logger.info('start solox server')
+        logger.info('Start solox server ...')
         flag = getServerStatus(host, port)
     webbrowser.open(f'http://{host}:{port}/?platform=Android&lan=en', new=2)
     logger.info(f'Running on http://{host}:{port}/?platform=Android&lan=en (Press CTRL+C to quit)')
 
 
 def startServer(host: str, port: int):
     """
```

### Comparing `solox-2.6.4/solox/public/_iosPerf.py` & `solox-2.6.5/solox/public/_iosPerf.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/public/adb/mac/adb` & `solox-2.6.5/solox/public/adb/mac/adb`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/public/adb.py` & `solox-2.6.5/solox/public/adb.py`

 * *Files 9% similar despite different names*

```diff
@@ -76,14 +76,19 @@
         self.adb_path = builtin_adb_path()
 
     def shell(self, cmd, deviceId):
         run_cmd = f'{self.adb_path} -s {deviceId} shell {cmd}'
         result = subprocess.Popen(run_cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE).communicate()[
             0].decode("utf-8").strip()
         return result
+    
+    def tcp_shell(self, cmd, deviceId):
+        run_cmd = f'{self.adb_path} -s {deviceId} shell {cmd}'
+        result = os.system(run_cmd)
+        return result
 
     def shell_noDevice(self, cmd):
         run_cmd = f'{self.adb_path} {cmd}'
         result = os.system(run_cmd)
         return result
```

### Comparing `solox-2.6.4/solox/public/apm.py` & `solox-2.6.5/solox/public/apm.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,27 +82,27 @@
         time.sleep(1)
         processCpuTime_2 = self.getprocessCpuStat()
         totalCpuTime_2 = self.getTotalCpuStat()
         sysCpuTime_2 = self.getSysCpuStat()
         appCpuRate = round(float((processCpuTime_2 - processCpuTime_1) / (totalCpuTime_2 - totalCpuTime_1) * 100), 2)
         sysCpuRate = round(float((sysCpuTime_2 - sysCpuTime_1) / (totalCpuTime_2 - totalCpuTime_1) * 100), 2)
         if noLog is False:
-            apm_time = datetime.datetime.now().strftime('%H:%M:%S')
+            apm_time = datetime.datetime.now().strftime('%H:%M:%S.%f')
             f.add_log(os.path.join(f.report_dir,'cpu_app.log'), apm_time, appCpuRate)
             f.add_log(os.path.join(f.report_dir,'cpu_sys.log'), apm_time, sysCpuRate)
 
         return appCpuRate, sysCpuRate
 
     def getiOSCpuRate(self, noLog=False):
         """get the iOS cpu rate of a process, unit:%"""
         apm = iosAPM(self.pkgName)
         appCpuRate = round(float(apm.getPerformance(apm.cpu)[0]), 2)
         sysCpuRate = round(float(apm.getPerformance(apm.cpu)[1]), 2)
         if noLog is False:
-            apm_time = datetime.datetime.now().strftime('%H:%M:%S')
+            apm_time = datetime.datetime.now().strftime('%H:%M:%S.%f')
             f.add_log(os.path.join(f.report_dir,'cpu_app.log'), apm_time, appCpuRate)
             f.add_log(os.path.join(f.report_dir,'cpu_sys.log'), apm_time, sysCpuRate)
         return appCpuRate, sysCpuRate
 
     def getCpuRate(self, noLog=False):
         """Get the cpu rate of a process, unit:%"""
         appCpuRate, systemCpuRate = self.getAndroidCpuRate(noLog) if self.platform == Platform.Android else self.getiOSCpuRate(noLog)
@@ -137,16 +137,15 @@
         dalvikPass = 0
         return totalPass, nativePass, dalvikPass
 
     def getProcessMem(self, noLog=False):
         """Get the app memory"""
         totalPass, nativePass, dalvikPass = self.getAndroidMem() if self.platform == Platform.Android else self.getiOSMem()
         if noLog is False:    
-            time.sleep(1)    
-            apm_time = datetime.datetime.now().strftime('%H:%M:%S')
+            apm_time = datetime.datetime.now().strftime('%H:%M:%S.%f')
             f.add_log(os.path.join(f.report_dir,'mem_total.log'), apm_time, totalPass)
             if self.platform == Platform.Android:
                 f.add_log(os.path.join(f.report_dir,'mem_native.log'), apm_time, nativePass)
                 f.add_log(os.path.join(f.report_dir,'mem_dalvik.log'), apm_time, dalvikPass)
         return totalPass, nativePass, dalvikPass
 
 class Battery(object):
@@ -169,31 +168,29 @@
         adb.shell(cmd=cmd, deviceId=self.deviceId)
         # Get phone battery info
         cmd = 'dumpsys battery'
         output = adb.shell(cmd=cmd, deviceId=self.deviceId)
         level = int(re.findall(u'level:\s?(\d+)', output)[0])
         temperature = int(re.findall(u'temperature:\s?(\d+)', output)[0]) / 10
         if noLog is False:
-             time.sleep(1)
-             apm_time = datetime.datetime.now().strftime('%H:%M:%S')
+             apm_time = datetime.datetime.now().strftime('%H:%M:%S.%f')
              f.add_log(os.path.join(f.report_dir,'battery_level.log'), apm_time, level)
              f.add_log(os.path.join(f.report_dir,'battery_tem.log'), apm_time, temperature)
         return level, temperature
     
     def getiOSBattery(self, noLog=False):
         """Get ios battery info, unit:%"""
         d  = tidevice.Device()
         ioDict =  d.get_io_power()
         tem = m._setValue(ioDict['Diagnostics']['IORegistry']['Temperature'])
         current = m._setValue(abs(ioDict['Diagnostics']['IORegistry']['InstantAmperage']))
         voltage = m._setValue(ioDict['Diagnostics']['IORegistry']['Voltage'])
         power = current * voltage / 1000
         if noLog is False:
-            time.sleep(1)
-            apm_time = datetime.datetime.now().strftime('%H:%M:%S')
+            apm_time = datetime.datetime.now().strftime('%H:%M:%S.%f')
             f.add_log(os.path.join(f.report_dir,'battery_tem.log'), apm_time, tem) # unknown
             f.add_log(os.path.join(f.report_dir,'battery_current.log'), apm_time, current) #mA
             f.add_log(os.path.join(f.report_dir,'battery_voltage.log'), apm_time, voltage) #mV
             f.add_log(os.path.join(f.report_dir,'battery_power.log'), apm_time, power)
         return tem, current, voltage, power
 
     def recoverBattery(self):
@@ -246,15 +243,15 @@
         recNum = round(float(apm_data[0]), 2)
         return sendNum, recNum
 
     def getNetWorkData(self, wifi=True, noLog=False):
         """Get the upflow and downflow data, unit:KB"""
         sendNum, recNum = self.getAndroidNet(wifi) if self.platform == Platform.Android else self.getiOSNet()
         if noLog is False:
-            apm_time = datetime.datetime.now().strftime('%H:%M:%S')
+            apm_time = datetime.datetime.now().strftime('%H:%M:%S.%f')
             f.add_log(os.path.join(f.report_dir,'upflow.log'), apm_time, sendNum)
             f.add_log(os.path.join(f.report_dir,'downflow.log'), apm_time, recNum)
         return sendNum, recNum
 
 class FPS(object):
 
     def __init__(self, pkgName, deviceId, platform=Platform.Android, surfaceview=True):
@@ -267,27 +264,25 @@
     def getAndroidFps(self, noLog=False):
         """get Android Fps, unit:HZ"""
         monitors = FPSMonitor(device_id=self.deviceId, package_name=self.pkgName, frequency=1,
                               surfaceview=self.surfaceview, start_time=TimeUtils.getCurrentTimeUnderline())
         monitors.start()
         fps, jank = monitors.stop()
         if noLog is False:
-            time.sleep(1)
-            apm_time = datetime.datetime.now().strftime('%H:%M:%S')
+            apm_time = datetime.datetime.now().strftime('%H:%M:%S.%f')
             f.add_log(os.path.join(f.report_dir,'fps.log'), apm_time, fps)
             f.add_log(os.path.join(f.report_dir,'jank.log'), apm_time, jank)
         return fps, jank
 
     def getiOSFps(self, noLog=False):
         """get iOS Fps"""
         apm = iosAPM(self.pkgName)
         fps = int(apm.getPerformance(apm.fps))
         if noLog is False:
-            time.sleep(1)
-            apm_time = datetime.datetime.now().strftime('%H:%M:%S')
+            apm_time = datetime.datetime.now().strftime('%H:%M:%S.%f')
             f.add_log(os.path.join(f.report_dir,'fps.log'), apm_time, fps)
         return fps, 0
 
     def getFPS(self, noLog=False):
         """get fps、jank"""
         fps, jank = self.getAndroidFps(noLog) if self.platform == Platform.Android else self.getiOSFps(noLog)
         return fps, jank
@@ -296,16 +291,15 @@
     def __init__(self, pkgName):
         self.pkgName = pkgName
 
     def getGPU(self, noLog=False):
         apm = iosAPM(self.pkgName)
         gpu = apm.getPerformance(apm.gpu)
         if noLog is False:
-            time.sleep(1)
-            apm_time = datetime.datetime.now().strftime('%H:%M:%S')
+            apm_time = datetime.datetime.now().strftime('%H:%M:%S.%f')
             f.add_log(os.path.join(f.report_dir,'gpu.log'), apm_time, gpu)
         return gpu   
 
 class iosAPM(object):
 
     def __init__(self, pkgName, deviceId=tidevice.Device()):
         self.pkgName = pkgName
@@ -367,16 +361,16 @@
                 break
         return result
 
     def collectMemory(self):
         _memory = MEM(self.pkgName, self.deviceId, self.platform, pid=self.pid)
         result = {}
         while True:
-            totalPass, nativePass, dalvikPass = _memory.getProcessMem(noLog=self.noLog)
-            result = {'totalPass': totalPass, 'nativePass': nativePass, 'dalvikPass': dalvikPass}
+            total, native, dalvik = _memory.getProcessMem(noLog=self.noLog)
+            result = {'total': total, 'native': native, 'dalvik': dalvik}
             logger.info(f'memory: {result}')
             if time.time() > self.end_time:
                 break
         return result
 
     def collectBattery(self):
         _battery = Battery(self.deviceId, self.platform)
@@ -396,15 +390,15 @@
         _flow = Flow(self.pkgName, self.deviceId, self.platform, pid=self.pid)
         if self.noLog is False:
             data = _flow.setAndroidNet(wifi=wifi)
             f.record_net('pre', data[0], data[1])
         result = {}
         while True:
             upFlow, downFlow = _flow.getNetWorkData(wifi=wifi,noLog=self.noLog)
-            result = {'upFlow': upFlow, 'downFlow': downFlow}
+            result = {'send': upFlow, 'recv': downFlow}
             logger.info(f'network: {result}')
             if time.time() > self.end_time:
                 break
         return result
 
     def collectFps(self):
         _fps = FPS(self.pkgName, self.deviceId, self.platform, self.surfaceview)
```

### Comparing `solox-2.6.4/solox/public/apm_pk.py` & `solox-2.6.5/solox/public/apm_pk.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             time.sleep(1)
             processCpuTime2_second = self.getprocessCpuStat(pkgName=self.pkgNameList[1], deviceId=self.deviceId2)
             totalCpuTime2_second = self.getTotalCpuStat(deviceId=self.deviceId2)
 
         appCpuRate1 = round(float((processCpuTime1_second - processCpuTime1_first) / (totalCpuTime1_second - totalCpuTime1_first) * 100), 2)
         appCpuRate2 = round(float((processCpuTime2_second - processCpuTime2_first) / (totalCpuTime2_second - totalCpuTime2_first) * 100), 2)
         
-        apm_time = datetime.datetime.now().strftime('%H:%M:%S')
+        apm_time = datetime.datetime.now().strftime('%H:%M:%S.%f')
         f.add_log(f'{f.report_dir}/cpu_app1.log', apm_time, appCpuRate1)
         f.add_log(f'{f.report_dir}/cpu_app2.log', apm_time, appCpuRate2)
 
 
         return appCpuRate1, appCpuRate2
 
 
@@ -100,15 +100,15 @@
         if len(self.pkgNameList) == 1:
             totalPass1 = self.getAndroidMem(self.pkgNameList[0], self.deviceId1)
             totalPass2 = self.getAndroidMem(self.pkgNameList[0], self.deviceId2)
         else:
             totalPass1 = self.getAndroidMem(self.pkgNameList[0], self.deviceId1)
             totalPass2 = self.getAndroidMem(self.pkgNameList[1], self.deviceId2)
         
-        apm_time = datetime.datetime.now().strftime('%H:%M:%S')
+        apm_time = datetime.datetime.now().strftime('%H:%M:%S.%f')
         f.add_log(f'{f.report_dir}/mem1.log', apm_time, totalPass1)
         f.add_log(f'{f.report_dir}/mem2.log', apm_time, totalPass2)
 
         return totalPass1, totalPass2
 
 
 class Flow_PK:
@@ -141,15 +141,15 @@
         if len(self.pkgNameList) == 1:
             network1 = self.getAndroidNet(self.pkgNameList[0], self.deviceId1)
             network2 = self.getAndroidNet(self.pkgNameList[0], self.deviceId2)
         else:
             network1 = self.getAndroidNet(self.pkgNameList[0], self.deviceId1)
             network2 = self.getAndroidNet(self.pkgNameList[1], self.deviceId2)
         
-        apm_time = datetime.datetime.now().strftime('%H:%M:%S')    
+        apm_time = datetime.datetime.now().strftime('%H:%M:%S.%f')    
         f.add_log(f'{f.report_dir}/network1.log', apm_time, network1)
         f.add_log(f'{f.report_dir}/network2.log', apm_time, network2)
         return network1, network2
 
 
 class FPS_PK:
 
@@ -174,14 +174,14 @@
             fps1 = self.getAndroidFps(pkgName=self.pkgNameList[0], deviceId=self.deviceId1)
             fps2 = self.getAndroidFps(pkgName=self.pkgNameList[0], deviceId=self.deviceId2)
 
         else:
             fps1 = self.getAndroidFps(pkgName=self.pkgNameList[0], deviceId=self.deviceId1)
             fps2 = self.getAndroidFps(pkgName=self.pkgNameList[1], deviceId=self.deviceId2)
         
-        apm_time = datetime.datetime.now().strftime('%H:%M:%S')
+        apm_time = datetime.datetime.now().strftime('%H:%M:%S.%f')
         f.add_log(f'{f.report_dir}/fps1.log', apm_time, fps1)
         f.add_log(f'{f.report_dir}/fps2.log', apm_time, fps2)
 
         return fps1, fps2
```

### Comparing `solox-2.6.4/solox/public/common.py` & `solox-2.6.5/solox/public/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import shutil
 import time
 import requests
 from logzero import logger
 from solox.public.adb import adb
 from tqdm import tqdm
 import traceback
+import socket
 from urllib.request import urlopen
 import ssl
 import xlwt
 from jinja2 import Environment, FileSystemLoader
  
 class Platform:
     Android = 'Android'
@@ -113,14 +114,33 @@
         return deviceInfo
 
     def getPkgnameByiOS(self, udid):
         """Get all package names of the corresponding iOS device"""
         pkgResult = self.execCmd(f'tidevice --udid {udid} applist').split('\n')
         pkgNames = [pkgResult[i].split(' ')[0] for i in range(len(pkgResult))]
         return pkgNames
+    
+    def localIP(self):
+        try:
+            s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+            s.connect(('8.8.8.8', 80))
+            ip = s.getsockname()[0]
+        except Exception:
+            logger.error('get local ip failed')
+            ip = '127.0.0.1'
+        finally:
+            s.close()
+        return ip
+    
+    def tcpConnect(self, deviceId, port):
+        logger.info('TCP mode port')
+        adb.tcp_shell(deviceId=deviceId, cmd='tcpip {}'.format(port))
+        logger.info('Connect result')
+        result = adb.tcp_shell(cmd='connect {}:{}'.format(self.localIP(), port))
+        return result
 
     def devicesCheck(self, platform, deviceid=None, pkgname=None):
         """Check the device environment"""
         match(platform):
             case Platform.Android:
                 if len(self.getDeviceIds()) == 0:
                     raise Exception('no devices found')
@@ -350,15 +370,14 @@
                     log_data_list.append({
                         "x": line.split('=')[0].strip(),
                         "y": float(line.split('=')[1].strip())
                     })
                     target_data_list.append(float(line.split('=')[1].strip()))
         return log_data_list, target_data_list
         
-    
     def getCpuLog(self, platform, scene):
         targetDic = {}
         targetDic['cpuAppData'] = self.readLog(scene=scene, filename='cpu_app.log')[0]
         targetDic['cpuSysData'] = self.readLog(scene=scene, filename='cpu_sys.log')[0]
         result = {'status': 1, 'cpuAppData': targetDic['cpuAppData'], 'cpuSysData': targetDic['cpuSysData']}
         return result
     
@@ -631,15 +650,14 @@
         apm_dict['totalPassAvg2'] = totalPassAvg2
         apm_dict['network1'] = network1
         apm_dict['network2'] = network2
         apm_dict['fpsAvg1'] = fpsAvg1
         apm_dict['fpsAvg2'] = fpsAvg2
         return apm_dict
 
-
 class Method:
     
     @classmethod
     def _request(cls, request, object):
         match(request.method):
             case 'POST':
                 return request.form[object]
@@ -701,7 +719,26 @@
     def installIPA(self, path):
         result = Devices.execCmd('tidevice install {}'.format(path))
         if result == 0:
             os.remove(path)
             return True, result
         else:
             return False, result
+
+# class Config:
+
+#     def __init__(self):
+#         self.configRoot = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'config')
+
+#     def get_devices(self):
+#         config_path = os.path.join(self.configRoot, 'devices.json')
+#         content = {}
+#         with open(config_path, "r", encoding="utf-8") as f:
+#             content = json.load(f)
+#         devices = content['content']    
+#         return devices
+
+#     def set_devices(self):
+#         pass
+
+#     def remove_device(self, deviceid):
+#         pass
```

### Comparing `solox-2.6.4/solox/public/fps.py` & `solox-2.6.5/solox/public/fps.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,27 +56,35 @@
             self.collector_thread = None
             if self.fps_queue:
                 self.fps_queue.task_done()
      
     def get_surfaceview_activity(self):
         activity_name = ''
         activity_line = ''
-        dumpsys_result = adb.shell(cmd='dumpsys SurfaceFlinger --list | {} {}'.format(d.filterType(), self.package_name), deviceId=self.device)
-        dumpsys_result_list = dumpsys_result.split('\n')    
-        for line in dumpsys_result_list:
-            if line.startswith('SurfaceView') and line.find(self.package_name) != -1:
-                activity_line = line.strip()
-                break
-        if activity_line:       
-            activity_name = activity_line.split(' ')[2]
-        else:
-            activity_name = dumpsys_result_list[len(dumpsys_result_list) - 1]
-            if not activity_name.__contains__(self.package_name):
-                logger.error('get activity name failed, Please provide SurfaceFlinger --list information to the author')
-                logger.info('dumpsys SurfaceFlinger --list info: {}'.format(dumpsys_result))
+        try:
+            dumpsys_result = adb.shell(cmd='dumpsys SurfaceFlinger --list | {} {}'.format(d.filterType(), self.package_name), deviceId=self.device)
+            dumpsys_result_list = dumpsys_result.split('\n')    
+            for line in dumpsys_result_list:
+                if line.startswith('SurfaceView') and line.find(self.package_name) != -1:
+                    activity_line = line.strip()
+                    break
+            if activity_line:
+                if activity_line.find(' ')  != -1:      
+                    activity_name = activity_line.split(' ')[2]
+                else:
+                    activity_name = activity_line.replace('SurfaceView','').replace('[','').replace(']','')    
+            else:
+                activity_name = dumpsys_result_list[len(dumpsys_result_list) - 1]
+                if not activity_name.__contains__(self.package_name):
+                    logger.error('get activity name failed, Please provide SurfaceFlinger --list information to the author')
+                    logger.info('dumpsys SurfaceFlinger --list info: {}'.format(dumpsys_result))
+        except Exception:
+            traceback.print_exc()
+            logger.error('get activity name failed, Please provide SurfaceFlinger --list information to the author')
+            logger.info('dumpsys SurfaceFlinger --list info: {}'.format(dumpsys_result))
         return activity_name
      
     def get_focus_activity(self):
         activity_name = ''
         activity_line = ''
         dumpsys_result = adb.shell(cmd='dumpsys window windows', deviceId=self.device)
         dumpsys_result_list = dumpsys_result.split('\n')
```

### Comparing `solox-2.6.4/solox/public/iosperf/__main__.py` & `solox-2.6.5/solox/public/iosperf/__main__.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/public/iosperf/_crash.py` & `solox-2.6.5/solox/public/iosperf/_crash.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/public/iosperf/_device.py` & `solox-2.6.5/solox/public/iosperf/_device.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/public/iosperf/_hexdump.py` & `solox-2.6.5/solox/public/iosperf/_hexdump.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/public/iosperf/_imagemounter.py` & `solox-2.6.5/solox/public/iosperf/_imagemounter.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/public/iosperf/_installation.py` & `solox-2.6.5/solox/public/iosperf/_installation.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/public/iosperf/_instruments.py` & `solox-2.6.5/solox/public/iosperf/_instruments.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/public/iosperf/_ipautil.py` & `solox-2.6.5/solox/public/iosperf/_ipautil.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/public/iosperf/_perf.py` & `solox-2.6.5/solox/public/iosperf/_perf.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/public/iosperf/_proto.py` & `solox-2.6.5/solox/public/iosperf/_proto.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/public/iosperf/_relay.py` & `solox-2.6.5/solox/public/iosperf/_relay.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/public/iosperf/_safe_socket.py` & `solox-2.6.5/solox/public/iosperf/_safe_socket.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/public/iosperf/_ssl.py` & `solox-2.6.5/solox/public/iosperf/_ssl.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/public/iosperf/_sync.py` & `solox-2.6.5/solox/public/iosperf/_sync.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/public/iosperf/_types.py` & `solox-2.6.5/solox/public/iosperf/_types.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/public/iosperf/_usbmux.py` & `solox-2.6.5/solox/public/iosperf/_usbmux.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/public/iosperf/_utils.py` & `solox-2.6.5/solox/public/iosperf/_utils.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/public/iosperf/_wdaproxy.py` & `solox-2.6.5/solox/public/iosperf/_wdaproxy.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/public/iosperf/bplist.py` & `solox-2.6.5/solox/public/iosperf/bplist.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/public/iosperf/exceptions.py` & `solox-2.6.5/solox/public/iosperf/exceptions.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/public/iosperf/plistlib2.py` & `solox-2.6.5/solox/public/iosperf/plistlib2.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/public/iosperf/requests_usbmux.py` & `solox-2.6.5/solox/public/iosperf/requests_usbmux.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/public/iosperf/struct2.py` & `solox-2.6.5/solox/public/iosperf/struct2.py`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/public/report_template/android.html` & `solox-2.6.5/solox/public/report_template/android.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/public/report_template/ios.html` & `solox-2.6.5/solox/public/report_template/ios.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/static/css/highlight.min.css` & `solox-2.6.5/solox/static/css/highlight.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/static/css/select2-bootstrap-5-theme.min.css` & `solox-2.6.5/solox/static/css/select2-bootstrap-5-theme.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/static/css/select2-bootstrap-5-theme.rtl.min.css` & `solox-2.6.5/solox/static/css/select2-bootstrap-5-theme.rtl.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/static/css/select2.min.css` & `solox-2.6.5/solox/static/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/static/css/sweetalert2.min.css` & `solox-2.6.5/solox/static/css/sweetalert2.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/static/css/tabler.demo.min.css` & `solox-2.6.5/solox/static/css/tabler.demo.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/static/css/tabler.min.css` & `solox-2.6.5/solox/static/css/tabler.min.css`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/static/image/404.png` & `solox-2.6.5/solox/static/image/404.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/static/image/500.png` & `solox-2.6.5/solox/static/image/500.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/static/image/avatar.png` & `solox-2.6.5/solox/static/image/avatar.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/static/image/coffee.png` & `solox-2.6.5/solox/static/image/coffee.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/static/image/empty.png` & `solox-2.6.5/solox/static/image/empty.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/static/image/readme/home.png` & `solox-2.6.5/solox/static/image/readme/home.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/static/image/readme/pk.png` & `solox-2.6.5/solox/static/image/readme/pk.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/static/js/apexcharts.js` & `solox-2.6.5/solox/static/js/apexcharts.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/static/js/gray.js` & `solox-2.6.5/solox/static/js/gray.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/static/js/highlight.min.js` & `solox-2.6.5/solox/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/static/js/highstock.js` & `solox-2.6.5/solox/static/js/highstock.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/static/js/html2canvas.min.js` & `solox-2.6.5/solox/static/js/html2canvas.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/static/js/jquery.min.js` & `solox-2.6.5/solox/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/static/js/select2.min.js` & `solox-2.6.5/solox/static/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/static/js/socket.io.js` & `solox-2.6.5/solox/static/js/socket.io.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/static/js/sweetalert2.min.js` & `solox-2.6.5/solox/static/js/sweetalert2.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/static/js/tabler.demo.min.js` & `solox-2.6.5/solox/static/js/tabler.demo.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/static/js/tabler.min.js` & `solox-2.6.5/solox/static/js/tabler.min.js`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/static/logo/logo.png` & `solox-2.6.5/solox/static/logo/logo.png`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/templates/404.html` & `solox-2.6.5/solox/templates/404.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/templates/500.html` & `solox-2.6.5/solox/templates/500.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/templates/analysis.html` & `solox-2.6.5/solox/templates/analysis.html`

 * *Files 0% similar despite different names*

```diff
@@ -702,14 +702,21 @@
             grid: {
                 padding: {
                     top: -20,
                     bottom: -4
                 },
             strokeDashArray: 4,
             },
+            xaxis: {
+                name: "time",
+                tickAmount:6,
+                labels: {
+                    rotate: 0,
+                }
+            },
         };
         return options
     }
 
     var cpu_chart = new ApexCharts(document.querySelector("#chart-cpu"), options('line'));
     cpu_chart.render();
     $('#cpu_loading').click(function () {
```

### Comparing `solox-2.6.4/solox/templates/analysis_compare.html` & `solox-2.6.5/solox/templates/analysis_compare.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/templates/analysis_pk.html` & `solox-2.6.5/solox/templates/analysis_pk.html`

 * *Files 0% similar despite different names*

```diff
@@ -497,14 +497,21 @@
             grid: {
                 padding: {
                     top: -20,
                     bottom: -4
                 },
             strokeDashArray: 4,
             },
+            xaxis: {
+                name: "time",
+                tickAmount:6,
+                labels: {
+                    rotate: 0,
+                }
+            },
         };
         return options
     }
 
     var cpu_chart = new ApexCharts(document.querySelector("#chart-cpu"), options('line'));
     cpu_chart.render();
     $('#cpu_loading').click(function () {
```

### Comparing `solox-2.6.4/solox/templates/base.html` & `solox-2.6.5/solox/templates/base.html`

 * *Files 4% similar despite different names*

```diff
@@ -126,15 +126,15 @@
                     <ul class="list-inline list-inline-dots mb-0">
                         <li class="list-inline-item">
                             Copyright &copy; <label id="curYear"></label>
                             <a href="https://github.com/smart-test-ti" class="link-secondary">SoloX</a>.{% if lan == 'cn' %} 保留所有权利 {% else %} All rights reserved {% endif %}
                         </li>
                         <li class="list-inline-item">
                             <a href="https://github.com/smart-test-ti/SoloX/releases" target="_blank" class="link-secondary" rel="noopener">
-                                {% if lan == 'cn' %} 版本 {% else %} Releases {% endif %} . V2.6.4
+                                {% if lan == 'cn' %} 版本 {% else %} Releases {% endif %} . V2.6.5
                             </a>
                         </li>
                     </ul>
                 </div>
             </div>
         </div>
     </footer>
@@ -146,33 +146,51 @@
             {% if lan == 'cn' %} 设置 {% else %} Setting {% endif %}
         </h2>
         <button type="button" class="btn-close text-reset" data-bs-dismiss="offcanvas" aria-label="Close"></button>
     </div>
     <div class="offcanvas-body">
         <div class="card-tabs">
             <ul class="nav nav-tabs">
-              <li class="nav-item"><a href="#tab-top-1" class="nav-link active" data-bs-toggle="tab">Warning Value</a></li>
-              <li class="nav-item"><a href="#tab-top-2" class="nav-link" data-bs-toggle="tab">Timer</a></li>
-              <li class="nav-item"><a href="#tab-top-3" class="nav-link" data-bs-toggle="tab">Agent &nbsp;
-                {% if lan == 'en' %}
-                <span class="form-help" data-bs-toggle="popover" data-bs-placement="top" data-bs-html="true" data-bs-content="
-                Start solox on the Slave machine first, and then configure the Host here.
-            </p>Note: The port number cannot be the same as the Master machine</p>
-            ">?</span>
-            {% else %}
-            <span class="form-help" data-bs-toggle="popover" data-bs-placement="top" data-bs-html="true" data-bs-content="
-            先在其他机器启动solox,然后将Host配置在这里
-            </p>注意：端口号不能和主机器一样</p>
-            ">?</span>
-            {% endif %}
-            </a></li>
+                <!-- https://adbshell.com/commands/adb-connect -->
+                <!-- <li class="nav-item"><a href="#tab-top-1" class="nav-link active" data-bs-toggle="tab">{% if lan == 'cn' %} 无线连接 {% else %} Wireless {% endif %}</a></li> -->
+                <li class="nav-item"><a href="#tab-top-2" class="nav-link" data-bs-toggle="tab">{% if lan == 'cn' %} 告警值 {% else %} Warning Value {% endif %}</a></li>
+                <li class="nav-item"><a href="#tab-top-3" class="nav-link" data-bs-toggle="tab">{% if lan == 'cn' %} 定时器 {% else %} Timer {% endif %}</a></li>
+                <li class="nav-item"><a href="#tab-top-4" class="nav-link" data-bs-toggle="tab">{% if lan == 'cn' %} 远程访问 {% else %} Remote {% endif %} &nbsp;
+                    {% if lan == 'en' %}
+                    <span class="form-help" data-bs-toggle="popover" data-bs-placement="top" data-bs-html="true" data-bs-content="
+                    Start solox on the Slave machine first, and then configure the Host here.</p>Note: The port number cannot be the same as the Master machine</p>">?</span>
+                    {% else %}
+                    <span class="form-help" data-bs-toggle="popover" data-bs-placement="top" data-bs-html="true" data-bs-content="先在其他机器启动solox,然后将Host配置在这里</p>注意：端口号不能和主机器一样</p> ">?</span>
+                    {% endif %}</a>
+                </li>
             </ul>
             <div class="tab-content">
-              <!-- Content of card #1 -->
-              <div id="tab-top-1" class="card tab-pane active show">
+                <!-- <div id="tab-top-1" class="card tab-pane active show">
+                    <div class="card-body">
+                        <div class="card">
+                            <div class="ribbon bg-green">Device</div>
+                            <div class="card-body">
+                                <h3 class="card-title">BRNUT21B15044184</h3>
+                            </div>
+                            <div class="card-footer">
+                                <div class="row align-items-center">
+                                    <div class="col-auto">
+                                        <input id="port" type="text" class="form-control"  placeholder="Input tcp mode port">
+                                    </div>
+                                    <div class="col-auto ms-auto">
+                                        <label class="form-check form-switch m-0">
+                                            <input class="form-check-input position-static" type="checkbox">
+                                        </label>
+                                    </div>
+                                </div>
+                            </div>
+                        </div>
+                    </div>
+                </div> -->
+              <div id="tab-top-2" class="card tab-pane">
                 <div class="card-body">
                     <div class="row mb-3">
                         <div class="col-md-6 col-xl-12">
                             <div class="mb-3">
                                 <label class="form-label">{% if lan == 'cn' %} CPU告警值 {% else %} CPU warning value {% endif %}</label>
                                 <input id="cpu_warning_value" type="text" class="form-control"  placeholder="Input placeholder" value="{{ cpuWarning }}">
                             </div>
@@ -197,27 +215,27 @@
                                 <input id="downflow_warning_value" type="text" class="form-control"  placeholder="Input placeholder" value="{{ netdataRecvWarning }}">
                             </div>
                         </div>
                     </div>
                 </div>
               </div>
               <!-- Content of card #2 -->
-              <div id="tab-top-2" class="card tab-pane">
+              <div id="tab-top-3" class="card tab-pane">
                 <div class="card-body">
                     <div class="row mb-3">
                         <div class="col-md-6 col-xl-12">
                             <div class="mb-3">
                                 <label class="form-label">{% if lan == 'cn' %} 持续执行时间（分钟） {% else %} Duration（minutes） {% endif %}</label>
-                                <input id="running_value" type="text" class="form-control"  placeholder="Input placeholder" value="{{ runningTime }}">
+                                <input id="duration" type="text" class="form-control"  placeholder="Input placeholder" value="{{ duration }}">
                             </div>
                         </div>
                     </div>
                 </div>
               </div>
-              <div id="tab-top-3" class="card tab-pane">
+              <div id="tab-top-4" class="card tab-pane">
                 <div class="card-body">
                     <div class="table">
                         <table class="table mb-0">
                             <thead>
                                 <tr>
                                     <th>PC</th>
                                     <th>HOST</th>
@@ -243,21 +261,20 @@
                                     </td>
                                 </tr>
                           </tbody>
                         </table>
                     </div>
                 </div>
             </div>
-            </div>
-          </div>
-        
-        <a class="btn btn-primary mt-3" onclick="saveWorningValue()">
-            {% if lan == 'cn' %} 保存 {% else %} Save {% endif %}
-        </a>
+        </div>
     </div>
+    <a class="btn btn-primary mt-3" onclick="saveWorningValue()">
+        {% if lan == 'cn' %} 保存 {% else %} Save {% endif %}
+    </a>
+</div>
 </div>
 
 <!-- JQ JS -->
 <script src="./static/js/jquery.min.js"></script>
 <!-- tabler -->
 <script src="./static/js/tabler.min.js"></script>
 <script src="./static/js/tabler.demo.min.js"></script>
@@ -367,15 +384,15 @@
             data:{
                 cpuWarning:parseInt($('#cpu_warning_value').val()),
                 memWarning:parseInt($('#mem_warning_value').val()),
                 fpsWarning:parseInt($('#fps_warning_value').val()),
                 netdataRecvWarning:parseInt($('#down_warning_value').val()),
                 netdataSendWarning:parseInt($('#upflow_warning_value').val()),
                 betteryWarning:parseInt($('#battery_warning_value').val()),
-                runningTime:parseInt($('#running_value').val()),
+                duration:parseInt($('#duration').val()),
                 solox_host: $('#host').val(),
                 host_switch:host_switch
             },
             beforeSend: function () {
                 SwalLoading('Save data','Saving warning data.')
             },
             success: function (data) {
```

#### html2text {}

```diff
@@ -24,33 +24,35 @@
 ***** {% block page_title %} {% endblock %} *****
 {% block ms_auto %}{% endblock %}
 {% block page_body %}{% endblock %}
     * {%_if_lan_==_'cn'_%}_ææ¡£_{%_else_%}_Documentation_{%_endif_%}
     * {%_if_lan_==_'cn'_%}_æºç _{%_else_%}_Source_code_{%_endif_%}
     * Copyright ©  SoloX.{% if lan == 'cn' %} ä¿çæææå© {% else %} All
       rights reserved {% endif %}
-    * {%_if_lan_==_'cn'_%}_çæ¬_{%_else_%}_Releases_{%_endif_%}_._V2.6.4
+    * {%_if_lan_==_'cn'_%}_çæ¬_{%_else_%}_Releases_{%_endif_%}_._V2.6.5
 *****  {% if lan == 'cn' %} è®¾ç½® {% else %} Setting {% endif %} *****
-    * Warning_Value
-    * Timer
-    * Agent_ _{%_if_lan_==_'en'_%}_?_{%_else_%}_?_{%_endif_%}
+    *
+    * {%_if_lan_==_'cn'_%}_åè­¦å¼_{%_else_%}_Warning_Value_{%_endif_%}
+    * {%_if_lan_==_'cn'_%}_å®æ¶å¨_{%_else_%}_Timer_{%_endif_%}
+    * {%_if_lan_==_'cn'_%}_è¿ç¨è®¿é®_{%_else_%}_Remote_{%_endif_%}_ _{%_if
+      lan_==_'en'_%}_?_{%_else_%}_?_{%_endif_%}
 {% if lan == 'cn' %} CPUåè­¦å¼ {% else %} CPU warning value {% endif %} [{
 { cpuWarning }}    ]
 {% if lan == 'cn' %} åå­åè­¦å¼ {% else %} Memory warning value {% endif
 %} [{{ memWarning }}    ]
 {% if lan == 'cn' %} FPSåè­¦å¼ {% else %} FPS warning value {% endif %} [{
 { fpsWarning }}    ]
 {% if lan == 'cn' %} çµéåè­¦å¼ {% else %} Battery warning value {% endif
 %} [{{ betteryWarning }}]
 {% if lan == 'cn' %} ä¸è¡æµéåè­¦å¼ {% else %} Send network data warning
 value {% endif %} [{{ netdataSendWarning }}]
 {% if lan == 'cn' %} ä¸è¡æµéåè­¦å¼ {% else %} Recv network data warning
 value {% endif %} [{{ netdataRecvWarning }}]
 {% if lan == 'cn' %} æç»­æ§è¡æ¶é´ï¼åéï¼ {% else %}
-Durationï¼minutesï¼ {% endif %} [{{ runningTime }}   ]
+Durationï¼minutesï¼ {% endif %} [{{ duration }}      ]
 PC HOST              SWITCH
    [{{ solox_host }}  {% if host_switch == '1' %} * {% else %} ⁰ {% endif
    ]                 %}
 {% if lan == 'cn' %} ä¿å­ {% else %} Save {% endif %}
```

### Comparing `solox-2.6.4/solox/templates/index.html` & `solox-2.6.5/solox/templates/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     </ul>
                 </div>
                 <div class="card-body">
                     <div class="tab-content">
                         <div class="tab-pane active show" id="tabs-apm-target">
                             <label class="dropdown-item cursor-pointer"><input class="form-check-input m-0 me-2 cursor-pointer" id="cpu_checkbox" type="checkbox" checked name="cpu"> CPU</label>
                             <label class="dropdown-item cursor-pointer"><input class="form-check-input m-0 me-2 cursor-pointer" id="mem_checkbox" type="checkbox" checked name="mem"> {% if lan == 'cn' %} 内存 {% else %} Memory {% endif %}</label>
-                            <label class="dropdown-item cursor-pointer"><input class="form-check-input m-0 me-2 cursor-pointer" id="flow_checkbox" type="checkbox" checked name="Network-Data"> {% if lan == 'cn' %} 流量 {% else %} Network Data {% endif %}
+                            <label class="dropdown-item cursor-pointer"><input class="form-check-input m-0 me-2 cursor-pointer" id="flow_checkbox" type="checkbox" checked name="Network-Data"> {% if lan == 'cn' %} 流量 {% else %} Network {% endif %}
                                 {% if platform == 'Android' %}
                                 <span class="ms-auto">
                                     <label class="form-check form-check-single form-switch">
                                         <input id="net-switch" class="form-check-input cursor-pointer" type="checkbox" checked name="net-switch" style="margin-right: 5px"> Wifi
                                     </label>
                                 </span>
                                 {% endif %}
@@ -343,27 +343,30 @@
             data:{
                 platform:platform,
                 device:this.value
             },
             beforeSend: function () {
                 $('.select-app').empty();
                 $('.select-app').append('<option></option>');
+                if(platform == 'Android'){
+                    $('.select-pid').empty();
+                }
                 if(lan == 'cn' ){
                     SwalLoading('初始化','正在获取该设备上的所有APP, 请您稍等！');
                 }else{
                     SwalLoading('Package initialization!','Initializing Packages, please wait a mmoment.');
                 }
                 
             },
             success: function (data) {
                 if(data['status'] != 1 ) {
                     if(lan == 'cn' ){
                         SwalFire('error', '连接失败','请检查当前移动设备的是否连接了PC端', 2000);
                     }else{
-                        SwalFire('error', 'Connection failed !', 'No devices found', 2000);
+                        SwalFire('error', 'Connect failed !', 'No devices found', 2000);
                     } 
                 }else{
                     for(var i=0;i<data['pkgnames'].length;i++){
                         $('.select-app').append('<option>'+data['pkgnames'][i]+'</option>')
                     }
                     swal.close();
                 }
@@ -379,16 +382,17 @@
             cache: false,
             data:{
                 platform:platform,
                 device:$('.select-device').val(),
                 pkgname:this.value
             },
             beforeSend: function () {
-                $('.select-pid').empty();
-                // $('.select-pid').append('<option></option>');
+                if(platform == 'Android'){
+                    $('.select-pid').empty();
+                }
                 if(lan == 'cn' ){
                     SwalLoading('初始化','正在获取该APP上的所有进程, 请您稍等！');
                 }else{
                     SwalLoading('Process initialization!','Initializing Process, please wait a mmoment.');
                 }
                 
             },
@@ -396,15 +400,14 @@
                 if(data['status'] != 1 ) {
                     if(lan == 'cn' ){
                         SwalFire('error', '连接失败','请检查当前移动设备的是否连接了PC端', 2000);
                     }else{
                         SwalFire('error', 'Connection failed !', 'No pid found', 2000);
                     } 
                 }else{
-                    // $('.select-pid').val(data['pids'][0]);
                     for(var i=0;i<data['pids'].length;i++){
                         $('.select-pid').append('<option>'+data['pids'][i]+'</option>')
                     }
                     swal.close();
                 }
             }
         });
@@ -429,27 +432,30 @@
             type: "GET",
             async: true,
             cache: false,
             beforeSend: function () {
                 $('.select-device').empty();
                 $('.select-app').empty();
                 $('.select-app').append('<option></option>');
+                if(platform == 'Android'){
+                    $('.select-pid').empty();
+                }
                 if(lan == 'cn' ){
                     SwalLoading('初始化','正在初始化设备环境，请您稍等！');
                 }else{
                     SwalLoading('Device initialization!','Initializing device environment, please wait a moment.');
                 }
                 },
             success: function (data) {
                 console.log(data);
                 if(data['status'] != 1 ) {
                     if(lan == 'cn' ){
                         SwalFire('error', '连接失败','请检查当前移动设备的是否连接了PC端', 2000);
                     }else{
-                        SwalFire('error', 'Connet failed !', 'No devices found', 2000);
+                        SwalFire('error', 'Connect failed !', 'No devices found', 2000);
                     } 
                 }else{
                     for(var i=0;i<data['devices'].length;i++){
                         $('.select-device').append('<option>'+data['devices'][i]+'</option>');
                     }
                     for(var i=0;i<data['pkgnames'].length;i++){
                         $('.select-app').append('<option>'+data['pkgnames'][i]+'</option>');
@@ -1175,15 +1181,15 @@
         let battery_chart = chartsInitialize(type,'Battery');
         return battery_chart
     }
 
     function memInitialize(){
         //初始化mem
         let type = platform == 'Android' ? 'mem_android' : 'mem_ios';
-        let mem_chart = chartsInitialize(type,'MEM（MB）');
+        let mem_chart = chartsInitialize(type,'Memory（MB）');
         return mem_chart
     }
 
     function networkInitialize(){
         //初始化network
         let network_chart = chartsInitialize('network','Network Data（KB)');
         return network_chart
@@ -1331,15 +1337,15 @@
     }
 
     function collectMem(device,pkgname){
         var mem_checkbox = $('#mem_checkbox').is(':checked');
         if(mem_checkbox){
             memInitialize();
             let type = platform == 'Android' ? 'mem_android' : 'mem_ios';
-            mem_chart = collectPers(device,pkgname,type,'MEM（MB）',getMemPss(pkgname,device));
+            mem_chart = collectPers(device,pkgname,type,'Memory（MB）',getMemPss(pkgname,device));
         }
     }
 
     function collectNetwork(device,pkgname){
         var flow_checkbox = $('#flow_checkbox').is(':checked');
         var net_switch = $('#net-switch').is(':checked');
         if(flow_checkbox){
@@ -1421,16 +1427,16 @@
             collectMem(device,pkgname);
             collectNetwork(device,pkgname);
             collectFps(device,pkgname);
             collectBattery(device);
             if(platform == 'iOS'){
                 collectGpu(pkgname);
             }
-            if(parseInt($('#running_value').val()) > 0){
-                var times = parseInt($('#running_value').val()) * 60 * 1000
+            if(parseInt($('#duration').val()) > 0){
+                var times = parseInt($('#duration').val()) * 60 * 1000
                 setTimeout("stopTask()", times)
             }
         }else{
             if(lan == 'cn'){
                 SwalFire('error','执行错误','没有选择APP或者设备',2000);
             }else{
                 SwalFire('error','Execution error','No device or package name selected',2000);
@@ -1508,15 +1514,15 @@
                     }
                 },
                 complete: function(){
                     swal.close();
                 }
             });
         }else{
-            SwalFire('error','Execution error','device is empty',2000)
+            SwalFire('error','Execution error','No devices found',2000)
         }
     }
 
     function getStartupTimeByAndroid(){
         let device = $('.select-device').val();
         let activity = $('#activity').val().trim();
         if(device && activity){
@@ -1542,15 +1548,15 @@
                     }
                 },
                 complete: function(){
                     swal.close();
                 }
             });
         }else{
-            SwalFire('error','Execution error','device or activity is empty',2000)
+            SwalFire('error','Execution error','No devices or activity found',2000)
         }
     }
 
     function getStartupTimeByiOS(){
         let pkgname = $('.select-app').val();
         if(pkgname){
             $.ajax({
@@ -1603,15 +1609,15 @@
             type: "POST",
             async: true,
             cache: false,
             processData: false,
             contentType: false,
             data:formData,
             beforeSend: function () {
-                SwalLoading('Install App!','Installing file to device, please wait。');
+                SwalLoading('Install App!','Installing file to device, please wait a moment.');
                 },
             success: function (data) {
                 console.log(data);
                 if(data['status'] != 1 ) {
                     SwalFire('error', 'Install failed !', data['msg'], 2000);
                 }else{
                     SwalFire('success', 'Install success !', '', 2000);
```

### Comparing `solox-2.6.4/solox/templates/pk.html` & `solox-2.6.5/solox/templates/pk.html`

 * *Files 0% similar despite different names*

```diff
@@ -235,15 +235,15 @@
                 $('.device1').empty();
                 $('.device2').empty();
                 SwalLoading('Device initialization!','Initializing device environment, please wait。');
                 },
             success: function (data) {
                 console.log(data);
                 if(data['status'] != 1 ) {
-                    SwalFire('error', 'Connet failed !', 'Please check if the device is connected', 2000);
+                    SwalFire('error', 'Connect failed !', 'Please check if the device is connected', 2000);
                 }else{
                     if(data['devices'].length <2){
                         SwalFire('error', 'Android Devices < 2 !', 'Please check if the device nums are 2', 2000);
                     }else{
                         $('.device1').val(data['devices'][0]);
                         $('.device2').val(data['devices'][1]);
                         if(model == '2-devices'){
```

### Comparing `solox-2.6.4/solox/templates/report.html` & `solox-2.6.5/solox/templates/report.html`

 * *Files identical despite different names*

### Comparing `solox-2.6.4/solox/view/apis.py` & `solox-2.6.5/solox/view/apis.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,26 +19,26 @@
     """set apm data to cookie"""
     cpuWarning = request.args.get('cpuWarning')
     memWarning = request.args.get('memWarning')
     fpsWarning = request.args.get('fpsWarning')
     netdataRecvWarning = request.args.get('netdataRecvWarning')
     netdataSendWarning = request.args.get('netdataSendWarning')
     betteryWarning = request.args.get('betteryWarning')
-    runningTime = request.args.get('runningTime')
+    duration = request.args.get('duration')
     solox_host = request.args.get('solox_host')
     host_switch = request.args.get('host_switch')
 
     resp = make_response('set cookie ok')
     resp.set_cookie('cpuWarning', cpuWarning)
     resp.set_cookie('memWarning', memWarning)
     resp.set_cookie('fpsWarning', fpsWarning)
     resp.set_cookie('netdataRecvWarning', netdataRecvWarning)
     resp.set_cookie('netdataSendWarning', netdataSendWarning)
     resp.set_cookie('betteryWarning', betteryWarning)
-    resp.set_cookie('runningTime', runningTime)
+    resp.set_cookie('duration', duration)
     resp.set_cookie('solox_host', solox_host)
     resp.set_cookie('host_switch', host_switch)
     return resp
 
 
 @api.route('/apm/initialize', methods=['post', 'get'])
 def initialize():
@@ -87,14 +87,29 @@
             case _:
                 result = {'status': 0, 'msg': f'no this platform = {platform}'}        
     except Exception:
         traceback.print_exc()
         result = {'status': 0, 'msg': 'devices connect error!'}
     return result
 
+# @api.route('/device/tcp/connect', methods=['post', 'get'])
+# def tcpConnect():
+#     """tcp connect """
+#     deviceid = method._request(request, 'deviceid')
+#     port = method._request(request, 'port')
+#     try:
+#         final = d.tcpConnect(deviceId=deviceid, port=port)
+#         if final == 0:
+#             result = {'status': 1, 'msg': 'success'}
+#         else:
+#             result = {'status': 0, 'msg': 'connect failed'}
+#     except Exception as e:
+#          traceback.print_exc()
+#          result = {'status': 0, 'msg': e}            
+#     return result
 
 @api.route('/device/packagenames', methods=['post', 'get'])
 def packageNames():
     """get devices packageNames"""
     platform = method._request(request, 'platform')
     device = method._request(request, 'device')
     match(platform):
```

### Comparing `solox-2.6.4/solox/view/pages.py` & `solox-2.6.5/solox/view/pages.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import json
 import os
 import traceback
 from flask import Blueprint
 from flask import render_template
 from flask import request
-from solox.public.common import File,Method
+from solox.public.common import Devices,File,Method
 from logzero import logger
 
 page = Blueprint("page", __name__)
+d = Devices()
 m = Method()
 f = File()
 
 @page.app_errorhandler(404)
 def page_404(e):
     return render_template('404.html', **locals()), 404
 
@@ -27,45 +28,45 @@
     lan = request.args.get('lan')
     cpuWarning = (0, request.cookies.get('cpuWarning'))[request.cookies.get('cpuWarning') not in [None, 'NaN']]
     memWarning = (0, request.cookies.get('memWarning'))[request.cookies.get('memWarning') not in [None, 'NaN']]
     fpsWarning = (0, request.cookies.get('fpsWarning'))[request.cookies.get('fpsWarning') not in [None, 'NaN']]
     netdataRecvWarning = (0, request.cookies.get('netdataRecvWarning'))[request.cookies.get('netdataRecvWarning') not in [None, 'NaN']]
     netdataSendWarning = (0, request.cookies.get('netdataSendWarning'))[request.cookies.get('netdataSendWarning') not in [None, 'NaN']]
     betteryWarning = (0, request.cookies.get('betteryWarning'))[request.cookies.get('betteryWarning') not in [None, 'NaN']]
-    runningTime = (0, request.cookies.get('runningTime'))[request.cookies.get('runningTime') not in [None, 'NaN']]
+    duration = (0, request.cookies.get('duration'))[request.cookies.get('duration') not in [None, 'NaN']]
     solox_host = ('', request.cookies.get('solox_host'))[request.cookies.get('solox_host') not in [None, 'NaN']]
     host_switch = request.cookies.get('host_switch')
     return render_template('index.html', **locals())
 
 @page.route('/pk')
 def pk():
     lan = request.args.get('lan')
     model = request.args.get('model')
     cpuWarning = (0, request.cookies.get('cpuWarning'))[request.cookies.get('cpuWarning') not in [None, 'NaN']]
     memWarning = (0, request.cookies.get('memWarning'))[request.cookies.get('memWarning') not in [None, 'NaN']]
     fpsWarning = (0, request.cookies.get('fpsWarning'))[request.cookies.get('fpsWarning') not in [None, 'NaN']]
     netdataRecvWarning = (0, request.cookies.get('netdataRecvWarning'))[request.cookies.get('netdataRecvWarning') not in [None, 'NaN']]
     netdataSendWarning = (0, request.cookies.get('netdataSendWarning'))[request.cookies.get('netdataSendWarning') not in [None, 'NaN']]
     betteryWarning = (0, request.cookies.get('betteryWarning'))[request.cookies.get('betteryWarning') not in [None, 'NaN']]
-    runningTime = (0, request.cookies.get('runningTime'))[request.cookies.get('runningTime') not in [None, 'NaN']]
+    duration = (0, request.cookies.get('duration'))[request.cookies.get('duration') not in [None, 'NaN']]
     solox_host = ('', request.cookies.get('solox_host'))[request.cookies.get('solox_host') not in [None, 'NaN']]
     host_switch = request.cookies.get('host_switch')
     return render_template('pk.html', **locals())
 
 
 @page.route('/report')
 def report():
     lan = request.args.get('lan')
     cpuWarning = (0, request.cookies.get('cpuWarning'))[request.cookies.get('cpuWarning') not in [None, 'NaN']]
     memWarning = (0, request.cookies.get('memWarning'))[request.cookies.get('memWarning') not in [None, 'NaN']]
     fpsWarning = (0, request.cookies.get('fpsWarning'))[request.cookies.get('fpsWarning') not in [None, 'NaN']]
     netdataRecvWarning = (0, request.cookies.get('netdataRecvWarning'))[request.cookies.get('netdataRecvWarning') not in [None, 'NaN']]
     netdataSendWarning = (0, request.cookies.get('netdataSendWarning'))[request.cookies.get('netdataSendWarning') not in [None, 'NaN']]
     betteryWarning = (0, request.cookies.get('betteryWarning'))[request.cookies.get('betteryWarning') not in [None, 'NaN']]
-    runningTime = (0, request.cookies.get('runningTime'))[request.cookies.get('runningTime') not in [None, 'NaN']]
+    duration = (0, request.cookies.get('duration'))[request.cookies.get('duration') not in [None, 'NaN']]
     solox_host = ('', request.cookies.get('solox_host'))[request.cookies.get('solox_host') not in [None, 'NaN']]
     host_switch = request.cookies.get('host_switch')
     report_dir = os.path.join(os.getcwd(), 'report')
     if not os.path.exists(report_dir):
         os.mkdir(report_dir)
     dirs = os.listdir(report_dir)
     dir_list = reversed(sorted(dirs, key=lambda x: os.path.getmtime(os.path.join(report_dir, x))))
@@ -100,15 +101,15 @@
     platform = request.args.get('platform')
     cpuWarning = (0, request.cookies.get('cpuWarning'))[request.cookies.get('cpuWarning') not in [None, 'NaN']]
     memWarning = (0, request.cookies.get('memWarning'))[request.cookies.get('memWarning') not in [None, 'NaN']]
     fpsWarning = (0, request.cookies.get('fpsWarning'))[request.cookies.get('fpsWarning') not in [None, 'NaN']]
     netdataRecvWarning = (0, request.cookies.get('netdataRecvWarning'))[request.cookies.get('netdataRecvWarning') not in [None, 'NaN']]
     netdataSendWarning = (0, request.cookies.get('netdataSendWarning'))[request.cookies.get('netdataSendWarning') not in [None, 'NaN']]
     betteryWarning = (0, request.cookies.get('betteryWarning'))[request.cookies.get('betteryWarning') not in [None, 'NaN']]
-    runningTime = (0, request.cookies.get('runningTime'))[request.cookies.get('runningTime') not in [None, 'NaN']]
+    duration = (0, request.cookies.get('duration'))[request.cookies.get('duration') not in [None, 'NaN']]
     solox_host = ('', request.cookies.get('solox_host'))[request.cookies.get('solox_host') not in [None, 'NaN']]
     host_switch = request.cookies.get('host_switch')
     report_dir = os.path.join(os.getcwd(), 'report')
     dirs = os.listdir(report_dir)
     filter_dir = f.filter_secen(scene)
     apm_data = {}
     for dir in dirs:
@@ -131,15 +132,15 @@
     model = request.args.get('model')
     cpuWarning = (0, request.cookies.get('cpuWarning'))[request.cookies.get('cpuWarning') not in [None, 'NaN']]
     memWarning = (0, request.cookies.get('memWarning'))[request.cookies.get('memWarning') not in [None, 'NaN']]
     fpsWarning = (0, request.cookies.get('fpsWarning'))[request.cookies.get('fpsWarning') not in [None, 'NaN']]
     netdataRecvWarning = (0, request.cookies.get('netdataRecvWarning'))[request.cookies.get('netdataRecvWarning') not in [None, 'NaN']]
     netdataSendWarning = (0, request.cookies.get('netdataSendWarning'))[request.cookies.get('netdataSendWarning') not in [None, 'NaN']]
     betteryWarning = (0, request.cookies.get('betteryWarning'))[request.cookies.get('betteryWarning') not in [None, 'NaN']]
-    runningTime = (0, request.cookies.get('runningTime'))[request.cookies.get('runningTime') not in [None, 'NaN']]
+    duration = (0, request.cookies.get('duration'))[request.cookies.get('duration') not in [None, 'NaN']]
     solox_host = ('', request.cookies.get('solox_host'))[request.cookies.get('solox_host') not in [None, 'NaN']]
     host_switch = request.cookies.get('host_switch')
     report_dir = os.path.join(os.getcwd(), 'report')
     dirs = os.listdir(report_dir)
     apm_data = {}
     for dir in dirs:
         if dir == scene:
@@ -162,17 +163,22 @@
     app = request.args.get('app')
     cpuWarning = (0, request.cookies.get('cpuWarning'))[request.cookies.get('cpuWarning') not in [None, 'NaN']]
     memWarning = (0, request.cookies.get('memWarning'))[request.cookies.get('memWarning') not in [None, 'NaN']]
     fpsWarning = (0, request.cookies.get('fpsWarning'))[request.cookies.get('fpsWarning') not in [None, 'NaN']]
     netdataRecvWarning = (0, request.cookies.get('netdataRecvWarning'))[request.cookies.get('netdataRecvWarning') not in [None, 'NaN']]
     netdataSendWarning = (0, request.cookies.get('netdataSendWarning'))[request.cookies.get('netdataSendWarning') not in [None, 'NaN']]
     betteryWarning = (0, request.cookies.get('betteryWarning'))[request.cookies.get('betteryWarning') not in [None, 'NaN']]
-    runningTime = (0, request.cookies.get('runningTime'))[request.cookies.get('runningTime') not in [None, 'NaN']]
+    duration = (0, request.cookies.get('duration'))[request.cookies.get('duration') not in [None, 'NaN']]
     solox_host = ('', request.cookies.get('solox_host'))[request.cookies.get('solox_host') not in [None, 'NaN']]
     host_switch = request.cookies.get('host_switch')
-    if platform == 'Android':
-        apm_data1 = f._setAndroidPerfs(scene1)
-        apm_data2 = f._setAndroidPerfs(scene2)
-    elif platform == 'iOS':
-        apm_data1 = f._setiOSPerfs(scene1)
-        apm_data2 = f._setiOSPerfs(scene2)   
+    try:
+        if platform == 'Android':
+            apm_data1 = f._setAndroidPerfs(scene1)
+            apm_data2 = f._setAndroidPerfs(scene2)
+        elif platform == 'iOS':
+            apm_data1 = f._setiOSPerfs(scene1)
+            apm_data2 = f._setiOSPerfs(scene2)
+    except ZeroDivisionError:
+        pass 
+    except Exception:
+        traceback.print_exc()          
     return render_template('analysis_compare.html', **locals())
```

### Comparing `solox-2.6.4/solox/web.py` & `solox-2.6.5/solox/web.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,17 +38,17 @@
         if thread:
             thread = socketio.start_background_task(target=backgroundThread)
 
 
 def backgroundThread():
     global thread
     try:
-        logger.info('Initializing adb environment ...')
-        os.system('adb kill-server')
-        os.system('adb start-server')
+        # logger.info('Initializing adb environment ...')
+        # os.system('adb kill-server')
+        # os.system('adb start-server')
         current_time = time.strftime("%Y%m%d%H", time.localtime())
         logPath = os.path.join(os.getcwd(),'adblog',f'{current_time}.log')
         logcat = subprocess.Popen(f'adb logcat *:E > {logPath}', stdout=subprocess.PIPE,
                                   shell=True)
         with open(logPath, "r") as f:
             while thread:
                 socketio.sleep(1)
@@ -69,15 +69,15 @@
 
 def hostIP():
     try:
         s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         s.connect(('8.8.8.8', 80))
         ip = s.getsockname()[0]
     except Exception as e:
-        raise e
+        ip = '127.0.0.1'
     finally:
         s.close()
     return ip
 
 
 def listeningPort(port):
     if platform.system() != 'Windows':
@@ -94,40 +94,37 @@
                 line = line.strip()
                 pid = re.findall(r'[1-9]\d*', line)
                 pid_list.append(pid[-1])
             pid_set = list(set(pid_list))[0]
             pid_cmd = 'taskkill -PID {} -F'.format(pid_set)
             os.system(pid_cmd)
 
-
 def getServerStatus(host: str, port: int):
     r = requests.get('http://{}:{}'.format(host, port), timeout=2.0)
     flag = (True, False)[r.status_code == 200]
     return flag
 
 
 def openUrl(host: str, port: int):
     flag = True
     while flag:
-        logger.info('start solox server')
+        logger.info('Start solox server ...')
         flag = getServerStatus(host, port)
     webbrowser.open('http://{}:{}/?platform=Android&lan=en'.format(host, port), new=2)
     logger.info('Running on http://{}:{}/?platform=Android&lan=en (Press CTRL+C to quit)'.format(host, port))
 
 
 def startServer(host: str, port: int):
     socketio.run(app, host=host, debug=False, port=port)
 
-
 def main(host=hostIP(), port=50003):
     try:
         listeningPort(port=port)
-        pool = multiprocessing.Pool(processes=2)
-        pool.apply_async(startServer, (host, port))
-        pool.apply_async(openUrl, (host, port))
-        pool.close()
-        pool.join()
-    except Exception:
-        traceback.print_exc()
+        with multiprocessing.Pool(processes=2) as pool:
+            pool.apply_async(startServer, (host, port))
+            pool.apply_async(openUrl, (host, port))
+            pool.join()
+    except Exception as e:
+        logger.exception(e)
     except KeyboardInterrupt:
         logger.info('stop solox success')
-        sys.exit()
+        sys.exit()
```

### Comparing `solox-2.6.4/solox.egg-info/PKG-INFO` & `solox-2.6.5/solox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solox
-Version: 2.6.4
+Version: 2.6.5
 Summary: SoloX - Real-time collection tool for Android/iOS performance data.
 Home-page: https://github.com/smart-test-ti/SoloX
 Author: Rafa Chen
 Author-email: rafacheninc@gamil.com
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -49,15 +49,15 @@
 💡 If Windows users need to test ios, install and start Itunes. [**Documentation**](https://github.com/alibaba/taobao-iphone-device)
 
 ## 📥Installation
 
 ### default
 
 ```shell
-pip install -U solox  (pip install solox==2.6.2)
+pip install -U solox  (pip install solox==2.6.4)
 ```
 
 ### mirrors
 
 ```shell
 pip install -i  https://mirrors.ustc.edu.cn/pypi/web/simple -U solox
 ```
@@ -81,16 +81,14 @@
 ## 🏴󠁣󠁩󠁣󠁭󠁿Collect in python
 
 ```python
 
 from solox.public.apm import APM
 from solox.public.common import Devices
 
-# solox version >= 2.1.2
-
 d = Devices()
 pids = d.getPid(deviceId='ca6bd5a5', pkgName='com.bilibili.app.in') # for android
 
 apm = APM(pkgName='com.bilibili.app.in',platform='Android', deviceId='ca6bd5a5', 
           surfaceview=True, noLog=True, pid=None)
 # apm = APM(pkgName='com.bilibili.app.in', platform='iOS') only supports one device
 # surfaceview： False = gfxinfo (Developer - GPU rendering mode - adb shell dumpsys gfxinfo)
@@ -105,15 +103,15 @@
 gpu = apm.collectGpu() # % only supports ios
 
 # ************* Collect all performance parameter ************* #
 apm = APM(pkgName='com.bilibili.app.in',platform='Android', deviceId='ca6bd5a5', 
           surfaceview=True, noLog=False, pid=None, duration=20) # duration : second
 # apm = APM(pkgName='com.bilibili.app.in', platform='iOS',  noLog=False, duration=20)
 if __name__ == '__main__':
-     apm.collectAll()
+     apm.collectAll() # will generate HTML report
 ```
 
 ## 🏴󠁣󠁩󠁣󠁭󠁿Collect in API
 
 ### Start the service in the background
 
 ```
```

### Comparing `solox-2.6.4/solox.egg-info/SOURCES.txt` & `solox-2.6.5/solox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

