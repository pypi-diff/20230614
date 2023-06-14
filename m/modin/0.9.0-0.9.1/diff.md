# Comparing `tmp/modin-0.9.0.tar.gz` & `tmp/modin-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/modin-0.9.0.tar", last modified: Thu Mar  4 23:03:14 2021, max compression
+gzip compressed data, was "dist/modin-0.9.1.tar", last modified: Tue Mar 16 01:55:39 2021, max compression
```

## Comparing `modin-0.9.0.tar` & `modin-0.9.1.tar`

### file list

```diff
@@ -1,526 +1,314 @@
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    10890 2021-03-04 23:03:14.000000 modin-0.9.0/PKG-INFO
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     3349 2021-03-04 23:02:43.000000 modin-0.9.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      683 2021-03-04 23:02:43.000000 modin-0.9.0/environment-dev.yml
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/docker/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      103 2021-03-04 23:02:43.000000 modin-0.9.0/docker/Dockerfile
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    11357 2021-03-04 23:02:43.000000 modin-0.9.0/LICENSE
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/stress_tests/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1688 2021-03-04 23:02:43.000000 modin-0.9.0/stress_tests/run_stress_tests.sh
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/stress_tests/kaggle/
--rwxr-xr-x   0 DevinPetersohn   (501) staff       (20)      566 2021-03-04 23:02:43.000000 modin-0.9.0/stress_tests/kaggle/kaggle8.py
--rwxr-xr-x   0 DevinPetersohn   (501) staff       (20)    16176 2021-03-04 23:02:43.000000 modin-0.9.0/stress_tests/kaggle/kaggle18.py
--rwxr-xr-x   0 DevinPetersohn   (501) staff       (20)    10182 2021-03-04 23:02:43.000000 modin-0.9.0/stress_tests/kaggle/kaggle19.py
--rwxr-xr-x   0 DevinPetersohn   (501) staff       (20)     3786 2021-03-04 23:02:43.000000 modin-0.9.0/stress_tests/kaggle/kaggle9.py
--rwxr-xr-x   0 DevinPetersohn   (501) staff       (20)     1935 2021-03-04 23:02:43.000000 modin-0.9.0/stress_tests/kaggle/kaggle22.py
--rwxr-xr-x   0 DevinPetersohn   (501) staff       (20)     6403 2021-03-04 23:02:43.000000 modin-0.9.0/stress_tests/kaggle/kaggle6.py
--rwxr-xr-x   0 DevinPetersohn   (501) staff       (20)    16033 2021-03-04 23:02:43.000000 modin-0.9.0/stress_tests/kaggle/kaggle12.py
--rwxr-xr-x   0 DevinPetersohn   (501) staff       (20)    16285 2021-03-04 23:02:43.000000 modin-0.9.0/stress_tests/kaggle/kaggle7.py
--rwxr-xr-x   0 DevinPetersohn   (501) staff       (20)     1416 2021-03-04 23:02:43.000000 modin-0.9.0/stress_tests/kaggle/kaggle13.py
--rwxr-xr-x   0 DevinPetersohn   (501) staff       (20)     9077 2021-03-04 23:02:43.000000 modin-0.9.0/stress_tests/kaggle/kaggle3.py
--rwxr-xr-x   0 DevinPetersohn   (501) staff       (20)      364 2021-03-04 23:02:43.000000 modin-0.9.0/stress_tests/kaggle/kaggle17.py
--rwxr-xr-x   0 DevinPetersohn   (501) staff       (20)    12532 2021-03-04 23:02:43.000000 modin-0.9.0/stress_tests/kaggle/kaggle4.py
--rwxr-xr-x   0 DevinPetersohn   (501) staff       (20)     8897 2021-03-04 23:02:43.000000 modin-0.9.0/stress_tests/kaggle/kaggle10.py
--rwxr-xr-x   0 DevinPetersohn   (501) staff       (20)     6764 2021-03-04 23:02:43.000000 modin-0.9.0/stress_tests/kaggle/kaggle20.py
--rwxr-xr-x   0 DevinPetersohn   (501) staff       (20)    18153 2021-03-04 23:02:43.000000 modin-0.9.0/stress_tests/kaggle/kaggle14.py
--rwxr-xr-x   0 DevinPetersohn   (501) staff       (20)     9580 2021-03-04 23:02:43.000000 modin-0.9.0/stress_tests/kaggle/kaggle5.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    31341 2021-03-04 23:02:43.000000 modin-0.9.0/stress_tests/test_kaggle_ipynb.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/ci/
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/ci/teamcity/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     2698 2021-03-04 23:02:43.000000 modin-0.9.0/ci/teamcity/comment_on_pr.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1007 2021-03-04 23:02:43.000000 modin-0.9.0/ci/teamcity/build-docker.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1259 2021-03-04 23:02:43.000000 modin-0.9.0/ci/teamcity/Dockerfile.teamcity-ci
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/ci/benchmarks/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     3082 2021-03-04 23:02:43.000000 modin-0.9.0/ci/benchmarks/run_benchmark.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     8651 2021-03-04 23:02:43.000000 modin-0.9.0/ci/benchmarks/test_benchmarks.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1990 2021-03-04 23:02:43.000000 modin-0.9.0/ci/benchmarks/df_op_benchmark.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      900 2021-03-04 23:02:43.000000 modin-0.9.0/ci/benchmarks/generate_data.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)       12 2021-03-04 23:02:43.000000 modin-0.9.0/ci/benchmarks/.gitignore
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      426 2021-03-04 23:02:43.000000 modin-0.9.0/ci/benchmarks/utils.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1224 2021-03-04 23:02:43.000000 modin-0.9.0/ci/benchmarks/groupby_benchmark.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     2292 2021-03-04 23:02:43.000000 modin-0.9.0/ci/benchmarks/join_merge_benchmark.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1789 2021-03-04 23:02:43.000000 modin-0.9.0/ci/benchmarks/arithmetic_benchmark.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      878 2021-03-04 23:02:43.000000 modin-0.9.0/ci/benchmarks/io_benchmark.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/ci/benchmarks/pandas/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1894 2021-03-04 23:02:43.000000 modin-0.9.0/ci/benchmarks/pandas/df_op_benchmark.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     3123 2021-03-04 23:02:43.000000 modin-0.9.0/ci/benchmarks/pandas/run_pandas_benchmark.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      426 2021-03-04 23:02:43.000000 modin-0.9.0/ci/benchmarks/pandas/utils.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      968 2021-03-04 23:02:43.000000 modin-0.9.0/ci/benchmarks/pandas/groupby_benchmark.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1873 2021-03-04 23:02:43.000000 modin-0.9.0/ci/benchmarks/pandas/join_merge_benchmark.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1631 2021-03-04 23:02:43.000000 modin-0.9.0/ci/benchmarks/pandas/arithmetic_benchmark.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      774 2021-03-04 23:02:43.000000 modin-0.9.0/ci/benchmarks/pandas/io_benchmark.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/ci/jenkins/
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/ci/jenkins/performance-tests/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      352 2021-03-04 23:02:43.000000 modin-0.9.0/ci/jenkins/performance-tests/run_perf_ci.sh
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      332 2021-03-04 23:02:43.000000 modin-0.9.0/ci/jenkins/performance-tests/Dockerfile
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      691 2021-03-04 23:02:43.000000 modin-0.9.0/ci/jenkins/performance-tests/run_perf_test.sh
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)       45 2021-03-04 23:02:43.000000 modin-0.9.0/ci/jenkins/README.md
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/ci/jenkins/build-tests/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      899 2021-03-04 23:02:43.000000 modin-0.9.0/ci/jenkins/build-tests/run_test.sh
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      332 2021-03-04 23:02:43.000000 modin-0.9.0/ci/jenkins/build-tests/run_ci.sh
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      237 2021-03-04 23:02:43.000000 modin-0.9.0/ci/jenkins/build-tests/Dockerfile
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/asv_bench/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     6719 2021-03-04 23:02:43.000000 modin-0.9.0/asv_bench/asv.conf.json
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/asv_bench/benchmarks/
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/asv_bench/benchmarks/io/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/asv_bench/benchmarks/io/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     4848 2021-03-04 23:02:43.000000 modin-0.9.0/asv_bench/benchmarks/io/csv.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      806 2021-03-04 23:02:43.000000 modin-0.9.0/asv_bench/benchmarks/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     6877 2021-03-04 23:02:43.000000 modin-0.9.0/asv_bench/benchmarks/utils.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/asv_bench/benchmarks/scalability/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     2006 2021-03-04 23:02:43.000000 modin-0.9.0/asv_bench/benchmarks/scalability/scalability_benchmarks.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/asv_bench/benchmarks/scalability/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    17519 2021-03-04 23:02:43.000000 modin-0.9.0/asv_bench/benchmarks/benchmarks.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      523 2021-03-04 23:02:43.000000 modin-0.9.0/CODEOWNERS
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      137 2021-03-04 23:02:43.000000 modin-0.9.0/MANIFEST.in
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/requirements/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      358 2021-03-04 23:02:43.000000 modin-0.9.0/requirements/env_omnisci.yml
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/docs/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     5108 2021-03-04 23:02:43.000000 modin-0.9.0/docs/index.rst
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/docs/developer/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    12247 2021-03-04 23:02:43.000000 modin-0.9.0/docs/developer/architecture.rst
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/docs/developer/pandas/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     3045 2021-03-04 23:02:43.000000 modin-0.9.0/docs/developer/pandas/partition_api.rst
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     3502 2021-03-04 23:02:43.000000 modin-0.9.0/docs/modin_xgboost.rst
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/docs/comparisons/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)       58 2021-03-04 23:02:43.000000 modin-0.9.0/docs/comparisons/index.rst
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     3111 2021-03-04 23:02:43.000000 modin-0.9.0/docs/comparisons/pandas.rst
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     4732 2021-03-04 23:02:43.000000 modin-0.9.0/docs/comparisons/dask.rst
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)       70 2021-03-04 23:02:43.000000 modin-0.9.0/docs/comparisons/spark.rst
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     9212 2021-03-04 23:02:43.000000 modin-0.9.0/docs/contributing.rst
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/docs/UsingPandasonRay/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      314 2021-03-04 23:02:43.000000 modin-0.9.0/docs/UsingPandasonRay/index.rst
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     2747 2021-03-04 23:02:43.000000 modin-0.9.0/docs/modin_vs_dask.md
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     3142 2021-03-04 23:02:43.000000 modin-0.9.0/docs/conf.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      685 2021-03-04 23:02:43.000000 modin-0.9.0/docs/contact.rst
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/docs/UsingPandasonDask/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      306 2021-03-04 23:02:43.000000 modin-0.9.0/docs/UsingPandasonDask/index.rst
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/docs/img/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    65421 2021-03-04 23:02:43.000000 modin-0.9.0/docs/img/modin_architecture_diagram.png
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     9648 2021-03-04 23:02:43.000000 modin-0.9.0/docs/img/powered_by_ray_big.svg
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)   218612 2021-03-04 23:02:43.000000 modin-0.9.0/docs/img/modin_cluster.png
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     9636 2021-03-04 23:02:43.000000 modin-0.9.0/docs/img/powered_by_ray_small.svg
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    70298 2021-03-04 23:02:43.000000 modin-0.9.0/docs/img/convert_to_pandas.png
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    18306 2021-03-04 23:02:43.000000 modin-0.9.0/docs/img/MODIN_ver2_hrz.png
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    62652 2021-03-04 23:02:43.000000 modin-0.9.0/docs/img/Modin_Pandas_Import.gif
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    44451 2021-03-04 23:02:43.000000 modin-0.9.0/docs/img/block_partitions_diagram.png
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)   147815 2021-03-04 23:02:43.000000 modin-0.9.0/docs/img/10000_meter.png
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)   790663 2021-03-04 23:02:43.000000 modin-0.9.0/docs/img/query_planner.png
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)   737376 2021-03-04 23:02:43.000000 modin-0.9.0/docs/img/component_view.png
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    23211 2021-03-04 23:02:43.000000 modin-0.9.0/docs/img/modin_multicore.png
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    22851 2021-03-04 23:02:43.000000 modin-0.9.0/docs/img/pandas_multicore.png
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    37478 2021-03-04 23:02:43.000000 modin-0.9.0/docs/img/read_csv_benchmark.png
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    31355 2021-03-04 23:02:43.000000 modin-0.9.0/docs/img/MODIN_ver2.png
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)   173247 2021-03-04 23:02:43.000000 modin-0.9.0/docs/img/modin_architecture.png
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/docs/examples/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      334 2021-03-04 23:02:43.000000 modin-0.9.0/docs/examples/index.rst
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     3928 2021-03-04 23:02:43.000000 modin-0.9.0/docs/installation.rst
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     5831 2021-03-04 23:02:43.000000 modin-0.9.0/docs/using_modin.rst
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     3138 2021-03-04 23:02:43.000000 modin-0.9.0/docs/troubleshooting.rst
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      226 2021-03-04 23:02:43.000000 modin-0.9.0/docs/requirements-doc.txt
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1403 2021-03-04 23:02:43.000000 modin-0.9.0/docs/release-procedure.md
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/docs/supported_apis/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     2210 2021-03-04 23:02:43.000000 modin-0.9.0/docs/supported_apis/index.rst
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     7425 2021-03-04 23:02:43.000000 modin-0.9.0/docs/supported_apis/utilities_supported.rst
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    88061 2021-03-04 23:02:43.000000 modin-0.9.0/docs/supported_apis/dataframe_supported.rst
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     5927 2021-03-04 23:02:43.000000 modin-0.9.0/docs/supported_apis/io_supported.rst
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    57576 2021-03-04 23:02:43.000000 modin-0.9.0/docs/supported_apis/series_supported.rst
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     2378 2021-03-04 23:02:43.000000 modin-0.9.0/docs/out_of_core.rst
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/docs/UsingPyarrowonRay/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)       48 2021-03-04 23:02:43.000000 modin-0.9.0/docs/UsingPyarrowonRay/index.rst
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/docs/UsingSQLonRay/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1353 2021-03-04 23:02:43.000000 modin-0.9.0/docs/UsingSQLonRay/index.rst
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)       49 2021-03-04 23:02:43.000000 modin-0.9.0/NOTICE
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     8917 2021-03-04 23:02:43.000000 modin-0.9.0/README.md
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1980 2021-03-04 23:02:43.000000 modin-0.9.0/setup.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      422 2021-03-04 23:02:43.000000 modin-0.9.0/requirements-dev.txt
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     2650 2021-03-04 23:02:43.000000 modin-0.9.0/.gitignore
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/LICENSE_HEADER
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/examples/
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/examples/cluster/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     2600 2021-03-04 23:02:43.000000 modin-0.9.0/examples/cluster/taxi-runner.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1569 2021-03-04 23:02:43.000000 modin-0.9.0/examples/cluster/experimental_cloud.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1845 2021-03-04 23:02:43.000000 modin-0.9.0/examples/cluster/mortgage-runner.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     5711 2021-03-04 23:02:43.000000 modin-0.9.0/examples/cluster/aws_example.yaml
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     2011 2021-03-04 23:02:43.000000 modin-0.9.0/examples/cluster/h2o-runner.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/examples/tutorial/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)       77 2021-03-04 23:02:43.000000 modin-0.9.0/examples/tutorial/requirements.txt
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      123 2021-03-04 23:02:43.000000 modin-0.9.0/examples/tutorial/Dockerfile
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)       66 2021-03-04 23:02:43.000000 modin-0.9.0/examples/tutorial/README.md
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/examples/tutorial/tutorial_notebooks/
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/examples/tutorial/tutorial_notebooks/cluster/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     3822 2021-03-04 23:02:43.000000 modin-0.9.0/examples/tutorial/tutorial_notebooks/cluster/exercise_5.ipynb
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     3861 2021-03-04 23:02:43.000000 modin-0.9.0/examples/tutorial/tutorial_notebooks/cluster/exercise_4.ipynb
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     7119 2021-03-04 23:02:43.000000 modin-0.9.0/examples/tutorial/tutorial_notebooks/cluster/modin-cluster.yaml
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/examples/tutorial/tutorial_notebooks/introduction/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     9932 2021-03-04 23:02:43.000000 modin-0.9.0/examples/tutorial/tutorial_notebooks/introduction/exercise_3.ipynb
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     6632 2021-03-04 23:02:43.000000 modin-0.9.0/examples/tutorial/tutorial_notebooks/introduction/exercise_1.ipynb
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    12898 2021-03-04 23:02:43.000000 modin-0.9.0/examples/tutorial/tutorial_notebooks/introduction/exercise_2.ipynb
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/examples/tutorial/tutorial_notebooks/img/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)   218612 2021-03-04 23:02:43.000000 modin-0.9.0/examples/tutorial/tutorial_notebooks/img/modin_cluster.png
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    70298 2021-03-04 23:02:43.000000 modin-0.9.0/examples/tutorial/tutorial_notebooks/img/convert_to_pandas.png
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    18306 2021-03-04 23:02:43.000000 modin-0.9.0/examples/tutorial/tutorial_notebooks/img/MODIN_ver2_hrz.png
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    12948 2021-03-04 23:02:43.000000 modin-0.9.0/examples/tutorial/tutorial_notebooks/img/read_csv_perf.png
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    23211 2021-03-04 23:02:43.000000 modin-0.9.0/examples/tutorial/tutorial_notebooks/img/modin_multicore.png
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    22851 2021-03-04 23:02:43.000000 modin-0.9.0/examples/tutorial/tutorial_notebooks/img/pandas_multicore.png
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    51080 2021-03-04 23:02:43.000000 modin-0.9.0/examples/tutorial/tutorial_notebooks/img/modin_cluster_perf.png
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/examples/docker/
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/examples/docker/census-on-omnisci/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1385 2021-03-04 23:02:43.000000 modin-0.9.0/examples/docker/census-on-omnisci/build-docker-image.sh
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     2433 2021-03-04 23:02:43.000000 modin-0.9.0/examples/docker/census-on-omnisci/census-omnisci.dockerfile
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     5426 2021-03-04 23:02:43.000000 modin-0.9.0/examples/docker/census-on-omnisci/census-omnisci.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/examples/docker/taxi-on-omnisci/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     2027 2021-03-04 23:02:43.000000 modin-0.9.0/examples/docker/taxi-on-omnisci/nyc-taxi-omnisci.dockerfile
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1307 2021-03-04 23:02:43.000000 modin-0.9.0/examples/docker/taxi-on-omnisci/build-docker-image.sh
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     4783 2021-03-04 23:02:43.000000 modin-0.9.0/examples/docker/taxi-on-omnisci/nyc-taxi-omnisci.py
--rwxr-xr-x   0 DevinPetersohn   (501) staff       (20)      992 2021-03-04 23:02:43.000000 modin-0.9.0/examples/docker/build.sh
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     2217 2021-03-04 23:02:43.000000 modin-0.9.0/examples/docker/nyc-taxi.dockerfile
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     3057 2021-03-04 23:02:43.000000 modin-0.9.0/examples/docker/nyc-taxi.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/examples/docker/plasticc-on-omnisci/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1325 2021-03-04 23:02:43.000000 modin-0.9.0/examples/docker/plasticc-on-omnisci/build-docker-image.sh
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     7630 2021-03-04 23:02:43.000000 modin-0.9.0/examples/docker/plasticc-on-omnisci/plasticc-omnisci.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     2741 2021-03-04 23:02:43.000000 modin-0.9.0/examples/docker/plasticc-on-omnisci/plasticc-omnisci.dockerfile
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/examples/spreadsheet/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)       76 2021-03-04 23:02:43.000000 modin-0.9.0/examples/spreadsheet/requirements.txt
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     9786 2021-03-04 23:02:43.000000 modin-0.9.0/examples/spreadsheet/tutorial.ipynb
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    48285 2021-03-04 23:02:43.000000 modin-0.9.0/examples/modin-scikit-learn-example.ipynb
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/examples/data/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    41084 2021-03-04 23:02:43.000000 modin-0.9.0/examples/data/boston_housing.csv
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/examples/jupyter/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    32403 2021-03-04 23:02:43.000000 modin-0.9.0/examples/jupyter/NYC_Taxi.ipynb
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     9936 2021-03-04 23:02:43.000000 modin-0.9.0/examples/jupyter/NYC_Taxi_cloud.ipynb
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/experimental/
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/experimental/xgboost/
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/experimental/xgboost/test/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/xgboost/test/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1168 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/xgboost/test/test_default.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      881 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/xgboost/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1968 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/xgboost/utils.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    12739 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/xgboost/xgboost_ray.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     4185 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/xgboost/xgboost.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/experimental/backends/
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/experimental/backends/omnisci/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    21484 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/backends/omnisci/query_compiler.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/backends/omnisci/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/backends/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/__init__.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/experimental/sklearn/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/sklearn/__init__.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/experimental/sklearn/model_selection/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      862 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/sklearn/model_selection/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      975 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/sklearn/model_selection/train_test_split.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/experimental/engines/
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/experimental/engines/pandas_on_ray/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     8286 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/engines/pandas_on_ray/io_exp.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/engines/pandas_on_ray/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     6290 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/engines/pandas_on_ray/sql.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/experimental/engines/omnisci_on_ray/
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/experimental/engines/omnisci_on_ray/test/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/engines/omnisci_on_ray/test/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    53694 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/engines/omnisci_on_ray/test/test_dataframe.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     9725 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/engines/omnisci_on_ray/io.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/engines/omnisci_on_ray/__init__.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/experimental/engines/omnisci_on_ray/frame/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     2055 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/engines/omnisci_on_ray/frame/partition.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    10175 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/engines/omnisci_on_ray/frame/df_algebra.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/engines/omnisci_on_ray/frame/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     3989 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/engines/omnisci_on_ray/frame/calcite_algebra.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    20326 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/engines/omnisci_on_ray/frame/calcite_builder.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     6525 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/engines/omnisci_on_ray/frame/calcite_serializer.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     7719 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/engines/omnisci_on_ray/frame/partition_manager.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1877 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/engines/omnisci_on_ray/frame/axis_partition.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     4268 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/engines/omnisci_on_ray/frame/omnisci_worker.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    54138 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/engines/omnisci_on_ray/frame/data.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     9935 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/engines/omnisci_on_ray/frame/expr.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/engines/__init__.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/experimental/engines/pyarrow_on_ray/
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/experimental/engines/pyarrow_on_ray/series/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/engines/pyarrow_on_ray/series/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1803 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/engines/pyarrow_on_ray/io.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/engines/pyarrow_on_ray/__init__.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/experimental/engines/pyarrow_on_ray/frame/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1936 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/engines/pyarrow_on_ray/frame/partition.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/engines/pyarrow_on_ray/frame/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1384 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/engines/pyarrow_on_ray/frame/partition_manager.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     7740 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/engines/pyarrow_on_ray/frame/axis_partition.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     2246 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/engines/pyarrow_on_ray/frame/data.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/experimental/cloud/
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/experimental/cloud/tracing/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/cloud/tracing/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     4052 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/cloud/tracing/tracing_connection.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     7175 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/cloud/tracing/parse_rpyc_trace.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/experimental/cloud/test/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/cloud/test/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     4497 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/cloud/test/test_cloud.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     6969 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/cloud/ray-autoscaler.yml
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1258 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/cloud/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     9276 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/cloud/rayscale.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     7556 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/cloud/connection.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1648 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/cloud/omnisci.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     6712 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/cloud/meta_magic.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    11522 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/cloud/cluster.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    27221 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/cloud/rpyc_proxy.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     3801 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/cloud/local_cluster.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     2341 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/cloud/base.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/experimental/pandas/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     6697 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/pandas/io_exp.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/experimental/pandas/test/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/pandas/test/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     4416 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/pandas/test/test_io_exp.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1316 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/pandas/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     6867 2021-03-04 23:02:43.000000 modin-0.9.0/modin/experimental/pandas/numpy_wrap.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    12745 2021-03-04 23:02:43.000000 modin-0.9.0/modin/conftest.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/test/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1226 2021-03-04 23:02:43.000000 modin-0.9.0/modin/test/test_envvar_catcher.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     2058 2021-03-04 23:02:43.000000 modin-0.9.0/modin/test/test_backends_api.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     2060 2021-03-04 23:02:43.000000 modin-0.9.0/modin/test/test_envvar_npartitions.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/test/backends/
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/test/backends/base/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     2925 2021-03-04 23:02:43.000000 modin-0.9.0/modin/test/backends/base/test_internals.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/test/backends/pandas/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1912 2021-03-04 23:02:43.000000 modin-0.9.0/modin/test/backends/pandas/test_internals.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/test/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     4037 2021-03-04 23:02:43.000000 modin-0.9.0/modin/test/test_partition_api.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     2291 2021-03-04 23:02:43.000000 modin-0.9.0/modin/test/test_headers.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      497 2021-03-04 23:03:14.000000 modin-0.9.0/modin/_version.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/spreadsheet/
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/spreadsheet/test/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/spreadsheet/test/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1986 2021-03-04 23:02:43.000000 modin-0.9.0/modin/spreadsheet/test/test_general.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1073 2021-03-04 23:02:43.000000 modin-0.9.0/modin/spreadsheet/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     8448 2021-03-04 23:02:43.000000 modin-0.9.0/modin/spreadsheet/general.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/distributed/
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/distributed/dataframe/
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/distributed/dataframe/pandas/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     6760 2021-03-04 23:02:43.000000 modin-0.9.0/modin/distributed/dataframe/pandas/partitions.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      894 2021-03-04 23:02:43.000000 modin-0.9.0/modin/distributed/dataframe/pandas/__init__.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/config/
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/config/test/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     2052 2021-03-04 23:02:43.000000 modin-0.9.0/modin/config/test/test_envvars.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/config/test/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     2936 2021-03-04 23:02:43.000000 modin-0.9.0/modin/config/test/test_parameter.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     7293 2021-03-04 23:02:43.000000 modin-0.9.0/modin/config/envvars.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      870 2021-03-04 23:02:43.000000 modin-0.9.0/modin/config/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     4942 2021-03-04 23:02:43.000000 modin-0.9.0/modin/config/pubsub.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1172 2021-03-04 23:02:43.000000 modin-0.9.0/modin/config/__main__.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/data_management/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/data_management/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     4416 2021-03-04 23:02:43.000000 modin-0.9.0/modin/data_management/utils.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/data_management/factories/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     5760 2021-03-04 23:02:43.000000 modin-0.9.0/modin/data_management/factories/dispatcher.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/data_management/factories/test/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/data_management/factories/test/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     3027 2021-03-04 23:02:43.000000 modin-0.9.0/modin/data_management/factories/test/test_dispatcher.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1193 2021-03-04 23:02:43.000000 modin-0.9.0/modin/data_management/factories/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    10030 2021-03-04 23:02:43.000000 modin-0.9.0/modin/data_management/factories/factories.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/data_management/functions/
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/data_management/functions/default_methods/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1073 2021-03-04 23:02:43.000000 modin-0.9.0/modin/data_management/functions/default_methods/dataframe_default.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      965 2021-03-04 23:02:43.000000 modin-0.9.0/modin/data_management/functions/default_methods/series_default.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1344 2021-03-04 23:02:43.000000 modin-0.9.0/modin/data_management/functions/default_methods/rolling_default.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      947 2021-03-04 23:02:43.000000 modin-0.9.0/modin/data_management/functions/default_methods/str_default.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1484 2021-03-04 23:02:43.000000 modin-0.9.0/modin/data_management/functions/default_methods/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      947 2021-03-04 23:02:43.000000 modin-0.9.0/modin/data_management/functions/default_methods/cat_default.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      951 2021-03-04 23:02:43.000000 modin-0.9.0/modin/data_management/functions/default_methods/datetime_default.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     3346 2021-03-04 23:02:43.000000 modin-0.9.0/modin/data_management/functions/default_methods/default.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1771 2021-03-04 23:02:43.000000 modin-0.9.0/modin/data_management/functions/default_methods/binary_default.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1333 2021-03-04 23:02:43.000000 modin-0.9.0/modin/data_management/functions/default_methods/any_default.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1528 2021-03-04 23:02:43.000000 modin-0.9.0/modin/data_management/functions/default_methods/resample_default.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     5268 2021-03-04 23:02:43.000000 modin-0.9.0/modin/data_management/functions/default_methods/groupby_default.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     9871 2021-03-04 23:02:43.000000 modin-0.9.0/modin/data_management/functions/groupby_function.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1209 2021-03-04 23:02:43.000000 modin-0.9.0/modin/data_management/functions/mapfunction.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1291 2021-03-04 23:02:43.000000 modin-0.9.0/modin/data_management/functions/foldfunction.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1733 2021-03-04 23:02:43.000000 modin-0.9.0/modin/data_management/functions/mapreducefunction.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1313 2021-03-04 23:02:43.000000 modin-0.9.0/modin/data_management/functions/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     3260 2021-03-04 23:02:43.000000 modin-0.9.0/modin/data_management/functions/binary_function.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1431 2021-03-04 23:02:43.000000 modin-0.9.0/modin/data_management/functions/reductionfunction.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1358 2021-03-04 23:02:43.000000 modin-0.9.0/modin/data_management/functions/function.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/backends/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1058 2021-03-04 23:02:43.000000 modin-0.9.0/modin/backends/__init__.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/backends/base/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    64647 2021-03-04 23:02:43.000000 modin-0.9.0/modin/backends/base/query_compiler.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      862 2021-03-04 23:02:43.000000 modin-0.9.0/modin/backends/base/__init__.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/backends/pandas/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)   111848 2021-03-04 23:02:43.000000 modin-0.9.0/modin/backends/pandas/query_compiler.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      866 2021-03-04 23:02:43.000000 modin-0.9.0/modin/backends/pandas/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    17941 2021-03-04 23:02:43.000000 modin-0.9.0/modin/backends/pandas/parsers.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/backends/pyarrow/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     7820 2021-03-04 23:02:43.000000 modin-0.9.0/modin/backends/pyarrow/query_compiler.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      868 2021-03-04 23:02:43.000000 modin-0.9.0/modin/backends/pyarrow/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1995 2021-03-04 23:02:43.000000 modin-0.9.0/modin/backends/pyarrow/parsers.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     2403 2021-03-04 23:02:43.000000 modin-0.9.0/modin/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1924 2021-03-04 23:02:43.000000 modin-0.9.0/modin/apply_license_header.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     3221 2021-03-04 23:02:43.000000 modin-0.9.0/modin/error_message.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     4788 2021-03-04 23:02:43.000000 modin-0.9.0/modin/utils.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/engines/
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/engines/dask/
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/engines/dask/pandas_on_dask/
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/engines/dask/pandas_on_dask/series/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/dask/pandas_on_dask/series/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     2484 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/dask/pandas_on_dask/io.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/dask/pandas_on_dask/__init__.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/engines/dask/pandas_on_dask/frame/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     7341 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/dask/pandas_on_dask/frame/partition.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/dask/pandas_on_dask/frame/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     5346 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/dask/pandas_on_dask/frame/partition_manager.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     4533 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/dask/pandas_on_dask/frame/axis_partition.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1985 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/dask/pandas_on_dask/frame/data.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1275 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/dask/task_wrapper.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/dask/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1295 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/dask/utils.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/engines/python/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/python/__init__.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/engines/python/pandas_on_python/
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/engines/python/pandas_on_python/series/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/python/pandas_on_python/series/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1090 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/python/pandas_on_python/io.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/python/pandas_on_python/__init__.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/engines/python/pandas_on_python/frame/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     6096 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/python/pandas_on_python/frame/partition.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/python/pandas_on_python/frame/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1385 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/python/pandas_on_python/frame/partition_manager.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1898 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/python/pandas_on_python/frame/axis_partition.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      978 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/python/pandas_on_python/frame/data.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/__init__.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/engines/ray/
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/engines/ray/pandas_on_ray/
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/engines/ray/pandas_on_ray/series/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/ray/pandas_on_ray/series/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     2593 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/ray/pandas_on_ray/io.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/ray/pandas_on_ray/__init__.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/engines/ray/pandas_on_ray/frame/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     8472 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/ray/pandas_on_ray/frame/partition.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/ray/pandas_on_ray/frame/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     3203 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/ray/pandas_on_ray/frame/modin_aqp.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     9090 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/ray/pandas_on_ray/frame/partition_manager.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     4106 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/ray/pandas_on_ray/frame/axis_partition.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1731 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/ray/pandas_on_ray/frame/data.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1135 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/ray/task_wrapper.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/ray/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     6484 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/ray/utils.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/engines/ray/generic/
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/engines/ray/generic/series/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/ray/generic/series/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     6012 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/ray/generic/io.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/ray/generic/__init__.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/engines/ray/generic/frame/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/ray/generic/frame/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1589 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/ray/generic/frame/partition_manager.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/engines/base/
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/engines/base/series/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/base/series/__init__.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/engines/base/io/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    19466 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/base/io/io.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1921 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/base/io/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     5403 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/base/io/file_dispatcher.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/engines/base/io/column_stores/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     5758 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/base/io/column_stores/parquet_dispatcher.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/base/io/column_stores/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     4536 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/base/io/column_stores/column_store_dispatcher.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     2787 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/base/io/column_stores/hdf_dispatcher.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1805 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/base/io/column_stores/feather_dispatcher.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/engines/base/io/text/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     4054 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/base/io/text/json_dispatcher.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/base/io/text/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    10411 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/base/io/text/excel_dispatcher.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    13119 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/base/io/text/text_file_dispatcher.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    19053 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/base/io/text/csv_glob_dispatcher.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    14084 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/base/io/text/csv_dispatcher.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    10803 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/base/io/text/fwf_dispatcher.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/engines/base/io/sql/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/base/io/sql/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     4538 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/base/io/sql/sql_dispatcher.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/base/__init__.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/engines/base/frame/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     5782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/base/frame/partition.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/base/frame/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    37276 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/base/frame/partition_manager.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    13348 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/base/frame/axis_partition.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    78911 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/base/frame/data.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      682 2021-03-04 23:02:43.000000 modin-0.9.0/modin/engines/base/README.md
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/pandas/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     3867 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/accessor.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/pandas/test/
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/pandas/test/dataframe/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    12797 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/dataframe/test_iter.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    42449 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/dataframe/test_map_metadata.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/dataframe/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    46097 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/dataframe/test_indexing.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    10811 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/dataframe/test_udf.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    11955 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/dataframe/test_reduction.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     7991 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/dataframe/test_binary.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    39909 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/dataframe/test_default.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    21862 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/dataframe/test_window.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    18994 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/dataframe/test_join_sort.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     8886 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/test_rolling.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     4767 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/test_reshape.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    68515 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/test_io.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    39428 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/utils.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     7226 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/test_concat.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    53395 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/test_groupby.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    11091 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/test_api.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    23959 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/test_general.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/pandas/test/data/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      494 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/data/issue_2074.csv
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    13216 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/data/modin_error_book.xlsx
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1672 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/data/issue_2239.csv
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      281 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/data/test_time_parsing.csv
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    73763 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/data/blah.csv
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)       24 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/data/test_categories.csv
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)       70 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/data/test_usecols.csv
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)       21 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/data/test_null_col.csv
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      782 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/data/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    13221 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/data/excel_sheetname_title.xlsx
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/pandas/test/data/hdfs.parquet/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      644 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/data/hdfs.parquet/part-00002-a7bff54c-2ff4-4654-9783-626542bd3a90-c000.snappy.parquet
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      628 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/data/hdfs.parquet/part-00001-a7bff54c-2ff4-4654-9783-626542bd3a90-c000.snappy.parquet
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      636 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/data/hdfs.parquet/part-00000-a7bff54c-2ff4-4654-9783-626542bd3a90-c000.snappy.parquet
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)       70 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/data/test_delim.csv
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1046 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/data/newlines.csv
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      692 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/data/issue_976.csv
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)       71 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/data/test_categories.json
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    10725 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/data/test_emptyline.xlsx
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)   163694 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/test/test_series.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    21825 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/series_utils.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    83996 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/dataframe.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     2322 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/plotting.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    21200 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/io.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    57220 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/series.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     7232 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1996 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/iterator.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     4226 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/utils.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    26128 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/indexing.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    34919 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/groupby.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)   116267 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/base.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    20508 2021-03-04 23:02:43.000000 modin-0.9.0/modin/pandas/general.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin/sql/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      838 2021-03-04 23:02:43.000000 modin-0.9.0/modin/sql/__init__.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     2240 2021-03-04 23:02:43.000000 modin-0.9.0/modin/sql/connection.py
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/scripts/
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/scripts/conda-recipe/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)       82 2021-03-04 23:02:43.000000 modin-0.9.0/scripts/conda-recipe/conda_build_config.yaml
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      171 2021-03-04 23:02:43.000000 modin-0.9.0/scripts/conda-recipe/run_test.py
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      947 2021-03-04 23:02:43.000000 modin-0.9.0/scripts/conda-recipe/meta.yaml
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/.github/
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/.github/workflows/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    12766 2021-03-04 23:02:43.000000 modin-0.9.0/.github/workflows/push.yml
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    22715 2021-03-04 23:02:43.000000 modin-0.9.0/.github/workflows/ci.yml
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1366 2021-03-04 23:02:43.000000 modin-0.9.0/.github/stale.yml
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      653 2021-03-04 23:02:43.000000 modin-0.9.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      850 2021-03-04 23:02:43.000000 modin-0.9.0/.github/ISSUE_TEMPLATE.md
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      356 2021-03-04 23:02:43.000000 modin-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      799 2021-03-04 23:02:43.000000 modin-0.9.0/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      114 2021-03-04 23:02:43.000000 modin-0.9.0/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)       43 2021-03-04 23:02:43.000000 modin-0.9.0/.gitattributes
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      329 2021-03-04 23:02:43.000000 modin-0.9.0/commitlint.config.js
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)     1263 2021-03-04 23:03:14.000000 modin-0.9.0/setup.cfg
-drwxr-xr-x   0 DevinPetersohn   (501) staff       (20)        0 2021-03-04 23:03:14.000000 modin-0.9.0/modin.egg-info/
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    10890 2021-03-04 23:03:13.000000 modin-0.9.0/modin.egg-info/PKG-INFO
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    16204 2021-03-04 23:03:13.000000 modin-0.9.0/modin.egg-info/SOURCES.txt
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)      393 2021-03-04 23:03:13.000000 modin-0.9.0/modin.egg-info/requires.txt
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)        6 2021-03-04 23:03:13.000000 modin-0.9.0/modin.egg-info/top_level.txt
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)        1 2021-03-04 23:03:13.000000 modin-0.9.0/modin.egg-info/dependency_links.txt
--rw-r--r--   0 DevinPetersohn   (501) staff       (20)    68611 2021-03-04 23:02:43.000000 modin-0.9.0/versioneer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.623445 modin-0.9.1/
+-rwxrwxrwx   0 root         (0) root         (0)      137 2021-03-16 01:45:29.868853 modin-0.9.1/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)    10890 2021-03-16 01:55:39.623445 modin-0.9.1/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     8917 2021-03-16 01:51:31.857295 modin-0.9.1/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.631894 modin-0.9.1/modin/
+-rwxrwxrwx   0 root         (0) root         (0)     2403 2021-03-16 01:45:21.000000 modin-0.9.1/modin/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      497 2021-03-16 01:55:39.631894 modin-0.9.1/modin/_version.py
+-rwxrwxrwx   0 root         (0) root         (0)     1924 2021-03-16 01:45:21.000000 modin-0.9.1/modin/apply_license_header.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:38.971017 modin-0.9.1/modin/backends/
+-rwxrwxrwx   0 root         (0) root         (0)     1058 2021-03-16 01:45:21.000000 modin-0.9.1/modin/backends/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:38.975006 modin-0.9.1/modin/backends/base/
+-rwxrwxrwx   0 root         (0) root         (0)      862 2021-03-16 01:45:21.000000 modin-0.9.1/modin/backends/base/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    64819 2021-03-16 01:45:21.000000 modin-0.9.1/modin/backends/base/query_compiler.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:38.987253 modin-0.9.1/modin/backends/pandas/
+-rwxrwxrwx   0 root         (0) root         (0)      866 2021-03-16 01:45:21.000000 modin-0.9.1/modin/backends/pandas/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    17941 2021-03-16 01:45:21.000000 modin-0.9.1/modin/backends/pandas/parsers.py
+-rwxrwxrwx   0 root         (0) root         (0)   116711 2021-03-16 01:45:21.000000 modin-0.9.1/modin/backends/pandas/query_compiler.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:38.997254 modin-0.9.1/modin/backends/pyarrow/
+-rwxrwxrwx   0 root         (0) root         (0)      868 2021-03-16 01:45:21.000000 modin-0.9.1/modin/backends/pyarrow/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1995 2021-03-16 01:45:21.000000 modin-0.9.1/modin/backends/pyarrow/parsers.py
+-rwxrwxrwx   0 root         (0) root         (0)     7820 2021-03-16 01:45:21.000000 modin-0.9.1/modin/backends/pyarrow/query_compiler.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.008197 modin-0.9.1/modin/config/
+-rwxrwxrwx   0 root         (0) root         (0)      870 2021-03-16 01:45:21.000000 modin-0.9.1/modin/config/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1172 2021-03-16 01:45:21.000000 modin-0.9.1/modin/config/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8874 2021-03-16 01:45:21.000000 modin-0.9.1/modin/config/envvars.py
+-rwxrwxrwx   0 root         (0) root         (0)     4942 2021-03-16 01:45:21.000000 modin-0.9.1/modin/config/pubsub.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.013068 modin-0.9.1/modin/config/test/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/config/test/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2052 2021-03-16 01:45:21.000000 modin-0.9.1/modin/config/test/test_envvars.py
+-rwxrwxrwx   0 root         (0) root         (0)     2936 2021-03-16 01:45:21.000000 modin-0.9.1/modin/config/test/test_parameter.py
+-rwxrwxrwx   0 root         (0) root         (0)    13138 2021-03-16 01:45:21.000000 modin-0.9.1/modin/conftest.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.016063 modin-0.9.1/modin/data_management/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/data_management/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.021046 modin-0.9.1/modin/data_management/factories/
+-rwxrwxrwx   0 root         (0) root         (0)     1193 2021-03-16 01:45:21.000000 modin-0.9.1/modin/data_management/factories/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5760 2021-03-16 01:45:21.000000 modin-0.9.1/modin/data_management/factories/dispatcher.py
+-rwxrwxrwx   0 root         (0) root         (0)    10030 2021-03-16 01:45:21.000000 modin-0.9.1/modin/data_management/factories/factories.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.028027 modin-0.9.1/modin/data_management/factories/test/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/data_management/factories/test/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3027 2021-03-16 01:45:21.000000 modin-0.9.1/modin/data_management/factories/test/test_dispatcher.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.044411 modin-0.9.1/modin/data_management/functions/
+-rwxrwxrwx   0 root         (0) root         (0)     1313 2021-03-16 01:45:21.000000 modin-0.9.1/modin/data_management/functions/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3260 2021-03-16 01:45:21.000000 modin-0.9.1/modin/data_management/functions/binary_function.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.072283 modin-0.9.1/modin/data_management/functions/default_methods/
+-rwxrwxrwx   0 root         (0) root         (0)     1484 2021-03-16 01:45:21.000000 modin-0.9.1/modin/data_management/functions/default_methods/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1333 2021-03-16 01:45:21.000000 modin-0.9.1/modin/data_management/functions/default_methods/any_default.py
+-rwxrwxrwx   0 root         (0) root         (0)     1771 2021-03-16 01:45:21.000000 modin-0.9.1/modin/data_management/functions/default_methods/binary_default.py
+-rwxrwxrwx   0 root         (0) root         (0)      947 2021-03-16 01:45:21.000000 modin-0.9.1/modin/data_management/functions/default_methods/cat_default.py
+-rwxrwxrwx   0 root         (0) root         (0)     1073 2021-03-16 01:45:21.000000 modin-0.9.1/modin/data_management/functions/default_methods/dataframe_default.py
+-rwxrwxrwx   0 root         (0) root         (0)      951 2021-03-16 01:45:21.000000 modin-0.9.1/modin/data_management/functions/default_methods/datetime_default.py
+-rwxrwxrwx   0 root         (0) root         (0)     3346 2021-03-16 01:45:21.000000 modin-0.9.1/modin/data_management/functions/default_methods/default.py
+-rwxrwxrwx   0 root         (0) root         (0)     5268 2021-03-16 01:45:21.000000 modin-0.9.1/modin/data_management/functions/default_methods/groupby_default.py
+-rwxrwxrwx   0 root         (0) root         (0)     1528 2021-03-16 01:45:21.000000 modin-0.9.1/modin/data_management/functions/default_methods/resample_default.py
+-rwxrwxrwx   0 root         (0) root         (0)     1344 2021-03-16 01:45:21.000000 modin-0.9.1/modin/data_management/functions/default_methods/rolling_default.py
+-rwxrwxrwx   0 root         (0) root         (0)      965 2021-03-16 01:45:21.000000 modin-0.9.1/modin/data_management/functions/default_methods/series_default.py
+-rwxrwxrwx   0 root         (0) root         (0)      947 2021-03-16 01:45:21.000000 modin-0.9.1/modin/data_management/functions/default_methods/str_default.py
+-rwxrwxrwx   0 root         (0) root         (0)     1291 2021-03-16 01:45:21.000000 modin-0.9.1/modin/data_management/functions/foldfunction.py
+-rwxrwxrwx   0 root         (0) root         (0)     1358 2021-03-16 01:45:21.000000 modin-0.9.1/modin/data_management/functions/function.py
+-rwxrwxrwx   0 root         (0) root         (0)     9871 2021-03-16 01:45:21.000000 modin-0.9.1/modin/data_management/functions/groupby_function.py
+-rwxrwxrwx   0 root         (0) root         (0)     1209 2021-03-16 01:45:21.000000 modin-0.9.1/modin/data_management/functions/mapfunction.py
+-rwxrwxrwx   0 root         (0) root         (0)     1615 2021-03-16 01:45:21.000000 modin-0.9.1/modin/data_management/functions/mapreducefunction.py
+-rwxrwxrwx   0 root         (0) root         (0)     1313 2021-03-16 01:45:21.000000 modin-0.9.1/modin/data_management/functions/reductionfunction.py
+-rwxrwxrwx   0 root         (0) root         (0)     4416 2021-03-16 01:45:21.000000 modin-0.9.1/modin/data_management/utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.074250 modin-0.9.1/modin/distributed/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/distributed/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.076245 modin-0.9.1/modin/distributed/dataframe/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/distributed/dataframe/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.080263 modin-0.9.1/modin/distributed/dataframe/pandas/
+-rwxrwxrwx   0 root         (0) root         (0)      894 2021-03-16 01:45:21.000000 modin-0.9.1/modin/distributed/dataframe/pandas/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6760 2021-03-16 01:45:21.000000 modin-0.9.1/modin/distributed/dataframe/pandas/partitions.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.085220 modin-0.9.1/modin/engines/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.087216 modin-0.9.1/modin/engines/base/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/base/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.104820 modin-0.9.1/modin/engines/base/frame/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/base/frame/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    13348 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/base/frame/axis_partition.py
+-rwxrwxrwx   0 root         (0) root         (0)    79032 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/base/frame/data.py
+-rwxrwxrwx   0 root         (0) root         (0)     5871 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/base/frame/partition.py
+-rwxrwxrwx   0 root         (0) root         (0)    38696 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/base/frame/partition_manager.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.114098 modin-0.9.1/modin/engines/base/io/
+-rwxrwxrwx   0 root         (0) root         (0)     1921 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/base/io/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.131052 modin-0.9.1/modin/engines/base/io/column_stores/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/base/io/column_stores/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4536 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/base/io/column_stores/column_store_dispatcher.py
+-rwxrwxrwx   0 root         (0) root         (0)     1805 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/base/io/column_stores/feather_dispatcher.py
+-rwxrwxrwx   0 root         (0) root         (0)     2787 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/base/io/column_stores/hdf_dispatcher.py
+-rwxrwxrwx   0 root         (0) root         (0)     5758 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/base/io/column_stores/parquet_dispatcher.py
+-rwxrwxrwx   0 root         (0) root         (0)     5403 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/base/io/file_dispatcher.py
+-rwxrwxrwx   0 root         (0) root         (0)    19466 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/base/io/io.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.134508 modin-0.9.1/modin/engines/base/io/sql/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/base/io/sql/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4538 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/base/io/sql/sql_dispatcher.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.161620 modin-0.9.1/modin/engines/base/io/text/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/base/io/text/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    14084 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/base/io/text/csv_dispatcher.py
+-rwxrwxrwx   0 root         (0) root         (0)    19053 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/base/io/text/csv_glob_dispatcher.py
+-rwxrwxrwx   0 root         (0) root         (0)    10411 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/base/io/text/excel_dispatcher.py
+-rwxrwxrwx   0 root         (0) root         (0)    10803 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/base/io/text/fwf_dispatcher.py
+-rwxrwxrwx   0 root         (0) root         (0)     4054 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/base/io/text/json_dispatcher.py
+-rwxrwxrwx   0 root         (0) root         (0)    13119 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/base/io/text/text_file_dispatcher.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.166778 modin-0.9.1/modin/engines/base/series/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/base/series/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.172342 modin-0.9.1/modin/engines/dask/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/dask/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.176153 modin-0.9.1/modin/engines/dask/pandas_on_dask/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/dask/pandas_on_dask/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.187082 modin-0.9.1/modin/engines/dask/pandas_on_dask/frame/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/dask/pandas_on_dask/frame/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4533 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/dask/pandas_on_dask/frame/axis_partition.py
+-rwxrwxrwx   0 root         (0) root         (0)     1985 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/dask/pandas_on_dask/frame/data.py
+-rwxrwxrwx   0 root         (0) root         (0)     7454 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/dask/pandas_on_dask/frame/partition.py
+-rwxrwxrwx   0 root         (0) root         (0)     5346 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/dask/pandas_on_dask/frame/partition_manager.py
+-rwxrwxrwx   0 root         (0) root         (0)     2484 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/dask/pandas_on_dask/io.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.189078 modin-0.9.1/modin/engines/dask/pandas_on_dask/series/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/dask/pandas_on_dask/series/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1275 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/dask/task_wrapper.py
+-rwxrwxrwx   0 root         (0) root         (0)     1404 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/dask/utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.190075 modin-0.9.1/modin/engines/python/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/python/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.194210 modin-0.9.1/modin/engines/python/pandas_on_python/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/python/pandas_on_python/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.205383 modin-0.9.1/modin/engines/python/pandas_on_python/frame/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/python/pandas_on_python/frame/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1898 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/python/pandas_on_python/frame/axis_partition.py
+-rwxrwxrwx   0 root         (0) root         (0)      978 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/python/pandas_on_python/frame/data.py
+-rwxrwxrwx   0 root         (0) root         (0)     6149 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/python/pandas_on_python/frame/partition.py
+-rwxrwxrwx   0 root         (0) root         (0)     1385 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/python/pandas_on_python/frame/partition_manager.py
+-rwxrwxrwx   0 root         (0) root         (0)     1090 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/python/pandas_on_python/io.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.210033 modin-0.9.1/modin/engines/python/pandas_on_python/series/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/python/pandas_on_python/series/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.216106 modin-0.9.1/modin/engines/ray/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/ray/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.219623 modin-0.9.1/modin/engines/ray/generic/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/ray/generic/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.223359 modin-0.9.1/modin/engines/ray/generic/frame/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/ray/generic/frame/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1589 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/ray/generic/frame/partition_manager.py
+-rwxrwxrwx   0 root         (0) root         (0)     6012 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/ray/generic/io.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.226350 modin-0.9.1/modin/engines/ray/generic/series/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/ray/generic/series/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.229931 modin-0.9.1/modin/engines/ray/pandas_on_ray/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/ray/pandas_on_ray/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.248030 modin-0.9.1/modin/engines/ray/pandas_on_ray/frame/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/ray/pandas_on_ray/frame/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4106 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/ray/pandas_on_ray/frame/axis_partition.py
+-rwxrwxrwx   0 root         (0) root         (0)     1731 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/ray/pandas_on_ray/frame/data.py
+-rwxrwxrwx   0 root         (0) root         (0)     3203 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/ray/pandas_on_ray/frame/modin_aqp.py
+-rwxrwxrwx   0 root         (0) root         (0)     8642 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/ray/pandas_on_ray/frame/partition.py
+-rwxrwxrwx   0 root         (0) root         (0)     9090 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/ray/pandas_on_ray/frame/partition_manager.py
+-rwxrwxrwx   0 root         (0) root         (0)     2593 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/ray/pandas_on_ray/io.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.253017 modin-0.9.1/modin/engines/ray/pandas_on_ray/series/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/ray/pandas_on_ray/series/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1135 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/ray/task_wrapper.py
+-rwxrwxrwx   0 root         (0) root         (0)     6594 2021-03-16 01:45:21.000000 modin-0.9.1/modin/engines/ray/utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     3221 2021-03-16 01:45:21.000000 modin-0.9.1/modin/error_message.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.254984 modin-0.9.1/modin/experimental/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.256010 modin-0.9.1/modin/experimental/backends/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/backends/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.260004 modin-0.9.1/modin/experimental/backends/omnisci/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/backends/omnisci/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    21592 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/backends/omnisci/query_compiler.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.286153 modin-0.9.1/modin/experimental/cloud/
+-rwxrwxrwx   0 root         (0) root         (0)     1258 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/cloud/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2341 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/cloud/base.py
+-rwxrwxrwx   0 root         (0) root         (0)    11522 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/cloud/cluster.py
+-rwxrwxrwx   0 root         (0) root         (0)     7556 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/cloud/connection.py
+-rwxrwxrwx   0 root         (0) root         (0)     3801 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/cloud/local_cluster.py
+-rwxrwxrwx   0 root         (0) root         (0)     6712 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/cloud/meta_magic.py
+-rwxrwxrwx   0 root         (0) root         (0)     1648 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/cloud/omnisci.py
+-rwxrwxrwx   0 root         (0) root         (0)     6969 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/cloud/ray-autoscaler.yml
+-rwxrwxrwx   0 root         (0) root         (0)     9276 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/cloud/rayscale.py
+-rwxrwxrwx   0 root         (0) root         (0)    27221 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/cloud/rpyc_proxy.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.292963 modin-0.9.1/modin/experimental/cloud/test/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/cloud/test/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4497 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/cloud/test/test_cloud.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.297981 modin-0.9.1/modin/experimental/cloud/tracing/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/cloud/tracing/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7175 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/cloud/tracing/parse_rpyc_trace.py
+-rwxrwxrwx   0 root         (0) root         (0)     4052 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/cloud/tracing/tracing_connection.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.299974 modin-0.9.1/modin/experimental/engines/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/engines/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.303936 modin-0.9.1/modin/experimental/engines/omnisci_on_ray/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/engines/omnisci_on_ray/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.342859 modin-0.9.1/modin/experimental/engines/omnisci_on_ray/frame/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/engines/omnisci_on_ray/frame/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1877 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/engines/omnisci_on_ray/frame/axis_partition.py
+-rwxrwxrwx   0 root         (0) root         (0)     3989 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/engines/omnisci_on_ray/frame/calcite_algebra.py
+-rwxrwxrwx   0 root         (0) root         (0)    20326 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/engines/omnisci_on_ray/frame/calcite_builder.py
+-rwxrwxrwx   0 root         (0) root         (0)     6525 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/engines/omnisci_on_ray/frame/calcite_serializer.py
+-rwxrwxrwx   0 root         (0) root         (0)    54138 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/engines/omnisci_on_ray/frame/data.py
+-rwxrwxrwx   0 root         (0) root         (0)    10175 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/engines/omnisci_on_ray/frame/df_algebra.py
+-rwxrwxrwx   0 root         (0) root         (0)     9935 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/engines/omnisci_on_ray/frame/expr.py
+-rwxrwxrwx   0 root         (0) root         (0)     4268 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/engines/omnisci_on_ray/frame/omnisci_worker.py
+-rwxrwxrwx   0 root         (0) root         (0)     2105 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/engines/omnisci_on_ray/frame/partition.py
+-rwxrwxrwx   0 root         (0) root         (0)     7719 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/engines/omnisci_on_ray/frame/partition_manager.py
+-rwxrwxrwx   0 root         (0) root         (0)     9725 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/engines/omnisci_on_ray/io.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.347847 modin-0.9.1/modin/experimental/engines/omnisci_on_ray/test/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/engines/omnisci_on_ray/test/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    53694 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/engines/omnisci_on_ray/test/test_dataframe.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.359815 modin-0.9.1/modin/experimental/engines/pandas_on_ray/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/engines/pandas_on_ray/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8286 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/engines/pandas_on_ray/io_exp.py
+-rwxrwxrwx   0 root         (0) root         (0)     6290 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/engines/pandas_on_ray/sql.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.366801 modin-0.9.1/modin/experimental/engines/pyarrow_on_ray/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/engines/pyarrow_on_ray/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.379947 modin-0.9.1/modin/experimental/engines/pyarrow_on_ray/frame/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/engines/pyarrow_on_ray/frame/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7740 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/engines/pyarrow_on_ray/frame/axis_partition.py
+-rwxrwxrwx   0 root         (0) root         (0)     2246 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/engines/pyarrow_on_ray/frame/data.py
+-rwxrwxrwx   0 root         (0) root         (0)     1936 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/engines/pyarrow_on_ray/frame/partition.py
+-rwxrwxrwx   0 root         (0) root         (0)     1384 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/engines/pyarrow_on_ray/frame/partition_manager.py
+-rwxrwxrwx   0 root         (0) root         (0)     1803 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/engines/pyarrow_on_ray/io.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.385168 modin-0.9.1/modin/experimental/engines/pyarrow_on_ray/series/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/engines/pyarrow_on_ray/series/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.390187 modin-0.9.1/modin/experimental/pandas/
+-rwxrwxrwx   0 root         (0) root         (0)     1316 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/pandas/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6697 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/pandas/io_exp.py
+-rwxrwxrwx   0 root         (0) root         (0)     6867 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/pandas/numpy_wrap.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.393209 modin-0.9.1/modin/experimental/pandas/test/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/pandas/test/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4416 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/pandas/test/test_io_exp.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.395204 modin-0.9.1/modin/experimental/sklearn/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/sklearn/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.399165 modin-0.9.1/modin/experimental/sklearn/model_selection/
+-rwxrwxrwx   0 root         (0) root         (0)      862 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/sklearn/model_selection/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      975 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/sklearn/model_selection/train_test_split.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.408170 modin-0.9.1/modin/experimental/xgboost/
+-rwxrwxrwx   0 root         (0) root         (0)      871 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/xgboost/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.415151 modin-0.9.1/modin/experimental/xgboost/test/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/xgboost/test/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1147 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/xgboost/test/test_default.py
+-rwxrwxrwx   0 root         (0) root         (0)     1968 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/xgboost/utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     4968 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/xgboost/xgboost.py
+-rwxrwxrwx   0 root         (0) root         (0)    12739 2021-03-16 01:45:21.000000 modin-0.9.1/modin/experimental/xgboost/xgboost_ray.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.467472 modin-0.9.1/modin/pandas/
+-rwxrwxrwx   0 root         (0) root         (0)     7232 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3867 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/accessor.py
+-rwxrwxrwx   0 root         (0) root         (0)   116231 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/base.py
+-rwxrwxrwx   0 root         (0) root         (0)    84700 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/dataframe.py
+-rwxrwxrwx   0 root         (0) root         (0)    20508 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/general.py
+-rwxrwxrwx   0 root         (0) root         (0)    34919 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/groupby.py
+-rwxrwxrwx   0 root         (0) root         (0)    26128 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/indexing.py
+-rwxrwxrwx   0 root         (0) root         (0)    21200 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/io.py
+-rwxrwxrwx   0 root         (0) root         (0)     1996 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/iterator.py
+-rwxrwxrwx   0 root         (0) root         (0)     2322 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/plotting.py
+-rwxrwxrwx   0 root         (0) root         (0)    57783 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/series.py
+-rwxrwxrwx   0 root         (0) root         (0)    21825 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/series_utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.506098 modin-0.9.1/modin/pandas/test/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/test/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.539915 modin-0.9.1/modin/pandas/test/data/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/test/data/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    73763 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/test/data/blah.csv
+-rwxrwxrwx   0 root         (0) root         (0)      494 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/test/data/issue_2074.csv
+-rwxrwxrwx   0 root         (0) root         (0)     1672 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/test/data/issue_2239.csv
+-rwxrwxrwx   0 root         (0) root         (0)      692 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/test/data/issue_976.csv
+-rwxrwxrwx   0 root         (0) root         (0)     1046 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/test/data/newlines.csv
+-rwxrwxrwx   0 root         (0) root         (0)       24 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/test/data/test_categories.csv
+-rwxrwxrwx   0 root         (0) root         (0)       70 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/test/data/test_delim.csv
+-rwxrwxrwx   0 root         (0) root         (0)       21 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/test/data/test_null_col.csv
+-rwxrwxrwx   0 root         (0) root         (0)      281 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/test/data/test_time_parsing.csv
+-rwxrwxrwx   0 root         (0) root         (0)       70 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/test/data/test_usecols.csv
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.588431 modin-0.9.1/modin/pandas/test/dataframe/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/test/dataframe/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8053 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/test/dataframe/test_binary.py
+-rwxrwxrwx   0 root         (0) root         (0)    39677 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/test/dataframe/test_default.py
+-rwxrwxrwx   0 root         (0) root         (0)    53924 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/test/dataframe/test_indexing.py
+-rwxrwxrwx   0 root         (0) root         (0)    11553 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/test/dataframe/test_iter.py
+-rwxrwxrwx   0 root         (0) root         (0)    18994 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/test/dataframe/test_join_sort.py
+-rwxrwxrwx   0 root         (0) root         (0)    42449 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/test/dataframe/test_map_metadata.py
+-rwxrwxrwx   0 root         (0) root         (0)     1795 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/test/dataframe/test_pickle.py
+-rwxrwxrwx   0 root         (0) root         (0)    12232 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/test/dataframe/test_reduction.py
+-rwxrwxrwx   0 root         (0) root         (0)    10811 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/test/dataframe/test_udf.py
+-rwxrwxrwx   0 root         (0) root         (0)    21862 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/test/dataframe/test_window.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.595413 modin-0.9.1/modin/pandas/test/internals/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/test/internals/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1037 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/test/internals/test_benchmark_mode.py
+-rwxrwxrwx   0 root         (0) root         (0)    11091 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/test/test_api.py
+-rwxrwxrwx   0 root         (0) root         (0)     7226 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/test/test_concat.py
+-rwxrwxrwx   0 root         (0) root         (0)    23959 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/test/test_general.py
+-rwxrwxrwx   0 root         (0) root         (0)    53395 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/test/test_groupby.py
+-rwxrwxrwx   0 root         (0) root         (0)    68738 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/test/test_io.py
+-rwxrwxrwx   0 root         (0) root         (0)     4767 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/test/test_reshape.py
+-rwxrwxrwx   0 root         (0) root         (0)     8886 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/test/test_rolling.py
+-rwxrwxrwx   0 root         (0) root         (0)   163694 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/test/test_series.py
+-rwxrwxrwx   0 root         (0) root         (0)    39598 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/test/utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     4226 2021-03-16 01:45:21.000000 modin-0.9.1/modin/pandas/utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.601246 modin-0.9.1/modin/spreadsheet/
+-rwxrwxrwx   0 root         (0) root         (0)     1073 2021-03-16 01:45:21.000000 modin-0.9.1/modin/spreadsheet/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8448 2021-03-16 01:45:21.000000 modin-0.9.1/modin/spreadsheet/general.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.609524 modin-0.9.1/modin/spreadsheet/test/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/spreadsheet/test/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1986 2021-03-16 01:45:21.000000 modin-0.9.1/modin/spreadsheet/test/test_general.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.612783 modin-0.9.1/modin/sql/
+-rwxrwxrwx   0 root         (0) root         (0)      838 2021-03-16 01:45:21.000000 modin-0.9.1/modin/sql/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2240 2021-03-16 01:45:21.000000 modin-0.9.1/modin/sql/connection.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:39.622418 modin-0.9.1/modin/test/
+-rwxrwxrwx   0 root         (0) root         (0)      782 2021-03-16 01:45:21.000000 modin-0.9.1/modin/test/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2078 2021-03-16 01:45:21.000000 modin-0.9.1/modin/test/test_backends_api.py
+-rwxrwxrwx   0 root         (0) root         (0)     1226 2021-03-16 01:45:21.000000 modin-0.9.1/modin/test/test_envvar_catcher.py
+-rwxrwxrwx   0 root         (0) root         (0)     2060 2021-03-16 01:45:21.000000 modin-0.9.1/modin/test/test_envvar_npartitions.py
+-rwxrwxrwx   0 root         (0) root         (0)     2291 2021-03-16 01:45:21.000000 modin-0.9.1/modin/test/test_headers.py
+-rwxrwxrwx   0 root         (0) root         (0)     4037 2021-03-16 01:45:21.000000 modin-0.9.1/modin/test/test_partition_api.py
+-rwxrwxrwx   0 root         (0) root         (0)     4788 2021-03-16 01:45:21.000000 modin-0.9.1/modin/utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2021-03-16 01:55:38.970047 modin-0.9.1/modin.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)    10890 2021-03-16 01:55:38.000000 modin-0.9.1/modin.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)    10268 2021-03-16 01:55:38.000000 modin-0.9.1/modin.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2021-03-16 01:55:38.000000 modin-0.9.1/modin.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)      393 2021-03-16 01:55:38.000000 modin-0.9.1/modin.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        6 2021-03-16 01:55:38.000000 modin-0.9.1/modin.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)     1263 2021-03-16 01:55:39.628431 modin-0.9.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1980 2021-03-16 01:51:29.000000 modin-0.9.1/setup.py
+-rwxrwxrwx   0 root         (0) root         (0)    68611 2021-03-16 01:45:21.000000 modin-0.9.1/versioneer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `modin-0.9.0/PKG-INFO` & `modin-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: modin
-Version: 0.9.0
+Version: 0.9.1
 Summary: Modin: Make your pandas code run faster by changing one line of code.
 Home-page: https://github.com/modin-project/modin
 License: Apache 2
 Description: <p align="center"><a href="https://modin.readthedocs.io"><img width=77% alt="" src="https://github.com/modin-project/modin/blob/3d6368edf311995ad231ec5342a51cd9e4e3dc20/docs/img/MODIN_ver2_hrz.png?raw=true"></a></p>
         <h2 align="center">Scale your pandas workflows by changing one line of code</h2>
         
         <p align="center">
         <a href="https://discuss.modin.org"><img alt="" src="https://img.shields.io/badge/discourse-forum-purple.svg?logo=discourse&logoColor=white" align="center"></a>
         <a href="https://codecov.io/gh/modin-project/modin"><img src="https://codecov.io/gh/modin-project/modin/branch/master/graph/badge.svg" align="center"/></a>
         <a href="https://github.com/modin-project/modin/actions"><img src="https://github.com/modin-project/modin/workflows/master/badge.svg" align="center"></a>
         <a href="https://modin.readthedocs.io/en/latest/?badge=latest"><img alt="" src="https://readthedocs.org/projects/modin/badge/?version=latest" align="center"></a>
-        <a href="https://pypi.org/project/modin/"><img alt="" src="https://img.shields.io/badge/pypi-0.9.0-blue.svg" align="center"></a>
+        <a href="https://pypi.org/project/modin/"><img alt="" src="https://img.shields.io/badge/pypi-0.9.1-blue.svg" align="center"></a>
         </p>
         
         <p align="center"><b>To use Modin, replace the pandas import:</b></p>
         
         ```python
         # import pandas as pd
         import modin.pandas as pd
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: modin Version: 0.9.0 Summary: Modin: Make your
+Metadata-Version: 2.1 Name: modin Version: 0.9.1 Summary: Modin: Make your
 pandas code run faster by changing one line of code. Home-page: https://
 github.com/modin-project/modin License: Apache 2 Description:
      ***** Scale your pandas workflows by changing one line of code *****
    [https://codecov.io/gh/modin-project/modin/branch/master/graph/badge.svg]
      [https://github.com/modin-project/modin/workflows/master/badge.svg]
                    To use Modin, replace the pandas import:
 ```python # import pandas as pd import modin.pandas as pd ``` ### Installation
```

### Comparing `modin-0.9.0/asv_bench/benchmarks/io/__init__.py` & `modin-0.9.1/modin/config/test/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/asv_bench/benchmarks/__init__.py` & `modin-0.9.1/modin/data_management/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,9 +6,7 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
-
-"""Modin benchmarks"""
```

### Comparing `modin-0.9.0/asv_bench/benchmarks/utils.py` & `modin-0.9.1/modin/experimental/engines/pyarrow_on_ray/frame/axis_partition.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,237 +7,215 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 
-import os
-import logging
-import modin.pandas as pd
-import pandas
-import numpy as np
-import uuid
-
-RAND_LOW = 0
-RAND_HIGH = 100
-random_state = np.random.RandomState(seed=42)
-
-
-try:
-    from modin.config import NPartitions
-
-    NPARTITIONS = NPartitions.get()
-except ImportError:
-    NPARTITIONS = pd.DEFAULT_NPARTITIONS
-
-try:
-    from modin.config import TestDatasetSize, AsvImplementation, Engine
-
-    ASV_USE_IMPL = AsvImplementation.get()
-    ASV_DATASET_SIZE = TestDatasetSize.get() or "Small"
-    ASV_USE_ENGINE = Engine.get()
-except ImportError:
-    # The same benchmarking code can be run for different versions of Modin, so in
-    # case of an error importing important variables, we'll just use predefined values
-    ASV_USE_IMPL = os.environ.get("MODIN_ASV_USE_IMPL", "modin")
-    ASV_DATASET_SIZE = os.environ.get("MODIN_TEST_DATASET_SIZE", "Small")
-    ASV_USE_ENGINE = os.environ.get("MODIN_ENGINE", "Ray")
-
-assert ASV_USE_IMPL in ("modin", "pandas")
-
-BINARY_OP_DATA_SIZE = {
-    "Big": [
-        ((5000, 5000), (5000, 5000)),
-        # the case extremely inefficient
-        # ((20, 500_000), (10, 1_000_000)),
-        ((500_000, 20), (1_000_000, 10)),
-    ],
-    "Small": [
-        ((250, 250), (250, 250)),
-        ((20, 10_000), (10, 25_000)),
-        ((10_000, 20), (25_000, 10)),
-    ],
-}
-
-UNARY_OP_DATA_SIZE = {
-    "Big": [
-        (5000, 5000),
-        # the case extremely inefficient
-        # (10, 1_000_000),
-        (1_000_000, 10),
-    ],
-    "Small": [
-        (250, 250),
-        (10, 10_000),
-        (10_000, 10),
-    ],
-}
-
-GROUPBY_NGROUPS = {
-    "Big": [100, "huge_amount_groups"],
-    "Small": [5],
-}
-
-IMPL = {
-    "modin": pd,
-    "pandas": pandas,
-}
-
-
-def translator_groupby_ngroups(groupby_ngroups, shape):
-    if ASV_DATASET_SIZE == "Big":
-        if groupby_ngroups == "huge_amount_groups":
-            return min(shape[0] // 2, 5000)
-        return groupby_ngroups
-    else:
-        return groupby_ngroups
-
-
-class weakdict(dict):
-    __slots__ = ("__weakref__",)
-
+from modin.engines.base.frame.axis_partition import BaseFrameAxisPartition
+from .partition import PyarrowOnRayFramePartition
 
-data_cache = dict()
-dataframes_cache = dict()
+import ray
+import pyarrow
 
 
-def gen_int_data(nrows, ncols, rand_low, rand_high):
-    cache_key = ("int", nrows, ncols, rand_low, rand_high)
-    if cache_key in data_cache:
-        return data_cache[cache_key]
-
-    logging.info(
-        "Generating int data {} rows and {} columns [{}-{}]".format(
-            nrows, ncols, rand_low, rand_high
-        )
-    )
-    data = {
-        "col{}".format(i): random_state.randint(rand_low, rand_high, size=(nrows))
-        for i in range(ncols)
-    }
-    data_cache[cache_key] = weakdict(data)
-    return data
-
-
-def gen_str_int_data(nrows, ncols, rand_low, rand_high):
-    cache_key = ("str_int", nrows, ncols, rand_low, rand_high)
-    if cache_key in data_cache:
-        return data_cache[cache_key]
-
-    logging.info(
-        "Generating str_int data {} rows and {} columns [{}-{}]".format(
-            nrows, ncols, rand_low, rand_high
+class PyarrowOnRayFrameAxisPartition(BaseFrameAxisPartition):
+    def __init__(self, list_of_blocks):
+        # Unwrap from BaseFramePartition object for ease of use
+        self.list_of_blocks = [obj.oid for obj in list_of_blocks]
+
+    def apply(self, func, num_splits=None, other_axis_partition=None, **kwargs):
+        """Applies func to the object in the plasma store.
+
+        See notes in Parent class about this method.
+
+        Args:
+            func: The function to apply.
+            num_splits: The number of times to split the result object.
+            other_axis_partition: Another `PyarrowOnRayFrameAxisPartition` object to apply to
+                func with this one.
+
+        Returns:
+            A list of `RayRemotePartition` objects.
+        """
+        if num_splits is None:
+            num_splits = len(self.list_of_blocks)
+
+        if other_axis_partition is not None:
+            return [
+                PyarrowOnRayFramePartition(obj)
+                for obj in deploy_ray_func_between_two_axis_partitions._remote(
+                    args=(self.axis, func, num_splits, len(self.list_of_blocks), kwargs)
+                    + tuple(self.list_of_blocks + other_axis_partition.list_of_blocks),
+                    num_returns=num_splits,
+                )
+            ]
+
+        args = [self.axis, func, num_splits, kwargs]
+        args.extend(self.list_of_blocks)
+        return [
+            PyarrowOnRayFramePartition(obj)
+            for obj in deploy_ray_axis_func._remote(args, num_returns=num_splits)
+        ]
+
+    def shuffle(self, func, num_splits=None, **kwargs):
+        """Shuffle the order of the data in this axis based on the `func`.
+
+        Extends `BaseFrameAxisPartition.shuffle`.
+
+        :param func:
+        :param num_splits:
+        :param kwargs:
+        :return:
+        """
+        if num_splits is None:
+            num_splits = len(self.list_of_blocks)
+
+        args = [self.axis, func, num_splits, kwargs]
+        args.extend(self.list_of_blocks)
+        return [
+            PyarrowOnRayFramePartition(obj)
+            for obj in deploy_ray_axis_func._remote(args, num_returns=num_splits)
+        ]
+
+
+class PyarrowOnRayFrameColumnPartition(PyarrowOnRayFrameAxisPartition):
+    """The column partition implementation for Ray. All of the implementation
+    for this class is in the parent class, and this class defines the axis
+    to perform the computation over.
+    """
+
+    axis = 0
+
+
+class PyarrowOnRayFrameRowPartition(PyarrowOnRayFrameAxisPartition):
+    """The row partition implementation for Ray. All of the implementation
+    for this class is in the parent class, and this class defines the axis
+    to perform the computation over.
+    """
+
+    axis = 1
+
+
+def concat_arrow_table_partitions(axis, partitions):
+    if axis == 0:
+        table = pyarrow.Table.from_batches(
+            [part.to_batches(part.num_rows)[0] for part in partitions]
         )
+    else:
+        table = partitions[0].drop([partitions[0].columns[-1].name])
+        for obj in partitions[1:]:
+            i = 0
+            for col in obj.itercolumns():
+                if i < obj.num_columns - 1:
+                    table = table.append_column(col)
+                i += 1
+        table = table.append_column(partitions[0].columns[-1])
+    return table
+
+
+def split_arrow_table_result(axis, result, num_partitions, num_splits, metadata):
+    chunksize = (
+        num_splits // num_partitions
+        if num_splits % num_partitions == 0
+        else num_splits // num_partitions + 1
     )
-    data = gen_int_data(nrows, ncols, rand_low, rand_high).copy()
-    data["gb_col"] = [
-        "str_{}".format(random_state.randint(rand_low, rand_high)) for i in range(nrows)
-    ]
-    data_cache[cache_key] = weakdict(data)
-    return data
-
-
-def gen_data(data_type, nrows, ncols, rand_low, rand_high):
-    if data_type == "int":
-        return gen_int_data(nrows, ncols, rand_low, rand_high)
-    elif data_type == "str_int":
-        return gen_str_int_data(nrows, ncols, rand_low, rand_high)
+    if axis == 0:
+        return [
+            pyarrow.Table.from_batches([part]) for part in result.to_batches(chunksize)
+        ]
     else:
-        assert False
+        return [
+            result.drop(
+                [
+                    result.columns[i].name
+                    for i in range(result.num_columns)
+                    if i >= n * chunksize or i < (n - 1) * chunksize
+                ]
+            )
+            .append_column(result.columns[-1])
+            .replace_schema_metadata(metadata=metadata)
+            for n in range(1, num_splits)
+        ] + [
+            result.drop(
+                [
+                    result.columns[i].name
+                    for i in range(result.num_columns)
+                    if i < (num_splits - 1) * chunksize
+                ]
+            ).replace_schema_metadata(metadata=metadata)
+        ]
+
+
+@ray.remote
+def deploy_ray_axis_func(axis, func, num_splits, kwargs, *partitions):
+    """Deploy a function along a full axis in Ray.
+
+    Args:
+        axis: The axis to perform the function along.
+        func: The function to perform.
+        num_splits: The number of splits to return
+            (see `split_result_of_axis_func_pandas`)
+        kwargs: A dictionary of keyword arguments.
+        partitions: All partitions that make up the full axis (row or column)
+
+    Returns:
+        A list of Pandas DataFrames.
+    """
+    table = concat_arrow_table_partitions(axis, partitions)
+    try:
+        result = func(table, **kwargs)
+    except Exception:
+        result = pyarrow.Table.from_pandas(func(table.to_pandas(), **kwargs))
+    return split_arrow_table_result(
+        axis, result, len(partitions), num_splits, table.schema.metadata
+    )
 
 
-def generate_dataframe(
-    impl,
-    data_type,
-    nrows,
-    ncols,
-    rand_low,
-    rand_high,
-    groupby_ncols=None,
-    count_groups=None,
+@ray.remote
+def deploy_ray_func_between_two_axis_partitions(
+    axis, func, num_splits, len_of_left, kwargs, *partitions
 ):
-    assert not (
-        (groupby_ncols is None) ^ (count_groups is None)
-    ), "You must either specify both parameters 'groupby_ncols' and 'count_groups' or none of them."
-
-    if groupby_ncols and count_groups:
-        ncols -= groupby_ncols
-        cache_key = (
-            impl,
-            data_type,
-            nrows,
-            ncols,
-            rand_low,
-            rand_high,
-            groupby_ncols,
-            count_groups,
-        )
-    else:
-        cache_key = (impl, data_type, nrows, ncols, rand_low, rand_high)
-
-    if cache_key in dataframes_cache:
-        return dataframes_cache[cache_key]
+    """Deploy a function along a full axis between two data sets in Ray.
 
-    logging.info(
-        "Allocating {} DataFrame {}: {} rows and {} columns [{}-{}]".format(
-            impl, data_type, nrows, ncols, rand_low, rand_high
-        )
+    Args:
+        axis: The axis to perform the function along.
+        func: The function to perform.
+        num_splits: The number of splits to return
+            (see `split_result_of_axis_func_pandas`).
+        len_of_left: The number of values in `partitions` that belong to the
+            left data set.
+        kwargs: A dictionary of keyword arguments.
+        partitions: All partitions that make up the full axis (row or column)
+            for both data sets.
+
+    Returns:
+        A list of Pandas DataFrames.
+    """
+    lt_table = concat_arrow_table_partitions(axis, partitions[:len_of_left])
+    rt_table = concat_arrow_table_partitions(axis, partitions[len_of_left:])
+    try:
+        result = func(lt_table, rt_table, **kwargs)
+    except Exception:
+        lt_frame = lt_table.from_pandas()
+        rt_frame = rt_table.from_pandas()
+        result = pyarrow.Table.from_pandas(func(lt_frame, rt_frame, **kwargs))
+    return split_arrow_table_result(
+        axis, result, len(result.num_rows), num_splits, result.schema.metadata
     )
-    data = gen_data(data_type, nrows, ncols, rand_low, rand_high)
-
-    if groupby_ncols and count_groups:
-        groupby_columns = [f"groupby_col{x}" for x in range(groupby_ncols)]
-        for groupby_col in groupby_columns:
-            data[groupby_col] = np.tile(np.arange(count_groups), nrows // count_groups)
-
-    if impl == "modin":
-        df = pd.DataFrame(data)
-    elif impl == "pandas":
-        df = pandas.DataFrame(data)
-    else:
-        assert False
-
-    if groupby_ncols and count_groups:
-        dataframes_cache[cache_key] = df, groupby_columns
-        return df, groupby_columns
-
-    dataframes_cache[cache_key] = df
-    return df
-
-
-def random_string():
-    return str(uuid.uuid1())
-
-
-def random_columns(df_columns, columns_number):
-    return list(random_state.choice(df_columns, size=columns_number))
-
-
-def random_booleans(number):
-    return list(random_state.choice([True, False], size=number))
-
-
-def execute(df):
-    "Make sure the calculations are done."
-    if ASV_USE_IMPL == "modin":
-        partitions = df._query_compiler._modin_frame._partitions
-        map(lambda partition: partition.drain_call_queue(), partitions)
-        if ASV_USE_ENGINE == "Ray":
-            from ray import wait
-
-            map(lambda partition: wait(partition.oid), partitions)
-        elif ASV_USE_ENGINE == "Dask":
-            from dask.distributed import wait
-
-            map(lambda partition: wait(partition.future), partitions)
-        elif ASV_USE_ENGINE == "Python":
-            pass
-
-    elif ASV_USE_IMPL == "pandas":
-        pass
-    else:
-        raise ValueError(f"wrong value of {ASV_USE_IMPL}")
 
 
-def get_shape_id(array):
-    return "_".join([str(element) for element in array])
+@ray.remote
+def deploy_ray_shuffle_func(axis, func, numsplits, kwargs, *partitions):
+    """Deploy a function that defines the partitions along this axis.
+
+    Args:
+        axis:
+        func:
+        numsplits:
+        kwargs:
+        partitions:
+
+    Returns:
+        A list of Pandas DataFrames.
+    """
+    pass
```

### Comparing `modin-0.9.0/asv_bench/benchmarks/scalability/scalability_benchmarks.py` & `modin-0.9.1/modin/data_management/functions/default_methods/binary_default.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,58 +7,38 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 
-import modin.pandas as pd
-from modin.pandas.utils import from_pandas
-from modin.utils import to_pandas
+from .any_default import AnyDefault
+
 import pandas
+from pandas.core.dtypes.common import is_list_like
+
+
+class BinaryDefault(AnyDefault):
+    @classmethod
+    def build_default_to_pandas(cls, fn, fn_name):
+        def bin_ops_wrapper(df, other, *args, **kwargs):
+            squeeze_other = kwargs.pop("broadcast", False) or kwargs.pop(
+                "squeeze_other", False
+            )
+            squeeze_self = kwargs.pop("squeeze_self", False)
+
+            if squeeze_other:
+                other = other.squeeze(axis=1)
+
+            if squeeze_self:
+                df = df.squeeze(axis=1)
+
+            result = fn(df, other, *args, **kwargs)
+            if (
+                not isinstance(result, pandas.Series)
+                and not isinstance(result, pandas.DataFrame)
+                and is_list_like(result)
+            ):
+                result = pandas.DataFrame(result)
+            return result
 
-from ..utils import (
-    gen_data,
-    generate_dataframe,
-    RAND_LOW,
-    RAND_HIGH,
-    ASV_DATASET_SIZE,
-    UNARY_OP_DATA_SIZE,
-    execute,
-)
-
-
-class TimeFromPandas:
-    param_names = ["shape", "cpus"]
-    params = [
-        UNARY_OP_DATA_SIZE[ASV_DATASET_SIZE],
-        [4, 16, 32],
-    ]
-
-    def setup(self, shape, cpus):
-        self.data = pandas.DataFrame(gen_data("int", *shape, RAND_LOW, RAND_HIGH))
-        from modin.config import NPartitions
-
-        NPartitions.get = lambda: cpus
-        # trigger ray init
-        pd.DataFrame([])
-
-    def time_from_pandas(self, shape, cpus):
-        execute(from_pandas(self.data))
-
-
-class TimeToPandas:
-    param_names = ["shape", "cpus"]
-    params = [
-        UNARY_OP_DATA_SIZE[ASV_DATASET_SIZE],
-        [4, 16, 32],
-    ]
-
-    def setup(self, shape, cpus):
-        from modin.config import NPartitions
-
-        NPartitions.get = lambda: cpus
-        self.data = generate_dataframe("modin", "int", *shape, RAND_LOW, RAND_HIGH)
-
-    def time_to_pandas(self, shape, cpus):
-        # to_pandas is already synchronous
-        to_pandas(self.data)
+        return super().build_default_to_pandas(bin_ops_wrapper, fn_name)
```

### Comparing `modin-0.9.0/asv_bench/benchmarks/scalability/__init__.py` & `modin-0.9.1/modin/data_management/factories/test/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/README.md` & `modin-0.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <h2 align="center">Scale your pandas workflows by changing one line of code</h2>
 
 <p align="center">
 <a href="https://discuss.modin.org"><img alt="" src="https://img.shields.io/badge/discourse-forum-purple.svg?logo=discourse&logoColor=white" align="center"></a>
 <a href="https://codecov.io/gh/modin-project/modin"><img src="https://codecov.io/gh/modin-project/modin/branch/master/graph/badge.svg" align="center"/></a>
 <a href="https://github.com/modin-project/modin/actions"><img src="https://github.com/modin-project/modin/workflows/master/badge.svg" align="center"></a>
 <a href="https://modin.readthedocs.io/en/latest/?badge=latest"><img alt="" src="https://readthedocs.org/projects/modin/badge/?version=latest" align="center"></a>
-<a href="https://pypi.org/project/modin/"><img alt="" src="https://img.shields.io/badge/pypi-0.9.0-blue.svg" align="center"></a>
+<a href="https://pypi.org/project/modin/"><img alt="" src="https://img.shields.io/badge/pypi-0.9.1-blue.svg" align="center"></a>
 </p>
 
 <p align="center"><b>To use Modin, replace the pandas import:</b></p>
 
 ```python
 # import pandas as pd
 import modin.pandas as pd
```

### Comparing `modin-0.9.0/setup.py` & `modin-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/LICENSE_HEADER` & `modin-0.9.1/modin/distributed/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/examples/cluster/experimental_cloud.py` & `modin-0.9.1/modin/config/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,29 +7,20 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 
-"""
-This is a very basic sample script for running things remotely.
-It requires `aws_credentials` file to be present in current working directory.
+from . import *  # noqa: F403, F401
+from .pubsub import Parameter
 
-On credentials file format see https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-files.html#cli-configure-files-where
-"""
 
-import logging
+def print_config_help():
+    for objname in sorted(globals()):
+        obj = globals()[objname]
+        if isinstance(obj, type) and issubclass(obj, Parameter) and not obj.is_abstract:
+            print(f"{obj.get_help()}\n\tCurrent value: {obj.get()}")  # noqa: T001
 
-import modin.pandas as pd
-from modin.experimental.cloud import cluster
 
-# set up verbose logging so Ray autoscaler would print a lot of things
-# and we'll see that stuff is alive and kicking
-logging.basicConfig(format="%(asctime)s %(message)s")
-logger = logging.getLogger()
-logger.setLevel(logging.DEBUG)
-
-example_cluster = cluster.create("aws", "aws_credentials")
-with example_cluster:
-    remote_df = pd.DataFrame([1, 2, 3, 4])
-    print(len(remote_df))  # len() is executed remotely
+if __name__ == "__main__":
+    print_config_help()
```

### Comparing `modin-0.9.0/examples/cluster/mortgage-runner.py` & `modin-0.9.1/modin/experimental/pandas/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,44 +7,24 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 
+from modin.config import IsExperimental
 
-# pip install git+https://github.com/intel-ai/ibis.git@develop
-# pip install braceexpand
+IsExperimental.put(True)
 
-# NOTE: expects https://github.com/intel-ai/omniscripts checked out and in PYTHONPATH
-
-# the following import turns on experimental mode in Modin,
-# including enabling running things in remote cloud
-import modin.experimental.pandas as pd  # noqa: F401
-from modin.experimental.cloud import create_cluster
-
-from mortgage import run_benchmark
-
-test_cluster = create_cluster(
-    "aws",
-    "aws_credentials",
-    cluster_name="rayscale-test",
-    region="eu-north-1",
-    zone="eu-north-1b",
-    image="ami-00e1e82d7d4ca80d3",
+# import numpy_wrap as early as possible to intercept all "import numpy" statements
+# in the user code
+from .numpy_wrap import _CAUGHT_NUMPY  # noqa F401
+from modin.pandas import *  # noqa F401, F403
+from .io_exp import read_sql, read_csv_glob  # noqa F401
+import warnings
+
+
+warnings.warn(
+    "Thank you for using the Modin Experimental pandas API."
+    "\nPlease note that some of these APIs deviate from pandas in order to "
+    "provide improved performance."
 )
-with test_cluster:
-
-    parameters = {
-        "data_file": "https://modin-datasets.s3.amazonaws.com/mortgage",
-        # "data_file": "s3://modin-datasets/mortgage",
-        "dfiles_num": 1,
-        "no_ml": True,
-        "validation": False,
-        "no_ibis": True,
-        "no_pandas": False,
-        "pandas_mode": "Modin_on_ray",
-        "ray_tmpdir": "/tmp",
-        "ray_memory": 1024 * 1024 * 1024,
-    }
-
-    run_benchmark(parameters)
```

### Comparing `modin-0.9.0/examples/cluster/aws_example.yaml` & `modin-0.9.1/modin/experimental/cloud/ray-autoscaler.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # An unique identifier for the head node and workers of this cluster.
 cluster_name: default
 
 # The minimum number of workers nodes to launch in addition to the head
 # node. This number should be >= 0.
-min_workers: 0
+min_workers: 2
 
 # The maximum number of workers nodes to launch in addition to the head
 # node. This takes precedence over min_workers.
-max_workers: 5
+max_workers: 2
 
 # The initial number of worker nodes to launch in addition to the head
 # node. When the cluster is first brought up (or when it is refreshed with a
 # subsequent `ray up`) this number of nodes will be started.
 initial_workers: 2
 
+autoscaling_mode: aggressive
+
 # This executes all commands on all nodes in the docker container,
 # and opens all the necessary ports to support the Ray cluster.
 # Empty string means disabled.
 docker:
     image: "" # e.g., tensorflow/tensorflow:1.5.0-py3
     container_name: "" # e.g. ray_docker
     run_options: []  # Extra options to pass into "docker run"
@@ -31,27 +33,28 @@
     # worker_run_options: []
 
 # The autoscaler will scale up the cluster to this target fraction of resource
 # usage. For example, if a cluster of 10 nodes is 100% busy and
 # target_utilization is 0.8, it would resize the cluster to 13. This fraction
 # can be decreased to increase the aggressiveness of upscaling.
 # This value must be less than 1.0 for scaling to happen.
-target_utilization_fraction: 0.8
+target_utilization_fraction: 1.0
 
 # If a node is idle for this many minutes, it will be removed.
-idle_timeout_minutes: 5
+idle_timeout_minutes: 60
 
 # Cloud-provider specific configuration.
 provider:
     type: aws
     region: us-west-1
     # Availability zone(s), comma-separated, that nodes may be launched in.
     # Nodes are currently spread between zones by a round-robin approach,
     # however this implementation detail should not be relied upon.
-    availability_zone: us-west-1a,us-west-1b
+    availability_zone: us-west-1a,us-west-1c
+    # use_internal_ips: True
 
 # How Ray will authenticate with newly launched nodes.
 auth:
     ssh_user: ubuntu
 # By default Ray creates a new private keypair, but you can also use your own.
 # If you do so, make sure to also set "KeyName" in the head and worker node
 # configurations below.
@@ -59,35 +62,41 @@
 
 # Provider-specific config for the head node, e.g. instance type. By default
 # Ray will auto-configure unspecified fields such as SubnetId and KeyName.
 # For more documentation on available fields, see:
 # http://boto3.readthedocs.io/en/latest/reference/services/ec2.html#EC2.ServiceResource.create_instances
 head_node:
     InstanceType: m5.large
-    ImageId: ami-09c2435df1137686f # Deep Learning AMI
+    ImageId: ami-0f56279347d2fa43e
 
     # You can provision additional disk space with a conf as follows
     BlockDeviceMappings:
         - DeviceName: /dev/sda1
           Ebs:
-              VolumeSize: 75
+              VolumeSize: 40
 
+    # NetworkInterfaces:
+    #     - AssociatePublicIpAddress: True
     # Additional options in the boto docs.
 
 # Provider-specific config for worker nodes, e.g. instance type. By default
 # Ray will auto-configure unspecified fields such as SubnetId and KeyName.
 # For more documentation on available fields, see:
 # http://boto3.readthedocs.io/en/latest/reference/services/ec2.html#EC2.ServiceResource.create_instances
 worker_nodes:
     InstanceType: m5.large
-    ImageId: ami-09c2435df1137686f # Deep Learning AMI
+    ImageId: ami-0f56279347d2fa43e
 
+    BlockDeviceMappings:
+        - DeviceName: /dev/sda1
+          Ebs:
+              VolumeSize: 40
     # Run workers on spot by default. Comment this out to use on-demand.
-    InstanceMarketOptions:
-        MarketType: spot
+    # InstanceMarketOptions:
+    #    MarketType: spot
         # Additional options can be found in the boto docs, e.g.
         #   SpotOptions:
         #       MaxPrice: MAX_HOURLY_PRICE
 
     # Additional options in the boto docs.
 
 # Files or directories to copy to the head and worker nodes. The format is a
@@ -100,36 +109,64 @@
 # List of commands that will be run before `setup_commands`. If docker is
 # enabled, these commands will run outside the container and before docker
 # is setup.
 initialization_commands: []
 
 # List of shell commands to run to set up nodes.
 setup_commands:
-    - pip install s3fs
-    - pip install modin
-    - echo 'export MODIN_RAY_CLUSTER=True' >> ~/.bashrc
+    - |
+        wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh -O ~/miniconda.sh
+        bash ~/miniconda.sh -b -p ~/miniconda -f -u
+        $HOME/miniconda/bin/conda init bash
+        source ~/.bashrc
+        conda create --name modin --yes
+        conda activate modin
+        conda install --yes -c intel/label/modin -c conda-forge {{CONDA_PACKAGES}}
+
+        pip install colorful cloudpickle
+        # ray now executes "ray stop" which expects "ray" to be in $PATH
+        # so place a symlink to current "ray" binary to /usr/local/bin
+        sudo ln -s `which ray` /usr/local/bin/ray
+        echo 'export MODIN_RAY_CLUSTER=True' >> ~/.bashrc
+
     # Consider uncommenting these if you also want to run apt-get commands during setup
     # - sudo pkill -9 apt-get || true
     # - sudo pkill -9 dpkg || true
     # - sudo dpkg --configure -a
 
 # Custom commands that will be run on the head node after common setup.
 head_setup_commands:
-    - pip install boto3==1.4.8  # 1.4.8 adds InstanceMarketOptions
-    - echo 'export MODIN_REDIS_ADDRESS="localhost:6379"' >> ~/.bashrc
+    - |
+        source ~/.bashrc
+        conda activate modin
+        echo 'export MODIN_REDIS_ADDRESS="localhost:6379"' >> ~/.bashrc
 
 # Custom commands that will be run on worker nodes after common setup.
 worker_setup_commands: []
 
 # Command to start ray on the head node. You don't need to change this.
 head_start_ray_commands:
-    - ray stop
-    - echo 'export MEMORY_STORE_SIZE=$(awk "/MemFree/ { printf \"%d \\n\", \$2*1024}" /proc/meminfo)' >> ~/.bashrc
-    - echo 'export TMPDIR="$(dirname $(mktemp tmp.XXXXXXXXXX -ut))"' >> ~/.bashrc
-    - ulimit -n 65536; ray start --head --redis-port=6379 --object-manager-port=8076 --autoscaling-config=~/ray_bootstrap_config.yaml --object-store-memory=$MEMORY_STORE_SIZE --plasma-directory=$TMPDIR
+    - |
+        source ~/.bashrc
+        conda activate modin
+        ray stop
+
+        export MEMORY_STORE_SIZE=$(awk "/MemFree/ { printf \"%d \\n\", \$2*1024*0.8}" /proc/meminfo)
+        export TMPDIR="$(dirname $(mktemp tmp.XXXXXXXXXX -ut))"
+        echo 'export MEMORY_STORE_SIZE=$(awk "/MemFree/ { printf \"%d \\n\", \$2*1024*0.8}" /proc/meminfo)' >> ~/.bashrc
+        echo 'export TMPDIR="$(dirname $(mktemp tmp.XXXXXXXXXX -ut))"' >> ~/.bashrc
+
+        ulimit -n 65536; ray start --head --redis-shard-ports=6380 --port=6379 --object-manager-port=8076 --autoscaling-config=~/ray_bootstrap_config.yaml --object-store-memory=$MEMORY_STORE_SIZE --plasma-directory=$TMPDIR
 
 # Command to start ray on worker nodes. You don't need to change this.
 worker_start_ray_commands:
-    - ray stop
-    - echo 'export MEMORY_STORE_SIZE=$(awk "/MemFree/ { printf \"%d \\n\", \$2*1024}" /proc/meminfo)' >> ~/.bashrc
-    - echo 'export TMPDIR="$(dirname $(mktemp tmp.XXXXXXXXXX -ut))"' >> ~/.bashrc
-    - ulimit -n 65536; ray start --redis-address=$RAY_HEAD_IP:6379 --object-manager-port=8076 --object-store-memory=$MEMORY_STORE_SIZE --plasma-directory=$TMPDIR
+    - |
+        source ~/.bashrc
+        conda activate modin
+        ray stop
+
+        export MEMORY_STORE_SIZE=$(awk "/MemFree/ { printf \"%d \\n\", \$2*1024*0.8}" /proc/meminfo)
+        export TMPDIR="$(dirname $(mktemp tmp.XXXXXXXXXX -ut))"
+        echo 'export MEMORY_STORE_SIZE=$(awk "/MemFree/ { printf \"%d \\n\", \$2*1024*0.8}" /proc/meminfo)' >> ~/.bashrc
+        echo 'export TMPDIR="$(dirname $(mktemp tmp.XXXXXXXXXX -ut))"' >> ~/.bashrc
+
+        ulimit -n 65536; ray start --address=$RAY_HEAD_IP:6379 --object-manager-port=8076 --object-store-memory=$MEMORY_STORE_SIZE --plasma-directory=$TMPDIR
```

### Comparing `modin-0.9.0/examples/cluster/h2o-runner.py` & `modin-0.9.1/modin/experimental/cloud/omnisci.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,45 +7,40 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 
+import warnings
 
-# pip install git+https://github.com/intel-ai/ibis.git@develop
-# pip install braceexpand
+from .rayscale import RayCluster
+from .cluster import Provider
 
-# NOTE: expects https://github.com/intel-ai/omniscripts checked out and in PYTHONPATH
 
-# the following import turns on experimental mode in Modin,
-# including enabling running things in remote cloud
-import modin.experimental.pandas as pd  # noqa: F401
-from modin.experimental.cloud import create_cluster
-
-from h2o import run_benchmark
-
-test_cluster = create_cluster(
-    "aws",
-    "aws_credentials",
-    cluster_name="rayscale-test",
-    region="eu-north-1",
-    zone="eu-north-1b",
-    image="ami-00e1e82d7d4ca80d3",
-)
-with test_cluster:
-    parameters = {
-        "no_pandas": False,
-        "pandas_mode": "Modin_on_ray",
-        "ray_tmpdir": "/tmp",
-        "ray_memory": 1024 * 1024 * 1024,
-        "extended_functionality": False,
-    }
-
-    # G1... - for groupby queries; J1... - for join queries;
-    # Additional required files inside h2o-data folder:
-    # - J1_1e6_1e0_0_0.csv
-    # - J1_1e6_1e3_0_0.csv
-    # - J1_1e6_1e6_0_0.csv
-    for data_file in ["G1_5e5_1e2_0_0.csv", "J1_1e6_NA_0_0.csv"]:
-        parameters["data_file"] = f"https://modin-datasets.s3.amazonaws.com/h2o/{data_file}"
-        run_benchmark(parameters)
+class RemoteOmnisci(RayCluster):
+    target_engine = "Cloudray"
+    target_partition = "Omnisci"
+
+    def __init__(
+        self,
+        provider: Provider,
+        project_name: str = None,
+        cluster_name: str = "modin-cluster",
+        worker_count: int = 0,
+        head_node_type: str = None,
+        worker_node_type: str = None,
+        add_conda_packages: list = None,
+    ):
+        if worker_count != 0:
+            warnings.warn(
+                "Current Omnisci on cloud does not support multi-node setups, not requesting worker nodes"
+            )
+        super().__init__(
+            provider,
+            project_name,
+            cluster_name,
+            0,
+            head_node_type,
+            worker_node_type,
+            add_conda_packages,
+        )
```

### Comparing `modin-0.9.0/examples/docker/census-on-omnisci/build-docker-image.sh` & `modin-0.9.1/modin/test/test_envvar_catcher.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,32 @@
-#!/bin/bash -e
-
 # Licensed to Modin Development Team under one or more contributor license agreements.
 # See the NOTICE file distributed with this work for additional information regarding
 # copyright ownership.  The Modin Development Team licenses this file to you under the
 # Apache License, Version 2.0 (the "License"); you may not use this file except in
 # compliance with the License.  You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 
-echo "Note: a user is responsible for preparing the dataset.
-The dataset must be named as 'ipums_education2income_1970-2010.csv' and
-be in the folder with 'census-omnisci.dockerfile'. It can be downloaded by link:
-'https://rapidsai-data.s3.us-east-2.amazonaws.com/datasets/ipums_education2income_1970-2010.csv.gz'"
+import os
+import pytest
+
+
+@pytest.fixture
+def nameset():
+    name = "hey_i_am_an_env_var"
+    os.environ[name] = "i am a value"
+    yield name
+    del os.environ[name]
 
-cd "`dirname \"$0\"`"
 
-docker build -f census-omnisci.dockerfile -t census-omnisci --build-arg no_proxy \
-    --build-arg https_proxy --build-arg http_proxy --build-arg conda_extra_channel .
-printf "\n\nTo run the benchmark execute:\n\tdocker run --rm census-omnisci\n"
+def test_envvar_catcher(nameset):
+    with pytest.raises(AssertionError):
+        os.environ.get("Modin_FOO", "bar")
+    with pytest.raises(AssertionError):
+        "modin_qux" not in os.environ
+    assert "yay_random_name" not in os.environ
+    assert os.environ[nameset]
```

### Comparing `modin-0.9.0/examples/docker/taxi-on-omnisci/build-docker-image.sh` & `modin-0.9.1/modin/experimental/xgboost/test/test_default.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,30 @@
-#!/bin/bash -e
-
 # Licensed to Modin Development Team under one or more contributor license agreements.
 # See the NOTICE file distributed with this work for additional information regarding
 # copyright ownership.  The Modin Development Team licenses this file to you under the
 # Apache License, Version 2.0 (the "License"); you may not use this file except in
 # compliance with the License.  You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 
-echo "Note: a user is responsible for preparing the dataset.
-The dataset must be named as 'trips_xaa.csv' and be in the folder with 'nyc-taxi-omnisci.dockerfile'.
-It Can be generated by following the instructions on the link:
-'https://github.com/toddwschneider/nyc-taxi-data#instructions'"
 
-cd "`dirname \"$0\"`"
+import pytest
+from modin.config import Engine
+
+import modin.experimental.xgboost as xgb
+import modin.pandas as pd
+
 
-docker build -f nyc-taxi-omnisci.dockerfile -t nyc-taxi-omnisci --build-arg https_proxy --build-arg http_proxy .
-printf "\n\nTo run the benchmark execute:\n\tdocker run --rm nyc-taxi-omnisci\n"
+@pytest.mark.skipif(
+    Engine.get() == "Ray",
+    reason="This test doesn't make sense on Ray backend.",
+)
+def test_backend():
+    try:
+        xgb.train({}, xgb.DMatrix(pd.DataFrame([0]), pd.DataFrame([0])))
+    except ValueError:
+        pass
```

### Comparing `modin-0.9.0/examples/docker/build.sh` & `modin-0.9.1/modin/config/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,15 @@
-#!/bin/bash -e
-
 # Licensed to Modin Development Team under one or more contributor license agreements.
 # See the NOTICE file distributed with this work for additional information regarding
 # copyright ownership.  The Modin Development Team licenses this file to you under the
 # Apache License, Version 2.0 (the "License"); you may not use this file except in
 # compliance with the License.  You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 
-cd "`dirname \"$0\"`"
-
-docker build -f nyc-taxi.dockerfile -t nyc-taxi --build-arg https_proxy --build-arg http_proxy .
-printf "\n\nTo run the benchmark execute:\n\tdocker run --rm nyc-taxi\n"
+from .pubsub import Parameter  # noqa: F401
+from .envvars import *  # noqa: F403, F401
```

### Comparing `modin-0.9.0/modin/experimental/xgboost/test/__init__.py` & `modin-0.9.1/modin/distributed/dataframe/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/xgboost/test/test_default.py` & `modin-0.9.1/modin/data_management/functions/function.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,24 +7,29 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 
+from typing import Optional
 
-import pytest
-from modin.config import Engine
 
-import modin.experimental.xgboost as xgb
+class Function(object):
+    def __init__(self):
+        raise ValueError(
+            "Please use {}.register instead of the constructor".format(
+                type(self).__name__
+            )
+        )
 
+    @classmethod
+    def call(cls, func, **call_kwds):
+        raise NotImplementedError("Please implement in child class")
 
-@pytest.mark.skipif(
-    Engine.get() == "Ray",
-    reason="This test doesn't make sense on Ray backend.",
-)
-@pytest.mark.parametrize("func", ["train", "predict"])
-def test_backend(func):
-    try:
-        getattr(xgb, func)({}, xgb.ModinDMatrix(None, None))
-    except ValueError:
-        pass
+    @classmethod
+    def register(cls, func, **kwargs):
+        return cls.call(func, **kwargs)
+
+    @classmethod
+    def validate_axis(cls, axis: Optional[int]) -> int:
+        return 0 if axis is None else axis
```

### Comparing `modin-0.9.0/modin/experimental/xgboost/__init__.py` & `modin-0.9.1/modin/experimental/xgboost/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,10 +7,10 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 
-from .xgboost import ModinDMatrix, train, predict
+from .xgboost import DMatrix, Booster, train
 
-__all__ = ["ModinDMatrix", "train", "predict"]
+__all__ = ["DMatrix", "Booster", "train"]
```

### Comparing `modin-0.9.0/modin/experimental/xgboost/utils.py` & `modin-0.9.1/modin/experimental/xgboost/utils.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/xgboost/xgboost_ray.py` & `modin-0.9.1/modin/experimental/xgboost/xgboost_ray.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/xgboost/xgboost.py` & `modin-0.9.1/modin/experimental/xgboost/xgboost.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,129 +15,153 @@
 import logging
 from typing import Dict, Optional
 from multiprocessing import cpu_count
 
 import xgboost as xgb
 
 from modin.config import Engine
+import modin.pandas as pd
 
 LOGGER = logging.getLogger("[modin.xgboost]")
 
 
-class ModinDMatrix(xgb.DMatrix):
+class DMatrix(xgb.DMatrix):
     """
     DMatrix holding on references to DataFrame.
 
     Parameters
     ----------
     data : DataFrame
         Data source of DMatrix.
     label : DataFrame
         Labels used for training.
 
     Notes
     -----
-    Currently ModinDMatrix supports only `data` and `label` parameters.
+    Currently DMatrix supports only `data` and `label` parameters.
     """
 
     def __init__(self, data, label):
+        assert isinstance(
+            data, pd.DataFrame
+        ), f"Type of `data` is {type(data)}, but expected {pd.DataFrame}."
+        assert isinstance(
+            label, (pd.DataFrame, pd.Series)
+        ), f"Type of `data` is {type(label)}, but expected {pd.DataFrame} or {pd.Series}."
+
         self.data = data
         self.label = label
 
     def __iter__(self):
         yield self.data
         yield self.label
 
 
+class Booster(xgb.Booster):
+    """
+    A Modin Booster of XGBoost.
+
+    Booster is the model of xgboost, that contains low level routines for
+    training, prediction and evaluation.
+
+    Parameters
+    ----------
+    params : dict. Default is None
+        Parameters for boosters.
+    cache : list
+        List of cache items.
+    model_file : string/os.PathLike/Booster/bytearray
+        Path to the model file if it's string or PathLike.
+    """
+
+    def __init__(self, params=None, cache=(), model_file=None):
+        super(Booster, self).__init__(params=params, cache=cache, model_file=model_file)
+
+    def predict(
+        self,
+        data: DMatrix,
+        nthread: Optional[int] = cpu_count(),
+        **kwargs,
+    ):
+        """
+        Run prediction with a trained booster.
+
+        Parameters
+        ----------
+        data : DMatrix
+            Input data used for prediction.
+        nthread : int. Default is number of threads on master node
+            Number of threads for using in each node.
+        \\*\\*kwargs :
+            Other parameters are the same as `xgboost.Booster.predict`.
+
+        Returns
+        -------
+        ``modin.pandas.DataFrame``
+            Modin DataFrame with prediction results.
+        """
+        LOGGER.info("Prediction started")
+
+        if Engine.get() == "Ray":
+            from .xgboost_ray import _predict
+        else:
+            raise ValueError("Current version supports only Ray engine.")
+
+        assert isinstance(
+            data, DMatrix
+        ), f"Type of `data` is {type(data)}, but expected {DMatrix}."
+
+        result = _predict(self.copy(), data, nthread, **kwargs)
+        LOGGER.info("Prediction finished")
+
+        return result
+
+
 def train(
     params: Dict,
-    dtrain: ModinDMatrix,
+    dtrain: DMatrix,
     *args,
     evals=(),
     nthread: Optional[int] = cpu_count(),
+    evals_result: Optional[Dict] = None,
     **kwargs,
 ):
     """
     Train XGBoost model.
 
     Parameters
     ----------
     params : dict
         Booster params.
-    dtrain : ModinDMatrix
+    dtrain : DMatrix
         Data to be trained against.
-    evals: list of pairs (ModinDMatrix, string)
+    evals: list of pairs (DMatrix, string)
         List of validation sets for which metrics will evaluated during training.
         Validation metrics will help us track the performance of the model.
     nthread : int. Default is number of threads on master node
         Number of threads for using in each node.
+    evals_result : dict. Default is None
+        Dict to store evaluation results in.
     \\*\\*kwargs :
-        Other parameters are the same as `xgboost.train` except for
-        `evals_result`, which is returned as part of function return value
-        instead of argument.
+        Other parameters are the same as `xgboost.train`.
 
     Returns
     -------
-    dict
-        A dictionary containing trained booster and evaluation history.
-        `history` field is the same as `eval_result` from `xgboost.train`.
-
-        .. code-block:: python
-
-            {'booster': xgboost.Booster,
-             'history': {'train': {'logloss': ['0.48253', '0.35953']},
-                         'eval': {'logloss': ['0.480385', '0.357756']}}}
+    ``modin.experimental.xgboost.Booster``
+        A trained booster.
     """
     LOGGER.info("Training started")
 
     if Engine.get() == "Ray":
         from .xgboost_ray import _train
     else:
         raise ValueError("Current version supports only Ray engine.")
 
+    assert isinstance(
+        dtrain, DMatrix
+    ), f"Type of `dtrain` is {type(dtrain)}, but expected {DMatrix}."
     result = _train(dtrain, nthread, params, *args, evals=evals, **kwargs)
-    LOGGER.info("Training finished")
-    return result
-
-
-def predict(
-    model,
-    data: ModinDMatrix,
-    nthread: Optional[int] = cpu_count(),
-    **kwargs,
-):
-    """
-    Run prediction with a trained booster.
+    if isinstance(evals_result, dict):
+        evals_result.update(result["history"])
 
-    Parameters
-    ----------
-    model : A Booster or a dictionary returned by `modin.experimental.xgboost.train`
-        The trained model.
-    data : ModinDMatrix
-        Input data used for prediction.
-    nthread : int. Default is number of threads on master node
-        Number of threads for using in each node.
-
-    Returns
-    -------
-    modin.pandas.DataFrame
-        Modin DataFrame with prediction results.
-    """
-    LOGGER.info("Prediction started")
-
-    if Engine.get() == "Ray":
-        from .xgboost_ray import _predict
-    else:
-        raise ValueError("Current version supports only Ray engine.")
-
-    if isinstance(model, xgb.Booster):
-        booster = model
-    elif isinstance(model, dict):
-        booster = model["booster"]
-    else:
-        raise TypeError(
-            f"Expected types for `model` xgb.Booster or dict, but presented type is {type(model)}"
-        )
-    result = _predict(booster, data, nthread, **kwargs)
-    LOGGER.info("Prediction finished")
-
-    return result
+    LOGGER.info("Training finished")
+    return Booster(model_file=result["booster"])
```

### Comparing `modin-0.9.0/modin/experimental/backends/omnisci/query_compiler.py` & `modin-0.9.1/modin/experimental/backends/omnisci/query_compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,18 @@
     lazy_execution = True
 
     def __init__(self, frame, shape_hint=None):
         assert frame is not None
         self._modin_frame = frame
         self._shape_hint = shape_hint
 
+    def finalize():
+        # TODO: implement this for OmniSci backend
+        raise NotImplementedError()
+
     def to_pandas(self):
         return self._modin_frame.to_pandas()
 
     @classmethod
     def from_pandas(cls, df, data_cls):
         return cls(data_cls.from_pandas(df))
```

### Comparing `modin-0.9.0/modin/experimental/backends/omnisci/__init__.py` & `modin-0.9.1/modin/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/backends/__init__.py` & `modin-0.9.1/modin/engines/base/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/__init__.py` & `modin-0.9.1/modin/engines/base/frame/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/sklearn/__init__.py` & `modin-0.9.1/modin/engines/base/io/column_stores/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/sklearn/model_selection/__init__.py` & `modin-0.9.1/modin/experimental/sklearn/model_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/sklearn/model_selection/train_test_split.py` & `modin-0.9.1/modin/experimental/sklearn/model_selection/train_test_split.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/engines/pandas_on_ray/io_exp.py` & `modin-0.9.1/modin/experimental/engines/pandas_on_ray/io_exp.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/engines/pandas_on_ray/__init__.py` & `modin-0.9.1/modin/engines/base/io/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/engines/pandas_on_ray/sql.py` & `modin-0.9.1/modin/experimental/engines/pandas_on_ray/sql.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/engines/omnisci_on_ray/test/__init__.py` & `modin-0.9.1/modin/engines/base/io/text/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/engines/omnisci_on_ray/test/test_dataframe.py` & `modin-0.9.1/modin/experimental/engines/omnisci_on_ray/test/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/engines/omnisci_on_ray/io.py` & `modin-0.9.1/modin/experimental/engines/omnisci_on_ray/io.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/engines/omnisci_on_ray/__init__.py` & `modin-0.9.1/modin/engines/base/series/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/engines/omnisci_on_ray/frame/partition.py` & `modin-0.9.1/modin/experimental/engines/omnisci_on_ray/frame/partition.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,17 @@
         return obj.to_pandas()
 
     def get(self):
         if self.arrow_table is not None:
             return self.arrow_table
         return ray.get(self.oid)
 
+    def wait(self):
+        ray.wait([self.oid])
+
     @classmethod
     def put(cls, obj):
         return OmnisciOnRayFramePartition(
             object_id=ray.put(obj),
             length=len(obj.index),
             width=len(obj.columns),
         )
```

### Comparing `modin-0.9.0/modin/experimental/engines/omnisci_on_ray/frame/df_algebra.py` & `modin-0.9.1/modin/experimental/engines/omnisci_on_ray/frame/df_algebra.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/engines/omnisci_on_ray/frame/__init__.py` & `modin-0.9.1/modin/engines/dask/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/engines/omnisci_on_ray/frame/calcite_algebra.py` & `modin-0.9.1/modin/experimental/engines/omnisci_on_ray/frame/calcite_algebra.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/engines/omnisci_on_ray/frame/calcite_builder.py` & `modin-0.9.1/modin/experimental/engines/omnisci_on_ray/frame/calcite_builder.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/engines/omnisci_on_ray/frame/calcite_serializer.py` & `modin-0.9.1/modin/experimental/engines/omnisci_on_ray/frame/calcite_serializer.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/engines/omnisci_on_ray/frame/partition_manager.py` & `modin-0.9.1/modin/experimental/engines/omnisci_on_ray/frame/partition_manager.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/engines/omnisci_on_ray/frame/axis_partition.py` & `modin-0.9.1/modin/experimental/engines/omnisci_on_ray/frame/axis_partition.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/engines/omnisci_on_ray/frame/omnisci_worker.py` & `modin-0.9.1/modin/experimental/engines/omnisci_on_ray/frame/omnisci_worker.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/engines/omnisci_on_ray/frame/data.py` & `modin-0.9.1/modin/experimental/engines/omnisci_on_ray/frame/data.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/engines/omnisci_on_ray/frame/expr.py` & `modin-0.9.1/modin/experimental/engines/omnisci_on_ray/frame/expr.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/engines/__init__.py` & `modin-0.9.1/modin/engines/dask/pandas_on_dask/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/engines/pyarrow_on_ray/series/__init__.py` & `modin-0.9.1/modin/engines/dask/pandas_on_dask/frame/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/engines/pyarrow_on_ray/io.py` & `modin-0.9.1/modin/experimental/engines/pyarrow_on_ray/io.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/engines/pyarrow_on_ray/__init__.py` & `modin-0.9.1/modin/engines/dask/pandas_on_dask/series/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/engines/pyarrow_on_ray/frame/partition.py` & `modin-0.9.1/modin/experimental/engines/pyarrow_on_ray/frame/partition.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/engines/pyarrow_on_ray/frame/__init__.py` & `modin-0.9.1/modin/engines/python/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/engines/pyarrow_on_ray/frame/partition_manager.py` & `modin-0.9.1/modin/experimental/engines/pyarrow_on_ray/frame/partition_manager.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/engines/pyarrow_on_ray/frame/axis_partition.py` & `modin-0.9.1/modin/engines/ray/pandas_on_ray/frame/partition.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,215 +7,258 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 
-from modin.engines.base.frame.axis_partition import BaseFrameAxisPartition
-from .partition import PyarrowOnRayFramePartition
+import pandas
+
+from modin.data_management.utils import length_fn_pandas, width_fn_pandas
+from modin.engines.base.frame.partition import BaseFramePartition
+from modin.engines.ray.utils import handle_ray_task_error
 
 import ray
-import pyarrow
+from ray.worker import RayTaskError
+from ray.services import get_node_ip_address
 
 
-class PyarrowOnRayFrameAxisPartition(BaseFrameAxisPartition):
-    def __init__(self, list_of_blocks):
-        # Unwrap from BaseFramePartition object for ease of use
-        self.list_of_blocks = [obj.oid for obj in list_of_blocks]
+class PandasOnRayFramePartition(BaseFramePartition):
+    def __init__(self, object_id, length=None, width=None, ip=None, call_queue=None):
+        assert type(object_id) is ray.ObjectRef
+
+        self.oid = object_id
+        if call_queue is None:
+            call_queue = []
+        self.call_queue = call_queue
+        self._length_cache = length
+        self._width_cache = width
+        self._ip_cache = ip
 
-    def apply(self, func, num_splits=None, other_axis_partition=None, **kwargs):
-        """Applies func to the object in the plasma store.
+    def get(self):
+        """Gets the object out of the plasma store.
 
-        See notes in Parent class about this method.
+        Returns:
+            The object from the plasma store.
+        """
+        if len(self.call_queue):
+            self.drain_call_queue()
+        try:
+            return ray.get(self.oid)
+        except RayTaskError as e:
+            handle_ray_task_error(e)
+
+    def apply(self, func, **kwargs):
+        """Apply a function to the object stored in this partition.
+
+        Note: It does not matter if func is callable or an ObjectRef. Ray will
+            handle it correctly either way. The keyword arguments are sent as a
+            dictionary.
 
         Args:
             func: The function to apply.
-            num_splits: The number of times to split the result object.
-            other_axis_partition: Another `PyarrowOnRayFrameAxisPartition` object to apply to
-                func with this one.
 
         Returns:
-            A list of `RayRemotePartition` objects.
+            A RayRemotePartition object.
         """
-        if num_splits is None:
-            num_splits = len(self.list_of_blocks)
-
-        if other_axis_partition is not None:
-            return [
-                PyarrowOnRayFramePartition(obj)
-                for obj in deploy_ray_func_between_two_axis_partitions._remote(
-                    args=(self.axis, func, num_splits, len(self.list_of_blocks), kwargs)
-                    + tuple(self.list_of_blocks + other_axis_partition.list_of_blocks),
-                    num_returns=num_splits,
-                )
-            ]
-
-        args = [self.axis, func, num_splits, kwargs]
-        args.extend(self.list_of_blocks)
-        return [
-            PyarrowOnRayFramePartition(obj)
-            for obj in deploy_ray_axis_func._remote(args, num_returns=num_splits)
-        ]
+        oid = self.oid
+        call_queue = self.call_queue + [(func, kwargs)]
+        result, length, width, ip = deploy_ray_func.remote(call_queue, oid)
+        return PandasOnRayFramePartition(result, length, width, ip)
+
+    def add_to_apply_calls(self, func, **kwargs):
+        return PandasOnRayFramePartition(
+            self.oid, call_queue=self.call_queue + [(func, kwargs)]
+        )
 
-    def shuffle(self, func, num_splits=None, **kwargs):
-        """Shuffle the order of the data in this axis based on the `func`.
+    def drain_call_queue(self):
+        if len(self.call_queue) == 0:
+            return
+        oid = self.oid
+        call_queue = self.call_queue
+        (
+            self.oid,
+            self._length_cache,
+            self._width_cache,
+            self._ip_cache,
+        ) = deploy_ray_func.remote(call_queue, oid)
+        self.call_queue = []
+
+    def wait(self):
+        self.drain_call_queue()
+        try:
+            ray.wait([self.oid])
+        except RayTaskError as e:
+            handle_ray_task_error(e)
+
+    def __copy__(self):
+        return PandasOnRayFramePartition(
+            self.oid,
+            length=self._length_cache,
+            width=self._width_cache,
+            ip=self._ip_cache,
+            call_queue=self.call_queue,
+        )
 
-        Extends `BaseFrameAxisPartition.shuffle`.
+    def to_pandas(self):
+        """Convert the object stored in this partition to a Pandas DataFrame.
 
-        :param func:
-        :param num_splits:
-        :param kwargs:
-        :return:
+        Returns:
+            A Pandas DataFrame.
         """
-        if num_splits is None:
-            num_splits = len(self.list_of_blocks)
-
-        args = [self.axis, func, num_splits, kwargs]
-        args.extend(self.list_of_blocks)
-        return [
-            PyarrowOnRayFramePartition(obj)
-            for obj in deploy_ray_axis_func._remote(args, num_returns=num_splits)
-        ]
+        dataframe = self.get()
+        assert type(dataframe) is pandas.DataFrame or type(dataframe) is pandas.Series
+        return dataframe
 
+    def to_numpy(self, **kwargs):
+        """
+        Convert the object stored in this partition to a NumPy array.
 
-class PyarrowOnRayFrameColumnPartition(PyarrowOnRayFrameAxisPartition):
-    """The column partition implementation for Ray. All of the implementation
-    for this class is in the parent class, and this class defines the axis
-    to perform the computation over.
-    """
+        Returns
+        -------
+            A NumPy array.
+        """
+        return self.apply(lambda df, **kwargs: df.to_numpy(**kwargs)).get()
 
-    axis = 0
+    def mask(self, row_indices, col_indices):
+        if (
+            (isinstance(row_indices, slice) and row_indices == slice(None))
+            or (
+                not isinstance(row_indices, slice)
+                and self._length_cache is not None
+                and len(row_indices) == self._length_cache
+            )
+        ) and (
+            (isinstance(col_indices, slice) and col_indices == slice(None))
+            or (
+                not isinstance(col_indices, slice)
+                and self._width_cache is not None
+                and len(col_indices) == self._width_cache
+            )
+        ):
+            return self.__copy__()
 
+        new_obj = self.add_to_apply_calls(
+            lambda df: pandas.DataFrame(df.iloc[row_indices, col_indices])
+        )
+        if not isinstance(row_indices, slice):
+            new_obj._length_cache = len(row_indices)
+        if not isinstance(col_indices, slice):
+            new_obj._width_cache = len(col_indices)
+        return new_obj
+
+    @classmethod
+    def put(cls, obj):
+        """Put an object in the Plasma store and wrap it in this object.
 
-class PyarrowOnRayFrameRowPartition(PyarrowOnRayFrameAxisPartition):
-    """The row partition implementation for Ray. All of the implementation
-    for this class is in the parent class, and this class defines the axis
-    to perform the computation over.
-    """
+        Args:
+            obj: The object to be put.
 
-    axis = 1
+        Returns:
+            A `RayRemotePartition` object.
+        """
+        return PandasOnRayFramePartition(ray.put(obj), len(obj.index), len(obj.columns))
 
+    @classmethod
+    def preprocess_func(cls, func):
+        """Put a callable function into the plasma store for use in `apply`.
 
-def concat_arrow_table_partitions(axis, partitions):
-    if axis == 0:
-        table = pyarrow.Table.from_batches(
-            [part.to_batches(part.num_rows)[0] for part in partitions]
-        )
-    else:
-        table = partitions[0].drop([partitions[0].columns[-1].name])
-        for obj in partitions[1:]:
-            i = 0
-            for col in obj.itercolumns():
-                if i < obj.num_columns - 1:
-                    table = table.append_column(col)
-                i += 1
-        table = table.append_column(partitions[0].columns[-1])
-    return table
-
-
-def split_arrow_table_result(axis, result, num_partitions, num_splits, metadata):
-    chunksize = (
-        num_splits // num_partitions
-        if num_splits % num_partitions == 0
-        else num_splits // num_partitions + 1
-    )
-    if axis == 0:
-        return [
-            pyarrow.Table.from_batches([part]) for part in result.to_batches(chunksize)
-        ]
-    else:
-        return [
-            result.drop(
-                [
-                    result.columns[i].name
-                    for i in range(result.num_columns)
-                    if i >= n * chunksize or i < (n - 1) * chunksize
-                ]
-            )
-            .append_column(result.columns[-1])
-            .replace_schema_metadata(metadata=metadata)
-            for n in range(1, num_splits)
-        ] + [
-            result.drop(
-                [
-                    result.columns[i].name
-                    for i in range(result.num_columns)
-                    if i < (num_splits - 1) * chunksize
-                ]
-            ).replace_schema_metadata(metadata=metadata)
-        ]
-
-
-@ray.remote
-def deploy_ray_axis_func(axis, func, num_splits, kwargs, *partitions):
-    """Deploy a function along a full axis in Ray.
-
-    Args:
-        axis: The axis to perform the function along.
-        func: The function to perform.
-        num_splits: The number of splits to return
-            (see `split_result_of_axis_func_pandas`)
-        kwargs: A dictionary of keyword arguments.
-        partitions: All partitions that make up the full axis (row or column)
-
-    Returns:
-        A list of Pandas DataFrames.
-    """
-    table = concat_arrow_table_partitions(axis, partitions)
-    try:
-        result = func(table, **kwargs)
-    except Exception:
-        result = pyarrow.Table.from_pandas(func(table.to_pandas(), **kwargs))
-    return split_arrow_table_result(
-        axis, result, len(partitions), num_splits, table.schema.metadata
-    )
+        Args:
+            func: The function to preprocess.
 
+        Returns:
+            A ray.ObjectRef.
+        """
+        return ray.put(func)
 
-@ray.remote
-def deploy_ray_func_between_two_axis_partitions(
-    axis, func, num_splits, len_of_left, kwargs, *partitions
-):
-    """Deploy a function along a full axis between two data sets in Ray.
-
-    Args:
-        axis: The axis to perform the function along.
-        func: The function to perform.
-        num_splits: The number of splits to return
-            (see `split_result_of_axis_func_pandas`).
-        len_of_left: The number of values in `partitions` that belong to the
-            left data set.
-        kwargs: A dictionary of keyword arguments.
-        partitions: All partitions that make up the full axis (row or column)
-            for both data sets.
-
-    Returns:
-        A list of Pandas DataFrames.
-    """
-    lt_table = concat_arrow_table_partitions(axis, partitions[:len_of_left])
-    rt_table = concat_arrow_table_partitions(axis, partitions[len_of_left:])
+    def length(self):
+        if self._length_cache is None:
+            if len(self.call_queue):
+                self.drain_call_queue()
+            else:
+                self._length_cache, self._width_cache = get_index_and_columns.remote(
+                    self.oid
+                )
+        if isinstance(self._length_cache, ray.ObjectRef):
+            try:
+                self._length_cache = ray.get(self._length_cache)
+            except RayTaskError as e:
+                handle_ray_task_error(e)
+        return self._length_cache
+
+    def width(self):
+        if self._width_cache is None:
+            if len(self.call_queue):
+                self.drain_call_queue()
+            else:
+                self._length_cache, self._width_cache = get_index_and_columns.remote(
+                    self.oid
+                )
+        if isinstance(self._width_cache, ray.ObjectRef):
+            try:
+                self._width_cache = ray.get(self._width_cache)
+            except RayTaskError as e:
+                handle_ray_task_error(e)
+        return self._width_cache
+
+    def ip(self):
+        if self._ip_cache is None:
+            if len(self.call_queue):
+                self.drain_call_queue()
+            else:
+                self._ip_cache = self.apply(lambda df: df)._ip_cache
+        if isinstance(self._ip_cache, ray.ObjectID):
+            try:
+                self._ip_cache = ray.get(self._ip_cache)
+            except RayTaskError as e:
+                handle_ray_task_error(e)
+        return self._ip_cache
+
+    @classmethod
+    def length_extraction_fn(cls):
+        return length_fn_pandas
+
+    @classmethod
+    def width_extraction_fn(cls):
+        return width_fn_pandas
+
+    @classmethod
+    def empty(cls):
+        return cls.put(pandas.DataFrame())
+
+
+@ray.remote(num_returns=2)
+def get_index_and_columns(df):
+    return len(df.index), len(df.columns)
+
+
+@ray.remote(num_returns=4)
+def deploy_ray_func(call_queue, partition):  # pragma: no cover
+    def deserialize(obj):
+        if isinstance(obj, ray.ObjectRef):
+            return ray.get(obj)
+        return obj
+
+    if len(call_queue) > 1:
+        for func, kwargs in call_queue[:-1]:
+            func = deserialize(func)
+            kwargs = deserialize(kwargs)
+            try:
+                partition = func(partition, **kwargs)
+            except ValueError:
+                partition = func(partition.copy(), **kwargs)
+    func, kwargs = call_queue[-1]
+    func = deserialize(func)
+    kwargs = deserialize(kwargs)
     try:
-        result = func(lt_table, rt_table, **kwargs)
-    except Exception:
-        lt_frame = lt_table.from_pandas()
-        rt_frame = rt_table.from_pandas()
-        result = pyarrow.Table.from_pandas(func(lt_frame, rt_frame, **kwargs))
-    return split_arrow_table_result(
-        axis, result, len(result.num_rows), num_splits, result.schema.metadata
+        result = func(partition, **kwargs)
+    # Sometimes Arrow forces us to make a copy of an object before we operate on it. We
+    # don't want the error to propagate to the user, and we want to avoid copying unless
+    # we absolutely have to.
+    except ValueError:
+        result = func(partition.copy(), **kwargs)
+    return (
+        result,
+        len(result) if hasattr(result, "__len__") else 0,
+        len(result.columns) if hasattr(result, "columns") else 0,
+        get_node_ip_address(),
     )
-
-
-@ray.remote
-def deploy_ray_shuffle_func(axis, func, numsplits, kwargs, *partitions):
-    """Deploy a function that defines the partitions along this axis.
-
-    Args:
-        axis:
-        func:
-        numsplits:
-        kwargs:
-        partitions:
-
-    Returns:
-        A list of Pandas DataFrames.
-    """
-    pass
```

### Comparing `modin-0.9.0/modin/experimental/engines/pyarrow_on_ray/frame/data.py` & `modin-0.9.1/modin/experimental/engines/pyarrow_on_ray/frame/data.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/cloud/tracing/__init__.py` & `modin-0.9.1/modin/engines/python/pandas_on_python/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/cloud/tracing/tracing_connection.py` & `modin-0.9.1/modin/experimental/cloud/tracing/tracing_connection.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/cloud/tracing/parse_rpyc_trace.py` & `modin-0.9.1/modin/experimental/cloud/tracing/parse_rpyc_trace.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/cloud/test/__init__.py` & `modin-0.9.1/modin/engines/python/pandas_on_python/frame/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/cloud/test/test_cloud.py` & `modin-0.9.1/modin/experimental/cloud/test/test_cloud.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/cloud/__init__.py` & `modin-0.9.1/modin/experimental/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/cloud/rayscale.py` & `modin-0.9.1/modin/experimental/cloud/rayscale.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/cloud/connection.py` & `modin-0.9.1/modin/experimental/cloud/connection.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/cloud/omnisci.py` & `modin-0.9.1/modin/data_management/factories/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,40 +7,23 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 
-import warnings
+from . import factories
 
-from .rayscale import RayCluster
-from .cluster import Provider
 
+def _get_remote_engines():
+    for name in dir(factories):
+        obj = getattr(factories, name)
+        if isinstance(obj, type) and issubclass(
+            obj, factories.ExperimentalRemoteFactory
+        ):
+            try:
+                yield obj.get_info().engine
+            except factories.NotRealFactory:
+                pass
 
-class RemoteOmnisci(RayCluster):
-    target_engine = "Cloudray"
-    target_partition = "Omnisci"
 
-    def __init__(
-        self,
-        provider: Provider,
-        project_name: str = None,
-        cluster_name: str = "modin-cluster",
-        worker_count: int = 0,
-        head_node_type: str = None,
-        worker_node_type: str = None,
-        add_conda_packages: list = None,
-    ):
-        if worker_count != 0:
-            warnings.warn(
-                "Current Omnisci on cloud does not support multi-node setups, not requesting worker nodes"
-            )
-        super().__init__(
-            provider,
-            project_name,
-            cluster_name,
-            0,
-            head_node_type,
-            worker_node_type,
-            add_conda_packages,
-        )
+REMOTE_ENGINES = set(_get_remote_engines())
```

### Comparing `modin-0.9.0/modin/experimental/cloud/meta_magic.py` & `modin-0.9.1/modin/experimental/cloud/meta_magic.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/cloud/cluster.py` & `modin-0.9.1/modin/experimental/cloud/cluster.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/cloud/rpyc_proxy.py` & `modin-0.9.1/modin/experimental/cloud/rpyc_proxy.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/cloud/local_cluster.py` & `modin-0.9.1/modin/experimental/cloud/local_cluster.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/cloud/base.py` & `modin-0.9.1/modin/experimental/cloud/base.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/pandas/io_exp.py` & `modin-0.9.1/modin/experimental/pandas/io_exp.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/pandas/test/__init__.py` & `modin-0.9.1/modin/engines/python/pandas_on_python/series/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/pandas/test/test_io_exp.py` & `modin-0.9.1/modin/experimental/pandas/test/test_io_exp.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/experimental/pandas/__init__.py` & `modin-0.9.1/modin/data_management/functions/default_methods/any_default.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,24 +7,29 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 
-from modin.config import IsExperimental
+from .default import DefaultMethod
 
-IsExperimental.put(True)
 
-# import numpy_wrap as early as possible to intercept all "import numpy" statements
-# in the user code
-from .numpy_wrap import _CAUGHT_NUMPY  # noqa F401
-from modin.pandas import *  # noqa F401, F403
-from .io_exp import read_sql, read_csv_glob  # noqa F401
-import warnings
-
-
-warnings.warn(
-    "Thank you for using the Modin Experimental pandas API."
-    "\nPlease note that some of these APIs deviate from pandas in order to "
-    "provide improved performance."
-)
+class ObjTypeDeterminer:
+    def __getattr__(self, key):
+        def func(df, *args, **kwargs):
+            prop = getattr(df, key)
+            if callable(prop):
+                return prop(*args, **kwargs)
+            else:
+                return prop
+
+        return func
+
+
+class AnyDefault(DefaultMethod):
+    @classmethod
+    def register(cls, func, obj_type=None, **kwargs):
+        if obj_type is None:
+            obj_type = ObjTypeDeterminer()
+
+        return cls.call(func, obj_type=obj_type, **kwargs)
```

### Comparing `modin-0.9.0/modin/experimental/pandas/numpy_wrap.py` & `modin-0.9.1/modin/experimental/pandas/numpy_wrap.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/conftest.py` & `modin-0.9.1/modin/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,19 @@
     )
     parser.addoption(
         "--backend",
         action="store",
         default=None,
         help="specifies backend to run tests on",
     )
+    parser.addoption(
+        "--extra-test-parameters",
+        action="store_true",
+        help="activate extra test parameter combinations",
+    )
 
 
 class Patcher:
     def __init__(self, conn, *pairs):
         self.pairs = pairs
         self.originals = None
         self.conn = conn
@@ -181,14 +186,17 @@
 BASE_BACKEND_NAME = "BaseOnPython"
 
 
 class TestQC(BaseQueryCompiler):
     def __init__(self, modin_frame):
         self._modin_frame = modin_frame
 
+    def finalize(self):
+        self._modin_frame.finalize()
+
     @classmethod
     def from_pandas(cls, df, data_cls):
         return cls(data_cls.from_pandas(df))
 
     @classmethod
     def from_arrow(cls, at, data_cls):
         return cls(data_cls.from_arrow(at))
@@ -212,14 +220,19 @@
 
 def set_base_backend(name=BASE_BACKEND_NAME):
     setattr(factories, f"{name}Factory", BaseOnPythonFactory)
     modin.set_backends(engine="python", partition=name.split("On")[0])
 
 
 def pytest_configure(config):
+    if config.option.extra_test_parameters is not None:
+        import modin.pandas.test.utils as utils
+
+        utils.extra_test_parameters = config.option.extra_test_parameters
+
     backend = config.option.backend
 
     if backend is None:
         return
 
     if backend == BASE_BACKEND_NAME:
         set_base_backend(BASE_BACKEND_NAME)
```

### Comparing `modin-0.9.0/modin/test/test_backends_api.py` & `modin-0.9.1/modin/test/test_backends_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 BACKENDS = [PandasQueryCompiler, PyarrowQueryCompiler]
 
 
 def test_base_abstract_methods():
     allowed_abstract_methods = [
         "__init__",
         "free",
+        "finalize",
         "to_pandas",
         "from_pandas",
         "from_arrow",
         "default_to_pandas",
     ]
 
     not_implemented_methods = BASE_BACKEND.__abstractmethods__.difference(
```

### Comparing `modin-0.9.0/modin/test/test_envvar_npartitions.py` & `modin-0.9.1/modin/test/test_envvar_npartitions.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/test/__init__.py` & `modin-0.9.1/modin/engines/ray/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/test/test_partition_api.py` & `modin-0.9.1/modin/test/test_partition_api.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/test/test_headers.py` & `modin-0.9.1/modin/test/test_headers.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/spreadsheet/test/__init__.py` & `modin-0.9.1/modin/engines/ray/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/spreadsheet/test/test_general.py` & `modin-0.9.1/modin/spreadsheet/test/test_general.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/spreadsheet/__init__.py` & `modin-0.9.1/modin/spreadsheet/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/spreadsheet/general.py` & `modin-0.9.1/modin/spreadsheet/general.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/distributed/dataframe/pandas/partitions.py` & `modin-0.9.1/modin/distributed/dataframe/pandas/partitions.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/distributed/dataframe/pandas/__init__.py` & `modin-0.9.1/modin/distributed/dataframe/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/config/test/test_envvars.py` & `modin-0.9.1/modin/config/test/test_envvars.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/config/test/__init__.py` & `modin-0.9.1/modin/engines/ray/generic/frame/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/config/test/test_parameter.py` & `modin-0.9.1/modin/config/test/test_parameter.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/config/envvars.py` & `modin-0.9.1/modin/config/envvars.py`

 * *Files 17% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     """
 
     varname = "MODIN_REDIS_ADDRESS"
 
 
 class CpuCount(EnvironmentVariable, type=int):
     """
-    How may CPU cores to utilize across the whole distribution
+    How many CPU cores to use when initialization of the Modin engine.
     """
 
     varname = "MODIN_CPUS"
 
     @classmethod
     def _get_default(cls):
         import multiprocessing
@@ -141,21 +141,42 @@
     """
 
     varname = "MODIN_MEMORY"
 
 
 class NPartitions(EnvironmentVariable, type=int):
     """
-    How many partitions to use by default
+    How many partitions to use for a Modin DataFrame (along each axis)
     """
 
     varname = "MODIN_NPARTITIONS"
+    # This flag is used to detect whether NPartitions is default value or not
+    _is_default = False
+
+    @classmethod
+    def put(cls, value):
+        super().put(value)
+        cls._is_default = False
+
+    @classmethod
+    def put_if_default(cls, value):
+        """
+        Put specific value if NPartitions wasn't set by a user yet
+
+        Notes
+        -----
+        This method is used to set NPartitions from cluster resources internally
+        and should not be called by a user.
+        """
+        if cls._is_default:
+            cls.put(value)
 
     @classmethod
     def _get_default(cls):
+        cls._is_default = True
         return CpuCount.get()
 
 
 class RayPlasmaDir(EnvironmentVariable, type=ExactStr):
     """
     Path to Plasma storage for Ray
     """
@@ -256,14 +277,47 @@
     def enable(cls):
         cls.put(True)
 
     @classmethod
     def disable(cls):
         cls.put(False)
 
+    @classmethod
+    def put(cls, value):
+        if value and BenchmarkMode.get():
+            raise ValueError("ProgressBar isn't compatible with BenchmarkMode")
+        super().put(value)
+
+
+class BenchmarkMode(EnvironmentVariable, type=bool):
+    """
+    Whether or not to perform computations syncronous.
+    """
+
+    varname = "MODIN_BENCHMARK_MODE"
+    default = False
+
+    @classmethod
+    def put(cls, value):
+        if value and ProgressBar.get():
+            raise ValueError("BenchmarkMode isn't compatible with ProgressBar")
+        super().put(value)
+
+
+class PersistentPickle(EnvironmentVariable, type=bool):
+    """
+    When set to off, it allows faster serialization which is only
+    valid in current run (i.e. useless for saving to disk).
+    When set to on, Modin objects could be saved to disk and loaded
+    but serialization/deserialization could take more time.
+    """
+
+    varname = "MODIN_PERSISTENT_PICKLE"
+    default = False
+
 
 def _check_vars():
     """
     Look out for any environment variables that start with "MODIN_" prefix
     that are unknown - they might be a typo, so warn a user
     """
     valid_names = {
```

### Comparing `modin-0.9.0/modin/config/__init__.py` & `modin-0.9.1/modin/data_management/functions/default_methods/datetime_default.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,9 +7,14 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 
-from .pubsub import Parameter  # noqa: F401
-from .envvars import *  # noqa: F403, F401
+from .series_default import SeriesDefault
+
+
+class DateTimeDefault(SeriesDefault):
+    @classmethod
+    def frame_wrapper(cls, df):
+        return df.squeeze(axis=1).dt
```

### Comparing `modin-0.9.0/modin/config/pubsub.py` & `modin-0.9.1/modin/config/pubsub.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/config/__main__.py` & `modin-0.9.1/modin/engines/base/io/column_stores/feather_dispatcher.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,20 +7,34 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 
-from . import *  # noqa: F403, F401
-from .pubsub import Parameter
+from modin.engines.base.io.column_stores.column_store_dispatcher import (
+    ColumnStoreDispatcher,
+)
 
 
-def print_config_help():
-    for objname in sorted(globals()):
-        obj = globals()[objname]
-        if isinstance(obj, type) and issubclass(obj, Parameter) and not obj.is_abstract:
-            print(f"{obj.get_help()}\n\tCurrent value: {obj.get()}")  # noqa: T001
+class FeatherDispatcher(ColumnStoreDispatcher):
+    @classmethod
+    def _read(cls, path, columns=None, **kwargs):
+        """Read data from the file path, returning a Modin DataFrame.
+           Modin only supports pyarrow engine for now.
 
+        Args:
+            path: The filepath of the feather file.
+                  We only support local files for now.
+                Multi threading is set to False by default
+            columns: Not supported by pandas api, but can be passed here
+                     to read only specific columns
 
-if __name__ == "__main__":
-    print_config_help()
+        Notes:
+            pyarrow feather is used. Please refer to the documentation here
+            https://arrow.apache.org/docs/python/api.html#feather-format
+        """
+        if columns is None:
+            from pyarrow.feather import read_feather
+
+            df = read_feather(path)
+        return cls.build_query_compiler(path, df.columns, use_threads=False)
```

### Comparing `modin-0.9.0/modin/data_management/__init__.py` & `modin-0.9.1/modin/engines/ray/generic/series/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/data_management/utils.py` & `modin-0.9.1/modin/data_management/utils.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/data_management/factories/dispatcher.py` & `modin-0.9.1/modin/data_management/factories/dispatcher.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/data_management/factories/test/__init__.py` & `modin-0.9.1/modin/engines/ray/pandas_on_ray/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/data_management/factories/test/test_dispatcher.py` & `modin-0.9.1/modin/data_management/factories/test/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/data_management/factories/factories.py` & `modin-0.9.1/modin/data_management/factories/factories.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/data_management/functions/default_methods/dataframe_default.py` & `modin-0.9.1/modin/data_management/functions/default_methods/dataframe_default.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/data_management/functions/default_methods/series_default.py` & `modin-0.9.1/modin/data_management/functions/default_methods/series_default.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/data_management/functions/default_methods/rolling_default.py` & `modin-0.9.1/modin/data_management/functions/default_methods/rolling_default.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/data_management/functions/default_methods/str_default.py` & `modin-0.9.1/modin/data_management/functions/default_methods/str_default.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/data_management/functions/default_methods/__init__.py` & `modin-0.9.1/modin/data_management/functions/default_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/data_management/functions/default_methods/cat_default.py` & `modin-0.9.1/modin/data_management/functions/default_methods/cat_default.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/data_management/functions/default_methods/datetime_default.py` & `modin-0.9.1/modin/backends/base/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,10 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 
-from .series_default import SeriesDefault
+from .query_compiler import BaseQueryCompiler
 
-
-class DateTimeDefault(SeriesDefault):
-    @classmethod
-    def frame_wrapper(cls, df):
-        return df.squeeze(axis=1).dt
+__all__ = ["BaseQueryCompiler"]
```

### Comparing `modin-0.9.0/modin/data_management/functions/default_methods/default.py` & `modin-0.9.1/modin/data_management/functions/default_methods/default.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/data_management/functions/default_methods/binary_default.py` & `modin-0.9.1/modin/engines/ray/task_wrapper.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,38 +7,23 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 
-from .any_default import AnyDefault
+import ray
 
-import pandas
-from pandas.core.dtypes.common import is_list_like
 
+@ray.remote
+def deploy_ray_func(func, args):  # pragma: no cover
+    return func(**args)
 
-class BinaryDefault(AnyDefault):
+
+class RayTask:
     @classmethod
-    def build_default_to_pandas(cls, fn, fn_name):
-        def bin_ops_wrapper(df, other, *args, **kwargs):
-            squeeze_other = kwargs.pop("broadcast", False) or kwargs.pop(
-                "squeeze_other", False
-            )
-            squeeze_self = kwargs.pop("squeeze_self", False)
-
-            if squeeze_other:
-                other = other.squeeze(axis=1)
-
-            if squeeze_self:
-                df = df.squeeze(axis=1)
-
-            result = fn(df, other, *args, **kwargs)
-            if (
-                not isinstance(result, pandas.Series)
-                and not isinstance(result, pandas.DataFrame)
-                and is_list_like(result)
-            ):
-                result = pandas.DataFrame(result)
-            return result
+    def deploy(cls, func, num_returns, kwargs):
+        return deploy_ray_func._remote(args=(func, kwargs), num_returns=num_returns)
 
-        return super().build_default_to_pandas(bin_ops_wrapper, fn_name)
+    @classmethod
+    def materialize(cls, obj_id):
+        return ray.get(obj_id)
```

### Comparing `modin-0.9.0/modin/data_management/functions/default_methods/any_default.py` & `modin-0.9.1/modin/data_management/functions/mapfunction.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,29 +7,21 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 
-from .default import DefaultMethod
+from .function import Function
 
 
-class ObjTypeDeterminer:
-    def __getattr__(self, key):
-        def func(df, *args, **kwargs):
-            prop = getattr(df, key)
-            if callable(prop):
-                return prop(*args, **kwargs)
-            else:
-                return prop
-
-        return func
-
-
-class AnyDefault(DefaultMethod):
+class MapFunction(Function):
     @classmethod
-    def register(cls, func, obj_type=None, **kwargs):
-        if obj_type is None:
-            obj_type = ObjTypeDeterminer()
+    def call(cls, function, *call_args, **call_kwds):
+        def caller(query_compiler, *args, **kwargs):
+            return query_compiler.__constructor__(
+                query_compiler._modin_frame._map(
+                    lambda x: function(x, *args, **kwargs), *call_args, **call_kwds
+                )
+            )
 
-        return cls.call(func, obj_type=obj_type, **kwargs)
+        return caller
```

### Comparing `modin-0.9.0/modin/data_management/functions/default_methods/resample_default.py` & `modin-0.9.1/modin/data_management/functions/default_methods/resample_default.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/data_management/functions/default_methods/groupby_default.py` & `modin-0.9.1/modin/data_management/functions/default_methods/groupby_default.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/data_management/functions/groupby_function.py` & `modin-0.9.1/modin/data_management/functions/groupby_function.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/data_management/functions/foldfunction.py` & `modin-0.9.1/modin/data_management/functions/foldfunction.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/data_management/functions/mapreducefunction.py` & `modin-0.9.1/modin/data_management/functions/mapreducefunction.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,22 +14,20 @@
 from .function import Function
 
 
 class MapReduceFunction(Function):
     @classmethod
     def call(cls, map_function, reduce_function, **call_kwds):
         def caller(query_compiler, *args, **kwargs):
-            preserve_index = call_kwds.pop("preserve_index", True)
             axis = call_kwds.get("axis", kwargs.get("axis"))
             return query_compiler.__constructor__(
                 query_compiler._modin_frame._map_reduce(
                     cls.validate_axis(axis),
                     lambda x: map_function(x, *args, **kwargs),
                     lambda y: reduce_function(y, *args, **kwargs),
-                    preserve_index=preserve_index,
                 )
             )
 
         return caller
 
     @classmethod
     def register(cls, map_function, reduce_function=None, **kwargs):
```

### Comparing `modin-0.9.0/modin/data_management/functions/__init__.py` & `modin-0.9.1/modin/data_management/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/data_management/functions/binary_function.py` & `modin-0.9.1/modin/data_management/functions/binary_function.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/data_management/functions/reductionfunction.py` & `modin-0.9.1/modin/data_management/functions/reductionfunction.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,18 +14,16 @@
 from .function import Function
 
 
 class ReductionFunction(Function):
     @classmethod
     def call(cls, reduction_function, **call_kwds):
         def caller(query_compiler, *args, **kwargs):
-            preserve_index = call_kwds.pop("preserve_index", True)
             axis = call_kwds.get("axis", kwargs.get("axis"))
             return query_compiler.__constructor__(
                 query_compiler._modin_frame._fold_reduce(
                     cls.validate_axis(axis),
                     lambda x: reduction_function(x, *args, **kwargs),
-                    preserve_index=preserve_index,
                 )
             )
 
         return caller
```

### Comparing `modin-0.9.0/modin/data_management/functions/function.py` & `modin-0.9.1/modin/engines/dask/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,29 +7,32 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 
-from typing import Optional
+from modin.config import CpuCount, NPartitions
+from modin.error_message import ErrorMessage
 
 
-class Function(object):
-    def __init__(self):
-        raise ValueError(
-            "Please use {}.register instead of the constructor".format(
-                type(self).__name__
-            )
+def initialize_dask():
+    from distributed.client import get_client
+
+    try:
+        client = get_client()
+    except ValueError:
+        from distributed import Client
+
+        # The indentation here is intentional, we want the code to be indented.
+        ErrorMessage.not_initialized(
+            "Dask",
+            """
+    from distributed import Client
+
+    client = Client()
+""",
         )
+        client = Client(n_workers=CpuCount.get())
 
-    @classmethod
-    def call(cls, func, **call_kwds):
-        raise NotImplementedError("Please implement in child class")
-
-    @classmethod
-    def register(cls, func, **kwargs):
-        return cls.call(func, **kwargs)
-
-    @classmethod
-    def validate_axis(cls, axis: Optional[int]) -> int:
-        return 0 if axis is None else axis
+    num_cpus = len(client.ncores())
+    NPartitions.put_if_default(num_cpus)
```

### Comparing `modin-0.9.0/modin/backends/__init__.py` & `modin-0.9.1/modin/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/backends/base/query_compiler.py` & `modin-0.9.1/modin/backends/base/query_compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,14 +155,19 @@
     # Data Management Methods
     @abc.abstractmethod
     def free(self):
         """In the future, this will hopefully trigger a cleanup of this object."""
         # TODO create a way to clean up this object.
         pass
 
+    @abc.abstractmethod
+    def finalize(self):
+        """Finalize constructing the dataframe calling all deferred functions which were used to build it."""
+        pass
+
     # END Data Management Methods
 
     # To/From Pandas
     @abc.abstractmethod
     def to_pandas(self):
         """Converts Modin DataFrame to Pandas DataFrame.
```

### Comparing `modin-0.9.0/modin/backends/base/__init__.py` & `modin-0.9.1/modin/engines/ray/pandas_on_ray/frame/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,11 +6,7 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
-
-from .query_compiler import BaseQueryCompiler
-
-__all__ = ["BaseQueryCompiler"]
```

### Comparing `modin-0.9.0/modin/backends/pandas/query_compiler.py` & `modin-0.9.1/modin/backends/pandas/query_compiler.py`

 * *Files 4% similar despite different names*

```diff
@@ -197,14 +197,17 @@
                 result.name = "__reduced__"
             result = result.to_frame()
         if isinstance(result, pandas.DataFrame):
             return self.from_pandas(result, type(self._modin_frame))
         else:
             return result
 
+    def finalize(self):
+        self._modin_frame.finalize()
+
     def to_pandas(self):
         return self._modin_frame.to_pandas()
 
     @classmethod
     def from_pandas(cls, df, data_cls):
         return cls(data_cls.from_pandas(df))
 
@@ -527,21 +530,110 @@
         """Removes all levels from index and sets a default level_0 index.
 
         Returns:
             A new QueryCompiler with updated data and reset index.
         """
         drop = kwargs.get("drop", False)
         level = kwargs.get("level", None)
-        # TODO Implement level
-        if level is not None or self.has_multiindex():
-            return self.default_to_pandas(pandas.DataFrame.reset_index, **kwargs)
+        new_index = None
+        if level is not None:
+            if not isinstance(level, (tuple, list)):
+                level = [level]
+            level = [self.index._get_level_number(lev) for lev in level]
+            uniq_sorted_level = sorted(set(level))
+            if len(uniq_sorted_level) < self.index.nlevels:
+                # We handle this by separately computing the index. We could just
+                # put the labels into the data and pull them back out, but that is
+                # expensive.
+                new_index = (
+                    self.index.droplevel(uniq_sorted_level)
+                    if len(level) < self.index.nlevels
+                    else pandas.RangeIndex(len(self.index))
+                )
+        else:
+            uniq_sorted_level = list(range(self.index.nlevels))
+
         if not drop:
-            return self.__constructor__(self._modin_frame.from_labels())
-        new_self = self.copy()
-        new_self.index = pandas.RangeIndex(len(new_self.index))
+            if len(uniq_sorted_level) < self.index.nlevels:
+                # These are the index levels that will remain after the reset_index
+                keep_levels = [
+                    i for i in range(self.index.nlevels) if i not in uniq_sorted_level
+                ]
+                new_copy = self.copy()
+                # Change the index to have only the levels that will be inserted
+                # into the data. We will replace the old levels later.
+                new_copy.index = self.index.droplevel(keep_levels)
+                new_copy.index.names = [
+                    "level_{}".format(level_value)
+                    if new_copy.index.names[level_index] is None
+                    else new_copy.index.names[level_index]
+                    for level_index, level_value in enumerate(uniq_sorted_level)
+                ]
+                new_modin_frame = new_copy._modin_frame.from_labels()
+                # Replace the levels that will remain as a part of the index.
+                new_modin_frame.index = new_index
+            else:
+                new_modin_frame = self._modin_frame.from_labels()
+            if isinstance(new_modin_frame.columns, pandas.MultiIndex):
+                # Fix col_level and col_fill in generated column names because from_labels works with assumption
+                # that col_level and col_fill are not specified but it expands tuples in level names.
+                col_level = kwargs.get("col_level", 0)
+                col_fill = kwargs.get("col_fill", "")
+                if col_level != 0 or col_fill != "":
+                    # Modify generated column names if col_level and col_fil have values different from default.
+                    levels_names_list = [
+                        f"level_{level_index}" if level_name is None else level_name
+                        for level_index, level_name in enumerate(self.index.names)
+                    ]
+                    if col_fill is None:
+                        # Initialize col_fill if it is None.
+                        # This is some weird undocumented Pandas behavior to take first
+                        # element of the last column name.
+                        last_col_name = levels_names_list[uniq_sorted_level[-1]]
+                        last_col_name = (
+                            list(last_col_name)
+                            if isinstance(last_col_name, tuple)
+                            else [last_col_name]
+                        )
+                        if len(last_col_name) not in (1, self.columns.nlevels):
+                            raise ValueError(
+                                "col_fill=None is incompatible "
+                                f"with incomplete column name {last_col_name}"
+                            )
+                        col_fill = last_col_name[0]
+                    columns_list = new_modin_frame.columns.tolist()
+                    for level_index, level_value in enumerate(uniq_sorted_level):
+                        level_name = levels_names_list[level_value]
+                        # Expand tuples into separate items and fill the rest with col_fill
+                        top_level = [col_fill] * col_level
+                        middle_level = (
+                            list(level_name)
+                            if isinstance(level_name, tuple)
+                            else [level_name]
+                        )
+                        bottom_level = [col_fill] * (
+                            self.columns.nlevels - (col_level + len(middle_level))
+                        )
+                        item = tuple(top_level + middle_level + bottom_level)
+                        if len(item) > self.columns.nlevels:
+                            raise ValueError(
+                                "Item must have length equal to number of levels."
+                            )
+                        columns_list[level_index] = item
+                    new_modin_frame.columns = pandas.MultiIndex.from_tuples(
+                        columns_list, names=self.columns.names
+                    )
+            new_self = self.__constructor__(new_modin_frame)
+        else:
+            new_self = self.copy()
+            new_self.index = (
+                pandas.RangeIndex(len(new_self.index))
+                if new_index is None
+                else new_index
+            )
         return new_self
 
     def set_index_from_columns(
         self, keys: List[Hashable], drop: bool = True, append: bool = False
     ):
         """Create new row labels from a list of columns.
 
@@ -716,15 +808,14 @@
                 sum_cols = sum_cols.sum(axis=axis, skipna=False)
                 count_cols = count_cols.sum(axis=axis, skipna=False)
             return sum_cols / count_cols
 
         return MapReduceFunction.register(
             map_fn,
             reduce_fn,
-            preserve_index=(kwargs.get("numeric_only") is not None),
         )(self, axis=axis, **kwargs)
 
     def value_counts(self, **kwargs):
         """
         Return a QueryCompiler of Series containing counts of unique values.
 
         Returns
```

### Comparing `modin-0.9.0/modin/backends/pandas/__init__.py` & `modin-0.9.1/modin/backends/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/backends/pandas/parsers.py` & `modin-0.9.1/modin/backends/pandas/parsers.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/backends/pyarrow/query_compiler.py` & `modin-0.9.1/modin/backends/pyarrow/query_compiler.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/backends/pyarrow/__init__.py` & `modin-0.9.1/modin/backends/pyarrow/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/backends/pyarrow/parsers.py` & `modin-0.9.1/modin/backends/pyarrow/parsers.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/__init__.py` & `modin-0.9.1/modin/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/apply_license_header.py` & `modin-0.9.1/modin/apply_license_header.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/error_message.py` & `modin-0.9.1/modin/error_message.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/utils.py` & `modin-0.9.1/modin/utils.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/dask/pandas_on_dask/series/__init__.py` & `modin-0.9.1/modin/engines/ray/pandas_on_ray/series/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/dask/pandas_on_dask/io.py` & `modin-0.9.1/modin/engines/dask/pandas_on_dask/io.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/dask/pandas_on_dask/__init__.py` & `modin-0.9.1/modin/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/dask/pandas_on_dask/frame/partition.py` & `modin-0.9.1/modin/engines/dask/pandas_on_dask/frame/partition.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from modin.data_management.utils import length_fn_pandas, width_fn_pandas
 from modin.engines.base.frame.partition import BaseFramePartition
 
 from distributed.client import get_client
 from distributed import Future
 from distributed.utils import get_ip
 import cloudpickle as pkl
+from dask.distributed import wait
 
 
 def apply_list_of_funcs(funcs, df):
     for func, kwargs in funcs:
         if isinstance(func, bytes):
             func = pkl.loads(func)
         df = func(df, **kwargs)
@@ -96,14 +97,18 @@
         if len(self.call_queue) == 0:
             return
         new_partition = self.apply(lambda x: x)
         self.future = new_partition.future
         self._ip_cache = new_partition._ip_cache
         self.call_queue = []
 
+    def wait(self):
+        self.drain_call_queue()
+        wait(self.future)
+
     def mask(self, row_indices, col_indices):
         new_obj = self.add_to_apply_calls(
             lambda df: pandas.DataFrame(df.iloc[row_indices, col_indices])
         )
         if not isinstance(row_indices, slice):
             new_obj._length_cache = len(row_indices)
         if not isinstance(col_indices, slice):
```

### Comparing `modin-0.9.0/modin/engines/dask/pandas_on_dask/frame/__init__.py` & `modin-0.9.1/modin/experimental/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/dask/pandas_on_dask/frame/partition_manager.py` & `modin-0.9.1/modin/engines/dask/pandas_on_dask/frame/partition_manager.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/dask/pandas_on_dask/frame/axis_partition.py` & `modin-0.9.1/modin/engines/dask/pandas_on_dask/frame/axis_partition.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/dask/pandas_on_dask/frame/data.py` & `modin-0.9.1/modin/engines/dask/pandas_on_dask/frame/data.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/dask/task_wrapper.py` & `modin-0.9.1/modin/engines/dask/task_wrapper.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/dask/__init__.py` & `modin-0.9.1/modin/experimental/backends/omnisci/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/dask/utils.py` & `modin-0.9.1/modin/engines/python/pandas_on_python/io.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,29 +7,16 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 
-from modin.config import CpuCount
-from modin.error_message import ErrorMessage
+from modin.engines.base.io import BaseIO
+from modin.backends.pandas.query_compiler import PandasQueryCompiler
+from modin.engines.python.pandas_on_python.frame.data import PandasOnPythonFrame
 
 
-def initialize_dask():
-    from distributed.client import get_client
+class PandasOnPythonIO(BaseIO):
 
-    try:
-        get_client()
-    except ValueError:
-        from distributed import Client
-
-        # The indentation here is intentional, we want the code to be indented.
-        ErrorMessage.not_initialized(
-            "Dask",
-            """
-    from distributed import Client
-
-    client = Client()
-""",
-        )
-        Client(n_workers=CpuCount.get())
+    frame_cls = PandasOnPythonFrame
+    query_compiler_cls = PandasQueryCompiler
```

### Comparing `modin-0.9.0/modin/engines/python/__init__.py` & `modin-0.9.1/modin/experimental/cloud/test/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/python/pandas_on_python/series/__init__.py` & `modin-0.9.1/modin/experimental/cloud/tracing/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/python/pandas_on_python/io.py` & `modin-0.9.1/modin/pandas/test/internals/test_benchmark_mode.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 
-from modin.engines.base.io import BaseIO
-from modin.backends.pandas.query_compiler import PandasQueryCompiler
-from modin.engines.python.pandas_on_python.frame.data import PandasOnPythonFrame
+# test BenchmarkMode == True
 
+import modin.pandas as pd
+from modin.pandas.test.utils import test_data_values
+from modin.config import BenchmarkMode
 
-class PandasOnPythonIO(BaseIO):
 
-    frame_cls = PandasOnPythonFrame
-    query_compiler_cls = PandasQueryCompiler
+def test_syncronous_mode():
+    assert BenchmarkMode.get()
+    pd.DataFrame(test_data_values[0]).mean()
```

### Comparing `modin-0.9.0/modin/engines/python/pandas_on_python/__init__.py` & `modin-0.9.1/modin/experimental/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/python/pandas_on_python/frame/partition.py` & `modin-0.9.1/modin/engines/python/pandas_on_python/frame/partition.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,17 @@
         )
 
     def drain_call_queue(self):
         if len(self.call_queue) == 0:
             return
         self.apply(lambda x: x)
 
+    def wait(self):
+        self.drain_call_queue()
+
     def mask(self, row_indices=None, col_indices=None):
         new_obj = self.add_to_apply_calls(
             lambda df: pandas.DataFrame(df.iloc[row_indices, col_indices])
         )
         if not isinstance(row_indices, slice):
             new_obj._length_cache = len(row_indices)
         if not isinstance(col_indices, slice):
```

### Comparing `modin-0.9.0/modin/engines/python/pandas_on_python/frame/__init__.py` & `modin-0.9.1/modin/experimental/engines/omnisci_on_ray/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/python/pandas_on_python/frame/partition_manager.py` & `modin-0.9.1/modin/engines/python/pandas_on_python/frame/partition_manager.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/python/pandas_on_python/frame/axis_partition.py` & `modin-0.9.1/modin/engines/python/pandas_on_python/frame/axis_partition.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/python/pandas_on_python/frame/data.py` & `modin-0.9.1/modin/engines/python/pandas_on_python/frame/data.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/__init__.py` & `modin-0.9.1/modin/experimental/engines/omnisci_on_ray/frame/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/ray/pandas_on_ray/series/__init__.py` & `modin-0.9.1/modin/experimental/engines/omnisci_on_ray/test/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/ray/pandas_on_ray/io.py` & `modin-0.9.1/modin/engines/ray/pandas_on_ray/io.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/ray/pandas_on_ray/__init__.py` & `modin-0.9.1/modin/experimental/engines/pandas_on_ray/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/ray/pandas_on_ray/frame/__init__.py` & `modin-0.9.1/modin/experimental/engines/pyarrow_on_ray/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/ray/pandas_on_ray/frame/modin_aqp.py` & `modin-0.9.1/modin/engines/ray/pandas_on_ray/frame/modin_aqp.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/ray/pandas_on_ray/frame/partition_manager.py` & `modin-0.9.1/modin/engines/ray/pandas_on_ray/frame/partition_manager.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/ray/pandas_on_ray/frame/axis_partition.py` & `modin-0.9.1/modin/engines/ray/pandas_on_ray/frame/axis_partition.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/ray/pandas_on_ray/frame/data.py` & `modin-0.9.1/modin/engines/ray/pandas_on_ray/frame/data.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/ray/__init__.py` & `modin-0.9.1/modin/experimental/engines/pyarrow_on_ray/frame/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/ray/utils.py` & `modin-0.9.1/modin/engines/ray/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from modin.config import (
     IsRayCluster,
     RayRedisAddress,
     CpuCount,
     Memory,
     RayPlasmaDir,
     IsOutOfCore,
+    NPartitions,
 )
 
 
 def handle_ray_task_error(e):
     for s in e.traceback_str.split("\n")[::-1]:
         if "Error" in s or "Exception" in s:
             try:
@@ -160,7 +161,10 @@
             )
         _move_stdlib_ahead_of_site_packages()
         ray.worker.global_worker.run_function_on_all_workers(
             _move_stdlib_ahead_of_site_packages
         )
 
         ray.worker.global_worker.run_function_on_all_workers(_import_pandas)
+
+    num_cpus = int(ray.cluster_resources()["CPU"])
+    NPartitions.put_if_default(num_cpus)
```

### Comparing `modin-0.9.0/modin/engines/ray/generic/series/__init__.py` & `modin-0.9.1/modin/experimental/engines/pyarrow_on_ray/series/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/ray/generic/io.py` & `modin-0.9.1/modin/engines/ray/generic/io.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/ray/generic/__init__.py` & `modin-0.9.1/modin/experimental/pandas/test/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/ray/generic/frame/__init__.py` & `modin-0.9.1/modin/experimental/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/ray/generic/frame/partition_manager.py` & `modin-0.9.1/modin/engines/ray/generic/frame/partition_manager.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/base/series/__init__.py` & `modin-0.9.1/modin/experimental/xgboost/test/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/base/io/io.py` & `modin-0.9.1/modin/engines/base/io/io.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/base/io/__init__.py` & `modin-0.9.1/modin/engines/base/io/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/base/io/file_dispatcher.py` & `modin-0.9.1/modin/engines/base/io/file_dispatcher.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/base/io/column_stores/parquet_dispatcher.py` & `modin-0.9.1/modin/engines/base/io/column_stores/parquet_dispatcher.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/base/io/column_stores/__init__.py` & `modin-0.9.1/modin/pandas/test/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/base/io/column_stores/column_store_dispatcher.py` & `modin-0.9.1/modin/engines/base/io/column_stores/column_store_dispatcher.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/base/io/column_stores/hdf_dispatcher.py` & `modin-0.9.1/modin/engines/base/io/column_stores/hdf_dispatcher.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/base/io/text/json_dispatcher.py` & `modin-0.9.1/modin/engines/base/io/text/json_dispatcher.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/base/io/text/__init__.py` & `modin-0.9.1/modin/pandas/test/data/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/base/io/text/excel_dispatcher.py` & `modin-0.9.1/modin/engines/base/io/text/excel_dispatcher.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/base/io/text/text_file_dispatcher.py` & `modin-0.9.1/modin/engines/base/io/text/text_file_dispatcher.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/base/io/text/csv_glob_dispatcher.py` & `modin-0.9.1/modin/engines/base/io/text/csv_glob_dispatcher.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/base/io/text/csv_dispatcher.py` & `modin-0.9.1/modin/engines/base/io/text/csv_dispatcher.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/base/io/text/fwf_dispatcher.py` & `modin-0.9.1/modin/engines/base/io/text/fwf_dispatcher.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/base/io/sql/__init__.py` & `modin-0.9.1/modin/pandas/test/dataframe/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/base/io/sql/sql_dispatcher.py` & `modin-0.9.1/modin/engines/base/io/sql/sql_dispatcher.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/base/__init__.py` & `modin-0.9.1/modin/pandas/test/internals/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/base/frame/partition.py` & `modin-0.9.1/modin/engines/base/frame/partition.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,18 @@
         """
         pass
 
     def drain_call_queue(self):
         """Execute all functionality stored in the call queue."""
         pass
 
+    def wait(self):
+        """Wait for partition' computations result."""
+        pass
+
     def to_pandas(self):
         """Convert the object stored in this partition to a Pandas DataFrame.
 
         Note: If the underlying object is a Pandas DataFrame, this will likely
             only need to call `get`
 
         Returns
```

### Comparing `modin-0.9.0/modin/engines/base/frame/__init__.py` & `modin-0.9.1/modin/spreadsheet/test/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/base/frame/partition_manager.py` & `modin-0.9.1/modin/engines/base/frame/partition_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,52 @@
 from abc import ABC
 import numpy as np
 import pandas
 import warnings
 
 from modin.error_message import ErrorMessage
 from modin.data_management.utils import compute_chunksize
-from modin.config import NPartitions, ProgressBar
+from modin.config import NPartitions, ProgressBar, BenchmarkMode
 
 from pandas.api.types import union_categoricals
 import os
 
 
+def wait_computations_if_benchmark_mode(func):
+    """
+    Synchronize performing a function in benchmark mode.
+
+    Parameters
+    ----------
+    func: callable
+        A function that should be performed in syncronous mode.
+
+    Note
+    ----
+        `func` should return numpy array with partitions.
+    """
+    if BenchmarkMode.get():
+
+        def wait(*args, **kwargs):
+            """Wait for computation results."""
+            result = func(*args, **kwargs)
+            if isinstance(result, tuple):
+                partitions = result[0]
+            else:
+                partitions = result
+            # need to go through all the values of the map iterator
+            # since `wait` does not return anything, we need to explicitly add
+            # the return `True` value from the lambda
+            all(map(lambda partition: partition.wait() or True, partitions.flatten()))
+            return result
+
+        return wait
+    return func
+
+
 class BaseFrameManager(ABC):
     """Partition class is the class to use for storing each partition. It must extend the `BaseFramePartition` class.
 
     It is the base class for managing the dataframe data layout and operators.
     """
 
     _partition_class = None
@@ -140,14 +172,15 @@
         else:
             mapped_partitions = cls.map_partitions(partitions, map_func)
         return cls.map_axis_partitions(
             axis, mapped_partitions, reduce_func, enumerate_partitions=True
         )
 
     @classmethod
+    @wait_computations_if_benchmark_mode
     def broadcast_apply_select_indices(
         cls,
         axis,
         apply_func,
         left,
         right,
         left_indices,
@@ -210,14 +243,15 @@
             ]
         )
         if not axis:
             new_partitions = new_partitions.T
         return new_partitions
 
     @classmethod
+    @wait_computations_if_benchmark_mode
     def broadcast_apply(cls, axis, apply_func, left, right, other_name="r"):
         """Broadcast the right partitions to left and apply a function.
 
         Note: This will often be overridden by implementations. It materializes the
             entire partitions of the right and applies them to the left through `apply`.
 
         Parameters
@@ -257,14 +291,15 @@
                 for row_idx in range(len(left))
             ]
         )
 
         return new_partitions
 
     @classmethod
+    @wait_computations_if_benchmark_mode
     def broadcast_axis_partitions(
         cls,
         axis,
         apply_func,
         left,
         right,
         keep_partitioning=False,
@@ -334,14 +369,15 @@
         )
         # If we are mapping over columns, they are returned to use the same as
         # rows, so we need to transpose the returned 2D NumPy array to return
         # the structure to the correct order.
         return result_blocks.T if not axis else result_blocks
 
     @classmethod
+    @wait_computations_if_benchmark_mode
     def map_partitions(cls, partitions, map_func):
         """Apply `map_func` to every partition.
 
         Parameters
         ----------
         map_func: callable
            The function to apply.
@@ -355,14 +391,15 @@
             [
                 [part.apply(preprocessed_map_func) for part in row_of_parts]
                 for row_of_parts in partitions
             ]
         )
 
     @classmethod
+    @wait_computations_if_benchmark_mode
     def lazy_map_partitions(cls, partitions, map_func):
         """
         Apply `map_func` to every partition lazily.
 
         Parameters
         ----------
         map_func: callable
@@ -426,14 +463,15 @@
             keep_partitioning=keep_partitioning,
             right=None,
             lengths=lengths,
             enumerate_partitions=enumerate_partitions,
         )
 
     @classmethod
+    @wait_computations_if_benchmark_mode
     def simple_shuffle(cls, axis, partitions, map_func, lengths):
         """
         Shuffle data using `lengths` via `map_func`.
 
         Parameters
         ----------
             axis : 0 or 1
@@ -565,14 +603,15 @@
             A NumPy array
         """
         return np.block(
             [[block.to_numpy(**kwargs) for block in row] for row in partitions]
         )
 
     @classmethod
+    @wait_computations_if_benchmark_mode
     def from_pandas(cls, df, return_dims=False):
         """Return the partitions from Pandas DataFrame."""
 
         def update_bar(pbar, f):
             if ProgressBar.get():
                 pbar.update(1)
             return f
@@ -697,14 +736,15 @@
         -------
             A list of BaseFramePartition objects.
         """
         preprocessed_func = cls.preprocess_func(func)
         return [obj.apply(preprocessed_func, **kwargs) for obj in partitions]
 
     @classmethod
+    @wait_computations_if_benchmark_mode
     def apply_func_to_select_indices(
         cls, axis, partitions, func, indices, keep_remaining=False
     ):
         """Apply a function to select indices.
 
         Note: Your internal function must take a kwarg `internal_indices` for
             this to work correctly. This prevents information leakage of the
@@ -799,14 +839,15 @@
                         )
                         for i in range(len(partitions_for_apply))
                     ]
                 )
         return result.T if not axis else result
 
     @classmethod
+    @wait_computations_if_benchmark_mode
     def apply_func_to_select_indices_along_full_axis(
         cls, axis, partitions, func, indices, keep_remaining=False
     ):
         """Apply a function to a select subset of full columns/rows.
 
         Note: This should be used when you need to apply a function that relies
             on some global information for the entire column/row, but only need
@@ -908,14 +949,15 @@
                         )
                         for i in range(len(partitions_for_remaining))
                     ]
                 )
         return result.T if not axis else result
 
     @classmethod
+    @wait_computations_if_benchmark_mode
     def apply_func_to_indices_both_axis(
         cls,
         partitions,
         func,
         row_partitions_list,
         col_partitions_list,
         item_to_distribute=None,
@@ -954,14 +996,15 @@
                 )
                 partition_copy[row_blk_idx, col_blk_idx] = block_result
                 col_position_counter += len(col_internal_idx)
             row_position_counter += len(row_internal_idx)
         return partition_copy
 
     @classmethod
+    @wait_computations_if_benchmark_mode
     def binary_operation(cls, axis, left, func, right):
         """
         Apply a function that requires two BasePandasFrame objects.
 
         Parameters
         ----------
             axis : int
```

### Comparing `modin-0.9.0/modin/engines/base/frame/axis_partition.py` & `modin-0.9.1/modin/engines/base/frame/axis_partition.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/engines/base/frame/data.py` & `modin-0.9.1/modin/engines/base/frame/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -542,54 +542,66 @@
 
         Returns
         -------
         BasePandasFrame
             A new BasePandasFrame.
         """
         new_row_labels = pandas.RangeIndex(len(self.index))
-        # Column labels are different for multilevel index.
-        if len(self.index.names) > 1:
-            # We will also use the `new_column_names` in the calculation of the internal metadata, so this is a
-            # lightweight way of ensuring the metadata matches.
-            new_column_names = pandas.Index(
-                [
-                    self.index.names[i]
-                    if self.index.names[i] is not None
-                    else "level_{}".format(i)
-                    for i in range(len(self.index.names))
-                ]
-            )
-            new_columns = new_column_names.append(self.columns)
+
+        if self.index.nlevels > 1:
+            level_names = [
+                self.index.names[i]
+                if self.index.names[i] is not None
+                else "level_{}".format(i)
+                for i in range(self.index.nlevels)
+            ]
         else:
-            # See note above about usage of `new_column_names`.
-            new_column_names = pandas.Index(
+            level_names = [
+                self.index.names[0]
+                if self.index.names[0] is not None
+                else "index"
+                if "index" not in self.columns
+                else "level_{}".format(0)
+            ]
+
+        # We will also use the `new_column_names` in the calculation of the internal metadata, so this is a
+        # lightweight way of ensuring the metadata matches.
+        if self.columns.nlevels > 1:
+            # Column labels are different for multilevel index.
+            new_column_names = pandas.MultiIndex.from_tuples(
+                # Set level names on the 1st columns level and fill up empty level names with empty string.
+                # Expand tuples in level names. This is how reset_index works when col_level col_fill are not specified.
                 [
-                    self.index.names[0]
-                    if self.index.names[0] is not None
-                    else "index"
-                    if "index" not in self.columns
-                    else "level_{}".format(0)
-                ]
+                    tuple(
+                        list(level) + [""] * (self.columns.nlevels - len(level))
+                        if isinstance(level, tuple)
+                        else [level] + [""] * (self.columns.nlevels - 1)
+                    )
+                    for level in level_names
+                ],
+                names=self.columns.names,
             )
-            new_columns = new_column_names.append(self.columns)
+        else:
+            new_column_names = pandas.Index(level_names, tupleize_cols=False)
+        new_columns = new_column_names.append(self.columns)
 
         def from_labels_executor(df, **kwargs):
             # Setting the names here ensures that external and internal metadata always match.
             df.index.names = new_column_names
             return df.reset_index()
 
         new_parts = self._frame_mgr_cls.apply_func_to_select_indices(
             0,
             self._partitions,
             from_labels_executor,
             [0],
             keep_remaining=True,
         )
         new_column_widths = [
-            len(self.index.names) + self._column_widths[0]
+            self.index.nlevels + self._column_widths[0]
         ] + self._column_widths[1:]
         result = self.__constructor__(
             new_parts,
             new_row_labels,
             new_columns,
             row_lengths=self._row_lengths_cache,
             column_widths=new_column_widths,
@@ -957,15 +969,15 @@
         def merge(left_index, right_index):
             if axis == 1 and how == "outer" and not sort:
                 return left_index.union(right_index, sort=False)
             else:
                 return left_index.join(right_index, how=how, sort=sort)
 
         # define condition for joining indexes
-        all_indices_equal = all(indexes[0].equals(index) for index in [indexes[1:]])
+        all_indices_equal = all(indexes[0].equals(index) for index in indexes[1:])
         do_join_index = how is not None and not all_indices_equal
 
         # define condition for joining indexes with getting indexers
         need_indexers = (
             axis == 0
             and not all_indices_equal
             and any(not index.is_unique for index in indexes)
@@ -1040,66 +1052,58 @@
                 # consistent with what we have done. In the case of a reduction, the
                 # data for axis=0 should be a single value for each column. By
                 # transposing the data after we convert to a DataFrame, we ensure that
                 # the columns of the result line up with the columns from the data.
                 # axis=1 does not have this requirement because the index already will
                 # line up with the index of the data based on how pandas creates a
                 # DataFrame from a Series.
-                return pandas.DataFrame(series_result).T
-            return pandas.DataFrame(series_result)
+                result = pandas.DataFrame(series_result).T
+                result.index = ["__reduced__"]
+            else:
+                result = pandas.DataFrame(series_result)
+                if isinstance(series_result, pandas.Series):
+                    result.columns = ["__reduced__"]
+            return result
 
         return _map_reduce_func
 
-    def _compute_map_reduce_metadata(self, axis, new_parts, preserve_index=True):
+    def _compute_map_reduce_metadata(self, axis, new_parts):
         """
         Compute the metadata for the result of reduce function.
 
         Parameters
         ----------
         axis: int,
             The axis on which reduce function was applied
         new_parts: numpy 2D array
             Partitions with the result of applied function
-        preserve_index: boolean
-            The flag to preserve labels for the reduced axis.
 
         Returns
         -------
         BasePandasFrame
             Pandas series containing the reduced data.
         """
         new_axes, new_axes_lengths = [0, 0], [0, 0]
 
         new_axes[axis] = ["__reduced__"]
-        if preserve_index:
-            new_axes[axis ^ 1] = self.axes[axis ^ 1]
-        else:
-            new_axes[axis ^ 1] = self._compute_axis_labels(axis ^ 1, new_parts)
+        new_axes[axis ^ 1] = self.axes[axis ^ 1]
 
         new_axes_lengths[axis] = [1]
         new_axes_lengths[axis ^ 1] = self._axes_lengths[axis ^ 1]
 
-        if axis == 0 or self._dtypes is None:
-            new_dtypes = self._dtypes
-        elif preserve_index:
-            new_dtypes = pandas.Series(
-                [find_common_type(self.dtypes.values)], index=new_axes[axis]
-            )
-        else:
-            new_dtypes = None
+        new_dtypes = None
         result = self.__constructor__(
             new_parts,
             *new_axes,
             *new_axes_lengths,
             new_dtypes,
         )
-        result._apply_index_objs(axis)
         return result
 
-    def _fold_reduce(self, axis, func, preserve_index=True):
+    def _fold_reduce(self, axis, func):
         """
         Apply function that reduce Manager to series but require knowledge of full axis.
 
         Parameters
         ----------
             axis : 0 or 1
                 The axis to apply the function to (0 - index, 1 - columns).
@@ -1113,34 +1117,29 @@
         BasePandasFrame
             Pandas series containing the reduced data.
         """
         func = self._build_mapreduce_func(axis, func)
         new_parts = self._frame_mgr_cls.map_axis_partitions(
             axis, self._partitions, func
         )
-        return self._compute_map_reduce_metadata(
-            axis, new_parts, preserve_index=preserve_index
-        )
+        return self._compute_map_reduce_metadata(axis, new_parts)
 
-    def _map_reduce(self, axis, map_func, reduce_func=None, preserve_index=True):
+    def _map_reduce(self, axis, map_func, reduce_func=None):
         """
         Apply function that will reduce the data to a Pandas Series.
 
         Parameters
         ----------
             axis : 0 or 1
                 0 for columns and 1 for rows.
             map_func : callable
                 Callable function to map the dataframe.
             reduce_func : callable
                 Callable function to reduce the dataframe.
                 If none, then apply map_func twice. Default is None.
-            preserve_index : boolean
-                The flag to preserve index for default behavior
-                map and reduce operations. Default is True.
 
         Returns
         -------
         BasePandasFrame
             A new dataframe.
         """
         map_func = self._build_mapreduce_func(axis, map_func)
@@ -1149,17 +1148,15 @@
         else:
             reduce_func = self._build_mapreduce_func(axis, reduce_func)
 
         map_parts = self._frame_mgr_cls.map_partitions(self._partitions, map_func)
         reduce_parts = self._frame_mgr_cls.map_axis_partitions(
             axis, map_parts, reduce_func
         )
-        return self._compute_map_reduce_metadata(
-            axis, reduce_parts, preserve_index=preserve_index
-        )
+        return self._compute_map_reduce_metadata(axis, reduce_parts)
 
     def _map(self, func, dtypes=None, validate_index=False, validate_columns=False):
         """Perform a function that maps across the entire dataset.
 
         Parameters
         ----------
             func : callable
@@ -1767,16 +1764,14 @@
         ]
 
         # If all frames are empty
         if len(non_empty_frames_idx) == 0:
             return self._partitions, [o._partitions for o in other], joined_index
 
         base_frame_idx = non_empty_frames_idx[0]
-        base_frame = frames[base_frame_idx]
-
         other_frames = frames[base_frame_idx + 1 :]
 
         # Picking first non-empty frame
         base_frame = frames[non_empty_frames_idx[0]]
         base_index = base_frame.axes[axis]
 
         # define conditions for reindexing and repartitioning `self` frame
@@ -2130,7 +2125,16 @@
             new_partitions,
             self.columns,
             self.index,
             self._column_widths,
             self._row_lengths,
             dtypes=new_dtypes,
         )
+
+    def finalize(self):
+        """
+        Perform all deferred calls on partitions.
+
+        This makes the Frame independent of history of queries
+        that were used to build it.
+        """
+        [part.drain_call_queue() for row in self._partitions for part in row]
```

### Comparing `modin-0.9.0/modin/pandas/accessor.py` & `modin-0.9.1/modin/pandas/accessor.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/pandas/test/dataframe/test_iter.py` & `modin-0.9.1/modin/pandas/test/dataframe/test_iter.py`

 * *Files 4% similar despite different names*

```diff
@@ -226,46 +226,14 @@
 "2016-08-26 09:00:20.578",3,60.152996,24.745216,3.90000009536743,"STILL",69,"IN_VEHICLE",31,"UNKNOWN",0"""
     pandas_df = pandas.read_csv(io.StringIO(string_data))
     modin_df = pd.read_csv(io.StringIO(string_data))
     assert repr(pandas_df) == repr(modin_df)
 
 
 @pytest.mark.parametrize("data", test_data_values, ids=test_data_keys)
-def test_reset_index_with_multi_index(data):
-    modin_df = pd.DataFrame(data)
-    pandas_df = pandas.DataFrame(data)
-
-    if len(modin_df.columns) > len(pandas_df.columns):
-        col0 = modin_df.columns[0]
-        col1 = modin_df.columns[1]
-        modin_cols = modin_df.groupby([col0, col1]).count().reset_index().columns
-        pandas_cols = pandas_df.groupby([col0, col1]).count().reset_index().columns
-
-        assert modin_cols.equals(pandas_cols)
-
-
-def test_reset_index_with_named_index():
-    modin_df = pd.DataFrame(test_data_values[0])
-    pandas_df = pandas.DataFrame(test_data_values[0])
-
-    modin_df.index.name = pandas_df.index.name = "NAME_OF_INDEX"
-    df_equals(modin_df, pandas_df)
-    df_equals(modin_df.reset_index(drop=False), pandas_df.reset_index(drop=False))
-
-    modin_df.reset_index(drop=True, inplace=True)
-    pandas_df.reset_index(drop=True, inplace=True)
-    df_equals(modin_df, pandas_df)
-
-    modin_df = pd.DataFrame(test_data_values[0])
-    pandas_df = pandas.DataFrame(test_data_values[0])
-    modin_df.index.name = pandas_df.index.name = "NEW_NAME"
-    df_equals(modin_df.reset_index(drop=False), pandas_df.reset_index(drop=False))
-
-
-@pytest.mark.parametrize("data", test_data_values, ids=test_data_keys)
 def test_inplace_series_ops(data):
     pandas_df = pandas.DataFrame(data)
     modin_df = pd.DataFrame(data)
 
     if len(modin_df.columns) > len(pandas_df.columns):
         col0 = modin_df.columns[0]
         col1 = modin_df.columns[1]
```

### Comparing `modin-0.9.0/modin/pandas/test/dataframe/test_map_metadata.py` & `modin-0.9.1/modin/pandas/test/dataframe/test_map_metadata.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/pandas/test/dataframe/__init__.py` & `modin-0.9.1/modin/test/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/pandas/test/dataframe/test_indexing.py` & `modin-0.9.1/modin/pandas/test/dataframe/test_indexing.py`

 * *Files 20% similar despite different names*

```diff
@@ -31,14 +31,16 @@
     test_data_keys,
     axis_keys,
     axis_values,
     int_arg_keys,
     int_arg_values,
     create_test_dfs,
     eval_general,
+    generate_multiindex,
+    extra_test_parameters,
 )
 from modin.config import NPartitions
 
 NPartitions.put(4)
 
 # Force matplotlib to not use any Xwindows backend.
 matplotlib.use("Agg")
@@ -919,14 +921,276 @@
     modin_df_cp = modin_df.copy()
     pd_df_cp = pandas_df.copy()
     modin_df_cp.reset_index(inplace=True)
     pd_df_cp.reset_index(inplace=True)
     df_equals(modin_df_cp, pd_df_cp)
 
 
+@pytest.mark.parametrize(
+    "data",
+    [
+        pytest.param(
+            test_data["int_data"],
+            marks=pytest.mark.skipif(not extra_test_parameters, reason="extra"),
+        ),
+        test_data["float_nan_data"],
+    ],
+    ids=["int_data", "float_nan_data"],
+)
+@pytest.mark.parametrize("nlevels", [3])
+@pytest.mark.parametrize("columns_multiindex", [True, False])
+@pytest.mark.parametrize(
+    "level",
+    [
+        "no_level",
+        None,
+        0,
+        1,
+        2,
+        [2, 0],
+        [2, 1],
+        [1, 0],
+        pytest.param(
+            [2, 1, 2],
+            marks=pytest.mark.skipif(not extra_test_parameters, reason="extra"),
+        ),
+        pytest.param(
+            [0, 0, 0, 0],
+            marks=pytest.mark.skipif(not extra_test_parameters, reason="extra"),
+        ),
+        pytest.param(
+            ["level_name_1"],
+            marks=pytest.mark.skipif(not extra_test_parameters, reason="extra"),
+        ),
+        pytest.param(
+            ["level_name_2", "level_name_1"],
+            marks=pytest.mark.skipif(not extra_test_parameters, reason="extra"),
+        ),
+        pytest.param(
+            [2, "level_name_0"],
+            marks=pytest.mark.skipif(not extra_test_parameters, reason="extra"),
+        ),
+    ],
+)
+@pytest.mark.parametrize("col_level", ["no_col_level", 0, 1, 2])
+@pytest.mark.parametrize("col_fill", ["no_col_fill", None, 0, "new"])
+@pytest.mark.parametrize("drop", [False])
+@pytest.mark.parametrize(
+    "multiindex_levels_names_max_levels",
+    [
+        0,
+        1,
+        2,
+        pytest.param(
+            3, marks=pytest.mark.skipif(not extra_test_parameters, reason="extra")
+        ),
+        pytest.param(
+            4, marks=pytest.mark.skipif(not extra_test_parameters, reason="extra")
+        ),
+    ],
+)
+@pytest.mark.parametrize(
+    "none_in_index_names",
+    [
+        pytest.param(
+            False,
+            marks=pytest.mark.skipif(not extra_test_parameters, reason="extra"),
+        ),
+        True,
+        "mixed_1st_None",
+        pytest.param(
+            "mixed_2nd_None",
+            marks=pytest.mark.skipif(not extra_test_parameters, reason="extra"),
+        ),
+    ],
+)
+def test_reset_index_with_multi_index_no_drop(
+    data,
+    nlevels,
+    columns_multiindex,
+    level,
+    col_level,
+    col_fill,
+    drop,
+    multiindex_levels_names_max_levels,
+    none_in_index_names,
+):
+    data_rows = len(data[list(data.keys())[0]])
+    index = generate_multiindex(data_rows, nlevels=nlevels)
+    data_columns = len(data.keys())
+    columns = (
+        generate_multiindex(data_columns, nlevels=nlevels)
+        if columns_multiindex
+        else pandas.RangeIndex(0, data_columns)
+    )
+    # Replace original data columns with generated
+    data = {columns[ind]: data[key] for ind, key in enumerate(data)}
+    index.names = (
+        [f"level_{i}" for i in range(index.nlevels)]
+        if multiindex_levels_names_max_levels == 0
+        else [
+            tuple(
+                [
+                    f"level_{i}_name_{j}"
+                    for j in range(
+                        0,
+                        max(multiindex_levels_names_max_levels + 1 - index.nlevels, 0)
+                        + i,
+                    )
+                ]
+            )
+            if max(multiindex_levels_names_max_levels + 1 - index.nlevels, 0) + i > 0
+            else f"level_{i}"
+            for i in range(index.nlevels)
+        ]
+    )
+
+    if none_in_index_names is True:
+        index.names = [None] * len(index.names)
+    elif none_in_index_names:
+        names_list = list(index.names)
+        start_index = 0 if none_in_index_names == "mixed_1st_None" else 1
+        names_list[start_index::2] = [None] * len(names_list[start_index::2])
+        index.names = names_list
+
+    modin_df = pd.DataFrame(data, index=index, columns=columns)
+    pandas_df = pandas.DataFrame(data, index=index, columns=columns)
+
+    if isinstance(level, list):
+        level = [
+            index.names[int(x[len("level_name_") :])]
+            if isinstance(x, str) and x.startswith("level_name_")
+            else x
+            for x in level
+        ]
+
+    kwargs = {"drop": drop}
+    if level != "no_level":
+        kwargs["level"] = level
+    if col_level != "no_col_level":
+        kwargs["col_level"] = col_level
+    if col_fill != "no_col_fill":
+        kwargs["col_fill"] = col_fill
+    eval_general(modin_df, pandas_df, lambda df: df.reset_index(**kwargs))
+
+
+@pytest.mark.parametrize(
+    "data",
+    [
+        pytest.param(
+            test_data["int_data"],
+            marks=pytest.mark.skipif(not extra_test_parameters, reason="extra"),
+        ),
+        test_data["float_nan_data"],
+    ],
+    ids=["int_data", "float_nan_data"],
+)
+@pytest.mark.parametrize("nlevels", [3])
+@pytest.mark.parametrize(
+    "level",
+    [
+        "no_level",
+        None,
+        0,
+        1,
+        2,
+        [2, 0],
+        [2, 1],
+        [1, 0],
+        pytest.param(
+            [2, 1, 2],
+            marks=pytest.mark.skipif(not extra_test_parameters, reason="extra"),
+        ),
+        pytest.param(
+            [0, 0, 0, 0],
+            marks=pytest.mark.skipif(not extra_test_parameters, reason="extra"),
+        ),
+        pytest.param(
+            ["level_name_1"],
+            marks=pytest.mark.skipif(not extra_test_parameters, reason="extra"),
+        ),
+        pytest.param(
+            ["level_name_2", "level_name_1"],
+            marks=pytest.mark.skipif(not extra_test_parameters, reason="extra"),
+        ),
+        pytest.param(
+            [2, "level_name_0"],
+            marks=pytest.mark.skipif(not extra_test_parameters, reason="extra"),
+        ),
+    ],
+)
+@pytest.mark.parametrize(
+    "multiindex_levels_names_max_levels",
+    [
+        0,
+        1,
+        2,
+        pytest.param(
+            3, marks=pytest.mark.skipif(not extra_test_parameters, reason="extra")
+        ),
+        pytest.param(
+            4, marks=pytest.mark.skipif(not extra_test_parameters, reason="extra")
+        ),
+    ],
+)
+@pytest.mark.parametrize(
+    "none_in_index_names",
+    [
+        pytest.param(
+            False,
+            marks=pytest.mark.skipif(not extra_test_parameters, reason="extra"),
+        ),
+        True,
+        "mixed_1st_None",
+        pytest.param(
+            "mixed_2nd_None",
+            marks=pytest.mark.skipif(not extra_test_parameters, reason="extra"),
+        ),
+    ],
+)
+def test_reset_index_with_multi_index_drop(
+    data, nlevels, level, multiindex_levels_names_max_levels, none_in_index_names
+):
+    test_reset_index_with_multi_index_no_drop(
+        data,
+        nlevels,
+        True,
+        level,
+        "no_col_level",
+        "no_col_fill",
+        True,
+        multiindex_levels_names_max_levels,
+        none_in_index_names,
+    )
+
+
+@pytest.mark.parametrize("index_levels_names_max_levels", [0, 1, 2])
+def test_reset_index_with_named_index(index_levels_names_max_levels):
+    modin_df = pd.DataFrame(test_data_values[0])
+    pandas_df = pandas.DataFrame(test_data_values[0])
+
+    index_name = (
+        tuple([f"name_{j}" for j in range(0, index_levels_names_max_levels)])
+        if index_levels_names_max_levels > 0
+        else "NAME_OF_INDEX"
+    )
+    modin_df.index.name = pandas_df.index.name = index_name
+    df_equals(modin_df, pandas_df)
+    df_equals(modin_df.reset_index(drop=False), pandas_df.reset_index(drop=False))
+
+    modin_df.reset_index(drop=True, inplace=True)
+    pandas_df.reset_index(drop=True, inplace=True)
+    df_equals(modin_df, pandas_df)
+
+    modin_df = pd.DataFrame(test_data_values[0])
+    pandas_df = pandas.DataFrame(test_data_values[0])
+    modin_df.index.name = pandas_df.index.name = index_name
+    df_equals(modin_df.reset_index(drop=False), pandas_df.reset_index(drop=False))
+
+
 @pytest.mark.parametrize("data", test_data_values, ids=test_data_keys)
 @pytest.mark.parametrize("axis", axis_values, ids=axis_keys)
 def test_sample(data, axis):
     modin_df = pd.DataFrame(data)
     pandas_df = pandas.DataFrame(data)
 
     with pytest.raises(ValueError):
```

### Comparing `modin-0.9.0/modin/pandas/test/dataframe/test_udf.py` & `modin-0.9.1/modin/pandas/test/dataframe/test_udf.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/pandas/test/dataframe/test_reduction.py` & `modin-0.9.1/modin/pandas/test/dataframe/test_reduction.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,14 +128,25 @@
     eval_general(
         modin_df,
         pandas_df,
         lambda df: df.count(axis=axis, level=level),
     )
 
 
+@pytest.mark.parametrize("data", test_data_values, ids=test_data_keys)
+def test_count_dtypes(data):
+    modin_df, pandas_df = pd.DataFrame(data), pandas.DataFrame(data)
+
+    eval_general(
+        modin_df,
+        pandas_df,
+        lambda df: df.isna().count(axis=0),
+    )
+
+
 @pytest.mark.parametrize("percentiles", [None, 0.10, 0.11, 0.44, 0.78, 0.99])
 @pytest.mark.parametrize("data", test_data_values, ids=test_data_keys)
 def test_describe(data, percentiles):
     eval_general(
         *create_test_dfs(data),
         lambda df: df.describe(percentiles=percentiles),
     )
```

### Comparing `modin-0.9.0/modin/pandas/test/dataframe/test_binary.py` & `modin-0.9.1/modin/pandas/test/dataframe/test_binary.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,7 +237,8 @@
 def test_duplicate_indexes():
     data = [0, 1, 2, 3, 4, 5]
     modin_df1, pandas_df1 = create_test_dfs(
         {"a": data, "b": data}, index=[0, 1, 2, 0, 1, 2]
     )
     modin_df2, pandas_df2 = create_test_dfs({"a": data, "b": data})
     df_equals(modin_df1 / modin_df2, pandas_df1 / pandas_df2)
+    df_equals(modin_df1 / modin_df1, pandas_df1 / pandas_df1)
```

### Comparing `modin-0.9.0/modin/pandas/test/dataframe/test_default.py` & `modin-0.9.1/modin/pandas/test/dataframe/test_default.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,14 @@
         ("from_records", lambda df: {"data": to_pandas(df)}),
         ("hist", lambda df: {"column": "int_col"}),
         ("infer_objects", None),
         ("interpolate", None),
         ("lookup", lambda df: {"row_labels": [0], "col_labels": ["int_col"]}),
         ("mask", lambda df: {"cond": df != 0}),
         ("pct_change", None),
-        ("__getstate__", None),
         ("to_xarray", None),
         ("flags", None),
         ("set_flags", lambda df: {"allows_duplicate_labels": False}),
     ],
 )
 def test_ops_defaulting_to_pandas(op, make_args):
     modin_df = pd.DataFrame(test_data_diff_dtype).drop(["str_col", "bool_col"], axis=1)
@@ -84,23 +83,14 @@
 
 def test_style():
     data = test_data_values[0]
     with pytest.warns(UserWarning):
         pd.DataFrame(data).style
 
 
-def test___setstate__():
-    data = test_data_values[0]
-    with pytest.warns(UserWarning):
-        try:
-            pd.DataFrame(data).__setstate__(None)
-        except TypeError:
-            pass
-
-
 def test_to_timestamp():
     idx = pd.date_range("1/1/2012", periods=5, freq="M")
     df = pd.DataFrame(np.random.randint(0, 100, size=(len(idx), 4)), index=idx)
 
     with pytest.warns(UserWarning):
         df.to_period().to_timestamp()
```

### Comparing `modin-0.9.0/modin/pandas/test/dataframe/test_window.py` & `modin-0.9.1/modin/pandas/test/dataframe/test_window.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/pandas/test/dataframe/test_join_sort.py` & `modin-0.9.1/modin/pandas/test/dataframe/test_join_sort.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/pandas/test/test_rolling.py` & `modin-0.9.1/modin/pandas/test/test_rolling.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/pandas/test/__init__.py` & `modin-0.9.1/modin/sql/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,7 +6,11 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
+
+from .connection import connect
+
+__all__ = ["connect"]
```

### Comparing `modin-0.9.0/modin/pandas/test/test_reshape.py` & `modin-0.9.1/modin/pandas/test/test_reshape.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/pandas/test/test_io.py` & `modin-0.9.1/modin/pandas/test/test_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -349,15 +349,24 @@
         )
 
     @pytest.mark.parametrize("true_values", [["Yes"], ["Yes", "true"], None])
     @pytest.mark.parametrize("false_values", [["No"], ["No", "false"], None])
     @pytest.mark.parametrize("skiprows", [2, lambda x: x % 2])
     @pytest.mark.parametrize("skipfooter", [0, 10])
     @pytest.mark.parametrize("nrows", [35, None])
-    @pytest.mark.parametrize("names", [["c1", "c2", "c3", "c4"], None])
+    @pytest.mark.parametrize(
+        "names",
+        [
+            pytest.param(
+                ["c1", "c2", "c3", "c4"],
+                marks=pytest.mark.xfail(reason="Excluded because of the issue #2845"),
+            ),
+            None,
+        ],
+    )
     def test_read_csv_parsing_2(
         self,
         request,
         true_values,
         false_values,
         skiprows,
         skipfooter,
@@ -1275,15 +1284,14 @@
                 df_modin = pd.read_json(buf)
                 df_equals(df_pandas, df_modin)
         finally:
             teardown_test_files([unique_filename])
 
 
 class TestExcel:
-    @pytest.mark.xfail(reason="read_excel is broken for now, see #1733 for details")
     @check_file_leaks
     def test_read_excel(self):
         unique_filename = get_unique_filename(extension="xlsx")
         try:
             setup_excel_file(filename=unique_filename)
             eval_io(
                 fn_name="read_excel",
@@ -1832,14 +1840,18 @@
         modin_df, pandas_df = create_test_dfs(TEST_DATA)
         eval_to_file(
             modin_obj=modin_df, pandas_obj=pandas_df, fn="to_stata", extension="stata"
         )
 
 
 class TestFeather:
+    @pytest.mark.xfail(
+        Engine.get() != "Python",
+        reason="Excluded because of the issue #2845",
+    )
     def test_read_feather(self):
         unique_filename = get_unique_filename(extension="feather")
         try:
             setup_feather_file(filename=unique_filename)
 
             eval_io(
                 fn_name="read_feather",
```

### Comparing `modin-0.9.0/modin/pandas/test/utils.py` & `modin-0.9.1/modin/pandas/test/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,18 @@
 from io import BytesIO
 import os
 from string import ascii_letters
 import csv
 import psutil
 import functools
 
+# Flag activated on command line with "--extra-test-parameters" option.
+# Used in some tests to perform additional parameter combinations.
+extra_test_parameters = False
+
 random_state = np.random.RandomState(seed=42)
 
 DATASET_SIZE_DICT = {
     "Small": (2 ** 2, 2 ** 3),
     "Normal": (2 ** 6, 2 ** 8),
     "Big": (2 ** 7, 2 ** 12),
 }
```

### Comparing `modin-0.9.0/modin/pandas/test/test_concat.py` & `modin-0.9.1/modin/pandas/test/test_concat.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/pandas/test/test_groupby.py` & `modin-0.9.1/modin/pandas/test/test_groupby.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/pandas/test/test_api.py` & `modin-0.9.1/modin/pandas/test/test_api.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/pandas/test/test_general.py` & `modin-0.9.1/modin/pandas/test/test_general.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/pandas/test/data/issue_2239.csv` & `modin-0.9.1/modin/pandas/test/data/issue_2239.csv`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/pandas/test/data/blah.csv` & `modin-0.9.1/modin/pandas/test/data/blah.csv`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/pandas/test/data/newlines.csv` & `modin-0.9.1/modin/pandas/test/data/newlines.csv`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/pandas/test/data/issue_976.csv` & `modin-0.9.1/modin/pandas/test/data/issue_976.csv`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/pandas/test/test_series.py` & `modin-0.9.1/modin/pandas/test/test_series.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/pandas/series_utils.py` & `modin-0.9.1/modin/pandas/series_utils.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/pandas/dataframe.py` & `modin-0.9.1/modin/pandas/dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 import numpy as np
 import sys
 from typing import IO, Optional, Sequence, Tuple, Union, Mapping, Iterator
 import warnings
 
 from modin.error_message import ErrorMessage
 from modin.utils import _inherit_docstrings, to_pandas, hashable
-from modin.config import Engine, IsExperimental
+from modin.config import Engine, IsExperimental, PersistentPickle
 from .utils import (
     from_pandas,
     from_non_pandas,
 )
 from . import _update_engine
 from .iterator import PartitionIterator
 from .series import Series
@@ -2090,17 +2090,14 @@
 
     def __contains__(self, key):
         return self.columns.__contains__(key)
 
     def __round__(self, decimals=0):
         return self._default_to_pandas(pandas.DataFrame.__round__, decimals=decimals)
 
-    def __setstate__(self, state):
-        return self._default_to_pandas(pandas.DataFrame.__setstate__, state)
-
     def __delitem__(self, key):
         if key not in self:
             raise KeyError(key)
         self._update_inplace(new_query_compiler=self._query_compiler.delitem(key))
 
     __add__ = add
     __iadd__ = add  # pragma: no cover
@@ -2412,12 +2409,35 @@
             return self.where(key)
         elif is_mi_columns:
             return self._default_to_pandas(pandas.DataFrame.__getitem__, key)
             # return self._getitem_multilevel(key)
         else:
             return self._getitem_column(key)
 
+    # Persistance support methods - BEGIN
+    @classmethod
+    def _inflate_light(cls, query_compiler):
+        """
+        Re-creates the object from previously-serialized lightweight representation.
+
+        The method is used for faster but not disk-storable persistence.
+        """
+        return cls(query_compiler=query_compiler)
+
+    @classmethod
+    def _inflate_full(cls, pandas_df):
+        """Re-creates the object from previously-serialized disk-storable representation."""
+        return cls(data=from_pandas(pandas_df))
+
+    def __reduce__(self):
+        self._query_compiler.finalize()
+        if PersistentPickle.get():
+            return self._inflate_full, (self._to_pandas(),)
+        return self._inflate_light, (self._query_compiler,)
+
+    # Persistance support methods - END
+
 
 if IsExperimental.get():
     from modin.experimental.cloud.meta_magic import make_wrapped_class
 
     make_wrapped_class(DataFrame, "make_dataframe_wrapper")
```

### Comparing `modin-0.9.0/modin/pandas/plotting.py` & `modin-0.9.1/modin/pandas/plotting.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/pandas/io.py` & `modin-0.9.1/modin/pandas/io.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/pandas/series.py` & `modin-0.9.1/modin/pandas/series.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from pandas._libs.lib import no_default
 from pandas._typing import IndexKeyFunc
 import sys
 from typing import Union, Optional
 import warnings
 
 from modin.utils import _inherit_docstrings, to_pandas, Engine
-from modin.config import IsExperimental
+from modin.config import IsExperimental, PersistentPickle
 from .base import BasePandasDataset, _ATTRS_NO_LOOKUP
 from .iterator import PartitionIterator
 from .utils import from_pandas, is_scalar
 from .accessor import CachedAccessor, SparseAccessor
 from . import _update_engine
 
 
@@ -1730,12 +1730,29 @@
                     result = self._query_compiler.getitem_row_array(key)
             except TypeError:
                 result = self._query_compiler.getitem_row_array(key)
         if reduce_dimension:
             return self._reduce_dimension(result)
         return self.__constructor__(query_compiler=result)
 
+    # Persistance support methods - BEGIN
+    @classmethod
+    def _inflate_light(cls, query_compiler, name):
+        return cls(query_compiler=query_compiler, name=name)
+
+    @classmethod
+    def _inflate_full(cls, pandas_series):
+        return cls(data=pandas_series)
+
+    def __reduce__(self):
+        self._query_compiler.finalize()
+        if PersistentPickle.get():
+            return self._inflate_full, (self._to_pandas(),)
+        return self._inflate_light, (self._query_compiler, self.name)
+
+    # Persistance support methods - END
+
 
 if IsExperimental.get():
     from modin.experimental.cloud.meta_magic import make_wrapped_class
 
     make_wrapped_class(Series, "make_series_wrapper")
```

### Comparing `modin-0.9.0/modin/pandas/__init__.py` & `modin-0.9.1/modin/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/pandas/iterator.py` & `modin-0.9.1/modin/pandas/iterator.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/pandas/utils.py` & `modin-0.9.1/modin/pandas/utils.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/pandas/indexing.py` & `modin-0.9.1/modin/pandas/indexing.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/pandas/groupby.py` & `modin-0.9.1/modin/pandas/groupby.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/pandas/base.py` & `modin-0.9.1/modin/pandas/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,43 @@
 # special meaning and needs to be distinguished from a user explicitly passing None.
 sentinel = object()
 
 # Do not lookup certain attributes in columns or index, as they're used for some
 # special purposes, like serving remote context
 _ATTRS_NO_LOOKUP = {"____id_pack__", "__name__"}
 
+_DEFAULT_BEHAVIOUR = {
+    "__init__",
+    "__class__",
+    "_get_index",
+    "_set_index",
+    "empty",
+    "index",
+    "columns",
+    "name",
+    "dtypes",
+    "dtype",
+    "_get_name",
+    "_set_name",
+    "_default_to_pandas",
+    "_query_compiler",
+    "_to_pandas",
+    "_build_repr_df",
+    "_reduce_dimension",
+    "__repr__",
+    "__len__",
+    "_create_or_update_from_compiler",
+    "_update_inplace",
+    # for persistance support;
+    # see DataFrame methods docstrings for more
+    "_inflate_light",
+    "_inflate_full",
+    "__reduce__",
+} | _ATTRS_NO_LOOKUP
+
 
 class BasePandasDataset(object):
     """
     Implement most of the common code that exists in DataFrame/Series.
 
     Since both objects share the same underlying representation, and the algorithms
     are the same, we use this object to define the general behavior of those objects
@@ -1836,15 +1865,18 @@
             not drop
             and not self._query_compiler.has_multiindex()
             and all(n in self.columns for n in ["level_0", "index"])
         ):
             raise ValueError("cannot insert level_0, already exists")
         else:
             new_query_compiler = self._query_compiler.reset_index(
-                drop=drop, level=level
+                drop=drop,
+                level=level,
+                col_level=col_level,
+                col_fill=col_fill,
             )
         return self._create_or_update_from_compiler(new_query_compiler, inplace)
 
     def rfloordiv(self, other, axis="columns", level=None, fill_value=None):
         return self._binary_op(
             "rfloordiv", other, axis=axis, level=level, fill_value=fill_value
         )
@@ -2720,17 +2752,14 @@
         self.iloc[indexer] = value
 
     def _getitem_slice(self, key: slice):
         if key.start is None and key.stop is None:
             return self.copy()
         return self.iloc[key]
 
-    def __getstate__(self):
-        return self._default_to_pandas("__getstate__")
-
     def __gt__(self, right):
         return self.gt(right)
 
     def __invert__(self):
         if not all(is_numeric_dtype(d) for d in self._get_dtypes()):
             raise TypeError(
                 "bad operand type for unary ~: '{}'".format(
@@ -2791,38 +2820,15 @@
         return len(self._query_compiler.index) * len(self._query_compiler.columns)
 
     @property
     def values(self):
         return self.to_numpy()
 
     def __getattribute__(self, item):
-        default_behaviors = {
-            "__init__",
-            "__class__",
-            "_get_index",
-            "_set_index",
-            "empty",
-            "index",
-            "columns",
-            "name",
-            "dtypes",
-            "dtype",
-            "_get_name",
-            "_set_name",
-            "_default_to_pandas",
-            "_query_compiler",
-            "_to_pandas",
-            "_build_repr_df",
-            "_reduce_dimension",
-            "__repr__",
-            "__len__",
-            "_create_or_update_from_compiler",
-            "_update_inplace",
-        } | _ATTRS_NO_LOOKUP
-        if item not in default_behaviors and not self._query_compiler.lazy_execution:
+        if item not in _DEFAULT_BEHAVIOUR and not self._query_compiler.lazy_execution:
             method = object.__getattribute__(self, item)
             is_callable = callable(method)
             # We default to pandas on empty DataFrames. This avoids a large amount of
             # pain in underlying implementation and returns a result immediately rather
             # than dealing with the edge cases that empty DataFrames have.
             if is_callable and self.empty:
```

### Comparing `modin-0.9.0/modin/pandas/general.py` & `modin-0.9.1/modin/pandas/general.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin/sql/connection.py` & `modin-0.9.1/modin/sql/connection.py`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/setup.cfg` & `modin-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `modin-0.9.0/modin.egg-info/PKG-INFO` & `modin-0.9.1/modin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: modin
-Version: 0.9.0
+Version: 0.9.1
 Summary: Modin: Make your pandas code run faster by changing one line of code.
 Home-page: https://github.com/modin-project/modin
 License: Apache 2
 Description: <p align="center"><a href="https://modin.readthedocs.io"><img width=77% alt="" src="https://github.com/modin-project/modin/blob/3d6368edf311995ad231ec5342a51cd9e4e3dc20/docs/img/MODIN_ver2_hrz.png?raw=true"></a></p>
         <h2 align="center">Scale your pandas workflows by changing one line of code</h2>
         
         <p align="center">
         <a href="https://discuss.modin.org"><img alt="" src="https://img.shields.io/badge/discourse-forum-purple.svg?logo=discourse&logoColor=white" align="center"></a>
         <a href="https://codecov.io/gh/modin-project/modin"><img src="https://codecov.io/gh/modin-project/modin/branch/master/graph/badge.svg" align="center"/></a>
         <a href="https://github.com/modin-project/modin/actions"><img src="https://github.com/modin-project/modin/workflows/master/badge.svg" align="center"></a>
         <a href="https://modin.readthedocs.io/en/latest/?badge=latest"><img alt="" src="https://readthedocs.org/projects/modin/badge/?version=latest" align="center"></a>
-        <a href="https://pypi.org/project/modin/"><img alt="" src="https://img.shields.io/badge/pypi-0.9.0-blue.svg" align="center"></a>
+        <a href="https://pypi.org/project/modin/"><img alt="" src="https://img.shields.io/badge/pypi-0.9.1-blue.svg" align="center"></a>
         </p>
         
         <p align="center"><b>To use Modin, replace the pandas import:</b></p>
         
         ```python
         # import pandas as pd
         import modin.pandas as pd
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: modin Version: 0.9.0 Summary: Modin: Make your
+Metadata-Version: 2.1 Name: modin Version: 0.9.1 Summary: Modin: Make your
 pandas code run faster by changing one line of code. Home-page: https://
 github.com/modin-project/modin License: Apache 2 Description:
      ***** Scale your pandas workflows by changing one line of code *****
    [https://codecov.io/gh/modin-project/modin/branch/master/graph/badge.svg]
      [https://github.com/modin-project/modin/workflows/master/badge.svg]
                    To use Modin, replace the pandas import:
 ```python # import pandas as pd import modin.pandas as pd ``` ### Installation
```

### Comparing `modin-0.9.0/versioneer.py` & `modin-0.9.1/versioneer.py`

 * *Files identical despite different names*

