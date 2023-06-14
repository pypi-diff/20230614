# Comparing `tmp/oceanum-0.7.7.tar.gz` & `tmp/oceanum-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oceanum-0.7.7.tar", last modified: Thu Jun  8 20:58:07 2023, max compression
+gzip compressed data, was "oceanum-0.7.8.tar", last modified: Wed Jun 14 05:24:13 2023, max compression
```

## Comparing `oceanum-0.7.7.tar` & `oceanum-0.7.8.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-08 20:58:07.151425 oceanum-0.7.7/
--rw-rw-r--   0 dave      (1000) dave      (1000)      151 2023-05-14 22:31:40.000000 oceanum-0.7.7/AUTHORS.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     3501 2023-05-14 22:31:40.000000 oceanum-0.7.7/CONTRIBUTING.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)       89 2023-05-14 22:31:40.000000 oceanum-0.7.7/HISTORY.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     1077 2023-05-14 22:31:40.000000 oceanum-0.7.7/LICENSE
--rw-rw-r--   0 dave      (1000) dave      (1000)      262 2023-05-14 22:31:40.000000 oceanum-0.7.7/MANIFEST.in
--rw-rw-r--   0 dave      (1000) dave      (1000)     1180 2023-06-08 20:58:07.151425 oceanum-0.7.7/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)      788 2023-05-14 22:31:40.000000 oceanum-0.7.7/README.rst
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-08 20:58:07.107426 oceanum-0.7.7/docs/
--rw-rw-r--   0 dave      (1000) dave      (1000)      639 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/Makefile
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-08 20:58:07.103426 oceanum-0.7.7/docs/_build/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-08 20:58:07.103426 oceanum-0.7.7/docs/_build/html/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-08 20:58:07.107426 oceanum-0.7.7/docs/_build/html/_static/
--rw-rw-r--   0 dave      (1000) dave      (1000)      286 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/_build/html/_static/file.png
--rw-rw-r--   0 dave      (1000) dave      (1000)       90 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/_build/html/_static/minus.png
--rw-rw-r--   0 dave      (1000) dave      (1000)       90 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/_build/html/_static/plus.png
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-08 20:58:07.103426 oceanum-0.7.7/docs/_templates/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-08 20:58:07.111425 oceanum-0.7.7/docs/_templates/autosummary/
--rw-rw-r--   0 dave      (1000) dave      (1000)      481 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/_templates/autosummary/class.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)       73 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/about.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      593 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/api.rst
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-08 20:58:07.103426 oceanum-0.7.7/docs/classes/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-08 20:58:07.111425 oceanum-0.7.7/docs/classes/datamesh/
--rw-rw-r--   0 dave      (1000) dave      (1000)      406 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/classes/datamesh/oceanum.datamesh.Catalog.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      713 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/classes/datamesh/oceanum.datamesh.Connector.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      131 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/classes/datamesh/oceanum.datamesh.Datasource.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      116 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/classes/datamesh/oceanum.datamesh.Query.rst
--rwxrwxr-x   0 dave      (1000) dave      (1000)     5220 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/conf.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      160 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/index.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     1133 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/installation.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      801 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/make.bat
--rw-rw-r--   0 dave      (1000) dave      (1000)       58 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/modules.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      967 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/oceanum.datamesh.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      365 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/oceanum.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     1437 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/usage.rst
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-08 20:58:07.111425 oceanum-0.7.7/oceanum/
--rw-rw-r--   0 dave      (1000) dave      (1000)      474 2023-06-08 20:52:48.000000 oceanum-0.7.7/oceanum/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      313 2023-05-14 22:31:40.000000 oceanum-0.7.7/oceanum/cli.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-08 20:58:07.123425 oceanum-0.7.7/oceanum/datamesh/
--rw-rw-r--   0 dave      (1000) dave      (1000)      122 2023-05-14 22:31:40.000000 oceanum-0.7.7/oceanum/datamesh/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3425 2023-05-14 22:31:40.000000 oceanum-0.7.7/oceanum/datamesh/catalog.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    20720 2023-06-08 20:52:11.000000 oceanum-0.7.7/oceanum/datamesh/connection.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    10443 2023-05-14 22:31:40.000000 oceanum-0.7.7/oceanum/datamesh/datasource.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      144 2023-05-14 22:31:40.000000 oceanum-0.7.7/oceanum/datamesh/exceptions.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     7537 2023-05-14 22:35:23.000000 oceanum-0.7.7/oceanum/datamesh/query.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     4683 2023-05-14 22:31:40.000000 oceanum-0.7.7/oceanum/datamesh/zarr.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-08 20:58:07.119425 oceanum-0.7.7/oceanum.egg-info/
--rw-rw-r--   0 dave      (1000) dave      (1000)     1180 2023-06-08 20:58:06.000000 oceanum-0.7.7/oceanum.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)     1384 2023-06-08 20:58:07.000000 oceanum-0.7.7/oceanum.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-06-08 20:58:06.000000 oceanum-0.7.7/oceanum.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       45 2023-06-08 20:58:06.000000 oceanum-0.7.7/oceanum.egg-info/entry_points.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-06-08 20:58:06.000000 oceanum-0.7.7/oceanum.egg-info/not-zip-safe
--rw-rw-r--   0 dave      (1000) dave      (1000)      128 2023-06-08 20:58:06.000000 oceanum-0.7.7/oceanum.egg-info/requires.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        8 2023-06-08 20:58:06.000000 oceanum-0.7.7/oceanum.egg-info/top_level.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)      419 2023-06-08 20:58:07.151425 oceanum-0.7.7/setup.cfg
--rw-rw-r--   0 dave      (1000) dave      (1000)     1373 2023-05-14 22:31:40.000000 oceanum-0.7.7/setup.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-08 20:58:07.127425 oceanum-0.7.7/tests/
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-05-14 22:31:40.000000 oceanum-0.7.7/tests/__init__.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-08 20:58:07.151425 oceanum-0.7.7/tests/data/
--rw-rw-r--   0 dave      (1000) dave      (1000)    21010 2023-05-14 22:31:40.000000 oceanum-0.7.7/tests/data/grid_data_1.nc
--rw-rw-r--   0 dave      (1000) dave      (1000)  2029589 2023-05-14 22:31:40.000000 oceanum-0.7.7/tests/data/ocean_test_1.mp4
--rw-rw-r--   0 dave      (1000) dave      (1000)     1727 2023-05-14 22:31:40.000000 oceanum-0.7.7/tests/data/point_data_1.csv
--rw-rw-r--   0 dave      (1000) dave      (1000)     1222 2023-05-14 22:31:40.000000 oceanum-0.7.7/tests/test_catalog.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1072 2023-05-14 22:31:40.000000 oceanum-0.7.7/tests/test_datamesh_connect.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1643 2023-05-14 22:31:40.000000 oceanum-0.7.7/tests/test_datamesh_load.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2578 2023-05-14 22:31:40.000000 oceanum-0.7.7/tests/test_datamesh_query.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3255 2023-05-14 22:31:40.000000 oceanum-0.7.7/tests/test_datamesh_write.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2936 2023-05-14 22:31:40.000000 oceanum-0.7.7/tests/test_datasource.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1482 2023-05-14 22:31:40.000000 oceanum-0.7.7/tests/test_query.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      805 2023-05-14 22:31:40.000000 oceanum-0.7.7/tests/test_video_compat.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 05:24:13.396674 oceanum-0.7.8/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      151 2023-05-14 22:31:40.000000 oceanum-0.7.8/AUTHORS.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3501 2023-05-14 22:31:40.000000 oceanum-0.7.8/CONTRIBUTING.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)       89 2023-05-14 22:31:40.000000 oceanum-0.7.8/HISTORY.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1077 2023-05-14 22:31:40.000000 oceanum-0.7.8/LICENSE
+-rw-rw-r--   0 dave      (1000) dave      (1000)      262 2023-05-14 22:31:40.000000 oceanum-0.7.8/MANIFEST.in
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1180 2023-06-14 05:24:13.396674 oceanum-0.7.8/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      788 2023-05-14 22:31:40.000000 oceanum-0.7.8/README.rst
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 05:24:13.380674 oceanum-0.7.8/docs/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      639 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/Makefile
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 05:24:13.376674 oceanum-0.7.8/docs/_build/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 05:24:13.376674 oceanum-0.7.8/docs/_build/html/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 05:24:13.384674 oceanum-0.7.8/docs/_build/html/_static/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      286 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/_build/html/_static/file.png
+-rw-rw-r--   0 dave      (1000) dave      (1000)       90 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 dave      (1000) dave      (1000)       90 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/_build/html/_static/plus.png
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 05:24:13.376674 oceanum-0.7.8/docs/_templates/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 05:24:13.384674 oceanum-0.7.8/docs/_templates/autosummary/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      481 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/_templates/autosummary/class.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)       73 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/about.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      593 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/api.rst
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 05:24:13.376674 oceanum-0.7.8/docs/classes/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 05:24:13.384674 oceanum-0.7.8/docs/classes/datamesh/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      406 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/classes/datamesh/oceanum.datamesh.Catalog.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      713 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/classes/datamesh/oceanum.datamesh.Connector.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      131 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/classes/datamesh/oceanum.datamesh.Datasource.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      116 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/classes/datamesh/oceanum.datamesh.Query.rst
+-rwxrwxr-x   0 dave      (1000) dave      (1000)     5220 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/conf.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      160 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/index.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1133 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/installation.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      801 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/make.bat
+-rw-rw-r--   0 dave      (1000) dave      (1000)       58 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/modules.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      967 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/oceanum.datamesh.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      365 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/oceanum.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1437 2023-05-14 22:31:40.000000 oceanum-0.7.8/docs/usage.rst
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 05:24:13.384674 oceanum-0.7.8/oceanum/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      474 2023-06-14 05:17:45.000000 oceanum-0.7.8/oceanum/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      313 2023-05-14 22:31:40.000000 oceanum-0.7.8/oceanum/cli.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 05:24:13.388674 oceanum-0.7.8/oceanum/datamesh/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      122 2023-05-14 22:31:40.000000 oceanum-0.7.8/oceanum/datamesh/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3425 2023-05-14 22:31:40.000000 oceanum-0.7.8/oceanum/datamesh/catalog.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    20720 2023-06-08 20:52:11.000000 oceanum-0.7.8/oceanum/datamesh/connection.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    10443 2023-05-14 22:31:40.000000 oceanum-0.7.8/oceanum/datamesh/datasource.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      144 2023-05-14 22:31:40.000000 oceanum-0.7.8/oceanum/datamesh/exceptions.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     7537 2023-05-14 22:35:23.000000 oceanum-0.7.8/oceanum/datamesh/query.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5037 2023-06-14 04:46:09.000000 oceanum-0.7.8/oceanum/datamesh/zarr.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 05:24:13.388674 oceanum-0.7.8/oceanum.egg-info/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1180 2023-06-14 05:24:13.000000 oceanum-0.7.8/oceanum.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1384 2023-06-14 05:24:13.000000 oceanum-0.7.8/oceanum.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-06-14 05:24:13.000000 oceanum-0.7.8/oceanum.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       45 2023-06-14 05:24:13.000000 oceanum-0.7.8/oceanum.egg-info/entry_points.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-06-14 05:24:13.000000 oceanum-0.7.8/oceanum.egg-info/not-zip-safe
+-rw-rw-r--   0 dave      (1000) dave      (1000)      128 2023-06-14 05:24:13.000000 oceanum-0.7.8/oceanum.egg-info/requires.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        8 2023-06-14 05:24:13.000000 oceanum-0.7.8/oceanum.egg-info/top_level.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)      419 2023-06-14 05:24:13.396674 oceanum-0.7.8/setup.cfg
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1373 2023-05-14 22:31:40.000000 oceanum-0.7.8/setup.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 05:24:13.388674 oceanum-0.7.8/tests/
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-05-14 22:31:40.000000 oceanum-0.7.8/tests/__init__.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 05:24:13.396674 oceanum-0.7.8/tests/data/
+-rw-rw-r--   0 dave      (1000) dave      (1000)    21010 2023-05-14 22:31:40.000000 oceanum-0.7.8/tests/data/grid_data_1.nc
+-rw-rw-r--   0 dave      (1000) dave      (1000)  2029589 2023-05-14 22:31:40.000000 oceanum-0.7.8/tests/data/ocean_test_1.mp4
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1727 2023-05-14 22:31:40.000000 oceanum-0.7.8/tests/data/point_data_1.csv
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1222 2023-05-14 22:31:40.000000 oceanum-0.7.8/tests/test_catalog.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1072 2023-05-14 22:31:40.000000 oceanum-0.7.8/tests/test_datamesh_connect.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1643 2023-05-14 22:31:40.000000 oceanum-0.7.8/tests/test_datamesh_load.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2578 2023-05-14 22:31:40.000000 oceanum-0.7.8/tests/test_datamesh_query.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3255 2023-05-14 22:31:40.000000 oceanum-0.7.8/tests/test_datamesh_write.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2936 2023-05-14 22:31:40.000000 oceanum-0.7.8/tests/test_datasource.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1482 2023-05-14 22:31:40.000000 oceanum-0.7.8/tests/test_query.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      805 2023-05-14 22:31:40.000000 oceanum-0.7.8/tests/test_video_compat.py
```

### Comparing `oceanum-0.7.7/CONTRIBUTING.rst` & `oceanum-0.7.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.7/LICENSE` & `oceanum-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.7/PKG-INFO` & `oceanum-0.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oceanum
-Version: 0.7.7
+Version: 0.7.8
 Summary: Library for oceanum.io services
 Home-page: https://github.com/oceanum/oceanum-python
 Author: Oceanum Developers
 Author-email: developers@oceanum.science
 License: MIT license
 Keywords: oceanum
 License-File: LICENSE
```

### Comparing `oceanum-0.7.7/README.rst` & `oceanum-0.7.8/README.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.7/docs/Makefile` & `oceanum-0.7.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.7/docs/api.rst` & `oceanum-0.7.8/docs/api.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.7/docs/classes/datamesh/oceanum.datamesh.Connector.rst` & `oceanum-0.7.8/docs/classes/datamesh/oceanum.datamesh.Connector.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.7/docs/conf.py` & `oceanum-0.7.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.7/docs/installation.rst` & `oceanum-0.7.8/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.7/docs/make.bat` & `oceanum-0.7.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.7/docs/oceanum.datamesh.rst` & `oceanum-0.7.8/docs/oceanum.datamesh.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.7/docs/usage.rst` & `oceanum-0.7.8/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.7/oceanum/datamesh/catalog.py` & `oceanum-0.7.8/oceanum/datamesh/catalog.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.7/oceanum/datamesh/connection.py` & `oceanum-0.7.8/oceanum/datamesh/connection.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.7/oceanum/datamesh/datasource.py` & `oceanum-0.7.8/oceanum/datamesh/datasource.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.7/oceanum/datamesh/query.py` & `oceanum-0.7.8/oceanum/datamesh/query.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.7/oceanum/datamesh/zarr.py` & `oceanum-0.7.8/oceanum/datamesh/zarr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import requests
 import re
+import time
 import xarray
 import numpy
 from collections.abc import MutableMapping
 
 from .exceptions import DatameshWriteError
 
 try:
@@ -11,25 +12,35 @@
 
     _VIDEO_SUPPORT = True
 except:
     _VIDEO_SUPPORT = False
 
 
 class ZarrClient(MutableMapping):
-    def __init__(self, connection, datasource, method="post"):
+    def __init__(self, connection, datasource, method="post", retries=5):
         self.datasource = datasource
         self.method = method
         self.headers = {**connection._auth_headers, "cache-control": "no-transform"}
         self.gateway = connection._gateway + "/zarr"
+        self.retries = retries
+
+    def _get(self, path):
+        retries = 0
+        while retries < self.retries:
+            try:
+                resp = requests.get(path, headers=self.headers)
+            except requests.RequestException:
+                time.sleep(0.1 * 2**retries)
+                retries += 1
+            else:
+                return resp
 
     def __getitem__(self, item):
-        resp = requests.get(
-            f"{self.gateway}/{self.datasource}/{item}", headers=self.headers
-        )
-        if resp.status_code != 200:
+        resp = self._get(f"{self.gateway}/{self.datasource}/{item}")
+        if resp.status_code >= 300:
             raise KeyError(item)
         return resp.content
 
     def __setitem__(self, item, value):
         if self.method == "put":
             requests.put(
                 f"{self.gateway}/{self.datasource}/{item}",
@@ -45,15 +56,17 @@
 
     def __delitem__(self, item):
         requests.delete(
             f"{self.gateway}/{self.datasource}/{item}", headers=self.headers
         )
 
     def __iter__(self):
-        resp = requests.get(f"{self.gateway}/{self.datasource}", headers=self.headers)
+        resp = self._get(f"{self.gateway}/{self.datasource}")
+        if not resp:
+            return
         ex = re.compile(r"""<(a|A)\s+(?:[^>]*?\s+)?(href|HREF)=["'](?P<url>[^"']+)""")
         links = [u[2] for u in ex.findall(resp.text)]
         for link in links:
             yield link
 
     def __len__(self):
         return 0
```

### Comparing `oceanum-0.7.7/oceanum.egg-info/PKG-INFO` & `oceanum-0.7.8/oceanum.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oceanum
-Version: 0.7.7
+Version: 0.7.8
 Summary: Library for oceanum.io services
 Home-page: https://github.com/oceanum/oceanum-python
 Author: Oceanum Developers
 Author-email: developers@oceanum.science
 License: MIT license
 Keywords: oceanum
 License-File: LICENSE
```

### Comparing `oceanum-0.7.7/oceanum.egg-info/SOURCES.txt` & `oceanum-0.7.8/oceanum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.7/setup.py` & `oceanum-0.7.8/setup.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.7/tests/data/grid_data_1.nc` & `oceanum-0.7.8/tests/data/grid_data_1.nc`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.7/tests/data/ocean_test_1.mp4` & `oceanum-0.7.8/tests/data/ocean_test_1.mp4`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.7/tests/data/point_data_1.csv` & `oceanum-0.7.8/tests/data/point_data_1.csv`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.7/tests/test_catalog.py` & `oceanum-0.7.8/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.7/tests/test_datamesh_connect.py` & `oceanum-0.7.8/tests/test_datamesh_connect.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.7/tests/test_datamesh_load.py` & `oceanum-0.7.8/tests/test_datamesh_load.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.7/tests/test_datamesh_query.py` & `oceanum-0.7.8/tests/test_datamesh_query.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.7/tests/test_datamesh_write.py` & `oceanum-0.7.8/tests/test_datamesh_write.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.7/tests/test_datasource.py` & `oceanum-0.7.8/tests/test_datasource.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.7/tests/test_query.py` & `oceanum-0.7.8/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.7/tests/test_video_compat.py` & `oceanum-0.7.8/tests/test_video_compat.py`

 * *Files identical despite different names*

