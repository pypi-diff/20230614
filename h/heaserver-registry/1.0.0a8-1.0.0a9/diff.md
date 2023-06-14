# Comparing `tmp/heaserver-registry-1.0.0a8.tar.gz` & `tmp/heaserver-registry-1.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\heaserver-registry-1.0.0a8.tar", last modified: Thu Jun 24 00:41:20 2021, max compression
+gzip compressed data, was "dist\heaserver-registry-1.0.0a9.tar", last modified: Thu Jun 24 20:01:44 2021, max compression
```

## Comparing `heaserver-registry-1.0.0a8.tar` & `heaserver-registry-1.0.0a9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2021-06-24 00:41:20.564486 heaserver-registry-1.0.0a8/
--rw-rw-rw-   0        0        0       37 2021-06-15 23:55:23.000000 heaserver-registry-1.0.0a8/MANIFEST.in
--rw-rw-rw-   0        0        0      333 2021-06-24 00:41:20.563489 heaserver-registry-1.0.0a8/PKG-INFO
--rw-rw-rw-   0        0        0     3516 2021-06-20 02:06:55.000000 heaserver-registry-1.0.0a8/README.md
--rw-rw-rw-   0        0        0       42 2021-06-24 00:41:20.564486 heaserver-registry-1.0.0a8/setup.cfg
--rw-rw-rw-   0        0        0      984 2021-06-24 00:41:01.000000 heaserver-registry-1.0.0a8/setup.py
-drwxrwxrwx   0        0        0        0 2021-06-24 00:41:20.488494 heaserver-registry-1.0.0a8/src/
-drwxrwxrwx   0        0        0        0 2021-06-24 00:41:20.487535 heaserver-registry-1.0.0a8/src/heaserver/
-drwxrwxrwx   0        0        0        0 2021-06-24 00:41:20.519508 heaserver-registry-1.0.0a8/src/heaserver/registry/
--rw-rw-rw-   0        0        0        0 2020-02-24 16:38:54.000000 heaserver-registry-1.0.0a8/src/heaserver/registry/__init__.py
--rw-rw-rw-   0        0        0     7143 2021-06-23 22:32:06.000000 heaserver-registry-1.0.0a8/src/heaserver/registry/service.py
-drwxrwxrwx   0        0        0        0 2021-06-24 00:41:20.521480 heaserver-registry-1.0.0a8/src/heaserver/registry/wstl/
--rw-rw-rw-   0        0        0     4248 2020-07-03 06:00:05.000000 heaserver-registry-1.0.0a8/src/heaserver/registry/wstl/all.json
-drwxrwxrwx   0        0        0        0 2021-06-24 00:41:20.549481 heaserver-registry-1.0.0a8/src/heaserver_registry.egg-info/
--rw-rw-rw-   0        0        0      333 2021-06-24 00:41:20.000000 heaserver-registry-1.0.0a8/src/heaserver_registry.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      546 2021-06-24 00:41:20.000000 heaserver-registry-1.0.0a8/src/heaserver_registry.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-06-24 00:41:20.000000 heaserver-registry-1.0.0a8/src/heaserver_registry.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2021-06-24 00:41:20.000000 heaserver-registry-1.0.0a8/src/heaserver_registry.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2021-06-24 00:41:20.000000 heaserver-registry-1.0.0a8/src/heaserver_registry.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2021-06-24 00:41:20.000000 heaserver-registry-1.0.0a8/src/heaserver_registry.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2021-06-24 00:41:20.489479 heaserver-registry-1.0.0a8/tests/
-drwxrwxrwx   0        0        0        0 2021-06-24 00:41:20.490480 heaserver-registry-1.0.0a8/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2021-06-24 00:41:20.560483 heaserver-registry-1.0.0a8/tests/heaserver/registrytest/
--rw-rw-rw-   0        0        0        0 2020-02-24 16:38:54.000000 heaserver-registry-1.0.0a8/tests/heaserver/registrytest/__init__.py
--rw-rw-rw-   0        0        0     2072 2021-06-23 22:17:28.000000 heaserver-registry-1.0.0a8/tests/heaserver/registrytest/componenttestcase.py
--rw-rw-rw-   0        0        0     1217 2020-07-03 22:55:50.000000 heaserver-registry-1.0.0a8/tests/heaserver/registrytest/test_all.py
+drwxrwxrwx   0        0        0        0 2021-06-24 20:01:44.068056 heaserver-registry-1.0.0a9/
+-rw-rw-rw-   0        0        0       37 2021-06-24 16:29:23.000000 heaserver-registry-1.0.0a9/MANIFEST.in
+-rw-rw-rw-   0        0        0     4339 2021-06-24 20:01:44.067055 heaserver-registry-1.0.0a9/PKG-INFO
+-rw-rw-rw-   0        0        0     3516 2021-06-24 16:29:23.000000 heaserver-registry-1.0.0a9/README.md
+-rw-rw-rw-   0        0        0       42 2021-06-24 20:01:44.068056 heaserver-registry-1.0.0a9/setup.cfg
+-rw-rw-rw-   0        0        0     1328 2021-06-24 20:01:04.000000 heaserver-registry-1.0.0a9/setup.py
+drwxrwxrwx   0        0        0        0 2021-06-24 20:01:43.991053 heaserver-registry-1.0.0a9/src/
+drwxrwxrwx   0        0        0        0 2021-06-24 20:01:43.990054 heaserver-registry-1.0.0a9/src/heaserver/
+drwxrwxrwx   0        0        0        0 2021-06-24 20:01:44.000060 heaserver-registry-1.0.0a9/src/heaserver/registry/
+-rw-rw-rw-   0        0        0        0 2020-02-24 16:38:54.000000 heaserver-registry-1.0.0a9/src/heaserver/registry/__init__.py
+-rw-rw-rw-   0        0        0     7143 2021-06-24 16:29:23.000000 heaserver-registry-1.0.0a9/src/heaserver/registry/service.py
+drwxrwxrwx   0        0        0        0 2021-06-24 20:01:44.002086 heaserver-registry-1.0.0a9/src/heaserver/registry/wstl/
+-rw-rw-rw-   0        0        0     4248 2020-07-03 06:00:05.000000 heaserver-registry-1.0.0a9/src/heaserver/registry/wstl/all.json
+drwxrwxrwx   0        0        0        0 2021-06-24 20:01:44.051056 heaserver-registry-1.0.0a9/src/heaserver_registry.egg-info/
+-rw-rw-rw-   0        0        0     4339 2021-06-24 20:01:43.000000 heaserver-registry-1.0.0a9/src/heaserver_registry.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      546 2021-06-24 20:01:43.000000 heaserver-registry-1.0.0a9/src/heaserver_registry.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-06-24 20:01:43.000000 heaserver-registry-1.0.0a9/src/heaserver_registry.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2021-06-24 20:01:43.000000 heaserver-registry-1.0.0a9/src/heaserver_registry.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2021-06-24 20:01:43.000000 heaserver-registry-1.0.0a9/src/heaserver_registry.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2021-06-24 20:01:43.000000 heaserver-registry-1.0.0a9/src/heaserver_registry.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-06-24 20:01:43.992060 heaserver-registry-1.0.0a9/tests/
+drwxrwxrwx   0        0        0        0 2021-06-24 20:01:43.992060 heaserver-registry-1.0.0a9/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2021-06-24 20:01:44.064087 heaserver-registry-1.0.0a9/tests/heaserver/registrytest/
+-rw-rw-rw-   0        0        0        0 2020-02-24 16:38:54.000000 heaserver-registry-1.0.0a9/tests/heaserver/registrytest/__init__.py
+-rw-rw-rw-   0        0        0     2072 2021-06-24 16:29:23.000000 heaserver-registry-1.0.0a9/tests/heaserver/registrytest/componenttestcase.py
+-rw-rw-rw-   0        0        0     1217 2020-07-03 22:55:50.000000 heaserver-registry-1.0.0a9/tests/heaserver/registrytest/test_all.py
```

### Comparing `heaserver-registry-1.0.0a8/README.md` & `heaserver-registry-1.0.0a9/README.md`

 * *Files identical despite different names*

### Comparing `heaserver-registry-1.0.0a8/src/heaserver/registry/service.py` & `heaserver-registry-1.0.0a9/src/heaserver/registry/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-registry-1.0.0a8/src/heaserver/registry/wstl/all.json` & `heaserver-registry-1.0.0a9/src/heaserver/registry/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-registry-1.0.0a8/src/heaserver_registry.egg-info/SOURCES.txt` & `heaserver-registry-1.0.0a9/src/heaserver_registry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-registry-1.0.0a8/tests/heaserver/registrytest/componenttestcase.py` & `heaserver-registry-1.0.0a9/tests/heaserver/registrytest/componenttestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-registry-1.0.0a8/tests/heaserver/registrytest/test_all.py` & `heaserver-registry-1.0.0a9/tests/heaserver/registrytest/test_all.py`

 * *Files identical despite different names*

