# Comparing `tmp/tensorcircuit-nightly-0.9.1.dev20230607.tar.gz` & `tmp/tensorcircuit-nightly-0.9.1.dev20230608.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorcircuit-nightly-0.9.1.dev20230607.tar", last modified: Wed Jun  7 12:47:24 2023, max compression
+gzip compressed data, was "tensorcircuit-nightly-0.9.1.dev20230608.tar", last modified: Thu Jun  8 12:42:14 2023, max compression
```

## Comparing `tensorcircuit-nightly-0.9.1.dev20230607.tar` & `tensorcircuit-nightly-0.9.1.dev20230608.tar`

### file list

```diff
@@ -1,137 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 12:47:24.298089 tensorcircuit-nightly-0.9.1.dev20230607/
--rw-r--r--   0 runner    (1001) docker     (122)    25828 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    21593 2023-06-07 12:47:24.298089 tensorcircuit-nightly-0.9.1.dev20230607/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    19131 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     6535 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/README_cn.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 12:47:24.286089 tensorcircuit-nightly-0.9.1.dev20230607/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 12:47:24.286089 tensorcircuit-nightly-0.9.1.dev20230607/docs/source/
--rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/docs/source/advance.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6356 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/docs/source/cnconf.py
--rw-r--r--   0 runner    (1001) docker     (122)     6461 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     8192 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/docs/source/contribution.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10971 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/docs/source/generate_rst.py
--rw-r--r--   0 runner    (1001) docker     (122)     5839 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10071 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/docs/source/infras.rst
--rw-r--r--   0 runner    (1001) docker     (122)      680 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/docs/source/modules.rst.backup
--rw-r--r--   0 runner    (1001) docker     (122)    27533 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/docs/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8223 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/docs/source/sharpbits.rst
--rw-r--r--   0 runner    (1001) docker     (122)      226 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/docs/source/textbooktoc.rst
--rw-r--r--   0 runner    (1001) docker     (122)      710 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/docs/source/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/docs/source/tutorial_cn.rst
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/docs/source/whitepapertoc.rst
--rw-r--r--   0 runner    (1001) docker     (122)      531 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/docs/source/whitepapertoc_cn.rst
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-07 12:47:24.298089 tensorcircuit-nightly-0.9.1.dev20230607/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-06-07 12:47:17.000000 tensorcircuit-nightly-0.9.1.dev20230607/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 12:47:24.290089 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/
--rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-06-07 12:47:17.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3101 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/about.py
--rw-r--r--   0 runner    (1001) docker     (122)    43480 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/abstractcircuit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 12:47:24.290089 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/applications/
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    34460 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/applications/dqas.py
--rw-r--r--   0 runner    (1001) docker     (122)    15348 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/applications/graphdata.py
--rw-r--r--   0 runner    (1001) docker     (122)    18124 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/applications/layers.py
--rw-r--r--   0 runner    (1001) docker     (122)    14032 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/applications/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    36391 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/applications/vags.py
--rw-r--r--   0 runner    (1001) docker     (122)    15117 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/applications/van.py
--rw-r--r--   0 runner    (1001) docker     (122)    23416 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/applications/vqes.py
--rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/asciiart.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 12:47:24.290089 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/backends/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    57621 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/backends/abstract_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/backends/backend_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)    14928 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/backends/cupy_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)    24925 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/backends/jax_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     4024 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/backends/jax_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/backends/numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)    24148 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/backends/pytorch_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     3825 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/backends/pytorch_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    35980 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/backends/tensorflow_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     3377 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/backends/tf_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    34020 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/basecircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)    28637 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/channels.py
--rw-r--r--   0 runner    (1001) docker     (122)    36220 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/circuit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 12:47:24.294089 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/cloud/
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14582 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/cloud/abstraction.py
--rw-r--r--   0 runner    (1001) docker     (122)    17866 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/cloud/apis.py
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/cloud/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2265 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/cloud/local.py
--rw-r--r--   0 runner    (1001) docker     (122)     2613 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/cloud/quafu_provider.py
--rw-r--r--   0 runner    (1001) docker     (122)    14325 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/cloud/tencent.py
--rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/cloud/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    11518 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/cloud/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 12:47:24.294089 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/compiler/
--rw-r--r--   0 runner    (1001) docker     (122)      241 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3258 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/compiler/composed_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)     6032 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/compiler/qiskit_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)     9595 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/compiler/simple_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    29573 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/cons.py
--rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/densitymatrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    17639 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/experimental.py
--rw-r--r--   0 runner    (1001) docker     (122)    29016 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/gates.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 12:47:24.294089 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)      545 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/interfaces/numpy.py
--rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/interfaces/scipy.py
--rw-r--r--   0 runner    (1001) docker     (122)     3355 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/interfaces/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (122)    10364 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/interfaces/tensortrans.py
--rw-r--r--   0 runner    (1001) docker     (122)     5117 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/interfaces/torch.py
--rw-r--r--   0 runner    (1001) docker     (122)    10126 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/keras.py
--rw-r--r--   0 runner    (1001) docker     (122)    15399 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/mps_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    34519 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/mpscircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)    11861 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/noisemodel.py
--rw-r--r--   0 runner    (1001) docker     (122)    82850 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/quantum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 12:47:24.294089 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/results/
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3435 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/results/counts.py
--rw-r--r--   0 runner    (1001) docker     (122)    31362 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/results/readout_mitigation.py
--rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/simplify.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 12:47:24.294089 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/templates/blocks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/templates/chems.py
--rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/templates/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     5811 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/templates/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     3934 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/templates/graphs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10942 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/templates/measurements.py
--rw-r--r--   0 runner    (1001) docker     (122)     4621 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/torchnn.py
--rw-r--r--   0 runner    (1001) docker     (122)    27335 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/translation.py
--rw-r--r--   0 runner    (1001) docker     (122)     7060 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 12:47:24.294089 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    21593 2023-06-07 12:47:24.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3561 2023-06-07 12:47:24.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-07 12:47:24.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      110 2023-06-07 12:47:24.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-07 12:47:24.000000 tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 12:47:24.298089 tensorcircuit-nightly-0.9.1.dev20230607/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)    33735 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tests/test_calibrating.py
--rw-r--r--   0 runner    (1001) docker     (122)    11237 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tests/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (122)    47707 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tests/test_circuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     5606 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tests/test_cloud.py
--rw-r--r--   0 runner    (1001) docker     (122)     3419 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tests/test_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    17232 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tests/test_dmcircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tests/test_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tests/test_gates.py
--rw-r--r--   0 runner    (1001) docker     (122)    13220 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tests/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tests/test_keras.py
--rw-r--r--   0 runner    (1001) docker     (122)     7445 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tests/test_miscs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10552 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tests/test_mpscircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     5637 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tests/test_noisemodel.py
--rw-r--r--   0 runner    (1001) docker     (122)      753 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tests/test_qaoa.py
--rw-r--r--   0 runner    (1001) docker     (122)    16823 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tests/test_quantum.py
--rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tests/test_quantum_attr.py
--rw-r--r--   0 runner    (1001) docker     (122)    11050 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tests/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (122)     2823 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tests/test_torchnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-06-07 12:23:30.000000 tensorcircuit-nightly-0.9.1.dev20230607/tests/test_van.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:42:14.869526 tensorcircuit-nightly-0.9.1.dev20230608/
+-rw-r--r--   0 runner    (1001) docker     (122)    25883 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    24257 2023-06-08 12:42:14.869526 tensorcircuit-nightly-0.9.1.dev20230608/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    21395 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     6535 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/README_cn.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:42:14.853525 tensorcircuit-nightly-0.9.1.dev20230608/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:42:14.857525 tensorcircuit-nightly-0.9.1.dev20230608/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/docs/source/advance.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6356 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/docs/source/cnconf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6461 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8192 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/docs/source/contribution.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10971 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3704 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/docs/source/generate_rst.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5839 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10071 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/docs/source/infras.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      710 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      680 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/docs/source/modules.rst.backup
+-rw-r--r--   0 runner    (1001) docker     (122)    27533 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8223 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/docs/source/sharpbits.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/docs/source/textbooktoc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      710 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/docs/source/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/docs/source/tutorial_cn.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/docs/source/whitepapertoc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/docs/source/whitepapertoc_cn.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-08 12:42:14.869526 tensorcircuit-nightly-0.9.1.dev20230608/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-06-08 12:42:07.000000 tensorcircuit-nightly-0.9.1.dev20230608/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:42:14.861526 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/
+-rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-06-08 12:42:07.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3101 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/about.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43480 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/abstractcircuit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:42:14.861526 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/applications/
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34460 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/applications/dqas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15348 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/applications/graphdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18124 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/applications/layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14032 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/applications/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36391 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/applications/vags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15117 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/applications/van.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23416 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/applications/vqes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/asciiart.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:42:14.865526 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/backends/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    57621 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/backends/abstract_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/backends/backend_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14928 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/backends/cupy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24925 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/backends/jax_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4024 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/backends/jax_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/backends/numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24148 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/backends/pytorch_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3825 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/backends/pytorch_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35980 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/backends/tensorflow_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3377 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/backends/tf_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34020 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/basecircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28637 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/channels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36220 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/circuit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:42:14.865526 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/cloud/
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14582 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/cloud/abstraction.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17866 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/cloud/apis.py
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/cloud/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2265 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/cloud/local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2613 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/cloud/quafu_provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14325 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/cloud/tencent.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/cloud/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11518 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/cloud/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:42:14.865526 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/compiler/
+-rw-r--r--   0 runner    (1001) docker     (122)      241 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3258 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/compiler/composed_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6032 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/compiler/qiskit_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9595 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/compiler/simple_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29573 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/cons.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/densitymatrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17639 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29016 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/gates.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:42:14.865526 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)      545 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/interfaces/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/interfaces/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3355 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/interfaces/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10364 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/interfaces/tensortrans.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5117 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/interfaces/torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10126 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/keras.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15399 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/mps_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34519 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/mpscircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11861 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/noisemodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    82850 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/quantum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:42:14.865526 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/results/
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3435 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/results/counts.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:42:14.865526 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/results/qem/
+-rw-r--r--   0 runner    (1001) docker     (122)      419 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/results/qem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3056 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/results/qem/benchmark_circuits.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11852 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/results/qem/qem_methods.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31362 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/results/readout_mitigation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/simplify.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:42:14.865526 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/templates/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/templates/chems.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/templates/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5811 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/templates/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3934 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/templates/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10942 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/templates/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4621 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/torchnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27335 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/translation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7060 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:42:14.869526 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    24257 2023-06-08 12:42:14.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3706 2023-06-08 12:42:14.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-08 12:42:14.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-06-08 12:42:14.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-08 12:42:14.000000 tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:42:14.869526 tensorcircuit-nightly-0.9.1.dev20230608/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33735 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tests/test_calibrating.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11237 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tests/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    47707 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tests/test_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5606 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tests/test_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3419 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tests/test_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17232 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tests/test_dmcircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tests/test_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tests/test_gates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13220 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tests/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tests/test_keras.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7445 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tests/test_miscs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10552 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tests/test_mpscircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5637 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tests/test_noisemodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)      753 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tests/test_qaoa.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4304 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tests/test_qem.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16823 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tests/test_quantum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tests/test_quantum_attr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11050 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tests/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2823 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tests/test_torchnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-06-08 12:16:45.000000 tensorcircuit-nightly-0.9.1.dev20230608/tests/test_van.py
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/CHANGELOG.md` & `tensorcircuit-nightly-0.9.1.dev20230608/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 
 - introduce two stage compiling for `batch_expectation_ps` to save some compiling overhead
 
 - Add experimental support for ODE backend pulse level control simulation/analog quantum computing
 
 - make the pulse level control support differentiating the end time
 
+- Add new qem module with qem methods: zne, dd and rc
+
 ### Fixed
 
 - `tc.results.counts.plot_histogram` now can dispatch kws to corresponding qiskit method
 
 - New implementation for `c.inverse()` to partially avoid unrecognized gate name issue
 
 - Fixed bug for `batch_expectation_ps` for jax backend
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/HISTORY.md` & `tensorcircuit-nightly-0.9.1.dev20230608/HISTORY.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/LICENSE` & `tensorcircuit-nightly-0.9.1.dev20230608/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/PKG-INFO` & `tensorcircuit-nightly-0.9.1.dev20230608/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorcircuit-nightly
-Version: 0.9.1.dev20230607
+Version: 0.9.1.dev20230608
 Summary: nightly release for tensorcircuit
 Home-page: https://github.com/refraction-ray/tensorcircuit-dev
 Author: TensorCircuit Authors
 Author-email: znfesnpbh.tc@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
@@ -125,14 +125,64 @@
         
         - Elegance
         
           - Flexibility: customized contraction, multiple ML backend/interface choices, multiple dtype precisions, multiple QPU providers
         
           - API design: quantum for humans, less code, more power
         
+        - Batteries included
+        
+          <details>
+          <summary> Tons of amazing features and built in tools for research (click for details) </summary>
+        
+          - Support **super large circuit simulation** using tensor network engine.
+        
+          - Support **noisy simulation** with both Monte Carlo and density matrix (tensor network powered) modes.
+        
+          - Support **approximate simulation** with MPS-TEBD modes.
+        
+          - Support **analog/digital hybrid simulation** (time dependent Hamiltonian evolution, **pulse** level simulation) with neural ode modes.
+        
+          - Support **qudits simulation**.
+        
+          - Highly customizable **noise model** with gate error and scalable readout error.
+        
+          - Support for **non-unitary** gate and post-selection simulation.
+        
+          - Support **real quantum devices access** from different providers.
+        
+          - **Scalable readout error mitigation** native to both bitstring and expectation level with automatic qubit mapping consideration.
+        
+          - **Advanced quantum error mitigation methods** and pipelines such as ZNE, DD, RC, etc.
+        
+          - Support **MPS/MPO** as representations for input states, quantum gates and observables to be measured.
+        
+          - Support **vectorized parallelism** on circuit inputs, circuit parameters, circuit structures, circuit measurements and these vectorization can be nested.
+        
+          - Gradients can be obtained with both **automatic differenation** and parameter shift (vmap accelerated) modes.
+        
+          - **Machine learning interface/layer/model** abstraction in both TensorFlow and PyTorch for both numerical simulation and real QPU experiments.
+        
+          - Circuit sampling supports both final state sampling and perfect sampling from tensor networks.
+        
+          - Light cone reduction support for local expectation calculation.
+        
+          - Highly customizable tensor network contraction path finder with opteinsum interface.
+        
+          - Observables are supported in measurement, sparse matrix, dense matrix and MPO format.
+        
+          - Super fast weighted sum Pauli string Hamiltonian matrix generation.
+        
+          - Reusable common circuit/measurement/problem templates and patterns.
+        
+          - SOTA quantum algorithm and model implementations.
+        
+          - Support hybrid workflows and pipelines with CPU/GPU/QPU hardware from local/cloud/hpc resources using tf/torch/jax/cupy/numpy frameoworks all at the same time.
+        
+          </details>
         
         ## Contributing
         
         ### Status
         
         This project is released by [Tencent Quantum Lab](https://quantum.tencent.com/) and is created and maintained by [Shi-Xin Zhang](https://github.com/refraction-ray) with current core authors [Shi-Xin Zhang](https://github.com/refraction-ray) and [Yu-Qin Chen](https://github.com/yutuer21). We also thank [contributions](https://github.com/tencent-quantum-lab/tensorcircuit/graphs/contributors) from the lab and the open source community.
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/README.md` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit_nightly.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,242 +1,309 @@
-<p align="center">
-  <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
-    <img width=90% src="docs/source/statics/logov2.jpg">
-  </a>
-</p>
-
-<p align="center">
-  <!-- tests (GitHub actions) -->
-  <a href="https://github.com/tencent-quantum-lab/tensorcircuit/actions/workflows/ci.yml">
-    <img src="https://img.shields.io/github/actions/workflow/status/tencent-quantum-lab/tensorcircuit/ci.yml?branch=master" />
-  </a>
-  <!-- docs -->
-  <a href="https://tensorcircuit.readthedocs.io/">
-    <img src="https://img.shields.io/badge/docs-link-green.svg?logo=read-the-docs"/>
-  </a>
-  <!-- PyPI -->
-  <a href="https://pypi.org/project/tensorcircuit/">
-    <img src="https://img.shields.io/pypi/v/tensorcircuit.svg?logo=pypi"/>
-  </a>
-  <!-- binder -->
-  <a href="https://mybinder.org/v2/gh/refraction-ray/tc-env/master?urlpath=git-pull%3Frepo%3Dhttps%253A%252F%252Fgithub.com%252Ftencent-quantum-lab%252Ftensorcircuit%26urlpath%3Dlab%252Ftree%252Ftensorcircuit%252F%26branch%3Dmaster">
-    <img src="https://mybinder.org/badge_logo.svg"/>
-  </a>
-  <!-- License -->
-  <a href="./LICENSE">
-    <img src="https://img.shields.io/badge/license-Apache%202.0-blue.svg?logo=apache"/>
-  </a>
-</p>
-
-<p align="center"> English | <a href="README_cn.md"> 简体中文 </a></p>
-
-TensorCircuit is the next generation of quantum software framework with support for automatic differentiation, just-in-time compiling, hardware acceleration, and vectorized parallelism.
-
-TensorCircuit is built on top of modern machine learning frameworks: Jax, TensorFlow, and PyTorch. It is specifically suitable for highly efficient simulations of quantum-classical hybrid paradigm and variational quantum algorithms in ideal, noisy and approximate cases. It also supports real quantum hardware access and provides CPU/GPU/QPU hybrid deployment solutions since v0.9.
-
-## Getting Started
-
-Please begin with [Quick Start](/docs/source/quickstart.rst) in the [full documentation](https://tensorcircuit.readthedocs.io/).
-
-For more information on software usage, sota algorithm implementation and engineer paradigm demonstration, please refer to 60+ [example scripts](/examples) and 30+ [tutorial notebooks](https://tensorcircuit.readthedocs.io/en/latest/#tutorials). API docstrings and test cases in [tests](/tests) are also informative.
-
-The following are some minimal demos.
-
-- Circuit manipulation:
-
-```python
-import tensorcircuit as tc
-c = tc.Circuit(2)
-c.H(0)
-c.CNOT(0,1)
-c.rx(1, theta=0.2)
-print(c.wavefunction())
-print(c.expectation_ps(z=[0, 1]))
-print(c.sample(allow_state=True, batch=1024, format="count_dict_bin"))
-```
-
-- Runtime behavior customization:
-
-```python
-tc.set_backend("tensorflow")
-tc.set_dtype("complex128")
-tc.set_contractor("greedy")
-```
-
-- Automatic differentiations with jit:
-
-```python
-def forward(theta):
-    c = tc.Circuit(2)
-    c.R(0, theta=theta, alpha=0.5, phi=0.8)
-    return tc.backend.real(c.expectation((tc.gates.z(), [0])))
-
-g = tc.backend.grad(forward)
-g = tc.backend.jit(g)
-theta = tc.array_to_tensor(1.0)
-print(g(theta))
-```
-
-## Install
-
-The package is written in pure Python and can be obtained via pip as:
-
-```python
-pip install tensorcircuit
-```
-
-We recommend you install this package with tensorflow also installed as:
-
-```python
-pip install tensorcircuit[tensorflow]
-```
-
-Other optional dependencies include `[torch]`, `[jax]`, `[qiskit]` and `[cloud]`.
-
-For the nightly build of tensorcircuit with new features, try:
-
-```python
-pip uninstall tensorcircuit
-pip install tensorcircuit-nightly
-```
-
-We also have [Docker support](/docker).
-
-## Advantages
-
-- Tensor network simulation engine based
-
-- JIT, AD, vectorized parallelism compatible
-
-- GPU support, quantum device access support, hybrid deployment support
-
-- Efficiency
-
-  - Time: 10 to 10^6+ times acceleration compared to TensorFlow Quantum, Pennylane or Qiskit
-
-  - Space: 600+ qubits 1D VQE workflow (converged energy inaccuracy: < 1%)
-
-- Elegance
-
-  - Flexibility: customized contraction, multiple ML backend/interface choices, multiple dtype precisions, multiple QPU providers
-
-  - API design: quantum for humans, less code, more power
-
-
-## Contributing
-
-### Status
-
-This project is released by [Tencent Quantum Lab](https://quantum.tencent.com/) and is created and maintained by [Shi-Xin Zhang](https://github.com/refraction-ray) with current core authors [Shi-Xin Zhang](https://github.com/refraction-ray) and [Yu-Qin Chen](https://github.com/yutuer21). We also thank [contributions](https://github.com/tencent-quantum-lab/tensorcircuit/graphs/contributors) from the lab and the open source community.
-
-### Citation
-
-If this project helps in your research, please cite our software whitepaper published in Quantum:
-
-[TensorCircuit: a Quantum Software Framework for the NISQ Era](https://quantum-journal.org/papers/q-2023-02-02-912/)
-
-which is also a good introduction to the software.
-
-### Guidelines
-
-For contribution guidelines and notes, see [CONTRIBUTING](/CONTRIBUTING.md).
-
-We welcome [issues](https://github.com/tencent-quantum-lab/tensorcircuit/issues), [PRs](https://github.com/tencent-quantum-lab/tensorcircuit/pulls), and [discussions](https://github.com/tencent-quantum-lab/tensorcircuit/discussions) from everyone, and these are all hosted on GitHub.
-
-### License
-
-TensorCircuit is open source, released under the Apache License, Version 2.0.
-
-### Contributors
-
-<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
-<!-- prettier-ignore-start -->
-<!-- markdownlint-disable -->
-<table>
-  <tbody>
-    <tr>
-      <td align="center" valign="top" width="16.66%"><a href="https://re-ra.xyz"><img src="https://avatars.githubusercontent.com/u/35157286?v=4?s=100" width="100px;" alt="Shixin Zhang"/><br /><sub><b>Shixin Zhang</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=refraction-ray" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=refraction-ray" title="Documentation">📖</a> <a href="#example-refraction-ray" title="Examples">💡</a> <a href="#ideas-refraction-ray" title="Ideas, Planning, & Feedback">🤔</a> <a href="#infra-refraction-ray" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#maintenance-refraction-ray" title="Maintenance">🚧</a> <a href="#research-refraction-ray" title="Research">🔬</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/pulls?q=is%3Apr+reviewed-by%3Arefraction-ray" title="Reviewed Pull Requests">👀</a> <a href="#translation-refraction-ray" title="Translation">🌍</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=refraction-ray" title="Tests">⚠️</a> <a href="#tutorial-refraction-ray" title="Tutorials">✅</a> <a href="#talk-refraction-ray" title="Talks">📢</a> <a href="#question-refraction-ray" title="Answering Questions">💬</a></td>
-      <td align="center" valign="top" width="16.66%"><a href="https://github.com/yutuer21"><img src="https://avatars.githubusercontent.com/u/83822724?v=4?s=100" width="100px;" alt="Yuqin Chen"/><br /><sub><b>Yuqin Chen</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=yutuer21" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=yutuer21" title="Documentation">📖</a> <a href="#example-yutuer21" title="Examples">💡</a> <a href="#ideas-yutuer21" title="Ideas, Planning, & Feedback">🤔</a> <a href="#research-yutuer21" title="Research">🔬</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=yutuer21" title="Tests">⚠️</a> <a href="#tutorial-yutuer21" title="Tutorials">✅</a> <a href="#talk-yutuer21" title="Talks">📢</a></td>
-      <td align="center" valign="top" width="16.66%"><a href="http://jiezhongqiu.com"><img src="https://avatars.githubusercontent.com/u/3853009?v=4?s=100" width="100px;" alt="Jiezhong Qiu"/><br /><sub><b>Jiezhong Qiu</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=xptree" title="Code">💻</a> <a href="#example-xptree" title="Examples">💡</a> <a href="#ideas-xptree" title="Ideas, Planning, & Feedback">🤔</a> <a href="#research-xptree" title="Research">🔬</a></td>
-      <td align="center" valign="top" width="16.66%"><a href="http://liwt31.github.io"><img src="https://avatars.githubusercontent.com/u/22628546?v=4?s=100" width="100px;" alt="Weitang Li"/><br /><sub><b>Weitang Li</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=liwt31" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=liwt31" title="Documentation">📖</a> <a href="#ideas-liwt31" title="Ideas, Planning, & Feedback">🤔</a> <a href="#research-liwt31" title="Research">🔬</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=liwt31" title="Tests">⚠️</a> <a href="#talk-liwt31" title="Talks">📢</a></td>
-      <td align="center" valign="top" width="16.66%"><a href="https://github.com/SUSYUSTC"><img src="https://avatars.githubusercontent.com/u/30529122?v=4?s=100" width="100px;" alt="Jiace Sun"/><br /><sub><b>Jiace Sun</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=SUSYUSTC" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=SUSYUSTC" title="Documentation">📖</a> <a href="#example-SUSYUSTC" title="Examples">💡</a> <a href="#ideas-SUSYUSTC" title="Ideas, Planning, & Feedback">🤔</a> <a href="#research-SUSYUSTC" title="Research">🔬</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=SUSYUSTC" title="Tests">⚠️</a></td>
-      <td align="center" valign="top" width="16.66%"><a href="https://github.com/Zhouquan-Wan"><img src="https://avatars.githubusercontent.com/u/54523490?v=4?s=100" width="100px;" alt="Zhouquan Wan"/><br /><sub><b>Zhouquan Wan</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=Zhouquan-Wan" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=Zhouquan-Wan" title="Documentation">📖</a> <a href="#example-Zhouquan-Wan" title="Examples">💡</a> <a href="#ideas-Zhouquan-Wan" title="Ideas, Planning, & Feedback">🤔</a> <a href="#research-Zhouquan-Wan" title="Research">🔬</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=Zhouquan-Wan" title="Tests">⚠️</a> <a href="#tutorial-Zhouquan-Wan" title="Tutorials">✅</a></td>
-    </tr>
-    <tr>
-      <td align="center" valign="top" width="16.66%"><a href="https://github.com/ls-iastu"><img src="https://avatars.githubusercontent.com/u/70554346?v=4?s=100" width="100px;" alt="Shuo Liu"/><br /><sub><b>Shuo Liu</b></sub></a><br /><a href="#example-ls-iastu" title="Examples">💡</a> <a href="#research-ls-iastu" title="Research">🔬</a> <a href="#tutorial-ls-iastu" title="Tutorials">✅</a></td>
-      <td align="center" valign="top" width="16.66%"><a href="https://github.com/YHPeter"><img src="https://avatars.githubusercontent.com/u/44126839?v=4?s=100" width="100px;" alt="Hao Yu"/><br /><sub><b>Hao Yu</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=YHPeter" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=YHPeter" title="Documentation">📖</a> <a href="#infra-YHPeter" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=YHPeter" title="Tests">⚠️</a> <a href="#tutorial-YHPeter" title="Tutorials">✅</a></td>
-      <td align="center" valign="top" width="16.66%"><a href="https://github.com/SexyCarrots"><img src="https://avatars.githubusercontent.com/u/63588721?v=4?s=100" width="100px;" alt="Xinghan Yang"/><br /><sub><b>Xinghan Yang</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=SexyCarrots" title="Documentation">📖</a> <a href="#translation-SexyCarrots" title="Translation">🌍</a> <a href="#tutorial-SexyCarrots" title="Tutorials">✅</a></td>
-      <td align="center" valign="top" width="16.66%"><a href="https://github.com/JachyMeow"><img src="https://avatars.githubusercontent.com/u/114171061?v=4?s=100" width="100px;" alt="JachyMeow"/><br /><sub><b>JachyMeow</b></sub></a><br /><a href="#tutorial-JachyMeow" title="Tutorials">✅</a> <a href="#translation-JachyMeow" title="Translation">🌍</a></td>
-      <td align="center" valign="top" width="16.66%"><a href="https://github.com/Mzye21"><img src="https://avatars.githubusercontent.com/u/86239031?v=4?s=100" width="100px;" alt="Zhaofeng Ye"/><br /><sub><b>Zhaofeng Ye</b></sub></a><br /><a href="#design-Mzye21" title="Design">🎨</a></td>
-      <td align="center" valign="top" width="16.66%"><a href="https://github.com/erertertet"><img src="https://avatars.githubusercontent.com/u/41342153?v=4?s=100" width="100px;" alt="erertertet"/><br /><sub><b>erertertet</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=erertertet" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=erertertet" title="Documentation">📖</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=erertertet" title="Tests">⚠️</a></td>
-    </tr>
-    <tr>
-      <td align="center" valign="top" width="16.66%"><a href="https://github.com/yicongzheng"><img src="https://avatars.githubusercontent.com/u/107173985?v=4?s=100" width="100px;" alt="Yicong Zheng"/><br /><sub><b>Yicong Zheng</b></sub></a><br /><a href="#tutorial-yicongzheng" title="Tutorials">✅</a></td>
-      <td align="center" valign="top" width="16.66%"><a href="https://marksong.tech"><img src="https://avatars.githubusercontent.com/u/78847784?v=4?s=100" width="100px;" alt="Zixuan Song"/><br /><sub><b>Zixuan Song</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=MarkSong535" title="Documentation">📖</a> <a href="#translation-MarkSong535" title="Translation">🌍</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=MarkSong535" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=MarkSong535" title="Tests">⚠️</a></td>
-      <td align="center" valign="top" width="16.66%"><a href="https://github.com/buwantaiji"><img src="https://avatars.githubusercontent.com/u/25216189?v=4?s=100" width="100px;" alt="Hao Xie"/><br /><sub><b>Hao Xie</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=buwantaiji" title="Documentation">📖</a></td>
-      <td align="center" valign="top" width="16.66%"><a href="https://github.com/pramitsingh0"><img src="https://avatars.githubusercontent.com/u/52959209?v=4?s=100" width="100px;" alt="Pramit Singh"/><br /><sub><b>Pramit Singh</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=pramitsingh0" title="Tests">⚠️</a></td>
-      <td align="center" valign="top" width="16.66%"><a href="https://github.com/JAllcock"><img src="https://avatars.githubusercontent.com/u/26302022?v=4?s=100" width="100px;" alt="Jonathan Allcock"/><br /><sub><b>Jonathan Allcock</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=JAllcock" title="Documentation">📖</a> <a href="#ideas-JAllcock" title="Ideas, Planning, & Feedback">🤔</a> <a href="#talk-JAllcock" title="Talks">📢</a></td>
-      <td align="center" valign="top" width="16.66%"><a href="https://github.com/nealchen2003"><img src="https://avatars.githubusercontent.com/u/45502551?v=4?s=100" width="100px;" alt="nealchen2003"/><br /><sub><b>nealchen2003</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=nealchen2003" title="Documentation">📖</a></td>
-    </tr>
-    <tr>
-      <td align="center" valign="top" width="16.66%"><a href="https://github.com/eurethia"><img src="https://avatars.githubusercontent.com/u/84611606?v=4?s=100" width="100px;" alt="隐公观鱼"/><br /><sub><b>隐公观鱼</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=eurethia" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=eurethia" title="Tests">⚠️</a></td>
-      <td align="center" valign="top" width="16.66%"><a href="https://github.com/WiuYuan"><img src="https://avatars.githubusercontent.com/u/108848998?v=4?s=100" width="100px;" alt="WiuYuan"/><br /><sub><b>WiuYuan</b></sub></a><br /><a href="#example-WiuYuan" title="Examples">💡</a></td>
-      <td align="center" valign="top" width="16.66%"><a href="https://www.linkedin.com/in/felix-xu-16a153196/"><img src="https://avatars.githubusercontent.com/u/61252303?v=4?s=100" width="100px;" alt="Felix Xu"/><br /><sub><b>Felix Xu</b></sub></a><br /><a href="#tutorial-FelixXu35" title="Tutorials">✅</a></td>
-    </tr>
-  </tbody>
-</table>
-
-<!-- markdownlint-restore -->
-<!-- prettier-ignore-end -->
-
-<!-- ALL-CONTRIBUTORS-LIST:END -->
-<!-- prettier-ignore-start -->
-<!-- markdownlint-disable -->
-
-<!-- markdownlint-restore -->
-<!-- prettier-ignore-end -->
-
-<!-- ALL-CONTRIBUTORS-LIST:END -->
-
-## Research and Applications
-
-### DQAS
-
-For the application of Differentiable Quantum Architecture Search, see [applications](/tensorcircuit/applications).
-
-Reference paper: https://arxiv.org/abs/2010.08561 (published in QST).
-
-### VQNHE
-
-For the application of Variational Quantum-Neural Hybrid Eigensolver, see [applications](/tensorcircuit/applications).
-
-Reference paper: https://arxiv.org/abs/2106.05105 (published in PRL) and https://arxiv.org/abs/2112.10380.
-
-### VQEX-MBL
-
-For the application of VQEX on MBL phase identification, see the [tutorial](/docs/source/tutorials/vqex_mbl.ipynb).
-
-Reference paper: https://arxiv.org/abs/2111.13719 (published in PRB).
-
-### Stark-DTC
-
-For the numerical demosntration of discrete time crystal enabled by Stark many-body localization, see the Floquet simulation [demo](/examples/timeevolution_trotter.py).
-
-Reference paper: https://arxiv.org/abs/2208.02866 (published in PRL).
-
-### RA-Training
-
-For the numerical simulation of variational quantum algorithm training using random gate activation strategy by us, see the [project repo](https://github.com/ls-iastu/RAtraining).
-
-Reference paper: https://arxiv.org/abs/2303.08154.
-
-### TenCirChem
-
-[TenCirChem](https://github.com/tencent-quantum-lab/TenCirChem) is an efficient and versatile quantum computation package for molecular properties. TenCirChem is based on TensorCircuit and is optimized for chemistry applications.
-
-Reference paper: https://arxiv.org/abs/2303.10825.
-
-### EMQAOA-DARBO
-
-For the numerical simulation and hardware experiments with error mitigation on QAOA, see the [project repo](https://github.com/sherrylixuecheng/EMQAOA-DARBO).
-
-Reference paper: https://arxiv.org/abs/2303.14877.
+Metadata-Version: 2.1
+Name: tensorcircuit-nightly
+Version: 0.9.1.dev20230608
+Summary: nightly release for tensorcircuit
+Home-page: https://github.com/refraction-ray/tensorcircuit-dev
+Author: TensorCircuit Authors
+Author-email: znfesnpbh.tc@gmail.com
+License: UNKNOWN
+Description: <p align="center">
+          <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
+            <img width=90% src="docs/source/statics/logov2.jpg">
+          </a>
+        </p>
+        
+        <p align="center">
+          <!-- tests (GitHub actions) -->
+          <a href="https://github.com/tencent-quantum-lab/tensorcircuit/actions/workflows/ci.yml">
+            <img src="https://img.shields.io/github/actions/workflow/status/tencent-quantum-lab/tensorcircuit/ci.yml?branch=master" />
+          </a>
+          <!-- docs -->
+          <a href="https://tensorcircuit.readthedocs.io/">
+            <img src="https://img.shields.io/badge/docs-link-green.svg?logo=read-the-docs"/>
+          </a>
+          <!-- PyPI -->
+          <a href="https://pypi.org/project/tensorcircuit/">
+            <img src="https://img.shields.io/pypi/v/tensorcircuit.svg?logo=pypi"/>
+          </a>
+          <!-- binder -->
+          <a href="https://mybinder.org/v2/gh/refraction-ray/tc-env/master?urlpath=git-pull%3Frepo%3Dhttps%253A%252F%252Fgithub.com%252Ftencent-quantum-lab%252Ftensorcircuit%26urlpath%3Dlab%252Ftree%252Ftensorcircuit%252F%26branch%3Dmaster">
+            <img src="https://mybinder.org/badge_logo.svg"/>
+          </a>
+          <!-- License -->
+          <a href="./LICENSE">
+            <img src="https://img.shields.io/badge/license-Apache%202.0-blue.svg?logo=apache"/>
+          </a>
+        </p>
+        
+        <p align="center"> English | <a href="README_cn.md"> 简体中文 </a></p>
+        
+        TensorCircuit is the next generation of quantum software framework with support for automatic differentiation, just-in-time compiling, hardware acceleration, and vectorized parallelism.
+        
+        TensorCircuit is built on top of modern machine learning frameworks: Jax, TensorFlow, and PyTorch. It is specifically suitable for highly efficient simulations of quantum-classical hybrid paradigm and variational quantum algorithms in ideal, noisy and approximate cases. It also supports real quantum hardware access and provides CPU/GPU/QPU hybrid deployment solutions since v0.9.
+        
+        ## Getting Started
+        
+        Please begin with [Quick Start](/docs/source/quickstart.rst) in the [full documentation](https://tensorcircuit.readthedocs.io/).
+        
+        For more information on software usage, sota algorithm implementation and engineer paradigm demonstration, please refer to 60+ [example scripts](/examples) and 30+ [tutorial notebooks](https://tensorcircuit.readthedocs.io/en/latest/#tutorials). API docstrings and test cases in [tests](/tests) are also informative.
+        
+        The following are some minimal demos.
+        
+        - Circuit manipulation:
+        
+        ```python
+        import tensorcircuit as tc
+        c = tc.Circuit(2)
+        c.H(0)
+        c.CNOT(0,1)
+        c.rx(1, theta=0.2)
+        print(c.wavefunction())
+        print(c.expectation_ps(z=[0, 1]))
+        print(c.sample(allow_state=True, batch=1024, format="count_dict_bin"))
+        ```
+        
+        - Runtime behavior customization:
+        
+        ```python
+        tc.set_backend("tensorflow")
+        tc.set_dtype("complex128")
+        tc.set_contractor("greedy")
+        ```
+        
+        - Automatic differentiations with jit:
+        
+        ```python
+        def forward(theta):
+            c = tc.Circuit(2)
+            c.R(0, theta=theta, alpha=0.5, phi=0.8)
+            return tc.backend.real(c.expectation((tc.gates.z(), [0])))
+        
+        g = tc.backend.grad(forward)
+        g = tc.backend.jit(g)
+        theta = tc.array_to_tensor(1.0)
+        print(g(theta))
+        ```
+        
+        ## Install
+        
+        The package is written in pure Python and can be obtained via pip as:
+        
+        ```python
+        pip install tensorcircuit
+        ```
+        
+        We recommend you install this package with tensorflow also installed as:
+        
+        ```python
+        pip install tensorcircuit[tensorflow]
+        ```
+        
+        Other optional dependencies include `[torch]`, `[jax]`, `[qiskit]` and `[cloud]`.
+        
+        For the nightly build of tensorcircuit with new features, try:
+        
+        ```python
+        pip uninstall tensorcircuit
+        pip install tensorcircuit-nightly
+        ```
+        
+        We also have [Docker support](/docker).
+        
+        ## Advantages
+        
+        - Tensor network simulation engine based
+        
+        - JIT, AD, vectorized parallelism compatible
+        
+        - GPU support, quantum device access support, hybrid deployment support
+        
+        - Efficiency
+        
+          - Time: 10 to 10^6+ times acceleration compared to TensorFlow Quantum, Pennylane or Qiskit
+        
+          - Space: 600+ qubits 1D VQE workflow (converged energy inaccuracy: < 1%)
+        
+        - Elegance
+        
+          - Flexibility: customized contraction, multiple ML backend/interface choices, multiple dtype precisions, multiple QPU providers
+        
+          - API design: quantum for humans, less code, more power
+        
+        - Batteries included
+        
+          <details>
+          <summary> Tons of amazing features and built in tools for research (click for details) </summary>
+        
+          - Support **super large circuit simulation** using tensor network engine.
+        
+          - Support **noisy simulation** with both Monte Carlo and density matrix (tensor network powered) modes.
+        
+          - Support **approximate simulation** with MPS-TEBD modes.
+        
+          - Support **analog/digital hybrid simulation** (time dependent Hamiltonian evolution, **pulse** level simulation) with neural ode modes.
+        
+          - Support **qudits simulation**.
+        
+          - Highly customizable **noise model** with gate error and scalable readout error.
+        
+          - Support for **non-unitary** gate and post-selection simulation.
+        
+          - Support **real quantum devices access** from different providers.
+        
+          - **Scalable readout error mitigation** native to both bitstring and expectation level with automatic qubit mapping consideration.
+        
+          - **Advanced quantum error mitigation methods** and pipelines such as ZNE, DD, RC, etc.
+        
+          - Support **MPS/MPO** as representations for input states, quantum gates and observables to be measured.
+        
+          - Support **vectorized parallelism** on circuit inputs, circuit parameters, circuit structures, circuit measurements and these vectorization can be nested.
+        
+          - Gradients can be obtained with both **automatic differenation** and parameter shift (vmap accelerated) modes.
+        
+          - **Machine learning interface/layer/model** abstraction in both TensorFlow and PyTorch for both numerical simulation and real QPU experiments.
+        
+          - Circuit sampling supports both final state sampling and perfect sampling from tensor networks.
+        
+          - Light cone reduction support for local expectation calculation.
+        
+          - Highly customizable tensor network contraction path finder with opteinsum interface.
+        
+          - Observables are supported in measurement, sparse matrix, dense matrix and MPO format.
+        
+          - Super fast weighted sum Pauli string Hamiltonian matrix generation.
+        
+          - Reusable common circuit/measurement/problem templates and patterns.
+        
+          - SOTA quantum algorithm and model implementations.
+        
+          - Support hybrid workflows and pipelines with CPU/GPU/QPU hardware from local/cloud/hpc resources using tf/torch/jax/cupy/numpy frameoworks all at the same time.
+        
+          </details>
+        
+        ## Contributing
+        
+        ### Status
+        
+        This project is released by [Tencent Quantum Lab](https://quantum.tencent.com/) and is created and maintained by [Shi-Xin Zhang](https://github.com/refraction-ray) with current core authors [Shi-Xin Zhang](https://github.com/refraction-ray) and [Yu-Qin Chen](https://github.com/yutuer21). We also thank [contributions](https://github.com/tencent-quantum-lab/tensorcircuit/graphs/contributors) from the lab and the open source community.
+        
+        ### Citation
+        
+        If this project helps in your research, please cite our software whitepaper published in Quantum:
+        
+        [TensorCircuit: a Quantum Software Framework for the NISQ Era](https://quantum-journal.org/papers/q-2023-02-02-912/)
+        
+        which is also a good introduction to the software.
+        
+        ### Guidelines
+        
+        For contribution guidelines and notes, see [CONTRIBUTING](/CONTRIBUTING.md).
+        
+        We welcome [issues](https://github.com/tencent-quantum-lab/tensorcircuit/issues), [PRs](https://github.com/tencent-quantum-lab/tensorcircuit/pulls), and [discussions](https://github.com/tencent-quantum-lab/tensorcircuit/discussions) from everyone, and these are all hosted on GitHub.
+        
+        ### License
+        
+        TensorCircuit is open source, released under the Apache License, Version 2.0.
+        
+        ### Contributors
+        
+        <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+        <!-- prettier-ignore-start -->
+        <!-- markdownlint-disable -->
+        <table>
+          <tbody>
+            <tr>
+              <td align="center" valign="top" width="16.66%"><a href="https://re-ra.xyz"><img src="https://avatars.githubusercontent.com/u/35157286?v=4?s=100" width="100px;" alt="Shixin Zhang"/><br /><sub><b>Shixin Zhang</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=refraction-ray" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=refraction-ray" title="Documentation">📖</a> <a href="#example-refraction-ray" title="Examples">💡</a> <a href="#ideas-refraction-ray" title="Ideas, Planning, & Feedback">🤔</a> <a href="#infra-refraction-ray" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#maintenance-refraction-ray" title="Maintenance">🚧</a> <a href="#research-refraction-ray" title="Research">🔬</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/pulls?q=is%3Apr+reviewed-by%3Arefraction-ray" title="Reviewed Pull Requests">👀</a> <a href="#translation-refraction-ray" title="Translation">🌍</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=refraction-ray" title="Tests">⚠️</a> <a href="#tutorial-refraction-ray" title="Tutorials">✅</a> <a href="#talk-refraction-ray" title="Talks">📢</a> <a href="#question-refraction-ray" title="Answering Questions">💬</a></td>
+              <td align="center" valign="top" width="16.66%"><a href="https://github.com/yutuer21"><img src="https://avatars.githubusercontent.com/u/83822724?v=4?s=100" width="100px;" alt="Yuqin Chen"/><br /><sub><b>Yuqin Chen</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=yutuer21" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=yutuer21" title="Documentation">📖</a> <a href="#example-yutuer21" title="Examples">💡</a> <a href="#ideas-yutuer21" title="Ideas, Planning, & Feedback">🤔</a> <a href="#research-yutuer21" title="Research">🔬</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=yutuer21" title="Tests">⚠️</a> <a href="#tutorial-yutuer21" title="Tutorials">✅</a> <a href="#talk-yutuer21" title="Talks">📢</a></td>
+              <td align="center" valign="top" width="16.66%"><a href="http://jiezhongqiu.com"><img src="https://avatars.githubusercontent.com/u/3853009?v=4?s=100" width="100px;" alt="Jiezhong Qiu"/><br /><sub><b>Jiezhong Qiu</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=xptree" title="Code">💻</a> <a href="#example-xptree" title="Examples">💡</a> <a href="#ideas-xptree" title="Ideas, Planning, & Feedback">🤔</a> <a href="#research-xptree" title="Research">🔬</a></td>
+              <td align="center" valign="top" width="16.66%"><a href="http://liwt31.github.io"><img src="https://avatars.githubusercontent.com/u/22628546?v=4?s=100" width="100px;" alt="Weitang Li"/><br /><sub><b>Weitang Li</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=liwt31" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=liwt31" title="Documentation">📖</a> <a href="#ideas-liwt31" title="Ideas, Planning, & Feedback">🤔</a> <a href="#research-liwt31" title="Research">🔬</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=liwt31" title="Tests">⚠️</a> <a href="#talk-liwt31" title="Talks">📢</a></td>
+              <td align="center" valign="top" width="16.66%"><a href="https://github.com/SUSYUSTC"><img src="https://avatars.githubusercontent.com/u/30529122?v=4?s=100" width="100px;" alt="Jiace Sun"/><br /><sub><b>Jiace Sun</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=SUSYUSTC" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=SUSYUSTC" title="Documentation">📖</a> <a href="#example-SUSYUSTC" title="Examples">💡</a> <a href="#ideas-SUSYUSTC" title="Ideas, Planning, & Feedback">🤔</a> <a href="#research-SUSYUSTC" title="Research">🔬</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=SUSYUSTC" title="Tests">⚠️</a></td>
+              <td align="center" valign="top" width="16.66%"><a href="https://github.com/Zhouquan-Wan"><img src="https://avatars.githubusercontent.com/u/54523490?v=4?s=100" width="100px;" alt="Zhouquan Wan"/><br /><sub><b>Zhouquan Wan</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=Zhouquan-Wan" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=Zhouquan-Wan" title="Documentation">📖</a> <a href="#example-Zhouquan-Wan" title="Examples">💡</a> <a href="#ideas-Zhouquan-Wan" title="Ideas, Planning, & Feedback">🤔</a> <a href="#research-Zhouquan-Wan" title="Research">🔬</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=Zhouquan-Wan" title="Tests">⚠️</a> <a href="#tutorial-Zhouquan-Wan" title="Tutorials">✅</a></td>
+            </tr>
+            <tr>
+              <td align="center" valign="top" width="16.66%"><a href="https://github.com/ls-iastu"><img src="https://avatars.githubusercontent.com/u/70554346?v=4?s=100" width="100px;" alt="Shuo Liu"/><br /><sub><b>Shuo Liu</b></sub></a><br /><a href="#example-ls-iastu" title="Examples">💡</a> <a href="#research-ls-iastu" title="Research">🔬</a> <a href="#tutorial-ls-iastu" title="Tutorials">✅</a></td>
+              <td align="center" valign="top" width="16.66%"><a href="https://github.com/YHPeter"><img src="https://avatars.githubusercontent.com/u/44126839?v=4?s=100" width="100px;" alt="Hao Yu"/><br /><sub><b>Hao Yu</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=YHPeter" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=YHPeter" title="Documentation">📖</a> <a href="#infra-YHPeter" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=YHPeter" title="Tests">⚠️</a> <a href="#tutorial-YHPeter" title="Tutorials">✅</a></td>
+              <td align="center" valign="top" width="16.66%"><a href="https://github.com/SexyCarrots"><img src="https://avatars.githubusercontent.com/u/63588721?v=4?s=100" width="100px;" alt="Xinghan Yang"/><br /><sub><b>Xinghan Yang</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=SexyCarrots" title="Documentation">📖</a> <a href="#translation-SexyCarrots" title="Translation">🌍</a> <a href="#tutorial-SexyCarrots" title="Tutorials">✅</a></td>
+              <td align="center" valign="top" width="16.66%"><a href="https://github.com/JachyMeow"><img src="https://avatars.githubusercontent.com/u/114171061?v=4?s=100" width="100px;" alt="JachyMeow"/><br /><sub><b>JachyMeow</b></sub></a><br /><a href="#tutorial-JachyMeow" title="Tutorials">✅</a> <a href="#translation-JachyMeow" title="Translation">🌍</a></td>
+              <td align="center" valign="top" width="16.66%"><a href="https://github.com/Mzye21"><img src="https://avatars.githubusercontent.com/u/86239031?v=4?s=100" width="100px;" alt="Zhaofeng Ye"/><br /><sub><b>Zhaofeng Ye</b></sub></a><br /><a href="#design-Mzye21" title="Design">🎨</a></td>
+              <td align="center" valign="top" width="16.66%"><a href="https://github.com/erertertet"><img src="https://avatars.githubusercontent.com/u/41342153?v=4?s=100" width="100px;" alt="erertertet"/><br /><sub><b>erertertet</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=erertertet" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=erertertet" title="Documentation">📖</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=erertertet" title="Tests">⚠️</a></td>
+            </tr>
+            <tr>
+              <td align="center" valign="top" width="16.66%"><a href="https://github.com/yicongzheng"><img src="https://avatars.githubusercontent.com/u/107173985?v=4?s=100" width="100px;" alt="Yicong Zheng"/><br /><sub><b>Yicong Zheng</b></sub></a><br /><a href="#tutorial-yicongzheng" title="Tutorials">✅</a></td>
+              <td align="center" valign="top" width="16.66%"><a href="https://marksong.tech"><img src="https://avatars.githubusercontent.com/u/78847784?v=4?s=100" width="100px;" alt="Zixuan Song"/><br /><sub><b>Zixuan Song</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=MarkSong535" title="Documentation">📖</a> <a href="#translation-MarkSong535" title="Translation">🌍</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=MarkSong535" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=MarkSong535" title="Tests">⚠️</a></td>
+              <td align="center" valign="top" width="16.66%"><a href="https://github.com/buwantaiji"><img src="https://avatars.githubusercontent.com/u/25216189?v=4?s=100" width="100px;" alt="Hao Xie"/><br /><sub><b>Hao Xie</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=buwantaiji" title="Documentation">📖</a></td>
+              <td align="center" valign="top" width="16.66%"><a href="https://github.com/pramitsingh0"><img src="https://avatars.githubusercontent.com/u/52959209?v=4?s=100" width="100px;" alt="Pramit Singh"/><br /><sub><b>Pramit Singh</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=pramitsingh0" title="Tests">⚠️</a></td>
+              <td align="center" valign="top" width="16.66%"><a href="https://github.com/JAllcock"><img src="https://avatars.githubusercontent.com/u/26302022?v=4?s=100" width="100px;" alt="Jonathan Allcock"/><br /><sub><b>Jonathan Allcock</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=JAllcock" title="Documentation">📖</a> <a href="#ideas-JAllcock" title="Ideas, Planning, & Feedback">🤔</a> <a href="#talk-JAllcock" title="Talks">📢</a></td>
+              <td align="center" valign="top" width="16.66%"><a href="https://github.com/nealchen2003"><img src="https://avatars.githubusercontent.com/u/45502551?v=4?s=100" width="100px;" alt="nealchen2003"/><br /><sub><b>nealchen2003</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=nealchen2003" title="Documentation">📖</a></td>
+            </tr>
+            <tr>
+              <td align="center" valign="top" width="16.66%"><a href="https://github.com/eurethia"><img src="https://avatars.githubusercontent.com/u/84611606?v=4?s=100" width="100px;" alt="隐公观鱼"/><br /><sub><b>隐公观鱼</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=eurethia" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=eurethia" title="Tests">⚠️</a></td>
+              <td align="center" valign="top" width="16.66%"><a href="https://github.com/WiuYuan"><img src="https://avatars.githubusercontent.com/u/108848998?v=4?s=100" width="100px;" alt="WiuYuan"/><br /><sub><b>WiuYuan</b></sub></a><br /><a href="#example-WiuYuan" title="Examples">💡</a></td>
+              <td align="center" valign="top" width="16.66%"><a href="https://www.linkedin.com/in/felix-xu-16a153196/"><img src="https://avatars.githubusercontent.com/u/61252303?v=4?s=100" width="100px;" alt="Felix Xu"/><br /><sub><b>Felix Xu</b></sub></a><br /><a href="#tutorial-FelixXu35" title="Tutorials">✅</a></td>
+            </tr>
+          </tbody>
+        </table>
+        
+        <!-- markdownlint-restore -->
+        <!-- prettier-ignore-end -->
+        
+        <!-- ALL-CONTRIBUTORS-LIST:END -->
+        <!-- prettier-ignore-start -->
+        <!-- markdownlint-disable -->
+        
+        <!-- markdownlint-restore -->
+        <!-- prettier-ignore-end -->
+        
+        <!-- ALL-CONTRIBUTORS-LIST:END -->
+        
+        ## Research and Applications
+        
+        ### DQAS
+        
+        For the application of Differentiable Quantum Architecture Search, see [applications](/tensorcircuit/applications).
+        
+        Reference paper: https://arxiv.org/abs/2010.08561 (published in QST).
+        
+        ### VQNHE
+        
+        For the application of Variational Quantum-Neural Hybrid Eigensolver, see [applications](/tensorcircuit/applications).
+        
+        Reference paper: https://arxiv.org/abs/2106.05105 (published in PRL) and https://arxiv.org/abs/2112.10380.
+        
+        ### VQEX-MBL
+        
+        For the application of VQEX on MBL phase identification, see the [tutorial](/docs/source/tutorials/vqex_mbl.ipynb).
+        
+        Reference paper: https://arxiv.org/abs/2111.13719 (published in PRB).
+        
+        ### Stark-DTC
+        
+        For the numerical demosntration of discrete time crystal enabled by Stark many-body localization, see the Floquet simulation [demo](/examples/timeevolution_trotter.py).
+        
+        Reference paper: https://arxiv.org/abs/2208.02866 (published in PRL).
+        
+        ### RA-Training
+        
+        For the numerical simulation of variational quantum algorithm training using random gate activation strategy by us, see the [project repo](https://github.com/ls-iastu/RAtraining).
+        
+        Reference paper: https://arxiv.org/abs/2303.08154.
+        
+        ### TenCirChem
+        
+        [TenCirChem](https://github.com/tencent-quantum-lab/TenCirChem) is an efficient and versatile quantum computation package for molecular properties. TenCirChem is based on TensorCircuit and is optimized for chemistry applications.
+        
+        Reference paper: https://arxiv.org/abs/2303.10825.
+        
+        ### EMQAOA-DARBO
+        
+        For the numerical simulation and hardware experiments with error mitigation on QAOA, see the [project repo](https://github.com/sherrylixuecheng/EMQAOA-DARBO).
+        
+        Reference paper: https://arxiv.org/abs/2303.14877.
+        
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+Provides-Extra: tensorflow
+Provides-Extra: jax
+Provides-Extra: torch
+Provides-Extra: qiskit
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/README_cn.md` & `tensorcircuit-nightly-0.9.1.dev20230608/README_cn.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/docs/source/advance.rst` & `tensorcircuit-nightly-0.9.1.dev20230608/docs/source/advance.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/docs/source/cnconf.py` & `tensorcircuit-nightly-0.9.1.dev20230608/docs/source/cnconf.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/docs/source/conf.py` & `tensorcircuit-nightly-0.9.1.dev20230608/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/docs/source/contribution.rst` & `tensorcircuit-nightly-0.9.1.dev20230608/docs/source/contribution.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/docs/source/faq.rst` & `tensorcircuit-nightly-0.9.1.dev20230608/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/docs/source/index.rst` & `tensorcircuit-nightly-0.9.1.dev20230608/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/docs/source/infras.rst` & `tensorcircuit-nightly-0.9.1.dev20230608/docs/source/infras.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/docs/source/modules.rst` & `tensorcircuit-nightly-0.9.1.dev20230608/docs/source/modules.rst.backup`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/docs/source/quickstart.rst` & `tensorcircuit-nightly-0.9.1.dev20230608/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/docs/source/sharpbits.rst` & `tensorcircuit-nightly-0.9.1.dev20230608/docs/source/sharpbits.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/docs/source/tutorial.rst` & `tensorcircuit-nightly-0.9.1.dev20230608/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/docs/source/tutorial_cn.rst` & `tensorcircuit-nightly-0.9.1.dev20230608/docs/source/tutorial_cn.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/docs/source/whitepapertoc_cn.rst` & `tensorcircuit-nightly-0.9.1.dev20230608/docs/source/whitepapertoc_cn.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/setup.py` & `tensorcircuit-nightly-0.9.1.dev20230608/setup.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/__init__.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.9.1.dev20230607"
+__version__ = "0.9.1.dev20230608"
 __author__ = "TensorCircuit Authors"
 __creator__ = "refraction-ray"
 
 from .utils import gpu_memory_share
 
 gpu_memory_share()
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/about.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/about.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/abstractcircuit.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/abstractcircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/applications/dqas.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/applications/dqas.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/applications/graphdata.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/applications/graphdata.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/applications/layers.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/applications/layers.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/applications/utils.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/applications/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/applications/vags.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/applications/vags.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/applications/van.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/applications/van.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/applications/vqes.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/applications/vqes.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/asciiart.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/asciiart.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/backends/abstract_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/backends/abstract_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/backends/backend_factory.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/backends/backend_factory.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/backends/cupy_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/backends/cupy_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/backends/jax_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/backends/jax_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/backends/jax_ops.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/backends/jax_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/backends/numpy_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/backends/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/backends/pytorch_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/backends/pytorch_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/backends/pytorch_ops.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/backends/pytorch_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/backends/tensorflow_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/backends/tensorflow_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/backends/tf_ops.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/backends/tf_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/basecircuit.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/basecircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/channels.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/channels.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/circuit.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/circuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/cloud/abstraction.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/cloud/abstraction.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/cloud/apis.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/cloud/apis.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/cloud/local.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/cloud/local.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/cloud/quafu_provider.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/cloud/quafu_provider.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/cloud/tencent.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/cloud/tencent.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/cloud/utils.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/cloud/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/cloud/wrapper.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/cloud/wrapper.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/compiler/composed_compiler.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/compiler/composed_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/compiler/qiskit_compiler.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/compiler/qiskit_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/compiler/simple_compiler.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/compiler/simple_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/cons.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/cons.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/densitymatrix.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/densitymatrix.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/experimental.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/experimental.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/gates.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/gates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/interfaces/__init__.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/interfaces/numpy.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/interfaces/numpy.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/interfaces/scipy.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/interfaces/scipy.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/interfaces/tensorflow.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/interfaces/tensorflow.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/interfaces/tensortrans.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/interfaces/tensortrans.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/interfaces/torch.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/interfaces/torch.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/keras.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/keras.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/mps_base.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/mps_base.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/mpscircuit.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/mpscircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/noisemodel.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/noisemodel.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/quantum.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/quantum.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/results/counts.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/results/counts.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/results/readout_mitigation.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/results/readout_mitigation.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/simplify.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/simplify.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/templates/blocks.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/templates/blocks.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/templates/chems.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/templates/chems.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/templates/dataset.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/templates/dataset.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/templates/ensemble.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/templates/ensemble.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/templates/graphs.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/templates/graphs.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/templates/measurements.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/templates/measurements.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/torchnn.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/torchnn.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/translation.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/translation.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/utils.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit/vis.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit/vis.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit_nightly.egg-info/PKG-INFO` & `tensorcircuit-nightly-0.9.1.dev20230608/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,259 +1,292 @@
-Metadata-Version: 2.1
-Name: tensorcircuit-nightly
-Version: 0.9.1.dev20230607
-Summary: nightly release for tensorcircuit
-Home-page: https://github.com/refraction-ray/tensorcircuit-dev
-Author: TensorCircuit Authors
-Author-email: znfesnpbh.tc@gmail.com
-License: UNKNOWN
-Description: <p align="center">
-          <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
-            <img width=90% src="docs/source/statics/logov2.jpg">
-          </a>
-        </p>
-        
-        <p align="center">
-          <!-- tests (GitHub actions) -->
-          <a href="https://github.com/tencent-quantum-lab/tensorcircuit/actions/workflows/ci.yml">
-            <img src="https://img.shields.io/github/actions/workflow/status/tencent-quantum-lab/tensorcircuit/ci.yml?branch=master" />
-          </a>
-          <!-- docs -->
-          <a href="https://tensorcircuit.readthedocs.io/">
-            <img src="https://img.shields.io/badge/docs-link-green.svg?logo=read-the-docs"/>
-          </a>
-          <!-- PyPI -->
-          <a href="https://pypi.org/project/tensorcircuit/">
-            <img src="https://img.shields.io/pypi/v/tensorcircuit.svg?logo=pypi"/>
-          </a>
-          <!-- binder -->
-          <a href="https://mybinder.org/v2/gh/refraction-ray/tc-env/master?urlpath=git-pull%3Frepo%3Dhttps%253A%252F%252Fgithub.com%252Ftencent-quantum-lab%252Ftensorcircuit%26urlpath%3Dlab%252Ftree%252Ftensorcircuit%252F%26branch%3Dmaster">
-            <img src="https://mybinder.org/badge_logo.svg"/>
-          </a>
-          <!-- License -->
-          <a href="./LICENSE">
-            <img src="https://img.shields.io/badge/license-Apache%202.0-blue.svg?logo=apache"/>
-          </a>
-        </p>
-        
-        <p align="center"> English | <a href="README_cn.md"> 简体中文 </a></p>
-        
-        TensorCircuit is the next generation of quantum software framework with support for automatic differentiation, just-in-time compiling, hardware acceleration, and vectorized parallelism.
-        
-        TensorCircuit is built on top of modern machine learning frameworks: Jax, TensorFlow, and PyTorch. It is specifically suitable for highly efficient simulations of quantum-classical hybrid paradigm and variational quantum algorithms in ideal, noisy and approximate cases. It also supports real quantum hardware access and provides CPU/GPU/QPU hybrid deployment solutions since v0.9.
-        
-        ## Getting Started
-        
-        Please begin with [Quick Start](/docs/source/quickstart.rst) in the [full documentation](https://tensorcircuit.readthedocs.io/).
-        
-        For more information on software usage, sota algorithm implementation and engineer paradigm demonstration, please refer to 60+ [example scripts](/examples) and 30+ [tutorial notebooks](https://tensorcircuit.readthedocs.io/en/latest/#tutorials). API docstrings and test cases in [tests](/tests) are also informative.
-        
-        The following are some minimal demos.
-        
-        - Circuit manipulation:
-        
-        ```python
-        import tensorcircuit as tc
-        c = tc.Circuit(2)
-        c.H(0)
-        c.CNOT(0,1)
-        c.rx(1, theta=0.2)
-        print(c.wavefunction())
-        print(c.expectation_ps(z=[0, 1]))
-        print(c.sample(allow_state=True, batch=1024, format="count_dict_bin"))
-        ```
-        
-        - Runtime behavior customization:
-        
-        ```python
-        tc.set_backend("tensorflow")
-        tc.set_dtype("complex128")
-        tc.set_contractor("greedy")
-        ```
-        
-        - Automatic differentiations with jit:
-        
-        ```python
-        def forward(theta):
-            c = tc.Circuit(2)
-            c.R(0, theta=theta, alpha=0.5, phi=0.8)
-            return tc.backend.real(c.expectation((tc.gates.z(), [0])))
-        
-        g = tc.backend.grad(forward)
-        g = tc.backend.jit(g)
-        theta = tc.array_to_tensor(1.0)
-        print(g(theta))
-        ```
-        
-        ## Install
-        
-        The package is written in pure Python and can be obtained via pip as:
-        
-        ```python
-        pip install tensorcircuit
-        ```
-        
-        We recommend you install this package with tensorflow also installed as:
-        
-        ```python
-        pip install tensorcircuit[tensorflow]
-        ```
-        
-        Other optional dependencies include `[torch]`, `[jax]`, `[qiskit]` and `[cloud]`.
-        
-        For the nightly build of tensorcircuit with new features, try:
-        
-        ```python
-        pip uninstall tensorcircuit
-        pip install tensorcircuit-nightly
-        ```
-        
-        We also have [Docker support](/docker).
-        
-        ## Advantages
-        
-        - Tensor network simulation engine based
-        
-        - JIT, AD, vectorized parallelism compatible
-        
-        - GPU support, quantum device access support, hybrid deployment support
-        
-        - Efficiency
-        
-          - Time: 10 to 10^6+ times acceleration compared to TensorFlow Quantum, Pennylane or Qiskit
-        
-          - Space: 600+ qubits 1D VQE workflow (converged energy inaccuracy: < 1%)
-        
-        - Elegance
-        
-          - Flexibility: customized contraction, multiple ML backend/interface choices, multiple dtype precisions, multiple QPU providers
-        
-          - API design: quantum for humans, less code, more power
-        
-        
-        ## Contributing
-        
-        ### Status
-        
-        This project is released by [Tencent Quantum Lab](https://quantum.tencent.com/) and is created and maintained by [Shi-Xin Zhang](https://github.com/refraction-ray) with current core authors [Shi-Xin Zhang](https://github.com/refraction-ray) and [Yu-Qin Chen](https://github.com/yutuer21). We also thank [contributions](https://github.com/tencent-quantum-lab/tensorcircuit/graphs/contributors) from the lab and the open source community.
-        
-        ### Citation
-        
-        If this project helps in your research, please cite our software whitepaper published in Quantum:
-        
-        [TensorCircuit: a Quantum Software Framework for the NISQ Era](https://quantum-journal.org/papers/q-2023-02-02-912/)
-        
-        which is also a good introduction to the software.
-        
-        ### Guidelines
-        
-        For contribution guidelines and notes, see [CONTRIBUTING](/CONTRIBUTING.md).
-        
-        We welcome [issues](https://github.com/tencent-quantum-lab/tensorcircuit/issues), [PRs](https://github.com/tencent-quantum-lab/tensorcircuit/pulls), and [discussions](https://github.com/tencent-quantum-lab/tensorcircuit/discussions) from everyone, and these are all hosted on GitHub.
-        
-        ### License
-        
-        TensorCircuit is open source, released under the Apache License, Version 2.0.
-        
-        ### Contributors
-        
-        <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
-        <!-- prettier-ignore-start -->
-        <!-- markdownlint-disable -->
-        <table>
-          <tbody>
-            <tr>
-              <td align="center" valign="top" width="16.66%"><a href="https://re-ra.xyz"><img src="https://avatars.githubusercontent.com/u/35157286?v=4?s=100" width="100px;" alt="Shixin Zhang"/><br /><sub><b>Shixin Zhang</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=refraction-ray" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=refraction-ray" title="Documentation">📖</a> <a href="#example-refraction-ray" title="Examples">💡</a> <a href="#ideas-refraction-ray" title="Ideas, Planning, & Feedback">🤔</a> <a href="#infra-refraction-ray" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#maintenance-refraction-ray" title="Maintenance">🚧</a> <a href="#research-refraction-ray" title="Research">🔬</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/pulls?q=is%3Apr+reviewed-by%3Arefraction-ray" title="Reviewed Pull Requests">👀</a> <a href="#translation-refraction-ray" title="Translation">🌍</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=refraction-ray" title="Tests">⚠️</a> <a href="#tutorial-refraction-ray" title="Tutorials">✅</a> <a href="#talk-refraction-ray" title="Talks">📢</a> <a href="#question-refraction-ray" title="Answering Questions">💬</a></td>
-              <td align="center" valign="top" width="16.66%"><a href="https://github.com/yutuer21"><img src="https://avatars.githubusercontent.com/u/83822724?v=4?s=100" width="100px;" alt="Yuqin Chen"/><br /><sub><b>Yuqin Chen</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=yutuer21" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=yutuer21" title="Documentation">📖</a> <a href="#example-yutuer21" title="Examples">💡</a> <a href="#ideas-yutuer21" title="Ideas, Planning, & Feedback">🤔</a> <a href="#research-yutuer21" title="Research">🔬</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=yutuer21" title="Tests">⚠️</a> <a href="#tutorial-yutuer21" title="Tutorials">✅</a> <a href="#talk-yutuer21" title="Talks">📢</a></td>
-              <td align="center" valign="top" width="16.66%"><a href="http://jiezhongqiu.com"><img src="https://avatars.githubusercontent.com/u/3853009?v=4?s=100" width="100px;" alt="Jiezhong Qiu"/><br /><sub><b>Jiezhong Qiu</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=xptree" title="Code">💻</a> <a href="#example-xptree" title="Examples">💡</a> <a href="#ideas-xptree" title="Ideas, Planning, & Feedback">🤔</a> <a href="#research-xptree" title="Research">🔬</a></td>
-              <td align="center" valign="top" width="16.66%"><a href="http://liwt31.github.io"><img src="https://avatars.githubusercontent.com/u/22628546?v=4?s=100" width="100px;" alt="Weitang Li"/><br /><sub><b>Weitang Li</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=liwt31" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=liwt31" title="Documentation">📖</a> <a href="#ideas-liwt31" title="Ideas, Planning, & Feedback">🤔</a> <a href="#research-liwt31" title="Research">🔬</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=liwt31" title="Tests">⚠️</a> <a href="#talk-liwt31" title="Talks">📢</a></td>
-              <td align="center" valign="top" width="16.66%"><a href="https://github.com/SUSYUSTC"><img src="https://avatars.githubusercontent.com/u/30529122?v=4?s=100" width="100px;" alt="Jiace Sun"/><br /><sub><b>Jiace Sun</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=SUSYUSTC" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=SUSYUSTC" title="Documentation">📖</a> <a href="#example-SUSYUSTC" title="Examples">💡</a> <a href="#ideas-SUSYUSTC" title="Ideas, Planning, & Feedback">🤔</a> <a href="#research-SUSYUSTC" title="Research">🔬</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=SUSYUSTC" title="Tests">⚠️</a></td>
-              <td align="center" valign="top" width="16.66%"><a href="https://github.com/Zhouquan-Wan"><img src="https://avatars.githubusercontent.com/u/54523490?v=4?s=100" width="100px;" alt="Zhouquan Wan"/><br /><sub><b>Zhouquan Wan</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=Zhouquan-Wan" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=Zhouquan-Wan" title="Documentation">📖</a> <a href="#example-Zhouquan-Wan" title="Examples">💡</a> <a href="#ideas-Zhouquan-Wan" title="Ideas, Planning, & Feedback">🤔</a> <a href="#research-Zhouquan-Wan" title="Research">🔬</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=Zhouquan-Wan" title="Tests">⚠️</a> <a href="#tutorial-Zhouquan-Wan" title="Tutorials">✅</a></td>
-            </tr>
-            <tr>
-              <td align="center" valign="top" width="16.66%"><a href="https://github.com/ls-iastu"><img src="https://avatars.githubusercontent.com/u/70554346?v=4?s=100" width="100px;" alt="Shuo Liu"/><br /><sub><b>Shuo Liu</b></sub></a><br /><a href="#example-ls-iastu" title="Examples">💡</a> <a href="#research-ls-iastu" title="Research">🔬</a> <a href="#tutorial-ls-iastu" title="Tutorials">✅</a></td>
-              <td align="center" valign="top" width="16.66%"><a href="https://github.com/YHPeter"><img src="https://avatars.githubusercontent.com/u/44126839?v=4?s=100" width="100px;" alt="Hao Yu"/><br /><sub><b>Hao Yu</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=YHPeter" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=YHPeter" title="Documentation">📖</a> <a href="#infra-YHPeter" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=YHPeter" title="Tests">⚠️</a> <a href="#tutorial-YHPeter" title="Tutorials">✅</a></td>
-              <td align="center" valign="top" width="16.66%"><a href="https://github.com/SexyCarrots"><img src="https://avatars.githubusercontent.com/u/63588721?v=4?s=100" width="100px;" alt="Xinghan Yang"/><br /><sub><b>Xinghan Yang</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=SexyCarrots" title="Documentation">📖</a> <a href="#translation-SexyCarrots" title="Translation">🌍</a> <a href="#tutorial-SexyCarrots" title="Tutorials">✅</a></td>
-              <td align="center" valign="top" width="16.66%"><a href="https://github.com/JachyMeow"><img src="https://avatars.githubusercontent.com/u/114171061?v=4?s=100" width="100px;" alt="JachyMeow"/><br /><sub><b>JachyMeow</b></sub></a><br /><a href="#tutorial-JachyMeow" title="Tutorials">✅</a> <a href="#translation-JachyMeow" title="Translation">🌍</a></td>
-              <td align="center" valign="top" width="16.66%"><a href="https://github.com/Mzye21"><img src="https://avatars.githubusercontent.com/u/86239031?v=4?s=100" width="100px;" alt="Zhaofeng Ye"/><br /><sub><b>Zhaofeng Ye</b></sub></a><br /><a href="#design-Mzye21" title="Design">🎨</a></td>
-              <td align="center" valign="top" width="16.66%"><a href="https://github.com/erertertet"><img src="https://avatars.githubusercontent.com/u/41342153?v=4?s=100" width="100px;" alt="erertertet"/><br /><sub><b>erertertet</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=erertertet" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=erertertet" title="Documentation">📖</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=erertertet" title="Tests">⚠️</a></td>
-            </tr>
-            <tr>
-              <td align="center" valign="top" width="16.66%"><a href="https://github.com/yicongzheng"><img src="https://avatars.githubusercontent.com/u/107173985?v=4?s=100" width="100px;" alt="Yicong Zheng"/><br /><sub><b>Yicong Zheng</b></sub></a><br /><a href="#tutorial-yicongzheng" title="Tutorials">✅</a></td>
-              <td align="center" valign="top" width="16.66%"><a href="https://marksong.tech"><img src="https://avatars.githubusercontent.com/u/78847784?v=4?s=100" width="100px;" alt="Zixuan Song"/><br /><sub><b>Zixuan Song</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=MarkSong535" title="Documentation">📖</a> <a href="#translation-MarkSong535" title="Translation">🌍</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=MarkSong535" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=MarkSong535" title="Tests">⚠️</a></td>
-              <td align="center" valign="top" width="16.66%"><a href="https://github.com/buwantaiji"><img src="https://avatars.githubusercontent.com/u/25216189?v=4?s=100" width="100px;" alt="Hao Xie"/><br /><sub><b>Hao Xie</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=buwantaiji" title="Documentation">📖</a></td>
-              <td align="center" valign="top" width="16.66%"><a href="https://github.com/pramitsingh0"><img src="https://avatars.githubusercontent.com/u/52959209?v=4?s=100" width="100px;" alt="Pramit Singh"/><br /><sub><b>Pramit Singh</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=pramitsingh0" title="Tests">⚠️</a></td>
-              <td align="center" valign="top" width="16.66%"><a href="https://github.com/JAllcock"><img src="https://avatars.githubusercontent.com/u/26302022?v=4?s=100" width="100px;" alt="Jonathan Allcock"/><br /><sub><b>Jonathan Allcock</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=JAllcock" title="Documentation">📖</a> <a href="#ideas-JAllcock" title="Ideas, Planning, & Feedback">🤔</a> <a href="#talk-JAllcock" title="Talks">📢</a></td>
-              <td align="center" valign="top" width="16.66%"><a href="https://github.com/nealchen2003"><img src="https://avatars.githubusercontent.com/u/45502551?v=4?s=100" width="100px;" alt="nealchen2003"/><br /><sub><b>nealchen2003</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=nealchen2003" title="Documentation">📖</a></td>
-            </tr>
-            <tr>
-              <td align="center" valign="top" width="16.66%"><a href="https://github.com/eurethia"><img src="https://avatars.githubusercontent.com/u/84611606?v=4?s=100" width="100px;" alt="隐公观鱼"/><br /><sub><b>隐公观鱼</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=eurethia" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=eurethia" title="Tests">⚠️</a></td>
-              <td align="center" valign="top" width="16.66%"><a href="https://github.com/WiuYuan"><img src="https://avatars.githubusercontent.com/u/108848998?v=4?s=100" width="100px;" alt="WiuYuan"/><br /><sub><b>WiuYuan</b></sub></a><br /><a href="#example-WiuYuan" title="Examples">💡</a></td>
-              <td align="center" valign="top" width="16.66%"><a href="https://www.linkedin.com/in/felix-xu-16a153196/"><img src="https://avatars.githubusercontent.com/u/61252303?v=4?s=100" width="100px;" alt="Felix Xu"/><br /><sub><b>Felix Xu</b></sub></a><br /><a href="#tutorial-FelixXu35" title="Tutorials">✅</a></td>
-            </tr>
-          </tbody>
-        </table>
-        
-        <!-- markdownlint-restore -->
-        <!-- prettier-ignore-end -->
-        
-        <!-- ALL-CONTRIBUTORS-LIST:END -->
-        <!-- prettier-ignore-start -->
-        <!-- markdownlint-disable -->
-        
-        <!-- markdownlint-restore -->
-        <!-- prettier-ignore-end -->
-        
-        <!-- ALL-CONTRIBUTORS-LIST:END -->
-        
-        ## Research and Applications
-        
-        ### DQAS
-        
-        For the application of Differentiable Quantum Architecture Search, see [applications](/tensorcircuit/applications).
-        
-        Reference paper: https://arxiv.org/abs/2010.08561 (published in QST).
-        
-        ### VQNHE
-        
-        For the application of Variational Quantum-Neural Hybrid Eigensolver, see [applications](/tensorcircuit/applications).
-        
-        Reference paper: https://arxiv.org/abs/2106.05105 (published in PRL) and https://arxiv.org/abs/2112.10380.
-        
-        ### VQEX-MBL
-        
-        For the application of VQEX on MBL phase identification, see the [tutorial](/docs/source/tutorials/vqex_mbl.ipynb).
-        
-        Reference paper: https://arxiv.org/abs/2111.13719 (published in PRB).
-        
-        ### Stark-DTC
-        
-        For the numerical demosntration of discrete time crystal enabled by Stark many-body localization, see the Floquet simulation [demo](/examples/timeevolution_trotter.py).
-        
-        Reference paper: https://arxiv.org/abs/2208.02866 (published in PRL).
-        
-        ### RA-Training
-        
-        For the numerical simulation of variational quantum algorithm training using random gate activation strategy by us, see the [project repo](https://github.com/ls-iastu/RAtraining).
-        
-        Reference paper: https://arxiv.org/abs/2303.08154.
-        
-        ### TenCirChem
-        
-        [TenCirChem](https://github.com/tencent-quantum-lab/TenCirChem) is an efficient and versatile quantum computation package for molecular properties. TenCirChem is based on TensorCircuit and is optimized for chemistry applications.
-        
-        Reference paper: https://arxiv.org/abs/2303.10825.
-        
-        ### EMQAOA-DARBO
-        
-        For the numerical simulation and hardware experiments with error mitigation on QAOA, see the [project repo](https://github.com/sherrylixuecheng/EMQAOA-DARBO).
-        
-        Reference paper: https://arxiv.org/abs/2303.14877.
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-Provides-Extra: tensorflow
-Provides-Extra: jax
-Provides-Extra: torch
-Provides-Extra: qiskit
+<p align="center">
+  <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
+    <img width=90% src="docs/source/statics/logov2.jpg">
+  </a>
+</p>
+
+<p align="center">
+  <!-- tests (GitHub actions) -->
+  <a href="https://github.com/tencent-quantum-lab/tensorcircuit/actions/workflows/ci.yml">
+    <img src="https://img.shields.io/github/actions/workflow/status/tencent-quantum-lab/tensorcircuit/ci.yml?branch=master" />
+  </a>
+  <!-- docs -->
+  <a href="https://tensorcircuit.readthedocs.io/">
+    <img src="https://img.shields.io/badge/docs-link-green.svg?logo=read-the-docs"/>
+  </a>
+  <!-- PyPI -->
+  <a href="https://pypi.org/project/tensorcircuit/">
+    <img src="https://img.shields.io/pypi/v/tensorcircuit.svg?logo=pypi"/>
+  </a>
+  <!-- binder -->
+  <a href="https://mybinder.org/v2/gh/refraction-ray/tc-env/master?urlpath=git-pull%3Frepo%3Dhttps%253A%252F%252Fgithub.com%252Ftencent-quantum-lab%252Ftensorcircuit%26urlpath%3Dlab%252Ftree%252Ftensorcircuit%252F%26branch%3Dmaster">
+    <img src="https://mybinder.org/badge_logo.svg"/>
+  </a>
+  <!-- License -->
+  <a href="./LICENSE">
+    <img src="https://img.shields.io/badge/license-Apache%202.0-blue.svg?logo=apache"/>
+  </a>
+</p>
+
+<p align="center"> English | <a href="README_cn.md"> 简体中文 </a></p>
+
+TensorCircuit is the next generation of quantum software framework with support for automatic differentiation, just-in-time compiling, hardware acceleration, and vectorized parallelism.
+
+TensorCircuit is built on top of modern machine learning frameworks: Jax, TensorFlow, and PyTorch. It is specifically suitable for highly efficient simulations of quantum-classical hybrid paradigm and variational quantum algorithms in ideal, noisy and approximate cases. It also supports real quantum hardware access and provides CPU/GPU/QPU hybrid deployment solutions since v0.9.
+
+## Getting Started
+
+Please begin with [Quick Start](/docs/source/quickstart.rst) in the [full documentation](https://tensorcircuit.readthedocs.io/).
+
+For more information on software usage, sota algorithm implementation and engineer paradigm demonstration, please refer to 60+ [example scripts](/examples) and 30+ [tutorial notebooks](https://tensorcircuit.readthedocs.io/en/latest/#tutorials). API docstrings and test cases in [tests](/tests) are also informative.
+
+The following are some minimal demos.
+
+- Circuit manipulation:
+
+```python
+import tensorcircuit as tc
+c = tc.Circuit(2)
+c.H(0)
+c.CNOT(0,1)
+c.rx(1, theta=0.2)
+print(c.wavefunction())
+print(c.expectation_ps(z=[0, 1]))
+print(c.sample(allow_state=True, batch=1024, format="count_dict_bin"))
+```
+
+- Runtime behavior customization:
+
+```python
+tc.set_backend("tensorflow")
+tc.set_dtype("complex128")
+tc.set_contractor("greedy")
+```
+
+- Automatic differentiations with jit:
+
+```python
+def forward(theta):
+    c = tc.Circuit(2)
+    c.R(0, theta=theta, alpha=0.5, phi=0.8)
+    return tc.backend.real(c.expectation((tc.gates.z(), [0])))
+
+g = tc.backend.grad(forward)
+g = tc.backend.jit(g)
+theta = tc.array_to_tensor(1.0)
+print(g(theta))
+```
+
+## Install
+
+The package is written in pure Python and can be obtained via pip as:
+
+```python
+pip install tensorcircuit
+```
+
+We recommend you install this package with tensorflow also installed as:
+
+```python
+pip install tensorcircuit[tensorflow]
+```
+
+Other optional dependencies include `[torch]`, `[jax]`, `[qiskit]` and `[cloud]`.
+
+For the nightly build of tensorcircuit with new features, try:
+
+```python
+pip uninstall tensorcircuit
+pip install tensorcircuit-nightly
+```
+
+We also have [Docker support](/docker).
+
+## Advantages
+
+- Tensor network simulation engine based
+
+- JIT, AD, vectorized parallelism compatible
+
+- GPU support, quantum device access support, hybrid deployment support
+
+- Efficiency
+
+  - Time: 10 to 10^6+ times acceleration compared to TensorFlow Quantum, Pennylane or Qiskit
+
+  - Space: 600+ qubits 1D VQE workflow (converged energy inaccuracy: < 1%)
+
+- Elegance
+
+  - Flexibility: customized contraction, multiple ML backend/interface choices, multiple dtype precisions, multiple QPU providers
+
+  - API design: quantum for humans, less code, more power
+
+- Batteries included
+
+  <details>
+  <summary> Tons of amazing features and built in tools for research (click for details) </summary>
+
+  - Support **super large circuit simulation** using tensor network engine.
+
+  - Support **noisy simulation** with both Monte Carlo and density matrix (tensor network powered) modes.
+
+  - Support **approximate simulation** with MPS-TEBD modes.
+
+  - Support **analog/digital hybrid simulation** (time dependent Hamiltonian evolution, **pulse** level simulation) with neural ode modes.
+
+  - Support **qudits simulation**.
+
+  - Highly customizable **noise model** with gate error and scalable readout error.
+
+  - Support for **non-unitary** gate and post-selection simulation.
+
+  - Support **real quantum devices access** from different providers.
+
+  - **Scalable readout error mitigation** native to both bitstring and expectation level with automatic qubit mapping consideration.
+
+  - **Advanced quantum error mitigation methods** and pipelines such as ZNE, DD, RC, etc.
+
+  - Support **MPS/MPO** as representations for input states, quantum gates and observables to be measured.
+
+  - Support **vectorized parallelism** on circuit inputs, circuit parameters, circuit structures, circuit measurements and these vectorization can be nested.
+
+  - Gradients can be obtained with both **automatic differenation** and parameter shift (vmap accelerated) modes.
+
+  - **Machine learning interface/layer/model** abstraction in both TensorFlow and PyTorch for both numerical simulation and real QPU experiments.
+
+  - Circuit sampling supports both final state sampling and perfect sampling from tensor networks.
+
+  - Light cone reduction support for local expectation calculation.
+
+  - Highly customizable tensor network contraction path finder with opteinsum interface.
+
+  - Observables are supported in measurement, sparse matrix, dense matrix and MPO format.
+
+  - Super fast weighted sum Pauli string Hamiltonian matrix generation.
+
+  - Reusable common circuit/measurement/problem templates and patterns.
+
+  - SOTA quantum algorithm and model implementations.
+
+  - Support hybrid workflows and pipelines with CPU/GPU/QPU hardware from local/cloud/hpc resources using tf/torch/jax/cupy/numpy frameoworks all at the same time.
+
+  </details>
+
+## Contributing
+
+### Status
+
+This project is released by [Tencent Quantum Lab](https://quantum.tencent.com/) and is created and maintained by [Shi-Xin Zhang](https://github.com/refraction-ray) with current core authors [Shi-Xin Zhang](https://github.com/refraction-ray) and [Yu-Qin Chen](https://github.com/yutuer21). We also thank [contributions](https://github.com/tencent-quantum-lab/tensorcircuit/graphs/contributors) from the lab and the open source community.
+
+### Citation
+
+If this project helps in your research, please cite our software whitepaper published in Quantum:
+
+[TensorCircuit: a Quantum Software Framework for the NISQ Era](https://quantum-journal.org/papers/q-2023-02-02-912/)
+
+which is also a good introduction to the software.
+
+### Guidelines
+
+For contribution guidelines and notes, see [CONTRIBUTING](/CONTRIBUTING.md).
+
+We welcome [issues](https://github.com/tencent-quantum-lab/tensorcircuit/issues), [PRs](https://github.com/tencent-quantum-lab/tensorcircuit/pulls), and [discussions](https://github.com/tencent-quantum-lab/tensorcircuit/discussions) from everyone, and these are all hosted on GitHub.
+
+### License
+
+TensorCircuit is open source, released under the Apache License, Version 2.0.
+
+### Contributors
+
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+<table>
+  <tbody>
+    <tr>
+      <td align="center" valign="top" width="16.66%"><a href="https://re-ra.xyz"><img src="https://avatars.githubusercontent.com/u/35157286?v=4?s=100" width="100px;" alt="Shixin Zhang"/><br /><sub><b>Shixin Zhang</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=refraction-ray" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=refraction-ray" title="Documentation">📖</a> <a href="#example-refraction-ray" title="Examples">💡</a> <a href="#ideas-refraction-ray" title="Ideas, Planning, & Feedback">🤔</a> <a href="#infra-refraction-ray" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#maintenance-refraction-ray" title="Maintenance">🚧</a> <a href="#research-refraction-ray" title="Research">🔬</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/pulls?q=is%3Apr+reviewed-by%3Arefraction-ray" title="Reviewed Pull Requests">👀</a> <a href="#translation-refraction-ray" title="Translation">🌍</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=refraction-ray" title="Tests">⚠️</a> <a href="#tutorial-refraction-ray" title="Tutorials">✅</a> <a href="#talk-refraction-ray" title="Talks">📢</a> <a href="#question-refraction-ray" title="Answering Questions">💬</a></td>
+      <td align="center" valign="top" width="16.66%"><a href="https://github.com/yutuer21"><img src="https://avatars.githubusercontent.com/u/83822724?v=4?s=100" width="100px;" alt="Yuqin Chen"/><br /><sub><b>Yuqin Chen</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=yutuer21" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=yutuer21" title="Documentation">📖</a> <a href="#example-yutuer21" title="Examples">💡</a> <a href="#ideas-yutuer21" title="Ideas, Planning, & Feedback">🤔</a> <a href="#research-yutuer21" title="Research">🔬</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=yutuer21" title="Tests">⚠️</a> <a href="#tutorial-yutuer21" title="Tutorials">✅</a> <a href="#talk-yutuer21" title="Talks">📢</a></td>
+      <td align="center" valign="top" width="16.66%"><a href="http://jiezhongqiu.com"><img src="https://avatars.githubusercontent.com/u/3853009?v=4?s=100" width="100px;" alt="Jiezhong Qiu"/><br /><sub><b>Jiezhong Qiu</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=xptree" title="Code">💻</a> <a href="#example-xptree" title="Examples">💡</a> <a href="#ideas-xptree" title="Ideas, Planning, & Feedback">🤔</a> <a href="#research-xptree" title="Research">🔬</a></td>
+      <td align="center" valign="top" width="16.66%"><a href="http://liwt31.github.io"><img src="https://avatars.githubusercontent.com/u/22628546?v=4?s=100" width="100px;" alt="Weitang Li"/><br /><sub><b>Weitang Li</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=liwt31" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=liwt31" title="Documentation">📖</a> <a href="#ideas-liwt31" title="Ideas, Planning, & Feedback">🤔</a> <a href="#research-liwt31" title="Research">🔬</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=liwt31" title="Tests">⚠️</a> <a href="#talk-liwt31" title="Talks">📢</a></td>
+      <td align="center" valign="top" width="16.66%"><a href="https://github.com/SUSYUSTC"><img src="https://avatars.githubusercontent.com/u/30529122?v=4?s=100" width="100px;" alt="Jiace Sun"/><br /><sub><b>Jiace Sun</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=SUSYUSTC" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=SUSYUSTC" title="Documentation">📖</a> <a href="#example-SUSYUSTC" title="Examples">💡</a> <a href="#ideas-SUSYUSTC" title="Ideas, Planning, & Feedback">🤔</a> <a href="#research-SUSYUSTC" title="Research">🔬</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=SUSYUSTC" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="16.66%"><a href="https://github.com/Zhouquan-Wan"><img src="https://avatars.githubusercontent.com/u/54523490?v=4?s=100" width="100px;" alt="Zhouquan Wan"/><br /><sub><b>Zhouquan Wan</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=Zhouquan-Wan" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=Zhouquan-Wan" title="Documentation">📖</a> <a href="#example-Zhouquan-Wan" title="Examples">💡</a> <a href="#ideas-Zhouquan-Wan" title="Ideas, Planning, & Feedback">🤔</a> <a href="#research-Zhouquan-Wan" title="Research">🔬</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=Zhouquan-Wan" title="Tests">⚠️</a> <a href="#tutorial-Zhouquan-Wan" title="Tutorials">✅</a></td>
+    </tr>
+    <tr>
+      <td align="center" valign="top" width="16.66%"><a href="https://github.com/ls-iastu"><img src="https://avatars.githubusercontent.com/u/70554346?v=4?s=100" width="100px;" alt="Shuo Liu"/><br /><sub><b>Shuo Liu</b></sub></a><br /><a href="#example-ls-iastu" title="Examples">💡</a> <a href="#research-ls-iastu" title="Research">🔬</a> <a href="#tutorial-ls-iastu" title="Tutorials">✅</a></td>
+      <td align="center" valign="top" width="16.66%"><a href="https://github.com/YHPeter"><img src="https://avatars.githubusercontent.com/u/44126839?v=4?s=100" width="100px;" alt="Hao Yu"/><br /><sub><b>Hao Yu</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=YHPeter" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=YHPeter" title="Documentation">📖</a> <a href="#infra-YHPeter" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=YHPeter" title="Tests">⚠️</a> <a href="#tutorial-YHPeter" title="Tutorials">✅</a></td>
+      <td align="center" valign="top" width="16.66%"><a href="https://github.com/SexyCarrots"><img src="https://avatars.githubusercontent.com/u/63588721?v=4?s=100" width="100px;" alt="Xinghan Yang"/><br /><sub><b>Xinghan Yang</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=SexyCarrots" title="Documentation">📖</a> <a href="#translation-SexyCarrots" title="Translation">🌍</a> <a href="#tutorial-SexyCarrots" title="Tutorials">✅</a></td>
+      <td align="center" valign="top" width="16.66%"><a href="https://github.com/JachyMeow"><img src="https://avatars.githubusercontent.com/u/114171061?v=4?s=100" width="100px;" alt="JachyMeow"/><br /><sub><b>JachyMeow</b></sub></a><br /><a href="#tutorial-JachyMeow" title="Tutorials">✅</a> <a href="#translation-JachyMeow" title="Translation">🌍</a></td>
+      <td align="center" valign="top" width="16.66%"><a href="https://github.com/Mzye21"><img src="https://avatars.githubusercontent.com/u/86239031?v=4?s=100" width="100px;" alt="Zhaofeng Ye"/><br /><sub><b>Zhaofeng Ye</b></sub></a><br /><a href="#design-Mzye21" title="Design">🎨</a></td>
+      <td align="center" valign="top" width="16.66%"><a href="https://github.com/erertertet"><img src="https://avatars.githubusercontent.com/u/41342153?v=4?s=100" width="100px;" alt="erertertet"/><br /><sub><b>erertertet</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=erertertet" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=erertertet" title="Documentation">📖</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=erertertet" title="Tests">⚠️</a></td>
+    </tr>
+    <tr>
+      <td align="center" valign="top" width="16.66%"><a href="https://github.com/yicongzheng"><img src="https://avatars.githubusercontent.com/u/107173985?v=4?s=100" width="100px;" alt="Yicong Zheng"/><br /><sub><b>Yicong Zheng</b></sub></a><br /><a href="#tutorial-yicongzheng" title="Tutorials">✅</a></td>
+      <td align="center" valign="top" width="16.66%"><a href="https://marksong.tech"><img src="https://avatars.githubusercontent.com/u/78847784?v=4?s=100" width="100px;" alt="Zixuan Song"/><br /><sub><b>Zixuan Song</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=MarkSong535" title="Documentation">📖</a> <a href="#translation-MarkSong535" title="Translation">🌍</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=MarkSong535" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=MarkSong535" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="16.66%"><a href="https://github.com/buwantaiji"><img src="https://avatars.githubusercontent.com/u/25216189?v=4?s=100" width="100px;" alt="Hao Xie"/><br /><sub><b>Hao Xie</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=buwantaiji" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="16.66%"><a href="https://github.com/pramitsingh0"><img src="https://avatars.githubusercontent.com/u/52959209?v=4?s=100" width="100px;" alt="Pramit Singh"/><br /><sub><b>Pramit Singh</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=pramitsingh0" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="16.66%"><a href="https://github.com/JAllcock"><img src="https://avatars.githubusercontent.com/u/26302022?v=4?s=100" width="100px;" alt="Jonathan Allcock"/><br /><sub><b>Jonathan Allcock</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=JAllcock" title="Documentation">📖</a> <a href="#ideas-JAllcock" title="Ideas, Planning, & Feedback">🤔</a> <a href="#talk-JAllcock" title="Talks">📢</a></td>
+      <td align="center" valign="top" width="16.66%"><a href="https://github.com/nealchen2003"><img src="https://avatars.githubusercontent.com/u/45502551?v=4?s=100" width="100px;" alt="nealchen2003"/><br /><sub><b>nealchen2003</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=nealchen2003" title="Documentation">📖</a></td>
+    </tr>
+    <tr>
+      <td align="center" valign="top" width="16.66%"><a href="https://github.com/eurethia"><img src="https://avatars.githubusercontent.com/u/84611606?v=4?s=100" width="100px;" alt="隐公观鱼"/><br /><sub><b>隐公观鱼</b></sub></a><br /><a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=eurethia" title="Code">💻</a> <a href="https://github.com/tencent-quantum-lab/tensorcircuit/commits?author=eurethia" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="16.66%"><a href="https://github.com/WiuYuan"><img src="https://avatars.githubusercontent.com/u/108848998?v=4?s=100" width="100px;" alt="WiuYuan"/><br /><sub><b>WiuYuan</b></sub></a><br /><a href="#example-WiuYuan" title="Examples">💡</a></td>
+      <td align="center" valign="top" width="16.66%"><a href="https://www.linkedin.com/in/felix-xu-16a153196/"><img src="https://avatars.githubusercontent.com/u/61252303?v=4?s=100" width="100px;" alt="Felix Xu"/><br /><sub><b>Felix Xu</b></sub></a><br /><a href="#tutorial-FelixXu35" title="Tutorials">✅</a></td>
+    </tr>
+  </tbody>
+</table>
+
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
+
+<!-- ALL-CONTRIBUTORS-LIST:END -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
+
+<!-- ALL-CONTRIBUTORS-LIST:END -->
+
+## Research and Applications
+
+### DQAS
+
+For the application of Differentiable Quantum Architecture Search, see [applications](/tensorcircuit/applications).
+
+Reference paper: https://arxiv.org/abs/2010.08561 (published in QST).
+
+### VQNHE
+
+For the application of Variational Quantum-Neural Hybrid Eigensolver, see [applications](/tensorcircuit/applications).
+
+Reference paper: https://arxiv.org/abs/2106.05105 (published in PRL) and https://arxiv.org/abs/2112.10380.
+
+### VQEX-MBL
+
+For the application of VQEX on MBL phase identification, see the [tutorial](/docs/source/tutorials/vqex_mbl.ipynb).
+
+Reference paper: https://arxiv.org/abs/2111.13719 (published in PRB).
+
+### Stark-DTC
+
+For the numerical demosntration of discrete time crystal enabled by Stark many-body localization, see the Floquet simulation [demo](/examples/timeevolution_trotter.py).
+
+Reference paper: https://arxiv.org/abs/2208.02866 (published in PRL).
+
+### RA-Training
+
+For the numerical simulation of variational quantum algorithm training using random gate activation strategy by us, see the [project repo](https://github.com/ls-iastu/RAtraining).
+
+Reference paper: https://arxiv.org/abs/2303.08154.
+
+### TenCirChem
+
+[TenCirChem](https://github.com/tencent-quantum-lab/TenCirChem) is an efficient and versatile quantum computation package for molecular properties. TenCirChem is based on TensorCircuit and is optimized for chemistry applications.
+
+Reference paper: https://arxiv.org/abs/2303.10825.
+
+### EMQAOA-DARBO
+
+For the numerical simulation and hardware experiments with error mitigation on QAOA, see the [project repo](https://github.com/sherrylixuecheng/EMQAOA-DARBO).
+
+Reference paper: https://arxiv.org/abs/2303.14877.
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tensorcircuit_nightly.egg-info/SOURCES.txt` & `tensorcircuit-nightly-0.9.1.dev20230608/tensorcircuit_nightly.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,17 @@
 tensorcircuit/interfaces/scipy.py
 tensorcircuit/interfaces/tensorflow.py
 tensorcircuit/interfaces/tensortrans.py
 tensorcircuit/interfaces/torch.py
 tensorcircuit/results/__init__.py
 tensorcircuit/results/counts.py
 tensorcircuit/results/readout_mitigation.py
+tensorcircuit/results/qem/__init__.py
+tensorcircuit/results/qem/benchmark_circuits.py
+tensorcircuit/results/qem/qem_methods.py
 tensorcircuit/templates/__init__.py
 tensorcircuit/templates/blocks.py
 tensorcircuit/templates/chems.py
 tensorcircuit/templates/dataset.py
 tensorcircuit/templates/ensemble.py
 tensorcircuit/templates/graphs.py
 tensorcircuit/templates/measurements.py
@@ -109,14 +112,15 @@
 tests/test_gates.py
 tests/test_interfaces.py
 tests/test_keras.py
 tests/test_miscs.py
 tests/test_mpscircuit.py
 tests/test_noisemodel.py
 tests/test_qaoa.py
+tests/test_qem.py
 tests/test_quantum.py
 tests/test_quantum_attr.py
 tests/test_results.py
 tests/test_simplify.py
 tests/test_templates.py
 tests/test_torchnn.py
 tests/test_van.py
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tests/conftest.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tests/test_backends.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tests/test_calibrating.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tests/test_calibrating.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tests/test_channels.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tests/test_channels.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tests/test_circuit.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tests/test_circuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tests/test_cloud.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tests/test_cloud.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tests/test_compiler.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tests/test_dmcircuit.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tests/test_dmcircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tests/test_ensemble.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tests/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tests/test_gates.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tests/test_gates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tests/test_interfaces.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tests/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tests/test_keras.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tests/test_keras.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tests/test_miscs.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tests/test_miscs.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tests/test_mpscircuit.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tests/test_mpscircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tests/test_noisemodel.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tests/test_noisemodel.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tests/test_qaoa.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tests/test_qaoa.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tests/test_quantum.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tests/test_quantum.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tests/test_quantum_attr.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tests/test_quantum_attr.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tests/test_results.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tests/test_simplify.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tests/test_simplify.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tests/test_templates.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tests/test_torchnn.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tests/test_torchnn.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230607/tests/test_van.py` & `tensorcircuit-nightly-0.9.1.dev20230608/tests/test_van.py`

 * *Files identical despite different names*

