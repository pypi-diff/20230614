# Comparing `tmp/asociita-0.1.9.tar.gz` & `tmp/asociita-0.1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asociita-0.1.9.tar", max compression
+gzip compressed data, was "asociita-0.1.9.1.tar", max compression
```

## Comparing `asociita-0.1.9.tar` & `asociita-0.1.9.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1063 2023-05-29 08:30:33.477904 asociita-0.1.9/LICENSE
--rw-r--r--   0        0        0     2812 2023-05-29 08:30:33.477904 asociita-0.1.9/README.md
--rw-r--r--   0        0        0        0 2023-05-29 08:30:33.477904 asociita-0.1.9/asociita/__init__.py
--rw-r--r--   0        0        0     3881 2023-05-29 08:30:33.477904 asociita-0.1.9/asociita/components/archiver/archive_manager.py
--rw-r--r--   0        0        0     6970 2023-06-05 13:24:07.885952 asociita-0.1.9/asociita/components/evaluator/evaluation_manager.py
--rw-r--r--   0        0        0    13324 2023-05-29 08:30:33.477904 asociita-0.1.9/asociita/components/evaluator/mr_evaluator.py
--rw-r--r--   0        0        0     9972 2023-06-05 09:45:20.347198 asociita-0.1.9/asociita/components/evaluator/or_evaluator.py
--rw-r--r--   0        0        0     2106 2023-06-05 13:51:59.255884 asociita-0.1.9/asociita/components/evaluator/sample_evaluator.py
--rw-r--r--   0        0        0     4370 2023-06-06 11:35:25.808272 asociita-0.1.9/asociita/components/nodes/federated_node.py
--rw-r--r--   0        0        0     7549 2023-06-06 11:41:23.091887 asociita-0.1.9/asociita/components/orchestrator/evaluator_orchestrator.py
--rw-r--r--   0        0        0     6226 2023-06-06 11:42:03.726476 asociita-0.1.9/asociita/components/orchestrator/fedopt_orchestrator.py
--rw-r--r--   0        0        0    11069 2023-06-06 11:35:25.808272 asociita-0.1.9/asociita/components/orchestrator/generic_orchestrator.py
--rw-r--r--   0        0        0     3288 2023-06-07 13:08:30.716688 asociita-0.1.9/asociita/datasets/fetch_data.py
--rw-r--r--   0        0        0     3012 2023-06-07 14:34:09.128863 asociita-0.1.9/asociita/datasets/load_cifar.py
--rw-r--r--   0        0        0     2973 2023-06-07 14:34:21.476438 asociita-0.1.9/asociita/datasets/load_fmnist.py
--rw-r--r--   0        0        0     2955 2023-06-07 14:33:17.378645 asociita-0.1.9/asociita/datasets/load_mnist.py
--rw-r--r--   0        0        0     1314 2023-06-07 14:34:55.775257 asociita-0.1.9/asociita/datasets/save_blueprint.py
--rw-r--r--   0        0        0     6830 2023-06-07 14:40:50.095085 asociita-0.1.9/asociita/datasets/shard_splits.py
--rw-r--r--   0        0        0     5962 2023-05-30 10:15:28.967345 asociita-0.1.9/asociita/datasets/shard_transformation.py
--rw-r--r--   0        0        0      391 2023-06-05 10:23:46.853997 asociita-0.1.9/asociita/exceptions/evaluatorexception.py
--rw-r--r--   0        0        0      322 2023-05-29 08:30:33.477904 asociita-0.1.9/asociita/exceptions/settingexception.py
--rw-r--r--   0        0        0      679 2023-05-29 08:30:33.481904 asociita-0.1.9/asociita/models/pytorch/cifar10.py
--rw-r--r--   0        0        0    14810 2023-06-06 11:35:25.808272 asociita-0.1.9/asociita/models/pytorch/federated_model.py
--rw-r--r--   0        0        0      288 2023-06-01 15:35:54.360809 asociita-0.1.9/asociita/models/pytorch/fmnist.py
--rw-r--r--   0        0        0      934 2023-05-31 13:26:40.943955 asociita-0.1.9/asociita/models/pytorch/mnist.py
--rw-r--r--   0        0        0     5918 2023-05-29 08:30:33.481904 asociita-0.1.9/asociita/utils/computations.py
--rw-r--r--   0        0        0      613 2023-05-29 08:30:33.481904 asociita-0.1.9/asociita/utils/custom_transformations.py
--rw-r--r--   0        0        0     4648 2023-05-29 08:30:33.481904 asociita-0.1.9/asociita/utils/handlers.py
--rw-r--r--   0        0        0      572 2023-05-29 08:30:33.481904 asociita-0.1.9/asociita/utils/helpers.py
--rw-r--r--   0        0        0     1904 2023-06-06 11:38:43.941409 asociita-0.1.9/asociita/utils/loggers.py
--rw-r--r--   0        0        0     7791 2023-06-05 13:21:15.847962 asociita-0.1.9/asociita/utils/optimizers.py
--rw-r--r--   0        0        0     4526 2023-06-05 10:50:02.994008 asociita-0.1.9/asociita/utils/orchestrations.py
--rw-r--r--   0        0        0     1026 2023-05-29 08:30:33.481904 asociita-0.1.9/asociita/utils/showcase.py
--rw-r--r--   0        0        0      678 2023-06-07 14:46:31.479257 asociita-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 asociita-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-29 08:30:33.477904 asociita-0.1.9.1/LICENSE
+-rw-r--r--   0        0        0     2812 2023-05-29 08:30:33.477904 asociita-0.1.9.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 08:30:33.477904 asociita-0.1.9.1/asociita/__init__.py
+-rw-r--r--   0        0        0     3881 2023-05-29 08:30:33.477904 asociita-0.1.9.1/asociita/components/archiver/archive_manager.py
+-rw-r--r--   0        0        0     6970 2023-06-05 13:24:07.885952 asociita-0.1.9.1/asociita/components/evaluator/evaluation_manager.py
+-rw-r--r--   0        0        0    13324 2023-05-29 08:30:33.477904 asociita-0.1.9.1/asociita/components/evaluator/mr_evaluator.py
+-rw-r--r--   0        0        0     9972 2023-06-05 09:45:20.347198 asociita-0.1.9.1/asociita/components/evaluator/or_evaluator.py
+-rw-r--r--   0        0        0     2106 2023-06-05 13:51:59.255884 asociita-0.1.9.1/asociita/components/evaluator/sample_evaluator.py
+-rw-r--r--   0        0        0     4370 2023-06-06 11:35:25.808272 asociita-0.1.9.1/asociita/components/nodes/federated_node.py
+-rw-r--r--   0        0        0     7549 2023-06-06 11:41:23.091887 asociita-0.1.9.1/asociita/components/orchestrator/evaluator_orchestrator.py
+-rw-r--r--   0        0        0     6226 2023-06-06 11:42:03.726476 asociita-0.1.9.1/asociita/components/orchestrator/fedopt_orchestrator.py
+-rw-r--r--   0        0        0    11069 2023-06-06 11:35:25.808272 asociita-0.1.9.1/asociita/components/orchestrator/generic_orchestrator.py
+-rw-r--r--   0        0        0     3288 2023-06-07 13:08:30.716688 asociita-0.1.9.1/asociita/datasets/fetch_data.py
+-rw-r--r--   0        0        0     3012 2023-06-07 14:34:09.128863 asociita-0.1.9.1/asociita/datasets/load_cifar.py
+-rw-r--r--   0        0        0     2973 2023-06-07 14:34:21.476438 asociita-0.1.9.1/asociita/datasets/load_fmnist.py
+-rw-r--r--   0        0        0     2955 2023-06-07 14:33:17.378645 asociita-0.1.9.1/asociita/datasets/load_mnist.py
+-rw-r--r--   0        0        0     1314 2023-06-07 14:34:55.775257 asociita-0.1.9.1/asociita/datasets/save_blueprint.py
+-rw-r--r--   0        0        0     6838 2023-06-09 14:54:11.498938 asociita-0.1.9.1/asociita/datasets/shard_splits.py
+-rw-r--r--   0        0        0     5962 2023-05-30 10:15:28.967345 asociita-0.1.9.1/asociita/datasets/shard_transformation.py
+-rw-r--r--   0        0        0      391 2023-06-05 10:23:46.853997 asociita-0.1.9.1/asociita/exceptions/evaluatorexception.py
+-rw-r--r--   0        0        0      322 2023-05-29 08:30:33.477904 asociita-0.1.9.1/asociita/exceptions/settingexception.py
+-rw-r--r--   0        0        0      679 2023-05-29 08:30:33.481904 asociita-0.1.9.1/asociita/models/pytorch/cifar10.py
+-rw-r--r--   0        0        0    14810 2023-06-06 11:35:25.808272 asociita-0.1.9.1/asociita/models/pytorch/federated_model.py
+-rw-r--r--   0        0        0      288 2023-06-01 15:35:54.360809 asociita-0.1.9.1/asociita/models/pytorch/fmnist.py
+-rw-r--r--   0        0        0      934 2023-05-31 13:26:40.943955 asociita-0.1.9.1/asociita/models/pytorch/mnist.py
+-rw-r--r--   0        0        0     5918 2023-05-29 08:30:33.481904 asociita-0.1.9.1/asociita/utils/computations.py
+-rw-r--r--   0        0        0      613 2023-05-29 08:30:33.481904 asociita-0.1.9.1/asociita/utils/custom_transformations.py
+-rw-r--r--   0        0        0     4648 2023-05-29 08:30:33.481904 asociita-0.1.9.1/asociita/utils/handlers.py
+-rw-r--r--   0        0        0      572 2023-05-29 08:30:33.481904 asociita-0.1.9.1/asociita/utils/helpers.py
+-rw-r--r--   0        0        0     1904 2023-06-06 11:38:43.941409 asociita-0.1.9.1/asociita/utils/loggers.py
+-rw-r--r--   0        0        0     7791 2023-06-05 13:21:15.847962 asociita-0.1.9.1/asociita/utils/optimizers.py
+-rw-r--r--   0        0        0     4526 2023-06-05 10:50:02.994008 asociita-0.1.9.1/asociita/utils/orchestrations.py
+-rw-r--r--   0        0        0     1026 2023-05-29 08:30:33.481904 asociita-0.1.9.1/asociita/utils/showcase.py
+-rw-r--r--   0        0        0      680 2023-06-09 14:54:34.742141 asociita-0.1.9.1/pyproject.toml
+-rw-r--r--   0        0        0     3767 1970-01-01 00:00:00.000000 asociita-0.1.9.1/PKG-INFO
```

### Comparing `asociita-0.1.9/LICENSE` & `asociita-0.1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9/README.md` & `asociita-0.1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9/asociita/components/archiver/archive_manager.py` & `asociita-0.1.9.1/asociita/components/archiver/archive_manager.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9/asociita/components/evaluator/evaluation_manager.py` & `asociita-0.1.9.1/asociita/components/evaluator/evaluation_manager.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9/asociita/components/evaluator/mr_evaluator.py` & `asociita-0.1.9.1/asociita/components/evaluator/mr_evaluator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9/asociita/components/evaluator/or_evaluator.py` & `asociita-0.1.9.1/asociita/components/evaluator/or_evaluator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9/asociita/components/evaluator/sample_evaluator.py` & `asociita-0.1.9.1/asociita/components/evaluator/sample_evaluator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9/asociita/components/nodes/federated_node.py` & `asociita-0.1.9.1/asociita/components/nodes/federated_node.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9/asociita/components/orchestrator/evaluator_orchestrator.py` & `asociita-0.1.9.1/asociita/components/orchestrator/evaluator_orchestrator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9/asociita/components/orchestrator/fedopt_orchestrator.py` & `asociita-0.1.9.1/asociita/components/orchestrator/fedopt_orchestrator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9/asociita/components/orchestrator/generic_orchestrator.py` & `asociita-0.1.9.1/asociita/components/orchestrator/generic_orchestrator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9/asociita/datasets/fetch_data.py` & `asociita-0.1.9.1/asociita/datasets/fetch_data.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9/asociita/datasets/load_cifar.py` & `asociita-0.1.9.1/asociita/datasets/load_cifar.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9/asociita/datasets/load_fmnist.py` & `asociita-0.1.9.1/asociita/datasets/load_fmnist.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9/asociita/datasets/load_mnist.py` & `asociita-0.1.9.1/asociita/datasets/load_mnist.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9/asociita/datasets/save_blueprint.py` & `asociita-0.1.9.1/asociita/datasets/save_blueprint.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9/asociita/datasets/shard_splits.py` & `asociita-0.1.9.1/asociita/datasets/shard_splits.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
                 
                 # 2. Apllying weights
                 pandas_df["weights"] = pandas_df['label'].apply(lambda x: sampling_weights[x])
                 sample = pandas_df.sample(n = sample_size, weights='weights', random_state=42)
                 
                 counts = sample['label'].value_counts().sort_index()
                 # 3. Selecting indexes and performing test - train split.
-                sampled_data = dataset.filter(lambda idx: idx in list(sample.index), with_indices=True)
+                sampled_data = dataset.filter(lambda filter, idx: idx in list(sample.index), with_indices=True)
                 agent_data = sampled_data.train_test_split(test_size=settings["local_test_size"])
                 nodes_data.append([agent_data['train'], agent_data['test']])
                 
                 # 4. Removing samples indexes
                 pandas_df.drop(sample.index, inplace=True)
             else:
                 nodes_data.append([]) # Inserting placeholder to preserve in-list order.
```

### Comparing `asociita-0.1.9/asociita/datasets/shard_transformation.py` & `asociita-0.1.9.1/asociita/datasets/shard_transformation.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9/asociita/models/pytorch/cifar10.py` & `asociita-0.1.9.1/asociita/models/pytorch/cifar10.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9/asociita/models/pytorch/federated_model.py` & `asociita-0.1.9.1/asociita/models/pytorch/federated_model.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9/asociita/models/pytorch/mnist.py` & `asociita-0.1.9.1/asociita/models/pytorch/mnist.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9/asociita/utils/computations.py` & `asociita-0.1.9.1/asociita/utils/computations.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9/asociita/utils/custom_transformations.py` & `asociita-0.1.9.1/asociita/utils/custom_transformations.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9/asociita/utils/handlers.py` & `asociita-0.1.9.1/asociita/utils/handlers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9/asociita/utils/helpers.py` & `asociita-0.1.9.1/asociita/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9/asociita/utils/loggers.py` & `asociita-0.1.9.1/asociita/utils/loggers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9/asociita/utils/optimizers.py` & `asociita-0.1.9.1/asociita/utils/optimizers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9/asociita/utils/orchestrations.py` & `asociita-0.1.9.1/asociita/utils/orchestrations.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9/asociita/utils/showcase.py` & `asociita-0.1.9.1/asociita/utils/showcase.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.9/pyproject.toml` & `asociita-0.1.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asociita"
-version = "0.1.9"
+version = "0.1.9.1"
 description = "An intuitive and modular simulator for assessing the marginal value of a client's contribution in a decentralized setting."
 authors = ["Maciej Zuziak <maciejkrzysztof.zuziak@isti.cnr.it>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Scolpe/Asociita"
 repository = "https://github.com/Scolpe/Asociita"
```

### Comparing `asociita-0.1.9/PKG-INFO` & `asociita-0.1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asociita
-Version: 0.1.9
+Version: 0.1.9.1
 Summary: An intuitive and modular simulator for assessing the marginal value of a client's contribution in a decentralized setting.
 Home-page: https://github.com/Scolpe/Asociita
 License: MIT
 Author: Maciej Zuziak
 Author-email: maciejkrzysztof.zuziak@isti.cnr.it
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

