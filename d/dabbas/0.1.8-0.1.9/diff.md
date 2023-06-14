# Comparing `tmp/dabbas-0.1.8.tar.gz` & `tmp/dabbas-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dabbas-0.1.8.tar", last modified: Mon May 15 11:30:57 2023, max compression
+gzip compressed data, was "dabbas-0.1.9.tar", last modified: Mon May 15 11:45:41 2023, max compression
```

## Comparing `dabbas-0.1.8.tar` & `dabbas-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 nikhilsaraf   (501) staff       (20)        0 2023-05-15 11:30:57.773878 dabbas-0.1.8/
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)      393 2023-05-15 11:30:57.773591 dabbas-0.1.8/PKG-INFO
-drwxr-xr-x   0 nikhilsaraf   (501) staff       (20)        0 2023-05-15 11:30:57.770791 dabbas-0.1.8/atlas/
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)       21 2023-04-23 17:17:29.000000 dabbas-0.1.8/atlas/__init__.py
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)     6280 2023-04-24 17:54:58.000000 dabbas-0.1.8/atlas/atlas.py
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)     8113 2023-04-24 09:22:52.000000 dabbas-0.1.8/atlas/boundary.py
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)     1479 2023-05-15 11:11:09.000000 dabbas-0.1.8/atlas/db.py
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)     2793 2023-04-23 19:43:28.000000 dabbas-0.1.8/atlas/schema.py
-drwxr-xr-x   0 nikhilsaraf   (501) staff       (20)        0 2023-05-15 11:30:57.772006 dabbas-0.1.8/dabbas/
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)      134 2023-04-19 15:30:00.000000 dabbas-0.1.8/dabbas/__init__.py
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)     2399 2023-04-19 03:44:35.000000 dabbas-0.1.8/dabbas/cache.py
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)     1294 2023-05-15 11:00:11.000000 dabbas-0.1.8/dabbas/connection.py
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)     2748 2023-04-19 15:29:41.000000 dabbas-0.1.8/dabbas/main.py
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)     5376 2023-05-15 11:10:48.000000 dabbas-0.1.8/dabbas/map.py
-drwxr-xr-x   0 nikhilsaraf   (501) staff       (20)        0 2023-05-15 11:30:57.773322 dabbas-0.1.8/dabbas.egg-info/
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)      393 2023-05-15 11:30:57.000000 dabbas-0.1.8/dabbas.egg-info/PKG-INFO
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)      354 2023-05-15 11:30:57.000000 dabbas-0.1.8/dabbas.egg-info/SOURCES.txt
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)        1 2023-05-15 11:30:57.000000 dabbas-0.1.8/dabbas.egg-info/dependency_links.txt
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)       58 2023-05-15 11:30:57.000000 dabbas-0.1.8/dabbas.egg-info/entry_points.txt
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)      101 2023-05-15 11:30:57.000000 dabbas-0.1.8/dabbas.egg-info/requires.txt
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)       13 2023-05-15 11:30:57.000000 dabbas-0.1.8/dabbas.egg-info/top_level.txt
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)       38 2023-05-15 11:30:57.773927 dabbas-0.1.8/setup.cfg
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)      895 2023-05-15 11:30:57.000000 dabbas-0.1.8/setup.py
+drwxr-xr-x   0 nikhilsaraf   (501) staff       (20)        0 2023-05-15 11:45:41.931469 dabbas-0.1.9/
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)      393 2023-05-15 11:45:41.931043 dabbas-0.1.9/PKG-INFO
+drwxr-xr-x   0 nikhilsaraf   (501) staff       (20)        0 2023-05-15 11:45:41.926041 dabbas-0.1.9/atlas/
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)       21 2023-04-23 17:17:29.000000 dabbas-0.1.9/atlas/__init__.py
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)     6280 2023-04-24 17:54:58.000000 dabbas-0.1.9/atlas/atlas.py
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)     8113 2023-04-24 09:22:52.000000 dabbas-0.1.9/atlas/boundary.py
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)     1479 2023-05-15 11:11:09.000000 dabbas-0.1.9/atlas/db.py
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)     2793 2023-04-23 19:43:28.000000 dabbas-0.1.9/atlas/schema.py
+drwxr-xr-x   0 nikhilsaraf   (501) staff       (20)        0 2023-05-15 11:45:41.927598 dabbas-0.1.9/dabbas/
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)      134 2023-04-19 15:30:00.000000 dabbas-0.1.9/dabbas/__init__.py
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)     2399 2023-04-19 03:44:35.000000 dabbas-0.1.9/dabbas/cache.py
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)     1294 2023-05-15 11:00:11.000000 dabbas-0.1.9/dabbas/connection.py
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)     2748 2023-04-19 15:29:41.000000 dabbas-0.1.9/dabbas/main.py
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)     5408 2023-05-15 11:43:46.000000 dabbas-0.1.9/dabbas/map.py
+drwxr-xr-x   0 nikhilsaraf   (501) staff       (20)        0 2023-05-15 11:45:41.930666 dabbas-0.1.9/dabbas.egg-info/
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)      393 2023-05-15 11:45:41.000000 dabbas-0.1.9/dabbas.egg-info/PKG-INFO
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)      354 2023-05-15 11:45:41.000000 dabbas-0.1.9/dabbas.egg-info/SOURCES.txt
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)        1 2023-05-15 11:45:41.000000 dabbas-0.1.9/dabbas.egg-info/dependency_links.txt
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)       58 2023-05-15 11:45:41.000000 dabbas-0.1.9/dabbas.egg-info/entry_points.txt
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)      101 2023-05-15 11:45:41.000000 dabbas-0.1.9/dabbas.egg-info/requires.txt
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)       13 2023-05-15 11:45:41.000000 dabbas-0.1.9/dabbas.egg-info/top_level.txt
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)       38 2023-05-15 11:45:41.931540 dabbas-0.1.9/setup.cfg
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)      895 2023-05-15 11:45:36.000000 dabbas-0.1.9/setup.py
```

### Comparing `dabbas-0.1.8/atlas/atlas.py` & `dabbas-0.1.9/atlas/atlas.py`

 * *Files identical despite different names*

### Comparing `dabbas-0.1.8/atlas/boundary.py` & `dabbas-0.1.9/atlas/boundary.py`

 * *Files identical despite different names*

### Comparing `dabbas-0.1.8/atlas/db.py` & `dabbas-0.1.9/atlas/db.py`

 * *Files identical despite different names*

### Comparing `dabbas-0.1.8/atlas/schema.py` & `dabbas-0.1.9/atlas/schema.py`

 * *Files identical despite different names*

### Comparing `dabbas-0.1.8/dabbas/cache.py` & `dabbas-0.1.9/dabbas/cache.py`

 * *Files identical despite different names*

### Comparing `dabbas-0.1.8/dabbas/connection.py` & `dabbas-0.1.9/dabbas/connection.py`

 * *Files identical despite different names*

### Comparing `dabbas-0.1.8/dabbas/main.py` & `dabbas-0.1.9/dabbas/main.py`

 * *Files identical despite different names*

### Comparing `dabbas-0.1.8/dabbas/map.py` & `dabbas-0.1.9/dabbas/map.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         print(e)
         return csv
 
 
 T = TypeVar('T')
 
 
-def read_sql(sql, con=connection_url(), latitude='latitude', longitude='longitude', geometry=['geometry', 'geom'], format='', **kwargs) -> gpd.GeoDataFrame:
+def read_sql(sql, con=connection_url(), latitude='latitude', longitude='longitude', geometry=['geometry', 'geom', 'wkb_geometry'], format='', **kwargs) -> gpd.GeoDataFrame:
     cols, results = query(sql)
     sql = pd.DataFrame(results, columns=[col[0] for col in cols])
     try:
         return sql.geo(latitude=latitude, longitude=longitude, geometry=geometry, format=format, **kwargs)
     except Exception as e:
         print(e)
         return sql
@@ -73,15 +73,15 @@
     'geojson': shape,
     'wkt': wkt.loads,
     'wkb': wkb.loads,
     '': parse_geometry
 }
 
 
-def create_geometry_column(df: pd.DataFrame, format='', geometry=['geometry', 'geom'], latitude='latitude', longitude='longitude'):
+def create_geometry_column(df: pd.DataFrame, format='', geometry=['geometry', 'geom', 'wkb_geometry'], latitude='latitude', longitude='longitude'):
     df = df.copy()
     if len(df) == 0:
         raise Exception('No data in Dataset to create geometry')
 
     if type(geometry) == str and geometry in df:
         if format in format_map:
             df.loc[:, 'geometry'] = df.loc[:,
```

### Comparing `dabbas-0.1.8/setup.py` & `dabbas-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dabbas",
-    version="0.1.8",
+    version="0.1.9",
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "db = db.main:main",
             "dabbas = db.main:main",
         ],
     },
```

