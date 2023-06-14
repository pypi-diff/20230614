# Comparing `tmp/substrafl-0.37.0rc1.tar.gz` & `tmp/substrafl-0.37.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "substrafl-0.37.0rc1.tar", last modified: Tue Jun 13 15:16:46 2023, max compression
+gzip compressed data, was "substrafl-0.37.0rc2.tar", last modified: Wed Jun 14 15:52:22 2023, max compression
```

## Comparing `substrafl-0.37.0rc1.tar` & `substrafl-0.37.0rc2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:16:46.180891 substrafl-0.37.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-13 15:16:46.180891 substrafl-0.37.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 15:16:46.180891 substrafl-0.37.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:16:46.176890 substrafl-0.37.0rc1/substrafl/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:16:46.176890 substrafl-0.37.0rc1/substrafl/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/algorithms/algo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:16:46.176890 substrafl-0.37.0rc1/substrafl/algorithms/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/algorithms/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15452 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/algorithms/pytorch/torch_base_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/algorithms/pytorch/torch_fed_avg_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/algorithms/pytorch/torch_fed_pca_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    18129 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/algorithms/pytorch/torch_newton_raphson_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    23454 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/algorithms/pytorch/torch_scaffold_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/algorithms/pytorch/torch_single_organization_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/algorithms/pytorch/weight_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/compute_plan_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:16:46.176890 substrafl-0.37.0rc1/substrafl/dependency/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/dependency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/dependency/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/dependency/path_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/dependency/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/evaluation_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14812 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:16:46.176890 substrafl-0.37.0rc1/substrafl/index_generator/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/index_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/index_generator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/index_generator/np_index_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    18170 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/model_loading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:16:46.176890 substrafl-0.37.0rc1/substrafl/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/nodes/aggregation_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/nodes/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:16:46.180891 substrafl-0.37.0rc1/substrafl/nodes/references/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/nodes/references/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/nodes/references/local_state.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/nodes/references/shared_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/nodes/test_data_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    13179 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/nodes/train_data_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:16:46.180891 substrafl-0.37.0rc1/substrafl/remote/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/remote/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/remote/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:16:46.180891 substrafl-0.37.0rc1/substrafl/remote/register/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/remote/register/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/remote/register/manage_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)    15539 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/remote/register/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/remote/remote_struct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:16:46.180891 substrafl-0.37.0rc1/substrafl/remote/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/remote/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/remote/serializers/pickle_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/remote/serializers/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/remote/substratools_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:16:46.180891 substrafl-0.37.0rc1/substrafl/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12026 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/strategies/fed_avg.py
--rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/strategies/fed_pca.py
--rw-r--r--   0 runner    (1001) docker     (123)    15033 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/strategies/newton_raphson.py
--rw-r--r--   0 runner    (1001) docker     (123)    17740 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/strategies/scaffold.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/strategies/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     6823 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/strategies/single_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/strategies/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:16:46.176890 substrafl-0.37.0rc1/substrafl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-13 15:16:45.000000 substrafl-0.37.0rc1/substrafl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-13 15:16:46.000000 substrafl-0.37.0rc1/substrafl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 15:16:45.000000 substrafl-0.37.0rc1/substrafl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-13 15:16:45.000000 substrafl-0.37.0rc1/substrafl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-13 15:16:45.000000 substrafl-0.37.0rc1/substrafl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:52:21.998115 substrafl-0.37.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-14 15:52:21.998115 substrafl-0.37.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 15:52:21.998115 substrafl-0.37.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:52:21.990115 substrafl-0.37.0rc2/substrafl/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:52:21.990115 substrafl-0.37.0rc2/substrafl/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/algorithms/algo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:52:21.994115 substrafl-0.37.0rc2/substrafl/algorithms/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/algorithms/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15452 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/algorithms/pytorch/torch_base_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/algorithms/pytorch/torch_fed_avg_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/algorithms/pytorch/torch_fed_pca_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18129 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/algorithms/pytorch/torch_newton_raphson_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23454 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/algorithms/pytorch/torch_scaffold_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/algorithms/pytorch/torch_single_organization_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/algorithms/pytorch/weight_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/compute_plan_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:52:21.994115 substrafl-0.37.0rc2/substrafl/dependency/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/dependency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/dependency/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/dependency/path_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/dependency/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/evaluation_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14754 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:52:21.994115 substrafl-0.37.0rc2/substrafl/index_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/index_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/index_generator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/index_generator/np_index_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18170 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/model_loading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:52:21.994115 substrafl-0.37.0rc2/substrafl/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/nodes/aggregation_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/nodes/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:52:21.994115 substrafl-0.37.0rc2/substrafl/nodes/references/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/nodes/references/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/nodes/references/local_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/nodes/references/shared_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/nodes/test_data_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13179 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/nodes/train_data_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:52:21.998115 substrafl-0.37.0rc2/substrafl/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/remote/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/remote/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:52:21.998115 substrafl-0.37.0rc2/substrafl/remote/register/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/remote/register/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/remote/register/generate_wheel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/remote/register/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/remote/remote_struct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:52:21.998115 substrafl-0.37.0rc2/substrafl/remote/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/remote/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/remote/serializers/pickle_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/remote/serializers/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/remote/substratools_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:52:21.998115 substrafl-0.37.0rc2/substrafl/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12026 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/strategies/fed_avg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/strategies/fed_pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15033 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/strategies/newton_raphson.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17740 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/strategies/scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/strategies/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6823 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/strategies/single_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-06-14 15:52:18.000000 substrafl-0.37.0rc2/substrafl/strategies/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:52:21.990115 substrafl-0.37.0rc2/substrafl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-14 15:52:21.000000 substrafl-0.37.0rc2/substrafl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-14 15:52:21.000000 substrafl-0.37.0rc2/substrafl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 15:52:21.000000 substrafl-0.37.0rc2/substrafl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-14 15:52:21.000000 substrafl-0.37.0rc2/substrafl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-14 15:52:21.000000 substrafl-0.37.0rc2/substrafl.egg-info/top_level.txt
```

### Comparing `substrafl-0.37.0rc1/LICENSE` & `substrafl-0.37.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/PKG-INFO` & `substrafl-0.37.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrafl
-Version: 0.37.0rc1
+Version: 0.37.0rc2
 Summary: A high-level federated learning Python library to run      federated learning experiments at scale on a Substra network
 Home-page: https://docs.substra.org/
 Author: Owkin, Inc.
 License: Apache 2.0
 Description: readme
 Keywords: substrafl
 Platform: UNKNOWN
```

### Comparing `substrafl-0.37.0rc1/README.md` & `substrafl-0.37.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/pyproject.toml` & `substrafl-0.37.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/setup.py` & `substrafl-0.37.0rc2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,14 @@
         "substra~=0.45.0rc1",
         "substratools~=0.20.0",
         "pydantic>=1.9.0",
         "pip>=21.2",
         "wheel",
         "six",
         "packaging",
-        "pip-tools",
     ],
     extras_require={
         "dev": [
             "pytest>=6.2.4",
             "pytest-cov>=2.12.0",
             "pytest-mock",
             "pre-commit>=2.13.0",
```

### Comparing `substrafl-0.37.0rc1/substrafl/__init__.py` & `substrafl-0.37.0rc2/substrafl/__init__.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/substrafl/algorithms/algo.py` & `substrafl-0.37.0rc2/substrafl/algorithms/algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/substrafl/algorithms/pytorch/__init__.py` & `substrafl-0.37.0rc2/substrafl/algorithms/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/substrafl/algorithms/pytorch/torch_base_algo.py` & `substrafl-0.37.0rc2/substrafl/algorithms/pytorch/torch_base_algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/substrafl/algorithms/pytorch/torch_fed_avg_algo.py` & `substrafl-0.37.0rc2/substrafl/algorithms/pytorch/torch_fed_avg_algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/substrafl/algorithms/pytorch/torch_fed_pca_algo.py` & `substrafl-0.37.0rc2/substrafl/algorithms/pytorch/torch_fed_pca_algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/substrafl/algorithms/pytorch/torch_newton_raphson_algo.py` & `substrafl-0.37.0rc2/substrafl/algorithms/pytorch/torch_newton_raphson_algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/substrafl/algorithms/pytorch/torch_scaffold_algo.py` & `substrafl-0.37.0rc2/substrafl/algorithms/pytorch/torch_scaffold_algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/substrafl/algorithms/pytorch/torch_single_organization_algo.py` & `substrafl-0.37.0rc2/substrafl/algorithms/pytorch/torch_single_organization_algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/substrafl/algorithms/pytorch/weight_manager.py` & `substrafl-0.37.0rc2/substrafl/algorithms/pytorch/weight_manager.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/substrafl/compute_plan_builder.py` & `substrafl-0.37.0rc2/substrafl/compute_plan_builder.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/substrafl/dependency/constants.py` & `substrafl-0.37.0rc2/substrafl/dependency/constants.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/substrafl/dependency/path_management.py` & `substrafl-0.37.0rc2/substrafl/dependency/path_management.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/substrafl/dependency/schemas.py` & `substrafl-0.37.0rc2/substrafl/dependency/schemas.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,19 +17,18 @@
         **local-worker** or with **tmp_substrafl** as prefix are ignored during the installation.
 
     Args:
         editable_mode (bool): If set to False, substra, substrafl and substratools used in the
             Dockerfiles submitted to Substra platform will be taken from pypi.
             If set to True, it will be the one installed in editable mode from your python environment.
             Defaults to False.
-        pypi_dependencies (List[str]): Python packages installable from PyPI.
-        local_installable_dependencies (List[pathlib.Path]): Local installable packages.
-            Each one can either be a wheel or a local folder. If it's a local folder, the command
-            `python -m pip wheel .` will be run, so each folder needs to be a valid Python module (containing a valid
-            `setup.py` or `pyproject.toml`). See the documentation of pip wheel for more details.
+        dependencies (List[str]): Python packages installable from pypi.
+        local_dependencies (List[pathlib.Path]): Local installable packages. The command
+            `pip install -e .` will be executed in each of those folders hence a `setup.py` must be present in each
+            folder.
         local_code (List[pathlib.Path]): Local relative imports used by your script. All files / folders will be
             pasted to the level of the running script.
         excluded_paths (List[pathlib.Path]): Local paths excluded from `local_dependencies` / `local_code`.
             Default to [].
         excluded_regex (List[pathlib.Path]): Regex used to exclude files from `local_dependencies` / `local_code`.
             Default to [].
             Always excludes common data formats (see
@@ -37,24 +36,24 @@
         force_included_paths (List[pathlib.Path]): Force include files otherwise excluded by `excluded_paths`
             and `excluded_regex`
             Default to []
     """
 
     editable_mode: bool = False
     pypi_dependencies: List[str] = Field(default_factory=list)
-    local_installable_dependencies: List[Path] = Field(default_factory=list)
+    local_dependencies: List[Path] = Field(default_factory=list)
     local_code: List[Path] = Field(default_factory=list)
     excluded_paths: List[Path] = Field(default_factory=list)
     excluded_regex: List[str] = Field(default_factory=list)
     force_included_paths: List[Path] = Field(default_factory=list)
 
     class Config:
         arbitrary_types_allowed = True
 
-    @validator("local_installable_dependencies", "local_code")
+    @validator("local_dependencies", "local_code")
     def resolve_path(cls, v):  # noqa: N805
         """Resolve list of local code paths and check if they exist."""
         not_existing_paths = list()
         resolved_paths = list()
         for path in v:
             if not Path(path).exists():
                 not_existing_paths += [f"\n\t{Path(path)} AS {Path(path).resolve()}"]
@@ -64,17 +63,17 @@
         if not_existing_paths:
             raise InvalidPathError(
                 f"Couldn't resolve :{''.join(not_existing_paths)}\nPlease explicit the input path(s)."
             )
 
         return resolved_paths
 
-    @validator("local_installable_dependencies")
+    @validator("local_dependencies")
     def check_setup(cls, v):  # noqa: N805
-        """Check the presence of a setup.py file or a pyproject.toml in the provided paths."""
+        """Check the presence of a setup.py file in the provided paths."""
         not_installable = list()
         for dependency_path in v:
             installable_dir = (dependency_path / "setup.py").is_file() or (dependency_path / "pyproject.toml").is_file()
             if dependency_path.is_dir() and not installable_dir:
                 not_installable.append(dependency_path)
             # The user can also give tar.gz archives
         if not_installable:
@@ -83,15 +82,15 @@
                 f"But neither setup.py or pyproject.toml was found in :{', '.join([str(p) for p in not_installable])}"
             )
         return v
 
     def copy_dependencies_local_package(self, *, dest_dir: Path) -> List[Path]:
         return path_management.copy_paths(
             dest_dir=dest_dir,
-            src=self.local_installable_dependencies,
+            src=self.local_dependencies,
             force_included=self.force_included_paths,
             excluded=self.excluded_paths,
             excluded_regex=self.excluded_regex,
         )
 
     def copy_dependencies_local_code(self, *, dest_dir: Path) -> List[Path]:
         return path_management.copy_paths(
```

### Comparing `substrafl-0.37.0rc1/substrafl/evaluation_strategy.py` & `substrafl-0.37.0rc2/substrafl/evaluation_strategy.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/substrafl/exceptions.py` & `substrafl-0.37.0rc2/substrafl/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,26 +6,14 @@
     """No batch size found."""
 
 
 class SubstraToolsDeprecationWarning(DeprecationWarning):
     """The substratools version used is deprecated."""
 
 
-class UnsupportedPythonVersionError(Exception):
-    """The Python version used is not supported by Substra."""
-
-
-class InvalidUserModuleError(Exception):
-    """The local folder passed by the user as a dependency is not a valid Python module."""
-
-
-class InvalidDependenciesError(Exception):
-    """The set of constraints given on dependencies cannot be solved or is otherwise invalid (wrong package name)."""
-
-
 class CriterionReductionError(Exception):
     """The criterion reduction must be set to 'mean' to use the Newton-Raphson strategy."""
 
 
 class DampingFactorValueError(Exception):
     """The damping factor must be greater than 0 and less than or equal to 1"""
```

### Comparing `substrafl-0.37.0rc1/substrafl/experiment.py` & `substrafl-0.37.0rc2/substrafl/experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,15 +252,14 @@
         client (substra.Client): A substra client to interact with the Substra platform
         strategy (Strategy): The strategy that will be executed
         train_data_nodes (typing.List[TrainDataNode]): List of the nodes where training on data
             occurs evaluation_strategy (EvaluationStrategy, Optional): If None performance will not be measured at all.
             Otherwise measuring of performance will follow the EvaluationStrategy. Defaults to None.
         aggregation_node (typing.Optional[AggregationNode]): For centralized strategy, the aggregation
             node, where all the shared tasks occurs else None.
-        evaluation_strategy: Optional[EvaluationStrategy]
         num_rounds (int): The number of time your strategy will be executed
         dependencies (Dependency, Optional): Dependencies of the experiment. It must be defined from
             the SubstraFL Dependency class. Defaults None.
         experiment_folder (typing.Union[str, pathlib.Path]): path to the folder where the experiment summary is saved.
         clean_models (bool): Clean the intermediary models on the Substra platform. Set it to False
             if you want to download or re-use intermediary models. This causes the disk space to fill
             quickly so should be set to True unless needed. Defaults to True.
```

### Comparing `substrafl-0.37.0rc1/substrafl/index_generator/base.py` & `substrafl-0.37.0rc2/substrafl/index_generator/base.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/substrafl/index_generator/np_index_generator.py` & `substrafl-0.37.0rc2/substrafl/index_generator/np_index_generator.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/substrafl/logger.py` & `substrafl-0.37.0rc2/substrafl/logger.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/substrafl/model_loading.py` & `substrafl-0.37.0rc2/substrafl/model_loading.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/substrafl/nodes/__init__.py` & `substrafl-0.37.0rc2/substrafl/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/substrafl/nodes/aggregation_node.py` & `substrafl-0.37.0rc2/substrafl/nodes/aggregation_node.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/substrafl/nodes/node.py` & `substrafl-0.37.0rc2/substrafl/nodes/node.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/substrafl/nodes/test_data_node.py` & `substrafl-0.37.0rc2/substrafl/nodes/test_data_node.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/substrafl/nodes/train_data_node.py` & `substrafl-0.37.0rc2/substrafl/nodes/train_data_node.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/substrafl/remote/decorators.py` & `substrafl-0.37.0rc2/substrafl/remote/decorators.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/substrafl/remote/operations.py` & `substrafl-0.37.0rc2/substrafl/remote/operations.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/substrafl/remote/register/register.py` & `substrafl-0.37.0rc2/substrafl/remote/register/register.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,76 +1,63 @@
 """
 Create the Substra function assets and register them to the platform.
 """
-
 import logging
 import os
 import tarfile
 import tempfile
 import typing
 import warnings
 from distutils import util
 from pathlib import Path
-from pathlib import PurePosixPath
 from platform import python_version
 
 import substra
 import substratools
 from packaging import version
 
 import substrafl
 from substrafl import exceptions
 from substrafl.constants import TMP_SUBSTRAFL_PREFIX
 from substrafl.dependency import Dependency
-from substrafl.exceptions import UnsupportedPythonVersionError
 from substrafl.nodes.node import InputIdentifiers
-from substrafl.remote.register.manage_dependencies import compile_requirements
-from substrafl.remote.register.manage_dependencies import copy_local_wheels
-from substrafl.remote.register.manage_dependencies import get_pypi_dependencies_versions
-from substrafl.remote.register.manage_dependencies import local_lib_wheels
+from substrafl.remote.register.generate_wheel import local_lib_wheels
+from substrafl.remote.register.generate_wheel import pypi_lib_wheels
 from substrafl.remote.remote_struct import RemoteStruct
 from substrafl.remote.substratools_methods import RemoteMethod
 
 logger = logging.getLogger(__name__)
 
 # Substra tools version for which the image naming scheme changed
 MINIMAL_DOCKER_SUBSTRATOOLS_VERSION = "0.16.0"
 
-# minimal and maximal values of Python 3 minor versions supported
-# we need to store this as integer, else "3.10" < "3.9" (string comparison)
-MINIMAL_PYTHON_VERSION = 8  # 3.8
-MAXIMAL_PYTHON_VERSION = 10  # 3.10
-
 _DEFAULT_SUBSTRATOOLS_IMAGE = "ghcr.io/substra/substra-tools:\
 {substratools_version}-nvidiacuda11.8.0-base-ubuntu22.04-python{python_version}"
 
 SUBSTRAFL_FOLDER = "substrafl_internal"
 
 DOCKERFILE_TEMPLATE = """
 FROM {docker_image}
 
 # install dependencies
 RUN python{python_version} -m pip install -U pip
 
-# Copy local wheels
-{copy_wheels}
-
-# Copy requirements.txt
-COPY {internal_dir}/requirements.txt requirements.txt
+# Install substrafl, substra (and substratools if editable mode)
+{cl_deps}
 
-# Install requirements
-RUN python{python_version} -m pip install --no-cache-dir -r requirements.txt
+# PyPi dependencies
+{pypi_dependencies}
 
-# Copy all other files
-COPY function.py .
-COPY {internal_dir}/cls_cloudpickle {internal_dir}/
-COPY {internal_dir}/description.md {internal_dir}/
-{copy_local_code}
+# Install local dependencies
+{local_dependencies}
 
 ENTRYPOINT ["python{python_version}", "function.py", "--function-name", "{method_name}"]
+
+COPY . .
+
 """
 
 FUNCTION = """
 import json
 import cloudpickle
 
 import substratools as tools
@@ -90,136 +77,62 @@
     remote_instance.register_substratools_function()
 
     # Execute the function using substra-tools
     tools.execute()
 """
 
 
+def iter_dockerfile_install_command(paths: typing.List[Path], python_major_minor: str) -> str:
+    for path in paths:
+        # Does not work with path.is_dir(), surely a race condition. Should be removed in  #123
+        formatted_path = (str(path) + "/") if not path.is_file() else path
+        yield f"COPY {path}  {path} \nRUN python{python_major_minor} -m pip install --no-cache-dir {formatted_path} \n"
+
+
+def _copy_local_packages(path: Path, python_major_minor: str, operation_dir: Path, dependencies: Dependency):
+    """Copy the local libraries given by the user and generate the installation command."""
+    path.mkdir(exist_ok=True)
+    dependencies_paths = dependencies.copy_dependencies_local_package(dest_dir=operation_dir)
+
+    local_dependencies_cmd = "\n".join(iter_dockerfile_install_command(dependencies_paths, python_major_minor))
+
+    return local_dependencies_cmd
+
+
 def _create_archive(archive_path: Path, src_path: Path):
     """Create a tar archive from a folder"""
     with tarfile.open(archive_path, "w:gz") as tar:
         for filepath in src_path.glob("*"):
             if not filepath.name.endswith(".tar.gz"):
                 tar.add(filepath, arcname=filepath.name, recursive=True)
 
 
-def _check_python_version(python_major_minor: str) -> None:
-    """Raise UnsupportedPythonVersionError exception if the Python version is not supported"""
-    major, minor = python_major_minor.split(".")
-    if major != "3":
-        raise UnsupportedPythonVersionError("Only Python 3 is supported")
-    if int(minor) < MINIMAL_PYTHON_VERSION or int(minor) > MAXIMAL_PYTHON_VERSION:
-        raise UnsupportedPythonVersionError(
-            f"The current Python version is {python_major_minor}, which is unsupported;"
-            f"supported versions are 3.{MINIMAL_PYTHON_VERSION} to 3.{MAXIMAL_PYTHON_VERSION}"
-        )
-
-
-def _get_base_docker_image(python_major_minor: str, editable_mode: bool) -> str:
+def _get_base_docker_image(python_major_minor: str, editable_mode: bool):
     """Get the base Docker image for the Dockerfile"""
 
     substratools_image_version = substratools.__version__
     if util.strtobool(os.environ.get("USE_LATEST_SUBSTRATOOLS", "False")):
         substratools_image_version = "latest"
     elif version.parse(substratools_image_version) < version.parse(MINIMAL_DOCKER_SUBSTRATOOLS_VERSION):
         if not editable_mode:
             warnings.warn(
                 f"Your environment uses substra-tools={substratools_image_version}. Version \
                 {MINIMAL_DOCKER_SUBSTRATOOLS_VERSION} will be used on Docker.",
                 exceptions.SubstraToolsDeprecationWarning,
                 stacklevel=2,
             )
         substratools_image_version = MINIMAL_DOCKER_SUBSTRATOOLS_VERSION
-
-    _check_python_version(python_major_minor)
-
     substratools_image = _DEFAULT_SUBSTRATOOLS_IMAGE.format(
         substratools_version=substratools_image_version,
         python_version=python_major_minor,
     )
 
     return substratools_image
 
 
-def _generate_copy_local_files(local_files: typing.List[Path]) -> str:
-    # In Dockerfiles, we need to always have '/'. PurePosixPath resolves that.
-    return "\n".join([f"COPY {PurePosixPath(file)} {PurePosixPath(file)}" for file in local_files])
-
-
-def _create_dockerfile(install_libraries: bool, dependencies: Dependency, operation_dir: Path, method_name: str) -> str:
-    substrafl_internal = operation_dir / SUBSTRAFL_FOLDER
-    substrafl_internal.mkdir(exist_ok=True)
-
-    # get Python version
-    # Required to select the correct version of python inside the docker Image
-    # Cloudpickle will crash if we don't deserialize with the same major.minor
-    python_major_minor = ".".join(python_version().split(".")[:2])
-
-    # Get the base Docker image
-    substratools_image = _get_base_docker_image(
-        python_major_minor=python_major_minor, editable_mode=dependencies.editable_mode
-    )
-
-    pypi_dependencies = dependencies.pypi_dependencies
-    wheels = []
-    # Build Substrafl, Substra and Substratools, and local dependencies wheels if necessary
-    if install_libraries:
-        # Substrafl, Substra and Substratools
-        # Install either from pypi wheel or repo in editable mode
-        if dependencies.editable_mode or util.strtobool(os.environ.get("SUBSTRA_FORCE_EDITABLE_MODE", "False")):
-            substra_wheel_dir = substrafl_internal / "dist"
-            substra_wheels = local_lib_wheels(
-                lib_modules=[
-                    substrafl,
-                    substra,
-                    substratools,
-                ],  # We reinstall substratools in editable mode to overwrite the installed version
-                dest_dir=substra_wheel_dir,
-            )
-            wheels += [substra_wheel_dir.relative_to(operation_dir) / wheel_name for wheel_name in substra_wheels]
-        else:
-            pypi_dependencies += get_pypi_dependencies_versions(
-                lib_modules=[substrafl],
-            )
-
-        local_dep_dir = substrafl_internal / "local_dependencies"
-        wheels += [
-            local_dep_dir.relative_to(operation_dir) / wheel_name
-            for wheel_name in copy_local_wheels(
-                path=local_dep_dir,
-                dependencies=dependencies,
-            )
-        ]
-        # generate the copy wheel command
-        copy_wheels_cmd = _generate_copy_local_files(wheels)
-
-        # create a requirements.in with all requirements (substra libs and user-defined)
-        dependency_list = pypi_dependencies + wheels
-
-    else:
-        dependency_list = []
-        copy_wheels_cmd = ""
-
-    # user-defined local dependencies
-    local_paths = dependencies.copy_dependencies_local_code(dest_dir=operation_dir)
-    copy_local_code_cmd = _generate_copy_local_files(local_paths)
-
-    # pip-compile the requirements.in into a requirements.txt
-    compile_requirements(dependency_list, operation_dir=operation_dir, sub_dir=SUBSTRAFL_FOLDER)
-
-    return DOCKERFILE_TEMPLATE.format(
-        docker_image=substratools_image,
-        python_version=python_major_minor,
-        copy_wheels=copy_wheels_cmd,
-        copy_local_code=copy_local_code_cmd,
-        method_name=method_name,
-        internal_dir=SUBSTRAFL_FOLDER,
-    )
-
-
 def _create_substra_function_files(
     remote_struct: RemoteStruct,
     install_libraries: bool,
     dependencies: Dependency,
     operation_dir: Path,
 ) -> typing.Tuple[Path, Path]:
     """Creates the necessary files from the remote struct to register the associated function to substra, zip them into
@@ -229,72 +142,109 @@
 
             - the RemoteStruct (wrapped code) dump file
             - the wheel of the current version of Substrafl and Substra
             - the Dockerfile
             - the description.md
             - the function.py entrypoint
 
-        Target tree structure:
-            ├── Dockerfile
-            ├── function.py
-            ├── function.tar.gz
-            ├── local_code.py
-            └── substrafl_internal
-                ├── cls_cloudpickle
-                ├── description.md
-                ├── dist
-                │   ├── substra-0.44.0-py3-none-any.whl
-                │   ├── substrafl-0.36.0-py3-none-any.whl
-                │   └── substratools-0.20.0-py3-none-any.whl
-                ├── local_dependencies
-                │   └── local-module-1.6.1-py3-none-any.whl
-                ├── requirements.in
-                └── requirements.txt
-
     Args:
         remote_struct (RemoteStruct): A representation of a substra algorithm.
         install_libraries (bool): whether we need to build the wheels and copy the files to install the libraries
         dependencies (Dependency): Function dependencies.
         operation_dir (pathlib.Path): path to the operation directory
 
         Returns:
             Tuple[Path, Path]: The archive path and the description file path.
     """
     substrafl_internal = operation_dir / SUBSTRAFL_FOLDER
     substrafl_internal.mkdir()
 
     remote_struct.save(dest=substrafl_internal)
 
-    # Write dockerfile based on template
-    dockerfile_path = operation_dir / "Dockerfile"
-    dockerfile_path.write_text(
-        _create_dockerfile(
-            install_libraries=install_libraries,
-            dependencies=dependencies,
-            operation_dir=operation_dir,
-            method_name=remote_struct._method_name,
-        )
+    # get Python version
+    # Required to select the correct version of python inside the docker Image
+    # Cloudpickle will crash if we don't deserialize with the same major.minor
+    python_major_minor = ".".join(python_version().split(".")[:2])
+
+    # Build Substrafl, Substra and Substratools wheel if needed
+    install_cmd = ""
+    if install_libraries:
+        # Install either from pypi wheel or repo in editable mode
+        if dependencies.editable_mode or util.strtobool(os.environ.get("SUBSTRA_FORCE_EDITABLE_MODE", "False")):
+            install_cmd = local_lib_wheels(
+                lib_modules=[
+                    substrafl,
+                    substra,
+                    substratools,
+                ],  # We reinstall substratools in editable mode to overwrite the installed version
+                operation_dir=operation_dir,
+                python_major_minor=python_major_minor,
+                dest_dir=f"{SUBSTRAFL_FOLDER}/dist",
+            )
+        else:
+            install_cmd = pypi_lib_wheels(
+                lib_modules=[substrafl, substra],
+                operation_dir=operation_dir,
+                python_major_minor=python_major_minor,
+                dest_dir=f"{SUBSTRAFL_FOLDER}/dist",
+            )
+
+    # Pypi dependencies docker command if specified by the user
+    pypi_dependencies_cmd = (
+        f"RUN python{python_major_minor} -m pip install --no-cache-dir {' '.join(dependencies.pypi_dependencies)}"
+        if dependencies is not None and len(dependencies.pypi_dependencies) > 0
+        else ""
     )
 
+    # The files to copy to the container must be in the same folder as the Dockerfile
+    local_dependencies_cmd = ""
+    if dependencies is not None:
+        dependencies.copy_dependencies_local_code(dest_dir=operation_dir)
+        if install_libraries:
+            local_dep_dir = substrafl_internal / "local_dependencies"
+            local_dependencies_cmd = _copy_local_packages(
+                path=local_dep_dir,
+                dependencies=dependencies,
+                python_major_minor=python_major_minor,
+                operation_dir=operation_dir,
+            )
+
     # Write template to function.py
     function_path = operation_dir / "function.py"
     function_path.write_text(
         FUNCTION.format(
             substrafl_folder=SUBSTRAFL_FOLDER,
         )
     )
 
     # Write description
     description_path = substrafl_internal / "description.md"
     description_path.write_text("# Substrafl Operation")
 
+    # Get the base Docker image
+    substratools_image = _get_base_docker_image(
+        python_major_minor=python_major_minor, editable_mode=dependencies.editable_mode
+    )
+
+    # Write dockerfile based on template
+    dockerfile_path = operation_dir / "Dockerfile"
+    dockerfile_path.write_text(
+        DOCKERFILE_TEMPLATE.format(
+            docker_image=substratools_image,
+            python_version=python_major_minor,
+            cl_deps=install_cmd,
+            pypi_dependencies=pypi_dependencies_cmd,
+            local_dependencies=local_dependencies_cmd,
+            method_name=remote_struct._method_name,
+        )
+    )
+
     # Create necessary archive to register the operation on substra
     archive_path = operation_dir / "function.tar.gz"
     _create_archive(archive_path=archive_path, src_path=operation_dir)
-
     return archive_path, description_path
 
 
 def register_function(
     *,
     client: substra.Client,
     remote_struct: RemoteStruct,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `substrafl-0.37.0rc1/substrafl/remote/remote_struct.py` & `substrafl-0.37.0rc2/substrafl/remote/remote_struct.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/substrafl/remote/serializers/pickle_serializer.py` & `substrafl-0.37.0rc2/substrafl/remote/serializers/pickle_serializer.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/substrafl/remote/substratools_methods.py` & `substrafl-0.37.0rc2/substrafl/remote/substratools_methods.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/substrafl/strategies/fed_avg.py` & `substrafl-0.37.0rc2/substrafl/strategies/fed_avg.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/substrafl/strategies/fed_pca.py` & `substrafl-0.37.0rc2/substrafl/strategies/fed_pca.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/substrafl/strategies/newton_raphson.py` & `substrafl-0.37.0rc2/substrafl/strategies/newton_raphson.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/substrafl/strategies/scaffold.py` & `substrafl-0.37.0rc2/substrafl/strategies/scaffold.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/substrafl/strategies/schemas.py` & `substrafl-0.37.0rc2/substrafl/strategies/schemas.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/substrafl/strategies/single_organization.py` & `substrafl-0.37.0rc2/substrafl/strategies/single_organization.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/substrafl/strategies/strategy.py` & `substrafl-0.37.0rc2/substrafl/strategies/strategy.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.37.0rc1/substrafl.egg-info/PKG-INFO` & `substrafl-0.37.0rc2/substrafl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrafl
-Version: 0.37.0rc1
+Version: 0.37.0rc2
 Summary: A high-level federated learning Python library to run      federated learning experiments at scale on a Substra network
 Home-page: https://docs.substra.org/
 Author: Owkin, Inc.
 License: Apache 2.0
 Description: readme
 Keywords: substrafl
 Platform: UNKNOWN
```

### Comparing `substrafl-0.37.0rc1/substrafl.egg-info/SOURCES.txt` & `substrafl-0.37.0rc2/substrafl.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 substrafl/nodes/references/shared_state.py
 substrafl/remote/__init__.py
 substrafl/remote/decorators.py
 substrafl/remote/operations.py
 substrafl/remote/remote_struct.py
 substrafl/remote/substratools_methods.py
 substrafl/remote/register/__init__.py
-substrafl/remote/register/manage_dependencies.py
+substrafl/remote/register/generate_wheel.py
 substrafl/remote/register/register.py
 substrafl/remote/serializers/__init__.py
 substrafl/remote/serializers/pickle_serializer.py
 substrafl/remote/serializers/serializer.py
 substrafl/strategies/__init__.py
 substrafl/strategies/fed_avg.py
 substrafl/strategies/fed_pca.py
```

