# Comparing `tmp/descarteslabs-2.0.0.tar.gz` & `tmp/descarteslabs-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "descarteslabs-2.0.0.tar", last modified: Mon Jun 12 20:04:12 2023, max compression
+gzip compressed data, was "descarteslabs-2.0.1.tar", last modified: Wed Jun 14 16:23:02 2023, max compression
```

## Comparing `descarteslabs-2.0.0.tar` & `descarteslabs-2.0.1.tar`

### file list

```diff
@@ -1,243 +1,243 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.738190 descarteslabs-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-12 20:04:12.738190 descarteslabs-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    85194 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.710188 descarteslabs-2.0.0/descarteslabs/
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.710188 descarteslabs-2.0.0/descarteslabs/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29383 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/auth/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.710188 descarteslabs-2.0.0/descarteslabs/auth/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/auth/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16934 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/auth/tests/test_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.710188 descarteslabs-2.0.0/descarteslabs/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/catalog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.710188 descarteslabs-2.0.0/descarteslabs/compute/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/compute/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.710188 descarteslabs-2.0.0/descarteslabs/config/
--rw-r--r--   0 runner    (1001) docker     (123)    10119 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/config/settings.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.710188 descarteslabs-2.0.0/descarteslabs/config/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/config/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13316 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/config/tests/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.710188 descarteslabs-2.0.0/descarteslabs/core/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.714188 descarteslabs-2.0.0/descarteslabs/core/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64062 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/catalog/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    36605 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/catalog/band.py
--rw-r--r--   0 runner    (1001) docker     (123)    29762 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/catalog/blob.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/catalog/blob_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/catalog/blob_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)    37861 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/catalog/catalog_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/catalog/catalog_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/catalog/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    63243 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/catalog/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    50022 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/catalog/image_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/catalog/image_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    17853 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/catalog/image_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/catalog/named_catalog_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    21970 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/catalog/product.py
--rw-r--r--   0 runner    (1001) docker     (123)    26305 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/catalog/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)    21847 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/catalog/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.714188 descarteslabs-2.0.0/descarteslabs/core/catalog/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/catalog/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/catalog/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   118250 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/catalog/tests/mock_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    36523 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/catalog/tests/test_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    28972 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/catalog/tests/test_band.py
--rw-r--r--   0 runner    (1001) docker     (123)    16050 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/catalog/tests/test_catalog_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/catalog/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/catalog/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    45554 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/catalog/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    14560 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/catalog/tests/test_image_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    25515 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/catalog/tests/test_image_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)    28485 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/catalog/tests/test_product.py
--rw-r--r--   0 runner    (1001) docker     (123)    30418 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/catalog/tests/test_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)    20303 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/catalog/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/catalog/tests/test_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.714188 descarteslabs-2.0.0/descarteslabs/core/client/
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/addons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.714188 descarteslabs-2.0.0/descarteslabs/core/client/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/auth/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.714188 descarteslabs-2.0.0/descarteslabs/core/client/auth/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/auth/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/auth/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.722189 descarteslabs-2.0.0/descarteslabs/core/client/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/scripts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/scripts/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.722189 descarteslabs-2.0.0/descarteslabs/core/client/scripts/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/scripts/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/scripts/tests/test_scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.722189 descarteslabs-2.0.0/descarteslabs/core/client/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.722189 descarteslabs-2.0.0/descarteslabs/core/client/services/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/services/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/services/metadata/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    35310 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/services/metadata/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.722189 descarteslabs-2.0.0/descarteslabs/core/client/services/metadata/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/services/metadata/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.722189 descarteslabs-2.0.0/descarteslabs/core/client/services/metadata/tests/e2e/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/services/metadata/tests/e2e/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/services/metadata/tests/e2e/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/services/metadata/tests/test_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.726189 descarteslabs-2.0.0/descarteslabs/core/client/services/raster/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/services/raster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/services/raster/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    14392 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/services/raster/geotiff_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    33564 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/services/raster/raster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.726189 descarteslabs-2.0.0/descarteslabs/core/client/services/raster/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/services/raster/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.726189 descarteslabs-2.0.0/descarteslabs/core/client/services/raster/tests/e2e/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/services/raster/tests/e2e/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41637 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/services/raster/tests/e2e/iowa_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    14970 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/services/raster/tests/e2e/test_raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/services/raster/tests/test_geotiff_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/services/raster/tests/test_raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/services/raster/tests/test_raster_rasterio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.726189 descarteslabs-2.0.0/descarteslabs/core/client/services/service/
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/services/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/services/service/api_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    29553 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/services/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.726189 descarteslabs-2.0.0/descarteslabs/core/client/services/service/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/services/service/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19843 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/services/service/tests/test_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.726189 descarteslabs-2.0.0/descarteslabs/core/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.726189 descarteslabs-2.0.0/descarteslabs/core/common/client/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/client/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/client/document.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.730189 descarteslabs-2.0.0/descarteslabs/core/common/client/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/client/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/client/tests/test_attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.730189 descarteslabs-2.0.0/descarteslabs/core/common/collection/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15722 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/collection/collection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.730189 descarteslabs-2.0.0/descarteslabs/core/common/collection/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/collection/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/collection/tests/test_collection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.730189 descarteslabs-2.0.0/descarteslabs/core/common/display/
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/display/_display.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.730189 descarteslabs-2.0.0/descarteslabs/core/common/display/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/display/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/display/tests/test_display.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.730189 descarteslabs-2.0.0/descarteslabs/core/common/dltile/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/dltile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/dltile/_tiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/dltile/conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/dltile/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/dltile/rasterize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.730189 descarteslabs-2.0.0/descarteslabs/core/common/dltile/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/dltile/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/dltile/tests/test_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11665 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/dltile/tests/test_dltiles.py
--rw-r--r--   0 runner    (1001) docker     (123)    19529 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/dltile/tile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/dltile/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11527 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/dltile/utm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.734190 descarteslabs-2.0.0/descarteslabs/core/common/dotdict/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/dotdict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16257 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/dotdict/dotdict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.734190 descarteslabs-2.0.0/descarteslabs/core/common/dotdict/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/dotdict/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14087 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/dotdict/tests/test_dotdict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.734190 descarteslabs-2.0.0/descarteslabs/core/common/geo/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/geo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53135 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/geo/geocontext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.734190 descarteslabs-2.0.0/descarteslabs/core/common/geo/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/geo/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23527 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/geo/tests/test_geocontext.py
--rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/geo/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/geo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.734190 descarteslabs-2.0.0/descarteslabs/core/common/http/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/http/authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/http/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/http/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/http/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/http/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.734190 descarteslabs-2.0.0/descarteslabs/core/common/http/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/http/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/http/tests/test_authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/http/tests/test_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/http/tests/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/http/tests/test_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.734190 descarteslabs-2.0.0/descarteslabs/core/common/property_filtering/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/property_filtering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16486 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/property_filtering/filtering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.734190 descarteslabs-2.0.0/descarteslabs/core/common/property_filtering/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/property_filtering/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/property_filtering/tests/test_filtering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.734190 descarteslabs-2.0.0/descarteslabs/core/common/registry/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/registry/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.734190 descarteslabs-2.0.0/descarteslabs/core/common/retry/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/retry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8281 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/retry/retry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.738190 descarteslabs-2.0.0/descarteslabs/core/common/retry/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/retry/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/retry/tests/test_retry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.738190 descarteslabs-2.0.0/descarteslabs/core/common/shapely_support/
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/shapely_support/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.738190 descarteslabs-2.0.0/descarteslabs/core/common/shapely_support/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/shapely_support/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/shapely_support/tests/test_shapely_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.738190 descarteslabs-2.0.0/descarteslabs/core/common/threading/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/threading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/threading/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.738190 descarteslabs-2.0.0/descarteslabs/core/common/threading/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/threading/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/common/threading/tests/test_local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.738190 descarteslabs-2.0.0/descarteslabs/core/compute/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26184 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/compute/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/compute/compute_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.738190 descarteslabs-2.0.0/descarteslabs/core/compute/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/compute/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/compute/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/compute/tests/test_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/compute/tests/test_job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.738190 descarteslabs-2.0.0/descarteslabs/core/geo/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/geo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.738190 descarteslabs-2.0.0/descarteslabs/core/scenes/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/scenes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/scenes/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    33638 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/scenes/scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    28225 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/scenes/scenecollection.py
--rw-r--r--   0 runner    (1001) docker     (123)    12610 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/scenes/search_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.738190 descarteslabs-2.0.0/descarteslabs/core/scenes/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/scenes/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/scenes/tests/mock_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/scenes/tests/test_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/scenes/tests/test_scenecollection.py
--rw-r--r--   0 runner    (1001) docker     (123)    16157 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/scenes/tests/test_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.738190 descarteslabs-2.0.0/descarteslabs/core/third_party/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/third_party/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.738190 descarteslabs-2.0.0/descarteslabs/core/third_party/boltons/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/third_party/boltons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32185 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/third_party/boltons/funcutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.738190 descarteslabs-2.0.0/descarteslabs/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.738190 descarteslabs-2.0.0/descarteslabs/geo/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/geo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.738190 descarteslabs-2.0.0/descarteslabs/scenes/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/scenes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.738190 descarteslabs-2.0.0/descarteslabs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/descarteslabs/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:04:12.710188 descarteslabs-2.0.0/descarteslabs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-12 20:04:12.000000 descarteslabs-2.0.0/descarteslabs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8354 2023-06-12 20:04:12.000000 descarteslabs-2.0.0/descarteslabs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 20:04:12.000000 descarteslabs-2.0.0/descarteslabs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-12 20:04:12.000000 descarteslabs-2.0.0/descarteslabs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-12 20:04:12.000000 descarteslabs-2.0.0/descarteslabs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-12 20:04:12.000000 descarteslabs-2.0.0/descarteslabs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 20:04:12.738190 descarteslabs-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-06-12 20:04:07.000000 descarteslabs-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.282386 descarteslabs-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-14 16:23:02.282386 descarteslabs-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    85441 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.266386 descarteslabs-2.0.1/descarteslabs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.266386 descarteslabs-2.0.1/descarteslabs/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29383 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/auth/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.266386 descarteslabs-2.0.1/descarteslabs/auth/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/auth/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16934 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/auth/tests/test_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.266386 descarteslabs-2.0.1/descarteslabs/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/catalog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.266386 descarteslabs-2.0.1/descarteslabs/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/compute/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.266386 descarteslabs-2.0.1/descarteslabs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)    10119 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/config/settings.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.266386 descarteslabs-2.0.1/descarteslabs/config/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/config/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13316 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/config/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.266386 descarteslabs-2.0.1/descarteslabs/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.270386 descarteslabs-2.0.1/descarteslabs/core/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64062 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/catalog/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36605 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/catalog/band.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29762 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/catalog/blob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/catalog/blob_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/catalog/blob_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37861 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/catalog/catalog_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/catalog/catalog_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/catalog/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63243 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/catalog/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50022 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/catalog/image_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/catalog/image_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17853 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/catalog/image_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/catalog/named_catalog_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21970 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/catalog/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26305 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/catalog/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21847 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/catalog/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.270386 descarteslabs-2.0.1/descarteslabs/core/catalog/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/catalog/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/catalog/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118250 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/catalog/tests/mock_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36523 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/catalog/tests/test_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28972 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/catalog/tests/test_band.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16050 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/catalog/tests/test_catalog_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/catalog/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/catalog/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45554 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/catalog/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14560 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/catalog/tests/test_image_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25515 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/catalog/tests/test_image_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28485 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/catalog/tests/test_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30418 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/catalog/tests/test_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20303 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/catalog/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/catalog/tests/test_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.270386 descarteslabs-2.0.1/descarteslabs/core/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/addons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.270386 descarteslabs-2.0.1/descarteslabs/core/client/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/auth/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.270386 descarteslabs-2.0.1/descarteslabs/core/client/auth/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/auth/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/auth/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.270386 descarteslabs-2.0.1/descarteslabs/core/client/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/scripts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/scripts/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.270386 descarteslabs-2.0.1/descarteslabs/core/client/scripts/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/scripts/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/scripts/tests/test_scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.270386 descarteslabs-2.0.1/descarteslabs/core/client/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.270386 descarteslabs-2.0.1/descarteslabs/core/client/services/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/services/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/services/metadata/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35310 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/services/metadata/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.270386 descarteslabs-2.0.1/descarteslabs/core/client/services/metadata/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/services/metadata/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.270386 descarteslabs-2.0.1/descarteslabs/core/client/services/metadata/tests/e2e/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/services/metadata/tests/e2e/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/services/metadata/tests/e2e/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/services/metadata/tests/test_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.274386 descarteslabs-2.0.1/descarteslabs/core/client/services/raster/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/services/raster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/services/raster/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14392 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/services/raster/geotiff_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33684 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/services/raster/raster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.274386 descarteslabs-2.0.1/descarteslabs/core/client/services/raster/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/services/raster/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.274386 descarteslabs-2.0.1/descarteslabs/core/client/services/raster/tests/e2e/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/services/raster/tests/e2e/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41637 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/services/raster/tests/e2e/iowa_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14970 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/services/raster/tests/e2e/test_raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/services/raster/tests/test_geotiff_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/services/raster/tests/test_raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/services/raster/tests/test_raster_rasterio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.274386 descarteslabs-2.0.1/descarteslabs/core/client/services/service/
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/services/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/services/service/api_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29553 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/services/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.274386 descarteslabs-2.0.1/descarteslabs/core/client/services/service/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/services/service/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19843 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/services/service/tests/test_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.274386 descarteslabs-2.0.1/descarteslabs/core/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.274386 descarteslabs-2.0.1/descarteslabs/core/common/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/client/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/client/document.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.274386 descarteslabs-2.0.1/descarteslabs/core/common/client/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/client/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/client/tests/test_attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.274386 descarteslabs-2.0.1/descarteslabs/core/common/collection/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15722 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/collection/collection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.274386 descarteslabs-2.0.1/descarteslabs/core/common/collection/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/collection/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/collection/tests/test_collection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.274386 descarteslabs-2.0.1/descarteslabs/core/common/display/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/display/_display.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.274386 descarteslabs-2.0.1/descarteslabs/core/common/display/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/display/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/display/tests/test_display.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.274386 descarteslabs-2.0.1/descarteslabs/core/common/dltile/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/dltile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/dltile/_tiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/dltile/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/dltile/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/dltile/rasterize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.274386 descarteslabs-2.0.1/descarteslabs/core/common/dltile/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/dltile/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/dltile/tests/test_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11665 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/dltile/tests/test_dltiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19529 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/dltile/tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/dltile/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11527 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/dltile/utm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.274386 descarteslabs-2.0.1/descarteslabs/core/common/dotdict/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/dotdict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16257 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/dotdict/dotdict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.274386 descarteslabs-2.0.1/descarteslabs/core/common/dotdict/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/dotdict/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14087 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/dotdict/tests/test_dotdict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.274386 descarteslabs-2.0.1/descarteslabs/core/common/geo/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/geo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53135 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/geo/geocontext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.278386 descarteslabs-2.0.1/descarteslabs/core/common/geo/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/geo/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23527 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/geo/tests/test_geocontext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/geo/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/geo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.278386 descarteslabs-2.0.1/descarteslabs/core/common/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/http/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/http/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/http/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/http/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/http/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.278386 descarteslabs-2.0.1/descarteslabs/core/common/http/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/http/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/http/tests/test_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/http/tests/test_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/http/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/http/tests/test_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.278386 descarteslabs-2.0.1/descarteslabs/core/common/property_filtering/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/property_filtering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16486 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/property_filtering/filtering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.278386 descarteslabs-2.0.1/descarteslabs/core/common/property_filtering/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/property_filtering/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/property_filtering/tests/test_filtering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.278386 descarteslabs-2.0.1/descarteslabs/core/common/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/registry/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.278386 descarteslabs-2.0.1/descarteslabs/core/common/retry/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/retry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8281 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/retry/retry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.278386 descarteslabs-2.0.1/descarteslabs/core/common/retry/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/retry/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/retry/tests/test_retry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.278386 descarteslabs-2.0.1/descarteslabs/core/common/shapely_support/
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/shapely_support/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.278386 descarteslabs-2.0.1/descarteslabs/core/common/shapely_support/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/shapely_support/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/shapely_support/tests/test_shapely_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.278386 descarteslabs-2.0.1/descarteslabs/core/common/threading/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/threading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/threading/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.278386 descarteslabs-2.0.1/descarteslabs/core/common/threading/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/threading/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/common/threading/tests/test_local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.278386 descarteslabs-2.0.1/descarteslabs/core/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26184 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/compute/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/compute/compute_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.278386 descarteslabs-2.0.1/descarteslabs/core/compute/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/compute/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/compute/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/compute/tests/test_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/compute/tests/test_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.278386 descarteslabs-2.0.1/descarteslabs/core/geo/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/geo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.278386 descarteslabs-2.0.1/descarteslabs/core/scenes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/scenes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/scenes/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33638 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/scenes/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28225 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/scenes/scenecollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12610 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/scenes/search_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.282386 descarteslabs-2.0.1/descarteslabs/core/scenes/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/scenes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/scenes/tests/mock_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/scenes/tests/test_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/scenes/tests/test_scenecollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16157 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/scenes/tests/test_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.282386 descarteslabs-2.0.1/descarteslabs/core/third_party/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/third_party/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.282386 descarteslabs-2.0.1/descarteslabs/core/third_party/boltons/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/third_party/boltons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32185 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/third_party/boltons/funcutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.282386 descarteslabs-2.0.1/descarteslabs/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.282386 descarteslabs-2.0.1/descarteslabs/geo/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/geo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.282386 descarteslabs-2.0.1/descarteslabs/scenes/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/scenes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.282386 descarteslabs-2.0.1/descarteslabs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/descarteslabs/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:23:02.266386 descarteslabs-2.0.1/descarteslabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-14 16:23:02.000000 descarteslabs-2.0.1/descarteslabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8354 2023-06-14 16:23:02.000000 descarteslabs-2.0.1/descarteslabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 16:23:02.000000 descarteslabs-2.0.1/descarteslabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-14 16:23:02.000000 descarteslabs-2.0.1/descarteslabs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-14 16:23:02.000000 descarteslabs-2.0.1/descarteslabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-14 16:23:02.000000 descarteslabs-2.0.1/descarteslabs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 16:23:02.282386 descarteslabs-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-06-14 16:22:55.000000 descarteslabs-2.0.1/setup.py
```

### Comparing `descarteslabs-2.0.0/LICENSE` & `descarteslabs-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/PKG-INFO` & `descarteslabs-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: descarteslabs
-Version: 2.0.0
+Version: 2.0.1
 Summary: Descartes Labs Python Client
 Home-page: https://github.com/descarteslabs/descarteslabs-python
 Author: Descartes Labs
 Author-email: hello@descarteslabs.com
 License: Apache 2.0
-Download-URL: https://github.com/descarteslabs/descarteslabs-python/archive/v2.0.0.tar.gz
+Download-URL: https://github.com/descarteslabs/descarteslabs-python/archive/v2.0.1.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `descarteslabs-2.0.0/README.md` & `descarteslabs-2.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,20 @@
 The `descarteslabs` python package, available at [https://pypi.org/project/descarteslabs/](https://pypi.org/project/descarteslabs/), provides client-side access to the Descartes Labs Platform for our customers. You must be a registered customer with access to our Descartes Labs Platform before you can make use of this package with our platform.
 
 The documentation for the latest release can be found at [https://docs.descarteslabs.com](https://docs.descarteslabs.com). For any issues please request Customer Support at [https://support.descarteslabs.com](https://support.descarteslabs.com).
 
 Changelog
 =========
 
+## [2.0.1] - 2023-06-14
+
+### Raster
+
+- Due to recent changes in `urllib3`, rastering operations were failing to retry certain errors which ought to be retried, causing more failures to propagate to the user than was desirable. This is now fixed.
+
 ## [2.0.0] - 2023-06-12
 
 (Release notes from all the 2.0.0 release candidates are summarized here for completeness.)
 
 ### Supported platforms
 
 - Deprecated support for Python 3.7 (will end of life in July).
```

### Comparing `descarteslabs-2.0.0/descarteslabs/__init__.py` & `descarteslabs-2.0.1/descarteslabs/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/auth/__init__.py` & `descarteslabs-2.0.1/descarteslabs/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/auth/auth.py` & `descarteslabs-2.0.1/descarteslabs/auth/auth.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/auth/tests/test_auth.py` & `descarteslabs-2.0.1/descarteslabs/auth/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/catalog/__init__.py` & `descarteslabs-2.0.1/descarteslabs/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/compute/__init__.py` & `descarteslabs-2.0.1/descarteslabs/compute/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/config/__init__.py` & `descarteslabs-2.0.1/descarteslabs/config/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/config/settings.toml` & `descarteslabs-2.0.1/descarteslabs/config/settings.toml`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/config/tests/test_config.py` & `descarteslabs-2.0.1/descarteslabs/config/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/catalog/__init__.py` & `descarteslabs-2.0.1/descarteslabs/core/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/catalog/attributes.py` & `descarteslabs-2.0.1/descarteslabs/core/catalog/attributes.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/catalog/band.py` & `descarteslabs-2.0.1/descarteslabs/core/catalog/band.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/catalog/blob.py` & `descarteslabs-2.0.1/descarteslabs/core/catalog/blob.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/catalog/blob_download.py` & `descarteslabs-2.0.1/descarteslabs/core/catalog/blob_download.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/catalog/blob_upload.py` & `descarteslabs-2.0.1/descarteslabs/core/catalog/blob_upload.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/catalog/catalog_base.py` & `descarteslabs-2.0.1/descarteslabs/core/catalog/catalog_base.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/catalog/catalog_client.py` & `descarteslabs-2.0.1/descarteslabs/core/catalog/catalog_client.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/catalog/helpers.py` & `descarteslabs-2.0.1/descarteslabs/core/catalog/helpers.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/catalog/image.py` & `descarteslabs-2.0.1/descarteslabs/core/catalog/image.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/catalog/image_collection.py` & `descarteslabs-2.0.1/descarteslabs/core/catalog/image_collection.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/catalog/image_types.py` & `descarteslabs-2.0.1/descarteslabs/core/catalog/image_types.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/catalog/image_upload.py` & `descarteslabs-2.0.1/descarteslabs/core/catalog/image_upload.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/catalog/named_catalog_base.py` & `descarteslabs-2.0.1/descarteslabs/core/catalog/named_catalog_base.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/catalog/product.py` & `descarteslabs-2.0.1/descarteslabs/core/catalog/product.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/catalog/scaling.py` & `descarteslabs-2.0.1/descarteslabs/core/catalog/scaling.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/catalog/search.py` & `descarteslabs-2.0.1/descarteslabs/core/catalog/search.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/catalog/tests/base.py` & `descarteslabs-2.0.1/descarteslabs/core/catalog/tests/base.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/catalog/tests/mock_data.py` & `descarteslabs-2.0.1/descarteslabs/core/catalog/tests/mock_data.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/catalog/tests/test_attributes.py` & `descarteslabs-2.0.1/descarteslabs/core/catalog/tests/test_attributes.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/catalog/tests/test_band.py` & `descarteslabs-2.0.1/descarteslabs/core/catalog/tests/test_band.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/catalog/tests/test_catalog_base.py` & `descarteslabs-2.0.1/descarteslabs/core/catalog/tests/test_catalog_base.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/catalog/tests/test_download.py` & `descarteslabs-2.0.1/descarteslabs/core/catalog/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/catalog/tests/test_filters.py` & `descarteslabs-2.0.1/descarteslabs/core/catalog/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/catalog/tests/test_image.py` & `descarteslabs-2.0.1/descarteslabs/core/catalog/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/catalog/tests/test_image_collection.py` & `descarteslabs-2.0.1/descarteslabs/core/catalog/tests/test_image_collection.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/catalog/tests/test_image_upload.py` & `descarteslabs-2.0.1/descarteslabs/core/catalog/tests/test_image_upload.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/catalog/tests/test_product.py` & `descarteslabs-2.0.1/descarteslabs/core/catalog/tests/test_product.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/catalog/tests/test_scaling.py` & `descarteslabs-2.0.1/descarteslabs/core/catalog/tests/test_scaling.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/catalog/tests/test_search.py` & `descarteslabs-2.0.1/descarteslabs/core/catalog/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/catalog/tests/test_summary.py` & `descarteslabs-2.0.1/descarteslabs/core/catalog/tests/test_summary.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/client/__init__.py` & `descarteslabs-2.0.1/descarteslabs/core/client/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/client/addons.py` & `descarteslabs-2.0.1/descarteslabs/core/client/addons.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/client/auth/cli.py` & `descarteslabs-2.0.1/descarteslabs/core/client/auth/cli.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/client/auth/tests/test_cli.py` & `descarteslabs-2.0.1/descarteslabs/core/client/auth/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/client/deprecation.py` & `descarteslabs-2.0.1/descarteslabs/core/client/deprecation.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/client/exceptions.py` & `descarteslabs-2.0.1/descarteslabs/core/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/client/scripts/__main__.py` & `descarteslabs-2.0.1/descarteslabs/core/client/scripts/__main__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/client/scripts/cli.py` & `descarteslabs-2.0.1/descarteslabs/core/client/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/client/scripts/tests/test_scripts.py` & `descarteslabs-2.0.1/descarteslabs/core/client/scripts/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/client/services/metadata/__init__.py` & `descarteslabs-2.0.1/descarteslabs/core/client/services/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/client/services/metadata/cli.py` & `descarteslabs-2.0.1/descarteslabs/core/client/services/metadata/cli.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/client/services/metadata/metadata.py` & `descarteslabs-2.0.1/descarteslabs/core/client/services/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/client/services/metadata/tests/e2e/test_metadata.py` & `descarteslabs-2.0.1/descarteslabs/core/client/services/metadata/tests/e2e/test_metadata.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/client/services/metadata/tests/test_metadata.py` & `descarteslabs-2.0.1/descarteslabs/core/client/services/metadata/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/client/services/raster/__init__.py` & `descarteslabs-2.0.1/descarteslabs/core/client/services/raster/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/client/services/raster/cli.py` & `descarteslabs-2.0.1/descarteslabs/core/client/services/raster/cli.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/client/services/raster/geotiff_utils.py` & `descarteslabs-2.0.1/descarteslabs/core/client/services/raster/geotiff_utils.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/client/services/raster/raster.py` & `descarteslabs-2.0.1/descarteslabs/core/client/services/raster/raster.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import blosc
 import numpy as np
 from descarteslabs.auth import Auth
 from descarteslabs.config import get_settings
 from descarteslabs.exceptions import ServerError
 from PIL import Image
 from tqdm import tqdm
-from urllib3.exceptions import IncompleteRead, ProtocolError
+from urllib3.exceptions import IncompleteRead, ProtocolError, ReadTimeoutError
 
 from ....common.dltile import Tile
 from ....common.http.service import DefaultClientMixin
 from ..service.service import Service
 from .geotiff_utils import make_geotiff
 
 DEFAULT_MAX_WORKERS = 8
@@ -205,17 +205,18 @@
         headers = {}
 
     while True:
         headers["x-retry-count"] = str(retry_count)
 
         try:
             return req(headers=headers)
-        except (IncompleteRead, ProtocolError, ServerError):
+        except (IncompleteRead, ProtocolError, ReadTimeoutError, ServerError):
             # IncompleteRead: Response length doesn’t match expected Content-Length
             # ProtocolError: Something unexpected happened mid-request/response
+            # ReadTimeoutError: timeout occurred while reading response from server
             # ServerError: the usual retryable bad status >= 500. Normally won't
             # occur thanks to the client Retry configuration.
             if retry_count == MAX_RETRIES:
                 raise
         # MaxRetry and all other ClientError types will be raised to our caller
 
         if retry_count:
```

### Comparing `descarteslabs-2.0.0/descarteslabs/core/client/services/raster/tests/e2e/iowa_geometry.py` & `descarteslabs-2.0.1/descarteslabs/core/client/services/raster/tests/e2e/iowa_geometry.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/client/services/raster/tests/e2e/test_raster.py` & `descarteslabs-2.0.1/descarteslabs/core/client/services/raster/tests/e2e/test_raster.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/client/services/raster/tests/test_geotiff_utils.py` & `descarteslabs-2.0.1/descarteslabs/core/client/services/raster/tests/test_geotiff_utils.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/client/services/raster/tests/test_raster.py` & `descarteslabs-2.0.1/descarteslabs/core/client/services/raster/tests/test_raster.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/client/services/raster/tests/test_raster_rasterio.py` & `descarteslabs-2.0.1/descarteslabs/core/client/services/raster/tests/test_raster_rasterio.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/client/services/service/__init__.py` & `descarteslabs-2.0.1/descarteslabs/core/client/services/service/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/client/services/service/api_service.py` & `descarteslabs-2.0.1/descarteslabs/core/client/services/service/api_service.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/client/services/service/service.py` & `descarteslabs-2.0.1/descarteslabs/core/client/services/service/service.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/client/services/service/tests/test_service.py` & `descarteslabs-2.0.1/descarteslabs/core/client/services/service/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/client/version.py` & `descarteslabs-2.0.1/descarteslabs/core/client/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "2.0.0"
+__version__ = "2.0.1"
```

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/client/__init__.py` & `descarteslabs-2.0.1/descarteslabs/core/common/client/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/client/attributes.py` & `descarteslabs-2.0.1/descarteslabs/core/common/client/attributes.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/client/document.py` & `descarteslabs-2.0.1/descarteslabs/core/common/client/document.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/client/tests/test_attributes.py` & `descarteslabs-2.0.1/descarteslabs/core/common/client/tests/test_attributes.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/collection/__init__.py` & `descarteslabs-2.0.1/descarteslabs/core/common/collection/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/collection/collection.py` & `descarteslabs-2.0.1/descarteslabs/core/common/collection/collection.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/collection/tests/test_collection.py` & `descarteslabs-2.0.1/descarteslabs/core/common/collection/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/display/__init__.py` & `descarteslabs-2.0.1/descarteslabs/core/common/display/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/display/_display.py` & `descarteslabs-2.0.1/descarteslabs/core/common/display/_display.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/display/tests/test_display.py` & `descarteslabs-2.0.1/descarteslabs/core/common/display/tests/test_display.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/dltile/__init__.py` & `descarteslabs-2.0.1/descarteslabs/core/common/dltile/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/dltile/_tiling.py` & `descarteslabs-2.0.1/descarteslabs/core/common/dltile/_tiling.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/dltile/conversions.py` & `descarteslabs-2.0.1/descarteslabs/core/common/dltile/conversions.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/dltile/exceptions.py` & `descarteslabs-2.0.1/descarteslabs/core/common/dltile/exceptions.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/dltile/rasterize.py` & `descarteslabs-2.0.1/descarteslabs/core/common/dltile/rasterize.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/dltile/tests/test_conversions.py` & `descarteslabs-2.0.1/descarteslabs/core/common/dltile/tests/test_conversions.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/dltile/tests/test_dltiles.py` & `descarteslabs-2.0.1/descarteslabs/core/common/dltile/tests/test_dltiles.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/dltile/tile.py` & `descarteslabs-2.0.1/descarteslabs/core/common/dltile/tile.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/dltile/utils.py` & `descarteslabs-2.0.1/descarteslabs/core/common/dltile/utils.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/dltile/utm.py` & `descarteslabs-2.0.1/descarteslabs/core/common/dltile/utm.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/dotdict/__init__.py` & `descarteslabs-2.0.1/descarteslabs/core/common/dotdict/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/dotdict/dotdict.py` & `descarteslabs-2.0.1/descarteslabs/core/common/dotdict/dotdict.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/dotdict/tests/test_dotdict.py` & `descarteslabs-2.0.1/descarteslabs/core/common/dotdict/tests/test_dotdict.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/geo/__init__.py` & `descarteslabs-2.0.1/descarteslabs/core/common/geo/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/geo/geocontext.py` & `descarteslabs-2.0.1/descarteslabs/core/common/geo/geocontext.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/geo/tests/test_geocontext.py` & `descarteslabs-2.0.1/descarteslabs/core/common/geo/tests/test_geocontext.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/geo/tests/test_utils.py` & `descarteslabs-2.0.1/descarteslabs/core/common/geo/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/geo/utils.py` & `descarteslabs-2.0.1/descarteslabs/core/common/geo/utils.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/http/__init__.py` & `descarteslabs-2.0.1/descarteslabs/core/common/http/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/http/authorization.py` & `descarteslabs-2.0.1/descarteslabs/core/common/http/authorization.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/http/proxy.py` & `descarteslabs-2.0.1/descarteslabs/core/common/http/proxy.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/http/retry.py` & `descarteslabs-2.0.1/descarteslabs/core/common/http/retry.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/http/service.py` & `descarteslabs-2.0.1/descarteslabs/core/common/http/service.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/http/session.py` & `descarteslabs-2.0.1/descarteslabs/core/common/http/session.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/http/tests/test_authorization.py` & `descarteslabs-2.0.1/descarteslabs/core/common/http/tests/test_authorization.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/http/tests/test_proxy.py` & `descarteslabs-2.0.1/descarteslabs/core/common/http/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/http/tests/test_retry.py` & `descarteslabs-2.0.1/descarteslabs/core/common/http/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/http/tests/test_service.py` & `descarteslabs-2.0.1/descarteslabs/core/common/http/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/property_filtering/__init__.py` & `descarteslabs-2.0.1/descarteslabs/core/common/property_filtering/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/property_filtering/filtering.py` & `descarteslabs-2.0.1/descarteslabs/core/common/property_filtering/filtering.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/property_filtering/tests/test_filtering.py` & `descarteslabs-2.0.1/descarteslabs/core/common/property_filtering/tests/test_filtering.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/registry/__init__.py` & `descarteslabs-2.0.1/descarteslabs/core/common/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/registry/registry.py` & `descarteslabs-2.0.1/descarteslabs/core/common/registry/registry.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/retry/__init__.py` & `descarteslabs-2.0.1/descarteslabs/core/common/retry/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/retry/retry.py` & `descarteslabs-2.0.1/descarteslabs/core/common/retry/retry.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/retry/tests/test_retry.py` & `descarteslabs-2.0.1/descarteslabs/core/common/retry/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/shapely_support/__init__.py` & `descarteslabs-2.0.1/descarteslabs/core/common/shapely_support/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/shapely_support/tests/test_shapely_support.py` & `descarteslabs-2.0.1/descarteslabs/core/common/shapely_support/tests/test_shapely_support.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/threading/local.py` & `descarteslabs-2.0.1/descarteslabs/core/common/threading/local.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/common/threading/tests/test_local.py` & `descarteslabs-2.0.1/descarteslabs/core/common/threading/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/compute/__init__.py` & `descarteslabs-2.0.1/descarteslabs/core/compute/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/compute/compute.py` & `descarteslabs-2.0.1/descarteslabs/core/compute/compute.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/compute/compute_client.py` & `descarteslabs-2.0.1/descarteslabs/core/compute/compute_client.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/compute/tests/base.py` & `descarteslabs-2.0.1/descarteslabs/core/compute/tests/base.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/compute/tests/test_function.py` & `descarteslabs-2.0.1/descarteslabs/core/compute/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/compute/tests/test_job.py` & `descarteslabs-2.0.1/descarteslabs/core/compute/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/scenes/__init__.py` & `descarteslabs-2.0.1/descarteslabs/core/scenes/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/scenes/helpers.py` & `descarteslabs-2.0.1/descarteslabs/core/scenes/helpers.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/scenes/scene.py` & `descarteslabs-2.0.1/descarteslabs/core/scenes/scene.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/scenes/scenecollection.py` & `descarteslabs-2.0.1/descarteslabs/core/scenes/scenecollection.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/scenes/search_api.py` & `descarteslabs-2.0.1/descarteslabs/core/scenes/search_api.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/scenes/tests/mock_data.py` & `descarteslabs-2.0.1/descarteslabs/core/scenes/tests/mock_data.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/scenes/tests/test_scene.py` & `descarteslabs-2.0.1/descarteslabs/core/scenes/tests/test_scene.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/scenes/tests/test_scenecollection.py` & `descarteslabs-2.0.1/descarteslabs/core/scenes/tests/test_scenecollection.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/scenes/tests/test_search.py` & `descarteslabs-2.0.1/descarteslabs/core/scenes/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/third_party/boltons/__init__.py` & `descarteslabs-2.0.1/descarteslabs/core/third_party/boltons/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/core/third_party/boltons/funcutils.py` & `descarteslabs-2.0.1/descarteslabs/core/third_party/boltons/funcutils.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/exceptions.py` & `descarteslabs-2.0.1/descarteslabs/exceptions.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/geo/__init__.py` & `descarteslabs-2.0.1/descarteslabs/geo/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs/scenes/__init__.py` & `descarteslabs-2.0.1/descarteslabs/scenes/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs.egg-info/PKG-INFO` & `descarteslabs-2.0.1/descarteslabs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: descarteslabs
-Version: 2.0.0
+Version: 2.0.1
 Summary: Descartes Labs Python Client
 Home-page: https://github.com/descarteslabs/descarteslabs-python
 Author: Descartes Labs
 Author-email: hello@descarteslabs.com
 License: Apache 2.0
-Download-URL: https://github.com/descarteslabs/descarteslabs-python/archive/v2.0.0.tar.gz
+Download-URL: https://github.com/descarteslabs/descarteslabs-python/archive/v2.0.1.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `descarteslabs-2.0.0/descarteslabs.egg-info/SOURCES.txt` & `descarteslabs-2.0.1/descarteslabs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/descarteslabs.egg-info/requires.txt` & `descarteslabs-2.0.1/descarteslabs.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `descarteslabs-2.0.0/setup.py` & `descarteslabs-2.0.1/setup.py`

 * *Files identical despite different names*

