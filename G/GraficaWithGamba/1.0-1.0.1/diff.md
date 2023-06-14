# Comparing `tmp/GraficaWithGamba-1.0.tar.gz` & `tmp/GraficaWithGamba-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GraficaWithGamba-1.0.tar", last modified: Wed Jun 14 14:37:16 2023, max compression
+gzip compressed data, was "GraficaWithGamba-1.0.1.tar", last modified: Wed Jun 14 15:15:23 2023, max compression
```

## Comparing `GraficaWithGamba-1.0.tar` & `GraficaWithGamba-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 14:37:16.100520 GraficaWithGamba-1.0/
--rw-rw-rw-   0        0        0     1091 2023-06-14 14:27:15.000000 GraficaWithGamba-1.0/LICENSE
--rw-rw-rw-   0        0        0      532 2023-06-14 14:37:16.100520 GraficaWithGamba-1.0/PKG-INFO
--rw-rw-rw-   0        0        0       60 2023-06-14 14:26:35.000000 GraficaWithGamba-1.0/README.md
--rw-rw-rw-   0        0        0      468 2023-06-14 14:36:24.000000 GraficaWithGamba-1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-14 14:37:16.101522 GraficaWithGamba-1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-14 14:37:16.072581 GraficaWithGamba-1.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-14 14:37:16.080559 GraficaWithGamba-1.0/src/GraficaWithGamba/
--rw-rw-rw-   0        0        0        0 2023-06-14 14:17:35.000000 GraficaWithGamba-1.0/src/GraficaWithGamba/__init__.py
--rw-rw-rw-   0        0        0     7031 2023-06-14 04:45:07.000000 GraficaWithGamba-1.0/src/GraficaWithGamba/grafica.py
-drwxrwxrwx   0        0        0        0 2023-06-14 14:37:16.099220 GraficaWithGamba-1.0/src/GraficaWithGamba.egg-info/
--rw-rw-rw-   0        0        0      532 2023-06-14 14:37:16.000000 GraficaWithGamba-1.0/src/GraficaWithGamba.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-06-14 14:37:16.000000 GraficaWithGamba-1.0/src/GraficaWithGamba.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 14:37:16.000000 GraficaWithGamba-1.0/src/GraficaWithGamba.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-14 14:37:16.000000 GraficaWithGamba-1.0/src/GraficaWithGamba.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 15:15:23.188199 GraficaWithGamba-1.0.1/
+-rw-rw-rw-   0        0        0     1091 2023-06-14 14:27:15.000000 GraficaWithGamba-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      845 2023-06-14 15:15:23.187201 GraficaWithGamba-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2023-06-14 15:10:19.000000 GraficaWithGamba-1.0.1/README.md
+-rw-rw-rw-   0        0        0      491 2023-06-14 15:13:20.000000 GraficaWithGamba-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-14 15:15:23.189195 GraficaWithGamba-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-14 15:15:23.159276 GraficaWithGamba-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-14 15:15:23.169249 GraficaWithGamba-1.0.1/src/GraficaWithGamba/
+-rw-rw-rw-   0        0        0        0 2023-06-14 14:17:35.000000 GraficaWithGamba-1.0.1/src/GraficaWithGamba/__init__.py
+-rw-rw-rw-   0        0        0     7031 2023-06-14 14:59:11.000000 GraficaWithGamba-1.0.1/src/GraficaWithGamba/grafica.py
+drwxrwxrwx   0        0        0        0 2023-06-14 15:15:23.185205 GraficaWithGamba-1.0.1/src/GraficaWithGamba.egg-info/
+-rw-rw-rw-   0        0        0      845 2023-06-14 15:15:23.000000 GraficaWithGamba-1.0.1/src/GraficaWithGamba.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-06-14 15:15:23.000000 GraficaWithGamba-1.0.1/src/GraficaWithGamba.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 15:15:23.000000 GraficaWithGamba-1.0.1/src/GraficaWithGamba.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-14 15:15:23.000000 GraficaWithGamba-1.0.1/src/GraficaWithGamba.egg-info/top_level.txt
```

### Comparing `GraficaWithGamba-1.0/LICENSE` & `GraficaWithGamba-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `GraficaWithGamba-1.0/src/GraficaWithGamba/grafica.py` & `GraficaWithGamba-1.0.1/src/GraficaWithGamba/grafica.py`

 * *Files identical despite different names*

