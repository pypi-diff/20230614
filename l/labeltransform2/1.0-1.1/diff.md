# Comparing `tmp/labeltransform2-1.0.tar.gz` & `tmp/labeltransform2-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labeltransform2-1.0.tar", last modified: Wed Jun 14 08:22:02 2023, max compression
+gzip compressed data, was "labeltransform2-1.1.tar", last modified: Wed Jun 14 08:28:10 2023, max compression
```

## Comparing `labeltransform2-1.0.tar` & `labeltransform2-1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 08:22:02.290852 labeltransform2-1.0/
--rw-rw-rw-   0        0        0    11558 2023-06-14 02:18:41.000000 labeltransform2-1.0/LICENSE
--rw-rw-rw-   0        0        0      179 2023-06-14 08:22:02.290852 labeltransform2-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      961 2023-06-14 02:18:41.000000 labeltransform2-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 08:22:02.285855 labeltransform2-1.0/detect/
--rw-rw-rw-   0        0        0       34 2023-06-14 07:41:09.000000 labeltransform2-1.0/detect/__init__.py
--rw-rw-rw-   0        0        0     3623 2023-06-14 07:40:11.000000 labeltransform2-1.0/detect/generate_voc.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:22:02.289854 labeltransform2-1.0/labeltransform2.egg-info/
--rw-rw-rw-   0        0        0      179 2023-06-14 08:22:02.000000 labeltransform2-1.0/labeltransform2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-06-14 08:22:02.000000 labeltransform2-1.0/labeltransform2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 08:22:02.000000 labeltransform2-1.0/labeltransform2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-06-14 08:22:02.000000 labeltransform2-1.0/labeltransform2.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-14 08:22:02.000000 labeltransform2-1.0/labeltransform2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 08:22:02.290852 labeltransform2-1.0/setup.cfg
--rw-rw-rw-   0        0        0      302 2023-06-14 08:21:58.000000 labeltransform2-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:28:10.820267 labeltransform2-1.1/
+-rw-rw-rw-   0        0        0    11558 2023-06-14 02:18:41.000000 labeltransform2-1.1/LICENSE
+-rw-rw-rw-   0        0        0      179 2023-06-14 08:28:10.820267 labeltransform2-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      961 2023-06-14 02:18:41.000000 labeltransform2-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 08:28:10.814265 labeltransform2-1.1/labeltransform2/
+-rw-rw-rw-   0        0        0       34 2023-06-14 07:41:09.000000 labeltransform2-1.1/labeltransform2/__init__.py
+-rw-rw-rw-   0        0        0     3623 2023-06-14 07:40:11.000000 labeltransform2-1.1/labeltransform2/generate_voc.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:28:10.819268 labeltransform2-1.1/labeltransform2.egg-info/
+-rw-rw-rw-   0        0        0      179 2023-06-14 08:28:10.000000 labeltransform2-1.1/labeltransform2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-06-14 08:28:10.000000 labeltransform2-1.1/labeltransform2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 08:28:10.000000 labeltransform2-1.1/labeltransform2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-06-14 08:28:10.000000 labeltransform2-1.1/labeltransform2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-14 08:28:10.000000 labeltransform2-1.1/labeltransform2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 08:28:10.820267 labeltransform2-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      303 2023-06-14 08:28:05.000000 labeltransform2-1.1/setup.py
```

### Comparing `labeltransform2-1.0/LICENSE` & `labeltransform2-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `labeltransform2-1.0/README.md` & `labeltransform2-1.1/README.md`

 * *Files identical despite different names*

### Comparing `labeltransform2-1.0/detect/generate_voc.py` & `labeltransform2-1.1/labeltransform2/generate_voc.py`

 * *Files identical despite different names*

