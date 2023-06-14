# Comparing `tmp/rpcm-1.4.8.tar.gz` & `tmp/rpcm-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpcm-1.4.8.tar", last modified: Tue Jan 31 11:24:42 2023, max compression
+gzip compressed data, was "rpcm-1.4.9.tar", last modified: Wed Jun 14 07:08:29 2023, max compression
```

## Comparing `rpcm-1.4.8.tar` & `rpcm-1.4.9.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 carlo      (501) staff       (20)        0 2023-01-31 11:24:42.218523 rpcm-1.4.8/
--rw-r--r--   0 carlo      (501) staff       (20)     1324 2021-12-02 22:08:27.000000 rpcm-1.4.8/LICENSE
--rw-r--r--   0 carlo      (501) staff       (20)     4617 2023-01-31 11:24:42.218129 rpcm-1.4.8/PKG-INFO
--rw-r--r--   0 carlo      (501) staff       (20)     4228 2021-12-02 22:41:41.000000 rpcm-1.4.8/README.md
-drwxr-xr-x   0 carlo      (501) staff       (20)        0 2023-01-31 11:24:42.214763 rpcm-1.4.8/rpcm/
--rw-r--r--   0 carlo      (501) staff       (20)      266 2023-01-31 11:23:39.000000 rpcm-1.4.8/rpcm/__about__.py
--rw-r--r--   0 carlo      (501) staff       (20)     7365 2022-03-09 16:47:27.000000 rpcm-1.4.8/rpcm/__init__.py
--rw-r--r--   0 carlo      (501) staff       (20)       33 2022-07-27 17:26:09.000000 rpcm-1.4.8/rpcm/__main__.py
--rw-r--r--   0 carlo      (501) staff       (20)     6786 2020-08-06 17:59:35.000000 rpcm-1.4.8/rpcm/cli.py
--rw-r--r--   0 carlo      (501) staff       (20)      611 2019-07-22 21:23:59.000000 rpcm-1.4.8/rpcm/geo.py
--rw-r--r--   0 carlo      (501) staff       (20)    10146 2022-07-06 20:18:09.000000 rpcm-1.4.8/rpcm/rpc_file_readers.py
--rw-r--r--   0 carlo      (501) staff       (20)    18715 2022-08-11 13:46:25.000000 rpcm-1.4.8/rpcm/rpc_model.py
--rw-r--r--   0 carlo      (501) staff       (20)     4898 2022-03-28 15:22:18.000000 rpcm-1.4.8/rpcm/utils.py
-drwxr-xr-x   0 carlo      (501) staff       (20)        0 2023-01-31 11:24:42.217433 rpcm-1.4.8/rpcm.egg-info/
--rw-r--r--   0 carlo      (501) staff       (20)     4617 2023-01-31 11:24:41.000000 rpcm-1.4.8/rpcm.egg-info/PKG-INFO
--rw-r--r--   0 carlo      (501) staff       (20)      329 2023-01-31 11:24:41.000000 rpcm-1.4.8/rpcm.egg-info/SOURCES.txt
--rw-r--r--   0 carlo      (501) staff       (20)        1 2023-01-31 11:24:41.000000 rpcm-1.4.8/rpcm.egg-info/dependency_links.txt
--rw-r--r--   0 carlo      (501) staff       (20)       64 2023-01-31 11:24:41.000000 rpcm-1.4.8/rpcm.egg-info/entry_points.txt
--rw-r--r--   0 carlo      (501) staff       (20)       67 2023-01-31 11:24:41.000000 rpcm-1.4.8/rpcm.egg-info/requires.txt
--rw-r--r--   0 carlo      (501) staff       (20)        5 2023-01-31 11:24:41.000000 rpcm-1.4.8/rpcm.egg-info/top_level.txt
--rw-r--r--   0 carlo      (501) staff       (20)       38 2023-01-31 11:24:42.218672 rpcm-1.4.8/setup.cfg
--rw-r--r--   0 carlo      (501) staff       (20)     1065 2022-03-28 15:23:38.000000 rpcm-1.4.8/setup.py
+drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-14 07:08:29.715392 rpcm-1.4.9/
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1324 2023-01-30 17:42:28.000000 rpcm-1.4.9/LICENSE
+-rw-rw-r--   0 coco      (1000) coco      (1000)     4617 2023-06-14 07:08:29.715392 rpcm-1.4.9/PKG-INFO
+-rw-rw-r--   0 coco      (1000) coco      (1000)     4228 2023-01-30 17:42:28.000000 rpcm-1.4.9/README.md
+drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-14 07:08:29.715392 rpcm-1.4.9/rpcm/
+-rw-rw-r--   0 coco      (1000) coco      (1000)      266 2023-06-14 07:06:48.000000 rpcm-1.4.9/rpcm/__about__.py
+-rw-rw-r--   0 coco      (1000) coco      (1000)     7365 2023-01-30 17:42:28.000000 rpcm-1.4.9/rpcm/__init__.py
+-rw-rw-r--   0 coco      (1000) coco      (1000)     6786 2023-01-30 17:42:28.000000 rpcm-1.4.9/rpcm/cli.py
+-rw-rw-r--   0 coco      (1000) coco      (1000)      611 2019-07-23 10:29:39.000000 rpcm-1.4.9/rpcm/geo.py
+-rw-rw-r--   0 coco      (1000) coco      (1000)    10569 2023-06-14 07:04:35.000000 rpcm-1.4.9/rpcm/rpc_file_readers.py
+-rw-rw-r--   0 coco      (1000) coco      (1000)    17982 2023-01-30 17:42:28.000000 rpcm-1.4.9/rpcm/rpc_model.py
+-rw-rw-r--   0 coco      (1000) coco      (1000)     4898 2023-01-30 17:42:28.000000 rpcm-1.4.9/rpcm/utils.py
+drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-06-14 07:08:29.715392 rpcm-1.4.9/rpcm.egg-info/
+-rw-rw-r--   0 coco      (1000) coco      (1000)     4617 2023-06-14 07:08:29.000000 rpcm-1.4.9/rpcm.egg-info/PKG-INFO
+-rw-rw-r--   0 coco      (1000) coco      (1000)      312 2023-06-14 07:08:29.000000 rpcm-1.4.9/rpcm.egg-info/SOURCES.txt
+-rw-rw-r--   0 coco      (1000) coco      (1000)        1 2023-06-14 07:08:29.000000 rpcm-1.4.9/rpcm.egg-info/dependency_links.txt
+-rw-rw-r--   0 coco      (1000) coco      (1000)       64 2023-06-14 07:08:29.000000 rpcm-1.4.9/rpcm.egg-info/entry_points.txt
+-rw-rw-r--   0 coco      (1000) coco      (1000)       67 2023-06-14 07:08:29.000000 rpcm-1.4.9/rpcm.egg-info/requires.txt
+-rw-rw-r--   0 coco      (1000) coco      (1000)        5 2023-06-14 07:08:29.000000 rpcm-1.4.9/rpcm.egg-info/top_level.txt
+-rw-rw-r--   0 coco      (1000) coco      (1000)       38 2023-06-14 07:08:29.715392 rpcm-1.4.9/setup.cfg
+-rw-rw-r--   0 coco      (1000) coco      (1000)     1065 2023-01-30 17:42:28.000000 rpcm-1.4.9/setup.py
```

### Comparing `rpcm-1.4.8/LICENSE` & `rpcm-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rpcm-1.4.8/PKG-INFO` & `rpcm-1.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpcm
-Version: 1.4.8
+Version: 1.4.9
 Summary: Rational Polynomial Camera Model for optical satellite images.
 Home-page: https://github.com/centreborelli/rpcm
 Author: Carlo de Franchis
 Author-email: carlo.de-franchis@ens-paris-saclay.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3
```

### Comparing `rpcm-1.4.8/README.md` & `rpcm-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `rpcm-1.4.8/rpcm/__init__.py` & `rpcm-1.4.9/rpcm/__init__.py`

 * *Files identical despite different names*

### Comparing `rpcm-1.4.8/rpcm/cli.py` & `rpcm-1.4.9/rpcm/cli.py`

 * *Files identical despite different names*

### Comparing `rpcm-1.4.8/rpcm/geo.py` & `rpcm-1.4.9/rpcm/geo.py`

 * *Files identical despite different names*

### Comparing `rpcm-1.4.8/rpcm/rpc_file_readers.py` & `rpcm-1.4.9/rpcm/rpc_file_readers.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,14 +62,21 @@
         return ' '.join([dic["%s_%s" % (prefix, str(x))] for x in indices])
 
     d['SAMP_NUM_COEFF']  = parse_coeff(d, "SAMP_NUM_COEFF", range(1, 21))
     d['SAMP_DEN_COEFF']  = parse_coeff(d, "SAMP_DEN_COEFF", range(1, 21))
     d['LINE_NUM_COEFF']  = parse_coeff(d, "LINE_NUM_COEFF", range(1, 21))
     d['LINE_DEN_COEFF']  = parse_coeff(d, "LINE_DEN_COEFF", range(1, 21))
 
+    # if the LON/LAT coefficients are present then it must be an "extended ikonos"
+    if 'LON_NUM_COEFF_1' in d:
+        d['LON_NUM_COEFF']  = parse_coeff(d, "LON_NUM_COEFF", range(1, 21))
+        d['LON_DEN_COEFF']  = parse_coeff(d, "LON_DEN_COEFF", range(1, 21))
+        d['LAT_NUM_COEFF']   = parse_coeff(d, "LAT_NUM_COEFF" , range(1, 21))
+        d['LAT_DEN_COEFF']   = parse_coeff(d, "LAT_DEN_COEFF" , range(1, 21))
+
     return d
 
 
 
 def read_rpc_xml(rpc_content):
     """
     Read RPC file assuming the XML format and determine whether it's a pleiades, spot-6 or worldview image
```

### Comparing `rpcm-1.4.8/rpcm/rpc_model.py` & `rpcm-1.4.9/rpcm/rpc_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -307,28 +307,14 @@
         # azimuth is the clockwise angle with respect to the North
         # of the projection of the satellite direction on the horizontal plane
         # This can be computed by taking the argument of a complex number
         # in a coordinate system where northing is the x axis and easting the y axis
         easting, northing = satellite_direction[:2]
         azimuth = np.degrees(np.angle(complex(northing, easting)))
 
-        # convert azimuth from ]-180, +180] to [0, 360[
-        azimuth = azimuth % 360
-
-        # TODO Don't convert to UTM but stay in ECEF. Vertical direction in UTM is not accurate!
-        transformer = pyproj.Transformer.from_crs(4326, 4978, always_xy=True)
-        [x0, x1], [y0, y1], [z0, z1] = transformer.transform([lon0, lon1], [lat0, lat1], [z + 0*s, z + 1*s])
-        p0 = np.array([x0, y0, z0])
-        p1 = np.array([x1, y1, z1])
-        satellite_direction = (p1 - p0) / np.linalg.norm(p1 - p0)
-        vertical_direction = p0 / np.linalg.norm(p0)
-
-        # zenith is the angle between the satellite direction and the vertical
-        zenith = np.degrees(np.arccos(np.dot(satellite_direction, vertical_direction)))
-
         return zenith, azimuth
 
 
     def __repr__(self):
         return """
     # Projection function coefficients
       col_num = {}
```

### Comparing `rpcm-1.4.8/rpcm/utils.py` & `rpcm-1.4.9/rpcm/utils.py`

 * *Files identical despite different names*

### Comparing `rpcm-1.4.8/rpcm.egg-info/PKG-INFO` & `rpcm-1.4.9/rpcm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpcm
-Version: 1.4.8
+Version: 1.4.9
 Summary: Rational Polynomial Camera Model for optical satellite images.
 Home-page: https://github.com/centreborelli/rpcm
 Author: Carlo de Franchis
 Author-email: carlo.de-franchis@ens-paris-saclay.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3
```

### Comparing `rpcm-1.4.8/setup.py` & `rpcm-1.4.9/setup.py`

 * *Files identical despite different names*

