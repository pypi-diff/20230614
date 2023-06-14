# Comparing `tmp/spatial-moto-0.0.2.tar.gz` & `tmp/spatial-moto-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatial-moto-0.0.2.tar", last modified: Wed Jun 14 11:09:17 2023, max compression
+gzip compressed data, was "spatial-moto-0.0.3.tar", last modified: Wed Jun 14 11:19:45 2023, max compression
```

## Comparing `spatial-moto-0.0.2.tar` & `spatial-moto-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0 walido    (1000) walido    (1000)        0 2023-06-14 11:09:17.038865 spatial-moto-0.0.2/
--rwxrwxrwx   0 walido    (1000) walido    (1000)     1071 2023-06-14 09:31:33.000000 spatial-moto-0.0.2/LICENSE
--rwxrwxrwx   0 walido    (1000) walido    (1000)      669 2023-06-14 11:09:17.038363 spatial-moto-0.0.2/PKG-INFO
--rwxrwxrwx   0 walido    (1000) walido    (1000)     1114 2023-06-14 11:06:59.000000 spatial-moto-0.0.2/README.md
--rwxrwxrwx   0 walido    (1000) walido    (1000)       38 2023-06-14 11:09:17.039024 spatial-moto-0.0.2/setup.cfg
--rwxrwxrwx   0 walido    (1000) walido    (1000)     1306 2023-06-14 11:08:48.000000 spatial-moto-0.0.2/setup.py
-drwxrwxrwx   0 walido    (1000) walido    (1000)        0 2023-06-14 11:09:16.967275 spatial-moto-0.0.2/spatial_moto.egg-info/
--rwxrwxrwx   0 walido    (1000) walido    (1000)      669 2023-06-14 11:09:16.000000 spatial-moto-0.0.2/spatial_moto.egg-info/PKG-INFO
--rwxrwxrwx   0 walido    (1000) walido    (1000)      374 2023-06-14 11:09:16.000000 spatial-moto-0.0.2/spatial_moto.egg-info/SOURCES.txt
--rwxrwxrwx   0 walido    (1000) walido    (1000)        1 2023-06-14 11:09:16.000000 spatial-moto-0.0.2/spatial_moto.egg-info/dependency_links.txt
--rwxrwxrwx   0 walido    (1000) walido    (1000)       92 2023-06-14 11:09:16.000000 spatial-moto-0.0.2/spatial_moto.egg-info/requires.txt
--rwxrwxrwx   0 walido    (1000) walido    (1000)       12 2023-06-14 11:09:16.000000 spatial-moto-0.0.2/spatial_moto.egg-info/top_level.txt
-drwxrwxrwx   0 walido    (1000) walido    (1000)        0 2023-06-14 11:09:16.983274 spatial-moto-0.0.2/spatialmoto/
--rwxrwxrwx   0 walido    (1000) walido    (1000)      211 2023-06-14 09:48:03.000000 spatial-moto-0.0.2/spatialmoto/__init__.py
--rwxrwxrwx   0 walido    (1000) walido    (1000)     4990 2023-06-14 09:33:34.000000 spatial-moto-0.0.2/spatialmoto/blocks.py
--rwxrwxrwx   0 walido    (1000) walido    (1000)     2385 2023-06-14 09:31:33.000000 spatial-moto-0.0.2/spatialmoto/clusters.py
-drwxrwxrwx   0 walido    (1000) walido    (1000)        0 2023-06-14 11:09:16.985114 spatial-moto-0.0.2/spatialmoto/data/
--rwxrwxrwx   0 walido    (1000) walido    (1000)  5186120 2023-06-14 09:31:33.000000 spatial-moto-0.0.2/spatialmoto/data/ames.geojson
--rwxrwxrwx   0 walido    (1000) walido    (1000)      225 2023-06-14 10:54:39.000000 spatial-moto-0.0.2/spatialmoto/datasets.py
--rwxrwxrwx   0 walido    (1000) walido    (1000)     2263 2023-06-14 09:31:33.000000 spatial-moto-0.0.2/spatialmoto/plotting.py
--rwxrwxrwx   0 walido    (1000) walido    (1000)     1942 2023-06-14 09:31:33.000000 spatial-moto-0.0.2/spatialmoto/stats.py
+drwxrwxrwx   0 walido    (1000) walido    (1000)        0 2023-06-14 11:19:45.745050 spatial-moto-0.0.3/
+-rwxrwxrwx   0 walido    (1000) walido    (1000)     1071 2023-06-14 09:31:33.000000 spatial-moto-0.0.3/LICENSE
+-rwxrwxrwx   0 walido    (1000) walido    (1000)      669 2023-06-14 11:19:45.744512 spatial-moto-0.0.3/PKG-INFO
+-rwxrwxrwx   0 walido    (1000) walido    (1000)     1114 2023-06-14 11:06:59.000000 spatial-moto-0.0.3/README.md
+-rwxrwxrwx   0 walido    (1000) walido    (1000)       38 2023-06-14 11:19:45.745972 spatial-moto-0.0.3/setup.cfg
+-rwxrwxrwx   0 walido    (1000) walido    (1000)     1306 2023-06-14 11:19:22.000000 spatial-moto-0.0.3/setup.py
+drwxrwxrwx   0 walido    (1000) walido    (1000)        0 2023-06-14 11:19:45.572112 spatial-moto-0.0.3/spatial_moto.egg-info/
+-rwxrwxrwx   0 walido    (1000) walido    (1000)      669 2023-06-14 11:19:45.000000 spatial-moto-0.0.3/spatial_moto.egg-info/PKG-INFO
+-rwxrwxrwx   0 walido    (1000) walido    (1000)      374 2023-06-14 11:19:45.000000 spatial-moto-0.0.3/spatial_moto.egg-info/SOURCES.txt
+-rwxrwxrwx   0 walido    (1000) walido    (1000)        1 2023-06-14 11:19:45.000000 spatial-moto-0.0.3/spatial_moto.egg-info/dependency_links.txt
+-rwxrwxrwx   0 walido    (1000) walido    (1000)       92 2023-06-14 11:19:45.000000 spatial-moto-0.0.3/spatial_moto.egg-info/requires.txt
+-rwxrwxrwx   0 walido    (1000) walido    (1000)       12 2023-06-14 11:19:45.000000 spatial-moto-0.0.3/spatial_moto.egg-info/top_level.txt
+drwxrwxrwx   0 walido    (1000) walido    (1000)        0 2023-06-14 11:19:45.586846 spatial-moto-0.0.3/spatialmoto/
+-rwxrwxrwx   0 walido    (1000) walido    (1000)      211 2023-06-14 09:48:03.000000 spatial-moto-0.0.3/spatialmoto/__init__.py
+-rwxrwxrwx   0 walido    (1000) walido    (1000)     4990 2023-06-14 09:33:34.000000 spatial-moto-0.0.3/spatialmoto/blocks.py
+-rwxrwxrwx   0 walido    (1000) walido    (1000)     2385 2023-06-14 09:31:33.000000 spatial-moto-0.0.3/spatialmoto/clusters.py
+drwxrwxrwx   0 walido    (1000) walido    (1000)        0 2023-06-14 11:19:45.588667 spatial-moto-0.0.3/spatialmoto/data/
+-rwxrwxrwx   0 walido    (1000) walido    (1000)  5186120 2023-06-14 09:31:33.000000 spatial-moto-0.0.3/spatialmoto/data/ames.geojson
+-rwxrwxrwx   0 walido    (1000) walido    (1000)      225 2023-06-14 10:54:39.000000 spatial-moto-0.0.3/spatialmoto/datasets.py
+-rwxrwxrwx   0 walido    (1000) walido    (1000)     2263 2023-06-14 09:31:33.000000 spatial-moto-0.0.3/spatialmoto/plotting.py
+-rwxrwxrwx   0 walido    (1000) walido    (1000)     1942 2023-06-14 09:31:33.000000 spatial-moto-0.0.3/spatialmoto/stats.py
```

### Comparing `spatial-moto-0.0.2/LICENSE` & `spatial-moto-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spatial-moto-0.0.2/PKG-INFO` & `spatial-moto-0.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatial-moto
-Version: 0.0.2
+Version: 0.0.3
 Summary: spatial-moto: test 1
 Home-page: https://github.com/WalidGharianiEAGLE/spatial-moto
 License: MIT
 Keywords: spatial
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `spatial-moto-0.0.2/README.md` & `spatial-moto-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `spatial-moto-0.0.2/setup.py` & `spatial-moto-0.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # Dependencies
 with open('requirements.txt') as f:
     requirements = f.readlines()
 
 setup(
     name='spatial-moto',
-    version="0.0.02",
+    version="0.0.03",
     packages=["spatialmoto"],
     description=("spatial-moto: test 1"),
     #long_description=README,
     license="MIT",
     keywords="spatial",
     url="https://github.com/WalidGharianiEAGLE/spatial-moto",
```

### Comparing `spatial-moto-0.0.2/spatial_moto.egg-info/PKG-INFO` & `spatial-moto-0.0.3/spatial_moto.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatial-moto
-Version: 0.0.2
+Version: 0.0.3
 Summary: spatial-moto: test 1
 Home-page: https://github.com/WalidGharianiEAGLE/spatial-moto
 License: MIT
 Keywords: spatial
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `spatial-moto-0.0.2/spatialmoto/blocks.py` & `spatial-moto-0.0.3/spatialmoto/blocks.py`

 * *Files identical despite different names*

### Comparing `spatial-moto-0.0.2/spatialmoto/clusters.py` & `spatial-moto-0.0.3/spatialmoto/clusters.py`

 * *Files identical despite different names*

### Comparing `spatial-moto-0.0.2/spatialmoto/data/ames.geojson` & `spatial-moto-0.0.3/spatialmoto/data/ames.geojson`

 * *Files identical despite different names*

### Comparing `spatial-moto-0.0.2/spatialmoto/plotting.py` & `spatial-moto-0.0.3/spatialmoto/plotting.py`

 * *Files identical despite different names*

### Comparing `spatial-moto-0.0.2/spatialmoto/stats.py` & `spatial-moto-0.0.3/spatialmoto/stats.py`

 * *Files identical despite different names*

