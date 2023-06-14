# Comparing `tmp/pyTMD-2.0.4.tar.gz` & `tmp/pyTMD-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyTMD-2.0.4.tar", last modified: Wed May 10 18:23:56 2023, max compression
+gzip compressed data, was "pyTMD-2.0.5.tar", last modified: Wed Jun 14 19:11:59 2023, max compression
```

## Comparing `pyTMD-2.0.4.tar` & `pyTMD-2.0.5.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 18:23:56.429118 pyTMD-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (122)      442 2023-05-10 18:23:42.000000 pyTMD-2.0.4/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (122)      955 2023-05-10 18:23:42.000000 pyTMD-2.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     5545 2023-05-10 18:23:42.000000 pyTMD-2.0.4/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (122)      620 2023-05-10 18:23:42.000000 pyTMD-2.0.4/CONTRIBUTORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-05-10 18:23:42.000000 pyTMD-2.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-10 18:23:42.000000 pyTMD-2.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6792 2023-05-10 18:23:56.429118 pyTMD-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5890 2023-05-10 18:23:42.000000 pyTMD-2.0.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-05-10 18:23:42.000000 pyTMD-2.0.4/postBuild
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 18:23:56.413118 pyTMD-2.0.4/pyTMD/
--rw-r--r--   0 runner    (1001) docker     (122)     1422 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    20738 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/arguments.py
--rw-r--r--   0 runner    (1001) docker     (122)    43001 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/astro.py
--rw-r--r--   0 runner    (1001) docker     (122)     3376 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/calc_astrol_longitudes.py
--rw-r--r--   0 runner    (1001) docker     (122)     9072 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/check_tide_points.py
--rw-r--r--   0 runner    (1001) docker     (122)    43968 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/compute_tide_corrections.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    12861 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    16129 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/convert_crs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2974 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/convert_ll_xy.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 18:23:56.425118 pyTMD-2.0.4/pyTMD/data/
--rwxr-xr-x   0 runner    (1001) docker     (122)    12369 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/data/deltat.data
--rwxr-xr-x   0 runner    (1001) docker     (122)  3534588 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/data/finals.all
--rwxr-xr-x   0 runner    (1001) docker     (122)    30345 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/data/historic_deltat.data
--rwxr-xr-x   0 runner    (1001) docker     (122)   130160 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/data/iers_deltat.data
--rwxr-xr-x   0 runner    (1001) docker     (122)    10666 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/data/leap-seconds.list
--rwxr-xr-x   0 runner    (1001) docker     (122)    78880 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/data/mean-pole.tab
--rwxr-xr-x   0 runner    (1001) docker     (122)   154120 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/data/merged_deltat.data
--rwxr-xr-x   0 runner    (1001) docker     (122)  6325011 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/data/opoleloadcoefcmcor.txt.gz
--rwxr-xr-x   0 runner    (1001) docker     (122)    41126 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/data/ser7.dat
--rw-r--r--   0 runner    (1001) docker     (122)     5849 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/data/tab5.2e.txt
--rw-r--r--   0 runner    (1001) docker     (122)   145678 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/data/tab5.3a.txt
--rw-r--r--   0 runner    (1001) docker     (122)   113660 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/data/tab5.3b.txt
--rw-r--r--   0 runner    (1001) docker     (122)    17529 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/eop.py
--rw-r--r--   0 runner    (1001) docker     (122)    15243 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/interpolate.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 18:23:56.429118 pyTMD-2.0.4/pyTMD/io/
--rw-r--r--   0 runner    (1001) docker     (122)    43622 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/io/ATLAS.py
--rw-r--r--   0 runner    (1001) docker     (122)    31908 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/io/FES.py
--rw-r--r--   0 runner    (1001) docker     (122)    28562 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/io/GOT.py
--rw-r--r--   0 runner    (1001) docker     (122)    71516 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/io/OTIS.py
--rw-r--r--   0 runner    (1001) docker     (122)      188 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4469 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/io/constituents.py
--rw-r--r--   0 runner    (1001) docker     (122)    66799 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/io/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     6162 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/io/ocean_pole_tide.py
--rw-r--r--   0 runner    (1001) docker     (122)     4743 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/load_constituent.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4904 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/load_nodal_corrections.py
--rw-r--r--   0 runner    (1001) docker     (122)    42856 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/predict.py
--rw-r--r--   0 runner    (1001) docker     (122)    61796 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/spatial.py
--rw-r--r--   0 runner    (1001) docker     (122)     2966 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/tidal_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (122)    59301 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/time.py
--rw-r--r--   0 runner    (1001) docker     (122)    11840 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/tools.py
--rw-r--r--   0 runner    (1001) docker     (122)    39544 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/utilities.py
--rw-r--r--   0 runner    (1001) docker     (122)      382 2023-05-10 18:23:42.000000 pyTMD-2.0.4/pyTMD/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 18:23:56.413118 pyTMD-2.0.4/pyTMD.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6792 2023-05-10 18:23:56.000000 pyTMD-2.0.4/pyTMD.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1555 2023-05-10 18:23:56.000000 pyTMD-2.0.4/pyTMD.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-10 18:23:56.000000 pyTMD-2.0.4/pyTMD.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-05-10 18:23:56.000000 pyTMD-2.0.4/pyTMD.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-10 18:23:56.000000 pyTMD-2.0.4/pyTMD.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-10 18:23:42.000000 pyTMD-2.0.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)       88 2023-05-10 18:23:42.000000 pyTMD-2.0.4/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 18:23:56.429118 pyTMD-2.0.4/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)     5497 2023-05-10 18:23:42.000000 pyTMD-2.0.4/scripts/arcticdata_tides.py
--rw-r--r--   0 runner    (1001) docker     (122)    13412 2023-05-10 18:23:42.000000 pyTMD-2.0.4/scripts/aviso_fes_tides.py
--rw-r--r--   0 runner    (1001) docker     (122)    14751 2023-05-10 18:23:42.000000 pyTMD-2.0.4/scripts/compute_LPET_elevations.py
--rw-r--r--   0 runner    (1001) docker     (122)    18641 2023-05-10 18:23:42.000000 pyTMD-2.0.4/scripts/compute_LPT_displacements.py
--rw-r--r--   0 runner    (1001) docker     (122)    20962 2023-05-10 18:23:42.000000 pyTMD-2.0.4/scripts/compute_OPT_displacements.py
--rw-r--r--   0 runner    (1001) docker     (122)    19178 2023-05-10 18:23:42.000000 pyTMD-2.0.4/scripts/compute_SET_displacements.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    23166 2023-05-10 18:23:42.000000 pyTMD-2.0.4/scripts/compute_tidal_currents.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    23367 2023-05-10 18:23:42.000000 pyTMD-2.0.4/scripts/compute_tidal_elevations.py
--rw-r--r--   0 runner    (1001) docker     (122)    11545 2023-05-10 18:23:42.000000 pyTMD-2.0.4/scripts/reduce_OTIS_files.py
--rw-r--r--   0 runner    (1001) docker     (122)     5125 2023-05-10 18:23:42.000000 pyTMD-2.0.4/scripts/usap_cats_tides.py
--rw-r--r--   0 runner    (1001) docker     (122)     7921 2023-05-10 18:23:42.000000 pyTMD-2.0.4/scripts/verify_box_tpxo.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-10 18:23:56.429118 pyTMD-2.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3960 2023-05-10 18:23:42.000000 pyTMD-2.0.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-10 18:23:42.000000 pyTMD-2.0.4/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:11:59.154677 pyTMD-2.0.5/
+-rw-r--r--   0 runner    (1001) docker     (122)      442 2023-06-14 19:11:42.000000 pyTMD-2.0.5/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)      955 2023-06-14 19:11:42.000000 pyTMD-2.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     5545 2023-06-14 19:11:42.000000 pyTMD-2.0.5/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      620 2023-06-14 19:11:42.000000 pyTMD-2.0.5/CONTRIBUTORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-06-14 19:11:42.000000 pyTMD-2.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-06-14 19:11:42.000000 pyTMD-2.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6785 2023-06-14 19:11:59.154677 pyTMD-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5883 2023-06-14 19:11:42.000000 pyTMD-2.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-06-14 19:11:42.000000 pyTMD-2.0.5/postBuild
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:11:59.138677 pyTMD-2.0.5/pyTMD/
+-rw-r--r--   0 runner    (1001) docker     (122)     1422 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    20738 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43421 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/astro.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3376 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/calc_astrol_longitudes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9072 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/check_tide_points.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43968 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/compute_tide_corrections.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    12861 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16129 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/convert_crs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2974 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/convert_ll_xy.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:11:59.150677 pyTMD-2.0.5/pyTMD/data/
+-rwxr-xr-x   0 runner    (1001) docker     (122)    12369 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/data/deltat.data
+-rwxr-xr-x   0 runner    (1001) docker     (122)  3539852 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/data/finals.all
+-rwxr-xr-x   0 runner    (1001) docker     (122)    30345 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/data/historic_deltat.data
+-rwxr-xr-x   0 runner    (1001) docker     (122)   130160 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/data/iers_deltat.data
+-rwxr-xr-x   0 runner    (1001) docker     (122)    10666 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/data/leap-seconds.list
+-rwxr-xr-x   0 runner    (1001) docker     (122)    78944 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/data/mean-pole.tab
+-rwxr-xr-x   0 runner    (1001) docker     (122)   154820 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/data/merged_deltat.data
+-rwxr-xr-x   0 runner    (1001) docker     (122)  6325011 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/data/opoleloadcoefcmcor.txt.gz
+-rwxr-xr-x   0 runner    (1001) docker     (122)    41600 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/data/ser7.dat
+-rw-r--r--   0 runner    (1001) docker     (122)     5849 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/data/tab5.2e.txt
+-rw-r--r--   0 runner    (1001) docker     (122)   145678 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/data/tab5.3a.txt
+-rw-r--r--   0 runner    (1001) docker     (122)   113660 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/data/tab5.3b.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    17529 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/eop.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15243 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/interpolate.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:11:59.150677 pyTMD-2.0.5/pyTMD/io/
+-rw-r--r--   0 runner    (1001) docker     (122)    43622 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/io/ATLAS.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31955 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/io/FES.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28562 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/io/GOT.py
+-rw-r--r--   0 runner    (1001) docker     (122)    71516 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/io/OTIS.py
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4469 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/io/constituents.py
+-rw-r--r--   0 runner    (1001) docker     (122)    66877 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/io/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6162 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/io/ocean_pole_tide.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4743 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/load_constituent.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4904 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/load_nodal_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42856 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/predict.py
+-rw-r--r--   0 runner    (1001) docker     (122)    61851 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2966 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/tidal_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (122)    59968 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11877 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/tools.py
+-rw-r--r--   0 runner    (1001) docker     (122)    49462 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      382 2023-06-14 19:11:42.000000 pyTMD-2.0.5/pyTMD/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:11:59.138677 pyTMD-2.0.5/pyTMD.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6785 2023-06-14 19:11:58.000000 pyTMD-2.0.5/pyTMD.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1555 2023-06-14 19:11:59.000000 pyTMD-2.0.5/pyTMD.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 19:11:58.000000 pyTMD-2.0.5/pyTMD.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-06-14 19:11:58.000000 pyTMD-2.0.5/pyTMD.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-14 19:11:58.000000 pyTMD-2.0.5/pyTMD.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-06-14 19:11:42.000000 pyTMD-2.0.5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2023-06-14 19:11:42.000000 pyTMD-2.0.5/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 19:11:59.154677 pyTMD-2.0.5/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)     5875 2023-06-14 19:11:42.000000 pyTMD-2.0.5/scripts/arcticdata_tides.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13977 2023-06-14 19:11:42.000000 pyTMD-2.0.5/scripts/aviso_fes_tides.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14779 2023-06-14 19:11:42.000000 pyTMD-2.0.5/scripts/compute_LPET_elevations.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18669 2023-06-14 19:11:42.000000 pyTMD-2.0.5/scripts/compute_LPT_displacements.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20990 2023-06-14 19:11:42.000000 pyTMD-2.0.5/scripts/compute_OPT_displacements.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19206 2023-06-14 19:11:42.000000 pyTMD-2.0.5/scripts/compute_SET_displacements.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    23194 2023-06-14 19:11:42.000000 pyTMD-2.0.5/scripts/compute_tidal_currents.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    23395 2023-06-14 19:11:42.000000 pyTMD-2.0.5/scripts/compute_tidal_elevations.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11560 2023-06-14 19:11:42.000000 pyTMD-2.0.5/scripts/reduce_OTIS_files.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5130 2023-06-14 19:11:42.000000 pyTMD-2.0.5/scripts/usap_cats_tides.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7926 2023-06-14 19:11:42.000000 pyTMD-2.0.5/scripts/verify_box_tpxo.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-14 19:11:59.154677 pyTMD-2.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3960 2023-06-14 19:11:42.000000 pyTMD-2.0.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-14 19:11:42.000000 pyTMD-2.0.5/version.txt
```

### Comparing `pyTMD-2.0.4/.gitignore` & `pyTMD-2.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.4/CODE_OF_CONDUCT.rst` & `pyTMD-2.0.5/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.4/CONTRIBUTORS.rst` & `pyTMD-2.0.5/CONTRIBUTORS.rst`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.4/LICENSE` & `pyTMD-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.4/PKG-INFO` & `pyTMD-2.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTMD
-Version: 2.0.4
+Version: 2.0.5
 Summary: Tide Model Driver to read OTIS, GOT and FES formatted tidal solutions and make tidal predictions
 Home-page: https://github.com/tsutterley/pyTMD
 Author: Tyler Sutterley
 Author-email: tsutterl@uw.edu
 License: MIT
 Keywords: Ocean Tides,Load Tides,Pole Tides,Tidal Prediction,OTIS,GOT,FES
 Classifier: Development Status :: 3 - Alpha
@@ -80,15 +80,15 @@
 
 - `dateutil: powerful extensions to datetime <https://dateutil.readthedocs.io/en/stable/>`_
 - `lxml: processing XML and HTML in Python <https://pypi.python.org/pypi/lxml>`_
 - `netCDF4: Python interface to the netCDF C library <https://unidata.github.io/netcdf4-python/>`_
 - `numpy: Scientific Computing Tools For Python <https://www.numpy.org>`_
 - `pyproj: Python interface to PROJ library <https://pypi.org/project/pyproj/>`_
 - `scipy: Scientific Tools for Python <https://www.scipy.org/>`_
-- `setuptools_scm: manager for python package versions using scm metadata <https://pypi.org/project/setuptools-scm/1.9.0/>`_
+- `setuptools_scm: manager for python package versions using scm metadata <https://pypi.org/project/setuptools-scm>`_
 
 References
 ##########
 
     T. C. Sutterley, T. Markus, T. A. Neumann, M. R. van den Broeke, J. M. van Wessem, and S. R. M. Ligtenberg,
     "Antarctic ice shelf thickness change from multimission lidar mapping", *The Cryosphere*,
     13, 1801-1817, (2019). `doi: 10.5194/tc-13-1801-2019 <https://doi.org/10.5194/tc-13-1801-2019>`_
```

### Comparing `pyTMD-2.0.4/README.rst` & `pyTMD-2.0.5/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 - `dateutil: powerful extensions to datetime <https://dateutil.readthedocs.io/en/stable/>`_
 - `lxml: processing XML and HTML in Python <https://pypi.python.org/pypi/lxml>`_
 - `netCDF4: Python interface to the netCDF C library <https://unidata.github.io/netcdf4-python/>`_
 - `numpy: Scientific Computing Tools For Python <https://www.numpy.org>`_
 - `pyproj: Python interface to PROJ library <https://pypi.org/project/pyproj/>`_
 - `scipy: Scientific Tools for Python <https://www.scipy.org/>`_
-- `setuptools_scm: manager for python package versions using scm metadata <https://pypi.org/project/setuptools-scm/1.9.0/>`_
+- `setuptools_scm: manager for python package versions using scm metadata <https://pypi.org/project/setuptools-scm>`_
 
 References
 ##########
 
     T. C. Sutterley, T. Markus, T. A. Neumann, M. R. van den Broeke, J. M. van Wessem, and S. R. M. Ligtenberg,
     "Antarctic ice shelf thickness change from multimission lidar mapping", *The Cryosphere*,
     13, 1801-1817, (2019). `doi: 10.5194/tc-13-1801-2019 <https://doi.org/10.5194/tc-13-1801-2019>`_
```

### Comparing `pyTMD-2.0.4/pyTMD/__init__.py` & `pyTMD-2.0.5/pyTMD/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.4/pyTMD/arguments.py` & `pyTMD-2.0.5/pyTMD/arguments.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.4/pyTMD/astro.py` & `pyTMD-2.0.5/pyTMD/astro.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 REFERENCES:
     Jean Meeus, Astronomical Algorithms, 2nd edition, 1998.
     Oliver Montenbruck, Practical Ephemeris Calculations, 1989.
 
 UPDATE HISTORY:
     Updated 05/2023: add wrapper function for nutation angles
+        download JPL kernel file if not currently existing
     Updated 04/2023: added low resolution solar and lunar positions
         added function with more phase angles of the sun and moon
         functions to calculate solar and lunar positions with ephemerides
         add jplephem documentation to Spacecraft and Planet Kernel segments
         fix solar ephemeride function to include SSB to sun segment
         use a higher resolution estimate of the Greenwich hour angle
         use ITRS reference frame for high-resolution ephemeride calculations
@@ -46,18 +47,19 @@
     Updated 09/2017: Rewritten in Python
     Rewritten in Matlab by Lana Erofeeva 2003
     Written by Richard Ray 12/1990
 """
 from __future__ import annotations
 
 import logging
+import pathlib
 import numpy as np
 from pyTMD.time import timescale
 from pyTMD.eop import iers_polar_motion
-from pyTMD.utilities import get_data_path
+from pyTMD.utilities import get_data_path, from_jpl_ssd
 
 # attempt imports
 try:
     import jplephem.spk
 except (ImportError, ModuleNotFoundError) as exc:
     logging.debug("jplephem not available")
 
@@ -473,14 +475,17 @@
         `doi: 10.3847/1538-3881/abd414
         <https://doi.org/10.3847/1538-3881/abd414>`_
     """
     # set default keyword arguments
     kwargs.setdefault('kernel', _default_kernel)
     # create timescale from Modified Julian Day (MJD)
     ts = timescale(MJD=MJD)
+    # download kernel file if not currently existing
+    if not pathlib.Path(kwargs['kernel']).exists():
+        from_jpl_ssd(kernel=None, local=kwargs['kernel'])
     # read JPL ephemerides kernel
     SPK = jplephem.spk.SPK.open(kwargs['kernel'])
     # segments for computing position of the sun
     # segment 0 SOLAR SYSTEM BARYCENTER -> segment 10 SUN
     SSB_to_Sun = SPK[0, 10]
     # segment 0 SOLAR SYSTEM BARYCENTER -> segment 3 EARTH BARYCENTER
     SSB_to_EMB = SPK[0, 3]
@@ -609,14 +614,17 @@
         "The JPL Planetary and Lunar Ephemerides DE440 and DE441",
         *The Astronomical Journal*, 161(3), 105, (2021).
         `doi: 10.3847/1538-3881/abd414
         <https://doi.org/10.3847/1538-3881/abd414>`_
     """
     # set default keyword arguments
     kwargs.setdefault('kernel', _default_kernel)
+    # download kernel file if not currently existing
+    if not pathlib.Path(kwargs['kernel']).exists():
+        from_jpl_ssd(kernel=None, local=kwargs['kernel'])
     # create timescale from Modified Julian Day (MJD)
     ts = timescale(MJD=MJD)
     # read JPL ephemerides kernel
     SPK = jplephem.spk.SPK.open(kwargs['kernel'])
     # segments for computing position of the moon
     # segment 3 EARTH BARYCENTER -> segment 399 EARTH
     EMB_to_Earth = SPK[3, 399]
@@ -798,16 +806,16 @@
         j1['L_Me'], j1['L_Ve'], j1['L_E'], j1['L_Ma'], j1['L_J'],
         j1['L_Sa'], j1['L_U'], j1['L_Ne'], j1['p_A']]
     arg0 = np.dot(n0, np.mod(fa, ts.tau))
     arg1 = np.dot(n1, np.mod(fa, ts.tau))
     # evaluate the complementary terms and convert to radians
     complement = ts.masec2rad*(np.dot(j0['Cs'], np.sin(arg0)) +
         np.dot(j0['Cc'], np.cos(arg0)) +
-        T*np.dot(j1['Cs'], np.sin(arg1)) +
-        T*np.dot(j1['Cc'], np.cos(arg1)))
+        ts.T*np.dot(j1['Cs'], np.sin(arg1)) +
+        ts.T*np.dot(j1['Cc'], np.cos(arg1)))
     # return the complementary terms
     return complement
 
 def _frame_bias_matrix():
     """
     Frame bias rotation matrix
     """
```

### Comparing `pyTMD-2.0.4/pyTMD/calc_astrol_longitudes.py` & `pyTMD-2.0.5/pyTMD/calc_astrol_longitudes.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.4/pyTMD/check_tide_points.py` & `pyTMD-2.0.5/pyTMD/check_tide_points.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.4/pyTMD/compute_tide_corrections.py` & `pyTMD-2.0.5/pyTMD/compute_tide_corrections.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.4/pyTMD/constants.py` & `pyTMD-2.0.5/pyTMD/constants.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.4/pyTMD/convert_crs.py` & `pyTMD-2.0.5/pyTMD/convert_crs.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.4/pyTMD/convert_ll_xy.py` & `pyTMD-2.0.5/pyTMD/convert_ll_xy.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.4/pyTMD/data/deltat.data` & `pyTMD-2.0.5/pyTMD/data/deltat.data`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.4/pyTMD/data/finals.all` & `pyTMD-2.0.5/pyTMD/data/finals.all`

 * *Files 0% similar despite different names*

```diff
@@ -17993,794 +17993,794 @@
 22 4 7 59676.00 I  0.047706 0.000019  0.440056 0.000020  I-0.0990861 0.0000074 -0.5566 0.0053  I  -106.894    0.620    -8.605    0.039  0.047660  0.440084 -0.0991087  -106.904    -8.610  
 22 4 8 59677.00 I  0.049433 0.000018  0.441874 0.000019  I-0.0985111 0.0000074 -0.5857 0.0053  I  -106.565    0.620    -8.665    0.039  0.049412  0.441800 -0.0985116  -106.602    -8.670  
 22 4 9 59678.00 I  0.051231 0.000015  0.443552 0.000017  I-0.0979307 0.0000077 -0.5669 0.0050  I  -106.083    0.620    -8.840    0.039  0.051279  0.443588 -0.0979207  -106.131    -8.844  
 22 410 59679.00 I  0.052565 0.000016  0.445332 0.000019  I-0.0973866 0.0000066 -0.5204 0.0051  I  -105.529    0.786    -9.102    0.045  0.052631  0.445310 -0.0973816  -105.574    -9.106  
 22 411 59680.00 I  0.053446 0.000015  0.447041 0.000018  I-0.0969113 0.0000066 -0.4098 0.0041  I  -105.062    0.786    -9.348    0.045  0.053447  0.447037 -0.0969159  -105.095    -9.347  
 22 412 59681.00 I  0.054290 0.000013  0.449062 0.000017  I-0.0965831 0.0000048 -0.2510 0.0038  I  -104.883    0.835    -9.501    0.112  0.054284  0.449011 -0.0965845  -104.884    -9.491  
 22 413 59682.00 I  0.055326 0.000011  0.451035 0.000017  I-0.0964339 0.0000039 -0.0184 0.0033  I  -105.048    0.835    -9.551    0.112  0.055292  0.451073 -0.0964523  -105.062    -9.565  
-22 414 59683.00 I  0.056533 0.000011  0.452915 0.000017  I-0.0965583 0.0000044  0.2502 0.0029  I  -105.349    0.835    -9.494    0.112  0.056547  0.452892 -0.0965557  -105.379    -9.547  
+22 414 59683.00 I  0.056533 0.000011  0.452915 0.000017  I-0.0965583 0.0000044  0.2502 0.0029  I  -105.349    0.835    -9.493    0.112  0.056547  0.452892 -0.0965557  -105.379    -9.547  
 22 415 59684.00 I  0.057880 0.000015  0.454454 0.000018  I-0.0969079 0.0000043  0.4396 0.0030  I  -105.523    0.835    -9.313    0.112  0.057823  0.454485 -0.0968994  -105.550    -9.362  
 22 416 59685.00 I  0.059422 0.000018  0.456174 0.000016  I-0.0974121 0.0000042  0.5529 0.0031  I  -105.584    0.778    -9.059    0.154  0.059424  0.456172 -0.0974129  -105.603    -9.095  
 22 417 59686.00 I  0.061286 0.000020  0.457791 0.000016  I-0.0979771 0.0000044  0.5563 0.0043  I  -105.790    0.778    -8.874    0.154  0.061164  0.457851 -0.0979865  -105.807    -8.908  
 22 418 59687.00 I  0.063721 0.000022  0.459297 0.000016  I-0.0984833 0.0000074  0.4355 0.0043  I  -106.252    0.806    -8.891    0.015  0.063734  0.459266 -0.0985020  -106.274    -8.922  
-22 419 59688.00 I  0.066169 0.000023  0.460809 0.000016  I-0.0988174 0.0000075  0.2225 0.0042  I  -106.734    0.806    -9.084    0.015  0.066192  0.460869 -0.0988272  -106.773    -9.104  
-22 420 59689.00 I  0.068331 0.000027  0.462008 0.000026  I-0.0989000 0.0000041 -0.0756 0.0043  I  -106.892    0.792    -9.298    0.084  0.068329  0.461999 -0.0988949  -106.960    -9.291  
-22 421 59690.00 I  0.070493 0.000026  0.463048 0.000026  I-0.0986843 0.0000043 -0.3196 0.0032  I  -106.639    0.792    -9.423    0.084  0.070468  0.463064 -0.0987060  -106.695    -9.434  
-22 422 59691.00 I  0.072758 0.000023  0.464119 0.000027  I-0.0983194 0.0000049 -0.3878 0.0033  I  -106.183    0.792    -9.469    0.084  0.072707  0.464098 -0.0983386  -106.211    -9.508  
-22 423 59692.00 I  0.075224 0.000022  0.465083 0.000026  I-0.0979269 0.0000049 -0.4013 0.0037  I  -105.770    0.792    -9.496    0.084  0.075204  0.465058 -0.0979051  -105.797    -9.527  
-22 424 59693.00 I  0.077856 0.000017  0.466283 0.000040  I-0.0975412 0.0000056 -0.3417 0.0037  I  -105.474    0.768    -9.537    0.101  0.077859  0.466247 -0.0975194  -105.498    -9.555  
-22 425 59694.00 I  0.080485 0.000015  0.467920 0.000040  I-0.0972766 0.0000056 -0.1828 0.0055  I  -105.254    0.768    -9.578    0.101  0.080557  0.467896 -0.0972632  -105.265    -9.590  
-22 426 59695.00 I  0.082817 0.000012  0.469862 0.000035  I-0.0971782 0.0000095 -0.0162 0.0040  I  -105.108    0.734    -9.591    0.070  0.082859  0.469891 -0.0971847  -105.109    -9.593  
-22 427 59696.00 I  0.084841 0.000019  0.471453 0.000035  I-0.0972281 0.0000058  0.1021 0.0055  I  -105.101    0.742    -9.539    0.138  0.084908  0.471486 -0.0972203  -105.096    -9.548  
-22 428 59697.00 I  0.086493 0.000020  0.472743 0.000035  I-0.0973574 0.0000055  0.1456 0.0043  I  -105.262    0.742    -9.389    0.138  0.086518  0.472819 -0.0973522  -105.258    -9.407  
-22 429 59698.00 I  0.087931 0.000020  0.473543 0.000036  I-0.0974953 0.0000063  0.1172 0.0041  I  -105.486    0.742    -9.168    0.138  0.087895  0.473595 -0.0974914  -105.480    -9.203  
-22 430 59699.00 I  0.089677 0.000019  0.474074 0.000012  I-0.0975714 0.0000060  0.0277 0.0043  I  -105.626    0.749    -8.989    0.183  0.089653  0.474104 -0.0975559  -105.614    -9.011  
-22 5 1 59700.00 I  0.091698 0.000020  0.474621 0.000014  I-0.0975428 0.0000060 -0.0854 0.0043  I  -105.649    0.749    -8.979    0.183  0.091728  0.474632 -0.0975257  -105.627    -8.987  
-22 5 2 59701.00 I  0.093634 0.000024  0.475316 0.000020  I-0.0974058 0.0000062 -0.1830 0.0046  I  -105.648    0.749    -9.150    0.116  0.093634  0.475311 -0.0974187  -105.619    -9.154  
-22 5 3 59702.00 I  0.095564 0.000018  0.476114 0.000019  I-0.0971898 0.0000071 -0.2415 0.0044  I  -105.690    0.749    -9.369    0.030  0.095563  0.476140 -0.0972185  -105.662    -9.372  
-22 5 4 59703.00 I  0.097693 0.000023  0.476934 0.000028  I-0.0969119 0.0000062 -0.3327 0.0047  I  -105.741    0.784    -9.492    0.037  0.097691  0.476906 -0.0969126  -105.734    -9.493  
-22 5 5 59704.00 I  0.099820 0.000023  0.477875 0.000028  I-0.0965118 0.0000061 -0.4617 0.0044  I  -105.742    0.784    -9.521    0.037  0.099882  0.477903 -0.0964992  -105.770    -9.526  
-22 5 6 59705.00 I  0.101675 0.000024  0.478832 0.000028  I-0.0960246 0.0000062 -0.4825 0.0043  I  -105.695    0.784    -9.584    0.037  0.101687  0.478833 -0.0960256  -105.754    -9.581  
-22 5 7 59706.00 I  0.103386 0.000024  0.479498 0.000027  I-0.0955678 0.0000062 -0.4402 0.0040  I  -105.575    0.784    -9.772    0.037  0.103404  0.479538 -0.0955546  -105.646    -9.779  
-22 5 8 59707.00 I  0.105106 0.000024  0.480063 0.000027  I-0.0951540 0.0000051 -0.3685 0.0040  I  -105.296    0.796   -10.015    0.102  0.105117  0.480078 -0.0951550  -105.347   -10.030  
-22 5 9 59708.00 I  0.106695 0.000024  0.480513 0.000027  I-0.0948667 0.0000052 -0.1890 0.0036  I  -104.887    0.796   -10.184    0.102  0.106699  0.480537 -0.0949242  -104.904   -10.197  
-22 510 59709.00 I  0.108521 0.000019  0.480973 0.000018  I-0.0947987 0.0000052  0.0588 0.0032  I  -104.622    0.772   -10.246    0.139  0.108427  0.480933 -0.0948334  -104.607   -10.261  
-22 511 59710.00 I  0.110913 0.000019  0.481771 0.000026  I-0.0949980 0.0000037  0.3479 0.0033  I  -104.756    0.770   -10.275    0.158  0.110941  0.481776 -0.0950144  -104.732   -10.281  
-22 512 59711.00 I  0.113494 0.000018  0.482667 0.000026  I-0.0954640 0.0000041  0.5455 0.0031  I  -105.181    0.770   -10.283    0.158  0.113474  0.482707 -0.0954543  -105.174   -10.290  
-22 513 59712.00 I  0.116069 0.000018  0.483383 0.000026  I-0.0960615 0.0000049  0.6605 0.0037  I  -105.539    0.770   -10.145    0.158  0.116107  0.483379 -0.0960629  -105.566   -10.162  
-22 514 59713.00 I  0.118510 0.000014  0.483942 0.000021  I-0.0967521 0.0000061  0.6769 0.0039  I  -105.727    0.768    -9.783    0.175  0.118527  0.483975 -0.0967431  -105.773    -9.799  
-22 515 59714.00 I  0.120714 0.000021  0.484477 0.000032  I-0.0973746 0.0000061  0.5711 0.0044  I  -106.021    0.850    -9.387    0.156  0.120799  0.484444 -0.0973670  -106.086    -9.399  
-22 516 59715.00 I  0.122297 0.000022  0.485288 0.000031  I-0.0978783 0.0000063  0.4174 0.0059  I  -106.570    0.850    -9.269    0.156  0.122385  0.485333 -0.0978659  -106.653    -9.281  
-22 517 59716.00 I  0.123269 0.000022  0.485822 0.000025  I-0.0981863 0.0000101  0.1945 0.0062  I  -107.055    0.996    -9.502    0.128  0.123240  0.485912 -0.0981728  -107.146    -9.513  
-22 518 59717.00 I  0.124657 0.000028  0.485658 0.000040  I-0.0982695 0.0000106 -0.0219 0.0073  I  -107.059    1.005    -9.843    0.134  0.124614  0.485666 -0.0982338  -107.148    -9.846  
-22 519 59718.00 I  0.126491 0.000027  0.485546 0.000040  I-0.0981575 0.0000105 -0.1934 0.0076  I  -106.589    1.005   -10.040    0.134  0.126492  0.485563 -0.0980742  -106.655   -10.034  
-22 520 59719.00 I  0.128445 0.000027  0.485605 0.000040  I-0.0979287 0.0000108 -0.2268 0.0081  I  -106.037    1.005   -10.085    0.134  0.128370  0.485536 -0.0979421  -106.062   -10.068  
-22 521 59720.00 I  0.130661 0.000022  0.486032 0.000033  I-0.0977459 0.0000124 -0.1342 0.0070  I  -105.739    1.028   -10.087    0.145  0.130677  0.486020 -0.0977739  -105.765   -10.071  
-22 522 59721.00 I  0.132973 0.000026  0.486744 0.000041  I-0.0976768 0.0000089  0.0077 0.0076  I  -105.717    0.874   -10.070    0.090  0.132949  0.486774 -0.0977075  -105.758   -10.059  
-22 523 59722.00 I  0.135353 0.000026  0.487369 0.000041  I-0.0977624 0.0000088  0.1528 0.0060  I  -105.790    0.874    -9.983    0.090  0.135359  0.487350 -0.0977582  -105.848    -9.982  
-22 524 59723.00 I  0.137677 0.000021  0.488142 0.000028  I-0.0979667 0.0000080  0.2507 0.0055  I  -105.807    0.828    -9.817    0.055  0.137703  0.488205 -0.0979698  -105.891    -9.829  
-22 525 59724.00 I  0.139652 0.000023  0.488534 0.000037  I-0.0982384 0.0000066  0.2722 0.0052  I  -105.793    0.868    -9.608    0.057  0.139642  0.488593 -0.0982642  -105.852    -9.614  
-22 526 59725.00 I  0.141660 0.000022  0.488494 0.000037  I-0.0984847 0.0000065  0.2144 0.0046  I  -105.887    0.868    -9.368    0.057  0.141637  0.488529 -0.0985094  -105.918    -9.361  
-22 527 59726.00 I  0.143579 0.000023  0.488465 0.000037  I-0.0986411 0.0000065  0.0783 0.0046  I  -106.147    0.868    -9.108    0.057  0.143638  0.488445 -0.0986407  -106.153    -9.084  
-22 528 59727.00 I  0.145156 0.000017  0.488364 0.000028  I-0.0986082 0.0000066 -0.1570 0.0047  I  -106.453    0.896    -8.926    0.059  0.145102  0.488400 -0.0986068  -106.467    -8.914  
-22 529 59728.00 I  0.146684 0.000016  0.488245 0.000029  I-0.0983140 0.0000067 -0.4317 0.0045  I  -106.639    0.896    -8.969    0.059  0.146706  0.488268 -0.0983314  -106.669    -8.976  
-22 530 59729.00 I  0.148142 0.000026  0.487967 0.000040  I-0.0977444 0.0000060 -0.7076 0.0048  I  -106.662    0.852    -9.276    0.044  0.148067  0.488086 -0.0977877  -106.716    -9.292  
-22 531 59730.00 I  0.149845 0.000024  0.487088 0.000030  I-0.0969122 0.0000070 -0.9435 0.0042  I  -106.607    0.791    -9.682    0.022  0.149795  0.487092 -0.0969563  -106.700    -9.703  
-22 6 1 59731.00 I  0.152003 0.000030  0.486176 0.000040  I-0.0958957 0.0000059 -1.0646 0.0047  I  -106.571    0.998    -9.951    0.041  0.151943  0.486170 -0.0959109  -106.731    -9.971  
-22 6 2 59732.00 I  0.154335 0.000030  0.485423 0.000040  I-0.0947970 0.0000063 -1.1435 0.0045  I  -106.608    0.998   -10.006    0.041  0.154357  0.485426 -0.0947757  -106.670   -10.005  
-22 6 3 59733.00 I  0.156609 0.000030  0.484774 0.000040  I-0.0936398 0.0000068 -1.1289 0.0046  I  -106.744    0.998    -9.980    0.041  0.156589  0.484781 -0.0936356  -106.660    -9.955  
-22 6 4 59734.00 I  0.158876 0.000030  0.484145 0.000039  I-0.0925762 0.0000067 -1.0032 0.0051  I  -106.914    0.998   -10.017    0.041  0.158889  0.484149 -0.0925602  -106.851    -9.984  
-22 6 5 59735.00 I  0.161158 0.000021  0.483621 0.000028  I-0.0916252 0.0000077 -0.9022 0.0047  I  -106.931    1.250   -10.089    0.057  0.161161  0.483622 -0.0916220  -106.921   -10.058  
-22 6 6 59736.00 I  0.163476 0.000027  0.483151 0.000034  I-0.0907867 0.0000066 -0.7564 0.0053  I  -106.703    1.009   -10.071    0.084  0.163382  0.483150 -0.0908246  -106.715   -10.044  
-22 6 7 59737.00 I  0.166257 0.000021  0.482841 0.000020  I-0.0901364 0.0000073 -0.5384 0.0047  I  -106.450    0.875    -9.941    0.099  0.166198  0.482812 -0.0901686  -106.474    -9.925  
-22 6 8 59738.00 I  0.169366 0.000026  0.482835 0.000040  I-0.0896847 0.0000066 -0.3958 0.0049  I  -106.534    0.903    -9.833    0.086  0.169346  0.482843 -0.0896819  -106.581    -9.834  
-22 6 9 59739.00 I  0.172337 0.000026  0.482859 0.000041  I-0.0893328 0.0000066 -0.2891 0.0047  I  -107.025    0.903    -9.819    0.086  0.172338  0.482895 -0.0893344  -107.056    -9.817  
-22 610 59740.00 I  0.175171 0.000026  0.482888 0.000041  I-0.0890942 0.0000067 -0.2194 0.0047  I  -107.637    0.903    -9.756    0.086  0.175150  0.482907 -0.0890843  -107.652    -9.745  
-22 611 59741.00 I  0.177826 0.000026  0.482630 0.000041  I-0.0888492 0.0000068 -0.2842 0.0044  I  -108.182    0.903    -9.473    0.086  0.177834  0.482720 -0.0888551  -108.201    -9.465  
-22 612 59742.00 I  0.180320 0.000022  0.481995 0.000044  I-0.0884940 0.0000057 -0.4445 0.0044  I  -108.787    0.773    -9.087    0.090  0.180290  0.482016 -0.0885165  -108.809    -9.083  
-22 613 59743.00 I  0.182802 0.000022  0.481217 0.000044  I-0.0879285 0.0000056 -0.6999 0.0041  I  -109.509    0.773    -8.952    0.090  0.182826  0.481258 -0.0879480  -109.531    -8.942  
-22 614 59744.00 I  0.185077 0.000015  0.480375 0.000026  I-0.0870865 0.0000059 -0.9783 0.0039  I  -110.000    0.690    -9.206    0.105  0.185100  0.480403 -0.0870940  -110.036    -9.188  
-22 615 59745.00 I  0.187071 0.000035  0.479276 0.000036  I-0.0859923 0.0000055 -1.1956 0.0040  I  -109.879    0.704    -9.597    0.140  0.187052  0.479331 -0.0859830  -109.873    -9.588  
-22 616 59746.00 I  0.189198 0.000035  0.478011 0.000036  I-0.0847403 0.0000055 -1.2779 0.0039  I  -109.274    0.704    -9.829    0.140  0.189149  0.478024 -0.0847332  -109.222    -9.837  
-22 617 59747.00 I  0.191615 0.000035  0.476727 0.000036  I-0.0834987 0.0000056 -1.1735 0.0049  I  -108.681    0.704    -9.902    0.140  0.191602  0.476728 -0.0834949  -108.594    -9.934  
-22 618 59748.00 I  0.194038 0.000033  0.475538 0.000027  I-0.0824299 0.0000082 -0.9592 0.0054  I  -108.440    0.837    -9.955    0.222  0.194019  0.475550 -0.0824189  -108.365    -9.983  
-22 619 59749.00 I  0.196593 0.000033  0.474522 0.000027  I-0.0815733 0.0000092 -0.7661 0.0051  I  -108.556    0.837    -9.957    0.222  0.196541  0.474534 -0.0815575  -108.509    -9.976  
-22 620 59750.00 I  0.199463 0.000034  0.473569 0.000034  I-0.0808818 0.0000062 -0.6209 0.0055  I  -108.865    0.811    -9.779    0.159  0.199454  0.473574 -0.0808812  -108.836    -9.796  
-22 621 59751.00 I  0.202394 0.000012  0.472814 0.000023  I-0.0803065 0.0000059 -0.5507 0.0039  I  -109.177    0.808    -9.449    0.137  0.202403  0.472799 -0.0803109  -109.153    -9.467  
-22 622 59752.00 I  0.205097 0.000015  0.472255 0.000027  I-0.0797506 0.0000047 -0.5700 0.0038  I  -109.379    0.719    -9.158    0.135  0.205128  0.472282 -0.0797589  -109.347    -9.174  
-22 623 59753.00 I  0.207617 0.000016  0.471607 0.000028  I-0.0791237 0.0000049 -0.7178 0.0034  I  -109.530    0.719    -9.017    0.135  0.207619  0.471645 -0.0791011  -109.587    -9.025  
-22 624 59754.00 I  0.210143 0.000016  0.470771 0.000028  I-0.0783040 0.0000050 -0.8985 0.0035  I  -109.778    0.719    -8.977    0.135  0.210148  0.470821 -0.0782976  -109.961    -8.971  
-22 625 59755.00 I  0.212734 0.000017  0.469692 0.000028  I-0.0773340 0.0000050 -1.0572 0.0034  I  -110.138    0.719    -8.983    0.135  0.212693  0.469719 -0.0773260  -110.305    -8.982  
-22 626 59756.00 I  0.215401 0.000023  0.468441 0.000029  I-0.0761715 0.0000047 -1.2701 0.0035  I  -110.452    0.782    -9.102    0.139  0.215376  0.468485 -0.0761726  -110.571    -9.112  
-22 627 59757.00 I  0.218222 0.000023  0.467029 0.000028  I-0.0748172 0.0000048 -1.4127 0.0038  I  -110.568    0.782    -9.405    0.139  0.218164  0.467038 -0.0748406  -110.659    -9.428  
-22 628 59758.00 I  0.221337 0.000021  0.465597 0.000025  I-0.0733620 0.0000059 -1.5075 0.0040  I  -110.511    0.910    -9.794    0.144  0.221330  0.465623 -0.0733645  -110.576    -9.834  
-22 629 59759.00 I  0.224404 0.000022  0.464144 0.000038  I-0.0718066 0.0000065 -1.5892 0.0046  I  -110.442    0.947   -10.029    0.126  0.224443  0.464165 -0.0718011  -110.473   -10.052  
-22 630 59760.00 I  0.227228 0.000022  0.462598 0.000037  I-0.0702105 0.0000070 -1.5903 0.0048  I  -110.497    0.947    -9.979    0.126  0.227220  0.462671 -0.0702118  -110.474    -9.975  
-22 7 1 59761.00 I  0.230018 0.000022  0.460847 0.000037  I-0.0686605 0.0000072 -1.4879 0.0066  I  -110.702    0.947    -9.759    0.126  0.230002  0.460818 -0.0686663  -110.599    -9.722  
-22 7 2 59762.00 I  0.232934 0.000011  0.459215 0.000031  I-0.0672410 0.0000112 -1.3668 0.0058  I  -110.971    1.012    -9.587    0.082  0.232881  0.459225 -0.0672447  -110.959    -9.582  
-22 7 3 59763.00 I  0.236097 0.000015  0.457823 0.000041  I-0.0659491 0.0000092 -1.1793 0.0072  I  -111.139    0.873    -9.531    0.141  0.236109  0.457809 -0.0659625  -111.150    -9.536  
-22 7 4 59764.00 I  0.239191 0.000015  0.456540 0.000041  I-0.0649146 0.0000090 -0.8952 0.0058  I  -111.087    0.873    -9.488    0.141  0.239234  0.456579 -0.0649159  -111.121    -9.498  
-22 7 5 59765.00 I  0.241894 0.000013  0.455121 0.000035  I-0.0641420 0.0000072 -0.6610 0.0055  I  -110.909    0.820    -9.377    0.171  0.241892  0.455171 -0.0641393  -110.976    -9.390  
-22 7 6 59766.00 I  0.244459 0.000013  0.453293 0.000035  I-0.0635560 0.0000062 -0.5365 0.0048  I  -110.895    0.820    -9.261    0.171  0.244450  0.453302 -0.0635337  -110.950    -9.262  
-22 7 7 59767.00 I  0.247125 0.000013  0.451608 0.000035  I-0.0630519 0.0000063 -0.4634 0.0045  I  -111.265    0.820    -9.236    0.171  0.247124  0.451582 -0.0630501  -111.305    -9.226  
-22 7 8 59768.00 I  0.249746 0.000013  0.450109 0.000035  I-0.0625976 0.0000065 -0.4853 0.0047  I  -111.936    0.820    -9.244    0.171  0.249756  0.450120 -0.0625785  -111.978    -9.228  
-22 7 9 59769.00 I  0.252293 0.000009  0.448653 0.000024  I-0.0620343 0.0000071 -0.6483 0.0038  I  -112.679    0.877    -9.148    0.179  0.252297  0.448682 -0.0620271  -112.723    -9.129  
-22 710 59770.00 I  0.254694 0.000016  0.447028 0.000025  I-0.0612804 0.0000041 -0.8732 0.0043  I  -113.384    0.803    -8.977    0.143  0.254733  0.447060 -0.0612967  -113.423    -8.960  
-22 711 59771.00 I  0.256801 0.000016  0.445401 0.000017  I-0.0602888 0.0000047 -1.0954 0.0031  I  -113.968    0.771    -8.953    0.116  0.256857  0.445395 -0.0603249  -114.007    -8.936  
-22 712 59772.00 I  0.258321 0.000017  0.443917 0.000017  I-0.0591188 0.0000047 -1.2300 0.0030  I  -114.198    0.771    -9.165    0.116  0.258411  0.443974 -0.0591324  -114.246    -9.142  
-22 713 59773.00 I  0.259223 0.000017  0.442026 0.000020  I-0.0578269 0.0000037 -1.3704 0.0030  I  -113.927    0.783    -9.408    0.153  0.259174  0.442066 -0.0577813  -113.960    -9.403  
-22 714 59774.00 I  0.260256 0.000017  0.439915 0.000020  I-0.0564445 0.0000038 -1.3115 0.0027  I  -113.400    0.783    -9.466    0.153  0.260201  0.439888 -0.0564587  -113.418    -9.484  
-22 715 59775.00 I  0.261705 0.000018  0.438129 0.000019  I-0.0552622 0.0000040 -1.0778 0.0036  I  -113.026    0.783    -9.421    0.153  0.261642  0.438122 -0.0552630  -113.037    -9.466  
-22 716 59776.00 I  0.263451 0.000013  0.436348 0.000018  I-0.0542801 0.0000061 -0.8706 0.0029  I  -112.967    0.808    -9.463    0.195  0.263441  0.436373 -0.0542876  -112.983    -9.496  
-22 717 59777.00 I  0.265296 0.000017  0.434376 0.000019  I-0.0535137 0.0000041 -0.6852 0.0037  I  -113.148    0.864    -9.534    0.136  0.265267  0.434398 -0.0535228  -113.161    -9.544  
-22 718 59778.00 I  0.267260 0.000017  0.432334 0.000019  I-0.0528832 0.0000041 -0.5794 0.0031  I  -113.505    0.864    -9.412    0.136  0.267234  0.432352 -0.0528927  -113.506    -9.398  
-22 719 59779.00 I  0.269239 0.000018  0.430284 0.000014  I-0.0523133 0.0000046 -0.5984 0.0029  I  -113.979    0.894    -9.081    0.066  0.269260  0.430298 -0.0523068  -113.947    -9.037  
-22 720 59780.00 I  0.270985 0.000025  0.428191 0.000029  I-0.0516619 0.0000042 -0.6910 0.0032  I  -114.405    0.821    -8.811    0.126  0.270974  0.428173 -0.0516628  -114.393    -8.784  
-22 721 59781.00 I  0.272566 0.000025  0.426252 0.000029  I-0.0509175 0.0000044 -0.8252 0.0031  I  -114.656    0.821    -8.809    0.126  0.272574  0.426255 -0.0508922  -114.674    -8.805  
-22 722 59782.00 I  0.274104 0.000025  0.424462 0.000030  I-0.0499868 0.0000046 -1.0336 0.0040  I  -114.827    0.821    -9.001    0.126  0.274053  0.424453 -0.0499591  -114.884    -9.018  
-22 723 59783.00 I  0.275661 0.000023  0.422673 0.000029  I-0.0488637 0.0000068 -1.2019 0.0038  I  -115.068    0.680    -9.190    0.176  0.275681  0.422673 -0.0488673  -115.096    -9.210  
-22 724 59784.00 I  0.277055 0.000023  0.420910 0.000035  I-0.0475899 0.0000061 -1.3494 0.0045  I  -115.345    0.776    -9.322    0.182  0.277006  0.420915 -0.0476028  -115.333    -9.343  
-22 725 59785.00 I  0.278485 0.000023  0.419325 0.000035  I-0.0461853 0.0000059 -1.4356 0.0051  I  -115.498    0.776    -9.491    0.182  0.278471  0.419285 -0.0462003  -115.452    -9.519  
-22 726 59786.00 I  0.279855 0.000014  0.417904 0.000025  I-0.0447445 0.0000082 -1.4443 0.0052  I  -115.482    0.870    -9.730    0.190  0.279867  0.417962 -0.0447491  -115.399    -9.768  
-22 727 59787.00 I  0.281074 0.000023  0.416119 0.000039  I-0.0432977 0.0000086 -1.4500 0.0062  I  -115.416    0.830    -9.900    0.179  0.281044  0.416126 -0.0432579  -115.379    -9.934  
-22 728 59788.00 I  0.282267 0.000023  0.414141 0.000038  I-0.0418469 0.0000093 -1.4487 0.0070  I  -115.408    0.830    -9.844    0.179  0.282267  0.414205 -0.0417953  -115.431    -9.867  
-22 729 59789.00 I  0.283372 0.000022  0.411848 0.000038  I-0.0404312 0.0000111 -1.3549 0.0101  I  -115.451    0.830    -9.589    0.179  0.283345  0.411841 -0.0404282  -115.538    -9.595  
-22 730 59790.00 I  0.284624 0.000021  0.409427 0.000032  I-0.0391829 0.0000179 -1.1239 0.0077  I  -115.481    0.671    -9.334    0.152  0.284587  0.409400 -0.0392089  -115.593    -9.353  
-22 731 59791.00 I  0.285988 0.000025  0.407284 0.000041  I-0.0381740 0.0000107 -0.9213 0.0104  I  -115.463    0.777    -9.232    0.276  0.286000  0.407286 -0.0381849  -115.593    -9.273  
-22 8 1 59792.00 I  0.287130 0.000025  0.405197 0.000041  I-0.0373444 0.0000107 -0.7063 0.0069  I  -115.386    0.777    -9.258    0.276  0.287161  0.405194 -0.0373892  -115.536    -9.320  
-22 8 2 59793.00 I  0.287887 0.000019  0.403236 0.000032  I-0.0367524 0.0000088 -0.5181 0.0068  I  -115.276    0.760    -9.288    0.277  0.287882  0.403262 -0.0367846  -115.439    -9.376  
-22 8 3 59794.00 I  0.288545 0.000019  0.400998 0.000032  I-0.0362662 0.0000084 -0.4557 0.0057  I  -115.252    0.760    -9.258    0.277  0.288468  0.401019 -0.0362792  -115.414    -9.314  
-22 8 4 59795.00 I  0.289527 0.000020  0.398720 0.000032  I-0.0358181 0.0000073 -0.4618 0.0055  I  -115.487    0.760    -9.205    0.277  0.289489  0.398709 -0.0358145  -115.635    -9.222  
-22 8 5 59796.00 I  0.290537 0.000019  0.396553 0.000032  I-0.0353231 0.0000071 -0.5264 0.0052  I  -116.042    0.760    -9.178    0.277  0.290582  0.396579 -0.0353263  -116.154    -9.192  
-22 8 6 59797.00 I  0.291094 0.000015  0.394197 0.000017  I-0.0347348 0.0000073 -0.6826 0.0044  I  -116.770    0.717    -9.178    0.251  0.291080  0.394221 -0.0347316  -116.838    -9.204  
-22 8 7 59798.00 I  0.291548 0.000021  0.391643 0.000021  I-0.0339401 0.0000052 -0.8924 0.0047  I  -117.409    0.700    -9.224    0.255  0.291487  0.391652 -0.0339451  -117.435    -9.261  
-22 8 8 59799.00 I  0.292337 0.000020  0.389021 0.000014  I-0.0329722 0.0000058 -1.0357 0.0039  I  -117.722    0.685    -9.355    0.258  0.292293  0.389056 -0.0329721  -117.715    -9.399  
-22 8 9 59800.00 I  0.293210 0.000019  0.386220 0.000014  I-0.0318940 0.0000058 -1.1032 0.0037  I  -117.607    0.685    -9.520    0.258  0.293211  0.386232 -0.0318918  -117.585    -9.565  
-22 810 59801.00 I  0.293835 0.000021  0.383251 0.000026  I-0.0308084 0.0000045 -1.0430 0.0039  I  -117.203    0.743    -9.546    0.269  0.293803  0.383250 -0.0308088  -117.149    -9.591  
-22 811 59802.00 I  0.294451 0.000021  0.380334 0.000027  I-0.0298561 0.0000051 -0.8386 0.0036  I  -116.848    0.743    -9.352    0.269  0.294459  0.380298 -0.0298577  -116.770    -9.397  
-22 812 59803.00 I  0.295060 0.000021  0.377818 0.000027  I-0.0291393 0.0000057 -0.6098 0.0043  I  -116.775    0.743    -9.121    0.269  0.295055  0.377755 -0.0291384  -116.681    -9.171  
-22 813 59804.00 I  0.295579 0.000015  0.375709 0.000025  I-0.0286242 0.0000068 -0.4179 0.0043  I  -116.898    0.780    -9.090    0.278  0.295537  0.375740 -0.0286307  -116.834    -9.134  
-22 814 59805.00 I  0.296373 0.000014  0.373568 0.000025  I-0.0282806 0.0000064 -0.2948 0.0046  I  -117.029    0.780    -9.224    0.278  0.296313  0.373591 -0.0282983  -117.006    -9.266  
-22 815 59806.00 I  0.297512 0.000015  0.371304 0.000029  I-0.0279874 0.0000063 -0.3135 0.0064  I  -117.196    0.779    -9.256    0.230  0.297500  0.371314 -0.0279699  -117.203    -9.307  
-22 816 59807.00 I  0.298550 0.000014  0.369042 0.000019  I-0.0276157 0.0000110 -0.4461 0.0065  I  -117.539    0.779    -9.069    0.125  0.298583  0.369059 -0.0276395  -117.555    -9.139  
-22 817 59808.00 I  0.299277 0.000019  0.366742 0.000030  I-0.0270842 0.0000114 -0.6119 0.0080  I  -118.001    0.760    -8.854    0.125  0.299254  0.366732 -0.0270866  -118.003    -8.949  
-22 818 59809.00 I  0.299910 0.000020  0.364400 0.000031  I-0.0263618 0.0000115 -0.8682 0.0081  I  -118.372    0.760    -8.836    0.125  0.299866  0.364425 -0.0263517  -118.274    -8.865  
-22 819 59810.00 I  0.300903 0.000020  0.362025 0.000030  I-0.0253584 0.0000115 -1.0929 0.0083  I  -118.566    0.760    -8.999    0.125  0.300823  0.362010 -0.0253455  -118.335    -8.928  
-22 820 59811.00 I  0.302125 0.000020  0.359758 0.000030  I-0.0241888 0.0000120 -1.2792 0.0073  I  -118.672    0.760    -9.151    0.125  0.302176  0.359779 -0.0241871  -118.439    -9.105  
-22 821 59812.00 I  0.303009 0.000024  0.357421 0.000041  I-0.0228220 0.0000091 -1.3997 0.0074  I  -118.743    0.614    -9.185    0.108  0.302992  0.357455 -0.0228266  -118.572    -9.196  
-22 822 59813.00 I  0.303768 0.000023  0.354930 0.000041  I-0.0214199 0.0000088 -1.4289 0.0058  I  -118.711    0.614    -9.191    0.108  0.303769  0.354926 -0.0213929  -118.632    -9.243  
-22 823 59814.00 I  0.304486 0.000019  0.352484 0.000034  I-0.0199959 0.0000073 -1.3632 0.0052  I  -118.541    0.616    -9.290    0.104  0.304513  0.352500 -0.0199836  -118.587    -9.375  
-22 824 59815.00 I  0.304888 0.000018  0.349901 0.000039  I-0.0187048 0.0000057 -1.2636 0.0047  I  -118.308    0.714    -9.445    0.131  0.304896  0.349874 -0.0186613  -118.307    -9.531  
-22 825 59816.00 I  0.305185 0.000018  0.347450 0.000039  I-0.0174463 0.0000059 -1.2314 0.0040  I  -118.107    0.714    -9.495    0.131  0.305201  0.347486 -0.0174037  -118.023    -9.577  
-22 826 59817.00 I  0.305355 0.000017  0.344924 0.000039  I-0.0162886 0.0000056 -1.0596 0.0044  I  -117.944    0.714    -9.357    0.131  0.305398  0.344912 -0.0162851  -117.767    -9.438  
-22 827 59818.00 I  0.305270 0.000010  0.342339 0.000023  I-0.0153432 0.0000065 -0.8395 0.0038  I  -117.795    0.895    -9.125    0.159  0.305290  0.342335 -0.0153482  -117.637    -9.193  
-22 828 59819.00 I  0.304966 0.000020  0.339915 0.000030  I-0.0146130 0.0000051 -0.6090 0.0041  I  -117.681    0.774    -8.981    0.178  0.304974  0.339946 -0.0146136  -117.565    -9.035  
-22 829 59820.00 I  0.304625 0.000020  0.337394 0.000030  I-0.0141175 0.0000049 -0.4014 0.0037  I  -117.644    0.774    -9.007    0.178  0.304586  0.337401 -0.0140968  -117.551    -9.055  
-22 830 59821.00 I  0.304498 0.000020  0.334986 0.000023  I-0.0137965 0.0000053 -0.2348 0.0032  I  -117.661    0.717    -9.129    0.191  0.304464  0.334971 -0.0137838  -117.601    -9.176  
-22 831 59822.00 I  0.304617 0.000022  0.332728 0.000027  I-0.0136230 0.0000040 -0.1431 0.0034  I  -117.689    0.747    -9.210    0.165  0.304595  0.332751 -0.0136099  -117.612    -9.248  
-22 9 1 59823.00 I  0.304750 0.000022  0.330386 0.000027  I-0.0134686 0.0000041 -0.1767 0.0032  I  -117.787    0.747    -9.184    0.165  0.304814  0.330440 -0.0134836  -117.693    -9.211  
-22 9 2 59824.00 I  0.304506 0.000022  0.327664 0.000027  I-0.0132462 0.0000050 -0.2806 0.0035  I  -118.070    0.747    -9.104    0.165  0.304501  0.327651 -0.0132494  -118.154    -9.102  
-22 9 3 59825.00 I  0.304210 0.000012  0.325045 0.000017  I-0.0128899 0.0000057 -0.4371 0.0043  I  -118.518    0.778    -9.070    0.133  0.304186  0.324993 -0.0128821  -118.590    -9.080  
-22 9 4 59826.00 I  0.304085 0.000015  0.322759 0.000024  I-0.0123677 0.0000070 -0.6065 0.0046  I  -118.883    0.750    -9.143    0.193  0.304085  0.322764 -0.0123741  -118.929    -9.170  
-22 9 5 59827.00 I  0.303787 0.000015  0.320457 0.000023  I-0.0117012 0.0000071 -0.7029 0.0075  I  -118.887    0.750    -9.283    0.193  0.303820  0.320481 -0.0117203  -118.916    -9.328  
-22 9 6 59828.00 I  0.303228 0.000014  0.317957 0.000019  I-0.0110127 0.0000133 -0.6468 0.0063  I  -118.480    0.719    -9.351    0.246  0.303248  0.318029 -0.0110190  -118.525    -9.426  
-22 9 7 59829.00 I  0.302620 0.000015  0.314925 0.000027  I-0.0104235 0.0000103 -0.5430 0.0082  I  -117.922    0.887    -9.202    0.188  0.302652  0.314951 -0.0103738  -117.930    -9.248  
-22 9 8 59830.00 I  0.301723 0.000016  0.311761 0.000028  I-0.0099635 0.0000097 -0.3287 0.0072  I  -117.587    0.887    -8.845    0.188  0.301793  0.311758 -0.0099952  -117.557    -8.853  
-22 9 9 59831.00 I  0.300346 0.000017  0.308693 0.000029  I-0.0097973 0.0000102 -0.0208 0.0068  I  -117.613    0.887    -8.495    0.188  0.300297  0.308670 -0.0098037  -117.537    -8.461  
-22 910 59832.00 I  0.299161 0.000014  0.305663 0.000024  I-0.0098957 0.0000095  0.2087 0.0058  I  -117.807    1.155    -8.381    0.070  0.299086  0.305665 -0.0098938  -117.785    -8.354  
-22 911 59833.00 I  0.298571 0.000024  0.302851 0.000036  I-0.0101846 0.0000057  0.3481 0.0055  I  -117.909    1.007    -8.506    0.141  0.298524  0.302843 -0.0101991  -117.949    -8.495  
-22 912 59834.00 I  0.298128 0.000024  0.300270 0.000036  I-0.0105534 0.0000057  0.3720 0.0042  I  -117.924    1.007    -8.664    0.141  0.298153  0.300265 -0.0105663  -118.003    -8.665  
-22 913 59835.00 I  0.297554 0.000024  0.297926 0.000032  I-0.0108733 0.0000062  0.2298 0.0037  I  -118.064    0.934    -8.704    0.175  0.297509  0.297897 -0.0108687  -118.179    -8.722  
-22 914 59836.00 I  0.296978 0.000025  0.295807 0.000051  I-0.0109921 0.0000048  0.0247 0.0040  I  -118.400    0.930    -8.681    0.134  0.296992  0.295809 -0.0110048  -118.515    -8.694  
-22 915 59837.00 I  0.296334 0.000024  0.293809 0.000051  I-0.0109032 0.0000049 -0.2389 0.0034  I  -118.757    0.930    -8.727    0.134  0.296326  0.293853 -0.0109071  -118.881    -8.735  
-22 916 59838.00 I  0.295609 0.000024  0.291699 0.000051  I-0.0105284 0.0000048 -0.4602 0.0039  I  -118.920    0.930    -8.842    0.134  0.295633  0.291666 -0.0105453  -119.064    -8.840  
-22 917 59839.00 I  0.294744 0.000015  0.289611 0.000043  I-0.0099908 0.0000061 -0.6573 0.0035  I  -118.830    0.926    -8.900    0.072  0.294765  0.289613 -0.0099966  -118.954    -8.905  
-22 918 59840.00 I  0.293576 0.000020  0.287789 0.000057  I-0.0092324 0.0000052 -0.7984 0.0040  I  -118.558    0.998    -8.834    0.118  0.293594  0.287789 -0.0092502  -118.640    -8.844  
-22 919 59841.00 I  0.292285 0.000020  0.285843 0.000056  I-0.0084335 0.0000052 -0.8210 0.0040  I  -118.192    0.998    -8.732    0.118  0.292235  0.285928 -0.0084134  -118.223    -8.750  
-22 920 59842.00 I  0.291356 0.000020  0.283523 0.000039  I-0.0075709 0.0000060 -0.9020 0.0035  I  -117.817    1.067    -8.735    0.149  0.291284  0.283515 -0.0075559  -117.778    -8.771  
-22 921 59843.00 I  0.290657 0.000020  0.281046 0.000041  I-0.0066828 0.0000046 -0.8229 0.0037  I  -117.525    0.969    -8.846    0.115  0.290675  0.281089 -0.0066950  -117.531    -8.864  
-22 922 59844.00 I  0.289762 0.000020  0.278371 0.000041  I-0.0059691 0.0000044 -0.6116 0.0034  I  -117.370    0.969    -8.930    0.115  0.289785  0.278400 -0.0059969  -117.441    -8.921  
-22 923 59845.00 I  0.288625 0.000019  0.275550 0.000041  I-0.0054454 0.0000049 -0.4428 0.0038  I  -117.323    0.969    -8.857    0.115  0.288673  0.275532 -0.0054471  -117.457    -8.810  
-22 924 59846.00 I  0.287260 0.000013  0.272936 0.000016  I-0.0050921 0.0000063 -0.2480 0.0036  I  -117.318    0.763    -8.651    0.022  0.287244  0.272949 -0.0051006  -117.468    -8.622  
-22 925 59847.00 I  0.285951 0.000027  0.270430 0.000037  I-0.0049465 0.0000054 -0.0618 0.0041  I  -117.333    0.723    -8.458    0.183  0.285878  0.270404 -0.0049635  -117.484    -8.457  
-22 926 59848.00 I  0.285167 0.000027  0.268165 0.000037  I-0.0049533 0.0000054  0.0787 0.0043  I  -117.383    0.723    -8.414    0.183  0.285103  0.268121 -0.0049793  -117.537    -8.441  
-22 927 59849.00 I  0.284710 0.000027  0.266423 0.000035  I-0.0050996 0.0000066  0.2061 0.0039  I  -117.466    0.699    -8.523    0.247  0.284746  0.266357 -0.0051012  -117.616    -8.597  
-22 928 59850.00 I  0.283878 0.000028  0.264922 0.000035  I-0.0053099 0.0000055  0.1666 0.0041  I  -117.562    0.627    -8.655    0.177  0.283878  0.264953 -0.0053014  -117.693    -8.702  
-22 929 59851.00 I  0.283008 0.000027  0.263304 0.000035  I-0.0053962 0.0000048  0.0171 0.0036  I  -117.663    0.627    -8.692    0.177  0.282943  0.263319 -0.0054180  -117.779    -8.707  
-22 930 59852.00 I  0.282323 0.000027  0.261509 0.000035  I-0.0053342 0.0000048 -0.1623 0.0035  I  -117.778    0.627    -8.623    0.177  0.282338  0.261528 -0.0053388  -117.905    -8.603  
-2210 1 59853.00 I  0.281362 0.000013  0.259745 0.000014  I-0.0050464 0.0000050 -0.4173 0.0034  I  -117.857    0.514    -8.534    0.036  0.281388  0.259744 -0.0049041  -117.934    -8.536  
-2210 2 59854.00 I  0.280043 0.000011  0.257884 0.000014  I-0.0045487 0.0000049 -0.5250 0.0033  I  -117.774    0.514    -8.512    0.036  0.280092  0.257931 -0.0043864  -117.763    -8.633  
-2210 3 59855.00 I  0.278450 0.000018  0.255736 0.000015  I-0.0040472 0.0000043 -0.4801 0.0038  I  -117.410    0.880    -8.557    0.121  0.278478  0.255746 -0.0040146  -117.380    -8.681  
-2210 4 59856.00 I  0.276547 0.000017  0.253520 0.000015  I-0.0035918 0.0000058 -0.4251 0.0030  I  -116.810    1.094    -8.578    0.164  0.276607  0.253527 -0.0035590  -116.777    -8.672  
-2210 5 59857.00 I  0.274395 0.000017  0.251432 0.000021  I-0.0032284 0.0000042 -0.2760 0.0037  I  -116.208    1.048    -8.478    0.140  0.274352  0.251450 -0.0032281  -116.158    -8.550  
-2210 6 59858.00 I  0.272446 0.000021  0.249225 0.000021  I-0.0030735 0.0000047 -0.0259 0.0033  I  -115.870    1.048    -8.246    0.140  0.272409  0.249284 -0.0030816  -115.892    -8.306  
-2210 7 59859.00 I  0.270893 0.000024  0.246721 0.000019  I-0.0031817 0.0000051  0.2393 0.0035  I  -115.873    1.048    -7.990    0.140  0.270869  0.246728 -0.0031810  -115.963    -8.047  
-2210 8 59860.00 I  0.269391 0.000024  0.244284 0.000019  I-0.0035383 0.0000052  0.4630 0.0039  I  -116.056    1.048    -7.831    0.140  0.269464  0.244272 -0.0035337  -116.181    -7.889  
-2210 9 59861.00 I  0.267405 0.000019  0.242149 0.000017  I-0.0040726 0.0000058  0.5813 0.0033  I  -116.188    1.007    -7.792    0.112  0.267436  0.242181 -0.0040628  -116.323    -7.852  
-221010 59862.00 I  0.265327 0.000021  0.239992 0.000019  I-0.0046613 0.0000042  0.5807 0.0038  I  -116.197    0.874    -7.810    0.088  0.265240  0.239987 -0.0046541  -116.330    -7.871  
-221011 59863.00 I  0.263669 0.000021  0.237871 0.000012  I-0.0051858 0.0000050  0.4356 0.0032  I  -116.209    0.740    -7.835    0.055  0.263701  0.237885 -0.0051692  -116.344    -7.899  
-221012 59864.00 I  0.262030 0.000020  0.235728 0.000012  I-0.0055026 0.0000047  0.2007 0.0035  I  -116.363    0.783    -7.883    0.043  0.262046  0.235701 -0.0055011  -116.517    -7.950  
-221013 59865.00 I  0.259880 0.000018  0.233780 0.000012  I-0.0055839 0.0000049 -0.0440 0.0035  I  -116.617    0.783    -7.970    0.043  0.260021  0.233734 -0.0055722  -116.707    -8.023  
-221014 59866.00 I  0.256987 0.000018  0.232088 0.000011  I-0.0054369 0.0000051 -0.2219 0.0036  I  -116.775    0.783    -8.049    0.043  0.256936  0.232102 -0.0054362  -116.793    -8.078  
-221015 59867.00 I  0.254059 0.000018  0.230367 0.000011  I-0.0051795 0.0000053 -0.2815 0.0042  I  -116.667    0.783    -8.045    0.043  0.254063  0.230356 -0.0051876  -116.700    -8.075  
-221016 59868.00 I  0.251191 0.000018  0.228842 0.000026  I-0.0048947 0.0000066 -0.2786 0.0042  I  -116.282    0.899    -7.956    0.072  0.251206  0.228893 -0.0049099  -116.365    -7.987  
-221017 59869.00 I  0.248067 0.000022  0.227228 0.000027  I-0.0046568 0.0000064 -0.1721 0.0050  I  -115.752    0.899    -7.885    0.072  0.248052  0.227286 -0.0046783  -115.804    -7.935  
-221018 59870.00 I  0.245191 0.000020  0.225137 0.000028  I-0.0045624 0.0000075 -0.0299 0.0046  I  -115.218    0.932    -7.935    0.095  0.245102  0.225158 -0.0045660  -115.200    -8.015  
-221019 59871.00 I  0.243016 0.000019  0.222944 0.000034  I-0.0045918 0.0000067  0.0969 0.0050  I  -114.761    0.988    -8.085    0.131  0.243041  0.222898 -0.0045814  -114.747    -8.164  
-221020 59872.00 I  0.240704 0.000020  0.221151 0.000034  I-0.0047742 0.0000067  0.2779 0.0047  I  -114.447    0.988    -8.190    0.131  0.240817  0.221191 -0.0047645  -114.446    -8.265  
-221021 59873.00 I  0.237720 0.000020  0.219311 0.000034  I-0.0051502 0.0000065  0.4669 0.0053  I  -114.357    0.988    -8.118    0.131  0.237688  0.219313 -0.0051434  -114.344    -8.197  
-221022 59874.00 I  0.234655 0.000019  0.217534 0.000023  I-0.0057149 0.0000083  0.6766 0.0048  I  -114.523    1.044    -7.862    0.163  0.234606  0.217522 -0.0057243  -114.532    -7.927  
-221023 59875.00 I  0.232019 0.000015  0.216033 0.000026  I-0.0065072 0.0000070  0.8978 0.0055  I  -114.840    0.896    -7.540    0.137  0.231878  0.216031 -0.0064986  -114.866    -7.589  
-221024 59876.00 I  0.230033 0.000016  0.214646 0.000026  I-0.0074610 0.0000071  0.9706 0.0050  I  -115.124    0.896    -7.301    0.137  0.230043  0.214645 -0.0074339  -115.163    -7.341  
-221025 59877.00 I  0.228137 0.000016  0.213211 0.000023  I-0.0084031 0.0000072  0.9075 0.0050  I  -115.259    0.739    -7.232    0.089  0.228137  0.213232 -0.0084121  -115.318    -7.265  
-221026 59878.00 I  0.226079 0.000016  0.211770 0.000023  I-0.0092495 0.0000071  0.7650 0.0051  I  -115.255    0.739    -7.324    0.089  0.226115  0.211747 -0.0092591  -115.297    -7.349  
-221027 59879.00 I  0.223699 0.000015  0.210386 0.000022  I-0.0098860 0.0000071  0.4812 0.0048  I  -115.194    0.739    -7.484    0.089  0.223756  0.210409 -0.0098856  -115.222    -7.492  
-221028 59880.00 I  0.220829 0.000013  0.208851 0.000022  I-0.0102130 0.0000065  0.2008 0.0054  I  -115.114    0.739    -7.599    0.089  0.220823  0.208832 -0.0102779  -115.143    -7.612  
-221029 59881.00 I  0.217712 0.000013  0.207409 0.000017  I-0.0103254 0.0000081  0.0338 0.0043  I  -114.987    0.748    -7.609    0.051  0.217709  0.207418 -0.0103958  -115.022    -7.628  
-221030 59882.00 I  0.214510 0.000016  0.206265 0.000024  I-0.0102972 0.0000057 -0.0836 0.0047  I  -114.766    0.780    -7.555    0.167  0.214473  0.206229 -0.0103095  -114.810    -7.575  
-221031 59883.00 I  0.211392 0.000016  0.205212 0.000019  I-0.0101973 0.0000049 -0.0839 0.0038  I  -114.440    0.806    -7.516    0.226  0.211345  0.205237 -0.0101927  -114.492    -7.538  
-2211 1 59884.00 I  0.208608 0.000017  0.204242 0.000021  I-0.0101869 0.0000049  0.0882 0.0033  I  -114.044    0.806    -7.509    0.226  0.208514  0.204211 -0.0101774  -114.100    -7.544  
-2211 2 59885.00 I  0.206230 0.000018  0.203468 0.000026  I-0.0104110 0.0000045  0.3720 0.0034  I  -113.657    0.829    -7.483    0.192  0.206235  0.203545 -0.0104065  -113.700    -7.501  
-2211 3 59886.00 I  0.203875 0.000019  0.202379 0.000026  I-0.0109490 0.0000047  0.7099 0.0031  I  -113.378    0.829    -7.392    0.192  0.203841  0.202359 -0.0109528  -113.392    -7.399  
-2211 4 59887.00 I  0.201541 0.000018  0.201374 0.000026  I-0.0118059 0.0000044  0.9730 0.0041  I  -113.284    0.829    -7.243    0.192  0.201477  0.201353 -0.0118134  -113.257    -7.249  
-2211 5 59888.00 I  0.199498 0.000015  0.200681 0.000019  I-0.0128218 0.0000066  1.0165 0.0032  I  -113.375    0.852    -7.059    0.145  0.199403  0.200700 -0.0128173  -113.353    -7.066  
-2211 6 59889.00 I  0.197923 0.000015  0.199801 0.000025  I-0.0138082 0.0000047  0.9680 0.0043  I  -113.545    0.736    -6.862    0.097  0.197880  0.199789 -0.0138349  -113.543    -6.869  
-2211 7 59890.00 I  0.196415 0.000015  0.199008 0.000023  I-0.0147313 0.0000054  0.8401 0.0035  I  -113.642    0.736    -6.683    0.097  0.196436  0.198985 -0.0147274  -113.659    -6.688  
-2211 8 59891.00 I  0.194600 0.000028  0.198378 0.000025  I-0.0154511 0.0000053  0.6003 0.0036  I  -113.614    0.662    -6.585    0.027  0.194574  0.198424 -0.0154466  -113.660    -6.582  
-2211 9 59892.00 I  0.192635 0.000027  0.197577 0.000025  I-0.0159487 0.0000048  0.4110 0.0035  I  -113.553    0.662    -6.626    0.027  0.192696  0.197558 -0.0159684  -113.571    -6.657  
-221110 59893.00 I  0.190360 0.000027  0.196720 0.000025  I-0.0162472 0.0000047  0.1441 0.0032  I  -113.575    0.662    -6.784    0.027  0.190367  0.196722 -0.0162302  -113.564    -6.849  
-221111 59894.00 I  0.187844 0.000027  0.195891 0.000025  I-0.0162361 0.0000041 -0.1252 0.0041  I  -113.643    0.662    -6.941    0.027  0.187822  0.195880 -0.0162520  -113.631    -7.013  
-221112 59895.00 I  0.185418 0.000027  0.195030 0.000018  I-0.0160488 0.0000067 -0.2386 0.0029  I  -113.593    0.739    -6.991    0.002  0.185361  0.195076 -0.0160839  -113.596    -7.056  
-221113 59896.00 I  0.183321 0.000028  0.193962 0.000022  I-0.0157853 0.0000040 -0.2729 0.0038  I  -113.330    0.716    -6.948    0.082  0.183217  0.193981 -0.0158151  -113.352    -6.999  
-221114 59897.00 I  0.181908 0.000014  0.192835 0.000015  I-0.0155290 0.0000034 -0.2294 0.0027  I  -112.924    0.714    -6.924    0.090  0.181786  0.192794 -0.0155444  -112.967    -6.958  
-221115 59898.00 I  0.181149 0.000015  0.192237 0.000015  I-0.0153533 0.0000035 -0.1057 0.0026  I  -112.489    0.714    -6.991    0.090  0.181089  0.192167 -0.0153549  -112.549    -7.008  
-221116 59899.00 I  0.180591 0.000016  0.192106 0.000022  I-0.0153330 0.0000039  0.0641 0.0027  I  -112.067    0.740    -7.083    0.128  0.180613  0.192084 -0.0153236  -112.120    -7.099  
-221117 59900.00 I  0.179829 0.000015  0.192248 0.000023  I-0.0154898 0.0000042  0.2586 0.0029  I  -111.705    0.740    -7.071    0.128  0.179894  0.192217 -0.0154871  -111.735    -7.093  
-221118 59901.00 I  0.178495 0.000016  0.192646 0.000023  I-0.0158574 0.0000044  0.4745 0.0041  I  -111.561    0.740    -6.902    0.128  0.178587  0.192658 -0.0158559  -111.559    -6.936  
-221119 59902.00 I  0.176650 0.000012  0.192925 0.000020  I-0.0164186 0.0000071  0.6297 0.0031  I  -111.786    0.775    -6.640    0.159  0.176631  0.192939 -0.0164100  -111.782    -6.671  
-221120 59903.00 I  0.174676 0.000012  0.192883 0.000023  I-0.0171102 0.0000043  0.7650 0.0041  I  -112.281    0.703    -6.374    0.142  0.174678  0.192941 -0.0171134  -112.283    -6.399  
-221121 59904.00 I  0.172507 0.000012  0.192690 0.000023  I-0.0179166 0.0000042  0.8042 0.0030  I  -112.743    0.703    -6.140    0.142  0.172482  0.192686 -0.0178985  -112.747    -6.164  
-221122 59905.00 I  0.170166 0.000011  0.192510 0.000017  I-0.0186673 0.0000041  0.6894 0.0038  I  -112.971    0.650    -5.974    0.128  0.170135  0.192562 -0.0186627  -112.985    -5.999  
-221123 59906.00 I  0.167914 0.000014  0.192110 0.000035  I-0.0192786 0.0000063  0.5243 0.0038  I  -113.014    0.651    -5.963    0.121  0.167864  0.192125 -0.0192839  -113.015    -5.992  
-221124 59907.00 I  0.165798 0.000014  0.191649 0.000035  I-0.0196865 0.0000064  0.2709 0.0046  I  -112.965    0.651    -6.144    0.121  0.165815  0.191634 -0.0196773  -112.960    -6.178  
-221125 59908.00 I  0.163386 0.000014  0.191406 0.000035  I-0.0198183 0.0000067  0.0111 0.0061  I  -112.800    0.651    -6.380    0.121  0.163449  0.191394 -0.0198119  -112.800    -6.422  
-221126 59909.00 I  0.160411 0.000016  0.191123 0.000034  I-0.0197335 0.0000103 -0.1744 0.0060  I  -112.499    0.651    -6.463    0.113  0.160439  0.191188 -0.0197408  -112.502    -6.504  
-221127 59910.00 I  0.156936 0.000016  0.190783 0.000034  I-0.0195087 0.0000100 -0.2422 0.0064  I  -112.171    0.651    -6.352    0.113  0.156985  0.190819 -0.0195486  -112.173    -6.392  
-221128 59911.00 I  0.153234 0.000016  0.190262 0.000036  I-0.0193018 0.0000077 -0.1519 0.0059  I  -111.942    0.736    -6.211    0.087  0.153168  0.190278 -0.0193141  -111.939    -6.246  
-221129 59912.00 I  0.149942 0.000013  0.189790 0.000016  I-0.0192279 0.0000064  0.0073 0.0047  I  -111.811    0.832    -6.173    0.051  0.149881  0.189736 -0.0192085  -111.789    -6.198  
-221130 59913.00 I  0.147025 0.000017  0.189832 0.000022  I-0.0193202 0.0000054  0.1777 0.0041  I  -111.708    0.751    -6.197    0.094  0.146998  0.189837 -0.0193120  -111.648    -6.204  
-2212 1 59914.00 I  0.144055 0.000021  0.190078 0.000022  I-0.0195939 0.0000051  0.3798 0.0037  I  -111.623    0.751    -6.170    0.094  0.144039  0.190129 -0.0196037  -111.563    -6.191  
-2212 2 59915.00 I  0.141127 0.000021  0.189960 0.000023  I-0.0200307 0.0000051  0.4346 0.0036  I  -111.587    0.751    -6.064    0.094  0.141086  0.190030 -0.0200182  -111.557    -6.103  
-2212 3 59916.00 I  0.138501 0.000021  0.189628 0.000024  I-0.0204323 0.0000051  0.3970 0.0035  I  -111.616    0.751    -5.917    0.094  0.138520  0.189588 -0.0204483  -111.593    -5.954  
-2212 4 59917.00 I  0.135670 0.000022  0.189544 0.000025  I-0.0208113 0.0000048  0.3191 0.0036  I  -111.697    0.814    -5.757    0.131  0.135739  0.189603 -0.0208072  -111.696    -5.787  
-2212 5 59918.00 I  0.132719 0.000023  0.189098 0.000025  I-0.0210310 0.0000050  0.1227 0.0036  I  -111.740    0.814    -5.596    0.131  0.132595  0.189132 -0.0210271  -111.763    -5.625  
-2212 6 59919.00 I  0.130243 0.000023  0.188804 0.000021  I-0.0210519 0.0000053 -0.0881 0.0037  I  -111.650    0.986    -5.494    0.142  0.130234  0.188807 -0.0210546  -111.664    -5.528  
-2212 7 59920.00 I  0.127862 0.000020  0.188834 0.000024  I-0.0208563 0.0000055 -0.2946 0.0039  I  -111.476    0.838    -5.541    0.113  0.127804  0.188914 -0.0208636  -111.530    -5.568  
-2212 8 59921.00 I  0.125542 0.000018  0.188710 0.000023  I-0.0204801 0.0000057 -0.4490 0.0041  I  -111.358    0.838    -5.750    0.113  0.125550  0.188683 -0.0204842  -111.431    -5.765  
-2212 9 59922.00 I  0.123013 0.000018  0.188908 0.000021  I-0.0199683 0.0000061 -0.5733 0.0049  I  -111.367    0.838    -6.002    0.113  0.123051  0.188943 -0.0199575  -111.450    -5.997  
-221210 59923.00 I  0.120044 0.000016  0.189244 0.000016  I-0.0193466 0.0000079 -0.6583 0.0046  I  -111.403    0.680    -6.145    0.074  0.120023  0.189212 -0.0193465  -111.433    -6.148  
-221211 59924.00 I  0.117118 0.000016  0.189440 0.000024  I-0.0186865 0.0000069 -0.6389 0.0052  I  -111.328    0.690    -6.154    0.158  0.117059  0.189519 -0.0187186  -111.306    -6.171  
-221212 59925.00 I  0.114540 0.000014  0.189327 0.000024  I-0.0181000 0.0000069 -0.5260 0.0043  I  -111.104    0.690    -6.137    0.158  0.114474  0.189311 -0.0181257  -111.063    -6.164  
-221213 59926.00 I  0.112258 0.000014  0.189386 0.000024  I-0.0176349 0.0000052 -0.4120 0.0042  I  -110.761    0.814    -6.172    0.193  0.112235  0.189380 -0.0176371  -110.733    -6.213  
-221214 59927.00 I  0.110085 0.000014  0.189773 0.000024  I-0.0172862 0.0000048 -0.2676 0.0034  I  -110.321    0.814    -6.191    0.193  0.110057  0.189733 -0.0172887  -110.324    -6.215  
-221215 59928.00 I  0.107805 0.000014  0.190633 0.000023  I-0.0171043 0.0000043 -0.1095 0.0032  I  -109.852    0.814    -6.076    0.193  0.107848  0.190644 -0.0170929  -109.882    -6.084  
-221216 59929.00 I  0.105273 0.000014  0.191581 0.000023  I-0.0170815 0.0000041  0.0914 0.0030  I  -109.576    0.814    -5.844    0.193  0.105276  0.191662 -0.0170407  -109.642    -5.845  
-221217 59930.00 I  0.102628 0.000011  0.192140 0.000016  I-0.0172736 0.0000041  0.2518 0.0030  I  -109.720    0.903    -5.642    0.178  0.102588  0.192217 -0.0171383  -109.796    -5.644  
-221218 59931.00 I  0.100234 0.000024  0.192465 0.000038  I-0.0175355 0.0000044  0.2635 0.0038  I  -110.233    0.796    -5.555    0.137  0.100160  0.192490 -0.0173664  -110.291    -5.561  
-221219 59932.00 I  0.098289 0.000024  0.192767 0.000037  I-0.0177821 0.0000065  0.2198 0.0031  I  -110.805    0.687    -5.485    0.080  0.098210  0.192803 -0.0177187  -110.824    -5.496  
-221220 59933.00 I  0.096780 0.000026  0.193098 0.000038  I-0.0179687 0.0000045  0.1569 0.0040  I  -111.251    0.630    -5.327    0.078  0.096711  0.193084 -0.0179634  -111.212    -5.340  
-221221 59934.00 I  0.095783 0.000025  0.193369 0.000038  I-0.0180915 0.0000046  0.0808 0.0033  I  -111.661    0.630    -5.201    0.078  0.095777  0.193348 -0.0181234  -111.654    -5.239  
-221222 59935.00 I  0.094827 0.000026  0.194012 0.000039  I-0.0181006 0.0000047 -0.0842 0.0033  I  -112.054    0.630    -5.333    0.078  0.094877  0.193950 -0.0181060  -112.105    -5.394  
-221223 59936.00 I  0.093412 0.000028  0.194949 0.000039  I-0.0179155 0.0000048 -0.2718 0.0033  I  -112.157    0.630    -5.687    0.078  0.093472  0.194922 -0.0178955  -112.150    -5.759  
-221224 59937.00 I  0.091299 0.000019  0.196101 0.000017  I-0.0176065 0.0000047 -0.3109 0.0034  I  -111.801    0.565    -5.935    0.075  0.091397  0.196126 -0.0175841  -111.706    -6.007  
-221225 59938.00 I  0.088380 0.000019  0.197002 0.000016  I-0.0173420 0.0000048 -0.2050 0.0041  I  -111.256    0.565    -5.874    0.075  0.088402  0.197099 -0.0173115  -111.094    -5.943  
-221226 59939.00 I  0.085232 0.000042  0.197368 0.000041  I-0.0172482 0.0000066  0.0561 0.0039  I  -110.922    0.578    -5.678    0.166  0.085204  0.197391 -0.0172323  -110.709    -5.742  
-221227 59940.00 I  0.081991 0.000042  0.197787 0.000041  I-0.0174689 0.0000062  0.3613 0.0044  I  -110.868    0.578    -5.600    0.166  0.082060  0.197809 -0.0174541  -110.623    -5.660  
-221228 59941.00 I  0.078272 0.000044  0.198344 0.000042  I-0.0179183 0.0000057  0.5088 0.0042  I  -110.909    0.656    -5.613    0.153  0.078253  0.198379 -0.0179243  -110.647    -5.673  
-221229 59942.00 I  0.074738 0.000043  0.198601 0.000042  I-0.0184524 0.0000057  0.5538 0.0040  I  -110.946    0.656    -5.528    0.153  0.074744  0.198584 -0.0184719  -110.694    -5.570  
-221230 59943.00 I  0.071203 0.000043  0.199206 0.000041  I-0.0190020 0.0000055  0.5269 0.0040  I  -111.032    0.656    -5.314    0.153  0.071281  0.199199 -0.0190102  -110.793    -5.341  
-221231 59944.00 I  0.067041 0.000043  0.200080 0.000041  I-0.0194825 0.0000057  0.4288 0.0045  I  -111.201    0.656    -5.125    0.153  0.067074  0.200103 -0.0194855  -110.973    -5.182  
-23 1 1 59945.00 I  0.062786 0.000019  0.200919 0.000015  I-0.0198241 0.0000071  0.2244 0.0042  I  -111.392    0.715    -5.058    0.140  0.062699  0.200944 -0.0197967  -111.162    -5.163  
-23 1 2 59946.00 I  0.059055 0.000022  0.201756 0.000023  I-0.0199237 0.0000061 -0.0026 0.0055  I  -111.512    0.573    -5.059    0.097  0.059003  0.201796 -0.0199243  -111.443    -5.114  
-23 1 3 59947.00 I  0.055737 0.000019  0.202460 0.000034  I-0.0198258 0.0000083 -0.2090 0.0053  I  -111.469    0.606    -5.072    0.132  0.055638  0.202514 -0.0198250  -111.467    -5.128  
-23 1 4 59948.00 I  0.052977 0.000019  0.203016 0.000035  I-0.0195029 0.0000087 -0.4239 0.0063  I  -111.218    0.606    -5.156    0.132  0.052933  0.202990 -0.0195007  -111.313    -5.194  
-23 1 5 59949.00 I  0.050803 0.000019  0.203873 0.000036  I-0.0190209 0.0000095 -0.5102 0.0064  I  -110.849    0.606    -5.390    0.132  0.050795  0.203830 -0.0190232  -110.822    -5.531  
-23 1 6 59950.00 I  0.048797 0.000020  0.205075 0.000036  I-0.0185006 0.0000095 -0.5423 0.0066  I  -110.557    0.606    -5.689    0.132  0.048795  0.205101 -0.0184663  -110.510    -5.834  
-23 1 7 59951.00 I  0.046882 0.000019  0.206241 0.000036  I-0.0179517 0.0000093 -0.5281 0.0068  I  -110.422    0.606    -5.873    0.132  0.046853  0.206221 -0.0179143  -110.392    -5.984  
-23 1 8 59952.00 I  0.045143 0.000016  0.207584 0.000032  I-0.0174789 0.0000098 -0.4104 0.0063  I  -110.350    0.816    -5.861    0.177  0.045146  0.207590 -0.0174487  -110.316    -5.948  
-23 1 9 59953.00 I  0.043364 0.000011  0.209053 0.000016  I-0.0171414 0.0000085 -0.2611 0.0063  I  -110.218    0.807    -5.750    0.146  0.043370  0.209111 -0.0171274  -110.159    -5.821  
-23 110 59954.00 I  0.041296 0.000010  0.210242 0.000014  I-0.0169623 0.0000078 -0.0951 0.0055  I  -109.978    0.807    -5.672    0.146  0.041325  0.210288 -0.0169671  -109.874    -5.733  
-23 111 59955.00 I  0.038966 0.000015  0.211106 0.000015  I-0.0169544 0.0000071  0.0806 0.0050  I  -109.660    0.754    -5.624    0.124  0.038979  0.211134 -0.0169747  -109.583    -5.665  
-23 112 59956.00 I  0.036561 0.000014  0.211940 0.000014  I-0.0170840 0.0000062  0.1377 0.0049  I  -109.330    0.754    -5.514    0.124  0.036547  0.211915 -0.0170559  -109.296    -5.533  
-23 113 59957.00 I  0.034182 0.000014  0.213038 0.000014  I-0.0172129 0.0000067  0.1439 0.0059  I  -109.128    0.754    -5.350    0.124  0.034173  0.213022 -0.0172046  -109.147    -5.343  
-23 114 59958.00 I  0.031794 0.000013  0.214424 0.000012  I-0.0173780 0.0000100  0.1685 0.0057  I  -109.206    0.669    -5.284    0.088  0.031810  0.214393 -0.0173877  -109.253    -5.273  
-23 115 59959.00 I  0.029348 0.000016  0.216072 0.000021  I-0.0175473 0.0000092  0.1852 0.0069  I  -109.544    0.637    -5.405    0.113  0.029351  0.216047 -0.0175710  -109.621    -5.396  
-23 116 59960.00 I  0.026873 0.000016  0.217964 0.000021  I-0.0177223 0.0000096  0.1237 0.0073  I  -109.926    0.637    -5.573    0.113  0.026882  0.217923 -0.0177110  -110.037    -5.563  
-23 117 59961.00 I  0.024332 0.000012  0.220219 0.000019  I-0.0177507 0.0000114 -0.0699 0.0070  I  -110.263    0.618    -5.571    0.129  0.024343  0.220214 -0.0177400  -110.403    -5.564  
-23 118 59962.00 I  0.021691 0.000039  0.222446 0.000019  I-0.0175815 0.0000102 -0.2667 0.0075  I  -110.744    0.676    -5.452    0.136  0.021681  0.222504 -0.0175873  -110.857    -5.445  
-23 119 59963.00 I  0.019115 0.000040  0.224215 0.000019  I-0.0172334 0.0000099 -0.4154 0.0071  I  -111.419    0.676    -5.518    0.136  0.019078  0.224261 -0.0172362  -111.474    -5.516  
-23 120 59964.00 I  0.016663 0.000040  0.225636 0.000019  I-0.0167586 0.0000100 -0.5405 0.0081  I  -111.873    0.676    -5.878    0.136  0.016715  0.225678 -0.0167521  -111.849    -5.887  
-23 121 59965.00 I  0.013978 0.000039  0.226843 0.000011  I-0.0161722 0.0000128 -0.6062 0.0061  I  -111.678    0.845    -6.222    0.148  0.014033  0.226892 -0.0161896  -111.635    -6.235  
-23 122 59966.00 I  0.010876 0.000040  0.227751 0.000014  I-0.0156162 0.0000070 -0.4621 0.0072  I  -110.999    0.550    -6.218    0.105  0.010879  0.227740 -0.0156593  -110.964    -6.230  
-23 123 59967.00 I  0.007811 0.000040  0.228860 0.000016  I-0.0152836 0.0000066 -0.2113 0.0047  I  -110.403    0.550    -5.965    0.105  0.007728  0.228830 -0.0153087  -110.393    -5.970  
-23 124 59968.00 I  0.005409 0.000019  0.230211 0.000017  I-0.0152066 0.0000063  0.0787 0.0045  I  -110.171    0.354    -5.799    0.066  0.005300  0.230244 -0.0152158  -110.223    -5.787  
-23 125 59969.00 I  0.003919 0.000023  0.231456 0.000027  I-0.0154123 0.0000062  0.2828 0.0045  I  -110.167    0.569    -5.797    0.149  0.003852  0.231401 -0.0153642  -110.193    -5.799  
-23 126 59970.00 I  0.002888 0.000024  0.233326 0.000029  I-0.0156952 0.0000063  0.2558 0.0043  I  -110.257    0.569    -5.756    0.149  0.002927  0.233231 -0.0156349  -110.268    -5.775  
-23 127 59971.00 I  0.001580 0.000024  0.235870 0.000030  I-0.0159019 0.0000061  0.1627 0.0050  I  -110.440    0.569    -5.596    0.149  0.001593  0.235918 -0.0158886  -110.468    -5.635  
-23 128 59972.00 I  0.000382 0.000022  0.238117 0.000030  I-0.0159939 0.0000077 -0.0105 0.0046  I  -110.658    0.709    -5.505    0.193  0.000279  0.238107 -0.0159862  -110.687    -5.537  
-23 129 59973.00 I -0.000272 0.000026  0.240384 0.000033  I-0.0158863 0.0000070 -0.1675 0.0051  I  -110.780    0.831    -5.637    0.183 -0.000230  0.240378 -0.0158927  -110.794    -5.657  
-23 130 59974.00 I -0.000860 0.000025  0.242657 0.000033  I-0.0156617 0.0000067 -0.3160 0.0051  I  -110.770    0.831    -5.889    0.183 -0.000925  0.242670 -0.0156444  -110.750    -5.905  
-23 131 59975.00 I -0.001399 0.000022  0.245014 0.000026  I-0.0152307 0.0000075 -0.5352 0.0046  I  -110.670    1.146    -6.069    0.163 -0.001326  0.244961 -0.0152262  -110.583    -6.080  
-23 2 1 59976.00 I -0.002309 0.000021  0.247812 0.000044  I-0.0146170 0.0000062 -0.6772 0.0048  I  -110.483    1.038    -6.146    0.176 -0.002296  0.247864 -0.0146010  -110.444    -6.163  
-23 2 2 59977.00 I -0.003561 0.000021  0.250310 0.000044  I-0.0138942 0.0000061 -0.7653 0.0045  I  -110.206    1.038    -6.240    0.176 -0.003547  0.250346 -0.0138591  -110.219    -6.262  
-23 2 3 59978.00 I -0.004904 0.000021  0.252506 0.000043  I-0.0131142 0.0000064 -0.7699 0.0046  I  -109.945    1.038    -6.398    0.176 -0.004856  0.252572 -0.0130960  -109.978    -6.426  
-23 2 4 59979.00 I -0.006471 0.000017  0.254279 0.000041  I-0.0124022 0.0000070 -0.6312 0.0042  I  -109.831    0.944    -6.503    0.187 -0.006428  0.254285 -0.0124190  -109.861    -6.529  
-23 2 5 59980.00 I -0.008209 0.000019  0.255937 0.000041  I-0.0118695 0.0000053 -0.4395 0.0044  I  -109.848    0.729    -6.432    0.154 -0.008204  0.255923 -0.0118777  -109.870    -6.457  
-23 2 6 59981.00 I -0.009960 0.000020  0.257733 0.000041  I-0.0115082 0.0000053 -0.2930 0.0037  I  -109.838    0.729    -6.225    0.154 -0.009964  0.257731 -0.0114958  -109.866    -6.252  
-23 2 7 59982.00 I -0.011916 0.000020  0.259667 0.000017  I-0.0112781 0.0000051 -0.1629 0.0032  I  -109.683    0.541    -6.037    0.116 -0.011876  0.259655 -0.0112745  -109.747    -6.070  
-23 2 8 59983.00 I -0.014092 0.000033  0.261639 0.000038  I-0.0111853 0.0000035 -0.0240 0.0031  I  -109.407    0.739    -5.952    0.086 -0.014175  0.261674 -0.0111959  -109.435    -5.978  
-23 2 9 59984.00 I -0.015723 0.000033  0.263453 0.000038  I-0.0112377 0.0000034  0.1379 0.0026  I  -109.143    0.739    -5.923    0.086 -0.015815  0.263434 -0.0112446  -109.132    -5.933  
-23 210 59985.00 I -0.016726 0.000032  0.265588 0.000038  I-0.0114608 0.0000039  0.2990 0.0031  I  -109.015    0.739    -5.903    0.086 -0.016692  0.265519 -0.0114722  -108.968    -5.888  
-23 211 59986.00 I -0.017893 0.000029  0.268005 0.000037  I-0.0117978 0.0000052  0.3465 0.0029  I  -109.086    0.911    -5.945    0.044 -0.017796  0.268043 -0.0117909  -109.040    -5.942  
-23 212 59987.00 I -0.019635 0.000029  0.270435 0.000037  I-0.0121300 0.0000044  0.3227 0.0034  I  -109.308    0.766    -6.117    0.124 -0.019580  0.270405 -0.0121316  -109.260    -6.133  
-23 213 59988.00 I -0.021943 0.000029  0.273088 0.000038  I-0.0124043 0.0000044  0.1822 0.0035  I  -109.543    0.766    -6.351    0.124 -0.021949  0.273140 -0.0123642  -109.473    -6.379  
-23 214 59989.00 I -0.024483 0.000015  0.275695 0.000018  I-0.0124673 0.0000055 -0.0397 0.0036  I  -109.724    0.669    -6.481    0.163 -0.024489  0.275701 -0.0124632  -109.625    -6.523  
-23 215 59990.00 I -0.026965 0.000028  0.278180 0.000020  I-0.0123414 0.0000058 -0.2120 0.0039  I  -109.979    0.644    -6.487    0.150 -0.026961  0.278194 -0.0123539  -109.980    -6.504  
-23 216 59991.00 I -0.029371 0.000027  0.280690 0.000021  I-0.0120581 0.0000054 -0.3400 0.0040  I  -110.406    0.644    -6.568    0.150 -0.029393  0.280732 -0.0120613  -110.553    -6.554  
-23 217 59992.00 I -0.031759 0.000027  0.282893 0.000023  I-0.0116893 0.0000054 -0.3844 0.0049  I  -110.766    0.644    -6.863    0.150 -0.031780  0.282935 -0.0116902  -111.072    -6.818  
-23 218 59993.00 I -0.033991 0.000025  0.284847 0.000023  I-0.0113602 0.0000081 -0.2161 0.0045  I  -110.672    0.401    -7.189    0.084 -0.034066  0.284869 -0.0113623  -110.935    -7.143  
-23 219 59994.00 I -0.035823 0.000032  0.286845 0.000028  I-0.0113092 0.0000071  0.1087 0.0054  I  -110.105    0.723    -7.250    0.201 -0.035884  0.286825 -0.0113117  -110.257    -7.216  
-23 220 59995.00 I -0.037241 0.000031  0.288962 0.000027  I-0.0115755 0.0000071  0.4273 0.0049  I  -109.463    0.723    -7.046    0.201 -0.037338  0.288920 -0.0115669  -109.509    -7.029  
-23 221 59996.00 I -0.038246 0.000021  0.291495 0.000025  I-0.0121539 0.0000068  0.7162 0.0045  I  -109.083    0.769    -6.853    0.230 -0.038274  0.291422 -0.0121587  -109.019    -6.868  
-23 222 59997.00 I -0.038779 0.000023  0.294616 0.000025  I-0.0129434 0.0000056  0.8116 0.0046  I  -108.997    0.742    -6.809    0.179 -0.038866  0.294588 -0.0129291  -108.925    -6.815  
-23 223 59998.00 I -0.038964 0.000025  0.298256 0.000023  I-0.0137351 0.0000063  0.7809 0.0048  I  -109.136    0.742    -6.788    0.179 -0.038960  0.298263 -0.0137066  -109.077    -6.785  
-23 224 59999.00 I -0.039164 0.000025  0.301855 0.000023  I-0.0144986 0.0000077  0.7305 0.0057  I  -109.461    0.742    -6.697    0.179 -0.039119  0.301926 -0.0145020  -109.413    -6.693  
-23 225 60000.00 I -0.039676 0.000017  0.305101 0.000012  I-0.0151485 0.0000095  0.5375 0.0058  I  -109.838    0.661    -6.674    0.065 -0.039564  0.305114 -0.0151424  -109.790    -6.690  
-23 226 60001.00 I -0.040939 0.000021  0.308169 0.000017  I-0.0155416 0.0000088  0.2486 0.0065  I  -110.068    0.721    -6.866    0.058 -0.040856  0.308232 -0.0155421  -110.020    -6.905  
-23 227 60002.00 I -0.042704 0.000021  0.310720 0.000018  I-0.0156487 0.0000089 -0.0314 0.0076  I  -110.088    0.721    -7.178    0.058 -0.042777  0.310760 -0.0156050  -110.045    -7.236  
-23 228 60003.00 I -0.044028 0.000020  0.313321 0.000018  I-0.0155140 0.0000125 -0.2059 0.0064  I  -109.978    0.881    -7.382    0.021 -0.044051  0.313293 -0.0155019  -109.938    -7.454  
-23 3 1 60004.00 I -0.045094 0.000019  0.316290 0.000019  I-0.0152981 0.0000093 -0.1968 0.0073  I  -109.760    0.860    -7.398    0.122 -0.045086  0.316379 -0.0152786  -109.729    -7.431  
-23 3 2 60005.00 I -0.046059 0.000018  0.318742 0.000019  I-0.0151048 0.0000077 -0.2343 0.0059  I  -109.391    0.860    -7.357    0.122                                                     
-23 3 3 60006.00 I -0.046662 0.000016  0.321114 0.000019  I-0.0148428 0.0000074 -0.2317 0.0053  I  -108.939    0.860    -7.396    0.122                                                     
-23 3 4 60007.00 I -0.046920 0.000012  0.323798 0.000016  I-0.0146892 0.0000072 -0.0856 0.0049  I  -108.601    0.815    -7.476    0.217                                                     
-23 3 5 60008.00 I -0.046594 0.000036  0.326590 0.000019  I-0.0146899 0.0000065  0.1155 0.0047  I  -108.485    0.909    -7.452    0.104                                                     
-23 3 6 60009.00 I -0.045655 0.000037  0.329778 0.000018  I-0.0149303 0.0000060  0.3471 0.0047  I  -108.494    0.909    -7.280    0.104                                                     
-23 3 7 60010.00 I -0.044607 0.000036  0.333305 0.000017  I-0.0153729 0.0000068  0.5452 0.0040  I  -108.473    0.929    -7.082    0.044                                                     
-23 3 8 60011.00 I -0.043512 0.000037  0.336633 0.000016  I-0.0160144 0.0000054  0.7245 0.0042  I  -108.402    0.795    -7.004    0.038                                                     
-23 3 9 60012.00 I -0.042352 0.000037  0.339812 0.000016  I-0.0167934 0.0000050  0.8182 0.0036  I  -108.377    0.795    -7.072    0.038                                                     
-23 310 60013.00 I -0.041303 0.000037  0.343079 0.000015  I-0.0176197 0.0000048  0.8185 0.0031  I  -108.451    0.795    -7.207    0.038                                                     
-23 311 60014.00 I -0.040750 0.000013  0.346411 0.000009  I-0.0184076 0.0000038  0.7504 0.0035  I  -108.577    0.697    -7.341    0.034                                                     
-23 312 60015.00 I -0.040529 0.000013  0.349519 0.000010  I-0.0190955 0.0000050  0.6074 0.0032  I  -108.692    0.740    -7.472    0.052                                                     
-23 313 60016.00 I -0.040089 0.000013  0.352556 0.000010  I-0.0195973 0.0000052  0.3892 0.0041  I  -108.759    0.740    -7.613    0.052                                                     
-23 314 60017.00 I -0.039702 0.000014  0.355962 0.000012  I-0.0199053 0.0000064  0.2651 0.0040  I  -108.752    0.812    -7.748    0.072                                                     
-23 315 60018.00 I -0.039676 0.000014  0.359426 0.000012  I-0.0201092 0.0000062  0.0860 0.0045  I  -108.662    0.812    -7.869    0.072                                                     
-23 316 60019.00 I -0.039798 0.000013  0.362273 0.000012  I-0.0200828 0.0000063 -0.0765 0.0043  I  -108.523    0.812    -8.015    0.072                                                     
-23 317 60020.00 I -0.039667 0.000012  0.364618 0.000012  I-0.0200346 0.0000061 -0.0039 0.0045  I  -108.359    0.812    -8.204    0.072                                                     
-23 318 60021.00 I -0.039055 0.000011  0.366839 0.000011  I-0.0201205 0.0000064  0.2053 0.0036  I  -108.157    0.322    -8.346    0.160                                                     
-23 319 60022.00 I -0.038098 0.000013  0.368982 0.000012  I-0.0204823 0.0000038  0.5260 0.0037  I  -107.940    0.618    -8.312    0.078                                                     
-23 320 60023.00 I -0.036912 0.000009  0.371252 0.000008  I-0.0211481 0.0000037  0.7737 0.0027  I  -107.779    0.618    -8.122    0.078                                                     
-23 321 60024.00 I -0.035479 0.000009  0.373933 0.000008  I-0.0219994 0.0000037  0.9307 0.0029  I  -107.712    0.618    -7.952    0.078                                                     
-23 322 60025.00 I -0.033921 0.000012  0.377070 0.000012  I-0.0229696 0.0000045  0.9681 0.0030  I  -107.716    0.707    -7.911    0.051                                                     
-23 323 60026.00 I -0.032493 0.000012  0.380217 0.000013  I-0.0238906 0.0000046  0.8705 0.0033  I  -107.807    0.707    -7.942    0.051                                                     
-23 324 60027.00 I -0.031182 0.000011  0.383297 0.000013  I-0.0246833 0.0000048  0.6911 0.0036  I  -108.032    0.707    -7.964    0.051                                                     
-23 325 60028.00 I -0.029863 0.000009  0.386398 0.000013  I-0.0252281 0.0000056  0.3777 0.0033  I  -108.331    0.760    -8.024    0.019                                                     
-23 326 60029.00 I -0.028393 0.000014  0.389489 0.000018  I-0.0254387 0.0000045  0.0642 0.0036  I  -108.543    0.803    -8.200    0.111                                                     
-23 327 60030.00 I -0.026607 0.000014  0.392602 0.000018  I-0.0253946 0.0000045 -0.1350 0.0035  I  -108.576    0.803    -8.441    0.111                                                     
-23 328 60031.00 I -0.024709 0.000013  0.395453 0.000016  I-0.0251881 0.0000054 -0.2759 0.0033  I  -108.466    0.855    -8.595    0.160                                                     
-23 329 60032.00 I -0.023045 0.000016  0.397855 0.000020  I-0.0248770 0.0000049 -0.3142 0.0038  I  -108.236    0.748    -8.615    0.111                                                     
-23 330 60033.00 I -0.021724 0.000019  0.400028 0.000021  I-0.0245949 0.0000053 -0.2468 0.0041  I  -107.846    0.748    -8.609    0.111                                                     
-23 331 60034.00 I -0.020386 0.000020  0.402185 0.000021  I-0.0243988 0.0000066 -0.1332 0.0051  I  -107.337    0.748    -8.700    0.111                                                     
-23 4 1 60035.00 I -0.018859 0.000018  0.404604 0.000018  I-0.0243379 0.0000086  0.0086 0.0052  I  -106.905    0.681    -8.858    0.021                                                     
-23 4 2 60036.00 I -0.017328 0.000019  0.407371 0.000020  I-0.0244346 0.0000080  0.2062 0.0057  I  -106.739    0.752    -8.927    0.064                                                     
-23 4 3 60037.00 I -0.015623 0.000019  0.409983 0.000020  I-0.0247491 0.0000074  0.4001 0.0057  I  -106.831    0.752    -8.808    0.064                                                     
-23 4 4 60038.00 I -0.013828 0.000019  0.412632 0.000017  I-0.0252205 0.0000080  0.5511 0.0053  I  -107.017    0.827    -8.572    0.091                                                     
-23 4 5 60039.00 I -0.012262 0.000015  0.415452 0.000016  I-0.0258395 0.0000075  0.6668 0.0045  I  -107.171    0.827    -8.392    0.091                                                     
-23 4 6 60040.00 I -0.010695 0.000014  0.418299 0.000015  I-0.0265260 0.0000042  0.6982 0.0042  I  -107.290    0.827    -8.375    0.091                                                     
-23 4 7 60041.00 I -0.009135 0.000016  0.421177 0.000016  I-0.0272234 0.0000037  0.6921 0.0027  I  -107.415    0.827    -8.494    0.091                                                     
-23 4 8 60042.00 I -0.007828 0.000017  0.423799 0.000013  I-0.0278895 0.0000035  0.6238 0.0034  I  -107.547    0.623    -8.646    0.041                                                     
-23 4 9 60043.00 I -0.006576 0.000020  0.426300 0.000014  I-0.0284459 0.0000056  0.4801 0.0051  I  -107.663    0.623    -8.762    0.041                                                     
-23 410 60044.00 I -0.005292 0.000021  0.428820 0.000031  I-0.0288332 0.0000096  0.2869 0.0052  I  -107.737    0.807    -8.850    0.052                                                     
-23 411 60045.00 I -0.004038 0.000023  0.431406 0.000037  I-0.0290175 0.0000088  0.0872 0.0067  I  -107.717    0.807    -8.951    0.052                                                     
-23 412 60046.00 I -0.002990 0.000027  0.434157 0.000046  I-0.0290319 0.0000094 -0.0397 0.0061  I  -107.512    0.807    -9.085    0.052                                                     
-23 413 60047.00 I -0.002338 0.000032  0.436744 0.000045  I-0.0289827 0.0000085 -0.0327 0.0062  P  -107.117    0.278    -9.229    0.145                                                     
-23 414 60048.00 I -0.001819 0.000034  0.439283 0.000045  I-0.0290127 0.0000081  0.1129 0.0059  P  -106.640    0.288    -9.330    0.148                                                     
-23 415 60049.00 I -0.001066 0.000090  0.441657 0.000092  I-0.0292411 0.0000083  0.3561 0.0060  P  -106.290    0.297    -9.328    0.151                                                     
-23 416 60050.00 I  0.000200 0.000091  0.443585 0.000091  I-0.0297580 0.0000089  0.6984 0.0062  P  -106.224    0.304    -9.210    0.154                                                     
-23 417 60051.00 I  0.001657 0.000090  0.445290 0.000092  I-0.0306114 0.0000093  0.9611 0.0061  P  -106.421    0.309    -9.026    0.155                                                     
-23 418 60052.00 I  0.002987 0.000090  0.446940 0.000092  I-0.0316040 0.0000082  0.9952 0.0062  P  -106.720    0.313    -8.867    0.157                                                     
-23 419 60053.00 I  0.004305 0.000091  0.448616 0.000091  I-0.0325574 0.0000083  0.8959 0.0061  P  -106.960    0.316    -8.786    0.158                                                     
-23 420 60054.00 I  0.005764 0.000091  0.450465 0.000091  I-0.0333667 0.0000089  0.7091 0.0070  P  -107.104    0.318    -8.775    0.158                                                     
-23 421 60055.00 I  0.007427 0.000091  0.452647 0.000091  I-0.0339484 0.0000113  0.4405 0.0076  P  -107.221    0.319    -8.817    0.159                                                     
-23 422 60056.00 I  0.009113 0.000091  0.455146 0.000091  I-0.0342550 0.0000123  0.1938 0.0080  P  -107.362    0.320    -8.923    0.159                                                     
-23 423 60057.00 I  0.010750 0.000091  0.457872 0.000090  I-0.0343540 0.0000114  0.0011 0.0080  P  -107.498    0.321    -9.092    0.160                                                     
-23 424 60058.00 I  0.012658 0.000090  0.460576 0.000091  I-0.0342664 0.0000101 -0.1641 0.0077  P  -107.563    0.321    -9.258    0.160                                                     
-23 425 60059.00 I  0.014958 0.000091  0.462922 0.000093  I-0.0340566 0.0000105 -0.2370 0.0073  P  -107.516    0.321    -9.342    0.160                                                     
-23 426 60060.00 I  0.017303 0.000091  0.465025 0.000091  I-0.0338232 0.0000106 -0.2177 0.0066  P  -107.336    0.321    -9.352    0.160                                                     
-23 427 60061.00 I  0.019415 0.000090  0.467238 0.000090  I-0.0336324 0.0000079                 P  -107.006    0.322    -9.390    0.160                                                     
-23 428 60062.00 P  0.021500 0.000609  0.469218 0.000465  P-0.0335307 0.0001080                 P  -106.558    0.322    -9.531    0.160                                                     
-23 429 60063.00 P  0.023535 0.000904  0.471236 0.000766  P-0.0335677 0.0002041                 P  -106.134    0.322    -9.719    0.160                                                     
-23 430 60064.00 P  0.025626 0.001139  0.473071 0.001025  P-0.0337684 0.0003028                 P  -105.930    0.322    -9.802    0.160                                                     
-23 5 1 60065.00 P  0.027749 0.001342  0.474787 0.001261  P-0.0341255 0.0004021                 P  -106.055    0.322    -9.681    0.160                                                     
-23 5 2 60066.00 P  0.029939 0.001524  0.476435 0.001481  P-0.0346244 0.0005017                 P  -106.433    0.322    -9.411    0.160                                                     
-23 5 3 60067.00 P  0.032223 0.001691  0.478048 0.001689  P-0.0352347 0.0006014                 P  -106.862    0.322    -9.145    0.160                                                     
-23 5 4 60068.00 P  0.034596 0.001846  0.479640 0.001887  P-0.0358935 0.0007012                 P  -107.183    0.322    -9.009    0.160                                                     
-23 5 5 60069.00 P  0.037027 0.001992  0.481213 0.002078  P-0.0364921 0.0007500                 P  -107.387    0.322    -9.031    0.160                                                     
-23 5 6 60070.00 P  0.039491 0.002130  0.482773 0.002262  P-0.0369163 0.0005500                 P  -107.567    0.322    -9.170    0.160                                                     
-23 5 7 60071.00 P  0.041976 0.002262  0.484298 0.002440  P-0.0370816 0.0007548                 P  -107.770    0.322    -9.368    0.160                                                     
-23 5 8 60072.00 P  0.044471 0.002388  0.485767 0.002613  P-0.0370035 0.0009344                 P  -107.919    0.322    -9.572    0.160                                                     
-23 5 9 60073.00 P  0.046977 0.002510  0.487192 0.002782  P-0.0367542 0.0010994                 P  -107.884    0.322    -9.740    0.160                                                     
-23 510 60074.00 P  0.049509 0.002627  0.488582 0.002947  P-0.0364366 0.0012543                 P  -107.610    0.322    -9.846    0.160                                                     
-23 511 60075.00 P  0.052068 0.002740  0.489930 0.003109  P-0.0361623 0.0014016                 P  -107.176    0.322    -9.889    0.160                                                     
-23 512 60076.00 P  0.054642 0.002850  0.491231 0.003267  P-0.0360305 0.0015429                 P  -106.735    0.322    -9.875    0.160                                                     
-23 513 60077.00 P  0.057230 0.002957  0.492483 0.003422  P-0.0361034 0.0016792                 P  -106.431    0.322    -9.806    0.160                                                     
-23 514 60078.00 P  0.059836 0.003061  0.493689 0.003575  P-0.0364047 0.0018113                 P  -106.341    0.322    -9.687    0.160                                                     
-23 515 60079.00 P  0.062464 0.003162  0.494848 0.003725  P-0.0368909 0.0019399                 P  -106.468    0.322    -9.531    0.160                                                     
-23 516 60080.00 P  0.065116 0.003261  0.495960 0.003873  P-0.0374412 0.0020652                 P  -106.743    0.322    -9.351    0.160                                                     
-23 517 60081.00 P  0.067793 0.003358  0.497026 0.004019  P-0.0379318 0.0021877                 P  -107.050    0.322    -9.174    0.160                                                     
-23 518 60082.00 P  0.070491 0.003453  0.498050 0.004163  P-0.0382537 0.0023077                 P  -107.269    0.322    -9.054    0.160                                                     
-23 519 60083.00 P  0.073209 0.003545  0.499036 0.004304  P-0.0383224 0.0024255                 P  -107.352    0.322    -9.061    0.160                                                     
-23 520 60084.00 P  0.075944 0.003636  0.499982 0.004444  P-0.0380999 0.0025411                 P  -107.355    0.322    -9.222    0.160                                                     
-23 521 60085.00 P  0.078692 0.003726  0.500888 0.004583  P-0.0376153 0.0026548                 P  -107.379    0.322    -9.471    0.160                                                     
-23 522 60086.00 P  0.081452 0.003813  0.501753 0.004719  P-0.0369379 0.0027668                 P  -107.461    0.322    -9.677    0.160                                                     
-23 523 60087.00 P  0.084224 0.003900  0.502576 0.004855  P-0.0361511 0.0028772                 P  -107.552    0.322    -9.754    0.160                                                     
-23 524 60088.00 P  0.087007 0.003984  0.503355 0.004988  P-0.0353369 0.0029860                 P  -107.581    0.322    -9.748    0.160                                                     
-23 525 60089.00 P  0.089800 0.004068  0.504090 0.005121  P-0.0345677 0.0030934                 P  -107.508    0.322    -9.780    0.160                                                     
-23 526 60090.00 P  0.092604 0.004150  0.504783 0.005252  P-0.0339047 0.0031995                 P  -107.312    0.322    -9.904    0.160                                                     
-23 527 60091.00 P  0.095417 0.004231  0.505432 0.005381  P-0.0333877 0.0033043                 P  -107.017    0.322   -10.030    0.160                                                     
-23 528 60092.00 P  0.098239 0.004311  0.506037 0.005510  P-0.0330278 0.0034080                 P  -106.763    0.322   -10.018    0.160                                                     
-23 529 60093.00 P  0.101069 0.004390  0.506598 0.005637  P-0.0328174 0.0035105                 P  -106.784    0.322    -9.825    0.160                                                     
-23 530 60094.00 P  0.103906 0.004467  0.507115 0.005764  P-0.0327199 0.0036120                 P  -107.211    0.322    -9.546    0.160                                                     
-23 531 60095.00 P  0.106750 0.004544  0.507589 0.005889  P-0.0326785 0.0037124                 P  -107.889    0.322    -9.304    0.160                                                     
-23 6 1 60096.00 P  0.109601 0.004620  0.508019 0.006013  P-0.0326131 0.0038119                 P  -108.498    0.322    -9.148    0.160                                                     
-23 6 2 60097.00 P  0.112457 0.004694  0.508407 0.006136  P-0.0324290 0.0039105                 P  -108.877    0.322    -9.082    0.160                                                     
-23 6 3 60098.00 P  0.115317 0.004768  0.508750 0.006259  P-0.0320484 0.0040082                 P  -109.134    0.322    -9.140    0.160                                                     
-23 6 4 60099.00 P  0.118180 0.004841  0.509051 0.006380  P-0.0314371 0.0041051                 P  -109.381    0.322    -9.359    0.160                                                     
-23 6 5 60100.00 P  0.121046 0.004913  0.509308 0.006500  P-0.0306248 0.0042012                 P  -109.512    0.322    -9.662    0.160                                                     
-23 6 6 60101.00 P  0.123913 0.004985  0.509522 0.006620  P-0.0297054 0.0042965                 P  -109.359    0.322    -9.875    0.160                                                     
-23 6 7 60102.00 P  0.126782 0.005056  0.509692 0.006739  P-0.0288150 0.0043911                 P  -108.978    0.322    -9.887    0.160                                                     
-23 6 8 60103.00 P  0.129650 0.005125  0.509818 0.006857  P-0.0280774 0.0044849                 P  -108.642    0.322    -9.755    0.160                                                     
-23 6 9 60104.00 P  0.132518 0.005195  0.509901 0.006974  P-0.0275749 0.0045781                 P  -108.551    0.322    -9.608    0.160                                                     
-23 610 60105.00 P  0.135384 0.005263  0.509940 0.007090  P-0.0273112 0.0046706                 P  -108.661    0.322    -9.507    0.160                                                     
-23 611 60106.00 P  0.138249 0.005331  0.509935 0.007206  P-0.0272236 0.0047625                 P  -108.809    0.322    -9.424    0.160                                                     
-23 612 60107.00 P  0.141110 0.005398  0.509887 0.007321  P-0.0272054 0.0048537                 P  -108.920    0.322    -9.315    0.160                                                     
-23 613 60108.00 P  0.143968 0.005465  0.509796 0.007435  P-0.0271323 0.0049444                 P  -109.070    0.322    -9.157    0.160                                                     
-23 614 60109.00 P  0.146822 0.005531  0.509661 0.007549  P-0.0268981 0.0050344                 P  -109.341    0.322    -8.969    0.160                                                     
-23 615 60110.00 P  0.149671 0.005596  0.509483 0.007662  P-0.0264294 0.0051240                 P  -109.673    0.322    -8.825    0.160                                                     
-23 616 60111.00 P  0.152514 0.005661  0.509262 0.007774  P-0.0256968 0.0052129                 P  -109.909    0.322    -8.838    0.160                                                     
-23 617 60112.00 P  0.155350 0.005725  0.508999 0.007885  P-0.0247123 0.0053014                 P  -109.979    0.322    -9.073    0.160                                                     
-23 618 60113.00 P  0.158179 0.005789  0.508692 0.007996  P-0.0235275 0.0053893                 P  -109.974    0.322    -9.446    0.160                                                     
-23 619 60114.00 P  0.161001 0.005852  0.508342 0.008107  P-0.0222220 0.0054768                 P  -110.025    0.322    -9.752    0.160                                                     
-23 620 60115.00 P  0.163813 0.005915  0.507950 0.008217  P-0.0208764 0.0055637                 P  -110.165    0.322    -9.831    0.160                                                     
-23 621 60116.00 P  0.166616 0.005977  0.507516 0.008326  P-0.0195681 0.0056502                 P  -110.343    0.322    -9.712    0.160                                                     
-23 622 60117.00 P  0.169408 0.006039  0.507039 0.008435  P-0.0183613 0.0057362                 P  -110.499    0.322    -9.571    0.160                                                     
-23 623 60118.00 P  0.172189 0.006100  0.506520 0.008543  P-0.0172940 0.0058218                 P  -110.557    0.322    -9.521    0.160                                                     
-23 624 60119.00 P  0.174959 0.006161  0.505960 0.008650  P-0.0163799 0.0059070                 P  -110.442    0.322    -9.496    0.160                                                     
-23 625 60120.00 P  0.177717 0.006221  0.505357 0.008758  P-0.0156112 0.0059917                 P  -110.208    0.322    -9.370    0.160                                                     
-23 626 60121.00 P  0.180461 0.006281  0.504713 0.008864  P-0.0149551 0.0060760                 P  -110.142    0.322    -9.142    0.160                                                     
-23 627 60122.00 P  0.183191 0.006340  0.504028 0.008970  P-0.0143643 0.0061599                 P  -110.555    0.322    -8.958    0.160                                                     
-23 628 60123.00 P  0.185907 0.006399  0.503302 0.009076  P-0.0137728 0.0062434                 P  -111.413    0.322    -8.925    0.160                                                     
-23 629 60124.00 P  0.188608 0.006458  0.502535 0.009181  P-0.0130994 0.0063266                 P  -112.302    0.322    -8.979    0.160                                                     
-23 630 60125.00 P  0.191292 0.006516  0.501727 0.009286  P-0.0122650 0.0064093                 P  -112.871    0.322    -9.003    0.160                                                     
-23 7 1 60126.00 P  0.193960 0.006574  0.500880 0.009390  P-0.0112211 0.0064917                 P  -113.141    0.322    -9.026    0.160                                                     
-23 7 2 60127.00 P  0.196611 0.006632  0.499992 0.009494  P-0.0099751 0.0065737                 P  -113.269    0.322    -9.183    0.160                                                     
-23 7 3 60128.00 P  0.199244 0.006689  0.499064 0.009597  P-0.0085984 0.0066554                 P  -113.215    0.322    -9.455    0.160                                                     
-23 7 4 60129.00 P  0.201858 0.006745  0.498098 0.009700  P-0.0072181 0.0067368                 P  -112.895    0.322    -9.621    0.160                                                     
-23 7 5 60130.00 P  0.204452 0.006802  0.497092 0.009803  P-0.0059789 0.0068177                 P  -112.498    0.322    -9.531    0.160                                                     
-23 7 6 60131.00 P  0.207027 0.006858  0.496047 0.009905  P-0.0049909 0.0068984                 P  -112.373    0.322    -9.315    0.160                                                     
-23 7 7 60132.00 P  0.209581 0.006914  0.494964 0.010006  P-0.0042882 0.0069788                 P  -112.639    0.322    -9.189    0.160                                                     
-23 7 8 60133.00 P  0.212114 0.006969  0.493842 0.010108  P-0.0038173 0.0070588                 P  -113.093    0.322    -9.180    0.160                                                     
-23 7 9 60134.00 P  0.214624 0.007024  0.492683 0.010209  P-0.0034636 0.0071385                 P  -113.469    0.322    -9.160    0.160                                                     
-23 710 60135.00 P  0.217112 0.007079  0.491486 0.010309  P-0.0030867 0.0072179                 P  -113.667    0.322    -9.067    0.160                                                     
-23 711 60136.00 P  0.219577 0.007133  0.490253 0.010409  P-0.0025646 0.0072970                 P  -113.773    0.322    -8.960    0.160                                                     
-23 712 60137.00 P  0.222018 0.007187  0.488982 0.010509  P-0.0018183 0.0073758                                                                                                             
-23 713 60138.00 P  0.224435 0.007241  0.487676 0.010608  P-0.0008148 0.0074544                                                                                                             
-23 714 60139.00 P  0.226826 0.007294  0.486333 0.010707  P 0.0004295 0.0075326                                                                                                             
-23 715 60140.00 P  0.229192 0.007347  0.484955 0.010806  P 0.0018653 0.0076106                                                                                                             
-23 716 60141.00 P  0.231532 0.007400  0.483542 0.010904  P 0.0034216 0.0076883                                                                                                             
-23 717 60142.00 P  0.233844 0.007453  0.482094 0.011002  P 0.0050178 0.0077657                                                                                                             
-23 718 60143.00 P  0.236130 0.007505  0.480612 0.011100  P 0.0065759 0.0078428                                                                                                             
-23 719 60144.00 P  0.238387 0.007557  0.479096 0.011197  P 0.0080291 0.0079197                                                                                                             
-23 720 60145.00 P  0.240616 0.007609  0.477547 0.011294  P 0.0093314 0.0079964                                                                                                             
-23 721 60146.00 P  0.242815 0.007660  0.475964 0.011391  P 0.0104615 0.0080728                                                                                                             
-23 722 60147.00 P  0.244985 0.007712  0.474350 0.011487  P 0.0114255 0.0081489                                                                                                             
-23 723 60148.00 P  0.247125 0.007763  0.472703 0.011583  P 0.0122537 0.0082248                                                                                                             
-23 724 60149.00 P  0.249234 0.007813  0.471025 0.011679  P 0.0129944 0.0083005                                                                                                             
-23 725 60150.00 P  0.251311 0.007864  0.469316 0.011774  P 0.0137082 0.0083759                                                                                                             
-23 726 60151.00 P  0.253357 0.007914  0.467576 0.011869  P 0.0144644 0.0084511                                                                                                             
-23 727 60152.00 P  0.255371 0.007964  0.465806 0.011964  P 0.0153333 0.0085261                                                                                                             
-23 728 60153.00 P  0.257352 0.008014  0.464007 0.012059  P 0.0163704 0.0086008                                                                                                             
-23 729 60154.00 P  0.259299 0.008063  0.462179 0.012153  P 0.0175943 0.0086754                                                                                                             
-23 730 60155.00 P  0.261213 0.008113  0.460322 0.012247  P 0.0189649 0.0087497                                                                                                             
-23 731 60156.00 P  0.263093 0.008162  0.458437 0.012341  P 0.0203776 0.0088237                                                                                                             
-23 8 1 60157.00 P  0.264938 0.008211  0.456525 0.012434  P 0.0216850 0.0088976                                                                                                             
-23 8 2 60158.00 P  0.266748 0.008259  0.454586 0.012527  P 0.0227443 0.0089713                                                                                                             
-23 8 3 60159.00 P  0.268522 0.008308  0.452621 0.012620  P 0.0234766 0.0090448                                                                                                             
-23 8 4 60160.00 P  0.270261 0.008356  0.450629 0.012712  P 0.0238991 0.0091180                                                                                                             
-23 8 5 60161.00 P  0.271963 0.008404  0.448613 0.012805  P 0.0241204 0.0091911                                                                                                             
-23 8 6 60162.00 P  0.273628 0.008452  0.446572 0.012897  P 0.0243034 0.0092639                                                                                                             
-23 8 7 60163.00 P  0.275258 0.008499  0.444505 0.012989  P 0.0246031 0.0093366                                                                                                             
-23 8 8 60164.00 P  0.276849 0.008547  0.442414 0.013080  P 0.0251257 0.0094091                                                                                                             
-23 8 9 60165.00 P  0.278403 0.008594  0.440300 0.013172  P 0.0259117 0.0094814                                                                                                             
-23 810 60166.00 P  0.279919 0.008641  0.438164 0.013263  P 0.0269440 0.0095535                                                                                                             
-23 811 60167.00 P  0.281396 0.008688  0.436007 0.013353  P 0.0281671 0.0096254                                                                                                             
-23 812 60168.00 P  0.282834 0.008734  0.433828 0.013444  P 0.0295067 0.0096971                                                                                                             
-23 813 60169.00 P  0.284232 0.008781  0.431628 0.013534  P 0.0308811 0.0097686                                                                                                             
-23 814 60170.00 P  0.285591 0.008827  0.429409 0.013624  P 0.0322409 0.0098400                                                                                                             
-23 815 60171.00 P  0.286910 0.008873  0.427171 0.013714  P 0.0334934 0.0099112                                                                                                             
-23 816 60172.00 P  0.288189 0.008919  0.424914 0.013804  P 0.0345874 0.0099822                                                                                                             
-23 817 60173.00 P  0.289428 0.008965  0.422639 0.013893  P 0.0354956 0.0100531                                                                                                             
-23 818 60174.00 P  0.290625 0.009010  0.420346 0.013983  P 0.0362182 0.0101238                                                                                                             
-23 819 60175.00 P  0.291782 0.009056  0.418037 0.014072  P 0.0367833 0.0101943                                                                                                             
-23 820 60176.00 P  0.292897 0.009101  0.415712 0.014160  P 0.0372418 0.0102646                                                                                                             
-23 821 60177.00 P  0.293971 0.009146  0.413371 0.014249  P 0.0376592 0.0103348                                                                                                             
-23 822 60178.00 P  0.295003 0.009191  0.411015 0.014337  P 0.0381063 0.0104048                                                                                                             
-23 823 60179.00 P  0.295993 0.009235  0.408645 0.014425  P 0.0386494 0.0104747                                                                                                             
-23 824 60180.00 P  0.296941 0.009280  0.406262 0.014513  P 0.0393405 0.0105444                                                                                                             
-23 825 60181.00 P  0.297846 0.009324  0.403865 0.014601  P 0.0402031 0.0106139                                                                                                             
-23 826 60182.00 P  0.298709 0.009368  0.401457 0.014689  P 0.0412161 0.0106833                                                                                                             
-23 827 60183.00 P  0.299530 0.009413  0.399037 0.014776  P 0.0423017 0.0107526                                                                                                             
-23 828 60184.00 P  0.300307 0.009456  0.396606 0.014863  P 0.0433319 0.0108216                                                                                                             
-23 829 60185.00 P  0.301041 0.009500  0.394165 0.014950  P 0.0441596 0.0108906                                                                                                             
-23 830 60186.00 P  0.301732 0.009544  0.391714 0.015037  P 0.0446683 0.0109594                                                                                                             
-23 831 60187.00 P  0.302380 0.009587  0.389254 0.015123  P 0.0448220 0.0110280                                                                                                             
-23 9 1 60188.00 P  0.302985 0.009631  0.386786 0.015209  P 0.0446878 0.0110965                                                                                                             
-23 9 2 60189.00 P  0.303546 0.009674  0.384310 0.015296  P 0.0444152 0.0111649                                                                                                             
-23 9 3 60190.00 P  0.304063 0.009717  0.381828 0.015381  P 0.0441848 0.0112331                                                                                                             
-23 9 4 60191.00 P  0.304537 0.009760  0.379339 0.015467  P 0.0441487 0.0113012                                                                                                             
-23 9 5 60192.00 P  0.304967 0.009802  0.376845 0.015553  P 0.0443903 0.0113691                                                                                                             
-23 9 6 60193.00 P  0.305353 0.009845  0.374345 0.015638  P 0.0449160 0.0114369                                                                                                             
-23 9 7 60194.00 P  0.305695 0.009887  0.371842 0.015723  P 0.0456738 0.0115046                                                                                                             
-23 9 8 60195.00 P  0.305994 0.009930  0.369335 0.015808  P 0.0465813 0.0115721                                                                                                             
-23 9 9 60196.00 P  0.306249 0.009972  0.366825 0.015893  P 0.0475482 0.0116395                                                                                                             
-23 910 60197.00 P  0.306459 0.010014  0.364313 0.015978  P 0.0484896 0.0117067                                                                                                             
-23 911 60198.00 P  0.306626 0.010056  0.361799 0.016062  P 0.0493323 0.0117739                                                                                                             
-23 912 60199.00 P  0.306750 0.010097  0.359285 0.016147  P 0.0500210 0.0118409                                                                                                             
-23 913 60200.00 P  0.306829 0.010139  0.356770 0.016231  P 0.0505217 0.0119077                                                                                                             
-23 914 60201.00 P  0.306865 0.010181  0.354256 0.016315  P 0.0508275 0.0119745                                                                                                             
-23 915 60202.00 P  0.306856 0.010222  0.351743 0.016399  P 0.0509594 0.0120411                                                                                                             
-23 916 60203.00 P  0.306805 0.010263  0.349232 0.016482  P 0.0509650 0.0121076                                                                                                             
-23 917 60204.00 P  0.306709 0.010304  0.346723 0.016566  P 0.0509108 0.0121740                                                                                                             
-23 918 60205.00 P  0.306571 0.010345  0.344218 0.016649  P 0.0508729 0.0122402                                                                                                             
-23 919 60206.00 P  0.306389 0.010386  0.341716 0.016732  P 0.0509240 0.0123063                                                                                                             
-23 920 60207.00 P  0.306163 0.010427  0.339218 0.016815  P 0.0511197 0.0123723                                                                                                             
-23 921 60208.00 P  0.305895 0.010468  0.336726 0.016898  P 0.0514866 0.0124382                                                                                                             
-23 922 60209.00 P  0.305584 0.010508  0.334240 0.016981  P 0.0520114 0.0125040                                                                                                             
-23 923 60210.00 P  0.305229 0.010549  0.331760 0.017063  P 0.0526331 0.0125696                                                                                                             
-23 924 60211.00 P  0.304832 0.010589  0.329287 0.017146  P 0.0532454 0.0126352                                                                                                             
-23 925 60212.00 P  0.304393 0.010629  0.326822 0.017228  P 0.0537145 0.0127006                                                                                                             
-23 926 60213.00 P  0.303911 0.010669  0.324366 0.017310  P 0.0539128 0.0127659                                                                                                             
-23 927 60214.00 P  0.303387 0.010709  0.321918 0.017392  P 0.0537648 0.0128311                                                                                                             
-23 928 60215.00 P  0.302822 0.010749  0.319480 0.017474  P 0.0532825 0.0128962                                                                                                             
-23 929 60216.00 P  0.302214 0.010789  0.317053 0.017555  P 0.0525721 0.0129612                                                                                                             
-23 930 60217.00 P  0.301565 0.010828  0.314636 0.017637  P 0.0518038 0.0130260                                                                                                             
-2310 1 60218.00 P  0.300875 0.010868  0.312231 0.017718  P 0.0511561 0.0130908                                                                                                             
-2310 2 60219.00 P  0.300144 0.010907  0.309839 0.017799  P 0.0507601 0.0131554                                                                                                             
-2310 3 60220.00 P  0.299372 0.010947  0.307459 0.017880  P 0.0506685 0.0132199                                                                                                             
-2310 4 60221.00 P  0.298560 0.010986  0.305092 0.017961  P 0.0508567 0.0132844                                                                                                             
-2310 5 60222.00 P  0.297708 0.011025  0.302740 0.018042  P 0.0512483 0.0133487                                                                                                             
-2310 6 60223.00 P  0.296815 0.011064  0.300402 0.018123  P 0.0517448 0.0134129                                                                                                             
-2310 7 60224.00 P  0.295884 0.011103  0.298080 0.018203  P 0.0522506 0.0134770                                                                                                             
-2310 8 60225.00 P  0.294912 0.011141  0.295773 0.018284  P 0.0526857 0.0135410                                                                                                             
-2310 9 60226.00 P  0.293902 0.011180  0.293483 0.018364  P 0.0529885 0.0136050                                                                                                             
-231010 60227.00 P  0.292854 0.011219  0.291210 0.018444  P 0.0531202 0.0136688                                                                                                             
-231011 60228.00 P  0.291767 0.011257  0.288955 0.018524  P 0.0530662 0.0137325                                                                                                             
-231012 60229.00 P  0.290642 0.011296  0.286718 0.018604  P 0.0528392 0.0137961                                                                                                             
-231013 60230.00 P  0.289480 0.011334  0.284500 0.018683  P 0.0524778 0.0138596                                                                                                             
-231014 60231.00 P  0.288281 0.011372  0.282301 0.018763  P 0.0520438 0.0139230                                                                                                             
-231015 60232.00 P  0.287044 0.011410  0.280122 0.018842  P 0.0516138 0.0139863                                                                                                             
-231016 60233.00 P  0.285772 0.011448  0.277963 0.018921  P 0.0512674 0.0140495                                                                                                             
-231017 60234.00 P  0.284463 0.011486  0.275826 0.019001  P 0.0510719 0.0141127                                                                                                             
-231018 60235.00 P  0.283119 0.011524  0.273710 0.019080  P 0.0510659 0.0141757                                                                                                             
-231019 60236.00 P  0.281740 0.011561  0.271616 0.019158  P 0.0512442 0.0142386                                                                                                             
-231020 60237.00 P  0.280326 0.011599  0.269545 0.019237  P 0.0515541 0.0143014                                                                                                             
-231021 60238.00 P  0.278878 0.011637  0.267497 0.019316  P 0.0518997 0.0143642                                                                                                             
-231022 60239.00 P  0.277396 0.011674  0.265472 0.019394  P 0.0521588 0.0144268                                                                                                             
-231023 60240.00 P  0.275881 0.011711  0.263472 0.019473  P 0.0522097 0.0144894                                                                                                             
-231024 60241.00 P  0.274332 0.011749  0.261497 0.019551  P 0.0519642 0.0145519                                                                                                             
-231025 60242.00 P  0.272752 0.011786  0.259546 0.019629  P 0.0513989 0.0146142                                                                                                             
-231026 60243.00 P  0.271139 0.011823  0.257621 0.019707  P 0.0505721 0.0146765                                                                                                             
-231027 60244.00 P  0.269495 0.011860  0.255723 0.019785  P 0.0496129 0.0147387                                                                                                             
-231028 60245.00 P  0.267820 0.011897  0.253851 0.019863  P 0.0486859 0.0148008                                                                                                             
-231029 60246.00 P  0.266115 0.011934  0.252006 0.019941  P 0.0479408 0.0148629                                                                                                             
-231030 60247.00 P  0.264379 0.011970  0.250188 0.020018  P 0.0474690 0.0149248                                                                                                             
-231031 60248.00 P  0.262615 0.012007  0.248399 0.020096  P 0.0472851 0.0149867                                                                                                             
-2311 1 60249.00 P  0.260821 0.012043  0.246637 0.020173  P 0.0473358 0.0150484                                                                                                             
-2311 2 60250.00 P  0.258999 0.012080  0.244905 0.020250  P 0.0475285 0.0151101                                                                                                             
-2311 3 60251.00 P  0.257149 0.012116  0.243202 0.020327  P 0.0477618 0.0151717                                                                                                             
-2311 4 60252.00 P  0.255272 0.012153  0.241528 0.020404  P 0.0479466 0.0152332                                                                                                             
-2311 5 60253.00 P  0.253368 0.012189  0.239885 0.020481  P 0.0480149 0.0152946                                                                                                             
-2311 6 60254.00 P  0.251439 0.012225  0.238272 0.020558  P 0.0479218 0.0153560                                                                                                             
-2311 7 60255.00 P  0.249483 0.012261  0.236690 0.020634  P 0.0476451 0.0154172                                                                                                             
-2311 8 60256.00 P  0.247503 0.012297  0.235139 0.020711  P 0.0471862 0.0154784                                                                                                             
-2311 9 60257.00 P  0.245498 0.012333  0.233619 0.020787  P 0.0465716 0.0155395                                                                                                             
-231110 60258.00 P  0.243470 0.012369  0.232132 0.020864  P 0.0458531 0.0156005                                                                                                             
-231111 60259.00 P  0.241418 0.012405  0.230677 0.020940  P 0.0451043 0.0156614                                                                                                             
-231112 60260.00 P  0.239343 0.012440  0.229254 0.021016  P 0.0444110 0.0157223                                                                                                             
-231113 60261.00 P  0.237247 0.012476  0.227864 0.021092  P 0.0438562 0.0157831                                                                                                             
-231114 60262.00 P  0.235129 0.012511  0.226508 0.021168  P 0.0435000 0.0158438                                                                                                             
-231115 60263.00 P  0.232990 0.012547  0.225185 0.021243  P 0.0433589 0.0159044                                                                                                             
-231116 60264.00 P  0.230832 0.012582  0.223896 0.021319  P 0.0433945 0.0159649                                                                                                             
-231117 60265.00 P  0.228653 0.012617  0.222641 0.021395  P 0.0435162 0.0160254                                                                                                             
-231118 60266.00 P  0.226456 0.012653  0.221421 0.021470  P 0.0436006 0.0160858                                                                                                             
-231119 60267.00 P  0.224241 0.012688  0.220235 0.021546  P 0.0435246 0.0161461                                                                                                             
-231120 60268.00 P  0.222008 0.012723  0.219085 0.021621  P 0.0432010 0.0162063                                                                                                             
-231121 60269.00 P  0.219757 0.012758  0.217969 0.021696  P 0.0426059 0.0162665                                                                                                             
-231122 60270.00 P  0.217491 0.012793  0.216889 0.021771  P 0.0417890 0.0163265                                                                                                             
-231123 60271.00 P  0.215209 0.012828  0.215845 0.021846  P 0.0408640 0.0163866                                                                                                             
-231124 60272.00 P  0.212911 0.012862  0.214837 0.021921  P 0.0399825 0.0164465                                                                                                             
-231125 60273.00 P  0.210600 0.012897  0.213865 0.021996  P 0.0392942 0.0165063                                                                                                             
-231126 60274.00 P  0.208274 0.012932  0.212929 0.022070  P 0.0389021 0.0165661                                                                                                             
-231127 60275.00 P  0.205936 0.012966  0.212030 0.022145  P 0.0388359 0.0166258                                                                                                             
-231128 60276.00 P  0.203585 0.013001  0.211167 0.022219  P 0.0390596 0.0166855                                                                                                             
-231129 60277.00 P  0.201223 0.013035  0.210341 0.022294  P 0.0395015 0.0167451                                                                                                             
-231130 60278.00 P  0.198849 0.013070  0.209553 0.022368  P 0.0400779 0.0168046                                                                                                             
-2312 1 60279.00 P  0.196465 0.013104  0.208801 0.022442  P 0.0406978 0.0168640                                                                                                             
-2312 2 60280.00 P  0.194071 0.013138  0.208087 0.022516  P 0.0412682 0.0169233                                                                                                             
-2312 3 60281.00 P  0.191668 0.013172  0.207410 0.022590  P 0.0417085 0.0169826                                                                                                             
-2312 4 60282.00 P  0.189257 0.013206  0.206771 0.022664  P 0.0419631 0.0170419                                                                                                             
-2312 5 60283.00 P  0.186838 0.013240  0.206170 0.022738  P 0.0420175 0.0171010                                                                                                             
-2312 6 60284.00 P  0.184412 0.013274  0.205606 0.022811  P 0.0419412 0.0171601                                                                                                             
-2312 7 60285.00 P  0.181980 0.013308  0.205081 0.022885  P 0.0418369 0.0172191                                                                                                             
-2312 8 60286.00 P  0.179542 0.013342  0.204593 0.022959  P 0.0416830 0.0172780                                                                                                             
-2312 9 60287.00 P  0.177099 0.013376  0.204143 0.023032  P 0.0415537 0.0173369                                                                                                             
-231210 60288.00 P  0.174652 0.013410  0.203731 0.023105  P 0.0415743 0.0173957                                                                                                             
-231211 60289.00 P  0.172201 0.013443  0.203358 0.023179  P 0.0417571 0.0174545                                                                                                             
-231212 60290.00 P  0.169747 0.013477  0.203022 0.023252  P 0.0422176 0.0175131                                                                                                             
-231213 60291.00 P  0.167291 0.013510  0.202725 0.023325  P 0.0429097 0.0175718                                                                                                             
-231214 60292.00 P  0.164834 0.013544  0.202466 0.023398  P 0.0436917 0.0176303                                                                                                             
-231215 60293.00 P  0.162375 0.013577  0.202245 0.023471  P 0.0444560 0.0176888                                                                                                             
-231216 60294.00 P  0.159917 0.013611  0.202063 0.023543  P 0.0450289 0.0177472                                                                                                             
-231217 60295.00 P  0.157459 0.013644  0.201918 0.023616  P 0.0453556 0.0178055                                                                                                             
-231218 60296.00 P  0.155002 0.013677  0.201812 0.023689  P 0.0454324 0.0178638                                                                                                             
-231219 60297.00 P  0.152546 0.013710  0.201743 0.023761  P 0.0451616 0.0179220                                                                                                             
-231220 60298.00 P  0.150094 0.013743  0.201713 0.023834  P 0.0446772 0.0179802                                                                                                             
-231221 60299.00 P  0.147644 0.013776  0.201721 0.023906  P 0.0442080 0.0180383                                                                                                             
-231222 60300.00 P  0.145199 0.013809  0.201766 0.023978  P 0.0437720 0.0180963                                                                                                             
-231223 60301.00 P  0.142758 0.013842  0.201850 0.024051  P 0.0435796 0.0181543                                                                                                             
-231224 60302.00 P  0.140322 0.013875  0.201971 0.024123  P 0.0435857 0.0182122                                                                                                             
-231225 60303.00 P  0.137892 0.013908  0.202130 0.024195  P 0.0438538 0.0182700                                                                                                             
-231226 60304.00 P  0.135468 0.013940  0.202326 0.024267  P 0.0442804 0.0183278                                                                                                             
-231227 60305.00 P  0.133052 0.013973  0.202560 0.024338  P 0.0448303 0.0183855                                                                                                             
-231228 60306.00 P  0.130643 0.014006  0.202831 0.024410  P 0.0454067 0.0184432                                                                                                             
-231229 60307.00 P  0.128243 0.014038  0.203139 0.024482  P 0.0459122 0.0185008                                                                                                             
-231230 60308.00 P  0.125853 0.014071  0.203484 0.024554  P 0.0462828 0.0185583                                                                                                             
-231231 60309.00 P  0.123472 0.014103  0.203866 0.024625  P 0.0465129 0.0186158                                                                                                             
-24 1 1 60310.00 P  0.121101 0.014136  0.204285 0.024697  P 0.0465067 0.0186732                                                                                                             
-24 1 2 60311.00 P  0.118741 0.014168  0.204740 0.024768  P 0.0463767 0.0187306                                                                                                             
-24 1 3 60312.00 P  0.116394 0.014200  0.205232 0.024839  P 0.0461709 0.0187879                                                                                                             
-24 1 4 60313.00 P  0.114058 0.014232  0.205759 0.024910  P 0.0459194 0.0188451                                                                                                             
-24 1 5 60314.00 P  0.111736 0.014265  0.206322 0.024982  P 0.0457071 0.0189023                                                                                                             
-24 1 6 60315.00 P  0.109427 0.014297  0.206921 0.025053  P 0.0456175 0.0189594                                                                                                             
-24 1 7 60316.00 P  0.107132 0.014329  0.207556 0.025124  P 0.0457165 0.0190165                                                                                                             
-24 1 8 60317.00 P  0.104852 0.014361  0.208225 0.025195  P 0.0460445 0.0190735                                                                                                             
-24 1 9 60318.00 P  0.102588 0.014393  0.208929 0.025265  P 0.0466387 0.0191305                                                                                                             
-24 110 60319.00 P  0.100340 0.014425  0.209669 0.025336  P 0.0473939 0.0191874                                                                                                             
-24 111 60320.00 P  0.098108 0.014456  0.210442 0.025407  P 0.0482096 0.0192442                                                                                                             
-24 112 60321.00 P  0.095893 0.014488  0.211250 0.025477  P 0.0489080 0.0193010                                                                                                             
-24 113 60322.00 P  0.093697 0.014520  0.212091 0.025548  P 0.0493736 0.0193577                                                                                                             
-24 114 60323.00 P  0.091518 0.014552  0.212966 0.025618  P 0.0494698 0.0194144                                                                                                             
-24 115 60324.00 P  0.089359 0.014583  0.213874 0.025689  P 0.0492097 0.0194710                                                                                                             
-24 116 60325.00 P  0.087219 0.014615  0.214815 0.025759  P 0.0488662 0.0195276                                                                                                             
-24 117 60326.00 P  0.085099 0.014646  0.215789 0.025829  P 0.0485051 0.0195841                                                                                                             
-24 118 60327.00 P  0.083000 0.014678  0.216795 0.025899  P 0.0483270 0.0196405                                                                                                             
-24 119 60328.00 P  0.080923 0.014709  0.217833 0.025969  P 0.0483326 0.0196969                                                                                                             
-24 120 60329.00 P  0.078866 0.014741  0.218902 0.026039  P 0.0486390 0.0197532                                                                                                             
-24 121 60330.00 P  0.076833 0.014772  0.220003 0.026109  P 0.0491327 0.0198095                                                                                                             
-24 122 60331.00 P  0.074822 0.014803  0.221135 0.026179  P 0.0498234 0.0198658                                                                                                             
-24 123 60332.00 P  0.072834 0.014835  0.222297 0.026249  P 0.0505894 0.0199219                                                                                                             
-24 124 60333.00 P  0.070870 0.014866  0.223489 0.026319  P 0.0513096 0.0199781                                                                                                             
-24 125 60334.00 P  0.068931 0.014897  0.224711 0.026388  P 0.0518992 0.0200341                                                                                                             
-24 126 60335.00 P  0.067016 0.014928  0.225962 0.026458  P 0.0523067 0.0200902                                                                                                             
-24 127 60336.00 P  0.065127 0.014959  0.227242 0.026527  P 0.0524787 0.0201461                                                                                                             
-24 128 60337.00 P  0.063264 0.014990  0.228551 0.026597  P 0.0524781 0.0202021                                                                                                             
-24 129 60338.00 P  0.061426 0.015021  0.229888 0.026666  P 0.0523301 0.0202579                                                                                                             
-24 130 60339.00 P  0.059616 0.015052  0.231253 0.026735  P 0.0520729 0.0203137                                                                                                             
-24 131 60340.00 P  0.057833 0.015083  0.232644 0.026805  P 0.0517763 0.0203695                                                                                                             
-24 2 1 60341.00 P  0.056078 0.015113  0.234063 0.026874  P 0.0514996 0.0204252                                                                                                             
-24 2 2 60342.00 P  0.054350 0.015144  0.235508 0.026943  P 0.0512642 0.0204809                                                                                                             
-24 2 3 60343.00 P  0.052652 0.015175  0.236979 0.027012  P 0.0511788 0.0205365                                                                                                             
-24 2 4 60344.00 P  0.050982 0.015205  0.238475 0.027081  P 0.0512445 0.0205920                                                                                                             
-24 2 5 60345.00 P  0.049341 0.015236  0.239997 0.027150  P 0.0514714 0.0206475                                                                                                             
-24 2 6 60346.00 P  0.047731 0.015267  0.241543 0.027218  P 0.0518228 0.0207030                                                                                                             
-24 2 7 60347.00 P  0.046151 0.015297  0.243113 0.027287  P 0.0522952 0.0207584                                                                                                             
-24 2 8 60348.00 P  0.044601 0.015328  0.244706 0.027356  P 0.0526760 0.0208138                                                                                                             
-24 2 9 60349.00 P  0.043082 0.015358  0.246323 0.027424  P 0.0528869 0.0208691                                                                                                             
-24 210 60350.00 P  0.041595 0.015388  0.247962 0.027493  P 0.0527814 0.0209243                                                                                                             
-24 211 60351.00 P  0.040139 0.015419  0.249624 0.027561  P 0.0522585 0.0209795                                                                                                             
-24 212 60352.00 P  0.038715 0.015449  0.251307 0.027630  P 0.0514242 0.0210347                                                                                                             
-24 213 60353.00 P  0.037324 0.015479  0.253011 0.027698  P 0.0505031 0.0210898                                                                                                             
-24 214 60354.00 P  0.035965 0.015509  0.254736 0.027766  P 0.0497110 0.0211449                                                                                                             
-24 215 60355.00 P  0.034640 0.015540  0.256480 0.027834  P 0.0491538 0.0211999                                                                                                             
-24 216 60356.00 P  0.033348 0.015570  0.258245 0.027903  P 0.0489245 0.0212548                                                                                                             
-24 217 60357.00 P  0.032090 0.015600  0.260028 0.027971  P 0.0489961 0.0213098                                                                                                             
-24 218 60358.00 P  0.030865 0.015630  0.261830 0.028039  P 0.0493041 0.0213646                                                                                                             
-24 219 60359.00 P  0.029675 0.015660  0.263649 0.028107  P 0.0498066 0.0214195                                                                                                             
-24 220 60360.00 P  0.028519 0.015690  0.265486 0.028175  P 0.0503365 0.0214742                                                                                                             
-24 221 60361.00 P  0.027399 0.015720  0.267340 0.028242  P 0.0508384 0.0215290                                                                                                             
-24 222 60362.00 P  0.026313 0.015749  0.269210 0.028310  P 0.0512073 0.0215837                                                                                                             
-24 223 60363.00 P  0.025262 0.015779  0.271096 0.028378  P 0.0514034 0.0216383                                                                                                             
-24 224 60364.00 P  0.024247 0.015809  0.272997 0.028445  P 0.0513907 0.0216929                                                                                                             
-24 225 60365.00 P  0.023268 0.015839  0.274913 0.028513  P 0.0512575 0.0217474                                                                                                             
-24 226 60366.00 P  0.022325 0.015868  0.276843 0.028580  P 0.0508828 0.0218019                                                                                                             
-24 227 60367.00 P  0.021418 0.015898  0.278786 0.028648  P 0.0504285 0.0218564                                                                                                             
-24 228 60368.00 P  0.020547 0.015928  0.280743 0.028715  P 0.0499940 0.0219108                                                                                                             
-24 229 60369.00 P  0.019713 0.015957  0.282711 0.028783  P 0.0496001 0.0219652                                                                                                             
-24 3 1 60370.00 P  0.018915 0.015987  0.284692 0.028850  P 0.0492945 0.0220195                                                                                                             
-24 3 2 60371.00 P  0.018155 0.016016  0.286683 0.028917  P 0.0491032 0.0220738                                                                                                             
-24 3 3 60372.00 P  0.017431 0.016046  0.288685 0.028984  P 0.0491006 0.0221280                                                                                                             
-24 3 4 60373.00 P  0.016745 0.016075  0.290698 0.029051  P 0.0492206 0.0221822                                                                                                             
-24 3 5 60374.00 P  0.016095 0.016104  0.292720 0.029118  P 0.0494549 0.0222363                                                                                                             
-24 3 6 60375.00 P  0.015483 0.016134  0.294750 0.029185  P 0.0497490 0.0222904                                                                                                             
-24 3 7 60376.00 P  0.014909 0.016163  0.296789 0.029252  P 0.0499638 0.0223444                                                                                                             
-24 3 8 60377.00 P  0.014372 0.016192  0.298836 0.029319  P 0.0498662 0.0223985                                                                                                             
-24 3 9 60378.00 P  0.013873 0.016221  0.300890 0.029386  P 0.0494344 0.0224524                                                                                                             
-24 310 60379.00 P  0.013412 0.016250  0.302950 0.029452  P 0.0486708 0.0225063                                                                                                             
-24 311 60380.00 P  0.012989 0.016280  0.305016 0.029519  P 0.0476832 0.0225602                                                                                                             
-24 312 60381.00 P  0.012603 0.016309  0.307088 0.029586  P 0.0466673 0.0226140                                                                                                             
-24 313 60382.00 P  0.012255 0.016338  0.309164 0.029652  P 0.0458657 0.0226678                                                                                                             
-24 314 60383.00 P  0.011945 0.016367  0.311245 0.029719  P 0.0453529 0.0227216                                                                                                             
-24 315 60384.00 P  0.011674 0.016396  0.313329 0.029785  P 0.0451817 0.0227753                                                                                                             
-24 316 60385.00 P  0.011440 0.016425  0.315416 0.029851  P 0.0453401 0.0228290                                                                                                             
-24 317 60386.00 P  0.011244 0.016453  0.317505 0.029918  P 0.0456535 0.0228826                                                                                                             
-24 318 60387.00 P  0.011086 0.016482  0.319597 0.029984  P 0.0460693 0.0229362                                                                                                             
-24 319 60388.00 P  0.010966 0.016511  0.321689 0.030050  P 0.0464914 0.0229897                                                                                                             
-24 320 60389.00 P  0.010884 0.016540  0.323782 0.030116  P 0.0468438 0.0230432                                                                                                             
-24 321 60390.00 P  0.010840 0.016569  0.325876 0.030182  P 0.0470460 0.0230966                                                                                                             
-24 322 60391.00 P  0.010833 0.016597  0.327968 0.030248  P 0.0470908 0.0231500                                                                                                             
-24 323 60392.00 P  0.010864 0.016626  0.330060 0.030314  P 0.0469821 0.0232034                                                                                                             
-24 324 60393.00 P  0.010933 0.016654  0.332150 0.030380  P 0.0466940 0.0232567                                                                                                             
-24 325 60394.00 P  0.011040 0.016683  0.334237 0.030446  P 0.0462492 0.0233100                                                                                                             
-24 326 60395.00 P  0.011184 0.016712  0.336322 0.030512  P 0.0457381 0.0233633                                                                                                             
-24 327 60396.00 P  0.011365 0.016740  0.338403 0.030578  P 0.0452591 0.0234165                                                                                                             
-24 328 60397.00 P  0.011584 0.016769  0.340480 0.030643  P 0.0449109 0.0234697                                                                                                             
-24 329 60398.00 P  0.011839 0.016797  0.342552 0.030709  P 0.0447445 0.0235228                                                                                                             
-24 330 60399.00 P  0.012132 0.016825  0.344619 0.030775  P 0.0447647 0.0235759                                                                                                             
-24 331 60400.00 P  0.012461 0.016854  0.346681 0.030840  P 0.0449747 0.0236289                                                                                                             
-24 4 1 60401.00 P  0.012828 0.016882  0.348736 0.030906  P 0.0452442 0.0236819                                                                                                             
-24 4 2 60402.00 P  0.013230 0.016910  0.350784 0.030971  P 0.0455560 0.0237349                                                                                                             
-24 4 3 60403.00 P  0.013669 0.016939  0.352825 0.031036  P 0.0457845 0.0237878                                                                                                             
-24 4 4 60404.00 P  0.014144 0.016967  0.354857 0.031102  P 0.0457536 0.0238407                                                                                                             
-24 4 5 60405.00 P  0.014655 0.016995  0.356881 0.031167  P 0.0454107 0.0238935                                                                                                             
-24 4 6 60406.00 P  0.015202 0.017023  0.358896 0.031232  P 0.0447695 0.0239463                                                                                                             
-24 4 7 60407.00 P  0.015784 0.017051  0.360902 0.031297  P 0.0438145 0.0239991                                                                                                             
-24 4 8 60408.00 P  0.016401 0.017079  0.362897 0.031362  P 0.0427448 0.0240518                                                                                                             
-24 4 9 60409.00 P  0.017054 0.017107  0.364881 0.031428  P 0.0417120 0.0241045                                                                                                             
-24 410 60410.00 P  0.017741 0.017135  0.366854 0.031493  P 0.0408498 0.0241572                                                                                                             
-24 411 60411.00 P  0.018463 0.017163  0.368815 0.031557  P 0.0402576 0.0242098                                                                                                             
-24 412 60412.00 P  0.019219 0.017191  0.370763 0.031622  P 0.0399386 0.0242624                                                                                                             
-24 413 60413.00 P  0.020009 0.017219  0.372699 0.031687  P 0.0398489 0.0243149                                                                                                             
-24 414 60414.00 P  0.020832 0.017247  0.374621 0.031752  P 0.0399089 0.0243674                                                                                                             
-24 415 60415.00 P  0.021690 0.017275  0.376529 0.031817  P 0.0399873 0.0244199                                                                                                             
-24 416 60416.00 P  0.022580 0.017303  0.378423 0.031881  P 0.0400005 0.0244723                                                                                                             
-24 417 60417.00 P  0.023503 0.017330  0.380302 0.031946  P 0.0398683 0.0245247                                                                                                             
-24 418 60418.00 P  0.024458 0.017358  0.382165 0.032011  P 0.0395609 0.0245770                                                                                                             
-24 419 60419.00 P  0.025445 0.017386  0.384013 0.032075  P 0.0390531 0.0246293                                                                                                             
-24 420 60420.00 P  0.026465 0.017413  0.385844 0.032140  P 0.0383783 0.0246816                                                                                                             
-24 421 60421.00 P  0.027515 0.017441  0.387658 0.032204  P 0.0375410 0.0247338                                                                                                             
-24 422 60422.00 P  0.028597 0.017469  0.389454 0.032268  P 0.0366522 0.0247860                                                                                                             
-24 423 60423.00 P  0.029710 0.017496  0.391233 0.032333  P 0.0358383 0.0248382                                                                                                             
-24 424 60424.00 P  0.030852 0.017524  0.392993 0.032397  P 0.0352065 0.0248903                                                                                                             
-24 425 60425.00 P  0.032025 0.017551  0.394734 0.032461  P 0.0348191 0.0249424                                                                                                             
-24 426 60426.00 P  0.033228 0.017579  0.396456 0.032525  P 0.0346363 0.0249945                                                                                                             
-24 427 60427.00 P  0.034459 0.017606  0.398159 0.032590  P 0.0346869 0.0250465                                                                                                             
-24 428 60428.00 P  0.035719 0.017634  0.399841 0.032654  P 0.0348689 0.0250985                                                                                                             
-24 429 60429.00 P  0.037008 0.017661  0.401502 0.032718  P 0.0351870 0.0251504                                                                                                             
-24 430 60430.00 P  0.038325 0.017688  0.403143 0.032782  P 0.0355292 0.0252023                                                                                                             
-24 5 1 60431.00 P  0.039669 0.017716  0.404762 0.032846  P 0.0357579 0.0252542                                                                                                             
-24 5 2 60432.00 P  0.041040 0.017743  0.406359 0.032910  P 0.0357293 0.0253060                                                                                                             
-24 5 3 60433.00 P  0.042437 0.017770  0.407934 0.032973  P 0.0353708 0.0253578                                                                                                             
-24 5 4 60434.00 P  0.043861 0.017797  0.409486 0.033037  P 0.0347628 0.0254096                                                                                                             
-24 5 5 60435.00                                                                                                                                                                            
-24 5 6 60436.00                                                                                                                                                                            
-24 5 7 60437.00                                                                                                                                                                            
-24 5 8 60438.00                                                                                                                                                                            
-24 5 9 60439.00                                                                                                                                                                            
-24 510 60440.00                                                                                                                                                                            
-24 511 60441.00                                                                                                                                                                            
-24 512 60442.00                                                                                                                                                                            
-24 513 60443.00                                                                                                                                                                            
-24 514 60444.00                                                                                                                                                                            
-24 515 60445.00                                                                                                                                                                            
-24 516 60446.00                                                                                                                                                                            
-24 517 60447.00                                                                                                                                                                            
-24 518 60448.00                                                                                                                                                                            
-24 519 60449.00                                                                                                                                                                            
-24 520 60450.00                                                                                                                                                                            
-24 521 60451.00                                                                                                                                                                            
-24 522 60452.00                                                                                                                                                                            
-24 523 60453.00                                                                                                                                                                            
-24 524 60454.00                                                                                                                                                                            
-24 525 60455.00                                                                                                                                                                            
-24 526 60456.00                                                                                                                                                                            
-24 527 60457.00                                                                                                                                                                            
-24 528 60458.00                                                                                                                                                                            
-24 529 60459.00                                                                                                                                                                            
-24 530 60460.00                                                                                                                                                                            
-24 531 60461.00                                                                                                                                                                            
-24 6 1 60462.00                                                                                                                                                                            
+22 419 59688.00 I  0.066169 0.000023  0.460809 0.000016  I-0.0988174 0.0000075  0.2225 0.0042  I  -106.782    0.806    -8.999    0.015  0.066192  0.460869 -0.0988272  -106.773    -9.104  
+22 420 59689.00 I  0.068331 0.000027  0.462008 0.000026  I-0.0989000 0.0000041 -0.0756 0.0043  I  -106.912    0.792    -9.262    0.084  0.068329  0.461999 -0.0988949  -106.960    -9.291  
+22 421 59690.00 I  0.070493 0.000026  0.463048 0.000026  I-0.0986843 0.0000043 -0.3196 0.0032  I  -106.641    0.792    -9.418    0.084  0.070468  0.463064 -0.0987060  -106.695    -9.434  
+22 422 59691.00 I  0.072758 0.000023  0.464119 0.000027  I-0.0983194 0.0000049 -0.3878 0.0033  I  -106.179    0.792    -9.477    0.084  0.072707  0.464098 -0.0983386  -106.211    -9.508  
+22 423 59692.00 I  0.075224 0.000022  0.465083 0.000026  I-0.0979269 0.0000049 -0.4013 0.0037  I  -105.765    0.792    -9.509    0.084  0.075204  0.465058 -0.0979051  -105.797    -9.527  
+22 424 59693.00 I  0.077856 0.000017  0.466283 0.000040  I-0.0975412 0.0000056 -0.3417 0.0037  I  -105.469    0.768    -9.550    0.101  0.077859  0.466247 -0.0975194  -105.498    -9.555  
+22 425 59694.00 I  0.080485 0.000015  0.467920 0.000040  I-0.0972766 0.0000056 -0.1828 0.0055  I  -105.250    0.768    -9.589    0.101  0.080557  0.467896 -0.0972632  -105.265    -9.590  
+22 426 59695.00 I  0.082817 0.000012  0.469862 0.000035  I-0.0971782 0.0000095 -0.0162 0.0040  I  -105.105    0.734    -9.598    0.070  0.082859  0.469891 -0.0971847  -105.109    -9.593  
+22 427 59696.00 I  0.084841 0.000019  0.471453 0.000035  I-0.0972281 0.0000058  0.1021 0.0055  I  -105.009    0.749    -9.695    0.183  0.084908  0.471486 -0.0972203  -105.096    -9.548  
+22 428 59697.00 I  0.086493 0.000020  0.472743 0.000035  I-0.0973574 0.0000055  0.1456 0.0043  I  -105.194    0.749    -9.487    0.183  0.086518  0.472819 -0.0973522  -105.258    -9.407  
+22 429 59698.00 I  0.087931 0.000020  0.473543 0.000036  I-0.0974953 0.0000063  0.1172 0.0041  I  -105.450    0.749    -9.213    0.183  0.087895  0.473595 -0.0974914  -105.480    -9.203  
+22 430 59699.00 I  0.089677 0.000019  0.474074 0.000012  I-0.0975714 0.0000060  0.0277 0.0043  I  -105.613    0.749    -8.997    0.183  0.089653  0.474104 -0.0975559  -105.614    -9.011  
+22 5 1 59700.00 I  0.091698 0.000020  0.474621 0.000014  I-0.0975428 0.0000060 -0.0854 0.0043  I  -105.650    0.749    -8.968    0.183  0.091728  0.474632 -0.0975257  -105.627    -8.987  
+22 5 2 59701.00 I  0.093634 0.000024  0.475316 0.000020  I-0.0974058 0.0000062 -0.1830 0.0046  I  -105.655    0.749    -9.133    0.116  0.093634  0.475311 -0.0974187  -105.619    -9.154  
+22 5 3 59702.00 I  0.095564 0.000018  0.476114 0.000019  I-0.0971898 0.0000071 -0.2415 0.0044  I  -105.768    0.749    -9.322    0.030  0.095563  0.476140 -0.0972185  -105.662    -9.372  
+22 5 4 59703.00 I  0.097693 0.000023  0.476934 0.000028  I-0.0969120 0.0000062 -0.3323 0.0047  I  -105.769    0.784    -9.473    0.037  0.097691  0.476906 -0.0969126  -105.734    -9.493  
+22 5 5 59704.00 I  0.099820 0.000023  0.477875 0.000028  I-0.0965122 0.0000061 -0.4620 0.0044  I  -105.743    0.784    -9.518    0.037  0.099882  0.477903 -0.0964992  -105.770    -9.526  
+22 5 6 59705.00 I  0.101675 0.000024  0.478832 0.000028  I-0.0960243 0.0000062 -0.4827 0.0043  I  -105.687    0.784    -9.589    0.037  0.101687  0.478833 -0.0960256  -105.754    -9.581  
+22 5 7 59706.00 I  0.103386 0.000024  0.479498 0.000027  I-0.0955680 0.0000062 -0.4398 0.0040  I  -105.566    0.784    -9.779    0.037  0.103404  0.479538 -0.0955546  -105.646    -9.779  
+22 5 8 59707.00 I  0.105106 0.000024  0.480063 0.000027  I-0.0951539 0.0000051 -0.3692 0.0040  I  -105.288    0.796   -10.022    0.102  0.105117  0.480078 -0.0951550  -105.347   -10.030  
+22 5 9 59708.00 I  0.106695 0.000024  0.480513 0.000027  I-0.0948662 0.0000052 -0.1889 0.0036  I  -104.882    0.796   -10.188    0.102  0.106699  0.480537 -0.0949242  -104.904   -10.197  
+22 510 59709.00 I  0.108521 0.000019  0.480972 0.000018  I-0.0947986 0.0000052  0.0589 0.0032  I  -104.620    0.772   -10.247    0.139  0.108427  0.480933 -0.0948334  -104.607   -10.261  
+22 511 59710.00 I  0.110913 0.000019  0.481771 0.000026  I-0.0949978 0.0000037  0.3482 0.0033  I  -104.755    0.770   -10.274    0.158  0.110941  0.481776 -0.0950144  -104.732   -10.281  
+22 512 59711.00 I  0.113494 0.000018  0.482666 0.000026  I-0.0954644 0.0000041  0.5456 0.0031  I  -105.181    0.770   -10.282    0.158  0.113474  0.482707 -0.0954543  -105.174   -10.290  
+22 513 59712.00 I  0.116069 0.000018  0.483382 0.000026  I-0.0960614 0.0000049  0.6602 0.0037  I  -105.540    0.770   -10.144    0.158  0.116107  0.483379 -0.0960629  -105.566   -10.162  
+22 514 59713.00 I  0.118511 0.000014  0.483943 0.000022  I-0.0967523 0.0000061  0.6771 0.0039  I  -105.727    0.768    -9.783    0.175  0.118527  0.483975 -0.0967431  -105.773    -9.799  
+22 515 59714.00 I  0.120714 0.000021  0.484477 0.000032  I-0.0973746 0.0000061  0.5708 0.0044  I  -106.021    0.850    -9.387    0.156  0.120799  0.484444 -0.0973670  -106.086    -9.399  
+22 516 59715.00 I  0.122296 0.000022  0.485288 0.000031  I-0.0978782 0.0000063  0.4175 0.0059  I  -106.570    0.850    -9.269    0.156  0.122385  0.485333 -0.0978659  -106.653    -9.281  
+22 517 59716.00 I  0.123269 0.000023  0.485820 0.000026  I-0.0981864 0.0000101  0.1947 0.0061  I  -107.056    0.996    -9.503    0.128  0.123240  0.485912 -0.0981728  -107.146    -9.513  
+22 518 59717.00 I  0.124657 0.000028  0.485658 0.000040  I-0.0982697 0.0000105 -0.0217 0.0073  I  -107.060    1.005    -9.843    0.134  0.124614  0.485666 -0.0982338  -107.148    -9.846  
+22 519 59718.00 I  0.126490 0.000027  0.485546 0.000040  I-0.0981577 0.0000105 -0.1941 0.0075  I  -106.590    1.005   -10.040    0.134  0.126492  0.485563 -0.0980742  -106.655   -10.034  
+22 520 59719.00 I  0.128445 0.000027  0.485604 0.000040  I-0.0979282 0.0000107 -0.2265 0.0081  I  -106.038    1.005   -10.084    0.134  0.128370  0.485536 -0.0979421  -106.062   -10.068  
+22 521 59720.00 I  0.130661 0.000022  0.486032 0.000033  I-0.0977464 0.0000123 -0.1338 0.0070  I  -105.740    1.028   -10.086    0.145  0.130677  0.486020 -0.0977739  -105.765   -10.071  
+22 522 59721.00 I  0.132973 0.000026  0.486744 0.000042  I-0.0976766 0.0000089  0.0069 0.0076  I  -105.718    0.874   -10.069    0.090  0.132949  0.486774 -0.0977075  -105.758   -10.059  
+22 523 59722.00 I  0.135353 0.000027  0.487369 0.000041  I-0.0977620 0.0000088  0.1529 0.0060  I  -105.790    0.874    -9.981    0.090  0.135359  0.487350 -0.0977582  -105.848    -9.982  
+22 524 59723.00 I  0.137677 0.000021  0.488142 0.000028  I-0.0979664 0.0000080  0.2508 0.0055  I  -105.807    0.828    -9.816    0.055  0.137703  0.488205 -0.0979698  -105.891    -9.829  
+22 525 59724.00 I  0.139652 0.000023  0.488534 0.000038  I-0.0982380 0.0000066  0.2718 0.0052  I  -105.793    0.868    -9.608    0.057  0.139642  0.488593 -0.0982642  -105.852    -9.614  
+22 526 59725.00 I  0.141660 0.000022  0.488494 0.000037  I-0.0984839 0.0000065  0.2145 0.0046  I  -105.887    0.868    -9.368    0.057  0.141637  0.488529 -0.0985094  -105.918    -9.361  
+22 527 59726.00 I  0.143579 0.000023  0.488465 0.000037  I-0.0986409 0.0000065  0.0790 0.0046  I  -106.147    0.868    -9.110    0.057  0.143638  0.488445 -0.0986407  -106.153    -9.084  
+22 528 59727.00 I  0.145156 0.000017  0.488364 0.000028  I-0.0986084 0.0000066 -0.1571 0.0047  I  -106.453    0.896    -8.928    0.059  0.145102  0.488400 -0.0986068  -106.467    -8.914  
+22 529 59728.00 I  0.146684 0.000016  0.488245 0.000029  I-0.0983139 0.0000067 -0.4317 0.0045  I  -106.638    0.896    -8.971    0.059  0.146706  0.488268 -0.0983314  -106.669    -8.976  
+22 530 59729.00 I  0.148142 0.000026  0.487967 0.000040  I-0.0977447 0.0000060 -0.7073 0.0048  I  -106.661    0.852    -9.278    0.044  0.148067  0.488086 -0.0977877  -106.716    -9.292  
+22 531 59730.00 I  0.149845 0.000024  0.487088 0.000030  I-0.0969122 0.0000070 -0.9442 0.0042  I  -106.606    0.791    -9.683    0.022  0.149795  0.487092 -0.0969563  -106.700    -9.703  
+22 6 1 59731.00 I  0.152003 0.000030  0.486176 0.000040  I-0.0958955 0.0000059 -1.0635 0.0047  I  -106.570    0.998    -9.951    0.041  0.151943  0.486170 -0.0959109  -106.731    -9.971  
+22 6 2 59732.00 I  0.154335 0.000030  0.485423 0.000040  I-0.0947983 0.0000062 -1.1436 0.0045  I  -106.608    0.998   -10.005    0.041  0.154357  0.485426 -0.0947757  -106.670   -10.005  
+22 6 3 59733.00 I  0.156609 0.000030  0.484774 0.000040  I-0.0936396 0.0000068 -1.1300 0.0046  I  -106.745    0.998    -9.979    0.041  0.156589  0.484781 -0.0936356  -106.660    -9.955  
+22 6 4 59734.00 I  0.158876 0.000030  0.484145 0.000039  I-0.0925763 0.0000067 -1.0026 0.0051  I  -106.915    0.998   -10.015    0.041  0.158889  0.484149 -0.0925602  -106.851    -9.984  
+22 6 5 59735.00 I  0.161158 0.000021  0.483621 0.000028  I-0.0916251 0.0000077 -0.9033 0.0047  I  -106.933    1.250   -10.088    0.057  0.161161  0.483622 -0.0916220  -106.921   -10.058  
+22 6 6 59736.00 I  0.163475 0.000027  0.483151 0.000034  I-0.0907856 0.0000065 -0.7563 0.0053  I  -106.704    1.009   -10.069    0.084  0.163382  0.483150 -0.0908246  -106.715   -10.044  
+22 6 7 59737.00 I  0.166257 0.000021  0.482841 0.000020  I-0.0901365 0.0000073 -0.5372 0.0046  I  -106.450    0.875    -9.939    0.099  0.166198  0.482812 -0.0901686  -106.474    -9.925  
+22 6 8 59738.00 I  0.169366 0.000026  0.482835 0.000040  I-0.0896850 0.0000065 -0.3968 0.0049  I  -106.534    0.903    -9.832    0.086  0.169346  0.482843 -0.0896819  -106.581    -9.834  
+22 6 9 59739.00 I  0.172337 0.000026  0.482859 0.000041  I-0.0893321 0.0000066 -0.2888 0.0046  I  -107.025    0.903    -9.819    0.086  0.172338  0.482895 -0.0893344  -107.056    -9.817  
+22 610 59740.00 I  0.175171 0.000026  0.482888 0.000041  I-0.0890948 0.0000066 -0.2185 0.0047  I  -107.638    0.903    -9.757    0.086  0.175150  0.482907 -0.0890843  -107.652    -9.745  
+22 611 59741.00 I  0.177826 0.000026  0.482630 0.000041  I-0.0888495 0.0000068 -0.2850 0.0044  I  -108.183    0.903    -9.475    0.086  0.177834  0.482720 -0.0888551  -108.201    -9.465  
+22 612 59742.00 I  0.180320 0.000022  0.481995 0.000044  I-0.0884938 0.0000057 -0.4446 0.0044  I  -108.787    0.773    -9.089    0.090  0.180290  0.482016 -0.0885165  -108.809    -9.083  
+22 613 59743.00 I  0.182802 0.000022  0.481217 0.000044  I-0.0879285 0.0000056 -0.6998 0.0041  I  -109.509    0.773    -8.953    0.090  0.182826  0.481258 -0.0879480  -109.531    -8.942  
+22 614 59744.00 I  0.185077 0.000015  0.480375 0.000026  I-0.0870865 0.0000059 -0.9782 0.0039  I  -109.999    0.690    -9.207    0.105  0.185100  0.480403 -0.0870940  -110.036    -9.188  
+22 615 59745.00 I  0.187071 0.000035  0.479276 0.000036  I-0.0859924 0.0000055 -1.1956 0.0040  I  -109.879    0.704    -9.596    0.140  0.187052  0.479331 -0.0859830  -109.873    -9.588  
+22 616 59746.00 I  0.189198 0.000035  0.478011 0.000036  I-0.0847403 0.0000055 -1.2779 0.0039  I  -109.275    0.704    -9.827    0.140  0.189149  0.478024 -0.0847332  -109.222    -9.837  
+22 617 59747.00 I  0.191615 0.000034  0.476726 0.000036  I-0.0834987 0.0000056 -1.1739 0.0049  I  -108.682    0.704    -9.900    0.140  0.191602  0.476728 -0.0834949  -108.594    -9.934  
+22 618 59748.00 I  0.194038 0.000033  0.475538 0.000027  I-0.0824295 0.0000081 -0.9590 0.0054  I  -108.441    0.837    -9.953    0.222  0.194019  0.475550 -0.0824189  -108.365    -9.983  
+22 619 59749.00 I  0.196593 0.000033  0.474522 0.000027  I-0.0815734 0.0000092 -0.7660 0.0051  I  -108.557    0.837    -9.955    0.222  0.196541  0.474534 -0.0815575  -108.509    -9.976  
+22 620 59750.00 I  0.199463 0.000034  0.473569 0.000034  I-0.0808815 0.0000062 -0.6210 0.0055  I  -108.866    0.811    -9.778    0.159  0.199454  0.473574 -0.0808812  -108.836    -9.796  
+22 621 59751.00 I  0.202394 0.000012  0.472814 0.000023  I-0.0803065 0.0000059 -0.5505 0.0039  I  -109.178    0.808    -9.449    0.137  0.202403  0.472799 -0.0803109  -109.153    -9.467  
+22 622 59752.00 I  0.205097 0.000015  0.472255 0.000027  I-0.0797506 0.0000047 -0.5695 0.0038  I  -109.380    0.719    -9.158    0.135  0.205128  0.472282 -0.0797589  -109.347    -9.174  
+22 623 59753.00 I  0.207617 0.000016  0.471607 0.000028  I-0.0791244 0.0000049 -0.7179 0.0034  I  -109.530    0.719    -9.018    0.135  0.207619  0.471645 -0.0791011  -109.587    -9.025  
+22 624 59754.00 I  0.210143 0.000016  0.470771 0.000028  I-0.0783038 0.0000050 -0.8994 0.0035  I  -109.778    0.719    -8.977    0.135  0.210148  0.470821 -0.0782976  -109.961    -8.971  
+22 625 59755.00 I  0.212734 0.000017  0.469692 0.000028  I-0.0773338 0.0000050 -1.0563 0.0034  I  -110.138    0.719    -8.983    0.135  0.212693  0.469719 -0.0773260  -110.305    -8.982  
+22 626 59756.00 I  0.215401 0.000023  0.468441 0.000029  I-0.0761717 0.0000047 -1.2717 0.0035  I  -110.451    0.782    -9.101    0.139  0.215376  0.468485 -0.0761726  -110.571    -9.112  
+22 627 59757.00 I  0.218222 0.000023  0.467029 0.000028  I-0.0748150 0.0000048 -1.4135 0.0038  I  -110.567    0.782    -9.404    0.139  0.218164  0.467038 -0.0748406  -110.659    -9.428  
+22 628 59758.00 I  0.221337 0.000021  0.465597 0.000025  I-0.0733612 0.0000059 -1.5060 0.0040  I  -110.511    0.910    -9.793    0.144  0.221330  0.465623 -0.0733645  -110.576    -9.834  
+22 629 59759.00 I  0.224404 0.000022  0.464144 0.000038  I-0.0718062 0.0000065 -1.5888 0.0046  I  -110.442    0.947   -10.029    0.126  0.224443  0.464165 -0.0718011  -110.473   -10.052  
+22 630 59760.00 I  0.227228 0.000022  0.462598 0.000037  I-0.0702106 0.0000070 -1.5905 0.0048  I  -110.497    0.947    -9.980    0.126  0.227220  0.462671 -0.0702118  -110.474    -9.975  
+22 7 1 59761.00 I  0.230018 0.000022  0.460847 0.000037  I-0.0686600 0.0000072 -1.4877 0.0066  I  -110.702    0.947    -9.762    0.126  0.230002  0.460818 -0.0686663  -110.599    -9.722  
+22 7 2 59762.00 I  0.232934 0.000011  0.459215 0.000031  I-0.0672413 0.0000112 -1.3666 0.0058  I  -110.971    1.012    -9.589    0.082  0.232881  0.459225 -0.0672447  -110.959    -9.582  
+22 7 3 59763.00 I  0.236097 0.000015  0.457823 0.000041  I-0.0659489 0.0000092 -1.1791 0.0072  I  -111.139    0.873    -9.533    0.141  0.236109  0.457809 -0.0659625  -111.150    -9.536  
+22 7 4 59764.00 I  0.239191 0.000015  0.456540 0.000041  I-0.0649152 0.0000090 -0.8952 0.0058  I  -111.087    0.873    -9.489    0.141  0.239234  0.456579 -0.0649159  -111.121    -9.498  
+22 7 5 59765.00 I  0.241894 0.000013  0.455121 0.000035  I-0.0641419 0.0000071 -0.6611 0.0055  I  -110.909    0.820    -9.377    0.171  0.241892  0.455171 -0.0641393  -110.976    -9.390  
+22 7 6 59766.00 I  0.244459 0.000013  0.453293 0.000035  I-0.0635565 0.0000062 -0.5367 0.0047  I  -110.895    0.820    -9.260    0.171  0.244450  0.453302 -0.0635337  -110.950    -9.262  
+22 7 7 59767.00 I  0.247125 0.000013  0.451608 0.000035  I-0.0630515 0.0000063 -0.4635 0.0045  I  -111.265    0.820    -9.234    0.171  0.247124  0.451582 -0.0630501  -111.305    -9.226  
+22 7 8 59768.00 I  0.249746 0.000013  0.450109 0.000035  I-0.0625980 0.0000065 -0.4849 0.0047  I  -111.936    0.820    -9.243    0.171  0.249756  0.450120 -0.0625785  -111.978    -9.228  
+22 7 9 59769.00 I  0.252293 0.000009  0.448653 0.000024  I-0.0620342 0.0000071 -0.6487 0.0038  I  -112.679    0.877    -9.148    0.179  0.252297  0.448682 -0.0620271  -112.723    -9.129  
+22 710 59770.00 I  0.254694 0.000016  0.447028 0.000025  I-0.0612804 0.0000041 -0.8730 0.0043  I  -113.384    0.803    -8.978    0.143  0.254733  0.447060 -0.0612967  -113.423    -8.960  
+22 711 59771.00 I  0.256802 0.000016  0.445401 0.000017  I-0.0602885 0.0000047 -1.0964 0.0031  I  -113.968    0.771    -8.954    0.116  0.256857  0.445395 -0.0603249  -114.007    -8.936  
+22 712 59772.00 I  0.258321 0.000016  0.443917 0.000017  I-0.0591181 0.0000047 -1.2284 0.0030  I  -114.198    0.771    -9.167    0.116  0.258411  0.443974 -0.0591324  -114.246    -9.142  
+22 713 59773.00 I  0.259223 0.000017  0.442026 0.000020  I-0.0578283 0.0000036 -1.3707 0.0030  I  -113.927    0.783    -9.408    0.153  0.259174  0.442066 -0.0577813  -113.960    -9.403  
+22 714 59774.00 I  0.260256 0.000017  0.439915 0.000020  I-0.0564435 0.0000037 -1.3125 0.0027  I  -113.400    0.783    -9.465    0.153  0.260201  0.439888 -0.0564587  -113.418    -9.484  
+22 715 59775.00 I  0.261705 0.000018  0.438129 0.000019  I-0.0552624 0.0000039 -1.0771 0.0035  I  -113.026    0.783    -9.419    0.153  0.261642  0.438122 -0.0552630  -113.037    -9.466  
+22 716 59776.00 I  0.263451 0.000013  0.436348 0.000018  I-0.0542796 0.0000060 -0.8709 0.0028  I  -112.968    0.808    -9.461    0.195  0.263441  0.436373 -0.0542876  -112.983    -9.496  
+22 717 59777.00 I  0.265296 0.000017  0.434376 0.000019  I-0.0535139 0.0000041 -0.6849 0.0036  I  -113.148    0.864    -9.533    0.136  0.265267  0.434398 -0.0535228  -113.161    -9.544  
+22 718 59778.00 I  0.267260 0.000017  0.432334 0.000019  I-0.0528829 0.0000040 -0.5796 0.0030  I  -113.506    0.864    -9.412    0.136  0.267234  0.432352 -0.0528927  -113.506    -9.398  
+22 719 59779.00 I  0.269239 0.000018  0.430284 0.000014  I-0.0523133 0.0000045 -0.5983 0.0029  I  -113.980    0.894    -9.083    0.066  0.269260  0.430298 -0.0523068  -113.947    -9.037  
+22 720 59780.00 I  0.270985 0.000025  0.428191 0.000029  I-0.0516616 0.0000041 -0.6910 0.0031  I  -114.405    0.821    -8.812    0.126  0.270974  0.428173 -0.0516628  -114.393    -8.784  
+22 721 59781.00 I  0.272566 0.000025  0.426252 0.000029  I-0.0509179 0.0000043 -0.8240 0.0030  I  -114.656    0.821    -8.809    0.126  0.272574  0.426255 -0.0508922  -114.674    -8.805  
+22 722 59782.00 I  0.274104 0.000025  0.424462 0.000030  I-0.0499879 0.0000045 -1.0342 0.0040  I  -114.827    0.821    -9.000    0.126  0.274053  0.424453 -0.0499591  -114.884    -9.018  
+22 723 59783.00 I  0.275661 0.000023  0.422673 0.000029  I-0.0488633 0.0000067 -1.2030 0.0038  I  -115.067    0.680    -9.188    0.176  0.275681  0.422673 -0.0488673  -115.096    -9.210  
+22 724 59784.00 I  0.277055 0.000023  0.420910 0.000035  I-0.0475897 0.0000060 -1.3483 0.0045  I  -115.345    0.776    -9.320    0.182  0.277006  0.420915 -0.0476028  -115.333    -9.343  
+22 725 59785.00 I  0.278485 0.000023  0.419325 0.000035  I-0.0461859 0.0000059 -1.4360 0.0050  I  -115.499    0.776    -9.490    0.182  0.278471  0.419285 -0.0462003  -115.452    -9.519  
+22 726 59786.00 I  0.279855 0.000014  0.417904 0.000025  I-0.0447445 0.0000081 -1.4434 0.0052  I  -115.482    0.870    -9.729    0.190  0.279867  0.417962 -0.0447491  -115.399    -9.768  
+22 727 59787.00 I  0.281074 0.000023  0.416119 0.000039  I-0.0433006 0.0000085 -1.4464 0.0061  I  -115.416    0.830    -9.901    0.179  0.281044  0.416126 -0.0432579  -115.379    -9.934  
+22 728 59788.00 I  0.282268 0.000023  0.414141 0.000038  I-0.0418516 0.0000092 -1.4497 0.0070  I  -115.407    0.830    -9.846    0.179  0.282267  0.414205 -0.0417953  -115.431    -9.867  
+22 729 59789.00 I  0.283372 0.000022  0.411848 0.000038  I-0.0404325 0.0000110 -1.3592 0.0099  I  -115.450    0.830    -9.591    0.179  0.283345  0.411841 -0.0404282  -115.538    -9.595  
+22 730 59790.00 I  0.284624 0.000021  0.409427 0.000032  I-0.0391818 0.0000176 -1.1231 0.0076  I  -115.480    0.671    -9.336    0.152  0.284587  0.409400 -0.0392089  -115.593    -9.353  
+22 731 59791.00 I  0.285988 0.000025  0.407284 0.000041  I-0.0381746 0.0000106 -0.9222 0.0103  I  -115.462    0.777    -9.233    0.276  0.286000  0.407286 -0.0381849  -115.593    -9.273  
+22 8 1 59792.00 I  0.287130 0.000025  0.405197 0.000041  I-0.0373422 0.0000106 -0.7071 0.0069  I  -115.386    0.777    -9.258    0.276  0.287161  0.405194 -0.0373892  -115.536    -9.320  
+22 8 2 59793.00 I  0.287887 0.000019  0.403236 0.000032  I-0.0367520 0.0000088 -0.5173 0.0067  I  -115.276    0.760    -9.287    0.277  0.287882  0.403262 -0.0367846  -115.439    -9.376  
+22 8 3 59794.00 I  0.288545 0.000019  0.400998 0.000032  I-0.0362649 0.0000083 -0.4555 0.0057  I  -115.252    0.760    -9.257    0.277  0.288468  0.401019 -0.0362792  -115.414    -9.314  
+22 8 4 59795.00 I  0.289527 0.000019  0.398720 0.000032  I-0.0358182 0.0000073 -0.4622 0.0055  I  -115.487    0.760    -9.205    0.277  0.289489  0.398709 -0.0358145  -115.635    -9.222  
+22 8 5 59796.00 I  0.290537 0.000019  0.396553 0.000032  I-0.0353212 0.0000071 -0.5267 0.0052  I  -116.042    0.760    -9.178    0.277  0.290582  0.396579 -0.0353263  -116.154    -9.192  
+22 8 6 59797.00 I  0.291094 0.000015  0.394196 0.000017  I-0.0347348 0.0000073 -0.6811 0.0044  I  -116.770    0.717    -9.180    0.251  0.291080  0.394221 -0.0347316  -116.838    -9.204  
+22 8 7 59798.00 I  0.291547 0.000021  0.391643 0.000021  I-0.0339400 0.0000051 -0.8924 0.0047  I  -117.409    0.700    -9.226    0.255  0.291487  0.391652 -0.0339451  -117.435    -9.261  
+22 8 8 59799.00 I  0.292337 0.000019  0.389021 0.000014  I-0.0329727 0.0000058 -1.0355 0.0039  I  -117.721    0.685    -9.357    0.258  0.292293  0.389056 -0.0329721  -117.715    -9.399  
+22 8 9 59800.00 I  0.293210 0.000019  0.386220 0.000014  I-0.0318941 0.0000058 -1.1033 0.0037  I  -117.606    0.685    -9.522    0.258  0.293211  0.386232 -0.0318918  -117.585    -9.565  
+22 810 59801.00 I  0.293834 0.000021  0.383251 0.000026  I-0.0308088 0.0000045 -1.0429 0.0039  I  -117.203    0.743    -9.547    0.269  0.293803  0.383250 -0.0308088  -117.149    -9.591  
+22 811 59802.00 I  0.294451 0.000021  0.380334 0.000027  I-0.0298560 0.0000051 -0.8392 0.0036  I  -116.848    0.743    -9.351    0.269  0.294459  0.380298 -0.0298577  -116.770    -9.397  
+22 812 59803.00 I  0.295060 0.000021  0.377818 0.000027  I-0.0291390 0.0000057 -0.6096 0.0043  I  -116.775    0.743    -9.119    0.269  0.295055  0.377755 -0.0291384  -116.681    -9.171  
+22 813 59804.00 I  0.295579 0.000015  0.375709 0.000025  I-0.0286243 0.0000068 -0.4175 0.0043  I  -116.899    0.780    -9.088    0.278  0.295537  0.375740 -0.0286307  -116.834    -9.134  
+22 814 59805.00 I  0.296373 0.000014  0.373568 0.000025  I-0.0282807 0.0000064 -0.2951 0.0046  I  -117.030    0.780    -9.221    0.278  0.296313  0.373591 -0.0282983  -117.006    -9.266  
+22 815 59806.00 I  0.297512 0.000015  0.371304 0.000029  I-0.0279871 0.0000063 -0.3135 0.0063  I  -117.197    0.779    -9.253    0.230  0.297500  0.371314 -0.0279699  -117.203    -9.307  
+22 816 59807.00 I  0.298550 0.000014  0.369042 0.000019  I-0.0276157 0.0000109 -0.4460 0.0065  I  -117.539    0.779    -9.067    0.125  0.298583  0.369059 -0.0276395  -117.555    -9.139  
+22 817 59808.00 I  0.299277 0.000019  0.366742 0.000030  I-0.0270844 0.0000113 -0.6108 0.0079  I  -118.002    0.760    -8.854    0.125  0.299254  0.366732 -0.0270866  -118.003    -8.949  
+22 818 59809.00 I  0.299910 0.000020  0.364400 0.000031  I-0.0263631 0.0000113 -0.8687 0.0080  I  -118.372    0.760    -8.839    0.125  0.299866  0.364425 -0.0263517  -118.274    -8.865  
+22 819 59810.00 I  0.300903 0.000020  0.362025 0.000030  I-0.0253588 0.0000113 -1.0911 0.0082  I  -118.565    0.760    -9.005    0.125  0.300823  0.362010 -0.0253455  -118.335    -8.928  
+22 820 59811.00 I  0.302125 0.000020  0.359758 0.000030  I-0.0241914 0.0000118 -1.2820 0.0072  I  -118.671    0.760    -9.157    0.125  0.302176  0.359779 -0.0241871  -118.439    -9.105  
+22 821 59812.00 I  0.303009 0.000024  0.357421 0.000041  I-0.0228181 0.0000089 -1.4029 0.0073  I  -118.741    0.614    -9.190    0.108  0.302992  0.357455 -0.0228266  -118.572    -9.196  
+22 822 59813.00 I  0.303768 0.000023  0.354930 0.000041  I-0.0214185 0.0000086 -1.4250 0.0057  I  -118.710    0.614    -9.194    0.108  0.303769  0.354926 -0.0213929  -118.632    -9.243  
+22 823 59814.00 I  0.304486 0.000019  0.352484 0.000034  I-0.0199966 0.0000072 -1.3617 0.0051  I  -118.540    0.616    -9.291    0.104  0.304513  0.352500 -0.0199836  -118.587    -9.375  
+22 824 59815.00 I  0.304888 0.000018  0.349901 0.000039  I-0.0187067 0.0000056 -1.2635 0.0046  I  -118.308    0.714    -9.444    0.131  0.304896  0.349874 -0.0186613  -118.307    -9.531  
+22 825 59816.00 I  0.305185 0.000018  0.347450 0.000039  I-0.0174471 0.0000057 -1.2329 0.0040  I  -118.108    0.714    -9.494    0.131  0.305201  0.347486 -0.0174037  -118.023    -9.577  
+22 826 59817.00 I  0.305355 0.000017  0.344923 0.000039  I-0.0162886 0.0000056 -1.0594 0.0043  I  -117.945    0.714    -9.355    0.131  0.305398  0.344912 -0.0162851  -117.767    -9.438  
+22 827 59818.00 I  0.305270 0.000010  0.342339 0.000023  I-0.0153437 0.0000064 -0.8397 0.0038  I  -117.796    0.895    -9.124    0.159  0.305290  0.342335 -0.0153482  -117.637    -9.193  
+22 828 59819.00 I  0.304966 0.000020  0.339915 0.000030  I-0.0146128 0.0000050 -0.6091 0.0040  I  -117.682    0.774    -8.979    0.178  0.304974  0.339946 -0.0146136  -117.565    -9.035  
+22 829 59820.00 I  0.304625 0.000020  0.337394 0.000030  I-0.0141179 0.0000049 -0.4011 0.0036  I  -117.644    0.774    -9.006    0.178  0.304586  0.337401 -0.0140968  -117.551    -9.055  
+22 830 59821.00 I  0.304499 0.000020  0.334986 0.000023  I-0.0137967 0.0000052 -0.2347 0.0032  I  -117.661    0.717    -9.129    0.191  0.304464  0.334971 -0.0137838  -117.601    -9.176  
+22 831 59822.00 I  0.304617 0.000022  0.332728 0.000027  I-0.0136235 0.0000040 -0.1432 0.0033  I  -117.689    0.747    -9.210    0.165  0.304595  0.332751 -0.0136099  -117.612    -9.248  
+22 9 1 59823.00 I  0.304750 0.000022  0.330386 0.000027  I-0.0134686 0.0000040 -0.1769 0.0032  I  -117.787    0.747    -9.185    0.165  0.304814  0.330440 -0.0134836  -117.693    -9.211  
+22 9 2 59824.00 I  0.304506 0.000022  0.327664 0.000027  I-0.0132464 0.0000050 -0.2806 0.0035  I  -118.070    0.747    -9.105    0.165  0.304501  0.327651 -0.0132494  -118.154    -9.102  
+22 9 3 59825.00 I  0.304210 0.000012  0.325045 0.000017  I-0.0128898 0.0000057 -0.4371 0.0043  I  -118.518    0.778    -9.071    0.133  0.304186  0.324993 -0.0128821  -118.590    -9.080  
+22 9 4 59826.00 I  0.304086 0.000015  0.322759 0.000024  I-0.0123680 0.0000070 -0.6064 0.0046  I  -118.883    0.750    -9.142    0.193  0.304085  0.322764 -0.0123741  -118.929    -9.170  
+22 9 5 59827.00 I  0.303787 0.000015  0.320457 0.000023  I-0.0117011 0.0000071 -0.7036 0.0075  I  -118.886    0.750    -9.281    0.193  0.303820  0.320481 -0.0117203  -118.916    -9.328  
+22 9 6 59828.00 I  0.303228 0.000013  0.317957 0.000019  I-0.0110127 0.0000132 -0.6450 0.0062  I  -118.480    0.719    -9.349    0.246  0.303248  0.318029 -0.0110190  -118.525    -9.426  
+22 9 7 59829.00 I  0.302620 0.000015  0.314925 0.000027  I-0.0104253 0.0000102 -0.5436 0.0082  I  -117.922    0.887    -9.201    0.188  0.302652  0.314951 -0.0103738  -117.930    -9.248  
+22 9 8 59830.00 I  0.301723 0.000016  0.311761 0.000028  I-0.0099629 0.0000096 -0.3300 0.0072  I  -117.587    0.887    -8.846    0.188  0.301793  0.311758 -0.0099952  -117.557    -8.853  
+22 9 9 59831.00 I  0.300345 0.000017  0.308693 0.000029  I-0.0097975 0.0000102 -0.0199 0.0068  I  -117.615    0.887    -8.497    0.188  0.300297  0.308670 -0.0098037  -117.537    -8.461  
+22 910 59832.00 I  0.299161 0.000014  0.305663 0.000024  I-0.0098959 0.0000095  0.2084 0.0058  I  -117.809    1.155    -8.384    0.070  0.299086  0.305665 -0.0098938  -117.785    -8.354  
+22 911 59833.00 I  0.298571 0.000024  0.302851 0.000036  I-0.0101845 0.0000057  0.3472 0.0055  I  -117.910    1.007    -8.507    0.141  0.298524  0.302843 -0.0101991  -117.949    -8.495  
+22 912 59834.00 I  0.298128 0.000024  0.300270 0.000036  I-0.0105524 0.0000057  0.3723 0.0042  I  -117.925    1.007    -8.663    0.141  0.298153  0.300265 -0.0105663  -118.003    -8.665  
+22 913 59835.00 I  0.297554 0.000024  0.297926 0.000032  I-0.0108733 0.0000061  0.2299 0.0037  I  -118.064    0.934    -8.702    0.175  0.297509  0.297897 -0.0108687  -118.179    -8.722  
+22 914 59836.00 I  0.296978 0.000025  0.295807 0.000051  I-0.0109915 0.0000048  0.0255 0.0039  I  -118.399    0.930    -8.680    0.134  0.296992  0.295809 -0.0110048  -118.515    -8.694  
+22 915 59837.00 I  0.296334 0.000024  0.293809 0.000051  I-0.0109042 0.0000048 -0.2391 0.0034  I  -118.757    0.930    -8.727    0.134  0.296326  0.293853 -0.0109071  -118.881    -8.735  
+22 916 59838.00 I  0.295609 0.000024  0.291699 0.000051  I-0.0105277 0.0000047 -0.4605 0.0038  I  -118.920    0.930    -8.843    0.134  0.295633  0.291666 -0.0105453  -119.064    -8.840  
+22 917 59839.00 I  0.294744 0.000015  0.289611 0.000043  I-0.0099915 0.0000060 -0.6569 0.0035  I  -118.830    0.926    -8.901    0.072  0.294765  0.289613 -0.0099966  -118.954    -8.905  
+22 918 59840.00 I  0.293576 0.000020  0.287789 0.000057  I-0.0092321 0.0000052 -0.7987 0.0040  I  -118.558    0.998    -8.833    0.118  0.293594  0.287789 -0.0092502  -118.640    -8.844  
+22 919 59841.00 I  0.292284 0.000020  0.285843 0.000056  I-0.0084342 0.0000052 -0.8200 0.0040  I  -118.193    0.998    -8.730    0.118  0.292235  0.285928 -0.0084134  -118.223    -8.750  
+22 920 59842.00 I  0.291356 0.000020  0.283523 0.000039  I-0.0075715 0.0000060 -0.9029 0.0034  I  -117.817    1.067    -8.733    0.149  0.291284  0.283515 -0.0075559  -117.778    -8.771  
+22 921 59843.00 I  0.290657 0.000020  0.281046 0.000041  I-0.0066827 0.0000045 -0.8228 0.0037  I  -117.525    0.969    -8.846    0.115  0.290675  0.281089 -0.0066950  -117.531    -8.864  
+22 922 59844.00 I  0.289762 0.000020  0.278371 0.000041  I-0.0059697 0.0000043 -0.6114 0.0033  I  -117.370    0.969    -8.933    0.115  0.289785  0.278400 -0.0059969  -117.441    -8.921  
+22 923 59845.00 I  0.288625 0.000019  0.275550 0.000041  I-0.0054453 0.0000048 -0.4437 0.0038  I  -117.323    0.969    -8.862    0.115  0.288673  0.275532 -0.0054471  -117.457    -8.810  
+22 924 59846.00 I  0.287260 0.000013  0.272936 0.000016  I-0.0050917 0.0000063 -0.2478 0.0036  I  -117.318    0.763    -8.654    0.022  0.287244  0.272949 -0.0051006  -117.468    -8.622  
+22 925 59847.00 I  0.285950 0.000027  0.270430 0.000037  I-0.0049465 0.0000053 -0.0616 0.0041  I  -117.333    0.723    -8.458    0.183  0.285878  0.270404 -0.0049635  -117.484    -8.457  
+22 926 59848.00 I  0.285167 0.000027  0.268165 0.000037  I-0.0049530 0.0000054  0.0782 0.0042  I  -117.383    0.723    -8.411    0.183  0.285103  0.268121 -0.0049793  -117.537    -8.441  
+22 927 59849.00 I  0.284710 0.000027  0.266423 0.000035  I-0.0050991 0.0000066  0.2068 0.0039  I  -117.467    0.699    -8.518    0.247  0.284746  0.266357 -0.0051012  -117.616    -8.597  
+22 928 59850.00 I  0.283878 0.000028  0.264922 0.000035  I-0.0053104 0.0000055  0.1669 0.0041  I  -117.563    0.627    -8.651    0.177  0.283878  0.264953 -0.0053014  -117.693    -8.702  
+22 929 59851.00 I  0.283008 0.000027  0.263304 0.000035  I-0.0053959 0.0000048  0.0160 0.0036  I  -117.662    0.627    -8.692    0.177  0.282943  0.263319 -0.0054180  -117.779    -8.707  
+22 930 59852.00 I  0.282323 0.000027  0.261509 0.000035  I-0.0053335 0.0000048 -0.1615 0.0035  I  -117.777    0.627    -8.626    0.177  0.282338  0.261528 -0.0053388  -117.905    -8.603  
+2210 1 59853.00 I  0.281362 0.000013  0.259745 0.000014  I-0.0050469 0.0000050 -0.4171 0.0034  I  -117.856    0.514    -8.539    0.036  0.281388  0.259744 -0.0049041  -117.934    -8.536  
+2210 2 59854.00 I  0.280043 0.000011  0.257883 0.000014  I-0.0045484 0.0000049 -0.5255 0.0033  I  -117.773    0.514    -8.516    0.036  0.280092  0.257931 -0.0043864  -117.763    -8.633  
+2210 3 59855.00 I  0.278450 0.000018  0.255736 0.000015  I-0.0040473 0.0000042 -0.4797 0.0038  I  -117.410    0.880    -8.559    0.121  0.278478  0.255746 -0.0040146  -117.380    -8.681  
+2210 4 59856.00 I  0.276547 0.000017  0.253520 0.000015  I-0.0035919 0.0000057 -0.4253 0.0030  I  -116.810    1.094    -8.579    0.164  0.276607  0.253527 -0.0035590  -116.777    -8.672  
+2210 5 59857.00 I  0.274395 0.000017  0.251432 0.000021  I-0.0032283 0.0000042 -0.2762 0.0037  I  -116.208    1.048    -8.477    0.140  0.274352  0.251450 -0.0032281  -116.158    -8.550  
+2210 6 59858.00 I  0.272446 0.000021  0.249225 0.000021  I-0.0030732 0.0000047 -0.0259 0.0033  I  -115.870    1.048    -8.245    0.140  0.272409  0.249284 -0.0030816  -115.892    -8.306  
+2210 7 59859.00 I  0.270893 0.000024  0.246721 0.000019  I-0.0031814 0.0000050  0.2390 0.0035  I  -115.874    1.048    -7.990    0.140  0.270869  0.246728 -0.0031810  -115.963    -8.047  
+2210 8 59860.00 I  0.269391 0.000024  0.244284 0.000019  I-0.0035376 0.0000051  0.4632 0.0038  I  -116.056    1.048    -7.831    0.140  0.269464  0.244272 -0.0035337  -116.181    -7.889  
+2210 9 59861.00 I  0.267405 0.000019  0.242149 0.000017  I-0.0040729 0.0000057  0.5828 0.0033  I  -116.188    1.007    -7.792    0.112  0.267436  0.242181 -0.0040628  -116.323    -7.852  
+221010 59862.00 I  0.265327 0.000021  0.239992 0.000019  I-0.0046627 0.0000041  0.5811 0.0038  I  -116.197    0.874    -7.809    0.088  0.265240  0.239987 -0.0046541  -116.330    -7.871  
+221011 59863.00 I  0.263669 0.000021  0.237871 0.000012  I-0.0051867 0.0000049  0.4344 0.0031  I  -116.209    0.740    -7.835    0.055  0.263701  0.237885 -0.0051692  -116.344    -7.899  
+221012 59864.00 I  0.262030 0.000020  0.235728 0.000012  I-0.0055025 0.0000047  0.2007 0.0034  I  -116.363    0.783    -7.883    0.043  0.262046  0.235701 -0.0055011  -116.517    -7.950  
+221013 59865.00 I  0.259880 0.000018  0.233780 0.000012  I-0.0055843 0.0000048 -0.0442 0.0034  I  -116.617    0.783    -7.971    0.043  0.260021  0.233734 -0.0055722  -116.707    -8.023  
+221014 59866.00 I  0.256987 0.000018  0.232088 0.000011  I-0.0054363 0.0000050 -0.2223 0.0036  I  -116.775    0.783    -8.050    0.043  0.256936  0.232102 -0.0054362  -116.793    -8.078  
+221015 59867.00 I  0.254059 0.000018  0.230367 0.000011  I-0.0051796 0.0000053 -0.2806 0.0041  I  -116.667    0.783    -8.047    0.043  0.254063  0.230356 -0.0051876  -116.700    -8.075  
+221016 59868.00 I  0.251191 0.000018  0.228842 0.000026  I-0.0048947 0.0000065 -0.2802 0.0042  I  -116.282    0.899    -7.957    0.072  0.251206  0.228893 -0.0049099  -116.365    -7.987  
+221017 59869.00 I  0.248067 0.000022  0.227228 0.000027  I-0.0046551 0.0000064 -0.1722 0.0050  I  -115.751    0.899    -7.886    0.072  0.248052  0.227286 -0.0046783  -115.804    -7.935  
+221018 59870.00 I  0.245191 0.000019  0.225137 0.000028  I-0.0045621 0.0000075 -0.0288 0.0046  I  -115.218    0.932    -7.935    0.095  0.245102  0.225158 -0.0045660  -115.200    -8.015  
+221019 59871.00 I  0.243016 0.000019  0.222944 0.000034  I-0.0045915 0.0000067  0.0966 0.0050  I  -114.761    0.988    -8.084    0.131  0.243041  0.222898 -0.0045814  -114.747    -8.164  
+221020 59872.00 I  0.240704 0.000020  0.221151 0.000034  I-0.0047741 0.0000067  0.2784 0.0047  I  -114.448    0.988    -8.189    0.131  0.240817  0.221191 -0.0047645  -114.446    -8.265  
+221021 59873.00 I  0.237719 0.000020  0.219311 0.000034  I-0.0051506 0.0000065  0.4670 0.0053  I  -114.358    0.988    -8.116    0.131  0.237688  0.219313 -0.0051434  -114.344    -8.197  
+221022 59874.00 I  0.234655 0.000019  0.217534 0.000023  I-0.0057147 0.0000081  0.6755 0.0047  I  -114.523    1.044    -7.860    0.163  0.234606  0.217522 -0.0057243  -114.532    -7.927  
+221023 59875.00 I  0.232019 0.000015  0.216033 0.000026  I-0.0065067 0.0000069  0.8992 0.0054  I  -114.840    0.896    -7.538    0.137  0.231878  0.216031 -0.0064986  -114.866    -7.589  
+221024 59876.00 I  0.230033 0.000016  0.214646 0.000026  I-0.0074623 0.0000070  0.9704 0.0050  I  -115.124    0.896    -7.299    0.137  0.230043  0.214645 -0.0074339  -115.163    -7.341  
+221025 59877.00 I  0.228137 0.000016  0.213211 0.000023  I-0.0084022 0.0000071  0.9057 0.0049  I  -115.259    0.739    -7.232    0.089  0.228137  0.213232 -0.0084121  -115.318    -7.265  
+221026 59878.00 I  0.226079 0.000016  0.211770 0.000023  I-0.0092487 0.0000070  0.7662 0.0050  I  -115.254    0.739    -7.325    0.089  0.226115  0.211747 -0.0092591  -115.297    -7.349  
+221027 59879.00 I  0.223699 0.000015  0.210386 0.000022  I-0.0098858 0.0000070  0.4804 0.0048  I  -115.193    0.739    -7.487    0.089  0.223756  0.210409 -0.0098856  -115.222    -7.492  
+221028 59880.00 I  0.220829 0.000013  0.208851 0.000022  I-0.0102115 0.0000065  0.2004 0.0053  I  -115.115    0.739    -7.601    0.089  0.220823  0.208832 -0.0102779  -115.143    -7.612  
+221029 59881.00 I  0.217712 0.000013  0.207409 0.000017  I-0.0103251 0.0000080  0.0357 0.0043  I  -114.987    0.748    -7.610    0.051  0.217709  0.207418 -0.0103958  -115.022    -7.628  
+221030 59882.00 I  0.214510 0.000016  0.206265 0.000024  I-0.0102979 0.0000056 -0.0839 0.0047  I  -114.767    0.780    -7.555    0.167  0.214473  0.206229 -0.0103095  -114.810    -7.575  
+221031 59883.00 I  0.211392 0.000016  0.205212 0.000019  I-0.0101970 0.0000049 -0.0842 0.0037  I  -114.440    0.806    -7.515    0.226  0.211345  0.205237 -0.0101927  -114.492    -7.538  
+2211 1 59884.00 I  0.208608 0.000017  0.204242 0.000021  I-0.0101874 0.0000048  0.0894 0.0033  I  -114.044    0.806    -7.507    0.226  0.208514  0.204211 -0.0101774  -114.100    -7.544  
+2211 2 59885.00 I  0.206230 0.000018  0.203468 0.000026  I-0.0104119 0.0000044  0.3714 0.0034  I  -113.657    0.829    -7.480    0.192  0.206235  0.203545 -0.0104065  -113.700    -7.501  
+2211 3 59886.00 I  0.203875 0.000019  0.202379 0.000026  I-0.0109487 0.0000047  0.7090 0.0031  I  -113.378    0.829    -7.391    0.192  0.203841  0.202359 -0.0109528  -113.392    -7.399  
+2211 4 59887.00 I  0.201541 0.000018  0.201374 0.000026  I-0.0118055 0.0000044  0.9735 0.0040  I  -113.284    0.829    -7.242    0.192  0.201477  0.201353 -0.0118134  -113.257    -7.249  
+2211 5 59888.00 I  0.199498 0.000014  0.200681 0.000019  I-0.0128218 0.0000065  1.0162 0.0032  I  -113.376    0.852    -7.059    0.145  0.199403  0.200700 -0.0128173  -113.353    -7.066  
+2211 6 59889.00 I  0.197923 0.000015  0.199801 0.000025  I-0.0138077 0.0000046  0.9682 0.0042  I  -113.545    0.736    -6.862    0.097  0.197880  0.199789 -0.0138349  -113.543    -6.869  
+2211 7 59890.00 I  0.196415 0.000015  0.199008 0.000023  I-0.0147317 0.0000053  0.8409 0.0035  I  -113.642    0.736    -6.683    0.097  0.196436  0.198985 -0.0147274  -113.659    -6.688  
+2211 8 59891.00 I  0.194600 0.000028  0.198378 0.000025  I-0.0154512 0.0000053  0.5989 0.0035  I  -113.613    0.662    -6.586    0.027  0.194574  0.198424 -0.0154466  -113.660    -6.582  
+2211 9 59892.00 I  0.192635 0.000027  0.197577 0.000025  I-0.0159477 0.0000047  0.4115 0.0035  I  -113.553    0.662    -6.628    0.027  0.192696  0.197558 -0.0159684  -113.571    -6.657  
+221110 59893.00 I  0.190360 0.000027  0.196720 0.000025  I-0.0162477 0.0000047  0.1447 0.0031  I  -113.575    0.662    -6.785    0.027  0.190367  0.196722 -0.0162302  -113.564    -6.849  
+221111 59894.00 I  0.187844 0.000027  0.195891 0.000025  I-0.0162357 0.0000041 -0.1262 0.0041  I  -113.643    0.662    -6.942    0.027  0.187822  0.195880 -0.0162520  -113.631    -7.013  
+221112 59895.00 I  0.185418 0.000027  0.195030 0.000018  I-0.0160482 0.0000067 -0.2383 0.0029  I  -113.593    0.739    -6.992    0.002  0.185361  0.195076 -0.0160839  -113.596    -7.056  
+221113 59896.00 I  0.183321 0.000028  0.193962 0.000022  I-0.0157851 0.0000040 -0.2724 0.0038  I  -113.330    0.716    -6.948    0.082  0.183217  0.193981 -0.0158151  -113.352    -6.999  
+221114 59897.00 I  0.181908 0.000014  0.192835 0.000015  I-0.0155292 0.0000034 -0.2292 0.0027  I  -112.924    0.714    -6.925    0.090  0.181786  0.192794 -0.0155444  -112.967    -6.958  
+221115 59898.00 I  0.181149 0.000015  0.192237 0.000015  I-0.0153534 0.0000035 -0.1058 0.0026  I  -112.489    0.714    -6.991    0.090  0.181089  0.192167 -0.0153549  -112.549    -7.008  
+221116 59899.00 I  0.180591 0.000016  0.192106 0.000022  I-0.0153326 0.0000039  0.0627 0.0027  I  -112.067    0.740    -7.083    0.128  0.180613  0.192084 -0.0153236  -112.120    -7.099  
+221117 59900.00 I  0.179829 0.000015  0.192248 0.000023  I-0.0154880 0.0000041  0.2587 0.0029  I  -111.705    0.740    -7.070    0.128  0.179894  0.192217 -0.0154871  -111.735    -7.093  
+221118 59901.00 I  0.178495 0.000016  0.192646 0.000023  I-0.0158574 0.0000044  0.4767 0.0041  I  -111.561    0.740    -6.901    0.128  0.178587  0.192658 -0.0158559  -111.559    -6.936  
+221119 59902.00 I  0.176650 0.000012  0.192925 0.000020  I-0.0164185 0.0000070  0.6260 0.0030  I  -111.786    0.775    -6.640    0.159  0.176631  0.192939 -0.0164100  -111.782    -6.671  
+221120 59903.00 I  0.174676 0.000012  0.192883 0.000023  I-0.0171056 0.0000042  0.7640 0.0041  I  -112.281    0.703    -6.374    0.142  0.174678  0.192941 -0.0171134  -112.283    -6.399  
+221121 59904.00 I  0.172507 0.000012  0.192690 0.000023  I-0.0179152 0.0000042  0.8080 0.0029  I  -112.743    0.703    -6.140    0.142  0.172482  0.192686 -0.0178985  -112.747    -6.164  
+221122 59905.00 I  0.170166 0.000011  0.192510 0.000017  I-0.0186674 0.0000040  0.6894 0.0038  I  -112.971    0.650    -5.974    0.128  0.170135  0.192562 -0.0186627  -112.985    -5.999  
+221123 59906.00 I  0.167914 0.000014  0.192110 0.000035  I-0.0192785 0.0000063  0.5243 0.0038  I  -113.013    0.651    -5.963    0.121  0.167864  0.192125 -0.0192839  -113.015    -5.992  
+221124 59907.00 I  0.165798 0.000014  0.191649 0.000035  I-0.0196865 0.0000064  0.2707 0.0046  I  -112.965    0.651    -6.144    0.121  0.165815  0.191634 -0.0196773  -112.960    -6.178  
+221125 59908.00 I  0.163386 0.000014  0.191406 0.000035  I-0.0198180 0.0000066  0.0114 0.0061  I  -112.800    0.651    -6.380    0.121  0.163449  0.191394 -0.0198119  -112.800    -6.422  
+221126 59909.00 I  0.160411 0.000016  0.191123 0.000034  I-0.0197339 0.0000103 -0.1741 0.0060  I  -112.499    0.651    -6.463    0.113  0.160439  0.191188 -0.0197408  -112.502    -6.504  
+221127 59910.00 I  0.156936 0.000016  0.190783 0.000034  I-0.0195087 0.0000100 -0.2429 0.0064  I  -112.172    0.651    -6.353    0.113  0.156985  0.190819 -0.0195486  -112.173    -6.392  
+221128 59911.00 I  0.153234 0.000015  0.190262 0.000036  I-0.0193014 0.0000077 -0.1518 0.0059  I  -111.943    0.736    -6.212    0.087  0.153168  0.190278 -0.0193141  -111.939    -6.246  
+221129 59912.00 I  0.149942 0.000013  0.189790 0.000016  I-0.0192279 0.0000064  0.0078 0.0047  I  -111.811    0.832    -6.175    0.051  0.149881  0.189736 -0.0192085  -111.789    -6.198  
+221130 59913.00 I  0.147025 0.000017  0.189832 0.000022  I-0.0193202 0.0000054  0.1771 0.0041  I  -111.708    0.751    -6.198    0.094  0.146998  0.189837 -0.0193120  -111.648    -6.204  
+2212 1 59914.00 I  0.144055 0.000021  0.190078 0.000022  I-0.0195934 0.0000051  0.3802 0.0037  I  -111.624    0.751    -6.171    0.094  0.144039  0.190129 -0.0196037  -111.563    -6.191  
+2212 2 59915.00 I  0.141127 0.000021  0.189960 0.000023  I-0.0200309 0.0000051  0.4342 0.0036  I  -111.587    0.751    -6.063    0.094  0.141086  0.190030 -0.0200182  -111.557    -6.103  
+2212 3 59916.00 I  0.138501 0.000021  0.189628 0.000025  I-0.0204315 0.0000051  0.3974 0.0035  I  -111.616    0.751    -5.915    0.094  0.138520  0.189588 -0.0204483  -111.593    -5.954  
+2212 4 59917.00 I  0.135670 0.000022  0.189544 0.000025  I-0.0208123 0.0000048  0.3203 0.0036  I  -111.697    0.814    -5.755    0.131  0.135739  0.189603 -0.0208072  -111.696    -5.787  
+2212 5 59918.00 I  0.132719 0.000023  0.189098 0.000025  I-0.0210315 0.0000050  0.1215 0.0035  I  -111.741    0.814    -5.594    0.131  0.132595  0.189132 -0.0210271  -111.763    -5.625  
+2212 6 59919.00 I  0.130243 0.000022  0.188804 0.000021  I-0.0210516 0.0000052 -0.0884 0.0037  I  -111.651    0.986    -5.493    0.142  0.130234  0.188807 -0.0210546  -111.664    -5.528  
+2212 7 59920.00 I  0.127862 0.000020  0.188834 0.000024  I-0.0208560 0.0000054 -0.2943 0.0038  I  -111.477    0.838    -5.541    0.113  0.127804  0.188914 -0.0208636  -111.530    -5.568  
+2212 8 59921.00 I  0.125542 0.000018  0.188710 0.000023  I-0.0204803 0.0000056 -0.4484 0.0040  I  -111.359    0.838    -5.751    0.113  0.125550  0.188683 -0.0204842  -111.431    -5.765  
+2212 9 59922.00 I  0.123013 0.000018  0.188908 0.000021  I-0.0199691 0.0000060 -0.5727 0.0048  I  -111.366    0.838    -6.004    0.113  0.123051  0.188943 -0.0199575  -111.450    -5.997  
+221210 59923.00 I  0.120044 0.000016  0.189244 0.000016  I-0.0193475 0.0000078 -0.6591 0.0045  I  -111.402    0.680    -6.147    0.074  0.120023  0.189212 -0.0193465  -111.433    -6.148  
+221211 59924.00 I  0.117118 0.000016  0.189440 0.000024  I-0.0186861 0.0000068 -0.6399 0.0052  I  -111.327    0.690    -6.155    0.158  0.117059  0.189519 -0.0187186  -111.306    -6.171  
+221212 59925.00 I  0.114540 0.000014  0.189327 0.000024  I-0.0180997 0.0000068 -0.5249 0.0043  I  -111.103    0.690    -6.137    0.158  0.114474  0.189311 -0.0181257  -111.063    -6.164  
+221213 59926.00 I  0.112258 0.000014  0.189386 0.000024  I-0.0176355 0.0000052 -0.4125 0.0042  I  -110.760    0.814    -6.171    0.193  0.112235  0.189380 -0.0176371  -110.733    -6.213  
+221214 59927.00 I  0.110085 0.000014  0.189773 0.000024  I-0.0172856 0.0000048 -0.2675 0.0033  I  -110.321    0.814    -6.189    0.193  0.110057  0.189733 -0.0172887  -110.324    -6.215  
+221215 59928.00 I  0.107805 0.000014  0.190633 0.000023  I-0.0171050 0.0000042 -0.1091 0.0032  I  -109.853    0.814    -6.075    0.193  0.107848  0.190644 -0.0170929  -109.882    -6.084  
+221216 59929.00 I  0.105273 0.000014  0.191581 0.000023  I-0.0170821 0.0000041  0.0935 0.0029  I  -109.577    0.814    -5.844    0.193  0.105276  0.191662 -0.0170407  -109.642    -5.845  
+221217 59930.00 I  0.102628 0.000011  0.192140 0.000016  I-0.0172782 0.0000040  0.2548 0.0030  I  -109.720    0.903    -5.642    0.178  0.102588  0.192217 -0.0171383  -109.796    -5.644  
+221218 59931.00 I  0.100234 0.000024  0.192465 0.000038  I-0.0175404 0.0000044  0.2622 0.0038  I  -110.233    0.796    -5.555    0.137  0.100160  0.192490 -0.0173664  -110.291    -5.561  
+221219 59932.00 I  0.098289 0.000024  0.192767 0.000037  I-0.0177852 0.0000065  0.2174 0.0031  I  -110.806    0.687    -5.485    0.080  0.098210  0.192803 -0.0177187  -110.824    -5.496  
+221220 59933.00 I  0.096780 0.000026  0.193098 0.000038  I-0.0179691 0.0000044  0.1544 0.0040  I  -111.251    0.630    -5.327    0.078  0.096711  0.193084 -0.0179634  -111.212    -5.340  
+221221 59934.00 I  0.095783 0.000025  0.193369 0.000038  I-0.0180904 0.0000046  0.0806 0.0032  I  -111.661    0.630    -5.202    0.078  0.095777  0.193348 -0.0181234  -111.654    -5.239  
+221222 59935.00 I  0.094827 0.000026  0.194012 0.000039  I-0.0181002 0.0000047 -0.0835 0.0033  I  -112.054    0.630    -5.334    0.078  0.094877  0.193950 -0.0181060  -112.105    -5.394  
+221223 59936.00 I  0.093412 0.000028  0.194949 0.000039  I-0.0179153 0.0000048 -0.2719 0.0033  I  -112.156    0.630    -5.688    0.078  0.093472  0.194922 -0.0178955  -112.150    -5.759  
+221224 59937.00 I  0.091300 0.000019  0.196101 0.000017  I-0.0176069 0.0000046 -0.3087 0.0034  I  -111.800    0.565    -5.935    0.075  0.091397  0.196126 -0.0175841  -111.706    -6.007  
+221225 59938.00 I  0.088380 0.000019  0.197002 0.000016  I-0.0173447 0.0000048 -0.2052 0.0040  I  -111.255    0.565    -5.874    0.075  0.088402  0.197099 -0.0173115  -111.094    -5.943  
+221226 59939.00 I  0.085232 0.000042  0.197368 0.000041  I-0.0172486 0.0000065  0.0544 0.0039  I  -110.921    0.578    -5.678    0.166  0.085204  0.197391 -0.0172323  -110.709    -5.742  
+221227 59940.00 I  0.081992 0.000042  0.197787 0.000041  I-0.0174695 0.0000062  0.3618 0.0043  I  -110.868    0.578    -5.599    0.166  0.082060  0.197809 -0.0174541  -110.623    -5.660  
+221228 59941.00 I  0.078272 0.000044  0.198344 0.000042  I-0.0179186 0.0000056  0.5083 0.0042  I  -110.908    0.656    -5.612    0.153  0.078253  0.198379 -0.0179243  -110.647    -5.673  
+221229 59942.00 I  0.074738 0.000043  0.198601 0.000042  I-0.0184525 0.0000057  0.5539 0.0039  I  -110.946    0.656    -5.527    0.153  0.074744  0.198584 -0.0184719  -110.694    -5.570  
+221230 59943.00 I  0.071203 0.000043  0.199206 0.000041  I-0.0190020 0.0000054  0.5263 0.0040  I  -111.033    0.656    -5.313    0.153  0.071281  0.199199 -0.0190102  -110.793    -5.341  
+221231 59944.00 I  0.067041 0.000043  0.200080 0.000041  I-0.0194826 0.0000056  0.4312 0.0044  I  -111.201    0.656    -5.126    0.153  0.067074  0.200103 -0.0194855  -110.973    -5.182  
+23 1 1 59945.00 I  0.062786 0.000019  0.200919 0.000015  I-0.0198272 0.0000070  0.2245 0.0041  I  -111.392    0.715    -5.060    0.140  0.062699  0.200944 -0.0197967  -111.162    -5.163  
+23 1 2 59946.00 I  0.059055 0.000022  0.201756 0.000023  I-0.0199244 0.0000060 -0.0038 0.0054  I  -111.512    0.573    -5.062    0.097  0.059003  0.201796 -0.0199243  -111.443    -5.114  
+23 1 3 59947.00 I  0.055737 0.000019  0.202460 0.000034  I-0.0198275 0.0000082 -0.2084 0.0052  I  -111.468    0.606    -5.076    0.132  0.055638  0.202514 -0.0198250  -111.467    -5.128  
+23 1 4 59948.00 I  0.052977 0.000019  0.203016 0.000035  I-0.0195035 0.0000086 -0.4253 0.0062  I  -111.218    0.606    -5.159    0.132  0.052933  0.202990 -0.0195007  -111.313    -5.194  
+23 1 5 59949.00 I  0.050803 0.000019  0.203873 0.000036  I-0.0190212 0.0000094 -0.5092 0.0064  I  -110.849    0.606    -5.389    0.132  0.050795  0.203830 -0.0190232  -110.822    -5.531  
+23 1 6 59950.00 I  0.048797 0.000020  0.205075 0.000036  I-0.0185021 0.0000094 -0.5419 0.0066  I  -110.558    0.606    -5.685    0.132  0.048795  0.205101 -0.0184663  -110.510    -5.834  
+23 1 7 59951.00 I  0.046882 0.000019  0.206241 0.000036  I-0.0179526 0.0000092 -0.5288 0.0068  I  -110.423    0.606    -5.868    0.132  0.046853  0.206221 -0.0179143  -110.392    -5.984  
+23 1 8 59952.00 I  0.045143 0.000016  0.207584 0.000032  I-0.0174794 0.0000097 -0.4110 0.0063  I  -110.351    0.816    -5.857    0.177  0.045146  0.207590 -0.0174487  -110.316    -5.948  
+23 1 9 59953.00 I  0.043364 0.000011  0.209053 0.000016  I-0.0171413 0.0000085 -0.2612 0.0062  I  -110.218    0.807    -5.747    0.146  0.043370  0.209111 -0.0171274  -110.159    -5.821  
+23 110 59954.00 I  0.041296 0.000010  0.210242 0.000014  I-0.0169624 0.0000077 -0.0953 0.0055  I  -109.979    0.807    -5.670    0.146  0.041325  0.210288 -0.0169671  -109.874    -5.733  
+23 111 59955.00 I  0.038966 0.000015  0.211106 0.000015  I-0.0169542 0.0000070  0.0813 0.0049  I  -109.660    0.754    -5.623    0.124  0.038979  0.211134 -0.0169747  -109.583    -5.665  
+23 112 59956.00 I  0.036561 0.000014  0.211940 0.000014  I-0.0170849 0.0000062  0.1378 0.0048  I  -109.329    0.754    -5.515    0.124  0.036547  0.211915 -0.0170559  -109.296    -5.533  
+23 113 59957.00 I  0.034182 0.000014  0.213038 0.000014  I-0.0172131 0.0000067  0.1441 0.0058  I  -109.127    0.754    -5.352    0.124  0.034173  0.213022 -0.0172046  -109.147    -5.343  
+23 114 59958.00 I  0.031794 0.000013  0.214424 0.000012  I-0.0173788 0.0000099  0.1675 0.0057  I  -109.205    0.669    -5.285    0.088  0.031810  0.214393 -0.0173877  -109.253    -5.273  
+23 115 59959.00 I  0.029348 0.000016  0.216072 0.000021  I-0.0175459 0.0000092  0.1844 0.0069  I  -109.543    0.637    -5.406    0.113  0.029351  0.216047 -0.0175710  -109.621    -5.396  
+23 116 59960.00 I  0.026873 0.000016  0.217964 0.000021  I-0.0177222 0.0000095  0.1250 0.0073  I  -109.926    0.637    -5.573    0.113  0.026882  0.217923 -0.0177110  -110.037    -5.563  
+23 117 59961.00 I  0.024332 0.000012  0.220219 0.000019  I-0.0177507 0.0000113 -0.0702 0.0069  I  -110.264    0.618    -5.570    0.129  0.024343  0.220214 -0.0177400  -110.403    -5.564  
+23 118 59962.00 I  0.021690 0.000039  0.222446 0.000019  I-0.0175804 0.0000101 -0.2696 0.0075  I  -110.745    0.676    -5.451    0.136  0.021681  0.222504 -0.0175873  -110.857    -5.445  
+23 119 59963.00 I  0.019115 0.000040  0.224215 0.000019  I-0.0172297 0.0000099 -0.4145 0.0071  I  -111.420    0.676    -5.517    0.136  0.019078  0.224261 -0.0172362  -111.474    -5.516  
+23 120 59964.00 I  0.016662 0.000040  0.225636 0.000019  I-0.0167588 0.0000100 -0.5373 0.0081  I  -111.874    0.676    -5.878    0.136  0.016715  0.225678 -0.0167521  -111.849    -5.887  
+23 121 59965.00 I  0.013978 0.000039  0.226843 0.000011  I-0.0161726 0.0000127 -0.6075 0.0061  I  -111.678    0.845    -6.222    0.148  0.014033  0.226892 -0.0161896  -111.635    -6.235  
+23 122 59966.00 I  0.010876 0.000040  0.227751 0.000014  I-0.0156157 0.0000070 -0.4620 0.0071  I  -110.999    0.550    -6.219    0.105  0.010879  0.227740 -0.0156593  -110.964    -6.230  
+23 123 59967.00 I  0.007811 0.000040  0.228860 0.000016  I-0.0152836 0.0000065 -0.2114 0.0047  I  -110.402    0.550    -5.967    0.105  0.007728  0.228830 -0.0153087  -110.393    -5.970  
+23 124 59968.00 I  0.005409 0.000019  0.230211 0.000017  I-0.0152061 0.0000062  0.0789 0.0045  I  -110.171    0.354    -5.801    0.066  0.005300  0.230244 -0.0152158  -110.223    -5.787  
+23 125 59969.00 I  0.003919 0.000023  0.231456 0.000027  I-0.0154130 0.0000062  0.2841 0.0044  I  -110.166    0.569    -5.798    0.149  0.003852  0.231401 -0.0153642  -110.193    -5.799  
+23 126 59970.00 I  0.002888 0.000024  0.233326 0.000029  I-0.0156959 0.0000062  0.2542 0.0043  I  -110.256    0.569    -5.755    0.149  0.002927  0.233231 -0.0156349  -110.268    -5.775  
+23 127 59971.00 I  0.001580 0.000024  0.235870 0.000030  I-0.0159008 0.0000061  0.1625 0.0049  I  -110.440    0.569    -5.595    0.149  0.001593  0.235918 -0.0158886  -110.468    -5.635  
+23 128 59972.00 I  0.000382 0.000022  0.238118 0.000030  I-0.0159939 0.0000076 -0.0101 0.0046  I  -110.659    0.709    -5.503    0.193  0.000279  0.238107 -0.0159862  -110.687    -5.537  
+23 129 59973.00 I -0.000272 0.000026  0.240384 0.000033  I-0.0158856 0.0000069 -0.1677 0.0051  I  -110.781    0.831    -5.636    0.183 -0.000230  0.240378 -0.0158927  -110.794    -5.657  
+23 130 59974.00 I -0.000860 0.000025  0.242657 0.000033  I-0.0156618 0.0000067 -0.3155 0.0051  I  -110.771    0.831    -5.890    0.183 -0.000925  0.242670 -0.0156444  -110.750    -5.905  
+23 131 59975.00 I -0.001399 0.000022  0.245014 0.000026  I-0.0152307 0.0000074 -0.5349 0.0045  I  -110.672    1.146    -6.069    0.163 -0.001326  0.244961 -0.0152262  -110.583    -6.080  
+23 2 1 59976.00 I -0.002309 0.000021  0.247812 0.000044  I-0.0146185 0.0000061 -0.6749 0.0048  I  -110.484    1.038    -6.147    0.176 -0.002296  0.247864 -0.0146010  -110.444    -6.163  
+23 2 2 59977.00 I -0.003561 0.000021  0.250311 0.000044  I-0.0138975 0.0000060 -0.7652 0.0044  I  -110.207    1.038    -6.241    0.176 -0.003547  0.250346 -0.0138591  -110.219    -6.262  
+23 2 3 59978.00 I -0.004904 0.000021  0.252506 0.000043  I-0.0131157 0.0000063 -0.7729 0.0046  I  -109.945    1.038    -6.397    0.176 -0.004856  0.252572 -0.0130960  -109.978    -6.426  
+23 2 4 59979.00 I -0.006471 0.000017  0.254279 0.000041  I-0.0124014 0.0000070 -0.6316 0.0041  I  -109.831    0.944    -6.502    0.187 -0.006428  0.254285 -0.0124190  -109.861    -6.529  
+23 2 5 59980.00 I -0.008209 0.000019  0.255937 0.000041  I-0.0118698 0.0000053 -0.4386 0.0044  I  -109.847    0.729    -6.431    0.154 -0.008204  0.255923 -0.0118777  -109.870    -6.457  
+23 2 6 59981.00 I -0.009960 0.000020  0.257733 0.000041  I-0.0115083 0.0000053 -0.2935 0.0037  I  -109.837    0.729    -6.223    0.154 -0.009964  0.257731 -0.0114958  -109.866    -6.252  
+23 2 7 59982.00 I -0.011916 0.000020  0.259667 0.000017  I-0.0112781 0.0000051 -0.1625 0.0032  I  -109.681    0.541    -6.036    0.116 -0.011876  0.259655 -0.0112745  -109.747    -6.070  
+23 2 8 59983.00 I -0.014092 0.000033  0.261639 0.000038  I-0.0111859 0.0000035 -0.0237 0.0030  I  -109.406    0.739    -5.952    0.086 -0.014175  0.261674 -0.0111959  -109.435    -5.978  
+23 2 9 59984.00 I -0.015723 0.000032  0.263453 0.000038  I-0.0112380 0.0000033  0.1369 0.0026  I  -109.143    0.739    -5.925    0.086 -0.015815  0.263434 -0.0112446  -109.132    -5.933  
+23 210 59985.00 I -0.016726 0.000032  0.265588 0.000038  I-0.0114602 0.0000038  0.2991 0.0030  I  -109.016    0.739    -5.905    0.086 -0.016692  0.265519 -0.0114722  -108.968    -5.888  
+23 211 59986.00 I -0.017893 0.000029  0.268005 0.000037  I-0.0117978 0.0000051  0.3462 0.0029  I  -109.087    0.911    -5.946    0.044 -0.017796  0.268043 -0.0117909  -109.040    -5.942  
+23 212 59987.00 I -0.019635 0.000029  0.270435 0.000037  I-0.0121293 0.0000044  0.3233 0.0033  I  -109.309    0.766    -6.118    0.124 -0.019580  0.270405 -0.0121316  -109.260    -6.133  
+23 213 59988.00 I -0.021943 0.000029  0.273088 0.000038  I-0.0124050 0.0000043  0.1823 0.0035  I  -109.543    0.766    -6.351    0.124 -0.021949  0.273140 -0.0123642  -109.473    -6.379  
+23 214 59989.00 I -0.024483 0.000015  0.275695 0.000018  I-0.0124666 0.0000054 -0.0406 0.0036  I  -109.724    0.669    -6.481    0.163 -0.024489  0.275701 -0.0124632  -109.625    -6.523  
+23 215 59990.00 I -0.026965 0.000028  0.278180 0.000020  I-0.0123412 0.0000058 -0.2113 0.0038  I  -109.978    0.644    -6.487    0.150 -0.026961  0.278194 -0.0123539  -109.980    -6.504  
+23 216 59991.00 I -0.029371 0.000027  0.280690 0.000021  I-0.0120580 0.0000054 -0.3399 0.0040  I  -110.405    0.644    -6.569    0.150 -0.029393  0.280732 -0.0120613  -110.553    -6.554  
+23 217 59992.00 I -0.031759 0.000027  0.282893 0.000023  I-0.0116893 0.0000054 -0.3849 0.0048  I  -110.765    0.644    -6.864    0.150 -0.031780  0.282935 -0.0116902  -111.072    -6.818  
+23 218 59993.00 I -0.033991 0.000025  0.284847 0.000023  I-0.0113596 0.0000080 -0.2157 0.0045  I  -110.671    0.401    -7.190    0.084 -0.034066  0.284869 -0.0113623  -110.935    -7.143  
+23 219 59994.00 I -0.035823 0.000032  0.286845 0.000028  I-0.0113099 0.0000071  0.1097 0.0053  I  -110.105    0.723    -7.250    0.201 -0.035884  0.286825 -0.0113117  -110.257    -7.216  
+23 220 59995.00 I -0.037241 0.000031  0.288962 0.000027  I-0.0115759 0.0000071  0.4259 0.0049  I  -109.463    0.723    -7.045    0.201 -0.037338  0.288920 -0.0115669  -109.509    -7.029  
+23 221 59996.00 I -0.038247 0.000021  0.291495 0.000025  I-0.0121535 0.0000067  0.7175 0.0045  I  -109.083    0.769    -6.850    0.230 -0.038274  0.291422 -0.0121587  -109.019    -6.868  
+23 222 59997.00 I -0.038779 0.000023  0.294616 0.000025  I-0.0129450 0.0000055  0.8115 0.0046  I  -108.997    0.742    -6.807    0.179 -0.038866  0.294588 -0.0129291  -108.925    -6.815  
+23 223 59998.00 I -0.038964 0.000025  0.298256 0.000023  I-0.0137345 0.0000062  0.7795 0.0047  I  -109.136    0.742    -6.787    0.179 -0.038960  0.298263 -0.0137066  -109.077    -6.785  
+23 224 59999.00 I -0.039165 0.000025  0.301855 0.000023  I-0.0144986 0.0000077  0.7312 0.0056  I  -109.461    0.742    -6.698    0.179 -0.039119  0.301926 -0.0145020  -109.413    -6.693  
+23 225 60000.00 I -0.039676 0.000017  0.305101 0.000012  I-0.0151484 0.0000094  0.5373 0.0058  I  -109.838    0.661    -6.676    0.065 -0.039564  0.305114 -0.0151424  -109.790    -6.690  
+23 226 60001.00 I -0.040939 0.000021  0.308169 0.000017  I-0.0155416 0.0000087  0.2486 0.0064  I  -110.068    0.721    -6.868    0.058 -0.040856  0.308232 -0.0155421  -110.020    -6.905  
+23 227 60002.00 I -0.042705 0.000021  0.310720 0.000018  I-0.0156487 0.0000088 -0.0309 0.0075  I  -110.088    0.721    -7.181    0.058 -0.042777  0.310760 -0.0156050  -110.045    -7.236  
+23 228 60003.00 I -0.044028 0.000020  0.313321 0.000018  I-0.0155141 0.0000123 -0.2074 0.0064  I  -109.978    0.881    -7.385    0.021 -0.044051  0.313293 -0.0155019  -109.938    -7.454  
+23 3 1 60004.00 I -0.045094 0.000019  0.316290 0.000019  I-0.0152968 0.0000092 -0.1953 0.0072  I  -109.760    0.860    -7.402    0.122 -0.045086  0.316379 -0.0152786  -109.729    -7.431  
+23 3 2 60005.00 I -0.046059 0.000018  0.318742 0.000019  I-0.0151071 0.0000075 -0.2323 0.0058  I  -109.391    0.860    -7.361    0.122 -0.046065  0.318766 -0.0150624  -109.433    -7.347  
+23 3 3 60006.00 I -0.046662 0.000016  0.321114 0.000019  I-0.0148441 0.0000072 -0.2336 0.0051  I  -108.939    0.860    -7.400    0.122 -0.046677  0.321138 -0.0148245  -108.998    -7.328  
+23 3 4 60007.00 I -0.046921 0.000012  0.323798 0.000016  I-0.0146894 0.0000069 -0.0865 0.0048  I  -108.601    0.815    -7.480    0.217 -0.046882  0.323792 -0.0146819  -108.638    -7.416  
+23 3 5 60008.00 I -0.046594 0.000036  0.326590 0.000019  I-0.0146895 0.0000064  0.1156 0.0045  I  -108.485    0.909    -7.454    0.104 -0.046540  0.326621 -0.0146823  -108.483    -7.439  
+23 3 6 60009.00 I -0.045655 0.000037  0.329778 0.000018  I-0.0149305 0.0000059  0.3474 0.0047  I  -108.494    0.909    -7.281    0.104 -0.045657  0.329817 -0.0149129  -108.456    -7.322  
+23 3 7 60010.00 I -0.044607 0.000036  0.333305 0.000017  I-0.0153729 0.0000068  0.5451 0.0040  I  -108.473    0.929    -7.082    0.044 -0.044599  0.333296 -0.0153659  -108.413    -7.174  
+23 3 8 60011.00 I -0.043512 0.000037  0.336633 0.000016  I-0.0160146 0.0000054  0.7245 0.0042  I  -108.402    0.795    -7.003    0.038 -0.043530  0.336616 -0.0160051  -108.388    -7.094  
+23 3 9 60012.00 I -0.042352 0.000037  0.339812 0.000016  I-0.0167933 0.0000050  0.8181 0.0036  I  -108.377    0.795    -7.071    0.038 -0.042352  0.339803 -0.0167760  -108.432    -7.140  
+23 310 60013.00 I -0.041303 0.000037  0.343079 0.000015  I-0.0176198 0.0000048  0.8186 0.0031  I  -108.451    0.795    -7.206    0.038 -0.041322  0.343084 -0.0176027  -108.573    -7.251  
+23 311 60014.00 I -0.040750 0.000013  0.346411 0.000009  I-0.0184075 0.0000038  0.7501 0.0034  I  -108.577    0.697    -7.341    0.034 -0.040776  0.346390 -0.0184047  -108.718    -7.379  
+23 312 60015.00 I -0.040529 0.000013  0.349519 0.000010  I-0.0190955 0.0000048  0.6083 0.0031  I  -108.692    0.740    -7.472    0.052 -0.040519  0.349496 -0.0190910  -108.819    -7.513  
+23 313 60016.00 I -0.040089 0.000013  0.352556 0.000010  I-0.0195981 0.0000049  0.3886 0.0039  I  -108.760    0.740    -7.613    0.052 -0.040097  0.352572 -0.0196023  -108.854    -7.660  
+23 314 60017.00 I -0.039702 0.000014  0.355962 0.000012  I-0.0199052 0.0000062  0.2663 0.0039  I  -108.752    0.812    -7.749    0.072 -0.039717  0.355976 -0.0199116  -108.796    -7.801  
+23 315 60018.00 I -0.039676 0.000014  0.359426 0.000012  I-0.0201114 0.0000060  0.0860 0.0043  I  -108.663    0.812    -7.869    0.072 -0.039696  0.359397 -0.0200604  -108.636    -7.924  
+23 316 60019.00 I -0.039798 0.000013  0.362273 0.000012  I-0.0200825 0.0000060 -0.0783 0.0042  I  -108.524    0.812    -8.014    0.072 -0.039824  0.362249 -0.0200712  -108.426    -8.068  
+23 317 60020.00 I -0.039667 0.000012  0.364618 0.000012  I-0.0200347 0.0000059 -0.0030 0.0043  I  -108.359    0.812    -8.204    0.072 -0.039666  0.364628 -0.0200376  -108.244    -8.259  
+23 318 60021.00 I -0.039055 0.000011  0.366839 0.000011  I-0.0201206 0.0000063  0.2047 0.0035  I  -108.157    0.322    -8.345    0.160 -0.039047  0.366850 -0.0201299  -108.073    -8.402  
+23 319 60022.00 I -0.038098 0.000013  0.368982 0.000012  I-0.0204822 0.0000037  0.5268 0.0036  I  -107.940    0.618    -8.310    0.078 -0.038102  0.368994 -0.0204875  -107.908    -8.371  
+23 320 60023.00 I -0.036912 0.000009  0.371252 0.000008  I-0.0211492 0.0000036  0.7737 0.0026  I  -107.779    0.618    -8.120    0.078 -0.036907  0.371284 -0.0211416  -107.809    -8.185  
+23 321 60024.00 I -0.035479 0.000009  0.373933 0.000008  I-0.0219996 0.0000036  0.9304 0.0029  I  -107.712    0.618    -7.950    0.078 -0.035480  0.373974 -0.0220007  -107.798    -8.018  
+23 322 60025.00 I -0.033921 0.000012  0.377070 0.000012  I-0.0229704 0.0000045  0.9682 0.0029  I  -107.716    0.707    -7.910    0.051 -0.033918  0.377072 -0.0229616  -107.800    -7.977  
+23 323 60026.00 I -0.032493 0.000012  0.380217 0.000013  I-0.0238905 0.0000046  0.8695 0.0033  I  -107.807    0.707    -7.941    0.051 -0.032503  0.380245 -0.0238876  -107.871    -8.006  
+23 324 60027.00 I -0.031182 0.000011  0.383297 0.000013  I-0.0246830 0.0000047  0.6915 0.0036  I  -108.031    0.707    -7.964    0.051 -0.031173  0.383274 -0.0246908  -108.068    -8.026  
+23 325 60028.00 I -0.029863 0.000009  0.386398 0.000013  I-0.0252284 0.0000056  0.3780 0.0033  I  -108.330    0.760    -8.025    0.019 -0.029863  0.386430 -0.0252241  -108.334    -8.069  
+23 326 60029.00 I -0.028394 0.000014  0.389489 0.000018  I-0.0254385 0.0000045  0.0630 0.0036  I  -108.541    0.803    -8.203    0.111 -0.028402  0.389466 -0.0254315  -108.511    -8.224  
+23 327 60030.00 I -0.026607 0.000014  0.392602 0.000018  I-0.0253934 0.0000045 -0.1349 0.0035  I  -108.574    0.803    -8.444    0.111 -0.026589  0.392633 -0.0253926  -108.515    -8.443  
+23 328 60031.00 I -0.024709 0.000013  0.395453 0.000016  I-0.0251879 0.0000053 -0.2753 0.0033  I  -108.463    0.855    -8.599    0.160 -0.024718  0.395445 -0.0251809  -108.385    -8.580  
+23 329 60032.00 I -0.023045 0.000016  0.397855 0.000020  I-0.0248767 0.0000048 -0.3142 0.0037  I  -108.233    0.748    -8.618    0.111 -0.023029  0.397858 -0.0248761  -108.184    -8.619  
+23 330 60033.00 I -0.021724 0.000019  0.400028 0.000021  I-0.0245951 0.0000052 -0.2463 0.0040  I  -107.843    0.748    -8.610    0.111 -0.021735  0.400017 -0.0245819  -107.840    -8.642  
+23 331 60034.00 I -0.020386 0.000020  0.402185 0.000021  I-0.0243993 0.0000065 -0.1327 0.0049  I  -107.336    0.748    -8.699    0.111 -0.020397  0.402194 -0.0243867  -107.382    -8.762  
+23 4 1 60035.00 I -0.018859 0.000018  0.404604 0.000018  I-0.0243386 0.0000084  0.0077 0.0051  I  -106.908    0.681    -8.855    0.021 -0.018832  0.404562 -0.0243447  -106.941    -8.931  
+23 4 2 60036.00 I -0.017328 0.000019  0.407371 0.000020  I-0.0244341 0.0000079  0.2064 0.0056  I  -106.750    0.752    -8.923    0.064                                                     
+23 4 3 60037.00 I -0.015623 0.000019  0.409983 0.000020  I-0.0247500 0.0000073  0.4008 0.0054  I  -106.855    0.752    -8.803    0.064                                                     
+23 4 4 60038.00 I -0.013827 0.000019  0.412632 0.000021  I-0.0252207 0.0000074  0.5500 0.0050  I  -107.057    0.771    -8.566    0.092                                                     
+23 4 5 60039.00 I -0.012262 0.000015  0.415451 0.000020  I-0.0258397 0.0000069  0.6681 0.0043  I  -107.233    0.771    -8.385    0.092                                                     
+23 4 6 60040.00 I -0.010696 0.000015  0.418305 0.000019  I-0.0265275 0.0000042  0.6979 0.0039  I  -107.374    0.771    -8.368    0.092                                                     
+23 4 7 60041.00 I -0.009135 0.000015  0.421176 0.000019  I-0.0272228 0.0000038  0.6896 0.0028  I  -107.513    0.771    -8.489    0.092                                                     
+23 4 8 60042.00 I -0.007829 0.000014  0.423801 0.000016  I-0.0278873 0.0000038  0.6233 0.0032  I  -107.651    0.631    -8.645    0.081                                                     
+23 4 9 60043.00 I -0.006568 0.000015  0.426292 0.000016  I-0.0284442 0.0000051  0.4816 0.0051  I  -107.765    0.631    -8.768    0.081                                                     
+23 410 60044.00 I -0.005306 0.000014  0.428799 0.000022  I-0.0288335 0.0000095  0.2890 0.0050  I  -107.835    0.807    -8.865    0.052                                                     
+23 411 60045.00 I -0.004033 0.000013  0.431389 0.000023  I-0.0290185 0.0000087  0.0855 0.0054  I  -107.809    0.807    -8.979    0.052                                                     
+23 412 60046.00 I -0.002967 0.000014  0.434147 0.000023  I-0.0290317 0.0000052 -0.0363 0.0051  I  -107.600    0.817    -9.129    0.025                                                     
+23 413 60047.00 I -0.002355 0.000016  0.436717 0.000023  I-0.0289846 0.0000052 -0.0420 0.0036  I  -107.173    0.817    -9.290    0.025                                                     
+23 414 60048.00 I -0.001837 0.000018  0.439279 0.000023  I-0.0290006 0.0000051  0.1109 0.0038  I  -106.645    0.817    -9.405    0.025                                                     
+23 415 60049.00 I -0.001123 0.000017  0.441663 0.000023  I-0.0292399 0.0000056  0.3642 0.0040  I  -106.236    0.817    -9.416    0.025                                                     
+23 416 60050.00 I  0.000178 0.000017  0.443568 0.000011  I-0.0297577 0.0000061  0.7036 0.0041  I  -106.114    0.706    -9.310    0.025                                                     
+23 417 60051.00 I  0.001667 0.000017  0.445287 0.000010  I-0.0306176 0.0000060  0.9544 0.0048  I  -106.268    0.706    -9.137    0.025                                                     
+23 418 60052.00 I  0.002963 0.000016  0.446945 0.000009  I-0.0315944 0.0000075  0.9890 0.0043  I  -106.537    0.636    -8.986    0.029                                                     
+23 419 60053.00 I  0.004293 0.000012  0.448612 0.000011  I-0.0325548 0.0000061  0.9014 0.0049  I  -106.755    0.648    -8.906    0.033                                                     
+23 420 60054.00 I  0.005752 0.000008  0.450447 0.000010  I-0.0333636 0.0000064  0.7132 0.0048  I  -106.883    0.648    -8.893    0.033                                                     
+23 421 60055.00 I  0.007427 0.000008  0.452616 0.000010  I-0.0339540 0.0000074  0.4436 0.0053  I  -106.985    0.648    -8.930    0.033                                                     
+23 422 60056.00 I  0.009104 0.000007  0.455126 0.000009  I-0.0342557 0.0000084  0.1889 0.0050  I  -107.111    0.705    -9.030    0.046                                                     
+23 423 60057.00 I  0.010719 0.000008  0.457863 0.000020  I-0.0343538 0.0000066  0.0004 0.0053  I  -107.231    0.848    -9.193    0.061                                                     
+23 424 60058.00 I  0.012629 0.000009  0.460581 0.000020  I-0.0342653 0.0000066 -0.1617 0.0053  I  -107.279    0.848    -9.355    0.061                                                     
+23 425 60059.00 I  0.014953 0.000010  0.462939 0.000019  I-0.0340606 0.0000084 -0.2332 0.0050  I  -107.218    0.870    -9.438    0.064                                                     
+23 426 60060.00 I  0.017319 0.000011  0.465022 0.000028  I-0.0338247 0.0000074 -0.2272 0.0055  I  -107.027    0.870    -9.449    0.064                                                     
+23 427 60061.00 I  0.019407 0.000011  0.467120 0.000029  I-0.0336194 0.0000072 -0.1817 0.0054  I  -106.690    0.870    -9.491    0.064                                                     
+23 428 60062.00 I  0.021468 0.000012  0.469075 0.000029  I-0.0334895 0.0000079 -0.0516 0.0062  I  -106.238    0.870    -9.638    0.064                                                     
+23 429 60063.00 I  0.023801 0.000011  0.470664 0.000023  I-0.0335369 0.0000101  0.1406 0.0069  I  -105.810    0.322    -9.835    0.160                                                     
+23 430 60064.00 I  0.025989 0.000011  0.472096 0.000023  I-0.0337777 0.0000113  0.3537 0.0072  I  -105.602    0.322    -9.927    0.160                                                     
+23 5 1 60065.00 I  0.027591 0.000011  0.473437 0.000023  I-0.0342371 0.0000102  0.5453 0.0086  I  -105.722    1.020    -9.816    0.099                                                     
+23 5 2 60066.00 I  0.028835 0.000009  0.474635 0.000008  I-0.0348282 0.0000129  0.6168 0.0070  I  -106.090    1.020    -9.558    0.099                                                     
+23 5 3 60067.00 I  0.030235 0.000008  0.475652 0.000009  I-0.0354586 0.0000097  0.6520 0.0079  I  -106.505    1.002    -9.304    0.075                                                     
+23 5 4 60068.00 I  0.031949 0.000009  0.476564 0.000008  I-0.0361380 0.0000091  0.7045 0.0067  I  -106.806    1.002    -9.179    0.075                                                     
+23 5 5 60069.00 I  0.033799 0.000009  0.477610 0.000008  I-0.0368130 0.0000093  0.5930 0.0063  I  -106.984    1.002    -9.215    0.075                                                     
+23 5 6 60070.00 I  0.035739 0.000010  0.478665 0.000009  I-0.0373242 0.0000087  0.4821 0.0065  I  -107.130    1.002    -9.371    0.075                                                     
+23 5 7 60071.00 I  0.037826 0.000011  0.479811 0.000010  I-0.0377573 0.0000090  0.3116 0.0063  I  -107.294    1.083    -9.592    0.152                                                     
+23 5 8 60072.00 I  0.039827 0.000012  0.481232 0.000012  I-0.0379487 0.0000091  0.1449 0.0073  I  -107.402    1.083    -9.822    0.152                                                     
+23 5 9 60073.00 I  0.041741 0.000012  0.482739 0.000011  I-0.0380824 0.0000114  0.0841 0.0074  I  -107.322    1.217   -10.018    0.224                                                     
+23 510 60074.00 I  0.043535 0.000011  0.484271 0.000011  I-0.0381415 0.0000117  0.0973 0.0075  P  -107.062    0.278   -10.129    0.145                                                     
+23 511 60075.00 I  0.045319 0.000012  0.485528 0.000010  I-0.0383566 0.0000097  0.3494 0.0072  P  -106.694    0.288   -10.149    0.148                                                     
+23 512 60076.00 I  0.047270 0.000078  0.486614 0.000078  I-0.0388331 0.0000083  0.5800 0.0067  P  -106.353    0.297   -10.099    0.151                                                     
+23 513 60077.00 I  0.049465 0.000078  0.487754 0.000078  I-0.0395258 0.0000092  0.8384 0.0061  P  -106.154    0.304    -9.996    0.154                                                     
+23 514 60078.00 I  0.052355 0.000085  0.489080 0.000085  I-0.0405252 0.0000090  1.1428 0.0061  P  -106.156    0.309    -9.850    0.155                                                     
+23 515 60079.00 I  0.055823 0.000091  0.490647 0.000091  I-0.0417656 0.0000079  1.3097 0.0059  P  -106.350    0.313    -9.671    0.157                                                     
+23 516 60080.00 I  0.059182 0.000091  0.492199 0.000091  I-0.0430864 0.0000075  1.3020 0.0057  P  -106.668    0.316    -9.471    0.158                                                     
+23 517 60081.00 I  0.062075 0.000091  0.493471 0.000091  I-0.0443097 0.0000083  1.1147 0.0058  P  -106.997    0.318    -9.275    0.158                                                     
+23 518 60082.00 I  0.064538 0.000091  0.494606 0.000091  I-0.0452777 0.0000088  0.8132 0.0055  P  -107.225    0.319    -9.138    0.159                                                     
+23 519 60083.00 I  0.066905 0.000091  0.495692 0.000090  I-0.0459284 0.0000073  0.4887 0.0059  P  -107.311    0.320    -9.131    0.159                                                     
+23 520 60084.00 I  0.069347 0.000091  0.496656 0.000091  I-0.0462757 0.0000078  0.2262 0.0058  P  -107.316    0.321    -9.280    0.160                                                     
+23 521 60085.00 I  0.071616 0.000091  0.497496 0.000091  I-0.0463859 0.0000089 -0.0208 0.0056  P  -107.343    0.321    -9.519    0.160                                                     
+23 522 60086.00 I  0.073729 0.000091  0.498189 0.000091  I-0.0462453 0.0000080 -0.2342 0.0059  P  -107.430    0.321    -9.717    0.160                                                     
+23 523 60087.00 I  0.076210 0.000091  0.498997 0.000091  I-0.0459641 0.0000076 -0.3077 0.0057  P  -107.527    0.321    -9.787    0.160                                                     
+23 524 60088.00 I  0.079152 0.000091  0.499991 0.000091  I-0.0456633 0.0000082 -0.2810 0.0058  P  -107.563    0.322    -9.775    0.160                                                     
+23 525 60089.00 I  0.082204 0.000090  0.501136 0.000091  I-0.0453859 0.0000087                 P  -107.495    0.322    -9.803    0.160                                                     
+23 526 60090.00 P  0.085155 0.000600  0.502166 0.000425  P-0.0451659 0.0001080                 P  -107.303    0.322    -9.923    0.160                                                     
+23 527 60091.00 P  0.088012 0.000891  0.503223 0.000700  P-0.0450616 0.0002041                 P  -107.011    0.322   -10.046    0.160                                                     
+23 528 60092.00 P  0.090860 0.001123  0.504149 0.000937  P-0.0451160 0.0003028                 P  -106.759    0.322   -10.030    0.160                                                     
+23 529 60093.00 P  0.093670 0.001323  0.504928 0.001153  P-0.0453306 0.0004021                 P  -106.781    0.322    -9.835    0.160                                                     
+23 530 60094.00 P  0.096449 0.001503  0.505583 0.001353  P-0.0456505 0.0005017                 P  -107.208    0.322    -9.554    0.160                                                     
+23 531 60095.00 P  0.099209 0.001667  0.506139 0.001543  P-0.0459875 0.0006014                 P  -107.886    0.322    -9.311    0.160                                                     
+23 6 1 60096.00 P  0.101978 0.001820  0.506625 0.001724  P-0.0462601 0.0007012                 P  -108.495    0.322    -9.154    0.160                                                     
+23 6 2 60097.00 P  0.104748 0.001964  0.507064 0.001899  P-0.0463965 0.0007500                 P  -108.875    0.322    -9.087    0.160                                                     
+23 6 3 60098.00 P  0.107500 0.002101  0.507466 0.002067  P-0.0463276 0.0005500                 P  -109.132    0.322    -9.144    0.160                                                     
+23 6 4 60099.00 P  0.110246 0.002231  0.507839 0.002229  P-0.0460431 0.0007548                 P  -109.380    0.322    -9.362    0.160                                                     
+23 6 5 60100.00 P  0.113002 0.002355  0.508160 0.002388  P-0.0455705 0.0009344                 P  -109.511    0.322    -9.664    0.160                                                     
+23 6 6 60101.00 P  0.115784 0.002475  0.508426 0.002542  P-0.0449965 0.0010994                 P  -109.358    0.322    -9.877    0.160                                                     
+23 6 7 60102.00 P  0.118582 0.002591  0.508655 0.002693  P-0.0444818 0.0012543                 P  -108.978    0.322    -9.889    0.160                                                     
+23 6 8 60103.00 P  0.121388 0.002702  0.508854 0.002841  P-0.0441560 0.0014016                 P  -108.642    0.322    -9.757    0.160                                                     
+23 6 9 60104.00 P  0.124195 0.002811  0.509021 0.002985  P-0.0441055 0.0015429                 P  -108.550    0.322    -9.609    0.160                                                     
+23 610 60105.00 P  0.126995 0.002916  0.509146 0.003127  P-0.0443337 0.0016792                 P  -108.661    0.322    -9.508    0.160                                                     
+23 611 60106.00 P  0.129785 0.003019  0.509226 0.003267  P-0.0447922 0.0018113                 P  -108.809    0.322    -9.425    0.160                                                     
+23 612 60107.00 P  0.132563 0.003119  0.509259 0.003404  P-0.0453632 0.0019399                 P  -108.920    0.322    -9.315    0.160                                                     
+23 613 60108.00 P  0.135334 0.003216  0.509241 0.003539  P-0.0458976 0.0020652                 P  -109.070    0.322    -9.157    0.160                                                     
+23 614 60109.00 P  0.138099 0.003312  0.509174 0.003672  P-0.0462685 0.0021877                 P  -109.341    0.322    -8.969    0.160                                                     
+23 615 60110.00 P  0.140863 0.003405  0.509058 0.003804  P-0.0463849 0.0023077                 P  -109.673    0.322    -8.825    0.160                                                     
+23 616 60111.00 P  0.143624 0.003496  0.508900 0.003933  P-0.0462053 0.0024255                 P  -109.909    0.322    -8.839    0.160                                                     
+23 617 60112.00 P  0.146381 0.003586  0.508700 0.004061  P-0.0457351 0.0025411                 P  -109.979    0.322    -9.074    0.160                                                     
+23 618 60113.00 P  0.149132 0.003674  0.508458 0.004187  P-0.0450274 0.0026548                 P  -109.974    0.322    -9.447    0.160                                                     
+23 619 60114.00 P  0.151877 0.003761  0.508173 0.004312  P-0.0441691 0.0027668                 P  -110.025    0.322    -9.753    0.160                                                     
+23 620 60115.00 P  0.154615 0.003846  0.507847 0.004436  P-0.0432430 0.0028772                 P  -110.165    0.322    -9.831    0.160                                                     
+23 621 60116.00 P  0.157344 0.003929  0.507479 0.004558  P-0.0423298 0.0029860                 P  -110.343    0.322    -9.712    0.160                                                     
+23 622 60117.00 P  0.160066 0.004012  0.507070 0.004679  P-0.0414937 0.0030934                 P  -110.499    0.322    -9.571    0.160                                                     
+23 623 60118.00 P  0.162777 0.004093  0.506621 0.004799  P-0.0407731 0.0031995                 P  -110.557    0.322    -9.521    0.160                                                     
+23 624 60119.00 P  0.165477 0.004173  0.506130 0.004917  P-0.0401827 0.0033043                 P  -110.442    0.322    -9.496    0.160                                                     
+23 625 60120.00 P  0.168165 0.004251  0.505599 0.005035  P-0.0397207 0.0034080                 P  -110.208    0.322    -9.370    0.160                                                     
+23 626 60121.00 P  0.170841 0.004329  0.505027 0.005151  P-0.0393635 0.0035105                 P  -110.142    0.322    -9.142    0.160                                                     
+23 627 60122.00 P  0.173503 0.004406  0.504414 0.005266  P-0.0390569 0.0036120                 P  -110.555    0.322    -8.958    0.160                                                     
+23 628 60123.00 P  0.176151 0.004481  0.503760 0.005381  P-0.0387358 0.0037124                 P  -111.413    0.322    -8.925    0.160                                                     
+23 629 60124.00 P  0.178786 0.004556  0.503066 0.005494  P-0.0383258 0.0038119                 P  -112.302    0.322    -8.980    0.160                                                     
+23 630 60125.00 P  0.181406 0.004630  0.502331 0.005607  P-0.0377456 0.0039105                 P  -112.871    0.322    -9.003    0.160                                                     
+23 7 1 60126.00 P  0.184011 0.004702  0.501557 0.005719  P-0.0369353 0.0040082                 P  -113.141    0.322    -9.026    0.160                                                     
+23 7 2 60127.00 P  0.186600 0.004774  0.500744 0.005830  P-0.0358970 0.0041051                 P  -113.269    0.322    -9.183    0.160                                                     
+23 7 3 60128.00 P  0.189172 0.004846  0.499891 0.005940  P-0.0347046 0.0042012                 P  -113.215    0.322    -9.455    0.160                                                     
+23 7 4 60129.00 P  0.191728 0.004916  0.499000 0.006049  P-0.0334883 0.0042965                 P  -112.895    0.322    -9.621    0.160                                                     
+23 7 5 60130.00 P  0.194265 0.004986  0.498071 0.006157  P-0.0323935 0.0043911                 P  -112.498    0.322    -9.531    0.160                                                     
+23 7 6 60131.00 P  0.196783 0.005055  0.497104 0.006265  P-0.0315298 0.0044849                 P  -112.373    0.322    -9.315    0.160                                                     
+23 7 7 60132.00 P  0.199283 0.005123  0.496099 0.006372  P-0.0309329 0.0045781                 P  -112.639    0.322    -9.189    0.160                                                     
+23 7 8 60133.00 P  0.201762 0.005191  0.495057 0.006479  P-0.0305522 0.0046706                 P  -113.093    0.322    -9.180    0.160                                                     
+23 7 9 60134.00 P  0.204220 0.005257  0.493978 0.006584  P-0.0302712 0.0047625                 P  -113.469    0.322    -9.160    0.160                                                     
+23 710 60135.00 P  0.206657 0.005324  0.492861 0.006689  P-0.0299560 0.0048537                 P  -113.667    0.322    -9.067    0.160                                                     
+23 711 60136.00 P  0.209073 0.005389  0.491709 0.006794  P-0.0294878 0.0049444                 P  -113.773    0.322    -8.960    0.160                                                     
+23 712 60137.00 P  0.211466 0.005454  0.490520 0.006897  P-0.0287941 0.0050344                 P  -113.944    0.322    -8.895    0.160                                                     
+23 713 60138.00 P  0.213836 0.005519  0.489296 0.007001  P-0.0278502 0.0051240                 P  -114.248    0.322    -8.882    0.160                                                     
+23 714 60139.00 P  0.216182 0.005583  0.488036 0.007103  P-0.0266720 0.0052129                 P  -114.580    0.322    -8.957    0.160                                                     
+23 715 60140.00 P  0.218504 0.005646  0.486741 0.007205  P-0.0253091 0.0053014                 P  -114.778    0.322    -9.185    0.160                                                     
+23 716 60141.00 P  0.220801 0.005709  0.485412 0.007307  P-0.0238318 0.0053893                 P  -114.805    0.322    -9.539    0.160                                                     
+23 717 60142.00 P  0.223073 0.005771  0.484049 0.007407  P-0.0223181 0.0054768                 P  -114.769    0.322    -9.835    0.160                                                     
+23 718 60143.00 P  0.225319 0.005833  0.482652 0.007508  P-0.0208438 0.0055637                 P  -114.780    0.322    -9.860    0.160                                                     
+23 719 60144.00 P  0.227539 0.005895  0.481221 0.007608  P-0.0194768 0.0056502                 P  -114.868    0.322    -9.592    0.160                                                     
+23 720 60145.00 P  0.229731 0.005955  0.479758 0.007707  P-0.0182612 0.0057362                 P  -114.997    0.322    -9.234    0.160                                                     
+23 721 60146.00 P  0.231896 0.006016  0.478263 0.007806  P-0.0172204 0.0058218                 P  -115.088    0.322    -9.000    0.160                                                     
+23 722 60147.00 P  0.234033 0.006076  0.476735 0.007904  P-0.0163450 0.0059070                 P  -115.044    0.322    -8.900    0.160                                                     
+23 723 60148.00 P  0.236141 0.006135  0.475176 0.008002  P-0.0156023 0.0059917                 P  -114.862    0.322    -8.810    0.160                                                     
+23 724 60149.00 P  0.238220 0.006194  0.473586 0.008100  P-0.0149420 0.0060760                 P  -114.767    0.322    -8.696    0.160                                                     
+23 725 60150.00 P  0.240269 0.006253  0.471965 0.008196  P-0.0142998 0.0061599                 P  -115.089    0.322    -8.689    0.160                                                     
+23 726 60151.00 P  0.242288 0.006311  0.470315 0.008293  P-0.0136072 0.0062434                 P  -115.896    0.322    -8.893    0.160                                                     
+23 727 60152.00 P  0.244276 0.006369  0.468634 0.008389  P-0.0127952 0.0063266                 P  -116.815    0.322    -9.198    0.160                                                     
+23 728 60153.00 P  0.246234 0.006426  0.466925 0.008485  P-0.0118082 0.0064093                 P  -117.397    0.322    -9.388    0.160                                                     
+23 729 60154.00 P  0.248159 0.006483  0.465186 0.008580  P-0.0106248 0.0064917                 P  -117.541    0.322    -9.415    0.160                                                     
+23 730 60155.00 P  0.250053 0.006540  0.463420 0.008675  P-0.0092847 0.0065737                 P  -117.407    0.322    -9.437    0.160                                                     
+23 731 60156.00 P  0.251914 0.006596  0.461626 0.008769  P-0.0078962 0.0066554                 P  -117.087    0.322    -9.517    0.160                                                     
+23 8 1 60157.00 P  0.253742 0.006652  0.459805 0.008863  P-0.0066047 0.0067368                 P  -116.655    0.322    -9.495    0.160                                                     
+23 8 2 60158.00 P  0.255536 0.006708  0.457957 0.008957  P-0.0055502 0.0068177                 P  -116.381    0.322    -9.271    0.160                                                     
+23 8 3 60159.00 P  0.257297 0.006763  0.456084 0.009050  P-0.0048119 0.0068984                 P  -116.529    0.322    -9.050    0.160                                                     
+23 8 4 60160.00 P  0.259023 0.006818  0.454184 0.009143  P-0.0043697 0.0069788                 P  -116.999    0.322    -9.083    0.160                                                     
+23 8 5 60161.00 P  0.260715 0.006873  0.452260 0.009236  P-0.0041135 0.0070588                 P  -117.463    0.322    -9.288    0.160                                                     
+23 8 6 60162.00 P  0.262372 0.006927  0.450311 0.009328  P-0.0038862 0.0071385                 P  -117.772    0.322    -9.368    0.160                                                     
+23 8 7 60163.00 P  0.263993 0.006981  0.448339 0.009420  P-0.0035333 0.0072179                 P  -117.998    0.322    -9.238    0.160                                                     
+23 8 8 60164.00 P  0.265578 0.007034  0.446343 0.009511  P-0.0029525 0.0072970                                                                                                             
+23 8 9 60165.00 P  0.267127 0.007088  0.444324 0.009602  P-0.0021044 0.0073758                                                                                                             
+23 810 60166.00 P  0.268640 0.007141  0.442284 0.009693  P-0.0010050 0.0074544                                                                                                             
+23 811 60167.00 P  0.270116 0.007194  0.440221 0.009784  P 0.0002908 0.0075326                                                                                                             
+23 812 60168.00 P  0.271554 0.007246  0.438138 0.009874  P 0.0017052 0.0076106                                                                                                             
+23 813 60169.00 P  0.272955 0.007298  0.436034 0.009964  P 0.0031524 0.0076883                                                                                                             
+23 814 60170.00 P  0.274318 0.007350  0.433911 0.010053  P 0.0045542 0.0077657                                                                                                             
+23 815 60171.00 P  0.275643 0.007402  0.431768 0.010142  P 0.0058435 0.0078428                                                                                                             
+23 816 60172.00 P  0.276929 0.007453  0.429606 0.010231  P 0.0069708 0.0079197                                                                                                             
+23 817 60173.00 P  0.278176 0.007504  0.427427 0.010320  P 0.0079089 0.0079964                                                                                                             
+23 818 60174.00 P  0.279385 0.007555  0.425230 0.010408  P 0.0086579 0.0080728                                                                                                             
+23 819 60175.00 P  0.280554 0.007605  0.423016 0.010496  P 0.0092455 0.0081489                                                                                                             
+23 820 60176.00 P  0.281683 0.007655  0.420786 0.010584  P 0.0097206 0.0082248                                                                                                             
+23 821 60177.00 P  0.282773 0.007706  0.418540 0.010671  P 0.0101495 0.0083005                                                                                                             
+23 822 60178.00 P  0.283822 0.007755  0.416280 0.010758  P 0.0106035 0.0083759                                                                                                             
+23 823 60179.00 P  0.284832 0.007805  0.414005 0.010845  P 0.0111499 0.0084511                                                                                                             
+23 824 60180.00 P  0.285801 0.007854  0.411717 0.010932  P 0.0118454 0.0085261                                                                                                             
+23 825 60181.00 P  0.286729 0.007903  0.409415 0.011018  P 0.0127140 0.0086008                                                                                                             
+23 826 60182.00 P  0.287616 0.007952  0.407101 0.011104  P 0.0137348 0.0086754                                                                                                             
+23 827 60183.00 P  0.288463 0.008001  0.404775 0.011190  P 0.0148302 0.0087497                                                                                                             
+23 828 60184.00 P  0.289268 0.008049  0.402438 0.011276  P 0.0158715 0.0088237                                                                                                             
+23 829 60185.00 P  0.290032 0.008097  0.400091 0.011361  P 0.0167113 0.0088976                                                                                                             
+23 830 60186.00 P  0.290754 0.008145  0.397733 0.011446  P 0.0172335 0.0089713                                                                                                             
+23 831 60187.00 P  0.291435 0.008193  0.395367 0.011531  P 0.0174028 0.0090448                                                                                                             
+23 9 1 60188.00 P  0.292074 0.008241  0.392992 0.011616  P 0.0172856 0.0091180                                                                                                             
+23 9 2 60189.00 P  0.292671 0.008288  0.390609 0.011700  P 0.0170311 0.0091911                                                                                                             
+23 9 3 60190.00 P  0.293227 0.008335  0.388218 0.011784  P 0.0168190 0.0092639                                                                                                             
+23 9 4 60191.00 P  0.293741 0.008382  0.385820 0.011868  P 0.0167994 0.0093366                                                                                                             
+23 9 5 60192.00 P  0.294212 0.008429  0.383416 0.011952  P 0.0170533 0.0094091                                                                                                             
+23 9 6 60193.00 P  0.294642 0.008475  0.381006 0.012035  P 0.0175863 0.0094814                                                                                                             
+23 9 7 60194.00 P  0.295029 0.008522  0.378592 0.012118  P 0.0183467 0.0095535                                                                                                             
+23 9 8 60195.00 P  0.295374 0.008568  0.376173 0.012201  P 0.0192522 0.0096254                                                                                                             
+23 9 9 60196.00 P  0.295677 0.008614  0.373751 0.012284  P 0.0202126 0.0096971                                                                                                             
+23 910 60197.00 P  0.295937 0.008660  0.371327 0.012367  P 0.0211439 0.0097686                                                                                                             
+23 911 60198.00 P  0.296156 0.008705  0.368900 0.012449  P 0.0219150 0.0098400                                                                                                             
+23 912 60199.00 P  0.296332 0.008751  0.366472 0.012531  P 0.0225329 0.0099112                                                                                                             
+23 913 60200.00 P  0.296466 0.008796  0.364044 0.012613  P 0.0229642 0.0099822                                                                                                             
+23 914 60201.00 P  0.296558 0.008841  0.361615 0.012695  P 0.0232020 0.0100531                                                                                                             
+23 915 60202.00 P  0.296607 0.008886  0.359187 0.012776  P 0.0232670 0.0101238                                                                                                             
+23 916 60203.00 P  0.296615 0.008931  0.356760 0.012858  P 0.0232069 0.0101943                                                                                                             
+23 917 60204.00 P  0.296580 0.008975  0.354335 0.012939  P 0.0230886 0.0102646                                                                                                             
+23 918 60205.00 P  0.296504 0.009020  0.351912 0.013020  P 0.0229880 0.0103348                                                                                                             
+23 919 60206.00 P  0.296386 0.009064  0.349493 0.013100  P 0.0229779 0.0104048                                                                                                             
+23 920 60207.00 P  0.296226 0.009108  0.347077 0.013181  P 0.0231143 0.0104747                                                                                                             
+23 921 60208.00 P  0.296024 0.009152  0.344666 0.013261  P 0.0234243 0.0105444                                                                                                             
+23 922 60209.00 P  0.295781 0.009196  0.342259 0.013341  P 0.0238951 0.0106139                                                                                                             
+23 923 60210.00 P  0.295497 0.009239  0.339859 0.013421  P 0.0244665 0.0106833                                                                                                             
+23 924 60211.00 P  0.295171 0.009283  0.337465 0.013501  P 0.0250329 0.0107526                                                                                                             
+23 925 60212.00 P  0.294805 0.009326  0.335078 0.013581  P 0.0254595 0.0108216                                                                                                             
+23 926 60213.00 P  0.294397 0.009369  0.332698 0.013660  P 0.0256189 0.0108906                                                                                                             
+23 927 60214.00 P  0.293949 0.009412  0.330327 0.013739  P 0.0254358 0.0109594                                                                                                             
+23 928 60215.00 P  0.293460 0.009455  0.327964 0.013818  P 0.0249224 0.0110280                                                                                                             
+23 929 60216.00 P  0.292931 0.009498  0.325611 0.013897  P 0.0241841 0.0110965                                                                                                             
+23 930 60217.00 P  0.292361 0.009540  0.323268 0.013976  P 0.0233906 0.0111649                                                                                                             
+2310 1 60218.00 P  0.291752 0.009583  0.320936 0.014055  P 0.0227193 0.0112331                                                                                                             
+2310 2 60219.00 P  0.291104 0.009625  0.318615 0.014133  P 0.0223008 0.0113012                                                                                                             
+2310 3 60220.00 P  0.290415 0.009667  0.316306 0.014211  P 0.0221877 0.0113691                                                                                                             
+2310 4 60221.00 P  0.289688 0.009709  0.314010 0.014289  P 0.0223548 0.0114369                                                                                                             
+2310 5 60222.00 P  0.288922 0.009751  0.311726 0.014367  P 0.0227245 0.0115046                                                                                                             
+2310 6 60223.00 P  0.288117 0.009793  0.309457 0.014445  P 0.0231989 0.0115721                                                                                                             
+2310 7 60224.00 P  0.287274 0.009834  0.307201 0.014522  P 0.0236820 0.0116395                                                                                                             
+2310 8 60225.00 P  0.286393 0.009876  0.304961 0.014600  P 0.0240932 0.0117067                                                                                                             
+2310 9 60226.00 P  0.285474 0.009917  0.302736 0.014677  P 0.0243708 0.0117739                                                                                                             
+231010 60227.00 P  0.284517 0.009958  0.300527 0.014754  P 0.0244757 0.0118409                                                                                                             
+231011 60228.00 P  0.283524 0.009999  0.298335 0.014831  P 0.0243937 0.0119077                                                                                                             
+231012 60229.00 P  0.282494 0.010040  0.296160 0.014907  P 0.0241374 0.0119745                                                                                                             
+231013 60230.00 P  0.281427 0.010081  0.294002 0.014984  P 0.0237462 0.0120411                                                                                                             
+231014 60231.00 P  0.280324 0.010122  0.291863 0.015060  P 0.0232821 0.0121076                                                                                                             
+231015 60232.00 P  0.279186 0.010162  0.289743 0.015137  P 0.0228220 0.0121740                                                                                                             
+231016 60233.00 P  0.278012 0.010203  0.287642 0.015213  P 0.0224461 0.0122402                                                                                                             
+231017 60234.00 P  0.276804 0.010243  0.285561 0.015289  P 0.0222224 0.0123063                                                                                                             
+231018 60235.00 P  0.275560 0.010283  0.283500 0.015365  P 0.0221897 0.0123723                                                                                                             
+231019 60236.00 P  0.274283 0.010323  0.281460 0.015440  P 0.0223440 0.0124382                                                                                                             
+231020 60237.00 P  0.272972 0.010363  0.279442 0.015516  P 0.0226325 0.0125040                                                                                                             
+231021 60238.00 P  0.271627 0.010403  0.277446 0.015591  P 0.0229593 0.0125696                                                                                                             
+231022 60239.00 P  0.270250 0.010443  0.275472 0.015667  P 0.0232019 0.0126352                                                                                                             
+231023 60240.00 P  0.268840 0.010482  0.273521 0.015742  P 0.0232385 0.0127006                                                                                                             
+231024 60241.00 P  0.267398 0.010522  0.271594 0.015817  P 0.0229825 0.0127659                                                                                                             
+231025 60242.00 P  0.265925 0.010561  0.269690 0.015892  P 0.0224115 0.0128311                                                                                                             
+231026 60243.00 P  0.264420 0.010601  0.267811 0.015966  P 0.0215848 0.0128962                                                                                                             
+231027 60244.00 P  0.262885 0.010640  0.265957 0.016041  P 0.0206336 0.0129612                                                                                                             
+231028 60245.00 P  0.261320 0.010679  0.264128 0.016115  P 0.0197243 0.0130260                                                                                                             
+231029 60246.00 P  0.259725 0.010718  0.262325 0.016190  P 0.0190088 0.0130908                                                                                                             
+231030 60247.00 P  0.258101 0.010757  0.260548 0.016264  P 0.0185810 0.0131554                                                                                                             
+231031 60248.00 P  0.256448 0.010796  0.258798 0.016338  P 0.0184575 0.0132199                                                                                                             
+2311 1 60249.00 P  0.254766 0.010834  0.257075 0.016412  P 0.0185871 0.0132844                                                                                                             
+2311 2 60250.00 P  0.253057 0.010873  0.255379 0.016486  P 0.0188782 0.0133487                                                                                                             
+2311 3 60251.00 P  0.251321 0.010911  0.253712 0.016559  P 0.0192290 0.0134129                                                                                                             
+2311 4 60252.00 P  0.249559 0.010950  0.252072 0.016633  P 0.0195486 0.0134770                                                                                                             
+2311 5 60253.00 P  0.247770 0.010988  0.250461 0.016706  P 0.0197656 0.0135410                                                                                                             
+2311 6 60254.00 P  0.245955 0.011026  0.248880 0.016780  P 0.0198328 0.0136050                                                                                                             
+2311 7 60255.00 P  0.244116 0.011064  0.247328 0.016853  P 0.0197287 0.0136688                                                                                                             
+2311 8 60256.00 P  0.242252 0.011102  0.245806 0.016926  P 0.0194573 0.0137325                                                                                                             
+2311 9 60257.00 P  0.240364 0.011140  0.244314 0.016999  P 0.0190488 0.0137961                                                                                                             
+231110 60258.00 P  0.238453 0.011177  0.242852 0.017071  P 0.0185552 0.0138596                                                                                                             
+231111 60259.00 P  0.236518 0.011215  0.241421 0.017144  P 0.0180464 0.0139230                                                                                                             
+231112 60260.00 P  0.234562 0.011253  0.240022 0.017217  P 0.0176014 0.0139863                                                                                                             
+231113 60261.00 P  0.232584 0.011290  0.238654 0.017289  P 0.0172966 0.0140495                                                                                                             
+231114 60262.00 P  0.230585 0.011327  0.237318 0.017361  P 0.0171866 0.0141127                                                                                                             
+231115 60263.00 P  0.228565 0.011365  0.236015 0.017434  P 0.0172852 0.0141757                                                                                                             
+231116 60264.00 P  0.226526 0.011402  0.234743 0.017506  P 0.0175533 0.0142386                                                                                                             
+231117 60265.00 P  0.224467 0.011439  0.233505 0.017578  P 0.0179020 0.0143014                                                                                                             
+231118 60266.00 P  0.222390 0.011476  0.232299 0.017649  P 0.0182108 0.0143642                                                                                                             
+231119 60267.00 P  0.220294 0.011513  0.231127 0.017721  P 0.0183597 0.0144268                                                                                                             
+231120 60268.00 P  0.218181 0.011550  0.229988 0.017793  P 0.0182614 0.0144894                                                                                                             
+231121 60269.00 P  0.216051 0.011587  0.228883 0.017864  P 0.0178862 0.0145519                                                                                                             
+231122 60270.00 P  0.213905 0.011623  0.227813 0.017936  P 0.0172734 0.0146142                                                                                                             
+231123 60271.00 P  0.211743 0.011660  0.226776 0.018007  P 0.0165245 0.0146765                                                                                                             
+231124 60272.00 P  0.209567 0.011696  0.225774 0.018078  P 0.0157798 0.0147387                                                                                                             
+231125 60273.00 P  0.207376 0.011733  0.224807 0.018149  P 0.0151820 0.0148008                                                                                                             
+231126 60274.00 P  0.205171 0.011769  0.223874 0.018220  P 0.0148385 0.0148629                                                                                                             
+231127 60275.00 P  0.202953 0.011805  0.222977 0.018291  P 0.0147954 0.0149248                                                                                                             
+231128 60276.00 P  0.200722 0.011841  0.222115 0.018362  P 0.0150318 0.0149867                                                                                                             
+231129 60277.00 P  0.198480 0.011877  0.221288 0.018433  P 0.0154745 0.0150484                                                                                                             
+231130 60278.00 P  0.196227 0.011913  0.220497 0.018503  P 0.0160240 0.0151101                                                                                                             
+2312 1 60279.00 P  0.193963 0.011949  0.219742 0.018573  P 0.0165794 0.0151717                                                                                                             
+2312 2 60280.00 P  0.191689 0.011985  0.219022 0.018644  P 0.0170566 0.0152332                                                                                                             
+2312 3 60281.00 P  0.189406 0.012021  0.218339 0.018714  P 0.0173972 0.0152946                                                                                                             
+2312 4 60282.00 P  0.187114 0.012056  0.217692 0.018784  P 0.0175724 0.0153560                                                                                                             
+2312 5 60283.00 P  0.184814 0.012092  0.217081 0.018854  P 0.0175834 0.0154172                                                                                                             
+2312 6 60284.00 P  0.182507 0.012127  0.216506 0.018924  P 0.0174586 0.0154784                                                                                                             
+2312 7 60285.00 P  0.180194 0.012163  0.215968 0.018994  P 0.0172470 0.0155395                                                                                                             
+2312 8 60286.00 P  0.177874 0.012198  0.215466 0.019064  P 0.0170104 0.0156005                                                                                                             
+2312 9 60287.00 P  0.175549 0.012233  0.215001 0.019133  P 0.0168159 0.0156614                                                                                                             
+231210 60288.00 P  0.173220 0.012269  0.214573 0.019203  P 0.0167287 0.0157223                                                                                                             
+231211 60289.00 P  0.170886 0.012304  0.214181 0.019272  P 0.0168009 0.0157831                                                                                                             
+231212 60290.00 P  0.168549 0.012339  0.213826 0.019342  P 0.0170546 0.0158438                                                                                                             
+231213 60291.00 P  0.166209 0.012374  0.213507 0.019411  P 0.0174652 0.0159044                                                                                                             
+231214 60292.00 P  0.163868 0.012409  0.213226 0.019480  P 0.0179536 0.0159649                                                                                                             
+231215 60293.00 P  0.161524 0.012443  0.212981 0.019549  P 0.0183995 0.0160254                                                                                                             
+231216 60294.00 P  0.159180 0.012478  0.212773 0.019618  P 0.0186751 0.0160858                                                                                                             
+231217 60295.00 P  0.156836 0.012513  0.212602 0.019687  P 0.0186863 0.0161461                                                                                                             
+231218 60296.00 P  0.154493 0.012547  0.212467 0.019756  P 0.0184044 0.0162063                                                                                                             
+231219 60297.00 P  0.152151 0.012582  0.212369 0.019824  P 0.0178740 0.0162665                                                                                                             
+231220 60298.00 P  0.149810 0.012616  0.212308 0.019893  P 0.0171976 0.0163265                                                                                                             
+231221 60299.00 P  0.147472 0.012651  0.212283 0.019961  P 0.0165063 0.0163866                                                                                                             
+231222 60300.00 P  0.145138 0.012685  0.212295 0.020030  P 0.0159272 0.0164465                                                                                                             
+231223 60301.00 P  0.142807 0.012719  0.212344 0.020098  P 0.0155534 0.0165063                                                                                                             
+231224 60302.00 P  0.140480 0.012753  0.212429 0.020166  P 0.0154262 0.0165661                                                                                                             
+231225 60303.00 P  0.138159 0.012787  0.212550 0.020234  P 0.0155333 0.0166258                                                                                                             
+231226 60304.00 P  0.135843 0.012821  0.212707 0.020302  P 0.0158223 0.0166855                                                                                                             
+231227 60305.00 P  0.133534 0.012855  0.212900 0.020370  P 0.0162144 0.0167451                                                                                                             
+231228 60306.00 P  0.131231 0.012889  0.213129 0.020438  P 0.0166167 0.0168046                                                                                                             
+231229 60307.00 P  0.128937 0.012923  0.213394 0.020506  P 0.0169465 0.0168640                                                                                                             
+231230 60308.00 P  0.126650 0.012957  0.213695 0.020574  P 0.0171649 0.0169233                                                                                                             
+231231 60309.00 P  0.124372 0.012991  0.214031 0.020641  P 0.0172859 0.0169826                                                                                                             
+24 1 1 60310.00 P  0.122104 0.013024  0.214403 0.020709  P 0.0173156 0.0170419                                                                                                             
+24 1 2 60311.00 P  0.119846 0.013058  0.214809 0.020776  P 0.0172388 0.0171010                                                                                                             
+24 1 3 60312.00 P  0.117599 0.013091  0.215251 0.020843  P 0.0170490 0.0171601                                                                                                             
+24 1 4 60313.00 P  0.115363 0.013125  0.215727 0.020911  P 0.0167657 0.0172191                                                                                                             
+24 1 5 60314.00 P  0.113139 0.013158  0.216238 0.020978  P 0.0164902 0.0172780                                                                                                             
+24 1 6 60315.00 P  0.110927 0.013191  0.216784 0.021045  P 0.0163037 0.0173369                                                                                                             
+24 1 7 60316.00 P  0.108729 0.013225  0.217364 0.021112  P 0.0161861 0.0173957                                                                                                             
+24 1 8 60317.00 P  0.106544 0.013258  0.217977 0.021179  P 0.0162250 0.0174545                                                                                                             
+24 1 9 60318.00 P  0.104374 0.013291  0.218624 0.021246  P 0.0164393 0.0175131                                                                                                             
+24 110 60319.00 P  0.102218 0.013324  0.219305 0.021313  P 0.0167400 0.0175718                                                                                                             
+24 111 60320.00 P  0.100078 0.013357  0.220019 0.021379  P 0.0171012 0.0176303                                                                                                             
+24 112 60321.00 P  0.097954 0.013390  0.220766 0.021446  P 0.0173851 0.0176888                                                                                                             
+24 113 60322.00 P  0.095847 0.013423  0.221545 0.021512  P 0.0173998 0.0177472                                                                                                             
+24 114 60323.00 P  0.093757 0.013456  0.222357 0.021579  P 0.0170933 0.0178055                                                                                                             
+24 115 60324.00 P  0.091684 0.013488  0.223201 0.021645  P 0.0164798 0.0178638                                                                                                             
+24 116 60325.00 P  0.089630 0.013521  0.224077 0.021711  P 0.0156854 0.0179220                                                                                                             
+24 117 60326.00 P  0.087594 0.013554  0.224984 0.021778  P 0.0149524 0.0179802                                                                                                             
+24 118 60327.00 P  0.085578 0.013586  0.225922 0.021844  P 0.0144053 0.0180383                                                                                                             
+24 119 60328.00 P  0.083582 0.013619  0.226891 0.021910  P 0.0141564 0.0180963                                                                                                             
+24 120 60329.00 P  0.081606 0.013651  0.227891 0.021976  P 0.0142418 0.0181543                                                                                                             
+24 121 60330.00 P  0.079651 0.013683  0.228921 0.022042  P 0.0145770 0.0182122                                                                                                             
+24 122 60331.00 P  0.077717 0.013716  0.229980 0.022107  P 0.0151148 0.0182700                                                                                                             
+24 123 60332.00 P  0.075806 0.013748  0.231069 0.022173  P 0.0157653 0.0183278                                                                                                             
+24 124 60333.00 P  0.073916 0.013780  0.232188 0.022239  P 0.0164975 0.0183855                                                                                                             
+24 125 60334.00 P  0.072050 0.013812  0.233335 0.022304  P 0.0172281 0.0184432                                                                                                             
+24 126 60335.00 P  0.070207 0.013845  0.234510 0.022370  P 0.0178879 0.0185008                                                                                                             
+24 127 60336.00 P  0.068388 0.013877  0.235713 0.022435  P 0.0184047 0.0185583                                                                                                             
+24 128 60337.00 P  0.066593 0.013909  0.236944 0.022501  P 0.0187388 0.0186158                                                                                                             
+24 129 60338.00 P  0.064824 0.013941  0.238202 0.022566  P 0.0188782 0.0186732                                                                                                             
+24 130 60339.00 P  0.063079 0.013972  0.239487 0.022631  P 0.0188329 0.0187306                                                                                                             
+24 131 60340.00 P  0.061360 0.014004  0.240798 0.022696  P 0.0187338 0.0187879                                                                                                             
+24 2 1 60341.00 P  0.059667 0.014036  0.242135 0.022761  P 0.0187172 0.0188451                                                                                                             
+24 2 2 60342.00 P  0.058001 0.014068  0.243497 0.022826  P 0.0187265 0.0189023                                                                                                             
+24 2 3 60343.00 P  0.056361 0.014099  0.244885 0.022891  P 0.0188416 0.0189594                                                                                                             
+24 2 4 60344.00 P  0.054749 0.014131  0.246297 0.022956  P 0.0191555 0.0190165                                                                                                             
+24 2 5 60345.00 P  0.053165 0.014163  0.247733 0.023021  P 0.0196285 0.0190735                                                                                                             
+24 2 6 60346.00 P  0.051609 0.014194  0.249193 0.023086  P 0.0203184 0.0191305                                                                                                             
+24 2 7 60347.00 P  0.050082 0.014226  0.250677 0.023150  P 0.0211126 0.0191874                                                                                                             
+24 2 8 60348.00 P  0.048583 0.014257  0.252183 0.023215  P 0.0218127 0.0192442                                                                                                             
+24 2 9 60349.00 P  0.047114 0.014288  0.253711 0.023279  P 0.0222873 0.0193010                                                                                                             
+24 210 60350.00 P  0.045675 0.014320  0.255262 0.023344  P 0.0223847 0.0193577                                                                                                             
+24 211 60351.00 P  0.044265 0.014351  0.256833 0.023408  P 0.0221236 0.0194144                                                                                                             
+24 212 60352.00 P  0.042886 0.014382  0.258426 0.023472  P 0.0216171 0.0194710                                                                                                             
+24 213 60353.00 P  0.041538 0.014413  0.260039 0.023537  P 0.0208840 0.0195276                                                                                                             
+24 214 60354.00 P  0.040221 0.014444  0.261672 0.023601  P 0.0201405 0.0195841                                                                                                             
+24 215 60355.00 P  0.038934 0.014475  0.263324 0.023665  P 0.0196365 0.0196405                                                                                                             
+24 216 60356.00 P  0.037680 0.014506  0.264995 0.023729  P 0.0193349 0.0196969                                                                                                             
+24 217 60357.00 P  0.036458 0.014537  0.266685 0.023793  P 0.0193549 0.0197532                                                                                                             
+24 218 60358.00 P  0.035267 0.014568  0.268393 0.023857  P 0.0195393 0.0198095                                                                                                             
+24 219 60359.00 P  0.034110 0.014599  0.270117 0.023921  P 0.0198757 0.0198658                                                                                                             
+24 220 60360.00 P  0.032985 0.014630  0.271859 0.023984  P 0.0202152 0.0199219                                                                                                             
+24 221 60361.00 P  0.031893 0.014661  0.273617 0.024048  P 0.0205229 0.0199781                                                                                                             
+24 222 60362.00 P  0.030834 0.014691  0.275391 0.024112  P 0.0207222 0.0200341                                                                                                             
+24 223 60363.00 P  0.029809 0.014722  0.277180 0.024175  P 0.0207513 0.0200902                                                                                                             
+24 224 60364.00 P  0.028817 0.014753  0.278984 0.024239  P 0.0205864 0.0201461                                                                                                             
+24 225 60365.00 P  0.027860 0.014783  0.280802 0.024302  P 0.0202677 0.0202021                                                                                                             
+24 226 60366.00 P  0.026937 0.014814  0.282633 0.024366  P 0.0197328 0.0202579                                                                                                             
+24 227 60367.00 P  0.026048 0.014844  0.284478 0.024429  P 0.0191359 0.0203137                                                                                                             
+24 228 60368.00 P  0.025193 0.014874  0.286335 0.024492  P 0.0185505 0.0203695                                                                                                             
+24 229 60369.00 P  0.024373 0.014905  0.288204 0.024555  P 0.0180182 0.0204252                                                                                                             
+24 3 1 60370.00 P  0.023589 0.014935  0.290085 0.024618  P 0.0176214 0.0204809                                                                                                             
+24 3 2 60371.00 P  0.022839 0.014965  0.291976 0.024681  P 0.0174195 0.0205365                                                                                                             
+24 3 3 60372.00 P  0.022124 0.014996  0.293878 0.024744  P 0.0174377 0.0205920                                                                                                             
+24 3 4 60373.00 P  0.021445 0.015026  0.295790 0.024807  P 0.0176575 0.0206475                                                                                                             
+24 3 5 60374.00 P  0.020801 0.015056  0.297711 0.024870  P 0.0180532 0.0207030                                                                                                             
+24 3 6 60375.00 P  0.020192 0.015086  0.299640 0.024933  P 0.0184609 0.0207584                                                                                                             
+24 3 7 60376.00 P  0.019620 0.015116  0.301577 0.024996  P 0.0187495 0.0208138                                                                                                             
+24 3 8 60377.00 P  0.019083 0.015146  0.303522 0.025058  P 0.0187446 0.0208691                                                                                                             
+24 3 9 60378.00 P  0.018582 0.015176  0.305474 0.025121  P 0.0183844 0.0209243                                                                                                             
+24 310 60379.00 P  0.018117 0.015206  0.307433 0.025184  P 0.0176192 0.0209795                                                                                                             
+24 311 60380.00 P  0.017687 0.015236  0.309397 0.025246  P 0.0165622 0.0210347                                                                                                             
+24 312 60381.00 P  0.017294 0.015266  0.311366 0.025309  P 0.0155738 0.0210898                                                                                                             
+24 313 60382.00 P  0.016937 0.015295  0.313340 0.025371  P 0.0147621 0.0211449                                                                                                             
+24 314 60383.00 P  0.016616 0.015325  0.315318 0.025433  P 0.0143211 0.0211999                                                                                                             
+24 315 60384.00 P  0.016331 0.015355  0.317300 0.025495  P 0.0141679 0.0212548                                                                                                             
+24 316 60385.00 P  0.016083 0.015385  0.319284 0.025558  P 0.0143408 0.0213098                                                                                                             
+24 317 60386.00 P  0.015870 0.015414  0.321271 0.025620  P 0.0146371 0.0213646                                                                                                             
+24 318 60387.00 P  0.015694 0.015444  0.323260 0.025682  P 0.0150142 0.0214195                                                                                                             
+24 319 60388.00 P  0.015553 0.015473  0.325250 0.025744  P 0.0153318 0.0214742                                                                                                             
+24 320 60389.00 P  0.015449 0.015503  0.327241 0.025806  P 0.0154823 0.0215290                                                                                                             
+24 321 60390.00 P  0.015381 0.015532  0.329231 0.025868  P 0.0154119 0.0215837                                                                                                             
+24 322 60391.00 P  0.015349 0.015561  0.331222 0.025930  P 0.0151088 0.0216383                                                                                                             
+24 323 60392.00 P  0.015352 0.015591  0.333211 0.025991  P 0.0145623 0.0216929                                                                                                             
+24 324 60393.00 P  0.015392 0.015620  0.335198 0.026053  P 0.0138748 0.0217474                                                                                                             
+24 325 60394.00 P  0.015467 0.015649  0.337184 0.026115  P 0.0131057 0.0218019                                                                                                             
+24 326 60395.00 P  0.015578 0.015679  0.339167 0.026176  P 0.0123224 0.0218564                                                                                                             
+24 327 60396.00 P  0.015725 0.015708  0.341146 0.026238  P 0.0116097 0.0219108                                                                                                             
+24 328 60397.00 P  0.015907 0.015737  0.343122 0.026299  P 0.0110313 0.0219652                                                                                                             
+24 329 60398.00 P  0.016124 0.015766  0.345093 0.026361  P 0.0105921 0.0220195                                                                                                             
+24 330 60399.00 P  0.016377 0.015795  0.347059 0.026422  P 0.0103740 0.0220738                                                                                                             
+24 331 60400.00 P  0.016665 0.015824  0.349020 0.026484  P 0.0103197 0.0221280                                                                                                             
+24 4 1 60401.00 P  0.016987 0.015853  0.350975 0.026545  P 0.0103822 0.0221822                                                                                                             
+24 4 2 60402.00 P  0.017345 0.015882  0.352923 0.026606  P 0.0104601 0.0222363                                                                                                             
+24 4 3 60403.00 P  0.017737 0.015911  0.354864 0.026667  P 0.0105190 0.0222904                                                                                                             
+24 4 4 60404.00 P  0.018163 0.015940  0.356797 0.026728  P 0.0103366 0.0223444                                                                                                             
+24 4 5 60405.00 P  0.018624 0.015969  0.358723 0.026790  P 0.0098859 0.0223985                                                                                                             
+24 4 6 60406.00 P  0.019119 0.015997  0.360639 0.026851  P 0.0090945 0.0224524                                                                                                             
+24 4 7 60407.00 P  0.019647 0.016026  0.362546 0.026912  P 0.0079451 0.0225063                                                                                                             
+24 4 8 60408.00 P  0.020209 0.016055  0.364443 0.026972  P 0.0066242 0.0225602                                                                                                             
+24 4 9 60409.00 P  0.020805 0.016084  0.366330 0.027033  P 0.0054011 0.0226140                                                                                                             
+24 410 60410.00 P  0.021433 0.016112  0.368206 0.027094  P 0.0044793 0.0226678                                                                                                             
+24 411 60411.00 P  0.022095 0.016141  0.370071 0.027155  P 0.0039168 0.0227216                                                                                                             
+24 412 60412.00 P  0.022789 0.016169  0.371924 0.027216  P 0.0037326 0.0227753                                                                                                             
+24 413 60413.00 P  0.023516 0.016198  0.373765 0.027276  P 0.0038197 0.0228290                                                                                                             
+24 414 60414.00 P  0.024274 0.016226  0.375592 0.027337  P 0.0040590 0.0228826                                                                                                             
+24 415 60415.00 P  0.025065 0.016255  0.377406 0.027397  P 0.0043839 0.0229362                                                                                                             
+24 416 60416.00 P  0.025887 0.016283  0.379207 0.027458  P 0.0046300 0.0229897                                                                                                             
+24 417 60417.00 P  0.026740 0.016312  0.380993 0.027518  P 0.0047702 0.0230432                                                                                                             
+24 418 60418.00 P  0.027624 0.016340  0.382764 0.027579  P 0.0047356 0.0230966                                                                                                             
+24 419 60419.00 P  0.028539 0.016368  0.384520 0.027639  P 0.0045312 0.0231500                                                                                                             
+24 420 60420.00 P  0.029484 0.016396  0.386260 0.027699  P 0.0041581 0.0232034                                                                                                             
+24 421 60421.00 P  0.030459 0.016425  0.387984 0.027759  P 0.0037453 0.0232567                                                                                                             
+24 422 60422.00 P  0.031463 0.016453  0.389691 0.027820  P 0.0031906 0.0233100                                                                                                             
+24 423 60423.00 P  0.032497 0.016481  0.391381 0.027880  P 0.0026789 0.0233633                                                                                                             
+24 424 60424.00 P  0.033560 0.016509  0.393053 0.027940  P 0.0023108 0.0234165                                                                                                             
+24 425 60425.00 P  0.034651 0.016537  0.394707 0.028000  P 0.0020967 0.0234697                                                                                                             
+24 426 60426.00 P  0.035770 0.016565  0.396343 0.028060  P 0.0020595 0.0235228                                                                                                             
+24 427 60427.00 P  0.036917 0.016593  0.397960 0.028120  P 0.0021795 0.0235759                                                                                                             
+24 428 60428.00 P  0.038092 0.016621  0.399557 0.028180  P 0.0024751 0.0236289                                                                                                             
+24 429 60429.00 P  0.039294 0.016649  0.401135 0.028239  P 0.0028136 0.0236819                                                                                                             
+24 430 60430.00 P  0.040522 0.016677  0.402692 0.028299  P 0.0031425 0.0237349                                                                                                             
+24 5 1 60431.00 P  0.041776 0.016705  0.404229 0.028359  P 0.0033937 0.0237878                                                                                                             
+24 5 2 60432.00 P  0.043056 0.016733  0.405745 0.028419  P 0.0034691 0.0238407                                                                                                             
+24 5 3 60433.00 P  0.044362 0.016760  0.407239 0.028478  P 0.0032130 0.0238935                                                                                                             
+24 5 4 60434.00 P  0.045692 0.016788  0.408712 0.028538  P 0.0027041 0.0239463                                                                                                             
+24 5 5 60435.00 P  0.047047 0.016816  0.410162 0.028597  P 0.0020247 0.0239991                                                                                                             
+24 5 6 60436.00 P  0.048426 0.016844  0.411590 0.028657  P 0.0013245 0.0240518                                                                                                             
+24 5 7 60437.00 P  0.049829 0.016871  0.412995 0.028716  P 0.0007864 0.0241045                                                                                                             
+24 5 8 60438.00 P  0.051255 0.016899  0.414377 0.028776  P 0.0006022 0.0241572                                                                                                             
+24 5 9 60439.00 P  0.052703 0.016926  0.415735 0.028835  P 0.0007608 0.0242098                                                                                                             
+24 510 60440.00 P  0.054174 0.016954  0.417069 0.028894  P 0.0012404 0.0242624                                                                                                             
+24 511 60441.00 P  0.055666 0.016982  0.418379 0.028954  P 0.0019716 0.0243149                                                                                                             
+24 512 60442.00 P  0.057180 0.017009  0.419664 0.029013  P 0.0027486 0.0243674                                                                                                             
+24 513 60443.00 P  0.058715 0.017036  0.420925 0.029072  P 0.0035218 0.0244199                                                                                                             
+24 514 60444.00 P  0.060269 0.017064  0.422160 0.029131  P 0.0042165 0.0244723                                                                                                             
+24 515 60445.00 P  0.061844 0.017091  0.423369 0.029190  P 0.0047941 0.0245247                                                                                                             
+24 516 60446.00 P  0.063438 0.017119  0.424553 0.029249  P 0.0052143 0.0245770                                                                                                             
+24 517 60447.00 P  0.065051 0.017146  0.425711 0.029308  P 0.0055141 0.0246293                                                                                                             
+24 518 60448.00 P  0.066682 0.017173  0.426842 0.029367  P 0.0057337 0.0246816                                                                                                             
+24 519 60449.00 P  0.068331 0.017200  0.427946 0.029426  P 0.0058762 0.0247338                                                                                                             
+24 520 60450.00 P  0.069997 0.017228  0.429024 0.029485  P 0.0059805 0.0247860                                                                                                             
+24 521 60451.00 P  0.071680 0.017255  0.430074 0.029543  P 0.0061402 0.0248382                                                                                                             
+24 522 60452.00 P  0.073379 0.017282  0.431097 0.029602  P 0.0064430 0.0248903                                                                                                             
+24 523 60453.00 P  0.075094 0.017309  0.432092 0.029661  P 0.0069648 0.0249424                                                                                                             
+24 524 60454.00 P  0.076824 0.017336  0.433060 0.029720  P 0.0077172 0.0249945                                                                                                             
+24 525 60455.00 P  0.078569 0.017363  0.433999 0.029778  P 0.0086499 0.0250465                                                                                                             
+24 526 60456.00 P  0.080328 0.017390  0.434910 0.029837  P 0.0097066 0.0250985                                                                                                             
+24 527 60457.00 P  0.082100 0.017417  0.435792 0.029895  P 0.0106961 0.0251504                                                                                                             
+24 528 60458.00 P  0.083886 0.017444  0.436645 0.029954  P 0.0115734 0.0252023                                                                                                             
+24 529 60459.00 P  0.085684 0.017471  0.437470 0.030012  P 0.0122381 0.0252542                                                                                                             
+24 530 60460.00 P  0.087494 0.017498  0.438265 0.030070  P 0.0125876 0.0253060                                                                                                             
+24 531 60461.00 P  0.089315 0.017525  0.439032 0.030129  P 0.0126809 0.0253578                                                                                                             
+24 6 1 60462.00 P  0.091147 0.017552  0.439768 0.030187  P 0.0126419 0.0254096                                                                                                             
 24 6 2 60463.00                                                                                                                                                                            
 24 6 3 60464.00                                                                                                                                                                            
 24 6 4 60465.00                                                                                                                                                                            
 24 6 5 60466.00                                                                                                                                                                            
 24 6 6 60467.00                                                                                                                                                                            
 24 6 7 60468.00                                                                                                                                                                            
 24 6 8 60469.00                                                                                                                                                                            
@@ -18795,7 +18795,35 @@
 24 617 60478.00                                                                                                                                                                            
 24 618 60479.00                                                                                                                                                                            
 24 619 60480.00                                                                                                                                                                            
 24 620 60481.00                                                                                                                                                                            
 24 621 60482.00                                                                                                                                                                            
 24 622 60483.00                                                                                                                                                                            
 24 623 60484.00                                                                                                                                                                            
+24 624 60485.00                                                                                                                                                                            
+24 625 60486.00                                                                                                                                                                            
+24 626 60487.00                                                                                                                                                                            
+24 627 60488.00                                                                                                                                                                            
+24 628 60489.00                                                                                                                                                                            
+24 629 60490.00                                                                                                                                                                            
+24 630 60491.00                                                                                                                                                                            
+24 7 1 60492.00                                                                                                                                                                            
+24 7 2 60493.00                                                                                                                                                                            
+24 7 3 60494.00                                                                                                                                                                            
+24 7 4 60495.00                                                                                                                                                                            
+24 7 5 60496.00                                                                                                                                                                            
+24 7 6 60497.00                                                                                                                                                                            
+24 7 7 60498.00                                                                                                                                                                            
+24 7 8 60499.00                                                                                                                                                                            
+24 7 9 60500.00                                                                                                                                                                            
+24 710 60501.00                                                                                                                                                                            
+24 711 60502.00                                                                                                                                                                            
+24 712 60503.00                                                                                                                                                                            
+24 713 60504.00                                                                                                                                                                            
+24 714 60505.00                                                                                                                                                                            
+24 715 60506.00                                                                                                                                                                            
+24 716 60507.00                                                                                                                                                                            
+24 717 60508.00                                                                                                                                                                            
+24 718 60509.00                                                                                                                                                                            
+24 719 60510.00                                                                                                                                                                            
+24 720 60511.00                                                                                                                                                                            
+24 721 60512.00
```

### Comparing `pyTMD-2.0.4/pyTMD/data/historic_deltat.data` & `pyTMD-2.0.5/pyTMD/data/historic_deltat.data`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.4/pyTMD/data/iers_deltat.data` & `pyTMD-2.0.5/pyTMD/data/iers_deltat.data`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.4/pyTMD/data/leap-seconds.list` & `pyTMD-2.0.5/pyTMD/data/leap-seconds.list`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.4/pyTMD/data/mean-pole.tab` & `pyTMD-2.0.5/pyTMD/data/mean-pole.tab`

 * *Files 2% similar despite different names*

```diff
@@ -2105,15 +2105,15 @@
 2005.20   0.0576019   0.3446973
 2005.25   0.0577918   0.3447411
 2005.30   0.0579830   0.3447838
 2005.35   0.0581756   0.3448253
 2005.40   0.0583695   0.3448657
 2005.45   0.0585648   0.3449049
 2005.50   0.0587615   0.3449429
-2005.55   0.0589595   0.3449797
+2005.55   0.0589594   0.3449797
 2005.60   0.0591588   0.3450154
 2005.65   0.0593595   0.3450499
 2005.70   0.0595615   0.3450833
 2005.75   0.0597648   0.3451154
 2005.80   0.0599695   0.3451465
 2005.85   0.0601755   0.3451764
 2005.90   0.0603828   0.3452051
@@ -2123,20 +2123,20 @@
 2006.10   0.0612252   0.3453088
 2006.15   0.0614390   0.3453320
 2006.20   0.0616541   0.3453541
 2006.25   0.0618705   0.3453751
 2006.30   0.0620881   0.3453950
 2006.35   0.0623070   0.3454139
 2006.40   0.0625270   0.3454317
-2006.45   0.0627484   0.3454485
+2006.45   0.0627483   0.3454485
 2006.50   0.0629709   0.3454644
 2006.55   0.0631946   0.3454792
 2006.60   0.0634194   0.3454930
 2006.65   0.0636455   0.3455059
-2006.70   0.0638727   0.3455179
+2006.70   0.0638726   0.3455179
 2006.75   0.0641010   0.3455290
 2006.80   0.0643304   0.3455391
 2006.85   0.0645609   0.3455484
 2006.90   0.0647925   0.3455568
 2006.95   0.0650252   0.3455644
 2007.00   0.0652589   0.3455712
 2007.05   0.0654936   0.3455772
@@ -2144,322 +2144,324 @@
 2007.15   0.0659661   0.3455870
 2007.20   0.0662038   0.3455908
 2007.25   0.0664424   0.3455939
 2007.30   0.0666819   0.3455964
 2007.35   0.0669224   0.3455982
 2007.40   0.0671637   0.3455995
 2007.45   0.0674059   0.3456001
-2007.50   0.0676489   0.3456002
-2007.55   0.0678928   0.3455998
-2007.60   0.0681374   0.3455989
+2007.50   0.0676489   0.3456003
+2007.55   0.0678927   0.3455999
+2007.60   0.0681374   0.3455990
 2007.65   0.0683827   0.3455976
-2007.70   0.0686289   0.3455958
+2007.70   0.0686288   0.3455959
 2007.75   0.0688757   0.3455937
-2007.80   0.0691232   0.3455911
+2007.80   0.0691232   0.3455912
 2007.85   0.0693714   0.3455883
 2007.90   0.0696202   0.3455851
 2007.95   0.0698697   0.3455817
-2008.00   0.0701197   0.3455780
+2008.00   0.0701197   0.3455781
 2008.05   0.0703703   0.3455742
-2008.10   0.0706215   0.3455701
-2008.15   0.0708731   0.3455659
-2008.20   0.0711253   0.3455616
-2008.25   0.0713779   0.3455573
-2008.30   0.0716309   0.3455529
-2008.35   0.0718844   0.3455485
-2008.40   0.0721382   0.3455441
-2008.45   0.0723924   0.3455398
-2008.50   0.0726470   0.3455356
-2008.55   0.0729018   0.3455315
-2008.60   0.0731570   0.3455276
-2008.65   0.0734124   0.3455239
-2008.70   0.0736680   0.3455204
-2008.75   0.0739238   0.3455172
-2008.80   0.0741799   0.3455143
-2008.85   0.0744360   0.3455117
-2008.90   0.0746924   0.3455094
-2008.95   0.0749488   0.3455076
-2009.00   0.0752053   0.3455061
-2009.05   0.0754619   0.3455052
-2009.10   0.0757185   0.3455047
-2009.15   0.0759751   0.3455047
-2009.20   0.0762317   0.3455053
-2009.25   0.0764883   0.3455065
-2009.30   0.0767449   0.3455083
-2009.35   0.0770013   0.3455107
-2009.40   0.0772577   0.3455138
-2009.45   0.0775139   0.3455176
-2009.50   0.0777701   0.3455221
-2009.55   0.0780260   0.3455274
-2009.60   0.0782818   0.3455334
-2009.65   0.0785374   0.3455403
-2009.70   0.0787927   0.3455480
-2009.75   0.0790479   0.3455565
-2009.80   0.0793027   0.3455659
-2009.85   0.0795574   0.3455763
-2009.90   0.0798117   0.3455875
-2009.95   0.0800657   0.3455997
-2010.00   0.0803194   0.3456129
-2010.05   0.0805727   0.3456270
-2010.10   0.0808258   0.3456422
-2010.15   0.0810784   0.3456584
-2010.20   0.0813307   0.3456756
-2010.25   0.0815825   0.3456939
-2010.30   0.0818340   0.3457133
-2010.35   0.0820851   0.3457337
-2010.40   0.0823357   0.3457553
-2010.45   0.0825859   0.3457780
-2010.50   0.0828356   0.3458019
-2010.55   0.0830848   0.3458268
-2010.60   0.0833336   0.3458530
-2010.65   0.0835819   0.3458803
-2010.70   0.0838298   0.3459088
-2010.75   0.0840771   0.3459385
-2010.80   0.0843239   0.3459693
-2010.85   0.0845702   0.3460014
-2010.90   0.0848160   0.3460346
-2010.95   0.0850613   0.3460691
-2011.00   0.0853060   0.3461048
-2011.05   0.0855502   0.3461416
-2011.10   0.0857939   0.3461797
-2011.15   0.0860370   0.3462190
-2011.20   0.0862796   0.3462595
-2011.25   0.0865217   0.3463013
-2011.30   0.0867631   0.3463442
-2011.35   0.0870041   0.3463883
-2011.40   0.0872445   0.3464336
-2011.45   0.0874843   0.3464801
-2011.50   0.0877236   0.3465278
-2011.55   0.0879623   0.3465767
-2011.60   0.0882005   0.3466267
-2011.65   0.0884381   0.3466779
-2011.70   0.0886751   0.3467302
-2011.75   0.0889117   0.3467837
-2011.80   0.0891476   0.3468382
-2011.85   0.0893831   0.3468939
-2011.90   0.0896180   0.3469506
-2011.95   0.0898523   0.3470085
-2012.00   0.0900861   0.3470674
-2012.05   0.0903194   0.3471273
-2012.10   0.0905522   0.3471882
-2012.15   0.0907844   0.3472502
-2012.20   0.0910161   0.3473131
-2012.25   0.0912473   0.3473770
-2012.30   0.0914780   0.3474418
-2012.35   0.0917082   0.3475075
-2012.40   0.0919380   0.3475741
-2012.45   0.0921672   0.3476416
-2012.50   0.0923959   0.3477099
-2012.55   0.0926242   0.3477791
-2012.60   0.0928520   0.3478490
-2012.65   0.0930793   0.3479197
-2012.70   0.0933062   0.3479911
-2012.75   0.0935326   0.3480632
-2012.80   0.0937586   0.3481360
-2012.85   0.0939841   0.3482095
-2012.90   0.0942092   0.3482836
-2012.95   0.0944339   0.3483582
-2013.00   0.0946582   0.3484334
-2013.05   0.0948820   0.3485092
-2013.10   0.0951055   0.3485854
-2013.15   0.0953285   0.3486621
-2013.20   0.0955512   0.3487392
-2013.25   0.0957735   0.3488167
-2013.30   0.0959955   0.3488946
-2013.35   0.0962170   0.3489728
-2013.40   0.0964382   0.3490513
-2013.45   0.0966591   0.3491300
-2013.50   0.0968796   0.3492090
-2013.55   0.0970997   0.3492882
-2013.60   0.0973196   0.3493675
-2013.65   0.0975391   0.3494469
-2013.70   0.0977582   0.3495264
-2013.75   0.0979771   0.3496060
-2013.80   0.0981956   0.3496856
-2013.85   0.0984139   0.3497652
-2013.90   0.0986318   0.3498447
-2013.95   0.0988495   0.3499241
-2014.00   0.0990669   0.3500034
-2014.05   0.0992839   0.3500825
-2014.10   0.0995007   0.3501614
-2014.15   0.0997172   0.3502402
-2014.20   0.0999335   0.3503186
-2014.25   0.1001494   0.3503967
-2014.30   0.1003651   0.3504745
-2014.35   0.1005806   0.3505520
-2014.40   0.1007957   0.3506290
-2014.45   0.1010106   0.3507056
-2014.50   0.1012253   0.3507817
-2014.55   0.1014397   0.3508573
-2014.60   0.1016538   0.3509324
-2014.65   0.1018677   0.3510069
-2014.70   0.1020813   0.3510808
-2014.75   0.1022947   0.3511541
-2014.80   0.1025078   0.3512267
-2014.85   0.1027207   0.3512987
-2014.90   0.1029333   0.3513699
-2014.95   0.1031456   0.3514404
-2015.00   0.1033577   0.3515100
-2015.05   0.1035696   0.3515789
-2015.10   0.1037811   0.3516469
-2015.15   0.1039924   0.3517141
-2015.20   0.1042035   0.3517804
-2015.25   0.1044143   0.3518457
-2015.30   0.1046247   0.3519102
-2015.35   0.1048350   0.3519736
-2015.40   0.1050449   0.3520360
-2015.45   0.1052545   0.3520975
-2015.50   0.1054639   0.3521579
-2015.55   0.1056730   0.3522172
-2015.60   0.1058817   0.3522755
-2015.65   0.1060902   0.3523326
-2015.70   0.1062983   0.3523886
-2015.75   0.1065061   0.3524435
-2015.80   0.1067136   0.3524972
-2015.85   0.1069208   0.3525497
-2015.90   0.1071276   0.3526010
-2015.95   0.1073341   0.3526511
-2016.00   0.1075402   0.3526999
-2016.05   0.1077459   0.3527475
-2016.10   0.1079513   0.3527939
-2016.15   0.1081563   0.3528389
-2016.20   0.1083609   0.3528827
-2016.25   0.1085652   0.3529251
-2016.30   0.1087690   0.3529662
-2016.35   0.1089724   0.3530060
-2016.40   0.1091753   0.3530444
-2016.45   0.1093779   0.3530815
-2016.50   0.1095799   0.3531172
-2016.55   0.1097816   0.3531516
-2016.60   0.1099827   0.3531845
-2016.65   0.1101834   0.3532161
-2016.70   0.1103836   0.3532463
-2016.75   0.1105833   0.3532750
-2016.80   0.1107825   0.3533024
-2016.85   0.1109812   0.3533283
-2016.90   0.1111794   0.3533529
-2016.95   0.1113770   0.3533760
-2017.00   0.1115740   0.3533976
-2017.05   0.1117705   0.3534179
-2017.10   0.1119664   0.3534367
-2017.15   0.1121618   0.3534540
-2017.20   0.1123565   0.3534700
-2017.25   0.1125506   0.3534844
-2017.30   0.1127442   0.3534975
-2017.35   0.1129370   0.3535091
-2017.40   0.1131293   0.3535193
-2017.45   0.1133208   0.3535281
-2017.50   0.1135117   0.3535354
-2017.55   0.1137020   0.3535413
-2017.60   0.1138915   0.3535457
-2017.65   0.1140804   0.3535488
-2017.70   0.1142685   0.3535504
-2017.75   0.1144559   0.3535506
-2017.80   0.1146426   0.3535493
-2017.85   0.1148285   0.3535467
-2017.90   0.1150137   0.3535427
-2017.95   0.1151981   0.3535373
-2018.00   0.1153817   0.3535305
-2018.05   0.1155645   0.3535223
-2018.10   0.1157465   0.3535127
-2018.15   0.1159278   0.3535018
-2018.20   0.1161082   0.3534894
-2018.25   0.1162877   0.3534758
-2018.30   0.1164665   0.3534608
-2018.35   0.1166443   0.3534444
-2018.40   0.1168213   0.3534267
-2018.45   0.1169975   0.3534077
-2018.50   0.1171727   0.3533874
-2018.55   0.1173471   0.3533658
-2018.60   0.1175206   0.3533428
-2018.65   0.1176931   0.3533186
-2018.70   0.1178648   0.3532931
-2018.75   0.1180355   0.3532664
-2018.80   0.1182053   0.3532384
-2018.85   0.1183741   0.3532091
-2018.90   0.1185420   0.3531786
-2018.95   0.1187089   0.3531468
-2019.00   0.1188749   0.3531139
-2019.05   0.1190399   0.3530797
-2019.10   0.1192039   0.3530444
-2019.15   0.1193669   0.3530078
-2019.20   0.1195289   0.3529701
-2019.25   0.1196899   0.3529312
-2019.30   0.1198499   0.3528912
-2019.35   0.1200089   0.3528500
-2019.40   0.1201668   0.3528077
-2019.45   0.1203238   0.3527643
-2019.50   0.1204797   0.3527197
-2019.55   0.1206345   0.3526741
-2019.60   0.1207884   0.3526274
-2019.65   0.1209411   0.3525795
-2019.70   0.1210928   0.3525307
-2019.75   0.1212435   0.3524807
-2019.80   0.1213931   0.3524298
-2019.85   0.1215416   0.3523777
-2019.90   0.1216891   0.3523247
-2019.95   0.1218354   0.3522707
-2020.00   0.1219807   0.3522156
-2020.05   0.1221250   0.3521596
-2020.10   0.1222681   0.3521025
-2020.15   0.1224101   0.3520446
-2020.20   0.1225511   0.3519856
-2020.25   0.1226909   0.3519257
-2020.30   0.1228297   0.3518649
-2020.35   0.1229674   0.3518031
-2020.40   0.1231039   0.3517404
-2020.45   0.1232394   0.3516769
-2020.50   0.1233738   0.3516124
-2020.55   0.1235070   0.3515470
-2020.60   0.1236392   0.3514808
-2020.65   0.1237702   0.3514136
-2020.70   0.1239002   0.3513457
-2020.75   0.1240290   0.3512769
-2020.80   0.1241567   0.3512072
-2020.85   0.1242833   0.3511367
-2020.90   0.1244088   0.3510654
-2020.95   0.1245332   0.3509933
-2021.00   0.1246565   0.3509204
-2021.05   0.1247787   0.3508468
-2021.10   0.1248998   0.3507723
-2021.15   0.1250197   0.3506970
-2021.20   0.1251386   0.3506210
-2021.25   0.1252563   0.3505443
-2021.30   0.1253730   0.3504668
-2021.35   0.1254885   0.3503885
-2021.40   0.1256029   0.3503096
-2021.45   0.1257163   0.3502299
-2021.50   0.1258285   0.3501495
-2021.55   0.1259397   0.3500684
-2021.60   0.1260497   0.3499866
-2021.65   0.1261587   0.3499042
-2021.70   0.1262666   0.3498210
-2021.75   0.1263733   0.3497372
-2021.80   0.1264790   0.3496527
-2021.85   0.1265836   0.3495676
-2021.90   0.1266872   0.3494818
-2021.95   0.1267896   0.3493954
-2022.00   0.1268910   0.3493084
-2022.05   0.1269913   0.3492207
-2022.10   0.1270905   0.3491325
-2022.15   0.1271887   0.3490436
-2022.20   0.1272858   0.3489541
-2022.25   0.1273818   0.3488640
-2022.30   0.1274768   0.3487734
-2022.35   0.1275708   0.3486821
-2022.40   0.1276636   0.3485903
-2022.45   0.1277555   0.3484979
-2022.50   0.1278463   0.3484050
-2022.55   0.1279360   0.3483115
-2022.60   0.1280247   0.3482175
-2022.65   0.1281124   0.3481229
-2022.70   0.1281991   0.3480278
-2022.75   0.1282847   0.3479322
-2022.80   0.1283693   0.3478360
-2022.85   0.1284529   0.3477394
-2022.90   0.1285355   0.3476422
-2022.95   0.1286171   0.3475446
-2023.00   0.1286976   0.3474464
-2023.05   0.1287772   0.3473478
-2023.10   0.1288558   0.3472487
-2023.15   0.1289334   0.3471491
-2023.20   0.1290100   0.3470490
+2008.10   0.0706214   0.3455701
+2008.15   0.0708731   0.3455660
+2008.20   0.0711252   0.3455617
+2008.25   0.0713778   0.3455573
+2008.30   0.0716309   0.3455530
+2008.35   0.0718843   0.3455486
+2008.40   0.0721382   0.3455442
+2008.45   0.0723924   0.3455399
+2008.50   0.0726469   0.3455357
+2008.55   0.0729018   0.3455316
+2008.60   0.0731569   0.3455277
+2008.65   0.0734123   0.3455240
+2008.70   0.0736679   0.3455205
+2008.75   0.0739238   0.3455173
+2008.80   0.0741798   0.3455143
+2008.85   0.0744359   0.3455118
+2008.90   0.0746923   0.3455095
+2008.95   0.0749487   0.3455077
+2009.00   0.0752052   0.3455063
+2009.05   0.0754617   0.3455053
+2009.10   0.0757183   0.3455048
+2009.15   0.0759750   0.3455049
+2009.20   0.0762316   0.3455055
+2009.25   0.0764882   0.3455067
+2009.30   0.0767447   0.3455085
+2009.35   0.0770011   0.3455109
+2009.40   0.0772575   0.3455140
+2009.45   0.0775137   0.3455178
+2009.50   0.0777698   0.3455223
+2009.55   0.0780258   0.3455276
+2009.60   0.0782815   0.3455337
+2009.65   0.0785371   0.3455406
+2009.70   0.0787924   0.3455483
+2009.75   0.0790476   0.3455568
+2009.80   0.0793024   0.3455663
+2009.85   0.0795570   0.3455766
+2009.90   0.0798113   0.3455879
+2009.95   0.0800653   0.3456001
+2010.00   0.0803190   0.3456133
+2010.05   0.0805723   0.3456274
+2010.10   0.0808253   0.3456426
+2010.15   0.0810779   0.3456588
+2010.20   0.0813301   0.3456761
+2010.25   0.0815820   0.3456944
+2010.30   0.0818334   0.3457138
+2010.35   0.0820844   0.3457343
+2010.40   0.0823350   0.3457560
+2010.45   0.0825851   0.3457787
+2010.50   0.0828348   0.3458026
+2010.55   0.0830840   0.3458276
+2010.60   0.0833328   0.3458538
+2010.65   0.0835810   0.3458811
+2010.70   0.0838288   0.3459097
+2010.75   0.0840761   0.3459394
+2010.80   0.0843228   0.3459703
+2010.85   0.0845691   0.3460024
+2010.90   0.0848148   0.3460357
+2010.95   0.0850600   0.3460702
+2011.00   0.0853047   0.3461060
+2011.05   0.0855488   0.3461429
+2011.10   0.0857924   0.3461811
+2011.15   0.0860354   0.3462204
+2011.20   0.0862779   0.3462610
+2011.25   0.0865199   0.3463028
+2011.30   0.0867613   0.3463458
+2011.35   0.0870021   0.3463900
+2011.40   0.0872424   0.3464354
+2011.45   0.0874821   0.3464820
+2011.50   0.0877212   0.3465298
+2011.55   0.0879598   0.3465788
+2011.60   0.0881979   0.3466289
+2011.65   0.0884353   0.3466802
+2011.70   0.0886723   0.3467327
+2011.75   0.0889086   0.3467862
+2011.80   0.0891444   0.3468409
+2011.85   0.0893797   0.3468967
+2011.90   0.0896144   0.3469536
+2011.95   0.0898486   0.3470116
+2012.00   0.0900822   0.3470706
+2012.05   0.0903153   0.3471307
+2012.10   0.0905478   0.3471918
+2012.15   0.0907798   0.3472540
+2012.20   0.0910113   0.3473171
+2012.25   0.0912422   0.3473811
+2012.30   0.0914727   0.3474461
+2012.35   0.0917026   0.3475121
+2012.40   0.0919320   0.3475789
+2012.45   0.0921610   0.3476466
+2012.50   0.0923894   0.3477152
+2012.55   0.0926173   0.3477846
+2012.60   0.0928448   0.3478547
+2012.65   0.0930717   0.3479257
+2012.70   0.0932982   0.3479974
+2012.75   0.0935242   0.3480698
+2012.80   0.0937498   0.3481429
+2012.85   0.0939749   0.3482167
+2012.90   0.0941996   0.3482911
+2012.95   0.0944238   0.3483661
+2013.00   0.0946476   0.3484416
+2013.05   0.0948709   0.3485177
+2013.10   0.0950939   0.3485943
+2013.15   0.0953164   0.3486714
+2013.20   0.0955385   0.3487489
+2013.25   0.0957602   0.3488269
+2013.30   0.0959815   0.3489052
+2013.35   0.0962024   0.3489838
+2013.40   0.0964229   0.3490628
+2013.45   0.0966431   0.3491420
+2013.50   0.0968628   0.3492215
+2013.55   0.0970822   0.3493012
+2013.60   0.0973012   0.3493810
+2013.65   0.0975199   0.3494610
+2013.70   0.0977382   0.3495412
+2013.75   0.0979562   0.3496213
+2013.80   0.0981738   0.3497015
+2013.85   0.0983911   0.3497818
+2013.90   0.0986080   0.3498619
+2013.95   0.0988246   0.3499420
+2014.00   0.0990409   0.3500221
+2014.05   0.0992569   0.3501019
+2014.10   0.0994725   0.3501816
+2014.15   0.0996878   0.3502611
+2014.20   0.0999028   0.3503404
+2014.25   0.1001174   0.3504194
+2014.30   0.1003318   0.3504980
+2014.35   0.1005458   0.3505764
+2014.40   0.1007595   0.3506543
+2014.45   0.1009729   0.3507319
+2014.50   0.1011860   0.3508090
+2014.55   0.1013988   0.3508857
+2014.60   0.1016112   0.3509618
+2014.65   0.1018234   0.3510374
+2014.70   0.1020352   0.3511125
+2014.75   0.1022467   0.3511869
+2014.80   0.1024579   0.3512607
+2014.85   0.1026688   0.3513339
+2014.90   0.1028794   0.3514064
+2014.95   0.1030896   0.3514782
+2015.00   0.1032995   0.3515492
+2015.05   0.1035090   0.3516195
+2015.10   0.1037183   0.3516889
+2015.15   0.1039272   0.3517576
+2015.20   0.1041357   0.3518254
+2015.25   0.1043439   0.3518923
+2015.30   0.1045517   0.3519583
+2015.35   0.1047592   0.3520234
+2015.40   0.1049663   0.3520876
+2015.45   0.1051730   0.3521508
+2015.50   0.1053794   0.3522129
+2015.55   0.1055853   0.3522741
+2015.60   0.1057909   0.3523343
+2015.65   0.1059960   0.3523934
+2015.70   0.1062008   0.3524514
+2015.75   0.1064051   0.3525083
+2015.80   0.1066090   0.3525641
+2015.85   0.1068124   0.3526188
+2015.90   0.1070154   0.3526724
+2015.95   0.1072180   0.3527247
+2016.00   0.1074201   0.3527759
+2016.05   0.1076216   0.3528259
+2016.10   0.1078228   0.3528747
+2016.15   0.1080234   0.3529223
+2016.20   0.1082235   0.3529687
+2016.25   0.1084230   0.3530138
+2016.30   0.1086221   0.3530576
+2016.35   0.1088206   0.3531002
+2016.40   0.1090185   0.3531415
+2016.45   0.1092159   0.3531816
+2016.50   0.1094127   0.3532203
+2016.55   0.1096089   0.3532577
+2016.60   0.1098045   0.3532938
+2016.65   0.1099994   0.3533286
+2016.70   0.1101938   0.3533621
+2016.75   0.1103875   0.3533943
+2016.80   0.1105805   0.3534251
+2016.85   0.1107729   0.3534546
+2016.90   0.1109645   0.3534827
+2016.95   0.1111555   0.3535095
+2017.00   0.1113458   0.3535350
+2017.05   0.1115353   0.3535591
+2017.10   0.1117241   0.3535819
+2017.15   0.1119122   0.3536033
+2017.20   0.1120995   0.3536233
+2017.25   0.1122860   0.3536421
+2017.30   0.1124717   0.3536594
+2017.35   0.1126566   0.3536755
+2017.40   0.1128407   0.3536902
+2017.45   0.1130239   0.3537035
+2017.50   0.1132063   0.3537155
+2017.55   0.1133878   0.3537262
+2017.60   0.1135685   0.3537355
+2017.65   0.1137482   0.3537436
+2017.70   0.1139271   0.3537503
+2017.75   0.1141050   0.3537556
+2017.80   0.1142821   0.3537597
+2017.85   0.1144581   0.3537625
+2017.90   0.1146332   0.3537640
+2017.95   0.1148074   0.3537641
+2018.00   0.1149805   0.3537630
+2018.05   0.1151527   0.3537607
+2018.10   0.1153238   0.3537570
+2018.15   0.1154940   0.3537521
+2018.20   0.1156631   0.3537460
+2018.25   0.1158311   0.3537386
+2018.30   0.1159981   0.3537299
+2018.35   0.1161641   0.3537201
+2018.40   0.1163289   0.3537090
+2018.45   0.1164927   0.3536967
+2018.50   0.1166553   0.3536833
+2018.55   0.1168169   0.3536686
+2018.60   0.1169773   0.3536528
+2018.65   0.1171366   0.3536358
+2018.70   0.1172947   0.3536176
+2018.75   0.1174517   0.3535983
+2018.80   0.1176075   0.3535779
+2018.85   0.1177622   0.3535563
+2018.90   0.1179157   0.3535336
+2018.95   0.1180679   0.3535099
+2019.00   0.1182190   0.3534850
+2019.05   0.1183688   0.3534590
+2019.10   0.1185175   0.3534320
+2019.15   0.1186649   0.3534040
+2019.20   0.1188111   0.3533749
+2019.25   0.1189560   0.3533447
+2019.30   0.1190997   0.3533136
+2019.35   0.1192421   0.3532814
+2019.40   0.1193833   0.3532482
+2019.45   0.1195232   0.3532141
+2019.50   0.1196618   0.3531790
+2019.55   0.1197991   0.3531429
+2019.60   0.1199352   0.3531058
+2019.65   0.1200699   0.3530679
+2019.70   0.1202034   0.3530289
+2019.75   0.1203355   0.3529891
+2019.80   0.1204664   0.3529484
+2019.85   0.1205959   0.3529068
+2019.90   0.1207241   0.3528643
+2019.95   0.1208510   0.3528209
+2020.00   0.1209766   0.3527767
+2020.05   0.1211008   0.3527316
+2020.10   0.1212237   0.3526857
+2020.15   0.1213453   0.3526390
+2020.20   0.1214655   0.3525915
+2020.25   0.1215844   0.3525431
+2020.30   0.1217019   0.3524940
+2020.35   0.1218181   0.3524441
+2020.40   0.1219330   0.3523934
+2020.45   0.1220465   0.3523420
+2020.50   0.1221587   0.3522898
+2020.55   0.1222695   0.3522368
+2020.60   0.1223790   0.3521832
+2020.65   0.1224871   0.3521288
+2020.70   0.1225939   0.3520738
+2020.75   0.1226993   0.3520180
+2020.80   0.1228034   0.3519615
+2020.85   0.1229061   0.3519044
+2020.90   0.1230075   0.3518466
+2020.95   0.1231075   0.3517882
+2021.00   0.1232062   0.3517291
+2021.05   0.1233035   0.3516693
+2021.10   0.1233995   0.3516090
+2021.15   0.1234941   0.3515480
+2021.20   0.1235874   0.3514864
+2021.25   0.1236794   0.3514243
+2021.30   0.1237700   0.3513615
+2021.35   0.1238593   0.3512981
+2021.40   0.1239473   0.3512342
+2021.45   0.1240339   0.3511697
+2021.50   0.1241192   0.3511047
+2021.55   0.1242032   0.3510391
+2021.60   0.1242858   0.3509730
+2021.65   0.1243672   0.3509063
+2021.70   0.1244472   0.3508392
+2021.75   0.1245259   0.3507715
+2021.80   0.1246033   0.3507033
+2021.85   0.1246794   0.3506346
+2021.90   0.1247542   0.3505654
+2021.95   0.1248277   0.3504958
+2022.00   0.1248999   0.3504256
+2022.05   0.1249709   0.3503550
+2022.10   0.1250405   0.3502840
+2022.15   0.1251089   0.3502125
+2022.20   0.1251760   0.3501405
+2022.25   0.1252418   0.3500682
+2022.30   0.1253064   0.3499953
+2022.35   0.1253697   0.3499221
+2022.40   0.1254317   0.3498485
+2022.45   0.1254925   0.3497744
+2022.50   0.1255521   0.3496999
+2022.55   0.1256104   0.3496251
+2022.60   0.1256675   0.3495498
+2022.65   0.1257234   0.3494742
+2022.70   0.1257780   0.3493982
+2022.75   0.1258314   0.3493218
+2022.80   0.1258837   0.3492451
+2022.85   0.1259347   0.3491680
+2022.90   0.1259845   0.3490906
+2022.95   0.1260331   0.3490128
+2023.00   0.1260805   0.3489347
+2023.05   0.1261268   0.3488562
+2023.10   0.1261719   0.3487775
+2023.15   0.1262158   0.3486984
+2023.20   0.1262585   0.3486190
+2023.25   0.1263001   0.3485392
+2023.30   0.1263405   0.3484592
```

### Comparing `pyTMD-2.0.4/pyTMD/data/merged_deltat.data` & `pyTMD-2.0.5/pyTMD/data/merged_deltat.data`

 * *Files 1% similar despite different names*

```diff
@@ -7700,7 +7700,42 @@
  2023  4 28 69.2175
  2023  4 29 69.2175
  2023  4 30 69.2178
  2023  5  1 69.2182
  2023  5  2 69.2188
  2023  5  3 69.2195
  2023  5  4 69.2201
+ 2023  5  5 69.2208
+ 2023  5  6 69.2213
+ 2023  5  7 69.2218
+ 2023  5  8 69.2220
+ 2023  5  9 69.2220
+ 2023  5 10 69.2221
+ 2023  5 11 69.2223
+ 2023  5 12 69.2228
+ 2023  5 13 69.2235
+ 2023  5 14 69.2245
+ 2023  5 15 69.2258
+ 2023  5 16 69.2271
+ 2023  5 17 69.2283
+ 2023  5 18 69.2293
+ 2023  5 19 69.2299
+ 2023  5 20 69.2303
+ 2023  5 21 69.2304
+ 2023  5 22 69.2302
+ 2023  5 23 69.2300
+ 2023  5 24 69.2297
+ 2023  5 25 69.2294
+ 2023  5 26 69.2291
+ 2023  5 27 69.2289
+ 2023  5 28 69.2290
+ 2023  5 29 69.2292
+ 2023  5 30 69.2295
+ 2023  5 31 69.2297
+ 2023  6  1 69.2300
+ 2023  6  2 69.2302
+ 2023  6  3 69.2302
+ 2023  6  4 69.2299
+ 2023  6  5 69.2294
+ 2023  6  6 69.2289
+ 2023  6  7 69.2284
+ 2023  6  8 69.2281
```

### Comparing `pyTMD-2.0.4/pyTMD/data/opoleloadcoefcmcor.txt.gz` & `pyTMD-2.0.5/pyTMD/data/opoleloadcoefcmcor.txt.gz`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.4/pyTMD/data/ser7.dat` & `pyTMD-2.0.5/pyTMD/data/ser7.dat`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
                                                                                
       **********************************************************************   
       *                                                                    *   
       *                   I E R S   B U L L E T I N - A                    *   
       *                                                                    *   
       *           Rapid Service/Prediction of Earth Orientation            *   
       **********************************************************************   
-      4 May 2023                                          Vol. XXXVI No. 018   
+      8 June 2023                                         Vol. XXXVI No. 023   
       ______________________________________________________________________   
       GENERAL INFORMATION:                                                     
          MJD = Julian Date - 2 400 000.5 days                                  
          UT2-UT1 = 0.022 sin(2*pi*T) - 0.012 cos(2*pi*T)                       
                                      - 0.006 sin(4*pi*T) + 0.007 cos(4*pi*T)   
             where pi = 3.14159265... and T is the date in Besselian years.     
          TT = TAI + 32.184 seconds                                             
@@ -49,521 +49,528 @@
      ________________________________________________________________________  
                                                                                
       COMBINED EARTH ORIENTATION PARAMETERS:                                   
                                                                                
                               IERS Rapid Service                               
               MJD      x    error     y    error   UT1-UTC   error             
                        "      "       "      "        s        s               
-   23  4 28  60062 0.02151 .00009 0.46907 .00009 -0.033484 0.000012          
-   23  4 29  60063 0.02382 .00009 0.47067 .00009 -0.033535 0.000012          
-   23  4 30  60064 0.02597 .00009 0.47211 .00009 -0.033779 0.000015          
-   23  5  1  60065 0.02758 .00009 0.47345 .00009 -0.034219 0.000012          
-   23  5  2  60066 0.02886 .00009 0.47464 .00009 -0.034805 0.000013          
-   23  5  3  60067 0.03027 .00009 0.47567 .00009 -0.035459 0.000012          
-   23  5  4  60068 0.03192 .00009 0.47664 .00009 -0.036125 0.000012          
+   23  6  2  60097 0.09927 .00009 0.50865 .00009 -0.046186 0.000010          
+   23  6  3  60098 0.10222 .00009 0.50940 .00009 -0.046162 0.000012          
+   23  6  4  60099 0.10514 .00009 0.51001 .00009 -0.045918 0.000016          
+   23  6  5  60100 0.10809 .00009 0.51040 .00009 -0.045448 0.000019          
+   23  6  6  60101 0.11119 .00009 0.51082 .00009 -0.044903 0.000020          
+   23  6  7  60102 0.11409 .00009 0.51127 .00009 -0.044423 0.000022          
+   23  6  8  60103 0.11660 .00009 0.51165 .00009 -0.044092 0.000028          
                                                                                
                               IERS Final Values                                
                                MJD        x        y      UT1-UTC              
                                           "        "         s                 
-           23  3  2           60005   -0.0461   0.3188  -0.01506       
-           23  3  3           60006   -0.0467   0.3211  -0.01482       
-           23  3  4           60007   -0.0469   0.3238  -0.01468       
-           23  3  5           60008   -0.0465   0.3266  -0.01468       
-           23  3  6           60009   -0.0457   0.3298  -0.01491       
-           23  3  7           60010   -0.0446   0.3333  -0.01537       
-           23  3  8           60011   -0.0435   0.3366  -0.01601       
-           23  3  9           60012   -0.0424   0.3398  -0.01678       
-           23  3 10           60013   -0.0413   0.3431  -0.01760       
-           23  3 11           60014   -0.0408   0.3464  -0.01840       
-           23  3 12           60015   -0.0405   0.3495  -0.01909       
-           23  3 13           60016   -0.0401   0.3526  -0.01960       
-           23  3 14           60017   -0.0397   0.3560  -0.01991       
-           23  3 15           60018   -0.0397   0.3594  -0.02006       
-           23  3 16           60019   -0.0398   0.3622  -0.02007       
-           23  3 17           60020   -0.0397   0.3646  -0.02004       
-           23  3 18           60021   -0.0390   0.3669  -0.02013       
-           23  3 19           60022   -0.0381   0.3690  -0.02049       
-           23  3 20           60023   -0.0369   0.3713  -0.02114       
-           23  3 21           60024   -0.0355   0.3740  -0.02200       
-           23  3 22           60025   -0.0339   0.3771  -0.02296       
-           23  3 23           60026   -0.0325   0.3802  -0.02389       
-           23  3 24           60027   -0.0312   0.3833  -0.02469       
-           23  3 25           60028   -0.0299   0.3864  -0.02522       
-           23  3 26           60029   -0.0284   0.3895  -0.02543       
-           23  3 27           60030   -0.0266   0.3926  -0.02539       
-           23  3 28           60031   -0.0247   0.3954  -0.02518       
-           23  3 29           60032   -0.0230   0.3979  -0.02488       
-           23  3 30           60033   -0.0217   0.4000  -0.02458       
-           23  3 31           60034   -0.0204   0.4022  -0.02439       
-           23  4  1           60035   -0.0188   0.4046  -0.02434       
+           23  4  2           60036   -0.0173   0.4074  -0.02446       
+           23  4  3           60037   -0.0156   0.4100  -0.02474       
+           23  4  4           60038   -0.0138   0.4126  -0.02522       
+           23  4  5           60039   -0.0123   0.4155  -0.02584       
+           23  4  6           60040   -0.0108   0.4183  -0.02654       
+           23  4  7           60041   -0.0091   0.4213  -0.02725       
+           23  4  8           60042   -0.0079   0.4238  -0.02792       
+           23  4  9           60043   -0.0065   0.4263  -0.02848       
+           23  4 10           60044   -0.0053   0.4288  -0.02885       
+           23  4 11           60045   -0.0041   0.4314  -0.02902       
+           23  4 12           60046   -0.0029   0.4342  -0.02903       
+           23  4 13           60047   -0.0024   0.4367  -0.02899       
+           23  4 14           60048   -0.0018   0.4393  -0.02901       
+           23  4 15           60049   -0.0012   0.4417  -0.02926       
+           23  4 16           60050    0.0002   0.4436  -0.02982       
+           23  4 17           60051    0.0017   0.4453  -0.03064       
+           23  4 18           60052    0.0029   0.4469  -0.03161       
+           23  4 19           60053    0.0043   0.4486  -0.03254       
+           23  4 20           60054    0.0057   0.4505  -0.03336       
+           23  4 21           60055    0.0074   0.4526  -0.03397       
+           23  4 22           60056    0.0092   0.4551  -0.03430       
+           23  4 23           60057    0.0107   0.4578  -0.03437       
+           23  4 24           60058    0.0126   0.4606  -0.03428       
+           23  4 25           60059    0.0149   0.4629  -0.03407       
+           23  4 26           60060    0.0173   0.4650  -0.03384       
+           23  4 27           60061    0.0194   0.4671  -0.03363       
+           23  4 28           60062    0.0214   0.4691  -0.03350       
+           23  4 29           60063    0.0238   0.4707  -0.03356       
+           23  4 30           60064    0.0260   0.4721  -0.03381       
+           23  5  1           60065    0.0276   0.4735  -0.03421       
                                                                                
       _______________________________________________________________________  
                                                                                
       PREDICTIONS:                                                             
       The following formulas will not reproduce the predictions given below,   
       but may be used to extend the predictions beyond the end of this table.  
                                                                                
-      x =  0.1424 - 0.0845 cos A + 0.0826 sin A - 0.0244 cos C + 0.0613 sin C  
-      y =  0.3369 + 0.0754 cos A + 0.0822 sin A + 0.0613 cos C + 0.0244 sin C  
-         UT1-UTC = -0.0082 + 0.00018 (MJD - 60076) - (UT2-UT1)                 
+      x =  0.1312 - 0.0139 cos A + 0.1174 sin A - 0.0006 cos C + 0.0595 sin C  
+      y =  0.3421 + 0.1071 cos A + 0.0149 sin A + 0.0595 cos C + 0.0006 sin C  
+         UT1-UTC = -0.0247 + 0.00014 (MJD - 60111) - (UT2-UT1)                 
                                                                                
-      where A = 2*pi*(MJD-60068)/365.25 and C = 2*pi*(MJD-60068)/435.          
+      where A = 2*pi*(MJD-60103)/365.25 and C = 2*pi*(MJD-60103)/435.          
                                                                                
-         TAI-UTC(MJD 60069) = 37.0                                             
+         TAI-UTC(MJD 60104) = 37.0                                             
       The accuracy may be estimated from the expressions:                      
-      S x,y = 0.00068 (MJD-60068)**0.80   S t = 0.00025 (MJD-60068)**0.75      
+      S x,y = 0.00068 (MJD-60103)**0.80   S t = 0.00025 (MJD-60103)**0.75      
       Estimated accuracies are:  Predictions     10 d   20 d   30 d   40 d     
                                  Polar coord's  0.004  0.007  0.010  0.013     
                                  UT1-UTC        0.0014 0.0024 0.0032 0.0040    
                                                                                
                     MJD      x(arcsec)   y(arcsec)   UT1-UTC(sec)              
-       2023  5  5  60069       0.0338      0.4777     -0.03679         
-       2023  5  6  60070       0.0359      0.4789     -0.03735         
-       2023  5  7  60071       0.0381      0.4802     -0.03771         
-       2023  5  8  60072       0.0405      0.4816     -0.03790         
-       2023  5  9  60073       0.0428      0.4831     -0.03799         
-       2023  5 10  60074       0.0453      0.4845     -0.03806         
-       2023  5 11  60075       0.0477      0.4859     -0.03822         
-       2023  5 12  60076       0.0502      0.4872     -0.03857         
-       2023  5 13  60077       0.0526      0.4884     -0.03915         
-       2023  5 14  60078       0.0551      0.4896     -0.03993         
-       2023  5 15  60079       0.0576      0.4908     -0.04082         
-       2023  5 16  60080       0.0601      0.4919     -0.04170         
-       2023  5 17  60081       0.0626      0.4930     -0.04244         
-       2023  5 18  60082       0.0652      0.4940     -0.04297         
-       2023  5 19  60083       0.0678      0.4949     -0.04322         
-       2023  5 20  60084       0.0704      0.4959     -0.04316         
-       2023  5 21  60085       0.0731      0.4968     -0.04283         
-       2023  5 22  60086       0.0757      0.4977     -0.04229         
-       2023  5 23  60087       0.0784      0.4986     -0.04161         
-       2023  5 24  60088       0.0811      0.4994     -0.04090         
-       2023  5 25  60089       0.0839      0.5002     -0.04023         
-       2023  5 26  60090       0.0866      0.5009     -0.03968         
-       2023  5 27  60091       0.0893      0.5016     -0.03928         
-       2023  5 28  60092       0.0920      0.5023     -0.03904         
-       2023  5 29  60093       0.0948      0.5029     -0.03895         
-       2023  5 30  60094       0.0975      0.5035     -0.03897         
-       2023  5 31  60095       0.1003      0.5040     -0.03902         
-       2023  6  1  60096       0.1031      0.5045     -0.03902         
-       2023  6  2  60097       0.1059      0.5050     -0.03887         
-       2023  6  3  60098       0.1086      0.5054     -0.03851         
-       2023  6  4  60099       0.1114      0.5058     -0.03790         
-       2023  6  5  60100       0.1142      0.5061     -0.03706         
-       2023  6  6  60101       0.1170      0.5064     -0.03610         
-       2023  6  7  60102       0.1198      0.5066     -0.03516         
-       2023  6  8  60103       0.1226      0.5068     -0.03437         
-       2023  6  9  60104       0.1254      0.5070     -0.03381         
-       2023  6 10  60105       0.1282      0.5071     -0.03349         
-       2023  6 11  60106       0.1310      0.5072     -0.03337         
-       2023  6 12  60107       0.1338      0.5072     -0.03333         
-       2023  6 13  60108       0.1366      0.5072     -0.03325         
-       2023  6 14  60109       0.1394      0.5071     -0.03302         
-       2023  6 15  60110       0.1422      0.5070     -0.03256         
-       2023  6 16  60111       0.1450      0.5069     -0.03185         
-       2023  6 17  60112       0.1478      0.5067     -0.03089         
-       2023  6 18  60113       0.1506      0.5065     -0.02974         
-       2023  6 19  60114       0.1533      0.5062     -0.02848         
-       2023  6 20  60115       0.1561      0.5059     -0.02718         
-       2023  6 21  60116       0.1588      0.5056     -0.02592         
-       2023  6 22  60117       0.1616      0.5052     -0.02476         
-       2023  6 23  60118       0.1643      0.5048     -0.02375         
-       2023  6 24  60119       0.1670      0.5043     -0.02290         
-       2023  6 25  60120       0.1697      0.5038     -0.02220         
-       2023  6 26  60121       0.1724      0.5032     -0.02162         
-       2023  6 27  60122       0.1751      0.5026     -0.02110         
-       2023  6 28  60123       0.1778      0.5020     -0.02057         
-       2023  6 29  60124       0.1805      0.5013     -0.01996         
-       2023  6 30  60125       0.1831      0.5006     -0.01918         
-       2023  7  1  60126       0.1857      0.4999     -0.01818         
-       2023  7  2  60127       0.1884      0.4991     -0.01697         
-       2023  7  3  60128       0.1910      0.4983     -0.01561         
-       2023  7  4  60129       0.1935      0.4974     -0.01423         
-       2023  7  5  60130       0.1961      0.4965     -0.01297         
-       2023  7  6  60131       0.1987      0.4955     -0.01196         
-       2023  7  7  60132       0.2012      0.4945     -0.01122         
-       2023  7  8  60133       0.2037      0.4935     -0.01071         
-       2023  7  9  60134       0.2062      0.4925     -0.01031         
-       2023  7 10  60135       0.2086      0.4914     -0.00988         
-       2023  7 11  60136       0.2111      0.4902     -0.00930         
-       2023  7 12  60137       0.2135      0.4891     -0.00850         
-       2023  7 13  60138       0.2159      0.4879     -0.00745         
-       2023  7 14  60139       0.2183      0.4866     -0.00618         
-       2023  7 15  60140       0.2206      0.4853     -0.00472         
-       2023  7 16  60141       0.2230      0.4840     -0.00314         
-       2023  7 17  60142       0.2253      0.4827     -0.00153         
-       2023  7 18  60143       0.2275      0.4813      0.00003         
-       2023  7 19  60144       0.2298      0.4799      0.00148         
-       2023  7 20  60145       0.2320      0.4784      0.00278         
-       2023  7 21  60146       0.2342      0.4770      0.00389         
-       2023  7 22  60147       0.2364      0.4754      0.00483         
-       2023  7 23  60148       0.2385      0.4739      0.00563         
-       2023  7 24  60149       0.2406      0.4723      0.00635         
-       2023  7 25  60150       0.2427      0.4707      0.00705         
-       2023  7 26  60151       0.2447      0.4691      0.00780         
-       2023  7 27  60152       0.2468      0.4674      0.00867         
-       2023  7 28  60153       0.2487      0.4657      0.00971         
-       2023  7 29  60154       0.2507      0.4640      0.01094         
-       2023  7 30  60155       0.2526      0.4622      0.01233         
-       2023  7 31  60156       0.2545      0.4605      0.01376         
-       2023  8  1  60157       0.2564      0.4587      0.01509         
-       2023  8  2  60158       0.2582      0.4568      0.01618         
-       2023  8  3  60159       0.2600      0.4550      0.01695         
-       2023  8  4  60160       0.2617      0.4531      0.01741         
-       2023  8  5  60161       0.2635      0.4512      0.01768         
-       2023  8  6  60162       0.2651      0.4492      0.01790         
-       2023  8  7  60163       0.2668      0.4472      0.01824         
-       2023  8  8  60164       0.2684      0.4453      0.01879         
-       2023  8  9  60165       0.2700      0.4433      0.01962         
-       2023  8 10  60166       0.2715      0.4412      0.02069         
-       2023  8 11  60167       0.2730      0.4392      0.02195         
-       2023  8 12  60168       0.2745      0.4371      0.02333         
-       2023  8 13  60169       0.2759      0.4350      0.02474         
-       2023  8 14  60170       0.2773      0.4329      0.02611         
-       2023  8 15  60171       0.2787      0.4307      0.02737         
-       2023  8 16  60172       0.2800      0.4286      0.02847         
-       2023  8 17  60173       0.2813      0.4264      0.02937         
-       2023  8 18  60174       0.2825      0.4242      0.03009         
-       2023  8 19  60175       0.2837      0.4220      0.03065         
-       2023  8 20  60176       0.2849      0.4198      0.03109         
-       2023  8 21  60177       0.2860      0.4175      0.03150         
-       2023  8 22  60178       0.2871      0.4153      0.03193         
-       2023  8 23  60179       0.2881      0.4130      0.03246         
-       2023  8 24  60180       0.2891      0.4107      0.03314         
-       2023  8 25  60181       0.2901      0.4084      0.03399         
-       2023  8 26  60182       0.2910      0.4061      0.03499         
-       2023  8 27  60183       0.2918      0.4038      0.03607         
-       2023  8 28  60184       0.2927      0.4014      0.03708         
-       2023  8 29  60185       0.2935      0.3991      0.03790         
-       2023  8 30  60186       0.2942      0.3967      0.03839         
-       2023  8 31  60187       0.2949      0.3944      0.03853         
-       2023  9  1  60188       0.2956      0.3920      0.03839         
-       2023  9  2  60189       0.2962      0.3896      0.03810         
-       2023  9  3  60190       0.2968      0.3872      0.03786         
-       2023  9  4  60191       0.2973      0.3848      0.03781         
-       2023  9  5  60192       0.2978      0.3824      0.03804         
-       2023  9  6  60193       0.2983      0.3800      0.03855         
-       2023  9  7  60194       0.2987      0.3776      0.03929         
-       2023  9  8  60195       0.2991      0.3752      0.04018         
-       2023  9  9  60196       0.2994      0.3727      0.04114         
-       2023  9 10  60197       0.2997      0.3703      0.04206         
-       2023  9 11  60198       0.2999      0.3679      0.04289         
-       2023  9 12  60199       0.3001      0.3654      0.04356         
-       2023  9 13  60200       0.3003      0.3630      0.04405         
-       2023  9 14  60201       0.3004      0.3606      0.04434         
-       2023  9 15  60202       0.3005      0.3581      0.04446         
-       2023  9 16  60203       0.3005      0.3557      0.04446         
-       2023  9 17  60204       0.3005      0.3533      0.04439         
-       2023  9 18  60205       0.3004      0.3508      0.04435         
-       2023  9 19  60206       0.3003      0.3484      0.04440         
-       2023  9 20  60207       0.3002      0.3460      0.04459         
-       2023  9 21  60208       0.3000      0.3436      0.04496         
-       2023  9 22  60209       0.2998      0.3411      0.04549         
-       2023  9 23  60210       0.2995      0.3387      0.04612         
-       2023  9 24  60211       0.2992      0.3363      0.04675         
-       2023  9 25  60212       0.2989      0.3339      0.04723         
-       2023  9 26  60213       0.2985      0.3315      0.04744         
-       2023  9 27  60214       0.2980      0.3291      0.04731         
-       2023  9 28  60215       0.2976      0.3268      0.04684         
-       2023  9 29  60216       0.2971      0.3244      0.04614         
-       2023  9 30  60217       0.2965      0.3220      0.04539         
-       2023 10  1  60218       0.2959      0.3197      0.04475         
-       2023 10  2  60219       0.2953      0.3174      0.04437         
-       2023 10  3  60220       0.2946      0.3150      0.04429         
-       2023 10  4  60221       0.2939      0.3127      0.04448         
-       2023 10  5  60222       0.2931      0.3104      0.04487         
-       2023 10  6  60223       0.2923      0.3081      0.04537         
-       2023 10  7  60224       0.2915      0.3059      0.04587         
-       2023 10  8  60225       0.2906      0.3036      0.04630         
-       2023 10  9  60226       0.2897      0.3014      0.04660         
-       2023 10 10  60227       0.2888      0.2992      0.04672         
-       2023 10 11  60228       0.2878      0.2969      0.04665         
-       2023 10 12  60229       0.2868      0.2947      0.04640         
-       2023 10 13  60230       0.2857      0.2926      0.04602         
-       2023 10 14  60231       0.2846      0.2904      0.04557         
-       2023 10 15  60232       0.2835      0.2883      0.04512         
-       2023 10 16  60233       0.2824      0.2862      0.04475         
-       2023 10 17  60234       0.2812      0.2841      0.04454         
-       2023 10 18  60235       0.2799      0.2820      0.04451         
-       2023 10 19  60236       0.2786      0.2799      0.04468         
-       2023 10 20  60237       0.2773      0.2779      0.04498         
-       2023 10 21  60238       0.2760      0.2759      0.04532         
-       2023 10 22  60239       0.2746      0.2739      0.04557         
-       2023 10 23  60240       0.2732      0.2719      0.04562         
-       2023 10 24  60241       0.2718      0.2699      0.04538         
-       2023 10 25  60242       0.2703      0.2680      0.04483         
-       2023 10 26  60243       0.2688      0.2661      0.04402         
-       2023 10 27  60244       0.2673      0.2642      0.04309         
-       2023 10 28  60245       0.2657      0.2624      0.04220         
-       2023 10 29  60246       0.2641      0.2605      0.04150         
-       2023 10 30  60247       0.2625      0.2587      0.04109         
-       2023 10 31  60248       0.2609      0.2570      0.04098         
-       2023 11  1  60249       0.2592      0.2552      0.04112         
-       2023 11  2  60250       0.2575      0.2535      0.04142         
-       2023 11  3  60251       0.2558      0.2518      0.04177         
-       2023 11  4  60252       0.2540      0.2501      0.04208         
-       2023 11  5  60253       0.2522      0.2485      0.04229         
-       2023 11  6  60254       0.2504      0.2469      0.04233         
-       2023 11  7  60255       0.2486      0.2453      0.04219         
-       2023 11  8  60256       0.2467      0.2438      0.04188         
-       2023 11  9  60257       0.2448      0.2423      0.04141         
-       2023 11 10  60258       0.2429      0.2408      0.04085         
-       2023 11 11  60259       0.2409      0.2393      0.04026         
-       2023 11 12  60260       0.2390      0.2379      0.03972         
-       2023 11 13  60261       0.2370      0.2365      0.03932         
-       2023 11 14  60262       0.2350      0.2351      0.03912         
-       2023 11 15  60263       0.2330      0.2338      0.03911         
-       2023 11 16  60264       0.2309      0.2325      0.03927         
-       2023 11 17  60265       0.2289      0.2312      0.03949         
-       2023 11 18  60266       0.2268      0.2300      0.03965         
-       2023 11 19  60267       0.2247      0.2288      0.03962         
-       2023 11 20  60268       0.2226      0.2276      0.03934         
-       2023 11 21  60269       0.2204      0.2265      0.03876         
-       2023 11 22  60270       0.2183      0.2254      0.03793         
-       2023 11 23  60271       0.2161      0.2243      0.03697         
-       2023 11 24  60272       0.2139      0.2233      0.03600         
-       2023 11 25  60273       0.2117      0.2223      0.03517         
-       2023 11 26  60274       0.2095      0.2213      0.03459         
-       2023 11 27  60275       0.2073      0.2204      0.03431         
-       2023 11 28  60276       0.2050      0.2195      0.03429         
-       2023 11 29  60277       0.2028      0.2187      0.03445         
-       2023 11 30  60278       0.2005      0.2178      0.03469         
-       2023 12  1  60279       0.1983      0.2171      0.03493         
-       2023 12  2  60280       0.1960      0.2163      0.03508         
-       2023 12  3  60281       0.1937      0.2156      0.03510         
-       2023 12  4  60282       0.1914      0.2149      0.03496         
-       2023 12  5  60283       0.1891      0.2143      0.03468         
-       2023 12  6  60284       0.1867      0.2137      0.03431         
-       2023 12  7  60285       0.1844      0.2131      0.03391         
-       2023 12  8  60286       0.1821      0.2126      0.03355         
-       2023 12  9  60287       0.1797      0.2121      0.03329         
-       2023 12 10  60288       0.1774      0.2116      0.03316         
-       2023 12 11  60289       0.1751      0.2112      0.03320         
-       2023 12 12  60290       0.1727      0.2108      0.03344         
-       2023 12 13  60291       0.1704      0.2105      0.03391         
-       2023 12 14  60292       0.1680      0.2101      0.03453         
-       2023 12 15  60293       0.1656      0.2099      0.03521         
-       2023 12 16  60294       0.1633      0.2096      0.03576         
-       2023 12 17  60295       0.1609      0.2094      0.03608         
-       2023 12 18  60296       0.1586      0.2093      0.03608         
-       2023 12 19  60297       0.1562      0.2091      0.03578         
-       2023 12 20  60298       0.1538      0.2090      0.03536         
-       2023 12 21  60299       0.1515      0.2090      0.03500         
-       2023 12 22  60300       0.1491      0.2090      0.03474         
-       2023 12 23  60301       0.1468      0.2090      0.03468         
-       2023 12 24  60302       0.1444      0.2090      0.03493         
-       2023 12 25  60303       0.1421      0.2091      0.03542         
-       2023 12 26  60304       0.1398      0.2093      0.03620         
-       2023 12 27  60305       0.1374      0.2094      0.03713         
-       2023 12 28  60306       0.1351      0.2096      0.03807         
-       2023 12 29  60307       0.1328      0.2099      0.03893         
-       2023 12 30  60308       0.1305      0.2101      0.03962         
-       2023 12 31  60309       0.1282      0.2104      0.04014         
-       2024  1  1  60310       0.1259      0.2108      0.04052         
-       2024  1  2  60311       0.1236      0.2112      0.04065         
-       2024  1  3  60312       0.1214      0.2116      0.04061         
-       2024  1  4  60313       0.1191      0.2120      0.04054         
-       2024  1  5  60314       0.1169      0.2125      0.04040         
-       2024  1  6  60315       0.1146      0.2130      0.04037         
-       2024  1  7  60316       0.1124      0.2136      0.04041         
-       2024  1  8  60317       0.1102      0.2142      0.04063         
-       2024  1  9  60318       0.1080      0.2148      0.04098         
-       2024  1 10  60319       0.1058      0.2154      0.04148         
-       2024  1 11  60320       0.1037      0.2161      0.04201         
-       2024  1 12  60321       0.1015      0.2168      0.04241         
-       2024  1 13  60322       0.0994      0.2176      0.04256         
-       2024  1 14  60323       0.0973      0.2184      0.04243         
-       2024  1 15  60324       0.0952      0.2192      0.04193         
-       2024  1 16  60325       0.0931      0.2200      0.04126         
-       2024  1 17  60326       0.0911      0.2209      0.04059         
-       2024  1 18  60327       0.0890      0.2218      0.04003         
-       2024  1 19  60328       0.0870      0.2228      0.03971         
-       2024  1 20  60329       0.0850      0.2238      0.03970         
-       2024  1 21  60330       0.0830      0.2248      0.04001         
-       2024  1 22  60331       0.0811      0.2258      0.04057         
-       2024  1 23  60332       0.0791      0.2269      0.04133         
-       2024  1 24  60333       0.0772      0.2280      0.04216         
-       2024  1 25  60334       0.0753      0.2291      0.04297         
-       2024  1 26  60335       0.0735      0.2302      0.04366         
-       2024  1 27  60336       0.0716      0.2314      0.04419         
-       2024  1 28  60337       0.0698      0.2326      0.04448         
-       2024  1 29  60338       0.0680      0.2339      0.04454         
-       2024  1 30  60339       0.0662      0.2351      0.04458         
-       2024  1 31  60340       0.0645      0.2364      0.04458         
-       2024  2  1  60341       0.0628      0.2377      0.04465         
-       2024  2  2  60342       0.0611      0.2391      0.04474         
-       2024  2  3  60343       0.0594      0.2404      0.04498         
-       2024  2  4  60344       0.0578      0.2418      0.04530         
-       2024  2  5  60345       0.0562      0.2432      0.04578         
-       2024  2  6  60346       0.0546      0.2447      0.04636         
-       2024  2  7  60347       0.0530      0.2461      0.04691         
-       2024  2  8  60348       0.0515      0.2476      0.04732         
-       2024  2  9  60349       0.0500      0.2491      0.04746         
-       2024  2 10  60350       0.0486      0.2507      0.04719         
-       2024  2 11  60351       0.0471      0.2522      0.04658         
-       2024  2 12  60352       0.0457      0.2538      0.04572         
-       2024  2 13  60353       0.0444      0.2554      0.04475         
-       2024  2 14  60354       0.0430      0.2570      0.04386         
-       2024  2 15  60355       0.0417      0.2586      0.04322         
-       2024  2 16  60356       0.0404      0.2603      0.04284         
-       2024  2 17  60357       0.0392      0.2620      0.04279         
-       2024  2 18  60358       0.0380      0.2637      0.04297         
-       2024  2 19  60359       0.0368      0.2654      0.04329         
-       2024  2 20  60360       0.0356      0.2671      0.04363         
-       2024  2 21  60361       0.0345      0.2689      0.04401         
-       2024  2 22  60362       0.0334      0.2706      0.04425         
-       2024  2 23  60363       0.0324      0.2724      0.04437         
-       2024  2 24  60364       0.0314      0.2742      0.04432         
-       2024  2 25  60365       0.0304      0.2760      0.04403         
-       2024  2 26  60366       0.0294      0.2778      0.04356         
-       2024  2 27  60367       0.0285      0.2796      0.04303         
-       2024  2 28  60368       0.0277      0.2815      0.04256         
-       2024  2 29  60369       0.0268      0.2833      0.04216         
-       2024  3  1  60370       0.0260      0.2852      0.04191         
-       2024  3  2  60371       0.0252      0.2871      0.04181         
-       2024  3  3  60372       0.0245      0.2890      0.04189         
-       2024  3  4  60373       0.0238      0.2909      0.04217         
-       2024  3  5  60374       0.0231      0.2928      0.04252         
-       2024  3  6  60375       0.0225      0.2947      0.04286         
-       2024  3  7  60376       0.0219      0.2967      0.04303         
-       2024  3  8  60377       0.0213      0.2986      0.04290         
-       2024  3  9  60378       0.0208      0.3005      0.04238         
-       2024  3 10  60379       0.0203      0.3025      0.04157         
-       2024  3 11  60380       0.0199      0.3044      0.04043         
-       2024  3 12  60381       0.0195      0.3064      0.03926         
-       2024  3 13  60382       0.0191      0.3084      0.03829         
-       2024  3 14  60383       0.0188      0.3104      0.03760         
-       2024  3 15  60384       0.0185      0.3123      0.03722         
-       2024  3 16  60385       0.0182      0.3143      0.03709         
-       2024  3 17  60386       0.0180      0.3163      0.03717         
-       2024  3 18  60387       0.0178      0.3183      0.03732         
-       2024  3 19  60388       0.0176      0.3203      0.03748         
-       2024  3 20  60389       0.0175      0.3223      0.03762         
-       2024  3 21  60390       0.0174      0.3242      0.03770         
-       2024  3 22  60391       0.0173      0.3262      0.03758         
-       2024  3 23  60392       0.0173      0.3282      0.03732         
-       2024  3 24  60393       0.0174      0.3302      0.03693         
-       2024  3 25  60394       0.0174      0.3322      0.03644         
-       2024  3 26  60395       0.0175      0.3342      0.03592         
-       2024  3 27  60396       0.0176      0.3362      0.03551         
-       2024  3 28  60397       0.0178      0.3381      0.03521         
-       2024  3 29  60398       0.0180      0.3401      0.03508         
-       2024  3 30  60399       0.0182      0.3421      0.03517         
-       2024  3 31  60400       0.0185      0.3440      0.03539         
-       2024  4  1  60401       0.0188      0.3460      0.03575         
-       2024  4  2  60402       0.0192      0.3480      0.03616         
-       2024  4  3  60403       0.0195      0.3499      0.03650         
-       2024  4  4  60404       0.0200      0.3518      0.03662         
-       2024  4  5  60405       0.0204      0.3538      0.03643         
-       2024  4  6  60406       0.0209      0.3557      0.03592         
-       2024  4  7  60407       0.0214      0.3576      0.03509         
-       2024  4  8  60408       0.0219      0.3595      0.03406         
-       2024  4  9  60409       0.0225      0.3614      0.03306         
-       2024  4 10  60410       0.0231      0.3633      0.03228         
-       2024  4 11  60411       0.0238      0.3652      0.03186         
-       2024  4 12  60412       0.0245      0.3670      0.03180         
-       2024  4 13  60413       0.0252      0.3689      0.03200         
-       2024  4 14  60414       0.0259      0.3707      0.03238         
-       2024  4 15  60415       0.0267      0.3725      0.03272         
-       2024  4 16  60416       0.0275      0.3743      0.03302         
-       2024  4 17  60417       0.0284      0.3761      0.03320         
-       2024  4 18  60418       0.0292      0.3779      0.03319         
-       2024  4 19  60419       0.0302      0.3797      0.03302         
-       2024  4 20  60420       0.0311      0.3814      0.03277         
-       2024  4 21  60421       0.0321      0.3832      0.03239         
-       2024  4 22  60422       0.0331      0.3849      0.03199         
-       2024  4 23  60423       0.0341      0.3866      0.03159         
-       2024  4 24  60424       0.0351      0.3883      0.03124         
-       2024  4 25  60425       0.0362      0.3900      0.03100         
-       2024  4 26  60426       0.0373      0.3916      0.03088         
-       2024  4 27  60427       0.0385      0.3932      0.03092         
-       2024  4 28  60428       0.0396      0.3949      0.03111         
-       2024  4 29  60429       0.0408      0.3964      0.03137         
-       2024  4 30  60430       0.0421      0.3980      0.03158         
-       2024  5  1  60431       0.0433      0.3996      0.03161         
-       2024  5  2  60432       0.0446      0.4011      0.03136         
-       2024  5  3  60433       0.0459      0.4026      0.03077         
+       2023  6  9  60104       0.1191      0.5119     -0.04401         
+       2023  6 10  60105       0.1215      0.5121     -0.04415         
+       2023  6 11  60106       0.1239      0.5123     -0.04445         
+       2023  6 12  60107       0.1264      0.5124     -0.04479         
+       2023  6 13  60108       0.1290      0.5124     -0.04506         
+       2023  6 14  60109       0.1317      0.5124     -0.04517         
+       2023  6 15  60110       0.1345      0.5124     -0.04504         
+       2023  6 16  60111       0.1372      0.5123     -0.04467         
+       2023  6 17  60112       0.1400      0.5122     -0.04404         
+       2023  6 18  60113       0.1428      0.5121     -0.04321         
+       2023  6 19  60114       0.1455      0.5119     -0.04229         
+       2023  6 20  60115       0.1483      0.5117     -0.04135         
+       2023  6 21  60116       0.1510      0.5114     -0.04047         
+       2023  6 22  60117       0.1537      0.5111     -0.03970         
+       2023  6 23  60118       0.1564      0.5107     -0.03907         
+       2023  6 24  60119       0.1591      0.5103     -0.03858         
+       2023  6 25  60120       0.1617      0.5099     -0.03824         
+       2023  6 26  60121       0.1644      0.5094     -0.03801         
+       2023  6 27  60122       0.1671      0.5088     -0.03784         
+       2023  6 28  60123       0.1697      0.5083     -0.03768         
+       2023  6 29  60124       0.1724      0.5076     -0.03746         
+       2023  6 30  60125       0.1750      0.5070     -0.03711         
+       2023  7  1  60126       0.1777      0.5063     -0.03658         
+       2023  7  2  60127       0.1803      0.5056     -0.03587         
+       2023  7  3  60128       0.1829      0.5048     -0.03505         
+       2023  7  4  60129       0.1855      0.5040     -0.03424         
+       2023  7  5  60130       0.1880      0.5031     -0.03357         
+       2023  7  6  60131       0.1906      0.5022     -0.03315         
+       2023  7  7  60132       0.1931      0.5013     -0.03298         
+       2023  7  8  60133       0.1956      0.5004     -0.03302         
+       2023  7  9  60134       0.1981      0.4994     -0.03314         
+       2023  7 10  60135       0.2006      0.4983     -0.03320         
+       2023  7 11  60136       0.2031      0.4972     -0.03309         
+       2023  7 12  60137       0.2055      0.4961     -0.03273         
+       2023  7 13  60138       0.2079      0.4950     -0.03210         
+       2023  7 14  60139       0.2103      0.4938     -0.03119         
+       2023  7 15  60140       0.2127      0.4926     -0.03008         
+       2023  7 16  60141       0.2150      0.4913     -0.02882         
+       2023  7 17  60142       0.2173      0.4900     -0.02751         
+       2023  7 18  60143       0.2196      0.4887     -0.02622         
+       2023  7 19  60144       0.2219      0.4873     -0.02503         
+       2023  7 20  60145       0.2241      0.4859     -0.02398         
+       2023  7 21  60146       0.2263      0.4845     -0.02310         
+       2023  7 22  60147       0.2285      0.4830     -0.02237         
+       2023  7 23  60148       0.2307      0.4815     -0.02176         
+       2023  7 24  60149       0.2328      0.4800     -0.02122         
+       2023  7 25  60150       0.2349      0.4784     -0.02070         
+       2023  7 26  60151       0.2370      0.4769     -0.02011         
+       2023  7 27  60152       0.2390      0.4752     -0.01940         
+       2023  7 28  60153       0.2411      0.4736     -0.01849         
+       2023  7 29  60154       0.2431      0.4719     -0.01738         
+       2023  7 30  60155       0.2450      0.4702     -0.01612         
+       2023  7 31  60156       0.2469      0.4685     -0.01480         
+       2023  8  1  60157       0.2488      0.4667     -0.01358         
+       2023  8  2  60158       0.2507      0.4649     -0.01260         
+       2023  8  3  60159       0.2525      0.4631     -0.01195         
+       2023  8  4  60160       0.2543      0.4612     -0.01160         
+       2023  8  5  60161       0.2561      0.4594     -0.01145         
+       2023  8  6  60162       0.2578      0.4575     -0.01134         
+       2023  8  7  60163       0.2595      0.4555     -0.01112         
+       2023  8  8  60164       0.2611      0.4536     -0.01066         
+       2023  8  9  60165       0.2628      0.4516     -0.00994         
+       2023  8 10  60166       0.2643      0.4496     -0.00896         
+       2023  8 11  60167       0.2659      0.4476     -0.00779         
+       2023  8 12  60168       0.2674      0.4456     -0.00649         
+       2023  8 13  60169       0.2689      0.4435     -0.00515         
+       2023  8 14  60170       0.2703      0.4414     -0.00385         
+       2023  8 15  60171       0.2717      0.4393     -0.00264         
+       2023  8 16  60172       0.2731      0.4372     -0.00160         
+       2023  8 17  60173       0.2744      0.4351     -0.00073         
+       2023  8 18  60174       0.2757      0.4329     -0.00005         
+       2023  8 19  60175       0.2769      0.4307      0.00048         
+       2023  8 20  60176       0.2782      0.4285      0.00091         
+       2023  8 21  60177       0.2793      0.4263      0.00130         
+       2023  8 22  60178       0.2805      0.4241      0.00173         
+       2023  8 23  60179       0.2815      0.4218      0.00225         
+       2023  8 24  60180       0.2826      0.4196      0.00293         
+       2023  8 25  60181       0.2836      0.4173      0.00379         
+       2023  8 26  60182       0.2846      0.4150      0.00481         
+       2023  8 27  60183       0.2855      0.4127      0.00590         
+       2023  8 28  60184       0.2864      0.4104      0.00695         
+       2023  8 29  60185       0.2873      0.4080      0.00780         
+       2023  8 30  60186       0.2881      0.4057      0.00833         
+       2023  8 31  60187       0.2888      0.4034      0.00850         
+       2023  9  1  60188       0.2896      0.4010      0.00839         
+       2023  9  2  60189       0.2902      0.3986      0.00813         
+       2023  9  3  60190       0.2909      0.3963      0.00791         
+       2023  9  4  60191       0.2915      0.3939      0.00788         
+       2023  9  5  60192       0.2921      0.3915      0.00812         
+       2023  9  6  60193       0.2926      0.3891      0.00865         
+       2023  9  7  60194       0.2930      0.3867      0.00940         
+       2023  9  8  60195       0.2935      0.3843      0.01029         
+       2023  9  9  60196       0.2939      0.3818      0.01124         
+       2023  9 10  60197       0.2942      0.3794      0.01216         
+       2023  9 11  60198       0.2945      0.3770      0.01298         
+       2023  9 12  60199       0.2948      0.3746      0.01364         
+       2023  9 13  60200       0.2950      0.3722      0.01411         
+       2023  9 14  60201       0.2952      0.3697      0.01439         
+       2023  9 15  60202       0.2954      0.3673      0.01450         
+       2023  9 16  60203       0.2955      0.3649      0.01449         
+       2023  9 17  60204       0.2955      0.3624      0.01442         
+       2023  9 18  60205       0.2955      0.3600      0.01437         
+       2023  9 19  60206       0.2955      0.3576      0.01441         
+       2023  9 20  60207       0.2954      0.3551      0.01459         
+       2023  9 21  60208       0.2953      0.3527      0.01496         
+       2023  9 22  60209       0.2952      0.3503      0.01548         
+       2023  9 23  60210       0.2950      0.3479      0.01611         
+       2023  9 24  60211       0.2948      0.3455      0.01673         
+       2023  9 25  60212       0.2945      0.3431      0.01712         
+       2023  9 26  60213       0.2942      0.3407      0.01725         
+       2023  9 27  60214       0.2938      0.3383      0.01703         
+       2023  9 28  60215       0.2934      0.3359      0.01648         
+       2023  9 29  60216       0.2930      0.3335      0.01570         
+       2023  9 30  60217       0.2925      0.3312      0.01487         
+       2023 10  1  60218       0.2920      0.3288      0.01415         
+       2023 10  2  60219       0.2914      0.3264      0.01369         
+       2023 10  3  60220       0.2909      0.3241      0.01353         
+       2023 10  4  60221       0.2902      0.3218      0.01366         
+       2023 10  5  60222       0.2895      0.3195      0.01398         
+       2023 10  6  60223       0.2888      0.3172      0.01441         
+       2023 10  7  60224       0.2881      0.3149      0.01485         
+       2023 10  8  60225       0.2873      0.3126      0.01522         
+       2023 10  9  60226       0.2865      0.3103      0.01546         
+       2023 10 10  60227       0.2856      0.3081      0.01552         
+       2023 10 11  60228       0.2847      0.3059      0.01540         
+       2023 10 12  60229       0.2838      0.3036      0.01510         
+       2023 10 13  60230       0.2828      0.3014      0.01467         
+       2023 10 14  60231       0.2818      0.2993      0.01416         
+       2023 10 15  60232       0.2807      0.2971      0.01366         
+       2023 10 16  60233       0.2796      0.2949      0.01324         
+       2023 10 17  60234       0.2785      0.2928      0.01297         
+       2023 10 18  60235       0.2773      0.2907      0.01289         
+       2023 10 19  60236       0.2762      0.2886      0.01300         
+       2023 10 20  60237       0.2749      0.2865      0.01325         
+       2023 10 21  60238       0.2737      0.2845      0.01353         
+       2023 10 22  60239       0.2724      0.2825      0.01373         
+       2023 10 23  60240       0.2711      0.2805      0.01373         
+       2023 10 24  60241       0.2697      0.2785      0.01344         
+       2023 10 25  60242       0.2683      0.2765      0.01283         
+       2023 10 26  60243       0.2669      0.2746      0.01197         
+       2023 10 27  60244       0.2654      0.2727      0.01099         
+       2023 10 28  60245       0.2639      0.2708      0.01005         
+       2023 10 29  60246       0.2624      0.2689      0.00931         
+       2023 10 30  60247       0.2609      0.2671      0.00885         
+       2023 10 31  60248       0.2593      0.2653      0.00870         
+       2023 11  1  60249       0.2577      0.2635      0.00880         
+       2023 11  2  60250       0.2561      0.2617      0.00906         
+       2023 11  3  60251       0.2544      0.2600      0.00939         
+       2023 11  4  60252       0.2527      0.2583      0.00968         
+       2023 11  5  60253       0.2510      0.2566      0.00986         
+       2023 11  6  60254       0.2493      0.2549      0.00990         
+       2023 11  7  60255       0.2475      0.2533      0.00976         
+       2023 11  8  60256       0.2457      0.2517      0.00946         
+       2023 11  9  60257       0.2439      0.2502      0.00903         
+       2023 11 10  60258       0.2420      0.2486      0.00851         
+       2023 11 11  60259       0.2402      0.2471      0.00797         
+       2023 11 12  60260       0.2383      0.2456      0.00750         
+       2023 11 13  60261       0.2364      0.2442      0.00717         
+       2023 11 14  60262       0.2344      0.2428      0.00704         
+       2023 11 15  60263       0.2325      0.2414      0.00712         
+       2023 11 16  60264       0.2305      0.2401      0.00737         
+       2023 11 17  60265       0.2285      0.2387      0.00770         
+       2023 11 18  60266       0.2265      0.2374      0.00799         
+       2023 11 19  60267       0.2245      0.2362      0.00812         
+       2023 11 20  60268       0.2224      0.2350      0.00800         
+       2023 11 21  60269       0.2203      0.2338      0.00760         
+       2023 11 22  60270       0.2183      0.2326      0.00696         
+       2023 11 23  60271       0.2161      0.2315      0.00618         
+       2023 11 24  60272       0.2140      0.2304      0.00540         
+       2023 11 25  60273       0.2119      0.2294      0.00477         
+       2023 11 26  60274       0.2097      0.2283      0.00437         
+       2023 11 27  60275       0.2076      0.2274      0.00427         
+       2023 11 28  60276       0.2054      0.2264      0.00445         
+       2023 11 29  60277       0.2032      0.2255      0.00482         
+       2023 11 30  60278       0.2010      0.2246      0.00530         
+       2023 12  1  60279       0.1988      0.2238      0.00578         
+       2023 12  2  60280       0.1965      0.2230      0.00620         
+       2023 12  3  60281       0.1943      0.2222      0.00648         
+       2023 12  4  60282       0.1920      0.2214      0.00661         
+       2023 12  5  60283       0.1898      0.2207      0.00659         
+       2023 12  6  60284       0.1875      0.2201      0.00643         
+       2023 12  7  60285       0.1852      0.2194      0.00619         
+       2023 12  8  60286       0.1830      0.2189      0.00592         
+       2023 12  9  60287       0.1807      0.2183      0.00569         
+       2023 12 10  60288       0.1784      0.2178      0.00559         
+       2023 12 11  60289       0.1761      0.2173      0.00568         
+       2023 12 12  60290       0.1738      0.2168      0.00599         
+       2023 12 13  60291       0.1714      0.2164      0.00650         
+       2023 12 14  60292       0.1691      0.2160      0.00715         
+       2023 12 15  60293       0.1668      0.2157      0.00779         
+       2023 12 16  60294       0.1645      0.2154      0.00830         
+       2023 12 17  60295       0.1622      0.2151      0.00857         
+       2023 12 18  60296       0.1599      0.2149      0.00853         
+       2023 12 19  60297       0.1575      0.2147      0.00823         
+       2023 12 20  60298       0.1552      0.2146      0.00775         
+       2023 12 21  60299       0.1529      0.2144      0.00723         
+       2023 12 22  60300       0.1506      0.2143      0.00681         
+       2023 12 23  60301       0.1483      0.2143      0.00661         
+       2023 12 24  60302       0.1459      0.2143      0.00669         
+       2023 12 25  60303       0.1436      0.2143      0.00705         
+       2023 12 26  60304       0.1413      0.2144      0.00763         
+       2023 12 27  60305       0.1390      0.2145      0.00836         
+       2023 12 28  60306       0.1367      0.2146      0.00912         
+       2023 12 29  60307       0.1344      0.2148      0.00983         
+       2023 12 30  60308       0.1322      0.2150      0.01041         
+       2023 12 31  60309       0.1299      0.2152      0.01082         
+       2024  1  1  60310       0.1276      0.2155      0.01106         
+       2024  1  2  60311       0.1254      0.2158      0.01113         
+       2024  1  3  60312       0.1231      0.2161      0.01107         
+       2024  1  4  60313       0.1209      0.2165      0.01092         
+       2024  1  5  60314       0.1187      0.2169      0.01075         
+       2024  1  6  60315       0.1164      0.2174      0.01061         
+       2024  1  7  60316       0.1142      0.2179      0.01057         
+       2024  1  8  60317       0.1120      0.2184      0.01069         
+       2024  1  9  60318       0.1099      0.2189      0.01098         
+       2024  1 10  60319       0.1077      0.2195      0.01141         
+       2024  1 11  60320       0.1055      0.2201      0.01188         
+       2024  1 12  60321       0.1034      0.2208      0.01224         
+       2024  1 13  60322       0.1013      0.2215      0.01235         
+       2024  1 14  60323       0.0992      0.2222      0.01217         
+       2024  1 15  60324       0.0971      0.2229      0.01170         
+       2024  1 16  60325       0.0950      0.2237      0.01105         
+       2024  1 17  60326       0.0929      0.2245      0.01036         
+       2024  1 18  60327       0.0909      0.2254      0.00979         
+       2024  1 19  60328       0.0889      0.2263      0.00943         
+       2024  1 20  60329       0.0869      0.2272      0.00931         
+       2024  1 21  60330       0.0849      0.2281      0.00934         
+       2024  1 22  60331       0.0829      0.2291      0.00962         
+       2024  1 23  60332       0.0810      0.2301      0.01002         
+       2024  1 24  60333       0.0791      0.2311      0.01042         
+       2024  1 25  60334       0.0772      0.2322      0.01078         
+       2024  1 26  60335       0.0753      0.2333      0.01096         
+       2024  1 27  60336       0.0734      0.2344      0.01099         
+       2024  1 28  60337       0.0716      0.2355      0.01096         
+       2024  1 29  60338       0.0698      0.2367      0.01083         
+       2024  1 30  60339       0.0680      0.2379      0.01062         
+       2024  1 31  60340       0.0663      0.2391      0.01032         
+       2024  2  1  60341       0.0645      0.2404      0.00996         
+       2024  2  2  60342       0.0628      0.2416      0.00967         
+       2024  2  3  60343       0.0611      0.2430      0.00950         
+       2024  2  4  60344       0.0595      0.2443      0.00941         
+       2024  2  5  60345       0.0578      0.2456      0.00948         
+       2024  2  6  60346       0.0562      0.2470      0.00968         
+       2024  2  7  60347       0.0546      0.2484      0.00989         
+       2024  2  8  60348       0.0531      0.2498      0.01006         
+       2024  2  9  60349       0.0516      0.2513      0.01006         
+       2024  2 10  60350       0.0501      0.2528      0.00970         
+       2024  2 11  60351       0.0486      0.2543      0.00898         
+       2024  2 12  60352       0.0472      0.2558      0.00797         
+       2024  2 13  60353       0.0458      0.2573      0.00685         
+       2024  2 14  60354       0.0444      0.2589      0.00588         
+       2024  2 15  60355       0.0430      0.2605      0.00521         
+       2024  2 16  60356       0.0417      0.2621      0.00491         
+       2024  2 17  60357       0.0404      0.2637      0.00496         
+       2024  2 18  60358       0.0392      0.2653      0.00524         
+       2024  2 19  60359       0.0380      0.2670      0.00566         
+       2024  2 20  60360       0.0368      0.2687      0.00612         
+       2024  2 21  60361       0.0356      0.2703      0.00659         
+       2024  2 22  60362       0.0345      0.2720      0.00699         
+       2024  2 23  60363       0.0334      0.2738      0.00729         
+       2024  2 24  60364       0.0323      0.2755      0.00743         
+       2024  2 25  60365       0.0313      0.2773      0.00739         
+       2024  2 26  60366       0.0303      0.2790      0.00717         
+       2024  2 27  60367       0.0293      0.2808      0.00681         
+       2024  2 28  60368       0.0284      0.2826      0.00644         
+       2024  2 29  60369       0.0275      0.2844      0.00621         
+       2024  3  1  60370       0.0266      0.2863      0.00605         
+       2024  3  2  60371       0.0258      0.2881      0.00604         
+       2024  3  3  60372       0.0250      0.2899      0.00624         
+       2024  3  4  60373       0.0243      0.2918      0.00658         
+       2024  3  5  60374       0.0235      0.2937      0.00709         
+       2024  3  6  60375       0.0228      0.2955      0.00762         
+       2024  3  7  60376       0.0222      0.2974      0.00798         
+       2024  3  8  60377       0.0216      0.2993      0.00804         
+       2024  3  9  60378       0.0210      0.3012      0.00768         
+       2024  3 10  60379       0.0204      0.3031      0.00697         
+       2024  3 11  60380       0.0199      0.3051      0.00607         
+       2024  3 12  60381       0.0194      0.3070      0.00502         
+       2024  3 13  60382       0.0190      0.3089      0.00406         
+       2024  3 14  60383       0.0186      0.3109      0.00341         
+       2024  3 15  60384       0.0182      0.3128      0.00301         
+       2024  3 16  60385       0.0179      0.3147      0.00293         
+       2024  3 17  60386       0.0176      0.3167      0.00297         
+       2024  3 18  60387       0.0173      0.3186      0.00311         
+       2024  3 19  60388       0.0171      0.3206      0.00319         
+       2024  3 20  60389       0.0169      0.3226      0.00320         
+       2024  3 21  60390       0.0167      0.3245      0.00306         
+       2024  3 22  60391       0.0166      0.3265      0.00274         
+       2024  3 23  60392       0.0165      0.3284      0.00223         
+       2024  3 24  60393       0.0164      0.3304      0.00161         
+       2024  3 25  60394       0.0164      0.3324      0.00081         
+       2024  3 26  60395       0.0164      0.3343      0.00000         
+       2024  3 27  60396       0.0165      0.3363     -0.00073         
+       2024  3 28  60397       0.0165      0.3382     -0.00135         
+       2024  3 29  60398       0.0167      0.3402     -0.00179         
+       2024  3 30  60399       0.0168      0.3421     -0.00200         
+       2024  3 31  60400       0.0170      0.3441     -0.00198         
+       2024  4  1  60401       0.0172      0.3460     -0.00179         
+       2024  4  2  60402       0.0175      0.3479     -0.00149         
+       2024  4  3  60403       0.0178      0.3499     -0.00124         
+       2024  4  4  60404       0.0181      0.3518     -0.00117         
+       2024  4  5  60405       0.0185      0.3537     -0.00142         
+       2024  4  6  60406       0.0188      0.3556     -0.00202         
+       2024  4  7  60407       0.0193      0.3575     -0.00295         
+       2024  4  8  60408       0.0197      0.3594     -0.00410         
+       2024  4  9  60409       0.0202      0.3613     -0.00508         
+       2024  4 10  60410       0.0207      0.3631     -0.00580         
+       2024  4 11  60411       0.0213      0.3650     -0.00610         
+       2024  4 12  60412       0.0219      0.3668     -0.00611         
+       2024  4 13  60413       0.0225      0.3687     -0.00582         
+       2024  4 14  60414       0.0232      0.3705     -0.00545         
+       2024  4 15  60415       0.0239      0.3723     -0.00505         
+       2024  4 16  60416       0.0246      0.3741     -0.00476         
+       2024  4 17  60417       0.0253      0.3759     -0.00467         
+       2024  4 18  60418       0.0261      0.3777     -0.00481         
+       2024  4 19  60419       0.0269      0.3795     -0.00516         
+       2024  4 20  60420       0.0278      0.3812     -0.00573         
+       2024  4 21  60421       0.0286      0.3830     -0.00639         
+       2024  4 22  60422       0.0295      0.3847     -0.00707         
+       2024  4 23  60423       0.0305      0.3864     -0.00770         
+       2024  4 24  60424       0.0314      0.3881     -0.00820         
+       2024  4 25  60425       0.0324      0.3897     -0.00851         
+       2024  4 26  60426       0.0334      0.3914     -0.00865         
+       2024  4 27  60427       0.0345      0.3930     -0.00855         
+       2024  4 28  60428       0.0355      0.3946     -0.00830         
+       2024  4 29  60429       0.0366      0.3962     -0.00799         
+       2024  4 30  60430       0.0377      0.3978     -0.00773         
+       2024  5  1  60431       0.0389      0.3994     -0.00755         
+       2024  5  2  60432       0.0401      0.4009     -0.00765         
+       2024  5  3  60433       0.0413      0.4024     -0.00801         
+       2024  5  4  60434       0.0425      0.4039     -0.00864         
+       2024  5  5  60435       0.0438      0.4054     -0.00953         
+       2024  5  6  60436       0.0450      0.4069     -0.01048         
+       2024  5  7  60437       0.0463      0.4083     -0.01124         
+       2024  5  8  60438       0.0477      0.4097     -0.01163         
+       2024  5  9  60439       0.0490      0.4111     -0.01166         
+       2024  5 10  60440       0.0504      0.4125     -0.01134         
+       2024  5 11  60441       0.0518      0.4138     -0.01080         
+       2024  5 12  60442       0.0532      0.4152     -0.01017         
+       2024  5 13  60443       0.0546      0.4165     -0.00951         
+       2024  5 14  60444       0.0561      0.4177     -0.00896         
+       2024  5 15  60445       0.0575      0.4190     -0.00854         
+       2024  5 16  60446       0.0590      0.4202     -0.00829         
+       2024  5 17  60447       0.0606      0.4214     -0.00819         
+       2024  5 18  60448       0.0621      0.4226     -0.00821         
+       2024  5 19  60449       0.0636      0.4237     -0.00822         
+       2024  5 20  60450       0.0652      0.4249     -0.00831         
+       2024  5 21  60451       0.0668      0.4260     -0.00830         
+       2024  5 22  60452       0.0684      0.4270     -0.00810         
+       2024  5 23  60453       0.0700      0.4281     -0.00772         
+       2024  5 24  60454       0.0717      0.4291     -0.00714         
+       2024  5 25  60455       0.0733      0.4301     -0.00643         
+       2024  5 26  60456       0.0750      0.4311     -0.00558         
+       2024  5 27  60457       0.0767      0.4320     -0.00478         
+       2024  5 28  60458       0.0784      0.4329     -0.00406         
+       2024  5 29  60459       0.0801      0.4338     -0.00349         
+       2024  5 30  60460       0.0818      0.4346     -0.00312         
+       2024  5 31  60461       0.0835      0.4355     -0.00303         
+       2024  6  1  60462       0.0853      0.4363     -0.00309         
+       2024  6  2  60463       0.0870      0.4370     -0.00320         
+       2024  6  3  60464       0.0888      0.4378     -0.00321         
+       2024  6  4  60465       0.0906      0.4385     -0.00299         
+       2024  6  5  60466       0.0923      0.4392     -0.00238         
+       2024  6  6  60467       0.0941      0.4398     -0.00147         
+       2024  6  7  60468       0.0959      0.4404     -0.00030         
       These predictions are based on all announced leap seconds.               
                                                                                
       CELESTIAL POLE OFFSET SERIES:                                            
                            NEOS Celestial Pole Offset Series                   
                        MJD      dpsi    error     deps    error                
                                         (msec. of arc)                         
-                      60047  -107.11    0.81   -9.29    0.04   
-                      60048  -106.56    0.81   -9.40    0.04   
+                      60084  -106.87    0.32   -9.47    0.16   
+                      60085  -106.93    0.32   -9.70    0.16   
+                      60086  -107.04    0.32   -9.90    0.16   
+                      60087  -107.17    0.32   -9.96    0.16   
+                      60088  -107.24    1.03   -9.93    0.02   
+                      60089  -107.20    1.03   -9.94    0.02   
+                      60090  -107.04    1.03  -10.04    0.02   
                                                                                
                      IERS Celestial Pole Offset Final Series                   
                            MJD          dpsi      deps                         
                                         (msec. of arc)                         
-                          60005      -109.4      -7.3                      
-                          60006      -109.0      -7.3                      
-                          60007      -108.6      -7.4                      
-                          60008      -108.5      -7.4                      
-                          60009      -108.5      -7.3                      
-                          60010      -108.4      -7.2                      
-                          60011      -108.4      -7.1                      
-                          60012      -108.4      -7.1                      
-                          60013      -108.6      -7.3                      
-                          60014      -108.7      -7.4                      
-                          60015      -108.8      -7.5                      
-                          60016      -108.9      -7.7                      
-                          60017      -108.8      -7.8                      
-                          60018      -108.6      -7.9                      
-                          60019      -108.4      -8.1                      
-                          60020      -108.2      -8.3                      
-                          60021      -108.1      -8.4                      
-                          60022      -107.9      -8.4                      
-                          60023      -107.8      -8.2                      
-                          60024      -107.8      -8.0                      
-                          60025      -107.8      -8.0                      
-                          60026      -107.9      -8.0                      
-                          60027      -108.1      -8.0                      
-                          60028      -108.3      -8.1                      
-                          60029      -108.5      -8.2                      
-                          60030      -108.5      -8.4                      
-                          60031      -108.4      -8.6                      
-                          60032      -108.2      -8.6                      
-                          60033      -107.8      -8.6                      
-                          60034      -107.4      -8.8                      
-                          60035      -106.9      -8.9                      
+                          60036      -106.7      -9.0                      
+                          60037      -106.8      -8.9                      
+                          60038      -107.0      -8.6                      
+                          60039      -107.2      -8.5                      
+                          60040      -107.5      -8.5                      
+                          60041      -107.7      -8.6                      
+                          60042      -107.8      -8.7                      
+                          60043      -107.9      -8.8                      
+                          60044      -108.0      -8.9                      
+                          60045      -107.9      -9.0                      
+                          60046      -107.6      -9.1                      
+                          60047      -107.1      -9.3                      
+                          60048      -106.4      -9.5                      
+                          60049      -106.0      -9.5                      
+                          60050      -106.0      -9.4                      
+                          60051      -106.2      -9.2                      
+                          60052      -106.6      -9.0                      
+                          60053      -106.9      -8.9                      
+                          60054      -107.0      -8.9                      
+                          60055      -107.0      -8.9                      
+                          60056      -107.2      -9.0                      
+                          60057      -107.3      -9.2                      
+                          60058      -107.3      -9.4                      
+                          60059      -107.2      -9.5                      
+                          60060      -106.7      -9.6                      
+                          60061      -106.2      -9.7                      
+                          60062      -106.0      -9.9                      
+                          60063      -106.1     -10.0                      
+                          60064      -105.9     -10.1                      
+                          60065      -106.1      -9.9                      
                                                             
                      IAU2000A Celestial Pole Offset Series  
                       MJD      dX     error     dY     error
                                     (msec. of arc)          
-                      60047    0.311  0.323   -0.003   0.040          
-                      60048    0.318  0.323   -0.002   0.040          
+                      60084    0.455  0.128   -0.113   0.160          
+                      60085    0.451  0.128   -0.099   0.160          
+                      60086    0.446  0.128   -0.085   0.160          
+                      60087    0.440  0.128   -0.069   0.160          
+                      60088    0.434  0.412   -0.053   0.022          
+                      60089    0.426  0.412   -0.036   0.022          
+                      60090    0.419  0.412   -0.019   0.022          
                                                                                
                                                                                
                  IAU2000A Celestial Pole Offset Final Series 
                              MJD     dX         dY           
                              (msec. of arc)          
-                           60005     0.31       0.12
-                           60006     0.31       0.19
-                           60007     0.32       0.17
-                           60008     0.34       0.11
-                           60009     0.35       0.04
-                           60010     0.35      -0.04
-                           60011     0.33      -0.06
-                           60012     0.29      -0.05
-                           60013     0.26      -0.04
-                           60014     0.25      -0.05
-                           60015     0.25      -0.06
-                           60016     0.26      -0.08
-                           60017     0.27      -0.09
-                           60018     0.30      -0.10
-                           60019     0.32      -0.11
-                           60020     0.32      -0.11
-                           60021     0.30      -0.11
-                           60022     0.28      -0.11
-                           60023     0.25      -0.11
-                           60024     0.23      -0.10
-                           60025     0.24      -0.07
-                           60026     0.26      -0.04
-                           60027     0.28      -0.01
-                           60028     0.30       0.04
-                           60029     0.32       0.10
-                           60030     0.33       0.14
-                           60031     0.34       0.16
-                           60032     0.32       0.12
-                           60033     0.29       0.06
-                           60034     0.27      -0.01
-                           60035     0.27      -0.06
+                           60036     0.29      -0.09
+                           60037     0.31      -0.11
+                           60038     0.32      -0.12
+                           60039     0.29      -0.12
+                           60040     0.25      -0.11
+                           60041     0.23      -0.09
+                           60042     0.22      -0.06
+                           60043     0.22      -0.02
+                           60044     0.23       0.01
+                           60045     0.24       0.04
+                           60046     0.27       0.04
+                           60047     0.32       0.01
+                           60048     0.35      -0.03
+                           60049     0.35      -0.05
+                           60050     0.32      -0.05
+                           60051     0.27      -0.04
+                           60052     0.23      -0.03
+                           60053     0.23      -0.01
+                           60054     0.24       0.02
+                           60055     0.26       0.04
+                           60056     0.28       0.06
+                           60057     0.30       0.08
+                           60058     0.32       0.08
+                           60059     0.34       0.07
+                           60060     0.47      -0.05
+                           60061     0.56      -0.15
+                           60062     0.47      -0.17
+                           60063     0.25      -0.09
+                           60064     0.25      -0.09
+                           60065     0.24      -0.10
```

### Comparing `pyTMD-2.0.4/pyTMD/data/tab5.2e.txt` & `pyTMD-2.0.5/pyTMD/data/tab5.2e.txt`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.4/pyTMD/data/tab5.3a.txt` & `pyTMD-2.0.5/pyTMD/data/tab5.3a.txt`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.4/pyTMD/data/tab5.3b.txt` & `pyTMD-2.0.5/pyTMD/data/tab5.3b.txt`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.4/pyTMD/eop.py` & `pyTMD-2.0.5/pyTMD/eop.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.4/pyTMD/interpolate.py` & `pyTMD-2.0.5/pyTMD/interpolate.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.4/pyTMD/io/ATLAS.py` & `pyTMD-2.0.5/pyTMD/io/ATLAS.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.4/pyTMD/io/FES.py` & `pyTMD-2.0.5/pyTMD/io/FES.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 FES.py
-Written by Tyler Sutterley (04/2023)
+Written by Tyler Sutterley (06/2023)
 
 Reads files for a tidal model and makes initial calculations to run tide program
 Includes functions to extract tidal harmonic constants from the
     FES (Finite Element Solution) tide models for given locations
 ascii and netCDF4 files can be been compressed using gzip
 
 Reads ascii and netCDF4 FES tidal solutions provided by AVISO
@@ -52,14 +52,15 @@
     netCDF4: Python interface to the netCDF C library
          https://unidata.github.io/netcdf4-python/netCDF4/index.html
 
 PROGRAM DEPENDENCIES:
     interpolate.py: interpolation routines for spatial data
 
 UPDATE HISTORY:
+    Updated 06/2023: extract ocean tide model variables for FES2012
     Updated 04/2023: added global HAMTIDE11 model
         using pathlib to define and expand tide model paths
     Updated 03/2023: add basic variable typing to function inputs
     Updated 12/2022: refactor tide read programs under io
         new functions to read and interpolate from constituents class
         new functions to output FES formatted netCDF4 files
         refactored interpolation routines into new module
@@ -706,18 +707,18 @@
         f = gzip.open(input_file, 'rb')
         fileID = netCDF4.Dataset(uuid.uuid4().hex, 'r', memory=f.read())
     else:
         fileID = netCDF4.Dataset(input_file, 'r')
     # variable dimensions for each model
     # amplitude and phase components for each type
     if kwargs['version'] in ('FES2012',):
-        lon = fileID.variables['longitude'][:]
-        lat = fileID.variables['latitude'][:]
-        amp_key = dict(z='amplitude', u='Ua', v='Va')[kwargs['type']]
-        phase_key = dict(z='phase', u='Ug', v='Vg')[kwargs['type']]
+        lon = fileID.variables['lon'][:]
+        lat = fileID.variables['lat'][:]
+        amp_key = dict(z='Ha', u='Ua', v='Va')[kwargs['type']]
+        phase_key = dict(z='Hg', u='Ug', v='Vg')[kwargs['type']]
     elif kwargs['version'] in ('FES2014','EOT20'):
         lon = fileID.variables['lon'][:]
         lat = fileID.variables['lat'][:]
         amp_key = dict(z='amplitude', u='Ua', v='Va')[kwargs['type']]
         phase_key = dict(z='phase', u='Ug', v='Vg')[kwargs['type']]
     elif kwargs['version'] in ('HAMTIDE11',):
         lon = fileID.variables['LON'][:]
```

### Comparing `pyTMD-2.0.4/pyTMD/io/GOT.py` & `pyTMD-2.0.5/pyTMD/io/GOT.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,15 +282,15 @@
         **kwargs
     ):
     """
     Reads files for Richard Ray's Global Ocean Tide (GOT) models
 
     Parameters
     ----------
-    model_files: str, list, pathlib.path or NoneType, default None
+    model_files: str, list, pathlib.Path or NoneType, default None
         list of model files for each constituent
     grid: str, default 'ascii'
         Tide model file type to read
 
             - ``'ascii'``: traditional GOT ascii format
             - ``'netcdf'``: GOT netCDF4 format
     compressed: bool, default False
```

### Comparing `pyTMD-2.0.4/pyTMD/io/OTIS.py` & `pyTMD-2.0.5/pyTMD/io/OTIS.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.4/pyTMD/io/constituents.py` & `pyTMD-2.0.5/pyTMD/io/constituents.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.4/pyTMD/io/model.py` & `pyTMD-2.0.5/pyTMD/io/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python
 u"""
 model.py
-Written by Tyler Sutterley (04/2023)
+Written by Tyler Sutterley (06/2023)
 Retrieves tide model parameters for named tide models and
     from model definition files
 
 UPDATE HISTORY:
+    Updated 06/2023: remap FES2012 e2 constituent to eps2
     Updated 04/2023: added global HAMTIDE11 model
         made ICESat, ICESat-2 and output file attributes properties
         updated model definition read function for currents
         using pathlib to define and expand tide model paths
         add basic file searching with glob strings in definition files
         add long_name and description attributes for current variables
         added exceptions for files missing when using glob patterns
@@ -1429,22 +1430,22 @@
         """
         # list of tidal constituents (not all are included in tidal program)
         # include negative look-behind and look-ahead for complex cases
         cindex = [r'(?<!s)sa','ssa','mm','msf',r'mt(?!m)(?!ide)','mf','alpha1',
             '2q1','sigma1',r'(?<!2)q1','rho1',r'(?<!rh)(?<!o)o1','tau1',
             'm1','chi1','pi1','p1','s1','k1','psi1','phi1','theta1','j1',
             'oo1','2n2','mu2',r'(?<!2)n2','nu2',r'(?<!2s)m2(?!a)(?!b)',
-            'm2a','m2b','lambda2','l2','t2',r'(?<!mn)(?<!mk)(?<!ep)s2',
+            'm2a','m2b','lambda2','l2','t2',r'(?<!mn)(?<!mk)(?<!ep)s2(?!0)',
             'r2','k2','eta2','mns2','2sm2','m3','mk3','s3','mn4','m4',
             'ms4','mk4',r'(?<!m)s4','s5','m6','s6','s7','s8','m8','mks2',
             'msqm','mtm',r'(?<!m)n4','eps2','z0']
         # compile regular expression
         rx = re.compile(r'(' + '|'.join(cindex) + r')', re.IGNORECASE)
         # known remapped cases
-        mapping = [('2n','2n2'), ('la2','lambda2')]
+        mapping = [('2n','2n2'), ('la2','lambda2'), ('e2','eps2')]
         # convert to pathlib.Path
         model_file = pathlib.Path(model_file)
         # check if there is a possible constituent name in the file name
         if rx.search(model_file.name):
             return rx.findall(model_file.name)[0].lower()
         # iterate over known remapped cases
         for m in mapping:
```

### Comparing `pyTMD-2.0.4/pyTMD/io/ocean_pole_tide.py` & `pyTMD-2.0.5/pyTMD/io/ocean_pole_tide.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.4/pyTMD/load_constituent.py` & `pyTMD-2.0.5/pyTMD/load_constituent.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.4/pyTMD/load_nodal_corrections.py` & `pyTMD-2.0.5/pyTMD/load_nodal_corrections.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.4/pyTMD/predict.py` & `pyTMD-2.0.5/pyTMD/predict.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.4/pyTMD/spatial.py` & `pyTMD-2.0.5/pyTMD/spatial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 spatial.py
-Written by Tyler Sutterley (04/2023)
+Written by Tyler Sutterley (05/2023)
 
 Utilities for reading, writing and operating on spatial data
 
 PYTHON DEPENDENCIES:
     numpy: Scientific Computing Tools For Python
         https://numpy.org
         https://numpy.org/doc/stable/user/numpy-for-matlab-users.html
@@ -18,14 +18,15 @@
     PyYAML: YAML parser and emitter for Python
         https://github.com/yaml/pyyaml
 
 PROGRAM DEPENDENCIES:
     constants.py: calculate reference parameters for common ellipsoids
 
 UPDATE HISTORY:
+    Updated 05/2023: use datetime parser within pyTMD.time module
     Updated 04/2023: copy inputs in cartesian to not modify original arrays
         added iterative methods for converting from cartesian to geodetic
         allow netCDF4 and HDF5 outputs to be appended to existing files
         using pathlib to define and expand paths
     Updated 03/2023: add basic variable typing to function inputs
     Updated 02/2023: use outputs from constants class for WGS84 parameters
         include more possible dimension names for gridded and drift outputs
@@ -70,15 +71,15 @@
 import uuid
 import yaml
 import logging
 import pathlib
 import datetime
 import warnings
 import numpy as np
-import dateutil.parser
+import pyTMD.time
 from pyTMD.constants import constants
 import pyTMD.version
 # attempt imports
 try:
     import osgeo.gdal, osgeo.osr, osgeo.gdalconst
 except (ImportError, ModuleNotFoundError) as exc:
     warnings.filterwarnings("module")
@@ -106,15 +107,15 @@
         input filename
     """
     # check if file presently exists with input case
     filename = pathlib.Path(filename).expanduser().absolute()
     if not filename.exists():
         # search for filename without case dependence
         f = [f.name for f in filename.parent.iterdir() if
-             re.match(filename.name, f.name, re.I)]
+            re.match(filename.name, f.name, re.I)]
         # raise error if no file found
         if not f:
             raise FileNotFoundError(str(filename))
         filename = filename.with_name(f.pop())
     # return the matched filename
     return filename
 
@@ -277,15 +278,15 @@
                 zip(columns, line.split(kwargs['delimiter']))}
         else:
             column = {c:r.replace('D', 'E') for c, r in
                 zip(columns, rx.findall(line))}
         # copy variables from column dict to output dictionary
         for c in columns:
             if (c == 'time') and kwargs['parse_dates']:
-                dinput[c][i] = dateutil.parser.parse(column[c])
+                dinput[c][i] = pyTMD.time.parse(column[c])
             else:
                 dinput[c][i] = np.float64(column[c])
     # convert to masked array if fill values
     if 'data' in dinput.keys() and '_FillValue' in dinput['attributes']['data'].keys():
         dinput['data'] = np.ma.asarray(dinput['data'])
         dinput['data'].fill_value = dinput['attributes']['data']['_FillValue']
         dinput['data'].mask = (dinput['data'].data == dinput['data'].fill_value)
```

### Comparing `pyTMD-2.0.4/pyTMD/tidal_ellipse.py` & `pyTMD-2.0.5/pyTMD/tidal_ellipse.py`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.4/pyTMD/time.py` & `pyTMD-2.0.5/pyTMD/time.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 PROGRAM DEPENDENCIES:
     utilities.py: download and management utilities for syncing files
 
 UPDATE HISTORY:
     Updated 05/2023: add timescale class for converting between time scales
         added timescale to_datetime function to create datetime arrays
         allow epoch arguments to be numpy datetime64 variables or strings
+        function to convert a string with time zone information to datetime
     Updated 04/2023: using pathlib to define and expand paths
     Updated 03/2023: add basic variable typing to function inputs
     Updated 12/2022: added interpolation for delta time (TT - UT1)
         output variables for some standard epochs used within tide programs
     Updated 11/2022: use IERS https server as default for Bulletin-A files
         added download function for latest Bulletin-A file from IERS
         added function to append from existing merged delta time file
@@ -77,18 +78,42 @@
 _ntp_epoch = (1900, 1, 1, 0, 0, 0)
 _unix_epoch = (1970, 1, 1, 0, 0, 0)
 _gps_epoch = (1980, 1, 6, 0, 0, 0)
 _tide_epoch = (1992, 1, 1, 0, 0, 0)
 _j2000_epoch = (2000, 1, 1, 12, 0, 0)
 _atlas_sdp_epoch = (2018, 1, 1, 0, 0, 0)
 
+# PURPOSE: parse a date string and convert to a datetime object in UTC
+def parse(date_string: str):
+    """
+    Parse a date string and convert to a naive ``datetime`` object in UTC
+
+    Parameters
+    ----------
+    date_string: str
+        formatted time string
+
+    Returns
+    -------
+    date: obj
+        output ``datetime`` object
+    """
+    # parse the date string
+    date = dateutil.parser.parse(date_string)
+    # convert to UTC if containing time-zone information
+    # then drop the timezone information to prevent unsupported errors
+    if date.tzinfo:
+        date = date.astimezone(dateutil.tz.UTC).replace(tzinfo=None)
+    # return the datetime object
+    return date
+
 # PURPOSE: parse a date string into epoch and units scale
 def parse_date_string(date_string: str):
     """
-    parse a date string of the form
+    Parse a date string of the form
 
     - time-units since ``yyyy-mm-dd hh:mm:ss``
     - ``yyyy-mm-dd hh:mm:ss`` for exact calendar dates
 
     Parameters
     ----------
     date_string: str
@@ -99,20 +124,20 @@
     epoch: list
         epoch of ``delta_time``
     conversion_factor: float
         multiplication factor to convert to seconds
     """
     # try parsing the original date string as a date
     try:
-        epoch = dateutil.parser.parse(date_string)
+        epoch = parse(date_string)
     except ValueError:
         pass
     else:
         # return the epoch (as list)
-        return (datetime_to_list(epoch),0.0)
+        return (datetime_to_list(epoch), 0.0)
     # split the date string into units and epoch
     units,epoch = split_date_string(date_string)
     if units not in _to_sec.keys():
         raise ValueError(f'Invalid units: {units}')
     # return the epoch (as list) and the time unit conversion factors
     return (datetime_to_list(epoch), _to_sec[units])
 
@@ -127,25 +152,25 @@
         time-units since yyyy-mm-dd hh:mm:ss
     """
     try:
         units,_,epoch = date_string.split(None, 2)
     except ValueError:
         raise ValueError(f'Invalid format: {date_string}')
     else:
-        return (units.lower(), dateutil.parser.parse(epoch))
+        return (units.lower(), parse(epoch))
 
 # PURPOSE: convert a datetime object into a list
 def datetime_to_list(date):
     """
-    convert a datetime object into a list
+    Convert a ``datetime`` object into a list
 
     Parameters
     ----------
-    date: datetime object
-        Input datetime object to convert
+    date: obj
+        Input ``datetime`` object to convert
 
     Returns
     -------
     date: list
         [year,month,day,hour,minute,second]
     """
     return [date.year, date.month, date.day,
@@ -190,33 +215,33 @@
 
 # PURPOSE: convert a numpy datetime array to delta times since an epoch
 def convert_datetime(
         date: float | np.ndarray,
         epoch: str | tuple | list | np.datetime64 = _unix_epoch
     ):
     """
-    Convert a numpy datetime array to seconds since ``epoch``
+    Convert a ``numpy`` ``datetime`` array to seconds since ``epoch``
 
     Parameters
     ----------
     date: np.ndarray
-        numpy datetime array
+        ``numpy`` ``datetime`` array
     epoch: str, tuple, list, np.ndarray, default (1970,1,1,0,0,0)
         epoch for output ``delta_time``
 
     Returns
     -------
     delta_time: float
         seconds since epoch
     """
     # convert epoch to datetime variables
     if isinstance(epoch, (tuple, list)):
         epoch = np.datetime64(datetime.datetime(*epoch))
     elif isinstance(epoch, str):
-        epoch = np.datetime64(dateutil.parser.parse(epoch))
+        epoch = np.datetime64(parse(epoch))
     # convert to delta time
     return (date - epoch) / np.timedelta64(1, 's')
 
 # PURPOSE: convert times from seconds since epoch1 to time since epoch2
 def convert_delta_time(
         delta_time: np.ndarray,
         epoch1: str | tuple | list | np.datetime64 | None = None,
@@ -237,19 +262,19 @@
     scale: float, default 1.0
         scaling factor for converting time to output units
     """
     # convert epochs to datetime variables
     if isinstance(epoch1, (tuple, list)):
         epoch1 = np.datetime64(datetime.datetime(*epoch1))
     elif isinstance(epoch1, str):
-        epoch1 = np.datetime64(dateutil.parser.parse(epoch1))
+        epoch1 = np.datetime64(parse(epoch1))
     if isinstance(epoch2, (tuple, list)):
         epoch2 = np.datetime64(datetime.datetime(*epoch2))
     elif isinstance(epoch2, str):
-        epoch2 = np.datetime64(dateutil.parser.parse(epoch2))
+        epoch2 = np.datetime64(parse(epoch2))
     # calculate the total difference in time in seconds
     delta_time_epochs = (epoch2 - epoch1) / np.timedelta64(1, 's')
     # subtract difference in time and rescale to output units
     return scale*(delta_time - delta_time_epochs)
 
 # PURPOSE: calculate the delta time from calendar date
 # http://scienceworld.wolfram.com/astronomy/JulianDate.html
@@ -297,15 +322,15 @@
         np.floor(275.0*month/9.0) + day + hour/24.0 + minute/1440.0 + \
         second/86400.0 + 1721028.5 - 2400000.5
     # convert epochs to datetime variables
     epoch1 = np.datetime64(datetime.datetime(*_mjd_epoch))
     if isinstance(epoch, (tuple, list)):
         epoch = np.datetime64(datetime.datetime(*epoch))
     elif isinstance(epoch, str):
-        epoch = np.datetime64(dateutil.parser.parse(epoch))
+        epoch = np.datetime64(parse(epoch))
     # calculate the total difference in time in days
     delta_time_epochs = (epoch - epoch1) / np.timedelta64(1, 'D')
     # return the date in units (default days) since epoch
     return scale*np.array(MJD - delta_time_epochs, dtype=np.float64)
 
 # PURPOSE: Converts from calendar dates into decimal years
 def convert_calendar_decimal(
@@ -710,15 +735,15 @@
             time since epoch
         """
         # convert epochs to numpy datetime variables
         epoch1 = np.datetime64(datetime.datetime(*_mjd_epoch))
         if isinstance(epoch, (tuple, list)):
             epoch = np.datetime64(datetime.datetime(*epoch))
         elif isinstance(epoch, str):
-            epoch = np.datetime64(dateutil.parser.parse(epoch))
+            epoch = np.datetime64(parse(epoch))
         # calculate the difference in epochs in days
         delta_time_epochs = (epoch - epoch1) / np.timedelta64(1, 'D')
         # return the date in time (default days) since epoch
         return scale*np.array(self.MJD - delta_time_epochs, dtype=np.float64)
 
     def to_datetime(self):
         """
@@ -974,15 +999,15 @@
     leap_secs = pyTMD.utilities.get_data_path(['data','leap-seconds.list'])
     # find line with file expiration as delta time
     with leap_secs.open(mode='r', encoding='utf8') as fid:
         secs, = [re.findall(r'\d+',i).pop() for i in fid.read().splitlines()
             if re.match(r'^(?=#@)',i)]
     # check that leap seconds file is still valid
     expiry = datetime.datetime(*_ntp_epoch) + datetime.timedelta(seconds=int(secs))
-    today = datetime.datetime.now()
+    today = datetime.datetime.utcnow()
     update_leap_seconds() if (expiry < today) else None
     # get leap seconds
     leap_UTC,TAI_UTC = np.loadtxt(leap_secs).T
     # TAI time is ahead of GPS by 19 seconds
     TAI_GPS = 19.0
     # convert leap second epochs from NTP to GPS
     # convert from time of 2nd leap second to time of 1st leap second
```

### Comparing `pyTMD-2.0.4/pyTMD/tools.py` & `pyTMD-2.0.5/pyTMD/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 tools.py
-Written by Tyler Sutterley (04/2023)
+Written by Tyler Sutterley (05/2023)
 Jupyter notebook, user interface and plotting tools
 
 PYTHON DEPENDENCIES:
     numpy: Scientific Computing Tools For Python
         https://numpy.org
         https://numpy.org/doc/stable/user/numpy-for-matlab-users.html
     ipywidgets: interactive HTML widgets for Jupyter notebooks and IPython
@@ -13,28 +13,28 @@
     ipyleaflet: Jupyter / Leaflet bridge enabling interactive maps
         https://github.com/jupyter-widgets/ipyleaflet
     matplotlib: Python 2D plotting library
         http://matplotlib.org/
         https://github.com/matplotlib/matplotlib
 
 UPDATE HISTORY:
+    Updated 05/2023: don't set a default directory for tide models
     Updated 04/2023: using pathlib to define and expand paths
     Updated 01/2023: use debug level logging instead of import warnings
     Updated 11/2022: place more imports within try/except statements
     Updated 08/2022: place some imports behind try/except statements
     Updated 05/2022: include world copy jump in webmercator maps
     Updated 03/2022: add marker relocation routines from notebooks
     Updated 02/2022: add leaflet map projections
     Written 09/2021
 """
 import io
 import copy
 import base64
 import logging
-import pathlib
 import datetime
 import numpy as np
 import matplotlib
 matplotlib.rcParams['axes.linewidth'] = 2.0
 matplotlib.rcParams["animation.html"] = "jshtml"
 import matplotlib.cm as cm
 import matplotlib.colorbar
@@ -66,15 +66,15 @@
         # set default keyword options
         kwargs.setdefault('style', {})
         # set style
         self.style = copy.copy(kwargs['style'])
 
         # set the directory with tide models
         self.directory = ipywidgets.Text(
-            value=pathlib.Path.cwd(),
+            value='',
             description='Directory:',
             disabled=False
         )
 
         # dropdown menu for setting tide model
         model_list = sorted(pyTMD.io.model.ocean_elevation() +
             pyTMD.io.model.load_elevation())
@@ -95,15 +95,15 @@
             disabled=False,
             style=self.style,
         )
         self.atlas.layout.display = 'none'
 
         # checkbox for setting if tide files are compressed
         self.compress = ipywidgets.Checkbox(
-            value=True,
+            value=False,
             description='Compressed?',
             disabled=False,
             style=self.style,
         )
 
         # date picker widget for setting time
         self.datepick = ipywidgets.DatePicker(
```

### Comparing `pyTMD-2.0.4/pyTMD/utilities.py` & `pyTMD-2.0.5/pyTMD/utilities.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 #!/usr/bin/env python
 u"""
 utilities.py
-Written by Tyler Sutterley (05/2023)
+Written by Tyler Sutterley (06/2023)
 Download and management utilities for syncing time and auxiliary files
 
 PYTHON DEPENDENCIES:
     lxml: processing XML and HTML in Python
         https://pypi.python.org/pypi/lxml
 
 UPDATE HISTORY:
+    Updated 06/2023: add functions to retrieve and revoke Earthdata tokens
     Updated 05/2023: add reify decorator for evaluation of properties
+        make urs a keyword argument in CCDIS list and download functions
+        add case for JPL kernel file download where local path is defined
     Updated 04/2023: using pathlib to define and expand paths
         added function to download ephemeride files from JPL SSD server
     Updated 03/2023: add basic variable typing to function inputs
     Updated 01/2023: updated SSL context to fix some deprecation warnings
     Updated 11/2022: added list program for IERS Bulletin-A https server
         use f-strings for formatting verbose or ascii output
     Updated 04/2022: updated docstrings to numpy documentation format
@@ -33,26 +36,30 @@
         generalize build opener function for different Earthdata instances
     Updated 08/2020: add GSFC CDDIS opener, login and download functions
     Written 08/2020
 """
 from __future__ import print_function, division, annotations
 
 import sys
+import os
 import re
 import io
 import ssl
+import json
 import netrc
 import ftplib
 import shutil
 import base64
 import socket
+import getpass
 import inspect
 import hashlib
 import logging
 import pathlib
+import builtins
 import warnings
 import posixpath
 import subprocess
 import lxml.etree
 import calendar, time
 import dateutil.parser
 if sys.version_info[0] == 2:
@@ -67,24 +74,24 @@
 # PURPOSE: get absolute path within a package from a relative path
 def get_data_path(relpath: list | str | pathlib.Path):
     """
     Get the absolute path within a package from a relative path
 
     Parameters
     ----------
-    relpath: list or str
+    relpath: list, str or pathlib.Path
         relative path
     """
     # current file path
     filename = inspect.getframeinfo(inspect.currentframe()).filename
     filepath = pathlib.Path(filename).absolute().parent
     if isinstance(relpath, list):
         # use *splat operator to extract from list
         return filepath.joinpath(*relpath)
-    elif isinstance(relpath, str):
+    elif isinstance(relpath, (str, pathlib.Path)):
         return filepath.joinpath(relpath)
 
 class reify(object):
     """Class decorator that puts the result of the method it
     decorates into the instance"""
     def __init__(self, wrapped):
         self.wrapped = wrapped
@@ -101,36 +108,36 @@
 # PURPOSE: platform independent file opener
 def file_opener(filename: str | pathlib.Path):
     """
     Platform independent file opener
 
     Parameters
     ----------
-    filename: str
+    filename: str or pathlib.Path
         path to file
     """
     filename = pathlib.Path(filename).expanduser()
     if (sys.platform == "win32"):
-        pathlib.os.startfile(filename, "explore")
+        os.startfile(filename, "explore")
     elif (sys.platform == "darwin"):
         subprocess.call(["open", filename])
     else:
         subprocess.call(["xdg-open", filename])
 
 # PURPOSE: get the hash value of a file
 def get_hash(
-        local: str | io.IOBase,
+        local: str | io.IOBase | pathlib.Path,
         algorithm: str = 'MD5'
     ):
     """
     Get the hash value from a local file or ``BytesIO`` object
 
     Parameters
     ----------
-    local: obj or str
+    local: obj, str or pathlib.Path
         BytesIO object or path to file
     algorithm: str, default 'MD5'
         hashing algorithm for checksum validation
 
             - ``'MD5'``: Message Digest
             - ``'sha1'``: Secure Hash Algorithm
     """
@@ -359,16 +366,16 @@
     value: float
         number to be rounded upward
     """
     return -int(-value//1)
 
 # PURPOSE: make a copy of a file with all system information
 def copy(
-        source: str,
-        destination: str,
+        source: str | pathlib.Path,
+        destination: str | pathlib.Path,
         move: bool = False,
         **kwargs
     ):
     """
     Copy or move a file with all system information
 
     Parameters
@@ -418,15 +425,15 @@
     except ftplib.error_perm:
         raise RuntimeError('Check login credentials')
     else:
         return True
 
 # PURPOSE: list a directory on a ftp host
 def ftp_list(
-        HOST: str,
+        HOST: str | list,
         username: str | None = None,
         password: str | None = None,
         timeout: int | None = None,
         basename: bool = False,
         pattern: str | None = None,
         sort: bool = False
     ):
@@ -500,15 +507,15 @@
         # close the ftp connection
         ftp.close()
         # return the list of items and last modified times
         return (output, mtimes)
 
 # PURPOSE: download a file from a ftp host
 def from_ftp(
-        HOST: str,
+        HOST: str | list,
         username: str | None = None,
         password: str | None = None,
         timeout: int | None = None,
         local: str | pathlib.Path | None = None,
         hash: str = '',
         chunk: int = 8192,
         verbose: bool = False,
@@ -586,15 +593,15 @@
             # store bytes to file using chunked transfer encoding
             remote_buffer.seek(0)
             with local.open(mode='wb') as f:
                 shutil.copyfileobj(remote_buffer, f, chunk)
             # change the permissions mode
             local.chmod(mode)
             # keep remote modification time of file and local access time
-            pathlib.os.utime(local, (local.stat().st_atime, remote_mtime))
+            os.utime(local, (local.stat().st_atime, remote_mtime))
         # close the ftp connection
         ftp.close()
         # return the bytesIO object
         remote_buffer.seek(0)
         return remote_buffer
 
 # default ssl context
@@ -611,22 +618,26 @@
         remote http host
     context: obj, default ssl.SSLContext(ssl.PROTOCOL_TLS)
         SSL context for ``urllib`` opener object
     """
     # attempt to connect to http host
     try:
         urllib2.urlopen(HOST, timeout=20, context=context)
+    except urllib2.HTTPError as exc:
+        logging.debug(exc.code)
+        raise RuntimeError(exc.reason) from exc
     except urllib2.URLError as exc:
+        logging.debug(exc.reason)
         raise RuntimeError('Check internet connection') from exc
     else:
         return True
 
 # PURPOSE: list a directory on an Apache http Server
 def http_list(
-        HOST: str,
+        HOST: str | list,
         timeout: int | None = None,
         context = _default_ssl_context,
         parser = lxml.etree.HTMLParser(),
         format: str = '%Y-%m-%d %H:%M',
         pattern: str = '',
         sort: bool = False
     ):
@@ -661,16 +672,21 @@
     if isinstance(HOST, str):
         HOST = url_split(HOST)
     # try listing from http
     try:
         # Create and submit request.
         request = urllib2.Request(posixpath.join(*HOST))
         response = urllib2.urlopen(request, timeout=timeout, context=context)
-    except (urllib2.HTTPError, urllib2.URLError):
-        raise Exception('List error from {0}'.format(posixpath.join(*HOST)))
+    except urllib2.HTTPError as exc:
+        logging.debug(exc.code)
+        raise RuntimeError(exc.reason) from exc
+    except urllib2.URLError as exc:
+        logging.debug(exc.reason)
+        msg = 'List error from {0}'.format(posixpath.join(*HOST))
+        raise Exception(msg) from exc
     else:
         # read and parse request for files (column names and modified times)
         tree = lxml.etree.parse(response, parser)
         colnames = tree.xpath('//tr/td[not(@*)]//a/@href')
         # get the Unix timestamp value for a modification time
         collastmod = [get_unix_time(i,format=format)
             for i in tree.xpath('//tr/td[@align="right"][1]/text()')]
@@ -687,18 +703,18 @@
             colnames = [colnames[indice] for indice in i]
             collastmod = [collastmod[indice] for indice in i]
         # return the list of column names and last modified times
         return (colnames, collastmod)
 
 # PURPOSE: download a file from a http host
 def from_http(
-        HOST: str,
+        HOST: str | list,
         timeout: int | None = None,
         context = _default_ssl_context,
-        local: str | pathlib.path | None = None,
+        local: str | pathlib.Path | None = None,
         hash: str = '',
         chunk: int = 16384,
         verbose: bool = False,
         fid = sys.stdout,
         mode: oct = 0o775
     ):
     """
@@ -767,14 +783,98 @@
                 shutil.copyfileobj(remote_buffer, f, chunk)
             # change the permissions mode
             local.chmod(mode)
         # return the bytesIO object
         remote_buffer.seek(0)
         return remote_buffer
 
+# PURPOSE: attempt to build an opener with netrc
+def attempt_login(
+        urs: str,
+        context=_default_ssl_context,
+        password_manager: bool = True,
+        get_ca_certs: bool = True,
+        redirect: bool = True,
+        authorization_header: bool = False,
+        **kwargs
+    ):
+    """
+    attempt to build a urllib opener for NASA Earthdata
+
+    Parameters
+    ----------
+    urs: str
+        Earthdata login URS 3 host
+    context: obj, default ssl.SSLContext(ssl.PROTOCOL_TLS)
+        SSL context for ``urllib`` opener object
+    password_manager: bool, default True
+        Create password manager context using default realm
+    get_ca_certs: bool, default True
+        Get list of loaded “certification authority” certificates
+    redirect: bool, default True
+        Create redirect handler object
+    authorization_header: bool, default False
+        Add base64 encoded authorization header to opener
+    username: str, default from environmental variable
+        NASA Earthdata username
+    password: str, default from environmental variable
+        NASA Earthdata password
+    retries: int, default 5
+        number of retry attempts
+    netrc: str, default ~/.netrc
+        path to .netrc file for authentication
+
+    Returns
+    -------
+    opener: obj
+        OpenerDirector instance
+    """
+    # set default keyword arguments
+    kwargs.setdefault('username', os.environ.get('EARTHDATA_USERNAME'))
+    kwargs.setdefault('password', os.environ.get('EARTHDATA_PASSWORD'))
+    kwargs.setdefault('retries', 5)
+    kwargs.setdefault('netrc', os.path.expanduser('~/.netrc'))
+    try:
+        # only necessary on jupyterhub
+        os.chmod(kwargs['netrc'], 0o600)
+        # try retrieving credentials from netrc
+        username, _, password = netrc.netrc(kwargs['netrc']).authenticators(urs)
+    except Exception as exc:
+        # try retrieving credentials from environmental variables
+        username, password = (kwargs['username'], kwargs['password'])
+        pass
+    # if username or password are not available
+    if not username:
+        username = builtins.input(f'Username for {urs}: ')
+    if not password:
+        prompt = f'Password for {username}@{urs}: '
+        password = getpass.getpass(prompt=prompt)
+    # for each retry
+    for retry in range(kwargs['retries']):
+        # build an opener for urs with credentials
+        opener = build_opener(username, password,
+            context=context,
+            password_manager=password_manager,
+            get_ca_certs=get_ca_certs,
+            redirect=redirect,
+            authorization_header=authorization_header,
+            urs=urs)
+        # try logging in by check credentials
+        try:
+            check_credentials()
+        except Exception as exc:
+            pass
+        else:
+            return opener
+        # reattempt login
+        username = builtins.input(f'Username for {urs}: ')
+        password = getpass.getpass(prompt=prompt)
+    # reached end of available retries
+    raise RuntimeError('End of Retries: Check NASA Earthdata credentials')
+
 # PURPOSE: "login" to NASA Earthdata with supplied credentials
 def build_opener(
         username: str,
         password: str,
         context=_default_ssl_context,
         password_manager: bool = True,
         get_ca_certs: bool = True,
@@ -799,14 +899,19 @@
         Get list of loaded “certification authority” certificates
     redirect: bool, default True
         Create redirect handler object
     authorization_header: bool, default False
         Add base64 encoded authorization header to opener
     urs: str, default 'https://urs.earthdata.nasa.gov'
         Earthdata login URS 3 host
+
+    Returns
+    -------
+    opener: obj
+        ``OpenerDirector`` instance
     """
     # https://docs.python.org/3/howto/urllib2.html#id5
     handler = []
     # create a password manager
     if password_manager:
         password_mgr = urllib2.HTTPPasswordMgrWithDefaultRealm()
         # Add the username and password for NASA Earthdata Login system
@@ -834,37 +939,199 @@
     # Now all calls to urllib2.urlopen use our opener.
     urllib2.install_opener(opener)
     # All calls to urllib2.urlopen will now use handler
     # Make sure not to include the protocol in with the URL, or
     # HTTPPasswordMgrWithDefaultRealm will be confused.
     return opener
 
+# PURPOSE: generate a NASA Earthdata user token
+def get_token(
+        HOST: str = 'https://urs.earthdata.nasa.gov/api/users/token',
+        username: str | None = None,
+        password: str | None = None,
+        build: bool = True,
+        urs: str = 'urs.earthdata.nasa.gov',
+    ):
+    """
+    Generate a NASA Earthdata User Token
+
+    Parameters
+    ----------
+    HOST: str or list
+        NASA Earthdata token API host
+    username: str or NoneType, default None
+        NASA Earthdata username
+    password: str or NoneType, default None
+        NASA Earthdata password
+    build: bool, default True
+        Build opener and check WebDAV credentials
+    timeout: int or NoneType, default None
+        timeout in seconds for blocking operations
+    urs: str, default 'urs.earthdata.nasa.gov'
+        NASA Earthdata URS 3 host
+
+    Returns
+    -------
+    token: dict
+        JSON response with NASA Earthdata User Token
+    """
+    # attempt to build urllib2 opener and check credentials
+    if build:
+        attempt_login(urs,
+            username=username,
+            password=password,
+            password_manager=False,
+            get_ca_certs=False,
+            redirect=False,
+            authorization_header=True)
+    # create post response with Earthdata token API
+    try:
+        request = urllib2.Request(HOST, method='POST')
+        response = urllib2.urlopen(request)
+    except urllib2.HTTPError as exc:
+        logging.debug(exc.code)
+        raise RuntimeError(exc.reason) from exc
+    except urllib2.URLError as exc:
+        logging.debug(exc.reason)
+        raise RuntimeError('Check internet connection') from exc
+    # read and return JSON response
+    return json.loads(response.read())
+
+# PURPOSE: generate a NASA Earthdata user token
+def list_tokens(
+        HOST: str = 'https://urs.earthdata.nasa.gov/api/users/tokens',
+        username: str | None = None,
+        password: str | None = None,
+        build: bool = True,
+        urs: str = 'urs.earthdata.nasa.gov',
+    ):
+    """
+    List the current associated NASA Earthdata User Tokens
+
+    Parameters
+    ----------
+    HOST: str
+        NASA Earthdata list token API host
+    username: str or NoneType, default None
+        NASA Earthdata username
+    password: str or NoneType, default None
+        NASA Earthdata password
+    build: bool, default True
+        Build opener and check WebDAV credentials
+    timeout: int or NoneType, default None
+        timeout in seconds for blocking operations
+    urs: str, default 'urs.earthdata.nasa.gov'
+        NASA Earthdata URS 3 host
+
+    Returns
+    -------
+    tokens: list
+        JSON response with NASA Earthdata User Tokens
+    """
+    # attempt to build urllib2 opener and check credentials
+    if build:
+        attempt_login(urs,
+            username=username,
+            password=password,
+            password_manager=False,
+            get_ca_certs=False,
+            redirect=False,
+            authorization_header=True)
+    # create get response with Earthdata list tokens API
+    try:
+        request = urllib2.Request(HOST)
+        response = urllib2.urlopen(request)
+    except urllib2.HTTPError as exc:
+        logging.debug(exc.code)
+        raise RuntimeError(exc.reason) from exc
+    except urllib2.URLError as exc:
+        logging.debug(exc.reason)
+        raise RuntimeError('Check internet connection') from exc
+    # read and return JSON response
+    return json.loads(response.read())
+
+# PURPOSE: revoke a NASA Earthdata user token
+def revoke_token(
+        token: str,
+        HOST: str = f'https://urs.earthdata.nasa.gov/api/users/revoke_token',
+        username: str | None = None,
+        password: str | None = None,
+        build: bool = True,
+        urs: str = 'urs.earthdata.nasa.gov',
+    ):
+    """
+    Generate a NASA Earthdata User Token
+
+    Parameters
+    ----------
+    token: str
+        NASA Earthdata token to be revoked
+    HOST: str
+        NASA Earthdata revoke token API host
+    username: str or NoneType, default None
+        NASA Earthdata username
+    password: str or NoneType, default None
+        NASA Earthdata password
+    build: bool, default True
+        Build opener and check WebDAV credentials
+    timeout: int or NoneType, default None
+        timeout in seconds for blocking operations
+    urs: str, default 'urs.earthdata.nasa.gov'
+        NASA Earthdata URS 3 host
+    """
+    # attempt to build urllib2 opener and check credentials
+    if build:
+        attempt_login(urs,
+            username=username,
+            password=password,
+            password_manager=False,
+            get_ca_certs=False,
+            redirect=False,
+            authorization_header=True)
+    # full path for NASA Earthdata revoke token API
+    url = f'{HOST}?token={token}'
+    # create post response with Earthdata revoke tokens API
+    try:
+        request = urllib2.Request(url, method='POST')
+        response = urllib2.urlopen(request)
+    except urllib2.HTTPError as exc:
+        logging.debug(exc.code)
+        raise RuntimeError(exc.reason) from exc
+    except urllib2.URLError as exc:
+        logging.debug(exc.reason)
+        raise RuntimeError('Check internet connection') from exc
+    # verbose response
+    logging.debug(f'Token Revoked: {token}')
+
 # PURPOSE: check that entered NASA Earthdata credentials are valid
 def check_credentials():
     """
     Check that entered NASA Earthdata credentials are valid
     """
     try:
         remote_path = posixpath.join('https://cddis.nasa.gov','archive')
         request = urllib2.Request(url=remote_path)
         response = urllib2.urlopen(request, timeout=20)
-    except urllib2.HTTPError:
-        raise RuntimeError('Check your NASA Earthdata credentials')
-    except urllib2.URLError:
-        raise RuntimeError('Check internet connection')
+    except urllib2.HTTPError as exc:
+        logging.debug(exc.code)
+        raise RuntimeError(exc.reason) from exc
+    except urllib2.URLError as exc:
+        logging.debug(exc.reason)
+        raise RuntimeError('Check internet connection') from exc
     else:
         return True
 
 # PURPOSE: list a directory on GSFC CDDIS https server
 def cddis_list(
-        HOST: str,
+        HOST: str | list,
         username: str | None = None,
         password: str | None = None,
         build: bool = True,
         timeout: int | None = None,
+        urs: str = 'urs.earthdata.nasa.gov',
         parser=lxml.etree.HTMLParser(),
         pattern: str = '',
         sort: bool = False
     ):
     """
     List a directory on GSFC CDDIS archive server
 
@@ -876,14 +1143,16 @@
         NASA Earthdata username
     password: str or NoneType, default None
         NASA Earthdata password
     build: bool, default True
         Build opener and check Earthdata credentials
     timeout: int or NoneType, default None
         timeout in seconds for blocking operations
+    urs: str, default 'urs.earthdata.nasa.gov'
+        NASA Earthdata URS 3 host
     parser: obj, default lxml.etree.HTMLParser()
         HTML parser for ``lxml``
     pattern: str, default ''
         regular expression pattern for reducing list
     sort: bool, default False
         sort output list
 
@@ -892,15 +1161,14 @@
     colnames: list
         column names in a directory
     collastmod: list
         last modification times for items in the directory
     """
     # use netrc credentials
     if build and not (username or password):
-        urs = 'urs.earthdata.nasa.gov'
         username,_,password = netrc.netrc().authenticators(urs)
     # build urllib2 opener and check credentials
     if build:
         # build urllib2 opener with credentials
         build_opener(username, password)
         # check credentials
         check_credentials()
@@ -941,19 +1209,20 @@
             colnames = [colnames[indice] for indice in i]
             collastmod = [collastmod[indice] for indice in i]
         # return the list of column names and last modified times
         return (colnames, collastmod)
 
 # PURPOSE: download a file from a GSFC CDDIS https server
 def from_cddis(
-        HOST: str,
+        HOST: str | list,
         username: str | None = None,
         password: str | None = None,
         build: bool = True,
         timeout: int | None = None,
+        urs: str = 'urs.earthdata.nasa.gov',
         local: str | pathlib.Path | None = None,
         hash: str = '',
         chunk: int = 16384,
         verbose: bool = False,
         fid=sys.stdout,
         mode: oct = 0o775
     ):
@@ -968,14 +1237,16 @@
         NASA Earthdata username
     password: str or NoneType, default None
         NASA Earthdata password
     build: bool, default True
         Build opener and check Earthdata credentials
     timeout: int or NoneType, default None
         timeout in seconds for blocking operations
+    urs: str, default 'urs.earthdata.nasa.gov'
+        NASA Earthdata URS 3 host
     local: str, pathlib.Path or NoneType, default None
         path to local file
     hash: str, default ''
         MD5 hash of local file
     chunk: int, default 16384
         chunk size for transfer encoding
     verbose: bool, default False
@@ -991,15 +1262,14 @@
         BytesIO representation of file
     """
     # create logger
     loglevel = logging.INFO if verbose else logging.CRITICAL
     logging.basicConfig(stream=fid, level=loglevel)
     # use netrc credentials
     if build and not (username or password):
-        urs = 'urs.earthdata.nasa.gov'
         username,_,password = netrc.netrc().authenticators(urs)
     # build urllib2 opener and check credentials
     if build:
         # build urllib2 opener with credentials
         build_opener(username, password)
         # check credentials
         check_credentials()
@@ -1043,15 +1313,15 @@
             local.chmod(mode)
         # return the bytesIO object
         remote_buffer.seek(0)
         return remote_buffer
 
 # PURPOSE: list a directory on IERS https Server
 def iers_list(
-        HOST: str,
+        HOST: str | list,
         timeout: int | None = None,
         context = _default_ssl_context,
         parser = lxml.etree.HTMLParser()
     ):
     """
     List a directory on IERS Bulletin-A https server
 
@@ -1077,16 +1347,21 @@
     if isinstance(HOST, str):
         HOST = url_split(HOST)
     # try listing from http
     try:
         # Create and submit request.
         request = urllib2.Request(posixpath.join(*HOST))
         response = urllib2.urlopen(request, timeout=timeout, context=context)
-    except (urllib2.HTTPError, urllib2.URLError):
-        raise Exception('List error from {0}'.format(posixpath.join(*HOST)))
+    except urllib2.HTTPError as exc:
+        logging.debug(exc.code)
+        raise RuntimeError(exc.reason) from exc
+    except urllib2.URLError as exc:
+        logging.debug(exc.reason)
+        msg = 'List error from {0}'.format(posixpath.join(*HOST))
+        raise Exception(msg) from exc
     else:
         # read and parse request for files (column names and modified times)
         tree = lxml.etree.parse(response, parser)
         colnames = tree.xpath('//tr/td[@class="$tdclass"][4]//a/@href')
         # get the Unix timestamp value for a modification time
         collastmod = [get_unix_time(i,format='%Y-%m-%d')
             for i in tree.xpath('//tr/td[@class="$tdclass"][2]/span/text()')]
@@ -1094,14 +1369,15 @@
         # return the list of column names and last modified times
         return (colnames[::-1], collastmod[::-1])
 
 def from_jpl_ssd(
         kernel='de440s.bsp',
         timeout: int | None = None,
         context = _default_ssl_context,
+        local: str | pathlib.Path | None = None,
         hash: str = '',
         chunk: int = 16384,
         verbose: bool = False,
         mode: oct = 0o775
     ):
     """
     Download `planetary ephemeride kernels`__ from the JPL Solar
@@ -1122,14 +1398,21 @@
     chunk: int, default 16384
         chunk size for transfer encoding
     verbose: bool, default False
         print file transfer information
     mode: oct, default 0o775
         permissions mode of output local file
     """
-    # local path to kernel file
-    local = get_data_path(['data',kernel])
+    # determine which kernel file to download
+    if (local is None):
+        # local path to kernel file
+        local = get_data_path(['data',kernel])
+    elif (kernel is None) and (local is not None):
+        # verify inputs for remote http host
+        local = pathlib.Path(local).expanduser().absolute()
+        kernel = local.name
     # remote host path to kernel file
     HOST = ['https://ssd.jpl.nasa.gov','ftp','eph','planets','bsp',kernel]
     # get kernel file from remote host
+    logging.info('Downloading JPL Planetary Ephemeride Kernel File')
     from_http(HOST, timeout=timeout, context=context, local=local,
         hash=hash, chunk=chunk, verbose=verbose, mode=mode)
```

### Comparing `pyTMD-2.0.4/pyTMD.egg-info/PKG-INFO` & `pyTMD-2.0.5/pyTMD.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTMD
-Version: 2.0.4
+Version: 2.0.5
 Summary: Tide Model Driver to read OTIS, GOT and FES formatted tidal solutions and make tidal predictions
 Home-page: https://github.com/tsutterley/pyTMD
 Author: Tyler Sutterley
 Author-email: tsutterl@uw.edu
 License: MIT
 Keywords: Ocean Tides,Load Tides,Pole Tides,Tidal Prediction,OTIS,GOT,FES
 Classifier: Development Status :: 3 - Alpha
@@ -80,15 +80,15 @@
 
 - `dateutil: powerful extensions to datetime <https://dateutil.readthedocs.io/en/stable/>`_
 - `lxml: processing XML and HTML in Python <https://pypi.python.org/pypi/lxml>`_
 - `netCDF4: Python interface to the netCDF C library <https://unidata.github.io/netcdf4-python/>`_
 - `numpy: Scientific Computing Tools For Python <https://www.numpy.org>`_
 - `pyproj: Python interface to PROJ library <https://pypi.org/project/pyproj/>`_
 - `scipy: Scientific Tools for Python <https://www.scipy.org/>`_
-- `setuptools_scm: manager for python package versions using scm metadata <https://pypi.org/project/setuptools-scm/1.9.0/>`_
+- `setuptools_scm: manager for python package versions using scm metadata <https://pypi.org/project/setuptools-scm>`_
 
 References
 ##########
 
     T. C. Sutterley, T. Markus, T. A. Neumann, M. R. van den Broeke, J. M. van Wessem, and S. R. M. Ligtenberg,
     "Antarctic ice shelf thickness change from multimission lidar mapping", *The Cryosphere*,
     13, 1801-1817, (2019). `doi: 10.5194/tc-13-1801-2019 <https://doi.org/10.5194/tc-13-1801-2019>`_
```

### Comparing `pyTMD-2.0.4/pyTMD.egg-info/SOURCES.txt` & `pyTMD-2.0.5/pyTMD.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyTMD-2.0.4/scripts/arcticdata_tides.py` & `pyTMD-2.0.5/scripts/arcticdata_tides.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 arcticdata_tides.py
-Written by Tyler Sutterley (04/2023)
+Written by Tyler Sutterley (05/2023)
 Download Arctic Ocean Tide Models from the NSF ArcticData archive
 
 AODTM-5: https://arcticdata.io/catalog/view/doi:10.18739/A2901ZG3N
 AOTIM-5: https://arcticdata.io/catalog/view/doi:10.18739/A2S17SS80
 AOTIM-5-2018: https://arcticdata.io/catalog/view/doi:10.18739/A21R6N14K
 Arc2kmTM: https://arcticdata.io/catalog/view/doi:10.18739/A2D21RK6K
 Gr1kmTM: https://arcticdata.io/catalog/view/doi:10.18739/A2B853K18
@@ -18,24 +18,26 @@
     -D X, --directory X: working data directory
     -T X, --tide X: Arctic tide model to download
         AODTM-5
         AOTIM-5
         AOTIM-5-2018
         Arc2kmTM
         Gr1kmTM
+    -t X, --timeout X: timeout in seconds for blocking operations
     -M X, --mode X: Local permissions mode of the files downloaded
 
 PYTHON DEPENDENCIES:
     future: Compatibility layer between Python 2 and Python 3
         https://python-future.org/
 
 PROGRAM DEPENDENCIES:
     utilities.py: download and management utilities for syncing files
 
 UPDATE HISTORY:
+    Updated 05/2023: added option to change connection timeout
     Updated 04/2023: using pathlib to define and expand paths
     Updated 11/2022: use f-strings for formatting verbose or ascii output
     Updated 06/2022: added Greenland 1km model (Gr1kmTM) to list of models
     Updated 04/2022: use argparse descriptions within documentation
     Updated 10/2021: using python logging for handling verbose output
     Updated 07/2021: can use prefix files to define command line arguments
     Updated 10/2020: using argparse to set command line parameters
@@ -50,14 +52,15 @@
 import argparse
 import posixpath
 import pyTMD.utilities
 
 # PURPOSE: Download Arctic Ocean Tide Models from the NSF ArcticData archive
 def arcticdata_tides(MODEL: str,
     DIRECTORY: str | pathlib.Path | None = None,
+    TIMEOUT: int | None = None,
     MODE: oct = 0o775):
 
     # create logger for verbosity level
     logger = pyTMD.utilities.build_logger(__name__,level=logging.INFO)
 
     # digital object identifier (doi) for each Arctic tide model
     DOI = {}
@@ -82,28 +85,28 @@
     # build host url for model
     resource_map_doi = f'resource_map_doi:{DOI[MODEL]}'
     HOST = ['https://arcticdata.io','metacat','d1','mn','v2','packages',
         pyTMD.utilities.quote_plus(posixpath.join('application','bagit-097')),
         pyTMD.utilities.quote_plus(resource_map_doi)]
     # download zipfile from host
     logger.info(f'{posixpath.join(*HOST)} -->\n')
-    zfile = zipfile.ZipFile(pyTMD.utilities.from_http(HOST))
+    zfile = zipfile.ZipFile(pyTMD.utilities.from_http(HOST, timeout=TIMEOUT))
     # find model files within zip file
     rx = re.compile(r'(grid|h[0]?|UV[0]?|Model|xy)_(.*?)',re.VERBOSE)
     members = [m for m in zfile.filelist if rx.search(m.filename)]
     # extract each member
     for m in members:
         # strip directories from member filename
         m.filename = posixpath.basename(m.filename)
         local_file = local_dir.joinpath(m.filename)
         logger.info(str(local_file))
         # extract file
         zfile.extract(m, path=local_dir)
         # change permissions mode
-        local_file.chmod(MODE)
+        local_file.chmod(mode=MODE)
     # close the zipfile object
     zfile.close()
 
 # PURPOSE: create argument parser
 def arguments():
     parser = argparse.ArgumentParser(
         description="""Download Arctic Ocean Tide Models from the NSF ArcticData
@@ -118,14 +121,18 @@
         type=pathlib.Path, default=pathlib.Path.cwd(),
         help='Working data directory')
     # Arctic Ocean tide model to download
     parser.add_argument('--tide','-T',
         metavar='TIDE', type=str, nargs='+', default=['Gr1kmTM'],
         choices=('AODTM-5','AOTIM-5','AOTIM-5-2018','Arc2kmTM','Gr1kmTM'),
         help='Arctic Ocean tide model to download')
+    # connection timeout
+    parser.add_argument('--timeout','-t',
+        type=int, default=360,
+        help='Timeout in seconds for blocking operations')
     # permissions mode of the local directories and files (number in octal)
     parser.add_argument('--mode','-M',
         type=lambda x: int(x,base=8), default=0o775,
         help='Permissions mode of the files downloaded')
     # return the parser
     return parser
 
@@ -136,12 +143,13 @@
     args,_ = parser.parse_known_args()
 
     # check internet connection before attempting to run program
     if pyTMD.utilities.check_connection('https://arcticdata.io'):
         for m in args.tide:
             arcticdata_tides(m,
                 DIRECTORY=args.directory,
+                TIMEOUT=args.timeout,
                 MODE=args.mode)
 
 # run main program
 if __name__ == '__main__':
     main()
```

### Comparing `pyTMD-2.0.4/scripts/aviso_fes_tides.py` & `pyTMD-2.0.5/scripts/aviso_fes_tides.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,25 +21,28 @@
     --tide X: FES tide model to download
         FES1999
         FES2004
         FES2012
         FES2014
     --load: download load tide model outputs (fes2014)
     --currents: download tide model current outputs (fes2012 and fes2014)
+    -G, --gzip: compress output ascii and netCDF4 tide files
+    -t X, --timeout X: timeout in seconds for blocking operations
     --log: output log of files downloaded
     -M X, --mode X: Local permissions mode of the files downloaded
 
 PYTHON DEPENDENCIES:
     future: Compatibility layer between Python 2 and Python 3
         https://python-future.org/
 
 PROGRAM DEPENDENCIES:
     utilities.py: download and management utilities for syncing files
 
 UPDATE HISTORY:
+    Updated 05/2023: added option to change connection timeout
     Updated 04/2023: using pathlib to define and expand paths
         added option to include AVISO FTP password as argument
     Updated 11/2022: added encoding for writing ascii files
         use f-strings for formatting verbose or ascii output
     Updated 04/2022: use argparse descriptions within documentation
     Updated 10/2021: using python logging for handling verbose output
     Updated 07/2021: can use prefix files to define command line arguments
@@ -47,15 +50,15 @@
     Updated 04/2021: set a default netrc file and check access
     Updated 10/2020: using argparse to set command line parameters
     Updated 07/2020: add gzip option to compress output ascii and netCDF4 files
     Updated 06/2020: added netrc option for alternative authentication
     Updated 05/2019: new authenticated ftp host (changed 2018-05-31)
     Written 09/2017
 """
-from __future__ import print_function
+from __future__ import print_function, annotations
 
 import sys
 import os
 import io
 import gzip
 import netrc
 import shutil
@@ -67,19 +70,27 @@
 import builtins
 import posixpath
 import calendar, time
 import ftplib
 import pyTMD.utilities
 
 # PURPOSE: download local AVISO FES files with ftp server
-def aviso_fes_tides(MODEL, DIRECTORY=None, USER='', PASSWORD='', LOAD=False,
-    CURRENTS=False, GZIP=False, LOG=False, MODE=None):
+def aviso_fes_tides(MODEL: str,
+    DIRECTORY: str | pathlib.Path | None = None,
+    USER: str = '',
+    PASSWORD: str = '',
+    LOAD: bool = False,
+    CURRENTS: bool = False,
+    GZIP: bool = False,
+    TIMEOUT: int | None = None,
+    LOG: bool = False,
+    MODE: oct = 0o775):
 
     # connect and login to AVISO ftp server
-    f = ftplib.FTP('ftp-access.aviso.altimetry.fr',timeout=1000)
+    f = ftplib.FTP('ftp-access.aviso.altimetry.fr', timeout=TIMEOUT)
     f.login(USER, PASSWORD)
     # check if local directory exists and recursively create if not
     localpath = pathlib.Path(DIRECTORY).joinpath(MODEL.lower()).expanduser()
     localpath.mkdir(MODE, parents=True, exist_ok=True)
 
     # create log file with list of downloaded files (or print to terminal)
     if LOG:
@@ -158,15 +169,15 @@
     for remotepath,tarmode,flatten in zip(FES[MODEL],TAR[MODEL],FLATTEN[MODEL]):
         # download file from ftp and decompress tar files
         ftp_download_file(logger,f,remotepath,localpath,tarmode,flatten,GZIP,MODE)
     # close the ftp connection
     f.quit()
     # close log file and set permissions level to MODE
     if LOG:
-        LOGFILE.chmod(MODE)
+        LOGFILE.chmod(mode=MODE)
 
 # PURPOSE: pull file from a remote ftp server and decompress if tar file
 def ftp_download_file(logger,ftp,remote_path,local_dir,tarmode,flatten,GZIP,MODE):
     # remote and local directory for data product
     remote_file = posixpath.join('auxiliary','tide_model',*remote_path)
 
     # Printing files transferred
@@ -200,28 +211,28 @@
                 local_file.parent.mkdir(mode=MODE, parents=True, exist_ok=True)
                 # extract file to local directory
                 with tar.extractfile(m) as fi,open(local_file, 'wb') as fo:
                     shutil.copyfileobj(fi, fo)
             # get last modified date of remote file within tar file
             # keep remote modification time of file and local access time
             pathlib.os.utime(local_file, (local_file.stat().st_atime, m.mtime))
-            local_file.chmod(MODE)
+            local_file.chmod(mode=MODE)
     else:
         # copy readme and uncompressed files directly
         local_file = local_dir.joinpath(local_dir,remote_path[-1])
         logger.info(f'\t{str(local_file)}\n')
         # copy remote file contents to local file
         with local_file.open('wb') as f:
             ftp.retrbinary(f'RETR {remote_file}', f.write)
         # get last modified date of remote file and convert into unix time
         mdtm = ftp.sendcmd(f'MDTM {remote_file}')
         remote_mtime = calendar.timegm(time.strptime(mdtm[4:],"%Y%m%d%H%M%S"))
         # keep remote modification time of file and local access time
         pathlib.os.utime(local_file, (local_file.stat().st_atime, remote_mtime))
-        local_file.chmod(MODE)
+        local_file.chmod(mode=MODE)
 
 # PURPOSE: create argument parser
 def arguments():
     parser = argparse.ArgumentParser(
         description="""Downloads the FES (Finite Element Solution) global tide
             model from AVISO.  Decompresses the model tar files into the
             constituent files and auxiliary files.
@@ -257,14 +268,18 @@
     parser.add_argument('--currents',
         default=False, action='store_true',
         help='Download tide model current outputs')
     # download FES tidal currents
     parser.add_argument('--gzip','-G',
         default=False, action='store_true',
         help='Compress output ascii and netCDF4 tide files')
+    # connection timeout
+    parser.add_argument('--timeout','-t',
+        type=int, default=360,
+        help='Timeout in seconds for blocking operations')
     # Output log file in form
     # AVISO_FES_tides_2002-04-01.log
     parser.add_argument('--log','-l',
         default=False, action='store_true',
         help='Output log file')
     # permissions mode of the local directories and files (number in octal)
     parser.add_argument('--mode','-M',
@@ -299,13 +314,14 @@
             aviso_fes_tides(m,
                 DIRECTORY=args.directory,
                 USER=args.user,
                 PASSWORD=args.password,
                 LOAD=args.load,
                 CURRENTS=args.currents,
                 GZIP=args.gzip,
+                TIMEOUT=args.timeout,
                 LOG=args.log,
                 MODE=args.mode)
 
 # run main program
 if __name__ == '__main__':
     main()
```

### Comparing `pyTMD-2.0.4/scripts/compute_LPET_elevations.py` & `pyTMD-2.0.5/scripts/compute_LPET_elevations.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,15 +255,15 @@
         pyTMD.spatial.to_netCDF4(output, attrib, output_file, data_type=TYPE)
     elif (FORMAT == 'HDF5'):
         pyTMD.spatial.to_HDF5(output, attrib, output_file)
     elif (FORMAT == 'geotiff'):
         pyTMD.spatial.to_geotiff(output, attrib, output_file,
             varname='tide_lpe')
     # change the permissions level to MODE
-    output_file.chmod(MODE)
+    output_file.chmod(mode=MODE)
 
 # PURPOSE: create argument parser
 def arguments():
     parser = argparse.ArgumentParser(
         description="""Calculates long-period equilibrium tidal elevations for
             an input file
             """,
@@ -336,15 +336,15 @@
     # Read the system arguments listed after the program
     parser = arguments()
     args,_ = parser.parse_known_args()
 
     # set output file from input filename if not entered
     if not args.outfile:
         vars = (args.infile.stem,'lpe_tide',args.infile.suffix)
-        args.outfile = '{0}_{1}{2}'.format(*vars)
+        args.outfile = args.infile.with_name('{0}_{1}{2}'.format(*vars))
 
     # run long period equilibrium tide program for input file
     compute_LPET_elevations(args.infile, args.outfile,
         FORMAT=args.format,
         VARIABLES=args.variables,
         HEADER=args.header,
         DELIMITER=args.delimiter,
```

### Comparing `pyTMD-2.0.4/scripts/compute_LPT_displacements.py` & `pyTMD-2.0.5/scripts/compute_LPT_displacements.py`

 * *Files 1% similar despite different names*

```diff
@@ -326,15 +326,15 @@
         pyTMD.spatial.to_netCDF4(output, attrib, output_file, data_type=TYPE)
     elif (FORMAT == 'HDF5'):
         pyTMD.spatial.to_HDF5(output, attrib, output_file)
     elif (FORMAT == 'geotiff'):
         pyTMD.spatial.to_geotiff(output, attrib, output_file,
             varname='tide_pole')
     # change the permissions level to MODE
-    output_file.chmod(MODE)
+    output_file.chmod(mode=MODE)
 
 # PURPOSE: create argument parser
 def arguments():
     parser = argparse.ArgumentParser(
         description="""Calculates radial pole load tide displacements for
             an input file following IERS Convention (2010) guidelines
             """,
@@ -415,15 +415,15 @@
     # Read the system arguments listed after the program
     parser = arguments()
     args,_ = parser.parse_known_args()
 
     # set output file from input filename if not entered
     if not args.outfile:
         vars = (args.infile.stem,'pole_tide',args.infile.suffix)
-        args.outfile = '{0}_{1}{2}'.format(*vars)
+        args.outfile = args.infile.with_name('{0}_{1}{2}'.format(*vars))
 
     # run load pole tide program for input file
     compute_LPT_displacements(args.infile, args.outfile,
         FORMAT=args.format,
         VARIABLES=args.variables,
         HEADER=args.header,
         DELIMITER=args.delimiter,
```

### Comparing `pyTMD-2.0.4/scripts/compute_OPT_displacements.py` & `pyTMD-2.0.5/scripts/compute_OPT_displacements.py`

 * *Files 1% similar despite different names*

```diff
@@ -365,15 +365,15 @@
         pyTMD.spatial.to_netCDF4(output, attrib, output_file, data_type=TYPE)
     elif (FORMAT == 'HDF5'):
         pyTMD.spatial.to_HDF5(output, attrib, output_file)
     elif (FORMAT == 'geotiff'):
         pyTMD.spatial.to_geotiff(output, attrib, output_file,
             varname='tide_oc_pole')
     # change the permissions level to MODE
-    output_file.chmod(MODE)
+    output_file.chmod(mode=MODE)
 
 # PURPOSE: create argument parser
 def arguments():
     parser = argparse.ArgumentParser(
         description="""Calculates radial ocean pole load tide displacements for
             an input file following IERS Convention (2010) guidelines
             """,
@@ -459,15 +459,15 @@
     # Read the system arguments listed after the program
     parser = arguments()
     args,_ = parser.parse_known_args()
 
     # set output file from input filename if not entered
     if not args.outfile:
         vars = (args.infile.stem,'ocean_pole_tide',args.infile.suffix)
-        args.outfile = '{0}_{1}{2}'.format(*vars)
+        args.outfile = args.infile.with_name('{0}_{1}{2}'.format(*vars))
 
     # run ocean pole tide program for input file
     compute_OPT_displacements(args.infile, args.outfile,
         FORMAT=args.format,
         VARIABLES=args.variables,
         HEADER=args.header,
         DELIMITER=args.delimiter,
```

### Comparing `pyTMD-2.0.4/scripts/compute_SET_displacements.py` & `pyTMD-2.0.5/scripts/compute_SET_displacements.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,15 +333,15 @@
         pyTMD.spatial.to_netCDF4(output, attrib, output_file, data_type=TYPE)
     elif (FORMAT == 'HDF5'):
         pyTMD.spatial.to_HDF5(output, attrib, output_file)
     elif (FORMAT == 'geotiff'):
         pyTMD.spatial.to_geotiff(output, attrib, output_file,
             varname='tide_se')
     # change the permissions level to MODE
-    output_file.chmod(MODE)
+    output_file.chmod(mode=MODE)
 
 # PURPOSE: create argument parser
 def arguments():
     parser = argparse.ArgumentParser(
         description="""Calculates solid earth load tide displacements for
             an input file following IERS Convention (2010) guidelines
             """,
@@ -426,15 +426,15 @@
     # Read the system arguments listed after the program
     parser = arguments()
     args,_ = parser.parse_known_args()
 
     # set output file from input filename if not entered
     if not args.outfile:
         vars = (args.infile.stem,'solid_earth_tide',args.infile.suffix)
-        args.outfile = '{0}_{1}{2}'.format(*vars)
+        args.outfile = args.infile.with_name('{0}_{1}{2}'.format(*vars))
 
     # run solid earth tide program for input file
     compute_SET_displacements(args.infile, args.outfile,
         FORMAT=args.format,
         VARIABLES=args.variables,
         HEADER=args.header,
         DELIMITER=args.delimiter,
```

### Comparing `pyTMD-2.0.4/scripts/compute_tidal_currents.py` & `pyTMD-2.0.5/scripts/compute_tidal_currents.py`

 * *Files 0% similar despite different names*

```diff
@@ -379,15 +379,15 @@
     elif (FORMAT == 'geotiff'):
         # merge current variables into a single variable
         output['data'] = np.concatenate((output['u'],output['v']),axis=-1)
         attrib['data'] = {'_FillValue':fill_value}
         pyTMD.spatial.to_geotiff(output, attrib, output_file,
             varname='data')
     # change the permissions level to MODE
-    output_file.chmod(MODE)
+    output_file.chmod(mode=MODE)
 
 # PURPOSE: create argument parser
 def arguments():
     parser = argparse.ArgumentParser(
         description="""Calculates zonal and meridional tidal currents for
             an input file
             """,
@@ -494,15 +494,15 @@
     # Read the system arguments listed after the program
     parser = arguments()
     args,_ = parser.parse_known_args()
 
     # set output file from input filename if not entered
     if not args.outfile:
         vars = (args.infile.stem,args.tide,'_currents',args.infile.suffix)
-        args.outfile = '{0}_{1}{2}{3}'.format(*vars)
+        args.outfile = args.infile.with_name('{0}_{1}{2}{3}'.format(*vars))
 
     # run tidal current program for input file
     compute_tidal_currents(args.directory, args.infile, args.outfile,
         TIDE_MODEL=args.tide,
         ATLAS_FORMAT=args.atlas_format,
         GZIP=args.gzip,
         DEFINITION_FILE=args.definition_file,
```

### Comparing `pyTMD-2.0.4/scripts/compute_tidal_elevations.py` & `pyTMD-2.0.5/scripts/compute_tidal_elevations.py`

 * *Files 1% similar despite different names*

```diff
@@ -376,15 +376,15 @@
         pyTMD.spatial.to_netCDF4(output, attrib, output_file, data_type=TYPE)
     elif (FORMAT == 'HDF5'):
         pyTMD.spatial.to_HDF5(output, attrib, output_file)
     elif (FORMAT == 'geotiff'):
         pyTMD.spatial.to_geotiff(output, attrib, output_file,
             varname=output_variable)
     # change the permissions level to MODE
-    output_file.chmod(MODE)
+    output_file.chmod(mode=MODE)
 
 # PURPOSE: create argument parser
 def arguments():
     parser = argparse.ArgumentParser(
         description="""Calculates tidal elevations for an input file
             """,
         fromfile_prefix_chars="@"
@@ -496,15 +496,15 @@
     parser = arguments()
     args,_ = parser.parse_known_args()
 
     # set output file from input filename if not entered
     if not args.outfile:
         flexure_flag = '_FLEXURE' if args.apply_flexure else ''
         vars = (args.infile.stem,args.tide,flexure_flag,args.infile.suffix)
-        args.outfile = '{0}_{1}{2}{3}'.format(*vars)
+        args.outfile = args.infile.with_name('{0}_{1}{2}{3}'.format(*vars))
 
     # run tidal elevation program for input file
     compute_tidal_elevations(args.directory, args.infile, args.outfile,
         TIDE_MODEL=args.tide,
         ATLAS_FORMAT=args.atlas_format,
         GZIP=args.gzip,
         DEFINITION_FILE=args.definition_file,
```

### Comparing `pyTMD-2.0.4/scripts/reduce_OTIS_files.py` & `pyTMD-2.0.5/scripts/reduce_OTIS_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
     mz1 = np.zeros((ny,nx),dtype='>i4')
     hz1[:,:] = hz[indy,indx].reshape(ny,nx)
     mz1[:,:] = mz[indy,indx].reshape(ny,nx)
     # output reduced grid to file
     new_grid_file = create_unique_filename(model.grid_file)
     pyTMD.io.OTIS.output_otis_grid(new_grid_file,xlim,ylim,hz1,mz1,iob,dt)
     # change the permissions level to MODE
-    new_grid_file.chmod(MODE)
+    new_grid_file.chmod(mode=MODE)
 
     # combine ATLAS sub-grids into single output grid
     # reduce elevation files to bounds
     try:
         # get parameters for tide model
         model = model.elevation(TIDE_MODEL)
     except Exception as exc:
@@ -164,15 +164,15 @@
             # reduce elevation to new bounds
             z1[:,:,i] = z[indy,indx].reshape(ny,nx)
         # output reduced elevation components
         new_model_file['z'] = create_unique_filename(model_file['z'])
         pyTMD.io.OTIS.output_otis_elevation(new_model_file['z'], z1,
             xlim, ylim, constituents)
         # change the permissions level to MODE
-        new_model_file['z'].chmod(MODE)
+        new_model_file['z'].chmod(mode=MODE)
 
     # combine ATLAS sub-grids into single output grid
     # reduce transport files to bounds
     try:
         # get parameters for tide model
         model = model.current(TIDE_MODEL)
     except Exception as exc:
@@ -197,15 +197,15 @@
             u1[:,:,i] = u[indy,indx].reshape(ny,nx)
             v1[:,:,i] = v[indy,indx].reshape(ny,nx)
         # output reduced transport components
         new_model_file['uv'] = create_unique_filename(model_file['u'])
         pyTMD.io.OTIS.output_otis_transport(new_model_file['u'], u1, v1,
             xlim, ylim, constituents)
         # change the permissions level to MODE
-        new_model_file['u'].chmod(MODE)
+        new_model_file['u'].chmod(mode=MODE)
 
 # PURPOSE: create a unique filename adding a numerical instance if existing
 def create_unique_filename(filename):
     # split filename into parts
     filename = pathlib.Path(filename)
     basename = filename.stem
     suffix = '' if (filename.suffix in ('.out','.oce')) else filename.suffix
```

### Comparing `pyTMD-2.0.4/scripts/usap_cats_tides.py` & `pyTMD-2.0.5/scripts/usap_cats_tides.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         # strip directories from member filename
         m.filename = posixpath.basename(m.filename)
         local_file = local_dir.joinpath(m.filename)
         logger.info(f'\t{str(local_file)}\n')
         # extract file
         zfile.extract(m, path=local_dir)
         # change permissions mode
-        local_file.chmod(MODE)
+        local_file.chmod(mode=MODE)
     # close the zipfile object
     zfile.close()
 
 # PURPOSE: create argument parser
 def arguments():
     parser = argparse.ArgumentParser(
         description="""Download Circum-Antarctic Tidal Simulations from the
```

### Comparing `pyTMD-2.0.4/scripts/verify_box_tpxo.py` & `pyTMD-2.0.5/scripts/verify_box_tpxo.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         if sha1 != entry['sha1']:
             logger.critical(f'Remote checksum: {entry["sha1"]}')
             logger.critical(f'Local checksum: {sha1}')
             raise Exception('Checksum verification failed')
         # keep remote modification time of file and local access time
         pathlib.os.utime(local, (local.stat().st_atime, remote_mtime))
         # change the permissions mode of the local file
-        local.chmod(MODE)
+        local.chmod(mode=MODE)
 
 # PURPOSE: create argument parser
 def arguments():
     parser = argparse.ArgumentParser(
         description="""Verifies downloaded TPXO9-atlas global
             tide models from the box file sharing service
             """,
```

### Comparing `pyTMD-2.0.4/setup.py` & `pyTMD-2.0.5/setup.py`

 * *Files identical despite different names*

