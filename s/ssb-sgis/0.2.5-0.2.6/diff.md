# Comparing `tmp/ssb_sgis-0.2.5.tar.gz` & `tmp/ssb_sgis-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_sgis-0.2.5.tar", max compression
+gzip compressed data, was "ssb_sgis-0.2.6.tar", max compression
```

## Comparing `ssb_sgis-0.2.5.tar` & `ssb_sgis-0.2.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1074 2023-06-08 11:05:20.483431 ssb_sgis-0.2.5/LICENSE
--rw-r--r--   0        0        0     7543 2023-06-08 11:05:20.483431 ssb_sgis-0.2.5/README.md
--rw-r--r--   0        0        0     2539 2023-06-08 11:05:50.623519 ssb_sgis-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     2334 2023-06-08 11:05:50.623519 ssb_sgis-0.2.5/src/sgis/__init__.py
--rw-r--r--   0        0        0     3442 2023-06-08 11:05:50.623519 ssb_sgis-0.2.5/src/sgis/dapla.py
--rw-r--r--   0        0        0      576 2023-06-08 11:05:20.519431 ssb_sgis-0.2.5/src/sgis/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-08 11:05:20.519431 ssb_sgis-0.2.5/src/sgis/geopandas_tools/__init__.py
--rw-r--r--   0        0        0     8080 2023-06-08 11:05:50.623519 ssb_sgis-0.2.5/src/sgis/geopandas_tools/buffer_dissolve_explode.py
--rw-r--r--   0        0        0    17659 2023-06-08 11:05:50.623519 ssb_sgis-0.2.5/src/sgis/geopandas_tools/general.py
--rw-r--r--   0        0        0     5870 2023-06-08 11:05:50.623519 ssb_sgis-0.2.5/src/sgis/geopandas_tools/geometry_types.py
--rw-r--r--   0        0        0    14520 2023-06-08 11:05:20.519431 ssb_sgis-0.2.5/src/sgis/geopandas_tools/neighbors.py
--rw-r--r--   0        0        0    11862 2023-06-08 11:05:50.623519 ssb_sgis-0.2.5/src/sgis/geopandas_tools/overlay.py
--rw-r--r--   0        0        0     6888 2023-06-08 11:05:20.519431 ssb_sgis-0.2.5/src/sgis/geopandas_tools/point_operations.py
--rw-r--r--   0        0        0    20336 2023-06-08 11:05:50.623519 ssb_sgis-0.2.5/src/sgis/geopandas_tools/polygon_operations.py
--rw-r--r--   0        0        0     9722 2023-06-08 11:05:20.519431 ssb_sgis-0.2.5/src/sgis/geopandas_tools/to_geodataframe.py
--rw-r--r--   0        0        0     2674 2023-06-08 11:05:20.519431 ssb_sgis-0.2.5/src/sgis/helpers.py
--rw-r--r--   0        0        0        0 2023-06-08 11:05:20.519431 ssb_sgis-0.2.5/src/sgis/maps/__init__.py
--rw-r--r--   0        0        0    21872 2023-06-08 11:05:50.623519 ssb_sgis-0.2.5/src/sgis/maps/explore.py
--rw-r--r--   0        0        0     1923 2023-06-08 11:05:50.623519 ssb_sgis-0.2.5/src/sgis/maps/httpserver.py
--rw-r--r--   0        0        0    20499 2023-06-08 11:05:20.519431 ssb_sgis-0.2.5/src/sgis/maps/legend.py
--rw-r--r--   0        0        0    18490 2023-06-08 11:05:50.623519 ssb_sgis-0.2.5/src/sgis/maps/map.py
--rw-r--r--   0        0        0    15961 2023-06-08 11:05:50.623519 ssb_sgis-0.2.5/src/sgis/maps/maps.py
--rw-r--r--   0        0        0    14132 2023-06-08 11:05:20.519431 ssb_sgis-0.2.5/src/sgis/maps/thematicmap.py
--rw-r--r--   0        0        0        0 2023-06-08 11:05:20.519431 ssb_sgis-0.2.5/src/sgis/networkanalysis/__init__.py
--rw-r--r--   0        0        0     6218 2023-06-08 11:05:20.519431 ssb_sgis-0.2.5/src/sgis/networkanalysis/_get_route.py
--rw-r--r--   0        0        0     2017 2023-06-08 11:05:20.519431 ssb_sgis-0.2.5/src/sgis/networkanalysis/_od_cost_matrix.py
--rw-r--r--   0        0        0     4206 2023-06-08 11:05:20.519431 ssb_sgis-0.2.5/src/sgis/networkanalysis/_points.py
--rw-r--r--   0        0        0     4487 2023-06-08 11:05:20.519431 ssb_sgis-0.2.5/src/sgis/networkanalysis/_service_area.py
--rw-r--r--   0        0        0    12433 2023-06-08 11:05:20.519431 ssb_sgis-0.2.5/src/sgis/networkanalysis/closing_network_holes.py
--rw-r--r--   0        0        0    12369 2023-06-08 11:05:50.623519 ssb_sgis-0.2.5/src/sgis/networkanalysis/cutting_lines.py
--rw-r--r--   0        0        0     9375 2023-06-08 11:05:20.519431 ssb_sgis-0.2.5/src/sgis/networkanalysis/directednetwork.py
--rw-r--r--   0        0        0     3359 2023-06-08 11:05:20.523431 ssb_sgis-0.2.5/src/sgis/networkanalysis/finding_isolated_networks.py
--rw-r--r--   0        0        0     7686 2023-06-08 11:05:20.523431 ssb_sgis-0.2.5/src/sgis/networkanalysis/network.py
--rw-r--r--   0        0        0    66761 2023-06-08 11:05:20.523431 ssb_sgis-0.2.5/src/sgis/networkanalysis/networkanalysis.py
--rw-r--r--   0        0        0    12643 2023-06-08 11:05:20.523431 ssb_sgis-0.2.5/src/sgis/networkanalysis/networkanalysisrules.py
--rw-r--r--   0        0        0     6767 2023-06-08 11:05:50.623519 ssb_sgis-0.2.5/src/sgis/networkanalysis/nodes.py
--rw-r--r--   0        0        0        0 2023-06-08 11:05:20.523431 ssb_sgis-0.2.5/src/sgis/py.typed
--rw-r--r--   0        0        0     3774 2023-06-08 11:05:20.523431 ssb_sgis-0.2.5/src/sgis/read_parquet.py
--rw-r--r--   0        0        0     8831 1970-01-01 00:00:00.000000 ssb_sgis-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-14 06:46:13.344762 ssb_sgis-0.2.6/LICENSE
+-rw-r--r--   0        0        0     7543 2023-06-14 06:46:13.344762 ssb_sgis-0.2.6/README.md
+-rw-r--r--   0        0        0     2539 2023-06-14 06:46:34.180997 ssb_sgis-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     2334 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/__init__.py
+-rw-r--r--   0        0        0     3542 2023-06-14 06:46:34.180997 ssb_sgis-0.2.6/src/sgis/dapla.py
+-rw-r--r--   0        0        0      576 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/geopandas_tools/__init__.py
+-rw-r--r--   0        0        0     8080 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/geopandas_tools/buffer_dissolve_explode.py
+-rw-r--r--   0        0        0    17659 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/geopandas_tools/general.py
+-rw-r--r--   0        0        0     5870 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/geopandas_tools/geometry_types.py
+-rw-r--r--   0        0        0    14520 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/geopandas_tools/neighbors.py
+-rw-r--r--   0        0        0    11862 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/geopandas_tools/overlay.py
+-rw-r--r--   0        0        0     6888 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/geopandas_tools/point_operations.py
+-rw-r--r--   0        0        0    20336 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/geopandas_tools/polygon_operations.py
+-rw-r--r--   0        0        0     9722 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/geopandas_tools/to_geodataframe.py
+-rw-r--r--   0        0        0     2674 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/helpers.py
+-rw-r--r--   0        0        0        0 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/maps/__init__.py
+-rw-r--r--   0        0        0    23631 2023-06-14 06:46:34.180997 ssb_sgis-0.2.6/src/sgis/maps/explore.py
+-rw-r--r--   0        0        0     1923 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/maps/httpserver.py
+-rw-r--r--   0        0        0    20499 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/maps/legend.py
+-rw-r--r--   0        0        0    18490 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/maps/map.py
+-rw-r--r--   0        0        0    15961 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/maps/maps.py
+-rw-r--r--   0        0        0    14132 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/maps/thematicmap.py
+-rw-r--r--   0        0        0        0 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/networkanalysis/__init__.py
+-rw-r--r--   0        0        0     6218 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/networkanalysis/_get_route.py
+-rw-r--r--   0        0        0     2017 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/networkanalysis/_od_cost_matrix.py
+-rw-r--r--   0        0        0     4206 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/networkanalysis/_points.py
+-rw-r--r--   0        0        0     4487 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/networkanalysis/_service_area.py
+-rw-r--r--   0        0        0    12433 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/networkanalysis/closing_network_holes.py
+-rw-r--r--   0        0        0    12369 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/networkanalysis/cutting_lines.py
+-rw-r--r--   0        0        0     9375 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/networkanalysis/directednetwork.py
+-rw-r--r--   0        0        0     3359 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/networkanalysis/finding_isolated_networks.py
+-rw-r--r--   0        0        0     7686 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/networkanalysis/network.py
+-rw-r--r--   0        0        0    66761 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/networkanalysis/networkanalysis.py
+-rw-r--r--   0        0        0    12643 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/networkanalysis/networkanalysisrules.py
+-rw-r--r--   0        0        0     6767 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/networkanalysis/nodes.py
+-rw-r--r--   0        0        0        0 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/py.typed
+-rw-r--r--   0        0        0     3774 2023-06-14 06:46:13.380762 ssb_sgis-0.2.6/src/sgis/read_parquet.py
+-rw-r--r--   0        0        0     8831 1970-01-01 00:00:00.000000 ssb_sgis-0.2.6/PKG-INFO
```

### Comparing `ssb_sgis-0.2.5/LICENSE` & `ssb_sgis-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.5/README.md` & `ssb_sgis-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.5/pyproject.toml` & `ssb_sgis-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-sgis"
-version = "0.2.5"
+version = "0.2.6"
 description = "GIS functions used at Statistics Norway."
 authors = ["Statistics Norway <ort@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "sgis", from = "src"}]
 homepage = "https://github.com/statisticsnorway/ssb-sgis"
 repository = "https://github.com/statisticsnorway/ssb-sgis"
```

### Comparing `ssb_sgis-0.2.5/src/sgis/__init__.py` & `ssb_sgis-0.2.6/src/sgis/__init__.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.5/src/sgis/dapla.py` & `ssb_sgis-0.2.6/src/sgis/dapla.py`

 * *Files 17% similar despite different names*

```diff
@@ -43,30 +43,34 @@
             or read_file, depending on the file type.
 
      Returns:
          A GeoDataFrame.
     """
     fs = dp.FileClient.get_gcs_file_system()
 
-    try:
-        if "parquet" in path:
-            with fs.open(path, mode="rb") as file:
+    if "parquet" in path:
+        with fs.open(path, mode="rb") as file:
+            try:
                 return gpd.read_parquet(file, **kwargs)
-        else:
-            with fs.open(path, mode="rb") as file:
+            except ValueError as e:
+                df = dp.read_pandas(path, **kwargs)
+                if not len(df):
+                    return df
+                else:
+                    raise e
+    else:
+        with fs.open(path, mode="rb") as file:
+            try:
                 return gpd.read_file(file, **kwargs)
-    except FileNotFoundError as e:
-        parent = str(Path(path).parent)
-        if exists(parent):
-            print(
-                f"Didn't find the file {path}."
-                "\nHere are the files in the parent directory:"
-            )
-            print(dp.FileClient().ls(parent))
-        raise e
+            except ValueError as e:
+                df = dp.read_pandas(path, **kwargs)
+                if not len(df):
+                    return df
+                else:
+                    raise e
 
 
 def write_geopandas(
     df: gpd.GeoDataFrame, gcs_path: str, overwrite: bool = True, **kwargs
 ) -> None:
     """Writes a GeoDataFrame to the speficied format.
```

### Comparing `ssb_sgis-0.2.5/src/sgis/exceptions.py` & `ssb_sgis-0.2.6/src/sgis/exceptions.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.5/src/sgis/geopandas_tools/buffer_dissolve_explode.py` & `ssb_sgis-0.2.6/src/sgis/geopandas_tools/buffer_dissolve_explode.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.5/src/sgis/geopandas_tools/general.py` & `ssb_sgis-0.2.6/src/sgis/geopandas_tools/general.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.5/src/sgis/geopandas_tools/geometry_types.py` & `ssb_sgis-0.2.6/src/sgis/geopandas_tools/geometry_types.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.5/src/sgis/geopandas_tools/neighbors.py` & `ssb_sgis-0.2.6/src/sgis/geopandas_tools/neighbors.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.5/src/sgis/geopandas_tools/overlay.py` & `ssb_sgis-0.2.6/src/sgis/geopandas_tools/overlay.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.5/src/sgis/geopandas_tools/point_operations.py` & `ssb_sgis-0.2.6/src/sgis/geopandas_tools/point_operations.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.5/src/sgis/geopandas_tools/polygon_operations.py` & `ssb_sgis-0.2.6/src/sgis/geopandas_tools/polygon_operations.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.5/src/sgis/geopandas_tools/to_geodataframe.py` & `ssb_sgis-0.2.6/src/sgis/geopandas_tools/to_geodataframe.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.5/src/sgis/helpers.py` & `ssb_sgis-0.2.6/src/sgis/helpers.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.5/src/sgis/maps/explore.py` & `ssb_sgis-0.2.6/src/sgis/maps/explore.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 from statistics import mean
 
 import branca as bc
 import folium
 import matplotlib
 import numpy as np
 import pandas as pd
+from folium import plugins
 from geopandas import GeoDataFrame
 from IPython.display import display
+from jinja2 import Template
 from shapely.geometry import LineString
 
 from ..geopandas_tools.general import clean_geoms, make_all_singlepart
 from ..geopandas_tools.geometry_types import get_geom_type
 from ..geopandas_tools.to_geodataframe import to_gdf
 from ..helpers import unit_is_degrees
 from .httpserver import run_html_server
@@ -57,24 +59,50 @@
     "max_lat",
     "min_lon",
     "max_lon",
     "max_bounds",
 ]
 
 
+class MeasureControlFix(plugins.MeasureControl):
+    """To fix a bug in the lenght measurement control.
+
+    Kudos to abewartech (https://github.com/ljagis/leaflet-measure/issues/171).
+    """
+
+    _template = Template(
+        """
+{% macro script(this, kwargs) %}
+    L.Control.Measure.include({ _setCaptureMarkerIcon: function () { this._captureMarker.options.autoPanOnFocus = false; this._captureMarker.setIcon( L.divIcon({ iconSize: this._map.getSize().multiplyBy(2), }), ); }, });
+    var {{ this.get_name() }} = new L.Control.Measure(
+        {{ this.options|tojson }});
+    {{this._parent.get_name()}}.addControl({{this.get_name()}});
+
+{% endmacro %}
+    """
+    )
+
+    def __init__(self, active_color="red", completed_color="red", **kwargs):
+        super().__init__(
+            active_color=active_color, completed_color=completed_color, **kwargs
+        )
+
+
 class Explore(Map):
     def __init__(
         self,
         *gdfs,
         column: str | None = None,
         popup: bool = True,
         max_zoom: int = 30,
         smooth_factor: float = 1.5,
         browser: bool = False,
         prefer_canvas: bool = True,
+        measure_control: bool = True,
+        geocoder: bool = True,
         save=None,
         **kwargs,
     ):
         self.browser = browser
         if not self.browser and "show_in_browser" in kwargs:
             self.browser = kwargs.pop("show_in_browser")
         if not self.browser and "in_browser" in kwargs:
@@ -82,14 +110,16 @@
 
         super().__init__(*gdfs, column=column, **kwargs)
 
         self.popup = popup
         self.max_zoom = max_zoom
         self.smooth_factor = smooth_factor
         self.prefer_canvas = prefer_canvas
+        self.measure_control = measure_control
+        self.geocoder = geocoder
         self.save = save
 
         self._to_single_geom_type()
 
         if self._is_categorical:
             if len(self.gdfs) == 1:
                 self._split_categories()
@@ -287,16 +317,16 @@
 
         _categorical_legend(
             self.map,
             self._column,
             self._categories_colors_dict.keys(),
             self._categories_colors_dict.values(),
         )
-        folium.TileLayer("stamentoner").add_to(self.map)
-        folium.TileLayer("cartodbdark_matter").add_to(self.map)
+        folium.TileLayer("stamentoner", max_zoom=self.max_zoom).add_to(self.map)
+        folium.TileLayer("cartodbdark_matter", max_zoom=self.max_zoom).add_to(self.map)
         self.map.add_child(folium.LayerControl())
 
     def _create_continous_map(self):
         self._prepare_continous_map()
         if self.scheme:
             classified = self._classify_from_bins(self._gdf, bins=self.bins)
             classified_sequential = self._push_classification(classified)
@@ -444,14 +474,34 @@
             tiles=tiles,
             attr=attr,
             width=width,
             height=height,
             **map_kwds,
         )
 
+        if self.measure_control:
+            MeasureControlFix(
+                primary_length_unit="meters",
+                secondary_length_unit="kilometers",
+                primary_area_unit="sqmeters",
+                secondary_area_unit="sqkilometers",
+                position="bottomleft",
+                capture_z_index=False,
+            ).add_to(m)
+
+        plugins.Fullscreen(
+            position="topleft",
+            title="Expand me",
+            title_cancel="Exit me",
+            force_separate_button=True,
+        ).add_to(m)
+
+        if self.geocoder:
+            plugins.Geocoder(position="topright").add_to(m)
+
         # fit bounds to get a proper zoom level
         if fit and "zoom_start" not in kwargs:
             m.fit_bounds([[bounds[1], bounds[0]], [bounds[3], bounds[2]]])
 
         return m
 
     def _make_geojson(
```

### Comparing `ssb_sgis-0.2.5/src/sgis/maps/httpserver.py` & `ssb_sgis-0.2.6/src/sgis/maps/httpserver.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.5/src/sgis/maps/legend.py` & `ssb_sgis-0.2.6/src/sgis/maps/legend.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.5/src/sgis/maps/map.py` & `ssb_sgis-0.2.6/src/sgis/maps/map.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.5/src/sgis/maps/maps.py` & `ssb_sgis-0.2.6/src/sgis/maps/maps.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.5/src/sgis/maps/thematicmap.py` & `ssb_sgis-0.2.6/src/sgis/maps/thematicmap.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.5/src/sgis/networkanalysis/_get_route.py` & `ssb_sgis-0.2.6/src/sgis/networkanalysis/_get_route.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.5/src/sgis/networkanalysis/_od_cost_matrix.py` & `ssb_sgis-0.2.6/src/sgis/networkanalysis/_od_cost_matrix.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.5/src/sgis/networkanalysis/_points.py` & `ssb_sgis-0.2.6/src/sgis/networkanalysis/_points.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.5/src/sgis/networkanalysis/_service_area.py` & `ssb_sgis-0.2.6/src/sgis/networkanalysis/_service_area.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.5/src/sgis/networkanalysis/closing_network_holes.py` & `ssb_sgis-0.2.6/src/sgis/networkanalysis/closing_network_holes.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.5/src/sgis/networkanalysis/cutting_lines.py` & `ssb_sgis-0.2.6/src/sgis/networkanalysis/cutting_lines.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.5/src/sgis/networkanalysis/directednetwork.py` & `ssb_sgis-0.2.6/src/sgis/networkanalysis/directednetwork.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.5/src/sgis/networkanalysis/finding_isolated_networks.py` & `ssb_sgis-0.2.6/src/sgis/networkanalysis/finding_isolated_networks.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.5/src/sgis/networkanalysis/network.py` & `ssb_sgis-0.2.6/src/sgis/networkanalysis/network.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.5/src/sgis/networkanalysis/networkanalysis.py` & `ssb_sgis-0.2.6/src/sgis/networkanalysis/networkanalysis.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.5/src/sgis/networkanalysis/networkanalysisrules.py` & `ssb_sgis-0.2.6/src/sgis/networkanalysis/networkanalysisrules.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.5/src/sgis/networkanalysis/nodes.py` & `ssb_sgis-0.2.6/src/sgis/networkanalysis/nodes.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.5/src/sgis/read_parquet.py` & `ssb_sgis-0.2.6/src/sgis/read_parquet.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.5/PKG-INFO` & `ssb_sgis-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssb-sgis
-Version: 0.2.5
+Version: 0.2.6
 Summary: GIS functions used at Statistics Norway.
 Home-page: https://github.com/statisticsnorway/ssb-sgis
 License: MIT
 Author: Statistics Norway
 Author-email: ort@ssb.no
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 3 - Alpha
```

