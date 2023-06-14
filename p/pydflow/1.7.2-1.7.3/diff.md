# Comparing `tmp/pydflow-1.7.2.tar.gz` & `tmp/pydflow-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydflow-1.7.2.tar", last modified: Tue Jun 13 01:44:56 2023, max compression
+gzip compressed data, was "pydflow-1.7.3.tar", last modified: Tue Jun 13 12:27:11 2023, max compression
```

## Comparing `pydflow-1.7.2.tar` & `pydflow-1.7.3.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:44:56.615004 pydflow-1.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-06-13 01:44:47.000000 pydflow-1.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-13 01:44:47.000000 pydflow-1.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    33145 2023-06-13 01:44:56.615004 pydflow-1.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    32758 2023-06-13 01:44:47.000000 pydflow-1.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 01:44:47.000000 pydflow-1.7.2/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 01:44:56.615004 pydflow-1.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-13 01:44:47.000000 pydflow-1.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:44:56.607004 pydflow-1.7.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:44:56.611004 pydflow-1.7.2/src/dflow/
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/argo_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:44:56.611004 pydflow-1.7.2/src/dflow/client/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17690 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/client/v1alpha1_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/client/v1alpha1_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/client/v1alpha1_retry_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/client/v1alpha1_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/client/v1alpha1_value_from.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/context_syntax.py
--rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)    11261 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    51335 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    23997 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/op_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:44:56.611004 pydflow-1.7.2/src/dflow/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14571 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/plugins/bohrium.py
--rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/plugins/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    23061 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/plugins/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/plugins/launching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/plugins/lebesgue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/plugins/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/plugins/oss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/plugins/ray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:44:56.611004 pydflow-1.7.2/src/dflow/python/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/python/op.py
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/python/opio.py
--rw-r--r--   0 runner    (1001) docker     (123)    31692 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/python/python_op_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    12145 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/python/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    16413 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)   102304 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/util_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    25552 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    45085 2023-06-13 01:44:47.000000 pydflow-1.7.2/src/dflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:44:56.611004 pydflow-1.7.2/src/pydflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    33145 2023-06-13 01:44:56.000000 pydflow-1.7.2/src/pydflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-13 01:44:56.000000 pydflow-1.7.2/src/pydflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 01:44:56.000000 pydflow-1.7.2/src/pydflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-13 01:44:56.000000 pydflow-1.7.2/src/pydflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-13 01:44:56.000000 pydflow-1.7.2/src/pydflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-13 01:44:56.000000 pydflow-1.7.2/src/pydflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:44:56.615004 pydflow-1.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-13 01:44:47.000000 pydflow-1.7.2/tests/test_big_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-13 01:44:47.000000 pydflow-1.7.2/tests/test_conditional_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-13 01:44:47.000000 pydflow-1.7.2/tests/test_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-13 01:44:47.000000 pydflow-1.7.2/tests/test_group_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-06-13 01:44:47.000000 pydflow-1.7.2/tests/test_makevasp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-13 01:44:47.000000 pydflow-1.7.2/tests/test_python.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-13 01:44:47.000000 pydflow-1.7.2/tests/test_recurse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-13 01:44:47.000000 pydflow-1.7.2/tests/test_reuse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-13 01:44:47.000000 pydflow-1.7.2/tests/test_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-13 01:44:47.000000 pydflow-1.7.2/tests/test_subpath_slices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:27:11.671557 pydflow-1.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-06-13 12:27:00.000000 pydflow-1.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-13 12:27:00.000000 pydflow-1.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    33145 2023-06-13 12:27:11.671557 pydflow-1.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    32758 2023-06-13 12:27:00.000000 pydflow-1.7.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 12:27:00.000000 pydflow-1.7.3/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 12:27:11.671557 pydflow-1.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-13 12:27:00.000000 pydflow-1.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:27:11.659556 pydflow-1.7.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:27:11.663556 pydflow-1.7.3/src/dflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/argo_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:27:11.667557 pydflow-1.7.3/src/dflow/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17690 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/client/v1alpha1_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/client/v1alpha1_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/client/v1alpha1_retry_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/client/v1alpha1_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/client/v1alpha1_value_from.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/context_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11261 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51335 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23997 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/op_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:27:11.667557 pydflow-1.7.3/src/dflow/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14571 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/plugins/bohrium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/plugins/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23061 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/plugins/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/plugins/launching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/plugins/lebesgue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/plugins/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/plugins/oss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/plugins/ray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:27:11.667557 pydflow-1.7.3/src/dflow/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/python/op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/python/opio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31751 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/python/python_op_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12145 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/python/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16413 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102606 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/util_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25552 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45085 2023-06-13 12:27:00.000000 pydflow-1.7.3/src/dflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:27:11.671557 pydflow-1.7.3/src/pydflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    33145 2023-06-13 12:27:11.000000 pydflow-1.7.3/src/pydflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-13 12:27:11.000000 pydflow-1.7.3/src/pydflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 12:27:11.000000 pydflow-1.7.3/src/pydflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-13 12:27:11.000000 pydflow-1.7.3/src/pydflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-13 12:27:11.000000 pydflow-1.7.3/src/pydflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-13 12:27:11.000000 pydflow-1.7.3/src/pydflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:27:11.671557 pydflow-1.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-13 12:27:00.000000 pydflow-1.7.3/tests/test_big_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-13 12:27:00.000000 pydflow-1.7.3/tests/test_conditional_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-13 12:27:00.000000 pydflow-1.7.3/tests/test_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-13 12:27:00.000000 pydflow-1.7.3/tests/test_group_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-06-13 12:27:00.000000 pydflow-1.7.3/tests/test_makevasp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-13 12:27:00.000000 pydflow-1.7.3/tests/test_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-13 12:27:00.000000 pydflow-1.7.3/tests/test_recurse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-13 12:27:00.000000 pydflow-1.7.3/tests/test_reuse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-13 12:27:00.000000 pydflow-1.7.3/tests/test_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-13 12:27:00.000000 pydflow-1.7.3/tests/test_subpath_slices.py
```

### Comparing `pydflow-1.7.2/LICENSE` & `pydflow-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/PKG-INFO` & `pydflow-1.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydflow
-Version: 1.7.2
+Version: 1.7.3
 Summary: Dflow is a Python framework for constructing scientific computing workflows employing Argo Workflows as the workflow engine.
 Home-page: https://github.com/deepmodeling/dflow
 Author: Xinzijian Liu
 Author-email: liuxzj@dp.tech
 License: LGPLv3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pydflow-1.7.2/README.md` & `pydflow-1.7.3/README.md`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/setup.py` & `pydflow-1.7.3/setup.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/src/dflow/__init__.py` & `pydflow-1.7.3/src/dflow/__init__.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/src/dflow/argo_objects.py` & `pydflow-1.7.3/src/dflow/argo_objects.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/src/dflow/client/v1alpha1_artifact.py` & `pydflow-1.7.3/src/dflow/client/v1alpha1_artifact.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/src/dflow/client/v1alpha1_parameter.py` & `pydflow-1.7.3/src/dflow/client/v1alpha1_parameter.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/src/dflow/client/v1alpha1_retry_strategy.py` & `pydflow-1.7.3/src/dflow/client/v1alpha1_retry_strategy.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/src/dflow/client/v1alpha1_sequence.py` & `pydflow-1.7.3/src/dflow/client/v1alpha1_sequence.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/src/dflow/client/v1alpha1_value_from.py` & `pydflow-1.7.3/src/dflow/client/v1alpha1_value_from.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/src/dflow/common.py` & `pydflow-1.7.3/src/dflow/common.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/src/dflow/config.py` & `pydflow-1.7.3/src/dflow/config.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/src/dflow/context_syntax.py` & `pydflow-1.7.3/src/dflow/context_syntax.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/src/dflow/dag.py` & `pydflow-1.7.3/src/dflow/dag.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/src/dflow/executor.py` & `pydflow-1.7.3/src/dflow/executor.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/src/dflow/io.py` & `pydflow-1.7.3/src/dflow/io.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/src/dflow/main.py` & `pydflow-1.7.3/src/dflow/main.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/src/dflow/op_template.py` & `pydflow-1.7.3/src/dflow/op_template.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/src/dflow/plugins/bohrium.py` & `pydflow-1.7.3/src/dflow/plugins/bohrium.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/src/dflow/plugins/datasets.py` & `pydflow-1.7.3/src/dflow/plugins/datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 config = {
     "rclone_image": os.environ.get("RCLONE_IMAGE", "rclone/rclone:1.62.2"),
     "rclone_image_pull_policy": os.environ.get("RCLONE_IMAGE_PULL_POLICY"),
     "rclone_type": os.environ.get("DATASETS_RCLONE_TYPE", "ftp"),
     "ftp_host": os.environ.get("DATASETS_FTP_HOST",
                                "uftp.mlops-passthrough.dp.tech"),
     "webdav_host": os.environ.get("DATASETS_WEBDAV_HOST",
-                                  "https://webdav.launching.mlops.dp.tech"),
+                                  "https://webdav.mlops.dp.tech"),
     "user": os.environ.get("DATASETS_USER"),
     "password": os.environ.get("DATASETS_PASSWORD"),
 }
 
 
 class DatasetsArtifact(DispatcherArtifact):
     def __init__(self, element, version, type="datasets",
```

### Comparing `pydflow-1.7.2/src/dflow/plugins/dispatcher.py` & `pydflow-1.7.3/src/dflow/plugins/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/src/dflow/plugins/launching.py` & `pydflow-1.7.3/src/dflow/plugins/launching.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/src/dflow/plugins/lebesgue.py` & `pydflow-1.7.3/src/dflow/plugins/lebesgue.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/src/dflow/plugins/metadata.py` & `pydflow-1.7.3/src/dflow/plugins/metadata.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/src/dflow/plugins/oss.py` & `pydflow-1.7.3/src/dflow/plugins/oss.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/src/dflow/plugins/ray.py` & `pydflow-1.7.3/src/dflow/plugins/ray.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/src/dflow/python/op.py` & `pydflow-1.7.3/src/dflow/python/op.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/src/dflow/python/opio.py` & `pydflow-1.7.3/src/dflow/python/opio.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/src/dflow/python/python_op_template.py` & `pydflow-1.7.3/src/dflow/python/python_op_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -469,15 +469,16 @@
                         script += "    input_sign['%s'].type = List[Path]\n" %\
                             name
         if any([art.save_as_parameter
                 for art in self.inputs.artifacts.values()]):
             script += "    pids = []\n"
         for name, sign in input_sign.items():
             if isinstance(sign, Artifact):
-                if self.inputs.artifacts[name].save_as_parameter:
+                if name in self.inputs.artifacts and self.inputs.artifacts[
+                        name].save_as_parameter:
                     script += "    pids.append(jsonpickle.loads('{{inputs."\
                         "parameters.dflow_art_%s}}').%s('%s', '%s/inputs/"\
                         "artifacts/%s'))\n" % (name, self.download_method,
                                                name, self.tmp_root, name)
                 slices = self.get_slices(input_artifact_slices, name)
                 if self.slices is not None and self.slices.sub_path and \
                         name in self.slices.input_artifact:
```

### Comparing `pydflow-1.7.2/src/dflow/python/utils.py` & `pydflow-1.7.3/src/dflow/python/utils.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/src/dflow/resource.py` & `pydflow-1.7.3/src/dflow/resource.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/src/dflow/slurm.py` & `pydflow-1.7.3/src/dflow/slurm.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/src/dflow/step.py` & `pydflow-1.7.3/src/dflow/step.py`

 * *Files 0% similar despite different names*

```diff
@@ -1442,14 +1442,16 @@
 
             for name, art in self.inputs.artifacts.items():
                 if isinstance(art.source, S3Artifact) and not hasattr(
                         art.source, "local_path"):
                     path = os.path.abspath("download/%s" % randstr())
                     art.source.download(path=path, debug_download=True,
                                         remove_catalog=False)
+                    assert os.path.exists(path), "S3 key of the input art"\
+                        "ifact %s: %s does not exist" % (name, art.source.key)
                     fs = os.listdir(path)
                     if len(fs) == 1 and os.path.isfile(os.path.join(path,
                                                                     fs[0])):
                         os.rename(os.path.join(path, fs[0]), path + ".bk")
                         os.rmdir(path)
                         os.rename(path + ".bk", path)
                     art.source.local_path = path
@@ -1672,14 +1674,16 @@
                     art.source = art.source[:i+2]
                 art.source = get_var(art.source, scope)
             if isinstance(art.source, S3Artifact) and not hasattr(
                     art.source, "local_path"):
                 path = os.path.abspath("download/%s" % randstr())
                 art.source.download(path=path, debug_download=True,
                                     remove_catalog=False)
+                assert os.path.exists(path), "S3 key of the input art"\
+                    "ifact %s: %s does not exist" % (name, art.source.key)
                 fs = os.listdir(path)
                 if len(fs) == 1 and os.path.isfile(os.path.join(path,
                                                                 fs[0])):
                     os.rename(os.path.join(path, fs[0]), path + ".bk")
                     os.rmdir(path)
                     os.rename(path + ".bk", path)
                 art.source.local_path = path
```

### Comparing `pydflow-1.7.2/src/dflow/steps.py` & `pydflow-1.7.3/src/dflow/steps.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/src/dflow/task.py` & `pydflow-1.7.3/src/dflow/task.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/src/dflow/util_ops.py` & `pydflow-1.7.3/src/dflow/util_ops.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/src/dflow/utils.py` & `pydflow-1.7.3/src/dflow/utils.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/src/dflow/workflow.py` & `pydflow-1.7.3/src/dflow/workflow.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/src/pydflow.egg-info/PKG-INFO` & `pydflow-1.7.3/src/pydflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydflow
-Version: 1.7.2
+Version: 1.7.3
 Summary: Dflow is a Python framework for constructing scientific computing workflows employing Argo Workflows as the workflow engine.
 Home-page: https://github.com/deepmodeling/dflow
 Author: Xinzijian Liu
 Author-email: liuxzj@dp.tech
 License: LGPLv3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pydflow-1.7.2/src/pydflow.egg-info/SOURCES.txt` & `pydflow-1.7.3/src/pydflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/tests/test_big_parameter.py` & `pydflow-1.7.3/tests/test_big_parameter.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/tests/test_conditional_outputs.py` & `pydflow-1.7.3/tests/test_conditional_outputs.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/tests/test_dag.py` & `pydflow-1.7.3/tests/test_dag.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/tests/test_group_size.py` & `pydflow-1.7.3/tests/test_group_size.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/tests/test_makevasp.py` & `pydflow-1.7.3/tests/test_makevasp.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/tests/test_python.py` & `pydflow-1.7.3/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/tests/test_recurse.py` & `pydflow-1.7.3/tests/test_recurse.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/tests/test_reuse.py` & `pydflow-1.7.3/tests/test_reuse.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/tests/test_slices.py` & `pydflow-1.7.3/tests/test_slices.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.7.2/tests/test_subpath_slices.py` & `pydflow-1.7.3/tests/test_subpath_slices.py`

 * *Files identical despite different names*

