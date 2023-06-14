# Comparing `tmp/satellite_weather_downloader-1.8.3.tar.gz` & `tmp/satellite_weather_downloader-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satellite_weather_downloader-1.8.3.tar", max compression
+gzip compressed data, was "satellite_weather_downloader-1.8.4.tar", max compression
```

## Comparing `satellite_weather_downloader-1.8.3.tar` & `satellite_weather_downloader-1.8.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    35149 2023-05-03 18:11:19.813823 satellite_weather_downloader-1.8.3/LICENSE
--rw-r--r--   0        0        0     3072 2023-05-03 18:11:19.813823 satellite_weather_downloader-1.8.3/README.md
--rw-r--r--   0        0        0     1862 2023-05-03 18:14:17.198639 satellite_weather_downloader-1.8.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-03 18:11:19.817823 satellite_weather_downloader-1.8.3/satellite/__init__.py
--rw-r--r--   0        0        0      190 2023-05-03 18:11:19.817823 satellite_weather_downloader-1.8.3/satellite/downloader/__init__.py
--rw-r--r--   0        0        0     9715 2023-05-03 18:11:19.817823 satellite_weather_downloader-1.8.3/satellite/downloader/extract_reanalysis.py
--rw-r--r--   0        0        0       52 2023-05-03 18:11:19.817823 satellite_weather_downloader-1.8.3/satellite/downloader/reanalysis/__init__.py
--rw-r--r--   0        0        0    12112 2023-05-03 18:11:19.817823 satellite_weather_downloader-1.8.3/satellite/downloader/reanalysis/api_vars.py
--rw-r--r--   0        0        0    16153 2023-05-03 18:11:19.817823 satellite_weather_downloader-1.8.3/satellite/downloader/reanalysis/prompt.py
--rw-r--r--   0        0        0     2924 2023-05-03 18:11:19.817823 satellite_weather_downloader-1.8.3/satellite/downloader/request.py
--rw-r--r--   0        0        0      296 2023-05-03 18:11:19.817823 satellite_weather_downloader-1.8.3/satellite/weather/__init__.py
--rw-r--r--   0        0        0       20 2023-05-03 18:11:19.817823 satellite_weather_downloader-1.8.3/satellite/weather/_brazil/DSEI/__init__.py
--rw-r--r--   0        0        0     1360 2023-05-03 18:11:19.817823 satellite_weather_downloader-1.8.3/satellite/weather/_brazil/DSEI/areas.py
--rw-r--r--   0        0        0       11 2023-05-03 18:11:19.817823 satellite_weather_downloader-1.8.3/satellite/weather/_brazil/DSEI/areas_dsei.cst
--rw-r--r--   0        0        0     9413 2023-05-03 18:11:19.817823 satellite_weather_downloader-1.8.3/satellite/weather/_brazil/DSEI/areas_dsei.dbf
--rw-r--r--   0        0        0      417 2023-05-03 18:11:19.817823 satellite_weather_downloader-1.8.3/satellite/weather/_brazil/DSEI/areas_dsei.prj
--rw-r--r--   0        0        0 11174984 2023-05-03 18:11:19.897824 satellite_weather_downloader-1.8.3/satellite/weather/_brazil/DSEI/areas_dsei.shp
--rw-r--r--   0        0        0      372 2023-05-03 18:11:19.897824 satellite_weather_downloader-1.8.3/satellite/weather/_brazil/DSEI/areas_dsei.shx
--rw-r--r--   0        0        0       77 2023-05-03 18:11:19.897824 satellite_weather_downloader-1.8.3/satellite/weather/_brazil/__init__.py
--rw-r--r--   0        0        0     4119 2023-05-03 18:11:19.897824 satellite_weather_downloader-1.8.3/satellite/weather/_brazil/extract_coordinates.py
--rw-r--r--   0        0        0     1351 2023-05-03 18:11:19.897824 satellite_weather_downloader-1.8.3/satellite/weather/_brazil/extract_latlons.py
--rw-r--r--   0        0        0  1175429 2023-05-03 18:11:19.901824 satellite_weather_downloader-1.8.3/satellite/weather/_brazil/municipios.json
--rw-r--r--   0        0        0       40 2023-05-03 18:11:19.901824 satellite_weather_downloader-1.8.3/satellite/weather/utils/__init__.py
--rw-r--r--   0        0        0     4871 2023-05-03 18:11:19.901824 satellite_weather_downloader-1.8.3/satellite/weather/utils/episem.py
--rw-r--r--   0        0        0    13565 2023-05-03 18:11:19.901824 satellite_weather_downloader-1.8.3/satellite/weather/xr_extensions.py
--rw-r--r--   0        0        0     4888 1970-01-01 00:00:00.000000 satellite_weather_downloader-1.8.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-14 17:31:24.013339 satellite_weather_downloader-1.8.4/LICENSE
+-rw-r--r--   0        0        0     3072 2023-06-14 17:31:24.013339 satellite_weather_downloader-1.8.4/README.md
+-rw-r--r--   0        0        0     1862 2023-06-14 17:34:05.035947 satellite_weather_downloader-1.8.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-14 17:31:24.013339 satellite_weather_downloader-1.8.4/satellite/__init__.py
+-rw-r--r--   0        0        0      190 2023-06-14 17:31:24.013339 satellite_weather_downloader-1.8.4/satellite/downloader/__init__.py
+-rw-r--r--   0        0        0     9715 2023-06-14 17:31:24.013339 satellite_weather_downloader-1.8.4/satellite/downloader/extract_reanalysis.py
+-rw-r--r--   0        0        0       52 2023-06-14 17:31:24.013339 satellite_weather_downloader-1.8.4/satellite/downloader/reanalysis/__init__.py
+-rw-r--r--   0        0        0    12112 2023-06-14 17:31:24.013339 satellite_weather_downloader-1.8.4/satellite/downloader/reanalysis/api_vars.py
+-rw-r--r--   0        0        0    16153 2023-06-14 17:31:24.013339 satellite_weather_downloader-1.8.4/satellite/downloader/reanalysis/prompt.py
+-rw-r--r--   0        0        0     2924 2023-06-14 17:31:24.013339 satellite_weather_downloader-1.8.4/satellite/downloader/request.py
+-rw-r--r--   0        0        0      296 2023-06-14 17:31:24.013339 satellite_weather_downloader-1.8.4/satellite/weather/__init__.py
+-rw-r--r--   0        0        0       20 2023-06-14 17:31:24.013339 satellite_weather_downloader-1.8.4/satellite/weather/_brazil/DSEI/__init__.py
+-rw-r--r--   0        0        0     1360 2023-06-14 17:31:24.013339 satellite_weather_downloader-1.8.4/satellite/weather/_brazil/DSEI/areas.py
+-rw-r--r--   0        0        0       11 2023-06-14 17:31:24.013339 satellite_weather_downloader-1.8.4/satellite/weather/_brazil/DSEI/areas_dsei.cst
+-rw-r--r--   0        0        0     9413 2023-06-14 17:31:24.013339 satellite_weather_downloader-1.8.4/satellite/weather/_brazil/DSEI/areas_dsei.dbf
+-rw-r--r--   0        0        0      417 2023-06-14 17:31:24.013339 satellite_weather_downloader-1.8.4/satellite/weather/_brazil/DSEI/areas_dsei.prj
+-rw-r--r--   0        0        0 11174984 2023-06-14 17:31:24.085341 satellite_weather_downloader-1.8.4/satellite/weather/_brazil/DSEI/areas_dsei.shp
+-rw-r--r--   0        0        0      372 2023-06-14 17:31:24.085341 satellite_weather_downloader-1.8.4/satellite/weather/_brazil/DSEI/areas_dsei.shx
+-rw-r--r--   0        0        0       77 2023-06-14 17:31:24.085341 satellite_weather_downloader-1.8.4/satellite/weather/_brazil/__init__.py
+-rw-r--r--   0        0        0     4119 2023-06-14 17:31:24.085341 satellite_weather_downloader-1.8.4/satellite/weather/_brazil/extract_coordinates.py
+-rw-r--r--   0        0        0     1351 2023-06-14 17:31:24.085341 satellite_weather_downloader-1.8.4/satellite/weather/_brazil/extract_latlons.py
+-rw-r--r--   0        0        0  1175429 2023-06-14 17:31:24.089341 satellite_weather_downloader-1.8.4/satellite/weather/_brazil/municipios.json
+-rw-r--r--   0        0        0       40 2023-06-14 17:31:24.089341 satellite_weather_downloader-1.8.4/satellite/weather/utils/__init__.py
+-rw-r--r--   0        0        0     4871 2023-06-14 17:31:24.089341 satellite_weather_downloader-1.8.4/satellite/weather/utils/episem.py
+-rw-r--r--   0        0        0    13562 2023-06-14 17:31:24.093341 satellite_weather_downloader-1.8.4/satellite/weather/xr_extensions.py
+-rw-r--r--   0        0        0     4789 1970-01-01 00:00:00.000000 satellite_weather_downloader-1.8.4/PKG-INFO
```

### Comparing `satellite_weather_downloader-1.8.3/LICENSE` & `satellite_weather_downloader-1.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.3/README.md` & `satellite_weather_downloader-1.8.4/README.md`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.3/pyproject.toml` & `satellite_weather_downloader-1.8.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.2.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "satellite-weather-downloader"
-version = "1.8.3"  # changed by semantic-release
+version = "1.8.4"  # changed by semantic-release
 description = "The modules available in this package are designed to capture and proccess satellite data from Copernicus"
 readme = "README.md"
 authors = ["Luã Bida Vacaro <luabidaa@gmail.com>"]
 maintainers = ["Luã Bida Vacaro <luabidaa@gmail.com>"]
 license = "GNU GPL v3.0"
 repository = "https://github.com/osl-incubator/satellite-weather-downloader"
 homepage = "https://github.com/osl-incubator/satellite-weather-downloader"
```

### Comparing `satellite_weather_downloader-1.8.3/satellite/downloader/extract_reanalysis.py` & `satellite_weather_downloader-1.8.4/satellite/downloader/extract_reanalysis.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.3/satellite/downloader/reanalysis/api_vars.py` & `satellite_weather_downloader-1.8.4/satellite/downloader/reanalysis/api_vars.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.3/satellite/downloader/reanalysis/prompt.py` & `satellite_weather_downloader-1.8.4/satellite/downloader/reanalysis/prompt.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.3/satellite/downloader/request.py` & `satellite_weather_downloader-1.8.4/satellite/downloader/request.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.3/satellite/weather/_brazil/DSEI/areas.py` & `satellite_weather_downloader-1.8.4/satellite/weather/_brazil/DSEI/areas.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.3/satellite/weather/_brazil/DSEI/areas_dsei.dbf` & `satellite_weather_downloader-1.8.4/satellite/weather/_brazil/DSEI/areas_dsei.dbf`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.3/satellite/weather/_brazil/DSEI/areas_dsei.shp` & `satellite_weather_downloader-1.8.4/satellite/weather/_brazil/DSEI/areas_dsei.shp`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.3/satellite/weather/_brazil/extract_coordinates.py` & `satellite_weather_downloader-1.8.4/satellite/weather/_brazil/extract_coordinates.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.3/satellite/weather/_brazil/extract_latlons.py` & `satellite_weather_downloader-1.8.4/satellite/weather/_brazil/extract_latlons.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.3/satellite/weather/_brazil/municipios.json` & `satellite_weather_downloader-1.8.4/satellite/weather/_brazil/municipios.json`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.3/satellite/weather/utils/episem.py` & `satellite_weather_downloader-1.8.4/satellite/weather/utils/episem.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.3/satellite/weather/xr_extensions.py` & `satellite_weather_downloader-1.8.4/satellite/weather/xr_extensions.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,17 +93,17 @@
             self._geocode_to_sql(
                 geocode=geocode,
                 con=con,
                 schema=schema,
                 tablename=tablename,
                 raw=raw,
             )
-        logger.debug(
-            f'{len(geocodes)} geocodes updated on {schema}.{tablename}'
-        )
+            logger.debug(
+                f'{geocode} updated on {schema}.{tablename}'
+            )
 
     def geocode_ds(self, geocode: int, raw: bool):
         return asyncio.run(self._geocode_ds(geocode, raw))
 
     async def _final_dataframe(self, geocodes: Union[list, int], raw=False):
         geocodes = [geocodes] if isinstance(geocodes, int) else geocodes
```

### Comparing `satellite_weather_downloader-1.8.3/PKG-INFO` & `satellite_weather_downloader-1.8.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satellite-weather-downloader
-Version: 1.8.3
+Version: 1.8.4
 Summary: The modules available in this package are designed to capture and proccess satellite data from Copernicus
 Home-page: https://github.com/osl-incubator/satellite-weather-downloader
 License: GNU GPL v3.0
 Author: Luã Bida Vacaro
 Author-email: luabidaa@gmail.com
 Maintainer: Luã Bida Vacaro
 Maintainer-email: luabidaa@gmail.com
@@ -13,16 +13,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: MetPy (>=1.3.1,<2.0.0)
 Requires-Dist: SQLAlchemy (>=1.4.41,<2.0.0)
 Requires-Dist: amqp (>=5.1.1,<6.0.0)
 Requires-Dist: cdsapi (>=0.5.1,<0.6.0)
 Requires-Dist: dask (>=2023.3.1,<2024.0.0)
 Requires-Dist: geopandas (>=0.12.2,<0.13.0)
```

