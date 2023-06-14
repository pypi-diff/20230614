# Comparing `tmp/meteva_base-0.1.2-py3-none-any.whl.zip` & `tmp/meteva_base-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 207719 bytes, number of entries: 74
+Zip file size: 2792097 bytes, number of entries: 114
 -rw-rw-rw-  2.0 fat      174 b- defN 23-Apr-17 06:52 meteva_base/__init__.py
 -rw-rw-rw-  2.0 fat      141 b- defN 23-Apr-17 02:32 meteva_base/basicdata/__init__.py
 -rw-rw-rw-  2.0 fat     1199 b- defN 23-Jun-05 03:42 meteva_base/basicdata/const.py
 -rw-rw-rw-  2.0 fat     7385 b- defN 23-May-26 02:34 meteva_base/basicdata/ctl.py
 -rw-rw-rw-  2.0 fat    19260 b- defN 23-May-26 02:38 meteva_base/basicdata/dicts.py
 -rw-rw-rw-  2.0 fat    11163 b- defN 23-May-26 02:39 meteva_base/basicdata/grid.py
 -rw-rw-rw-  2.0 fat    32561 b- defN 23-May-26 02:58 meteva_base/basicdata/grid_data.py
@@ -45,32 +45,72 @@
 -rw-rw-rw-  2.0 fat     1649 b- defN 23-Apr-17 02:32 meteva_base/io/encoding.py
 -rw-rw-rw-  2.0 fat    17194 b- defN 23-May-26 09:05 meteva_base/io/ftpconn.py
 -rw-rw-rw-  2.0 fat     1771 b- defN 23-Apr-17 02:32 meteva_base/io/httpclient.py
 -rw-rw-rw-  2.0 fat     8190 b- defN 23-Apr-17 02:32 meteva_base/io/httpconn.py
 -rw-rw-rw-  2.0 fat     4882 b- defN 23-Apr-17 02:32 meteva_base/io/loglib.py
 -rw-rw-rw-  2.0 fat     6048 b- defN 23-Apr-17 02:32 meteva_base/io/print_grib_info.py
 -rw-rw-rw-  2.0 fat    20392 b- defN 23-Jun-14 01:15 meteva_base/io/read_graphydata.py
--rw-rw-rw-  2.0 fat    86511 b- defN 23-May-26 09:11 meteva_base/io/read_griddata.py
+-rw-rw-rw-  2.0 fat    86511 b- defN 23-Jun-14 04:34 meteva_base/io/read_griddata.py
 -rw-rw-rw-  2.0 fat    91510 b- defN 23-May-26 09:15 meteva_base/io/read_stadata.py
 -rw-rw-rw-  2.0 fat     4673 b- defN 23-May-26 09:19 meteva_base/io/write_array.py
 -rw-rw-rw-  2.0 fat    10883 b- defN 23-May-26 09:23 meteva_base/io/write_griddata.py
 -rw-rw-rw-  2.0 fat    12427 b- defN 23-May-26 09:25 meteva_base/io/write_stadata.py
+-rw-rw-rw-  2.0 fat     1770 b- defN 23-Apr-06 04:00 meteva_base/resources/colormaps/color_rain_1h.bak.txt
+-rw-rw-rw-  2.0 fat     1510 b- defN 23-Apr-06 04:00 meteva_base/resources/colormaps/color_rain_1h.txt
+-rw-rw-rw-  2.0 fat     2135 b- defN 23-Apr-06 04:00 meteva_base/resources/colormaps/color_rain_1h_error.txt
+-rw-rw-rw-  2.0 fat      169 b- defN 23-Apr-06 04:00 meteva_base/resources/colormaps/color_rain_24h.txt
+-rw-rw-rw-  2.0 fat     1783 b- defN 23-Apr-06 04:00 meteva_base/resources/colormaps/color_rain_3h.bak.txt
+-rw-rw-rw-  2.0 fat     1519 b- defN 23-Apr-06 04:00 meteva_base/resources/colormaps/color_rain_3h.txt
+-rw-rw-rw-  2.0 fat     2145 b- defN 23-Apr-06 04:00 meteva_base/resources/colormaps/color_rain_3h_error.txt
+-rw-rw-rw-  2.0 fat     4330 b- defN 23-Apr-06 04:00 meteva_base/resources/colormaps/color_rh.txt
+-rw-rw-rw-  2.0 fat     4369 b- defN 23-Apr-06 04:00 meteva_base/resources/colormaps/color_rh_error.txt
+-rw-rw-rw-  2.0 fat     4336 b- defN 23-Apr-06 04:00 meteva_base/resources/colormaps/color_tcdc.txt
+-rw-rw-rw-  2.0 fat     4412 b- defN 23-Apr-06 04:00 meteva_base/resources/colormaps/color_tcdc_error.txt
+-rw-rw-rw-  2.0 fat      646 b- defN 23-Apr-06 04:00 meteva_base/resources/colormaps/color_temp_2m.txt
+-rw-rw-rw-  2.0 fat      139 b- defN 23-Apr-06 04:00 meteva_base/resources/colormaps/color_vis.txt
+-rw-rw-rw-  2.0 fat     4386 b- defN 23-Apr-06 04:00 meteva_base/resources/colormaps/color_vis_error.txt
+-rw-rw-rw-  2.0 fat      186 b- defN 23-Apr-06 04:00 meteva_base/resources/colormaps/color_wind_speed.txt
+-rw-rw-rw-  2.0 fat     1754 b- defN 23-Apr-06 04:00 meteva_base/resources/colormaps/color_wind_speed_error.txt
+-rw-rw-rw-  2.0 fat   698853 b- defN 23-Apr-06 04:00 meteva_base/resources/maps/BOUNT_poly.dbf
+-rw-rw-rw-  2.0 fat      132 b- defN 23-Apr-06 04:00 meteva_base/resources/maps/BOUNT_poly.prj
+-rw-rw-rw-  2.0 fat  1249784 b- defN 23-Apr-06 04:00 meteva_base/resources/maps/BOUNT_poly.shp
+-rw-rw-rw-  2.0 fat    27356 b- defN 23-Apr-06 04:00 meteva_base/resources/maps/BOUNT_poly.shx
+-rw-rw-rw-  2.0 fat     5281 b- defN 23-Apr-06 04:00 meteva_base/resources/maps/NationalBorder.dbf
+-rw-rw-rw-  2.0 fat      132 b- defN 23-Apr-06 04:00 meteva_base/resources/maps/NationalBorder.prj
+-rw-rw-rw-  2.0 fat   165564 b- defN 23-Apr-06 04:00 meteva_base/resources/maps/NationalBorder.shp
+-rw-rw-rw-  2.0 fat     8444 b- defN 23-Apr-06 04:00 meteva_base/resources/maps/NationalBorder.shx
+-rw-rw-rw-  2.0 fat      168 b- defN 23-Apr-06 04:00 meteva_base/resources/maps/Province.dbf
+-rw-rw-rw-  2.0 fat      132 b- defN 23-Apr-06 04:00 meteva_base/resources/maps/Province.prj
+-rw-rw-rw-  2.0 fat   511192 b- defN 23-Apr-06 04:00 meteva_base/resources/maps/Province.shp
+-rw-rw-rw-  2.0 fat      372 b- defN 23-Apr-06 04:00 meteva_base/resources/maps/Province.shx
+-rw-rw-rw-  2.0 fat    62990 b- defN 23-Apr-06 04:00 meteva_base/resources/maps/hyd1_4p.dbf
+-rw-rw-rw-  2.0 fat   931572 b- defN 23-Apr-06 04:00 meteva_base/resources/maps/hyd1_4p.shp
+-rw-rw-rw-  2.0 fat     4500 b- defN 23-Apr-06 04:00 meteva_base/resources/maps/hyd1_4p.shx
+-rw-rw-rw-  2.0 fat    25256 b- defN 23-Apr-06 04:00 meteva_base/resources/maps/worldmap.dbf
+-rw-rw-rw-  2.0 fat      132 b- defN 23-Apr-06 04:00 meteva_base/resources/maps/worldmap.prj
+-rw-rw-rw-  2.0 fat   685424 b- defN 23-Apr-06 04:00 meteva_base/resources/maps/worldmap.shp
+-rw-rw-rw-  2.0 fat    40404 b- defN 23-Apr-06 04:00 meteva_base/resources/maps/worldmap.shx
+-rw-rw-rw-  2.0 fat  1190450 b- defN 23-Apr-06 04:00 meteva_base/resources/stations/geography_temp_delta.txt
+-rw-rw-rw-  2.0 fat    76646 b- defN 23-Apr-06 04:00 meteva_base/resources/stations/sta2411_alt.txt
+-rw-rw-rw-  2.0 fat     7663 b- defN 23-Apr-06 04:00 meteva_base/resources/stations/sta_global_alt_243.txt
+-rw-rw-rw-  2.0 fat   371710 b- defN 23-Apr-06 04:00 meteva_base/resources/stations/station_global_alt_11621.txt
+-rw-rw-rw-  2.0 fat   546988 b- defN 23-Apr-06 04:00 meteva_base/resources/stations/station_id_pro_county.txt
 -rw-rw-rw-  2.0 fat     1216 b- defN 23-Jun-11 10:54 meteva_base/tool/__init__.py
 -rw-rw-rw-  2.0 fat    42732 b- defN 23-Jun-11 01:42 meteva_base/tool/color_tools.py
 -rw-rw-rw-  2.0 fat    13841 b- defN 23-Apr-17 02:32 meteva_base/tool/copy_tools.py
 -rw-rw-rw-  2.0 fat     1246 b- defN 23-Jun-11 05:33 meteva_base/tool/frprmn2.py
 -rw-rw-rw-  2.0 fat     4699 b- defN 23-Jun-11 10:55 meteva_base/tool/grib_tools.py
 -rw-rw-rw-  2.0 fat    10981 b- defN 23-Jun-13 01:19 meteva_base/tool/grib_tools_py.py
 -rw-rw-rw-  2.0 fat     8802 b- defN 23-Apr-17 05:59 meteva_base/tool/maskout.py
 -rw-rw-rw-  2.0 fat    11227 b- defN 23-May-26 09:45 meteva_base/tool/math_tools.py
 -rw-rw-rw-  2.0 fat    12506 b- defN 23-Apr-17 02:32 meteva_base/tool/path_tools.py
 -rw-rw-rw-  2.0 fat   174805 b- defN 23-May-26 10:00 meteva_base/tool/plot_tools.py
 -rw-rw-rw-  2.0 fat    33020 b- defN 23-May-29 02:32 meteva_base/tool/plot_tools_adv.py
 -rw-rw-rw-  2.0 fat     4851 b- defN 23-Apr-17 02:32 meteva_base/tool/process_tools.py
--rw-rw-rw-  2.0 fat     3816 b- defN 23-Apr-17 03:21 meteva_base/tool/station_tools.py
+-rw-rw-rw-  2.0 fat     4585 b- defN 23-Jun-14 04:16 meteva_base/tool/station_tools.py
 -rw-rw-rw-  2.0 fat     5637 b- defN 23-Apr-17 02:32 meteva_base/tool/time_tools.py
--rw-rw-rw-  2.0 fat     1084 b- defN 23-Jun-14 02:22 meteva_base-0.1.2.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      824 b- defN 23-Jun-14 02:22 meteva_base-0.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-14 02:22 meteva_base-0.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Jun-14 02:22 meteva_base-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     6482 b- defN 23-Jun-14 02:22 meteva_base-0.1.2.dist-info/RECORD
-74 files, 1064738 bytes uncompressed, 197465 bytes compressed:  81.5%
+-rw-rw-rw-  2.0 fat     1084 b- defN 23-Jun-14 04:43 meteva_base-0.1.4.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      824 b- defN 23-Jun-14 04:43 meteva_base-0.1.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-14 04:43 meteva_base-0.1.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Jun-14 04:43 meteva_base-0.1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat    10627 b- defN 23-Jun-14 04:43 meteva_base-0.1.4.dist-info/RECORD
+114 files, 7716386 bytes uncompressed, 2775103 bytes compressed:  64.0%
```

## zipnote {}

```diff
@@ -159,14 +159,134 @@
 
 Filename: meteva_base/io/write_griddata.py
 Comment: 
 
 Filename: meteva_base/io/write_stadata.py
 Comment: 
 
+Filename: meteva_base/resources/colormaps/color_rain_1h.bak.txt
+Comment: 
+
+Filename: meteva_base/resources/colormaps/color_rain_1h.txt
+Comment: 
+
+Filename: meteva_base/resources/colormaps/color_rain_1h_error.txt
+Comment: 
+
+Filename: meteva_base/resources/colormaps/color_rain_24h.txt
+Comment: 
+
+Filename: meteva_base/resources/colormaps/color_rain_3h.bak.txt
+Comment: 
+
+Filename: meteva_base/resources/colormaps/color_rain_3h.txt
+Comment: 
+
+Filename: meteva_base/resources/colormaps/color_rain_3h_error.txt
+Comment: 
+
+Filename: meteva_base/resources/colormaps/color_rh.txt
+Comment: 
+
+Filename: meteva_base/resources/colormaps/color_rh_error.txt
+Comment: 
+
+Filename: meteva_base/resources/colormaps/color_tcdc.txt
+Comment: 
+
+Filename: meteva_base/resources/colormaps/color_tcdc_error.txt
+Comment: 
+
+Filename: meteva_base/resources/colormaps/color_temp_2m.txt
+Comment: 
+
+Filename: meteva_base/resources/colormaps/color_vis.txt
+Comment: 
+
+Filename: meteva_base/resources/colormaps/color_vis_error.txt
+Comment: 
+
+Filename: meteva_base/resources/colormaps/color_wind_speed.txt
+Comment: 
+
+Filename: meteva_base/resources/colormaps/color_wind_speed_error.txt
+Comment: 
+
+Filename: meteva_base/resources/maps/BOUNT_poly.dbf
+Comment: 
+
+Filename: meteva_base/resources/maps/BOUNT_poly.prj
+Comment: 
+
+Filename: meteva_base/resources/maps/BOUNT_poly.shp
+Comment: 
+
+Filename: meteva_base/resources/maps/BOUNT_poly.shx
+Comment: 
+
+Filename: meteva_base/resources/maps/NationalBorder.dbf
+Comment: 
+
+Filename: meteva_base/resources/maps/NationalBorder.prj
+Comment: 
+
+Filename: meteva_base/resources/maps/NationalBorder.shp
+Comment: 
+
+Filename: meteva_base/resources/maps/NationalBorder.shx
+Comment: 
+
+Filename: meteva_base/resources/maps/Province.dbf
+Comment: 
+
+Filename: meteva_base/resources/maps/Province.prj
+Comment: 
+
+Filename: meteva_base/resources/maps/Province.shp
+Comment: 
+
+Filename: meteva_base/resources/maps/Province.shx
+Comment: 
+
+Filename: meteva_base/resources/maps/hyd1_4p.dbf
+Comment: 
+
+Filename: meteva_base/resources/maps/hyd1_4p.shp
+Comment: 
+
+Filename: meteva_base/resources/maps/hyd1_4p.shx
+Comment: 
+
+Filename: meteva_base/resources/maps/worldmap.dbf
+Comment: 
+
+Filename: meteva_base/resources/maps/worldmap.prj
+Comment: 
+
+Filename: meteva_base/resources/maps/worldmap.shp
+Comment: 
+
+Filename: meteva_base/resources/maps/worldmap.shx
+Comment: 
+
+Filename: meteva_base/resources/stations/geography_temp_delta.txt
+Comment: 
+
+Filename: meteva_base/resources/stations/sta2411_alt.txt
+Comment: 
+
+Filename: meteva_base/resources/stations/sta_global_alt_243.txt
+Comment: 
+
+Filename: meteva_base/resources/stations/station_global_alt_11621.txt
+Comment: 
+
+Filename: meteva_base/resources/stations/station_id_pro_county.txt
+Comment: 
+
 Filename: meteva_base/tool/__init__.py
 Comment: 
 
 Filename: meteva_base/tool/color_tools.py
 Comment: 
 
 Filename: meteva_base/tool/copy_tools.py
@@ -201,23 +321,23 @@
 
 Filename: meteva_base/tool/station_tools.py
 Comment: 
 
 Filename: meteva_base/tool/time_tools.py
 Comment: 
 
-Filename: meteva_base-0.1.2.dist-info/LICENSE.txt
+Filename: meteva_base-0.1.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: meteva_base-0.1.2.dist-info/METADATA
+Filename: meteva_base-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: meteva_base-0.1.2.dist-info/WHEEL
+Filename: meteva_base-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: meteva_base-0.1.2.dist-info/top_level.txt
+Filename: meteva_base-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: meteva_base-0.1.2.dist-info/RECORD
+Filename: meteva_base-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## meteva_base/tool/station_tools.py

```diff
@@ -1,12 +1,13 @@
 import pkg_resources
 import re
-# import meteva
+import os
 import meteva_base
 import pandas as pd
+import urllib.request
 
 def fuzzyfinder(input_str, collection):
     suggestions = []
     pattern = '.*?'.join(input_str)    # Converts 'djm' to 'd.*?j.*?m'
     regex = re.compile(pattern)         # Compiles a regex.
     for item in collection:
         match = regex.search(item)      # Checks if the current item matches the regex.
@@ -98,9 +99,29 @@
 
     df = pd.DataFrame({
         "id":id_list,
         "province_name":pro_names
     })
 
     sta = meteva_base.sta_data(df)
+    return sta
 
-    return sta
+
+
+def get_china_dem_grd():
+    grd_alt_path = meteva_base.terrain_height_grd
+    if not os.path.exists(grd_alt_path):
+        url = "https://github.com/nmcdev/meteva/raw/master/meteva/resources/stations/dem_0.00833.nc"
+        try:
+            print("开始从github下载地形高度数据，请稍等")
+            urllib.request.urlretrieve(url, filename=grd_alt_path)
+        except Exception as e:
+            print("从github下载地形高度数据失败，请重试，或者手动从\n"+url+"\n下载文件并保存至\n"+grd_alt_path)
+            print(e)
+            return None
+    grd = meteva_base.read_griddata_from_nc(grd_alt_path)
+    return grd
+
+
+if __name__ == "__main__":
+    a = get_china_dem_grd()
+    print(a)
```

## Comparing `meteva_base-0.1.2.dist-info/LICENSE.txt` & `meteva_base-0.1.4.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `meteva_base-0.1.2.dist-info/METADATA` & `meteva_base-0.1.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meteva-base
-Version: 0.1.2
+Version: 0.1.4
 Summary: base classes and functions of generally meteorogical usage, like Basic_class/IO/calculation/plot .etc
 Home-page: https://github.com/nmcdev/nimm
 Author: NMC_WFT
 Author-email: pangzide003@163.com
 License: MIT
 Requires-Dist: numpy (>=1.12.1)
 Requires-Dist: pandas (>=1.0.4)
```

