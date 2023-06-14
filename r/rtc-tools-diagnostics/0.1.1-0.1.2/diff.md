# Comparing `tmp/rtc-tools-diagnostics-0.1.1.tar.gz` & `tmp/rtc-tools-diagnostics-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtc-tools-diagnostics-0.1.1.tar", last modified: Tue Jun 13 14:30:47 2023, max compression
+gzip compressed data, was "rtc-tools-diagnostics-0.1.2.tar", last modified: Wed Jun 14 12:06:40 2023, max compression
```

## Comparing `rtc-tools-diagnostics-0.1.1.tar` & `rtc-tools-diagnostics-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:30:47.208629 rtc-tools-diagnostics-0.1.1/
--rw-rw-rw-   0 root         (0) root         (0)     7652 2023-06-13 14:30:38.000000 rtc-tools-diagnostics-0.1.1/COPYING.LESSER
--rw-r--r--   0 root         (0) root         (0)      266 2023-06-13 14:30:47.208629 rtc-tools-diagnostics-0.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      201 2023-06-13 14:30:38.000000 rtc-tools-diagnostics-0.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:30:47.208629 rtc-tools-diagnostics-0.1.1/rtc_tools_diagnostics.egg-info/
--rw-r--r--   0 root         (0) root         (0)      266 2023-06-13 14:30:47.000000 rtc-tools-diagnostics-0.1.1/rtc_tools_diagnostics.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      314 2023-06-13 14:30:47.000000 rtc-tools-diagnostics-0.1.1/rtc_tools_diagnostics.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 14:30:47.000000 rtc-tools-diagnostics-0.1.1/rtc_tools_diagnostics.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-06-13 14:30:47.000000 rtc-tools-diagnostics-0.1.1/rtc_tools_diagnostics.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 14:30:47.000000 rtc-tools-diagnostics-0.1.1/rtc_tools_diagnostics.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:30:47.209629 rtc-tools-diagnostics-0.1.1/rtctools_diagnostics/
--rw-r--r--   0 root         (0) root         (0)      497 2023-06-13 14:30:47.209629 rtc-tools-diagnostics-0.1.1/rtctools_diagnostics/_version.py
--rw-rw-rw-   0 root         (0) root         (0)      246 2023-06-13 14:30:47.209629 rtc-tools-diagnostics-0.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      461 2023-06-13 14:30:38.000000 rtc-tools-diagnostics-0.1.1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    83607 2023-06-13 14:30:38.000000 rtc-tools-diagnostics-0.1.1/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 12:06:40.864255 rtc-tools-diagnostics-0.1.2/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2023-06-14 12:06:39.000000 rtc-tools-diagnostics-0.1.2/COPYING.LESSER
+-rw-r--r--   0 root         (0) root         (0)      406 2023-06-14 12:06:40.864255 rtc-tools-diagnostics-0.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      201 2023-06-14 12:06:39.000000 rtc-tools-diagnostics-0.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 12:06:40.864255 rtc-tools-diagnostics-0.1.2/rtc_tools_diagnostics.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      406 2023-06-14 12:06:40.000000 rtc-tools-diagnostics-0.1.2/rtc_tools_diagnostics.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      314 2023-06-14 12:06:40.000000 rtc-tools-diagnostics-0.1.2/rtc_tools_diagnostics.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 12:06:40.000000 rtc-tools-diagnostics-0.1.2/rtc_tools_diagnostics.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-06-14 12:06:40.000000 rtc-tools-diagnostics-0.1.2/rtc_tools_diagnostics.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 12:06:40.000000 rtc-tools-diagnostics-0.1.2/rtc_tools_diagnostics.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 12:06:40.865255 rtc-tools-diagnostics-0.1.2/rtctools_diagnostics/
+-rw-r--r--   0 root         (0) root         (0)      497 2023-06-14 12:06:40.865255 rtc-tools-diagnostics-0.1.2/rtctools_diagnostics/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      246 2023-06-14 12:06:40.864255 rtc-tools-diagnostics-0.1.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      725 2023-06-14 12:06:39.000000 rtc-tools-diagnostics-0.1.2/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)    83607 2023-06-14 12:06:39.000000 rtc-tools-diagnostics-0.1.2/versioneer.py
```

### Comparing `rtc-tools-diagnostics-0.1.1/COPYING.LESSER` & `rtc-tools-diagnostics-0.1.2/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `rtc-tools-diagnostics-0.1.1/versioneer.py` & `rtc-tools-diagnostics-0.1.2/versioneer.py`

 * *Files identical despite different names*

