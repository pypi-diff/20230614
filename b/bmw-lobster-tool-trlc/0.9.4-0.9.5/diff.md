# Comparing `tmp/bmw-lobster-tool-trlc-0.9.4.tar.gz` & `tmp/bmw-lobster-tool-trlc-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmw-lobster-tool-trlc-0.9.4.tar", last modified: Tue Jun 13 09:18:56 2023, max compression
+gzip compressed data, was "bmw-lobster-tool-trlc-0.9.5.tar", last modified: Wed Jun 14 14:03:19 2023, max compression
```

## Comparing `bmw-lobster-tool-trlc-0.9.4.tar` & `bmw-lobster-tool-trlc-0.9.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:56.525239 bmw-lobster-tool-trlc-0.9.4/
--rw-r--r--   0 florian   (1000) florian   (1000)     3210 2023-06-13 09:18:56.525239 bmw-lobster-tool-trlc-0.9.4/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)     2282 2023-06-13 09:17:37.000000 bmw-lobster-tool-trlc-0.9.4/README.md
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:56.525239 bmw-lobster-tool-trlc-0.9.4/bmw_lobster_tool_trlc.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     3210 2023-06-13 09:18:56.000000 bmw-lobster-tool-trlc-0.9.4/bmw_lobster_tool_trlc.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      317 2023-06-13 09:18:56.000000 bmw-lobster-tool-trlc-0.9.4/bmw_lobster_tool_trlc.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-13 09:18:56.000000 bmw-lobster-tool-trlc-0.9.4/bmw_lobster_tool_trlc.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       62 2023-06-13 09:18:56.000000 bmw-lobster-tool-trlc-0.9.4/bmw_lobster_tool_trlc.egg-info/entry_points.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       36 2023-06-13 09:18:56.000000 bmw-lobster-tool-trlc-0.9.4/bmw_lobster_tool_trlc.egg-info/requires.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-06-13 09:18:56.000000 bmw-lobster-tool-trlc-0.9.4/bmw_lobster_tool_trlc.egg-info/top_level.txt
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:56.525239 bmw-lobster-tool-trlc-0.9.4/lobster/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:56.525239 bmw-lobster-tool-trlc-0.9.4/lobster/tools/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:56.525239 bmw-lobster-tool-trlc-0.9.4/lobster/tools/trlc/
--rw-r--r--   0 florian   (1000) florian   (1000)    15533 2023-06-13 09:18:56.000000 bmw-lobster-tool-trlc-0.9.4/lobster/tools/trlc/trlc.py
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-06-13 09:18:56.525239 bmw-lobster-tool-trlc-0.9.4/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     2257 2023-06-13 09:17:37.000000 bmw-lobster-tool-trlc-0.9.4/setup.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-14 14:03:19.449640 bmw-lobster-tool-trlc-0.9.5/
+-rw-r--r--   0 florian   (1000) florian   (1000)     3210 2023-06-14 14:03:19.449640 bmw-lobster-tool-trlc-0.9.5/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     2282 2023-06-13 09:17:37.000000 bmw-lobster-tool-trlc-0.9.5/README.md
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-14 14:03:19.449640 bmw-lobster-tool-trlc-0.9.5/bmw_lobster_tool_trlc.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     3210 2023-06-14 14:03:19.000000 bmw-lobster-tool-trlc-0.9.5/bmw_lobster_tool_trlc.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      317 2023-06-14 14:03:19.000000 bmw-lobster-tool-trlc-0.9.5/bmw_lobster_tool_trlc.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-14 14:03:19.000000 bmw-lobster-tool-trlc-0.9.5/bmw_lobster_tool_trlc.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       62 2023-06-14 14:03:19.000000 bmw-lobster-tool-trlc-0.9.5/bmw_lobster_tool_trlc.egg-info/entry_points.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       36 2023-06-14 14:03:19.000000 bmw-lobster-tool-trlc-0.9.5/bmw_lobster_tool_trlc.egg-info/requires.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-06-14 14:03:19.000000 bmw-lobster-tool-trlc-0.9.5/bmw_lobster_tool_trlc.egg-info/top_level.txt
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-14 14:03:19.445640 bmw-lobster-tool-trlc-0.9.5/lobster/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-14 14:03:19.445640 bmw-lobster-tool-trlc-0.9.5/lobster/tools/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-14 14:03:19.449640 bmw-lobster-tool-trlc-0.9.5/lobster/tools/trlc/
+-rw-r--r--   0 florian   (1000) florian   (1000)    15533 2023-06-14 14:03:19.000000 bmw-lobster-tool-trlc-0.9.5/lobster/tools/trlc/trlc.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-06-14 14:03:19.449640 bmw-lobster-tool-trlc-0.9.5/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     2257 2023-06-13 09:17:37.000000 bmw-lobster-tool-trlc-0.9.5/setup.py
```

### Comparing `bmw-lobster-tool-trlc-0.9.4/PKG-INFO` & `bmw-lobster-tool-trlc-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-tool-trlc
-Version: 0.9.4
+Version: 0.9.5
 Summary: LOBSTER Tool for TRLC
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
```

### Comparing `bmw-lobster-tool-trlc-0.9.4/README.md` & `bmw-lobster-tool-trlc-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `bmw-lobster-tool-trlc-0.9.4/bmw_lobster_tool_trlc.egg-info/PKG-INFO` & `bmw-lobster-tool-trlc-0.9.5/bmw_lobster_tool_trlc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-tool-trlc
-Version: 0.9.4
+Version: 0.9.5
 Summary: LOBSTER Tool for TRLC
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
```

### Comparing `bmw-lobster-tool-trlc-0.9.4/lobster/tools/trlc/trlc.py` & `bmw-lobster-tool-trlc-0.9.5/lobster/tools/trlc/trlc.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-tool-trlc-0.9.4/setup.py` & `bmw-lobster-tool-trlc-0.9.5/setup.py`

 * *Files identical despite different names*

