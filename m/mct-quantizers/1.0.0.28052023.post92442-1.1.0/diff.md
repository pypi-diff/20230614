# Comparing `tmp/mct-quantizers-1.0.0.28052023.post92442.tar.gz` & `tmp/mct-quantizers-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mct-quantizers-1.0.0.28052023.post92442.tar", last modified: Sun May 28 09:24:43 2023, max compression
+gzip compressed data, was "mct-quantizers-1.1.0.tar", last modified: Wed Jun 14 12:12:13 2023, max compression
```

## Comparing `mct-quantizers-1.0.0.28052023.post92442.tar` & `mct-quantizers-1.1.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:24:43.794147 mct-quantizers-1.0.0.28052023.post92442/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-28 09:24:43.794147 mct-quantizers-1.0.0.28052023.post92442/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:24:43.786147 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:24:43.790147 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/common/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/common/base_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/common/get_all_subclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/common/get_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/common/quant_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/common/quant_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:24:43.790147 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/activation_quantization_holder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/load_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14264 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:24:43.790147 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:24:43.790147 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/activation_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:24:43.790147 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/weights_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/validation_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:24:43.790147 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/activation_quantization_holder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/load_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:24:43.790147 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:24:43.794147 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:24:43.794147 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-28 09:24:19.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:24:43.790147 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-28 09:24:43.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-28 09:24:43.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 09:24:43.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-28 09:24:43.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-28 09:24:43.000000 mct-quantizers-1.0.0.28052023.post92442/mct_quantizers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-28 09:24:43.794147 mct-quantizers-1.0.0.28052023.post92442/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-28 09:24:42.000000 mct-quantizers-1.0.0.28052023.post92442/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:12:13.699248 mct-quantizers-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-06-14 12:12:13.699248 mct-quantizers-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:12:13.687248 mct-quantizers-1.1.0/mct_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:12:13.691248 mct-quantizers-1.1.0/mct_quantizers/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/common/base_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/common/get_all_subclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/common/get_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/common/quant_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/common/quant_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:12:13.691248 mct-quantizers-1.1.0/mct_quantizers/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/activation_quantization_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11711 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:12:13.695248 mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:12:13.695248 mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:12:13.695248 mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/validation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:12:13.695248 mct-quantizers-1.1.0/mct_quantizers/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/activation_quantization_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:12:13.699248 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:12:13.699248 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:12:13.699248 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:12:13.687248 mct-quantizers-1.1.0/mct_quantizers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-06-14 12:12:13.000000 mct-quantizers-1.1.0/mct_quantizers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-06-14 12:12:13.000000 mct-quantizers-1.1.0/mct_quantizers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 12:12:13.000000 mct-quantizers-1.1.0/mct_quantizers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-14 12:12:13.000000 mct-quantizers-1.1.0/mct_quantizers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-14 12:12:13.000000 mct-quantizers-1.1.0/mct_quantizers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-14 12:12:13.699248 mct-quantizers-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/setup.py
```

### Comparing `mct-quantizers-1.0.0.28052023.post92442/LICENSE.md` & `mct-quantizers-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/__init__.py` & `mct-quantizers-1.1.0/mct_quantizers/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,11 +19,11 @@
 from mct_quantizers.pytorch.activation_quantization_holder import PytorchActivationQuantizationHolder
 from mct_quantizers.keras.load_model import keras_load_quantized_model
 from mct_quantizers.keras.quantize_wrapper import KerasQuantizationWrapper
 from mct_quantizers.pytorch.load_model import pytorch_load_quantized_model
 from mct_quantizers.pytorch.quantize_wrapper import PytorchQuantizationWrapper
 
 from mct_quantizers.common import constants
-from mct_quantizers.keras import quantizers
-from mct_quantizers.pytorch import quantizers
+from mct_quantizers.keras import quantizers as keras_quantizers
+from mct_quantizers.pytorch import quantizers as pytorch_quantizers
 
-__version__ = "1.0.0"
+__version__ = "1.1.0"
```

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/common/__init__.py` & `mct-quantizers-1.1.0/mct_quantizers/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/common/base_inferable_quantizer.py` & `mct-quantizers-1.1.0/mct_quantizers/common/base_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/common/constants.py` & `mct-quantizers-1.1.0/mct_quantizers/common/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 NUM_BITS = 'num_bits'
 SIGNED = 'signed'
 THRESHOLD = 'threshold'
 PER_CHANNEL = 'per_channel'
 MIN_RANGE = 'min_range'
 MAX_RANGE = 'max_range'
 CHANNEL_AXIS = 'channel_axis'
+INPUT_RANK = 'input_rank'
 CLUSTER_CENTERS = 'cluster_centers'
 
 
 ## Constant values
 
 LAYER = "layer"
 STEPS = "optimizer_step"
```

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/common/get_all_subclasses.py` & `mct-quantizers-1.1.0/mct_quantizers/common/get_all_subclasses.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/common/get_quantizers.py` & `mct-quantizers-1.1.0/mct_quantizers/common/get_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/common/quant_info.py` & `mct-quantizers-1.1.0/mct_quantizers/common/quant_info.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/common/quant_utils.py` & `mct-quantizers-1.1.0/mct_quantizers/common/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/__init__.py` & `mct-quantizers-1.1.0/mct_quantizers/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/activation_quantization_holder.py` & `mct-quantizers-1.1.0/mct_quantizers/keras/activation_quantization_holder.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,21 +11,24 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 
 from mct_quantizers.common.base_inferable_quantizer import BaseInferableQuantizer
-from mct_quantizers.common.constants import ACTIVATION_HOLDER_QUANTIZER, FOUND_TF, TRAINING
+from mct_quantizers.common.constants import ACTIVATION_HOLDER_QUANTIZER, FOUND_TF, TRAINING, STEPS
+from mct_quantizers.common.get_all_subclasses import get_all_subclasses
 from mct_quantizers.logger import Logger
 
 if FOUND_TF:
     import tensorflow as tf
     from keras.utils import tf_inspect
     from tensorflow_model_optimization.python.core.keras import utils
+    from mct_quantizers.keras.quantizers import BaseKerasInferableQuantizer
+
     keras = tf.keras
 
 
     def _make_quantizer_fn(quantizer, x, training):
         """Use currying to return True/False specialized fns to the cond."""
 
         def quantizer_fn():
@@ -70,18 +73,20 @@
 
             Args:
                 config(dict): dictionary  of  ActivationQuantizationHolder Configuration
 
             Returns: A ActivationQuantizationHolder object
 
             """
+            qi_inferable_custom_objects = {subclass.__name__: subclass for subclass in
+                                           get_all_subclasses(BaseKerasInferableQuantizer)}
             config = config.copy()
             activation_holder_quantizer = keras.utils.deserialize_keras_object(config.pop(ACTIVATION_HOLDER_QUANTIZER),
                                                                                module_objects=globals(),
-                                                                               custom_objects=None)
+                                                                               custom_objects=qi_inferable_custom_objects)
 
             return cls(activation_holder_quantizer=activation_holder_quantizer,
                        **config)
 
         def build(self, input_shape):
             """
             ActivationQuantizationHolder build function.
@@ -131,15 +136,18 @@
         def convert_to_inferable_quantizers(self):
             """
             Convert layer's quantizer to inferable quantizer.
 
             Returns:
                 None
             """
-            self.activation_holder_quantizer = self.activation_holder_quantizer.convert2inferable()
+            if hasattr(self.activation_holder_quantizer, 'convert2inferable') and callable(
+                    self.activation_holder_quantizer.convert2inferable):  # pragma: no cover
+                self.activation_holder_quantizer = self.activation_holder_quantizer.convert2inferable()
+                return self.from_config(self.get_config()) # return new layer with no weights. It assumes holder of inferable quantizers have no weights
 
 
 else:
     class KerasActivationQuantizationHolder:  # pragma: no cover
         def __init__(self, *args, **kwargs):
             Logger.error('Installing tensorflow and tensorflow_model_optimization is mandatory '
                          'when using ActivationQuantizationHolder. '
```

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/load_model.py` & `mct-quantizers-1.1.0/mct_quantizers/keras/load_model.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantize_wrapper.py` & `mct-quantizers-1.1.0/mct_quantizers/keras/quantize_wrapper.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,21 +11,23 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Dict, List, Any, Tuple
 
 from mct_quantizers.common.base_inferable_quantizer import BaseInferableQuantizer
-from mct_quantizers.common.constants import FOUND_TF, ACTIVATION_QUANTIZERS, WEIGHTS_QUANTIZERS, STEPS, LAYER, TRAINING
+from mct_quantizers.common.constants import FOUND_TF, WEIGHTS_QUANTIZERS, STEPS, LAYER, TRAINING
 from mct_quantizers.logger import Logger
+from mct_quantizers.common.get_all_subclasses import get_all_subclasses
 
 if FOUND_TF:
     import tensorflow as tf
     from tensorflow.python.util import tf_inspect
     from tensorflow_model_optimization.python.core.keras import utils
+    from mct_quantizers.keras.quantizers import BaseKerasInferableQuantizer
 
     keras = tf.keras
 
     def _make_quantizer_fn(quantizer, x, training):
         """Use currying to return True/False specialized fns to the cond."""
 
         def quantizer_fn():
@@ -48,28 +50,25 @@
         return name.split(':')[0].split('/')[-1]
 
 
     class KerasQuantizationWrapper(tf.keras.layers.Wrapper):
         def __init__(self,
                      layer,
                      weights_quantizers: Dict[str, BaseInferableQuantizer] = None,
-                     activation_quantizers: List[BaseInferableQuantizer] = None,
                      **kwargs):
             """
             Keras Quantization Wrapper takes a keras layer and quantizers and infer a quantized layer.
 
             Args:
                 layer: A keras layer.
                 weights_quantizers: A dictionary between a weight's name to its quantizer.
-                activation_quantizers: A list of activations quantization, one for each layer output.
             """
             super(KerasQuantizationWrapper, self).__init__(layer, **kwargs)
             self._track_trackable(layer, name='layer')
             self.weights_quantizers = weights_quantizers if weights_quantizers is not None else dict()
-            self.activation_quantizers = activation_quantizers if activation_quantizers is not None else list()
 
         def add_weights_quantizer(self, param_name: str, quantizer: BaseInferableQuantizer):
             """
             This function adds a weights quantizer to existing wrapper
 
             Args:
                 param_name: The name of the parameter to quantize
@@ -77,23 +76,14 @@
 
             Returns: None
 
             """
             self.weights_quantizers.update({param_name: quantizer})
 
         @property
-        def is_activation_quantization(self) -> bool:
-            """
-            This function check activation quantizer exists in wrapper.
-            Returns: a boolean if activation quantizer exists
-
-            """
-            return self.num_activation_quantizers > 0
-
-        @property
         def is_weights_quantization(self) -> bool:
             """
             This function check weights quantizer exists in wrapper.
 
             Returns: a boolean if weights quantizer exists
 
             """
@@ -102,30 +92,21 @@
         @property
         def num_weights_quantizers(self) -> int:
             """
             Returns: number of weights quantizers
             """
             return len(self.weights_quantizers)
 
-        @property
-        def num_activation_quantizers(self) -> int:
-            """
-            Returns: number of activations quantizers
-            """
-            return len(self.activation_quantizers)
-
         def get_config(self):
             """
             Returns: Configuration of KerasQuantizationWrapper.
 
             """
             base_config = super(KerasQuantizationWrapper, self).get_config()
-            config = {
-                ACTIVATION_QUANTIZERS: [keras.utils.serialize_keras_object(act) for act in self.activation_quantizers],
-                WEIGHTS_QUANTIZERS: {k: keras.utils.serialize_keras_object(v) for k, v in self.weights_quantizers.items()}}
+            config = {WEIGHTS_QUANTIZERS: {k: keras.utils.serialize_keras_object(v) for k, v in self.weights_quantizers.items()}}
             return dict(list(base_config.items()) + list(config.items()))
 
         def _set_weights_vars(self, is_training: bool = True):
             """
             This function sets weights quantizers vars to the layer
 
             Args:
@@ -137,46 +118,32 @@
             for name, quantizer in self.weights_quantizers.items():
                 weight = getattr(self.layer, name)
                 quantizer.initialize_quantization(weight.shape, _weight_name(weight.name) if is_training else None,
                                                   self)
                 self._weights_vars.append((name, weight, quantizer))
                 self._trainable_weights.append(weight) # Must when inherit from tf.keras.layers.Wrapper in tf2.10 and below
 
-        def _set_activations_vars(self):
-            """
-            This function sets activations quantizers vars to the layer
-
-            Returns: None
-            """
-            self._activation_vars = []
-            for i, quantizer in enumerate(self.activation_quantizers):
-                quantizer.initialize_quantization(None, self.layer.name + f'/out{i}', self)
-                self._activation_vars.append(quantizer)
-
         @classmethod
         def from_config(cls, config):
             """
 
             Args:
                 config(dict): dictionary  of  KerasQuantizationWrapper Configuration
 
             Returns: A KerasQuantizationWrapper
 
             """
             config = config.copy()
-            activation_quantizers = [keras.utils.deserialize_keras_object(act,
-                                                                          module_objects=globals(),
-                                                                          custom_objects=None) for act in
-                                     config.pop(ACTIVATION_QUANTIZERS)]
+            qi_inferable_custom_objects = {subclass.__name__: subclass for subclass in
+                                           get_all_subclasses(BaseKerasInferableQuantizer)}
             weights_quantizers = {k: keras.utils.deserialize_keras_object(v,
-                                                                         module_objects=globals(),
-                                                                         custom_objects=None) for k, v in
-                                 config.pop(WEIGHTS_QUANTIZERS).items()}
+                                                                          module_objects=globals(),
+                                                                          custom_objects=qi_inferable_custom_objects) for k, v in config.pop(WEIGHTS_QUANTIZERS).items()}
             layer = tf.keras.layers.deserialize(config.pop(LAYER))
-            return cls(layer=layer, weights_quantizers=weights_quantizers, activation_quantizers=activation_quantizers, **config)
+            return cls(layer=layer, weights_quantizers=weights_quantizers, **config)
 
         def build(self, input_shape):
             """
             KerasQuantization Wrapper build function.
             Args:
                 input_shape: the layer input shape
 
@@ -188,15 +155,14 @@
             self.optimizer_step = self.add_weight(
                 STEPS,
                 initializer=tf.keras.initializers.Constant(-1),
                 dtype=tf.dtypes.int32,
                 trainable=False)
 
             self._set_weights_vars()
-            self._set_activations_vars()
 
         def set_quantize_weights(self, quantized_weights: dict):
             """
             This function update layer weights after quantization.
 
             Args:
                 quantized_weights: a dict of weight to update
@@ -248,61 +214,43 @@
 
             args_spec = tf_inspect.getfullargspec(self.layer.call).args
             if TRAINING in args_spec:
                 outputs = self.layer.call(inputs, training=training, **kwargs)
             else:
                 outputs = self.layer.call(inputs, **kwargs)
 
-            # Quantize all activations if quantizers exist.
-            if self.is_activation_quantization:
-                num_outputs = len(outputs) if isinstance(outputs, (list, tuple)) else 1
-                if self.num_activation_quantizers != num_outputs:
-                    Logger.error('Quantization wrapper output quantization error: '
-                                 f'number of outputs and quantizers mismatch ({num_outputs}!='
-                                 f'{self.num_activation_quantizers}')
-                if num_outputs == 1:
-                    outputs = [outputs]
-
-                _outputs = []
-                for _output, act_quant in zip(outputs, self.activation_quantizers):
-                    activation_quantizer_args_spec = tf_inspect.getfullargspec(act_quant.__call__).args
-                    if TRAINING in activation_quantizer_args_spec:
-                        _outputs.append(utils.smart_cond(
-                            training,
-                            _make_quantizer_fn(act_quant, _output, True),
-                            _make_quantizer_fn(act_quant, _output, False)))
-                    else:
-                        # Keras activation inferable quantizer.
-                        _outputs.append(act_quant(_output))
-                outputs = _outputs[0] if num_outputs == 1 else _outputs
-
             return outputs
 
         def convert_to_inferable_quantizers(self):
             """
             Convert layer's quantizers to inferable.
 
             Returns:
                 None
             """
-            # Activations quantizers
-            inferable_activation_quantizers = []
-            if self.is_activation_quantization:
-                for quantizer in self.activation_quantizers:
-                    inferable_activation_quantizers.append(quantizer.convert2inferable())
-                self.activation_quantizers = inferable_activation_quantizers
-                self._set_activations_vars()
-
             # Weight quantizers
             inferable_weight_quantizers = {}
             if self.is_weights_quantization:
                 for name, quantizer in self.weights_quantizers.items():
-                    inferable_weight_quantizers.update({name: quantizer.convert2inferable()})
+                    if hasattr(quantizer, 'convert2inferable') and callable(quantizer.convert2inferable):
+                        inferable_weight_quantizers.update({name: quantizer.convert2inferable()})
                 self.weights_quantizers = inferable_weight_quantizers
-                self._set_weights_vars(False)
+
+            # Create new layer with inferable quantizers
+            inferable_quantizers_wrapper = self.from_config(self.get_config())
+            inferable_quantizers_wrapper.layer.build(self.get_input_shape_at(0))
+            layer_weights_list = []
+            for weight_attr in self.weights_quantizers.keys():
+                layer_weights_list.append(getattr(self.layer, weight_attr)) # quantized weights
+            layer_weights_list.extend(self.layer.get_weights()) # non quantized weights
+            inferable_quantizers_wrapper.layer.set_weights(layer_weights_list)
+
+            # The wrapper inference is using the weights of the quantizers so it expectes to create them by running _set_weights_vars
+            inferable_quantizers_wrapper._set_weights_vars(False)
+            return inferable_quantizers_wrapper
 
         def get_weights_vars(self) -> List[Tuple[str, Any, BaseInferableQuantizer]]:
             """
             A getter of the layer's weights variables.
 
             Returns:
                 List pf tuples of the wrapped layer's weights variables with weight name, values and assigned quantizer.
@@ -323,20 +271,18 @@
                 quantized_weights[name] = quantizer(w)
             return quantized_weights
 
 else:
     class KerasQuantizationWrapper(object):
         def __init__(self,
                      layer,
-                     weights_quantizers: Dict[str, BaseInferableQuantizer] = None,
-                     activation_quantizers: List[BaseInferableQuantizer] = None):
+                     weights_quantizers: Dict[str, BaseInferableQuantizer] = None):
             """
             Keras Quantization Wrapper takes a keras layer and quantizers and infer a quantized layer.
 
             Args:
                 layer: A keras layer.
                 weights_quantizers: A dictionary between a weight's name to its quantizer.
-                activation_quantizers: A list of activations quantization, one for each layer output.
             """
             Logger.critical('Installing tensorflow and tensorflow_model_optimization is mandatory '
                             'when using KerasQuantizationWrapper. '
                             'Could not find Tensorflow package.')  # pragma: no cover
```

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizer_utils.py` & `mct-quantizers-1.1.0/mct_quantizers/keras/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/__init__.py` & `mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py` & `mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py` & `mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py` & `mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             """
             # Call the superclass constructor with the given parameters, along with the target of Activation
             # quantization
             super(ActivationPOTInferableQuantizer, self).__init__(num_bits=num_bits,
                                                                   threshold=threshold,
                                                                   signed=signed)
 
-            is_threshold_pot = np.all([int(np.log2(x)) == np.log2(x) for x in self.threshold.flatten()])
+            is_threshold_pot = np.all([int(np.log2(x)) == np.log2(x) for x in np.asarray(self.threshold).flatten()])
             assert is_threshold_pot, f'Expected threshold to be power of 2 but is {self.threshold}'
 
 else:
     class ActivationPOTInferableQuantizer:  # pragma: no cover
         def __init__(self, *args, **kwargs):
             Logger.error('Installing tensorflow and tensorflow_model_optimization is mandatory '
                          'when using ActivationPOTInferableQuantizer. '
```

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py` & `mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,25 +44,27 @@
 
             Args:
                 num_bits: number of bits to use for quantization
                 threshold: threshold for quantizing activations
                 signed: whether or not to use signed quantization
             """
             assert isinstance(threshold, list), f'Expected threshold to be of type list but is {type(threshold)}'
+            # In activation per-channel quantization is not supported thus we expect a single min/max value.
+            assert len(threshold) == 1, f'In per-tensor quantization threshold should be of length 1 but is {len(threshold)}'
             assert all([isinstance(x, (float, np.float32, tf.float32)) for x in
                         threshold]), f'Expected threshold list to contain float or np.float values but found ' \
                                      f'{[type(x) for x in threshold]}'
 
-            self.threshold = np.asarray(threshold)
+            self.threshold = threshold
             self.signed = signed
 
-            delta = self.threshold / (2 ** (num_bits - int(self.signed)))
+            delta = self.threshold[0] / (2 ** (num_bits - int(self.signed)))
             # In activation quantization is per-tensor only - thus we pass the threshold as a list with a len of 1
-            min_range = list(-self.threshold) if self.signed else [0.0]
-            max_range = list(self.threshold - delta)
+            min_range = [-threshold[0]] if self.signed else [0.0]
+            max_range = [self.threshold[0] - delta]
 
             super(ActivationSymmetricInferableQuantizer, self).__init__(num_bits=num_bits,
                                                                         min_range=min_range,
                                                                         max_range=max_range)
 
         def get_config(self):
             """
```

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py` & `mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py` & `mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py` & `mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py` & `mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py` & `mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             # Call the superclass constructor with the given parameters, along with the target of Weights quantization
             super(WeightsPOTInferableQuantizer, self).__init__(num_bits=num_bits,
                                                                threshold=threshold,
                                                                per_channel=per_channel,
                                                                channel_axis=channel_axis,
                                                                input_rank=input_rank)
 
-            is_threshold_pot = np.all([int(np.log2(x)) == np.log2(x) for x in self.threshold.flatten()])
+            is_threshold_pot = np.all([int(np.log2(x)) == np.log2(x) for x in self._np_threshold.flatten()])
             assert is_threshold_pot, f'Expected threshold to be power of 2 but is {self.threshold}'
 
 
 else:
     class WeightsPOTInferableQuantizer:  # pragma: no cover
         def __init__(self, *args, **kwargs):
             raise Exception('Installing tensorflow and tensorflow_model_optimization is mandatory '
```

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py` & `mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,18 +50,18 @@
                 input_rank: number of dimensions of input tensor the quantizer quantizes
             """
             assert isinstance(threshold, list), f'Expected threshold to be of type list but is {type(threshold)}'
             assert all([isinstance(x, (float, np.float32, np.float64)) for x in
                         threshold]), f'Expected threshold list to contain float or np.float values but found ' \
                                      f'{[type(x) for x in threshold]}'
 
-            self.threshold = np.asarray(threshold)
-
-            _min_range = -self.threshold
-            _max_range = self.threshold - self.threshold / (2 ** (num_bits - 1))
+            self.threshold = threshold
+            self._np_threshold = np.asarray(threshold)
+            _min_range = -self._np_threshold
+            _max_range = self._np_threshold - self._np_threshold / (2 ** (num_bits - 1))
 
             super(WeightsSymmetricInferableQuantizer, self).__init__(num_bits=num_bits,
                                                                      min_range=list(_min_range),
                                                                      max_range=list(_max_range),
                                                                      per_channel=per_channel,
                                                                      channel_axis=channel_axis,
                                                                      input_rank=input_rank)
```

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py` & `mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,41 +53,44 @@
                 per_channel: whether to use per-channel quantization
                 channel_axis: axis along which to apply per-channel quantization
                 input_rank: number of dimensions of input tensor the quantizer quantizes
             """
 
             super(WeightsUniformInferableQuantizer, self).__init__()
 
+            self.min_range = min_range
+            self.max_range = max_range
+
             # Validate inputs properties
             validate_uniform_min_max_ranges(min_range,
                                             max_range)
 
             # Convert min/max to numpy arrays
-            min_range, max_range = np.asarray(min_range), np.asarray(max_range)
-            _min_range, _max_range = adjust_range_to_include_zero(min_range, max_range, num_bits)
-            validate_adjusted_min_max_ranges(min_range=min_range,
-                                             max_range=max_range,
-                                             adj_min=_min_range,
-                                             adj_max=_max_range)
+            min_range_np, max_range_np = np.asarray(min_range), np.asarray(max_range)
+            _min_range_np, _max_range_np = adjust_range_to_include_zero(min_range_np, max_range_np, num_bits)
+            validate_adjusted_min_max_ranges(min_range=min_range_np,
+                                             max_range=max_range_np,
+                                             adj_min=_min_range_np,
+                                             adj_max=_max_range_np)
 
             self.num_bits = num_bits
-            self.max_range = _max_range
-            self.min_range = _min_range
+            self.max_range_np = _max_range_np
+            self.min_range_np = _min_range_np
 
             if per_channel:
                 assert input_rank is not None, f'Input rank is missing in per channel quantization'
                 assert channel_axis is not None, f'Channel axis is missing in per channel quantization'
-                assert len(self.min_range) >= 1, f'In per-channel quantization min ranges list should be of length >= 1 but is {len(self.min_range)}'
-                assert len(self.max_range) >= 1, f'In per-channel quantization max ranges list should be of length >= 1 but is {len(self.max_range)}'
+                assert len(self.min_range_np) >= 1, f'In per-channel quantization min ranges list should be of length >= 1 but is {len(self.min_range_np)}'
+                assert len(self.max_range_np) >= 1, f'In per-channel quantization max ranges list should be of length >= 1 but is {len(self.max_range_np)}'
             else:
-                assert len(self.min_range) == 1, f'In per-tensor quantization min/max should be of length 1 but is {len(min_range)}'
-                assert len(self.min_range) == 1, f'In per-tensor quantization min_range should be of length 1 but is {len(self.min_range)}'
-                assert len(self.max_range) == 1, f'In per-tensor quantization max_range should be of length 1 but is {len(self.max_range)}'
-                self.min_range = self.min_range[0]
-                self.max_range = self.max_range[0]
+                assert len(self.min_range_np) == 1, f'In per-tensor quantization min/max should be of length 1 but is {len(self.min_range)}'
+                assert len(self.min_range_np) == 1, f'In per-tensor quantization min_range should be of length 1 but is {len(self.min_range_np)}'
+                assert len(self.max_range_np) == 1, f'In per-tensor quantization max_range should be of length 1 but is {len(self.max_range_np)}'
+                self.min_range_np = self.min_range_np[0]
+                self.max_range_np = self.max_range_np[0]
 
             self.per_channel = per_channel
             self.channel_axis = channel_axis
             self.input_rank = input_rank
 
             # Tensorflow's fake_quant_with_min_max_vars_per_channel only works on last axis, so
             # need to move the quantization axis to the last axis
@@ -119,28 +122,28 @@
                 # If a permutation vector has been created to move the channel axis to the last position
                 if self.perm_vec:
                     # Transpose the input tensor to move the channel axis to the last position
                     inputs = tf.transpose(inputs, perm=self.perm_vec)
 
                 # Quantize the input tensor using per-channel quantization
                 q_tensor = tf.quantization.fake_quant_with_min_max_vars_per_channel(inputs,
-                                                                                    min=self.min_range,
-                                                                                    max=self.max_range,
+                                                                                    min=self.min_range_np,
+                                                                                    max=self.max_range_np,
                                                                                     num_bits=self.num_bits)
                 if self.perm_vec:
                     # Transpose the quantized tensor back to its original shape
                     q_tensor = tf.transpose(q_tensor, perm=self.perm_vec)
 
                 # Return the quantized tensor
                 return q_tensor
             else:
                 # If per-channel quantization is not being used, quantize the input tensor using regular quantization
                 return tf.quantization.fake_quant_with_min_max_vars(inputs,
-                                                                    min=self.min_range,
-                                                                    max=self.max_range,
+                                                                    min=self.min_range_np,
+                                                                    max=self.max_range_np,
                                                                     num_bits=self.num_bits)
 
 
         def get_config(self):
             """
             Return a dictionary with the configuration of the quantizer.
```

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/keras/validation_functions.py` & `mct-quantizers-1.1.0/mct_quantizers/keras/validation_functions.py`

 * *Files 15% similar despite different names*

```diff
@@ -58,9 +58,12 @@
         adj_min: adjusted min range
         adj_max: adjusted max range
 
     """
 
     assert np.all(adj_min <= 0) and np.all(
         adj_max >= 0), f'Expected zero to be in the range, got min_range={adj_min}, max_range={adj_max}'
-    if not np.isclose(np.linalg.norm(adj_min - min_range), 0, atol=1e-6) or not np.isclose(np.linalg.norm(adj_max - max_range), 0, atol=1e-6):
+
+    grid_range = (max_range - min_range)
+    if not np.all(np.isclose((adj_min - min_range) / grid_range, 0, atol=1e-6)) \
+            or not np.all(np.isclose((adj_max - max_range) / grid_range, 0, atol=1e-6)):
         Logger.warning(f"Adjusting (min_range, max_range) from ({min_range},{max_range}) to ({adj_min},{adj_max})")  # pragma: no cover
```

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/logger.py` & `mct-quantizers-1.1.0/mct_quantizers/logger.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/__init__.py` & `mct-quantizers-1.1.0/mct_quantizers/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/activation_quantization_holder.py` & `mct-quantizers-1.1.0/mct_quantizers/pytorch/activation_quantization_holder.py`

 * *Files 13% similar despite different names*

```diff
@@ -54,15 +54,17 @@
 
         def convert_to_inferable_quantizers(self):
             """
             Convert a layer's quantizer to an inferable quantizer.
             Returns:
                 None
             """
-            self.activation_holder_quantizer = self.activation_holder_quantizer.convert2inferable()
+            if hasattr(self.activation_holder_quantizer, 'convert2inferable') and callable(
+                    self.activation_holder_quantizer.convert2inferable):  # pragma: no cover
+                self.activation_holder_quantizer = self.activation_holder_quantizer.convert2inferable()
 
 else:
     class PytorchActivationQuantizationHolder:  # pragma: no cover
         def __init__(self, *args, **kwargs):
             Logger.critical('Installing Pytorch is mandatory '
                             'when using PytorchActivationQuantizationHolder. '
                             'Could not find the torch package.')  # pragma: no cover
```

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/load_model.py` & `mct-quantizers-1.1.0/mct_quantizers/pytorch/load_model.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantize_wrapper.py` & `mct-quantizers-1.1.0/mct_quantizers/pytorch/quantize_wrapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,35 +24,31 @@
     import torch
     import torch.nn as nn
 
 
     class PytorchQuantizationWrapper(nn.Module):
         def __init__(self,
                      module: nn.Module,
-                     weights_quantizers: Dict[str, BaseInferableQuantizer] = None,
-                     activation_quantizers: List[BaseInferableQuantizer] = None):
+                     weights_quantizers: Dict[str, BaseInferableQuantizer] = None):
             """
             Pytorch Quantization Wrapper takes a pytorch module and quantizers and infer a quantized module.
 
             Args:
                 module: A pytorch module.
                 weights_quantizers: A dictionary between a weight's name to its quantizer.
-                activation_quantizers: A list of activations quantization, one for each layer output.
             """
             super().__init__()
             if isinstance(module, nn.Module):
                 self.add_module(LAYER, module)
             else:
                 # Functional layers
                 setattr(self, LAYER, module)
 
             self.weights_quantizers = weights_quantizers if weights_quantizers is not None else dict()
-            self.activation_quantizers = activation_quantizers if activation_quantizers is not None else list()
             self._set_weights_vars(True)
-            self._set_activation_vars()
 
         def add_weights_quantizer(self, param_name: str, quantizer: BaseInferableQuantizer):
             """
             This function adds a weights quantizer to existing wrapper
 
             Args:
                 param_name: The name of the parameter to quantize
@@ -60,23 +56,14 @@
 
             Returns: None
 
             """
             self.weights_quantizers.update({param_name: quantizer})
 
         @property
-        def is_activation_quantization(self) -> bool:
-            """
-            This function check activation quantizer exists in wrapper.
-            Returns: a boolean if activation quantizer exists
-
-            """
-            return self.num_activation_quantizers > 0
-
-        @property
         def is_weights_quantization(self) -> bool:
             """
             This function check weights quantizer exists in wrapper.
 
             Returns: a boolean if weights quantizer exists
 
             """
@@ -85,39 +72,25 @@
         @property
         def num_weights_quantizers(self) -> int:
             """
             Returns: number of weights quantizers
             """
             return len(self.weights_quantizers)
 
-        @property
-        def num_activation_quantizers(self) -> int:
-            """
-            Returns: number of activations quantizers
-            """
-            return len(self.activation_quantizers)
-
         def convert_to_inferable_quantizers(self):
             """
             Convert the wrapper quantizers with inferable quantizers
 
             """
-            # Activation quantizers
-            if self.is_activation_quantization:
-                inferable_activation_quantizers = []
-                for quantizer in self.activation_quantizers:
-                    inferable_activation_quantizers.append(quantizer.convert2inferable())
-                self.activation_quantizers = inferable_activation_quantizers
-                self._set_activation_vars()
-
             # Weight quantizers
             if self.is_weights_quantization:
                 inferable_weight_quantizers = {}
                 for name, quantizer in self.weights_quantizers.items():
-                    inferable_weight_quantizers.update({name: quantizer.convert2inferable()})
+                    if hasattr(quantizer, 'convert2inferable') and callable(quantizer.convert2inferable):
+                        inferable_weight_quantizers.update({name: quantizer.convert2inferable()})
                 self.weights_quantizers = inferable_weight_quantizers
                 self._set_weights_vars(False)
 
         def _set_weights_vars(self, is_training: bool = True):
             """
             Initialize learnable weights as parameters in the wrapper, and their quantizers
 
@@ -137,23 +110,14 @@
                 else:
                     weight = getattr(self, name).detach()
                     delattr(self.layer, name)
                     setattr(self.layer, name, weight)
                 quantizer.initialize_quantization(weight.shape, name, self)
                 self._weights_vars.append((name, getattr(self, name), quantizer))
 
-        def _set_activation_vars(self):
-            """
-            Initialize layer outputs and their quantizers in the wrapper
-            """
-            self._activation_vars = []
-            for i, quantizer in enumerate(self.activation_quantizers):
-                quantizer.initialize_quantization(None, f"tensor{i}", self)
-                self._activation_vars.append(quantizer)
-
         def set_quantize_weights(self, quantized_weights: dict):
             """
             This function updates layer weights after quantization.
 
             Args:
                 quantized_weights: a dict of weight to update
 
@@ -201,37 +165,20 @@
                     else:
                         quantized_weight = quantizer(unquantized_weight)
 
                     quantized_weights.update({name: quantized_weight})
 
                 self.set_quantize_weights(quantized_weights)
 
+
             # ----------------------------------
             # Layer operation
             # ----------------------------------
             outputs = self.layer(*args, **kwargs)
 
-            # ----------------------------------
-            # Quantize all activations
-            # ----------------------------------
-            if self.is_activation_quantization:
-
-                if not isinstance(outputs, list):
-                    outputs = [outputs]
-
-                if len(outputs) != self.num_activation_quantizers:
-                    Logger.error(f"Number of outputs {len(outputs)} is incompatible number of activation quantizers {self.num_activation_quantizers}")  # pragma: no cover
-
-                # Quantize all activations tensors
-                outputs_quantized = []
-                for quantizer, output in zip(self._activation_vars, outputs):
-                    outputs_quantized.append(quantizer(output))
-
-                outputs = outputs_quantized[0] if len(outputs_quantized) == 1 else outputs_quantized
-
             return outputs
 
         def get_quantized_weights(self) -> Dict[str, torch.Tensor]:
             """
 
             Returns: A dictionary of weights attributes to quantized weights.
 
@@ -242,20 +189,18 @@
                 quantized_weights[name] = quantizer(w)
             return quantized_weights
 
 else:
     class PytorchQuantizationWrapper(object):
         def __init__(self,
                      layer,
-                     weight_quantizers: Dict[str, BaseInferableQuantizer] = None,
-                     activation_quantizers: List[BaseInferableQuantizer] = None):
+                     weight_quantizers: Dict[str, BaseInferableQuantizer] = None):
             """
             Pytorch Quantization Wrapper takes a pytorch module and quantizers and infer a quantized layer.
 
             Args:
                 layer: A pytorch module.
                 weight_quantizers: A dictionary between a weight's name to its quantizer.
-                activation_quantizers: A list of activations quantization, one for each layer output.
             """
             Logger.critical('Installing Pytorch is mandatory '
                             'when using PytorchQuantizationWrapper. '
                             'Could not find torch package.')  # pragma: no cover
```

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizer_utils.py` & `mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/__init__.py` & `mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py` & `mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py` & `mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py` & `mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py` & `mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py` & `mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py` & `mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py` & `mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py` & `mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py` & `mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py` & `mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py` & `mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py` & `mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py` & `mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/mct_quantizers.egg-info/SOURCES.txt` & `mct-quantizers-1.1.0/mct_quantizers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.0.0.28052023.post92442/setup.py` & `mct-quantizers-1.1.0/setup.py`

 * *Files identical despite different names*

