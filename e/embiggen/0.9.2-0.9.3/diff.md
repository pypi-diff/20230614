# Comparing `tmp/embiggen-0.9.2.tar.gz` & `tmp/embiggen-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/embiggen-0.9.2.tar", last modified: Mon Sep 13 11:16:04 2021, max compression
+gzip compressed data, was "dist/embiggen-0.9.3.tar", last modified: Mon Sep 13 11:36:50 2021, max compression
```

## Comparing `embiggen-0.9.2.tar` & `embiggen-0.9.3.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-09-13 11:16:04.000000 embiggen-0.9.2/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     4351 2021-09-13 11:16:04.000000 embiggen-0.9.2/PKG-INFO
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-09-13 11:16:04.000000 embiggen-0.9.2/embiggen/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      943 2021-09-10 13:48:05.000000 embiggen-0.9.2/embiggen/__init__.py
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-09-13 11:16:04.000000 embiggen-0.9.2/embiggen/pipelines/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      197 2021-09-06 15:12:50.000000 embiggen-0.9.2/embiggen/pipelines/__init__.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)    12919 2021-09-07 20:00:12.000000 embiggen-0.9.2/embiggen/pipelines/compute_node_embedding.py
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-09-13 11:16:04.000000 embiggen-0.9.2/embiggen/utils/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     1314 2021-09-06 15:12:50.000000 embiggen-0.9.2/embiggen/utils/gpu_utilities.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     1733 2021-09-10 13:48:05.000000 embiggen-0.9.2/embiggen/utils/graph_to_sparse_tensor.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     2123 2021-09-06 15:12:50.000000 embiggen-0.9.2/embiggen/utils/parameter_validators.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      718 2021-09-06 15:12:50.000000 embiggen-0.9.2/embiggen/utils/__init__.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     3171 2021-09-06 15:12:50.000000 embiggen-0.9.2/embiggen/utils/tensorflow_utils.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)       64 2021-09-07 20:00:12.000000 embiggen-0.9.2/embiggen/__version__.py
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-09-13 11:16:04.000000 embiggen-0.9.2/embiggen/node_prediction/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)    20216 2021-09-07 20:00:12.000000 embiggen-0.9.2/embiggen/node_prediction/graph_convolutional_neural_networks.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      168 2021-09-10 13:48:05.000000 embiggen-0.9.2/embiggen/node_prediction/__init__.py
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-09-13 11:16:04.000000 embiggen-0.9.2/embiggen/visualizations/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      161 2021-08-14 08:03:02.000000 embiggen-0.9.2/embiggen/visualizations/__init__.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)    58764 2021-09-13 11:15:48.000000 embiggen-0.9.2/embiggen/visualizations/graph_visualization.py
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-09-13 11:16:04.000000 embiggen-0.9.2/embiggen/embedders/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     7925 2021-09-10 13:48:05.000000 embiggen-0.9.2/embiggen/embedders/graph_skipgram.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)    21827 2021-09-13 11:15:48.000000 embiggen-0.9.2/embiggen/embedders/siamese.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     8669 2021-09-07 20:00:12.000000 embiggen-0.9.2/embiggen/embedders/transh.py
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-09-13 11:16:04.000000 embiggen-0.9.2/embiggen/embedders/layers/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     7781 2021-09-06 15:12:50.000000 embiggen-0.9.2/embiggen/embedders/layers/graph_attention.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     3005 2021-09-06 15:12:50.000000 embiggen-0.9.2/embiggen/embedders/layers/noise_contrastive_estimation.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      385 2021-09-10 13:48:05.000000 embiggen-0.9.2/embiggen/embedders/layers/__init__.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     5867 2021-09-06 15:12:50.000000 embiggen-0.9.2/embiggen/embedders/layers/graph_convolution_layer.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     3067 2021-09-06 15:12:50.000000 embiggen-0.9.2/embiggen/embedders/layers/sampled_softmax.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     7910 2021-09-10 13:48:05.000000 embiggen-0.9.2/embiggen/embedders/graph_cbow.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      608 2021-09-06 15:12:50.000000 embiggen-0.9.2/embiggen/embedders/__init__.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)    10130 2021-09-06 15:12:50.000000 embiggen-0.9.2/embiggen/embedders/glove.py
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-09-13 11:16:04.000000 embiggen-0.9.2/embiggen/embedders/optimizers/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      158 2021-09-06 15:12:50.000000 embiggen-0.9.2/embiggen/embedders/optimizers/__init__.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     3739 2021-09-06 15:12:50.000000 embiggen-0.9.2/embiggen/embedders/optimizers/centralize_gradient.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     3959 2021-09-06 15:12:50.000000 embiggen-0.9.2/embiggen/embedders/skipgram.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     4737 2021-09-07 20:00:12.000000 embiggen-0.9.2/embiggen/embedders/transe.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)    11184 2021-09-13 11:14:35.000000 embiggen-0.9.2/embiggen/embedders/graph_glove.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)    13383 2021-09-06 15:12:50.000000 embiggen-0.9.2/embiggen/embedders/embedder.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)    12160 2021-09-07 20:00:12.000000 embiggen-0.9.2/embiggen/embedders/node2vec.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     8571 2021-09-07 20:00:12.000000 embiggen-0.9.2/embiggen/embedders/transr.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     4824 2021-09-07 20:00:12.000000 embiggen-0.9.2/embiggen/embedders/simple.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     3977 2021-09-06 15:12:50.000000 embiggen-0.9.2/embiggen/embedders/cbow.py
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-09-13 11:16:04.000000 embiggen-0.9.2/embiggen/transformers/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     4405 2021-09-07 20:00:12.000000 embiggen-0.9.2/embiggen/transformers/link_prediction_transformer.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)    13971 2021-08-14 08:03:02.000000 embiggen-0.9.2/embiggen/transformers/corpus_transformer.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      471 2021-08-14 08:03:02.000000 embiggen-0.9.2/embiggen/transformers/__init__.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     4050 2021-09-06 15:12:50.000000 embiggen-0.9.2/embiggen/transformers/node_transformer.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     4883 2021-09-06 15:12:50.000000 embiggen-0.9.2/embiggen/transformers/edge_transformer.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     4016 2021-09-07 20:00:12.000000 embiggen-0.9.2/embiggen/transformers/graph_transformer.py
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-09-13 11:16:04.000000 embiggen-0.9.2/embiggen/sequences/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     5746 2021-09-07 20:00:12.000000 embiggen-0.9.2/embiggen/sequences/edge_prediction_sequence.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     1935 2021-09-06 15:12:50.000000 embiggen-0.9.2/embiggen/sequences/abstract_sequence.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     7475 2021-09-07 20:00:12.000000 embiggen-0.9.2/embiggen/sequences/node2vec_sequence.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      454 2021-09-10 13:48:05.000000 embiggen-0.9.2/embiggen/sequences/__init__.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     2911 2021-09-06 15:12:50.000000 embiggen-0.9.2/embiggen/sequences/glove_sequence.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     2404 2021-09-06 15:12:50.000000 embiggen-0.9.2/embiggen/sequences/abstract_word2vec_sequence.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     1853 2021-09-07 20:00:12.000000 embiggen-0.9.2/embiggen/sequences/word2vec_sequence.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     2301 2021-09-07 20:00:12.000000 embiggen-0.9.2/embiggen/sequences/node_label_prediction_sequence.py
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-09-13 11:16:04.000000 embiggen-0.9.2/embiggen/edge_prediction/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     8938 2021-09-07 20:00:12.000000 embiggen-0.9.2/embiggen/edge_prediction/edge_prediction_model.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      547 2021-08-14 08:03:02.000000 embiggen-0.9.2/embiggen/edge_prediction/perceptron.py
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-09-13 11:16:04.000000 embiggen-0.9.2/embiggen/edge_prediction/layers/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      820 2021-08-14 08:03:02.000000 embiggen-0.9.2/embiggen/edge_prediction/layers/l1_edge_embedding.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      793 2021-08-14 08:03:02.000000 embiggen-0.9.2/embiggen/edge_prediction/layers/average_edge_embedding.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      770 2021-08-14 08:03:02.000000 embiggen-0.9.2/embiggen/edge_prediction/layers/__init__.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      780 2021-08-14 08:03:02.000000 embiggen-0.9.2/embiggen/edge_prediction/layers/concatenate_edge_embedding.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     3642 2021-09-06 15:12:50.000000 embiggen-0.9.2/embiggen/edge_prediction/layers/edge_embedding.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      866 2021-08-14 08:03:02.000000 embiggen-0.9.2/embiggen/edge_prediction/layers/l2_edge_embedding.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      832 2021-08-14 08:03:02.000000 embiggen-0.9.2/embiggen/edge_prediction/layers/hadamard_edge_embedding.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      815 2021-08-14 08:03:02.000000 embiggen-0.9.2/embiggen/edge_prediction/layers/sum_edge_embedding.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      915 2021-08-14 08:03:02.000000 embiggen-0.9.2/embiggen/edge_prediction/multi_layer_perceptron.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      202 2021-09-06 15:12:50.000000 embiggen-0.9.2/embiggen/edge_prediction/__init__.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     1626 2021-09-13 11:15:53.000000 embiggen-0.9.2/setup.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)       38 2021-09-13 11:16:04.000000 embiggen-0.9.2/setup.cfg
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     3192 2021-08-14 08:03:01.000000 embiggen-0.9.2/README.rst
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-09-13 11:16:04.000000 embiggen-0.9.2/embiggen.egg-info/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     4351 2021-09-13 11:16:04.000000 embiggen-0.9.2/embiggen.egg-info/PKG-INFO
--rw-r--r--   0 lucacappelletti   (501) staff       (20)        1 2021-09-06 15:13:14.000000 embiggen-0.9.2/embiggen.egg-info/not-zip-safe
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     2656 2021-09-13 11:16:04.000000 embiggen-0.9.2/embiggen.egg-info/SOURCES.txt
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      332 2021-09-13 11:16:04.000000 embiggen-0.9.2/embiggen.egg-info/requires.txt
--rw-r--r--   0 lucacappelletti   (501) staff       (20)        9 2021-09-13 11:16:04.000000 embiggen-0.9.2/embiggen.egg-info/top_level.txt
--rw-r--r--   0 lucacappelletti   (501) staff       (20)        1 2021-09-13 11:16:04.000000 embiggen-0.9.2/embiggen.egg-info/dependency_links.txt
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-09-13 11:36:50.000000 embiggen-0.9.3/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     4351 2021-09-13 11:36:50.000000 embiggen-0.9.3/PKG-INFO
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-09-13 11:36:49.000000 embiggen-0.9.3/embiggen/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      943 2021-09-10 13:48:05.000000 embiggen-0.9.3/embiggen/__init__.py
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-09-13 11:36:49.000000 embiggen-0.9.3/embiggen/pipelines/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      197 2021-09-06 15:12:50.000000 embiggen-0.9.3/embiggen/pipelines/__init__.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)    12919 2021-09-07 20:00:12.000000 embiggen-0.9.3/embiggen/pipelines/compute_node_embedding.py
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-09-13 11:36:50.000000 embiggen-0.9.3/embiggen/utils/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     1314 2021-09-06 15:12:50.000000 embiggen-0.9.3/embiggen/utils/gpu_utilities.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     1733 2021-09-10 13:48:05.000000 embiggen-0.9.3/embiggen/utils/graph_to_sparse_tensor.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     2123 2021-09-06 15:12:50.000000 embiggen-0.9.3/embiggen/utils/parameter_validators.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      718 2021-09-06 15:12:50.000000 embiggen-0.9.3/embiggen/utils/__init__.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     3171 2021-09-06 15:12:50.000000 embiggen-0.9.3/embiggen/utils/tensorflow_utils.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)       64 2021-09-07 20:00:12.000000 embiggen-0.9.3/embiggen/__version__.py
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-09-13 11:36:49.000000 embiggen-0.9.3/embiggen/node_prediction/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)    20216 2021-09-07 20:00:12.000000 embiggen-0.9.3/embiggen/node_prediction/graph_convolutional_neural_networks.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      168 2021-09-10 13:48:05.000000 embiggen-0.9.3/embiggen/node_prediction/__init__.py
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-09-13 11:36:50.000000 embiggen-0.9.3/embiggen/visualizations/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      161 2021-08-14 08:03:02.000000 embiggen-0.9.3/embiggen/visualizations/__init__.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)    58762 2021-09-13 11:36:27.000000 embiggen-0.9.3/embiggen/visualizations/graph_visualization.py
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-09-13 11:36:49.000000 embiggen-0.9.3/embiggen/embedders/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     7925 2021-09-10 13:48:05.000000 embiggen-0.9.3/embiggen/embedders/graph_skipgram.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)    21827 2021-09-13 11:15:48.000000 embiggen-0.9.3/embiggen/embedders/siamese.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     8669 2021-09-07 20:00:12.000000 embiggen-0.9.3/embiggen/embedders/transh.py
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-09-13 11:36:49.000000 embiggen-0.9.3/embiggen/embedders/layers/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     7781 2021-09-06 15:12:50.000000 embiggen-0.9.3/embiggen/embedders/layers/graph_attention.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     3005 2021-09-06 15:12:50.000000 embiggen-0.9.3/embiggen/embedders/layers/noise_contrastive_estimation.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      385 2021-09-10 13:48:05.000000 embiggen-0.9.3/embiggen/embedders/layers/__init__.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     5867 2021-09-06 15:12:50.000000 embiggen-0.9.3/embiggen/embedders/layers/graph_convolution_layer.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     3067 2021-09-06 15:12:50.000000 embiggen-0.9.3/embiggen/embedders/layers/sampled_softmax.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     7910 2021-09-10 13:48:05.000000 embiggen-0.9.3/embiggen/embedders/graph_cbow.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      608 2021-09-06 15:12:50.000000 embiggen-0.9.3/embiggen/embedders/__init__.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)    10130 2021-09-06 15:12:50.000000 embiggen-0.9.3/embiggen/embedders/glove.py
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-09-13 11:36:49.000000 embiggen-0.9.3/embiggen/embedders/optimizers/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      158 2021-09-06 15:12:50.000000 embiggen-0.9.3/embiggen/embedders/optimizers/__init__.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     3739 2021-09-06 15:12:50.000000 embiggen-0.9.3/embiggen/embedders/optimizers/centralize_gradient.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     3959 2021-09-06 15:12:50.000000 embiggen-0.9.3/embiggen/embedders/skipgram.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     4737 2021-09-07 20:00:12.000000 embiggen-0.9.3/embiggen/embedders/transe.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)    11184 2021-09-13 11:14:35.000000 embiggen-0.9.3/embiggen/embedders/graph_glove.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)    13383 2021-09-06 15:12:50.000000 embiggen-0.9.3/embiggen/embedders/embedder.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)    12160 2021-09-07 20:00:12.000000 embiggen-0.9.3/embiggen/embedders/node2vec.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     8571 2021-09-07 20:00:12.000000 embiggen-0.9.3/embiggen/embedders/transr.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     4824 2021-09-07 20:00:12.000000 embiggen-0.9.3/embiggen/embedders/simple.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     3977 2021-09-06 15:12:50.000000 embiggen-0.9.3/embiggen/embedders/cbow.py
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-09-13 11:36:49.000000 embiggen-0.9.3/embiggen/transformers/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     4405 2021-09-07 20:00:12.000000 embiggen-0.9.3/embiggen/transformers/link_prediction_transformer.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)    13971 2021-08-14 08:03:02.000000 embiggen-0.9.3/embiggen/transformers/corpus_transformer.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      471 2021-08-14 08:03:02.000000 embiggen-0.9.3/embiggen/transformers/__init__.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     4050 2021-09-06 15:12:50.000000 embiggen-0.9.3/embiggen/transformers/node_transformer.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     4883 2021-09-06 15:12:50.000000 embiggen-0.9.3/embiggen/transformers/edge_transformer.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     4016 2021-09-07 20:00:12.000000 embiggen-0.9.3/embiggen/transformers/graph_transformer.py
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-09-13 11:36:49.000000 embiggen-0.9.3/embiggen/sequences/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     5746 2021-09-07 20:00:12.000000 embiggen-0.9.3/embiggen/sequences/edge_prediction_sequence.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     1935 2021-09-06 15:12:50.000000 embiggen-0.9.3/embiggen/sequences/abstract_sequence.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     7475 2021-09-07 20:00:12.000000 embiggen-0.9.3/embiggen/sequences/node2vec_sequence.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      454 2021-09-10 13:48:05.000000 embiggen-0.9.3/embiggen/sequences/__init__.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     2911 2021-09-06 15:12:50.000000 embiggen-0.9.3/embiggen/sequences/glove_sequence.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     2404 2021-09-06 15:12:50.000000 embiggen-0.9.3/embiggen/sequences/abstract_word2vec_sequence.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     1853 2021-09-07 20:00:12.000000 embiggen-0.9.3/embiggen/sequences/word2vec_sequence.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     2301 2021-09-07 20:00:12.000000 embiggen-0.9.3/embiggen/sequences/node_label_prediction_sequence.py
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-09-13 11:36:49.000000 embiggen-0.9.3/embiggen/edge_prediction/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     8938 2021-09-07 20:00:12.000000 embiggen-0.9.3/embiggen/edge_prediction/edge_prediction_model.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      547 2021-08-14 08:03:02.000000 embiggen-0.9.3/embiggen/edge_prediction/perceptron.py
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-09-13 11:36:49.000000 embiggen-0.9.3/embiggen/edge_prediction/layers/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      820 2021-08-14 08:03:02.000000 embiggen-0.9.3/embiggen/edge_prediction/layers/l1_edge_embedding.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      793 2021-08-14 08:03:02.000000 embiggen-0.9.3/embiggen/edge_prediction/layers/average_edge_embedding.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      770 2021-08-14 08:03:02.000000 embiggen-0.9.3/embiggen/edge_prediction/layers/__init__.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      780 2021-08-14 08:03:02.000000 embiggen-0.9.3/embiggen/edge_prediction/layers/concatenate_edge_embedding.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     3642 2021-09-06 15:12:50.000000 embiggen-0.9.3/embiggen/edge_prediction/layers/edge_embedding.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      866 2021-08-14 08:03:02.000000 embiggen-0.9.3/embiggen/edge_prediction/layers/l2_edge_embedding.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      832 2021-08-14 08:03:02.000000 embiggen-0.9.3/embiggen/edge_prediction/layers/hadamard_edge_embedding.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      815 2021-08-14 08:03:02.000000 embiggen-0.9.3/embiggen/edge_prediction/layers/sum_edge_embedding.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      915 2021-08-14 08:03:02.000000 embiggen-0.9.3/embiggen/edge_prediction/multi_layer_perceptron.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      202 2021-09-06 15:12:50.000000 embiggen-0.9.3/embiggen/edge_prediction/__init__.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     1626 2021-09-13 11:36:44.000000 embiggen-0.9.3/setup.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)       38 2021-09-13 11:36:50.000000 embiggen-0.9.3/setup.cfg
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     3192 2021-08-14 08:03:01.000000 embiggen-0.9.3/README.rst
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-09-13 11:36:49.000000 embiggen-0.9.3/embiggen.egg-info/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     4351 2021-09-13 11:36:49.000000 embiggen-0.9.3/embiggen.egg-info/PKG-INFO
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)        1 2021-09-06 15:13:14.000000 embiggen-0.9.3/embiggen.egg-info/not-zip-safe
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     2656 2021-09-13 11:36:49.000000 embiggen-0.9.3/embiggen.egg-info/SOURCES.txt
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      332 2021-09-13 11:36:49.000000 embiggen-0.9.3/embiggen.egg-info/requires.txt
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)        9 2021-09-13 11:36:49.000000 embiggen-0.9.3/embiggen.egg-info/top_level.txt
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)        1 2021-09-13 11:36:49.000000 embiggen-0.9.3/embiggen.egg-info/dependency_links.txt
```

### Comparing `embiggen-0.9.2/PKG-INFO` & `embiggen-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embiggen
-Version: 0.9.2
+Version: 0.9.3
 Summary: Extended implementation of node2vec with several word2vec family algorithms
 Home-page: https://github.com/monarch-initiative/embiggen
 Author: Tommaso Fontana, Peter Robinson, Luca Cappelletti, Vida Ravanmehr
 Author-email: tommaso.fontana@mail.polimi.it, peter.robinson@jax.org, luca.cappelletti1@unimi.it, vida.ravanmehr@jax.org
 License: BSD3
 Description: Embiggen: Embedding Generator
         =========================================================================================
```

### Comparing `embiggen-0.9.2/embiggen/__init__.py` & `embiggen-0.9.3/embiggen/__init__.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/pipelines/compute_node_embedding.py` & `embiggen-0.9.3/embiggen/pipelines/compute_node_embedding.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/utils/gpu_utilities.py` & `embiggen-0.9.3/embiggen/utils/gpu_utilities.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/utils/graph_to_sparse_tensor.py` & `embiggen-0.9.3/embiggen/utils/graph_to_sparse_tensor.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/utils/parameter_validators.py` & `embiggen-0.9.3/embiggen/utils/parameter_validators.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/utils/__init__.py` & `embiggen-0.9.3/embiggen/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/utils/tensorflow_utils.py` & `embiggen-0.9.3/embiggen/utils/tensorflow_utils.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/node_prediction/graph_convolutional_neural_networks.py` & `embiggen-0.9.3/embiggen/node_prediction/graph_convolutional_neural_networks.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/visualizations/graph_visualization.py` & `embiggen-0.9.3/embiggen/visualizations/graph_visualization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1611,20 +1611,20 @@
         )
 
         color_bar = figure.colorbar(scatter[0], ax=axes)
         color_bar.set_alpha(1)
         color_bar.draw_all()
         return figure, axes
 
-    def plot_dot(self, engine: str = "circle"):
+    def plot_dot(self, engine: str = "circo"):
         """Return dot plot of the current graph.
         
         Parameters
         ------------------------------
-        engine: str = "circle",
+        engine: str = "circo",
             The engine to use to visualize the graph.
         
         Raises
         ------------------------------
         ModuleNotFoundError,
             If graphviz is not installed.
         """
```

### Comparing `embiggen-0.9.2/embiggen/embedders/graph_skipgram.py` & `embiggen-0.9.3/embiggen/embedders/graph_skipgram.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/embedders/siamese.py` & `embiggen-0.9.3/embiggen/embedders/siamese.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/embedders/transh.py` & `embiggen-0.9.3/embiggen/embedders/transh.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/embedders/layers/graph_attention.py` & `embiggen-0.9.3/embiggen/embedders/layers/graph_attention.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/embedders/layers/noise_contrastive_estimation.py` & `embiggen-0.9.3/embiggen/embedders/layers/noise_contrastive_estimation.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/embedders/layers/graph_convolution_layer.py` & `embiggen-0.9.3/embiggen/embedders/layers/graph_convolution_layer.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/embedders/layers/sampled_softmax.py` & `embiggen-0.9.3/embiggen/embedders/layers/sampled_softmax.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/embedders/graph_cbow.py` & `embiggen-0.9.3/embiggen/embedders/graph_cbow.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/embedders/__init__.py` & `embiggen-0.9.3/embiggen/embedders/__init__.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/embedders/glove.py` & `embiggen-0.9.3/embiggen/embedders/glove.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/embedders/optimizers/centralize_gradient.py` & `embiggen-0.9.3/embiggen/embedders/optimizers/centralize_gradient.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/embedders/skipgram.py` & `embiggen-0.9.3/embiggen/embedders/skipgram.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/embedders/transe.py` & `embiggen-0.9.3/embiggen/embedders/transe.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/embedders/graph_glove.py` & `embiggen-0.9.3/embiggen/embedders/graph_glove.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/embedders/embedder.py` & `embiggen-0.9.3/embiggen/embedders/embedder.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/embedders/node2vec.py` & `embiggen-0.9.3/embiggen/embedders/node2vec.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/embedders/transr.py` & `embiggen-0.9.3/embiggen/embedders/transr.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/embedders/simple.py` & `embiggen-0.9.3/embiggen/embedders/simple.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/embedders/cbow.py` & `embiggen-0.9.3/embiggen/embedders/cbow.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/transformers/link_prediction_transformer.py` & `embiggen-0.9.3/embiggen/transformers/link_prediction_transformer.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/transformers/corpus_transformer.py` & `embiggen-0.9.3/embiggen/transformers/corpus_transformer.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/transformers/node_transformer.py` & `embiggen-0.9.3/embiggen/transformers/node_transformer.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/transformers/edge_transformer.py` & `embiggen-0.9.3/embiggen/transformers/edge_transformer.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/transformers/graph_transformer.py` & `embiggen-0.9.3/embiggen/transformers/graph_transformer.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/sequences/edge_prediction_sequence.py` & `embiggen-0.9.3/embiggen/sequences/edge_prediction_sequence.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/sequences/abstract_sequence.py` & `embiggen-0.9.3/embiggen/sequences/abstract_sequence.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/sequences/node2vec_sequence.py` & `embiggen-0.9.3/embiggen/sequences/node2vec_sequence.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/sequences/glove_sequence.py` & `embiggen-0.9.3/embiggen/sequences/glove_sequence.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/sequences/abstract_word2vec_sequence.py` & `embiggen-0.9.3/embiggen/sequences/abstract_word2vec_sequence.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/sequences/word2vec_sequence.py` & `embiggen-0.9.3/embiggen/sequences/word2vec_sequence.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/sequences/node_label_prediction_sequence.py` & `embiggen-0.9.3/embiggen/sequences/node_label_prediction_sequence.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/edge_prediction/edge_prediction_model.py` & `embiggen-0.9.3/embiggen/edge_prediction/edge_prediction_model.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/edge_prediction/perceptron.py` & `embiggen-0.9.3/embiggen/edge_prediction/perceptron.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/edge_prediction/layers/l1_edge_embedding.py` & `embiggen-0.9.3/embiggen/edge_prediction/layers/l1_edge_embedding.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/edge_prediction/layers/average_edge_embedding.py` & `embiggen-0.9.3/embiggen/edge_prediction/layers/average_edge_embedding.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/edge_prediction/layers/__init__.py` & `embiggen-0.9.3/embiggen/edge_prediction/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/edge_prediction/layers/concatenate_edge_embedding.py` & `embiggen-0.9.3/embiggen/edge_prediction/layers/concatenate_edge_embedding.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/edge_prediction/layers/edge_embedding.py` & `embiggen-0.9.3/embiggen/edge_prediction/layers/edge_embedding.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/edge_prediction/layers/l2_edge_embedding.py` & `embiggen-0.9.3/embiggen/edge_prediction/layers/l2_edge_embedding.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/edge_prediction/layers/hadamard_edge_embedding.py` & `embiggen-0.9.3/embiggen/edge_prediction/layers/hadamard_edge_embedding.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/edge_prediction/layers/sum_edge_embedding.py` & `embiggen-0.9.3/embiggen/edge_prediction/layers/sum_edge_embedding.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen/edge_prediction/multi_layer_perceptron.py` & `embiggen-0.9.3/embiggen/edge_prediction/multi_layer_perceptron.py`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/setup.py` & `embiggen-0.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     "Peter Robinson":"peter.robinson@jax.org",
     "Luca Cappelletti":"luca.cappelletti1@unimi.it",
     "Tommaso Fontana":"tommaso.fontana@mail.polimi.it"
 }
 
 setup(
     name='embiggen',
-    version='0.9.2',
+    version='0.9.3',
     description='Extended implementation of node2vec with several word2vec family algorithms',
     long_description=readme(),
     url='https://github.com/monarch-initiative/embiggen',
     keywords='node2vec,word2vec,CBOW,SkipGram,GloVe',
     author=", ".join(list(authors.keys())),
     author_email=", ".join(list(authors.values())),
     license='BSD3',
```

### Comparing `embiggen-0.9.2/README.rst` & `embiggen-0.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `embiggen-0.9.2/embiggen.egg-info/PKG-INFO` & `embiggen-0.9.3/embiggen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embiggen
-Version: 0.9.2
+Version: 0.9.3
 Summary: Extended implementation of node2vec with several word2vec family algorithms
 Home-page: https://github.com/monarch-initiative/embiggen
 Author: Tommaso Fontana, Peter Robinson, Luca Cappelletti, Vida Ravanmehr
 Author-email: tommaso.fontana@mail.polimi.it, peter.robinson@jax.org, luca.cappelletti1@unimi.it, vida.ravanmehr@jax.org
 License: BSD3
 Description: Embiggen: Embedding Generator
         =========================================================================================
```

### Comparing `embiggen-0.9.2/embiggen.egg-info/SOURCES.txt` & `embiggen-0.9.3/embiggen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

