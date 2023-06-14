# Comparing `tmp/mct-quantizers-nightly-1.0.0.7062023.post161221.tar.gz` & `tmp/mct-quantizers-nightly-1.0.0.8062023.post1051.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mct-quantizers-nightly-1.0.0.7062023.post161221.tar", last modified: Wed Jun  7 16:12:22 2023, max compression
+gzip compressed data, was "mct-quantizers-nightly-1.0.0.8062023.post1051.tar", last modified: Thu Jun  8 00:10:51 2023, max compression
```

## Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221.tar` & `mct-quantizers-nightly-1.0.0.8062023.post1051.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:12:22.859715 mct-quantizers-nightly-1.0.0.7062023.post161221/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-06-07 16:12:22.859715 mct-quantizers-nightly-1.0.0.7062023.post161221/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:12:22.855715 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:12:22.855715 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/common/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/common/base_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/common/get_all_subclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/common/get_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/common/quant_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/common/quant_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:12:22.855715 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/activation_quantization_holder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/load_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14484 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:12:22.855715 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:12:22.855715 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/activation_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:12:22.855715 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/weights_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/validation_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:12:22.859715 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/activation_quantization_holder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/load_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:12:22.859715 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:12:22.859715 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:12:22.859715 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:12:22.859715 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-06-07 16:12:22.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-06-07 16:12:22.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 16:12:22.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 16:12:22.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-07 16:12:22.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-07 16:12:22.859715 mct-quantizers-nightly-1.0.0.7062023.post161221/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-07 16:12:21.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:10:51.943399 mct-quantizers-nightly-1.0.0.8062023.post1051/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-08 00:10:51.943399 mct-quantizers-nightly-1.0.0.8062023.post1051/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:10:51.935399 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:10:51.935399 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/common/base_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/common/get_all_subclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/common/get_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/common/quant_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/common/quant_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:10:51.935399 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/activation_quantization_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14484 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:10:51.935399 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:10:51.939399 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/quantizers/activation_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:10:51.939399 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/quantizers/weights_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/validation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:10:51.939399 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/activation_quantization_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:10:51.943399 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:10:51.943399 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:10:51.943399 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-06-08 00:10:33.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:10:51.943399 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-08 00:10:51.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-06-08 00:10:51.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 00:10:51.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 00:10:51.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-08 00:10:51.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-08 00:10:51.947399 mct-quantizers-nightly-1.0.0.8062023.post1051/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-08 00:10:51.000000 mct-quantizers-nightly-1.0.0.8062023.post1051/setup.py
```

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/LICENSE.md` & `mct-quantizers-nightly-1.0.0.8062023.post1051/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/PKG-INFO` & `mct-quantizers-nightly-1.0.0.8062023.post1051/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-quantizers-nightly
-Version: 1.0.0.7062023.post161221
+Version: 1.0.0.8062023.post1051
 Summary: Infrastructure for support neural networks compression
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Tollkit (MCT) Quantizers
         
         This is an open-source library that provides tools that enable to easily represent a quantized neural network, both in Keras and in PyTorch.
         It provides researchers, developers, and engineers a set of useful quantizers and, in addition, a simple interface for implementing new custom quantizers.
```

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/README.md` & `mct-quantizers-nightly-1.0.0.8062023.post1051/README.md`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/__init__.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/common/__init__.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/common/base_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/common/base_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/common/constants.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/common/constants.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/common/get_all_subclasses.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/common/get_all_subclasses.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/common/get_quantizers.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/common/get_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/common/quant_info.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/common/quant_info.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/common/quant_utils.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/common/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/__init__.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/activation_quantization_holder.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/activation_quantization_holder.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/load_model.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/load_model.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantize_wrapper.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/quantize_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizer_utils.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/__init__.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/validation_functions.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/keras/validation_functions.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/logger.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/logger.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/__init__.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/activation_quantization_holder.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/activation_quantization_holder.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/load_model.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/load_model.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantize_wrapper.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantize_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizer_utils.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/__init__.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers_nightly.egg-info/PKG-INFO` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-quantizers-nightly
-Version: 1.0.0.7062023.post161221
+Version: 1.0.0.8062023.post1051
 Summary: Infrastructure for support neural networks compression
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Tollkit (MCT) Quantizers
         
         This is an open-source library that provides tools that enable to easily represent a quantized neural network, both in Keras and in PyTorch.
         It provides researchers, developers, and engineers a set of useful quantizers and, in addition, a simple interface for implementing new custom quantizers.
```

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers_nightly.egg-info/SOURCES.txt` & `mct-quantizers-nightly-1.0.0.8062023.post1051/mct_quantizers_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post161221/setup.py` & `mct-quantizers-nightly-1.0.0.8062023.post1051/setup.py`

 * *Files identical despite different names*

