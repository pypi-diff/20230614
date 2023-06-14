# Comparing `tmp/here_geocoding-0.2.0.tar.gz` & `tmp/here_geocoding-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "here_geocoding-0.2.0.tar", last modified: Fri Jun  9 08:49:56 2023, max compression
+gzip compressed data, was "here_geocoding-0.3.0.tar", last modified: Wed Jun 14 14:46:29 2023, max compression
```

## Comparing `here_geocoding-0.2.0.tar` & `here_geocoding-0.3.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 08:49:56.632655 here_geocoding-0.2.0/
--rw-rw-rw-   0        0        0      176 2023-06-09 07:40:11.000000 here_geocoding-0.2.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3739 2023-06-09 07:40:11.000000 here_geocoding-0.2.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-06-09 07:40:11.000000 here_geocoding-0.2.0/HISTORY.rst
--rw-rw-rw-   0        0        0     1099 2023-06-09 07:40:11.000000 here_geocoding-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      273 2023-06-09 07:40:11.000000 here_geocoding-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4083 2023-06-09 08:49:56.632838 here_geocoding-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2890 2023-06-09 08:10:51.000000 here_geocoding-0.2.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-09 08:49:56.508283 here_geocoding-0.2.0/docs/
--rw-rw-rw-   0        0        0      635 2023-06-09 07:40:11.000000 here_geocoding-0.2.0/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-06-09 07:40:11.000000 here_geocoding-0.2.0/docs/authors.rst
--rw-rw-rw-   0        0        0     5049 2023-06-09 07:40:11.000000 here_geocoding-0.2.0/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-06-09 07:40:11.000000 here_geocoding-0.2.0/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-06-09 07:40:11.000000 here_geocoding-0.2.0/docs/history.rst
--rw-rw-rw-   0        0        0      331 2023-06-09 07:40:11.000000 here_geocoding-0.2.0/docs/index.rst
--rw-rw-rw-   0        0        0     1225 2023-06-09 07:40:11.000000 here_geocoding-0.2.0/docs/installation.rst
--rwxrwxrwx   0        0        0      812 2023-06-09 07:40:11.000000 here_geocoding-0.2.0/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-06-09 07:40:11.000000 here_geocoding-0.2.0/docs/readme.rst
--rw-rw-rw-   0        0        0       90 2023-06-09 07:40:11.000000 here_geocoding-0.2.0/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-06-09 08:49:56.548282 here_geocoding-0.2.0/here_geocoding/
--rw-rw-rw-   0        0        0      180 2023-06-09 07:44:37.000000 here_geocoding-0.2.0/here_geocoding/__init__.py
--rw-rw-rw-   0        0        0      436 2023-06-09 07:40:11.000000 here_geocoding-0.2.0/here_geocoding/cli.py
--rw-rw-rw-   0        0        0     3480 2023-06-09 07:48:31.000000 here_geocoding-0.2.0/here_geocoding/here_geocoding.py
-drwxrwxrwx   0        0        0        0 2023-06-09 08:49:56.598396 here_geocoding-0.2.0/here_geocoding.egg-info/
--rw-rw-rw-   0        0        0     4083 2023-06-09 08:49:56.000000 here_geocoding-0.2.0/here_geocoding.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      695 2023-06-09 08:49:56.000000 here_geocoding-0.2.0/here_geocoding.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 08:49:56.000000 here_geocoding-0.2.0/here_geocoding.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-06-09 08:49:56.000000 here_geocoding-0.2.0/here_geocoding.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-09 08:49:56.000000 here_geocoding-0.2.0/here_geocoding.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       55 2023-06-09 08:49:56.000000 here_geocoding-0.2.0/here_geocoding.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-09 08:49:56.000000 here_geocoding-0.2.0/here_geocoding.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      409 2023-06-09 08:49:56.634871 here_geocoding-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1857 2023-06-09 08:48:49.000000 here_geocoding-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 08:49:56.627635 here_geocoding-0.2.0/tests/
--rw-rw-rw-   0        0        0       45 2023-06-09 07:40:11.000000 here_geocoding-0.2.0/tests/__init__.py
--rw-rw-rw-   0        0        0    14059 2023-06-09 07:15:05.000000 here_geocoding-0.2.0/tests/address-sample.xlsx
--rw-rw-rw-   0        0        0     1141 2023-06-09 07:48:43.000000 here_geocoding-0.2.0/tests/examples.py
--rw-rw-rw-   0        0        0      934 2023-06-09 07:40:11.000000 here_geocoding-0.2.0/tests/test_here_geocoding.py
+drwxrwxrwx   0        0        0        0 2023-06-14 14:46:29.698233 here_geocoding-0.3.0/
+-rw-rw-rw-   0        0        0      176 2023-06-09 07:40:11.000000 here_geocoding-0.3.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3739 2023-06-09 07:40:11.000000 here_geocoding-0.3.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-06-09 07:40:11.000000 here_geocoding-0.3.0/HISTORY.rst
+-rw-rw-rw-   0        0        0     1099 2023-06-09 07:40:11.000000 here_geocoding-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-06-09 07:40:11.000000 here_geocoding-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4083 2023-06-14 14:46:29.699350 here_geocoding-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2890 2023-06-09 08:10:51.000000 here_geocoding-0.3.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-14 14:46:29.582171 here_geocoding-0.3.0/docs/
+-rw-rw-rw-   0        0        0      635 2023-06-09 07:40:11.000000 here_geocoding-0.3.0/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-06-09 07:40:11.000000 here_geocoding-0.3.0/docs/authors.rst
+-rw-rw-rw-   0        0        0     5049 2023-06-09 07:40:11.000000 here_geocoding-0.3.0/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-06-09 07:40:11.000000 here_geocoding-0.3.0/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-06-09 07:40:11.000000 here_geocoding-0.3.0/docs/history.rst
+-rw-rw-rw-   0        0        0      331 2023-06-09 07:40:11.000000 here_geocoding-0.3.0/docs/index.rst
+-rw-rw-rw-   0        0        0     1225 2023-06-09 07:40:11.000000 here_geocoding-0.3.0/docs/installation.rst
+-rwxrwxrwx   0        0        0      812 2023-06-09 07:40:11.000000 here_geocoding-0.3.0/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-06-09 07:40:11.000000 here_geocoding-0.3.0/docs/readme.rst
+-rw-rw-rw-   0        0        0       90 2023-06-09 07:40:11.000000 here_geocoding-0.3.0/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2023-06-14 14:46:29.597545 here_geocoding-0.3.0/here_geocoding/
+-rw-rw-rw-   0        0        0      180 2023-06-14 14:00:10.000000 here_geocoding-0.3.0/here_geocoding/__init__.py
+-rw-rw-rw-   0        0        0      436 2023-06-09 07:40:11.000000 here_geocoding-0.3.0/here_geocoding/cli.py
+-rw-rw-rw-   0        0        0     3846 2023-06-14 14:27:08.000000 here_geocoding-0.3.0/here_geocoding/here_geocoding.py
+drwxrwxrwx   0        0        0        0 2023-06-14 14:46:29.647123 here_geocoding-0.3.0/here_geocoding.egg-info/
+-rw-rw-rw-   0        0        0     4083 2023-06-14 14:46:28.000000 here_geocoding-0.3.0/here_geocoding.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      695 2023-06-14 14:46:29.000000 here_geocoding-0.3.0/here_geocoding.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 14:46:28.000000 here_geocoding-0.3.0/here_geocoding.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-14 14:46:28.000000 here_geocoding-0.3.0/here_geocoding.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-14 14:46:28.000000 here_geocoding-0.3.0/here_geocoding.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       55 2023-06-14 14:46:28.000000 here_geocoding-0.3.0/here_geocoding.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-14 14:46:28.000000 here_geocoding-0.3.0/here_geocoding.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      409 2023-06-14 14:46:29.710333 here_geocoding-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1857 2023-06-14 13:50:49.000000 here_geocoding-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 14:46:29.696736 here_geocoding-0.3.0/tests/
+-rw-rw-rw-   0        0        0       45 2023-06-09 07:40:11.000000 here_geocoding-0.3.0/tests/__init__.py
+-rw-rw-rw-   0        0        0    14059 2023-06-09 07:15:05.000000 here_geocoding-0.3.0/tests/address-sample.xlsx
+-rw-rw-rw-   0        0        0     1141 2023-06-09 07:48:43.000000 here_geocoding-0.3.0/tests/examples.py
+-rw-rw-rw-   0        0        0      934 2023-06-09 07:40:11.000000 here_geocoding-0.3.0/tests/test_here_geocoding.py
```

### Comparing `here_geocoding-0.2.0/CONTRIBUTING.rst` & `here_geocoding-0.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `here_geocoding-0.2.0/LICENSE` & `here_geocoding-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `here_geocoding-0.2.0/PKG-INFO` & `here_geocoding-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: here_geocoding
-Version: 0.2.0
+Version: 0.3.0
 Summary: The "here-geocoding" package is a Python library designed to streamline the process of converting addresses stored in an Excel (xlsx) file into latitude and longitude coordinates. It provides a convenient solution for geocoding large sets of addresses using the HERE geocoding service.
 Home-page: https://github.com/Mariosmsk/here_geocoding
 Author: Marios S. Kyriakou
 Author-email: mariosmsk@gmail.com
 License: MIT license
 Keywords: here_geocoding
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `here_geocoding-0.2.0/README.rst` & `here_geocoding-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `here_geocoding-0.2.0/docs/Makefile` & `here_geocoding-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `here_geocoding-0.2.0/docs/conf.py` & `here_geocoding-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `here_geocoding-0.2.0/docs/installation.rst` & `here_geocoding-0.3.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `here_geocoding-0.2.0/docs/make.bat` & `here_geocoding-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `here_geocoding-0.2.0/here_geocoding/here_geocoding.py` & `here_geocoding-0.3.0/here_geocoding/here_geocoding.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Main module."""
+import time
 import requests
 import pyproj  # 2.6.1post1
 import random
 import pandas as pd
 import urllib
 import json
 import os
@@ -18,18 +19,19 @@
         except:
             print('Use your api key: https://platform.here.com/admin/apps/')
 
     def address_to_lnglat(self, address=None, bbox=None, to_crs=None, geojson=False):
         if address is None:
             return False
         try:
+            x, y = 0, 0
             if bbox is None:
-                geo = self.ls.geocode(query=address)
+                geo = self.ls.geocode(query=address.rstrip())
             else:
-                geo = self.ls.autosuggest(query=address, search_in_bbox=bbox)
+                geo = self.ls.autosuggest(query=address.rstrip(), search_in_bbox=bbox)
             data_json = json.dumps(geo.to_geojson(), indent=2, sort_keys=True)
             data = json.loads(data_json)
             try:
                 lat = data['features'][0]['properties']['access'][0]['lat']
                 lng = data['features'][0]['properties']['access'][0]['lng']
             except:
                 try:
@@ -48,54 +50,56 @@
         if geojson:
             data = geo.to_geojson()
             return [data]
 
         return y, x
 
     def geocode_excel(self, file_path='', start_row=-1, end_row=None, address_column=None, bbox=None, to_crs=None,
-                      export_file_name='test', export_file_type='csv'):
+                      export_file_name='test', export_file_type='csv', showprint=True, create_continue=False, pause=0.01):
 
         df = pd.read_excel(file_path)
         if end_row is None:
             end_row = df[address_column].__len__()
 
         latlng = []
+        all_col_keys = list(df.keys())
+        all_col_keys.extend(['lat', 'lng'])
         for i, address in enumerate(df[address_column]):
+            if showprint:
+                print(i)
             if end_row < i:
                 break
             if i > start_row:
-                x, y = self.address_to_lnglat(address=address, bbox=bbox, to_crs=to_crs)
+                x, y = self.address_to_lnglat(address=address.rstrip(), bbox=bbox, to_crs=to_crs)
                 all_col_values = list(df.iloc[i, :])
                 all_col_values.extend([y, x])
                 latlng.append(all_col_values)
-
-        all_col_keys = list(df.keys())
-        all_col_keys.extend(['lat', 'lng'])
-        df_new = pd.DataFrame(latlng, columns=all_col_keys)
-        export_file = export_file_name + '.' + export_file_type
-        if export_file_type == 'csv':
-            df_new.to_csv(export_file)
-        if export_file_type == 'geojson':
-            geojson = {
-                "type": "FeatureCollection",
-                "features": []
-            }
-
-            for _, row in df_new.iterrows():
-                properties = {}
-                for key in df.keys():
-                    properties[key] = row[key]
-
-                feature = {
-                    "type": "Feature",
-                    "properties": properties,
-                    "geometry": {
-                        "type": "Point",
-                        "coordinates": [row['lat'], row['lng']]
-                        # Replace 'Longitude' and 'Latitude' with your column names
+                time.sleep(pause)
+            if create_continue or i == (end_row-1):
+                df_new = pd.DataFrame(latlng, columns=all_col_keys)
+                export_file = export_file_name + '.' + export_file_type
+                if export_file_type == 'csv':
+                    df_new.to_csv(export_file)
+                if export_file_type == 'geojson':
+                    geojson = {
+                        "type": "FeatureCollection",
+                        "features": []
                     }
-                }
-                geojson['features'].append(feature)
 
-            with open(export_file, 'w') as f:
-                json.dump(geojson, f)
-            print(f'File created "{export_file}".')
+                    for _, row in df_new.iterrows():
+                        properties = {}
+                        for key in df.keys():
+                            properties[key] = row[key]
+
+                        feature = {
+                            "type": "Feature",
+                            "properties": properties,
+                            "geometry": {
+                                "type": "Point",
+                                "coordinates": [row['lat'], row['lng']]
+                            }
+                        }
+                        geojson['features'].append(feature)
+
+                    with open(export_file, 'w') as f:
+                        json.dump(geojson, f)
+                    print(f'File created "{export_file}".')
```

### Comparing `here_geocoding-0.2.0/here_geocoding.egg-info/PKG-INFO` & `here_geocoding-0.3.0/here_geocoding.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: here-geocoding
-Version: 0.2.0
+Version: 0.3.0
 Summary: The "here-geocoding" package is a Python library designed to streamline the process of converting addresses stored in an Excel (xlsx) file into latitude and longitude coordinates. It provides a convenient solution for geocoding large sets of addresses using the HERE geocoding service.
 Home-page: https://github.com/Mariosmsk/here_geocoding
 Author: Marios S. Kyriakou
 Author-email: mariosmsk@gmail.com
 License: MIT license
 Keywords: here_geocoding
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `here_geocoding-0.2.0/here_geocoding.egg-info/SOURCES.txt` & `here_geocoding-0.3.0/here_geocoding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `here_geocoding-0.2.0/setup.py` & `here_geocoding-0.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,10 +44,10 @@
     include_package_data=True,
     keywords='here_geocoding',
     name='here_geocoding',
     packages=find_packages(include=['here_geocoding', 'here_geocoding.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/Mariosmsk/here_geocoding',
-    version='0.2.0',
+    version='0.3.0',
     zip_safe=False,
 )
```

### Comparing `here_geocoding-0.2.0/tests/address-sample.xlsx` & `here_geocoding-0.3.0/tests/address-sample.xlsx`

 * *Files identical despite different names*

### Comparing `here_geocoding-0.2.0/tests/examples.py` & `here_geocoding-0.3.0/tests/examples.py`

 * *Files identical despite different names*

### Comparing `here_geocoding-0.2.0/tests/test_here_geocoding.py` & `here_geocoding-0.3.0/tests/test_here_geocoding.py`

 * *Files identical despite different names*

