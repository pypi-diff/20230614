# Comparing `tmp/pyblock3-0.2.6.tar.gz` & `tmp/pyblock3-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyblock3-0.2.6.tar", last modified: Mon Sep  5 23:48:46 2022, max compression
+gzip compressed data, was "pyblock3-0.2.7.tar", last modified: Wed Jun 14 11:05:54 2023, max compression
```

## Comparing `pyblock3-0.2.6.tar` & `pyblock3-0.2.7.tar`

### file list

```diff
@@ -1,111 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 23:48:46.819071 pyblock3-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (121)    10224 2022-09-05 23:48:23.000000 pyblock3-0.2.6/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-09-05 23:48:23.000000 pyblock3-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-09-05 23:48:23.000000 pyblock3-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7052 2022-09-05 23:48:46.815071 pyblock3-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6704 2022-09-05 23:48:23.000000 pyblock3-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 23:48:46.807071 pyblock3-0.2.6/pyblock3/
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 23:48:46.811071 pyblock3-0.2.6/pyblock3/algebra/
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algebra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 23:48:46.811071 pyblock3-0.2.6/pyblock3/algebra/ad/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algebra/ad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    58810 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algebra/ad/flat.py
--rw-r--r--   0 runner    (1001) docker     (121)    25441 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algebra/ad/flat_impl.py
--rw-r--r--   0 runner    (1001) docker     (121)    23719 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algebra/ad/mps.py
--rw-r--r--   0 runner    (1001) docker     (121)    84642 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algebra/core.py
--rw-r--r--   0 runner    (1001) docker     (121)    77564 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algebra/fermion.py
--rw-r--r--   0 runner    (1001) docker     (121)     1278 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algebra/fermion_encoding.py
--rw-r--r--   0 runner    (1001) docker     (121)    33077 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algebra/fermion_large.py
--rw-r--r--   0 runner    (1001) docker     (121)    18829 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algebra/fermion_ops.py
--rw-r--r--   0 runner    (1001) docker     (121)     1737 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algebra/fermion_setting.py
--rw-r--r--   0 runner    (1001) docker     (121)     8225 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algebra/fermion_symmetry.py
--rw-r--r--   0 runner    (1001) docker     (121)    57471 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algebra/flat.py
--rw-r--r--   0 runner    (1001) docker     (121)    11001 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algebra/flat_functor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1604 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algebra/funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 23:48:46.811071 pyblock3-0.2.6/pyblock3/algebra/impl/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algebra/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24634 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algebra/impl/flat.py
--rw-r--r--   0 runner    (1001) docker     (121)      998 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algebra/integrate.py
--rw-r--r--   0 runner    (1001) docker     (121)     8135 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algebra/linalg.py
--rw-r--r--   0 runner    (1001) docker     (121)    23284 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algebra/mpe.py
--rw-r--r--   0 runner    (1001) docker     (121)    26255 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algebra/mps.py
--rw-r--r--   0 runner    (1001) docker     (121)     7797 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algebra/symmetry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 23:48:46.811071 pyblock3-0.2.6/pyblock3/algebra/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algebra/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6498 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algebra/tests/test_boson_cpp.py
--rw-r--r--   0 runner    (1001) docker     (121)     7888 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algebra/tests/test_boson_python.py
--rw-r--r--   0 runner    (1001) docker     (121)     7609 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algebra/tests/test_fermion_cpp.py
--rw-r--r--   0 runner    (1001) docker     (121)     7498 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algebra/tests/test_fermion_large.py
--rw-r--r--   0 runner    (1001) docker     (121)    10548 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algebra/tests/test_fermion_ops.py
--rw-r--r--   0 runner    (1001) docker     (121)     8829 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algebra/tests/test_fermion_python.py
--rw-r--r--   0 runner    (1001) docker     (121)     8764 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algebra/tests/test_symmetry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 23:48:46.811071 pyblock3-0.2.6/pyblock3/algorithms/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7554 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algorithms/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     7824 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algorithms/dmrg.py
--rw-r--r--   0 runner    (1001) docker     (121)     5380 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algorithms/green.py
--rw-r--r--   0 runner    (1001) docker     (121)     4267 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algorithms/linear.py
--rw-r--r--   0 runner    (1001) docker     (121)     5630 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algorithms/tddmrg.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 23:48:46.811071 pyblock3-0.2.6/pyblock3/algorithms/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algorithms/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2871 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algorithms/tests/test_dmrg.py
--rw-r--r--   0 runner    (1001) docker     (121)     2042 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algorithms/tests/test_ghf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1422 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algorithms/tests/test_sa.py
--rw-r--r--   0 runner    (1001) docker     (121)     3345 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/algorithms/tests/test_soc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 23:48:46.811071 pyblock3-0.2.6/pyblock3/block2/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/block2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11753 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/block2/hamil.py
--rw-r--r--   0 runner    (1001) docker     (121)    22856 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/block2/io.py
--rw-r--r--   0 runner    (1001) docker     (121)    25632 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/fcidump.py
--rw-r--r--   0 runner    (1001) docker     (121)    16903 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/hamiltonian.py
--rw-r--r--   0 runner    (1001) docker     (121)     7790 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/heisenberg.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 23:48:46.815071 pyblock3-0.2.6/pyblock3/symbolic/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/symbolic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11748 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/symbolic/expr.py
--rw-r--r--   0 runner    (1001) docker     (121)    37664 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/symbolic/symbolic.py
--rw-r--r--   0 runner    (1001) docker     (121)    22316 2022-09-05 23:48:23.000000 pyblock3-0.2.6/pyblock3/symbolic/symbolic_mpo.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 23:48:46.807071 pyblock3-0.2.6/pyblock3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7052 2022-09-05 23:48:46.000000 pyblock3-0.2.6/pyblock3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2565 2022-09-05 23:48:46.000000 pyblock3-0.2.6/pyblock3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-05 23:48:46.000000 pyblock3-0.2.6/pyblock3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-09-05 23:48:46.000000 pyblock3-0.2.6/pyblock3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-09-05 23:48:46.000000 pyblock3-0.2.6/pyblock3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-05 23:48:46.819071 pyblock3-0.2.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     3244 2022-09-05 23:48:24.000000 pyblock3-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 23:48:46.815071 pyblock3-0.2.6/src/
--rw-r--r--   0 runner    (1001) docker     (121)     8996 2022-09-05 23:48:23.000000 pyblock3-0.2.6/src/bond_info.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     4662 2022-09-05 23:48:23.000000 pyblock3-0.2.6/src/bond_info.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-09-05 23:48:23.000000 pyblock3-0.2.6/src/bond_info_tmpl.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    10314 2022-09-05 23:48:23.000000 pyblock3-0.2.6/src/fermion_symmetry.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    35638 2022-09-05 23:48:23.000000 pyblock3-0.2.6/src/flat_fermion.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2777 2022-09-05 23:48:23.000000 pyblock3-0.2.6/src/flat_fermion.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     2435 2022-09-05 23:48:23.000000 pyblock3-0.2.6/src/flat_fermion_tmpl.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    26392 2022-09-05 23:48:23.000000 pyblock3-0.2.6/src/flat_functor.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3396 2022-09-05 23:48:23.000000 pyblock3-0.2.6/src/flat_functor.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     3253 2022-09-05 23:48:23.000000 pyblock3-0.2.6/src/flat_functor_tmpl.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    73839 2022-09-05 23:48:23.000000 pyblock3-0.2.6/src/flat_sparse.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    11959 2022-09-05 23:48:23.000000 pyblock3-0.2.6/src/flat_sparse.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    10372 2022-09-05 23:48:23.000000 pyblock3-0.2.6/src/flat_sparse_tmpl.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 23:48:46.815071 pyblock3-0.2.6/src/gpu/
--rw-r--r--   0 runner    (1001) docker     (121)     3067 2022-09-05 23:48:23.000000 pyblock3-0.2.6/src/gpu/flat_fermion.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     2652 2022-09-05 23:48:23.000000 pyblock3-0.2.6/src/gpu/flat_fermion_tmpl.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    39837 2022-09-05 23:48:23.000000 pyblock3-0.2.6/src/hamiltonian.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1918 2022-09-05 23:48:23.000000 pyblock3-0.2.6/src/hamiltonian.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    42218 2022-09-05 23:48:23.000000 pyblock3-0.2.6/src/hamiltonian_ptree.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1221 2022-09-05 23:48:23.000000 pyblock3-0.2.6/src/hamiltonian_ptree.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    59786 2022-09-05 23:48:23.000000 pyblock3-0.2.6/src/main.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     6871 2022-09-05 23:48:23.000000 pyblock3-0.2.6/src/max_flow.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    36058 2022-09-05 23:48:23.000000 pyblock3-0.2.6/src/qc_expr.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    23892 2022-09-05 23:48:23.000000 pyblock3-0.2.6/src/qc_hamiltonian.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1117 2022-09-05 23:48:23.000000 pyblock3-0.2.6/src/qc_hamiltonian.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    26524 2022-09-05 23:48:23.000000 pyblock3-0.2.6/src/qc_mpo.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    10579 2022-09-05 23:48:23.000000 pyblock3-0.2.6/src/qc_symbolic.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     1575 2022-09-05 23:48:23.000000 pyblock3-0.2.6/src/symmetry_tmpl.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     3442 2022-09-05 23:48:23.000000 pyblock3-0.2.6/src/sz.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     7033 2022-09-05 23:48:23.000000 pyblock3-0.2.6/src/tensor.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3339 2022-09-05 23:48:23.000000 pyblock3-0.2.6/src/tensor.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     9043 2022-09-05 23:48:23.000000 pyblock3-0.2.6/src/tensor_einsum.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1450 2022-09-05 23:48:23.000000 pyblock3-0.2.6/src/tensor_einsum.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     7495 2022-09-05 23:48:23.000000 pyblock3-0.2.6/src/tensor_impl.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    30167 2022-09-05 23:48:23.000000 pyblock3-0.2.6/src/tensor_impl.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:54.825503 pyblock3-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-06-14 11:05:36.000000 pyblock3-0.2.7/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-14 11:05:36.000000 pyblock3-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-14 11:05:36.000000 pyblock3-0.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-06-14 11:05:54.821503 pyblock3-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-06-14 11:05:36.000000 pyblock3-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:54.805503 pyblock3-0.2.7/pyblock3/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:54.809503 pyblock3-0.2.7/pyblock3/algebra/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:54.813503 pyblock3-0.2.7/pyblock3/algebra/ad/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/ad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94198 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/ad/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41261 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/ad/fermion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18791 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/ad/fermion_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58861 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/ad/flat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25405 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/ad/flat_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24467 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/ad/mps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87649 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/einsum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82436 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/fermion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/fermion_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33077 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/fermion_large.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18829 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/fermion_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/fermion_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8371 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/fermion_symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58423 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/flat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11178 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/flat_functor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:54.813503 pyblock3-0.2.7/pyblock3/algebra/impl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24602 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/impl/flat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/integrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23715 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/mpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28783 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/mps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/symmetry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:54.813503 pyblock3-0.2.7/pyblock3/algebra/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/tests/test_boson_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/tests/test_boson_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/tests/test_fermion_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/tests/test_fermion_large.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/tests/test_fermion_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/tests/test_fermion_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algebra/tests/test_symmetry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:54.813503 pyblock3-0.2.7/pyblock3/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algorithms/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7824 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algorithms/dmrg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algorithms/green.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algorithms/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algorithms/tddmrg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:54.817503 pyblock3-0.2.7/pyblock3/algorithms/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algorithms/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algorithms/tests/test_dmrg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algorithms/tests/test_ghf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algorithms/tests/test_sa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/algorithms/tests/test_soc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:54.817503 pyblock3-0.2.7/pyblock3/block2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/block2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/block2/hamil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23824 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/block2/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25632 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/fcidump.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:54.817503 pyblock3-0.2.7/pyblock3/gaussian/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/gaussian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45689 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/gaussian/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16903 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/hamiltonian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/heisenberg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:54.817503 pyblock3-0.2.7/pyblock3/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/symbolic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11748 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/symbolic/expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37662 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/symbolic/symbolic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22316 2023-06-14 11:05:36.000000 pyblock3-0.2.7/pyblock3/symbolic/symbolic_mpo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:54.809503 pyblock3-0.2.7/pyblock3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-06-14 11:05:54.000000 pyblock3-0.2.7/pyblock3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-06-14 11:05:54.000000 pyblock3-0.2.7/pyblock3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:05:54.000000 pyblock3-0.2.7/pyblock3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-14 11:05:54.000000 pyblock3-0.2.7/pyblock3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 11:05:54.000000 pyblock3-0.2.7/pyblock3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 11:05:54.825503 pyblock3-0.2.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3446 2023-06-14 11:05:36.000000 pyblock3-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:54.821503 pyblock3-0.2.7/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     8996 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/bond_info.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/bond_info.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/bond_info_tmpl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/fermion_symmetry.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    35673 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/flat_fermion.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/flat_fermion.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/flat_fermion_tmpl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26561 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/flat_functor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/flat_functor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/flat_functor_tmpl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    74291 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/flat_sparse.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/flat_sparse.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10372 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/flat_sparse_tmpl.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:05:54.821503 pyblock3-0.2.7/src/gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/gpu/flat_fermion.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/gpu/flat_fermion_tmpl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    39837 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/hamiltonian.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/hamiltonian.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    42218 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/hamiltonian_ptree.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/hamiltonian_ptree.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    59786 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/max_flow.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    36058 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/qc_expr.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23892 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/qc_hamiltonian.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/qc_hamiltonian.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26524 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/qc_mpo.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/qc_symbolic.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/symmetry_tmpl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/sz.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/tensor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/tensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/tensor_einsum.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/tensor_einsum.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/tensor_impl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30167 2023-06-14 11:05:36.000000 pyblock3-0.2.7/src/tensor_impl.hpp
```

### Comparing `pyblock3-0.2.6/CMakeLists.txt` & `pyblock3-0.2.7/CMakeLists.txt`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 FIND_PROGRAM(CMAKE_C_COMPILER NAMES $ENV{CC} gcc PATHS ENV PATH NO_DEFAULT_PATH)
 FIND_PROGRAM(CMAKE_CXX_COMPILER NAMES $ENV{CXX} g++ PATHS ENV PATH NO_DEFAULT_PATH)
 
 OPTION(USE_MKL "MKL" OFF)
 OPTION(USE_HPTT "HPTT" OFF)
 OPTION(USE_GPU "GPU" OFF)
+OPTION(ARCH_ARM64 "MacOS arch arm64" OFF)
 
 IF (${USE_GPU})
     CMAKE_MINIMUM_REQUIRED(VERSION 3.9)
     FIND_PROGRAM(CMAKE_CUDA_COMPILER NAMES $ENV{NVCC} nvcc PATHS ENV PATH NO_DEFAULT_PATH)
     ENABLE_LANGUAGE(CUDA)
 ENDIF()
 
@@ -76,14 +77,22 @@
     SET(XPREP -Xpreprocessor)
     INCLUDE_DIRECTORIES(/usr/local/include)
 ENDIF()
 
 SET(PTHREAD pthread)
 CMAKE_POLICY(SET CMP0054 NEW) # quoted variable for STREQUAL
 
+IF (${ARCH_ARM64})
+    SET(ARCH_FLAG -arch arm64)
+    SET(ARCH_LINK_FLAGS "-arch arm64")
+ELSE()
+    SET(ARCH_FLAG "")
+    SET(ARCH_LINK_FLAGS "")
+ENDIF()
+
 IF (CMAKE_CXX_COMPILER_ID STREQUAL "Intel")
     SET(OMP_FLAG -qopenmp)
 ELSEIF (CMAKE_CXX_COMPILER_ID STREQUAL "MSVC")
     SET(OMP_FLAG -openmp)
 ELSE()
     SET(OMP_FLAG -fopenmp)
 ENDIF()
@@ -119,15 +128,23 @@
         SET(PTHREAD "")
     ENDIF()
     SET(MKL_OMP_LIB_NAME mkl_tbb_thread)
 ELSEIF (CMAKE_CXX_COMPILER_ID STREQUAL "Intel")
     FIND_LIBRARY(OMP_LIB_NAME NAMES iomp5 PATHS /usr/local/lib /usr/lib64 ${PYTHON_LIB_PATH})
     SET(MKL_OMP_LIB_NAME mkl_intel_thread)
 ELSEIF (CMAKE_CXX_COMPILER_ID STREQUAL "AppleClang")
-    FIND_LIBRARY(OMP_LIB_NAME NAMES iomp5 PATHS /usr/local/lib /usr/lib64 ${PYTHON_LIB_PATH})
+    IF("${OMP_LIB}" STREQUAL "OMP")
+        SET(OMP_LIB_FIND_NAME omp)
+    ELSE()
+        SET(OMP_LIB_FIND_NAME iomp5)
+    ENDIF()
+    FIND_LIBRARY(OMP_LIB_NAME NAMES ${OMP_LIB_FIND_NAME} PATHS $ENV{OMPROOT} $ENV{OMPROOT}/lib NO_DEFAULT_PATH)
+    IF (NOT OMP_LIB_NAME)
+        FIND_LIBRARY(OMP_LIB_NAME NAMES ${OMP_LIB_FIND_NAME} PATHS /usr/local/lib /usr/lib64 ${PYTHON_LIB_PATH})
+    ENDIF()
     SET(MKL_OMP_LIB_NAME mkl_intel_thread)
 ELSE()
     SET(OMP_LIB GNU)
     FIND_LIBRARY(OMP_LIB_NAME NAMES gomp PATHS /usr/local/lib /usr/lib64 ${PYTHON_LIB_PATH})
     IF (NOT OMP_LIB_NAME)
         EXECUTE_PROCESS(
             COMMAND ${CMAKE_CXX_COMPILER} -print-search-dirs
@@ -233,13 +250,15 @@
 IF ((NOT APPLE) AND (NOT WIN32))
     TARGET_LINK_LIBRARIES(${PROJECT_NAME} PUBLIC rt)
 ENDIF()
 
 TARGET_LINK_LIBRARIES(${PROJECT_NAME} PUBLIC ${OMP_LIB_NAME} ${PTHREAD})
 TARGET_LINK_LIBRARIES(${PROJECT_NAME} PUBLIC ${LAPACK_LIBRARIES} ${BLAS_LIBRARIES} ${MKL_LIBS} ${HPTT_LIB} ${CUT_LIB})
 
+MESSAGE(STATUS "ARCH_FLAG = ${ARCH_FLAG}")
 MESSAGE(STATUS "OPT_FLAG = ${OPT_FLAG}")
 MESSAGE(STATUS "OMP_LIB = ${OMP_LIB_NAME}")
 
 TARGET_INCLUDE_DIRECTORIES(${PROJECT_NAME} PUBLIC ${PYTHON_INCLUDE_DIRS} ${PYBIND_INCLUDE_DIRS} ${MKL_INCLUDE_DIR}
     ${HPTT_INCLUDE_DIR} ${CUT_INCLUDE_DIR} ${MGPU_INCLUDE_DIR})
-TARGET_COMPILE_OPTIONS(${PROJECT_NAME} BEFORE PRIVATE ${OPT_FLAG} ${MKL_FLAG} ${HPTT_FLAG} ${GPU_FLAG})
+TARGET_COMPILE_OPTIONS(${PROJECT_NAME} BEFORE PRIVATE ${OPT_FLAG} ${ARCH_FLAG} ${MKL_FLAG} ${HPTT_FLAG} ${GPU_FLAG})
+SET_TARGET_PROPERTIES(${PROJECT_NAME} PROPERTIES LINK_FLAGS "${ARCH_LINK_FLAGS}")
```

### Comparing `pyblock3-0.2.6/LICENSE` & `pyblock3-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/PKG-INFO` & `pyblock3-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyblock3
-Version: 0.2.6
+Version: 0.2.7
 Summary: An efficient python block-sparse tensor and MPS/DMRG library.
 Home-page: https://github.com/block-hczhai/pyblock3-preview
 Author: Huanchen Zhai, Yang Gao, and Garnet K.-L. Chan
 Author-email: hczhai@ucla.edu
 License: LICENSE
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -60,14 +60,20 @@
 Installation
 ------------
 
 Using ``pip``:
 
     pip install pyblock3
 
+To install the most recent development version, use:
+
+    pip install pyblock3==<version> --extra-index-url=https://block-hczhai.github.io/pyblock3-preview/pypi/
+
+where ``<version>`` can be some development version number like ``0.2.7rc5``.
+
 Or you can compile it manually:
 
 Dependence: `python3`, `psutil`, `numba`, and `numpy` (version >= 1.17.0). pyblock3 can run in pure python mode,
 in which no C++ source code is required to be compiled.
 
 For optimal performance, the C++ source code is used and there are some additional dependences:
```

### Comparing `pyblock3-0.2.6/README.md` & `pyblock3-0.2.7/pyblock3.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: pyblock3
+Version: 0.2.7
+Summary: An efficient python block-sparse tensor and MPS/DMRG library.
+Home-page: https://github.com/block-hczhai/pyblock3-preview
+Author: Huanchen Zhai, Yang Gao, and Garnet K.-L. Chan
+Author-email: hczhai@ucla.edu
+License: LICENSE
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 
 [![Documentation Status](https://readthedocs.org/projects/pyblock3/badge/?version=latest)](https://pyblock3.readthedocs.io/en/latest/?badge=latest)
 [![Build Status](https://github.com/block-hczhai/pyblock3-preview/workflows/build/badge.svg)](https://github.com/block-hczhai/pyblock3-preview/actions/workflows/build.yml)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![PyPI version](https://badge.fury.io/py/pyblock3.svg)](https://badge.fury.io/py/pyblock3)
 
 pyblock3
@@ -49,14 +60,20 @@
 Installation
 ------------
 
 Using ``pip``:
 
     pip install pyblock3
 
+To install the most recent development version, use:
+
+    pip install pyblock3==<version> --extra-index-url=https://block-hczhai.github.io/pyblock3-preview/pypi/
+
+where ``<version>`` can be some development version number like ``0.2.7rc5``.
+
 Or you can compile it manually:
 
 Dependence: `python3`, `psutil`, `numba`, and `numpy` (version >= 1.17.0). pyblock3 can run in pure python mode,
 in which no C++ source code is required to be compiled.
 
 For optimal performance, the C++ source code is used and there are some additional dependences:
```

### Comparing `pyblock3-0.2.6/pyblock3/algebra/ad/flat.py` & `pyblock3-0.2.7/pyblock3/algebra/ad/flat.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,15 @@
         for i in range(n_blocks):
             shapes[i] = spt.blocks[i].shape
             q_labels[i] = list(map(SZ.to_flat, spt.blocks[i].q_labels))
         idxs = np.zeros((n_blocks + 1, ), dtype=np.uint64)
         idxs[1:] = np.cumsum(shapes.prod(axis=1), dtype=np.uint64)
         data = np.zeros((idxs[-1], ), dtype=spt.dtype)
         for i in range(n_blocks):
-            data[idxs[i]:idxs[i + 1]] = spt.blocks[i].flatten()
+            data[idxs[i]:idxs[i + 1]] = spt.blocks[i].ravel()
         return FlatSparseTensor(q_labels, shapes, data, idxs)
     
     @staticmethod
     def from_flat(ft):
         return FlatSparseTensor(ft.q_labels, ft.shapes, ft.data, ft.idxs)
 
     def __str__(self):
@@ -468,18 +468,21 @@
             idxb = np.arange(0, axes, dtype=np.int32)
         else:
             idxa = np.array(axes[0], dtype=np.int32)
             idxb = np.array(axes[1], dtype=np.int32)
         idxa[idxa < 0] += a.ndim
         idxb[idxb < 0] += b.ndim
 
-        return a.__class__(*flat_sparse_tensordot(
+        r = a.__class__(*flat_sparse_tensordot(
             a.q_labels, a.shapes, a.data, a.idxs,
             b.q_labels, b.shapes, b.data, b.idxs,
             idxa, idxb))
+        if r.ndim == 0:
+            r = r.item()
+        return r
 
     def tensordot(self, b, axes=2):
         return np.tensordot(self, b, axes)
 
     @staticmethod
     def _hdot(a, b, out=None):
         """Horizontal contraction (contracting connected virtual dimensions)."""
@@ -710,15 +713,15 @@
             return v.__class__(
                 q_labels=v.q_labels[mask, 0], shapes=shapes,
                 data=jnp.concatenate([jnp.diag(v.data[i:j].reshape(sh, sh)) for i, j, sh in zip(v.idxs[:-1][mask], v.idxs[1:][mask], shapes)]))
         elif v.ndim == 1:
             return v.__class__(
                 q_labels=np.repeat(v.q_labels, 2, axis=1),
                 shapes=np.repeat(v.shapes, 2, axis=1),
-                data=jnp.concatenate([jnp.diag(v.data[i:j]).flatten() for i, j in zip(v.idxs, v.idxs[1:])]))
+                data=jnp.concatenate([jnp.diag(v.data[i:j]).ravel() for i, j in zip(v.idxs, v.idxs[1:])]))
         elif v.n_blocks != 0:
             raise RuntimeError("ndim for np.diag must be 1 or 2.")
         else:
             return v
 
     def diag(self):
         return np.diag(self)
@@ -780,20 +783,20 @@
         even : FlatSparseTensor
             Including blocks with even fermion parity.
     """
 
     def __init__(self, odd=None, even=None):
         self.odd = odd if odd is not None else FlatFermionTensor.ZERO
         self.even = even if even is not None else FlatFermionTensor.ZERO
-    
+
     def pytree_flatten(self):
         traced = (self.odd, self.even)
         others = ()
         return traced, others
-    
+
     @classmethod
     def pytree_unflatten(cls, others, traced):
         odd, even = traced
         return cls(odd=odd, even=even)
 
     def __array_ufunc__(self, ufunc, method, *inputs, **kwargs):
         if ufunc in _flat_fermion_tensor_numpy_func_impls:
```

### Comparing `pyblock3-0.2.6/pyblock3/algebra/ad/flat_impl.py` & `pyblock3-0.2.7/pyblock3/algebra/ad/flat_impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,17 +64,17 @@
                 mat = jnp.tensordot(mata, matb, axes=(list(idxa), list(idxb)))
                 outqk = outq.tobytes()
                 if outqk not in blocks_map:
                     blocks_map[outqk] = len(qs)
                     idxs.append(idxs[-1] + mat.size)
                     qs.append(outq)
                     shapes.append(mat.shape)
-                    mats.append(mat.flatten())
+                    mats.append(mat.ravel())
                 else:
-                    mats[blocks_map[outqk]] += mat.flatten()
+                    mats[blocks_map[outqk]] += mat.ravel()
 
     return (np.array(qs, dtype=np.uint32),
             np.array(shapes, dtype=np.uint32),
             jnp.concatenate(mats) if len(mats) != 0 else np.array(
                 [], dtype=adata.dtype),
             np.array(idxs, dtype=np.uint64))
 
@@ -146,25 +146,25 @@
         for qs in items[q][0]:
             if qs == pqs:
                 continue
             k, sh = linfo.finfo[q][qs]
             nk = np.multiply.reduce(sh)
             qq = np.array([x.to_flat() for x in qs + (q, )], dtype=aqs.dtype)
             sh = np.array(sh + (l.shape[-1], ), dtype=ashs.dtype)
-            l_blocks.append((qq, sh, l[k:k + nk, :].flatten()))
+            l_blocks.append((qq, sh, l[k:k + nk, :].ravel()))
             pqs = qs
         pqs = None
         for qs in items[q][1]:
             if qs == pqs:
                 continue
             k, sh = rinfo.finfo[q][qs]
             nk = np.multiply.reduce(sh)
             qq = np.array([x.to_flat() for x in (q, ) + qs], dtype=aqs.dtype)
             sh = np.array((r.shape[0], ) + sh, dtype=ashs.dtype)
-            r_blocks.append((qq, sh, r[:, k:k + nk].flatten()))
+            r_blocks.append((qq, sh, r[:, k:k + nk].ravel()))
             pqs = qs
     lqs = np.array([xl[0] for xl in l_blocks], dtype=aqs.dtype)
     lshs = np.array([xl[1] for xl in l_blocks], dtype=ashs.dtype)
     ldata = jnp.concatenate([xl[2] for xl in l_blocks])
     rqs = np.array([xr[0] for xr in r_blocks], dtype=aqs.dtype)
     rshs = np.array([xr[1] for xr in r_blocks], dtype=ashs.dtype)
     rdata = jnp.concatenate([xr[2] for xr in r_blocks])
@@ -199,25 +199,25 @@
         l_shapes = np.prod(pashs, axis=1)
         mat = jnp.concatenate([adata[aidxs[ia]:aidxs[ia + 1]].reshape((sh, -1))
                               for sh, ia in zip(l_shapes, v)], axis=0)
         l, s, r = jnp.linalg.svd(mat, full_matrices=False)
         rqs[ir, :] = qq
         rshs[ir] = r.shape
         ridxs[ir + 1] = ridxs[ir] + r.size
-        rmats[ir] = r.flatten()
+        rmats[ir] = r.ravel()
         sqs[ir, 0] = qq
         sshs[ir, 0] = s.shape[0]
         sidxs[ir + 1] = sidxs[ir] + s.shape[0]
         smats[ir] = s
         ls = np.split(l, list(accumulate(l_shapes[:-1])), axis=0)
         assert len(ls) == len(v)
         lshs[v, -1] = l.shape[-1]
         lidx[ill:ill + len(v)] = v
         for q, ia in zip(ls, v):
-            lmats[ia] = q.flatten()
+            lmats[ia] = q.ravel()
             ill += 1
     assert ill == nblocks_l
     rr = lqs[lidx], lshs[lidx], jnp.concatenate([lmats[x] for x in lidx]), None, \
         sqs, sshs, jnp.concatenate(smats), sidxs, \
         rqs, rshs, jnp.concatenate(rmats), ridxs
     return (rr, lidx) if indexed else r
 
@@ -249,25 +249,25 @@
         r_shapes = np.prod(pashs, axis=1)
         mat = jnp.concatenate(
             [adata[aidxs[ia]:aidxs[ia + 1]].reshape((-1, sh)) for sh, ia in zip(r_shapes, v)], axis=1)
         l, s, r = jnp.linalg.svd(mat, full_matrices=False)
         lqs[il, :] = qq
         lshs[il] = l.shape
         lidxs[il + 1] = lidxs[il] + l.size
-        lmats[il] = l.flatten()
+        lmats[il] = l.ravel()
         sqs[il, 0] = qq
         sshs[il, 0] = s.shape[0]
         sidxs[il + 1] = sidxs[il] + s.shape[0]
         smats[il] = s
         rs = np.split(r, list(accumulate(r_shapes[:-1])), axis=1)
         assert len(rs) == len(v)
         rshs[v, 0] = r.shape[0]
         ridx[irr:irr + len(v)] = v
         for q, ia in zip(rs, v):
-            rmats[ia] = q.flatten()
+            rmats[ia] = q.ravel()
             irr += 1
     assert irr == nblocks_r
     rr = lqs, lshs, jnp.concatenate(lmats), lidxs, \
         sqs, sshs, jnp.concatenate(smats), sidxs, \
         rqs[ridx], rshs[ridx], jnp.concatenate([rmats[x] for x in ridx]), None
     return (rr, ridx) if indexed else rr
 
@@ -292,20 +292,20 @@
         l_shapes = np.prod(pashs, axis=1)
         mat = jnp.concatenate([adata[aidxs[ia]:aidxs[ia + 1]].reshape((sh, -1))
                               for sh, ia in zip(l_shapes, v)], axis=0)
         q, r = jnp.linalg.qr(mat, mode='reduced')
         rqs[ir, :] = qq
         rshs[ir] = r.shape
         ridxs[ir + 1] = ridxs[ir] + r.size
-        rmats[ir] = r.flatten()
+        rmats[ir] = r.ravel()
         qs = np.split(q, list(accumulate(l_shapes[:-1])), axis=0)
         assert len(qs) == len(v)
         qshs[v, -1] = r.shape[0]
         for q, ia in zip(qs, v):
-            qmats[ia] = q.flatten()
+            qmats[ia] = q.ravel()
     return qqs, qshs, jnp.concatenate(qmats), None, rqs, rshs, jnp.concatenate(rmats), ridxs
 
 
 def flat_sparse_right_canonicalize(aqs, ashs, adata, aidxs):
     collected_cols = {}
     for i, q in enumerate(aqs[:, 0]):
         if q not in collected_cols:
@@ -325,20 +325,20 @@
         r_shapes = np.prod(pashs, axis=1)
         mat = jnp.concatenate(
             [adata[aidxs[ia]:aidxs[ia + 1]].reshape((-1, sh)).T for sh, ia in zip(r_shapes, v)], axis=0)
         q, r = jnp.linalg.qr(mat, mode='reduced')
         lqs[il, :] = qq
         lshs[il] = r.shape[::-1]
         lidxs[il + 1] = lidxs[il] + r.size
-        lmats[il] = r.T.flatten()
+        lmats[il] = r.T.ravel()
         qs = np.split(q, list(accumulate(r_shapes[:-1])), axis=0)
         assert len(qs) == len(v)
         qshs[v, 0] = r.shape[0]
         for q, ia in zip(qs, v):
-            qmats[ia] = q.T.flatten()
+            qmats[ia] = q.T.ravel()
     return lqs, lshs, jnp.concatenate(lmats), lidxs, qqs, qshs, jnp.concatenate(qmats), None
 
 
 def flat_sparse_left_svd_indexed(aqs, ashs, adata, aidxs):
     return flat_sparse_left_svd(aqs, ashs, adata, aidxs, indexed=True)
 
 
@@ -352,15 +352,15 @@
 
 def flat_sparse_right_canonicalize_indexed(aqs, ashs, adata, aidxs):
     return flat_sparse_right_canonicalize(aqs, ashs, adata, aidxs), np.arange(0, aqs.shape[0], dtype=int)
 
 
 def flat_sparse_transpose(aqs, ashs, adata, aidxs, axes):
     data = jnp.concatenate(
-        [jnp.transpose(adata[i:j].reshape(sh), axes=axes).flatten()
+        [jnp.transpose(adata[i:j].reshape(sh), axes=axes).ravel()
          for i, j, sh in zip(aidxs, aidxs[1:], ashs)])
     return (aqs[:, axes], ashs[:, axes], data, aidxs)
 
 
 def flat_sparse_get_infos(aqs, ashs):
     if len(aqs) == 0:
         return ()
@@ -452,15 +452,15 @@
         rsh[idxs[0]] = nk
         sl = tuple(slice(None) if ix != idxs[0] else slice(
             k, k + nk) for ix in range(len(rq)))
         # rdata[sl] = adata[aidxs[ia]:aidxs[ia + 1]].reshape(rsh)
         blocks_map[zrq] = (blocks_map[zrq][0], blocks_map[zrq][1],
             rdata.at[sl].set(adata[aidxs[ia]:aidxs[ia + 1]].reshape(rsh)))
     rqs, rshs, rdata = zip(*blocks_map.values())
-    return np.array(rqs, dtype=np.uint32), np.array(rshs, dtype=np.uint32), jnp.concatenate([d.flatten() for d in rdata]), None
+    return np.array(rqs, dtype=np.uint32), np.array(rshs, dtype=np.uint32), jnp.concatenate([d.ravel() for d in rdata]), None
 
 
 def flat_sparse_trans_fusing_info(info):
     import block3.sz as block3
     minfo = block3.MapFusing()
     for k, v in info.items():
         mp = block3.MapVUIntPUV()
@@ -523,28 +523,28 @@
         mat.shape = cshs[ic]
         # mat[: ashs[ia, 0], ..., : ashs[ia, -1]] += \
         #     adata[aidxs[ia]:aidxs[ia + 1]].reshape(ashs[ia])
         xmat = mat.at[: ashs[ia, 0], ..., : ashs[ia, -1]].set(
             mat[: ashs[ia, 0], ..., : ashs[ia, -1]]
             + adata[aidxs[ia]:aidxs[ia + 1]].reshape(ashs[ia])
         )
-        cdata = cdata.at[cidxs[ic]:cidxs[ic + 1]].set(xmat.flatten())
+        cdata = cdata.at[cidxs[ic]:cidxs[ic + 1]].set(xmat.ravel())
 
     # copy b blocks to smaller index in new block
     for ib, q in xbqs:
         ic = ic_map[sub_mp[q]]
         mat = cdata[cidxs[ic]:cidxs[ic + 1]]
         mat.shape = cshs[ic]
         # mat[-int(bshs[ib, 0]):, ..., -int(bshs[ib, -1]):] += \
         #     bdata[bidxs[ib]:bidxs[ib + 1]].reshape(bshs[ib])
         xmat = mat.at[-int(bshs[ib, 0]):, ..., -int(bshs[ib, -1]):].set(
             mat[-int(bshs[ib, 0]):, ..., -int(bshs[ib, -1]):]
             + bdata[bidxs[ib]:bidxs[ib + 1]].reshape(bshs[ib])
         )
-        cdata = cdata.at[cidxs[ic]:cidxs[ic + 1]].set(xmat.flatten())
+        cdata = cdata.at[cidxs[ic]:cidxs[ic + 1]].set(xmat.ravel())
 
     return cqs, cshs, cdata, cidxs
 
 
 def flat_sparse_truncate_svd(lqs, lshs, ldata, lidxs, sqs, sshs, sdata, sidxs,
                              rqs, rshs, rdata, ridxs, max_bond_dim=-1, cutoff=0.0,
                              max_dw=0.0, norm_cutoff=0.0, eigen_values=False):
@@ -597,15 +597,15 @@
         nkl, nkr = 0, 0
         while ikl + nkl < nl and lqs[ikl + nkl, -1] == sqs[ik, 0]:
             nkl += 1
         if nkl != 0:
             sh = lshs[ikl:ikl + nkl].copy()
             sh[:, -1] = ng
             dt = ldata[lidxs[ikl]:lidxs[ikl + nkl]
-                       ].reshape((-1, ns))[:, gl].flatten()
+                       ].reshape((-1, ns))[:, gl].ravel()
             l_blocks.append((lqs[ikl:ikl + nkl], sh, dt,
                              np.arange(ikl, ikl + nkl, dtype=int)))
         nsshs[iks, 0] = ng
         nsdata[iksz:iksz + ng] = sdata[sidxs[ik]:sidxs[ik + 1]][gl]
         ikr = idxgr[ik]
         while ikr + nkr < nr and rqs[ikr + nkr, 0] == sqs[ik, -1]:
             nkr += 1
@@ -614,15 +614,15 @@
             sh[:, 0] = ng
             rrx = ridxs[ikr:ikr + nkr + 1]
             rrxr = (rrx - ridxs[ikr]) // ns
             dt = np.concatenate(
                 [rdata[irst:ired].reshape((ns, -1))
                     for irst, ired in zip(rrx[:-1], rrx[1:])], axis=1)[gl, :]
             dt = np.concatenate(
-                [dt[:, irst:ired].flatten() for irst, ired in zip(rrxr[:-1], rrxr[1:])])
+                [dt[:, irst:ired].ravel() for irst, ired in zip(rrxr[:-1], rrxr[1:])])
             r_blocks.append((rqs[ikr:ikr + nkr], sh, dt,
                              np.arange(ikr, ikr + nkr, dtype=int)))
         if eigen_values:
             error += sdata[sidxs[ik]:sidxs[ik + 1]][gl_inv].sum()
         else:
             error += (sdata[sidxs[ik]:sidxs[ik + 1]][gl_inv] ** 2).sum()
         selected[ik] = True
```

### Comparing `pyblock3-0.2.6/pyblock3/algebra/ad/mps.py` & `pyblock3-0.2.7/pyblock3/algebra/ad/mps.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,34 +18,48 @@
 #
 
 """
 1D tensor network for MPS/MPO.
 """
 
 import numpy as np
-import jax.numpy as jnp
 from numpy.lib.mixins import NDArrayOperatorsMixin
 import numbers
 from collections import Counter
 from functools import reduce
 
 from ..symmetry import BondInfo, BondFusingInfo
 from ..core import SparseTensor, SubTensor, SliceableTensor, FermionTensor
-from .flat import FlatFermionTensor, FlatSparseTensor, jax_pytree_node
+from .flat import FlatFermionTensor, FlatSparseTensor
 from ..mps import MPSInfo
 from ...symbolic.symbolic import SymbolicSparseTensor
 
+from . import ENABLE_JAX
+
+if ENABLE_JAX:
+    import jax.numpy as jnp
+else:
+    jnp = np
 
 def implements(np_func):
     global _numpy_func_impls
     return lambda f: (_numpy_func_impls.update({np_func: f})
                       if np_func not in _numpy_func_impls else None,
                       _numpy_func_impls[np_func])[1]
 
 
+def jax_pytree_node(cls):
+    if ENABLE_JAX:
+        from jax import tree_util
+        tree_util.register_pytree_node(
+            cls, cls.pytree_flatten, cls.pytree_unflatten)
+    return cls
+
+
+
 _mps_numpy_func_impls = {}
 _numpy_func_impls = _mps_numpy_func_impls
 
 @jax_pytree_node
 class MPS(NDArrayOperatorsMixin):
     """
     Matrix Product State / Matrix Product Operator.
@@ -349,18 +363,23 @@
             if i == 0:
                 left = np.tensordot(
                     a.tensors[i], b.tensors[i], axes=(cidx, cidx))
             else:
                 lbra = np.tensordot(left, a.tensors[i], axes=([0], [0]))
                 left = np.tensordot(lbra, b.tensors[i], axes=(cidx, cidx))
 
+        if ENABLE_JAX:
+            r = left
+        else:
+            r = left if isinstance(left, float) else left.item()
+
         if out is not None:
-            out[()] = left.item()
+            out[()] = r
 
-        return left.item() + a.const * b.const
+        return r + a.const * b.const
 
     def dot(self, b, out=None):
         return np.dot(self, b, out=out)
 
     @staticmethod
     @implements(np.linalg.norm)
     def _norm(x):
@@ -409,16 +428,20 @@
             infos = [t.infos for t in tensors]
             prod_bonds.append(infos[0][0] ^ infos[0][1])
             for tl, tr in zip(infos[1:], infos[:-1]):
                 prod_bonds.append((tl[0] | tr[-2]) ^ (tl[1] | tr[-1]))
             prod_bonds.append(infos[-1][-2] ^ infos[-1][-1])
 
             for i in range(n_sites):
+                old_pattern = getattr(tensors[i], "pattern", None)
                 tensors[i] = tensors[i].fuse(-2, -1, info=prod_bonds[i + 1]
                                              ).fuse(0, 1, info=prod_bonds[i])
+                if old_pattern is not None:
+                    tensors[i].pattern = tensors[i].pattern[:-1] + old_pattern[-1]
+                
 
         r = MPS(tensors=tensors)
 
         # const terms
         if a.const != 0 and b.const == 0:
             r += a.const * b
         elif a.const == 0 and b.const != 0:
@@ -578,26 +601,33 @@
                 tensors[it] = FlatFermionTensor.from_fermion(ts)
             else:
                 tensors[it] = ts.to_flat()
         return MPS(tensors=tensors, const=self.const, opts=self.opts, dq=self.dq)
 
     @staticmethod
     def _from_flat(a):
-        return a.to_flat()
+        return a.from_flat()
 
     def from_flat(self):
         from ..flat import FlatFermionTensor as FF, FlatSparseTensor as FS
         m = self.to_flat()
         tensors = [None] * len(m.tensors)
         for it, ts in enumerate(m.tensors):
             if isinstance(ts, FS):
                 tensors[it] = FlatSparseTensor.from_flat(ts)
             else:
                 tensors[it] = FlatFermionTensor.from_flat(ts)
         return MPS(tensors=tensors, const=self.const, opts=self.opts, dq=self.dq)
+    
+    @staticmethod
+    def _from_core(a):
+        return a.from_core()
+
+    def from_core(self):
+        return MPS(tensors=self.tensors, const=self.const, opts=self.opts, dq=self.dq)
 
     @staticmethod
     def _simplify(a):
         """Reduce virtual bond dimensions for symbolic sparse tensors.
         Only works when tensor is SparseSymbolicTensor."""
         return a.simplify()
```

### Comparing `pyblock3-0.2.6/pyblock3/algebra/core.py` & `pyblock3-0.2.7/pyblock3/algebra/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -383,15 +383,15 @@
         """Ratio of number of non-zero elements to total number of elements."""
         idx = np.indices(self.shape).reshape((self.ndim, -1)).transpose()
         p = np.asarray(self)
         return len([0 for ix in idx if p[tuple(ix)] is not None]) / self.size
 
     @property
     def dtype(self):
-        for v in self.flatten():
+        for v in self.ravel():
             if not isinstance(v, int) or v != 0:
                 return v.dtype
         return float
 
     @staticmethod
     def _to_sparse(a):
         return a.to_sparse()
@@ -713,26 +713,30 @@
         return a.fuse(*idxs, info=info, pattern=pattern)
 
     def fuse(self, *idxs, info=None, pattern=None):
         """Fuse several legs to one leg.
 
         Args:
             idxs : tuple(int)
-                Leg indices to be fused. The new fused index will be idxs[0].
+                Leg indices to be fused. The new fused index will be min(idxs).
             info : BondFusingInfo (optional)
                 Indicating how quantum numbers are collected.
                 If not specified, the direct sum of quantum numbers will be used.
                 This will generate minimal and (often) incomplete fused shape.
             pattern : str (optional)
                 A str of '+'/'-'. Only required when info is not specified.
                 Indicating how quantum numbers are linearly combined.
                 len(pattern) == len(idxs)
         """
         blocks_map = {}
         idxs = [i if i >= 0 else self.ndim + i for i in idxs]
+        if len(idxs) == 0:
+            return self
+        midx = min(idxs)
+        fidxs = [x for x in idxs if x != midx]
         if info is None:
             info = self.kron_sum_info(*idxs, pattern=pattern)
         if pattern is None:
             pattern = info.pattern
         for block in self.blocks:
             qs = block.q_labels
             ns = block.shape
@@ -745,25 +749,87 @@
                 continue
             # fused shape for fused leg
             x = info[q]
             # starting index in fused dim for this block
             k = info.finfo[q][sqs][0]
             # shape in fused dim for this block
             nk = np.multiply.reduce([ns[ix] for ix in idxs])
-            new_qs = tuple(iq if iiq != idxs[0] else q for iiq, iq in enumerate(
-                qs) if iiq not in idxs[1:])
-            new_ns = [ix if iiq != idxs[0] else x for iiq,
-                      ix in enumerate(ns) if iiq not in idxs[1:]]
+            new_qs = tuple(iq if iiq != midx else q for iiq, iq in enumerate(
+                qs) if iiq not in fidxs)
+            new_ns = [ix if iiq != midx else x for iiq,
+                      ix in enumerate(ns) if iiq not in fidxs]
+            new_perm = []
+            for iiq in range(len(ns)):
+                if iiq not in fidxs:
+                    if iiq != midx:
+                        new_perm.append(iiq)
+                    else:
+                        new_perm.extend(idxs)
+            if new_qs not in blocks_map:
+                blocks_map[new_qs] = [tuple(new_ns), new_qs, []]
+            new_ns[midx] = nk
+            blk = np.transpose(block.data, new_perm)
+            blocks_map[new_qs][-1].append((k, nk, blk.reshape(tuple(new_ns))))
+        for k, v in blocks_map.items():
+            vx = []
+            ik = 0
+            ref_idx = None
+            for g in sorted(v[-1]):
+                if g[0] == ik:
+                    ik += g[1]
+                    vx.append(g[2])
+                    ref_idx = len(vx) - 1
+                else:
+                    nns = list(v[0])
+                    nns[midx] = g[0] - ik
+                    vx.append(np.zeros(tuple(nns)))
+                    vx.append(g[2])
+                    ref_idx = len(vx) - 1
+                    ik += g[1] + g[0] - ik
+            if ik != v[0][midx]:
+                nns = list(v[0])
+                nns[midx] = v[0][midx] - ik
+                vx.append(np.zeros(tuple(nns)))
+            if ref_idx is not None and not all([x.__class__ == vx[ref_idx].__class__ for x in vx]):
+                for iv in range(len(vx)):
+                    if vx[iv].__class__ != vx[ref_idx].__class__:
+                        try:
+                            vx[iv] = np.zeros_like(vx[ref_idx], shape=vx[iv].shape)
+                        except:
+                            vx[iv] = np.zeros(vx[iv].shape, like=vx[ref_idx])
+            blocks_map[k] = SubTensor(
+                reduced=np.concatenate(vx, axis=midx), q_labels=v[1])
+        if hasattr(self, 'pattern'):
+            out_pattern = ''.join([self.pattern[x] if x not in idxs else (
+                '' if x != midx else '+') for x in range(self.ndim)])
+            return self.__class__(blocks=list(blocks_map.values()), pattern=out_pattern)
+        else:
+            return self.__class__(blocks=list(blocks_map.values()))
+
+    def symmetry_fuse(self, finfos, symm_map):
+        """
+        Change from higher symmetry to lower symmetry.
+        
+        Args:
+            finfos : list(BondFusingInfo)
+                generated using BondFusingInfo.get_symmetry_fusing_info
+            symm_map : lambda h: l
+                Map from higher symemtry irrep to lower symmetry irrep
+        """
+        blocks_map = {}
+        for block in self.blocks:
+            new_qs = tuple(symm_map(q) for q in block.q_labels)
+            new_ns = tuple(finfos[iq][q] for iq, q in enumerate(new_qs))
             if new_qs not in blocks_map:
                 blocks_map[new_qs] = SubTensor.zeros(
                     tuple(new_ns), q_labels=new_qs, dtype=block.dtype)
-            new_ns[idxs[0]] = nk
-            sl = tuple(slice(None) if ix != idxs[0] else slice(
-                k, k + nk) for ix in range(len(ns)) if ix not in idxs[1:])
-            blocks_map[new_qs][sl] = np.asarray(block).reshape(tuple(new_ns))
+            fidxs = tuple(finfos[iq].finfo[q][qx] for iq, (q, qx)
+                        in enumerate(zip(new_qs, block.q_labels)))
+            sl = tuple(slice(k, k + nk) for k, nk in fidxs)
+            blocks_map[new_qs][sl] += block
         return self.__class__(blocks=list(blocks_map.values()))
 
     @staticmethod
     @implements(np.tensordot)
     def _tensordot(a, b, axes=2):
         """
         Contract two SparseTensor to form a new SparseTensor.
@@ -1862,14 +1928,19 @@
         even = a.even.kron_add(b.even, infos=infos)
         return FermionTensor(odd=odd, even=even)
 
     def kron_add(self, b, infos=None):
         """Direct sum of first and last legs.
         Middle legs are summed."""
         return self._kron_add(self, b, infos=infos)
+    
+    def symmetry_fuse(self, finfos, symm_map):
+        odd = self.odd.symmetry_fuse(finfos, symm_map)
+        even = self.even.symmetry_fuse(finfos, symm_map)
+        return self.__class__(odd=odd, even=even)
 
     def left_canonicalize(self, mode='reduced'):
         """
         Left canonicalization (using QR factorization).
         Left canonicalization needs to collect all left indices for each specific right index.
         So that we will only have one R, but left dim of q is unchanged.
```

### Comparing `pyblock3-0.2.6/pyblock3/algebra/fermion.py` & `pyblock3-0.2.7/pyblock3/algebra/fermion.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,22 +25,24 @@
 import numpy as np
 import string
 import block3.sz as _block3
 from .core import (SparseTensor, SubTensor,
                    _sparse_tensor_numpy_func_impls)
 from .flat import (FlatSparseTensor,
                    _flat_sparse_tensor_numpy_func_impls)
-from .symmetry import BondInfo
+from .symmetry import BondInfo, BondFusingInfo
 from . import fermion_setting as setting
 import time
 
 SVD_SCREENING = setting.SVD_SCREENING
 Q_LABELS_DTYPE = SHAPES_DTYPE = np.uint32
 INDEX_DTYPE = np.uint64
 
+ENABLE_FUSED_IMPLS = False
+
 def get_backend(symmetry):
     """Get the C++ backend for the input symmetry
 
     Parameters
     ----------
     symmetry : str or symmetry class
     """
@@ -1425,14 +1427,25 @@
             out[0].pattern = out_pattern
             out[0].shape=out_shape
         return self.__class__(blocks=blocks, pattern=out_pattern, shape=out_shape)
 
     @staticmethod
     @implements(np.tensordot)
     def _tensordot(a, b, axes=2):
+        if ENABLE_FUSED_IMPLS:
+            r = a.__class__._tensordot_fused(a, b, axes=axes)
+        else:
+            r = a.__class__._tensordot_basic(a, b, axes=axes)
+        if r.ndim == 0:
+            r = r.item()
+        return r
+
+    @staticmethod
+    def _tensordot_basic(a, b, axes=2):
+
         if isinstance(axes, int):
             idxa, idxb = list(range(-axes, 0)), list(range(0, axes))
         else:
             idxa, idxb = axes
         idxa = [x if x >= 0 else a.ndim + x for x in idxa]
         idxb = [x if x >= 0 else b.ndim + x for x in idxb]
 
@@ -1465,19 +1478,131 @@
                     mat = np.tensordot(np.asarray(block_a), np.asarray(
                         block_b), axes=(idxa, idxb)).view(block_a.__class__)
                     if outq not in blocks_map:
                         mat.q_labels = outq
                         blocks_map[outq] = mat * phase
                     else:
                         blocks_map[outq] += mat * phase
-        if len(out_idx_a) == 0 and len(out_idx_b) == 0:
-            return np.asarray(list(blocks_map.values())[0]).item()
+
         return a.__class__(blocks=list(blocks_map.values()), pattern=out_pattern, shape=tuple(out_shape))
 
     @staticmethod
+    def _tensordot_fused(a, b, axes=2):
+
+        if isinstance(axes, int):
+            idxa, idxb = list(range(-axes, 0)), list(range(0, axes))
+        else:
+            idxa, idxb = axes
+        idxa = [i if i >= 0 else a.ndim + i for i in idxa]
+        idxb = [i if i >= 0 else b.ndim + i for i in idxb]
+        a_bond_inds = tuple(idxa)
+        b_bond_inds = tuple(idxb)
+        a_out_inds = tuple(i for i in range(a.ndim) if i not in idxa)
+        b_out_inds = tuple(i for i in range(b.ndim) if i not in idxb)
+        a_out_shape = tuple(a.shape[ix] for ix in a_out_inds)
+        b_out_shape = tuple(b.shape[ix] for ix in b_out_inds)
+
+
+        a_reorder_inds = a_out_inds + a_bond_inds
+        b_reorder_inds = b_bond_inds[::-1] + b_out_inds
+
+        if a_reorder_inds != tuple(range(0, a.ndim)):
+            a = np.transpose(a, axes=a_reorder_inds)
+        if b_reorder_inds != tuple(range(0, b.ndim)):
+            b = np.transpose(b, axes=b_reorder_inds)
+
+        idxa, idxb = list(range(-len(a_bond_inds), 0)), list(range(0, len(b_bond_inds)))[::-1]
+
+        idxa = [i if i >= 0 else a.ndim + i for i in idxa]
+        idxb = [i if i >= 0 else b.ndim + i for i in idxb]
+        a_bond_inds = tuple(idxa)
+        b_bond_inds = tuple(idxb)
+        a_out_inds = tuple(i for i in range(a.ndim) if i not in idxa)
+        b_out_inds = tuple(i for i in range(b.ndim) if i not in idxb)
+
+        a_min_bond = min(a_bond_inds) if len(a_bond_inds) != 0 else -1
+        b_min_bond = min(b_bond_inds) if len(b_bond_inds) != 0 else -1
+        a_out_inds_alt = tuple(i - len([1 for j in a_bond_inds if j != a_min_bond and j < i])
+                               for i in a_out_inds)
+        b_out_inds_alt = tuple(i - len([1 for j in b_bond_inds if j != b_min_bond and j < i])
+                               for i in b_out_inds)
+
+        def get_items(t, idxs):
+            items = []
+            for block in t.blocks:
+                qs = tuple(block.q_labels[i] for i in idxs)
+                shs = tuple(block.shape[i] for i in idxs)
+                items.append((qs, shs))
+            return items
+
+        a_bond_pattern = ''.join([a.pattern[i] for i in a_bond_inds])
+        b_bond_pattern = ''.join([b.pattern[i] for i in b_bond_inds])
+        a_out_pattern = ''.join([a.pattern[i] for i in a_out_inds])
+        b_out_pattern = ''.join([b.pattern[i] for i in b_out_inds])
+
+        if not (len(idxa) == len(a.pattern) and len(idxb) == len(b.pattern) and idxa == idxb and a.pattern == b.pattern):
+            if len(b_bond_pattern) != 0 and all(xx == yy for xx, yy in zip(a_bond_pattern, b_bond_pattern)):
+                b_bond_pattern = ''.join(
+                    ['+' if x == '-' else '-' for x in b_bond_pattern])
+                b_out_pattern = ''.join(
+                    ['+' if x == '-' else '-' for x in b_out_pattern])
+            assert all(xx != yy for xx, yy in zip(
+                a_bond_pattern, b_bond_pattern))
+
+        items = get_items(a, a_bond_inds) + get_items(b, b_bond_inds)
+        bond_fuse_info = BondFusingInfo.kron_sum(items, pattern=a_bond_pattern)
+
+        a_out_fuse_info = a.kron_sum_info(*a_out_inds, pattern=a_out_pattern)
+        b_out_fuse_info = b.kron_sum_info(*b_out_inds, pattern=b_out_pattern)
+
+        af = (
+            a
+            .fuse(*a_bond_inds, info=bond_fuse_info)
+            .fuse(*a_out_inds_alt, info=a_out_fuse_info)
+        )
+        bf = (
+            b
+            .fuse(*b_bond_inds, info=bond_fuse_info)
+            .fuse(*b_out_inds_alt, info=b_out_fuse_info)
+        )
+
+        if len(a_bond_inds) != 0 and len(a_out_inds) != 0:
+            a_ax = [1 if min(a_out_inds) < min(a_bond_inds) else 0]
+        elif len(a_bond_inds) != 0:
+            a_ax = [0]
+        else:
+            a_ax = []
+
+        if len(b_bond_inds) != 0 and len(b_out_inds) != 0:
+            b_ax = [1 if min(b_out_inds) < min(b_bond_inds) else 0]
+        elif len(b_bond_inds) != 0:
+            b_ax = [0]
+        else:
+            b_ax = []
+
+        if len(b_ax) != 0:
+            bf.pattern = bf.pattern[:b_ax[0]] + '-' + bf.pattern[b_ax[0] + 1:]
+
+        zf = a.__class__._tensordot_basic(af, bf, axes=(a_ax, b_ax))
+
+        if len(a_out_inds) != 0 and len(b_out_inds) != 0:
+            zf = zf.unfuse(1, info=b_out_fuse_info)
+            z = zf.unfuse(0, info=a_out_fuse_info)
+        elif len(a_out_inds) != 0:
+            z = zf.unfuse(0, info=a_out_fuse_info)
+        elif len(b_out_inds) != 0:
+            z = zf.unfuse(0, info=b_out_fuse_info)
+        else:
+            z = zf
+        z.pattern = a_out_pattern + b_out_pattern
+        z._shape = a_out_shape + b_out_shape
+
+        return z
+
+    @staticmethod
     @implements(np.transpose)
     def _transpose(a, axes=None):
         if axes is None:
             axes = list(range(a.ndim))[::-1]
         phase = [compute_phase(block.q_labels, axes) for block in a.blocks]
         blocks = [np.transpose(block, axes=axes)*phase[ibk] for ibk, block in enumerate(a.blocks)]
         pattern = "".join([a.pattern[ix] for ix in axes])
@@ -1663,15 +1788,15 @@
         for i in range(n_blocks):
             shapes[i] = spt.blocks[i].shape
             q_labels[i] = list(map(cls.to_flat, spt.blocks[i].q_labels))
         idxs = np.zeros((n_blocks + 1, ), dtype=INDEX_DTYPE)
         idxs[1:] = np.cumsum(shapes.prod(axis=1), dtype=INDEX_DTYPE)
         data = np.zeros((idxs[-1], ), dtype=spt.dtype)
         for i in range(n_blocks):
-            data[idxs[i]:idxs[i + 1]] = spt.blocks[i].flatten()
+            data[idxs[i]:idxs[i + 1]] = spt.blocks[i].ravel()
         return FlatFermionTensor(q_labels, shapes, data, spt.pattern, idxs, symmetry=cls, shape=spt.shape)
 
     @staticmethod
     @implements(np.add)
     def _add(a, b):
         if isinstance(a, numbers.Number):
             data = a + b.data
```

### Comparing `pyblock3-0.2.6/pyblock3/algebra/fermion_encoding.py` & `pyblock3-0.2.7/pyblock3/algebra/fermion_encoding.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/pyblock3/algebra/fermion_large.py` & `pyblock3-0.2.7/pyblock3/algebra/fermion_large.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/pyblock3/algebra/fermion_ops.py` & `pyblock3-0.2.7/pyblock3/algebra/fermion_ops.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/pyblock3/algebra/fermion_setting.py` & `pyblock3-0.2.7/pyblock3/algebra/fermion_setting.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import sys
 from .fermion_symmetry import U11, U1, Z4, Z2, Z22
 
 this = sys.modules[__name__]
 this.SVD_SCREENING = 1e-28
 this.DEFAULT_SYMMETRY = U11
 this.DEFAULT_FLAT = True
+this.DEFAULT_AD = False
 this.DEFAULT_FERMION = True
 this.DEFAULT_LARGE = False
 this.DEFAULT_CUPY = False
 
 symmetry_map = {"U11": U11,
                 "U1": U1,
                 "Z2": Z2,
@@ -29,29 +30,36 @@
 
 def set_fermion(fermion):
     this.DEFAULT_FERMION = fermion
 
 def set_large(large):
     this.DEFAULT_LARGE = large
 
+def set_ad(ad):
+    this.DEFAULT_AD = ad
+
 def set_cupy(cupy):
     this.DEFAULT_CUPY = cupy
 
 def set_options(**kwargs):
     symmetry = kwargs.pop("symmetry", None)
     fermion = kwargs.pop("fermion", None)
     flat = kwargs.pop("flat", None)
+    ad = kwargs.pop("ad", None)
     large = kwargs.pop("large", None)
     cupy = kwargs.pop("cupy", None)
+    assert len(kwargs) == 0
     if symmetry is not None:
         set_symmetry(symmetry)
     if fermion is not None:
         set_fermion(fermion)
     if flat is not None:
         set_flat(flat)
+    if ad is not None:
+        set_ad(ad)
     if large is not None:
         set_large(large)
     if cupy is not None:
         set_cupy(cupy)
 
 def dispatch_settings(**kwargs):
     keys = list(kwargs.keys())
```

### Comparing `pyblock3-0.2.6/pyblock3/algebra/fermion_symmetry.py` & `pyblock3-0.2.7/pyblock3/algebra/fermion_symmetry.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,18 @@
     def __repr__(self):
         return "< U1(%d) >" % (self.n)
 
     @property
     def parity(self):
         return self.n % 2
 
+    @property
+    def is_fermion(self):
+        return self.parity == 1
+
     @classmethod
     def qpn_to_flat(cls, n):
         return (n + 8192) * 131072
 
     @classmethod
     def flat_to_qpn(cls, x):
         return x // 131072 - 8192
@@ -201,14 +205,18 @@
     def __hash__(self):
         return hash((self.n, self.sz))
 
     @property
     def parity(self):
         return self.n % 2
 
+    @property
+    def is_fermion(self):
+        return self.parity == 1
+
     @classmethod
     def flat_to_parity(cls, x):
         return (x // 131072) % 2
 
     @classmethod
     def qpn_to_flat(cls, n, sz):
         return ((n + 8192) * 16384 + (sz + 8192)) * 8
```

### Comparing `pyblock3-0.2.6/pyblock3/algebra/flat.py` & `pyblock3-0.2.7/pyblock3/algebra/flat.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,17 @@
             data = np.zeros_like(adata)
             block3.flat_sparse_tensor.transpose(ashs, adata, aidxs, axes, data)
             return (aqs[:, axes], ashs[:, axes], data, aidxs)
         flat_sparse_transpose = flat_sparse_transpose_impl
 
         def flat_sparse_skeleton_impl(bond_infos, pattern=None, dq=None):
             fdq = dq.to_flat() if dq is not None else SZ(0, 0, 0).to_flat()
+            ref = block3.MapUIntUInt()
+            ref[SZ(0, 0, 0).to_flat()] = 1
+            bond_infos = [ref if x is None else x for x in bond_infos]
             if pattern is None:
                 pattern = "+" * (len(bond_infos) - 1) + "-"
             return block3.flat_sparse_tensor.skeleton(block3.VectorMapUIntUInt(bond_infos), pattern, fdq)
         flat_sparse_skeleton = flat_sparse_skeleton_impl
 
         def flat_sparse_fix_pattern_impl(qs, pattern=None, dq=None):
             fdq = dq.to_flat() if dq is not None else SZ(0, 0, 0).to_flat()
@@ -152,18 +155,18 @@
         return self.q_labels.nbytes + self.shapes.nbytes + self.data.nbytes + self.idxs.nbytes
 
     def item(self):
         if len(self.data) == 0:
             return 0
         return self.data.item()
 
-    def to_sparse(self):
+    def to_sparse(self, qcls=SZ):
         blocks = [None] * self.n_blocks
         for i in range(self.n_blocks):
-            qs = tuple(map(SZ.from_flat, self.q_labels[i]))
+            qs = tuple(map(qcls.from_flat, self.q_labels[i]))
             blocks[i] = SubTensor(
                 self.data[self.idxs[i]:self.idxs[i + 1]].reshape(self.shapes[i]), q_labels=qs)
         return SparseTensor(blocks=blocks)
 
     @staticmethod
     def get_zero():
         zu = np.zeros((0, 0), dtype=np.uint32)
@@ -173,22 +176,23 @@
 
     @staticmethod
     def from_sparse(spt):
         ndim = spt.ndim
         n_blocks = spt.n_blocks
         shapes = np.zeros((n_blocks, ndim), dtype=np.uint32)
         q_labels = np.zeros((n_blocks, ndim), dtype=np.uint32)
+        qcls = spt.blocks[0].q_labels[0].__class__ if n_blocks != 0 and ndim != 0 else SZ
         for i in range(n_blocks):
             shapes[i] = spt.blocks[i].shape
-            q_labels[i] = list(map(SZ.to_flat, spt.blocks[i].q_labels))
+            q_labels[i] = list(map(qcls.to_flat, spt.blocks[i].q_labels))
         idxs = np.zeros((n_blocks + 1, ), dtype=np.uint64)
         idxs[1:] = np.cumsum(shapes.prod(axis=1), dtype=np.uint64)
         data = np.zeros((idxs[-1], ), dtype=spt.dtype)
         for i in range(n_blocks):
-            data[idxs[i]:idxs[i + 1]] = spt.blocks[i].flatten()
+            data[idxs[i]:idxs[i + 1]] = spt.blocks[i].ravel()
         return FlatSparseTensor(q_labels, shapes, data, idxs)
 
     def __str__(self):
         return str(self.to_sparse())
 
     def __repr__(self):
         return repr(self.to_sparse())
@@ -238,16 +242,17 @@
     @staticmethod
     def random(bond_infos, pattern=None, dq=None, dtype=float):
         """Create tensor from tuple of BondInfo with random elements."""
         qs, shs, idxs = flat_sparse_skeleton(bond_infos, pattern, dq)
         if dtype == float:
             data = np.random.random((idxs[-1], ))
         elif dtype == complex or dtype == np.complex128:
-            data = np.random.random(
-                (idxs[-1], )) + np.random.random((idxs[-1], )) * 1j
+            data = np.zeros((idxs[-1], ), dtype=complex)
+            data.real[:] = np.random.random( (idxs[-1], ))
+            data.imag[:] = np.random.random( (idxs[-1], ))
         else:
             return NotImplementedError('dtype %r not supported!' % dtype)
         return FlatSparseTensor(qs, shs, data, idxs)
     
     def fix_pattern(self, pattern=None, dq=None):
         cqs, cdq = flat_sparse_fix_pattern(self.q_labels, pattern, dq)
         return FlatSparseTensor(cqs, self.shapes, self.data, self.idxs), cdq
@@ -292,14 +297,25 @@
         for ib in range(self.n_blocks):
             q = bqs[ib].tobytes()
             if q in blocks_map:
                 ia = blocks_map[q]
                 bdata[bidxs[ib]:bidxs[ib + 1]] = adata[aidxs[ia]:aidxs[ia + 1]]
         return self
 
+    def cast_assign_removed(self, other):
+        """return the removed part of cast_assign."""
+        aqs, adata, aidxs = other.q_labels, other.data, other.idxs
+        blocks_map = {q.tobytes(): iq for iq, q in enumerate(self.q_labels)}
+        cdata = np.zeros_like(adata, dtype=adata.dtype)
+        for ia in range(other.n_blocks):
+            q = aqs[ia].tobytes()
+            if q not in blocks_map:
+                cdata[aidxs[ia]:aidxs[ia + 1]] = adata[aidxs[ia]:aidxs[ia + 1]]
+        return other.__class__(q_labels=aqs, shapes=other.shapes, data=cdata, idxs=aidxs)
+
     def normalize_along_axis(self, axis):
         if axis < 0:
             axis += self.ndim
         normsq = {}
         for ib in range(self.n_blocks):
             q = self.q_labels[ib, axis]
             if q not in normsq:
@@ -690,15 +706,15 @@
             return v.__class__(
                 q_labels=v.q_labels[mask, 0], shapes=shapes,
                 data=np.concatenate([np.diag(v.data[i:j].reshape(sh, sh)) for i, j, sh in zip(v.idxs[:-1][mask], v.idxs[1:][mask], shapes)]))
         elif v.ndim == 1:
             return v.__class__(
                 q_labels=np.repeat(v.q_labels, 2, axis=1),
                 shapes=np.repeat(v.shapes, 2, axis=1),
-                data=np.concatenate([np.diag(v.data[i:j]).flatten() for i, j in zip(v.idxs, v.idxs[1:])]))
+                data=np.concatenate([np.diag(v.data[i:j]).ravel() for i, j in zip(v.idxs, v.idxs[1:])]))
         elif v.n_blocks != 0:
             raise RuntimeError("ndim for np.diag must be 1 or 2.")
         else:
             return v
 
     def diag(self):
         return np.diag(self)
@@ -1000,27 +1016,27 @@
                 d = (a.ndim - 2) // 2
                 idx = range(d + 1, d + d + 1) if d != 1 else d + 1
                 blocks = [odd_b, even_a]
             # vertical
             else:
                 idx = a.ndim - len(idxa)
                 # 1-site op x n-site op
-                idx = range(idx, idx + min(idxb))
+                idx = range(idx, idx + min(idxb)) if len(idxb) != 0 else []
                 blocks = [odd_a, even_a]
         # op x state
         elif isinstance(a, FlatFermionTensor):
             idx = a.ndim - len(idxa)
             even = np.tensordot(a.even, b, (idxa, idxb))
             odd = np.tensordot(a.odd, b, (idxa, idxb))
             # op rotation / op x gauge (right multiply)
             if b.ndim - len(idxb) == 1:
                 def r(): return FlatFermionTensor(odd=odd, even=even)
             else:
                 # 1-site op x n-site state
-                idx = range(idx, idx + min(idxb))
+                idx = range(idx, idx + min(idxb)) if len(idxb) != 0 else []
                 blocks = [odd]
                 def r(): return odd + even
         # state x op
         elif isinstance(b, FlatFermionTensor):
             idx = 0
             even = np.tensordot(a, b.even, (idxa, idxb))
             odd = np.tensordot(a, b.odd, (idxa, idxb))
```

### Comparing `pyblock3-0.2.6/pyblock3/algebra/flat_functor.py` & `pyblock3-0.2.7/pyblock3/algebra/flat_functor.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,14 +55,16 @@
     import block3.sz as block3
 
     def flat_sparse_matmul_init_impl(spt, pattern, dq, symmetric, mpi):
         fdq = dq.to_flat() if dq is not None else SZ(0, 0, 0).to_flat()
         l, r = spt.tensors
         lo, le = l.odd, l.even
         ro, re = r.odd, r.even
+        if (lo.n_blocks == 0 and le.n_blocks == 0) or (ro.n_blocks == 0 and re.n_blocks == 0):
+            raise RuntimeError("Insufficient quantum numbers in initial states!")
         dl, dr, cinfos, vinfos = block3.flat_sparse_tensor.matmul_init(
             lo.q_labels, lo.shapes, le.q_labels, le.shapes, ro.q_labels,
             ro.shapes, re.q_labels, re.shapes)
         if mpi:
             from mpi4py import MPI
             comm = MPI.COMM_WORLD
             for cvw in [cinfos, vinfos]:
```

### Comparing `pyblock3-0.2.6/pyblock3/algebra/funcs.py` & `pyblock3-0.2.7/pyblock3/algebra/funcs.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/pyblock3/algebra/impl/flat.py` & `pyblock3-0.2.7/pyblock3/algebra/impl/flat.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,17 +63,17 @@
                 mat = np.tensordot(mata, matb, axes=(idxa, idxb))
                 outqk = outq.tobytes()
                 if outqk not in blocks_map:
                     blocks_map[outqk] = len(qs)
                     idxs.append(idxs[-1] + mat.size)
                     qs.append(outq)
                     shapes.append(mat.shape)
-                    mats.append(mat.flatten())
+                    mats.append(mat.ravel())
                 else:
-                    mats[blocks_map[outqk]] += mat.flatten()
+                    mats[blocks_map[outqk]] += mat.ravel()
 
     return (np.array(qs, dtype=np.uint32),
             np.array(shapes, dtype=np.uint32),
             np.concatenate(mats) if len(mats) != 0 else np.array(
                 [], dtype=adata.dtype),
             np.array(idxs, dtype=np.uint64))
 
@@ -145,25 +145,25 @@
         for qs in items[q][0]:
             if qs == pqs:
                 continue
             k, sh = linfo.finfo[q][qs]
             nk = np.multiply.reduce(sh)
             qq = np.array([x.to_flat() for x in qs + (q, )], dtype=aqs.dtype)
             sh = np.array(sh + (l.shape[-1], ), dtype=ashs.dtype)
-            l_blocks.append((qq, sh, l[k:k + nk, :].flatten()))
+            l_blocks.append((qq, sh, l[k:k + nk, :].ravel()))
             pqs = qs
         pqs = None
         for qs in items[q][1]:
             if qs == pqs:
                 continue
             k, sh = rinfo.finfo[q][qs]
             nk = np.multiply.reduce(sh)
             qq = np.array([x.to_flat() for x in (q, ) + qs], dtype=aqs.dtype)
             sh = np.array((r.shape[0], ) + sh, dtype=ashs.dtype)
-            r_blocks.append((qq, sh, r[:, k:k + nk].flatten()))
+            r_blocks.append((qq, sh, r[:, k:k + nk].ravel()))
             pqs = qs
     lqs = np.array([xl[0] for xl in l_blocks], dtype=aqs.dtype)
     lshs = np.array([xl[1] for xl in l_blocks], dtype=ashs.dtype)
     ldata = np.concatenate([xl[2] for xl in l_blocks])
     rqs = np.array([xr[0] for xr in r_blocks], dtype=aqs.dtype)
     rshs = np.array([xr[1] for xr in r_blocks], dtype=ashs.dtype)
     rdata = np.concatenate([xr[2] for xr in r_blocks])
@@ -198,25 +198,25 @@
         l_shapes = np.prod(pashs, axis=1)
         mat = np.concatenate([adata[aidxs[ia]:aidxs[ia + 1]].reshape((sh, -1))
                               for sh, ia in zip(l_shapes, v)], axis=0)
         l, s, r = np.linalg.svd(mat, full_matrices=False)
         rqs[ir, :] = qq
         rshs[ir] = r.shape
         ridxs[ir + 1] = ridxs[ir] + r.size
-        rmats[ir] = r.flatten()
+        rmats[ir] = r.ravel()
         sqs[ir, 0] = qq
         sshs[ir, 0] = s.shape[0]
         sidxs[ir + 1] = sidxs[ir] + s.shape[0]
         smats[ir] = s
         ls = np.split(l, list(accumulate(l_shapes[:-1])), axis=0)
         assert len(ls) == len(v)
         lshs[v, -1] = l.shape[-1]
         lidx[ill:ill + len(v)] = v
         for q, ia in zip(ls, v):
-            lmats[ia] = q.flatten()
+            lmats[ia] = q.ravel()
             ill += 1
     assert ill == nblocks_l
     rr = lqs[lidx], lshs[lidx], np.concatenate([lmats[x] for x in lidx]), None, \
         sqs, sshs, np.concatenate(smats), sidxs, \
         rqs, rshs, np.concatenate(rmats), ridxs
     return (rr, lidx) if indexed else r
 
@@ -248,25 +248,25 @@
         r_shapes = np.prod(pashs, axis=1)
         mat = np.concatenate(
             [adata[aidxs[ia]:aidxs[ia + 1]].reshape((-1, sh)) for sh, ia in zip(r_shapes, v)], axis=1)
         l, s, r = np.linalg.svd(mat, full_matrices=False)
         lqs[il, :] = qq
         lshs[il] = l.shape
         lidxs[il + 1] = lidxs[il] + l.size
-        lmats[il] = l.flatten()
+        lmats[il] = l.ravel()
         sqs[il, 0] = qq
         sshs[il, 0] = s.shape[0]
         sidxs[il + 1] = sidxs[il] + s.shape[0]
         smats[il] = s
         rs = np.split(r, list(accumulate(r_shapes[:-1])), axis=1)
         assert len(rs) == len(v)
         rshs[v, 0] = r.shape[0]
         ridx[irr:irr + len(v)] = v
         for q, ia in zip(rs, v):
-            rmats[ia] = q.flatten()
+            rmats[ia] = q.ravel()
             irr += 1
     assert irr == nblocks_r
     rr = lqs, lshs, np.concatenate(lmats), lidxs, \
         sqs, sshs, np.concatenate(smats), sidxs, \
         rqs[ridx], rshs[ridx], np.concatenate([rmats[x] for x in ridx]), None
     return (rr, ridx) if indexed else rr
 
@@ -291,20 +291,20 @@
         l_shapes = np.prod(pashs, axis=1)
         mat = np.concatenate([adata[aidxs[ia]:aidxs[ia + 1]].reshape((sh, -1))
                               for sh, ia in zip(l_shapes, v)], axis=0)
         q, r = np.linalg.qr(mat, mode='reduced')
         rqs[ir, :] = qq
         rshs[ir] = r.shape
         ridxs[ir + 1] = ridxs[ir] + r.size
-        rmats[ir] = r.flatten()
+        rmats[ir] = r.ravel()
         qs = np.split(q, list(accumulate(l_shapes[:-1])), axis=0)
         assert len(qs) == len(v)
         qshs[v, -1] = r.shape[0]
         for q, ia in zip(qs, v):
-            qmats[ia] = q.flatten()
+            qmats[ia] = q.ravel()
     return qqs, qshs, np.concatenate(qmats), None, rqs, rshs, np.concatenate(rmats), ridxs
 
 
 def flat_sparse_right_canonicalize(aqs, ashs, adata, aidxs):
     collected_cols = {}
     for i, q in enumerate(aqs[:, 0]):
         if q not in collected_cols:
@@ -324,20 +324,20 @@
         r_shapes = np.prod(pashs, axis=1)
         mat = np.concatenate(
             [adata[aidxs[ia]:aidxs[ia + 1]].reshape((-1, sh)).T for sh, ia in zip(r_shapes, v)], axis=0)
         q, r = np.linalg.qr(mat, mode='reduced')
         lqs[il, :] = qq
         lshs[il] = r.shape[::-1]
         lidxs[il + 1] = lidxs[il] + r.size
-        lmats[il] = r.T.flatten()
+        lmats[il] = r.T.ravel()
         qs = np.split(q, list(accumulate(r_shapes[:-1])), axis=0)
         assert len(qs) == len(v)
         qshs[v, 0] = r.shape[0]
         for q, ia in zip(qs, v):
-            qmats[ia] = q.T.flatten()
+            qmats[ia] = q.T.ravel()
     return lqs, lshs, np.concatenate(lmats), lidxs, qqs, qshs, np.concatenate(qmats), None
 
 
 def flat_sparse_left_svd_indexed(aqs, ashs, adata, aidxs):
     return flat_sparse_left_svd(aqs, ashs, adata, aidxs, indexed=True)
 
 
@@ -351,15 +351,15 @@
 
 def flat_sparse_right_canonicalize_indexed(aqs, ashs, adata, aidxs):
     return flat_sparse_right_canonicalize(aqs, ashs, adata, aidxs), np.arange(0, aqs.shape[0], dtype=int)
 
 
 def flat_sparse_transpose(aqs, ashs, adata, aidxs, axes):
     data = np.concatenate(
-        [np.transpose(adata[i:j].reshape(sh), axes=axes).flatten()
+        [np.transpose(adata[i:j].reshape(sh), axes=axes).ravel()
          for i, j, sh in zip(aidxs, aidxs[1:], ashs)])
     return (aqs[:, axes], ashs[:, axes], data, aidxs)
 
 
 def flat_sparse_get_infos(aqs, ashs):
     if len(aqs) == 0:
         return ()
@@ -449,15 +449,15 @@
             rdata = blocks_map[zrq][2]
         rsh = rsh.copy()
         rsh[idxs[0]] = nk
         sl = tuple(slice(None) if ix != idxs[0] else slice(
             k, k + nk) for ix in range(len(rq)))
         rdata[sl] = adata[aidxs[ia]:aidxs[ia + 1]].reshape(rsh)
     rqs, rshs, rdata = zip(*blocks_map.values())
-    return np.array(rqs, dtype=np.uint32), np.array(rshs, dtype=np.uint32), np.concatenate([d.flatten() for d in rdata]), None
+    return np.array(rqs, dtype=np.uint32), np.array(rshs, dtype=np.uint32), np.concatenate([d.ravel() for d in rdata]), None
 
 
 def flat_sparse_trans_fusing_info(info):
     import block3.sz as block3
     minfo = block3.MapFusing()
     for k, v in info.items():
         mp = block3.MapVUIntPUV()
@@ -584,15 +584,15 @@
         nkl, nkr = 0, 0
         while ikl + nkl < nl and lqs[ikl + nkl, -1] == sqs[ik, 0]:
             nkl += 1
         if nkl != 0:
             sh = lshs[ikl:ikl + nkl].copy()
             sh[:, -1] = ng
             dt = ldata[lidxs[ikl]:lidxs[ikl + nkl]
-                       ].reshape((-1, ns))[:, gl].flatten()
+                       ].reshape((-1, ns))[:, gl].ravel()
             l_blocks.append((lqs[ikl:ikl + nkl], sh, dt,
                              np.arange(ikl, ikl + nkl, dtype=int)))
         nsshs[iks, 0] = ng
         nsdata[iksz:iksz + ng] = sdata[sidxs[ik]:sidxs[ik + 1]][gl]
         ikr = idxgr[ik]
         while ikr + nkr < nr and rqs[ikr + nkr, 0] == sqs[ik, -1]:
             nkr += 1
@@ -601,15 +601,15 @@
             sh[:, 0] = ng
             rrx = ridxs[ikr:ikr + nkr + 1]
             rrxr = (rrx - ridxs[ikr]) // ns
             dt = np.concatenate(
                 [rdata[irst:ired].reshape((ns, -1))
                     for irst, ired in zip(rrx[:-1], rrx[1:])], axis=1)[gl, :]
             dt = np.concatenate(
-                [dt[:, irst:ired].flatten() for irst, ired in zip(rrxr[:-1], rrxr[1:])])
+                [dt[:, irst:ired].ravel() for irst, ired in zip(rrxr[:-1], rrxr[1:])])
             r_blocks.append((rqs[ikr:ikr + nkr], sh, dt,
                              np.arange(ikr, ikr + nkr, dtype=int)))
         if eigen_values:
             error += sdata[sidxs[ik]:sidxs[ik + 1]][gl_inv].sum()
         else:
             error += (sdata[sidxs[ik]:sidxs[ik + 1]][gl_inv] ** 2).sum()
         selected[ik] = True
```

### Comparing `pyblock3-0.2.6/pyblock3/algebra/integrate.py` & `pyblock3-0.2.7/pyblock3/algebra/integrate.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/pyblock3/algebra/linalg.py` & `pyblock3-0.2.7/pyblock3/algebra/linalg.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,19 +82,19 @@
     return NotImplemented
 
 
 def _olsen_precondition(q, c, ld, diag):
     """Olsen precondition."""
     t = c.copy()
     mask = np.abs(ld - diag) > 1E-12
-    t[mask] = t[mask] / (ld - diag[mask])
+    t[mask] /= ld - diag[mask]
     numerator = np.dot(t.conj(), q)
     denominator = np.dot(c.conj(), t)
     q += (-numerator / denominator) * c
-    q[mask] = q[mask] / (ld - diag[mask])
+    q[mask] /= ld - diag[mask]
 
 
 def _precondition(r, diag):
     """z = r / diag."""
     z = r.copy()
     if diag is not None:
         mask = np.abs(diag) > 1E-12
```

### Comparing `pyblock3-0.2.6/pyblock3/algebra/mpe.py` & `pyblock3-0.2.7/pyblock3/algebra/mpe.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,20 +100,24 @@
         if func not in _me_numpy_func_impls:
             return NotImplemented
         if not all(issubclass(t, self.__class__) for t in types):
             return NotImplemented
         return _me_numpy_func_impls[func](*args, **kwargs)
 
     def _init_identities(self):
-        qbl, qkl, qml = self.bra[0].infos[0], self.ket[0].infos[0], self.mpo[0].infos[0]
-        qbr, qkr, qmr = self.bra[-1].infos[-1], self.ket[-1].infos[-1], self.mpo[-1].infos[-1]
+        qbl = self.bra[0].infos[0] if len(self.bra[0].infos) != 0 else None
+        qkl = self.ket[0].infos[0] if len(self.ket[0].infos) != 0 else None
+        qbr = self.bra[-1].infos[-1] if len(self.bra[-1].infos) != 0 else None
+        qkr = self.ket[-1].infos[-1] if len(self.ket[-1].infos) != 0 else None
+        qml = qbl if self.mpo[0].n_blocks == 0 else self.mpo[0].infos[0]
+        qmr = qbl if self.mpo[-1].n_blocks == 0 else self.mpo[-1].infos[-1]
         l_mpo_id = self.mpo[0].ones(
             bond_infos=(qml, qbl, qkl, qml), pattern="++--")
         r_mpo_id = self.mpo[-1].ones(bond_infos=(qmr,
-                                                 qbr, qkr, qmr), pattern="++--", dq=self.mpo.dq)
+                                                 qbr, qkr, qmr), pattern="+-+-", dq=self.mpo.dq)
         l_bra_id = self.bra[0].ones(bond_infos=(qbl, ))
         r_bra_id = self.bra[-1].ones(bond_infos=(qbl, ))
         l_ket_id = self.ket[0].ones(bond_infos=(qkl, ))
         r_ket_id = self.ket[-1].ones(bond_infos=(qkl, ))
         return l_mpo_id, r_mpo_id, l_bra_id, r_bra_id, l_ket_id, r_ket_id
 
     def _left_canonicalize_site(self, mps, i):
@@ -258,15 +262,15 @@
 
     def _embedded_bra(self):
         """Change bra format for embedding into larger system."""
         return self._embedded_mps(self.bra, self.idents[2], self.idents[3])
 
     def _embedded_ket(self):
         """Change ket format for embedding into larger system."""
-        return self._embedded_mps(self.ket, self.idents[4], self.idents[5])
+        return self._embedded_mps(self.ket, self.idents[4].conj(), self.idents[5].conj())
 
     def _effective(self, l=0, r=2):
         """Get sub-system with sites [l, r)"""
         mpe = self.copy()
         mpe.build_envs(l=l, r=r)
         eff_ket = mpe._effective_ket(l=l, r=r)
         eff_bra = eff_ket if mpe.bra is mpe.ket else mpe._effective_bra(
@@ -370,26 +374,28 @@
     def rk4(self, dt, fast=False, eval_ener=True):
         if fast and self.ket.n_sites == 1 and self.mpo.n_sites == 2:
             from .flat_functor import FlatSparseFunctor
             pattern = '++' + '+' * (self.ket[0].ndim - 4) + '-+'
             fst = FlatSparseFunctor(
                 self.mpo, pattern=pattern, symmetric=False, mpi=self.mpi)
             b = fst.prepare_vector(self.ket[0])
+            brem = fst.cmat.cast_assign_removed(self.ket[0])
+            brem_nrm = np.linalg.norm(brem)
             k1 = dt * (fst @ b)
             k2 = dt * (fst @ (0.5 * k1 + b))
             k3 = dt * (fst @ (0.5 * k2 + b))
             k4 = dt * (fst @ (k3 + b))
             r1 = b + (31.0 / 162) * k1 + (14.0 / 162) * k2 + \
                 (14.0 / 162) * k3 + (-5.0 / 162) * k4
             r2 = b + (16.0 / 81) * k1 + (20.0 / 81) * k2 + \
                 (20.0 / 81) * k3 + (-2.0 / 81) * k4
             r3 = b + k1 / 6 + k2 / 3 + k3 / 3 + k4 / 6
-            g = np.linalg.norm(r3)
+            g = np.sqrt(np.linalg.norm(r3) ** 2 + brem_nrm ** 2)
             w = np.dot(r3.conj(), fst @ r3) / g ** 2 if eval_ener else 0
-            kets = [self.ket.__class__(tensors=[fst.finalize_vector(x)],
+            kets = [self.ket.__class__(tensors=[brem + fst.finalize_vector(x)],
                                        opts=self.ket.opts) for x in [b, r1, r2, r3]]
             nflop = fst.nflop
         else:
             raise NotImplementedError
         mpe = self.copy_shell(bra=kets[0], mpo=self.mpo, ket=kets[0])
         return w, g, kets, mpe, 4 + eval_ener, nflop
```

### Comparing `pyblock3-0.2.6/pyblock3/algebra/mps.py` & `pyblock3-0.2.7/pyblock3/algebra/mps.py`

 * *Files 3% similar despite different names*

```diff
@@ -373,14 +373,19 @@
         assert isinstance(a, MPS) and isinstance(b, MPS)
         assert a.n_sites == b.n_sites
         n_sites = a.n_sites
 
         if n_sites == 1:
             return MPS(tensors=[a[0] + b[0]], const=a.const + b.const, opts=a.opts, dq=a.dq)
 
+        if any([t.n_blocks == 0 for t in a.tensors]):
+            return MPS(tensors=b.tensors, const=a.const + b.const, opts=b.opts, dq=b.dq)
+        elif any([t.n_blocks == 0 for t in b.tensors]):
+            return MPS(tensors=a.tensors, const=a.const + b.const, opts=a.opts, dq=a.dq)
+
         ainfos = [t.infos for t in a.tensors]
         binfos = [t.infos for t in b.tensors]
         sum_bonds = []
         sum_bonds.append(ainfos[0][0])
         for i in range(n_sites - 1):
             x = ainfos[i + 1][0] | ainfos[i][-1]
             y = binfos[i + 1][0] | binfos[i][-1]
@@ -410,41 +415,48 @@
     def copy(self):
         return np.copy(self)
 
     @staticmethod
     @implements(np.dot)
     def _dot(a, b, out=None):
         if isinstance(a, numbers.Number) or isinstance(b, numbers.Number):
-            return np.multiply(a, b, out=out)
+            if isinstance(a, numbers.Number) and a == 0:
+                return 0.0
+            elif isinstance(b, numbers.Number) and b == 0:
+                return 0.0
+            else:
+                return np.multiply(a, b, out=out)
 
         assert isinstance(a, MPS) and isinstance(b, MPS)
         assert a.n_sites == b.n_sites
 
         left = np.array(0)
         for i in range(a.n_sites):
-            assert a.tensors[i].ndim == b.tensors[i].ndim
             if a.tensors[i].n_blocks == 0 or b.tensors[i].n_blocks == 0:
                 return 0
+            assert a.tensors[i].ndim == b.tensors[i].ndim
 
             if i != a.n_sites - 1:
                 cidx = list(range(0, a.tensors[i].ndim - 1))
             else:
                 cidx = list(range(0, a.tensors[i].ndim))
 
             if i == 0:
                 left = np.tensordot(
                     a.tensors[i], b.tensors[i], axes=(cidx, cidx))
             else:
                 lbra = np.tensordot(left, a.tensors[i], axes=([0], [0]))
                 left = np.tensordot(lbra, b.tensors[i], axes=(cidx, cidx))
+        
+        r = left if isinstance(left, float) else left.item()
 
         if out is not None:
-            out[()] = left.item()
+            out[()] = r
 
-        return left.item() + a.const * b.const
+        return r + a.const * b.const
 
     def dot(self, b, out=None):
         return np.dot(self, b, out=out)
 
     @staticmethod
     @implements(np.linalg.norm)
     def _norm(x):
@@ -464,15 +476,15 @@
         assert isinstance(a, MPS) and isinstance(b, MPS)
 
         opts = {**a.opts, **b.opts}
 
         if b.n_sites == 1:
             r = a.tensors[0].__class__.pdot(a.tensors, b.tensors[0])
             ir = r.infos
-            rl = r.ones(bond_infos=(ir[1], ir[0], ir[1]), pattern="-++")
+            rl = r.ones(bond_infos=(ir[1], ir[0], ir[1]), pattern="--+")
             rr = r.ones(bond_infos=(ir[-2], ir[-1], ir[-1]), pattern="++-")
             r = np.tensordot(rl, r, axes=2)
             r = np.tensordot(r, rr, axes=2)
             tensors = [r]
         elif a.n_sites == 1:
             raise NotImplementedError("not implemented yet")
         else:
@@ -482,15 +494,19 @@
             n_sites = a.n_sites
             tensors = [None] * n_sites
 
             if all(ta.ndim == tb.ndim and ta.ndim % 2 == 1 for ta, tb in zip(a.tensors, b.tensors)):
                 return np.dot(a, b, out=out)
 
             for i in range(n_sites):
+                if a.tensors[i].n_blocks == 0 or b.tensors[i].n_blocks == 0:
+                    return 0
                 tensors[i] = a.tensors[i].pdot(b.tensors[i])
+                if tensors[i].n_blocks == 0:
+                    return 0
 
             # merge virtual dims
             prod_bonds = []
             infos = [t.infos for t in tensors]
             prod_bonds.append(infos[0][0] ^ infos[0][1])
             for tl, tr in zip(infos[1:], infos[:-1]):
                 prod_bonds.append((tl[0] | tr[-2]) ^ (tl[1] | tr[-1]))
@@ -541,19 +557,48 @@
 
     def show_bond_dims(self):
         bonds = []
         infos = [t.infos for t in self.tensors]
         infos = [i if len(i) != 0 else (BondInfo(), ) for i in infos]
         bonds.append(infos[0][0])
         for i in range(self.n_sites - 1):
-            bonds.append(infos[i + 1][0] | infos[i][-1])
+            if len(infos[i + 1][0]) == 0:
+                bonds.append(infos[i][-1])
+            elif len(infos[i][-1]) == 0:
+                bonds.append(infos[i + 1][0])
+            else:
+                bonds.append(infos[i + 1][0] | infos[i][-1])
         bonds.append(infos[-1][-1])
         r = '|'.join([str(x.n_bonds) for x in bonds])
         return r if self.const == 0 else r + " (%+12.5f)" % self.const
 
+    def symmetry_fuse(self, symm_map, info=None):
+        infos = [t.infos for t in self.tensors]
+        bonds = []
+        bonds.append(infos[0][0])
+        for i in range(self.n_sites - 1):
+            bonds.append(infos[i + 1][0] | infos[i][-1])
+        bonds.append(infos[-1][-1])
+
+        tensors = [None] * self.n_sites
+        k = 0
+        for i in range(self.n_sites):
+            if info is None:
+                minfos = infos[i][1:self[i].ndim - 1]
+            elif len(info.basis) == self.n_sites:
+                minfos = (info.basis[i], ) * (self[i].ndim - 2)
+            else:
+                minfos = info.basis[k:k + self[i].ndim - 2]
+                k += self[i].ndim - 2
+            sinfos = (bonds[i], *minfos, bonds[i + 1])
+            finfos = [BondFusingInfo.get_symmetry_fusing_info(i, symm_map) for i in sinfos]
+            tensors[i] = self[i].symmetry_fuse(finfos, symm_map)
+        
+        return MPS(tensors=tensors, const=self.const, opts=self.opts, dq=self.dq)
+
     @staticmethod
     def _to_sliceable(a, info=None):
         return a.to_sliceable(info=info)
 
     def to_sliceable(self, info=None):
         """
         Get a shallow copy of MPS with SliceableTensor.
@@ -594,14 +639,30 @@
         tensors = [None] * len(self.tensors)
         for it, ts in enumerate(self.tensors):
             if isinstance(ts, FlatSparseTensor) or isinstance(ts, FlatFermionTensor):
                 tensors[it] = ts
             else:
                 tensors[it] = ts.to_sparse(dq=None if it == 0 else self.dq)
         return MPS(tensors=tensors, const=self.const, opts=self.opts, dq=self.dq)
+    
+    @staticmethod
+    def _to_ad_sparse(a):
+        return a.to_sparse()
+
+    def to_ad_sparse(self):
+        tensors = [None] * len(self.tensors)
+        from .ad.core import FermionTensor as ADFT, SparseTensor as ADST
+        for it, ts in enumerate(self.tensors):
+            if isinstance(ts, SparseTensor):
+                tensors[it] = ADST.from_non_ad(ts, pattern='++-')
+            elif isinstance(ts, FermionTensor):
+                tensors[it] = ADFT.from_non_ad(ts, pattern='++--')
+            else:
+                assert False
+        return MPS(tensors=tensors, const=self.const, opts=self.opts, dq=self.dq)
 
     @staticmethod
     def _to_symbolic(a):
         return a.to_sparse()
 
     def to_symbolic(self):
         tensors = [None] * len(self.tensors)
```

### Comparing `pyblock3-0.2.6/pyblock3/algebra/symmetry.py` & `pyblock3-0.2.7/pyblock3/algebra/symmetry.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,14 +88,18 @@
     def n_bonds(self):
         """Total number of bonds."""
         return sum(self.values())
 
     def item(self):
         assert len(self) == 1 and self[list(self)[0]] == 1
         return list(self)[0]
+    
+    @property
+    def symm_class(self):
+        return list(self)[0].__class__
 
     @staticmethod
     def tensor_product(a, b, ref=None):
         quanta = BondInfo()
         for ka, va in a.items():
             for kb, vb in b.items():
                 if ref is None or ka + kb in ref:
@@ -134,14 +138,25 @@
         n_total = self.n_bonds
         if n_total > bond_dim:
             for k, v in self.items():
                 self[k] = int(np.ceil(v * bond_dim / n_total + 0.1))
                 if ref is not None:
                     self[k] = min(self[k], ref[k])
 
+    def truncate_no_keep(self, bond_dim, ref=None):
+        n_total = self.n_bonds
+        if n_total > bond_dim:
+            for k, v in self.items():
+                self[k] = int(np.round(v * bond_dim / n_total + 0.1))
+                if ref is not None:
+                    self[k] = min(self[k], ref[k])
+            for k in list(self.keys()):
+                if self[k] == 0:
+                    del self[k]
+
     def keep_maximal(self):
         maxk = max(self)
         return BondInfo({maxk: self[maxk]})
 
     def __repr__(self):
         return " ".join(["%r = %d" % (k, v) for k, v in sorted(self.items(), key=lambda x: x[0])])
 
@@ -233,7 +248,29 @@
             for qs, shs in v:
                 if qs not in finfo[q]:
                     finfo[q][qs] = quanta[q], shs
                     quanta[q] += np.prod(shs, dtype=np.uint32)
                 else:
                     assert finfo[q][qs][1] == shs
         return BondFusingInfo(quanta, finfo=finfo, pattern=pattern)
+    
+    @staticmethod
+    def get_symmetry_fusing_info(info, symm_map):
+        """
+        Fusing info for tranfrom to lower symmetry.
+
+        Args:
+            info : BondInfo
+                BondInfo at higher symmetry
+            symm_map : lambda h: l
+                Map from higher symemtry irrep to lower symmetry irrep
+        """
+        quanta = BondInfo()
+        finfo = {}
+        for k, v in sorted(info.items(), key=lambda x: x[0]):
+            q = symm_map(k)
+            if q not in finfo:
+                finfo[q] = {}
+            finfo[q][k] = quanta[q], v
+            quanta[q] += v
+        return BondFusingInfo(quanta, finfo=finfo, pattern='+')
+
```

### Comparing `pyblock3-0.2.6/pyblock3/algebra/tests/test_boson_cpp.py` & `pyblock3-0.2.7/pyblock3/algebra/tests/test_boson_cpp.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/pyblock3/algebra/tests/test_boson_python.py` & `pyblock3-0.2.7/pyblock3/algebra/tests/test_boson_python.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/pyblock3/algebra/tests/test_fermion_cpp.py` & `pyblock3-0.2.7/pyblock3/algebra/tests/test_fermion_cpp.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/pyblock3/algebra/tests/test_fermion_large.py` & `pyblock3-0.2.7/pyblock3/algebra/tests/test_fermion_large.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/pyblock3/algebra/tests/test_fermion_ops.py` & `pyblock3-0.2.7/pyblock3/algebra/tests/test_fermion_ops.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/pyblock3/algebra/tests/test_fermion_python.py` & `pyblock3-0.2.7/pyblock3/algebra/tests/test_fermion_python.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/pyblock3/algebra/tests/test_symmetry.py` & `pyblock3-0.2.7/pyblock3/algebra/tests/test_symmetry.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/pyblock3/algorithms/core.py` & `pyblock3-0.2.7/pyblock3/algorithms/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
                             ex_wfn[0].conj(), ex_wfn[0], axes=((-3, -2, -1), ) * 2).real
                 if isinstance(wfns, list):
                     for ex_wfn, w in zip(wfns, weights):
                         dm = self.add_dm_noise(dm, mpo, ex_wfn, noise * w, forward)
                 else:
                     dm = self.add_dm_noise(dm, mpo, wfn, noise, forward)
                 if not self.mpi or self.mrank == 0:
-                    lsr = dm.tensor_svd(idx=3, pattern='+++---')
+                    lsr = dm.tensor_svd(idx=3, pattern='-++---')
                     l, _, _, error = pbalg.truncate_svd(
                         *lsr, cutoff=self.cutoff, max_bond_dim=bond_dim, eigen_values=True)
                     if isinstance(wfns, list):
                         for xwfn in wfns:
                             xwfn[:] = [l, np.tensordot(l.conj(), xwfn[0], axes=((0, 1, 2), ) * 2)]
                     else:
                         wfn[:] = [l, np.tensordot(l.conj(), wfn[0], axes=((0, 1, 2), ) * 2)]
@@ -135,15 +135,15 @@
                             ex_wfn[0].conj(), ex_wfn[0], axes=((0, 1, 2), ) * 2).real
                 if isinstance(wfns, list):
                      for ex_wfn, w in zip(wfns, weights):
                         dm = self.add_dm_noise(dm, mpo, ex_wfn, noise * w, forward)
                 else:
                     dm = self.add_dm_noise(dm, mpo, wfn, noise, forward)
                 if not self.mpi or self.mrank == 0:
-                    lsr = dm.tensor_svd(idx=3, pattern='-+-+-+')
+                    lsr = dm.tensor_svd(idx=3, pattern='-+-+--')
                     _, _, r, error = pbalg.truncate_svd(
                         *lsr, cutoff=self.cutoff, max_bond_dim=bond_dim, eigen_values=True)
                     if isinstance(wfns, list):
                         for xwfn in wfns:
                             xwfn[:] = [np.tensordot(xwfn[0], r.conj(), axes=((-3, -2, -1), ) * 2), r]
                     else:
                         wfn[:] = [np.tensordot(wfn[0], r.conj(), axes=((-3, -2, -1), ) * 2), r]
```

### Comparing `pyblock3-0.2.6/pyblock3/algorithms/dmrg.py` & `pyblock3-0.2.7/pyblock3/algorithms/dmrg.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/pyblock3/algorithms/green.py` & `pyblock3-0.2.7/pyblock3/algorithms/green.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/pyblock3/algorithms/linear.py` & `pyblock3-0.2.7/pyblock3/algorithms/linear.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/pyblock3/algorithms/tddmrg.py` & `pyblock3-0.2.7/pyblock3/algorithms/tddmrg.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/pyblock3/algorithms/tests/test_dmrg.py` & `pyblock3-0.2.7/pyblock3/algorithms/tests/test_dmrg.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/pyblock3/algorithms/tests/test_ghf.py` & `pyblock3-0.2.7/pyblock3/algorithms/tests/test_ghf.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/pyblock3/algorithms/tests/test_sa.py` & `pyblock3-0.2.7/pyblock3/algorithms/tests/test_sa.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/pyblock3/algorithms/tests/test_soc.py` & `pyblock3-0.2.7/pyblock3/algorithms/tests/test_soc.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/pyblock3/block2/hamil.py` & `pyblock3-0.2.7/pyblock3/block2/hamil.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,15 +151,15 @@
             mh1e = np.zeros((n_sites * (n_sites + 1) // 2))
             k = 0
             for i in range(0, n_sites):
                 for j in range(0, i + 1):
                     assert abs(h1e[i, j] - h1e[j, i]) < tol
                     mh1e[k] = h1e[i, j]
                     k += 1
-            mg2e = g2e.flatten().copy()
+            mg2e = g2e.ravel().copy()
             mh1e[np.abs(mh1e) < tol] = 0.0
             mg2e[np.abs(mg2e) < tol] = 0.0
             fcidump.initialize_su2(n_sites, n_elec, 0, 1, ecore, mh1e, mg2e)
             fcidump.orb_sym = VectorUInt8(orb_sym)
             with HamilTools._from_fcidump(fcidump, pg=pg) as hamil:
                 yield hamil
```

### Comparing `pyblock3-0.2.6/pyblock3/block2/io.py` & `pyblock3-0.2.7/pyblock3/block2/io.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,41 +30,44 @@
 from ..algebra.symmetry import SZ as ASZ
 from ..symbolic.expr import OpElement as AOpElement
 from ..symbolic.symbolic import SymbolicSparseTensor
 from ..symbolic.symbolic import SymbolicMatrix as ASymbolicMatrix
 from ..symbolic.symbolic import SymbolicRowVector as ASymbolicRowVector
 from ..symbolic.symbolic import SymbolicColumnVector as ASymbolicColumnVector
 
-from block2 import OpTypes, QCTypes, SZ, Tensor, Global, init_memory, release_memory
-from block2 import VectorInt, VectorDouble, VectorPIntInt, DoubleVectorAllocator, IntVectorAllocator
+from block2 import OpTypes, QCTypes, SZ, Global, init_memory, release_memory
+from block2 import VectorInt, VectorPIntInt, DoubleVectorAllocator, IntVectorAllocator
 from block2 import OpNames, SiteIndex
-from block2.sz import StateInfo, MPOQC, UnfusedMPS, CG, MPSInfo, VectorStateInfo
-from block2.sz import VectorVectorPSSTensor, VectorPSSTensor, SparseTensor, VectorSpTensor
-from block2.sz import OpElement, MPO, OpExpr, VectorOpExpr, OperatorTensor
+from block2.sz import StateInfo, CG, MPSInfo, VectorStateInfo, OpExpr, VectorOpExpr
 from block2.sz import SymbolicMatrix, SymbolicRowVector, SymbolicColumnVector
-from block2.sz import SparseMatrixInfo, SparseMatrix, TensorFunctions, OperatorFunctions, CG
-from block2.sz import VectorVectorPLMatInfo, VectorPLMatInfo, VectorSymbolic, VectorOpTensor
+from block2.sz import SparseMatrixInfo
+from block2.sz import VectorVectorPLMatInfo, VectorPLMatInfo, VectorSymbolic
 
 class MPSTools:
     @staticmethod
     def from_block2(bmps):
         """Translate block2 MPS to pyblock3 MPS."""
+        from block2.cpx.sz import UnfusedMPS as UMPS_C, MPS as MPS_C
+        if isinstance(bmps, UMPS_C) or isinstance(bmps, MPS_C):
+            import block2.cpx.sz as bx
+        else:
+            import block2.sz as bx
         tensors = [None] * bmps.n_sites
         cf = [c for c in bmps.canonical_form]
         if cf.count('C') + cf.count('K') + cf.count('S') != 1:
-            assert not isinstance(bmps, UnfusedMPS)
+            assert not isinstance(bmps, bx.UnfusedMPS)
             assert cf.count('C') == 2
             ix = cf.index('C')
             assert cf[ix + 1] == 'C'
             bmps.center = ix
             bmps.move_right(CG(), None)
             bmps.save_data()
-        if not isinstance(bmps, UnfusedMPS):
+        if not isinstance(bmps, bx.UnfusedMPS):
             bmps.load_data()
-            bmps = UnfusedMPS(bmps)
+            bmps = bx.UnfusedMPS(bmps)
         for i in range(0, bmps.n_sites):
             spd = bmps.tensors[i].data
             blocks = []
             for im in range(len(spd)):
                 qm = bmps.info.basis[i].quanta[im]
                 for ((ql, qr), ts) in spd[im]:
                     qx = tuple(ASZ(x.n, x.twos, x.pg) for x in (ql, qm, qr))
@@ -101,14 +104,18 @@
                 be saved to the current block2 global scratch folder.
         
         Returns:
             bmps : block2 MPS
                 To inspect this MPS, please make sure that the block2 global
                 scratch folder and stack memory are properly initialized.
         """
+        if mps.dtype == np.float32 or mps.dtype == np.float64 or mps.dtype == float:
+            import block2.sz as bx, block2 as bf
+        else:
+            import block2.cpx.sz as bx, block2.cpx as bf
         frame_back = Global.frame
         inited = False
         if Global.frame is None or save_dir is not None:
             if save_dir is None:
                 save_dir = './nodex'
             init_memory(isize=1 << 20, dsize=1 << 30, save_dir=save_dir)
             inited = True
@@ -154,30 +161,30 @@
                 p.n_states[ix] = v
             p.sort_states()
         minfo.tag = tag
         minfo.save_mutable()
         minfo.save_data("%s/%s-mps_info.bin" % (save_dir, tag))
         tensors = [None] * len(mps)
         for i, b in enumerate(basis):
-            tensors[i] = SparseTensor()
-            tensors[i].data = VectorVectorPSSTensor([VectorPSSTensor() for _ in range(b.n)])
+            tensors[i] = bx.SparseTensor()
+            tensors[i].data = bx.VectorVectorPSSTensor([bx.VectorPSSTensor() for _ in range(b.n)])
             for block in mps[i].blocks:
                 ql, qm, qr = [SZ(x.n, x.twos, x.pg) for x in block.q_labels]
                 im = b.find_state(qm)
                 assert im != -1
-                tensors[i].data[im].append(((ql, qr), Tensor(VectorInt(block.shape))))
-                tensors[i].data[im][-1][1].data = VectorDouble(np.asarray(block).flatten())
-        umps = UnfusedMPS()
+                tensors[i].data[im].append(((ql, qr), bf.Tensor(VectorInt(block.shape))))
+                np.array(tensors[i].data[im][-1][1], copy=False)[:] = block
+        umps = bx.UnfusedMPS()
         umps.info = minfo
         umps.n_sites = len(mps)
         umps.canonical_form = "L" * center + ("S" if center == len(mps) - 1 else "K") + \
             "R" * (len(mps) - center - 1)
         umps.center = center
         umps.dot = 1
-        umps.tensors = VectorSpTensor(tensors)
+        umps.tensors = bx.VectorSpTensor(tensors)
         umps = umps.finalize()
         if inited:
             release_memory()
             Global.frame = frame_back
         return umps
 
 
@@ -191,35 +198,40 @@
             q = expr.q_label
             op.q_label = ASZ(q.n, q.twos, q.pg)
             return op
         else:
             assert False
 
     @staticmethod
-    def tr_expr_to_block2(expr):
+    def tr_expr_to_block2(expr, bx):
         if expr == 0:
             return OpExpr()
         elif isinstance(expr, AOpElement):
             nsi = len(expr.site_index)
             if repr(expr.name) in ["X", "XL", "XR"]:
                 si = SiteIndex(expr.site_index, ())
             else:
                 si = SiteIndex(expr.site_index[:nsi // 2], expr.site_index[nsi // 2:])
             name = getattr(OpNames, repr(expr.name))
             q = expr.q_label
             ql = SZ(q.n, q.twos, q.pg)
-            return OpElement(name, si, ql, expr.factor)
+            return bx.OpElement(name, si, ql, expr.factor)
         else:
             assert False
 
     @staticmethod
     def from_block2(bmpo):
         """Translate block2 (un-simplified) MPO to pyblock2 symbolic MPO."""
+        from block2.cpx.sz import MPO as MPO_C
+        if isinstance(bmpo, MPO_C):
+            import block2.cpx.sz as bx
+        else:
+            import block2.sz as bx
         assert bmpo.schemer is None
-        if isinstance(bmpo, MPOQC):
+        if isinstance(bmpo, bx.MPOQC):
             assert bmpo.mode == QCTypes.NC or bmpo.mode == QCTypes.CN
         tensors = [None] * bmpo.n_sites
         for i in range(0, bmpo.n_sites):
             assert bmpo.tensors[i].lmat == bmpo.tensors[i].rmat
             mat = bmpo.tensors[i].lmat
             ops = bmpo.tensors[i].ops
             lop = bmpo.right_operator_names[i]
@@ -258,17 +270,21 @@
                              for expr in rop.data], dtype=object)
             xlop = ASymbolicColumnVector(n_rows=len(lopd), data=lopd)
             xrop = ASymbolicRowVector(n_cols=len(ropd), data=ropd)
             tensors[i] = SymbolicSparseTensor(xmat, xops, xlop, xrop)
         return MPS(tensors=tensors, const=bmpo.const_e)
 
     @staticmethod
-    def to_block2(mpo):
+    def to_block2(mpo, use_complex=False):
         """Translate pyblock2 symbolic MPO to block2 (un-simplified) MPO."""
-        bmpo = MPO(mpo.n_sites)
+        if not use_complex:
+            import block2.sz as bx
+        else:
+            import block2.cpx.sz as bx
+        bmpo = bx.MPO(mpo.n_sites)
         tensors = [None] * mpo.n_sites
         lops = [None] * mpo.n_sites
         rops = [None] * mpo.n_sites
         site_op_infos = [None] * mpo.n_sites
         site_basis = [None] * mpo.n_sites
         for i in range(0, mpo.n_sites):
             ts = mpo.tensors[i]
@@ -277,94 +293,99 @@
             pinfo = pinfo[0] | pinfo[1]
             site_basis[i] = StateInfo()
             site_basis[i].allocate(len(pinfo))
             for ix, (k, v) in enumerate(pinfo.items()):
                 site_basis[i].quanta[ix] = SZ(k.n, k.twos, k.pg)
                 site_basis[i].n_states[ix] = v
             site_basis[i].sort_states()
-            tensors[i] = OperatorTensor()
+            tensors[i] = bx.OperatorTensor()
             site_op_infos[i] = {}
             dalloc = DoubleVectorAllocator()
             ialloc = IntVectorAllocator()
-            matd = [SymbolicMPOTools.tr_expr_to_block2(expr) for expr in ts.mat.data]
+            matd = [SymbolicMPOTools.tr_expr_to_block2(expr, bx) for expr in ts.mat.data]
             if isinstance(ts.mat, ASymbolicRowVector):
                 tensors[i].lmat = SymbolicRowVector(ts.mat.n_cols)
                 tensors[i].lmat.data = VectorOpExpr(matd)
             elif isinstance(ts.mat, ASymbolicColumnVector):
                 tensors[i].lmat = SymbolicColumnVector(ts.mat.n_rows)
                 tensors[i].lmat.data = VectorOpExpr(matd)
             elif isinstance(ts.mat, ASymbolicMatrix):
                 tensors[i].lmat = SymbolicMatrix(ts.mat.n_rows, ts.mat.n_cols)
                 tensors[i].lmat.data = VectorOpExpr(matd)
                 tensors[i].lmat.indices = VectorPIntInt(ts.mat.indices)
             tensors[i].rmat = tensors[i].lmat
-            zero = SparseMatrix(dalloc)
+            zero = bx.SparseMatrix(dalloc)
             zero.factor = 0
             idq = SZ(0, 0, 0)
-            iop = OpElement(OpNames.I, SiteIndex(), idq, 1.0)
+            iop = bx.OpElement(OpNames.I, SiteIndex(), idq, 1.0)
             for expr, spmat in ts.ops.items():
-                xexpr = SymbolicMPOTools.tr_expr_to_block2(expr)
+                xexpr = SymbolicMPOTools.tr_expr_to_block2(expr, bx)
                 if isinstance(spmat, numbers.Number) or spmat.n_blocks == 0:
                     tensors[i].ops[xexpr] = zero
                     continue
                 assert isinstance(spmat, FermionTensor)
                 assert spmat.odd.n_blocks == 0 or spmat.even.n_blocks == 0
                 spx = spmat.even if spmat.odd.n_blocks == 0 else spmat.odd
                 dq = spx.blocks[0].q_labels[0] - spx.blocks[0].q_labels[1]
                 dq = SZ(dq.n, dq.twos, dq.pg)
                 if dq not in site_op_infos[i]:
                     site_op_infos[i][dq] = SparseMatrixInfo(ialloc)
                     site_op_infos[i][dq].initialize(site_basis[i], site_basis[i],
                         dq, dq.is_fermion)
                 minfo = site_op_infos[i][dq]
-                xmat = SparseMatrix(dalloc)
+                xmat = bx.SparseMatrix(dalloc)
                 xmat.allocate(minfo)
                 for block in spx.blocks:
                     ql, qr = block.q_labels
                     ql, qr = SZ(ql.n, ql.twos, ql.pg), SZ(qr.n, qr.twos, qr.pg)
                     iq = xmat.info.find_state(dq.combine(ql, qr))
-                    xmat[iq] = np.asarray(block).flatten()
+                    xmat[iq] = np.asarray(block).ravel()
                 tensors[i].ops[xexpr] = xmat
             if iop not in tensors[i].ops:
                 if idq not in site_op_infos[i]:
                     site_op_infos[i][idq] = SparseMatrixInfo(ialloc)
                     site_op_infos[i][idq].initialize(site_basis[i], site_basis[i],
                         idq, idq.is_fermion)
                 minfo = site_op_infos[i][idq]
-                xmat = SparseMatrix(dalloc)
+                xmat = bx.SparseMatrix(dalloc)
                 xmat.allocate(minfo)
                 for ix in range(0, minfo.n):
-                    xmat[ix] = np.identity(minfo.n_states_ket[ix]).flatten()
+                    xmat[ix] = np.identity(minfo.n_states_ket[ix]).ravel()
                 tensors[i].ops[iop] = xmat
-            lopd = [SymbolicMPOTools.tr_expr_to_block2(expr) for expr in ts.lop.data]
-            ropd = [SymbolicMPOTools.tr_expr_to_block2(expr) for expr in ts.rop.data]
+            lopd = [SymbolicMPOTools.tr_expr_to_block2(expr, bx) for expr in ts.lop.data]
+            ropd = [SymbolicMPOTools.tr_expr_to_block2(expr, bx) for expr in ts.rop.data]
             lops[i] = SymbolicColumnVector(len(lopd))
             rops[i] = SymbolicRowVector(len(ropd))
             lops[i].data = VectorOpExpr(lopd)
             rops[i].data = VectorOpExpr(ropd)
             site_op_infos[i] = VectorPLMatInfo(
                 sorted([(k, v) for k, v in site_op_infos[i].items()], key=lambda x: x[0]))
         bmpo.const_e = mpo.const
-        bmpo.tf = TensorFunctions(OperatorFunctions(CG()))
+        bmpo.tf = bx.TensorFunctions(bx.OperatorFunctions(CG()))
         bmpo.site_op_infos = VectorVectorPLMatInfo(site_op_infos)
         bmpo.basis = VectorStateInfo(site_basis)
         bmpo.sparse_form = "N" * mpo.n_sites
         bmpo.op = rops[-1][0]
         bmpo.right_operator_names = VectorSymbolic(lops)
         bmpo.left_operator_names = VectorSymbolic(rops)
-        bmpo.tensors = VectorOpTensor(tensors)
+        bmpo.tensors = bx.VectorOpTensor(tensors)
         return bmpo
 
 
 class MPOTools:
     @staticmethod
     def from_block2(bmpo):
         """Translate block2 (un-simplified) MPO to pyblock2 MPO."""
+        from block2.cpx.sz import MPO as MPO_C
+        if isinstance(bmpo, MPO_C):
+            import block2.cpx.sz as bx
+        else:
+            import block2.sz as bx
         assert bmpo.schemer is None
-        if isinstance(bmpo, MPOQC):
+        if isinstance(bmpo, bx.MPOQC):
             assert bmpo.mode == QCTypes.NC or bmpo.mode == QCTypes.CN
         tensors = [None] * bmpo.n_sites
         # translate operator name symbols to quantum labels
         idx_mps, idx_qss, idx_imps = [], [], []
         for i in range(0, bmpo.n_sites - 1):
             lidx_mp = {}
             lidx_qs = [op.q_label for op in bmpo.left_operator_names[i].data]
@@ -401,15 +422,16 @@
                             nu = spmat.info.n_states_bra[p]
                             nd = spmat.info.n_states_ket[p]
                             qx = (SZ(0, 0, 0), qu, qd, qr)
                             map_blocks = map_blocks_odd if (
                                 qu - qd).is_fermion else map_blocks_even
                             if qx not in map_blocks:
                                 map_blocks[qx] = SubTensor(
-                                    q_labels=qx, reduced=np.zeros((1, nu, nd, nr)))
+                                    q_labels=qx, reduced=np.zeros((1, nu, nd, nr),
+                                    dtype=np.array(expr.factor).dtype))
                             map_blocks[qx][0, :, :, ir] += expr.factor * \
                                 spmat.factor * np.array(spmat[p])
                     else:
                         assert False
             elif i == bmpo.n_sites - 1:
                 for k, expr in enumerate(mat.data):
                     if expr.get_type() == OpTypes.Zero:
@@ -428,15 +450,16 @@
                             nu = spmat.info.n_states_bra[p]
                             nd = spmat.info.n_states_ket[p]
                             qx = (ql, qu, qd, SZ(0, 0, 0))
                             map_blocks = map_blocks_odd if (
                                 qu - qd).is_fermion else map_blocks_even
                             if qx not in map_blocks:
                                 map_blocks[qx] = SubTensor(
-                                    q_labels=qx, reduced=np.zeros((nl, nu, nd, 1)))
+                                    q_labels=qx, reduced=np.zeros((nl, nu, nd, 1),
+                                    dtype=np.array(expr.factor).dtype))
                             map_blocks[qx][il, :, :, 0] += expr.factor * \
                                 spmat.factor * np.array(spmat[p])
                     else:
                         assert False
             else:
                 for (j, k), expr in zip(mat.indices, mat.data):
                     if expr.get_type() == OpTypes.Zero:
@@ -458,24 +481,25 @@
                             qx = (ql, qu, qd, qr)
                             map_blocks = map_blocks_odd if (
                                 qu - qd).is_fermion else map_blocks_even
                             if np.linalg.norm(np.array(spmat[p])) == 0:
                                 continue
                             if qx not in map_blocks:
                                 map_blocks[qx] = SubTensor(
-                                    q_labels=qx, reduced=np.zeros((nl, nu, nd, nr)))
+                                    q_labels=qx, reduced=np.zeros((nl, nu, nd, nr),
+                                    dtype=np.array(expr.factor).dtype))
                             map_blocks[qx][il, :, :, ir] += expr.factor * \
                                 spmat.factor * np.array(spmat[p])
                     else:
                         assert False
             tensors[i] = FermionTensor(
                 odd=list(map_blocks_odd.values()), even=list(map_blocks_even.values()))
         for i in range(0, len(tensors)):
             for block in tensors[i].odd.blocks + tensors[i].even.blocks:
                 block.q_labels = tuple(ASZ(x.n, x.twos, x.pg)
                                        for x in block.q_labels)
         return MPS(tensors=tensors, const=bmpo.const_e)
 
     @staticmethod
-    def to_block2(mpo):
+    def to_block2(mpo, use_complex=False):
         """Translate pyblock2 MPO to block2 (un-simplified) MPO."""
-        return SymbolicMPOTools.to_block2(mpo.to_symbolic())
+        return SymbolicMPOTools.to_block2(mpo.to_symbolic(), use_complex=use_complex)
```

### Comparing `pyblock3-0.2.6/pyblock3/fcidump.py` & `pyblock3-0.2.7/pyblock3/fcidump.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/pyblock3/hamiltonian.py` & `pyblock3-0.2.7/pyblock3/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/pyblock3/heisenberg.py` & `pyblock3-0.2.7/pyblock3/heisenberg.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/pyblock3/symbolic/expr.py` & `pyblock3-0.2.7/pyblock3/symbolic/expr.py`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/pyblock3/symbolic/symbolic.py` & `pyblock3-0.2.7/pyblock3/symbolic/symbolic.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     def __setitem__(self, idx, v):
         self.data[idx[0], idx[1]] = v
 
     def get_symbols(self):
         return set([abs(op) for op in self if op != 0])
 
     def __iter__(self):
-        yield from self.data.flatten()
+        yield from self.data.ravel()
 
     def __len__(self):
         return self.data.size
 
     def deflate(self):
         pass
```

### Comparing `pyblock3-0.2.6/pyblock3/symbolic/symbolic_mpo.py` & `pyblock3-0.2.7/pyblock3/symbolic/symbolic_mpo.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     def __init__(self, *args, **kwargs):
         if "hamil" not in kwargs and len(args) == 0:
             super().__init__(**kwargs)
             return
         else:
             hamil = kwargs["hamil"] if len(args) == 0 else args[0]
             symmetrized_p = kwargs.get("symmetrized_p", True)
-            opts = kwargs.get("opts", True)
+            opts = kwargs.get("opts", None)
         n_sites = hamil.n_sites
         vac = SZ(0, 0, 0)
         sz = [1, -1]
 
         tensors = [None] * n_sites
 
         v = hamil.fcidump.v
```

### Comparing `pyblock3-0.2.6/pyblock3.egg-info/PKG-INFO` & `pyblock3-0.2.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: pyblock3
-Version: 0.2.6
-Summary: An efficient python block-sparse tensor and MPS/DMRG library.
-Home-page: https://github.com/block-hczhai/pyblock3-preview
-Author: Huanchen Zhai, Yang Gao, and Garnet K.-L. Chan
-Author-email: hczhai@ucla.edu
-License: LICENSE
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 [![Documentation Status](https://readthedocs.org/projects/pyblock3/badge/?version=latest)](https://pyblock3.readthedocs.io/en/latest/?badge=latest)
 [![Build Status](https://github.com/block-hczhai/pyblock3-preview/workflows/build/badge.svg)](https://github.com/block-hczhai/pyblock3-preview/actions/workflows/build.yml)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![PyPI version](https://badge.fury.io/py/pyblock3.svg)](https://badge.fury.io/py/pyblock3)
 
 pyblock3
@@ -60,14 +49,20 @@
 Installation
 ------------
 
 Using ``pip``:
 
     pip install pyblock3
 
+To install the most recent development version, use:
+
+    pip install pyblock3==<version> --extra-index-url=https://block-hczhai.github.io/pyblock3-preview/pypi/
+
+where ``<version>`` can be some development version number like ``0.2.7rc5``.
+
 Or you can compile it manually:
 
 Dependence: `python3`, `psutil`, `numba`, and `numpy` (version >= 1.17.0). pyblock3 can run in pure python mode,
 in which no C++ source code is required to be compiled.
 
 For optimal performance, the C++ source code is used and there are some additional dependences:
```

### Comparing `pyblock3-0.2.6/pyblock3.egg-info/SOURCES.txt` & `pyblock3-0.2.7/pyblock3.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 pyblock3.egg-info/PKG-INFO
 pyblock3.egg-info/SOURCES.txt
 pyblock3.egg-info/dependency_links.txt
 pyblock3.egg-info/requires.txt
 pyblock3.egg-info/top_level.txt
 pyblock3/algebra/__init__.py
 pyblock3/algebra/core.py
+pyblock3/algebra/einsum.py
 pyblock3/algebra/fermion.py
 pyblock3/algebra/fermion_encoding.py
 pyblock3/algebra/fermion_large.py
 pyblock3/algebra/fermion_ops.py
 pyblock3/algebra/fermion_setting.py
 pyblock3/algebra/fermion_symmetry.py
 pyblock3/algebra/flat.py
@@ -25,14 +26,17 @@
 pyblock3/algebra/funcs.py
 pyblock3/algebra/integrate.py
 pyblock3/algebra/linalg.py
 pyblock3/algebra/mpe.py
 pyblock3/algebra/mps.py
 pyblock3/algebra/symmetry.py
 pyblock3/algebra/ad/__init__.py
+pyblock3/algebra/ad/core.py
+pyblock3/algebra/ad/fermion.py
+pyblock3/algebra/ad/fermion_ops.py
 pyblock3/algebra/ad/flat.py
 pyblock3/algebra/ad/flat_impl.py
 pyblock3/algebra/ad/mps.py
 pyblock3/algebra/impl/__init__.py
 pyblock3/algebra/impl/flat.py
 pyblock3/algebra/tests/__init__.py
 pyblock3/algebra/tests/test_boson_cpp.py
@@ -52,14 +56,16 @@
 pyblock3/algorithms/tests/test_dmrg.py
 pyblock3/algorithms/tests/test_ghf.py
 pyblock3/algorithms/tests/test_sa.py
 pyblock3/algorithms/tests/test_soc.py
 pyblock3/block2/__init__.py
 pyblock3/block2/hamil.py
 pyblock3/block2/io.py
+pyblock3/gaussian/__init__.py
+pyblock3/gaussian/core.py
 pyblock3/symbolic/__init__.py
 pyblock3/symbolic/expr.py
 pyblock3/symbolic/symbolic.py
 pyblock3/symbolic/symbolic_mpo.py
 src/bond_info.cpp
 src/bond_info.hpp
 src/bond_info_tmpl.hpp
```

### Comparing `pyblock3-0.2.6/setup.py` & `pyblock3-0.2.7/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import os
 import sys
 import subprocess
 import platform
 from setuptools import setup, find_packages, Extension
 from setuptools.command.build_ext import build_ext
 
+NO_COMPILE = os.environ.get("PYBLOCK3_NO_COMPILE", None) == "1"
+
 
 class CMakeExt(Extension):
     def __init__(self, name, cmdir='.'):
         Extension.__init__(self, name, [])
         self.cmake_lists_dir = os.path.abspath(cmdir)
 
 
@@ -35,15 +37,15 @@
             cmake_args = [
                 '-DCMAKE_BUILD_TYPE=%s' % cfg,
                 '-DCMAKE_LIBRARY_OUTPUT_DIRECTORY_{}={}'.format(
                     cfg.upper(), extdir),
                 '-DCMAKE_ARCHIVE_OUTPUT_DIRECTORY_{}={}'.format(
                     cfg.upper(), self.build_temp),
                 '-DPYTHON_EXECUTABLE_HINT={}'.format(sys.executable),
-                '-DUSE_MKL=ON'
+                '-DUSE_MKL=ON',
             ]
 
             # We can handle some platform-specific settings at our discretion
             if platform.system() == 'Windows':
                 plat = ('x64' if platform.architecture()
                         [0] == '64bit' else 'Win32')
                 cmake_args += [
@@ -66,29 +68,37 @@
             subprocess.check_call(['cmake', ext.cmake_lists_dir] + cmake_args,
                                   cwd=self.build_temp)
 
             subprocess.check_call(['cmake', '--build', '.', '--config', cfg, '--', '--jobs=4'],
                                   cwd=self.build_temp)
 
 
-setup(name='pyblock3',
-      version='0.2.6',
-      packages=find_packages(),
-      ext_modules=[CMakeExt('block3')],
-      cmdclass={'build_ext': CMakeBuild},
-      license='LICENSE',
-      description='An efficient python block-sparse tensor and MPS/DMRG library.',
-      long_description=open('README.md').read(),
-      long_description_content_type='text/markdown',
-      author='Huanchen Zhai, Yang Gao, and Garnet K.-L. Chan',
-      author_email='hczhai@ucla.edu',
-      url='https://github.com/block-hczhai/pyblock3-preview',
-      install_requires=[
-          "mkl==2019",
-          "mkl-include",
-          "numpy<1.23.0",
-          "psutil",
-          "pybind11",
-          "intel-openmp",
-          "cmake==3.17"
-      ]
-      )
+setup_options = dict(
+    name='pyblock3',
+    version='0.2.7',
+    packages=find_packages(),
+    license='LICENSE',
+    description='An efficient python block-sparse tensor and MPS/DMRG library.',
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
+    author='Huanchen Zhai, Yang Gao, and Garnet K.-L. Chan',
+    author_email='hczhai@ucla.edu',
+    url='https://github.com/block-hczhai/pyblock3-preview',
+    install_requires=["numpy"],
+)
+
+if not NO_COMPILE:
+    setup_options.update(dict(
+        ext_modules=[CMakeExt('block3')],
+        cmdclass={'build_ext': CMakeBuild},
+        install_requires=[
+            "mkl==2021.4",
+            "mkl-include",
+            "numpy<1.23.0",
+            "psutil",
+            "pybind11<=2.10.1",
+            "intel-openmp",
+            "cmake"
+        ]
+    ))
+
+setup(**setup_options)
```

### Comparing `pyblock3-0.2.6/src/bond_info.cpp` & `pyblock3-0.2.7/src/bond_info.cpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/src/bond_info.hpp` & `pyblock3-0.2.7/src/bond_info.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/src/bond_info_tmpl.hpp` & `pyblock3-0.2.7/src/bond_info_tmpl.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/src/fermion_symmetry.hpp` & `pyblock3-0.2.7/src/fermion_symmetry.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/src/flat_fermion.cpp` & `pyblock3-0.2.7/src/flat_fermion.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -132,16 +132,16 @@
     unordered_map<uint64_t, uint8_t> computed;
     for (int ia = 0; ia < n_blocks_a; ia++) {
         uint64_t par_pat = 0;
         for (int j = 0; j < ndima; j++)
             par_pat |= (uint64_t)Q::to_q(apqs[ia * asi + j * asj]).parity()
                        << j;
         if (!computed.count(par_pat))
-            computed[par_pat] = compute_phase(perma, ndima, par_pat,
-                                              &rev_idx[0], &fperm[0]);
+            computed[par_pat] =
+                compute_phase(perma, ndima, par_pat, &rev_idx[0], &fperm[0]);
         phase_a[ia] = 1 - (computed.at(par_pat) << 1);
     }
 
 #else
     // old impl
 
     for (int ia = 0; ia < n_blocks_a; ia++) {
@@ -316,33 +316,34 @@
         ctrqbs[i] = q_labels_hash(psh + i * bsi, nctr, pidxb, bsj);
         outqbs[i] = q_labels_hash(psh + i * bsi, ndimb - nctr, outb, bsj);
     }
 
 #ifdef _USE_NEW_PHASE
 
     assert(ndima <= 64 && ndimb <= 64);
-    vector<int32_t> rev_idx(max(ndima, ndimb) + 1), fperm(max(ndima, ndimb) + 1);
+    vector<int32_t> rev_idx(max(ndima, ndimb) + 1),
+        fperm(max(ndima, ndimb) + 1);
     unordered_map<uint64_t, uint8_t> computed_a, computed_b;
     for (int i = 0; i < n_blocks_a; i++) {
         uint64_t par_pat = 0;
         for (int j = 0; j < ndima; j++)
             par_pat |= (uint64_t)Q::to_q(apqs[i * asi + j * asj]).parity() << j;
         if (!computed_a.count(par_pat))
             computed_a[par_pat] = compute_phase2(ppidxa, ndima, nctr, par_pat,
-                                                &rev_idx[0], &fperm[0]);
+                                                 &rev_idx[0], &fperm[0]);
         phase_a[i] = 1 - (computed_a.at(par_pat) << 1);
     }
 
     for (int i = 0; i < n_blocks_b; i++) {
         uint64_t par_pat = 0;
         for (int j = 0; j < ndimb; j++)
             par_pat |= (uint64_t)Q::to_q(bpqs[i * bsi + j * bsj]).parity() << j;
         if (!computed_b.count(par_pat))
             computed_b[par_pat] = compute_phase3(ppidxb, ndimb, nctr, par_pat,
-                                                &rev_idx[0], &fperm[0]);
+                                                 &rev_idx[0], &fperm[0]);
         phase_b[i] = 1 - (computed_b.at(par_pat) << 1);
     }
 
 #else
 
     for (int i = 0; i < n_blocks_a; i++) {
         int pnuma[ndima];
@@ -445,16 +446,18 @@
             }
         }
     }
 
     vector<ssize_t> sh = {n_blocks_c, ndimc};
     py::array_t<uint32_t> cqs(sh), cshs(sh);
     py::array_t<uint64_t> cidxs(vector<ssize_t>{n_blocks_c + 1});
-    assert(cqs.strides()[1] == sizeof(uint32_t));
-    assert(cshs.strides()[1] == sizeof(uint32_t));
+    if (n_blocks_c != 0 && ndimc != 0) {
+        assert(cqs.strides()[1] == sizeof(uint32_t));
+        assert(cshs.strides()[1] == sizeof(uint32_t));
+    }
     py::array_t<FL> cdata(vector<ssize_t>{csize});
     uint32_t *pcqs = cqs.mutable_data(), *pcshs = cshs.mutable_data();
     uint64_t *pcidxs = cidxs.mutable_data();
     vector<uint32_t> psha(n_blocks_a * ndima), pshb(n_blocks_b * ndimb);
     for (int i = 0; i < n_blocks_a; i++)
         for (int j = 0; j < ndima; j++)
             psha[i * ndima + j] = ashs.data()[i * asi + j * asj];
```

### Comparing `pyblock3-0.2.6/src/flat_fermion.hpp` & `pyblock3-0.2.7/src/flat_fermion.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/src/flat_fermion_tmpl.hpp` & `pyblock3-0.2.7/src/flat_fermion_tmpl.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/src/flat_functor.cpp` & `pyblock3-0.2.7/src/flat_functor.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -98,16 +98,18 @@
         csize += (ssize_t)a_free_dim[ia] * a_ctr_dim[ia] * b_free_dim[ia];
         n_blocks_c++;
     }
 
     vector<ssize_t> sh = {n_blocks_c, ndimc};
     py::array_t<uint32_t> cqs(sh), cshs(sh);
     py::array_t<uint64_t> cidxs(vector<ssize_t>{n_blocks_c + 1});
-    assert(cqs.strides()[1] == sizeof(uint32_t));
-    assert(cshs.strides()[1] == sizeof(uint32_t));
+    if (n_blocks_c != 0 && ndimc != 0) {
+        assert(cqs.strides()[1] == sizeof(uint32_t));
+        assert(cshs.strides()[1] == sizeof(uint32_t));
+    }
     py::array_t<FL> cdata(vector<ssize_t>{csize});
     uint32_t *pcqs = cqs.mutable_data(), *pcshs = cshs.mutable_data();
     uint64_t *pcidxs = cidxs.mutable_data();
     FL *pc = cdata.mutable_data();
     const FL *pa = adata.data();
     const uint64_t *pia = aidxs.data();
     pcidxs[0] = 0;
@@ -141,15 +143,16 @@
 
 template <typename Q, typename FL>
 size_t flat_sparse_tensor_matmul(const py::array_t<int32_t> &plan,
                                  const py::array_t<FL> &adata,
                                  const py::array_t<FL> &bdata,
                                  py::array_t<FL> &cdata) {
     int nb = (int)plan.shape()[0], ndimp = (int)plan.shape()[1];
-    assert(plan.strides()[1] == sizeof(int32_t));
+    if (nb != 0)
+        assert(plan.strides()[1] == sizeof(int32_t));
     assert(ndimp == 12);
     const FL *pa = adata.data(), *pb = bdata.data();
     FL *pc = cdata.mutable_data();
     size_t nflop = 0;
     const CBLAS_LAYOUT layout = CblasRowMajor;
     vector<CBLAS_TRANSPOSE> ta(nb), tb(nb);
     vector<int> n(nb), m(nb), k(nb), gp(nb, 1), lda(nb), ldb(nb), ldc(nb);
@@ -376,16 +379,18 @@
             }
         }
     }
 
     vector<ssize_t> sh = {n_blocks_c, ndimc};
     py::array_t<uint32_t> cqs(sh), cshs(sh);
     py::array_t<uint64_t> cidxs(vector<ssize_t>{n_blocks_c + 1});
-    assert(cqs.strides()[1] == sizeof(uint32_t));
-    assert(cshs.strides()[1] == sizeof(uint32_t));
+    if (n_blocks_c != 0 && ndimc != 0) {
+        assert(cqs.strides()[1] == sizeof(uint32_t));
+        assert(cshs.strides()[1] == sizeof(uint32_t));
+    }
     uint32_t *pcqs = cqs.mutable_data(), *pcshs = cshs.mutable_data();
     uint64_t *pcidxs = cidxs.mutable_data();
     vector<uint32_t> psha(n_blocks_a * ndima), pshb(n_blocks_b * ndimb);
     for (int i = 0; i < n_blocks_a; i++)
         for (int j = 0; j < ndima; j++)
             psha[i * ndima + j] = ashs.data()[i * asi + j * asj];
     for (int i = 0; i < n_blocks_b; i++)
@@ -603,15 +608,16 @@
     }
     if (r.size() == 0)
         return py::array_t<int32_t>(vector<ssize_t>{0, 12});
     assert(r.size() != 0);
     ssize_t rz = (ssize_t)r[0].size();
     vector<ssize_t> sh = {(ssize_t)r.size(), rz};
     py::array_t<int32_t> ar(sh);
-    assert(ar.strides()[1] == sizeof(int32_t));
+    if (r.size() != 0 && rz != 0)
+        assert(ar.strides()[1] == sizeof(int32_t));
     for (size_t i = 0; i < r.size(); i++)
         memcpy(ar.mutable_data() + i * rz, r[i].data(), sizeof(int32_t) * rz);
 
     return ar;
 }
 
 #define TMPL_NAME flat_functor
```

### Comparing `pyblock3-0.2.6/src/flat_functor.hpp` & `pyblock3-0.2.7/src/flat_functor.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/src/flat_functor_tmpl.hpp` & `pyblock3-0.2.7/src/flat_functor_tmpl.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/src/flat_sparse.cpp` & `pyblock3-0.2.7/src/flat_sparse.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -235,16 +235,18 @@
             }
         }
     }
 
     vector<ssize_t> sh = {n_blocks_c, ndimc};
     py::array_t<uint32_t> cqs(sh), cshs(sh);
     py::array_t<uint64_t> cidxs(vector<ssize_t>{n_blocks_c + 1});
-    assert(cqs.strides()[1] == sizeof(uint32_t));
-    assert(cshs.strides()[1] == sizeof(uint32_t));
+    if (n_blocks_c != 0 && ndimc != 0) {
+        assert(cqs.strides()[1] == sizeof(uint32_t));
+        assert(cshs.strides()[1] == sizeof(uint32_t));
+    }
     py::array_t<FL> cdata(vector<ssize_t>{csize});
     uint32_t *pcqs = cqs.mutable_data(), *pcshs = cshs.mutable_data();
     uint64_t *pcidxs = cidxs.mutable_data();
     vector<uint32_t> psha(n_blocks_a * ndima), pshb(n_blocks_b * ndimb);
     for (int i = 0; i < n_blocks_a; i++)
         for (int j = 0; j < ndima; j++)
             psha[i * ndima + j] = ashs.data()[i * asi + j * asj];
@@ -424,16 +426,18 @@
 
     add_blocks(n_blocks_a, n_blocks_b, ndima, aqs.data(), bqs.data(), pia, pib,
                asi, asj, bsi, bsj, map_idx, iab_mp.data(), n_blocks_c, csize);
 
     vector<ssize_t> sh = {n_blocks_c, ndima};
     py::array_t<uint32_t> cqs(sh), cshs(sh);
     py::array_t<uint64_t> cidxs(vector<ssize_t>{n_blocks_c + 1});
-    assert(cqs.strides()[1] == sizeof(uint32_t));
-    assert(cshs.strides()[1] == sizeof(uint32_t));
+    if (n_blocks_c != 0 && ndima != 0) {
+        assert(cqs.strides()[1] == sizeof(uint32_t));
+        assert(cshs.strides()[1] == sizeof(uint32_t));
+    }
     uint32_t *pcqs = cqs.mutable_data(), *pcshs = cshs.mutable_data();
     uint64_t *pcidxs = cidxs.mutable_data();
     int ic = 0;
     pcidxs[0] = 0;
     vector<int> pic(n_blocks_a + n_blocks_b);
     for (auto &p : map_idx) {
         for (int iab : p.second) {
@@ -514,16 +518,18 @@
 
     add_blocks(n_blocks_a, n_blocks_b, ndima, aqs.data(), bqs.data(), pia, pib,
                asi, asj, bsi, bsj, map_idx, iab_mp.data(), n_blocks_c, csize);
 
     vector<ssize_t> sh = {n_blocks_c, ndima};
     py::array_t<uint32_t> cqs(sh), cshs(sh);
     py::array_t<uint64_t> cidxs(vector<ssize_t>{n_blocks_c + 1});
-    assert(cqs.strides()[1] == sizeof(uint32_t));
-    assert(cshs.strides()[1] == sizeof(uint32_t));
+    if (n_blocks_c != 0 && ndima != 0) {
+        assert(cqs.strides()[1] == sizeof(uint32_t));
+        assert(cshs.strides()[1] == sizeof(uint32_t));
+    }
     uint32_t *pcqs = cqs.mutable_data(), *pcshs = cshs.mutable_data();
     uint64_t *pcidxs = cidxs.mutable_data();
     int ic = 0;
     pcidxs[0] = 0;
     vector<int> pic(n_blocks_a + n_blocks_b);
     vector<uint32_t> dimlc(n_blocks_c), dimla(n_blocks_a), dimlb(n_blocks_b);
     for (int i = 0; i < n_blocks_a; i++) {
@@ -653,16 +659,18 @@
             n_blocks_c++;
         }
     }
 
     vector<ssize_t> sh = {n_blocks_c, ndimc};
     py::array_t<uint32_t> cqs(sh), cshs(sh);
     py::array_t<uint64_t> cidxs(vector<ssize_t>{n_blocks_c + 1});
-    assert(cqs.strides()[1] == sizeof(uint32_t));
-    assert(cshs.strides()[1] == sizeof(uint32_t));
+    if (n_blocks_c != 0 && ndimc != 0) {
+        assert(cqs.strides()[1] == sizeof(uint32_t));
+        assert(cshs.strides()[1] == sizeof(uint32_t));
+    }
     py::array_t<FL> cdata(vector<ssize_t>{csize});
     uint32_t *pcqs = cqs.mutable_data(), *pcshs = cshs.mutable_data();
     uint64_t *pcidxs = cidxs.mutable_data();
 
     pcidxs[0] = 0;
     const FL *pa = adata.data();
     FL *pc = cdata.mutable_data();
@@ -818,16 +826,18 @@
             shs.insert(shs.end(), shk.begin(), shk.end());
             idxs.push_back(idxs.back() + sz);
         }
     }
     vector<ssize_t> sh = {(ssize_t)qs.size() / ndim, ndim};
     py::array_t<uint32_t> cqs(sh), cshs(sh);
     py::array_t<uint64_t> cidxs(vector<ssize_t>{(ssize_t)idxs.size()});
-    assert(cqs.strides()[1] == sizeof(uint32_t));
-    assert(cshs.strides()[1] == sizeof(uint32_t));
+    if (qs.size() != 0) {
+        assert(cqs.strides()[1] == sizeof(uint32_t));
+        assert(cshs.strides()[1] == sizeof(uint32_t));
+    }
     memcpy(cqs.mutable_data(), qs.data(), qs.size() * sizeof(uint32_t));
     memcpy(cshs.mutable_data(), shs.data(), shs.size() * sizeof(uint32_t));
     memcpy(cidxs.mutable_data(), idxs.data(), idxs.size() * sizeof(uint64_t));
     return std::make_tuple(cqs, cshs, cidxs);
 }
 
 template <typename Q>
@@ -1024,22 +1034,25 @@
                      : std::make_tuple(lrqs, lrshs, lrdata, lridxs, qqs, qshs,
                                        qdata, qidxs);
 }
 
 template <typename Q, typename FL, DIRECTION L>
 tuple<py::array_t<uint32_t>, py::array_t<uint32_t>, py::array_t<FL>,
       py::array_t<uint64_t>, py::array_t<uint32_t>, py::array_t<uint32_t>,
-      py::array_t<typename GFP<FL>::FP>, py::array_t<uint64_t>, py::array_t<uint32_t>,
-      py::array_t<uint32_t>, py::array_t<FL>, py::array_t<uint64_t>>
+      py::array_t<typename GFP<FL>::FP>, py::array_t<uint64_t>,
+      py::array_t<uint32_t>, py::array_t<uint32_t>, py::array_t<FL>,
+      py::array_t<uint64_t>>
 flat_sparse_svd(const py::array_t<uint32_t> &aqs,
                 const py::array_t<uint32_t> &ashs, const py::array_t<FL> &adata,
                 const py::array_t<uint64_t> &aidxs, uint32_t *pxidx) {
     if (aqs.shape()[0] == 0)
-        return std::make_tuple(aqs, ashs, adata, aidxs, aqs, ashs, adata, aidxs,
-                               aqs, ashs, adata, aidxs);
+        return std::make_tuple(
+            aqs, ashs, adata, aidxs, aqs, ashs,
+            py::array_t<typename GFP<FL>::FP>(vector<ssize_t>{(ssize_t)0}),
+            aidxs, aqs, ashs, adata, aidxs);
     int n_blocks_a = (int)aqs.shape()[0], ndima = (int)aqs.shape()[1];
     const int cidx = L == LEFT ? ndima - 1 : 0;
     const ssize_t asi = aqs.strides()[0] / sizeof(uint32_t),
                   asj = aqs.strides()[1] / sizeof(uint32_t);
     assert(memcmp(aqs.strides(), ashs.strides(), 2 * sizeof(ssize_t)) == 0);
 
     unordered_map<uint32_t, vector<int>> collected;
@@ -1071,15 +1084,16 @@
     collect_blocks<L>(collected, asi, asj, n_blocks_a, ndima, cidx, paqs, pashs,
                       max_mshape, max_lshape, max_rshape, max_tmp_size, pqqs,
                       pqshs, pqidxs, plrqs, plrshs, plridxs, psqs, psshs,
                       psidxs, pxidx);
 
     py::array_t<FL> qdata(vector<ssize_t>{(ssize_t)pqidxs[n_blocks_a]});
     py::array_t<FL> lrdata(vector<ssize_t>{(ssize_t)plridxs[n_blocks_lr]});
-    py::array_t<typename GFP<FL>::FP> sdata(vector<ssize_t>{(ssize_t)psidxs[n_blocks_lr]});
+    py::array_t<typename GFP<FL>::FP> sdata(
+        vector<ssize_t>{(ssize_t)psidxs[n_blocks_lr]});
     FL *pq = qdata.mutable_data(), *plr = lrdata.mutable_data();
     typename GFP<FL>::FP *ps = sdata.mutable_data();
     memset(plr, 0, sizeof(FL) * plridxs[n_blocks_lr]);
     int iq = 0, ilr = 0;
     int lwork = max(max_lshape, max_rshape) * 34, info = 0;
     vector<FL> work(lwork), tmp(max_tmp_size),
         tmp2(L == LEFT ? 0 : max_tmp_size);
@@ -1159,28 +1173,30 @@
     return flat_sparse_canonicalize<Q, FL, RIGHT>(aqs, ashs, adata, aidxs,
                                                   nullptr);
 }
 
 template <typename Q, typename FL>
 tuple<py::array_t<uint32_t>, py::array_t<uint32_t>, py::array_t<FL>,
       py::array_t<uint64_t>, py::array_t<uint32_t>, py::array_t<uint32_t>,
-      py::array_t<typename GFP<FL>::FP>, py::array_t<uint64_t>, py::array_t<uint32_t>,
-      py::array_t<uint32_t>, py::array_t<FL>, py::array_t<uint64_t>>
+      py::array_t<typename GFP<FL>::FP>, py::array_t<uint64_t>,
+      py::array_t<uint32_t>, py::array_t<uint32_t>, py::array_t<FL>,
+      py::array_t<uint64_t>>
 flat_sparse_left_svd(const py::array_t<uint32_t> &aqs,
                      const py::array_t<uint32_t> &ashs,
                      const py::array_t<FL> &adata,
                      const py::array_t<uint64_t> &aidxs) {
     return flat_sparse_svd<Q, FL, LEFT>(aqs, ashs, adata, aidxs, nullptr);
 }
 
 template <typename Q, typename FL>
 tuple<py::array_t<uint32_t>, py::array_t<uint32_t>, py::array_t<FL>,
       py::array_t<uint64_t>, py::array_t<uint32_t>, py::array_t<uint32_t>,
-      py::array_t<typename GFP<FL>::FP>, py::array_t<uint64_t>, py::array_t<uint32_t>,
-      py::array_t<uint32_t>, py::array_t<FL>, py::array_t<uint64_t>>
+      py::array_t<typename GFP<FL>::FP>, py::array_t<uint64_t>,
+      py::array_t<uint32_t>, py::array_t<uint32_t>, py::array_t<FL>,
+      py::array_t<uint64_t>>
 flat_sparse_right_svd(const py::array_t<uint32_t> &aqs,
                       const py::array_t<uint32_t> &ashs,
                       const py::array_t<FL> &adata,
                       const py::array_t<uint64_t> &aidxs) {
     return flat_sparse_svd<Q, FL, RIGHT>(aqs, ashs, adata, aidxs, nullptr);
 }
 
@@ -1213,57 +1229,62 @@
         aqs, ashs, adata, aidxs, xidx.mutable_data());
     return make_pair(r, xidx);
 }
 
 template <typename Q, typename FL>
 pair<tuple<py::array_t<uint32_t>, py::array_t<uint32_t>, py::array_t<FL>,
            py::array_t<uint64_t>, py::array_t<uint32_t>, py::array_t<uint32_t>,
-           py::array_t<typename GFP<FL>::FP>, py::array_t<uint64_t>, py::array_t<uint32_t>,
-           py::array_t<uint32_t>, py::array_t<FL>, py::array_t<uint64_t>>,
+           py::array_t<typename GFP<FL>::FP>, py::array_t<uint64_t>,
+           py::array_t<uint32_t>, py::array_t<uint32_t>, py::array_t<FL>,
+           py::array_t<uint64_t>>,
      py::array_t<uint32_t>>
 flat_sparse_left_svd_indexed(const py::array_t<uint32_t> &aqs,
                              const py::array_t<uint32_t> &ashs,
                              const py::array_t<FL> &adata,
                              const py::array_t<uint64_t> &aidxs) {
     py::array_t<uint32_t> xidx(vector<ssize_t>{aqs.shape()[0]});
     const auto &r = flat_sparse_svd<Q, FL, LEFT>(aqs, ashs, adata, aidxs,
                                                  xidx.mutable_data());
     return make_pair(r, xidx);
 }
 
 template <typename Q, typename FL>
 pair<tuple<py::array_t<uint32_t>, py::array_t<uint32_t>, py::array_t<FL>,
            py::array_t<uint64_t>, py::array_t<uint32_t>, py::array_t<uint32_t>,
-           py::array_t<typename GFP<FL>::FP>, py::array_t<uint64_t>, py::array_t<uint32_t>,
-           py::array_t<uint32_t>, py::array_t<FL>, py::array_t<uint64_t>>,
+           py::array_t<typename GFP<FL>::FP>, py::array_t<uint64_t>,
+           py::array_t<uint32_t>, py::array_t<uint32_t>, py::array_t<FL>,
+           py::array_t<uint64_t>>,
      py::array_t<uint32_t>>
 flat_sparse_right_svd_indexed(const py::array_t<uint32_t> &aqs,
                               const py::array_t<uint32_t> &ashs,
                               const py::array_t<FL> &adata,
                               const py::array_t<uint64_t> &aidxs) {
     py::array_t<uint32_t> xidx(vector<ssize_t>{aqs.shape()[0]});
     const auto &r = flat_sparse_svd<Q, FL, RIGHT>(aqs, ashs, adata, aidxs,
                                                   xidx.mutable_data());
     return make_pair(r, xidx);
 }
 
 template <typename Q, typename FL>
 tuple<py::array_t<uint32_t>, py::array_t<uint32_t>, py::array_t<FL>,
       py::array_t<uint64_t>, py::array_t<uint32_t>, py::array_t<uint32_t>,
-      py::array_t<typename GFP<FL>::FP>, py::array_t<uint64_t>, py::array_t<uint32_t>,
-      py::array_t<uint32_t>, py::array_t<FL>, py::array_t<uint64_t>>
+      py::array_t<typename GFP<FL>::FP>, py::array_t<uint64_t>,
+      py::array_t<uint32_t>, py::array_t<uint32_t>, py::array_t<FL>,
+      py::array_t<uint64_t>>
 flat_sparse_tensor_svd(const py::array_t<uint32_t> &aqs,
                        const py::array_t<uint32_t> &ashs,
                        const py::array_t<FL> &adata,
                        const py::array_t<uint64_t> &aidxs, int idx,
                        const map_fusing &linfo, const map_fusing &rinfo,
                        const string &pattern) {
     if (aqs.shape()[0] == 0)
-        return std::make_tuple(aqs, ashs, adata, aidxs, aqs, ashs, adata, aidxs,
-                               aqs, ashs, adata, aidxs);
+        return std::make_tuple(
+            aqs, ashs, adata, aidxs, aqs, ashs,
+            py::array_t<typename GFP<FL>::FP>(vector<ssize_t>{(ssize_t)0}),
+            aidxs, aqs, ashs, adata, aidxs);
     const int n_blocks_a = (int)aqs.shape()[0], ndima = (int)aqs.shape()[1];
     const ssize_t asi = aqs.strides()[0] / sizeof(uint32_t),
                   asj = aqs.strides()[1] / sizeof(uint32_t);
     assert(memcmp(aqs.strides(), ashs.strides(), 2 * sizeof(ssize_t)) == 0);
     vector<vector<uint32_t>> ufqsl(n_blocks_a), ufqsr(n_blocks_a);
     vector<uint32_t> fqs(n_blocks_a);
     unordered_map<uint32_t, size_t> mat_mp;
@@ -1435,25 +1456,27 @@
     return std::make_tuple(lqs, lshs, ldata, lidxs, sqs, sshs, sdata, sidxs,
                            rqs, rshs, rdata, ridxs);
 }
 
 template <typename Q, typename FL>
 tuple<py::array_t<uint32_t>, py::array_t<uint32_t>, py::array_t<FL>,
       py::array_t<uint64_t>, py::array_t<uint32_t>, py::array_t<uint32_t>,
-      py::array_t<typename GFP<FL>::FP>, py::array_t<uint64_t>, py::array_t<uint32_t>,
-      py::array_t<uint32_t>, py::array_t<FL>, py::array_t<uint64_t>, typename GFP<FL>::FP>
+      py::array_t<typename GFP<FL>::FP>, py::array_t<uint64_t>,
+      py::array_t<uint32_t>, py::array_t<uint32_t>, py::array_t<FL>,
+      py::array_t<uint64_t>, typename GFP<FL>::FP>
 flat_sparse_truncate_svd(
     const py::array_t<uint32_t> &lqs, const py::array_t<uint32_t> &lshs,
     const py::array_t<FL> &ldata, const py::array_t<uint64_t> &lidxs,
     const py::array_t<uint32_t> &sqs, const py::array_t<uint32_t> &sshs,
-    const py::array_t<typename GFP<FL>::FP> &sdata, const py::array_t<uint64_t> &sidxs,
-    const py::array_t<uint32_t> &rqs, const py::array_t<uint32_t> &rshs,
-    const py::array_t<FL> &rdata, const py::array_t<uint64_t> &ridxs,
-    int max_bond_dim, typename GFP<FL>::FP cutoff, typename GFP<FL>::FP max_dw, typename GFP<FL>::FP norm_cutoff,
-    bool eigen_values) {
+    const py::array_t<typename GFP<FL>::FP> &sdata,
+    const py::array_t<uint64_t> &sidxs, const py::array_t<uint32_t> &rqs,
+    const py::array_t<uint32_t> &rshs, const py::array_t<FL> &rdata,
+    const py::array_t<uint64_t> &ridxs, int max_bond_dim,
+    typename GFP<FL>::FP cutoff, typename GFP<FL>::FP max_dw,
+    typename GFP<FL>::FP norm_cutoff, bool eigen_values) {
     if (sqs.shape()[0] == 0)
         return std::make_tuple(lqs, lshs, ldata, lidxs, sqs, sshs, sdata, sidxs,
                                sqs, sshs, sdata, sidxs, 0.0);
     int n_blocks_l = (int)lqs.shape()[0], ndiml = (int)lqs.shape()[1];
     int n_blocks_s = (int)sqs.shape()[0], ndims = (int)sqs.shape()[1];
     int n_blocks_r = (int)rqs.shape()[0], ndimr = (int)rqs.shape()[1];
 
@@ -1475,26 +1498,26 @@
                   rsj = rqs.strides()[1] / sizeof(uint32_t);
     assert(memcmp(lqs.strides(), lshs.strides(), 2 * sizeof(ssize_t)) == 0);
     assert(memcmp(sqs.strides(), sshs.strides(), 2 * sizeof(ssize_t)) == 0);
     assert(memcmp(rqs.strides(), rshs.strides(), 2 * sizeof(ssize_t)) == 0);
     for (int i = 0; i < n_blocks_s; i++)
         for (int j = pis[i]; j < pis[i + 1]; j++)
             ss.push_back(std::make_tuple(i, j, ps[j]));
-    sort(
-        ss.begin(), ss.end(),
-        [](const tuple<int, int, typename GFP<FL>::FP> &a, const tuple<int, int, typename GFP<FL>::FP> &b) {
-            return get<2>(a) > get<2>(b);
-        });
+    sort(ss.begin(), ss.end(),
+         [](const tuple<int, int, typename GFP<FL>::FP> &a,
+            const tuple<int, int, typename GFP<FL>::FP> &b) {
+             return get<2>(a) > get<2>(b);
+         });
     vector<tuple<int, int, typename GFP<FL>::FP>> ss_trunc = ss;
     if (max_dw != 0) {
         int p = 0;
         for (int i = (int)ss_trunc.size(); i > 0; i--) {
-            typename GFP<FL>::FP dw = eigen_values
-                            ? get<2>(ss_trunc[i])
-                            : get<2>(ss_trunc[i]) * get<2>(ss_trunc[i]);
+            typename GFP<FL>::FP dw =
+                eigen_values ? get<2>(ss_trunc[i])
+                             : get<2>(ss_trunc[i]) * get<2>(ss_trunc[i]);
             if (dw <= max_dw)
                 p++;
             else
                 break;
         }
         ss_trunc.resize(ss_trunc.size() - p);
     }
@@ -1505,19 +1528,19 @@
             if (get<2>(ss_trunc[i]) < cutoff) {
                 ss_trunc.resize(i);
                 break;
             }
     }
     if (max_bond_dim != -1 && (int)ss_trunc.size() > max_bond_dim)
         ss_trunc.resize(max_bond_dim);
-    sort(
-        ss_trunc.begin(), ss_trunc.end(),
-        [](const tuple<int, int, typename GFP<FL>::FP> &a, const tuple<int, int, typename GFP<FL>::FP> &b) {
-            return get<1>(a) < get<1>(b);
-        });
+    sort(ss_trunc.begin(), ss_trunc.end(),
+         [](const tuple<int, int, typename GFP<FL>::FP> &a,
+            const tuple<int, int, typename GFP<FL>::FP> &b) {
+             return get<1>(a) < get<1>(b);
+         });
 
     vector<pair<int, vector<int>>> selected;
     selected.reserve(n_blocks_s);
     for (auto &x : ss_trunc)
         if (selected.size() != 0 && selected.back().first == get<0>(x))
             selected.back().second.push_back(get<1>(x));
         else
```

### Comparing `pyblock3-0.2.6/src/flat_sparse.hpp` & `pyblock3-0.2.7/src/flat_sparse.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/src/flat_sparse_tmpl.hpp` & `pyblock3-0.2.7/src/flat_sparse_tmpl.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/src/gpu/flat_fermion.hpp` & `pyblock3-0.2.7/src/gpu/flat_fermion.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/src/gpu/flat_fermion_tmpl.hpp` & `pyblock3-0.2.7/src/gpu/flat_fermion_tmpl.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/src/hamiltonian.cpp` & `pyblock3-0.2.7/src/hamiltonian.cpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/src/hamiltonian.hpp` & `pyblock3-0.2.7/src/hamiltonian.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/src/hamiltonian_ptree.cpp` & `pyblock3-0.2.7/src/hamiltonian_ptree.cpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/src/hamiltonian_ptree.hpp` & `pyblock3-0.2.7/src/hamiltonian_ptree.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/src/main.cpp` & `pyblock3-0.2.7/src/main.cpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/src/max_flow.hpp` & `pyblock3-0.2.7/src/max_flow.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/src/qc_expr.hpp` & `pyblock3-0.2.7/src/qc_expr.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/src/qc_hamiltonian.cpp` & `pyblock3-0.2.7/src/qc_hamiltonian.cpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/src/qc_hamiltonian.hpp` & `pyblock3-0.2.7/src/qc_hamiltonian.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/src/qc_mpo.hpp` & `pyblock3-0.2.7/src/qc_mpo.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/src/qc_symbolic.hpp` & `pyblock3-0.2.7/src/qc_symbolic.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/src/symmetry_tmpl.hpp` & `pyblock3-0.2.7/src/symmetry_tmpl.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/src/sz.hpp` & `pyblock3-0.2.7/src/sz.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/src/tensor.cpp` & `pyblock3-0.2.7/src/tensor.cpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/src/tensor.hpp` & `pyblock3-0.2.7/src/tensor.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/src/tensor_einsum.cpp` & `pyblock3-0.2.7/src/tensor_einsum.cpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/src/tensor_einsum.hpp` & `pyblock3-0.2.7/src/tensor_einsum.hpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/src/tensor_impl.cpp` & `pyblock3-0.2.7/src/tensor_impl.cpp`

 * *Files identical despite different names*

### Comparing `pyblock3-0.2.6/src/tensor_impl.hpp` & `pyblock3-0.2.7/src/tensor_impl.hpp`

 * *Files identical despite different names*

