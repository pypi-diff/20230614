# Comparing `tmp/neuroshape-0.0.4.3.tar.gz` & `tmp/neuroshape-0.0.4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuroshape-0.0.4.3.tar", last modified: Sun Jun 11 10:22:48 2023, max compression
+gzip compressed data, was "neuroshape-0.0.4.3.1.tar", last modified: Wed Jun 14 05:33:10 2023, max compression
```

## Comparing `neuroshape-0.0.4.3.tar` & `neuroshape-0.0.4.3.1.tar`

### file list

```diff
@@ -1,61 +1,66 @@
-drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-11 10:22:48.858099 neuroshape-0.0.4.3/
--rw-r--r--   0 c3336955   (503) staff       (20)     1501 2023-06-07 11:17:25.000000 neuroshape-0.0.4.3/LICENSE
--rw-r--r--   0 c3336955   (503) staff       (20)     6793 2023-06-11 10:22:48.857577 neuroshape-0.0.4.3/PKG-INFO
--rw-r--r--   0 c3336955   (503) staff       (20)     4445 2023-06-07 11:17:25.000000 neuroshape-0.0.4.3/README.rst
-drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-11 10:22:48.837586 neuroshape-0.0.4.3/neuroshape/
--rw-r--r--   0 c3336955   (503) staff       (20)        0 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/__init__.py
--rw-r--r--   0 c3336955   (503) staff       (20)    21494 2023-06-08 07:46:54.000000 neuroshape-0.0.4.3/neuroshape/connectopic_laplacian.py
--rw-r--r--   0 c3336955   (503) staff       (20)     5054 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/eigenmaps.py
-drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-11 10:22:48.840874 neuroshape-0.0.4.3/neuroshape/nipype/
--rw-r--r--   0 c3336955   (503) staff       (20)        0 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/nipype/__init__.py
-drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-11 10:22:48.841250 neuroshape-0.0.4.3/neuroshape/nipype/interfaces/
--rw-r--r--   0 c3336955   (503) staff       (20)        0 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/nipype/interfaces/__init__.py
-drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-11 10:22:48.842109 neuroshape-0.0.4.3/neuroshape/nipype/interfaces/workbench/
--rw-r--r--   0 c3336955   (503) staff       (20)      269 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/nipype/interfaces/workbench/__init__.py
--rw-r--r--   0 c3336955   (503) staff       (20)    13219 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/nipype/interfaces/workbench/metric.py
-drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-11 10:22:48.845933 neuroshape-0.0.4.3/neuroshape/nulls/
--rw-r--r--   0 c3336955   (503) staff       (20)       44 2023-06-08 02:12:42.000000 neuroshape-0.0.4.3/neuroshape/nulls/__init__.py
--rw-r--r--   0 c3336955   (503) staff       (20)     5351 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/nulls/burt.py
--rw-r--r--   0 c3336955   (503) staff       (20)    20808 2023-06-10 12:03:52.000000 neuroshape-0.0.4.3/neuroshape/nulls/eigenshuff.py
--rw-r--r--   0 c3336955   (503) staff       (20)    11999 2023-06-10 12:04:52.000000 neuroshape-0.0.4.3/neuroshape/nulls/eigensphere.py
--rw-r--r--   0 c3336955   (503) staff       (20)    25239 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/nulls/nulls.py
--rw-r--r--   0 c3336955   (503) staff       (20)    27669 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/nulls/spins.py
-drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-11 10:22:48.848303 neuroshape-0.0.4.3/neuroshape/nulls/tests/
--rw-r--r--   0 c3336955   (503) staff       (20)        0 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/nulls/tests/__init__.py
--rw-r--r--   0 c3336955   (503) staff       (20)      530 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/nulls/tests/test_burt.py
--rw-r--r--   0 c3336955   (503) staff       (20)     4067 2023-06-10 23:16:09.000000 neuroshape-0.0.4.3/neuroshape/nulls/tests/test_eigenresamp.py
--rw-r--r--   0 c3336955   (503) staff       (20)      695 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/nulls/tests/test_nulls.py
--rw-r--r--   0 c3336955   (503) staff       (20)      814 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/nulls/tests/test_spins.py
--rw-r--r--   0 c3336955   (503) staff       (20)    12845 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/nulls/waveshuff.py
--rw-r--r--   0 c3336955   (503) staff       (20)     4078 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/permutation.py
--rw-r--r--   0 c3336955   (503) staff       (20)     5145 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/poly_eigenmaps.py
--rw-r--r--   0 c3336955   (503) staff       (20)     5400 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/stats.py
-drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-11 10:22:48.855561 neuroshape-0.0.4.3/neuroshape/utils/
--rw-r--r--   0 c3336955   (503) staff       (20)       25 2023-06-07 11:17:25.000000 neuroshape-0.0.4.3/neuroshape/utils/__init__.py
--rw-r--r--   0 c3336955   (503) staff       (20)     1345 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/utils/check_fs_subjid.py
--rw-r--r--   0 c3336955   (503) staff       (20)      616 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/utils/check_map.py
--rw-r--r--   0 c3336955   (503) staff       (20)     6553 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/utils/checks.py
--rw-r--r--   0 c3336955   (503) staff       (20)      917 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/utils/compare_parallel.py
--rw-r--r--   0 c3336955   (503) staff       (20)     3501 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/utils/compute_geodesic_distance.py
--rw-r--r--   0 c3336955   (503) staff       (20)     6248 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/utils/concavehull.py
--rw-r--r--   0 c3336955   (503) staff       (20)    10348 2023-06-11 10:15:49.000000 neuroshape-0.0.4.3/neuroshape/utils/eigen.py
--rw-r--r--   0 c3336955   (503) staff       (20)    25397 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/utils/fs_shapeDNA.py
--rw-r--r--   0 c3336955   (503) staff       (20)     9310 2023-06-07 11:17:25.000000 neuroshape-0.0.4.3/neuroshape/utils/geometry.py
--rw-r--r--   0 c3336955   (503) staff       (20)      348 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/utils/load_mesh_vertices.py
--rw-r--r--   0 c3336955   (503) staff       (20)     2639 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/utils/meshtransforms.py
--rw-r--r--   0 c3336955   (503) staff       (20)      201 2023-06-11 10:05:42.000000 neuroshape-0.0.4.3/neuroshape/utils/swap_single_row.py
--rw-r--r--   0 c3336955   (503) staff       (20)      540 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/utils/tmpname.py
--rw-r--r--   0 c3336955   (503) staff       (20)      193 2023-06-03 12:09:04.000000 neuroshape-0.0.4.3/neuroshape/utils/zscore_avg_method.py
--rw-r--r--   0 c3336955   (503) staff       (20)    15295 2023-06-07 11:17:25.000000 neuroshape-0.0.4.3/neuroshape/volume_eigenmodes.py
-drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-11 10:22:48.840423 neuroshape-0.0.4.3/neuroshape.egg-info/
--rw-r--r--   0 c3336955   (503) staff       (20)     6793 2023-06-11 10:22:48.000000 neuroshape-0.0.4.3/neuroshape.egg-info/PKG-INFO
--rw-r--r--   0 c3336955   (503) staff       (20)     1479 2023-06-11 10:22:48.000000 neuroshape-0.0.4.3/neuroshape.egg-info/SOURCES.txt
--rw-r--r--   0 c3336955   (503) staff       (20)        1 2023-06-11 10:22:48.000000 neuroshape-0.0.4.3/neuroshape.egg-info/dependency_links.txt
--rw-r--r--   0 c3336955   (503) staff       (20)       11 2023-06-11 10:22:48.000000 neuroshape-0.0.4.3/neuroshape.egg-info/top_level.txt
--rw-r--r--   0 c3336955   (503) staff       (20)      618 2023-06-11 10:22:46.000000 neuroshape-0.0.4.3/pyproject.toml
--rw-r--r--   0 c3336955   (503) staff       (20)       38 2023-06-11 10:22:48.858253 neuroshape-0.0.4.3/setup.cfg
--rw-r--r--   0 c3336955   (503) staff       (20)     1039 2023-06-11 10:22:27.000000 neuroshape-0.0.4.3/setup.py
-drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-11 10:22:48.856879 neuroshape-0.0.4.3/src/
--rw-r--r--   0 c3336955   (503) staff       (20)     4664 2023-06-06 11:30:08.000000 neuroshape-0.0.4.3/src/eta_squared.c
--rw-r--r--   0 c3336955   (503) staff       (20)     2545 2023-06-06 10:51:35.000000 neuroshape-0.0.4.3/src/euler_threshold.c
--rw-r--r--   0 c3336955   (503) staff       (20)     5946 2023-06-06 00:28:41.000000 neuroshape-0.0.4.3/src/glmfit.c
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-14 05:33:10.976475 neuroshape-0.0.4.3.1/
+-rw-r--r--   0 nik        (502) admin       (80)     1501 2023-06-07 02:08:37.000000 neuroshape-0.0.4.3.1/LICENSE
+-rw-r--r--   0 nik        (502) admin       (80)      470 2023-06-14 05:33:10.976178 neuroshape-0.0.4.3.1/PKG-INFO
+-rw-r--r--   0 nik        (502) admin       (80)     4445 2023-06-08 03:48:59.000000 neuroshape-0.0.4.3.1/README.rst
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-14 05:33:10.963008 neuroshape-0.0.4.3.1/neuroshape/
+-rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)    21316 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.1/neuroshape/connectopic_laplacian.py
+-rw-r--r--   0 nik        (502) admin       (80)     5054 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/eigenmaps.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-14 05:33:10.964486 neuroshape-0.0.4.3.1/neuroshape/nipype/
+-rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/nipype/__init__.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-14 05:33:10.964708 neuroshape-0.0.4.3.1/neuroshape/nipype/interfaces/
+-rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/nipype/interfaces/__init__.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-14 05:33:10.965237 neuroshape-0.0.4.3.1/neuroshape/nipype/interfaces/workbench/
+-rw-r--r--   0 nik        (502) admin       (80)      269 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/nipype/interfaces/workbench/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)    13219 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/nipype/interfaces/workbench/metric.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-14 05:33:10.967463 neuroshape-0.0.4.3.1/neuroshape/nulls/
+-rw-r--r--   0 nik        (502) admin       (80)       44 2023-06-08 03:48:59.000000 neuroshape-0.0.4.3.1/neuroshape/nulls/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)     5351 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/nulls/burt.py
+-rw-r--r--   0 nik        (502) admin       (80)    20808 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.1/neuroshape/nulls/eigenshuff.py
+-rw-r--r--   0 nik        (502) admin       (80)    11999 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.1/neuroshape/nulls/eigensphere.py
+-rw-r--r--   0 nik        (502) admin       (80)    25239 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/nulls/nulls.py
+-rw-r--r--   0 nik        (502) admin       (80)    27669 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/nulls/spins.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-14 05:33:10.969242 neuroshape-0.0.4.3.1/neuroshape/nulls/tests/
+-rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/nulls/tests/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)     4890 2023-06-13 05:36:45.000000 neuroshape-0.0.4.3.1/neuroshape/nulls/tests/eigenmode_replication.py
+-rw-r--r--   0 nik        (502) admin       (80)      530 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/nulls/tests/test_burt.py
+-rw-r--r--   0 nik        (502) admin       (80)     4194 2023-06-13 04:35:26.000000 neuroshape-0.0.4.3.1/neuroshape/nulls/tests/test_eigenresamp.py
+-rw-r--r--   0 nik        (502) admin       (80)      695 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/nulls/tests/test_nulls.py
+-rw-r--r--   0 nik        (502) admin       (80)      814 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/nulls/tests/test_spins.py
+-rw-r--r--   0 nik        (502) admin       (80)    12845 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/nulls/waveshuff.py
+-rw-r--r--   0 nik        (502) admin       (80)     4078 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/permutation.py
+-rw-r--r--   0 nik        (502) admin       (80)     5155 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.1/neuroshape/poly_eigenmaps.py
+-rw-r--r--   0 nik        (502) admin       (80)    13885 2023-06-14 05:13:56.000000 neuroshape-0.0.4.3.1/neuroshape/recon.py
+-rw-r--r--   0 nik        (502) admin       (80)     5400 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/stats.py
+-rw-r--r--   0 nik        (502) admin       (80)    11313 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.1/neuroshape/surface_eigenmodes.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-14 05:33:10.974722 neuroshape-0.0.4.3.1/neuroshape/utils/
+-rw-r--r--   0 nik        (502) admin       (80)       25 2023-06-07 00:31:38.000000 neuroshape-0.0.4.3.1/neuroshape/utils/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)     1345 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/utils/check_fs_subjid.py
+-rw-r--r--   0 nik        (502) admin       (80)      616 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/utils/check_map.py
+-rw-r--r--   0 nik        (502) admin       (80)     6553 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/utils/checks.py
+-rw-r--r--   0 nik        (502) admin       (80)      917 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/utils/compare_parallel.py
+-rw-r--r--   0 nik        (502) admin       (80)     3501 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/utils/compute_geodesic_distance.py
+-rw-r--r--   0 nik        (502) admin       (80)     6248 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/utils/concavehull.py
+-rw-r--r--   0 nik        (502) admin       (80)    12515 2023-06-14 04:42:48.000000 neuroshape-0.0.4.3.1/neuroshape/utils/eigen.py
+-rw-r--r--   0 nik        (502) admin       (80)      763 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.1/neuroshape/utils/fetch_atlas.py
+-rw-r--r--   0 nik        (502) admin       (80)    25397 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/utils/fs_shapeDNA.py
+-rw-r--r--   0 nik        (502) admin       (80)    27112 2023-06-13 07:24:43.000000 neuroshape-0.0.4.3.1/neuroshape/utils/geometry.py
+-rw-r--r--   0 nik        (502) admin       (80)      348 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/utils/load_mesh_vertices.py
+-rw-r--r--   0 nik        (502) admin       (80)     2639 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/utils/meshtransforms.py
+-rw-r--r--   0 nik        (502) admin       (80)      222 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.1/neuroshape/utils/normalize_data.py
+-rw-r--r--   0 nik        (502) admin       (80)      201 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/utils/swap_single_row.py
+-rw-r--r--   0 nik        (502) admin       (80)      540 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/utils/tmpname.py
+-rw-r--r--   0 nik        (502) admin       (80)      193 2023-06-04 23:43:38.000000 neuroshape-0.0.4.3.1/neuroshape/utils/zscore_avg_method.py
+-rw-r--r--   0 nik        (502) admin       (80)     9467 2023-06-13 01:26:03.000000 neuroshape-0.0.4.3.1/neuroshape/volume_eigenmodes.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-14 05:33:10.964208 neuroshape-0.0.4.3.1/neuroshape.egg-info/
+-rw-r--r--   0 nik        (502) admin       (80)      470 2023-06-14 05:33:10.000000 neuroshape-0.0.4.3.1/neuroshape.egg-info/PKG-INFO
+-rw-r--r--   0 nik        (502) admin       (80)     1647 2023-06-14 05:33:10.000000 neuroshape-0.0.4.3.1/neuroshape.egg-info/SOURCES.txt
+-rw-r--r--   0 nik        (502) admin       (80)        1 2023-06-14 05:33:10.000000 neuroshape-0.0.4.3.1/neuroshape.egg-info/dependency_links.txt
+-rw-r--r--   0 nik        (502) admin       (80)       11 2023-06-14 05:33:10.000000 neuroshape-0.0.4.3.1/neuroshape.egg-info/top_level.txt
+-rw-r--r--   0 nik        (502) admin       (80)      620 2023-06-14 05:32:56.000000 neuroshape-0.0.4.3.1/pyproject.toml
+-rw-r--r--   0 nik        (502) admin       (80)       38 2023-06-14 05:33:10.976579 neuroshape-0.0.4.3.1/setup.cfg
+-rw-r--r--   0 nik        (502) admin       (80)     1041 2023-06-14 05:33:07.000000 neuroshape-0.0.4.3.1/setup.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-14 05:33:10.975769 neuroshape-0.0.4.3.1/src/
+-rw-r--r--   0 nik        (502) admin       (80)     5389 2023-06-09 06:16:05.000000 neuroshape-0.0.4.3.1/src/eta_squared.c
+-rw-r--r--   0 nik        (502) admin       (80)     2545 2023-06-06 05:49:54.000000 neuroshape-0.0.4.3.1/src/euler_threshold.c
+-rw-r--r--   0 nik        (502) admin       (80)     5946 2023-06-06 05:46:53.000000 neuroshape-0.0.4.3.1/src/glmfit.c
```

### Comparing `neuroshape-0.0.4.3/LICENSE` & `neuroshape-0.0.4.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3/README.rst` & `neuroshape-0.0.4.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3/neuroshape/connectopic_laplacian.py` & `neuroshape-0.0.4.3.1/neuroshape/connectopic_laplacian.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,20 +13,20 @@
     $ python connectopic_laplacian.py ${data_input_filename} ${data_roi_filename} ${mask_filename} ${data_output_filename} -N ${num_gradients} --smoothing ${fwhm} --filtering
 
 @author: Nikitas C. Koussis, Systems Neuroscience Group Newcastle, 2023
 """
 
 import nibabel as nib
 import numpy as np
-from scipy.signal import detrend
 from scipy.ndimage import gaussian_filter
 from scipy.spatial.distance import pdist, squareform
 from scipy.sparse.csgraph import laplacian
 from numpy.linalg import svd
 from numpy.linalg import eigh
+from neuroshape.utils.normalize_data import normalize_data
 import os
 from argparse import ArgumentParser
 from nilearn import image, masking
 from subprocess import Popen
 from neuroshape.eta import eta_squared
 from neuroshape.euler import euler_threshold
 from os.path import split
@@ -136,20 +136,14 @@
     
     os.system(f'rm -f {script_file}')  
     output_filename = input_filename.replace('.nii','_filtered.nii')
     print("Saving filtered file to {}".format(output_filename))
     
     return output_filename
 
-def normalize_data(data):
-    data_normalized = np.subtract(data, np.mean(data, axis=0))
-    data_normalized = np.divide(data_normalized, np.std(data_normalized, axis=0))
-    
-    return data_normalized
-
 def compute_similarity(img_input, img_roi, img_mask):
     data_msk = masking.apply_mask(img_input, img_mask)
     print('Normalizing input timeseries')
     data_msk = normalize_data(data_msk)
     input_img = masking.unmask(data_msk, img_mask)
     
     data_ins = masking.apply_mask(input_img, img_roi)
@@ -370,15 +364,15 @@
         cort_filename = data_output_filename.replace('.nii.gz','_cortical_projection.nii.gz')
         print('Saving cortical projection file to {}'.cort_filename)
         
         nib.save(cort_img, cort_filename)
         
         
     
-    # save figures TODO
+    # TODO save figures
     
 
 
 def main(raw_args=None):
     
     #fmt = "%(asctime)s,%(msecs)d %(name)-2s " "%(levelname)-2s:\n\t %(message)s"
     #datefmt = "%y%m%d-%H:%M:%S"
```

### Comparing `neuroshape-0.0.4.3/neuroshape/eigenmaps.py` & `neuroshape-0.0.4.3.1/neuroshape/eigenmaps.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3/neuroshape/nipype/interfaces/workbench/metric.py` & `neuroshape-0.0.4.3.1/neuroshape/nipype/interfaces/workbench/metric.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3/neuroshape/nulls/burt.py` & `neuroshape-0.0.4.3.1/neuroshape/nulls/burt.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3/neuroshape/nulls/eigenshuff.py` & `neuroshape-0.0.4.3.1/neuroshape/nulls/eigenshuff.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3/neuroshape/nulls/eigensphere.py` & `neuroshape-0.0.4.3.1/neuroshape/nulls/eigensphere.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3/neuroshape/nulls/nulls.py` & `neuroshape-0.0.4.3.1/neuroshape/nulls/nulls.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3/neuroshape/nulls/spins.py` & `neuroshape-0.0.4.3.1/neuroshape/nulls/spins.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3/neuroshape/nulls/tests/test_burt.py` & `neuroshape-0.0.4.3.1/neuroshape/nulls/tests/test_burt.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3/neuroshape/nulls/tests/test_eigenresamp.py` & `neuroshape-0.0.4.3.1/neuroshape/nulls/tests/test_eigenresamp.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 from nilearn import plotting
 
 cmap = plt.get_cmap('bone_r')
 fontcolor = 'black'
 
 from neuroshape.nulls.eigensphere import eigenmode_resample
 
-def test_resampling(surface, evals, emodes, n=201, decomp_method='matrix'):
+def test_resampling(surface, evals, emodes, n=201, decomp_method='matrix', normalize=None):
     """
     Compute a single eigensphere resampled surrogate at modes = `n`
     """
     # test resampling
-    new_vertices = eigenmode_resample(surface, evals, emodes, decomp_method=decomp_method)
+    new_vertices = eigenmode_resample(surface, evals, emodes, decomp_method=decomp_method, normalize=normalize)
     
     #plot_surface(new_surface)
 
     return new_vertices
 
-def test_surrogates(surface_filename, n=201, num_surrogates=100):
+def test_surrogates(surface_filename, n=201, num_surrogates=100, normalize=None):
     """
     Compute a number of eigensphere resampled surrogates at modes = `n`
     """
     # load surface
     surface = nib.load(surface_filename)
     
     # make TriaMesh
@@ -48,16 +48,19 @@
     emodes = ev['Eigenvectors'][:,1:]
     emodes = emodes/np.linalg.norm(emodes, axis=0)
     evals = ev['Eigenvalues'][1:]
     
     # initialize the surrogate array - compute only the vertices, the faces are the same
     new_surfaces = np.zeros((num_surrogates, coords.shape[0], coords.shape[1]))
     
+    if normalize:
+        normalize = normalize
+    
     for i in range(num_surrogates):
-        new_surfaces[i] = test_resampling(surface, evals, emodes, n=200, decomp_method='regression')
+        new_surfaces[i] = test_resampling(surface, evals, emodes, n=200, decomp_method='regression', normalize=normalize)
     
     return new_surfaces
 
 def test_plot_surfaces(surface, new_surfaces, n=201, data=None, hemi='left', view='lateral', vmin=None, vmax=None, cmap='bone_r', show=True):
     # plot a number of new surfaces and compare to the original
     fig = plt.figure(figsize=(20, 7), constrained_layout=False)
     grid = gridspec.GridSpec(
```

### Comparing `neuroshape-0.0.4.3/neuroshape/nulls/tests/test_nulls.py` & `neuroshape-0.0.4.3.1/neuroshape/nulls/tests/test_nulls.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3/neuroshape/nulls/tests/test_spins.py` & `neuroshape-0.0.4.3.1/neuroshape/nulls/tests/test_spins.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3/neuroshape/nulls/waveshuff.py` & `neuroshape-0.0.4.3.1/neuroshape/nulls/waveshuff.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3/neuroshape/permutation.py` & `neuroshape-0.0.4.3.1/neuroshape/permutation.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3/neuroshape/poly_eigenmaps.py` & `neuroshape-0.0.4.3.1/neuroshape/poly_eigenmaps.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from lapy import TriaMesh
 from lapy.ShapeDNA import compute_shapedna
 import numpy as np
 from joblib import Parallel, delayed
-from .utils.dataio import dataio
+from brainsmash.utils.dataio import dataio
 from pathlib import Path
 
 __all__ = ['PolyLBO']
 
 class PolyLBO:
     """
     Description
```

### Comparing `neuroshape-0.0.4.3/neuroshape/stats.py` & `neuroshape-0.0.4.3.1/neuroshape/stats.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3/neuroshape/utils/check_fs_subjid.py` & `neuroshape-0.0.4.3.1/neuroshape/utils/check_fs_subjid.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3/neuroshape/utils/check_map.py` & `neuroshape-0.0.4.3.1/neuroshape/utils/check_map.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3/neuroshape/utils/checks.py` & `neuroshape-0.0.4.3.1/neuroshape/utils/checks.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3/neuroshape/utils/compare_parallel.py` & `neuroshape-0.0.4.3.1/neuroshape/utils/compare_parallel.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3/neuroshape/utils/compute_geodesic_distance.py` & `neuroshape-0.0.4.3.1/neuroshape/utils/compute_geodesic_distance.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3/neuroshape/utils/concavehull.py` & `neuroshape-0.0.4.3.1/neuroshape/utils/concavehull.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3/neuroshape/utils/eigen.py` & `neuroshape-0.0.4.3.1/neuroshape/utils/eigen.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,74 +1,143 @@
 import numpy as np
 from neuromaps.stats import compare_images
 from neuroshape.utils.swap_single_row import swap_single_row
 from lapy.TriaMesh import TriaMesh
+from lapy.ShapeDNA import compute_shapedna
+import nibabel as nib
 
 """
 Eigenmode helper functions (C) Systems Neuroscience Newcastle &
 Nikitas C. Koussis 2023
 """
 
-def maximise_recon_metric(eigs, y, metric='corr'):
+def compute_eigenmodes(surface, num_modes=200, nonzero=True):
     """
-    Takes a set of eigenmodes `eigs` and a single eigenmode `y` and swaps 
+    Calculates the eigenmodes and eigenvalues of a given surface.
+
+    Parameters
+    ----------
+    surface : nib.GiftiImage() or tuple of (`vertices`, `faces`)
+        Surface to compute LBO
+        
+    num_modes : int
+        Number of [0 > lambda_0 > ... > lambda_n] modes to return, default 200
+        if `nonzero` is True, return only [lambda_0 > ... > lambda_n] modes.
+        
+    nonzero : bool
+        Flag whether to return the first non-zero `num_modes` or not,
+        default True
+
+    Returns
+    -------
+    evals : np.ndarray of (num_modes,)
+        Eigenvalues [0 > lambda_0 > ... > lambda_n] corresponding to the 
+        eigenvalue solution to the Helmholtz equation solved by Finite Element 
+        Method in [1]
+    emodes : np.ndarray of (n_vertices, num_modes)
+        Eigenmodes corresponding to the eigenfunctions solved by Finite Element
+        Method in [1]
+        
+    References
+    ----------
+    [1] M. Reuter, F.-E. Wolter and N. Peinecke.
+    Laplace-Beltrami spectra as "Shape-DNA" of surfaces and solids.
+    Computer-Aided Design 38 (4), pp.342-366, 2006.
+    http://dx.doi.org/10.1016/j.cad.2005.10.011
+
+    """
+    
+    if isinstance(surface, nib.GiftiImage):
+        coords, faces = (surface.darrays[0].data, surface.darrays[1].data)
+        
+    if type(surface) == tuple:
+        coords, faces = surface
+        
+    if not isinstance(coords, np.ndarray) or not isinstance(faces, np.ndarray):
+        raise ValueError("Input surface must be a tuple or nib.GiftiImage class with two arrays `vertices` and `faces`")
+    if coords.shape[1] != faces.shape[1] and coords.shape[1] != 3:
+        # try transpose?
+        if coords.shape[0] == faces.shape[1]:
+            coords = coords.T
+        else:
+            raise ValueError("Input surface has incorrect number of dimensions, must be 3-D")
+            
+    # make surface a TriaMesh
+    tria = TriaMesh(coords, faces)
+    
+    # compute shapedna
+    ev = compute_shapedna(tria, k=num_modes+1)
+    
+    if nonzero is True:
+        evals = ev['Eigenvalues'][1:]
+        emodes = ev['Eigenmodes'][:, 1:]
+    
+    else:
+        evals = ev['Eigenvalues']
+        emodes = ev['Eigenmodes']
+    
+    return evals, emodes
+
+def maximise_recon_metric(emodes, y, metric='corr'):
+    """
+    Takes a set of eigenmodes `emodes` and a single eigenmode `y` and swaps 
     eigenmodes within an eigengroup to maximise `corr` in a
     reconstructed map of `y`. Other metrics are not implemented.
 
     Parameters
     ----------
-    eigs : (N,M) np.ndarray
+    emodes : (N,M) np.ndarray
         Eigenmode array to swap eigenmodes within eigengroups with N 
         eigenmodes and M vertices.
     y : (M,) or (M,1) or (1,M) np.ndarray
         Functional gradient map
     metric : str, optional
         Metric to maximise. The default is 'corr'.
 
     Returns
     -------
-    new_eigs : (N,M) np.ndarray
+    new_emodes : (N,M) np.ndarray
         Eigenmode array that maximises correlation within eigengroups.
     metric_out : float
         Maximized metric value
         
     Raises
     ------
     NotImplementedError : `metric` is not in the implemented classes
 
     """
         
     # swap within groups to maximise metric
     if metric != 'corr':
         raise NotImplementedError('{} is not implemented yet'.format(str(metric)))
         
-    # check if y and eigs in proper orientation
-    if not isinstance(eigs, np.ndarray) or not isinstance(y, np.ndarray):
-        raise TypeError('Eigenmodes and functional maps must be array-like, got type {}, and {}'.format(type(eigs),type(y)))
-    if eigs.ndim != 2 or y.ndim != 1:
-        raise ValueError('Eigenmodes must be 2-D and functional map must be 1-D, got {}D and {}D'.format(eigs.ndim, y.ndim))
-    if eigs.shape[1] != y.shape[0]:
-        if eigs.T.shape[1] == y.shape[0]:
-            eigs = eigs.T
+    # check if y and emodes in proper orientation
+    if not isinstance(emodes, np.ndarray) or not isinstance(y, np.ndarray):
+        raise TypeError('Eigenmodes and functional maps must be array-like, got type {}, and {}'.format(type(emodes),type(y)))
+    if emodes.ndim != 2 or y.ndim != 1:
+        raise ValueError('Eigenmodes must be 2-D and functional map must be 1-D, got {}D and {}D'.format(emodes.ndim, y.ndim))
+    if emodes.shape[1] != y.shape[0]:
+        if emodes.T.shape[1] == y.shape[0]:
+            emodes = emodes.T
         else:
             raise RuntimeError('Eigenmodes and functional maps must be able to be matrix multiplied, fix')
     
-    groups = _get_eigengroups(eigs)
+    groups = _get_eigengroups(emodes)
     
     # iterative swapping of eigenmodes within eigengroup to maximise metric   
-    new_eigs = find_optimum_eigengroups(eigs, y, groups)
+    new_emodes = find_optimum_eigengroups(emodes, y, groups)
     
-    return new_eigs
+    return new_emodes
 
 
-def _get_eigengroups(eigs):
+def _get_eigengroups(emodes):
     """
     Helper function to find eigengroups
     """
-    lam = eigs.shape[1] # number of eigenmodes
+    lam = emodes.shape[1] # number of eigenmodes
     l = np.floor((lam-1)/2).astype(int)    
     if lam == 1:
         return np.asarray([0])
     if lam == 2:
         groups = [np.zeros(1).astype(int)]
         groups.append(np.ones(1).astype(int))
         return groups
@@ -81,32 +150,32 @@
         if ii >= lam:
             groups.append(np.arange(i,lam-1))
             return groups
         groups.append(np.arange(i,ii))
         i = ii
 
 
-def find_optimum_eigengroups(eigs, y, groups, previous_corr=0., tol=0.001):
+def find_optimum_eigengroups(emodes, y, groups, previous_corr=0., tol=0.001):
     #copy original array and transpose for right shape
-    eigs_ = eigs.T
+    emodes_ = emodes.T
     if len(groups) == 2:
         if len(groups[0]) < 2:
-            return eigs_
+            return emodes_
+    
+    for group in groups:
+        emodes_swapped = np.vstack(swap_single_row(emodes_[:, group]))
     
-    eigs_swapped = np.vstack(swap_single_row(eigs_[:, groups[i]]) for i in range(len(groups)))
-    next_betas = np.matmul(eigs_swapped, y)
-    next_recon = np.matmul(next_betas.T, eigs_swapped).reshape(-1,)
+    next_betas = np.matmul(emodes_swapped.T, y)
+    next_recon = np.matmul(next_betas.T, emodes_swapped).reshape(-1,)
     next_corr = compare_images(y, next_recon)
     
-    try:
-        if (next_corr - previous_corr) > tol:
-            return eigs_.T
-    except:
-        return eigs_.T
-    eigs_ = eigs_swapped
+    if (next_corr - previous_corr) > tol:
+        return emodes_.T
+
+    emodes_ = emodes_swapped
     previous_corr = next_corr
     
 
 def reconstruct_surface(surface, eigenmodes, n=100, normalize='area', norm_factor=1, method=None):
     """
     Reconstruct a surface of `n_vertices` given a set of eigenmodes
 
@@ -182,20 +251,17 @@
         
         elif normalize == 'areas':
             areas = orig_tria.vertex_areas()
             tria_norm.v = new_tria.v/(areas ** (1/3))
         
         else:
             pass
+        
         new_vertices = tria_norm.v
         
-    #new_surface = nib.GiftiImage()
-    #new_surface.add_gifti_data_array(nib.gifti.gifti.GiftiDataArray(new_vertices))
-    #new_surface.add_gifti_data_array(nib.gifti.gifti.GiftiDataArray(faces))
-    
     return new_vertices
 
     
 def eigen_decomposition(data, eigenmodes, method='matrix'):
     """
     Decompose data using eigenmodes and calculate the coefficient of 
     contribution of each vector
```

### Comparing `neuroshape-0.0.4.3/neuroshape/utils/fs_shapeDNA.py` & `neuroshape-0.0.4.3.1/neuroshape/utils/fs_shapeDNA.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3/neuroshape/utils/meshtransforms.py` & `neuroshape-0.0.4.3.1/neuroshape/utils/meshtransforms.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3/neuroshape/utils/tmpname.py` & `neuroshape-0.0.4.3.1/neuroshape/utils/tmpname.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3/neuroshape.egg-info/SOURCES.txt` & `neuroshape-0.0.4.3.1/neuroshape.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 pyproject.toml
 setup.py
 neuroshape/__init__.py
 neuroshape/connectopic_laplacian.py
 neuroshape/eigenmaps.py
 neuroshape/permutation.py
 neuroshape/poly_eigenmaps.py
+neuroshape/recon.py
 neuroshape/stats.py
+neuroshape/surface_eigenmodes.py
 neuroshape/volume_eigenmodes.py
 neuroshape.egg-info/PKG-INFO
 neuroshape.egg-info/SOURCES.txt
 neuroshape.egg-info/dependency_links.txt
 neuroshape.egg-info/top_level.txt
 neuroshape/nipype/__init__.py
 neuroshape/nipype/interfaces/__init__.py
@@ -21,29 +23,32 @@
 neuroshape/nulls/burt.py
 neuroshape/nulls/eigenshuff.py
 neuroshape/nulls/eigensphere.py
 neuroshape/nulls/nulls.py
 neuroshape/nulls/spins.py
 neuroshape/nulls/waveshuff.py
 neuroshape/nulls/tests/__init__.py
+neuroshape/nulls/tests/eigenmode_replication.py
 neuroshape/nulls/tests/test_burt.py
 neuroshape/nulls/tests/test_eigenresamp.py
 neuroshape/nulls/tests/test_nulls.py
 neuroshape/nulls/tests/test_spins.py
 neuroshape/utils/__init__.py
 neuroshape/utils/check_fs_subjid.py
 neuroshape/utils/check_map.py
 neuroshape/utils/checks.py
 neuroshape/utils/compare_parallel.py
 neuroshape/utils/compute_geodesic_distance.py
 neuroshape/utils/concavehull.py
 neuroshape/utils/eigen.py
+neuroshape/utils/fetch_atlas.py
 neuroshape/utils/fs_shapeDNA.py
 neuroshape/utils/geometry.py
 neuroshape/utils/load_mesh_vertices.py
 neuroshape/utils/meshtransforms.py
+neuroshape/utils/normalize_data.py
 neuroshape/utils/swap_single_row.py
 neuroshape/utils/tmpname.py
 neuroshape/utils/zscore_avg_method.py
 src/eta_squared.c
 src/euler_threshold.c
 src/glmfit.c
```

### Comparing `neuroshape-0.0.4.3/pyproject.toml` & `neuroshape-0.0.4.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel", "numpy"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neuroshape"
-version = "0.0.4.3"
+version = "0.0.4.3.1"
 description = "For computing connectopic and geometric Laplacian eigenmodes and performing null hypothesis testing. As implementation is ongoing, this description is subject to rapid change."
 readme = "README.rst"
 authors = [
     {name = "Nikitas C. Koussis", email = "nikitas.koussis@gmail.com"},
 ]
 license = { file = "LICENSE" }
```

### Comparing `neuroshape-0.0.4.3/setup.py` & `neuroshape-0.0.4.3.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,14 @@
                    include_dirs=[numpy.get_include()])
 
 euler = Extension('neuroshape.euler', sources=['src/euler_threshold.c'],
                   include_dirs=[numpy.get_include()])
 
 # run the setup
 setup(name='neuroshape',
-      version='0.0.4.3',
+      version='0.0.4.3.1',
       description="For computing connectopic and geometric Laplacian eigenmodes and performing null hypothesis testing. As implementation is ongoing, this description is subject to rapid change.",
       author='Nikitas C. Koussis, Systems Neuroscience Group Newcastle',
       author_email='nikitas.koussis@gmail.com',
       url='https://github.com/nikitas-k/neuroshape-dev',
       packages=find_packages(),
       ext_modules=[eta, glmfit, euler])
```

### Comparing `neuroshape-0.0.4.3/src/eta_squared.c` & `neuroshape-0.0.4.3.1/src/eta_squared.c`

 * *Files 16% similar despite different names*

```diff
@@ -24,119 +24,135 @@
  *
  * For this program to work, numpy.vectorize must be called in
  * in python to generate a numpy-friendly function. See 
  * neuroshape/examples/compute_eta_squared.py for an example
  * 
  */
 
-/* declare main function */
-static PyObject* eta_squared(PyObject* self, PyObject* args);
-
-/*
- * This tells Python what methods this module has
- *
- */
-static PyMethodDef EtaMethods[] = {
-    {"eta_squared",
-        eta_squared,
-        METH_VARARGS, "Compute eta-squared coefficient row-wise of a 2-dimensional array."},
-    {NULL, NULL, 0, NULL}
-};
-
 /*
  * This actually defines the eta squared function for
  * input args from Python.
  */
 
 
 static PyObject* eta_squared(PyObject* self, PyObject* args)
 {
     PyArrayObject* arr;
     if (!PyArg_ParseTuple(args, "O!", &PyArray_Type, &arr))
         return NULL;
     
-    int num_rows = arr->dimensions[0];
-    int num_cols = arr->dimensions[1];
+    int N = arr->dimensions[0];
+    int p = arr->dimensions[1];
+    
     /* check number of dims and whether data is in correct format */
-    if ( num_rows < num_cols ) {
+    if ( N < p ) {
         printf('ERROR: Number of observations must exceed number of features (is your data transposed?)');
         return NULL;    
     }
     npy_intp nd = PyArray_NDIM(arr);
     if ( nd != 2 ) {
         printf('ERROR: Input must be a 2-dimensional matrix');
         return NULL;    
     }
     
-    npy_intp dims[2] = {num_rows, num_rows};
+    npy_intp dims[2] = {N, N};
 
     PyArrayObject* oarr = (PyArrayObject*)PyArray_SimpleNew(nd, dims, NPY_DOUBLE);
     if (oarr == NULL)
         return NULL;
 
-    double* data_ptr = PyArray_DATA(arr);
-    double* out_ptr = PyArray_DATA(oarr);
+    double* z = PyArray_DATA(arr);
+    double* eta = PyArray_DATA(oarr);
 
-    double mu_bar = 0.0;
-    double mu_1 = 0.0;
-    int count = 0;
+    double* mu = (double*)malloc(N * p * sizeof(double));
+    double* mu_bar = (double*)malloc(N * sizeof(double));
     
     npy_intp row_stride = PyArray_STRIDE(arr, 0) / sizeof(double);
     npy_intp col_stride = PyArray_STRIDE(arr, 1) / sizeof(double);
+    npy_intp outrow_stride = PyArray_STRIDE(oarr, 0) / sizeof(double);
+    npy_intp outcol_stride = PyArray_STRIDE(oarr, 1) / sizeof(double);
     
-    npy_intp i,j,k;
+    for (int i = 0; i < N; i++) {
+        // Calculate mu
+        for (int k = 0; k < p; k++) {
+            double sum = 0.0;
+            for (int j = 0; j < N; j++) {
+                if (j != i)
+                    sum += z[j * row_stride + k * col_stride];
+            }
+            mu[k] = (z[i * row_stride + k * col_stride] + sum) / N;
+        }
+
 
-    // Calculate mu_bar
-    for (i = 0; i < num_rows; i++) {
-        for (k = 0; k < num_rows; k++) {
-            for (j = 0; j < num_cols; j++) {
-                double vali = data_ptr[i * row_stride + j * col_stride];
-                double valk = data_ptr[k * row_stride + j * col_stride];
-                double mu = (vali + valk) / 2.0;
-                mu_1 += mu;
-                count++;
+        // Calculate mu_bar
+        for (int k = 0; k < p; k++) {
+            double sum = 0.0;
+            for (int j = 0; j < N; j++) {
+                sum += z[j * p + k];
             }
+            mu_bar[k] = sum / N;
         }
-    }
-    mu_bar = mu_1 / count;
 
-    // Calculate eta-squared coefficients
-    for (i = 0; i < num_rows; i++) {
-        for (k = 0; k < num_rows; k++) {
+        // Calculate eta_squared
+        for (int j = 0; j < N; j++) {
             double num = 0.0;
             double denom = 0.0;
-            for (j = 0; j < num_cols; j++) {
-                double vali = data_ptr[i * row_stride + j * col_stride];
-                double valk = data_ptr[k * row_stride + j * col_stride];
-                double mu = (vali + valk) / 2.0;
-                double diff_a = vali - mu;
-                double diff_b = valk - mu;
-                double powera = diff_a * diff_a;
-                double powerb = diff_b * diff_b;
-                double diff_bar_a = vali - mu_bar;
-                double diff_bar_b = valk - mu_bar;
-                double powerax = diff_bar_a * diff_bar_a;
-                double powerbx = diff_bar_b * diff_bar_b;
-                num += powera + powerb;
-                denom += powerax + powerbx;
-            }
-            if ( denom == 0.0 ){
-                double eta = 0.0;
-                out_ptr[i*num_rows + k] = eta;
-            } else {
-                double eta = 1.0 - (num / denom);
-                out_ptr[i*num_rows + k] = eta;
+            for (int k = 0; k < p; k++) {
+                double diff = z[i * row_stride + k * col_stride] - mu[k];
+                num += diff * diff;
+                double diff_bar = z[j * row_stride + k * col_stride] - mu_bar[k];
+                denom += diff_bar * diff_bar;
             }
-            
+            eta[j * outrow_stride + i * outcol_stride] = 1.0 - (num / denom);
         }
     }
 
-    Py_DECREF(out_ptr);
+    free(mu);
+    free(mu_bar);
+
     return PyArray_Return(oarr);
 }
+//     // Calculate eta-squared coefficients
+//     for (i = 0; i < num_rows; i++) {
+//         for (k = 0; k < num_rows; k++) {
+//             double num = 0.0;
+//             double denom = 0.0;
+//             for (j = 0; j < num_cols; j++) {
+//                 double vali = data_ptr[i * row_stride + j * col_stride];
+//                 double valk = data_ptr[k * row_stride + j * col_stride];
+//                 double mu = (vali + valk) / 2.0;
+//                 double diff_a = vali - mu;
+//                 double diff_b = valk - mu;
+//                 double powera = diff_a * diff_a;
+//                 double powerb = diff_b * diff_b;
+//                 double diff_bar_a = vali - mu_bar;
+//                 double diff_bar_b = valk - mu_bar;
+//                 double powerax = diff_bar_a * diff_bar_a;
+//                 double powerbx = diff_bar_b * diff_bar_b;
+//                 num += powera + powerb;
+//                 denom += powerax + powerbx;
+//             }
+//             if ( denom == 0.0 ){
+//                 double eta = 0.0;
+//                 out_ptr[i*num_rows + k] = eta;
+//             } else {
+//                 double eta = 1.0 - (num / denom);
+//                 out_ptr[i*num_rows + k] = eta;
+//             }
+//             
+//         }
+//     }
+
+
+static PyMethodDef EtaMethods[] = {
+    {"eta_squared",
+        eta_squared,
+        METH_VARARGS, "Compute eta-squared coefficient row-wise of a 2-dimensional array."},
+    {NULL, NULL, 0, NULL}
+};
 
 static struct PyModuleDef cModPyDem = {
     PyModuleDef_HEAD_INIT,
     "neuroshape.eta",
     "Eta-squared 2-dimensional array calculation implementation in C",
     -1,
     EtaMethods
```

### Comparing `neuroshape-0.0.4.3/src/euler_threshold.c` & `neuroshape-0.0.4.3.1/src/euler_threshold.c`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.3/src/glmfit.c` & `neuroshape-0.0.4.3.1/src/glmfit.c`

 * *Files identical despite different names*

