# Comparing `tmp/pyperformance-1.0.8.tar.gz` & `tmp/pyperformance-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyperformance-1.0.8.tar", last modified: Fri Jun  2 11:47:16 2023, max compression
+gzip compressed data, was "pyperformance-1.0.9.tar", last modified: Wed Jun 14 14:03:09 2023, max compression
```

## Comparing `pyperformance-1.0.8.tar` & `pyperformance-1.0.9.tar`

### file list

```diff
@@ -1,556 +1,724 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.674830 pyperformance-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-02 11:46:55.000000 pyperformance-1.0.8/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-02 11:46:55.000000 pyperformance-1.0.8/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-02 11:46:55.000000 pyperformance-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-02 11:47:16.674830 pyperformance-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-02 11:46:55.000000 pyperformance-1.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-06-02 11:46:55.000000 pyperformance-1.0.8/TODO.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.542829 pyperformance-1.0.8/benchmarks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_2to3/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_2to3/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_async_generators/
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_async_generators/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_async_tree/
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_async_tree/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_asyncio_tcp/
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_asyncio_tcp/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_chameleon/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_chameleon/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_chaos/
--rw-r--r--   0 runner    (1001) docker     (123)    10709 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_chaos/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_comprehensions/
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_comprehensions/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_concurrent_imap/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_concurrent_imap/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_coroutines/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_coroutines/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_coverage/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_coverage/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_crypto_pyaes/
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_crypto_pyaes/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_dask/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_dask/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_deepcopy/
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_deepcopy/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_deltablue/
--rw-r--r--   0 runner    (1001) docker     (123)    17136 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_deltablue/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_django_template/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_django_template/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_docutils/
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_docutils/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_dulwich_log/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_dulwich_log/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_fannkuch/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_fannkuch/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_float/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_float/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_gc_collect/
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_gc_collect/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_gc_traversal/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_gc_traversal/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_generators/
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_generators/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_genshi/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_genshi/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_go/
--rw-r--r--   0 runner    (1001) docker     (123)    13911 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_go/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.562829 pyperformance-1.0.8/benchmarks/bm_hexiom/
--rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_hexiom/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.562829 pyperformance-1.0.8/benchmarks/bm_hg_startup/
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_hg_startup/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.562829 pyperformance-1.0.8/benchmarks/bm_html5lib/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_html5lib/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.562829 pyperformance-1.0.8/benchmarks/bm_json_dumps/
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_json_dumps/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.562829 pyperformance-1.0.8/benchmarks/bm_json_loads/
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_json_loads/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.562829 pyperformance-1.0.8/benchmarks/bm_logging/
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_logging/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.562829 pyperformance-1.0.8/benchmarks/bm_mako/
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_mako/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.562829 pyperformance-1.0.8/benchmarks/bm_mdp/
--rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_mdp/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.562829 pyperformance-1.0.8/benchmarks/bm_meteor_contest/
--rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_meteor_contest/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.562829 pyperformance-1.0.8/benchmarks/bm_nbody/
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_nbody/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.562829 pyperformance-1.0.8/benchmarks/bm_nqueens/
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_nqueens/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.562829 pyperformance-1.0.8/benchmarks/bm_pathlib/
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_pathlib/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.562829 pyperformance-1.0.8/benchmarks/bm_pickle/
--rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_pickle/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.562829 pyperformance-1.0.8/benchmarks/bm_pidigits/
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_pidigits/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.562829 pyperformance-1.0.8/benchmarks/bm_pprint/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_pprint/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.562829 pyperformance-1.0.8/benchmarks/bm_pyflate/
--rwxr-xr-x   0 runner    (1001) docker     (123)    20078 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_pyflate/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.562829 pyperformance-1.0.8/benchmarks/bm_python_startup/
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_python_startup/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.562829 pyperformance-1.0.8/benchmarks/bm_raytrace/
--rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_raytrace/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.570829 pyperformance-1.0.8/benchmarks/bm_regex_compile/
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_regex_compile/bm_regex_effbot.py
--rw-r--r--   0 runner    (1001) docker     (123)   125978 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_regex_compile/bm_regex_v8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_regex_compile/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.570829 pyperformance-1.0.8/benchmarks/bm_regex_dna/
--rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_regex_dna/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.570829 pyperformance-1.0.8/benchmarks/bm_regex_effbot/
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_regex_effbot/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.570829 pyperformance-1.0.8/benchmarks/bm_regex_v8/
--rw-r--r--   0 runner    (1001) docker     (123)   125978 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_regex_v8/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.570829 pyperformance-1.0.8/benchmarks/bm_richards/
--rw-r--r--   0 runner    (1001) docker     (123)     9539 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_richards/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.570829 pyperformance-1.0.8/benchmarks/bm_richards_super/
--rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_richards_super/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.570829 pyperformance-1.0.8/benchmarks/bm_scimark/
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_scimark/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.570829 pyperformance-1.0.8/benchmarks/bm_spectral_norm/
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_spectral_norm/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.570829 pyperformance-1.0.8/benchmarks/bm_sqlalchemy_declarative/
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_sqlalchemy_declarative/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.570829 pyperformance-1.0.8/benchmarks/bm_sqlalchemy_imperative/
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_sqlalchemy_imperative/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.570829 pyperformance-1.0.8/benchmarks/bm_sqlglot/
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_sqlglot/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.570829 pyperformance-1.0.8/benchmarks/bm_sqlite_synth/
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_sqlite_synth/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.570829 pyperformance-1.0.8/benchmarks/bm_sympy/
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_sympy/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.574829 pyperformance-1.0.8/benchmarks/bm_telco/
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_telco/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.574829 pyperformance-1.0.8/benchmarks/bm_tomli_loads/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_tomli_loads/generate_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_tomli_loads/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.574829 pyperformance-1.0.8/benchmarks/bm_tornado_http/
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_tornado_http/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.574829 pyperformance-1.0.8/benchmarks/bm_typing_runtime_protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_typing_runtime_protocols/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.574829 pyperformance-1.0.8/benchmarks/bm_unpack_sequence/
--rw-r--r--   0 runner    (1001) docker     (123)    20968 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_unpack_sequence/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.574829 pyperformance-1.0.8/benchmarks/bm_xml_etree/
--rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_xml_etree/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.574829 pyperformance-1.0.8/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-02 11:46:55.000000 pyperformance-1.0.8/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    20317 2023-06-02 11:46:55.000000 pyperformance-1.0.8/doc/benchmarks.rst
--rw-r--r--   0 runner    (1001) docker     (123)    20403 2023-06-02 11:46:55.000000 pyperformance-1.0.8/doc/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-06-02 11:46:55.000000 pyperformance-1.0.8/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    25473 2023-06-02 11:46:55.000000 pyperformance-1.0.8/doc/cpython_results_2017.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-06-02 11:46:55.000000 pyperformance-1.0.8/doc/custom_benchmarks.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.578829 pyperformance-1.0.8/doc/images/
--rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-06-02 11:46:55.000000 pyperformance-1.0.8/doc/images/bm_chaos.png
--rw-r--r--   0 runner    (1001) docker     (123)    55274 2023-06-02 11:46:55.000000 pyperformance-1.0.8/doc/images/bm_raytrace.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    48901 2023-06-02 11:46:55.000000 pyperformance-1.0.8/doc/images/html5lib.png
--rw-r--r--   0 runner    (1001) docker     (123)    42433 2023-06-02 11:46:55.000000 pyperformance-1.0.8/doc/images/sympy_sum.png
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-02 11:46:55.000000 pyperformance-1.0.8/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-02 11:46:55.000000 pyperformance-1.0.8/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)    19415 2023-06-02 11:46:55.000000 pyperformance-1.0.8/doc/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.582829 pyperformance-1.0.8/pyperformance/
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7964 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/_benchmark_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/_benchmark_selections.py
--rw-r--r--   0 runner    (1001) docker     (123)    14475 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/_pip.py
--rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/_pyproject_toml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/_python.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/_pythoninfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/_venv.py
--rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7733 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)    33030 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/compile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.542829 pyperformance-1.0.8/pyperformance/data-files/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.582829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/MANIFEST
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.582829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.542829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.586829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/__init__.py.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/context_processors.py.txt
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/exceptions.py.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16817 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/mail.py.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/paginator.py.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/signals.py.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/template_loader.py.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15786 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/urlresolvers.py.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/xheaders.py.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.586829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_async_generators/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_async_generators/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_async_generators/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.586829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_async_tree/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_cpu_io_mixed.toml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_eager.toml
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_eager_cpu_io_mixed.toml
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_eager_io.toml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_eager_memoization.toml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_io.toml
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_memoization.toml
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_async_tree/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_async_tree/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.586829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_asyncio_tcp/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_asyncio_tcp/bm_asyncio_tcp_ssl.toml
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_asyncio_tcp/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_asyncio_tcp/run_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_asyncio_tcp/ssl_cert.pem
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_asyncio_tcp/ssl_key.pem
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.590829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_chameleon/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_chameleon/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_chameleon/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_chameleon/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.590829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_chaos/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_chaos/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)    10709 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_chaos/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.590829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_comprehensions/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_comprehensions/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_comprehensions/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.590829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_concurrent_imap/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_concurrent_imap/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_concurrent_imap/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.590829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_coroutines/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_coroutines/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_coroutines/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.590829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_coverage/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_coverage/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_coverage/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_coverage/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.590829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_crypto_pyaes/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_crypto_pyaes/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_crypto_pyaes/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_crypto_pyaes/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.590829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dask/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dask/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dask/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dask/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.590829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_deepcopy/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_deepcopy/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_deepcopy/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.594829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_deltablue/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_deltablue/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)    17136 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_deltablue/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.594829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_django_template/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_django_template/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_django_template/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_django_template/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.594829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.546829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.594829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.594829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)    10569 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/publisher.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/runtime-settings.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/transforms.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.598830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/distributing.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16986 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/enthought-plan.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/enthought-rfp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9172 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/hacking.txt
--rw-r--r--   0 runner    (1001) docker     (123)    25780 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/policies.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/pysource.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/release.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/repository.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.598830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/rst/
--rw-r--r--   0 runner    (1001) docker     (123)   113263 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/rst/alternatives.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35463 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/rst/problems.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/runtime-settings-processing.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/semantics.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9504 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/testing.txt
--rw-r--r--   0 runner    (1001) docker     (123)    98603 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/todo.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/website.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.598830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/cmdline-tool.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/html-stylesheets.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6869 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/i18n.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16349 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/rst-directives.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/rst-roles.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/security.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/index.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.598830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/
--rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0256.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11684 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0257.txt
--rw-r--r--   0 runner    (1001) docker     (123)    36399 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0258.txt
--rw-r--r--   0 runner    (1001) docker     (123)    32543 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0287.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.602830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/
--rw-r--r--   0 runner    (1001) docker     (123)   132076 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/doctree.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.602830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/
--rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/definitions.txt
--rw-r--r--   0 runner    (1001) docker     (123)    66717 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/directives.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13914 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/introduction.txt
--rw-r--r--   0 runner    (1001) docker     (123)    51188 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/mathematics.txt
--rw-r--r--   0 runner    (1001) docker     (123)   117454 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/restructuredtext.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/roles.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.606830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/
--rw-r--r--   0 runner    (1001) docker     (123)    64502 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/config.txt
--rw-r--r--   0 runner    (1001) docker     (123)    31991 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/emacs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/html.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.606830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/big-black.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/big-white.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/default.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/happy_monkey.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/medium-black.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/medium-white.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp-all.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp-breaks.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp-covers.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp-cuts.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp-empty.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp-objects.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/s5-files.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/s5-files.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/small-black.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/small-white.png
--rw-r--r--   0 runner    (1001) docker     (123)    62611 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/latex.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15571 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/mailing-lists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/manpage.txt
--rw-r--r--   0 runner    (1001) docker     (123)    38313 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/odt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.606830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/
--rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/cheatsheet.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/demo.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.610830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/biohazard-bitmap-scaling.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/biohazard-bitmap.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/biohazard-scaling.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/biohazard.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/biohazard.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/biohazard.swf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/pens.mp4
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/title-scaling.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/title.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/title.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11268 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/quickstart.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/smartquotes.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17347 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/tools.txt
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.610830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.546829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.610830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/COMMIT_EDITMSG
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/FETCH_HEAD
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/HEAD
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/ORIG_HEAD
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/config
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/description
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.614830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (123)      452 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      896 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/commit-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/post-update.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      398 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1642 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-commit.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1348 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-push.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     4951 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-rebase.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1239 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     3611 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/update.sample
--rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/index
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.614830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/info/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/info/exclude
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/info/refs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.614830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/HEAD
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.546829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.614830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/heads/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/heads/master
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.546829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.614830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/remotes/origin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/remotes/origin/HEAD
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/remotes/origin/bind_modules
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/remotes/origin/master
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/remotes/origin/zero_timeout
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.550829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.614830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/info/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/info/packs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.614830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/pack/
--rw-r--r--   0 runner    (1001) docker     (123)   247416 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/pack/pack-7e1b1ace85030071ca314cd565ae038bacc302a4.idx
--rw-r--r--   0 runner    (1001) docker     (123)  1774473 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/pack/pack-7e1b1ace85030071ca314cd565ae038bacc302a4.pack
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/packed-refs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.550829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/refs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.550829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/refs/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.618830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/refs/remotes/origin/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/refs/remotes/origin/HEAD
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.618830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_fannkuch/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_fannkuch/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_fannkuch/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.618830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_float/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_float/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_float/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.618830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_gc_collect/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_gc_collect/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_gc_collect/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.618830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_gc_traversal/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_gc_traversal/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_gc_traversal/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.622830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_generators/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_generators/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_generators/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.622830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_genshi/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_genshi/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_genshi/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_genshi/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.622830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_go/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_go/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)    13911 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_go/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.622830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_hexiom/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_hexiom/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_hexiom/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.622830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_hg_startup/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_hg_startup/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_hg_startup/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_hg_startup/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.622830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_html5lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.622830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_html5lib/data/
--rw-r--r--   0 runner    (1001) docker     (123)   133837 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_html5lib/data/w3_tr_html5.html
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_html5lib/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_html5lib/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_html5lib/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.626830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_json_dumps/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_json_dumps/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_json_dumps/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.626830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_json_loads/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_json_loads/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_json_loads/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.626830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_logging/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_logging/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_logging/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.626830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_mako/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_mako/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_mako/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_mako/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.626830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_mdp/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_mdp/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_mdp/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.626830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_meteor_contest/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_meteor_contest/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_meteor_contest/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.626830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_nbody/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_nbody/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_nbody/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.630830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_nqueens/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_nqueens/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_nqueens/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.630830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pathlib/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pathlib/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pathlib/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.630830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pickle/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pickle/bm_pickle_dict.toml
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pickle/bm_pickle_list.toml
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pickle/bm_pickle_pure_python.toml
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pickle/bm_unpickle.toml
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pickle/bm_unpickle_list.toml
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pickle/bm_unpickle_pure_python.toml
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pickle/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pickle/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.630830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pidigits/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pidigits/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pidigits/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.630830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pprint/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pprint/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pprint/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.630830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pyflate/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.630830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pyflate/data/
--rw-r--r--   0 runner    (1001) docker     (123)    67562 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pyflate/data/interpreter.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pyflate/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)    20078 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pyflate/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.634830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_python_startup/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_python_startup/bm_python_startup_no_site.toml
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_python_startup/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_python_startup/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.634830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_raytrace/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_raytrace/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_raytrace/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.638830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_compile/
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_compile/bm_regex_effbot.py
--rw-r--r--   0 runner    (1001) docker     (123)   125978 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_compile/bm_regex_v8.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_compile/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_compile/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.638830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_dna/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_dna/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_dna/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.642830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_effbot/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_effbot/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_effbot/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.642830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_v8/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_v8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)   125978 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_v8/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.642830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_richards/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_richards/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     9539 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_richards/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.642830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_richards_super/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_richards_super/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_richards_super/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.642830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_scimark/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_scimark/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_scimark/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.642830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_spectral_norm/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_spectral_norm/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_spectral_norm/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.642830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlalchemy_declarative/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlalchemy_declarative/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlalchemy_declarative/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlalchemy_declarative/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.642830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlalchemy_imperative/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlalchemy_imperative/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlalchemy_imperative/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlalchemy_imperative/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.646830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlglot/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlglot/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlglot/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlglot/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.646830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlite_synth/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlite_synth/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlite_synth/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.646830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sympy/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sympy/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sympy/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sympy/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.646830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_telco/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.646830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_telco/data/
--rw-r--r--   0 runner    (1001) docker     (123)   160000 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_telco/data/telco-bench.b
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_telco/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_telco/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.646830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_tomli_loads/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.646830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_tomli_loads/data/
--rw-r--r--   0 runner    (1001) docker     (123) 16824157 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_tomli_loads/data/tomli-bench-data.toml
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_tomli_loads/generate_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_tomli_loads/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_tomli_loads/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_tomli_loads/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.670830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_tornado_http/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_tornado_http/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_tornado_http/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_tornado_http/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.670830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_typing_runtime_protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_typing_runtime_protocols/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_typing_runtime_protocols/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.674830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_unpack_sequence/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_unpack_sequence/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)    20968 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_unpack_sequence/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.674830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_xml_etree/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_xml_etree/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_xml_etree/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.674830 pyperformance-1.0.8/pyperformance/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/venv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.582829 pyperformance-1.0.8/pyperformance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-02 11:47:16.000000 pyperformance-1.0.8/pyperformance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24213 2023-06-02 11:47:16.000000 pyperformance-1.0.8/pyperformance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 11:47:16.000000 pyperformance-1.0.8/pyperformance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-02 11:47:16.000000 pyperformance-1.0.8/pyperformance.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-02 11:47:16.000000 pyperformance-1.0.8/pyperformance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-02 11:47:16.000000 pyperformance-1.0.8/pyperformance.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-02 11:46:55.000000 pyperformance-1.0.8/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-02 11:46:55.000000 pyperformance-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 11:47:16.674830 pyperformance-1.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.924573 pyperformance-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-14 14:02:57.000000 pyperformance-1.0.9/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-14 14:02:57.000000 pyperformance-1.0.9/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-14 14:02:57.000000 pyperformance-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-14 14:03:09.924573 pyperformance-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-14 14:02:57.000000 pyperformance-1.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-06-14 14:02:57.000000 pyperformance-1.0.9/TODO.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.744572 pyperformance-1.0.9/benchmarks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.764572 pyperformance-1.0.9/benchmarks/bm_2to3/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.736572 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.736572 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.768572 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/btm_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/btm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixer_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15206 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixer_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.780572 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_asserts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_basestring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_except.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_execfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_exitfunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_funcattrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_future.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_getcwdu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_has_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_idioms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_imports2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_intern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_isinstance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_itertools_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_long.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_metaclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_methodattrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_ne.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_next.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_nonzero.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_numliterals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_paren.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_print.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_raise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_raw_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_reload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_renames.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_set_literal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_standarderror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_sys_exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_throw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_tuple_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_unicode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_urllib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_ws_comma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_xrange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_xreadlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/patcomp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.784572 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/pgen2/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/pgen2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9642 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/pgen2/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/pgen2/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/pgen2/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/pgen2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/pgen2/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13830 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/pgen2/pgen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1302 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/pgen2/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21119 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/pgen2/tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/pygram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27974 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/pytree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27507 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_2to3/vendor/src/lib2to3/refactor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.784572 pyperformance-1.0.9/benchmarks/bm_async_generators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_async_generators/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.784572 pyperformance-1.0.9/benchmarks/bm_async_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_async_tree/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.784572 pyperformance-1.0.9/benchmarks/bm_asyncio_tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_asyncio_tcp/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.784572 pyperformance-1.0.9/benchmarks/bm_chameleon/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_chameleon/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.784572 pyperformance-1.0.9/benchmarks/bm_chaos/
+-rw-r--r--   0 runner    (1001) docker     (123)    10709 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_chaos/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.784572 pyperformance-1.0.9/benchmarks/bm_comprehensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_comprehensions/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.784572 pyperformance-1.0.9/benchmarks/bm_concurrent_imap/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_concurrent_imap/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.784572 pyperformance-1.0.9/benchmarks/bm_coroutines/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_coroutines/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.784572 pyperformance-1.0.9/benchmarks/bm_coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_coverage/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.784572 pyperformance-1.0.9/benchmarks/bm_crypto_pyaes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_crypto_pyaes/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.784572 pyperformance-1.0.9/benchmarks/bm_dask/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_dask/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.784572 pyperformance-1.0.9/benchmarks/bm_deepcopy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_deepcopy/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.784572 pyperformance-1.0.9/benchmarks/bm_deltablue/
+-rw-r--r--   0 runner    (1001) docker     (123)    17136 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_deltablue/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.784572 pyperformance-1.0.9/benchmarks/bm_django_template/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_django_template/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.784572 pyperformance-1.0.9/benchmarks/bm_docutils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_docutils/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.784572 pyperformance-1.0.9/benchmarks/bm_dulwich_log/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_dulwich_log/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.784572 pyperformance-1.0.9/benchmarks/bm_fannkuch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_fannkuch/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.788572 pyperformance-1.0.9/benchmarks/bm_float/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_float/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.788572 pyperformance-1.0.9/benchmarks/bm_gc_collect/
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_gc_collect/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.788572 pyperformance-1.0.9/benchmarks/bm_gc_traversal/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_gc_traversal/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.788572 pyperformance-1.0.9/benchmarks/bm_generators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_generators/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.788572 pyperformance-1.0.9/benchmarks/bm_genshi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_genshi/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.788572 pyperformance-1.0.9/benchmarks/bm_go/
+-rw-r--r--   0 runner    (1001) docker     (123)    13911 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_go/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.788572 pyperformance-1.0.9/benchmarks/bm_hexiom/
+-rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_hexiom/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.788572 pyperformance-1.0.9/benchmarks/bm_hg_startup/
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_hg_startup/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.788572 pyperformance-1.0.9/benchmarks/bm_html5lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_html5lib/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.788572 pyperformance-1.0.9/benchmarks/bm_json_dumps/
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_json_dumps/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.788572 pyperformance-1.0.9/benchmarks/bm_json_loads/
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_json_loads/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.788572 pyperformance-1.0.9/benchmarks/bm_logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_logging/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.788572 pyperformance-1.0.9/benchmarks/bm_mako/
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_mako/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.788572 pyperformance-1.0.9/benchmarks/bm_mdp/
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_mdp/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.788572 pyperformance-1.0.9/benchmarks/bm_meteor_contest/
+-rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_meteor_contest/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.788572 pyperformance-1.0.9/benchmarks/bm_nbody/
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_nbody/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.788572 pyperformance-1.0.9/benchmarks/bm_nqueens/
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_nqueens/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.788572 pyperformance-1.0.9/benchmarks/bm_pathlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_pathlib/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.788572 pyperformance-1.0.9/benchmarks/bm_pickle/
+-rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_pickle/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.792572 pyperformance-1.0.9/benchmarks/bm_pidigits/
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_pidigits/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.792572 pyperformance-1.0.9/benchmarks/bm_pprint/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_pprint/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.792572 pyperformance-1.0.9/benchmarks/bm_pyflate/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20078 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_pyflate/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.792572 pyperformance-1.0.9/benchmarks/bm_python_startup/
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_python_startup/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.792572 pyperformance-1.0.9/benchmarks/bm_raytrace/
+-rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_raytrace/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.792572 pyperformance-1.0.9/benchmarks/bm_regex_compile/
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_regex_compile/bm_regex_effbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125978 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_regex_compile/bm_regex_v8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_regex_compile/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.792572 pyperformance-1.0.9/benchmarks/bm_regex_dna/
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_regex_dna/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.792572 pyperformance-1.0.9/benchmarks/bm_regex_effbot/
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_regex_effbot/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.792572 pyperformance-1.0.9/benchmarks/bm_regex_v8/
+-rw-r--r--   0 runner    (1001) docker     (123)   125978 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_regex_v8/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.792572 pyperformance-1.0.9/benchmarks/bm_richards/
+-rw-r--r--   0 runner    (1001) docker     (123)     9539 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_richards/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.792572 pyperformance-1.0.9/benchmarks/bm_richards_super/
+-rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_richards_super/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.792572 pyperformance-1.0.9/benchmarks/bm_scimark/
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_scimark/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.792572 pyperformance-1.0.9/benchmarks/bm_spectral_norm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_spectral_norm/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.792572 pyperformance-1.0.9/benchmarks/bm_sqlalchemy_declarative/
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_sqlalchemy_declarative/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.796572 pyperformance-1.0.9/benchmarks/bm_sqlalchemy_imperative/
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_sqlalchemy_imperative/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.796572 pyperformance-1.0.9/benchmarks/bm_sqlglot/
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_sqlglot/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.796572 pyperformance-1.0.9/benchmarks/bm_sqlite_synth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_sqlite_synth/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.796572 pyperformance-1.0.9/benchmarks/bm_sympy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_sympy/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.796572 pyperformance-1.0.9/benchmarks/bm_telco/
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_telco/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.796572 pyperformance-1.0.9/benchmarks/bm_tomli_loads/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_tomli_loads/generate_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_tomli_loads/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.796572 pyperformance-1.0.9/benchmarks/bm_tornado_http/
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_tornado_http/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.796572 pyperformance-1.0.9/benchmarks/bm_typing_runtime_protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_typing_runtime_protocols/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.796572 pyperformance-1.0.9/benchmarks/bm_unpack_sequence/
+-rw-r--r--   0 runner    (1001) docker     (123)    20968 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_unpack_sequence/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.796572 pyperformance-1.0.9/benchmarks/bm_xml_etree/
+-rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-06-14 14:02:57.000000 pyperformance-1.0.9/benchmarks/bm_xml_etree/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.800572 pyperformance-1.0.9/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-14 14:02:57.000000 pyperformance-1.0.9/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    20317 2023-06-14 14:02:57.000000 pyperformance-1.0.9/doc/benchmarks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    20530 2023-06-14 14:02:57.000000 pyperformance-1.0.9/doc/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-06-14 14:02:57.000000 pyperformance-1.0.9/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25473 2023-06-14 14:02:57.000000 pyperformance-1.0.9/doc/cpython_results_2017.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-06-14 14:02:57.000000 pyperformance-1.0.9/doc/custom_benchmarks.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.800572 pyperformance-1.0.9/doc/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-06-14 14:02:57.000000 pyperformance-1.0.9/doc/images/bm_chaos.png
+-rw-r--r--   0 runner    (1001) docker     (123)    55274 2023-06-14 14:02:57.000000 pyperformance-1.0.9/doc/images/bm_raytrace.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    48901 2023-06-14 14:02:57.000000 pyperformance-1.0.9/doc/images/html5lib.png
+-rw-r--r--   0 runner    (1001) docker     (123)    42433 2023-06-14 14:02:57.000000 pyperformance-1.0.9/doc/images/sympy_sum.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-14 14:02:57.000000 pyperformance-1.0.9/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-14 14:02:57.000000 pyperformance-1.0.9/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    19415 2023-06-14 14:02:57.000000 pyperformance-1.0.9/doc/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.804572 pyperformance-1.0.9/pyperformance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7964 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/_benchmark_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/_benchmark_selections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14475 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/_pip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/_pyproject_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/_pythoninfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/_venv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7733 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33030 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/compile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.748572 pyperformance-1.0.9/pyperformance/data-files/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.804572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/MANIFEST
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.804572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.748572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.808572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/__init__.py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/context_processors.py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/exceptions.py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16817 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/mail.py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/paginator.py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/signals.py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/template_loader.py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15786 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/urlresolvers.py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/xheaders.py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.808572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.748572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.812572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/
+-rw-r--r--   0 runner    (1001) docker     (123)     8696 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/Grammar.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/PatternGrammar.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/btm_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/btm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixer_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15206 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixer_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.820572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_asserts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_basestring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_except.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_execfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_exitfunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_funcattrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_future.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_getcwdu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_has_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_idioms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_imports2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_intern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_isinstance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_itertools_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_long.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_metaclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_methodattrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_ne.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_next.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_nonzero.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_numliterals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_paren.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_print.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_raise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_raw_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_reload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_renames.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_set_literal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_standarderror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_sys_exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_throw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_tuple_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_unicode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_urllib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_ws_comma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_xrange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_xreadlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/fixes/fix_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/patcomp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.824572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/pgen2/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/pgen2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9642 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/pgen2/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/pgen2/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/pgen2/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/pgen2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/pgen2/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13830 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/pgen2/pgen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1302 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/pgen2/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21119 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/pgen2/tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/pygram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27974 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/pytree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27507 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/vendor/src/lib2to3/refactor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.824572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_async_generators/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_async_generators/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_async_generators/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.828572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_async_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_cpu_io_mixed.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_cpu_io_mixed_tg.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_eager.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_eager_cpu_io_mixed.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_eager_cpu_io_mixed_tg.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_eager_io.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_eager_io_tg.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_eager_memoization.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_eager_memoization_tg.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_eager_tg.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_io.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_io_tg.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_memoization.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_memoization_tg.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_tg.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_async_tree/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_async_tree/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.832572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_asyncio_tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_asyncio_tcp/bm_asyncio_tcp_ssl.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_asyncio_tcp/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_asyncio_tcp/run_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_asyncio_tcp/ssl_cert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_asyncio_tcp/ssl_key.pem
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.832572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_chameleon/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_chameleon/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_chameleon/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_chameleon/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.832572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_chaos/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_chaos/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    10709 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_chaos/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.832572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_comprehensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_comprehensions/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_comprehensions/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.836572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_concurrent_imap/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_concurrent_imap/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_concurrent_imap/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.836572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_coroutines/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_coroutines/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_coroutines/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.836572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_coverage/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_coverage/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_coverage/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.836572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_crypto_pyaes/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_crypto_pyaes/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_crypto_pyaes/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_crypto_pyaes/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.836572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dask/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dask/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dask/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dask/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.836572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_deepcopy/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_deepcopy/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_deepcopy/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.840572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_deltablue/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_deltablue/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    17136 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_deltablue/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.840572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_django_template/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_django_template/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_django_template/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_django_template/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.840572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.752572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.840572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.840572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    10569 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/publisher.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/runtime-settings.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/transforms.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.844572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/distributing.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16986 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/enthought-plan.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/enthought-rfp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9172 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/hacking.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    25780 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/policies.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/pysource.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/release.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/repository.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.844572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/rst/
+-rw-r--r--   0 runner    (1001) docker     (123)   113263 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/rst/alternatives.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35463 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/rst/problems.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/runtime-settings-processing.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/semantics.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9504 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/testing.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    98603 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/todo.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/website.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.848572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/cmdline-tool.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/html-stylesheets.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6869 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/i18n.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16349 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/rst-directives.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/rst-roles.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/security.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/index.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.848572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/
+-rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0256.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11684 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0257.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    36399 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0258.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    32543 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0287.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.848572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/
+-rw-r--r--   0 runner    (1001) docker     (123)   132076 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/doctree.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.852573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/
+-rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/definitions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    66717 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/directives.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13914 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/introduction.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    51188 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/mathematics.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   117454 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/restructuredtext.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/roles.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.852573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/
+-rw-r--r--   0 runner    (1001) docker     (123)    64502 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/config.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    31991 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/emacs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/html.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.856572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/big-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/big-white.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/default.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/happy_monkey.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/medium-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/medium-white.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp-all.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp-breaks.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp-covers.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp-cuts.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp-empty.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp-objects.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/s5-files.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/s5-files.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/small-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/small-white.png
+-rw-r--r--   0 runner    (1001) docker     (123)    62611 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/latex.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15571 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/mailing-lists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/manpage.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    38313 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/odt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.856572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/
+-rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/cheatsheet.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/demo.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.860572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/biohazard-bitmap-scaling.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/biohazard-bitmap.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/biohazard-scaling.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/biohazard.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/biohazard.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/biohazard.swf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/pens.mp4
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/title-scaling.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/title.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/title.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11268 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/quickstart.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/smartquotes.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17347 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/tools.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.860572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.752572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.864573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/COMMIT_EDITMSG
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/FETCH_HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/ORIG_HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/config
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/description
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.864573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      452 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      896 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/post-update.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      398 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1642 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1348 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-push.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4951 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1239 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3611 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/update.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/index
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.868573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/info/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/info/exclude
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/info/refs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.868573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/HEAD
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.752572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.868573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/heads/master
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.752572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.868573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/remotes/origin/HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/remotes/origin/bind_modules
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/remotes/origin/master
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/remotes/origin/zero_timeout
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.756572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.868573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/info/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/info/packs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.868573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/pack/
+-rw-r--r--   0 runner    (1001) docker     (123)   247416 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/pack/pack-7e1b1ace85030071ca314cd565ae038bacc302a4.idx
+-rw-r--r--   0 runner    (1001) docker     (123)  1774473 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/pack/pack-7e1b1ace85030071ca314cd565ae038bacc302a4.pack
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/packed-refs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.756572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/refs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.756572 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.872573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/refs/remotes/origin/HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.872573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_fannkuch/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_fannkuch/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_fannkuch/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.872573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_float/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_float/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_float/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.872573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_gc_collect/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_gc_collect/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_gc_collect/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.872573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_gc_traversal/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_gc_traversal/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_gc_traversal/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.872573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_generators/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_generators/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_generators/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.876573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_genshi/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_genshi/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_genshi/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_genshi/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.876573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_go/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_go/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    13911 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_go/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.876573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_hexiom/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_hexiom/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_hexiom/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.876573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_hg_startup/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_hg_startup/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_hg_startup/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_hg_startup/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.876573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_html5lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.876573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_html5lib/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   133837 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_html5lib/data/w3_tr_html5.html
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_html5lib/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_html5lib/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_html5lib/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.880573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_json_dumps/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_json_dumps/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_json_dumps/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.880573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_json_loads/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_json_loads/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_json_loads/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.880573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_logging/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_logging/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.880573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_mako/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_mako/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_mako/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_mako/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.880573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_mdp/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_mdp/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_mdp/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.880573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_meteor_contest/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_meteor_contest/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_meteor_contest/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.880573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_nbody/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_nbody/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_nbody/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.884573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_nqueens/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_nqueens/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_nqueens/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.884573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_pathlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_pathlib/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_pathlib/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.884573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_pickle/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_pickle/bm_pickle_dict.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_pickle/bm_pickle_list.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_pickle/bm_pickle_pure_python.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_pickle/bm_unpickle.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_pickle/bm_unpickle_list.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_pickle/bm_unpickle_pure_python.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_pickle/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_pickle/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.884573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_pidigits/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_pidigits/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_pidigits/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.884573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_pprint/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_pprint/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_pprint/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.888573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_pyflate/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.888573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_pyflate/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    67562 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_pyflate/data/interpreter.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_pyflate/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20078 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_pyflate/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.888573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_python_startup/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_python_startup/bm_python_startup_no_site.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_python_startup/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_python_startup/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.888573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_raytrace/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_raytrace/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_raytrace/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.888573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_regex_compile/
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_regex_compile/bm_regex_effbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125978 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_regex_compile/bm_regex_v8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_regex_compile/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_regex_compile/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.888573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_regex_dna/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_regex_dna/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_regex_dna/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.892573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_regex_effbot/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_regex_effbot/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_regex_effbot/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.892573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_regex_v8/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_regex_v8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)   125978 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_regex_v8/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.892573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_richards/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_richards/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     9539 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_richards/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.892573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_richards_super/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_richards_super/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_richards_super/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.892573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_scimark/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_scimark/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_scimark/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.892573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_spectral_norm/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_spectral_norm/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_spectral_norm/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.892573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_sqlalchemy_declarative/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_sqlalchemy_declarative/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_sqlalchemy_declarative/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_sqlalchemy_declarative/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.896573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_sqlalchemy_imperative/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_sqlalchemy_imperative/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_sqlalchemy_imperative/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_sqlalchemy_imperative/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.896573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_sqlglot/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_sqlglot/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_sqlglot/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_sqlglot/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.896573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_sqlite_synth/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_sqlite_synth/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_sqlite_synth/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.896573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_sympy/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_sympy/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_sympy/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_sympy/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.896573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_telco/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.896573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_telco/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   160000 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_telco/data/telco-bench.b
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_telco/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_telco/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.900573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_tomli_loads/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.900573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_tomli_loads/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 16824157 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_tomli_loads/data/tomli-bench-data.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_tomli_loads/generate_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_tomli_loads/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_tomli_loads/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_tomli_loads/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.920573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_tornado_http/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_tornado_http/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_tornado_http/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_tornado_http/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.924573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_typing_runtime_protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_typing_runtime_protocols/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_typing_runtime_protocols/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.924573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_unpack_sequence/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_unpack_sequence/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    20968 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_unpack_sequence/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.924573 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_xml_etree/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_xml_etree/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_xml_etree/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.924573 pyperformance-1.0.9/pyperformance/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyperformance/venv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:03:09.804572 pyperformance-1.0.9/pyperformance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-14 14:03:09.000000 pyperformance-1.0.9/pyperformance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35304 2023-06-14 14:03:09.000000 pyperformance-1.0.9/pyperformance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 14:03:09.000000 pyperformance-1.0.9/pyperformance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-14 14:03:09.000000 pyperformance-1.0.9/pyperformance.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-14 14:03:09.000000 pyperformance-1.0.9/pyperformance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-14 14:03:09.000000 pyperformance-1.0.9/pyperformance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-14 14:02:57.000000 pyperformance-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-14 14:02:57.000000 pyperformance-1.0.9/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-14 14:02:57.000000 pyperformance-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 14:03:09.924573 pyperformance-1.0.9/setup.cfg
```

### Comparing `pyperformance-1.0.8/AUTHORS` & `pyperformance-1.0.9/AUTHORS`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/COPYING` & `pyperformance-1.0.9/COPYING`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/MANIFEST.in` & `pyperformance-1.0.9/MANIFEST.in`

 * *Files 18% similar despite different names*

```diff
@@ -12,9 +12,10 @@
 include pyperformance/*.py
 include pyperformance/requirements/requirements.txt
 include pyperformance/data-files/benchmarks/MANIFEST
 include pyperformance/data-files/benchmarks/bm_*/*.toml
 include pyperformance/data-files/benchmarks/bm_*/*.py
 include pyperformance/data-files/benchmarks/bm_*/requirements.txt
 include pyperformance/data-files/benchmarks/bm_*/*.pem
+recursive-include pyperformance/data-files/benchmarks/bm_*/vendor *
 recursive-include pyperformance/data-files/benchmarks/bm_*/data *
 recursive-exclude pyperformance/tests *
```

### Comparing `pyperformance-1.0.8/PKG-INFO` & `pyperformance-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyperformance
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python benchmark suite
 Author: Collin Winter, Jeffrey Yasskin
 License: MIT
 Project-URL: Homepage, https://github.com/python/pyperformance
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyperformance-1.0.8/README.rst` & `pyperformance-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/TODO.rst` & `pyperformance-1.0.9/TODO.rst`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_async_generators/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_async_generators/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_async_tree/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_async_tree/run_benchmark.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 2) "io": All leaf nodes simulate async IO workload (async sleep 50ms).
 3) "memoization": All leaf nodes simulate async IO workload with 90% of
                   the data memoized
 4) "cpu_io_mixed": Half of the leaf nodes simulate CPU-bound workload and
                    the other half simulate the same workload as the
                    "memoization" variant.
 
-All variants also have an "eager" flavor that uses
-the asyncio eager task factory (if available).
+All variants also have an "eager" flavor that uses the asyncio eager task
+factory (if available), and a "tg" variant that uses TaskGroups.
 """
 
 
 import asyncio
 import math
 import random
 
@@ -30,38 +30,53 @@
 IO_SLEEP_TIME = 0.05
 MEMOIZABLE_PERCENTAGE = 90
 CPU_PROBABILITY = 0.5
 FACTORIAL_N = 500
 
 
 class AsyncTree:
-    def __init__(self):
+    def __init__(self, use_task_groups=False):
         self.cache = {}
+        self.use_task_groups = use_task_groups
         # set to deterministic random, so that the results are reproducible
         random.seed(RANDOM_SEED)
 
     async def mock_io_call(self):
         await asyncio.sleep(IO_SLEEP_TIME)
 
     async def workload_func(self):
         raise NotImplementedError(
             "To be implemented by each variant's derived class."
         )
 
-    async def recurse(self, recurse_level):
+    async def recurse_with_gather(self, recurse_level):
         if recurse_level == 0:
             await self.workload_func()
             return
 
         await asyncio.gather(
-            *[self.recurse(recurse_level - 1) for _ in range(NUM_RECURSE_BRANCHES)]
+            *[self.recurse_with_gather(recurse_level - 1)
+              for _ in range(NUM_RECURSE_BRANCHES)]
         )
 
+    async def recurse_with_task_group(self, recurse_level):
+        if recurse_level == 0:
+            await self.workload_func()
+            return
+
+        async with asyncio.TaskGroup() as tg:
+            for _ in range(NUM_RECURSE_BRANCHES):
+                tg.create_task(
+                    self.recurse_with_task_group(recurse_level - 1))
+
     async def run(self):
-        await self.recurse(NUM_RECURSE_LEVELS)
+        if self.use_task_groups:
+            await self.recurse_with_task_group(NUM_RECURSE_LEVELS)
+        else:
+            await self.recurse_with_gather(NUM_RECURSE_LEVELS)
 
 
 class EagerMixin:
     async def run(self):
         loop = asyncio.get_running_loop()
         if hasattr(asyncio, 'eager_task_factory'):
             loop.set_task_factory(asyncio.eager_task_factory)
@@ -128,14 +143,16 @@
     runner.metadata["async_tree_memoizable_percentage"] = MEMOIZABLE_PERCENTAGE
     runner.metadata["async_tree_cpu_probability"] = CPU_PROBABILITY
     runner.metadata["async_tree_factorial_n"] = FACTORIAL_N
 
 
 def add_cmdline_args(cmd, args):
     cmd.append(args.benchmark)
+    if args.task_groups:
+        cmd.append("--task-groups")
 
 
 def add_parser_args(parser):
     parser.add_argument(
         "benchmark",
         choices=BENCHMARKS,
         help="""\
@@ -145,14 +162,20 @@
 3) "memoization": All leaf nodes simulate async IO workload with 90% of
                   the data memoized
 4) "cpu_io_mixed": Half of the leaf nodes simulate CPU-bound workload and
                    the other half simulate the same workload as the
                    "memoization" variant.
 """,
     )
+    parser.add_argument(
+        "--task-groups",
+        action="store_true",
+        default=False,
+        help="Use TaskGroups instead of gather.",
+    )
 
 
 BENCHMARKS = {
     "none": NoneAsyncTree,
     "eager": EagerAsyncTree,
     "io": IOAsyncTree,
     "eager_io": EagerIOAsyncTree,
@@ -167,9 +190,12 @@
     runner = pyperf.Runner(add_cmdline_args=add_cmdline_args)
     add_metadata(runner)
     add_parser_args(runner.argparser)
     args = runner.parse_args()
     benchmark = args.benchmark
 
     async_tree_class = BENCHMARKS[benchmark]
-    async_tree = async_tree_class()
-    runner.bench_async_func(f"async_tree_{benchmark}", async_tree.run)
+    async_tree = async_tree_class(use_task_groups=args.task_groups)
+    bench_name = f"async_tree_{benchmark}"
+    if args.task_groups:
+        bench_name += "_tg"
+    runner.bench_async_func(bench_name, async_tree.run)
```

### Comparing `pyperformance-1.0.8/benchmarks/bm_asyncio_tcp/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_asyncio_tcp/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_chameleon/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_chameleon/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_chaos/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_chaos/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_comprehensions/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_comprehensions/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_concurrent_imap/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_concurrent_imap/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_coroutines/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_coroutines/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_coverage/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_coverage/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_crypto_pyaes/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_crypto_pyaes/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_dask/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_dask/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_deepcopy/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_deepcopy/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_deltablue/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_deltablue/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_django_template/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_django_template/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_docutils/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_docutils/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_dulwich_log/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_dulwich_log/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_fannkuch/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_fannkuch/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_float/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_float/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_gc_collect/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_gc_collect/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_gc_traversal/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_gc_traversal/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_generators/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_generators/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_genshi/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_genshi/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_go/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_go/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_hexiom/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_hexiom/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_hg_startup/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_hg_startup/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_html5lib/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_html5lib/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_json_dumps/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_json_dumps/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_json_loads/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_json_loads/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_logging/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_logging/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_mako/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_mako/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_mdp/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_mdp/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_meteor_contest/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_meteor_contest/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_nbody/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_nbody/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_nqueens/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_nqueens/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_pathlib/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_pathlib/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_pickle/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_pickle/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_pidigits/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_pidigits/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_pprint/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_pprint/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_pyflate/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_pyflate/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_python_startup/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_python_startup/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_raytrace/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_raytrace/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_regex_compile/bm_regex_effbot.py` & `pyperformance-1.0.9/benchmarks/bm_regex_compile/bm_regex_effbot.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_regex_compile/bm_regex_v8.py` & `pyperformance-1.0.9/benchmarks/bm_regex_compile/bm_regex_v8.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_regex_compile/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_regex_compile/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_regex_dna/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_regex_dna/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_regex_effbot/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_regex_effbot/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_regex_v8/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_regex_v8/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_richards/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_richards/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_richards_super/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_richards_super/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_scimark/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_scimark/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_spectral_norm/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_spectral_norm/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_sqlalchemy_declarative/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_sqlalchemy_declarative/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_sqlalchemy_imperative/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_sqlalchemy_imperative/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_sqlglot/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_sqlglot/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_sqlite_synth/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_sqlite_synth/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_sympy/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_sympy/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_telco/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_telco/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_tomli_loads/generate_data.py` & `pyperformance-1.0.9/benchmarks/bm_tomli_loads/generate_data.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_tomli_loads/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_tomli_loads/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_tornado_http/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_tornado_http/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_typing_runtime_protocols/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_typing_runtime_protocols/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_unpack_sequence/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_unpack_sequence/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/benchmarks/bm_xml_etree/run_benchmark.py` & `pyperformance-1.0.9/benchmarks/bm_xml_etree/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/doc/Makefile` & `pyperformance-1.0.9/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/doc/benchmarks.rst` & `pyperformance-1.0.9/doc/benchmarks.rst`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/doc/changelog.rst` & `pyperformance-1.0.9/doc/changelog.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+Version 1.0.9 (2023-06-14)
+-------------
+* Vendor lib2to3 for Python 3.13+
+* Add TaskGroups variants to async_tree benchmarks
+
 Version 1.0.8 (2023-06-02)
 -------------
 
 * Move the main requirements.txt file to pyperformance/requirements
   so that dependabot can only run on that one file
 * Update dependencies of benchmarks not to specify setuptools
 * On older versions of Python, skip benchmarks that use features
```

### Comparing `pyperformance-1.0.8/doc/conf.py` & `pyperformance-1.0.9/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/doc/cpython_results_2017.rst` & `pyperformance-1.0.9/doc/cpython_results_2017.rst`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/doc/custom_benchmarks.rst` & `pyperformance-1.0.9/doc/custom_benchmarks.rst`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/doc/images/bm_chaos.png` & `pyperformance-1.0.9/doc/images/bm_chaos.png`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/doc/images/bm_raytrace.jpg` & `pyperformance-1.0.9/doc/images/bm_raytrace.jpg`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/doc/images/html5lib.png` & `pyperformance-1.0.9/doc/images/html5lib.png`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/doc/images/sympy_sum.png` & `pyperformance-1.0.9/doc/images/sympy_sum.png`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/doc/index.rst` & `pyperformance-1.0.9/doc/index.rst`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/doc/make.bat` & `pyperformance-1.0.9/doc/make.bat`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/doc/usage.rst` & `pyperformance-1.0.9/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/__init__.py` & `pyperformance-1.0.9/pyperformance/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os.path
 import sys
 
 
-VERSION = (1, 0, 8)
+VERSION = (1, 0, 9)
 __version__ = '.'.join(map(str, VERSION))
 
 
 PKG_ROOT = os.path.dirname(__file__)
 DATA_DIR = os.path.join(PKG_ROOT, 'data-files')
```

### Comparing `pyperformance-1.0.8/pyperformance/_benchmark.py` & `pyperformance-1.0.9/pyperformance/_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/_benchmark_metadata.py` & `pyperformance-1.0.9/pyperformance/_benchmark_metadata.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/_benchmark_selections.py` & `pyperformance-1.0.9/pyperformance/_benchmark_selections.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/_manifest.py` & `pyperformance-1.0.9/pyperformance/_manifest.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/_pip.py` & `pyperformance-1.0.9/pyperformance/_pip.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/_pyproject_toml.py` & `pyperformance-1.0.9/pyperformance/_pyproject_toml.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/_python.py` & `pyperformance-1.0.9/pyperformance/_python.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/_pythoninfo.py` & `pyperformance-1.0.9/pyperformance/_pythoninfo.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/_utils.py` & `pyperformance-1.0.9/pyperformance/_utils.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/_venv.py` & `pyperformance-1.0.9/pyperformance/_venv.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/cli.py` & `pyperformance-1.0.9/pyperformance/cli.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/commands.py` & `pyperformance-1.0.9/pyperformance/commands.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/compare.py` & `pyperformance-1.0.9/pyperformance/compare.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/compile.py` & `pyperformance-1.0.9/pyperformance/compile.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/context_processors.py.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/context_processors.py.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/exceptions.py.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/exceptions.py.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/mail.py.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/mail.py.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/paginator.py.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/paginator.py.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/urlresolvers.py.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/urlresolvers.py.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/xheaders.py.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/xheaders.py.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_async_generators/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_async_generators/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_async_tree/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_async_tree/run_benchmark.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 2) "io": All leaf nodes simulate async IO workload (async sleep 50ms).
 3) "memoization": All leaf nodes simulate async IO workload with 90% of
                   the data memoized
 4) "cpu_io_mixed": Half of the leaf nodes simulate CPU-bound workload and
                    the other half simulate the same workload as the
                    "memoization" variant.
 
-All variants also have an "eager" flavor that uses
-the asyncio eager task factory (if available).
+All variants also have an "eager" flavor that uses the asyncio eager task
+factory (if available), and a "tg" variant that uses TaskGroups.
 """
 
 
 import asyncio
 import math
 import random
 
@@ -30,38 +30,53 @@
 IO_SLEEP_TIME = 0.05
 MEMOIZABLE_PERCENTAGE = 90
 CPU_PROBABILITY = 0.5
 FACTORIAL_N = 500
 
 
 class AsyncTree:
-    def __init__(self):
+    def __init__(self, use_task_groups=False):
         self.cache = {}
+        self.use_task_groups = use_task_groups
         # set to deterministic random, so that the results are reproducible
         random.seed(RANDOM_SEED)
 
     async def mock_io_call(self):
         await asyncio.sleep(IO_SLEEP_TIME)
 
     async def workload_func(self):
         raise NotImplementedError(
             "To be implemented by each variant's derived class."
         )
 
-    async def recurse(self, recurse_level):
+    async def recurse_with_gather(self, recurse_level):
         if recurse_level == 0:
             await self.workload_func()
             return
 
         await asyncio.gather(
-            *[self.recurse(recurse_level - 1) for _ in range(NUM_RECURSE_BRANCHES)]
+            *[self.recurse_with_gather(recurse_level - 1)
+              for _ in range(NUM_RECURSE_BRANCHES)]
         )
 
+    async def recurse_with_task_group(self, recurse_level):
+        if recurse_level == 0:
+            await self.workload_func()
+            return
+
+        async with asyncio.TaskGroup() as tg:
+            for _ in range(NUM_RECURSE_BRANCHES):
+                tg.create_task(
+                    self.recurse_with_task_group(recurse_level - 1))
+
     async def run(self):
-        await self.recurse(NUM_RECURSE_LEVELS)
+        if self.use_task_groups:
+            await self.recurse_with_task_group(NUM_RECURSE_LEVELS)
+        else:
+            await self.recurse_with_gather(NUM_RECURSE_LEVELS)
 
 
 class EagerMixin:
     async def run(self):
         loop = asyncio.get_running_loop()
         if hasattr(asyncio, 'eager_task_factory'):
             loop.set_task_factory(asyncio.eager_task_factory)
@@ -128,14 +143,16 @@
     runner.metadata["async_tree_memoizable_percentage"] = MEMOIZABLE_PERCENTAGE
     runner.metadata["async_tree_cpu_probability"] = CPU_PROBABILITY
     runner.metadata["async_tree_factorial_n"] = FACTORIAL_N
 
 
 def add_cmdline_args(cmd, args):
     cmd.append(args.benchmark)
+    if args.task_groups:
+        cmd.append("--task-groups")
 
 
 def add_parser_args(parser):
     parser.add_argument(
         "benchmark",
         choices=BENCHMARKS,
         help="""\
@@ -145,14 +162,20 @@
 3) "memoization": All leaf nodes simulate async IO workload with 90% of
                   the data memoized
 4) "cpu_io_mixed": Half of the leaf nodes simulate CPU-bound workload and
                    the other half simulate the same workload as the
                    "memoization" variant.
 """,
     )
+    parser.add_argument(
+        "--task-groups",
+        action="store_true",
+        default=False,
+        help="Use TaskGroups instead of gather.",
+    )
 
 
 BENCHMARKS = {
     "none": NoneAsyncTree,
     "eager": EagerAsyncTree,
     "io": IOAsyncTree,
     "eager_io": EagerIOAsyncTree,
@@ -167,9 +190,12 @@
     runner = pyperf.Runner(add_cmdline_args=add_cmdline_args)
     add_metadata(runner)
     add_parser_args(runner.argparser)
     args = runner.parse_args()
     benchmark = args.benchmark
 
     async_tree_class = BENCHMARKS[benchmark]
-    async_tree = async_tree_class()
-    runner.bench_async_func(f"async_tree_{benchmark}", async_tree.run)
+    async_tree = async_tree_class(use_task_groups=args.task_groups)
+    bench_name = f"async_tree_{benchmark}"
+    if args.task_groups:
+        bench_name += "_tg"
+    runner.bench_async_func(bench_name, async_tree.run)
```

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_asyncio_tcp/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_asyncio_tcp/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_asyncio_tcp/ssl_cert.pem` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_asyncio_tcp/ssl_cert.pem`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_asyncio_tcp/ssl_key.pem` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_asyncio_tcp/ssl_key.pem`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_chameleon/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_chameleon/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_chaos/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_chaos/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_comprehensions/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_comprehensions/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_concurrent_imap/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_concurrent_imap/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_coroutines/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_coroutines/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_coverage/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_coverage/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_crypto_pyaes/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_crypto_pyaes/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dask/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dask/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_deepcopy/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_deepcopy/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_deltablue/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_deltablue/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_django_template/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_django_template/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/publisher.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/publisher.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/runtime-settings.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/runtime-settings.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/transforms.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/transforms.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/distributing.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/distributing.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/enthought-plan.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/enthought-plan.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/enthought-rfp.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/enthought-rfp.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/hacking.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/hacking.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/policies.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/policies.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/pysource.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/pysource.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/release.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/release.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/repository.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/repository.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/rst/alternatives.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/rst/alternatives.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/rst/problems.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/rst/problems.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/runtime-settings-processing.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/runtime-settings-processing.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/semantics.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/semantics.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/testing.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/testing.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/todo.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/todo.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/website.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/website.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/cmdline-tool.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/cmdline-tool.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/html-stylesheets.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/html-stylesheets.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/i18n.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/i18n.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/rst-directives.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/rst-directives.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/rst-roles.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/rst-roles.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/security.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/security.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/index.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/index.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0256.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0256.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0257.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0257.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0258.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0258.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0287.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0287.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/doctree.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/doctree.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/definitions.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/definitions.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/directives.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/directives.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/introduction.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/introduction.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/mathematics.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/mathematics.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/restructuredtext.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/restructuredtext.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/roles.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/roles.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/config.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/config.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/emacs.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/emacs.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/html.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/html.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/latex.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/latex.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/links.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/links.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/mailing-lists.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/mailing-lists.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/manpage.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/manpage.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/odt.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/odt.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/cheatsheet.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/cheatsheet.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/demo.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/demo.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/quickstart.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/quickstart.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/smartquotes.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/smartquotes.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/tools.txt` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/tools.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_docutils/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/COMMIT_EDITMSG` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/COMMIT_EDITMSG`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/commit-msg.sample` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-commit.sample` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-push.sample` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-rebase.sample` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/prepare-commit-msg.sample` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/update.sample` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/index` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/index`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/info/refs` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/info/refs`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/pack/pack-7e1b1ace85030071ca314cd565ae038bacc302a4.idx` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/pack/pack-7e1b1ace85030071ca314cd565ae038bacc302a4.idx`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/pack/pack-7e1b1ace85030071ca314cd565ae038bacc302a4.pack` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/pack/pack-7e1b1ace85030071ca314cd565ae038bacc302a4.pack`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/packed-refs` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/packed-refs`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_dulwich_log/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_fannkuch/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_fannkuch/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_float/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_float/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_gc_collect/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_gc_collect/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_gc_traversal/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_gc_traversal/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_generators/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_generators/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_genshi/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_genshi/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_go/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_go/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_hexiom/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_hexiom/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_hg_startup/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_hg_startup/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_html5lib/data/w3_tr_html5.html` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_html5lib/data/w3_tr_html5.html`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_html5lib/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_html5lib/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_json_dumps/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_json_dumps/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_json_loads/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_json_loads/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_logging/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_logging/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_mako/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_mako/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_mdp/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_mdp/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_meteor_contest/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_meteor_contest/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_nbody/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_nbody/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_nqueens/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_nqueens/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pathlib/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_pathlib/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pickle/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_pickle/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pidigits/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_pidigits/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pprint/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_pprint/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pyflate/data/interpreter.tar.bz2` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_pyflate/data/interpreter.tar.bz2`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pyflate/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_pyflate/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_python_startup/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_python_startup/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_raytrace/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_raytrace/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_compile/bm_regex_effbot.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_regex_compile/bm_regex_effbot.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_compile/bm_regex_v8.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_regex_compile/bm_regex_v8.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_compile/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_regex_compile/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_dna/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_regex_dna/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_effbot/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_regex_effbot/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_v8/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_regex_v8/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_richards/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_richards/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_richards_super/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_richards_super/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_scimark/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_scimark/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_spectral_norm/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_spectral_norm/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlalchemy_declarative/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_sqlalchemy_declarative/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlalchemy_imperative/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_sqlalchemy_imperative/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlglot/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_sqlglot/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlite_synth/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_sqlite_synth/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sympy/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_sympy/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_telco/data/telco-bench.b` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_telco/data/telco-bench.b`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_telco/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_telco/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_tomli_loads/data/tomli-bench-data.toml` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_tomli_loads/data/tomli-bench-data.toml`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_tomli_loads/generate_data.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_tomli_loads/generate_data.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_tomli_loads/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_tomli_loads/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_tornado_http/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_tornado_http/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_typing_runtime_protocols/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_typing_runtime_protocols/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_unpack_sequence/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_unpack_sequence/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_xml_etree/run_benchmark.py` & `pyperformance-1.0.9/pyperformance/data-files/benchmarks/bm_xml_etree/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/run.py` & `pyperformance-1.0.9/pyperformance/run.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance/venv.py` & `pyperformance-1.0.9/pyperformance/venv.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/pyperformance.egg-info/PKG-INFO` & `pyperformance-1.0.9/pyperformance.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyperformance
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python benchmark suite
 Author: Collin Winter, Jeffrey Yasskin
 License: MIT
 Project-URL: Homepage, https://github.com/python/pyperformance
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyperformance-1.0.8/pyproject.toml` & `pyperformance-1.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.8/requirements.in` & `pyperformance-1.0.9/requirements.in`

 * *Files identical despite different names*

