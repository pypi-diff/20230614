# Comparing `tmp/mapchete-2023.6.3.tar.gz` & `tmp/mapchete-2023.6.4.tar.gz`

## Comparing `mapchete-2023.6.3.tar` & `mapchete-2023.6.4.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/__init__.py
--rw-r--r--   0        0        0    29123 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/_core.py
--rw-r--r--   0        0        0    26311 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/_executor.py
--rw-r--r--   0        0        0    32289 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/_processing.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/_registered.py
--rw-r--r--   0        0        0    16702 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/_tasks.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/_timer.py
--rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/_user_process.py
--rw-r--r--   0        0        0    48622 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/config.py
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/errors.py
--rw-r--r--   0        0        0    17833 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/index.py
--rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/log.py
--rw-r--r--   0        0        0    25097 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/path.py
--rw-r--r--   0        0        0    17515 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/stac.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/testing.py
--rw-r--r--   0        0        0    15519 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/tile.py
--rw-r--r--   0        0        0     8410 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/types.py
--rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/validate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/cli/__init__.py
--rwxr-xr-x   0        0        0      308 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/cli/main.py
--rw-r--r--   0        0        0    11005 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/cli/options.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/cli/default/__init__.py
--rw-r--r--   0        0        0     3962 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/cli/default/convert.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/cli/default/cp.py
--rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/cli/default/create.py
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/cli/default/execute.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/cli/default/formats.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/cli/default/index.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/cli/default/processes.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/cli/default/rm.py
--rwxr-xr-x   0        0        0     5035 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/cli/default/serve.py
--rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/cli/default/stac.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/commands/__init__.py
--rw-r--r--   0        0        0    15981 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/commands/_convert.py
--rw-r--r--   0        0        0     8546 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/commands/_cp.py
--rw-r--r--   0        0        0     8548 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/commands/_execute.py
--rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/commands/_index.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/commands/_rm.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/commons/__init__.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/commons/clip.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/commons/contours.py
--rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/commons/hillshade.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/formats/__init__.py
--rw-r--r--   0        0        0    20760 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/formats/base.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/formats/drivers.py
--rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/formats/loaders.py
--rw-r--r--   0        0        0    12528 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/formats/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/formats/default/__init__.py
--rw-r--r--   0        0        0     6783 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/formats/default/_fiona_base.py
--rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/formats/default/flatgeobuf.py
--rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/formats/default/geobuf.py
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/formats/default/geojson.py
--rw-r--r--   0        0        0    22184 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/formats/default/gtiff.py
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/formats/default/mapchete_input.py
--rw-r--r--   0        0        0     6935 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/formats/default/png.py
--rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/formats/default/png_hillshade.py
--rw-r--r--   0        0        0    11231 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/formats/default/raster_file.py
--rw-r--r--   0        0        0    15913 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/formats/default/tile_directory.py
--rw-r--r--   0        0        0     9450 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/formats/default/vector_file.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/io/__init__.py
--rw-r--r--   0        0        0    12038 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/io/_geometry_operations.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/io/_json.py
--rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/io/_misc.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/io/_path.py
--rw-r--r--   0        0        0    44448 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/io/raster.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/io/settings.py
--rw-r--r--   0        0        0    22010 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/io/vector.py
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/processes/__init__.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/processes/contours.py
--rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/processes/convert.py
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/processes/hillshade.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/processes/examples/__init__.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/processes/examples/example_process.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/static/__init__.py
--rw-r--r--   0        0        0     8416 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/static/index.html
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/static/mapchete_template.mapchete
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 mapchete-2023.6.3/mapchete/static/process_template.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 mapchete-2023.6.3/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 mapchete-2023.6.3/LICENSE
--rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 mapchete-2023.6.3/README.rst
--rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 mapchete-2023.6.3/pyproject.toml
--rw-r--r--   0        0        0     9061 2020-02-02 00:00:00.000000 mapchete-2023.6.3/PKG-INFO
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/__init__.py
+-rw-r--r--   0        0        0    29123 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/_core.py
+-rw-r--r--   0        0        0    26311 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/_executor.py
+-rw-r--r--   0        0        0    32289 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/_processing.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/_registered.py
+-rw-r--r--   0        0        0    16702 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/_tasks.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/_timer.py
+-rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/_user_process.py
+-rw-r--r--   0        0        0    48622 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/config.py
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/errors.py
+-rw-r--r--   0        0        0    17833 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/index.py
+-rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/log.py
+-rw-r--r--   0        0        0    25018 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/path.py
+-rw-r--r--   0        0        0    17515 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/stac.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/testing.py
+-rw-r--r--   0        0        0    15519 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/tile.py
+-rw-r--r--   0        0        0     8410 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/types.py
+-rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/validate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/cli/__init__.py
+-rwxr-xr-x   0        0        0      308 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/cli/main.py
+-rw-r--r--   0        0        0    11005 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/cli/options.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/cli/default/__init__.py
+-rw-r--r--   0        0        0     3962 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/cli/default/convert.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/cli/default/cp.py
+-rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/cli/default/create.py
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/cli/default/execute.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/cli/default/formats.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/cli/default/index.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/cli/default/processes.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/cli/default/rm.py
+-rwxr-xr-x   0        0        0     5035 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/cli/default/serve.py
+-rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/cli/default/stac.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/commands/__init__.py
+-rw-r--r--   0        0        0    15981 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/commands/_convert.py
+-rw-r--r--   0        0        0     8546 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/commands/_cp.py
+-rw-r--r--   0        0        0     8548 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/commands/_execute.py
+-rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/commands/_index.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/commands/_rm.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/commons/__init__.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/commons/clip.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/commons/contours.py
+-rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/commons/hillshade.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/formats/__init__.py
+-rw-r--r--   0        0        0    20760 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/formats/base.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/formats/drivers.py
+-rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/formats/loaders.py
+-rw-r--r--   0        0        0    12528 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/formats/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/formats/default/__init__.py
+-rw-r--r--   0        0        0     6783 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/formats/default/_fiona_base.py
+-rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/formats/default/flatgeobuf.py
+-rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/formats/default/geobuf.py
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/formats/default/geojson.py
+-rw-r--r--   0        0        0    22184 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/formats/default/gtiff.py
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/formats/default/mapchete_input.py
+-rw-r--r--   0        0        0     6935 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/formats/default/png.py
+-rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/formats/default/png_hillshade.py
+-rw-r--r--   0        0        0    11231 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/formats/default/raster_file.py
+-rw-r--r--   0        0        0    15913 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/formats/default/tile_directory.py
+-rw-r--r--   0        0        0     9450 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/formats/default/vector_file.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/io/__init__.py
+-rw-r--r--   0        0        0    12038 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/io/_geometry_operations.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/io/_json.py
+-rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/io/_misc.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/io/_path.py
+-rw-r--r--   0        0        0    44448 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/io/raster.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/io/settings.py
+-rw-r--r--   0        0        0    22010 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/io/vector.py
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/processes/__init__.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/processes/contours.py
+-rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/processes/convert.py
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/processes/hillshade.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/processes/examples/__init__.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/processes/examples/example_process.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/static/__init__.py
+-rw-r--r--   0        0        0     8416 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/static/index.html
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/static/mapchete_template.mapchete
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 mapchete-2023.6.4/mapchete/static/process_template.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 mapchete-2023.6.4/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 mapchete-2023.6.4/LICENSE
+-rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 mapchete-2023.6.4/README.rst
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 mapchete-2023.6.4/pyproject.toml
+-rw-r--r--   0        0        0     9061 2020-02-02 00:00:00.000000 mapchete-2023.6.4/PKG-INFO
```

### Comparing `mapchete-2023.6.3/mapchete/__init__.py` & `mapchete-2023.6.4/mapchete/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,11 +15,11 @@
     "ProcessInfo",
     "Timer",
     "Executor",
     "FakeFuture",
     "SkippedFuture",
     "Job",
 ]
-__version__ = "2023.6.3"
+__version__ = "2023.6.4"
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
```

### Comparing `mapchete-2023.6.3/mapchete/_core.py` & `mapchete-2023.6.4/mapchete/_core.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/_executor.py` & `mapchete-2023.6.4/mapchete/_executor.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/_processing.py` & `mapchete-2023.6.4/mapchete/_processing.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/_registered.py` & `mapchete-2023.6.4/mapchete/_registered.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/_tasks.py` & `mapchete-2023.6.4/mapchete/_tasks.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/_timer.py` & `mapchete-2023.6.4/mapchete/_timer.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/_user_process.py` & `mapchete-2023.6.4/mapchete/_user_process.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/config.py` & `mapchete-2023.6.4/mapchete/config.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/errors.py` & `mapchete-2023.6.4/mapchete/errors.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/index.py` & `mapchete-2023.6.4/mapchete/index.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/log.py` & `mapchete-2023.6.4/mapchete/log.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/path.py` & `mapchete-2023.6.4/mapchete/path.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,14 @@
             storage_options = kwargs.get("fs_options")
         if storage_options:
             self._kwargs.update(storage_options=storage_options)
         self._fs = fs
         self._storage_options = dict(
             DEFAULT_STORAGE_OPTIONS, **self._kwargs.get("storage_options") or {}
         )
-        self._fs_session = self._kwargs.get("fs_session")
 
     @staticmethod
     def from_dict(dictionary) -> "MPath":
         path_str = dictionary.get("path")
         if not path_str:
             raise ValueError(
                 f"dictionary representation requires at least a 'path' item: {dictionary}"
@@ -141,15 +140,14 @@
                 requester_pays=self._storage_options.get(
                     "requester_pays", os.environ.get("AWS_REQUEST_PAYER") == "requester"
                 ),
                 config_kwargs=dict(
                     connect_timeout=self._storage_options.get("timeout"),
                     read_timeout=self._storage_options.get("timeout"),
                 ),
-                session=self._fs_session,
                 **{
                     k: v
                     for k, v in self._storage_options.items()
                     if k not in UNALLOWED_S3_KWARGS
                 },
             )
         elif self._path_str.startswith(("http://", "https://")):
@@ -172,15 +170,14 @@
                     for k, v in self._storage_options.items()
                     if k not in UNALLOWED_HTTP_KWARGS
                 },
             )
         else:
             return fsspec.filesystem("file", **self._storage_options)
 
-    @cached_property
     def fs_session(self):
         if hasattr(self.fs, "session"):
             return self.fs.session
         else:
             return None
 
     @cached_property
@@ -353,15 +350,17 @@
                 if allowed_remote_extensions:
                     extensions = allowed_remote_extensions.split(",") + (
                         default_remote_extensions
                     )
                 extensions = default_remote_extensions + [self.suffix]
                 # make sure current path extension is added to allowed_remote_extensions
                 gdal_opts.update(
-                    CPL_VSIL_CURL_ALLOWED_EXTENSIONS=", ".join(set(extensions))
+                    CPL_VSIL_CURL_ALLOWED_EXTENSIONS=", ".join(
+                        set([ext for ext in extensions if ext != ""])
+                    )
                 )
             if self.fs.kwargs.get("auth"):
                 gdal_opts.update(
                     GDAL_HTTP_USERPWD=f"{self.fs.kwargs['auth'].login}:{self.fs.kwargs['auth'].password}"
                 )
             gdal_opts.update(user_opts)
         else:
@@ -374,17 +373,16 @@
         # GDAL parses the paths in a weird way, so we have to be careful with a custom
         # endpoint
         if hasattr(self.fs, "endpoint_url") and isinstance(self.fs.endpoint_url, str):
             return self.fs.endpoint_url.lstrip("http://").lstrip("https://")
         else:
             return None
 
-    @cached_property
     def rio_session(self) -> "rasterio.session.Session":
-        if self.fs_session:
+        if self.fs_session():
             # rasterio accepts a Session object but only a boto3.session.Session
             # object and not a aiobotocore.session.AioSession which we get from fsspec
             return RioSession.from_path(
                 self._path_str,
                 aws_access_key_id=self.fs.key,
                 aws_secret_access_key=self.fs.secret,
                 endpoint_url=self._endpoint_url,
@@ -397,29 +395,28 @@
         """Return configuration parameters for rasterio.Env()."""
         out = self.gdal_env_params(
             opts=opts,
             allowed_remote_extensions=allowed_remote_extensions,
         )
         if self.is_remote():
             out.update(
-                session=self.rio_session, AWS_VIRTUAL_HOSTING=False, AWS_HTTPS=False
+                session=self.rio_session(), AWS_VIRTUAL_HOSTING=False, AWS_HTTPS=False
             )
         return out
 
     def rio_env(self, opts=None, allowed_remote_extensions=None) -> rasterio.Env:
         """Return preconfigured rasterio.Env context manager for path."""
         return rasterio.Env(
             **self.rio_env_config(
                 opts=opts, allowed_remote_extensions=allowed_remote_extensions
             )
         )
 
-    @cached_property
     def fio_session(self) -> "fiona.session.Session":
-        if self.fs_session:
+        if self.fs_session():
             # fiona accepts a Session object but only a boto3.session.Session
             # object and not a aiobotocore.session.AioSession which we get from fsspec
             return FioSession.from_path(
                 self._path_str,
                 aws_access_key_id=self.fs.key,
                 aws_secret_access_key=self.fs.secret,
                 endpoint_url=self._endpoint_url,
@@ -432,15 +429,15 @@
         """Return configuration parameters for fiona.Env()."""
         out = self.gdal_env_params(
             opts=opts,
             allowed_remote_extensions=allowed_remote_extensions,
         )
         if self.is_remote():
             out.update(
-                session=self.fio_session, AWS_VIRTUAL_HOSTING=False, AWS_HTTPS=False
+                session=self.fio_session(), AWS_VIRTUAL_HOSTING=False, AWS_HTTPS=False
             )
         return out
 
     def fio_env(self, opts=None, allowed_remote_extensions=None) -> fiona.Env:
         """Return preconfigured fiona.Env context manager for path."""
         return fiona.Env(
             **self.fio_env_config(
```

### Comparing `mapchete-2023.6.3/mapchete/stac.py` & `mapchete-2023.6.4/mapchete/stac.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/testing.py` & `mapchete-2023.6.4/mapchete/testing.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/tile.py` & `mapchete-2023.6.4/mapchete/tile.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/types.py` & `mapchete-2023.6.4/mapchete/types.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/validate.py` & `mapchete-2023.6.4/mapchete/validate.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/cli/options.py` & `mapchete-2023.6.4/mapchete/cli/options.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/cli/default/convert.py` & `mapchete-2023.6.4/mapchete/cli/default/convert.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/cli/default/cp.py` & `mapchete-2023.6.4/mapchete/cli/default/cp.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/cli/default/create.py` & `mapchete-2023.6.4/mapchete/cli/default/create.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/cli/default/execute.py` & `mapchete-2023.6.4/mapchete/cli/default/execute.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/cli/default/formats.py` & `mapchete-2023.6.4/mapchete/cli/default/formats.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/cli/default/index.py` & `mapchete-2023.6.4/mapchete/cli/default/index.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/cli/default/processes.py` & `mapchete-2023.6.4/mapchete/cli/default/processes.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/cli/default/rm.py` & `mapchete-2023.6.4/mapchete/cli/default/rm.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/cli/default/serve.py` & `mapchete-2023.6.4/mapchete/cli/default/serve.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/cli/default/stac.py` & `mapchete-2023.6.4/mapchete/cli/default/stac.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/commands/_convert.py` & `mapchete-2023.6.4/mapchete/commands/_convert.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/commands/_cp.py` & `mapchete-2023.6.4/mapchete/commands/_cp.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/commands/_execute.py` & `mapchete-2023.6.4/mapchete/commands/_execute.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/commands/_index.py` & `mapchete-2023.6.4/mapchete/commands/_index.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/commands/_rm.py` & `mapchete-2023.6.4/mapchete/commands/_rm.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/commons/clip.py` & `mapchete-2023.6.4/mapchete/commons/clip.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/commons/contours.py` & `mapchete-2023.6.4/mapchete/commons/contours.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/commons/hillshade.py` & `mapchete-2023.6.4/mapchete/commons/hillshade.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/formats/__init__.py` & `mapchete-2023.6.4/mapchete/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/formats/base.py` & `mapchete-2023.6.4/mapchete/formats/base.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/formats/loaders.py` & `mapchete-2023.6.4/mapchete/formats/loaders.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/formats/tools.py` & `mapchete-2023.6.4/mapchete/formats/tools.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/formats/default/_fiona_base.py` & `mapchete-2023.6.4/mapchete/formats/default/_fiona_base.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/formats/default/flatgeobuf.py` & `mapchete-2023.6.4/mapchete/formats/default/flatgeobuf.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/formats/default/geobuf.py` & `mapchete-2023.6.4/mapchete/formats/default/geobuf.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/formats/default/geojson.py` & `mapchete-2023.6.4/mapchete/formats/default/geojson.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/formats/default/gtiff.py` & `mapchete-2023.6.4/mapchete/formats/default/gtiff.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/formats/default/mapchete_input.py` & `mapchete-2023.6.4/mapchete/formats/default/mapchete_input.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/formats/default/png.py` & `mapchete-2023.6.4/mapchete/formats/default/png.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/formats/default/png_hillshade.py` & `mapchete-2023.6.4/mapchete/formats/default/png_hillshade.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/formats/default/raster_file.py` & `mapchete-2023.6.4/mapchete/formats/default/raster_file.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/formats/default/tile_directory.py` & `mapchete-2023.6.4/mapchete/formats/default/tile_directory.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/formats/default/vector_file.py` & `mapchete-2023.6.4/mapchete/formats/default/vector_file.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/io/__init__.py` & `mapchete-2023.6.4/mapchete/io/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/io/_geometry_operations.py` & `mapchete-2023.6.4/mapchete/io/_geometry_operations.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/io/_json.py` & `mapchete-2023.6.4/mapchete/io/_json.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/io/_misc.py` & `mapchete-2023.6.4/mapchete/io/_misc.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/io/raster.py` & `mapchete-2023.6.4/mapchete/io/raster.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/io/settings.py` & `mapchete-2023.6.4/mapchete/io/settings.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/io/vector.py` & `mapchete-2023.6.4/mapchete/io/vector.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/processes/__init__.py` & `mapchete-2023.6.4/mapchete/processes/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/processes/contours.py` & `mapchete-2023.6.4/mapchete/processes/contours.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/processes/convert.py` & `mapchete-2023.6.4/mapchete/processes/convert.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/processes/hillshade.py` & `mapchete-2023.6.4/mapchete/processes/hillshade.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/processes/examples/example_process.py` & `mapchete-2023.6.4/mapchete/processes/examples/example_process.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/static/index.html` & `mapchete-2023.6.4/mapchete/static/index.html`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/mapchete/static/process_template.py` & `mapchete-2023.6.4/mapchete/static/process_template.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/LICENSE` & `mapchete-2023.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/README.rst` & `mapchete-2023.6.4/README.rst`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/pyproject.toml` & `mapchete-2023.6.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mapchete-2023.6.3/PKG-INFO` & `mapchete-2023.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapchete
-Version: 2023.6.3
+Version: 2023.6.4
 Summary: Tile-based geodata processing using rasterio & Fiona
 Project-URL: Homepage, https://github.com/ungarj/mapchete
 Author-email: Joachim Ungar <joachim.ungar@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

