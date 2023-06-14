# Comparing `tmp/tensor_parallel-1.2.3.tar.gz` & `tmp/tensor_parallel-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensor_parallel-1.2.3.tar", last modified: Sun May 14 16:53:58 2023, max compression
+gzip compressed data, was "tensor_parallel-1.2.4.tar", last modified: Sun May 14 19:57:30 2023, max compression
```

## Comparing `tensor_parallel-1.2.3.tar` & `tensor_parallel-1.2.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:53:58.024569 tensor_parallel-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-05-14 16:53:58.028569 tensor_parallel-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-14 16:53:58.028569 tensor_parallel-1.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:53:58.020569 tensor_parallel-1.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:53:58.024569 tensor_parallel-1.2.3/src/tensor_parallel/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/src/tensor_parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/src/tensor_parallel/autoconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/src/tensor_parallel/aux_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/src/tensor_parallel/communications.py
--rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/src/tensor_parallel/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/src/tensor_parallel/cross_device_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/src/tensor_parallel/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/src/tensor_parallel/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/src/tensor_parallel/per_device_tensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/src/tensor_parallel/pretrained_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/src/tensor_parallel/shard.py
--rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/src/tensor_parallel/sharding.py
--rw-r--r--   0 runner    (1001) docker     (123)    19224 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/src/tensor_parallel/slicing_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/src/tensor_parallel/state_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11846 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/src/tensor_parallel/tensor_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/src/tensor_parallel/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/src/tensor_parallel/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:53:58.024569 tensor_parallel-1.2.3/src/tensor_parallel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-05-14 16:53:58.000000 tensor_parallel-1.2.3/src/tensor_parallel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-14 16:53:58.000000 tensor_parallel-1.2.3/src/tensor_parallel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 16:53:58.000000 tensor_parallel-1.2.3/src/tensor_parallel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-14 16:53:58.000000 tensor_parallel-1.2.3/src/tensor_parallel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-14 16:53:58.000000 tensor_parallel-1.2.3/src/tensor_parallel.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:53:58.024569 tensor_parallel-1.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/tests/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/tests/test_saving.py
--rw-r--r--   0 runner    (1001) docker     (123)    11171 2023-05-14 16:53:43.000000 tensor_parallel-1.2.3/tests/test_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:57:30.597556 tensor_parallel-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-14 19:57:17.000000 tensor_parallel-1.2.4/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-05-14 19:57:30.597556 tensor_parallel-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-05-14 19:57:17.000000 tensor_parallel-1.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-14 19:57:17.000000 tensor_parallel-1.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-14 19:57:30.597556 tensor_parallel-1.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:57:30.593556 tensor_parallel-1.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:57:30.597556 tensor_parallel-1.2.4/src/tensor_parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-14 19:57:17.000000 tensor_parallel-1.2.4/src/tensor_parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-14 19:57:17.000000 tensor_parallel-1.2.4/src/tensor_parallel/autoconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-14 19:57:17.000000 tensor_parallel-1.2.4/src/tensor_parallel/aux_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-05-14 19:57:17.000000 tensor_parallel-1.2.4/src/tensor_parallel/communications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-05-14 19:57:17.000000 tensor_parallel-1.2.4/src/tensor_parallel/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-05-14 19:57:17.000000 tensor_parallel-1.2.4/src/tensor_parallel/cross_device_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6093 2023-05-14 19:57:17.000000 tensor_parallel-1.2.4/src/tensor_parallel/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-05-14 19:57:17.000000 tensor_parallel-1.2.4/src/tensor_parallel/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-14 19:57:17.000000 tensor_parallel-1.2.4/src/tensor_parallel/per_device_tensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-05-14 19:57:17.000000 tensor_parallel-1.2.4/src/tensor_parallel/pretrained_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-05-14 19:57:17.000000 tensor_parallel-1.2.4/src/tensor_parallel/shard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-05-14 19:57:17.000000 tensor_parallel-1.2.4/src/tensor_parallel/sharding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19497 2023-05-14 19:57:17.000000 tensor_parallel-1.2.4/src/tensor_parallel/slicing_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-05-14 19:57:17.000000 tensor_parallel-1.2.4/src/tensor_parallel/state_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11969 2023-05-14 19:57:17.000000 tensor_parallel-1.2.4/src/tensor_parallel/tensor_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-05-14 19:57:17.000000 tensor_parallel-1.2.4/src/tensor_parallel/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-14 19:57:17.000000 tensor_parallel-1.2.4/src/tensor_parallel/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:57:30.597556 tensor_parallel-1.2.4/src/tensor_parallel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-05-14 19:57:30.000000 tensor_parallel-1.2.4/src/tensor_parallel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-14 19:57:30.000000 tensor_parallel-1.2.4/src/tensor_parallel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 19:57:30.000000 tensor_parallel-1.2.4/src/tensor_parallel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-14 19:57:30.000000 tensor_parallel-1.2.4/src/tensor_parallel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-14 19:57:30.000000 tensor_parallel-1.2.4/src/tensor_parallel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:57:30.597556 tensor_parallel-1.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-05-14 19:57:17.000000 tensor_parallel-1.2.4/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-14 19:57:17.000000 tensor_parallel-1.2.4/tests/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-05-14 19:57:17.000000 tensor_parallel-1.2.4/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-05-14 19:57:17.000000 tensor_parallel-1.2.4/tests/test_saving.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11391 2023-05-14 19:57:17.000000 tensor_parallel-1.2.4/tests/test_transformers.py
```

### Comparing `tensor_parallel-1.2.3/LICENCE` & `tensor_parallel-1.2.4/LICENCE`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.3/PKG-INFO` & `tensor_parallel-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensor_parallel
-Version: 1.2.3
+Version: 1.2.4
 Summary: Automatically shard your large model between multiple GPUs, works without torch.distributed
 Home-page: https://github.com/BlackSamorez/tensor_parallel
 Author: Andrei Panferov and Yaroslav Lisnyak
 Author-email: yalisnyak@nes.com
 Project-URL: Bug Tracker, https://github.com/BlackSamorez/tensor_parallel/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tensor_parallel Version: 1.2.3 Summary:
+Metadata-Version: 2.1 Name: tensor_parallel Version: 1.2.4 Summary:
 Automatically shard your large model between multiple GPUs, works without
 torch.distributed Home-page: https://github.com/BlackSamorez/tensor_parallel
 Author: Andrei Panferov and Yaroslav Lisnyak Author-email: yalisnyak@nes.com
 Project-URL: Bug Tracker, https://github.com/BlackSamorez/tensor_parallel/
 issues Classifier: Development Status :: 4 - Beta Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
```

### Comparing `tensor_parallel-1.2.3/README.md` & `tensor_parallel-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.3/setup.cfg` & `tensor_parallel-1.2.4/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tensor_parallel
-version = 1.2.3
+version = 1.2.4
 author = Andrei Panferov and Yaroslav Lisnyak
 author_email = yalisnyak@nes.com
 description = Automatically shard your large model between multiple GPUs, works without torch.distributed
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/BlackSamorez/tensor_parallel
 project_urls =
```

### Comparing `tensor_parallel-1.2.3/src/tensor_parallel/__init__.py` & `tensor_parallel-1.2.4/src/tensor_parallel/__init__.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.3/src/tensor_parallel/autoconfig.py` & `tensor_parallel-1.2.4/src/tensor_parallel/autoconfig.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.3/src/tensor_parallel/aux_actions.py` & `tensor_parallel-1.2.4/src/tensor_parallel/aux_actions.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.3/src/tensor_parallel/communications.py` & `tensor_parallel-1.2.4/src/tensor_parallel/communications.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.3/src/tensor_parallel/config.py` & `tensor_parallel-1.2.4/src/tensor_parallel/config.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.3/src/tensor_parallel/cross_device_ops.py` & `tensor_parallel-1.2.4/src/tensor_parallel/cross_device_ops.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.3/src/tensor_parallel/dispatch.py` & `tensor_parallel-1.2.4/src/tensor_parallel/dispatch.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Union
 
 import torch
 
 from tensor_parallel.pretrained_model import TensorParallelPreTrainedModel
 from tensor_parallel.sharding import Sharded
 from tensor_parallel.tensor_parallel import Config, TensorParallel
+from tensor_parallel.utils import find_tied_weight_aliases
 
 
 @contextmanager
 def save_tensor_parallel(model: Union[TensorParallel, TensorParallelPreTrainedModel, Sharded]):
     """Enables state_dict reconstruction for tensor_parallel models.
     With it '.state_dict()' produces a state dict that can be loaded into an underlying model.
     Example:
@@ -51,26 +52,34 @@
 
     Args:
         tp_model (Union[TensorParallel, TensorParallelPreTrainedModel]): tensor parallel model
 
     Returns:
         dict: parameter device mapping
     """
+    id_to_device = {}
+    for name, param in tp_model.named_parameters():
+        id_to_device[id(param)] = tp_model.devices[infer_sharded_data_device_id(name)]
+    for name, buffer in tp_model.named_buffers():
+        id_to_device[id(buffer)] = tp_model.devices[infer_sharded_data_device_id(name)]
+    id_to_aliases = find_tied_weight_aliases(tp_model)
+
     device_map = {}
-    for name, _ in tp_model.named_parameters():
-        device_map[name] = tp_model.devices[infer_sharded_data_device_id(name)]
-    for name, _ in tp_model.named_buffers():
-        device_map[name] = tp_model.devices[infer_sharded_data_device_id(name)]
+    for idx, aliases in id_to_aliases.items():
+        for alias in aliases:
+            device_map[alias] = id_to_device[idx]
+
     return device_map
 
 
 def convert_state_dict(
     input_state_dict, tensor_parallel_config: Config, world_size: int, for_pretrained: bool = False
 ) -> dict:
     """Creates a state_dict to be loaded into a tensor parallel model from a state_dict of a base model.
+    WARNING: this function doesn't properly work with tied weights. You'll probably need to fix the resulting state_dict by hand.
 
     Args:
         input_state_dict (_type_): state_dict to be converted
         tensor_parallel_config (Config): tensor parallel config for the base model
         world_size (int): number of devices of the tensor parallel model
         for_pretrained (bool, optional): Whether to create a state dict to be loaded into TensorParallelModel of PreTrainedTensorParallelModel. Defaults to False.
```

### Comparing `tensor_parallel-1.2.3/src/tensor_parallel/factory.py` & `tensor_parallel-1.2.4/src/tensor_parallel/factory.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.3/src/tensor_parallel/per_device_tensors.py` & `tensor_parallel-1.2.4/src/tensor_parallel/per_device_tensors.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.3/src/tensor_parallel/pretrained_model.py` & `tensor_parallel-1.2.4/src/tensor_parallel/pretrained_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 The TensorParallel module wrapper for Hugging Face PreTrainedModel
 """
 import logging
+from functools import lru_cache
 from typing import Any, Dict, Optional, Sequence
 
 import torch
 from torch import nn
 from transformers import PretrainedConfig, PreTrainedModel
 
 from tensor_parallel.config import TENSOR_PARALLEL_USE_NATIVE, Config
@@ -53,19 +54,14 @@
         if tensor_parallel_config is None:
             tensor_parallel_config = find_predefined_tensor_parallel_config(module.config, device_ids)
 
         self.wrapped_model = TensorParallel(
             module, device_ids, output_device, output_device_index, tensor_parallel_config
         )
 
-        self.encoder_shards = nn.ModuleList()
-        if module.config.is_encoder_decoder:
-            for encoder_decoder_shard in self.wrapped_model.module_shards:
-                self.encoder_shards.append(encoder_decoder_shard.get_encoder())
-
     @property
     def devices(self):
         return self.wrapped_model.devices
 
     @property
     def tensor_parallel_config(self):
         return self.wrapped_model.tensor_parallel_config
@@ -109,19 +105,24 @@
     def _reorder_cache(self, past, beam_idx):
         for i, shard in enumerate(self.wrapped_model.module_shards):
             shard._reorder_cache(
                 nested_map(lambda x: x[i] if isinstance(x, PerDeviceTensors) else x, past),
                 beam_idx.to(self.wrapped_model.devices[i]),
             )
 
+    @lru_cache(maxsize=None)
     def get_encoder(self):
         assert len(self.wrapped_model.module_shards), "Can't get encoder since no module shards present"
         if len(self.wrapped_model.module_shards) == 1:
             return self.wrapped_model.module_shards[0].get_encoder()
 
+        encoder_shards = [
+            encoder_decoder_shard.get_encoder() for encoder_decoder_shard in self.wrapped_model.module_shards
+        ]
+
         encoder_wrapper_class = None
         if isinstance(self.wrapped_model, TensorParallel):
 
             class _EncoderWrapper(torch.nn.Module):
                 def __init__(self, wrapped_pretrained_model: TensorParallelPreTrainedModel) -> None:
                     super().__init__()
                     self.wrapped_pretrained_model = wrapped_pretrained_model
@@ -129,22 +130,22 @@
                 def forward(self, *args, **kwargs):
                     (
                         inputs,
                         kwargs_tup,
                     ) = self.wrapped_pretrained_model.wrapped_model.prepare_args_kwargs_for_forward(*args, **kwargs)
                     if self.wrapped_pretrained_model.wrapped_model.all_cuda and not TENSOR_PARALLEL_USE_NATIVE:
                         return parallel_apply(
-                            self.wrapped_pretrained_model.encoder_shards,
+                            encoder_shards,
                             inputs,
                             kwargs_tup,
                             self.wrapped_pretrained_model.wrapped_model.devices,
                         )[self.wrapped_pretrained_model.wrapped_model.output_device_index]
                     else:
                         return parallel_apply_simple(
-                            self.wrapped_pretrained_model.encoder_shards,
+                            encoder_shards,
                             inputs,
                             kwargs_tup,
                             self.wrapped_pretrained_model.wrapped_model.devices,
                         )[self.wrapped_pretrained_model.wrapped_model.output_device_index]
 
             encoder_wrapper_class = _EncoderWrapper
 
@@ -165,22 +166,22 @@
                         inputs,
                         kwargs_tup,
                     ) = self.wrapped_pretrained_model.wrapped_model.module.prepare_args_kwargs_for_forward(
                         *args, **kwargs
                     )
                     if self.wrapped_pretrained_model.wrapped_model.module.all_cuda and not TENSOR_PARALLEL_USE_NATIVE:
                         return parallel_apply(
-                            self.wrapped_pretrained_model.encoder_shards,
+                            encoder_shards,
                             inputs,
                             kwargs_tup,
                             self.wrapped_pretrained_model.wrapped_model.module.devices,
                         )[self.wrapped_pretrained_model.wrapped_model.module.output_device_index]
                     else:
                         return parallel_apply_simple(
-                            self.wrapped_pretrained_model.encoder_shards,
+                            encoder_shards,
                             inputs,
                             kwargs_tup,
                             self.wrapped_pretrained_model.wrapped_model.module.devices,
                         )[self.wrapped_pretrained_model.wrapped_model.module.output_device_index]
 
             encoder_wrapper_class = _EncoderWrapper
```

### Comparing `tensor_parallel-1.2.3/src/tensor_parallel/shard.py` & `tensor_parallel-1.2.4/src/tensor_parallel/shard.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.3/src/tensor_parallel/sharding.py` & `tensor_parallel-1.2.4/src/tensor_parallel/sharding.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.3/src/tensor_parallel/slicing_configs.py` & `tensor_parallel-1.2.4/src/tensor_parallel/slicing_configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,16 @@
             r".*self_attention\.dense\.weight$": SplitInChunks(world_size=world_size, dim=1, chunk_size=head_dim),
             r".*self_attention\.dense\.bias$": Scale(world_size=world_size),
             # BloomMLP
             r".*mlp\.dense_h_to_4h\.(weight|bias)$": Split(world_size=world_size, dim=0),
             r".*mlp\.dense_4h_to_h\.weight$": Split(world_size=world_size, dim=1),
             r".*mlp\.dense_4h_to_h\.bias$": Scale(world_size=world_size),
             # BloomModel
-            r".*word_embeddings.weight$": Split(world_size=world_size, dim=1),
+            r".*word_embeddings\.weight$": Split(world_size=world_size, dim=1),
+            r".*lm_head\.weight$": Split(world_size=world_size, dim=1),
             # note: ^-- lm_head.weight is tied with word_embeddings
         },
         input_rules={
             r".*self_attention$": {"layer_past": select_kv_for_rank, "alibi": _split_alibi},
             r".*lm_head$": {0: "split -1"},  # note: we need to split lm_head inputs because
             # ... lm_head's weights (tied embeddings) are already split across input dimension
         },
@@ -104,27 +105,29 @@
             # T5DenseGatedActDense
             r".*DenseReluDense\.wi\.weight$": Split(world_size=world_size, dim=0),
             r".*DenseReluDense\.wi_0\.weight$": Split(world_size=world_size, dim=0),
             r".*DenseReluDense\.wi_1\.weight$": Split(world_size=world_size, dim=0),
             # T5DenseActDense
             r".*DenseReluDense\.wo\.weight$": Split(world_size=world_size, dim=1),
             # T5Model
-            r".*shared.weight$": Split(world_size=world_size, dim=1),
+            r".*embed_tokens\.weight$": Split(world_size=world_size, dim=1),
+            r".*shared\.weight$": Split(world_size=world_size, dim=1),
             r".*lm_head\.weight$": Split(world_size=world_size, dim=1),
             # note: ^-- lm_head.weight tied with word embeddings
         },
         input_rules={
             r".*SelfAttention$": {"past_key_value": select_kv_for_rank},
             r".*lm_head$": {0: "split -1"},  # note: we need to split lm_head inputs because
             # ... lm_head's weights (tied embeddings) are already split across input dimension
         },
         output_rules={
             r".*SelfAttention$": {0: "sum", 1: gather_kv_across_ranks},
             r".*DenseReluDense$": {0: "sum"},
             r".*shared$": {0: "gather -1"},
+            r".*embed_tokens$": {0: "gather -1"},
             r".*lm_head$": {0: "sum"},
         },
         attr_rules={
             r".*SelfAttention$": {
                 "n_heads": partial(split_num_heads, world_size=world_size),
                 "inner_dim": partial(split_inner_dim, num_heads=model_config.num_heads, world_size=world_size),
             },
@@ -212,14 +215,15 @@
             r".*c_fc\.weight$": Split(world_size=world_size, dim=1),
             r".*c_fc\.bias$": Split(world_size=world_size, dim=0),
             r".*mlp\.c_proj\.weight$": Split(world_size=world_size, dim=0),
             r".*mlp\.c_proj\.bias$": Scale(world_size=world_size),
             # GPT2Model
             r".*wte\.weight$": Split(world_size=world_size, dim=1),
             r".*wpe\.weight$": Split(world_size=world_size, dim=1),
+            r".*lm_head\.weight$": Split(world_size=world_size, dim=1),
             # GPT2LMHeadModel
             # note: ^-- lm_head.weight is tied with word_embeddings
         },
         input_rules={
             r".*[0-9]\.attn$": {"layer_past": select_kv_for_rank},
             r".*lm_head$": {0: "split -1"},  # note: we need to split lm_head inputs because
             # ... lm_head's weights (tied embeddings) are already split across input dimension
```

### Comparing `tensor_parallel-1.2.3/src/tensor_parallel/state_actions.py` & `tensor_parallel-1.2.4/src/tensor_parallel/state_actions.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.3/src/tensor_parallel/tensor_parallel.py` & `tensor_parallel-1.2.4/src/tensor_parallel/tensor_parallel.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,20 +132,29 @@
             return parallel_apply_simple(self.module_shards, inputs, kwargs_tup, self.devices)[self.output_device_index]
 
     def state_dict(self, *args, **kwargs):
         state_dict = super().state_dict(*args, **kwargs)
         if self.preserve_shards_when_saving:
             return state_dict
 
+        for i in range(len(self.module_shards)):
+            sanity_check_param_name = next(
+                name for name, _ in state_dict.items() if name.endswith(f"_sanity_check_params.{i}")
+            )
+            del state_dict[sanity_check_param_name]
+
         # fix names for zero-3'ed params that were inside _TensorParallelWrapper
         names_inside_tp_wrapper = [name for name in state_dict.keys() if "tp_wrapped_module." in name]
         for name in names_inside_tp_wrapper:
             state_dict[name.replace("tp_wrapped_module.", "")] = state_dict.pop(name)
 
-        shards_prefix = next(name for name, _ in state_dict.items() if "module_shards." in name)
+        try:
+            shards_prefix = next(name for name, _ in state_dict.items() if "module_shards." in name)
+        except StopIteration:
+            return state_dict  # no parameters are actually tensor parallel
         shards_prefix = shards_prefix[: shards_prefix.find("module_shards.") + len("module_shards.")]
         module_prefix = shards_prefix[: -len("module_shards.")]
 
         # get names for desired tensors and where to find them (shards of zero-3)
         is_name_prefixed = {}
         for name, tensor in state_dict.items():
             if name.startswith(shards_prefix + "0."):  # dict entry is from shards
@@ -167,20 +176,14 @@
                     tensor for name, tensor in state_dict.items() if name.endswith(unsharded_name)
                 )
             if is_prefixed:
                 # delete sharded tensor entries
                 for i in range(len(self.module_shards)):
                     del state_dict[f"{shards_prefix}{i}.{unsharded_name}"]
 
-        for i in range(len(self.module_shards)):
-            sanity_check_param_name = next(
-                name for name, _ in state_dict.items() if name.endswith(f"_sanity_check_params.{i}")
-            )
-            del state_dict[sanity_check_param_name]
-
         return state_dict
 
 
 def parallel_apply_simple(
     modules: Sequence[nn.Module],
     inputs: Sequence[Sequence[torch.Tensor]],
     kwargs_tup: Optional[Any],
```

### Comparing `tensor_parallel-1.2.3/src/tensor_parallel/wrapper.py` & `tensor_parallel-1.2.4/src/tensor_parallel/wrapper.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.3/src/tensor_parallel.egg-info/PKG-INFO` & `tensor_parallel-1.2.4/src/tensor_parallel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensor-parallel
-Version: 1.2.3
+Version: 1.2.4
 Summary: Automatically shard your large model between multiple GPUs, works without torch.distributed
 Home-page: https://github.com/BlackSamorez/tensor_parallel
 Author: Andrei Panferov and Yaroslav Lisnyak
 Author-email: yalisnyak@nes.com
 Project-URL: Bug Tracker, https://github.com/BlackSamorez/tensor_parallel/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tensor-parallel Version: 1.2.3 Summary:
+Metadata-Version: 2.1 Name: tensor-parallel Version: 1.2.4 Summary:
 Automatically shard your large model between multiple GPUs, works without
 torch.distributed Home-page: https://github.com/BlackSamorez/tensor_parallel
 Author: Andrei Panferov and Yaroslav Lisnyak Author-email: yalisnyak@nes.com
 Project-URL: Bug Tracker, https://github.com/BlackSamorez/tensor_parallel/
 issues Classifier: Development Status :: 4 - Beta Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
```

### Comparing `tensor_parallel-1.2.3/src/tensor_parallel.egg-info/SOURCES.txt` & `tensor_parallel-1.2.4/src/tensor_parallel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.3/tests/test_basic.py` & `tensor_parallel-1.2.4/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.3/tests/test_factory.py` & `tensor_parallel-1.2.4/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.3/tests/test_integration.py` & `tensor_parallel-1.2.4/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.3/tests/test_saving.py` & `tensor_parallel-1.2.4/tests/test_saving.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,41 +17,47 @@
 
 PATH_TO_SAVE = "/tmp/"
 
 
 @pytest.mark.parametrize("devices", [("cpu",) * 2, ("cpu",) * 3])
 @pytest.mark.parametrize("model_name", ["bert-base-uncased"])
 def test_no_parallelism_zero_3(devices, model_name):
-    model = AutoModel.from_pretrained(model_name).to(devices[0])
+    model = AutoModel.from_pretrained(model_name).to(devices[0]).half()
     model_state_dict = model.state_dict()
     model_tp = Sharded(
         TensorParallel(model, devices, tensor_parallel_config=Config({}, {}, {}, {}))
     )  # zero-3 sharding only
+    del model
     with save_tensor_parallel(model_tp):
         model_tp_state_dict = model_tp.state_dict()
+    del model_tp
 
     assert sorted(list(model_state_dict.keys())) == sorted(list(model_tp_state_dict.keys()))
 
     for name in model_state_dict.keys():
         data = model_state_dict[name]
         data_tp = model_tp_state_dict[name]
 
         assert data.shape == data_tp.shape
 
         torch.testing.assert_close(data, data_tp)
 
 
 @pytest.mark.parametrize("devices", [("cpu",) * 2, ("cpu",) * 3])
-@pytest.mark.parametrize("model_name", ["bert-base-uncased"])
+@pytest.mark.parametrize(
+    "model_name", ["bert-base-uncased", "hf-internal-testing/tiny-random-t5", "hf-internal-testing/tiny-random-t5"]
+)
 def test_parallelism_no_zero_3(devices, model_name):
-    model = AutoModel.from_pretrained(model_name).to(devices[0])
+    model = AutoModel.from_pretrained(model_name).to(devices[0]).half()
     model_state_dict = model.state_dict()
     model_tp = TensorParallelPreTrainedModel(model, devices)
+    del model
     with save_tensor_parallel(model_tp):
         model_tp_state_dict = model_tp.state_dict()
+    del model_tp
 
     assert sorted(list(model_state_dict.keys())) == sorted(list(model_tp_state_dict.keys()))
 
     for name in model_state_dict.keys():
         data = model_state_dict[name]
         data_tp = model_tp_state_dict[name]
 
@@ -59,87 +65,84 @@
 
         torch.testing.assert_close(data, data_tp)
 
 
 @pytest.mark.parametrize("devices", [("cpu",) * 2, ("cpu",) * 3])
 @pytest.mark.parametrize("model_name", ["bert-base-uncased"])
 def test_parallelism_zero_3(devices, model_name):
-    model = AutoModel.from_pretrained(model_name).to(devices[0])
+    model = AutoModel.from_pretrained(model_name).to(devices[0]).half()
     model_state_dict = model.state_dict()
     model_tp = tensor_parallel(model, devices, sharded=True)
+    del model
     with save_tensor_parallel(model_tp):
         model_tp_state_dict = model_tp.state_dict()
+    del model_tp
 
     assert sorted(list(model_state_dict.keys())) == sorted(list(model_tp_state_dict.keys()))
 
     for name in model_state_dict.keys():
         data = model_state_dict[name]
         data_tp = model_tp_state_dict[name]
 
-        assert data.shape == data_tp.shape
+        assert data.shape == data_tp.shape, name
 
         torch.testing.assert_close(data, data_tp, msg=lambda msg: f"{name}:\n{msg}")
 
 
 @pytest.mark.parametrize("devices", [("cpu",) * 2, ("cpu",) * 3])
-@pytest.mark.parametrize("model_name", ["bert-base-uncased"])
+@pytest.mark.parametrize(
+    "model_name", ["bert-base-uncased", "hf-internal-testing/tiny-random-t5", "hf-internal-testing/tiny-random-bloom"]
+)
 @pytest.mark.parametrize("shard_as_pretrained", [True, False])
 def test_save_keep_shards(devices, model_name, shard_as_pretrained):
-    model = AutoModel.from_pretrained(model_name).to(devices[0])
+    model = AutoModel.from_pretrained(model_name).to(devices[0]).half()
     if shard_as_pretrained:
         model_tp = TensorParallelPreTrainedModel(model, devices)
     else:
         model_tp = TensorParallel(model, devices)
 
     model_tp.load_state_dict(model_tp.state_dict())
 
 
-def test_sharding_meta():
-    model_name = "bert-base-uncased"
-    with init_empty_weights():
-        model_tp = TensorParallel(AutoModel.from_pretrained(model_name), ["meta", "meta"])
-
-    with pytest.raises(RuntimeError):
-        Sharded(model_tp)
-
-
 @pytest.mark.parametrize("devices", [("cpu",) * 2, ("cpu",) * 3])
-@pytest.mark.parametrize("model_name", ["bert-base-uncased"])
+@pytest.mark.parametrize(
+    "model_name", ["bert-base-uncased", "hf-internal-testing/tiny-random-t5", "hf-internal-testing/tiny-random-bloom"]
+)
 @pytest.mark.parametrize("pretrained", [True])
 def test_save_shards_load_shards(devices, model_name, pretrained):
     devices = [torch.device(device) for device in devices]
 
-    model = AutoModel.from_pretrained(model_name).to(devices[0])
+    model = AutoModel.from_pretrained(model_name).to(devices[0]).half()
     shraded_class = TensorParallelPreTrainedModel if pretrained else TensorParallel
     model_tp = shraded_class(model, devices)
 
     if pretrained:
         half_the_model = f"{sum([p.numel() for p in model_tp.parameters()]) // 1_000_000 // 2}MB"
         model_tp.save_pretrained(PATH_TO_SAVE, max_shard_size=half_the_model)
     else:
         torch.save(model_tp.state_dict(), PATH_TO_SAVE + "test_save_shards_load_shards.bin")
     del model_tp
 
     with init_empty_weights():
-        model_tp = shraded_class(AutoModel.from_config(AutoConfig.from_pretrained(model_name)), devices)
+        model_tp = shraded_class(AutoModel.from_config(AutoConfig.from_pretrained(model_name)).half(), devices)
 
     checkpoint = PATH_TO_SAVE + ("pytorch_model.bin.index.json" if pretrained else "test_save_shards_load_shards.bin")
     load_checkpoint_in_model(
         model_tp,
         checkpoint=checkpoint,
         device_map=infer_sharded_device_map(model_tp),
     )
     assert not "meta" in [p.device.type for p in model_tp.parameters()]
 
 
 @pytest.mark.parametrize("use_pretrained", [False, True])
 @pytest.mark.parametrize("devices", [("cpu",) * 2, ("cpu",) * 3])
 @pytest.mark.parametrize("model_name", ["bert-base-uncased"])
 def test_convert_state_dict(use_pretrained, devices, model_name):
-    model = AutoModel.from_pretrained(model_name).to(devices[0])
+    model = AutoModel.from_pretrained(model_name).to(devices[0]).half()
     torch.save(model.state_dict(), PATH_TO_SAVE + "test_convert_state_dict.bin")
 
     if use_pretrained:
         model_tp = TensorParallelPreTrainedModel(model, devices)
     else:
         model_tp = TensorParallel(model, devices)
     del model
```

### Comparing `tensor_parallel-1.2.3/tests/test_transformers.py` & `tensor_parallel-1.2.4/tests/test_transformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,18 +261,24 @@
 @pytest.mark.parametrize("sharded", [False, True])
 def test_encoder(use_predefined_config, model_name, sharded):
     torch.manual_seed(0)
 
     devices = ["cpu"] * 2
     model = T5ForConditionalGeneration.from_pretrained(model_name, low_cpu_mem_usage=True).float().to(devices[0])
 
-    input = torch.randint(1, 1000, size=(2, 3), device=devices[0])
-    out_ref = model.get_encoder()(input)
+    inp1 = torch.randint(1, 1000, size=(2, 3), device=devices[0])
+    inp2 = torch.randint(1, 1000, size=(2, 3), device=devices[0])
+
+    out1_ref = model.get_encoder()(inp1)
+    out2_ref = model.get_encoder()(inp2)
 
     if not use_predefined_config:
         model.config.architectures = ["Pretend we don't know this architecture"]
     model_tp = tensor_parallel(model, devices, sharded=sharded)
     assert isinstance(model_tp, TensorParallelPreTrainedModel)
     del model
 
-    out = model_tp.get_encoder()(input)
-    torch.testing.assert_close(out_ref, out, atol=3e-3, rtol=1e-05)
+    out1 = model_tp.get_encoder()(inp1)
+    out2 = model_tp.get_encoder()(inp2)
+
+    torch.testing.assert_close(out1_ref, out1, atol=3e-3, rtol=1e-05)
+    torch.testing.assert_close(out2_ref, out2, atol=3e-3, rtol=1e-05)
```

