# Comparing `tmp/wavpool-0.1.0.tar.gz` & `tmp/wavpool-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wavpool-0.1.0.tar", max compression
+gzip compressed data, was "wavpool-0.1.1.tar", max compression
```

## Comparing `wavpool-0.1.0.tar` & `wavpool-0.1.1.tar`

### file list

```diff
@@ -1,50 +1,51 @@
--rw-r--r--   0        0        0     1068 2023-03-02 20:17:07.601903 wavpool-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0      596 2023-06-14 20:12:20.895285 wavpool-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-06-14 20:00:23.369261 wavpool-0.1.0/wavpool/.DS_Store
--rw-r--r--   0        0        0       37 2023-02-20 18:58:16.615880 wavpool-0.1.0/wavpool/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2023-02-20 18:58:16.615946 wavpool-0.1.0/wavpool/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2023-02-20 18:58:16.615778 wavpool-0.1.0/wavpool/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2023-02-20 19:11:14.275406 wavpool-0.1.0/wavpool/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2023-02-20 19:11:14.275582 wavpool-0.1.0/wavpool/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2023-03-02 20:20:15.450100 wavpool-0.1.0/wavpool/__init__.py
--rw-r--r--   0        0        0      216 2023-05-16 17:57:31.144622 wavpool-0.1.0/wavpool/data_generators/__init__.py
--rw-r--r--   0        0        0      409 2023-05-16 18:52:26.862156 wavpool-0.1.0/wavpool/data_generators/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      906 2023-05-16 18:52:26.863176 wavpool-0.1.0/wavpool/data_generators/__pycache__/cifar_generator.cpython-310.pyc
--rw-r--r--   0        0        0     1699 2023-03-10 15:41:25.041784 wavpool-0.1.0/wavpool/data_generators/__pycache__/data_generator.cpython-310.pyc
--rw-r--r--   0        0        0      837 2023-05-16 18:52:27.027442 wavpool-0.1.0/wavpool/data_generators/__pycache__/fashion_mnist_generator.cpython-310.pyc
--rw-r--r--   0        0        0      795 2023-05-16 18:52:27.026890 wavpool-0.1.0/wavpool/data_generators/__pycache__/mnist_generator.cpython-310.pyc
--rw-r--r--   0        0        0      560 2023-05-16 17:57:31.144612 wavpool-0.1.0/wavpool/data_generators/cifar_generator.py
--rw-r--r--   0        0        0     2296 2023-03-10 15:17:25.706092 wavpool-0.1.0/wavpool/data_generators/data_generator.py
--rw-r--r--   0        0        0      438 2023-05-16 17:57:31.144634 wavpool-0.1.0/wavpool/data_generators/fashion_mnist_generator.py
--rw-r--r--   0        0        0      373 2023-05-16 17:57:31.144661 wavpool-0.1.0/wavpool/data_generators/mnist_generator.py
--rw-r--r--   0        0        0      182 2023-05-16 17:57:31.144651 wavpool-0.1.0/wavpool/models/__init__.py
--rw-r--r--   0        0        0      377 2023-05-16 18:52:26.842425 wavpool-0.1.0/wavpool/models/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2497 2023-03-24 14:17:48.365408 wavpool-0.1.0/wavpool/models/__pycache__/pooling_wav.cpython-310.pyc
--rw-r--r--   0        0        0     1435 2023-05-16 12:49:06.927343 wavpool-0.1.0/wavpool/models/__pycache__/vanillaCNN.cpython-310.pyc
--rw-r--r--   0        0        0     1990 2023-05-12 17:25:03.646772 wavpool-0.1.0/wavpool/models/__pycache__/vanillaMLP.cpython-310.pyc
--rw-r--r--   0        0        0     2413 2023-03-15 19:26:39.562765 wavpool-0.1.0/wavpool/models/__pycache__/voting_wavMLP.cpython-310.pyc
--rw-r--r--   0        0        0     2195 2023-03-16 13:39:06.604160 wavpool-0.1.0/wavpool/models/__pycache__/wavCNN.cpython-310.pyc
--rw-r--r--   0        0        0     1653 2023-05-16 18:52:26.843264 wavpool-0.1.0/wavpool/models/__pycache__/wavMLP.cpython-310.pyc
--rw-r--r--   0        0        0     2544 2023-05-16 18:52:26.857368 wavpool-0.1.0/wavpool/models/__pycache__/wavelet_layer.cpython-310.pyc
--rw-r--r--   0        0        0     3010 2023-05-16 18:52:26.861371 wavpool-0.1.0/wavpool/models/__pycache__/wavpool.cpython-310.pyc
--rw-r--r--   0        0        0     1478 2023-05-16 12:42:46.313669 wavpool-0.1.0/wavpool/models/vanillaCNN.py
--rw-r--r--   0        0        0     1768 2023-04-20 12:52:16.897105 wavpool-0.1.0/wavpool/models/vanillaMLP.py
--rw-r--r--   0        0        0     1630 2023-05-16 17:57:02.092990 wavpool-0.1.0/wavpool/models/wavMLP.py
--rw-r--r--   0        0        0     2122 2023-05-16 17:56:47.961851 wavpool-0.1.0/wavpool/models/wavelet_layer.py
--rw-r--r--   0        0        0     2867 2023-05-16 17:57:11.816319 wavpool-0.1.0/wavpool/models/wavpool.py
--rw-r--r--   0        0        0     5130 2023-05-12 17:25:05.871802 wavpool-0.1.0/wavpool/training/__pycache__/finetune_network.cpython-310.pyc
--rw-r--r--   0        0        0     4669 2023-05-17 17:19:32.067201 wavpool-0.1.0/wavpool/training/__pycache__/plot_results.cpython-310.pyc
--rw-r--r--   0        0        0     4308 2023-05-16 18:52:25.742806 wavpool-0.1.0/wavpool/training/__pycache__/train_model.cpython-310.pyc
--rw-r--r--   0        0        0     2115 2023-03-30 19:26:31.435099 wavpool-0.1.0/wavpool/training/__pycache__/training_metrics.cpython-310.pyc
--rw-r--r--   0        0        0     6850 2023-05-16 17:57:13.547418 wavpool-0.1.0/wavpool/training/finetune_network.py
--rw-r--r--   0        0        0     6092 2023-05-16 17:57:14.882187 wavpool-0.1.0/wavpool/training/plot_results.py
--rw-r--r--   0        0        0     5044 2023-05-16 17:57:31.144703 wavpool-0.1.0/wavpool/training/train_model.py
--rw-r--r--   0        0        0     1602 2023-03-30 19:15:46.046853 wavpool-0.1.0/wavpool/training/training_metrics.py
--rw-r--r--   0        0        0        0 2023-03-02 20:20:58.389105 wavpool-0.1.0/wavpool/utils/__init__.py
--rw-r--r--   0        0        0      148 2023-03-27 15:04:06.987733 wavpool-0.1.0/wavpool/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1751 2023-05-12 17:25:03.006087 wavpool-0.1.0/wavpool/utils/__pycache__/levels.cpython-310.pyc
--rw-r--r--   0        0        0      548 2023-03-27 15:04:06.987787 wavpool-0.1.0/wavpool/utils/__pycache__/voting.cpython-310.pyc
--rw-r--r--   0        0        0     1480 2023-05-04 14:32:31.422998 wavpool-0.1.0/wavpool/utils/levels.py
--rw-r--r--   0        0        0      367 2023-03-23 18:08:00.118508 wavpool-0.1.0/wavpool/utils/voting.py
--rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 wavpool-0.1.0/setup.py
--rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 wavpool-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-14 20:16:22.496915 wavpool-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     3803 2023-06-14 20:54:30.856171 wavpool-0.1.1/README.md
+-rw-r--r--   0        0        0      740 2023-06-14 20:21:20.493657 wavpool-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-06-14 20:00:23.369261 wavpool-0.1.1/wavpool/.DS_Store
+-rw-r--r--   0        0        0       37 2023-02-20 18:58:16.615880 wavpool-0.1.1/wavpool/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2023-02-20 18:58:16.615946 wavpool-0.1.1/wavpool/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2023-02-20 18:58:16.615778 wavpool-0.1.1/wavpool/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2023-02-20 19:11:14.275406 wavpool-0.1.1/wavpool/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2023-02-20 19:11:14.275582 wavpool-0.1.1/wavpool/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2023-03-02 20:20:15.450100 wavpool-0.1.1/wavpool/__init__.py
+-rw-r--r--   0        0        0      216 2023-05-16 17:57:31.144622 wavpool-0.1.1/wavpool/data_generators/__init__.py
+-rw-r--r--   0        0        0      409 2023-05-16 18:52:26.862156 wavpool-0.1.1/wavpool/data_generators/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      906 2023-05-16 18:52:26.863176 wavpool-0.1.1/wavpool/data_generators/__pycache__/cifar_generator.cpython-310.pyc
+-rw-r--r--   0        0        0     1699 2023-03-10 15:41:25.041784 wavpool-0.1.1/wavpool/data_generators/__pycache__/data_generator.cpython-310.pyc
+-rw-r--r--   0        0        0      837 2023-05-16 18:52:27.027442 wavpool-0.1.1/wavpool/data_generators/__pycache__/fashion_mnist_generator.cpython-310.pyc
+-rw-r--r--   0        0        0      795 2023-05-16 18:52:27.026890 wavpool-0.1.1/wavpool/data_generators/__pycache__/mnist_generator.cpython-310.pyc
+-rw-r--r--   0        0        0      560 2023-05-16 17:57:31.144612 wavpool-0.1.1/wavpool/data_generators/cifar_generator.py
+-rw-r--r--   0        0        0     2296 2023-03-10 15:17:25.706092 wavpool-0.1.1/wavpool/data_generators/data_generator.py
+-rw-r--r--   0        0        0      438 2023-05-16 17:57:31.144634 wavpool-0.1.1/wavpool/data_generators/fashion_mnist_generator.py
+-rw-r--r--   0        0        0      373 2023-05-16 17:57:31.144661 wavpool-0.1.1/wavpool/data_generators/mnist_generator.py
+-rw-r--r--   0        0        0      182 2023-05-16 17:57:31.144651 wavpool-0.1.1/wavpool/models/__init__.py
+-rw-r--r--   0        0        0      377 2023-05-16 18:52:26.842425 wavpool-0.1.1/wavpool/models/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2497 2023-03-24 14:17:48.365408 wavpool-0.1.1/wavpool/models/__pycache__/pooling_wav.cpython-310.pyc
+-rw-r--r--   0        0        0     1435 2023-05-16 12:49:06.927343 wavpool-0.1.1/wavpool/models/__pycache__/vanillaCNN.cpython-310.pyc
+-rw-r--r--   0        0        0     1990 2023-05-12 17:25:03.646772 wavpool-0.1.1/wavpool/models/__pycache__/vanillaMLP.cpython-310.pyc
+-rw-r--r--   0        0        0     2413 2023-03-15 19:26:39.562765 wavpool-0.1.1/wavpool/models/__pycache__/voting_wavMLP.cpython-310.pyc
+-rw-r--r--   0        0        0     2195 2023-03-16 13:39:06.604160 wavpool-0.1.1/wavpool/models/__pycache__/wavCNN.cpython-310.pyc
+-rw-r--r--   0        0        0     1653 2023-05-16 18:52:26.843264 wavpool-0.1.1/wavpool/models/__pycache__/wavMLP.cpython-310.pyc
+-rw-r--r--   0        0        0     2544 2023-05-16 18:52:26.857368 wavpool-0.1.1/wavpool/models/__pycache__/wavelet_layer.cpython-310.pyc
+-rw-r--r--   0        0        0     3010 2023-05-16 18:52:26.861371 wavpool-0.1.1/wavpool/models/__pycache__/wavpool.cpython-310.pyc
+-rw-r--r--   0        0        0     1478 2023-05-16 12:42:46.313669 wavpool-0.1.1/wavpool/models/vanillaCNN.py
+-rw-r--r--   0        0        0     1768 2023-04-20 12:52:16.897105 wavpool-0.1.1/wavpool/models/vanillaMLP.py
+-rw-r--r--   0        0        0     1630 2023-05-16 17:57:02.092990 wavpool-0.1.1/wavpool/models/wavMLP.py
+-rw-r--r--   0        0        0     2122 2023-05-16 17:56:47.961851 wavpool-0.1.1/wavpool/models/wavelet_layer.py
+-rw-r--r--   0        0        0     2867 2023-05-16 17:57:11.816319 wavpool-0.1.1/wavpool/models/wavpool.py
+-rw-r--r--   0        0        0     5130 2023-05-12 17:25:05.871802 wavpool-0.1.1/wavpool/training/__pycache__/finetune_network.cpython-310.pyc
+-rw-r--r--   0        0        0     4669 2023-05-17 17:19:32.067201 wavpool-0.1.1/wavpool/training/__pycache__/plot_results.cpython-310.pyc
+-rw-r--r--   0        0        0     4308 2023-05-16 18:52:25.742806 wavpool-0.1.1/wavpool/training/__pycache__/train_model.cpython-310.pyc
+-rw-r--r--   0        0        0     2115 2023-03-30 19:26:31.435099 wavpool-0.1.1/wavpool/training/__pycache__/training_metrics.cpython-310.pyc
+-rw-r--r--   0        0        0     6850 2023-05-16 17:57:13.547418 wavpool-0.1.1/wavpool/training/finetune_network.py
+-rw-r--r--   0        0        0     6092 2023-05-16 17:57:14.882187 wavpool-0.1.1/wavpool/training/plot_results.py
+-rw-r--r--   0        0        0     5044 2023-05-16 17:57:31.144703 wavpool-0.1.1/wavpool/training/train_model.py
+-rw-r--r--   0        0        0     1602 2023-03-30 19:15:46.046853 wavpool-0.1.1/wavpool/training/training_metrics.py
+-rw-r--r--   0        0        0        0 2023-03-02 20:20:58.389105 wavpool-0.1.1/wavpool/utils/__init__.py
+-rw-r--r--   0        0        0      148 2023-03-27 15:04:06.987733 wavpool-0.1.1/wavpool/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1751 2023-05-12 17:25:03.006087 wavpool-0.1.1/wavpool/utils/__pycache__/levels.cpython-310.pyc
+-rw-r--r--   0        0        0      548 2023-03-27 15:04:06.987787 wavpool-0.1.1/wavpool/utils/__pycache__/voting.cpython-310.pyc
+-rw-r--r--   0        0        0     1480 2023-05-04 14:32:31.422998 wavpool-0.1.1/wavpool/utils/levels.py
+-rw-r--r--   0        0        0      367 2023-03-23 18:08:00.118508 wavpool-0.1.1/wavpool/utils/voting.py
+-rw-r--r--   0        0        0     4946 1970-01-01 00:00:00.000000 wavpool-0.1.1/setup.py
+-rw-r--r--   0        0        0     4758 1970-01-01 00:00:00.000000 wavpool-0.1.1/PKG-INFO
```

### Comparing `wavpool-0.1.0/LICENSE.txt` & `wavpool-0.1.1/LICENSE.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) [year] [fullname]
+Copyright (c) 2023 M. Voetberg
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `wavpool-0.1.0/wavpool/.DS_Store` & `wavpool-0.1.1/wavpool/.DS_Store`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.0/wavpool/data_generators/__pycache__/cifar_generator.cpython-310.pyc` & `wavpool-0.1.1/wavpool/data_generators/__pycache__/cifar_generator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.0/wavpool/data_generators/__pycache__/data_generator.cpython-310.pyc` & `wavpool-0.1.1/wavpool/data_generators/__pycache__/data_generator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.0/wavpool/data_generators/__pycache__/fashion_mnist_generator.cpython-310.pyc` & `wavpool-0.1.1/wavpool/data_generators/__pycache__/fashion_mnist_generator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.0/wavpool/data_generators/__pycache__/mnist_generator.cpython-310.pyc` & `wavpool-0.1.1/wavpool/data_generators/__pycache__/mnist_generator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.0/wavpool/data_generators/cifar_generator.py` & `wavpool-0.1.1/wavpool/data_generators/cifar_generator.py`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.0/wavpool/data_generators/data_generator.py` & `wavpool-0.1.1/wavpool/data_generators/data_generator.py`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.0/wavpool/models/__pycache__/pooling_wav.cpython-310.pyc` & `wavpool-0.1.1/wavpool/models/__pycache__/pooling_wav.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.0/wavpool/models/__pycache__/vanillaCNN.cpython-310.pyc` & `wavpool-0.1.1/wavpool/models/__pycache__/vanillaCNN.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.0/wavpool/models/__pycache__/vanillaMLP.cpython-310.pyc` & `wavpool-0.1.1/wavpool/models/__pycache__/vanillaMLP.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.0/wavpool/models/__pycache__/voting_wavMLP.cpython-310.pyc` & `wavpool-0.1.1/wavpool/models/__pycache__/voting_wavMLP.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.0/wavpool/models/__pycache__/wavCNN.cpython-310.pyc` & `wavpool-0.1.1/wavpool/models/__pycache__/wavCNN.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.0/wavpool/models/__pycache__/wavMLP.cpython-310.pyc` & `wavpool-0.1.1/wavpool/models/__pycache__/wavMLP.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.0/wavpool/models/__pycache__/wavelet_layer.cpython-310.pyc` & `wavpool-0.1.1/wavpool/models/__pycache__/wavelet_layer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.0/wavpool/models/__pycache__/wavpool.cpython-310.pyc` & `wavpool-0.1.1/wavpool/models/__pycache__/wavpool.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.0/wavpool/models/vanillaCNN.py` & `wavpool-0.1.1/wavpool/models/vanillaCNN.py`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.0/wavpool/models/vanillaMLP.py` & `wavpool-0.1.1/wavpool/models/vanillaMLP.py`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.0/wavpool/models/wavMLP.py` & `wavpool-0.1.1/wavpool/models/wavMLP.py`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.0/wavpool/models/wavelet_layer.py` & `wavpool-0.1.1/wavpool/models/wavelet_layer.py`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.0/wavpool/models/wavpool.py` & `wavpool-0.1.1/wavpool/models/wavpool.py`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.0/wavpool/training/__pycache__/finetune_network.cpython-310.pyc` & `wavpool-0.1.1/wavpool/training/__pycache__/finetune_network.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.0/wavpool/training/__pycache__/plot_results.cpython-310.pyc` & `wavpool-0.1.1/wavpool/training/__pycache__/plot_results.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.0/wavpool/training/__pycache__/train_model.cpython-310.pyc` & `wavpool-0.1.1/wavpool/training/__pycache__/train_model.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.0/wavpool/training/__pycache__/training_metrics.cpython-310.pyc` & `wavpool-0.1.1/wavpool/training/__pycache__/training_metrics.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.0/wavpool/training/finetune_network.py` & `wavpool-0.1.1/wavpool/training/finetune_network.py`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.0/wavpool/training/plot_results.py` & `wavpool-0.1.1/wavpool/training/plot_results.py`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.0/wavpool/training/train_model.py` & `wavpool-0.1.1/wavpool/training/train_model.py`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.0/wavpool/training/training_metrics.py` & `wavpool-0.1.1/wavpool/training/training_metrics.py`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.0/wavpool/utils/__pycache__/levels.cpython-310.pyc` & `wavpool-0.1.1/wavpool/utils/__pycache__/levels.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.0/wavpool/utils/__pycache__/voting.cpython-310.pyc` & `wavpool-0.1.1/wavpool/utils/__pycache__/voting.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.0/wavpool/utils/levels.py` & `wavpool-0.1.1/wavpool/utils/levels.py`

 * *Files identical despite different names*

