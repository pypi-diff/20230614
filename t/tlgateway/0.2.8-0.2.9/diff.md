# Comparing `tmp/tlgateway-0.2.8.tar.gz` & `tmp/tlgateway-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/__w/impl-pytg/impl-pytg/dist/.tmp-8bbfxxhy/tlgateway-0.2.8.tar", last modified: Thu Mar  9 08:27:47 2023, max compression
+gzip compressed data, was "/__w/impl-pytg/impl-pytg/dist/.tmp-z_661wj2/tlgateway-0.2.9.tar", last modified: Fri Mar 17 00:41:57 2023, max compression
```

## Comparing `tlgateway-0.2.8.tar` & `tlgateway-0.2.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 08:27:47.000000 tlgateway-0.2.8/
--rw-r--r--   0 root         (0) root         (0)      787 2023-03-09 08:27:47.000000 tlgateway-0.2.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       49 2023-03-09 08:27:39.000000 tlgateway-0.2.8/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-09 08:27:47.000000 tlgateway-0.2.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1069 2023-03-09 08:27:39.000000 tlgateway-0.2.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 08:27:47.000000 tlgateway-0.2.8/tlgateway.egg-info/
--rw-r--r--   0 root         (0) root         (0)      787 2023-03-09 08:27:47.000000 tlgateway-0.2.8/tlgateway.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      183 2023-03-09 08:27:47.000000 tlgateway-0.2.8/tlgateway.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-09 08:27:47.000000 tlgateway-0.2.8/tlgateway.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-03-09 08:27:47.000000 tlgateway-0.2.8/tlgateway.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-09 08:27:47.000000 tlgateway-0.2.8/tlgateway.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 00:41:57.000000 tlgateway-0.2.9/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-03-17 00:41:57.000000 tlgateway-0.2.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       49 2023-03-17 00:41:46.000000 tlgateway-0.2.9/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-03-17 00:41:57.000000 tlgateway-0.2.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-03-17 00:41:46.000000 tlgateway-0.2.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 00:41:57.000000 tlgateway-0.2.9/tlgateway.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-03-17 00:41:57.000000 tlgateway-0.2.9/tlgateway.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      183 2023-03-17 00:41:57.000000 tlgateway-0.2.9/tlgateway.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-17 00:41:57.000000 tlgateway-0.2.9/tlgateway.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-03-17 00:41:57.000000 tlgateway-0.2.9/tlgateway.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-17 00:41:57.000000 tlgateway-0.2.9/tlgateway.egg-info/top_level.txt
```

### Comparing `tlgateway-0.2.8/PKG-INFO` & `tlgateway-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tlgateway
-Version: 0.2.8
+Version: 0.2.9
 Summary: Implemetation of trading gateway for traders.link
 Home-page: http://www.puyuan.tech
 Author: puyuan.tech
 Author-email: info@puyuan.tech
 Maintainer: puyuan_staff
 Maintainer-email: github@puyuan.tech
 License: MIT License
```

### Comparing `tlgateway-0.2.8/setup.py` & `tlgateway-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `tlgateway-0.2.8/tlgateway.egg-info/PKG-INFO` & `tlgateway-0.2.9/tlgateway.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tlgateway
-Version: 0.2.8
+Version: 0.2.9
 Summary: Implemetation of trading gateway for traders.link
 Home-page: http://www.puyuan.tech
 Author: puyuan.tech
 Author-email: info@puyuan.tech
 Maintainer: puyuan_staff
 Maintainer-email: github@puyuan.tech
 License: MIT License
```

