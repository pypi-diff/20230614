# Comparing `tmp/molgraph-0.3.8.tar.gz` & `tmp/molgraph-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molgraph-0.3.8.tar", last modified: Thu Jun  8 16:06:27 2023, max compression
+gzip compressed data, was "molgraph-0.3.9.tar", last modified: Mon Jun 12 12:28:59 2023, max compression
```

## Comparing `molgraph-0.3.8.tar` & `molgraph-0.3.9.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.918886 molgraph-0.3.8/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2022-05-10 17:47:45.000000 molgraph-0.3.8/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)     5709 2023-06-08 16:06:27.918886 molgraph-0.3.8/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     4989 2023-06-08 14:54:16.000000 molgraph-0.3.8/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.902886 molgraph-0.3.8/molgraph/
--rw-rw-r--   0 alex      (1000) alex      (1000)      408 2022-09-20 11:35:03.000000 molgraph-0.3.8/molgraph/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      954 2022-09-20 11:35:03.000000 molgraph-0.3.8/molgraph/_filter_warnings.py
--rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-06-08 14:54:16.000000 molgraph-0.3.8/molgraph/_version.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.906886 molgraph-0.3.8/molgraph/chemistry/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1086 2022-09-20 11:35:03.000000 molgraph-0.3.8/molgraph/chemistry/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.906886 molgraph-0.3.8/molgraph/chemistry/benchmark/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-29 19:00:10.000000 molgraph-0.3.8/molgraph/chemistry/benchmark/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    36677 2022-08-02 17:30:01.000000 molgraph-0.3.8/molgraph/chemistry/benchmark/configs.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13653 2022-09-20 11:35:03.000000 molgraph-0.3.8/molgraph/chemistry/benchmark/datasets.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     8971 2022-09-02 12:17:48.000000 molgraph-0.3.8/molgraph/chemistry/benchmark/splitters.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10276 2022-09-20 11:35:03.000000 molgraph-0.3.8/molgraph/chemistry/benchmark/tf_records.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2718 2022-09-02 12:17:48.000000 molgraph-0.3.8/molgraph/chemistry/conformer_generator.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10471 2022-08-03 19:47:51.000000 molgraph-0.3.8/molgraph/chemistry/conformer_utils.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    15266 2022-09-20 11:35:03.000000 molgraph-0.3.8/molgraph/chemistry/encoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13722 2022-09-20 11:37:26.000000 molgraph-0.3.8/molgraph/chemistry/features.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    21456 2023-04-12 17:28:19.000000 molgraph-0.3.8/molgraph/chemistry/molecular_encoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1840 2022-09-02 12:44:02.000000 molgraph-0.3.8/molgraph/chemistry/ops.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2760 2023-04-06 16:32:34.000000 molgraph-0.3.8/molgraph/chemistry/vis.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.906886 molgraph-0.3.8/molgraph/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3823 2023-06-06 20:54:37.000000 molgraph-0.3.8/molgraph/layers/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.910886 molgraph-0.3.8/molgraph/layers/attentional/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:18.000000 molgraph-0.3.8/molgraph/layers/attentional/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    12448 2023-06-07 12:34:11.000000 molgraph-0.3.8/molgraph/layers/attentional/attentive_fp_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11175 2023-06-07 12:34:11.000000 molgraph-0.3.8/molgraph/layers/attentional/gat_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9188 2023-06-07 12:34:11.000000 molgraph-0.3.8/molgraph/layers/attentional/gated_gcn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11222 2023-06-07 12:34:11.000000 molgraph-0.3.8/molgraph/layers/attentional/gatv2_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10436 2023-06-07 12:34:11.000000 molgraph-0.3.8/molgraph/layers/attentional/gmm_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14857 2023-06-07 13:20:34.000000 molgraph-0.3.8/molgraph/layers/attentional/gt_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13283 2023-06-07 13:25:59.000000 molgraph-0.3.8/molgraph/layers/base.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.910886 molgraph-0.3.8/molgraph/layers/convolutional/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:16.000000 molgraph-0.3.8/molgraph/layers/convolutional/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9825 2023-06-07 12:59:58.000000 molgraph-0.3.8/molgraph/layers/convolutional/gcn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9663 2023-06-07 12:34:11.000000 molgraph-0.3.8/molgraph/layers/convolutional/gcnii_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10612 2023-06-07 13:00:51.000000 molgraph-0.3.8/molgraph/layers/convolutional/gin_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10508 2023-06-07 12:34:11.000000 molgraph-0.3.8/molgraph/layers/convolutional/graph_sage_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.910886 molgraph-0.3.8/molgraph/layers/geometric/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-10 12:47:57.000000 molgraph-0.3.8/molgraph/layers/geometric/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1613 2022-09-02 11:38:53.000000 molgraph-0.3.8/molgraph/layers/geometric/_radial_basis.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9364 2023-06-07 12:34:11.000000 molgraph-0.3.8/molgraph/layers/geometric/dtnn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10190 2023-06-07 12:34:11.000000 molgraph-0.3.8/molgraph/layers/geometric/gcf_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.910886 molgraph-0.3.8/molgraph/layers/message_passing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-23 17:04:39.000000 molgraph-0.3.8/molgraph/layers/message_passing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    16685 2023-06-08 14:54:16.000000 molgraph-0.3.8/molgraph/layers/message_passing/edge_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13978 2023-06-07 15:46:32.000000 molgraph-0.3.8/molgraph/layers/message_passing/mpnn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6419 2023-04-17 15:25:58.000000 molgraph-0.3.8/molgraph/layers/ops.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.910886 molgraph-0.3.8/molgraph/layers/positional_encoding/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:08.000000 molgraph-0.3.8/molgraph/layers/positional_encoding/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10713 2023-06-07 13:25:59.000000 molgraph-0.3.8/molgraph/layers/positional_encoding/laplacian.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.910886 molgraph-0.3.8/molgraph/layers/postprocessing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:18:09.000000 molgraph-0.3.8/molgraph/layers/postprocessing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2538 2023-06-07 15:46:32.000000 molgraph-0.3.8/molgraph/layers/postprocessing/dot_product_incident.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2008 2022-08-18 17:05:41.000000 molgraph-0.3.8/molgraph/layers/postprocessing/extract_field.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2983 2022-09-20 11:35:03.000000 molgraph-0.3.8/molgraph/layers/postprocessing/gather_incident.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.914886 molgraph-0.3.8/molgraph/layers/preprocessing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:11.000000 molgraph-0.3.8/molgraph/layers/preprocessing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11080 2023-06-06 21:11:15.000000 molgraph-0.3.8/molgraph/layers/preprocessing/center_scaling.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4557 2023-06-06 20:54:37.000000 molgraph-0.3.8/molgraph/layers/preprocessing/dropout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9592 2023-06-06 21:11:15.000000 molgraph-0.3.8/molgraph/layers/preprocessing/embedding_lookup.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4234 2023-06-06 21:11:15.000000 molgraph-0.3.8/molgraph/layers/preprocessing/masking.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11858 2023-06-06 21:11:15.000000 molgraph-0.3.8/molgraph/layers/preprocessing/min_max_scaling.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6753 2023-06-06 21:11:15.000000 molgraph-0.3.8/molgraph/layers/preprocessing/projection.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    20494 2023-06-06 21:11:15.000000 molgraph-0.3.8/molgraph/layers/preprocessing/standard_scaling.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.914886 molgraph-0.3.8/molgraph/layers/readout/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:24.000000 molgraph-0.3.8/molgraph/layers/readout/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6710 2023-05-26 15:46:41.000000 molgraph-0.3.8/molgraph/layers/readout/attentive_fp_readout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4628 2023-06-08 14:54:16.000000 molgraph-0.3.8/molgraph/layers/readout/node_readout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3296 2022-09-20 11:35:03.000000 molgraph-0.3.8/molgraph/layers/readout/segment_pool.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6250 2022-09-14 11:22:14.000000 molgraph-0.3.8/molgraph/layers/readout/set_gather.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5418 2022-09-14 10:36:59.000000 molgraph-0.3.8/molgraph/layers/readout/transformer_encoder.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.914886 molgraph-0.3.8/molgraph/losses/
--rw-rw-r--   0 alex      (1000) alex      (1000)      456 2022-08-09 16:26:08.000000 molgraph-0.3.8/molgraph/losses/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2192 2022-06-01 11:22:01.000000 molgraph-0.3.8/molgraph/losses/link_losses.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5182 2022-08-15 09:20:55.000000 molgraph-0.3.8/molgraph/losses/masked_losses.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.914886 molgraph-0.3.8/molgraph/metrics/
--rw-rw-r--   0 alex      (1000) alex      (1000)      342 2022-08-09 16:18:46.000000 molgraph-0.3.8/molgraph/metrics/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2071 2022-06-01 11:25:29.000000 molgraph-0.3.8/molgraph/metrics/masked_metrics.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      517 2022-06-01 11:21:46.000000 molgraph-0.3.8/molgraph/metrics/mean_relative_error.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.914886 molgraph-0.3.8/molgraph/models/
--rw-rw-r--   0 alex      (1000) alex      (1000)      486 2023-04-06 15:13:35.000000 molgraph-0.3.8/molgraph/models/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7765 2023-06-08 14:54:16.000000 molgraph-0.3.8/molgraph/models/dgin.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6947 2023-06-08 14:54:16.000000 molgraph-0.3.8/molgraph/models/dmpnn.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.914886 molgraph-0.3.8/molgraph/models/interpretability/
--rw-rw-r--   0 alex      (1000) alex      (1000)       84 2022-08-12 12:53:20.000000 molgraph-0.3.8/molgraph/models/interpretability/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      223 2022-07-14 20:09:09.000000 molgraph-0.3.8/molgraph/models/interpretability/_filter_warnings.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6733 2022-09-20 11:35:03.000000 molgraph-0.3.8/molgraph/models/interpretability/activation_maps.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11937 2022-09-20 11:35:03.000000 molgraph-0.3.8/molgraph/models/interpretability/saliency.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6854 2023-06-07 16:34:42.000000 molgraph-0.3.8/molgraph/models/mpnn.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.914886 molgraph-0.3.8/molgraph/models/pretraining/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-06-05 19:46:32.000000 molgraph-0.3.8/molgraph/models/pretraining/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-06-05 19:46:46.000000 molgraph-0.3.8/molgraph/models/pretraining/attribute_masking.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.918886 molgraph-0.3.8/molgraph/tensors/
--rw-rw-r--   0 alex      (1000) alex      (1000)      184 2022-08-08 12:38:45.000000 molgraph-0.3.8/molgraph/tensors/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    22917 2022-08-05 18:22:59.000000 molgraph-0.3.8/molgraph/tensors/_graph_tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1844 2022-08-18 15:00:21.000000 molgraph-0.3.8/molgraph/tensors/graph_keras_tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    40311 2023-06-08 14:54:16.000000 molgraph-0.3.8/molgraph/tensors/graph_tensor.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.906886 molgraph-0.3.8/molgraph.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)     5709 2023-06-08 16:06:27.000000 molgraph-0.3.8/molgraph.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     3448 2023-06-08 16:06:27.000000 molgraph-0.3.8/molgraph.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-06-08 16:06:27.000000 molgraph-0.3.8/molgraph.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       78 2023-06-08 16:06:27.000000 molgraph-0.3.8/molgraph.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-06-08 16:06:27.000000 molgraph-0.3.8/molgraph.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-06-08 16:06:27.918886 molgraph-0.3.8/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1510 2023-06-08 09:43:15.000000 molgraph-0.3.8/setup.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.918886 molgraph-0.3.8/tests/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3633 2022-09-20 11:35:03.000000 molgraph-0.3.8/tests/test_chemistry.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    15601 2022-09-20 11:35:03.000000 molgraph-0.3.8/tests/test_interpretability.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    15816 2023-06-08 14:54:16.000000 molgraph-0.3.8/tests/test_layers.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3425 2023-04-06 13:54:41.000000 molgraph-0.3.8/tests/test_models.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2409 2023-04-06 15:41:44.000000 molgraph-0.3.8/tests/test_models_2.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    17467 2023-05-30 09:41:48.000000 molgraph-0.3.8/tests/test_tensors.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11741 2023-05-30 09:41:50.000000 molgraph-0.3.8/tests/test_tensors_2.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11755 2023-05-30 09:41:51.000000 molgraph-0.3.8/tests/test_tensors_3.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    12678 2023-05-30 09:41:54.000000 molgraph-0.3.8/tests/test_tensors_4.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-12 12:28:59.981851 molgraph-0.3.9/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2022-05-10 17:47:45.000000 molgraph-0.3.9/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5709 2023-06-12 12:28:59.981851 molgraph-0.3.9/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4989 2023-06-08 14:54:16.000000 molgraph-0.3.9/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-12 12:28:59.973851 molgraph-0.3.9/molgraph/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      407 2023-06-12 12:15:52.000000 molgraph-0.3.9/molgraph/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      964 2023-06-12 12:25:23.000000 molgraph-0.3.9/molgraph/_filter_warnings.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/_version.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-12 12:28:59.977851 molgraph-0.3.9/molgraph/chemistry/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1086 2022-09-20 11:35:03.000000 molgraph-0.3.9/molgraph/chemistry/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-12 12:28:59.977851 molgraph-0.3.9/molgraph/chemistry/benchmark/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-29 19:00:10.000000 molgraph-0.3.9/molgraph/chemistry/benchmark/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    36677 2022-08-02 17:30:01.000000 molgraph-0.3.9/molgraph/chemistry/benchmark/configs.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13653 2022-09-20 11:35:03.000000 molgraph-0.3.9/molgraph/chemistry/benchmark/datasets.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     8971 2022-09-02 12:17:48.000000 molgraph-0.3.9/molgraph/chemistry/benchmark/splitters.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10276 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/chemistry/benchmark/tf_records.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2718 2022-09-02 12:17:48.000000 molgraph-0.3.9/molgraph/chemistry/conformer_generator.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10471 2022-08-03 19:47:51.000000 molgraph-0.3.9/molgraph/chemistry/conformer_utils.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    15266 2022-09-20 11:35:03.000000 molgraph-0.3.9/molgraph/chemistry/encoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13722 2022-09-20 11:37:26.000000 molgraph-0.3.9/molgraph/chemistry/features.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    21484 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/chemistry/molecular_encoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1840 2022-09-02 12:44:02.000000 molgraph-0.3.9/molgraph/chemistry/ops.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2760 2023-04-06 16:32:34.000000 molgraph-0.3.9/molgraph/chemistry/vis.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-12 12:28:59.977851 molgraph-0.3.9/molgraph/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3823 2023-06-06 20:54:37.000000 molgraph-0.3.9/molgraph/layers/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-12 12:28:59.977851 molgraph-0.3.9/molgraph/layers/attentional/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:18.000000 molgraph-0.3.9/molgraph/layers/attentional/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    12067 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/layers/attentional/attentive_fp_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11105 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/layers/attentional/gat_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9083 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/layers/attentional/gated_gcn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11152 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/layers/attentional/gatv2_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10340 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/layers/attentional/gmm_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14777 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/layers/attentional/gt_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13201 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/layers/base.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-12 12:28:59.977851 molgraph-0.3.9/molgraph/layers/convolutional/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:16.000000 molgraph-0.3.9/molgraph/layers/convolutional/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9726 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/layers/convolutional/gcn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9564 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/layers/convolutional/gcnii_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10546 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/layers/convolutional/gin_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10024 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/layers/convolutional/graph_sage_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-12 12:28:59.977851 molgraph-0.3.9/molgraph/layers/geometric/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-10 12:47:57.000000 molgraph-0.3.9/molgraph/layers/geometric/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1613 2022-09-02 11:38:53.000000 molgraph-0.3.9/molgraph/layers/geometric/_radial_basis.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9189 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/layers/geometric/dtnn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10090 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/layers/geometric/gcf_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-12 12:28:59.977851 molgraph-0.3.9/molgraph/layers/message_passing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-23 17:04:39.000000 molgraph-0.3.9/molgraph/layers/message_passing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    16398 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/layers/message_passing/edge_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13721 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/layers/message_passing/mpnn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6419 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/layers/ops.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-12 12:28:59.977851 molgraph-0.3.9/molgraph/layers/positional_encoding/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:08.000000 molgraph-0.3.9/molgraph/layers/positional_encoding/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10716 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/layers/positional_encoding/laplacian.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-12 12:28:59.977851 molgraph-0.3.9/molgraph/layers/postprocessing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:18:09.000000 molgraph-0.3.9/molgraph/layers/postprocessing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3398 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/layers/postprocessing/dot_product_incident.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2013 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/layers/postprocessing/extract_field.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2983 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/layers/postprocessing/gather_incident.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-12 12:28:59.981851 molgraph-0.3.9/molgraph/layers/preprocessing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:11.000000 molgraph-0.3.9/molgraph/layers/preprocessing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10911 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/layers/preprocessing/center_scaling.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4557 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/layers/preprocessing/dropout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9518 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/layers/preprocessing/embedding_lookup.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4234 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/layers/preprocessing/masking.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11744 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/layers/preprocessing/min_max_scaling.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6665 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/layers/preprocessing/projection.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    20392 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/layers/preprocessing/standard_scaling.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-12 12:28:59.981851 molgraph-0.3.9/molgraph/layers/readout/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:24.000000 molgraph-0.3.9/molgraph/layers/readout/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6390 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/layers/readout/attentive_fp_readout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4628 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/layers/readout/node_readout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3285 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/layers/readout/segment_pool.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6239 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/layers/readout/set_gather.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5396 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/layers/readout/transformer_encoder.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-12 12:28:59.981851 molgraph-0.3.9/molgraph/losses/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      456 2022-08-09 16:26:08.000000 molgraph-0.3.9/molgraph/losses/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2236 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/losses/link_losses.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5212 2023-06-12 11:43:48.000000 molgraph-0.3.9/molgraph/losses/masked_losses.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-12 12:28:59.981851 molgraph-0.3.9/molgraph/metrics/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      342 2022-08-09 16:18:46.000000 molgraph-0.3.9/molgraph/metrics/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2071 2023-06-12 10:24:19.000000 molgraph-0.3.9/molgraph/metrics/masked_metrics.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      518 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/metrics/mean_relative_error.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-12 12:28:59.981851 molgraph-0.3.9/molgraph/models/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      486 2023-04-06 15:13:35.000000 molgraph-0.3.9/molgraph/models/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7765 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/models/dgin.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6947 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/models/dmpnn.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-12 12:28:59.981851 molgraph-0.3.9/molgraph/models/interpretability/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       84 2022-08-12 12:53:20.000000 molgraph-0.3.9/molgraph/models/interpretability/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      223 2022-07-14 20:09:09.000000 molgraph-0.3.9/molgraph/models/interpretability/_filter_warnings.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6733 2022-09-20 11:35:03.000000 molgraph-0.3.9/molgraph/models/interpretability/activation_maps.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11937 2023-06-12 10:24:43.000000 molgraph-0.3.9/molgraph/models/interpretability/saliency.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6865 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/models/mpnn.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-12 12:28:59.981851 molgraph-0.3.9/molgraph/models/pretraining/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-06-05 19:46:32.000000 molgraph-0.3.9/molgraph/models/pretraining/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-06-05 19:46:46.000000 molgraph-0.3.9/molgraph/models/pretraining/attribute_masking.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-12 12:28:59.981851 molgraph-0.3.9/molgraph/tensors/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      184 2022-08-08 12:38:45.000000 molgraph-0.3.9/molgraph/tensors/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    22917 2022-08-05 18:22:59.000000 molgraph-0.3.9/molgraph/tensors/_graph_tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1844 2022-08-18 15:00:21.000000 molgraph-0.3.9/molgraph/tensors/graph_keras_tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    42515 2023-06-12 11:28:34.000000 molgraph-0.3.9/molgraph/tensors/graph_tensor.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-12 12:28:59.977851 molgraph-0.3.9/molgraph.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5709 2023-06-12 12:28:59.000000 molgraph-0.3.9/molgraph.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3448 2023-06-12 12:28:59.000000 molgraph-0.3.9/molgraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-06-12 12:28:59.000000 molgraph-0.3.9/molgraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       78 2023-06-12 12:28:59.000000 molgraph-0.3.9/molgraph.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-06-12 12:28:59.000000 molgraph-0.3.9/molgraph.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-06-12 12:28:59.981851 molgraph-0.3.9/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1510 2023-06-08 09:43:15.000000 molgraph-0.3.9/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-12 12:28:59.981851 molgraph-0.3.9/tests/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3638 2023-06-12 11:28:34.000000 molgraph-0.3.9/tests/test_chemistry.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    15601 2022-09-20 11:35:03.000000 molgraph-0.3.9/tests/test_interpretability.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    15816 2023-06-08 14:54:16.000000 molgraph-0.3.9/tests/test_layers.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3425 2023-04-06 13:54:41.000000 molgraph-0.3.9/tests/test_models.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2409 2023-04-06 15:41:44.000000 molgraph-0.3.9/tests/test_models_2.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    17494 2023-06-12 11:28:34.000000 molgraph-0.3.9/tests/test_tensors.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11741 2023-05-30 09:41:50.000000 molgraph-0.3.9/tests/test_tensors_2.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11755 2023-05-30 09:41:51.000000 molgraph-0.3.9/tests/test_tensors_3.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    12678 2023-05-30 09:41:54.000000 molgraph-0.3.9/tests/test_tensors_4.py
```

### Comparing `molgraph-0.3.8/LICENSE` & `molgraph-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.8/PKG-INFO` & `molgraph-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgraph
-Version: 0.3.8
+Version: 0.3.9
 Summary: Implementations of graph neural networks for molecular machine learning
 Home-page: https://github.com/akensert/molgraph
 Author: Alexander Kensert
 Author-email: alexander.kensert@gmail.com
 License: MIT
 Keywords: graph-neural-networks,deep-learning,machine-learning,molecular-machine-learning,molecular-graphs,cheminformatics,bioinformatics
 Classifier: Programming Language :: Python :: 3
```

### Comparing `molgraph-0.3.8/README.md` & `molgraph-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.8/molgraph/_filter_warnings.py` & `molgraph-0.3.9/molgraph/_filter_warnings.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from warnings import filterwarnings
+# from warnings import filterwarnings
 
-filterwarnings('ignore',
-    message='Converting sparse IndexedSlices.*' +
-            'to a dense Tensor of unknown shape. ' +
-            'This may consume a large amount of memory.')
+# filterwarnings('ignore',
+#     message='Converting sparse IndexedSlices.*' +
+#             'to a dense Tensor of unknown shape. ' +
+#             'This may consume a large amount of memory.')
 
 import logging
 #logging.getLogger('tensorflow').setLevel(logging.ERROR)
 logging.basicConfig(level=logging.INFO, format='%(message)s')
 
 def ignore_gradient_warning(record):
     # If e.g. `update_edge_features` is passed to the last GAT layer, edge
```

### Comparing `molgraph-0.3.8/molgraph/chemistry/__init__.py` & `molgraph-0.3.9/molgraph/chemistry/__init__.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.8/molgraph/chemistry/benchmark/configs.py` & `molgraph-0.3.9/molgraph/chemistry/benchmark/configs.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.8/molgraph/chemistry/benchmark/datasets.py` & `molgraph-0.3.9/molgraph/chemistry/benchmark/datasets.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.8/molgraph/chemistry/benchmark/splitters.py` & `molgraph-0.3.9/molgraph/chemistry/benchmark/splitters.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.8/molgraph/chemistry/benchmark/tf_records.py` & `molgraph-0.3.9/molgraph/chemistry/benchmark/tf_records.py`

 * *Files 1% similar despite different names*

```diff
@@ -282,13 +282,13 @@
 
     data = tf.nest.map_structure(
         lambda x, s: tf.ensure_shape(
             tf.io.parse_tensor(x, s.dtype), s.shape), example, specs)
 
     x_spec = tf.nest.map_structure(
         lambda spec: tf.RaggedTensorSpec(
-            spec.shape, spec.dtype, 0, x['edge_dst'].dtype),
+            spec.shape, spec.dtype, 0, x['edge_src'].dtype),
         x_spec._data_spec)
     data['x'] = GraphTensor(x, x_spec)
     if extract_tuple is not None:
         data = tuple(data[key] for key in extract_tuple if key in data)
     return data
```

### Comparing `molgraph-0.3.8/molgraph/chemistry/conformer_generator.py` & `molgraph-0.3.9/molgraph/chemistry/conformer_generator.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.8/molgraph/chemistry/conformer_utils.py` & `molgraph-0.3.9/molgraph/chemistry/conformer_utils.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.8/molgraph/chemistry/encoders.py` & `molgraph-0.3.9/molgraph/chemistry/encoders.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.8/molgraph/chemistry/features.py` & `molgraph-0.3.9/molgraph/chemistry/features.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.8/molgraph/chemistry/molecular_encoders.py` & `molgraph-0.3.9/molgraph/chemistry/molecular_encoders.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
                 graph_tensor_list = [
                     gt for gt in graph_tensor_list if gt is not None]
 
                 # The list of `GraphTensor`s is concatenated to generate a single
                 # `GraphTensor` (disjoint [molecular] graph). The `separate` method
                 # is called to make the nested structures of the `GraphTensor`
                 # ragged. This will allow for batching of the `GraphTensor`.
-                return tf.concat(graph_tensor_list, axis=0).separate()
+                return tf.stack(graph_tensor_list, axis=0)
 
             return self.call(inputs, **kwargs)
 
 
 @dataclass
 class MolecularGraphEncoder(BaseMolecularGraphEncoder):
 
@@ -144,19 +144,19 @@
     ...     self_loops=False
     ... )
     >>> # Encode two molecules as a GraphTensor
     >>> graph_tensor = encoder(['CCC', 'CCO'])
     >>> # Merge subgraphs into a single disjoint graph
     >>> graph_tensor.merge()
     GraphTensor(
+      edge_src=<tf.Tensor: shape=(8,), dtype=int32>,
+      edge_dst=<tf.Tensor: shape=(8,), dtype=int32>,
       node_feature=<tf.Tensor: shape=(6, 119), dtype=float32>,
       edge_feature=<tf.Tensor: shape=(8, 4), dtype=float32>,
       positional_encoding=<tf.Tensor: shape=(6, 10), dtype=float32>,
-      edge_dst=<tf.Tensor: shape=(8,), dtype=int32>,
-      edge_src=<tf.Tensor: shape=(8,), dtype=int32>,
       graph_indicator=<tf.Tensor: shape=(6,), dtype=int32>)
 
     Generate a molecular graph with tokenizers:
 
     >>> # Define bond featurizer (to produce numerical encoding of atoms)
     >>> atom_tokenizer = molgraph.chemistry.Tokenizer([
     ...     molgraph.chemistry.features.Symbol(),
@@ -176,21 +176,22 @@
     ...     self_loops=False
     ... )
     >>> # Encode two molecules as a GraphTensor
     >>> graph_tensor = encoder(['CCC', 'CCO'])
     >>> # Merge subgraphs into a single disjoint graph
     >>> graph_tensor.merge()
     GraphTensor(
+      edge_src=<tf.Tensor: shape=(8,), dtype=int32>,
+      edge_dst=<tf.Tensor: shape=(8,), dtype=int32>,
       node_feature=<tf.Tensor: shape=(6,), dtype=string>,
       edge_feature=<tf.Tensor: shape=(8,), dtype=string>,
       positional_encoding=<tf.Tensor: shape=(6, 10), dtype=float32>,
-      edge_dst=<tf.Tensor: shape=(8,), dtype=int32>,
-      edge_src=<tf.Tensor: shape=(8,), dtype=int32>,
       graph_indicator=<tf.Tensor: shape=(6,), dtype=int32>)
 
+
     Obtain numerical encodings of atoms (``node_feature``) and bonds
     (``bond_feature``) with the EmbeddingLookup layer. This is only necessary
     when tokenizers are used to compute ``node_feature`` and ``edge_feature``:
 
     >>> # Define bond featurizer (to produce numerical encoding of atoms)
     >>> atom_tokenizer = molgraph.chemistry.Tokenizer([
     ...    molgraph.chemistry.features.Symbol(),
@@ -225,21 +226,20 @@
     ...    node_embedding,
     ...    edge_embedding,
     ... ])
     >>> # Pass GraphTensor to model
     >>> graph_tensor = model(graph_tensor)
     >>> graph_tensor
     GraphTensor(
+      edge_src=<tf.Tensor: shape=(8,), dtype=int32>,
+      edge_dst=<tf.Tensor: shape=(8,), dtype=int32>,
       node_feature=<tf.Tensor: shape=(6, 16), dtype=float32>,
       edge_feature=<tf.Tensor: shape=(8, 8), dtype=float32>,
       positional_encoding=<tf.Tensor: shape=(6, 10), dtype=float32>,
-      edge_dst=<tf.Tensor: shape=(8,), dtype=int32>,
-      edge_src=<tf.Tensor: shape=(8,), dtype=int32>,
       graph_indicator=<tf.Tensor: shape=(6,), dtype=int32>)
-
     '''
 
     bond_encoder: Optional[Union[
         Featurizer, Tokenizer, Callable]] = None
     molecule_from_string_fn: Callable[[str], Chem.Mol] = field(
         default_factory=lambda: partial(molecule_from_string, catch_errors=True),
         repr=False
@@ -273,15 +273,15 @@
 
         # Initialize data dictionary
         data = {}
 
         # Obtain destination and source node (atom) indices of edges (bonds)
         sparse_adjacency = _compute_adjacency(
             molecule, self.self_loops, sparse=True, dtype=index_dtype)
-        data['edge_dst'], data['edge_src'] = sparse_adjacency
+        data['edge_src'], data['edge_dst'] = sparse_adjacency
 
         # Obtain node (atom) features
         atoms = _get_atoms(molecule)
         data['node_feature'] = self.atom_encoder(atoms)
 
         # Obtain edge (bond) features (if `bond_encoder` exist)
         if self.bond_encoder is not None:
@@ -394,24 +394,24 @@
         data = {}
 
         dg = _compute_distance_geometry(
             molecule, radius=self.edge_radius)
 
         atoms = _get_atoms(molecule)
         data['node_feature'] = self.atom_encoder(atoms)
-        data['edge_dst'] = np.array(dg['edge_dst'], dtype=index_dtype)
         data['edge_src'] = np.array(dg['edge_src'], dtype=index_dtype)
-
+        data['edge_dst'] = np.array(dg['edge_dst'], dtype=index_dtype)
+        
         if not self.coulomb:
             edge_feature = np.expand_dims(dg['edge_length'], -1)
         else:
             nuclear_charge = np.array([
                 atom.GetAtomicNum() for atom in atoms], dtype=np.float32)
-            nuclear_charge_dst = np.take(nuclear_charge, dg['edge_dst'])
             nuclear_charge_src = np.take(nuclear_charge, dg['edge_src'])
+            nuclear_charge_dst = np.take(nuclear_charge, dg['edge_dst'])
             edge_feature = (
                 nuclear_charge_dst * nuclear_charge_src) / dg['edge_length']
             edge_feature = np.expand_dims(edge_feature, -1)
 
         data['edge_feature'] = np.array(edge_feature, dtype=np.float32)
 
         return GraphTensor(data)
@@ -419,24 +419,24 @@
 
 def _get_atoms(molecule: Chem.Mol) -> List[Chem.Atom]:
     'Returns a list of atoms given an RDKit mol object.'
     return list(molecule.GetAtoms())
 
 def _get_bonds(
     molecule: Chem.Mol,
+    edge_src: np.ndarray,
     edge_dst: np.ndarray,
-    edge_src: np.ndarray
 ) -> List[Chem.Bond]:
     '''Returns a list of bonds given an RDKit mol object. The order of the
     bonds in the list corresponds to the sparse adjacency matrix which is
     also part of the resulting `GraphTensor`.
     '''
     return [
         molecule.GetBondBetweenAtoms(int(i), int(j))
-        for (i, j) in zip(edge_dst, edge_src)
+        for (i, j) in zip(edge_src, edge_dst)
     ]
 
 def _compute_positional_encoding(
     molecule: Chem.Mol,
     dim: int = 20,
     dtype: np.dtype = np.float32,
 ) -> np.ndarray:
@@ -498,17 +498,17 @@
 
     if self_loops:
         adjacency += np.eye(adjacency.shape[0], dtype=adjacency.dtype)
 
     if not sparse:
         return adjacency.astype(dtype)
 
-    bond_dst, bond_src = np.where(adjacency)
+    edge_src, edge_dst = np.where(adjacency)
 
-    return bond_dst.astype(dtype), bond_src.astype(dtype)
+    return edge_src.astype(dtype), edge_dst.astype(dtype)
 
 def _compute_laplacian(
     adjacency: np.ndarray,
     dtype: np.dtype = np.float32
 ) -> np.ndarray:
     'Computes the laplacian matrix an adjacency matrix.'
     degree = np.sum(adjacency, axis=1)
@@ -517,24 +517,24 @@
     degree = np.diag(degree)
     adjacency = degree.dot(adjacency).dot(degree)
     laplacian = np.eye(adjacency.shape[0]) - adjacency
     return laplacian.astype(dtype)
 
 def _compute_distance_between_atoms(
     molecule: Chem.Mol,
-    edge_dst: int,
     edge_src: int,
+    edge_dst: int,
     unit: str
 ) -> float:
     'Computes distance between two atoms in the molecule.'
-    bond_length = Chem.rdMolTransforms.GetBondLength(
-        molecule.GetConformer(), edge_dst, edge_src)
+    edge_length = Chem.rdMolTransforms.GetBondLength(
+        molecule.GetConformer(), edge_src, edge_dst)
     if unit.lower() == 'bohr':
-        return bond_length * 1.8897259885789
-    return bond_length
+        return edge_length * 1.8897259885789
+    return edge_length
 
 def _compute_distance_geometry(
     molecule: Chem.Mol,
     radius: Optional[int] = None,
     unit: str = 'angstrom',
     atom: Union[Chem.Atom, None] = None,
     path: Union[List[int], None] = None,
@@ -544,26 +544,29 @@
     '''Recursively navigates paths (in molecule) up to a certain `radius` to
     accumulate distance geometric information. If radius is None, the distance
     between every atom in the molecule will be computed.
     '''
 
     if path is None:
         data = {
-            'edge_length': [], 'edge_dst': [], 'edge_src': [], 'edge_order': []}
+            'edge_length': [], 'edge_src': [], 'edge_dst': [], 'edge_order': []
+        }
         for atom in molecule.GetAtoms():
             path = _compute_distance_geometry(
-                molecule, radius, unit, atom, [atom.GetIdx()], data)
+                molecule, radius, unit, atom, [atom.GetIdx()], data
+            )
         return data
     elif radius and len(path) > (radius + 1):
         return path[:-1]
     elif len(path) > 1:
-        data['edge_dst'].append(path[0])
-        data['edge_src'].append(path[-1])
+        data['edge_src'].append(path[0])
+        data['edge_dst'].append(path[-1])
         data['edge_length'].append(
-            _compute_distance_between_atoms(molecule, path[0], path[-1], unit))
+            _compute_distance_between_atoms(molecule, path[0], path[-1], unit)
+        )
         data['edge_order'].append(-1 + len(path))
 
     for neighbor in atom.GetNeighbors():
         if neighbor.GetIdx() not in path:
             path.append(neighbor.GetIdx())
             path = _compute_distance_geometry(
                 molecule, radius, unit, neighbor, path, data)
```

### Comparing `molgraph-0.3.8/molgraph/chemistry/ops.py` & `molgraph-0.3.9/molgraph/chemistry/ops.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.8/molgraph/chemistry/vis.py` & `molgraph-0.3.9/molgraph/chemistry/vis.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.8/molgraph/layers/__init__.py` & `molgraph-0.3.9/molgraph/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.8/molgraph/layers/attentional/attentive_fp_conv.py` & `molgraph-0.3.9/molgraph/layers/attentional/attentive_fp_conv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,19 @@
 import tensorflow as tf
 from tensorflow import keras
-from keras.utils import tf_utils
-from tensorflow.keras import initializers
-from tensorflow.keras import regularizers
-from tensorflow.keras import constraints
-from tensorflow.keras import activations
-
+from keras import initializers
+from keras import regularizers
+from keras import constraints
 
 from typing import Optional
 from typing import Callable
 from typing import Union
-from typing import Tuple
-from typing import Type
 from typing import TypeVar
 
 from molgraph.tensors.graph_tensor import GraphTensor
-from molgraph.layers.base import BaseLayer
-from molgraph.layers.ops import softmax_edge_weights
-from molgraph.layers.ops import propagate_node_features
-from molgraph.layers.ops import reduce_features
 from molgraph.layers.attentional.gat_conv import GATConv
 
 
 Config = TypeVar('Config', bound=dict)
 
 
 @keras.utils.register_keras_serializable(package='molgraph')
@@ -40,16 +31,16 @@
 
     **Examples:**
 
     Inputs a ``GraphTensor`` encoding (two) subgraphs:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'edge_src': [[1, 0], [1, 2, 0, 2, 1, 0]],
+    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'node_feature': [
     ...             [[1.0, 0.0], [1.0, 0.0]],
     ...             [[1.0, 0.0], [1.0, 0.0], [0.0, 1.0]]
     ...         ],
     ...         'edge_feature': [
     ...             [[1.0, 0.0], [0.0, 1.0]],
     ...             [[0.0, 1.0], [0.0, 1.0], [1.0, 0.0],
@@ -66,16 +57,16 @@
     >>> gnn_model.output_shape
     (None, None, 16)
 
     Inputs a ``GraphTensor`` encoding a single disjoint graph:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'node_feature': [
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [0.0, 1.0]
     ...         ],
@@ -101,16 +92,16 @@
     >>> gnn_model.output_shape
     (None, 16)
 
     Create a complete AttentiveFP model:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'node_feature': [
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [0.0, 1.0]
     ...         ],
@@ -133,21 +124,20 @@
     ...     molgraph.layers.AttentiveFPConv(16, apply_initial_node_projection=True),
     ...     molgraph.layers.AttentiveFPConv(16),
     ...     molgraph.layers.AttentiveFPReadout(),
     ... ])
     >>> attentive_fp(graph_tensor).shape.as_list()
     [2, 16]
 
-
     Pass the same GRU cell to each layer to perform weight sharing:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'node_feature': [
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [0.0, 1.0]
     ...         ],
@@ -171,15 +161,14 @@
     ...     molgraph.layers.AttentiveFPConv(
     ...         16, apply_initial_node_projection=True, gru_cell=gru_cell),
     ...     molgraph.layers.AttentiveFPConv(16, gru_cell=gru_cell)
     ... ])
     >>> gnn_model.output_shape
     (None, 16)
 
-
     Args:
         units (int, None):
             Number of output units.
         apply_initial_node_projection (bool):
             Whether to perform an initial linear transformation on node features.
             Should be set to True for the first AttentiveFPConv layer in a sequence
             of AttentiveFPConv layers. Note that a node projection automatically 
@@ -224,15 +213,14 @@
         kernel_constraint (tf.keras.constraints.Constraint, None):
             Constraint function applied to the kernels. Default to None.
         bias_constraint (tf.keras.constraints.Constraint, None):
             Constraint function applied to the biases. Default to None.
 
     References:
         .. [#] https://pubs.acs.org/doi/10.1021/acs.jmedchem.9b00959
-
     '''
 
     def __init__(
         self,
         units: Optional[int] = None,
         apply_initial_node_projection: bool = False,
         gru_cell: Optional[tf.keras.layers.GRUCell] = None,
@@ -295,16 +283,15 @@
         if not isinstance(self.gru_cell, tf.keras.layers.GRUCell):
             self.gru_cell = tf.keras.layers.GRUCell(self.units)
 
     def subclass_call(self, tensor: GraphTensor) -> GraphTensor:
 
         if self.initial_projection is not None:
             tensor = tensor.update({
-                'node_feature': self.initial_projection(
-                    tensor.node_feature)
+                'node_feature': self.initial_projection(tensor.node_feature)
             })
 
         node_feature_state = tensor.node_feature
 
         tensor = super().subclass_call(tensor)
         
         node_feature_state, _ = self.gru_cell(
```

### Comparing `molgraph-0.3.8/molgraph/layers/attentional/gat_conv.py` & `molgraph-0.3.9/molgraph/layers/attentional/gatv2_conv.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,70 +1,67 @@
 import tensorflow as tf
 from tensorflow import keras
-from tensorflow.keras import initializers
-from tensorflow.keras import regularizers
-from tensorflow.keras import constraints
-from tensorflow.keras import activations
-
+from keras import initializers
+from keras import regularizers
+from keras import constraints
+from keras import activations
 
 from typing import Optional
 from typing import Callable
 from typing import Union
-from typing import Tuple
 
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.layers.base import BaseLayer
 from molgraph.layers.ops import softmax_edge_weights
 from molgraph.layers.ops import propagate_node_features
 from molgraph.layers.ops import reduce_features
 
 
 
 @keras.utils.register_keras_serializable(package='molgraph')
-class GATConv(BaseLayer):
+class GATv2Conv(BaseLayer):
 
-    '''Multi-head graph attention layer (GAT).
+    '''Multi-head graph attention (v2) layer (GATv2).
 
-    The implementation is based on Velickovic et al. (2018) [#]_ and
-    Dwivedi et al. (2022) [#]_.
+    The implementation is based on Brody et al. (2021) [#]_.
 
     **Examples:**
 
     Inputs a ``GraphTensor`` encoding (two) subgraphs:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'edge_src': [[1, 0], [1, 2, 0, 2, 1, 0]],
+    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'node_feature': [
     ...             [[1.0, 0.0], [1.0, 0.0]],
     ...             [[1.0, 0.0], [1.0, 0.0], [0.0, 1.0]]
     ...         ],
     ...         'edge_feature': [
     ...             [[1.0, 0.0], [0.0, 1.0]],
     ...             [[0.0, 1.0], [0.0, 1.0], [1.0, 0.0],
     ...              [0.0, 1.0], [1.0, 0.0], [0.0, 1.0]]
     ...         ],
     ...     }
     ... )
-    >>> # Build a model with GATConv
+    >>> # Build a model with GATv2Conv
     >>> gnn_model = tf.keras.Sequential([
     ...     tf.keras.Input(type_spec=graph_tensor.unspecific_spec),
-    ...     molgraph.layers.GATConv(16, activation='relu'),
-    ...     molgraph.layers.GATConv(16, activation='relu')
+    ...     molgraph.layers.GATv2Conv(16, activation='relu'),
+    ...     molgraph.layers.GATv2Conv(16, activation='relu')
     ... ])
     >>> gnn_model.output_shape
     (None, None, 16)
 
     Inputs a ``GraphTensor`` encoding a single disjoint graph:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'node_feature': [
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [0.0, 1.0]
     ...         ],
@@ -77,19 +74,19 @@
     ...             [1.0, 0.0],
     ...             [0.0, 1.0],
     ...             [1.0, 0.0],
     ...             [0.0, 1.0]
     ...         ],
     ...     }
     ... )
-    >>> # Build a model with GATConv
+    >>> # Build a model with GATv2Conv
     >>> gnn_model = tf.keras.Sequential([
     ...     tf.keras.Input(type_spec=graph_tensor.unspecific_spec),
-    ...     molgraph.layers.GATConv(16, activation='relu'),
-    ...     molgraph.layers.GATConv(16, activation='relu')
+    ...     molgraph.layers.GATv2Conv(16, activation='relu'),
+    ...     molgraph.layers.GATv2Conv(16, activation='relu')
     ... ])
     >>> gnn_model.output_shape
     (None, 16)
 
     Args:
         units (int, None):
             Number of output units.
@@ -131,16 +128,15 @@
             Default to None.
         kernel_constraint (tf.keras.constraints.Constraint, None):
             Constraint function applied to the kernels. Default to None.
         bias_constraint (tf.keras.constraints.Constraint, None):
             Constraint function applied to the biases. Default to None.
 
     References:
-        .. [#] https://arxiv.org/pdf/1710.10903.pdf
-        .. [#] https://arxiv.org/pdf/2003.00982.pdf
+        .. [#] https://arxiv.org/pdf/2105.14491.pdf
 
     '''
 
     def __init__(
         self,
         units: Optional[int] = 128,
         use_edge_features: bool = True,
@@ -182,15 +178,14 @@
             bias_constraint=bias_constraint,
             **kwargs)
 
         self.use_edge_features = use_edge_features
         self.num_heads = num_heads
         self.merge_mode = merge_mode
         self.apply_self_projection = self_projection
-        self.activation = activations.get('elu')
         self.attention_activation = activations.get(attention_activation)
 
     def subclass_build(
         self,
         node_feature_shape: Optional[tf.TensorShape] = None,
         edge_feature_shape: Optional[tf.TensorShape] = None
     ) -> None:
@@ -210,14 +205,16 @@
             self.edge_projection = self.get_einsum_dense(
                 'ij,jkh->ihk', (self.num_heads, self.units))
 
             if self.update_edge_features:
                 self.edge_out_projection = self.get_einsum_dense(
                     'ihj,jkh->ihk', (self.num_heads, self.units))
 
+        # Future implementation: Allow for non-shared weights?
+        # I.e., implement node_projection_dst and node_projection_src
         self.node_projection = self.get_einsum_dense(
             'ij,jkh->ihk', (self.num_heads, self.units))
 
         if self.apply_self_projection:
             self.self_projection = self.get_einsum_dense(
                 'ij,jkh->ihk', (self.num_heads, self.units))
 
@@ -225,50 +222,51 @@
             'ihj,jhk->ihk', (self.num_heads, 1))
 
         if self.merge_mode == 'concat':
             self.units *= self.num_heads
 
     def subclass_call(self, tensor: GraphTensor) -> GraphTensor:
 
-        # Edge dependent (i.e., `tensor.edge_src is not None`), from here
         node_feature = self.node_projection(tensor.node_feature)
-
-        attention_feature = tf.concat([
-            tf.gather(node_feature, tensor.edge_dst),
-            tf.gather(node_feature, tensor.edge_src)], axis=-1)
-
+        # Add dst and src node features, instead of concatenating them
+        attention_feature = (
+            tf.gather(node_feature, tensor.edge_dst) +
+            tf.gather(node_feature, tensor.edge_src)
+        )
         if self.use_edge_features:
             edge_feature = self.edge_projection(tensor.edge_feature)
-            attention_feature = tf.concat([attention_feature, edge_feature], axis=-1)
+            # Similarily, add associated edge features, instead of concatenating them
+            attention_feature += edge_feature
 
             if self.update_edge_features:
                 edge_feature = self.edge_out_projection(attention_feature)
                 edge_feature = reduce_features(
                     feature=edge_feature,
                     mode=self.merge_mode,
                     output_units=self.units)
+
                 tensor = tensor.update({'edge_feature': edge_feature})
 
-        edge_weights = self.attention_projection(attention_feature)
-        edge_weights = self.attention_activation(edge_weights)
+        # Apply activation before attention projection
+        edge_weights = self.attention_activation(attention_feature)
+        edge_weights = self.attention_projection(edge_weights)
+
         edge_weights = softmax_edge_weights(
             edge_weight=edge_weights,
             edge_dst=tensor.edge_dst)
 
         node_feature = propagate_node_features(
             node_feature=node_feature,
-            edge_dst=tensor.edge_dst,
             edge_src=tensor.edge_src,
+            edge_dst=tensor.edge_dst,
             edge_weight=edge_weights)
 
         if self.apply_self_projection:
             node_feature += self.self_projection(tensor.node_feature)
 
-        node_feature = self.activation(node_feature)
-
         node_feature = reduce_features(
             feature=node_feature,
             mode=self.merge_mode,
             output_units=self.units)
 
         return tensor.update({'node_feature': node_feature})
```

### Comparing `molgraph-0.3.8/molgraph/layers/attentional/gated_gcn_conv.py` & `molgraph-0.3.9/molgraph/layers/attentional/gated_gcn_conv.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import tensorflow as tf
 from tensorflow import keras
-from tensorflow.keras import initializers
-from tensorflow.keras import regularizers
-from tensorflow.keras import constraints
-from tensorflow.keras import activations
-from tensorflow.keras import layers
+from keras import initializers
+from keras import regularizers
+from keras import constraints
+from keras import activations
 
 from typing import Optional
 from typing import Callable
 from typing import Union
-from typing import Tuple
 
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.layers.base import BaseLayer
 from molgraph.layers.ops import softmax_edge_weights
 from molgraph.layers.ops import propagate_node_features
 
 
@@ -28,16 +26,16 @@
 
     **Examples:**
 
     Inputs a ``GraphTensor`` encoding (two) subgraphs:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'edge_src': [[1, 0], [1, 2, 0, 2, 1, 0]],
+    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'node_feature': [
     ...             [[1.0, 0.0], [1.0, 0.0]],
     ...             [[1.0, 0.0], [1.0, 0.0], [0.0, 1.0]]
     ...         ],
     ...         'edge_feature': [
     ...             [[1.0, 0.0], [0.0, 1.0]],
     ...             [[0.0, 1.0], [0.0, 1.0], [1.0, 0.0],
@@ -54,16 +52,16 @@
     >>> gnn_model.output_shape
     (None, None, 16)
 
     Inputs a ``GraphTensor`` encoding a single disjoint graph:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'node_feature': [
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [0.0, 1.0]
     ...         ],
@@ -215,16 +213,16 @@
         gate = softmax_edge_weights(
             edge_weight=gate,
             edge_dst=tensor.edge_dst,
             exponentiate=False)
 
         node_feature = propagate_node_features(
             node_feature=node_feature,
-            edge_dst=tensor.edge_dst,
             edge_src=tensor.edge_src,
+            edge_dst=tensor.edge_dst,
             edge_weight=gate)
 
         if self.apply_self_projection:
             node_feature += self.self_projection(tensor.node_feature)
 
         return tensor.update({'node_feature': node_feature})
```

### Comparing `molgraph-0.3.8/molgraph/layers/attentional/gatv2_conv.py` & `molgraph-0.3.9/molgraph/layers/attentional/gmm_conv.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,122 +1,101 @@
 import tensorflow as tf
 from tensorflow import keras
-from tensorflow.keras import initializers
-from tensorflow.keras import regularizers
-from tensorflow.keras import constraints
-from tensorflow.keras import activations
-
+from keras import initializers
+from keras import regularizers
+from keras import constraints
+from keras import layers
 
 from typing import Optional
 from typing import Callable
 from typing import Union
-from typing import Tuple
 
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.layers.base import BaseLayer
-from molgraph.layers.ops import softmax_edge_weights
 from molgraph.layers.ops import propagate_node_features
 from molgraph.layers.ops import reduce_features
 
 
 
 @keras.utils.register_keras_serializable(package='molgraph')
-class GATv2Conv(BaseLayer):
+class GMMConv(BaseLayer):
 
-    '''Multi-head graph attention (v2) layer (GATv2).
+    '''Multi-head graph gaussian mixture layer (MoNet)
 
-    The implementation is based on Brody et al. (2021) [#]_.
+    Implementation is based on Dwivedi et al. (2022) [#]_ and Monti et al. (2016) [#]_.
 
     **Examples:**
 
     Inputs a ``GraphTensor`` encoding (two) subgraphs:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'edge_src': [[1, 0], [1, 2, 0, 2, 1, 0]],
+    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'node_feature': [
     ...             [[1.0, 0.0], [1.0, 0.0]],
     ...             [[1.0, 0.0], [1.0, 0.0], [0.0, 1.0]]
     ...         ],
-    ...         'edge_feature': [
-    ...             [[1.0, 0.0], [0.0, 1.0]],
-    ...             [[0.0, 1.0], [0.0, 1.0], [1.0, 0.0],
-    ...              [0.0, 1.0], [1.0, 0.0], [0.0, 1.0]]
-    ...         ],
     ...     }
     ... )
-    >>> # Build a model with GATv2Conv
+    >>> # Build a model with GMMConv
     >>> gnn_model = tf.keras.Sequential([
     ...     tf.keras.Input(type_spec=graph_tensor.unspecific_spec),
-    ...     molgraph.layers.GATv2Conv(16, activation='relu'),
-    ...     molgraph.layers.GATv2Conv(16, activation='relu')
+    ...     molgraph.layers.GMMConv(16, activation='relu'),
+    ...     molgraph.layers.GMMConv(16, activation='relu')
     ... ])
     >>> gnn_model.output_shape
     (None, None, 16)
 
     Inputs a ``GraphTensor`` encoding a single disjoint graph:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'node_feature': [
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [0.0, 1.0]
     ...         ],
     ...         'graph_indicator': [0, 0, 1, 1, 1],
-    ...         'edge_feature': [
-    ...             [1.0, 0.0],
-    ...             [0.0, 1.0],
-    ...             [0.0, 1.0],
-    ...             [0.0, 1.0],
-    ...             [1.0, 0.0],
-    ...             [0.0, 1.0],
-    ...             [1.0, 0.0],
-    ...             [0.0, 1.0]
-    ...         ],
     ...     }
     ... )
-    >>> # Build a model with GATv2Conv
+    >>> # Build a model with GMMConv
     >>> gnn_model = tf.keras.Sequential([
     ...     tf.keras.Input(type_spec=graph_tensor.unspecific_spec),
-    ...     molgraph.layers.GATv2Conv(16, activation='relu'),
-    ...     molgraph.layers.GATv2Conv(16, activation='relu')
+    ...     molgraph.layers.GMMConv(16, activation='relu'),
+    ...     molgraph.layers.GMMConv(16, activation='relu')
     ... ])
     >>> gnn_model.output_shape
     (None, 16)
 
     Args:
         units (int, None):
             Number of output units.
-        use_edge_features (bool):
-            Whether or not to use edge features. Default to True.
-        num_heads (int):
+        num_kernels (int):
             Number of attention heads. Default to 8.
         merge_mode (str):
             The strategy for merging the heads. Either of 'concat', 'sum',
-            'mean' or None. If set to None, 'mean' is used. Default to 'concat'.
+            'mean' or None. If set to None, 'mean' is used. Default to 'sum'.
+        pseudo_coord_dim (int):
+            The dimension of the pseudo coordinate of the Gaussian kernel.
+            Default to 2.
         self_projection (bool):
             Whether to apply self projection. Default to True.
         batch_norm: (bool):
             Whether to apply batch normalization to the output. Default to True.
         residual: (bool)
             Whether to add skip connection to the output. Default to True.
         dropout: (float, None):
             Dropout applied to the output of the layer. Default to None.
-        attention_activation (tf.keras.activations.Activation, callable, str, None):
-            Activation function applied to the the attention scores.
-            Default to 'leaky_relu'.
         activation (tf.keras.activations.Activation, callable, str, None):
-            Activation function applied to the output of the layer.
-            Default to 'relu'.
+            Activation function applied to the output of the layer. Default to 'relu'.
         use_bias (bool):
             Whether the layer should use biases. Default to True.
         kernel_initializer (tf.keras.initializers.Initializer, str):
             Initializer function for the kernels. Default to
             tf.keras.initializers.TruncatedNormal(stddev=0.005).
         bias_initializer (tf.keras.initializers.Initializer, str):
             Initializer function for the biases. Default to
@@ -130,44 +109,41 @@
             Default to None.
         kernel_constraint (tf.keras.constraints.Constraint, None):
             Constraint function applied to the kernels. Default to None.
         bias_constraint (tf.keras.constraints.Constraint, None):
             Constraint function applied to the biases. Default to None.
 
     References:
-        .. [#] https://arxiv.org/pdf/2105.14491.pdf
+
+    .. [#] https://arxiv.org/pdf/2003.00982.pdf
+    .. [#] https://arxiv.org/pdf/1611.08402.pdf
 
     '''
 
     def __init__(
         self,
-        units: Optional[int] = 128,
-        use_edge_features: bool = True,
-        num_heads: int = 8,
-        merge_mode: Optional[str] = 'concat',
+        units: Optional[int] = None,
+        num_kernels: int = 8,
+        merge_mode: Optional[str] = 'sum',
+        pseudo_coord_dim=2,
         self_projection: bool = True,
         batch_norm: bool = True,
         residual: bool = True,
         dropout: Optional[float] = None,
-        attention_activation: Union[
-            None, str, Callable[[tf.Tensor], tf.Tensor]] = 'leaky_relu',
         activation: Union[None, str, Callable[[tf.Tensor], tf.Tensor]] = 'relu',
         use_bias: bool = True,
         kernel_initializer: Union[str, initializers.Initializer, None] = None,
         bias_initializer: Union[str, initializers.Initializer, None] = None,
         kernel_regularizer: Optional[regularizers.Regularizer] = None,
         bias_regularizer: Optional[regularizers.Regularizer] = None,
         activity_regularizer: Optional[regularizers.Regularizer] = None,
         kernel_constraint: Optional[constraints.Constraint] = None,
         bias_constraint: Optional[constraints.Constraint] = None,
         **kwargs
     ):
-        kwargs['update_edge_features'] = (
-            kwargs.get('update_edge_features', True) and use_edge_features
-        )
         super().__init__(
             units=units,
             batch_norm=batch_norm,
             residual=residual,
             dropout=dropout,
             activation=activation,
             use_bias=use_bias,
@@ -176,110 +152,118 @@
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
             **kwargs)
 
-        self.use_edge_features = use_edge_features
-        self.num_heads = num_heads
+        self.num_kernels = num_kernels
         self.merge_mode = merge_mode
+        self.pseudo_coord_dim = pseudo_coord_dim
         self.apply_self_projection = self_projection
-        self.attention_activation = activations.get(attention_activation)
 
     def subclass_build(
         self,
         node_feature_shape: Optional[tf.TensorShape] = None,
         edge_feature_shape: Optional[tf.TensorShape] = None
     ) -> None:
 
         if self.merge_mode == 'concat':
-            if not self.units or (self.units % self.num_heads != 0):
+            if not self.units or (self.units % self.num_kernels != 0):
                 raise ValueError(
-                    '`merge_mode` was set to `concat` and hence ' +
-                    ' need `units` to be divisble by `num_heads`')
-            self.units //= self.num_heads
+                    "`merge_mode` was set to `concat` and hence " +
+                    " need `units` to be divisble by `num_heads`")
+            self.units //= self.num_kernels
 
-        self.use_edge_features = (
-            self.use_edge_features and edge_feature_shape is not None
-        )
-        if self.use_edge_features:
-
-            self.edge_projection = self.get_einsum_dense(
-                'ij,jkh->ihk', (self.num_heads, self.units))
-
-            if self.update_edge_features:
-                self.edge_out_projection = self.get_einsum_dense(
-                    'ihj,jkh->ihk', (self.num_heads, self.units))
-
-        # Future implementation: Allow for non-shared weights?
-        # I.e., implement node_projection_dst and node_projection_src
         self.node_projection = self.get_einsum_dense(
-            'ij,jkh->ihk', (self.num_heads, self.units))
+            'ij,jkh->ihk', (self.num_kernels, self.units))
 
         if self.apply_self_projection:
             self.self_projection = self.get_einsum_dense(
-                'ij,jkh->ihk', (self.num_heads, self.units))
+                'ij,jkh->ihk', (self.num_kernels, self.units))
+
+        self.pseudo_coord_projection = layers.Dense(
+            self.pseudo_coord_dim, activation='tanh')
 
-        self.attention_projection = self.get_einsum_dense(
-            'ihj,jhk->ihk', (self.num_heads, 1))
+        self.mu = self.add_weight(
+            shape=(1, self.num_kernels, self.pseudo_coord_dim),
+            initializer='random_normal',
+            name='mu')
+
+        self.sigma_inv = self.add_weight(
+            shape=(1, self.num_kernels, self.pseudo_coord_dim),
+            initializer='ones',
+            name='sigma_inv')
 
         if self.merge_mode == 'concat':
-            self.units *= self.num_heads
+            self.units *= self.num_kernels
 
     def subclass_call(self, tensor: GraphTensor) -> GraphTensor:
 
         node_feature = self.node_projection(tensor.node_feature)
-        # Add dst and src node features, instead of concatenating them
-        attention_feature = (
-            tf.gather(node_feature, tensor.edge_dst) +
-            tf.gather(node_feature, tensor.edge_src)
-        )
-        if self.use_edge_features:
-            edge_feature = self.edge_projection(tensor.edge_feature)
-            # Similarily, add associated edge features, instead of concatenating them
-            attention_feature += edge_feature
-
-            if self.update_edge_features:
-                edge_feature = self.edge_out_projection(attention_feature)
-                edge_feature = reduce_features(
-                    feature=edge_feature,
-                    mode=self.merge_mode,
-                    output_units=self.units)
-
-                tensor = tensor.update({'edge_feature': edge_feature})
-
-        # Apply activation before attention projection
-        edge_weights = self.attention_activation(attention_feature)
-        edge_weights = self.attention_projection(edge_weights)
-
-        edge_weights = softmax_edge_weights(
-            edge_weight=edge_weights,
-            edge_dst=tensor.edge_dst)
+
+        edge_weights = self.compute_edge_weights(
+            tensor.edge_dst, tensor.edge_src)
 
         node_feature = propagate_node_features(
             node_feature=node_feature,
-            edge_dst=tensor.edge_dst,
             edge_src=tensor.edge_src,
+            edge_dst=tensor.edge_dst,
             edge_weight=edge_weights)
 
         if self.apply_self_projection:
             node_feature += self.self_projection(tensor.node_feature)
 
         node_feature = reduce_features(
             feature=node_feature,
             mode=self.merge_mode,
             output_units=self.units)
 
         return tensor.update({'node_feature': node_feature})
 
+    def compute_edge_weights(self, edge_dst, edge_src, clip_values=(-5, 5)):
+        """Computes edge weights via Gaussian kernels"""
+
+        def true_fn(edge_dst, edge_src, clip_values):
+            """If edges exist, call this function"""
+            # Compute self/neighbor degree-tuples (deg(i), deg(j))
+            degree = tf.math.bincount(edge_dst)
+            degree = tf.cast(degree, tf.float32)
+            degree = tf.where(degree == 0.0, 1.0, degree) ** -(1/2)
+            degree = tf.stack([
+                tf.gather(degree, edge_src),
+                tf.gather(degree, edge_dst),
+            ], axis=1)
+
+            # (n_edges, 2) @ (2, 2) -> (n_edges, 2)
+            pseudo_coord = self.pseudo_coord_projection(degree)
+            pseudo_coord = tf.expand_dims(pseudo_coord, 1)
+
+            # (n_edges, 1, dim), (1, kernels, dim)
+            edge_weights = -1/2 * (pseudo_coord - self.mu) ** 2
+            # (n_edges, kernels, dim)
+            edge_weights *= (self.sigma_inv ** 2)
+            # (n_edges, kernels, dim)
+            edge_weights = tf.reduce_sum(edge_weights, axis=-1, keepdims=True)
+            # (n_edges, kernels, 1)
+            return tf.exp(tf.clip_by_value(edge_weights, *clip_values))
+
+        def false_fn():
+            """If no edges exist, call this function"""
+            return tf.zeros([0, self.num_kernels, 1], dtype=tf.float32)
+
+        return tf.cond(
+            tf.greater(tf.shape(edge_dst)[0], 0),
+            lambda: true_fn(edge_dst, edge_src, clip_values),
+            lambda: false_fn()
+        )
+
     def get_config(self):
         base_config = super().get_config()
         config = {
-            'use_edge_features': self.use_edge_features,
-            'num_heads': self.num_heads,
+            'num_kernels': self.num_kernels,
             'merge_mode': self.merge_mode,
+            'pseudo_coord_dim': self.pseudo_coord_dim,
             'self_projection': self.apply_self_projection,
-            'attention_activation': activations.serialize(self.attention_activation),
         }
         base_config.update(config)
         return base_config
```

### Comparing `molgraph-0.3.8/molgraph/layers/attentional/gmm_conv.py` & `molgraph-0.3.9/molgraph/layers/geometric/gcf_conv.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,108 +1,122 @@
 import tensorflow as tf
 from tensorflow import keras
-from tensorflow.keras import initializers
-from tensorflow.keras import regularizers
-from tensorflow.keras import constraints
-from tensorflow.keras import activations
-from tensorflow.keras import layers
+from keras import initializers
+from keras import regularizers
+from keras import constraints
+import numpy as np
 
 from typing import Optional
 from typing import Callable
 from typing import Union
-from typing import Tuple
 
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.layers.base import BaseLayer
 from molgraph.layers.ops import propagate_node_features
-from molgraph.layers.ops import reduce_features
+from molgraph.layers.geometric import _radial_basis
 
 
 
 @keras.utils.register_keras_serializable(package='molgraph')
-class GMMConv(BaseLayer):
+class GCFConv(BaseLayer):
 
-    '''Multi-head graph gaussian mixture layer (MoNet)
+    """(Graph) continuous filter convolution layer ((G)CFConv).
 
-    Implementation is based on Dwivedi et al. (2022) [#]_ and Monti et al. (2016) [#]_.
+    Implementation is based on Schütt et al. (2017b) [#]_.
+
+    Operates on 3D molecular graphs (encoding distance geometry).
 
     **Examples:**
 
     Inputs a ``GraphTensor`` encoding (two) subgraphs:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'edge_src': [[1, 0], [1, 2, 0, 2, 1, 0]],
+    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'node_feature': [
     ...             [[1.0, 0.0], [1.0, 0.0]],
     ...             [[1.0, 0.0], [1.0, 0.0], [0.0, 1.0]]
     ...         ],
+    ...         # edge_feature encodes distances between edge_src and edge_dst
+    ...         'edge_feature': [[0.3, 0.3], [0.1, 0.2, 0.1, 0.4, 0.4, 0.2]],
     ...     }
     ... )
-    >>> # Build a model with GMMConv
+    >>> # Build a model with GCFConv
     >>> gnn_model = tf.keras.Sequential([
     ...     tf.keras.Input(type_spec=graph_tensor.unspecific_spec),
-    ...     molgraph.layers.GMMConv(16, activation='relu'),
-    ...     molgraph.layers.GMMConv(16, activation='relu')
+    ...     molgraph.layers.GCFConv(16, activation='relu'),
+    ...     molgraph.layers.GCFConv(16, activation='relu')
     ... ])
     >>> gnn_model.output_shape
     (None, None, 16)
 
     Inputs a ``GraphTensor`` encoding a single disjoint graph:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'node_feature': [
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [0.0, 1.0]
     ...         ],
     ...         'graph_indicator': [0, 0, 1, 1, 1],
+    ...         # edge_feature encodes distances between edge_src and edge_dst
+    ...         'edge_feature': [0.3, 0.3, 0.1, 0.2, 0.1, 0.4, 0.4, 0.2],
     ...     }
     ... )
-    >>> # Build a model with GMMConv
+    >>> # Build a model with GCFConv
     >>> gnn_model = tf.keras.Sequential([
     ...     tf.keras.Input(type_spec=graph_tensor.unspecific_spec),
-    ...     molgraph.layers.GMMConv(16, activation='relu'),
-    ...     molgraph.layers.GMMConv(16, activation='relu')
+    ...     molgraph.layers.GCFConv(16, activation='relu'),
+    ...     molgraph.layers.GCFConv(16, activation='relu')
     ... ])
     >>> gnn_model.output_shape
     (None, 16)
 
     Args:
         units (int, None):
-            Number of output units.
-        num_kernels (int):
-            Number of attention heads. Default to 8.
-        merge_mode (str):
-            The strategy for merging the heads. Either of 'concat', 'sum',
-            'mean' or None. If set to None, 'mean' is used. Default to 'sum'.
-        pseudo_coord_dim (int):
-            The dimension of the pseudo coordinate of the Gaussian kernel.
-            Default to 2.
+            The number of output units.
+        distance_min (float):
+            The smallest center (mean) to be used for the radial basis function.
+            I.e., it defines the minimum distance between atom pairs; or the
+            minimum electrostatic interaction between nuclei, in the case of
+            Coulomb values. Default to -1.0.
+        distance_max (float):
+            The largest center (mean) to be used for the radial basis function.
+            I.e., it defines the maximum distance between atom pairs; or the
+            maximum electrostatic interaction between nuclei, in the case of
+            Coulomb values. Default to 18.0.
+        distance_granularity (float):
+            The distance between each center (mean) of the radial basis function.
+            The smaller the granularity, the more centers will be used.
+            Default to 0.1.
+        rbf_stddev (float, str):
+            The standard deviation of the radial basis function. If 'auto',
+            'distance_granularity' will be used as standard deviation.
+            Default to 'auto'.
         self_projection (bool):
             Whether to apply self projection. Default to True.
         batch_norm: (bool):
             Whether to apply batch normalization to the output. Default to True.
         residual: (bool)
             Whether to add skip connection to the output. Default to True.
         dropout: (float, None):
             Dropout applied to the output of the layer. Default to None.
         activation (tf.keras.activations.Activation, callable, str, None):
-            Activation function applied to the output of the layer. Default to 'relu'.
+            Activation function applied to the output of the layer. Default to None.
         use_bias (bool):
             Whether the layer should use biases. Default to True.
         kernel_initializer (tf.keras.initializers.Initializer, str):
             Initializer function for the kernels. Default to
-            tf.keras.initializers.TruncatedNormal(stddev=0.005).
+            tf.keras.initializers.GlorotUniform().
         bias_initializer (tf.keras.initializers.Initializer, str):
             Initializer function for the biases. Default to
             tf.keras.initializers.Constant(0.).
         kernel_regularizer (tf.keras.regularizers.Regularizer, None):
             Regularizer function applied to the kernels. Default to None.
         bias_regularizer (tf.keras.regularizers.Regularizer, None):
             Regularizer function applied to the biases. Default to None.
@@ -111,31 +125,30 @@
             Default to None.
         kernel_constraint (tf.keras.constraints.Constraint, None):
             Constraint function applied to the kernels. Default to None.
         bias_constraint (tf.keras.constraints.Constraint, None):
             Constraint function applied to the biases. Default to None.
 
     References:
+        .. [#] https://arxiv.org/pdf/1706.08566.pdf
+    """
 
-    .. [#] https://arxiv.org/pdf/2003.00982.pdf
-    .. [#] https://arxiv.org/pdf/1611.08402.pdf
-
-    '''
 
     def __init__(
         self,
         units: Optional[int] = None,
-        num_kernels: int = 8,
-        merge_mode: Optional[str] = 'sum',
-        pseudo_coord_dim=2,
+        distance_min: float = -1.0,
+        distance_max: float = 18.0,
+        distance_granularity: float = 0.1,
+        rbf_stddev: Optional[Union[float, str]] = 'auto',
         self_projection: bool = True,
         batch_norm: bool = True,
         residual: bool = True,
         dropout: Optional[float] = None,
-        activation: Union[None, str, Callable[[tf.Tensor], tf.Tensor]] = 'relu',
+        activation: Union[None, str, Callable[[tf.Tensor], tf.Tensor]] = None,
         use_bias: bool = True,
         kernel_initializer: Union[str, initializers.Initializer, None] = None,
         bias_initializer: Union[str, initializers.Initializer, None] = None,
         kernel_regularizer: Optional[regularizers.Regularizer] = None,
         bias_regularizer: Optional[regularizers.Regularizer] = None,
         activity_regularizer: Optional[regularizers.Regularizer] = None,
         kernel_constraint: Optional[constraints.Constraint] = None,
@@ -154,117 +167,88 @@
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
             **kwargs)
 
-        self.num_kernels = num_kernels
-        self.merge_mode = merge_mode
-        self.pseudo_coord_dim = pseudo_coord_dim
+        self.activation = shifted_softplus
         self.apply_self_projection = self_projection
+        self.distance_min = distance_min
+        self.distance_max = distance_max
+        self.distance_granularity = distance_granularity
+        self.rbf_stddev = rbf_stddev
+
+        self.rbf = _radial_basis.RadialBasis(
+            self.distance_min,
+            self.distance_max,
+            self.distance_granularity,
+            self.rbf_stddev
+        )
 
     def subclass_build(
         self,
         node_feature_shape: Optional[tf.TensorShape] = None,
         edge_feature_shape: Optional[tf.TensorShape] = None
     ) -> None:
 
-        if self.merge_mode == 'concat':
-            if not self.units or (self.units % self.num_kernels != 0):
-                raise ValueError(
-                    "`merge_mode` was set to `concat` and hence " +
-                    " need `units` to be divisble by `num_heads`")
-            self.units //= self.num_kernels
+        self.filter_generator_1 = self.get_dense(self.units, self.activation)
+        self.filter_generator_2 = self.get_dense(self.units, self.activation)
 
-        self.node_projection = self.get_einsum_dense(
-            'ij,jkh->ihk', (self.num_kernels, self.units))
+        self.node_projection_1 = self.get_dense(self.units)
+        self.node_projection_2 = self.get_dense(self.units, self.activation)
+        self.node_projection_3 = self.get_dense(self.units)
 
         if self.apply_self_projection:
-            self.self_projection = self.get_einsum_dense(
-                'ij,jkh->ihk', (self.num_kernels, self.units))
-
-        self.pseudo_coord_projection = layers.Dense(
-            self.pseudo_coord_dim, activation='tanh')
-
-        self.mu = self.add_weight(
-            shape=(1, self.num_kernels, self.pseudo_coord_dim),
-            initializer='random_normal',
-            name='mu')
-
-        self.sigma_inv = self.add_weight(
-            shape=(1, self.num_kernels, self.pseudo_coord_dim),
-            initializer='ones',
-            name='sigma_inv')
-
-        if self.merge_mode == 'concat':
-            self.units *= self.num_kernels
+            self.self_projection = self.get_dense(self.units)
 
     def subclass_call(self, tensor: GraphTensor) -> GraphTensor:
 
-        node_feature = self.node_projection(tensor.node_feature)
+        cosine_weight = cosine_weight_from_distance(tensor.edge_feature),
+        rbf_feature = self.rbf(tensor.edge_feature)
+        rbf_weight = self.filter_generator_2(
+            self.filter_generator_1(rbf_feature))
 
-        edge_weights = self.compute_edge_weights(
-            tensor.edge_dst, tensor.edge_src)
+        node_feature = self.node_projection_1(tensor.node_feature)
+
+        rbf_weight *= cosine_weight
 
         node_feature = propagate_node_features(
             node_feature=node_feature,
-            edge_dst=tensor.edge_dst,
             edge_src=tensor.edge_src,
-            edge_weight=edge_weights)
+            edge_dst=tensor.edge_dst,
+            edge_weight=rbf_weight,
+            mode='mean')
 
         if self.apply_self_projection:
             node_feature += self.self_projection(tensor.node_feature)
 
-        node_feature = reduce_features(
-            feature=node_feature,
-            mode=self.merge_mode,
-            output_units=self.units)
+        node_feature = self.node_projection_3(
+            self.node_projection_2(node_feature))
 
         return tensor.update({'node_feature': node_feature})
 
-    def compute_edge_weights(self, edge_dst, edge_src, clip_values=(-5, 5)):
-        """Computes edge weights via Gaussian kernels"""
-
-        def true_fn(edge_dst, edge_src, clip_values):
-            """If edges exist, call this function"""
-            # Compute self/neighbor degree-tuples (deg(i), deg(j))
-            degree = tf.math.bincount(edge_dst)
-            degree = tf.cast(degree, tf.float32)
-            degree = tf.where(degree == 0.0, 1.0, degree) ** -(1/2)
-            degree = tf.stack([
-                tf.gather(degree, edge_dst),
-                tf.gather(degree, edge_src)], axis=1)
-
-            # (n_edges, 2) @ (2, 2) -> (n_edges, 2)
-            pseudo_coord = self.pseudo_coord_projection(degree)
-            pseudo_coord = tf.expand_dims(pseudo_coord, 1)
-
-            # (n_edges, 1, dim), (1, kernels, dim)
-            edge_weights = -1/2 * (pseudo_coord - self.mu) ** 2
-            # (n_edges, kernels, dim)
-            edge_weights *= (self.sigma_inv ** 2)
-            # (n_edges, kernels, dim)
-            edge_weights = tf.reduce_sum(edge_weights, axis=-1, keepdims=True)
-            # (n_edges, kernels, 1)
-            return tf.exp(tf.clip_by_value(edge_weights, *clip_values))
-
-        def false_fn():
-            """If no edges exist, call this function"""
-            return tf.zeros([0, self.num_kernels, 1], dtype=tf.float32)
-
-        return tf.cond(
-            tf.greater(tf.shape(edge_dst)[0], 0),
-            lambda: true_fn(edge_dst, edge_src, clip_values),
-            lambda: false_fn()
-        )
-
     def get_config(self):
         base_config = super().get_config()
-        config = {
-            'num_kernels': self.num_kernels,
-            'merge_mode': self.merge_mode,
-            'pseudo_coord_dim': self.pseudo_coord_dim,
+        base_config.update({
             'self_projection': self.apply_self_projection,
-        }
-        base_config.update(config)
+            'distance_min': self.distance_min,
+            'distance_max': self.distance_max,
+            'distance_granularity': self.distance_granularity,
+            'rbf_stddev': self.rbf_stddev
+        })
         return base_config
+
+
+def shifted_softplus(x):
+    return tf.math.log(0.5 * tf.math.exp(x) + 0.5)
+
+def cosine_weight_from_distance(
+    distance: tf.Tensor,
+    distance_cutoff: float = 10.,
+    dtype: tf.DType = tf.float32,
+) -> tf.Tensor:
+    """Passes distances (floating point values) to a cosine function to obtain
+    weights for associated source nodes. Outputted values (also floating point
+    values) are in range [0, 1].
+    """
+    return (0.5 * (tf.math.cos((distance / distance_cutoff) * np.pi) + 1))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `molgraph-0.3.8/molgraph/layers/attentional/gt_conv.py` & `molgraph-0.3.9/molgraph/layers/attentional/gt_conv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import tensorflow as tf
 from tensorflow import keras
-from tensorflow.keras import initializers
-from tensorflow.keras import regularizers
-from tensorflow.keras import constraints
-from tensorflow.keras import activations
-from tensorflow.keras import layers
+from keras import initializers
+from keras import regularizers
+from keras import constraints
+from keras import activations
+from keras import layers
 
 from typing import Optional
 from typing import Callable
 from typing import Union
-from typing import Tuple
 
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.layers.base import BaseLayer
 from molgraph.layers.ops import softmax_edge_weights
 from molgraph.layers.ops import propagate_node_features
 from molgraph.layers.ops import reduce_features
 
@@ -30,16 +29,16 @@
 
     **Examples:**
 
     Inputs a ``GraphTensor`` encoding (two) subgraphs:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'edge_src': [[1, 0], [1, 2, 0, 2, 1, 0]],
+    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'node_feature': [
     ...             [[1.0, 0.0], [1.0, 0.0]],
     ...             [[1.0, 0.0], [1.0, 0.0], [0.0, 1.0]]
     ...         ],
     ...         'edge_feature': [
     ...             [[1.0, 0.0], [0.0, 1.0]],
     ...             [[0.0, 1.0], [0.0, 1.0], [1.0, 0.0],
@@ -56,16 +55,16 @@
     >>> gnn_model.output_shape
     (None, None, 16)
 
     Inputs a ``GraphTensor`` encoding a single disjoint graph:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'node_feature': [
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [0.0, 1.0]
     ...         ],
@@ -281,20 +280,20 @@
 
         value = self.value_projection(tensor.node_feature)
 
         # Edge dependent. In rare cases, we input a graph with a single
         # node and no edges; below would throw an error in such cases.
 
         # Apply linear transformation to node and edge features
-        query = self.query_projection(tensor.node_feature)
         key = self.key_projection(tensor.node_feature)
+        query = self.query_projection(tensor.node_feature)
 
         # Gather self nodes' queries and corresponding neighbor nodes' keys
-        query = tf.gather(query, tensor.edge_dst)
         key = tf.gather(key, tensor.edge_src)
+        query = tf.gather(query, tensor.edge_dst)
         # tf.gather(value, edge_src) will be run inside self.propagate_features(..)
 
         attention_score = query * key
 
         # Rescale the attention scores
         attention_score = attention_score / tf.math.sqrt(float(self.units))
 
@@ -309,16 +308,16 @@
 
         attention_score = softmax_edge_weights(
             edge_weight=attention_score,
             edge_dst=tensor.edge_dst)
 
         node_feature = propagate_node_features(
             node_feature=value,
-            edge_dst=tensor.edge_dst,
             edge_src=tensor.edge_src,
+            edge_dst=tensor.edge_dst,
             edge_weight=attention_score)
 
         if self.apply_self_projection:
             node_feature += self.self_projection(tensor.node_feature)
 
         node_feature = self.feed_forward_network(
             'node', node_feature, tensor.node_feature)
```

### Comparing `molgraph-0.3.8/molgraph/layers/base.py` & `molgraph-0.3.9/molgraph/layers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import tensorflow as tf
 from tensorflow import keras
-from tensorflow.keras import layers
-from tensorflow.keras import initializers
-from tensorflow.keras import regularizers
-from tensorflow.keras import constraints
-from tensorflow.keras import activations
-
+from keras import layers
+from keras import initializers
+from keras import regularizers
+from keras import constraints
+from keras import activations
 from keras.utils import tf_utils
 
 from abc import ABC, abstractmethod
 
 from typing import Optional
 from typing import Callable
 from typing import Union
@@ -287,24 +286,24 @@
             **self.get_common_kwargs())
 
     def get_einsum_dense(
         self,
         equation: str,
         output_shape: Shape,
         activation: Activation = None,
-    ) -> layers.experimental.EinsumDense:
+    ) -> layers.EinsumDense:
 
         if self._use_bias:
             bias_axes = equation.split('->')[-1][1:]
             if len(bias_axes) == 0:
                 bias_axes = None
         else:
             bias_axes = None
 
-        return layers.experimental.EinsumDense(
+        return layers.EinsumDense(
             equation,
             output_shape,
             activation=activation,
             bias_axes=bias_axes,
             **self.get_common_kwargs())
 
     def compute_output_shape(
```

### Comparing `molgraph-0.3.8/molgraph/layers/convolutional/gcn_conv.py` & `molgraph-0.3.9/molgraph/layers/convolutional/gcn_conv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import tensorflow as tf
 from tensorflow import keras
-from tensorflow.keras import initializers
-from tensorflow.keras import regularizers
-from tensorflow.keras import constraints
-from tensorflow.keras import activations
+from keras import initializers
+from keras import regularizers
+from keras import constraints
 
 from typing import Optional
 from typing import Callable
 from typing import Union
-from typing import Tuple
 
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.layers.base import BaseLayer
 from molgraph.layers.ops import compute_edge_weights_from_degrees
 from molgraph.layers.ops import propagate_node_features
 
 
@@ -27,16 +25,16 @@
 
     **Examples:**
 
     Inputs a ``GraphTensor`` encoding (two) subgraphs:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'edge_src': [[1, 0], [1, 2, 0, 2, 1, 0]],
+    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'node_feature': [
     ...             [[1.0, 0.0], [1.0, 0.0]],
     ...             [[1.0, 0.0], [1.0, 0.0], [0.0, 1.0]]
     ...         ],
     ...     }
     ... )
     >>> # Build a model with GCNConv
@@ -48,16 +46,16 @@
     >>> gnn_model.output_shape
     (None, None, 16)
 
     Inputs a ``GraphTensor`` encoding a single disjoint graph:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'node_feature': [
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [0.0, 1.0]
     ...         ],
@@ -203,24 +201,24 @@
 
         if self.use_edge_features:
             node_feature = tf.expand_dims(tensor.node_feature, axis=-1)
         else:
             node_feature = tensor.node_feature
 
         edge_weight = compute_edge_weights_from_degrees(
-            edge_dst=tensor.edge_dst,
             edge_src=tensor.edge_src,
+            edge_dst=tensor.edge_dst,
             edge_feature=tensor.edge_feature if self.use_edge_features else None,
             mode=self.degree_normalization)
 
         # (n_edges, ndim, 1) x (n_edges, 1, edim) -> (n_edges, ndim, edim)
         node_feature = propagate_node_features(
             node_feature=node_feature,
-            edge_dst=tensor.edge_dst,
             edge_src=tensor.edge_src,
+            edge_dst=tensor.edge_dst,
             edge_weight=edge_weight)
 
         if hasattr(self, 'kernel_decomp'):
             # (n_dim, unit, n_bases) x (e_dim, n_bases) -> (n_dim, unit, e_dim)
             kernel = tf.einsum(
                 'ikb,eb->ike', self.kernel, self.kernel_decomp)
         else:
```

### Comparing `molgraph-0.3.8/molgraph/layers/convolutional/gcnii_conv.py` & `molgraph-0.3.9/molgraph/layers/convolutional/gcnii_conv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import tensorflow as tf
 from tensorflow import keras
-from tensorflow.keras import initializers
-from tensorflow.keras import regularizers
-from tensorflow.keras import constraints
-from tensorflow.keras import activations
+from keras import initializers
+from keras import regularizers
+from keras import constraints
 
 from typing import Optional
 from typing import Callable
 from typing import Union
-from typing import Tuple
 
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.layers.base import BaseLayer
 from molgraph.layers.ops import compute_edge_weights_from_degrees
 from molgraph.layers.ops import propagate_node_features
 
 
@@ -26,16 +24,16 @@
 
     **Examples:**
 
     Inputs a ``GraphTensor`` encoding (two) subgraphs:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'edge_src': [[1, 0], [1, 2, 0, 2, 1, 0]],
+    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'node_feature': [
     ...             [[1.0, 0.0], [1.0, 0.0]],
     ...             [[1.0, 0.0], [1.0, 0.0], [0.0, 1.0]]
     ...         ],
     ...     }
     ... )
     >>> # Build a model with GCNIIConv
@@ -47,16 +45,16 @@
     >>> gnn_model.output_shape
     (None, None, 16)
 
     Inputs a ``GraphTensor`` encoding a single disjoint graph:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'node_feature': [
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [0.0, 1.0]
     ...         ],
@@ -196,23 +194,23 @@
             tensor = tensor.update({
                 'node_feature': self.node_resample(tensor.node_feature)})
 
         if not hasattr(tensor, 'node_feature_initial'):
             tensor = tensor.update({'node_feature_initial': tensor.node_feature})
 
         edge_weight = compute_edge_weights_from_degrees(
-            edge_dst=tensor.edge_dst,
             edge_src=tensor.edge_src,
+            edge_dst=tensor.edge_dst,
             edge_feature=None,
             mode=self.degree_normalization)
 
         node_feature = propagate_node_features(
             node_feature=tensor.node_feature,
-            edge_dst=tensor.edge_dst,
             edge_src=tensor.edge_src,
+            edge_dst=tensor.edge_dst,
             edge_weight=edge_weight)
 
         identity = (
             (1 - self.alpha) * node_feature +
             self.alpha * tensor.node_feature_initial
         )
```

### Comparing `molgraph-0.3.8/molgraph/layers/convolutional/gin_conv.py` & `molgraph-0.3.9/molgraph/layers/convolutional/gin_conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import tensorflow as tf
 from tensorflow import keras
-from tensorflow.keras import initializers
-from tensorflow.keras import regularizers
-from tensorflow.keras import constraints
-from tensorflow.keras import activations
-from tensorflow.keras import layers
+from keras import initializers
+from keras import regularizers
+from keras import constraints
+from keras import activations
+from keras import layers
 
 from typing import Optional
 from typing import Callable
 from typing import Union
-from typing import Tuple
 
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.layers.base import BaseLayer
 from molgraph.layers.ops import compute_edge_weights_from_degrees
 from molgraph.layers.ops import propagate_node_features
 
 
@@ -28,16 +27,16 @@
 
     **Examples:**
 
     Inputs a ``GraphTensor`` encoding (two) subgraphs:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'edge_src': [[1, 0], [1, 2, 0, 2, 1, 0]],
+    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'node_feature': [
     ...             [[1.0, 0.0], [1.0, 0.0]],
     ...             [[1.0, 0.0], [1.0, 0.0], [0.0, 1.0]]
     ...         ],
     ...     }
     ... )
     >>> # Build a model with GINConv
@@ -49,16 +48,16 @@
     >>> gnn_model.output_shape
     (None, None, 16)
 
     Inputs a ``GraphTensor`` encoding a single disjoint graph:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'node_feature': [
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [0.0, 1.0]
     ...         ],
@@ -74,16 +73,16 @@
     >>> gnn_model.output_shape
     (None, 16)
 
     With edge features ("GINEConv"):
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'node_feature': [
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [0.0, 1.0]
     ...         ],
@@ -230,16 +229,17 @@
            self.self_projection = self.get_dense(self.units)
 
     def subclass_call(self, tensor: GraphTensor) -> GraphTensor:
 
         if not self.use_edge_features:
             node_feature_aggregated = propagate_node_features(
                 node_feature=tensor.node_feature,
+                edge_src=tensor.edge_src,
                 edge_dst=tensor.edge_dst,
-                edge_src=tensor.edge_src)
+            )
         else:
             node_feature_src = tf.gather(tensor.node_feature, tensor.edge_src)
             if hasattr(self, 'edge_projection'):
                 edge_feature_updated = self.edge_projection(tensor.edge_feature)
                 tensor = tensor.update({'edge_feature': edge_feature_updated})
             node_feature_src += tensor.edge_feature
             if self.apply_relu_activation:
```

### Comparing `molgraph-0.3.8/molgraph/layers/convolutional/graph_sage_conv.py` & `molgraph-0.3.9/molgraph/layers/convolutional/graph_sage_conv.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import tensorflow as tf
 from tensorflow import keras
-from tensorflow.keras import initializers
-from tensorflow.keras import regularizers
-from tensorflow.keras import constraints
-from tensorflow.keras import activations
-from tensorflow.keras import layers
+from keras import initializers
+from keras import regularizers
+from keras import constraints
+from keras import activations
+from keras import layers
 
 from typing import Optional
 from typing import Callable
 from typing import Union
-from typing import Tuple
 
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.layers.base import BaseLayer
-from molgraph.layers.ops import compute_edge_weights_from_degrees
 from molgraph.layers.ops import propagate_node_features
 
 
 
 @keras.utils.register_keras_serializable(package='molgraph')
 class GraphSageConv(BaseLayer):
 
@@ -28,16 +26,16 @@
 
     **Examples:**
 
     Inputs a ``GraphTensor`` encoding (two) subgraphs:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'edge_src': [[1, 0], [1, 2, 0, 2, 1, 0]],
+    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'node_feature': [
     ...             [[1.0, 0.0], [1.0, 0.0]],
     ...             [[1.0, 0.0], [1.0, 0.0], [0.0, 1.0]]
     ...         ],
     ...     }
     ... )
     >>> # Build a model with GraphSageConv
@@ -49,16 +47,16 @@
     >>> gnn_model.output_shape
     (None, None, 16)
 
     Inputs a ``GraphTensor`` encoding a single disjoint graph:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'node_feature': [
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [0.0, 1.0]
     ...         ],
@@ -179,25 +177,25 @@
     def subclass_call(self, tensor: GraphTensor) -> GraphTensor:
 
         if self.aggregation_mode == 'max':
             node_feature = self.node_src_projection(tensor.node_feature)
             node_feature = self.activation(node_feature)
             node_feature = propagate_node_features(
                 node_feature=node_feature,
-                edge_dst=tensor.edge_dst,
                 edge_src=tensor.edge_src,
+                edge_dst=tensor.edge_dst,
                 mode=self.aggregation_mode)
         elif self.aggregation_mode == 'lstm':
             node_feature = self.lstm_aggregate(
-                tensor.node_feature, tensor.edge_dst, tensor.edge_src)
+                tensor.node_feature, tensor.edge_src, tensor.edge_dst)
         else:
             node_feature = propagate_node_features(
                 node_feature=tensor.node_feature,
-                edge_dst=tensor.edge_dst,
                 edge_src=tensor.edge_src,
+                edge_dst=tensor.edge_dst,
                 mode=self.aggregation_mode)
 
         node_feature = tf.concat([node_feature, tensor.node_feature], axis=-1)
 
         node_feature = self.node_projection(node_feature)
 
         if self.apply_self_projection:
@@ -205,56 +203,48 @@
 
         if self.normalize:
             node_feature = self.activation(node_feature)
             node_feature = tf.math.l2_normalize(node_feature, axis=1)
 
         return tensor.update({'node_feature': node_feature})
 
-    def lstm_aggregate(self, node_feature, edge_dst, edge_src):
+    def lstm_aggregate(self, node_feature, edge_src, edge_dst):
 
-        def true_fn(node_feature, edge_dst, edge_src):
-            """If edges exist, call this function"""
+        def true_fn(node_feature, edge_src, edge_dst):
+            'If edges exist, call this function'
 
-            node_indices = tf.unique(edge_dst)[0]
+            # Get number of nodes
             num_nodes = tf.shape(node_feature)[0]
-            #print(node_indices)
 
-            # A bit of a hack to shuffle neighbor (source) nodes of the
-            # destination nodes.
-            random_indices = tf.random.shuffle(tf.range(tf.shape(edge_dst)[0]))
+            # Shuffle neighbor (source) nodes of the destination nodes.
+            random_indices = tf.random.shuffle(tf.range(tf.shape(edge_src)[0]))
             edge_dst = tf.gather(edge_dst, random_indices)
             edge_src = tf.gather(edge_src, random_indices)
             sorted_indices = tf.argsort(edge_dst)
             edge_dst = tf.gather(edge_dst, sorted_indices)
-            edge_dst -= tf.reduce_min(edge_dst)
             edge_src = tf.gather(edge_src, sorted_indices)
 
             # Gather source nodes followed by a partitioning of destination nodes
             node_feature = tf.RaggedTensor.from_value_rowids(
-                tf.gather(node_feature, edge_src), edge_dst)
+                tf.gather(node_feature, edge_src), edge_dst, num_nodes)
             node_feature = node_feature.to_tensor()
             # Pass to lstm for update
             node_feature = self.lstm(node_feature)
 
-            node_feature_dim = tf.shape(node_feature)[-1]
-
-            return tf.scatter_nd(
-                indices=tf.expand_dims(node_indices, axis=-1),
-                updates=node_feature,
-                shape=(num_nodes, node_feature_dim))
+            return node_feature
 
         def false_fn(node_feature):
             """If no edges exist, call this function"""
             return tf.zeros(
                 shape=(tf.shape(node_feature)[0], self.units),
                 dtype=node_feature.dtype)
 
         return tf.cond(
-            tf.greater(tf.shape(edge_dst)[0], 0),
-            lambda: true_fn(node_feature, edge_dst, edge_src),
+            tf.greater(tf.shape(edge_src)[0], 0),
+            lambda: true_fn(node_feature, edge_src, edge_dst),
             lambda: false_fn(node_feature)
         )
 
     def get_config(self):
         base_config = super().get_config()
         config = {
             'aggregation_mode': self.aggregation_mode,
```

### Comparing `molgraph-0.3.8/molgraph/layers/geometric/_radial_basis.py` & `molgraph-0.3.9/molgraph/layers/geometric/_radial_basis.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.8/molgraph/layers/geometric/dtnn_conv.py` & `molgraph-0.3.9/molgraph/layers/geometric/dtnn_conv.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 import tensorflow as tf
 from tensorflow import keras
-from tensorflow.keras import initializers
-from tensorflow.keras import regularizers
-from tensorflow.keras import constraints
-from tensorflow.keras import activations
-
-import numpy as np
+from keras import initializers
+from keras import regularizers
+from keras import constraints
 
 from typing import Optional
 from typing import Callable
 from typing import Union
-from typing import Tuple
 
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.layers.base import BaseLayer
-from molgraph.layers.ops import propagate_node_features
 from molgraph.layers.geometric import _radial_basis
 
 
 
 @keras.utils.register_keras_serializable(package='molgraph')
 class DTNNConv(BaseLayer):
 
@@ -28,21 +23,21 @@
 
     **Examples:**
 
     Inputs a ``GraphTensor`` encoding (two) subgraphs:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'edge_src': [[1, 0], [1, 2, 0, 2, 1, 0]],
+    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'node_feature': [
     ...             [[1.0, 0.0], [1.0, 0.0]],
     ...             [[1.0, 0.0], [1.0, 0.0], [0.0, 1.0]]
     ...         ],
-    ...         # edge_feature encodes distances between edge_dst and edge_src
+    ...         # edge_feature encodes distances between edge_src and edge_dst
     ...         'edge_feature': [[0.3, 0.3], [0.1, 0.2, 0.1, 0.4, 0.4, 0.2]],
     ...     }
     ... )
     >>> # Build a model with DTNNConv
     >>> gnn_model = tf.keras.Sequential([
     ...     tf.keras.Input(type_spec=graph_tensor.unspecific_spec),
     ...     molgraph.layers.DTNNConv(16, activation='relu'),
@@ -51,25 +46,25 @@
     >>> gnn_model.output_shape
     (None, None, 16)
 
     Inputs a ``GraphTensor`` encoding a single disjoint graph:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'node_feature': [
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [0.0, 1.0]
     ...         ],
     ...         'graph_indicator': [0, 0, 1, 1, 1],
-    ...         # edge_feature encodes distances between edge_dst and edge_src
+    ...         # edge_feature encodes distances between edge_src and edge_dst
     ...         'edge_feature': [0.3, 0.3, 0.1, 0.2, 0.1, 0.4, 0.4, 0.2],
     ...     }
     ... )
     >>> # Build a model with DTNNConv
     >>> gnn_model = tf.keras.Sequential([
     ...     tf.keras.Input(type_spec=graph_tensor.unspecific_spec),
     ...     molgraph.layers.DTNNConv(16, activation='relu'),
```

### Comparing `molgraph-0.3.8/molgraph/layers/geometric/gcf_conv.py` & `molgraph-0.3.9/molgraph/layers/attentional/gat_conv.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,125 +1,126 @@
 import tensorflow as tf
 from tensorflow import keras
-from tensorflow.keras import initializers
-from tensorflow.keras import regularizers
-from tensorflow.keras import constraints
-from tensorflow.keras import activations
-
-import numpy as np
+from keras import initializers
+from keras import regularizers
+from keras import constraints
+from keras import activations
 
 from typing import Optional
 from typing import Callable
 from typing import Union
-from typing import Tuple
 
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.layers.base import BaseLayer
+from molgraph.layers.ops import softmax_edge_weights
 from molgraph.layers.ops import propagate_node_features
-from molgraph.layers.geometric import _radial_basis
+from molgraph.layers.ops import reduce_features
 
 
 
 @keras.utils.register_keras_serializable(package='molgraph')
-class GCFConv(BaseLayer):
-
-    """(Graph) continuous filter convolution layer ((G)CFConv).
+class GATConv(BaseLayer):
 
-    Implementation is based on Schütt et al. (2017b) [#]_.
+    '''Multi-head graph attention layer (GAT).
 
-    Operates on 3D molecular graphs (encoding distance geometry).
+    The implementation is based on Velickovic et al. (2018) [#]_ and
+    Dwivedi et al. (2022) [#]_.
 
     **Examples:**
 
     Inputs a ``GraphTensor`` encoding (two) subgraphs:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'edge_src': [[1, 0], [1, 2, 0, 2, 1, 0]],
+    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'node_feature': [
     ...             [[1.0, 0.0], [1.0, 0.0]],
     ...             [[1.0, 0.0], [1.0, 0.0], [0.0, 1.0]]
     ...         ],
-    ...         # edge_feature encodes distances between edge_dst and edge_src
-    ...         'edge_feature': [[0.3, 0.3], [0.1, 0.2, 0.1, 0.4, 0.4, 0.2]],
+    ...         'edge_feature': [
+    ...             [[1.0, 0.0], [0.0, 1.0]],
+    ...             [[0.0, 1.0], [0.0, 1.0], [1.0, 0.0],
+    ...              [0.0, 1.0], [1.0, 0.0], [0.0, 1.0]]
+    ...         ],
     ...     }
     ... )
-    >>> # Build a model with GCFConv
+    >>> # Build a model with GATConv
     >>> gnn_model = tf.keras.Sequential([
     ...     tf.keras.Input(type_spec=graph_tensor.unspecific_spec),
-    ...     molgraph.layers.GCFConv(16, activation='relu'),
-    ...     molgraph.layers.GCFConv(16, activation='relu')
+    ...     molgraph.layers.GATConv(16, activation='relu'),
+    ...     molgraph.layers.GATConv(16, activation='relu')
     ... ])
     >>> gnn_model.output_shape
     (None, None, 16)
 
     Inputs a ``GraphTensor`` encoding a single disjoint graph:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'node_feature': [
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [0.0, 1.0]
     ...         ],
     ...         'graph_indicator': [0, 0, 1, 1, 1],
-    ...         # edge_feature encodes distances between edge_dst and edge_src
-    ...         'edge_feature': [0.3, 0.3, 0.1, 0.2, 0.1, 0.4, 0.4, 0.2],
+    ...         'edge_feature': [
+    ...             [1.0, 0.0],
+    ...             [0.0, 1.0],
+    ...             [0.0, 1.0],
+    ...             [0.0, 1.0],
+    ...             [1.0, 0.0],
+    ...             [0.0, 1.0],
+    ...             [1.0, 0.0],
+    ...             [0.0, 1.0]
+    ...         ],
     ...     }
     ... )
-    >>> # Build a model with GCFConv
+    >>> # Build a model with GATConv
     >>> gnn_model = tf.keras.Sequential([
     ...     tf.keras.Input(type_spec=graph_tensor.unspecific_spec),
-    ...     molgraph.layers.GCFConv(16, activation='relu'),
-    ...     molgraph.layers.GCFConv(16, activation='relu')
+    ...     molgraph.layers.GATConv(16, activation='relu'),
+    ...     molgraph.layers.GATConv(16, activation='relu')
     ... ])
     >>> gnn_model.output_shape
     (None, 16)
 
     Args:
         units (int, None):
-            The number of output units.
-        distance_min (float):
-            The smallest center (mean) to be used for the radial basis function.
-            I.e., it defines the minimum distance between atom pairs; or the
-            minimum electrostatic interaction between nuclei, in the case of
-            Coulomb values. Default to -1.0.
-        distance_max (float):
-            The largest center (mean) to be used for the radial basis function.
-            I.e., it defines the maximum distance between atom pairs; or the
-            maximum electrostatic interaction between nuclei, in the case of
-            Coulomb values. Default to 18.0.
-        distance_granularity (float):
-            The distance between each center (mean) of the radial basis function.
-            The smaller the granularity, the more centers will be used.
-            Default to 0.1.
-        rbf_stddev (float, str):
-            The standard deviation of the radial basis function. If 'auto',
-            'distance_granularity' will be used as standard deviation.
-            Default to 'auto'.
+            Number of output units.
+        use_edge_features (bool):
+            Whether or not to use edge features. Default to True.
+        num_heads (int):
+            Number of attention heads. Default to 8.
+        merge_mode (str):
+            The strategy for merging the heads. Either of 'concat', 'sum',
+            'mean' or None. If set to None, 'mean' is used. Default to 'concat'.
         self_projection (bool):
             Whether to apply self projection. Default to True.
         batch_norm: (bool):
             Whether to apply batch normalization to the output. Default to True.
         residual: (bool)
             Whether to add skip connection to the output. Default to True.
         dropout: (float, None):
             Dropout applied to the output of the layer. Default to None.
+        attention_activation (tf.keras.activations.Activation, callable, str, None):
+            Activation function applied to the the attention scores.
+            Default to 'leaky_relu'.
         activation (tf.keras.activations.Activation, callable, str, None):
-            Activation function applied to the output of the layer. Default to None.
+            Activation function applied to the output of the layer.
+            Default to 'relu'.
         use_bias (bool):
             Whether the layer should use biases. Default to True.
         kernel_initializer (tf.keras.initializers.Initializer, str):
             Initializer function for the kernels. Default to
-            tf.keras.initializers.GlorotUniform().
+            tf.keras.initializers.TruncatedNormal(stddev=0.005).
         bias_initializer (tf.keras.initializers.Initializer, str):
             Initializer function for the biases. Default to
             tf.keras.initializers.Constant(0.).
         kernel_regularizer (tf.keras.regularizers.Regularizer, None):
             Regularizer function applied to the kernels. Default to None.
         bias_regularizer (tf.keras.regularizers.Regularizer, None):
             Regularizer function applied to the biases. Default to None.
@@ -128,40 +129,45 @@
             Default to None.
         kernel_constraint (tf.keras.constraints.Constraint, None):
             Constraint function applied to the kernels. Default to None.
         bias_constraint (tf.keras.constraints.Constraint, None):
             Constraint function applied to the biases. Default to None.
 
     References:
-        .. [#] https://arxiv.org/pdf/1706.08566.pdf
-    """
+        .. [#] https://arxiv.org/pdf/1710.10903.pdf
+        .. [#] https://arxiv.org/pdf/2003.00982.pdf
 
+    '''
 
     def __init__(
         self,
-        units: Optional[int] = None,
-        distance_min: float = -1.0,
-        distance_max: float = 18.0,
-        distance_granularity: float = 0.1,
-        rbf_stddev: Optional[Union[float, str]] = 'auto',
+        units: Optional[int] = 128,
+        use_edge_features: bool = True,
+        num_heads: int = 8,
+        merge_mode: Optional[str] = 'concat',
         self_projection: bool = True,
         batch_norm: bool = True,
         residual: bool = True,
         dropout: Optional[float] = None,
-        activation: Union[None, str, Callable[[tf.Tensor], tf.Tensor]] = None,
+        attention_activation: Union[
+            None, str, Callable[[tf.Tensor], tf.Tensor]] = 'leaky_relu',
+        activation: Union[None, str, Callable[[tf.Tensor], tf.Tensor]] = 'relu',
         use_bias: bool = True,
         kernel_initializer: Union[str, initializers.Initializer, None] = None,
         bias_initializer: Union[str, initializers.Initializer, None] = None,
         kernel_regularizer: Optional[regularizers.Regularizer] = None,
         bias_regularizer: Optional[regularizers.Regularizer] = None,
         activity_regularizer: Optional[regularizers.Regularizer] = None,
         kernel_constraint: Optional[constraints.Constraint] = None,
         bias_constraint: Optional[constraints.Constraint] = None,
         **kwargs
     ):
+        kwargs['update_edge_features'] = (
+            kwargs.get('update_edge_features', True) and use_edge_features
+        )
         super().__init__(
             units=units,
             batch_norm=batch_norm,
             residual=residual,
             dropout=dropout,
             activation=activation,
             use_bias=use_bias,
@@ -170,88 +176,108 @@
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
             **kwargs)
 
-        self.activation = shifted_softplus
+        self.use_edge_features = use_edge_features
+        self.num_heads = num_heads
+        self.merge_mode = merge_mode
         self.apply_self_projection = self_projection
-        self.distance_min = distance_min
-        self.distance_max = distance_max
-        self.distance_granularity = distance_granularity
-        self.rbf_stddev = rbf_stddev
-
-        self.rbf = _radial_basis.RadialBasis(
-            self.distance_min,
-            self.distance_max,
-            self.distance_granularity,
-            self.rbf_stddev
-        )
+        self.activation = activations.get('elu')
+        self.attention_activation = activations.get(attention_activation)
 
     def subclass_build(
         self,
         node_feature_shape: Optional[tf.TensorShape] = None,
         edge_feature_shape: Optional[tf.TensorShape] = None
     ) -> None:
 
-        self.filter_generator_1 = self.get_dense(self.units, self.activation)
-        self.filter_generator_2 = self.get_dense(self.units, self.activation)
+        if self.merge_mode == 'concat':
+            if not self.units or (self.units % self.num_heads != 0):
+                raise ValueError(
+                    '`merge_mode` was set to `concat` and hence ' +
+                    ' need `units` to be divisble by `num_heads`')
+            self.units //= self.num_heads
 
-        self.node_projection_1 = self.get_dense(self.units)
-        self.node_projection_2 = self.get_dense(self.units, self.activation)
-        self.node_projection_3 = self.get_dense(self.units)
+        self.use_edge_features = (
+            self.use_edge_features and edge_feature_shape is not None
+        )
+        if self.use_edge_features:
+
+            self.edge_projection = self.get_einsum_dense(
+                'ij,jkh->ihk', (self.num_heads, self.units))
+
+            if self.update_edge_features:
+                self.edge_out_projection = self.get_einsum_dense(
+                    'ihj,jkh->ihk', (self.num_heads, self.units))
+
+        self.node_projection = self.get_einsum_dense(
+            'ij,jkh->ihk', (self.num_heads, self.units))
 
         if self.apply_self_projection:
-            self.self_projection = self.get_dense(self.units)
+            self.self_projection = self.get_einsum_dense(
+                'ij,jkh->ihk', (self.num_heads, self.units))
 
-    def subclass_call(self, tensor: GraphTensor) -> GraphTensor:
+        self.attention_projection = self.get_einsum_dense(
+            'ihj,jhk->ihk', (self.num_heads, 1))
+
+        if self.merge_mode == 'concat':
+            self.units *= self.num_heads
 
-        cosine_weight = cosine_weight_from_distance(tensor.edge_feature),
-        rbf_feature = self.rbf(tensor.edge_feature)
-        rbf_weight = self.filter_generator_2(
-            self.filter_generator_1(rbf_feature))
+    def subclass_call(self, tensor: GraphTensor) -> GraphTensor:
 
-        node_feature = self.node_projection_1(tensor.node_feature)
+        # Edge dependent (i.e., `tensor.edge_src is not None`), from here
+        node_feature = self.node_projection(tensor.node_feature)
 
-        rbf_weight *= cosine_weight
+        attention_feature = tf.concat([
+            tf.gather(node_feature, tensor.edge_dst),
+            tf.gather(node_feature, tensor.edge_src)], axis=-1)
+
+        if self.use_edge_features:
+            edge_feature = self.edge_projection(tensor.edge_feature)
+            attention_feature = tf.concat([attention_feature, edge_feature], axis=-1)
+
+            if self.update_edge_features:
+                edge_feature = self.edge_out_projection(attention_feature)
+                edge_feature = reduce_features(
+                    feature=edge_feature,
+                    mode=self.merge_mode,
+                    output_units=self.units)
+                tensor = tensor.update({'edge_feature': edge_feature})
+
+        edge_weights = self.attention_projection(attention_feature)
+        edge_weights = self.attention_activation(edge_weights)
+        edge_weights = softmax_edge_weights(
+            edge_weight=edge_weights,
+            edge_dst=tensor.edge_dst)
 
         node_feature = propagate_node_features(
             node_feature=node_feature,
-            edge_dst=tensor.edge_dst,
             edge_src=tensor.edge_src,
-            edge_weight=rbf_weight,
-            mode='mean')
+            edge_dst=tensor.edge_dst,
+            edge_weight=edge_weights)
 
         if self.apply_self_projection:
             node_feature += self.self_projection(tensor.node_feature)
 
-        node_feature = self.node_projection_3(
-            self.node_projection_2(node_feature))
+        node_feature = self.activation(node_feature)
+
+        node_feature = reduce_features(
+            feature=node_feature,
+            mode=self.merge_mode,
+            output_units=self.units)
 
         return tensor.update({'node_feature': node_feature})
 
     def get_config(self):
         base_config = super().get_config()
-        base_config.update({
+        config = {
+            'use_edge_features': self.use_edge_features,
+            'num_heads': self.num_heads,
+            'merge_mode': self.merge_mode,
             'self_projection': self.apply_self_projection,
-            'distance_min': self.distance_min,
-            'distance_max': self.distance_max,
-            'distance_granularity': self.distance_granularity,
-            'rbf_stddev': self.rbf_stddev
-        })
+            'attention_activation': activations.serialize(self.attention_activation),
+        }
+        base_config.update(config)
         return base_config
-
-
-def shifted_softplus(x):
-    return tf.math.log(0.5 * tf.math.exp(x) + 0.5)
-
-def cosine_weight_from_distance(
-    distance: tf.Tensor,
-    distance_cutoff: float = 10.,
-    dtype: tf.DType = tf.float32,
-) -> tf.Tensor:
-    """Passes distances (floating point values) to a cosine function to obtain
-    weights for associated source nodes. Outputted values (also floating point
-    values) are in range [0, 1].
-    """
-    return (0.5 * (tf.math.cos((distance / distance_cutoff) * np.pi) + 1))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `molgraph-0.3.8/molgraph/layers/message_passing/edge_conv.py` & `molgraph-0.3.9/molgraph/layers/message_passing/edge_conv.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 import tensorflow as tf
 from tensorflow import keras
 from keras.utils import tf_utils
-from tensorflow.keras import initializers
-from tensorflow.keras import regularizers
-from tensorflow.keras import constraints
-from tensorflow.keras import activations
-from tensorflow.keras import layers
-import math
+from keras import initializers
+from keras import regularizers
+from keras import constraints
+from keras import activations
 
 from typing import Optional
 from typing import Callable
 from typing import Union
-from typing import Tuple
 from typing import Type
 from typing import TypeVar
 
 from molgraph.tensors.graph_tensor import GraphTensor
-from molgraph.layers.base import BaseLayer
-from molgraph.layers.ops import compute_edge_weights_from_degrees
-from molgraph.layers.ops import propagate_node_features
 
 
 Config = TypeVar('Config', bound=dict)
 
 
 @keras.utils.register_keras_serializable(package='molgraph')
 class EdgeConv(tf.keras.layers.Layer):
@@ -41,16 +35,16 @@
     ways. For instance, it uses the very previous edge states (in `molgraph.layers.EdgeConv`) and 
     node states (in `molgraph.layers.GINConv`) as residual ("skip connections") rather than the very 
     initial edge states and node states respectively. Furthermore, this implementation also allows us to use
     GRU as the update function, though default is to use a Dense layer. 
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'node_feature': [
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [0.0, 1.0]
     ...         ],
@@ -224,15 +218,15 @@
             tensor = tensor.merge()
 
         # EdgeConv requires edge features, so if edge features do not exist,
         # we force edge features by initializing them as ones vector
         if not hasattr(tensor, 'edge_feature'):
             tensor = tensor.update({
                 'edge_feature': tf.ones(
-                    shape=[tf.shape(tensor.edge_dst)[0], 1], dtype=tf.float32)})
+                    shape=[tf.shape(tensor.edge_src)[0], 1], dtype=tf.float32)})
             
         if not self._built:
             initialize_edge_state = (
                 True if not hasattr(tensor, 'edge_state') else False)
             self._build(initialize_edge_state)
 
         if self._initialize_edge_state:
@@ -364,17 +358,16 @@
     message = tf.math.unsorted_segment_sum(edge_feature, edge_dst, num_nodes)
     message = tf.gather(message, edge_src)
     message -= _get_reverse_edge_features(edge_feature, edge_src, edge_dst)
     return message
 
 def _get_reverse_edge_features(edge_feature, edge_src, edge_dst):
     edge_exclude = tf.logical_and(
-        edge_dst[:, None] == edge_dst,
-        edge_src[:, None] == edge_src)
-        
+        edge_src[:, None] == edge_src,
+        edge_dst[:, None] == edge_dst
+    )
     edge_forward, edge_reverse = tf.split(tf.where(edge_exclude), 2, axis=-1)
-
     return tf.tensor_scatter_nd_add(
         tf.zeros_like(edge_feature), 
         tf.expand_dims(edge_forward, -1), 
         tf.gather(edge_feature, edge_reverse)
     )
```

### Comparing `molgraph-0.3.8/molgraph/layers/message_passing/mpnn_conv.py` & `molgraph-0.3.9/molgraph/layers/message_passing/mpnn_conv.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 import tensorflow as tf
 from tensorflow import keras
-from tensorflow.keras import initializers
-from tensorflow.keras import regularizers
-from tensorflow.keras import constraints
-from tensorflow.keras import activations
-from tensorflow.keras import layers
+from keras import initializers
+from keras import regularizers
+from keras import constraints
 import math
 
 from typing import Optional
 from typing import Callable
 from typing import Union
-from typing import Tuple
 
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.layers.base import BaseLayer
-from molgraph.layers.ops import compute_edge_weights_from_degrees
-from molgraph.layers.ops import propagate_node_features
 
 
 
 @keras.utils.register_keras_serializable(package='molgraph')
 class MPNNConv(BaseLayer):
 
     """Message passing neural network layer (MPNN)
@@ -32,16 +27,16 @@
 
     **Examples:**
 
     Inputs a ``GraphTensor`` encoding (two) subgraphs:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'edge_src': [[1, 0], [1, 2, 0, 2, 1, 0]],
+    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'node_feature': [
     ...             [[1.0, 0.0], [1.0, 0.0]],
     ...             [[1.0, 0.0], [1.0, 0.0], [0.0, 1.0]]
     ...         ],
     ...         'edge_feature': [
     ...             [[1.0, 0.0], [0.0, 1.0]],
     ...             [[0.0, 1.0], [0.0, 1.0], [1.0, 0.0],
@@ -58,16 +53,16 @@
     >>> gnn_model.output_shape
     (None, None, 16)
 
     Inputs a ``GraphTensor`` encoding a single disjoint graph:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'node_feature': [
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [0.0, 1.0]
     ...         ],
@@ -93,16 +88,16 @@
     >>> gnn_model.output_shape
     (None, 16)
 
     Pass the same GRU cell to each layer to perform weight sharing:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'node_feature': [
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [0.0, 1.0]
     ...         ],
@@ -264,21 +259,21 @@
                 'node_feature': self.node_resample(tensor.node_feature)})
 
         # MPNN requires edge features, if edge features do not exist,
         # we force edge features by initializing them as ones vector
         if not hasattr(tensor, 'edge_feature'):
             tensor = tensor.update({
                 'edge_feature': tf.ones(
-                    shape=[tf.shape(tensor.edge_dst)[0], 1], dtype=tf.float32)})
+                    shape=[tf.shape(tensor.edge_src)[0], 1], dtype=tf.float32)})
 
         node_feature_aggregated = message_step(
             node_feature=tensor.node_feature,
             edge_feature=tensor.edge_feature,
-            edge_dst=tensor.edge_dst,
             edge_src=tensor.edge_src,
+            edge_dst=tensor.edge_dst,
             projection=self.message_projection)
 
         node_feature_update = update_step(
             node_feature=node_feature_aggregated,
             node_feature_prev=tensor.node_feature,
             update_projection=self.update_fn,
             self_projection=self.self_projection)
@@ -314,29 +309,29 @@
             states=node_feature_prev)
     return node_feature
 
 
 def message_step(
     node_feature: tf.Tensor,
     edge_feature: tf.Tensor,
-    edge_dst: tf.Tensor,
     edge_src: tf.Tensor,
+    edge_dst: tf.Tensor,
     projection: keras.layers.Dense,
 ) -> tf.Tensor:
     '''Performs a message passing step.
 
     Args:
         node_feature (tf.Tensor):
             Node features; component of GraphTensor.
         edge_feature (tf.Tensor):
             Edge features; component of GraphTensor.
-        edge_dst (tf.Tensor):
-            Destination node indices; component of GraphTensor.
         edge_src (tf.Tensor):
             Source node indices; component of GraphTensor.
+        edge_dst (tf.Tensor):
+            Destination node indices; component of GraphTensor.
         projection (keras.layers.Dense):
             Dense layer that transforms edge features.
 
     Returns (tf.Tensor):
         Returns updated (aggregated) node features.
     '''
     output_units = int(math.sqrt(projection.units))
```

### Comparing `molgraph-0.3.8/molgraph/layers/ops.py` & `molgraph-0.3.9/molgraph/layers/ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 from typing import Optional
 from typing import Tuple
 
 
 def propagate_node_features(
     *,
     node_feature: tf.Tensor,
-    edge_dst: tf.Tensor,
     edge_src: tf.Tensor,
+    edge_dst: tf.Tensor,
     edge_weight: Optional[tf.Tensor] = None,
     mode: str = 'sum'
 ) -> tf.Tensor:
     '''Aggregates source node features to destination node features.
 
     Args:
         node_feature (tf.Tensor):
             Node features of graph tensor.
-        edge_dst (tf.Tensor):
-            Destination node indices of graph tensor. Entry i corresponds
-            to row i in node_feature.
         edge_src (tf.Tensor):
             Source node indices of graph tensor. Entry i corresponds
             to row i in node_feature.
+        edge_dst (tf.Tensor):
+            Destination node indices of graph tensor. Entry i corresponds
+            to row i in node_feature.
         edge_weight (tf.Tensor):
             Edge weights associated with edge_dst and edge_src.
 
     Returns:
         tf.Tensor: Updated node features via neighborhood aggregation.
     '''
 
@@ -89,52 +89,52 @@
     return tf.cond(
         tf.greater(tf.shape(edge_dst)[0], 0),
         lambda: true_fn(edge_weight, edge_dst, exponentiate, clip_values),
         lambda: false_fn(edge_weight))
 
 def compute_edge_weights_from_degrees(
     *,
-    edge_dst: tf.Tensor,
     edge_src: tf.Tensor,
+    edge_dst: tf.Tensor,
     edge_feature: Optional[tf.Tensor] = None,
     mode: Optional[str] = 'symmetric',
 ) -> tf.Tensor:
     '''Computes edge weights based on the number of nearest neighbors.
 
     These edge weights can subsequently be used as normalization coefficients
     for the neighborhood aggregation (``propagate_node_features``).
 
     Args:
-        edge_dst (tf.Tensor):
-            Destination node indices.
         edge_src (tf.Tensor):
             Source node indices.
+        edge_dst (tf.Tensor):
+            Destination node indices.
         edge_feature (tf.Tensor):
             Edge features associated with edge_dst and edge_src.
         mode (str):
             Type of normalization to use. Either of 'symmetric', 'row' or None.
             If None, 'row' is used. Default to 'symmetric'.
     Returns:
         tf.Tensor: Edge weights based on degrees.
     '''
 
     if edge_feature is None:
         edge_feature = tf.ones((tf.shape(edge_dst)[0], 1), dtype=tf.float32)
     else:
         edge_feature = tf.expand_dims(edge_feature, axis=1)
 
-    def true_fn(edge_dst, edge_src, edge_feature, mode):
+    def true_fn(edge_src, edge_dst, edge_feature, mode):
         'If edges exist, call this function.'
         # divide_no_nan makes sense? or tf.where(deg) -> .. * edge_feature
         degree = tf.math.unsorted_segment_sum(
             edge_feature, edge_dst, tf.reduce_max(edge_dst) + 1)
 
         if mode == 'symmetric':
             # symmetric norm (in matrix notation: A' = D^{-0.5} @ A @ D^{-0.5})
-            adjacency = tf.stack([edge_dst, edge_src], axis=1)
+            adjacency = tf.stack([edge_src, edge_dst], axis=1)
             degree = tf.sqrt(tf.reduce_prod(tf.gather(degree, adjacency), 1))
             edge_weight = tf.math.divide_no_nan(1., degree)
         else:
             # row norm (in matrix notation: A' = D^{-1} @ A)
             degree = tf.gather(degree, edge_dst)
             edge_weight = tf.math.divide_no_nan(1., degree)
 
@@ -144,16 +144,16 @@
         'If no edges exist, call this function.'
         edge_weight = tf.zeros(
             tf.TensorShape([0]).concatenate(edge_feature.shape[1:]),
             dtype=tf.float32)
         return edge_weight
 
     return tf.cond(
-        tf.greater(tf.shape(edge_dst)[0], 0),
-        lambda: true_fn(edge_dst, edge_src, edge_feature, mode),
+        tf.greater(tf.shape(edge_src)[0], 0),
+        lambda: true_fn(edge_src, edge_dst, edge_feature, mode),
         lambda: false_fn(edge_feature)
     )
 
 def reduce_features(
     *,
     feature: tf.Tensor,
     mode: Optional[str],
```

### Comparing `molgraph-0.3.8/molgraph/layers/positional_encoding/laplacian.py` & `molgraph-0.3.9/molgraph/layers/positional_encoding/laplacian.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import tensorflow as tf
 from tensorflow import keras
-from tensorflow.keras import layers
-from tensorflow.keras import initializers
-from tensorflow.keras import regularizers
-from tensorflow.keras import constraints
-from tensorflow.keras import activations
+from keras import layers
+from keras import initializers
+from keras import regularizers
+from keras import constraints
+from keras import activations
 
 from typing import Union
 from typing import Callable
 from typing import Optional
 
 from molgraph.tensors.graph_tensor import GraphTensor
 
@@ -20,16 +20,16 @@
 
     Implementation based on Dwivedi et al. (2021) [#]_ and Belkin et al. (2003) [#]_.
 
     **Example:**
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'node_feature': [
     ...             [1.0, 1.0],
     ...             [1.0, 1.0],
     ...             [1.0, 1.0],
     ...             [1.0, 1.0],
     ...             [1.0, 1.0]
     ...         ],
@@ -144,15 +144,15 @@
             bias_initializer=self.bias_initializer,
             kernel_regularizer=self.kernel_regularizer,
             bias_regularizer=self.bias_regularizer,
             activity_regularizer=self.activity_regularizer,
             kernel_constraint=self.kernel_constraint,
             bias_constraint=self.bias_constraint)
 
-    def call(self, tensor: GraphTensor) -> GraphTensor:
+    def call(self, tensor: GraphTensor, training: Optional[bool] = None) -> GraphTensor:
         '''Defines the computation from inputs to outputs.
 
         This method should not be called directly, but indirectly
         via ``__call__()``. Upon first call, the layer is automatically
         built via ``_build()``.
 
         Args:
@@ -180,15 +180,16 @@
 
         if not self._positional_encoding_precomputed:
             positional_encoding = compute_positional_encoding(
                 tensor, self._target_dim)
         else:
             positional_encoding = tensor.positional_encoding
 
-        positional_encoding = random_sign_flip(positional_encoding)
+        if training:
+            positional_encoding = random_sign_flip(positional_encoding)
         node_feature = tensor.node_feature + self.projection(positional_encoding)
         return tensor_orig.update({'node_feature': node_feature})
 
     @classmethod
     def from_config(cls, config):
         node_feature_shape = config.pop("node_feature_shape")
         positional_encoding_shape = config.pop("positional_encoding_shape")
@@ -218,15 +219,15 @@
             'positional_encoding_shape': self._positional_encoding_shape,
         }
         base_config.update(config)
         return base_config
 
 
 def compute_normalized_laplacian(adjacency, num_nodes):
-    degree = tf.math.bincount(adjacency[:, 0])
+    degree = tf.math.bincount(adjacency[:, 1])
     degree = tf.gather(degree, adjacency)
     adjacency_norm = tf.reduce_prod(tf.cast(degree, tf.float32), 1) ** -0.5
     laplacian_norm = tf.scatter_nd(
         adjacency, -adjacency_norm, (num_nodes, num_nodes))
     laplacian_norm += tf.eye(num_nodes, dtype=tf.float32)
     return laplacian_norm
 
@@ -238,15 +239,15 @@
     if dim < target_dim:
         pos_enc = tf.pad(pos_enc, [(0, 0), (0, target_dim - dim)])
     return pos_enc
 
 def compute_positional_encoding(tensor, target_dim):
 
     num_nodes = tf.shape(tensor.node_feature)[0]
-    adjacency = tf.stack([tensor.edge_dst, tensor.edge_src], axis=1)
+    adjacency = tf.stack([tensor.edge_src, tensor.edge_dst], axis=1)
 
     laplacian_norm = compute_normalized_laplacian(adjacency, num_nodes)
 
     graph_indicator = tensor.graph_indicator
 
     positional_encodings = tf.TensorArray(
         tf.float32, size=0, dynamic_size=True, infer_shape=False,
```

### Comparing `molgraph-0.3.8/molgraph/layers/postprocessing/dot_product_incident.py` & `molgraph-0.3.9/molgraph/layers/postprocessing/gather_incident.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,59 @@
 import tensorflow as tf
 from tensorflow import keras
 
 from molgraph.tensors.graph_tensor import GraphTensor
 
 
 @keras.utils.register_keras_serializable(package='molgraph')
-class DotProductIncident(keras.layers.Layer):
-    '''Performs dot product on the incident node features.
+class GatherIncident(keras.layers.Layer):
+    '''Gathers incident node features.
 
-    Useful for e.g., edge and link classification.
+    Useful for e.g., downstream edge and link classification.
 
     **Example:**
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'edge_src': [[1, 0], [1, 2, 0, 2, 1, 0]],
+    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'node_feature': [
-    ...             [[2.0, 0.0], [2.0, 0.0]],
-    ...             [[3.0, 0.0], [3.0, 0.0], [0.0, 3.0]]
+    ...             [[1.0, 0.0], [2.0, 0.0]],
+    ...             [[3.0, 0.0], [4.0, 0.0], [0.0, 5.0]]
     ...         ],
     ...     }
     ... )
+    >>> graph_tensor = graph_tensor.merge()
     >>> model = tf.keras.Sequential([
     ...     tf.keras.layers.Input(type_spec=graph_tensor.unspecific_spec),
-    ...     molgraph.layers.DotProductIncident()
+    ...     molgraph.layers.GatherIncident(concat=True)
     ... ])
     >>> model(graph_tensor)
-    <tf.RaggedTensor [[4.0, 4.0], [9.0, 0.0, 9.0, 0.0, 0.0, 0.0]]>
+    <tf.Tensor: shape=(8, 4), dtype=float32, numpy=
+    array([[2., 0., 1., 0.],
+           [1., 0., 2., 0.],
+           [4., 0., 3., 0.],
+           [0., 5., 3., 0.],
+           [3., 0., 4., 0.],
+           [0., 5., 4., 0.],
+           [4., 0., 0., 5.],
+           [3., 0., 0., 5.]], dtype=float32)>
 
     Args:
-        apply_sigmoid (bool):
-            Whether to apply a sigmoid activaton on the edge scores. 
-            Default to False.
+        concat (bool):
+            Whether to concatenate incident node features or not. If True,
+            resulting shape is (num_edges, num_features * 2), if False,
+            resulting shape is (num_edges, 2, num_features).
     '''
-    def __init__(self, apply_sigmoid: bool = False, **kwargs):
+
+    def __init__(self, concat: bool = True, **kwargs) -> None:
         super().__init__(**kwargs)
-        self._apply_sigmoid = apply_sigmoid
+        self.concat = concat
 
-    def call(self, tensor: GraphTensor) -> GraphTensor:
+    def call(self, tensor: GraphTensor) -> tf.Tensor:
         '''Defines the computation from inputs to outputs.
 
         This method should not be called directly, but indirectly
         via ``__call__()``. Upon first call, the layer is automatically
         built via ``build()``.
 
         Args:
@@ -52,22 +63,23 @@
         Returns:
             A ``tf.Tensor`` or `tf.RaggedTensor` based on the node_feature
             field of the inputted ``GraphTensor``.
         '''
         tensor_orig = tensor
         if isinstance(tensor.node_feature, tf.RaggedTensor):
             tensor = tensor.merge()
-        adjacency = tf.stack([
-            tensor.edge_dst, tensor.edge_src], axis=1)
-        node_feature_incident = tf.gather(
-            tensor.node_feature, adjacency)
-        edge_score = tf.reduce_sum(
-            tf.reduce_prod(node_feature_incident, axis=1), axis=1, keepdims=True)
-        if self._apply_sigmoid:
-            return tensor_orig.update({'edge_score': tf.nn.sigmoid(edge_score)})
-        return tensor_orig.update({'edge_score': edge_score})
+        node_feature_src = tf.gather(tensor.node_feature, tensor.edge_src)
+        node_feature_dst = tf.gather(tensor.node_feature, tensor.edge_dst)
+        if self.concat:
+            node_feature_incident = tf.concat([
+                node_feature_src, node_feature_dst], axis=1)
+        else:
+            node_feature_incident = tf.stack([
+                node_feature_src, node_feature_dst], axis=1)
+        tensor_orig = tensor_orig.update({
+            'edge_feature_incident': node_feature_incident})
+        return tensor_orig.edge_feature_incident
 
     def get_config(self):
-        config = super().get_config()
-        config.update({'apply_sigmoid', self._apply_sigmoid})
-        return config
-    
+        base_config = super().get_config()
+        base_config.update({'concat': self.concat})
+        return base_config
```

### Comparing `molgraph-0.3.8/molgraph/layers/postprocessing/extract_field.py` & `molgraph-0.3.9/molgraph/layers/postprocessing/extract_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 class ExtractField(keras.layers.Layer):
     '''Extract specific field of ``GraphTensor``.
 
     **Example:**
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'node_feature': [
     ...             [1., 0.],
     ...             [2., 0.],
     ...             [3., 0.],
     ...             [4., 0.],
     ...             [0., 5.]
     ...         ],
@@ -59,9 +59,9 @@
             A ``tf.Tensor`` or `tf.RaggedTensor` based on the node_feature
             field of the inputted ``GraphTensor``.
         '''
         return tensor[self.field]
 
     def get_config(self):
         base_config = super().get_config()
-        base_config.update({'field': field})
+        base_config.update({'field': self.field})
         return base_config
```

### Comparing `molgraph-0.3.8/molgraph/layers/preprocessing/center_scaling.py` & `molgraph-0.3.9/molgraph/layers/preprocessing/center_scaling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 import tensorflow as tf
 from tensorflow import keras
-from tensorflow.keras import layers
-from tensorflow.keras import initializers
+from keras import layers
 from keras.layers.preprocessing import preprocessing_utils as utils
 
-from typing import Tuple
-from typing import List
 from typing import Optional
-from typing import Union
-from typing import Tuple
-
 
 from molgraph.tensors.graph_tensor import GraphTensor
 
 
 
 @keras.utils.register_keras_serializable(package='molgraph')
-class CenterScaling(layers.experimental.preprocessing.PreprocessingLayer):
+class CenterScaling(layers.PreprocessingLayer):
 
     '''Centering.
 
     Specify, as keyword argument only,
     ``CenterScaling(feature='node_feature')`` to perform center scaling
     on the ``node_feature`` component of the ``GraphTensor``, or,
     ``CenterScaling(feature='edge_feature')`` to perform center scaling
@@ -29,16 +23,16 @@
 
     **Examples:**
 
     Adapt layer on ``GraphTensor`` directly:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'edge_src': [[1, 0], [1, 2, 0, 2, 1, 0]],
+    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'node_feature': [
     ...             [[1.0, 0.0], [1.0, 0.0]],
     ...             [[1.0, 0.0], [1.0, 0.0], [0.0, 1.0]]
     ...         ],
     ...     }
     ... )
     >>> # Initialize layer
@@ -59,16 +53,16 @@
            [ 0.19999999, -0.2       ],
            [-0.8       ,  0.8       ]], dtype=float32)>
 
     Adapt layer on ``tf.data.Dataset`` constructed from ``GraphTensor``:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'edge_src': [[1, 0], [1, 2, 0, 2, 1, 0]],
+    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'node_feature': [
     ...             [[1.0, 0.0], [1.0, 0.0]],
     ...             [[1.0, 0.0], [1.0, 0.0], [0.0, 1.0]]
     ...         ],
     ...     }
     ... )
     >>> # Obtain dataset
@@ -78,29 +72,29 @@
     ...    feature='node_feature')
     >>> # Adapt layer to graph_tensor
     >>> preprocessing.adapt(ds)
     >>> model = tf.keras.Sequential([
     ...     tf.keras.layers.Input(type_spec=graph_tensor.unspecific_spec),
     ...     preprocessing,
     ... ])
-    >>> output = model.predict(ds)
+    >>> output = model.predict(ds, verbose=0)
     >>> output.merge().node_feature
     <tf.Tensor: shape=(5, 2), dtype=float32, numpy=
     array([[ 0.19999999, -0.2       ],
            [ 0.19999999, -0.2       ],
            [ 0.19999999, -0.2       ],
            [ 0.19999999, -0.2       ],
            [-0.8       ,  0.8       ]], dtype=float32)>
 
     Adapt layer on merged ``GraphTensor``:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'node_feature': [
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [0.0, 1.0]
     ...         ],
```

### Comparing `molgraph-0.3.8/molgraph/layers/preprocessing/dropout.py` & `molgraph-0.3.9/molgraph/layers/preprocessing/dropout.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 class NodeDropout(keras.layers.Layer):
     '''Randomly dropping nodes from the graph.
 
     **Example:**
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'node_feature': [
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [0.0, 1.0]
     ...         ],
@@ -82,16 +82,16 @@
 class EdgeDropout(NodeDropout):
     '''Randomly dropping edges from the graph.
 
     **Example:**
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'node_feature': [
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [0.0, 1.0]
     ...         ],
```

### Comparing `molgraph-0.3.8/molgraph/layers/preprocessing/embedding_lookup.py` & `molgraph-0.3.9/molgraph/layers/preprocessing/embedding_lookup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import tensorflow as tf
 from tensorflow import keras
-from tensorflow.keras import layers
-from tensorflow.keras import initializers
-from tensorflow.keras import regularizers
-from tensorflow.keras import constraints
-from tensorflow.keras import activations
+from keras import layers
+from keras import initializers
+from keras import regularizers
+from keras import constraints
 
 from typing import Optional
 from typing import Union
 from typing import List
 
 from molgraph.tensors.graph_tensor import GraphTensor
 
@@ -30,16 +29,16 @@
 
     **Examples:**
 
     Adapt layer on ``GraphTensor`` directly:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'node_feature': [
     ...             'Sym:C', 'Sym:C', 'Sym:C', 'Sym:O', 'Sym:N',
     ...         ],
     ...         'graph_indicator': [0, 0, 1, 1, 1],
     ...     }
     ... )
     >>> # Initialize layer
@@ -55,16 +54,16 @@
     >>> graph_tensor.node_feature.shape
     TensorShape([5, 4])
 
     Adapt layer on dataset, constructed from ``GraphTensor``:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [[0, 1], [2, 2, 3, 3, 4, 4]],
     ...         'edge_src': [[1, 0], [3, 4, 2, 4, 3, 2]],
+    ...         'edge_dst': [[0, 1], [2, 2, 3, 3, 4, 4]],
     ...         'node_feature': [
     ...             ['Sym:C', 'Sym:C'], ['Sym:C', 'Sym:O', 'Sym:N'],
     ...         ],
     ...     }
     ... )
     >>> # Obtain dataset
     >>> ds = tf.data.Dataset.from_tensor_slices(graph_tensor).batch(2)
@@ -75,15 +74,15 @@
     >>> embedding.adapt(ds)
     >>> # Build model
     >>> model = tf.keras.Sequential([
     ...     tf.keras.layers.Input(type_spec=graph_tensor.unspecific_spec),
     ...     embedding,
     ... ])
     >>> # Predict (obtain new GraphTensor)
-    >>> output = model.predict(ds)
+    >>> output = model.predict(ds, verbose=0)
     >>> output.node_feature.shape
     TensorShape([2, None, 4])
 
     Args:
         output_dim (int):
             The output dimension of the embedding layer.
         input_dim (int, None):
```

### Comparing `molgraph-0.3.8/molgraph/layers/preprocessing/masking.py` & `molgraph-0.3.9/molgraph/layers/preprocessing/masking.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15,16 +15,16 @@
     Instead of specifying `feature`, ``NodeFeatureMasking(...)`` or 
     ``EdgeFeatureMasking(...)`` can be used instead.
 
     **Example:**
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...    data={
-    ...        'edge_dst': [0, 0, 1, 1, 1, 2, 3, 4],
     ...        'edge_src': [1, 4, 0, 2, 3, 1, 1, 0],
+    ...        'edge_dst': [0, 0, 1, 1, 1, 2, 3, 4],
     ...        'node_feature': [
     ...            'Sym:C|Hyb:SP3', 
     ...            'Sym:C|Hyb:SP2', 
     ...            'Sym:O|Hyb:SP2',
     ...            'Sym:O|Hyb:SP2', 
     ...            'Sym:N|Hyb:SP3'
     ...        ],
```

### Comparing `molgraph-0.3.8/molgraph/layers/preprocessing/min_max_scaling.py` & `molgraph-0.3.9/molgraph/layers/preprocessing/min_max_scaling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 import tensorflow as tf
 from tensorflow import keras
-from tensorflow.keras import layers
-from tensorflow.keras import initializers
-
-from keras import backend
+from keras import layers
+from keras import initializers
 from keras.layers.preprocessing import preprocessing_utils as utils
 
 from typing import Tuple
-from typing import List
 from typing import Optional
-from typing import Union
 from typing import Tuple
 
 
 from molgraph.tensors.graph_tensor import GraphTensor
 
 
 @keras.utils.register_keras_serializable(package='molgraph')
-class MinMaxScaling(layers.experimental.preprocessing.PreprocessingLayer):
+class MinMaxScaling(layers.PreprocessingLayer):
 
     '''Min-max scaling between a specified range.
 
     Specify, as keyword argument only,
     ``MinMaxScaling(feature='node_feature')`` to perform min-max scaling
     on the ``node_feature`` component of the ``GraphTensor``, or,
     ``MinMaxScaling(feature='edge_feature')`` to perform min-max scaling
@@ -30,16 +26,16 @@
 
     **Examples:**
 
     Adapt layer on ``GraphTensor`` directly:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'edge_src': [[1, 0], [1, 2, 0, 2, 1, 0]],
+    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'node_feature': [
     ...             [[2.0, 0.5], [2.0, 0.0]],
     ...             [[2.0, 0.0], [2.0, 0.5], [0.0, 2.0]]
     ...         ],
     ...     }
     ... )
     >>> # Initialize layer
@@ -60,16 +56,16 @@
            [1.  , 0.25],
            [0.  , 1.  ]], dtype=float32)>
 
     Adapt layer on ``tf.data.Dataset`` constructed from ``GraphTensor``:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'edge_src': [[1, 0], [1, 2, 0, 2, 1, 0]],
+    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'node_feature': [
     ...             [[2.0, 0.5], [2.0, 0.0]],
     ...             [[2.0, 0.0], [2.0, 0.5], [0.0, 2.0]]
     ...         ],
     ...     }
     ... )
     >>> # Obtain dataset
@@ -79,29 +75,29 @@
     ...    feature='node_feature')
     >>> # Adapt layer to graph_tensor
     >>> preprocessing.adapt(ds)
     >>> model = tf.keras.Sequential([
     ...     tf.keras.layers.Input(type_spec=graph_tensor.unspecific_spec),
     ...     preprocessing,
     ... ])
-    >>> output = model.predict(ds)
+    >>> output = model.predict(ds, verbose=0)
     >>> output.merge().node_feature
     <tf.Tensor: shape=(5, 2), dtype=float32, numpy=
     array([[1.  , 0.25],
            [1.  , 0.  ],
            [1.  , 0.  ],
            [1.  , 0.25],
            [0.  , 1.  ]], dtype=float32)>
 
     Adapt layer on merged ``GraphTensor``:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'node_feature': [
     ...             [2.0, 0.5],
     ...             [2.0, 0.0],
     ...             [2.0, 0.0],
     ...             [2.0, 0.5],
     ...             [0.0, 2.0]
     ...         ],
```

### Comparing `molgraph-0.3.8/molgraph/layers/preprocessing/projection.py` & `molgraph-0.3.9/molgraph/layers/preprocessing/projection.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import tensorflow as tf
 from tensorflow import keras
-from tensorflow.keras import layers
-from tensorflow.keras import initializers
-from tensorflow.keras import regularizers
-from tensorflow.keras import constraints
-from tensorflow.keras import activations
+from keras import layers
+from keras import initializers
+from keras import regularizers
+from keras import constraints
+from keras import activations
 
-from keras.utils import tf_utils
 
 
 @keras.utils.register_keras_serializable(package='molgraph')
 class FeatureProjection(layers.Layer):
 
     '''Feature projection via dense layer.
 
@@ -24,16 +23,16 @@
     Instead of specifying `feature`, ``NodeFeatureProjection(...)`` or 
     ``EdgeFeatureProjection(...)`` can be used instead.
 
     **Example:**
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'node_feature': [
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [0.0, 1.0]
     ...         ],
```

### Comparing `molgraph-0.3.8/molgraph/layers/preprocessing/standard_scaling.py` & `molgraph-0.3.9/molgraph/layers/preprocessing/standard_scaling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 import tensorflow as tf
 from tensorflow import keras
-from tensorflow.keras import layers
-from tensorflow.keras import initializers
+from keras import layers
+from keras import initializers
 from keras.layers.preprocessing import preprocessing_utils as utils
 
-from typing import Tuple
-from typing import List
 from typing import Optional
 from typing import Union
-from typing import Tuple
-
 
 from molgraph.tensors.graph_tensor import GraphTensor
 
 
 @keras.utils.register_keras_serializable(package='molgraph')
-class StandardScaling(layers.experimental.preprocessing.PreprocessingLayer):
+class StandardScaling(layers.PreprocessingLayer):
 
     '''Standard scaling, via centering and standardization.
 
     Specify, as keyword argument only,
     ``StandardScaling(feature='node_feature')`` to perform standard scaling
     on the ``node_feature`` component of the ``GraphTensor``, or,
     ``StandardScaling(feature='edge_feature')`` to perform standard scaling
@@ -28,16 +24,16 @@
 
     **Examples:**
 
     Adapt layer on ``GraphTensor`` directly:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'edge_src': [[1, 0], [1, 2, 0, 2, 1, 0]],
+    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'node_feature': [
     ...             [[2.0, 0.5], [2.0, 0.0]],
     ...             [[2.0, 0.0], [2.0, 0.5], [0.0, 2.0]]
     ...         ],
     ...     }
     ... )
     >>> # Initialize layer
@@ -58,16 +54,16 @@
            [ 0.50000006, -0.1360828 ],
            [-2.0000002 ,  1.9051588 ]], dtype=float32)>
 
     Adapt layer on ``tf.data.Dataset`` constructed from ``GraphTensor``:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'edge_src': [[1, 0], [1, 2, 0, 2, 1, 0]],
+    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'node_feature': [
     ...             [[2.0, 0.5], [2.0, 0.0]],
     ...             [[2.0, 0.0], [2.0, 0.5], [0.0, 2.0]]
     ...         ],
     ...     }
     ... )
     >>> # Obtain dataset
@@ -77,29 +73,29 @@
     ...    feature='node_feature')
     >>> # Adapt layer to graph_tensor
     >>> preprocessing.adapt(ds)
     >>> model = tf.keras.Sequential([
     ...     tf.keras.layers.Input(type_spec=graph_tensor.unspecific_spec),
     ...     preprocessing,
     ... ])
-    >>> output = model.predict(ds)
+    >>> output = model.predict(ds, verbose=0)
     >>> output.merge().node_feature
     <tf.Tensor: shape=(5, 2), dtype=float32, numpy=
     array([[ 0.50000006, -0.1360828 ],
            [ 0.50000006, -0.8164967 ],
            [ 0.50000006, -0.8164967 ],
            [ 0.50000006, -0.1360828 ],
            [-2.0000002 ,  1.9051588 ]], dtype=float32)>
 
     Adapt layer on merged ``GraphTensor``:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'node_feature': [
     ...             [2.0, 0.5],
     ...             [2.0, 0.0],
     ...             [2.0, 0.0],
     ...             [2.0, 0.5],
     ...             [0.0, 2.0]
     ...         ],
@@ -409,16 +405,16 @@
 
     **Examples:**
 
     Adapt layer on ``GraphTensor`` directly:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'edge_src': [[1, 0], [1, 2, 0, 2, 1, 0]],
+    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'node_feature': [
     ...             [[2.0, 0.5], [2.0, 0.0]],
     ...             [[2.0, 0.0], [2.0, 0.5], [0.0, 2.0]]
     ...         ],
     ...     }
     ... )
     >>> # Initialize layer
@@ -439,16 +435,16 @@
            [2.],
            [0.]], dtype=float32)>
 
     Adapt layer on ``tf.data.Dataset`` constructed from ``GraphTensor``:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'edge_src': [[1, 0], [1, 2, 0, 2, 1, 0]],
+    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'node_feature': [
     ...             [[2.0, 0.5], [2.0, 0.0]],
     ...             [[2.0, 0.0], [2.0, 0.5], [0.0, 2.0]]
     ...         ],
     ...     }
     ... )
     >>> # Obtain dataset
@@ -458,29 +454,29 @@
     ...    feature='node_feature', variance_threshold=0.6)
     >>> # Adapt layer to graph_tensor
     >>> preprocessing.adapt(ds)
     >>> model = tf.keras.Sequential([
     ...     tf.keras.layers.Input(type_spec=graph_tensor.unspecific_spec),
     ...     preprocessing,
     ... ])
-    >>> output = model.predict(ds)
+    >>> output = model.predict(ds, verbose=0)
     >>> output.merge().node_feature
     <tf.Tensor: shape=(5, 1), dtype=float32, numpy=
     array([[2.],
            [2.],
            [2.],
            [2.],
            [0.]], dtype=float32)>
 
     Adapt layer on merged ``GraphTensor``:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'node_feature': [
     ...             [2.0, 0.5],
     ...             [2.0, 0.0],
     ...             [2.0, 0.0],
     ...             [2.0, 0.5],
     ...             [0.0, 2.0]
     ...         ],
```

### Comparing `molgraph-0.3.8/molgraph/layers/readout/attentive_fp_readout.py` & `molgraph-0.3.9/molgraph/layers/readout/attentive_fp_readout.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,13 @@
 import tensorflow as tf
 from tensorflow import keras
-from keras.utils import tf_utils
-from tensorflow.keras import initializers
-from tensorflow.keras import regularizers
-from tensorflow.keras import constraints
-from tensorflow.keras import activations
-
 
 from typing import Optional
-from typing import Callable
-from typing import Union
 from typing import Tuple
-from typing import Type
 from typing import TypeVar
-from typing import Any
-
 
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.layers.attentional.gat_conv import GATConv
 
 
 Config = TypeVar('Config', bound=dict)
 
@@ -35,16 +24,16 @@
 
     **Examples:**
 
     Create a complete AttentiveFP model:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'node_feature': [
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [0.0, 1.0]
     ...         ],
@@ -68,28 +57,26 @@
     ...     molgraph.layers.AttentiveFPConv(16),
     ...     # ... 
     ...     molgraph.layers.AttentiveFPReadout(steps=4),
     ... ])
     >>> attentive_fp(graph_tensor).shape.as_list()
     [2, 16]
 
-
     Args:
         steps (int):
             Number of aggregation steps to perform. Default to 4.
         message_step (molgraph.layers.attentional.gat_conv.GATConv, None):
             The message passing step.
         update_step (tf.keras.layers.GRUCell, None):
             The update step. 
         final_node_projection (tf.keras.layers.Dense, None):
             The final projection applied to the output.
 
     References:
         .. [#] https://pubs.acs.org/doi/10.1021/acs.jmedchem.9b00959
-
     '''
 
     def __init__(
         self,
         steps: int = 4,
         message_step: Optional[GATConv] = None,
         update_step: Optional[tf.keras.layers.GRUCell] = None,
@@ -166,15 +153,15 @@
             edge_src_flat, graph_sizes)
         edge_dst = tf.RaggedTensor.from_row_lengths(
             edge_dst_flat, graph_sizes)
         return edge_src, edge_dst
     
     if isinstance(tensor.node_feature, tf.Tensor):
         # (None, node_dim) -> (batch_size, None, node_dim)
-        node_feature: tf.RaggedTensor = tf.RaggedTensor.from_value_rowids(
+        node_feature = tf.RaggedTensor.from_value_rowids(
             tensor.node_feature, tensor.graph_indicator)
     else:
         node_feature = tensor.node_feature
     
     edge_src, edge_dst = _get_edges(node_feature)
 
     # (batch_size, None, node_dim) -> (batch_size, 1, node_dim)
```

### Comparing `molgraph-0.3.8/molgraph/layers/readout/node_readout.py` & `molgraph-0.3.9/molgraph/layers/readout/node_readout.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
     '''Aggregates edge states to associated nodes.
 
     **Examples:**
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'node_feature': [
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [0.0, 1.0]
     ...         ],
@@ -48,26 +48,26 @@
     ...     molgraph.layers.GINConv(32),
     ...     molgraph.layers.Readout(),
     ...     tf.keras.layers.Dense(1, activation='sigmoid')
     ... ])
     >>> gnn_model.output_shape
     (None, 1)
 
-
     Args:
         target (str):
             Specifies which component to aggregate. Default to 'edge_state' which is the
             component produced by ``molgraph.layers.EdgeConv``.
         apply_transform (bool):
             Whether to perform a transformaton after the aggregation. Default to False.
         dense_kwargs (None, dict):
             Parameters to be passed to the dense layer in the transformation. Only relevant
             if ``apply_transform=True``. If None is passed, ``units`` is set to ``input_shape[-1]``
             and ``activation`` is set to ``relu``. Default to None.
     '''
+
     def __init__(
         self, 
         target: str = 'edge_state', 
         apply_transform: bool = True,
         dense_kwargs: Optional[dict] = None,
         **kwargs
     ):
```

### Comparing `molgraph-0.3.8/molgraph/layers/readout/segment_pool.py` & `molgraph-0.3.9/molgraph/layers/readout/segment_pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import tensorflow as tf
 from tensorflow import keras
-from tensorflow.keras import layers
+from keras import layers
 
 from molgraph.tensors.graph_tensor import GraphTensor
 
 
 
 @keras.utils.register_keras_serializable(package='molgraph')
 class SegmentPoolingReadout(layers.Layer):
@@ -13,16 +13,16 @@
 
     Alias: ``Readout``
 
     **Example:**
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'edge_src': [[1, 0], [1, 2, 0, 2, 1, 0]],
+    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'node_feature': [
     ...             [[1.0, 0.0], [1.0, 0.0]],
     ...             [[1.0, 0.0], [1.0, 0.0], [0.0, 1.0]]
     ...         ],
     ...     }
     ... )
     >>> model = tf.keras.Sequential([
```

### Comparing `molgraph-0.3.8/molgraph/layers/readout/set_gather.py` & `molgraph-0.3.9/molgraph/layers/readout/set_gather.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import tensorflow as tf
 from tensorflow import keras
-from tensorflow.keras import layers
+from keras import layers
 
 from typing import Tuple
 
 from molgraph.tensors.graph_tensor import GraphTensor
 
 
 
@@ -15,16 +15,16 @@
 
     Implementation based on Gilmer et al. (2017) [#]_ and Vinyals et al. (2016) [#]_.
 
     **Example:**
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'edge_src': [[1, 0], [1, 2, 0, 2, 1, 0]],
+    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'node_feature': [
     ...             [[1.0, 0.0], [1.0, 0.0]],
     ...             [[1.0, 0.0], [1.0, 0.0], [0.0, 1.0]]
     ...         ],
     ...     }
     ... )
     >>> model = tf.keras.Sequential([
```

### Comparing `molgraph-0.3.8/molgraph/layers/readout/transformer_encoder.py` & `molgraph-0.3.9/molgraph/layers/readout/transformer_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import tensorflow as tf
 from tensorflow import keras
-from tensorflow.keras import layers
-from tensorflow.keras import activations
+from keras import layers
+from keras import activations
 from keras.utils import tf_utils
 
 from typing import Tuple
 from typing import Union
 from typing import Callable
 
 from molgraph.tensors.graph_tensor import GraphTensor
@@ -17,16 +17,16 @@
 
     '''Transformer encoder layer for graph readout.
 
     **Example:**
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'edge_src': [[1, 0], [1, 2, 0, 2, 1, 0]],
+    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'node_feature': [
     ...             [[1.0, 0.0], [1.0, 0.0]],
     ...             [[1.0, 0.0], [1.0, 0.0], [0.0, 1.0]]
     ...         ],
     ...     }
     ... )
     >>> model = tf.keras.Sequential([
```

### Comparing `molgraph-0.3.8/molgraph/losses/link_losses.py` & `molgraph-0.3.9/molgraph/losses/link_losses.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,24 +18,24 @@
             label_smoothing=label_smoothing,
             axis=axis,
             reduction=reduction,
             name=name,
         )
 
     def call(self, positive_score, negative_score):
-        negative_score = tf.reshape(negative_score, (-1, 1))
         y_pred = tf.concat([
             positive_score, negative_score
         ], axis=0)
         y_true = tf.concat([
             tf.ones_like(positive_score), tf.zeros_like(negative_score)
         ], axis=0)
         return super().call(y_true, y_pred)
 
 
+# TODO: Make it work for len(y_true) != len(y_pred)
 @keras.utils.register_keras_serializable(package='molgraph.losses')
 class LinkContrastiveMarginLoss(keras.losses.Loss):
 
     def __init__(
         self,
         margin=1.,
         reduction=keras.losses.Reduction.AUTO,
@@ -48,14 +48,16 @@
         return tf.reduce_mean(tf.math.maximum(0., 1. - y_true + y_pred))
 
     def get_config(self):
         base_config = super().get_config()
         base_config.update({'margin': self.margin})
         return base_config
 
+
+# TODO: Make it work for len(y_true) != len(y_pred)
 @keras.utils.register_keras_serializable(package='molgraph.losses')
 class LinkContrastiveBinaryCrossentropy(keras.losses.Loss):
 
     def __init__(
         self,
         reduction=keras.losses.Reduction.AUTO,
         name='link_contrastive_bce_loss',
```

### Comparing `molgraph-0.3.8/molgraph/losses/masked_losses.py` & `molgraph-0.3.9/molgraph/losses/masked_losses.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,17 +89,17 @@
             return y_true * (1.0 - label_smoothing) + 0.5 * label_smoothing
 
         y_true = tf.cond(label_smoothing != 0., smooth_labels, lambda: y_true)
 
         return tf.cond(
             gamma != 0.0,
             lambda: keras.backend.binary_focal_crossentropy(
-                y_true, y_pred, gamma, self._from_logits),
+                y_true, y_pred, gamma=gamma, from_logits=self._from_logits),
             lambda: keras.backend.binary_crossentropy(
-                y_true, y_pred, self._from_logits))
+                y_true, y_pred, from_logits=self._from_logits))
 
     def get_config(self):
         base_config = super().get_config()
         base_config.update({
             'gamma': self._gamma,
             'from_logits': self._from_logits,
             'label_smoothing': self._label_smoothing,
```

### Comparing `molgraph-0.3.8/molgraph/metrics/masked_metrics.py` & `molgraph-0.3.9/molgraph/metrics/masked_metrics.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.8/molgraph/metrics/mean_relative_error.py` & `molgraph-0.3.9/molgraph/metrics/mean_relative_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import tensorflow as tf
 from tensorflow import keras
 
+
 @keras.utils.register_keras_serializable(package='molgraph.metrics')
 class MeanRelativeError(keras.metrics.Mean):
 
     def update_state(self, y_true, y_pred, sample_weight=None):
         y_true = tf.cast(y_true, self._dtype)
         y_pred = tf.cast(y_pred, self._dtype)
         abs_error = tf.abs(y_true - y_pred)
```

### Comparing `molgraph-0.3.8/molgraph/models/dgin.py` & `molgraph-0.3.9/molgraph/models/dgin.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     ``molgraph.chemistry.MolecularGraphEncoder(..., self_loops=True)``
     
     **Example:**
 
     >>> # Obtain GraphTensor
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'edge_src': [[1, 0], [1, 2, 0, 2, 1, 0]],
+    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'node_feature': [
     ...             [[1.0, 0.0], [1.0, 0.0]],
     ...             [[1.0, 0.0], [1.0, 0.0], [0.0, 1.0]]
     ...         ],
     ...     }
     ... )
     >>> # Build Functional model
@@ -168,16 +168,16 @@
         
         node_feature_initial = self.node_projection(
             node_feature * (1 + self.epsilon))
         
         for _ in range(self.node_message_steps):
             node_feature = propagate_node_features(
                 node_feature=node_feature, 
-                edge_dst=tensor.edge_dst,
-                edge_src=tensor.edge_src)
+                edge_src=tensor.edge_src,
+                edge_dst=tensor.edge_dst)
             node_feature = node_feature + node_feature_initial
             
         return tensor_orig.update({'node_feature': node_feature})
 
     def get_config(self) -> dict:
         base_config = super().get_config()
         config = {
```

### Comparing `molgraph-0.3.8/molgraph/models/dmpnn.py` & `molgraph-0.3.9/molgraph/models/dmpnn.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     ``molgraph.chemistry.MolecularGraphEncoder(..., self_loops=True)``
 
     **Example:**
 
     >>> # Obtain GraphTensor
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'edge_src': [[1, 0], [1, 2, 0, 2, 1, 0]],
+    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'node_feature': [
     ...             [[1.0, 0.0], [1.0, 0.0]],
     ...             [[1.0, 0.0], [1.0, 0.0], [0.0, 1.0]]
     ...         ],
     ...     }
     ... )
     >>> # Build Functional model
```

### Comparing `molgraph-0.3.8/molgraph/models/interpretability/activation_maps.py` & `molgraph-0.3.9/molgraph/models/interpretability/activation_maps.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.8/molgraph/models/interpretability/saliency.py` & `molgraph-0.3.9/molgraph/models/interpretability/saliency.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.8/molgraph/models/mpnn.py` & `molgraph-0.3.9/molgraph/models/mpnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,30 +20,30 @@
     And the update functions correspond to a single GRU by default.
 
     **Example:**
 
     >>> # Obtain GraphTensor
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'edge_src': [[1, 0], [1, 2, 0, 2, 1, 0]],
+    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'node_feature': [
     ...             [[1.0, 0.0], [1.0, 0.0]],
     ...             [[1.0, 0.0], [1.0, 0.0], [0.0, 1.0]]
     ...         ],
     ...     }
     ... )
     >>> # Build Functional model
     >>> inputs = tf.keras.layers.Input(type_spec=graph_tensor.unspecific_spec)
     >>> x = molgraph.models.MPNN(units=32, steps=4, name='mpnn')(inputs)
     >>> x = molgraph.layers.SetGatherReadout(name='readout')(x)
     >>> outputs = tf.keras.layers.Dense(10, activation='sigmoid')(x)
     >>> mpnn_classifier = tf.keras.Model(inputs, outputs)
     >>> # Make predictions
-    >>> preds = mpnn_classifier.predict(graph_tensor)
+    >>> preds = mpnn_classifier.predict(graph_tensor, verbose=0)
     >>> preds.shape
     (2, 10)
 
     Args:
         units (int, None):
             Number of hiden units of the message passing. These include the
             dense layers associated with the message functions, and GRU cells
@@ -120,38 +120,38 @@
             GraphTensor:
                 A ``GraphTensor`` with updated node features.
         '''
         tensor_orig = tensor
         if isinstance(tensor.node_feature, tf.RaggedTensor):
             tensor = tensor.merge()
 
-        edge_dst = tensor.edge_dst
         edge_src = tensor.edge_src
+        edge_dst = tensor.edge_dst
         node_feature_updated = tensor.node_feature
         # MPNN requires edge features, if edge features do not exist,
         # we initialize a ones vector.
         if not hasattr(tensor, 'edge_feature'):
             edge_feature = tf.ones(
-                shape=[tf.shape(edge_dst)[0], 1],
+                shape=[tf.shape(edge_src)[0], 1],
                 dtype=node_feature_updated.dtype)
         else:
             edge_feature = tensor.edge_feature
 
         if hasattr(self, 'node_resample'):
             node_feature_updated = self.node_resample(node_feature_updated)
 
         for _ in range(self.steps):
             if self.residual:
                 node_feature_residual = node_feature_updated
             # Perform a step of message passing (message function)
             node_feature_aggregated = message_step(
                 node_feature=node_feature_updated,
                 edge_feature=edge_feature,
-                edge_dst=edge_dst,
                 edge_src=edge_src,
+                edge_dst=edge_dst,
                 projection=self.message_projection)
             # Perform a step of GRU (update function)
             node_feature_updated, _ = self.update_step(
                 inputs=node_feature_aggregated,
                 states=node_feature_updated)
 
             if self.residual:
```

### Comparing `molgraph-0.3.8/molgraph/tensors/_graph_tensor.py` & `molgraph-0.3.9/molgraph/tensors/_graph_tensor.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.8/molgraph/tensors/graph_keras_tensor.py` & `molgraph-0.3.9/molgraph/tensors/graph_keras_tensor.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.8/molgraph/tensors/graph_tensor.py` & `molgraph-0.3.9/molgraph/tensors/graph_tensor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,160 +1,184 @@
 import tensorflow as tf
 from tensorflow.python.framework import composite_tensor
 from tensorflow.python.framework import type_spec
-from tensorflow.experimental import ExtensionType
-from tensorflow.experimental import BatchableExtensionType
 import numpy as np
 
 from typing import Optional
 from typing import Mapping
 from typing import List
 from typing import Tuple
 from typing import Union
 from typing import Any
 from typing import Type
 
 
+
 _allowable_input_types = (
     tf.Tensor,
     tf.RaggedTensor,
     np.ndarray,
     list,
     tuple
 )
-_required_fields = ['edge_dst', 'edge_src', 'node_feature']
 
-_non_updatable_fields = ['edge_dst', 'edge_src', 'graph_indicator']
+_required_fields = [
+    'edge_src', 
+    'edge_dst', 
+    'node_feature'
+]
+
+_non_updatable_fields = [
+    'edge_src', 
+    'edge_dst', 
+    'graph_indicator'
+]
 
-NestedTensors = Mapping[str, Union[tf.Tensor, tf.RaggedTensor]]
-NestedTensorSpecs = Mapping[str, Union[tf.TensorSpec, tf.RaggedTensorSpec]]
-NestedArrays = Mapping[
-    str, Union[ # TensorLike
+GraphData = Mapping[
+    str, 
+    Union[ 
         tf.Tensor,
         tf.RaggedTensor,
         np.ndarray,
         list,
         tuple
+    ] # TensorLike
+]
+
+GraphTensorData = Mapping[
+    str, 
+    Union[
+        tf.Tensor, 
+        tf.RaggedTensor
     ]
 ]
 
+GraphTensorDataSpec = Mapping[
+    str, 
+    Union[
+        tf.TensorSpec, 
+        tf.RaggedTensorSpec
+    ]
+]
 
 
 class GraphTensor(composite_tensor.CompositeTensor):
 
     '''A composite tensor encoding a molecular graph.
 
     The molecular graph (GraphTensor) could encode a single subgraph (single
     molecule) or multiple subgraphs (multiple molecules). The GraphTensor
     can either encode the molecular graph as a single (disjoint) graph (nested
     tensors) or as multiple subgraphs (nested ragged tensors). The former is
     advantageous for efficient computation while the latter is advantageous
-    for batching (via e.g., the tf._data.Dataset API).
+    for batching (via e.g., the tf.data.Dataset API).
 
     Args:
         data (dict):
-            Nested fields of the graph tensor. A dictionary of tensors
-            (tf.Tensor or tf.RaggedTensor), numpy arrays, lists or tuples.
+            Nested data of the graph tensor. Specifically, a dictionary of 
+            tensors (tf.Tensor or tf.RaggedTensor), numpy arrays, lists or tuples.
             Internally, values (of dict) will be converted to tensors.
         spec: (dict):
-            Nested specs (associated with data). A dictionary of
-            tensor specs (tf.TensorSpec or tf.RaggedTensorSpec).
-            Nested structure of spec should be match nested structure of data.
+            Nested specs (associated with nested data). Specifically, a dictionary 
+            of tensor specs (tf.TensorSpec or tf.RaggedTensorSpec). Nested structure 
+            of spec should be match nested structure of data.
         **data_kwargs (tf.Tensor, tf.RaggedTensor, np.array, list, tuple):
-            Components passed as keyword arguments. Can be combined with data.
+            Components passed as keyword arguments.
 
     **Examples:**
 
-    Initialize ``GraphTensor`` with dict of ragged arrays:
+    Initialize ``GraphTensor`` by passing a dict of ragged arrays,
+    resulting in a graph tensor instance with nested tf.RaggedTensor types:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'edge_src': [[1, 0], [1, 2, 0, 2, 1, 0]],
+    ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
     ...         'node_feature': [
     ...             [[1.0, 0.0], [1.0, 0.0]],
     ...             [[1.0, 0.0], [1.0, 0.0], [0.0, 1.0]]
     ...         ],
     ...     }
     ... )
     >>> graph_tensor.shape
     TensorShape([2, None, 2])
 
-    Initialize ``GraphTensor`` with dict of arrays:
+    Initialize ``GraphTensor`` by passing a dict of "rectangular" arrays,
+    resulting in a graph tensor instance with nested tf.Tensor types:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'node_feature': [
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [0.0, 1.0]
     ...         ],
     ...         'graph_indicator': [0, 0, 1, 1, 1],
     ...     }
     ... )
     >>> graph_tensor.shape
     TensorShape([5, 2])
 
-    Initialize ``GraphTensor`` with keyword arguments:
+    Initialize ``GraphTensor`` by passing data as keyword arguments:
 
     >>> graph_tensor = molgraph.GraphTensor(
-    ...     edge_dst=[[0, 1], [0, 0, 1, 1, 2, 2]],
     ...     edge_src=[[1, 0], [1, 2, 0, 2, 1, 0]],
+    ...     edge_dst=[[0, 1], [0, 0, 1, 1, 2, 2]],
     ...     node_feature=[
     ...         [[1.0, 0.0], [1.0, 0.0]],
     ...         [[1.0, 0.0], [1.0, 0.0], [0.0, 1.0]]
     ...     ]
     ... )
     >>> graph_tensor.shape
     TensorShape([2, None, 2])
 
     Merge subgraphs of ``GraphTensor``:
 
     >>> graph_tensor = molgraph.GraphTensor(
-    ...     edge_dst=[[0, 1], [0, 0, 1, 1, 2, 2]],
     ...     edge_src=[[1, 0], [1, 2, 0, 2, 1, 0]],
+    ...     edge_dst=[[0, 1], [0, 0, 1, 1, 2, 2]],
     ...     node_feature=[
     ...         [[1.0, 0.0], [1.0, 0.0]],
     ...         [[1.0, 0.0], [1.0, 0.0], [0.0, 1.0]]
     ...     ]
     ... )
     >>> graph_tensor = graph_tensor.merge()
     >>> graph_tensor.shape
     TensorShape([5, 2])
 
     Separate (merged) subgraphs of ``GraphTensor``:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'node_feature': [
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [0.0, 1.0]
     ...         ],
     ...         'graph_indicator': [0, 0, 1, 1, 1],
     ...     }
     ... )
     >>> graph_tensor = graph_tensor.separate()
     >>> graph_tensor.shape
     TensorShape([2, None, 2])
 
-    Add, update and remove nested fields of ``GraphTensor``:
+    Add, update and remove data from ``GraphTensor``:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'node_feature': [
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [0.0, 1.0]
     ...         ],
@@ -171,25 +195,25 @@
     >>> # Update exisiting field
     >>> graph_tensor = graph_tensor.update({
     ...     'node_feature': random_feature_2})
     >>> # Remove field
     >>> graph_tensor = graph_tensor.remove(['node_random_feature'])
     >>> graph_tensor
     GraphTensor(
-      edge_dst=<tf.Tensor: shape=(8,), dtype=int32>,
       edge_src=<tf.Tensor: shape=(8,), dtype=int32>,
+      edge_dst=<tf.Tensor: shape=(8,), dtype=int32>,
       node_feature=<tf.Tensor: shape=(5, 2), dtype=float32>,
       graph_indicator=<tf.Tensor: shape=(5,), dtype=int32>)
 
-    Use spec of ``GraphTensor`` in model:
+    Use spec of ``GraphTensor`` in ``keras.Sequential`` model:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'node_feature': [
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [0.0, 1.0]
     ...         ],
@@ -205,16 +229,16 @@
     >>> gnn_model.output_shape
     (5, 16)
 
     Use unspecific spec of ``GraphTensor`` instead (recommended):
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
+    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'node_feature': [
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [1.0, 0.0],
     ...             [0.0, 1.0]
     ...         ],
@@ -228,213 +252,243 @@
     ...     molgraph.layers.GCNConv(16, activation='relu')
     ... ])
     >>> gnn_model.output_shape
     (None, 16)
 
     '''
 
-    __slots__ = ['_data', '_spec']
+    __slots__ = ('_data', '_spec')
 
     def __init__(
         self,
-        data: Optional[NestedArrays] = None,
-        spec: Optional[NestedTensorSpecs] = None,
-        **data_kwargs # allows to pass data as keyword arguments
+        data: Optional[GraphData] = None,
+        spec: Optional[GraphTensorDataSpec] = None,
+        **data_kwargs 
     ) -> None:
+        
         super().__init__()
 
         if data is None:
             data = {}
 
         data.update(data_kwargs)
-        data = _maybe_convert_to_tensors(
-            data, check_keys=True, check_values=True)
+
+        data = _convert_to_tensors(
+            data, check_keys=True, check_values=True
+        )
 
         if spec is None:
             spec = tf.nest.map_structure(tf.type_spec_from_value, data)
         else:
             tf.nest.assert_same_structure(data, spec)
 
         data, spec = _maybe_add_graph_indicator(data, spec)
 
         self._spec = GraphTensorSpec(spec)
         self._data = data
 
-    # TODO: modify spec accordingly
-    def update(self, new_data: NestedArrays) -> 'GraphTensor':
-        '''Updates existing data fields or adds new data fields.
-
-        Constraints are put on the update method: new data needs to
-        match the size of existing data (e.g., same number of nodes or edges).
+    # TODO: should spec be modified?
+    def update(self, new_data: GraphData) -> 'GraphTensor':
+        '''Updates existing data or adds new data to GraphTensor instance.
+
+        Constraints are put on the update method: 
+            - New data needs to match the size of existing data (i.e., it has 
+              to have the same number of nodes or edges as the existing data).
+            - Furthermore, names of new data need to prepend either 'node' (if 
+              associated with nodes) or 'edge' (if associated with edges) to 
+              allow the GraphTensor to keep track of what data belong to which. 
 
         Args:
             new_data (dict):
-                Nested fields. A dictionary of tensors (``tf.Tensor`` or
-                ``tf.RaggedTensor``), numpy arrays, lists or tuples.
+                Nested data. Specifically, a dictionary of tensors (either 
+                ``tf.Tensor`` or ``tf.RaggedTensor``), `np.array`s, ``list``s 
+                or ``tuple``s.
 
         Returns:
-            An updated ``GraphTensor`` based on 'new_data'.
+            An updated ``GraphTensor`` instance.
 
         '''
-
-        new_data = _maybe_convert_to_tensors(new_data, check_values=True)
-
-        data = self._data.copy()
-
-        def convert_tensor(
+        def convert_value(
             new_value: Union[tf.Tensor, tf.RaggedTensor],
             old_value: Union[tf.Tensor, tf.RaggedTensor],
         ) -> Union[tf.Tensor, tf.RaggedTensor]:
+            
             if (
                 isinstance(new_value, tf.RaggedTensor) and
                 isinstance(old_value, tf.Tensor)
             ):
                 new_value = new_value.flat_values
+                _check_shape(old_value, new_value)
             elif (
-                isinstance(new_value, tf.Tensor) and
+                isinstance(new_value, tf.Tensor) and  
                 isinstance(old_value, tf.RaggedTensor)
             ):
                 new_value = old_value.with_flat_values(new_value)
+                # No need to assert shape as the method will throw an error 
+                # if shapes are mismatching.
+                #
+                # Edge case: User updates this graph tensor instance with values 
+                #            from another completely different graph, though
+                #            with the same number of total nodes (or edges);
+                #            `with_flat_values()` will accept it, though
+                #            the resulting ragged dimensions (`row_lengths()`)
+                #            could be a mismatch between this graph tensor instance
+                #            and the other graph from which the values come from.
+                #            Although this is very rare, it is important that the 
+                #            user in that case converts the tf.Tensor values into 
+                #            tf.RaggedTensor values of correct ragged dimensions 
+                #            (correct `row_lengths()`).
             else:
                 new_value = new_value
+                _check_shape(old_value, new_value)
 
             return new_value
 
-        for k in list(new_data.keys()):
+        new_data = _convert_to_tensors(new_data, check_values=True)
 
-            if k in _non_updatable_fields:
-                raise ValueError(f'{k} cannot be updated.')
+        data = self._data.copy()
+
+        fields = list(new_data.keys())
 
-            new_value = new_data.pop(k)
+        for field in fields:
 
-            # Make sure the new value has the same number of nodes or edges
-            # as the exisiting values of the graph tensor.
-            _assert_compatible_sizes(
-                new_value, data['node_feature'], data['edge_dst'])
+            # TODO: should we allow edge_src, edge_dst and graph_indicator to be updatable?
+            if field in _non_updatable_fields:
+                raise ValueError(f'{field} cannot be updated.')
 
-            if k in data:
-                data[k] = convert_tensor(new_value, data[k])
+            new_value = new_data.pop(field)
+
+            if field in data:
+                data[field] = convert_value(new_value, data[field])
             else:
-                if 'node' not in k and 'edge' not in k:
+                if not field.startswith('node') and not field.startswith('edge'):
                     raise ValueError(
-                        'Please prepend `node_` or `edge_` to the new fields added, ' + 
+                        'Please prepend "node" or "edge" to the new data added, ' + 
                         'depending on if they are associated with the nodes or edges ' + 
-                        'of the graph.')
-                data[k] = tf.cond(
-                    _compatible_sizes(new_value, data['node_feature']),
-                    lambda: convert_tensor(new_value, data['node_feature']),
-                    lambda: convert_tensor(new_value, data['edge_dst']))
+                        'of the graph respectively.'
+                    )
+                elif field.startswith('edge'):
+                    data[field] = convert_value(new_value, data['edge_src'])
+                else:
+                    data[field] = convert_value(new_value, data['node_feature'])
+
         return self.__class__(data)
 
-    # TODO: modify spec accordingly
+    # TODO: should spec be modified?
     def remove(
         self,
         fields: Union[str, List[str]]
     ) -> 'GraphTensor':
-        '''Removes data fields based on 'fields'.
+        '''Removes data from the ``GraphTensor`` instance.
 
         Args:
             fields (str, list[str]):
-                Data fields to be removed from the ``GraphTensor``.
-                Cannot remove 'edge_dst', 'edge_src' or 'graph_indicator'.
+                Data to be removed from the ``GraphTensor``. Currently, 
+                'edge_dst', 'edge_src' or 'graph_indicator' cannot be removed
+                from the ``GraphTensor`` instance.
 
         Returns:
-            GraphTensor: An updated graph tensor without fields specified
-            by 'fields'.
+            GraphTensor: An updated ``GraphTensor`` instance.
         '''
         data = self._data.copy()
+
         if isinstance(fields, str):
             fields = [fields]
+
         for field in fields:
+            
             if field in _non_updatable_fields:
                 raise ValueError(f'{field} cannot be removed.')
+        
             data.pop(field)
+
         return self.__class__(data)
 
     def merge(self) -> 'GraphTensor':
         '''Merges subgraphs into a single disjoint graph.
 
         Returns:
-            GraphTensor: A graph tensor
-            with nested tensors (``tf.Tensor``).
+            GraphTensor: A ``GraphTensor`` instance with nested "rectangular" tensors.
         '''
-        _assert_mergeable(self._data)
+        _check_mergeable(self._data)
 
         data = self._data.copy()
 
         increment = data['node_feature'].row_starts()
-        indices = data['edge_dst'].value_rowids()
+        indices = data['edge_src'].value_rowids()
         graph_indicator = data['node_feature'].value_rowids()
-        increment = tf.cast(increment, dtype=data['edge_dst'].dtype)
+        increment = tf.cast(increment, dtype=data['edge_src'].dtype)
         data = tf.nest.map_structure(lambda x: x.flat_values, data)
-        data['edge_dst'] += tf.gather(increment, indices)
         data['edge_src'] += tf.gather(increment, indices)
+        data['edge_dst'] += tf.gather(increment, indices)
         data['graph_indicator'] = graph_indicator
 
         return self.__class__(data)
 
     def separate(self) -> 'GraphTensor':
         '''Separates the (single disjoint) graph into its subgraphs.
 
         Returns:
-            GraphTensor: A graph tensor
-            with nested ragged tensors (``tf.RaggedTensor``).
+            GraphTensor: A ``GraphTensor`` instance with nested ragged tensors.
         '''
-        _assert_separable(self._data)
-
-        data = self._data.copy()
-
-        if 'graph_indicator' not in data:
-            return self.__class__(
-                tf.nest.map_structure(
-                    lambda x: tf.RaggedTensor.from_row_starts(x, [0]),
-                    data))
-
-        data = _remove_intersubgraph_edges(data)
-
-        graph_indicator = data.pop('graph_indicator')
-        edge_dst = data.pop('edge_dst')
-        edge_src = data.pop('edge_src')
-        graph_indicator_edges = tf.gather(graph_indicator, edge_dst)
 
         def to_ragged_tensor(
             tensor: Union[tf.Tensor, tf.RaggedTensor],
             graph_indicator: tf.Tensor,
             num_subgraphs: tf.Tensor,
         ) -> tf.RaggedTensor:
             if isinstance(tensor, tf.RaggedTensor):
                 return tensor
             return tf.RaggedTensor.from_value_rowids(
                 tensor, graph_indicator, num_subgraphs)
         
+
+        _check_separable(self._data)
+
+        data = self._data.copy()
+
+        if 'graph_indicator' not in data:
+            return self.__class__(
+                tf.nest.map_structure(
+                    lambda x: tf.RaggedTensor.from_row_starts(x, [0]), data
+                )
+            )
+
+        data = _remove_intersubgraph_edges(data)
+
+        graph_indicator = data.pop('graph_indicator')
+        edge_src = data.pop('edge_src')
+        edge_dst = data.pop('edge_dst')
+        graph_indicator_edges = tf.gather(graph_indicator, edge_src)
         num_subgraphs = self.num_subgraphs
 
-        data_edges = {k: v for (k, v) in data.items() if 'edge' in k}
-        # TODO: "not 'edge'" because of 'positional_encoding'. 
-        #       Change to 'node_position' ?
-        data_nodes = {k: v for (k, v) in data.items() if not 'edge' in k}
+        edge_data, node_data = {}, {}
+        for key, value in data.items():
+            if key.startswith('edge'):
+                edge_data[key] = value
+            else:
+                node_data[key] = value
 
-        data_edges = tf.nest.map_structure(
+        edge_data = tf.nest.map_structure(
             lambda x: to_ragged_tensor(
-                x, graph_indicator_edges, num_subgraphs), data_edges)
-        data_nodes = tf.nest.map_structure(
+                x, graph_indicator_edges, num_subgraphs), edge_data)
+        
+        node_data = tf.nest.map_structure(
             lambda x: to_ragged_tensor(
-                x, graph_indicator, num_subgraphs), data_nodes)   
+                x, graph_indicator, num_subgraphs), node_data)   
 
         decrement = tf.gather(
-            data_nodes['node_feature'].row_starts(), graph_indicator_edges)
-        decrement = tf.cast(decrement, dtype=edge_dst.dtype)
-        data_edges['edge_dst'] = tf.RaggedTensor.from_value_rowids(
-            edge_dst - decrement, graph_indicator_edges, num_subgraphs)
-        data_edges['edge_src'] = tf.RaggedTensor.from_value_rowids(
+            node_data['node_feature'].row_starts(), graph_indicator_edges)
+        decrement = tf.cast(decrement, dtype=edge_src.dtype)
+        edge_data['edge_src'] = tf.RaggedTensor.from_value_rowids(
             edge_src - decrement, graph_indicator_edges, num_subgraphs)
-
-        data_nodes.update(data_edges)
-
-        return self.__class__(data_nodes)
+        edge_data['edge_dst'] = tf.RaggedTensor.from_value_rowids(
+            edge_dst - decrement, graph_indicator_edges, num_subgraphs)
+        
+        return self.__class__({**node_data, **edge_data})
 
     @property
     def _type_spec(self) -> 'GraphTensorSpec':
         'CompositeTensor API.'
         return self._spec
 
     @property
@@ -446,15 +500,15 @@
         '''
         return self._type_spec
 
     @property
     def unspecific_spec(self):
         '''Unspecific spec of ``GraphTensor``.
 
-        Specifically, ``shape[0]`` of each nested spec is set to ``None``.
+        Specifically, ``shape[0]`` for all nested data specs are set to ``None``.
 
         It is recommended to use the ``unspecific_spec`` instead of ``spec``,
         especially when using the ``tf.saved_model`` API.
         '''
         def modify_spec(x):
             if isinstance(x, tf.RaggedTensorSpec):
                 return tf.RaggedTensorSpec(
@@ -488,68 +542,70 @@
     @property
     def num_subgraphs(self):
         if 'graph_indicator' in self._data:
             return tf.math.reduce_max(self._data['graph_indicator']) + 1
         elif isinstance(self._data['node_feature'], tf.RaggedTensor):
             return self._data['node_feature'].nrows()
         else:
-            return tf.constant(1, dtype=self._data['edge_dst'].dtype)
+            return tf.constant(1, dtype=self._data['edge_src'].dtype)
 
     def __getattr__(self, name: str) -> Union[tf.Tensor, tf.RaggedTensor, Any]:
-        '''Extract data fields as an attribute.
+        '''Extract any nested data as an attribute.
 
         Args:
             name (str):
-                The data fields to be extracted.
+                The data to be extracted. E.g. ``graph_tensor.node_feature``
 
         Returns:
-            Data fields based on 'name'.
-            Either a ``tf.Tensor`` or ``tf.RaggedTensor``.
+            Specific ``tf.Tensor`` or ``tf.RaggedTensor`` data from ``GraphTensor`` instance.
         '''
         if name in object.__getattribute__(self, '_data'):
             return self._data[name]
         return object.__getattribute__(self, name)
 
     def __getitem__(
         self,
         index: Union[str, int, List[int]]
     ) -> Union[tf.RaggedTensor, tf.Tensor, 'GraphTensor']:
-        '''Extract a data field or subgraphs via indexing.
+        '''Extract any nested data or subgraphs via indexing.
 
         Args:
             index (str, int, list[int]):
-                If str, extracts a data field of ``GraphTensor``; if int or
-                list[int], extracts specific subgraph(s) of ``GraphTensor``.
+                If ``str``, extracts specific data from ``GraphTensor`` instance; 
+                if ``int`` or ``list[int]``, extracts specific subgraph(s) of 
+                ``GraphTensor`` instance.
 
         Returns:
-            Either a ``tf.Tensor`` or ``tf.RaggedTensor`` (if index is a str)
-            or a ``GraphTensor`` (if index is a int or list[int]).
+            Either specific ``tf.Tensor`` or ``tf.RaggedTensor`` data (if index 
+            is a ``str``); or a ``GraphTensor`` instance (if index is an ``int`` 
+            or ``list[int]``).
         '''
         if isinstance(index, str):
             return self._data[index]
         if isinstance(index, slice):
             index = _slice_to_tensor(index, self.num_subgraphs)
         return tf.gather(self, index)
 
     def __iter__(self):
-        # Makes GraphTensor iterable
         if not tf.executing_eagerly():
             raise ValueError(
-                'Can only iterate over `GraphTensor` in eager mode.')
+                'Can only iterate over `GraphTensor` in eager mode.'
+            )
         return _Iterator(self, limit=self.num_subgraphs)
 
     def __repr__(self) -> str:
         fields = []
         for key, value in self._spec._data_spec.items():
             if isinstance(self._data[key], tf.RaggedTensor):
                 # Include value.ragged_rank and value.row_splits_dtype.name?
                 fields.append(
                     '{}=<tf.RaggedTensor: '.format(key) +
                     'shape={}, '.format(value.shape) +
                     'dtype={}>'.format(value.dtype.name)
+                    # TODO: include e.g. ragged_rank?
                 )
             elif isinstance(self._data[key], tf.Tensor):
                 fields.append(
                     '{}=<tf.Tensor: '.format(key) +
                     'shape={}, '.format(value.shape) +
                     'dtype={}>'.format(value.dtype.name)
                 )
@@ -559,19 +615,19 @@
 
         return f'GraphTensor(\n  ' + ',\n  '.join(fields) + ')'
 
 
 @type_spec.register('molgraph.tensors.graph_tensor.GraphTensorSpec')
 class GraphTensorSpec(type_spec.BatchableTypeSpec):
 
-    __slots__ = ['_data_spec', '_shape', '_dtype']
+    __slots__ = ('_data_spec', '_shape', '_dtype')
 
     def __init__(
         self,
-        data_spec: NestedTensorSpecs,
+        data_spec: GraphTensorDataSpec,
         shape: Optional[tf.TensorShape] = None,
         dtype: Optional[tf.DType] = None
     ) -> None:
         super().__init__()
 
         self._data_spec = data_spec
 
@@ -612,41 +668,41 @@
     @classmethod
     def from_value(cls, value: GraphTensor) -> 'GraphTensorSpec':
         # ExtensionType API
         return value._type_spec
 
     def _serialize(
         self
-    ) -> Tuple[NestedTensorSpecs, tf.TensorShape, tf.DType]:
+    ) -> Tuple[GraphTensorDataSpec, tf.TensorShape, tf.DType]:
         # ExtensionType API
         return (self._data_spec, self._shape, self._dtype)
 
     @classmethod
     def _deserialize(
         cls,
         serialization: Tuple[
-            NestedTensorSpecs,
+            GraphTensorDataSpec,
             Union[tf.TensorShape, None],
             Union[tf.DType, None]
         ]
     ) -> 'GraphTensorSpec':
         # ExtensionType API
         data_spec, shape, dtype = serialization
         return cls(data_spec, shape, dtype)
 
     @property
-    def _component_specs(self) -> NestedTensorSpecs:
+    def _component_specs(self) -> GraphTensorDataSpec:
         # ExtensionType API
         return self._data_spec
 
-    def _to_components(self, value: GraphTensor) -> NestedTensors:
+    def _to_components(self, value: GraphTensor) -> GraphTensorData:
         # ExtensionType API
         return value._data.copy()
 
-    def _from_components(self, components: NestedTensors) -> GraphTensor:
+    def _from_components(self, components: GraphTensorData) -> GraphTensor:
         # ExtensionType API
         return self.value_type(components, self._data_spec)
 
     def _batch(self, batch_size: Union[int, None]) -> 'GraphTensorSpec':
         # BatchableExtensionType API
         batched_data_spec = tf.nest.map_structure(
             lambda spec: spec._batch(batch_size), self._data_spec)
@@ -669,197 +725,187 @@
         return self._shape
 
     def _to_legacy_output_classes(self):
         # Legacy method of ExtensionType API
         return self
 
 
-def _remove_intersubgraph_edges(data: NestedTensors) -> NestedTensors:
-    '''Removes edges that connects two different subgraphs.
-
-    Applied only when graph_tensor.separate() is called
-    '''
-    subgraphs_dst = tf.gather(data['graph_indicator'], data['edge_dst'])
-    subgraphs_src = tf.gather(data['graph_indicator'], data['edge_src'])
-    mask = tf.where((subgraphs_dst - subgraphs_src) == 0, True, False)
-    data['edge_dst'] = tf.boolean_mask(data['edge_dst'], mask)
-    data['edge_src'] = tf.boolean_mask(data['edge_src'], mask)
-    for key in data.keys():
-        if key.startswith('edge') and key != 'edge_dst' and key != 'edge_src':
-            data[key] = tf.boolean_mask(data[key], mask)
-    return data
+def _assert(test: bool, message: str) -> None:
+    'Helper function to make assert statements.'
+    assert_op = tf.Assert(tf.reduce_all(test), [message])
+    if hasattr(assert_op, 'mark_used'):
+        assert_op.mark_used()
 
-def _maybe_convert_to_tensors(
-    data: NestedArrays,
-    check_values: bool = False,
-    check_keys: bool = False,
-) -> NestedTensors:
-    'Converts data values to tensors'
+def _check_shape(
+    a: Union[tf.Tensor, tf.RaggedTensor],
+    b: Union[tf.Tensor, tf.RaggedTensor],
+) -> None:
+    'Assert that a and b have the same number of nodes (or edges)'
 
-    if check_values:
-        _check_data_values(data)
+    _assert(type(a) == type(b), ['a and b need to be the same type'])
 
-    if check_keys:
-        _check_data_keys(data)
+    if isinstance(a, tf.Tensor):
+        _assert(
+            test=(tf.shape(a)[0] == tf.shape(b)[0]), 
+            message=(
+                'The shape of input `a` does not match the shape of input `b`'
+            )
+        )
+    else:
+        _assert(
+            test=(tf.shape(a)[:2] == tf.shape(b)[:2]), 
+            message=(
+                'The shape of input `a` does not match the shape of input `b`'
+            )
+        )
 
-    def _is_rectangular(x):
-        'Checks if tensor is rectangular (non-ragged)'
-        lengths = set()
-        for xi in x:
-            if not isinstance(xi, (tf.Tensor, np.ndarray, list, tuple)):
-                lengths.add(0)
-            else:
-                lengths.add(len(xi))
-        return len(lengths) <= 1
+def _check_tensor_types(data: GraphTensorData) -> None:
+    'Assert that all graph data are of the same tensor type.'
+    tests = [isinstance(x, tf.Tensor) for x in data.values()]
+    same_types = all(tests) or not any(tests)
+    _assert(
+        same_types, (
+            f'Nested tensors are not the same type. ' +
+             'Found both `tf.Tensor`s and `tf.RaggedTensor`s'
+        )
+    )
 
-    def maybe_convert(x):
-        'Convert to tensor or ragged tensor if needed'
-        if tf.is_tensor(x):
-            if isinstance(x, tf.Tensor):
-                return x
-            elif isinstance(x, tf.RaggedTensor):
-                _check_ragged_rank(x)
-                return x
-            else:
-                raise ValueError(
-                    'Tensor needs to be either `tf.Tensor` or `tf.RaggedTensor`.')
-        if _is_rectangular(x):
-            return tf.convert_to_tensor(x)
-        # TODO: slow; implement something like "fast_convert_to_ragged()"
-        return tf.ragged.constant(x, ragged_rank=1) 
+def _check_tensor_ranks(data: GraphTensorData) -> None:
+    'Assert that all graph data have the expected rank.'
+    for key, value in data.items():
+        max_rank = 1 if isinstance(value, tf.Tensor) else 2
+        if key in ['edge_dst', 'edge_src', 'graph_indicator']:
+            _assert(tf.rank(value) <= max_rank, '')
+        elif key in ['node_feature', 'edge_feature']:
+            _assert(tf.rank(value) <= max_rank+1, '')
+        else:
+            _assert(tf.rank(value) <= max_rank+1, '')
 
-    data = {k: maybe_convert(v) for (k, v) in data.items()}
-    _check_tensor_types(data)
-    return data
 
-def _check_data_keys(data: NestedArrays):
-    'Asserts that necessary fields exist in the graph (tensor)'
+def _check_data_keys(data: GraphData) -> None:
+    'Assert that required graph data exist.'
     for req_field in _required_fields:
-        assert_op = tf.Assert(
+        _assert(
             req_field in data, 
-            [f'`data` requires `{req_field}` field'])
-        _maybe_mark_used(assert_op)
-    return
+            f'`data` requires `{req_field}` field'
+        )
 
-def _check_data_values(data: NestedArrays):
-    'Asserts that the values of the data fields are of correct type'
+def _check_data_values(data: GraphData) -> None:
+    'Assert that all inputted graph data have the expected type'
     for key, value in data.items():
-        assert_op = tf.Assert(
-            isinstance(value, _allowable_input_types),
-            [
+        _assert(
+            isinstance(value, _allowable_input_types), (
                 f'Field `{key}` is needs to be a `tf.Tensor`, ' +
                 '`tf.RaggedTensor`, `np.ndarray`, `list` or `tuple`'
-            ]
+            )
         )
-        _maybe_mark_used(assert_op)
-    return
 
-def _check_tensor_types(data: NestedTensors):
-    'Asserts that all nested values of data are of the same tensor type'
-    tests = [isinstance(x, tf.Tensor) for x in data.values()]
-    same_types = all(tests) or not any(tests)
-    assert_op = tf.Assert(
-        same_types, [
-            f'Nested tensors are not the same type. ' +
-             'Found both `tf.Tensor`s and `tf.RaggedTensor`s'])
-    _maybe_mark_used(assert_op)
-    return
-
-def _check_ragged_rank(x: tf.RaggedTensor):
-    assert_op = tf.Assert(
-        tf.math.equal(x.ragged_rank, 1),
-        ['Ragged rank of field needs to be 1.'])
-    _maybe_mark_used(assert_op)
-    return
+def _check_mergeable(data: GraphTensorData) -> None:
+    'Assert that all nested tensors are ragged.'
+    all_ragged = all([
+        isinstance(x, tf.RaggedTensor) for x in data.values()
+    ])
+    _assert(all_ragged, (
+            'All data values need to be `tf.RaggedTensor`s to be merged.'
+        )
+    )
 
-def _compatible_sizes(
-    a: Union[tf.Tensor, tf.RaggedTensor],
-    b: Union[tf.Tensor, tf.RaggedTensor],
-) -> bool:
-    'Checks if the two inputs have the same number of nodes or edges'
-    def _get_size(x):
-        'Get number of nodes or edges'
-        if isinstance(x, tf.RaggedTensor):
-            x = x.flat_values
-        return tf.shape(x)[0]
-    return _get_size(a) == _get_size(b)
-
-def _assert_compatible_sizes(
-    target: Union[tf.Tensor, tf.RaggedTensor],
-    *comparators: Union[tf.Tensor, tf.RaggedTensor]
-):
-    assert_op = tf.Assert(
-        tf.math.reduce_any(
-            tf.nest.map_structure(
-                lambda comparator: _compatible_sizes(target, comparator),
-                comparators
-            )
-        ), [
-            'At least one of the added fields does not match ' +
-            'the size of the existing fields. Namely, one of the ' +
-            'added fields did not have the same numeber of ' +
-            'nodes or edges as the existig fields'
-        ]
+def _check_separable(data: GraphTensorData) -> None:
+    'Assert that all nested tensors are non-ragged'
+    all_non_ragged = all([
+        isinstance(x, tf.Tensor) for x in data.values()
+    ])
+    _assert(all_non_ragged, (
+            'All data values need to be `tf.Tensor`s to be separated.'
+        )
     )
-    _maybe_mark_used(assert_op)
-    return
+
+def _convert_to_tensors(
+    data: GraphData,
+    check_values: bool = False,
+    check_keys: bool = False,
+) -> GraphTensorData:
+    'Converts graph data (possibly ``np.array``s, ``list``s or ``tuple``s) to tensors.'
+
+    if check_keys:
+        _check_data_keys(data)
+
+    if check_values:
+        _check_data_values(data)
+
+    def to_tensor(x):
+        if not tf.is_tensor(x):
+            try:
+                return tf.convert_to_tensor(x)
+            except:
+                # TODO: slow; implement something like ``fast_convert_to_ragged()```
+                return tf.ragged.constant(x, ragged_rank=1)
+        else:
+            return x
+        
+    data = {k: to_tensor(v) for (k, v) in data.items()}
+
+    _check_tensor_types(data)
+    _check_tensor_ranks(data)
+
+    return data
 
 def _maybe_add_graph_indicator(
-    data: NestedTensors,
-    spec: NestedTensorSpecs,
-) -> NestedTensors:
-    'Maybe adds `graph_indicator` to data and spec.'
+    data: GraphTensorData,
+    spec: GraphTensorDataSpec,
+) -> GraphTensorData:
+    'Adds a `graph_indicator` if necessary.'
     if (
-        'graph_indicator' not in data and
-        isinstance(data['node_feature'], tf.Tensor) and
-        not isinstance(spec['node_feature'], tf.RaggedTensorSpec)
+        'graph_indicator' not in data 
+        and isinstance(data['node_feature'], tf.Tensor) 
+        and not isinstance(spec['node_feature'], tf.RaggedTensorSpec)
     ):
         data['graph_indicator'] = tf.zeros(
             tf.shape(data['node_feature'])[0],
-            dtype=data['edge_dst'].dtype)
+            dtype=data['edge_src'].dtype)
         spec['graph_indicator'] = tf.type_spec_from_value(
             data['graph_indicator'])
-        if isinstance(spec['edge_dst'], tf.RaggedTensorSpec):
+        if isinstance(spec['edge_src'], tf.RaggedTensorSpec):
             x = spec['graph_indicator']
             spec['graph_indicator'] = tf.RaggedTensorSpec(
-                x.shape, x.dtype, spec['edge_dst'].ragged_rank, spec['edge_dst'].row_splits_dtype
+                x.shape, x.dtype, spec['edge_src'].ragged_rank, spec['edge_src'].row_splits_dtype
             )
     return data, spec
 
-def _assert_mergeable(data: NestedTensors):
-    'Asserts that all nested tensors are ragged.'
-    assert_op = tf.Assert(
-        all([isinstance(x, tf.RaggedTensor) for x in data.values()]),
-        [f'All data values need to be `tf.RaggedTensor`s to be merged'])
-    _maybe_mark_used(assert_op)
-    return
-
-def _assert_separable(data: NestedTensors):
-    'Asserts that all nested tensors are non-ragged'
-    assert_op = tf.Assert(
-        all([isinstance(x, tf.Tensor) for x in data.values()]),
-        [f'All data values need to be `tf.Tensor`s to be separated'])
-    _maybe_mark_used(assert_op)
-    return
+def _remove_intersubgraph_edges(data: GraphTensorData) -> GraphTensorData:
+    '''Removes edges that connects two different subgraphs.
+
+    Applied only when graph_tensor.separate() is called, 
+    wherein we are "forced" to remove them.
+    '''
+    subgraphs_src = tf.gather(data['graph_indicator'], data['edge_src'])
+    subgraphs_dst = tf.gather(data['graph_indicator'], data['edge_dst'])
+    # Fine the intersubgraph edges:
+    mask = tf.where((subgraphs_dst - subgraphs_src) == 0, True, False)
+    # Remove these edges (including data that is associated with edges):
+    for key in data.keys():
+        if key.startswith('edge'):
+            data[key] = tf.boolean_mask(data[key], mask)
+    return data
 
 def _slice_to_tensor(slice_obj: slice, limit: int) -> tf.Tensor:
     '''Converts slice to a tf.range, which can subsequently be used with
     tf.gather to gather subgraphs.
 
     Note: GraphTensor is currently irreversible (e.g., x[::-1] or x[::-2]
     will not work).
     '''
     start = slice_obj.start
     stop = slice_obj.stop
     step = slice_obj.step
 
-    assert_op = tf.Assert(
+    _assert(
         step is None or not (step < 0 or step == 0),
-        ['Slice step cannot be negative or zero.'])
-    _maybe_mark_used(assert_op)
+        'Slice step cannot be negative or zero.'
+    )
 
     limit = tf.convert_to_tensor(limit)
 
     if stop is None:
         stop = limit
     else:
         stop = tf.convert_to_tensor(stop)
@@ -888,18 +934,38 @@
     else:
         step = tf.convert_to_tensor(step)
 
     start = tf.cond(start > stop, lambda: stop, lambda: start)
 
     return tf.range(start, stop, step)
 
-def _maybe_mark_used(assert_op):
-    if hasattr(assert_op, 'mark_used'):
-        assert_op.mark_used()
-    return
+
+# Make GraphTensor iterable:
+
+class _Iterator:
+
+    __slots__ = ['_iterable', '_index', '_limit']
+
+    def __init__(self, iterable: GraphTensor, limit: int) -> None:
+        self._iterable = iterable
+        self._limit = limit
+        self._index = 0
+
+    def __iter__(self):
+        return self
+
+    def __next__(self):
+        if self._index == self._limit:
+            raise StopIteration
+        result = self._iterable[self._index]
+        self._index += 1
+        return result
+
+
+# Override default tensorflow implemenations for GraphTensor:
 
 @tf.experimental.dispatch_for_api(tf.shape)
 def graph_tensor_tf_shape(
     input: GraphTensor,
     out_type=tf.dtypes.int32,
     name=None
 ):
@@ -934,15 +1000,14 @@
     params = GraphTensor(data)
 
     if not ragged and isinstance(params._data['node_feature'], tf.RaggedTensor):
         params = params.merge()
 
     return params
 
-
 @tf.experimental.dispatch_for_api(tf.concat)
 def graph_tensor_concat(
     values: List[GraphTensor],
     axis: int = 0,
     name: str = 'concat'
 ) -> GraphTensor:
     '''Concatenates list of graph tensors into a single graph tensor.
@@ -951,19 +1016,19 @@
     the batches (of possibly `GraphTensor`s).
     '''
 
     if axis is not None and axis != 0:
         raise ValueError(
             f'axis=0 is required for `{values[0].__class__.__name__}`s.')
 
-    def fast_ragged_stack(component_data, dtype):
-        row_lengths = [len(x) for x in component_data]
-        component_data_concat = tf.concat(component_data, axis=0)
+    def fast_ragged_stack(inputs, dtype):
+        row_lengths = [len(x) for x in inputs]
+        inputs_concat = tf.concat(inputs, axis=0)
         return tf.RaggedTensor.from_row_lengths(
-            component_data_concat, tf.cast(row_lengths, dtype))
+            inputs_concat, tf.cast(row_lengths, dtype))
 
     structure = values[0]._data
 
     ragged = tf.nest.map_structure(
         lambda x: isinstance(x['node_feature'], tf.RaggedTensor), values)
 
     if 0 < sum(ragged) < len(ragged):
@@ -973,15 +1038,15 @@
     else:
         # If first element is ragged, the rest is also ragged, and vice versa
         ragged = ragged[0]
 
     flat_sequence = tf.nest.map_structure(
         lambda x: tf.nest.flatten(x, expand_composites=True), values)
     
-    dtype = values[0]['edge_dst'].dtype
+    dtype = values[0]['edge_src'].dtype
 
     if ragged:
         # Keep only values (resulting from tf.nest.flatten)
         row_splits = [f[1::2] for f in flat_sequence]
         flat_sequence = [f[0::2] for f in flat_sequence]
         flat_sequence = tf.nest.map_structure(
             lambda v, r: tf.RaggedTensor.from_row_splits(v, r),
@@ -1003,14 +1068,61 @@
     values = GraphTensor(values)
 
     if ragged:
         return values
 
     return values.merge()
 
+@tf.experimental.dispatch_for_api(tf.stack)
+def graph_tensor_stack(
+    values: List[GraphTensor],
+    axis: int = 0,
+    name: str = 'stack'
+) -> GraphTensor:
+    '''Stacks list of graph tensors into a ragged GraphTensor.
+
+    Note: tf.stack(list_of_graph_tensors) only works (and make sense) 
+    if the graph data is non-ragged (namely, tf.Tensor types).
+    '''
+
+    if axis is not None and axis != 0:
+        raise ValueError(
+            f'axis=0 is required for `{values[0].__class__.__name__}`s.')
+
+    def fast_ragged_stack(inputs, dtype):
+        row_lengths = [len(x) for x in inputs]
+        inputs_concat = tf.concat(inputs, axis=0)
+        return tf.RaggedTensor.from_row_lengths(
+            inputs_concat, tf.cast(row_lengths, dtype))
+
+    structure = values[0]._data
+
+    ragged = tf.nest.map_structure(
+        lambda x: isinstance(x['node_feature'], tf.RaggedTensor), values)
+
+    if sum(ragged) > 0:
+        raise ValueError(
+            'Found ragged tensors. Can only stack non-ragged tensors.')
+
+    flat_sequence = tf.nest.map_structure(
+        lambda x: tf.nest.flatten(x, expand_composites=True), values)
+    
+    dtype = values[0]['edge_src'].dtype
+
+    flat_sequence = list(zip(*flat_sequence))
+
+    flat_sequence_stacked = [
+        fast_ragged_stack(x, dtype) for x in flat_sequence
+    ]
+
+    values = tf.nest.pack_sequence_as(
+        structure, flat_sequence_stacked)
+
+    return GraphTensor(values)
+
 
 @tf.experimental.dispatch_for_api(tf.matmul)
 def graph_tensor_matmul(
     a: GraphTensor,
     b,
     transpose_a=False,
     transpose_b=False,
@@ -1043,71 +1155,66 @@
 
     # indices of nodes to keep
     keep_nodes = tf.boolean_mask(tf.range(num_nodes), node_mask)
     
     # Get edge mask: 
     # edges where edge_dst AND edge_src exist in `keep_nodes` will be kept
     edge_mask = tf.logical_and(
-        tf.reduce_any(tf.expand_dims(tensor.edge_dst, -1) == keep_nodes, -1),
-        tf.reduce_any(tf.expand_dims(tensor.edge_src, -1) == keep_nodes, -1))
+        tf.reduce_any(tf.expand_dims(tensor.edge_src, -1) == keep_nodes, -1),
+        tf.reduce_any(tf.expand_dims(tensor.edge_dst, -1) == keep_nodes, -1)
+    )
     
     # Decrement (node) indices in edge_dst and edge_src:
     # as nodes are completely dropped, indices needs to be 
     # decremented accordingly.
     decr = tf.concat([[-1], keep_nodes], axis=0)
     decr = tf.math.cumsum(decr[1:] - decr[:-1] - 1)
     decr = tf.tensor_scatter_nd_add(
         tensor=tf.zeros((num_nodes,), dtype=decr.dtype),
         indices=tf.expand_dims(keep_nodes, -1),
         updates=decr)
     
     # Apply mask and decrement to edges
-    edge_dst = tf.boolean_mask(tensor.edge_dst, edge_mask)
-    edge_dst -= tf.gather(decr, edge_dst)
     edge_src = tf.boolean_mask(tensor.edge_src, edge_mask)
     edge_src -= tf.gather(decr, edge_src)
+    edge_dst = tf.boolean_mask(tensor.edge_dst, edge_mask)
+    edge_dst -= tf.gather(decr, edge_dst)
     
-    # Obtain components of the GraphTensor
+    # Obtain data of the GraphTensor
     data = tensor._data.copy()
     
     # Add new (masked) edge_dst and edge_src
-    data['edge_dst'] = edge_dst
     data['edge_src'] = edge_src
+    data['edge_dst'] = edge_dst
     
-    # Apply masks on the rest of the components and add to data
-    # Both components associated with edges and nodes will be masked
-    data['graph_indicator'] = tf.boolean_mask(
-        data['graph_indicator'], node_mask)
-    if 'positional_encoding' in data:
-        data['positional_encoding'] = tf.boolean_mask(
-            data['positional_encoding'], node_mask)
-    already_masked = [
-        'edge_dst', 'edge_src', 'graph_indicator', 'positional_encoding',
-    ]
+    # Apply masks on the rest of the data and add to data dict
+    # Both data associated with edges and nodes will be masked
     for key in data.keys():
-        if key not in already_masked:
+        if key not in ['edge_src', 'edge_dst']: # if not yet masked
             if key.startswith('edge'):
                  data[key] = tf.boolean_mask(data[key], edge_mask)
-            elif key.startswith('node'):
+            else:
                  data[key] = tf.boolean_mask(data[key], node_mask)  
                 
     return GraphTensor(**data)
 
 def _mask_edges(
     tensor: GraphTensor, 
     edge_mask: tf.Tensor
 ) -> GraphTensor:
-    # Obtain components of the GraphTensor
+    # Obtain data of the GraphTensor
     data = tensor._data.copy()
-    # Mask all components associated with edges
+    # Mask all data associated with edges
     for key in data.keys():
         if key.startswith('edge'):
              data[key] = tf.boolean_mask(data[key], edge_mask)   
     return GraphTensor(**data)
 
+# TODO: Allow tf.boolean_mask(graph_tensor, mask) to mask graphs,
+#       by specifying axis='graph'?
 @tf.experimental.dispatch_for_api(tf.boolean_mask)
 def graph_tensor_boolean_mask(
     tensor: GraphTensor, mask, axis=None,
 ) -> GraphTensor:
     '''Allows GraphTensor to be masked, via tf.boolean_mask.
     
     Conventiently, nodes or edges can be masked from the graph.
@@ -1143,25 +1250,24 @@
         tensor = _mask_nodes(tensor, mask)
     else:
         tensor = _mask_edges(tensor, mask)
     if ragged:
         return tensor.separate()
     return tensor
 
-
 @tf.experimental.dispatch_for_unary_elementwise_apis(GraphTensor)
 def graph_tensor_unary_elementwise_op_handler(api_func, x):
     '''Allows all unary elementwise operations (such as `tf.math.abs`)
     to handle graph tensors.
     '''
     return x.update({'node_feature': api_func(x.node_feature)})
 
 @tf.experimental.dispatch_for_binary_elementwise_apis(
-    Union[GraphTensor, tf.Tensor],
-    Union[GraphTensor, tf.Tensor])
+    Union[GraphTensor, tf.Tensor], Union[GraphTensor, tf.Tensor]
+)
 def graph_tensor_binary_elementwise_op_handler(api_func, x, y):
     '''Allows all binary elementwise operations (such as `tf.math.add`)
     to handle graph tensors.
     '''
     if isinstance(x, GraphTensor):
         x_values = x.node_feature
     else:
@@ -1176,26 +1282,8 @@
         return x.update({'node_feature': api_func(x_values, y_values)})
     elif isinstance(y, GraphTensor):
         return y.update({'node_feature': api_func(x_values, y_values)})
 
     return api_func(x_values, y_values)
 
 
-class _Iterator:
-    'Iterator for the graph tensors'
-
-    __slots__ = ['_iterable', '_index', '_limit']
 
-    def __init__(self, iterable: GraphTensor, limit: int) -> None:
-        self._iterable = iterable
-        self._limit = limit
-        self._index = 0
-
-    def __iter__(self):
-        return self
-
-    def __next__(self):
-        if self._index == self._limit:
-            raise StopIteration
-        result = self._iterable[self._index]
-        self._index += 1
-        return result
```

### Comparing `molgraph-0.3.8/molgraph.egg-info/PKG-INFO` & `molgraph-0.3.9/molgraph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgraph
-Version: 0.3.8
+Version: 0.3.9
 Summary: Implementations of graph neural networks for molecular machine learning
 Home-page: https://github.com/akensert/molgraph
 Author: Alexander Kensert
 Author-email: alexander.kensert@gmail.com
 License: MIT
 Keywords: graph-neural-networks,deep-learning,machine-learning,molecular-machine-learning,molecular-graphs,cheminformatics,bioinformatics
 Classifier: Programming Language :: Python :: 3
```

### Comparing `molgraph-0.3.8/molgraph.egg-info/SOURCES.txt` & `molgraph-0.3.9/molgraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.8/setup.py` & `molgraph-0.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.8/tests/test_chemistry.py` & `molgraph-0.3.9/tests/test_chemistry.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,16 +61,16 @@
          [0., 0., 1., 0., 0.],
          [0., 0., 1., 0., 1.],
          [0., 1., 0., 0., 0.],
          [0., 0., 1., 0., 0.],
          [0., 1., 0., 0., 0.],
          [0., 0., 1., 0., 0.],
          [0., 0., 1., 0., 0.]], dtype=tf.float32)
-    edge_dst = tf.constant([0, 0, 1, 1, 1, 2, 3, 4], dtype=tf.int32)
-    edge_src = tf.constant([1, 4, 0, 2, 3, 1, 1, 0], dtype=tf.int32)
+    edge_src = tf.constant([0, 0, 1, 1, 1, 2, 3, 4], dtype=tf.int32)
+    edge_dst = tf.constant([1, 4, 0, 2, 3, 1, 1, 0], dtype=tf.int32)
 
     # Define atomic encoders
     atom_encoder = Featurizer([
         features.Symbol({'C', 'N', 'O'}),
         features.Hybridization({'SP', 'SP2', 'SP3'}),
         features.HydrogenDonor(),
         features.HydrogenAcceptor(),
@@ -88,14 +88,15 @@
         'OCC1OC(C(C1O)O)n1cnc2c1ncnc2N',
         'C(C(=O)O)N',
         'C1=CC(=CC=C1CC(C(=O)O)N)O'
     ])
 
     assert tf.reduce_all(graph_tensor[1].node_feature == node_feature)
     assert tf.reduce_all(graph_tensor[1].edge_feature == edge_feature)
-    assert tf.reduce_all(graph_tensor[1].edge_dst == edge_dst)
     assert tf.reduce_all(graph_tensor[1].edge_src == edge_src)
+    assert tf.reduce_all(graph_tensor[1].edge_dst == edge_dst)
 
     assert tf.reduce_all(graph_tensor.merge()[1].node_feature == node_feature)
     assert tf.reduce_all(graph_tensor.merge()[1].edge_feature == edge_feature)
-    assert tf.reduce_all(graph_tensor.merge()[1].edge_dst == edge_dst)
     assert tf.reduce_all(graph_tensor.merge()[1].edge_src == edge_src)
+    assert tf.reduce_all(graph_tensor.merge()[1].edge_dst == edge_dst)
+
```

### Comparing `molgraph-0.3.8/tests/test_interpretability.py` & `molgraph-0.3.9/tests/test_interpretability.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.8/tests/test_layers.py` & `molgraph-0.3.9/tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.8/tests/test_models.py` & `molgraph-0.3.9/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.8/tests/test_models_2.py` & `molgraph-0.3.9/tests/test_models_2.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.8/tests/test_tensors.py` & `molgraph-0.3.9/tests/test_tensors.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,15 @@
 
     graph_tensor_merged = graph_tensor.merge()
     random_feature = tf.random.uniform(graph_tensor_merged.node_feature.shape)
     graph_tensor_merged = graph_tensor_merged.update({
         'node_random_feature': random_feature})
 
     with pytest.raises(tf.errors.InvalidArgumentError):
-        random_feature = tf.ragged.constant([[1., 2.], [4., 5., 6., 7.]])
+        random_feature = tf.ragged.constant([[[1.], [2.]], [[4.], [5.], [6.], [7.]]], ragged_rank=1)
         graph_tensor_merged = graph_tensor_merged.update({
             'node_random_feature': random_feature
         })
 
 @pytest.mark.parametrize('graph_tensor', [graph_tensor])
 def test_compatible_tf_function(graph_tensor) -> None:
```

### Comparing `molgraph-0.3.8/tests/test_tensors_2.py` & `molgraph-0.3.9/tests/test_tensors_2.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.8/tests/test_tensors_3.py` & `molgraph-0.3.9/tests/test_tensors_3.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.8/tests/test_tensors_4.py` & `molgraph-0.3.9/tests/test_tensors_4.py`

 * *Files identical despite different names*

