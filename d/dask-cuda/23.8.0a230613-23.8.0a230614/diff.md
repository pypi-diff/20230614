# Comparing `tmp/dask-cuda-23.8.0a230613.tar.gz` & `tmp/dask-cuda-23.8.0a230614.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-cuda-23.8.0a230613.tar", last modified: Tue Jun 13 05:07:26 2023, max compression
+gzip compressed data, was "dask-cuda-23.8.0a230614.tar", last modified: Wed Jun 14 05:07:42 2023, max compression
```

## Comparing `dask-cuda-23.8.0a230613.tar` & `dask-cuda-23.8.0a230614.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 05:07:26.947678 dask-cuda-23.8.0a230613/
--rw-r--r--   0 root         (0) root         (0)    11348 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/LICENSE
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1924 2023-06-13 05:07:26.943678 dask-cuda-23.8.0a230613/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1115 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 05:07:26.947678 dask-cuda-23.8.0a230613/dask_cuda/
--rw-r--r--   0 root         (0) root         (0)     1522 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/__init__.py
--rw-r--r--   0 root         (0) root         (0)      508 2023-06-13 05:07:26.947678 dask-cuda-23.8.0a230613/dask_cuda/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 05:07:26.939678 dask-cuda-23.8.0a230613/dask_cuda/benchmarks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/benchmarks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6393 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/benchmarks/common.py
--rw-r--r--   0 root         (0) root         (0)     8894 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/benchmarks/local_cudf_groupby.py
--rw-r--r--   0 root         (0) root         (0)    12437 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/benchmarks/local_cudf_merge.py
--rw-r--r--   0 root         (0) root         (0)     8598 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/benchmarks/local_cudf_shuffle.py
--rw-r--r--   0 root         (0) root         (0)    10752 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/benchmarks/local_cupy.py
--rw-r--r--   0 root         (0) root         (0)     6432 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/benchmarks/local_cupy_map_overlap.py
--rw-r--r--   0 root         (0) root         (0)    26888 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/benchmarks/utils.py
--rw-r--r--   0 root         (0) root         (0)    15870 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/cli.py
--rw-r--r--   0 root         (0) root         (0)     8589 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/cuda_worker.py
--rw-r--r--   0 root         (0) root         (0)    10038 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/device_host_file.py
--rw-r--r--   0 root         (0) root         (0)     6499 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/disk_io.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 05:07:26.939678 dask-cuda-23.8.0a230613/dask_cuda/explicit_comms/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/explicit_comms/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10478 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/explicit_comms/comms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 05:07:26.943678 dask-cuda-23.8.0a230613/dask_cuda/explicit_comms/dataframe/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/explicit_comms/dataframe/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20062 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/explicit_comms/dataframe/shuffle.py
--rw-r--r--   0 root         (0) root         (0)     3890 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/get_device_memory_objects.py
--rw-r--r--   0 root         (0) root         (0)     5231 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/initialize.py
--rw-r--r--   0 root         (0) root         (0)     1046 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/is_device_object.py
--rw-r--r--   0 root         (0) root         (0)     1457 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/is_spillable_object.py
--rw-r--r--   0 root         (0) root         (0)    17302 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/local_cuda_cluster.py
--rw-r--r--   0 root         (0) root         (0)     8108 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/proxify_device_objects.py
--rw-r--r--   0 root         (0) root         (0)    30850 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/proxify_host_file.py
--rw-r--r--   0 root         (0) root         (0)    29880 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/proxy_object.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 05:07:26.943678 dask-cuda-23.8.0a230613/dask_cuda/tests/
--rw-r--r--   0 root         (0) root         (0)     4910 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/tests/test_cudf_builtin_spilling.py
--rw-r--r--   0 root         (0) root         (0)    15517 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/tests/test_dask_cuda_worker.py
--rw-r--r--   0 root         (0) root         (0)     5882 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/tests/test_device_host_file.py
--rw-r--r--   0 root         (0) root         (0)     6381 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/tests/test_dgx.py
--rw-r--r--   0 root         (0) root         (0)    12036 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/tests/test_explicit_comms.py
--rw-r--r--   0 root         (0) root         (0)     1513 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/tests/test_gds.py
--rw-r--r--   0 root         (0) root         (0)     5235 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/tests/test_initialize.py
--rw-r--r--   0 root         (0) root         (0)    15675 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/tests/test_local_cuda_cluster.py
--rw-r--r--   0 root         (0) root         (0)    18492 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/tests/test_proxify_host_file.py
--rw-r--r--   0 root         (0) root         (0)    23464 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/tests/test_proxy.py
--rw-r--r--   0 root         (0) root         (0)     9452 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/tests/test_spill.py
--rw-r--r--   0 root         (0) root         (0)     8832 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     2399 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/tests/test_worker_spec.py
--rw-r--r--   0 root         (0) root         (0)    29398 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/utils.py
--rw-r--r--   0 root         (0) root         (0)     4356 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/dask_cuda/worker_spec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 05:07:26.939678 dask-cuda-23.8.0a230613/dask_cuda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1924 2023-06-13 05:07:26.000000 dask-cuda-23.8.0a230613/dask_cuda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1702 2023-06-13 05:07:26.000000 dask-cuda-23.8.0a230613/dask_cuda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 05:07:26.000000 dask-cuda-23.8.0a230613/dask_cuda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      136 2023-06-13 05:07:26.000000 dask-cuda-23.8.0a230613/dask_cuda.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      207 2023-06-13 05:07:26.000000 dask-cuda-23.8.0a230613/dask_cuda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-06-13 05:07:26.000000 dask-cuda-23.8.0a230613/dask_cuda.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 05:07:26.935677 dask-cuda-23.8.0a230613/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 05:07:26.943678 dask-cuda-23.8.0a230613/examples/ucx/
--rw-r--r--   0 root         (0) root         (0)     1262 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/examples/ucx/client_initialize.py
--rw-r--r--   0 root         (0) root         (0)     1983 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/examples/ucx/local_cuda_cluster.py
--rw-r--r--   0 root         (0) root         (0)     3251 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 05:07:26.943678 dask-cuda-23.8.0a230613/rtd/
--rw-r--r--   0 root         (0) root         (0)     6223 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/rtd/conf.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 05:07:26.947678 dask-cuda-23.8.0a230613/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      957 2023-06-13 05:07:18.000000 dask-cuda-23.8.0a230613/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 05:07:42.533974 dask-cuda-23.8.0a230614/
+-rw-r--r--   0 root         (0) root         (0)    11348 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1924 2023-06-14 05:07:42.533974 dask-cuda-23.8.0a230614/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1115 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 05:07:42.533974 dask-cuda-23.8.0a230614/dask_cuda/
+-rw-r--r--   0 root         (0) root         (0)     1498 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      508 2023-06-14 05:07:42.533974 dask-cuda-23.8.0a230614/dask_cuda/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 05:07:42.529974 dask-cuda-23.8.0a230614/dask_cuda/benchmarks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/benchmarks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6393 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/benchmarks/common.py
+-rw-r--r--   0 root         (0) root         (0)     8894 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/benchmarks/local_cudf_groupby.py
+-rw-r--r--   0 root         (0) root         (0)    12437 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/benchmarks/local_cudf_merge.py
+-rw-r--r--   0 root         (0) root         (0)     8598 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/benchmarks/local_cudf_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)    10752 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/benchmarks/local_cupy.py
+-rw-r--r--   0 root         (0) root         (0)     6432 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/benchmarks/local_cupy_map_overlap.py
+-rw-r--r--   0 root         (0) root         (0)    26888 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/benchmarks/utils.py
+-rw-r--r--   0 root         (0) root         (0)    15870 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/cli.py
+-rw-r--r--   0 root         (0) root         (0)     8589 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/cuda_worker.py
+-rw-r--r--   0 root         (0) root         (0)    10038 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/device_host_file.py
+-rw-r--r--   0 root         (0) root         (0)     6499 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/disk_io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 05:07:42.529974 dask-cuda-23.8.0a230614/dask_cuda/explicit_comms/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/explicit_comms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10478 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/explicit_comms/comms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 05:07:42.529974 dask-cuda-23.8.0a230614/dask_cuda/explicit_comms/dataframe/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/explicit_comms/dataframe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20056 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/explicit_comms/dataframe/shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     3890 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/get_device_memory_objects.py
+-rw-r--r--   0 root         (0) root         (0)     5231 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/initialize.py
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/is_device_object.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/is_spillable_object.py
+-rw-r--r--   0 root         (0) root         (0)    17302 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/local_cuda_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     8108 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/proxify_device_objects.py
+-rw-r--r--   0 root         (0) root         (0)    30850 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/proxify_host_file.py
+-rw-r--r--   0 root         (0) root         (0)    29880 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/proxy_object.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 05:07:42.533974 dask-cuda-23.8.0a230614/dask_cuda/tests/
+-rw-r--r--   0 root         (0) root         (0)     4910 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/tests/test_cudf_builtin_spilling.py
+-rw-r--r--   0 root         (0) root         (0)    15517 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/tests/test_dask_cuda_worker.py
+-rw-r--r--   0 root         (0) root         (0)     5882 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/tests/test_device_host_file.py
+-rw-r--r--   0 root         (0) root         (0)     6381 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/tests/test_dgx.py
+-rw-r--r--   0 root         (0) root         (0)    11150 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/tests/test_explicit_comms.py
+-rw-r--r--   0 root         (0) root         (0)     1513 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/tests/test_gds.py
+-rw-r--r--   0 root         (0) root         (0)     5235 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/tests/test_initialize.py
+-rw-r--r--   0 root         (0) root         (0)    15940 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/tests/test_local_cuda_cluster.py
+-rw-r--r--   0 root         (0) root         (0)    18492 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/tests/test_proxify_host_file.py
+-rw-r--r--   0 root         (0) root         (0)    23370 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/tests/test_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     9452 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/tests/test_spill.py
+-rw-r--r--   0 root         (0) root         (0)     8832 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2399 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/tests/test_worker_spec.py
+-rw-r--r--   0 root         (0) root         (0)    29398 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4356 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/dask_cuda/worker_spec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 05:07:42.525974 dask-cuda-23.8.0a230614/dask_cuda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1924 2023-06-14 05:07:42.000000 dask-cuda-23.8.0a230614/dask_cuda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1702 2023-06-14 05:07:42.000000 dask-cuda-23.8.0a230614/dask_cuda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 05:07:42.000000 dask-cuda-23.8.0a230614/dask_cuda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      136 2023-06-14 05:07:42.000000 dask-cuda-23.8.0a230614/dask_cuda.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      207 2023-06-14 05:07:42.000000 dask-cuda-23.8.0a230614/dask_cuda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-14 05:07:42.000000 dask-cuda-23.8.0a230614/dask_cuda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 05:07:42.521973 dask-cuda-23.8.0a230614/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 05:07:42.533974 dask-cuda-23.8.0a230614/examples/ucx/
+-rw-r--r--   0 root         (0) root         (0)     1262 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/examples/ucx/client_initialize.py
+-rw-r--r--   0 root         (0) root         (0)     1983 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/examples/ucx/local_cuda_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     3251 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 05:07:42.533974 dask-cuda-23.8.0a230614/rtd/
+-rw-r--r--   0 root         (0) root         (0)     6223 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/rtd/conf.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 05:07:42.533974 dask-cuda-23.8.0a230614/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      957 2023-06-14 05:07:34.000000 dask-cuda-23.8.0a230614/setup.py
```

### Comparing `dask-cuda-23.8.0a230613/LICENSE` & `dask-cuda-23.8.0a230614/LICENSE`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/PKG-INFO` & `dask-cuda-23.8.0a230614/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-cuda
-Version: 23.8.0a230613
+Version: 23.8.0a230614
 Summary: Utilities for Dask and CUDA interactions
 Author: NVIDIA Corporation
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rapidsai/dask-cuda
 Project-URL: Documentation, https://docs.rapids.ai/api/dask-cuda/stable/
 Project-URL: Source, https://github.com/rapidsai/dask-cuda
 Classifier: Intended Audience :: Developers
```

### Comparing `dask-cuda-23.8.0a230613/README.md` & `dask-cuda-23.8.0a230614/README.md`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/__init__.py` & `dask-cuda-23.8.0a230614/dask_cuda/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,32 +11,32 @@
 import dask.dataframe.multi
 import dask.bag.core
 
 from ._version import get_versions
 from .cuda_worker import CUDAWorker
 from .explicit_comms.dataframe.shuffle import (
     get_rearrange_by_column_wrapper,
-    get_default_shuffle_algorithm,
+    get_default_shuffle_method,
 )
 from .local_cuda_cluster import LocalCUDACluster
 from .proxify_device_objects import proxify_decorator, unproxify_decorator
 
 __version__ = get_versions()["version"]
 del get_versions
 
 
 # Monkey patching Dask to make use of explicit-comms when `DASK_EXPLICIT_COMMS=True`
 dask.dataframe.shuffle.rearrange_by_column = get_rearrange_by_column_wrapper(
     dask.dataframe.shuffle.rearrange_by_column
 )
-# We have to replace all modules that imports Dask's `get_default_shuffle_algorithm()`
+# We have to replace all modules that imports Dask's `get_default_shuffle_method()`
 # TODO: introduce a shuffle-algorithm dispatcher in Dask so we don't need this hack
-dask.dataframe.shuffle.get_default_shuffle_algorithm = get_default_shuffle_algorithm
-dask.dataframe.multi.get_default_shuffle_algorithm = get_default_shuffle_algorithm
-dask.bag.core.get_default_shuffle_algorithm = get_default_shuffle_algorithm
+dask.dataframe.shuffle.get_default_shuffle_method = get_default_shuffle_method
+dask.dataframe.multi.get_default_shuffle_method = get_default_shuffle_method
+dask.bag.core.get_default_shuffle_method = get_default_shuffle_method
 
 
 # Monkey patching Dask to make use of proxify and unproxify in compatibility mode
 dask.dataframe.shuffle.shuffle_group = proxify_decorator(
     dask.dataframe.shuffle.shuffle_group
 )
 dask.dataframe.core._concat = unproxify_decorator(dask.dataframe.core._concat)
```

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/benchmarks/common.py` & `dask-cuda-23.8.0a230614/dask_cuda/benchmarks/common.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/benchmarks/local_cudf_groupby.py` & `dask-cuda-23.8.0a230614/dask_cuda/benchmarks/local_cudf_groupby.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/benchmarks/local_cudf_merge.py` & `dask-cuda-23.8.0a230614/dask_cuda/benchmarks/local_cudf_merge.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/benchmarks/local_cudf_shuffle.py` & `dask-cuda-23.8.0a230614/dask_cuda/benchmarks/local_cudf_shuffle.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/benchmarks/local_cupy.py` & `dask-cuda-23.8.0a230614/dask_cuda/benchmarks/local_cupy.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/benchmarks/local_cupy_map_overlap.py` & `dask-cuda-23.8.0a230614/dask_cuda/benchmarks/local_cupy_map_overlap.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/benchmarks/utils.py` & `dask-cuda-23.8.0a230614/dask_cuda/benchmarks/utils.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/cli.py` & `dask-cuda-23.8.0a230614/dask_cuda/cli.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/cuda_worker.py` & `dask-cuda-23.8.0a230614/dask_cuda/cuda_worker.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/device_host_file.py` & `dask-cuda-23.8.0a230614/dask_cuda/device_host_file.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/disk_io.py` & `dask-cuda-23.8.0a230614/dask_cuda/disk_io.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/explicit_comms/comms.py` & `dask-cuda-23.8.0a230614/dask_cuda/explicit_comms/comms.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/explicit_comms/dataframe/shuffle.py` & `dask-cuda-23.8.0a230614/dask_cuda/explicit_comms/dataframe/shuffle.py`

 * *Files 1% similar despite different names*

```diff
@@ -581,17 +581,17 @@
                     col = [col]
                 return shuffle(kw["df"], col, kw["npartitions"], kw["ignore_index"])
         return func(*args, **kwargs)
 
     return wrapper
 
 
-def get_default_shuffle_algorithm() -> str:
+def get_default_shuffle_method() -> str:
     """Return the default shuffle algorithm used by Dask
 
     This changes the default shuffle algorithm from "p2p" to "tasks"
     when explicit comms is enabled.
     """
     ret = dask.config.get("dataframe.shuffle.algorithm", None)
     if ret is None and _use_explicit_comms():
         return "tasks"
-    return dask.utils.get_default_shuffle_algorithm()
+    return dask.utils.get_default_shuffle_method()
```

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/get_device_memory_objects.py` & `dask-cuda-23.8.0a230614/dask_cuda/get_device_memory_objects.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/initialize.py` & `dask-cuda-23.8.0a230614/dask_cuda/initialize.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/is_device_object.py` & `dask-cuda-23.8.0a230614/dask_cuda/is_device_object.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/is_spillable_object.py` & `dask-cuda-23.8.0a230614/dask_cuda/is_spillable_object.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/local_cuda_cluster.py` & `dask-cuda-23.8.0a230614/dask_cuda/local_cuda_cluster.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/proxify_device_objects.py` & `dask-cuda-23.8.0a230614/dask_cuda/proxify_device_objects.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/proxify_host_file.py` & `dask-cuda-23.8.0a230614/dask_cuda/proxify_host_file.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/proxy_object.py` & `dask-cuda-23.8.0a230614/dask_cuda/proxy_object.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/tests/test_cudf_builtin_spilling.py` & `dask-cuda-23.8.0a230614/dask_cuda/tests/test_cudf_builtin_spilling.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/tests/test_dask_cuda_worker.py` & `dask-cuda-23.8.0a230614/dask_cuda/tests/test_dask_cuda_worker.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/tests/test_device_host_file.py` & `dask-cuda-23.8.0a230614/dask_cuda/tests/test_device_host_file.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/tests/test_dgx.py` & `dask-cuda-23.8.0a230614/dask_cuda/tests/test_dgx.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/tests/test_explicit_comms.py` & `dask-cuda-23.8.0a230614/dask_cuda/tests/test_explicit_comms.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,37 +13,27 @@
 from dask.dataframe.utils import assert_eq
 from distributed import Client
 from distributed.deploy.local import LocalCluster
 
 import dask_cuda
 from dask_cuda.explicit_comms import comms
 from dask_cuda.explicit_comms.dataframe.shuffle import shuffle as explicit_comms_shuffle
-from dask_cuda.initialize import initialize
-from dask_cuda.utils import get_ucx_config
 
 mp = mp.get_context("spawn")  # type: ignore
 ucp = pytest.importorskip("ucp")
 
 # Notice, all of the following tests is executed in a new process such
 # that UCX options of the different tests doesn't conflict.
 
 
 async def my_rank(state, arg):
     return state["rank"] + arg
 
 
 def _test_local_cluster(protocol):
-    dask.config.update(
-        dask.config.global_config,
-        {
-            "distributed.comm.ucx": get_ucx_config(enable_tcp_over_ucx=True),
-        },
-        priority="new",
-    )
-
     with LocalCluster(
         protocol=protocol,
         dashboard_address=None,
         n_workers=4,
         threads_per_worker=1,
         processes=True,
     ) as cluster:
@@ -102,23 +92,14 @@
     else:
         return True
 
 
 def _test_dataframe_shuffle(backend, protocol, n_workers):
     if backend == "cudf":
         cudf = pytest.importorskip("cudf")
-        initialize(enable_tcp_over_ucx=True)
-    else:
-        dask.config.update(
-            dask.config.global_config,
-            {
-                "distributed.comm.ucx": get_ucx_config(enable_tcp_over_ucx=True),
-            },
-            priority="new",
-        )
 
     with LocalCluster(
         protocol=protocol,
         dashboard_address=None,
         n_workers=n_workers,
         threads_per_worker=1,
         processes=True,
@@ -216,25 +197,14 @@
         check_shuffle()
 
 
 def _test_dataframe_shuffle_merge(backend, protocol, n_workers):
     if backend == "cudf":
         cudf = pytest.importorskip("cudf")
 
-        initialize(enable_tcp_over_ucx=True)
-    else:
-
-        dask.config.update(
-            dask.config.global_config,
-            {
-                "distributed.comm.ucx": get_ucx_config(enable_tcp_over_ucx=True),
-            },
-            priority="new",
-        )
-
     with LocalCluster(
         protocol=protocol,
         dashboard_address=None,
         n_workers=n_workers,
         threads_per_worker=1,
         processes=True,
     ) as cluster:
@@ -283,15 +253,14 @@
     with dask_cuda.LocalCUDACluster(
         protocol=protocol,
         dashboard_address=None,
         n_workers=1,
         threads_per_worker=1,
         jit_unspill=True,
         device_memory_limit="1B",
-        enable_tcp_over_ucx=True if protocol == "ucx" else False,
     ) as cluster:
         with Client(cluster):
             np.random.seed(42)
             df = cudf.DataFrame.from_pandas(
                 pd.DataFrame({"key": np.random.random(100)})
             )
             ddf = dd.from_pandas(df.copy(), npartitions=4)
```

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/tests/test_gds.py` & `dask-cuda-23.8.0a230614/dask_cuda/tests/test_gds.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/tests/test_initialize.py` & `dask-cuda-23.8.0a230614/dask_cuda/tests/test_initialize.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/tests/test_local_cuda_cluster.py` & `dask-cuda-23.8.0a230614/dask_cuda/tests/test_local_cuda_cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,22 +83,33 @@
                     0,
                     3,
                     6,
                     8,
                 }
 
 
-@pytest.mark.parametrize("protocol", ["ucx", None])
 @gen_test(timeout=20)
-async def test_ucx_protocol(protocol):
+async def test_ucx_protocol():
+    pytest.importorskip("ucp")
+
+    async with LocalCUDACluster(
+        protocol="ucx", asynchronous=True, data=dict
+    ) as cluster:
+        assert all(
+            ws.address.startswith("ucx://") for ws in cluster.scheduler.workers.values()
+        )
+
+
+@gen_test(timeout=20)
+async def test_explicit_ucx_with_protocol_none():
     pytest.importorskip("ucp")
 
     initialize(enable_tcp_over_ucx=True)
     async with LocalCUDACluster(
-        protocol=protocol, enable_tcp_over_ucx=True, asynchronous=True, data=dict
+        protocol=None, enable_tcp_over_ucx=True, asynchronous=True, data=dict
     ) as cluster:
         assert all(
             ws.address.startswith("ucx://") for ws in cluster.scheduler.workers.values()
         )
 
 
 @pytest.mark.filterwarnings("ignore:Exception ignored in")
```

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/tests/test_proxify_host_file.py` & `dask-cuda-23.8.0a230614/dask_cuda/tests/test_proxify_host_file.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/tests/test_proxy.py` & `dask-cuda-23.8.0a230614/dask_cuda/tests/test_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -418,15 +418,14 @@
                 assert serializers_used == send_serializers[0]
         else:
             assert serializers_used == "dask"
 
     async with dask_cuda.LocalCUDACluster(
         n_workers=1,
         protocol=protocol,
-        enable_tcp_over_ucx=protocol == "ucx",
         asynchronous=True,
     ) as cluster:
         async with Client(cluster, asynchronous=True) as client:
             df = cudf.DataFrame({"a": range(10)})
             df = proxy_object.asproxy(
                 df, serializers=send_serializers, subclass=_PxyObjTest
             )
@@ -458,15 +457,14 @@
             assert serializer_used == "disk"
         else:
             assert serializer_used == "dask"
 
     async with dask_cuda.LocalCUDACluster(
         n_workers=1,
         protocol=protocol,
-        enable_tcp_over_ucx=protocol == "ucx",
         asynchronous=True,
     ) as cluster:
         async with Client(cluster, asynchronous=True) as client:
             df = cudf.DataFrame({"a": range(10)})
             df = proxy_object.asproxy(df, serializers=("disk",), subclass=_PxyObjTest)
             df._pxy_get().assert_on_deserializing = False
             df = await client.scatter(df)
```

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/tests/test_spill.py` & `dask-cuda-23.8.0a230614/dask_cuda/tests/test_spill.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/tests/test_utils.py` & `dask-cuda-23.8.0a230614/dask_cuda/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/tests/test_worker_spec.py` & `dask-cuda-23.8.0a230614/dask_cuda/tests/test_worker_spec.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/utils.py` & `dask-cuda-23.8.0a230614/dask_cuda/utils.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/dask_cuda/worker_spec.py` & `dask-cuda-23.8.0a230614/dask_cuda/worker_spec.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/dask_cuda.egg-info/PKG-INFO` & `dask-cuda-23.8.0a230614/dask_cuda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-cuda
-Version: 23.8.0a230613
+Version: 23.8.0a230614
 Summary: Utilities for Dask and CUDA interactions
 Author: NVIDIA Corporation
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rapidsai/dask-cuda
 Project-URL: Documentation, https://docs.rapids.ai/api/dask-cuda/stable/
 Project-URL: Source, https://github.com/rapidsai/dask-cuda
 Classifier: Intended Audience :: Developers
```

### Comparing `dask-cuda-23.8.0a230613/dask_cuda.egg-info/SOURCES.txt` & `dask-cuda-23.8.0a230614/dask_cuda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/examples/ucx/client_initialize.py` & `dask-cuda-23.8.0a230614/examples/ucx/client_initialize.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/examples/ucx/local_cuda_cluster.py` & `dask-cuda-23.8.0a230614/examples/ucx/local_cuda_cluster.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/pyproject.toml` & `dask-cuda-23.8.0a230614/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/rtd/conf.py` & `dask-cuda-23.8.0a230614/rtd/conf.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.8.0a230613/setup.py` & `dask-cuda-23.8.0a230614/setup.py`

 * *Files identical despite different names*

