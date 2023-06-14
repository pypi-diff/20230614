# Comparing `tmp/ml-pretrained-0.0.8.tar.gz` & `tmp/ml-pretrained-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-pretrained-0.0.8.tar", last modified: Wed Jun  7 05:40:04 2023, max compression
+gzip compressed data, was "ml-pretrained-0.0.9.tar", last modified: Tue Jun 13 21:52:47 2023, max compression
```

## Comparing `ml-pretrained-0.0.8.tar` & `ml-pretrained-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:40:04.708328 ml-pretrained-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-07 05:40:04.708328 ml-pretrained-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:40:04.708328 ml-pretrained-0.0.8/ml_pretrained.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-07 05:40:04.000000 ml-pretrained-0.0.8/ml_pretrained.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-07 05:40:04.000000 ml-pretrained-0.0.8/ml_pretrained.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 05:40:04.000000 ml-pretrained-0.0.8/ml_pretrained.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-07 05:40:04.000000 ml-pretrained-0.0.8/ml_pretrained.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 05:40:04.000000 ml-pretrained-0.0.8/ml_pretrained.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:40:04.708328 ml-pretrained-0.0.8/pretrained/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/pretrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16681 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/pretrained/blip.py
--rw-r--r--   0 runner    (1001) docker     (123)    40892 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/pretrained/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    26309 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/pretrained/hubert.py
--rw-r--r--   0 runner    (1001) docker     (123)    23674 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/pretrained/llama.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/pretrained/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/pretrained/rwkv.py
--rw-r--r--   0 runner    (1001) docker     (123)    60932 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/pretrained/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)    46647 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/pretrained/tacotron2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:40:04.708328 ml-pretrained-0.0.8/pretrained/vocoder/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/pretrained/vocoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/pretrained/vocoder/hifigan.py
--rw-r--r--   0 runner    (1001) docker     (123)    13020 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/pretrained/vocoder/waveglow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-07 05:40:04.708328 ml-pretrained-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:40:04.708328 ml-pretrained-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/tests/test_rwkv.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-07 05:39:53.000000 ml-pretrained-0.0.8/tests/test_tacotron2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:52:47.986707 ml-pretrained-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-13 21:52:35.000000 ml-pretrained-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-13 21:52:35.000000 ml-pretrained-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-06-13 21:52:47.986707 ml-pretrained-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-06-13 21:52:35.000000 ml-pretrained-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:52:47.982707 ml-pretrained-0.0.9/ml_pretrained.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-06-13 21:52:47.000000 ml-pretrained-0.0.9/ml_pretrained.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-13 21:52:47.000000 ml-pretrained-0.0.9/ml_pretrained.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 21:52:47.000000 ml-pretrained-0.0.9/ml_pretrained.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-13 21:52:47.000000 ml-pretrained-0.0.9/ml_pretrained.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-13 21:52:47.000000 ml-pretrained-0.0.9/ml_pretrained.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:52:47.986707 ml-pretrained-0.0.9/pretrained/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-13 21:52:35.000000 ml-pretrained-0.0.9/pretrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16680 2023-06-13 21:52:35.000000 ml-pretrained-0.0.9/pretrained/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40891 2023-06-13 21:52:35.000000 ml-pretrained-0.0.9/pretrained/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28957 2023-06-13 21:52:35.000000 ml-pretrained-0.0.9/pretrained/hubert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23673 2023-06-13 21:52:35.000000 ml-pretrained-0.0.9/pretrained/llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:52:35.000000 ml-pretrained-0.0.9/pretrained/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16262 2023-06-13 21:52:35.000000 ml-pretrained-0.0.9/pretrained/rwkv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60931 2023-06-13 21:52:35.000000 ml-pretrained-0.0.9/pretrained/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47611 2023-06-13 21:52:35.000000 ml-pretrained-0.0.9/pretrained/tacotron2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:52:47.986707 ml-pretrained-0.0.9/pretrained/triton/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:52:35.000000 ml-pretrained-0.0.9/pretrained/triton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9706 2023-06-13 21:52:35.000000 ml-pretrained-0.0.9/pretrained/triton/rwkv_kernel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:52:47.986707 ml-pretrained-0.0.9/pretrained/vocoder/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-13 21:52:35.000000 ml-pretrained-0.0.9/pretrained/vocoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9219 2023-06-13 21:52:35.000000 ml-pretrained-0.0.9/pretrained/vocoder/hifigan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12870 2023-06-13 21:52:35.000000 ml-pretrained-0.0.9/pretrained/vocoder/waveglow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-13 21:52:35.000000 ml-pretrained-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-13 21:52:47.986707 ml-pretrained-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-13 21:52:35.000000 ml-pretrained-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:52:47.986707 ml-pretrained-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-06-13 21:52:35.000000 ml-pretrained-0.0.9/tests/test_rwkv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-13 21:52:35.000000 ml-pretrained-0.0.9/tests/test_tacotron2.py
```

### Comparing `ml-pretrained-0.0.8/LICENSE` & `ml-pretrained-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.8/PKG-INFO` & `ml-pretrained-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-pretrained
-Version: 0.0.8
+Version: 0.0.9
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-pretrained
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
@@ -50,10 +50,12 @@
 
 This is a collection of pre-trained model implementations, which can be used in down-stream packages.
 
 ### Goal
 
 The goal of this repository is to make it as easy as possible to try out a pre-trained model, and eventually incorporate it into a new project. To that end, each implementation is a self-contained file, so that you can just copy-paste it wholesale into whatever project your using or use it directly without adding a bunch of dependencies. Additionally, the implementations use high-quality, modern Python syntax to be as easy to follow as possible.
 
+This also includes some custom Triton kernels for certain operations which may benefit from GPU acceleration.
+
 ### License
 
 Note that while this particular code is MIT licensed, but that does not mean that all of the model weights are. You should comply with the upstream licenses for models that you use.
```

### Comparing `ml-pretrained-0.0.8/README.md` & `ml-pretrained-0.0.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -33,10 +33,12 @@
 
 This is a collection of pre-trained model implementations, which can be used in down-stream packages.
 
 ### Goal
 
 The goal of this repository is to make it as easy as possible to try out a pre-trained model, and eventually incorporate it into a new project. To that end, each implementation is a self-contained file, so that you can just copy-paste it wholesale into whatever project your using or use it directly without adding a bunch of dependencies. Additionally, the implementations use high-quality, modern Python syntax to be as easy to follow as possible.
 
+This also includes some custom Triton kernels for certain operations which may benefit from GPU acceleration.
+
 ### License
 
 Note that while this particular code is MIT licensed, but that does not mean that all of the model weights are. You should comply with the upstream licenses for models that you use.
```

### Comparing `ml-pretrained-0.0.8/ml_pretrained.egg-info/PKG-INFO` & `ml-pretrained-0.0.9/ml_pretrained.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-pretrained
-Version: 0.0.8
+Version: 0.0.9
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-pretrained
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
@@ -50,10 +50,12 @@
 
 This is a collection of pre-trained model implementations, which can be used in down-stream packages.
 
 ### Goal
 
 The goal of this repository is to make it as easy as possible to try out a pre-trained model, and eventually incorporate it into a new project. To that end, each implementation is a self-contained file, so that you can just copy-paste it wholesale into whatever project your using or use it directly without adding a bunch of dependencies. Additionally, the implementations use high-quality, modern Python syntax to be as easy to follow as possible.
 
+This also includes some custom Triton kernels for certain operations which may benefit from GPU acceleration.
+
 ### License
 
 Note that while this particular code is MIT licensed, but that does not mean that all of the model weights are. You should comply with the upstream licenses for models that you use.
```

### Comparing `ml-pretrained-0.0.8/ml_pretrained.egg-info/SOURCES.txt` & `ml-pretrained-0.0.9/ml_pretrained.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -14,12 +14,14 @@
 pretrained/clip.py
 pretrained/hubert.py
 pretrained/llama.py
 pretrained/py.typed
 pretrained/rwkv.py
 pretrained/sam.py
 pretrained/tacotron2.py
+pretrained/triton/__init__.py
+pretrained/triton/rwkv_kernel.py
 pretrained/vocoder/__init__.py
 pretrained/vocoder/hifigan.py
 pretrained/vocoder/waveglow.py
 tests/test_rwkv.py
 tests/test_tacotron2.py
```

### Comparing `ml-pretrained-0.0.8/pretrained/blip.py` & `ml-pretrained-0.0.9/pretrained/blip.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,27 +27,26 @@
 from typing import Literal, Sequence, Union, get_args
 
 import numpy as np
 import PIL.Image
 import torch
 import torch.nn.functional as F
 import torchvision.transforms.functional as V
-from omegaconf import MISSING
-from torch import Tensor, nn
-
 from ml.core.config import conf_field
 from ml.models.activations import ActivationType, get_activation
 from ml.models.init import init_
 from ml.models.norms import NormType, get_norm_linear
 from ml.utils.checkpoint import ensure_downloaded
 from ml.utils.device.auto import AutoDevice
 from ml.utils.device.base import BaseDevice
 from ml.utils.large_models import init_empty_weights, meta_to_empty_func
 from ml.utils.logging import configure_logging
 from ml.utils.timer import Timer
+from omegaconf import MISSING
+from torch import Tensor, nn
 
 logger = logging.getLogger(__name__)
 
 RawImage = Union[PIL.Image.Image, Tensor, np.ndarray]
 
 PretrainedBlipKey = Literal[
     # ViT-B models
```

### Comparing `ml-pretrained-0.0.8/pretrained/clip.py` & `ml-pretrained-0.0.9/pretrained/clip.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,20 +45,19 @@
 from typing import Any, Callable, Literal, cast, get_args, overload
 
 import numpy as np
 import PIL.Image
 import torch
 import torch.nn.functional as F
 import torchvision
-from torch import Tensor, nn
-
 from ml.utils.checkpoint import ensure_downloaded
 from ml.utils.device.auto import AutoDevice
 from ml.utils.device.base import BaseDevice
 from ml.utils.logging import configure_logging
+from torch import Tensor, nn
 
 logger = logging.getLogger(__name__)
 
 URL_PREFIX = "https://openaipublic.azureedge.net/clip/models"
 
 PretrainedClipSize = Literal[
     "RN50",
```

### Comparing `ml-pretrained-0.0.8/pretrained/hubert.py` & `ml-pretrained-0.0.9/pretrained/hubert.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,29 +18,29 @@
 
 - ``"base"`` - 12 layers, 768 hidden size, 12 attention heads.
 - ``"large"`` - 24 layers, 1024 hidden size, 16 attention heads.
 - ``"extra_large"`` - 48 layers, 1280 hidden size, 16 attention heads.
 """
 
 import argparse
-import functools
 from dataclasses import dataclass
+from pathlib import Path
 from typing import Literal, cast, get_args
 
 import numpy as np
 import torch
 import torch.nn.functional as F
-from torch import Tensor, nn
-
 from ml.models.activations import ActivationType, get_activation
+from ml.utils.audio import Reader, read_audio
 from ml.utils.checkpoint import ensure_downloaded
 from ml.utils.device.auto import AutoDevice
 from ml.utils.device.base import BaseDevice
 from ml.utils.logging import configure_logging
 from ml.utils.timer import Timer
+from torch import Tensor, nn
 
 PretrainedHubertSize = Literal["base", "large", "extra_large"]
 
 
 @dataclass
 class HubertConfig:
     vocab_size: int
@@ -67,37 +67,23 @@
     pre_normalize: bool
 
     @property
     def num_feat_extract_layers(self) -> int:
         return len(self.conv_dim)
 
 
-class _MaskBuilder:
-    def __init__(self, device: torch.device, dtype: torch.dtype) -> None:
-        self.mask = self._get_mask_impl(device, dtype, 1)
-
-    def __call__(self, tsz: int) -> Tensor:
-        if self.mask.shape[0] < tsz:
-            self.mask = self._get_mask_impl(self.mask.device, self.mask.dtype, tsz)
-        return self.mask[:tsz, :tsz]
-
-    @staticmethod
-    def _get_mask_impl(device: torch.device, dtype: torch.dtype, tsz: int) -> Tensor:
-        mask = torch.full((1, 1, tsz, tsz), float("-inf"), device=device, dtype=dtype)
-        mask = torch.triu(mask, diagonal=1)
-        return mask
-
-    @functools.lru_cache()
-    @staticmethod
-    def get(device: torch.device, dtype: torch.dtype) -> "_MaskBuilder":
-        return _MaskBuilder(device, dtype)
-
-
-def get_mask(device: torch.device, dtype: torch.dtype, tsz: int) -> Tensor:
-    return _MaskBuilder.get(device, dtype)(tsz)
+def normalize_output_layer(output_layer: int | float | None, num_layers: int) -> int | None:
+    if output_layer is not None:
+        if isinstance(output_layer, float):
+            output_layer = round(output_layer * num_layers)
+        if output_layer < 0:
+            output_layer += num_layers
+        if not (0 <= output_layer < num_layers):
+            raise ValueError(f"output_layer={output_layer} is outside the range of available layers")
+    return output_layer
 
 
 class HubertSamePadLayer(nn.Module):
     def __init__(self, num_conv_pos_embeddings: int) -> None:
         super().__init__()
 
         self.num_pad_remove = 1 if num_conv_pos_embeddings % 2 == 0 else 0
@@ -207,15 +193,15 @@
         self.dropout = nn.Dropout(config.hidden_dropout)
         self.layer_norm = nn.LayerNorm(config.hidden_size, eps=config.layer_norm_eps)
         self.feed_forward = HubertFeedForward(config)
         self.final_layer_norm = nn.LayerNorm(config.hidden_size, eps=config.layer_norm_eps)
 
     def forward(self, hidden_states: Tensor, causal: bool = False) -> Tensor:
         attn_residual = hidden_states
-        hidden_states = self.attention(hidden_states, causal=causal)
+        hidden_states = self.attention.forward(hidden_states, causal=causal)
         hidden_states = self.dropout(hidden_states)
         hidden_states = attn_residual + hidden_states
 
         hidden_states = self.layer_norm(hidden_states)
         hidden_states = hidden_states + self.feed_forward(hidden_states)
         hidden_states = self.final_layer_norm(hidden_states)
 
@@ -225,28 +211,28 @@
 class HubertEncoder(nn.Module):
     def __init__(self, config: HubertConfig) -> None:
         super().__init__()
 
         self.pos_conv_embed = HubertPositionalConvEmbedding(config)
         self.layer_norm = nn.LayerNorm(config.hidden_size, eps=config.layer_norm_eps)
         self.dropout = nn.Dropout(config.hidden_dropout)
-        self.layers = nn.ModuleList([HubertEncoderLayer(config) for _ in range(config.num_hidden_layers)])
+        layers = nn.ModuleList([HubertEncoderLayer(config) for _ in range(config.num_hidden_layers)])
+        self.layers = cast(list[HubertEncoderLayer], layers)
         self.gradient_checkpointing = False
 
-    def forward(self, hidden_states: Tensor, causal: bool = False, output_layer: int | None = None) -> Tensor:
-        position_embeddings = self.pos_conv_embed(hidden_states)
+    def forward(self, hidden_states: Tensor, causal: bool = False, output_layer: int | float | None = None) -> Tensor:
+        position_embeddings = self.pos_conv_embed.forward(hidden_states)
         hidden_states = hidden_states + position_embeddings
         hidden_states = self.layer_norm(hidden_states)
         hidden_states = self.dropout(hidden_states)
-
+        output_layer = normalize_output_layer(output_layer, len(self.layers))
         for i, layer in enumerate(self.layers):
-            hidden_states = layer(hidden_states, causal=causal)
+            hidden_states = layer.forward(hidden_states, causal=causal)
             if output_layer is not None and i == output_layer:
                 break
-
         return hidden_states
 
 
 class HubertGroupNormConvLayer(nn.Module):
     def __init__(self, config: HubertConfig, layer_id: int = 0) -> None:
         super().__init__()
 
@@ -377,37 +363,38 @@
         self.layer_norm = nn.LayerNorm(config.hidden_size, eps=config.layer_norm_eps)
         self.feed_forward = HubertFeedForward(config)
         self.final_layer_norm = nn.LayerNorm(config.hidden_size, eps=config.layer_norm_eps)
 
     def forward(self, hidden_states: Tensor, causal: bool = False) -> Tensor:
         attn_residual = hidden_states
         hidden_states = self.layer_norm(hidden_states)
-        hidden_states = self.attention(hidden_states, causal=causal)
+        hidden_states = self.attention.forward(hidden_states, causal=causal)
         hidden_states = self.dropout(hidden_states)
         hidden_states = attn_residual + hidden_states
-        hidden_states = hidden_states + self.feed_forward(self.final_layer_norm(hidden_states))
+        hidden_states = hidden_states + self.feed_forward.forward(self.final_layer_norm(hidden_states))
         return hidden_states
 
 
 class HubertEncoderStableLayerNorm(nn.Module):
     def __init__(self, config: HubertConfig) -> None:
         super().__init__()
 
         self.pos_conv_embed = HubertPositionalConvEmbedding(config)
         self.layer_norm = nn.LayerNorm(config.hidden_size, eps=config.layer_norm_eps)
         self.dropout = nn.Dropout(config.hidden_dropout)
         layers = [HubertEncoderLayerStableLayerNorm(config) for _ in range(config.num_hidden_layers)]
-        self.layers = nn.ModuleList(layers)
+        self.layers = cast(list[HubertEncoderLayerStableLayerNorm], nn.ModuleList(layers))
 
-    def forward(self, hidden_states: Tensor, causal: bool = False, output_layer: int | None = None) -> Tensor:
+    def forward(self, hidden_states: Tensor, causal: bool = False, output_layer: int | float | None = None) -> Tensor:
         position_embeddings = self.pos_conv_embed(hidden_states)
         hidden_states = hidden_states + position_embeddings
         hidden_states = self.dropout(hidden_states)
+        output_layer = normalize_output_layer(output_layer, len(self.layers))
         for i, layer in enumerate(self.layers):
-            hidden_states = layer(hidden_states, causal=causal)
+            hidden_states = layer.forward(hidden_states, causal=causal)
             if output_layer is not None and i == output_layer:
                 break
         hidden_states = self.layer_norm(hidden_states)
         return hidden_states
 
 
 class Hubert(nn.Module):
@@ -420,19 +407,24 @@
         self.conv_stride = config.conv_stride
         self.pre_normalize = config.pre_normalize
 
         self.feature_extractor = HubertFeatureEncoder(config)
         self.feature_projection = HubertFeatureProjection(config)
         self.encoder = HubertEncoderStableLayerNorm(config) if config.do_stable_layer_norm else HubertEncoder(config)
 
-    def forward(self, input_values: Tensor | None, causal: bool = False, output_layer: int | None = None) -> Tensor:
+    def forward(
+        self,
+        input_values: Tensor | None,
+        causal: bool = False,
+        output_layer: int | float | None = None,
+    ) -> Tensor:
         extract_features = self.feature_extractor(input_values)
         extract_features = extract_features.transpose(1, 2)
         hidden_states = self.feature_projection(extract_features)
-        hidden_states = self.encoder(hidden_states, causal=causal, output_layer=output_layer)
+        hidden_states = self.encoder.forward(hidden_states, causal=causal, output_layer=output_layer)
         return hidden_states
 
     def predictor(self, *, device: BaseDevice | None = None) -> "HubertPredictor":
         return HubertPredictor(self, device=device)
 
 
 class HubertPredictor:
@@ -448,48 +440,62 @@
                 device returned by AutoDevice.detect_device().
         """
         super().__init__()
 
         self.device = AutoDevice.detect_device() if device is None else device
         self.model = hubert_model.eval()
         self.device.module_to(self.model)
+        self.sample_rate = 16_000  # True for all HuBERT models.
 
-    def predict(self, waveform: np.ndarray | Tensor, output_layer: int | None = None, causal: bool = False) -> Tensor:
+    def predict(
+        self,
+        waveform: np.ndarray | Tensor,
+        output_layer: int | float | None = None,
+        causal: bool = False,
+    ) -> Tensor:
         """Gets the hidden states for the given waveform.
 
         Args:
             waveform: The waveform to get hidden states for, with shape (B, T)
             output_layer: The layer to get hidden states from. If `None`, will
-                return the hidden states from the last layer.
+                return the hidden states from the last layer. If an `int`, will
+                return the hidden states from that layer. If a `float`, will
+                return the hidden states from the layer at that percentage of
+                the model. For example, `0.5` will return the hidden states
+                from the middle layer. Negative values will wrap around.
             causal: If set, use a causal attention mask.
 
         Returns:
             The hidden states for the given waveform, with shape (B, T, D)
         """
         waveform = self.device.tensor_to(waveform)
         return self.model.forward(waveform, causal=causal, output_layer=output_layer)
 
     def predict_in_chunks(
         self,
         waveform: Tensor | np.ndarray,
-        chunk_size: int,
-        output_layer: int | None = None,
+        chunk_size: int = 16_000 * 10,
+        output_layer: int | float | None = None,
         causal: bool = False,
     ) -> Tensor:
         """Gets the hidden states for the given waveform, in chunks.
 
         This is useful for processing very long waveforms, as it allows you to
         process the waveform in chunks, rather than loading the entire waveform
         into memory at once.
 
         Args:
             waveform: The waveform to get hidden states for, with shape (B, T)
-            chunk_size: The size of each chunk to process.
+            chunk_size: The size of each chunk to process, in frames.
             output_layer: The layer to get hidden states from. If `None`, will
-                return the hidden states from the last layer.
+                return the hidden states from the last layer. If an `int`, will
+                return the hidden states from that layer. If a `float`, will
+                return the hidden states from the layer at that percentage of
+                the model. For example, `0.5` will return the hidden states
+                from the middle layer. Negative values will wrap around.
             causal: If set, use a causal attention mask.
 
         Returns:
             The hidden states for the given waveform, with shape (B, T, D)
         """
         with torch.inference_mode():
             x = self.device.tensor_to(waveform)  # Loads entire waveform into device memory.
@@ -497,20 +503,65 @@
             if self.model.pre_normalize:
                 x = F.layer_norm(x, x.shape)
             x = x.view(1, -1)
 
             feat = []
             for start in range(0, x.size(1), chunk_size):
                 x_chunk = x[:, start : start + chunk_size]
-                get_mask(x_chunk.device, x_chunk.dtype, x_chunk.shape[1]) if self.causal else None
                 feat_chunk = self.model.forward(x_chunk, causal=causal, output_layer=output_layer)
                 feat.append(feat_chunk)
 
         return torch.cat(feat, 1).squeeze(0)
 
+    def predict_file(
+        self,
+        path: str | Path,
+        chunk_length_sec: float = 10.0,
+        output_layer: int | float | None = None,
+        causal: bool = False,
+        *,
+        reader: Reader = "av",
+    ) -> Tensor:
+        """Gets the hidden states for the given audio file, in chunks.
+
+        Args:
+            path: The path to the audio file to process.
+            chunk_length_sec: The length of each chunk to process, in seconds.
+            output_layer: The layer to get hidden states from. If `None`, will
+                return the hidden states from the last layer. If an `int`, will
+                return the hidden states from that layer. If a `float`, will
+                return the hidden states from the layer at that percentage of
+                the model. For example, `0.5` will return the hidden states
+                from the middle layer. Negative values will wrap around.
+            causal: If set, use a causal attention mask.
+            reader: The reader to use for reading the audio file.
+
+        Returns:
+            The hidden states for the given waveform, with shape (B, T, D)
+        """
+        chunk_length = round(chunk_length_sec * self.sample_rate)
+        with torch.inference_mode():
+            feat = []
+            for waveform_chunk in read_audio(
+                path,
+                chunk_length=chunk_length,
+                sampling_rate=self.sample_rate,
+                reader=reader,
+            ):
+                assert waveform_chunk.shape[0] == 1, "Expected mono-channel audio."
+                x = self.device.tensor_to(torch.from_numpy(waveform_chunk[0]))
+                if self.model.pre_normalize:
+                    x = F.layer_norm(x, x.shape)
+                x = x.view(1, -1)
+
+                feat_chunk = self.model.forward(x, causal=causal, output_layer=output_layer)
+                feat.append(feat_chunk)
+
+        return torch.cat(feat, 1).squeeze(0)
+
 
 EXCLUDE_KEYS = {"masked_spec_embed", ".weight", ".bias"}
 
 
 def _load_pretrained_hubert(
     size: PretrainedHubertSize,
     ckpt_url: str,
```

### Comparing `ml-pretrained-0.0.8/pretrained/llama.py` & `ml-pretrained-0.0.9/pretrained/llama.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,28 +35,27 @@
 import logging
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Iterator, Literal, get_args
 
 import torch
 import torch.nn.functional as F
-from omegaconf import MISSING
-from torch import Tensor, nn
-
 from ml.core.config import conf_field
 from ml.core.env import get_model_dir
 from ml.models.lora import maybe_lora
 from ml.models.parallel import ColumnParallelLinear, ParallelEmbedding, RowParallelLinear
 from ml.utils.device.auto import AutoDevice
 from ml.utils.device.base import BaseDevice
 from ml.utils.large_models import init_empty_weights, meta_to_empty_func
 from ml.utils.logging import configure_logging
 from ml.utils.parallel import parallel_group_info
 from ml.utils.timer import Timer
 from ml.utils.torch_distributed import MultiprocessConfig, launch_subprocesses
+from omegaconf import MISSING
+from torch import Tensor, nn
 
 logger = logging.getLogger(__name__)
 
 PretrainedLlamaKey = Literal["7B", "13B", "30B", "65B"]
 
 
 @dataclass
```

### Comparing `ml-pretrained-0.0.8/pretrained/rwkv.py` & `ml-pretrained-0.0.9/pretrained/rwkv.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,40 +18,45 @@
 
 Using the tokenizer requires installing the ``tokenizers`` library:
 
 .. code-block:: bash
 
     pip install tokenizers
 
+Additionally, using the training mode CUDA kernel requires installing ``triton``:
+
+.. code-block:: bash
+
+    pip install
+
 The choices for the model key are:
 
 - ``"169m"``
 - ``"430m"``
 - ``"1.5b"``
 - ``"3b"``
 - ``"7b"``
 - ``"14b"``
 """
 
 import argparse
 import logging
 from dataclasses import dataclass
-from typing import Any, Iterator, Literal, Sequence, get_args
+from typing import Any, Callable, Iterator, Literal, Sequence, get_args
 
 import torch
 import torch.nn.functional as F
-from torch import Tensor, nn
-
 from ml.models.lora import maybe_lora
 from ml.utils.checkpoint import ensure_downloaded
 from ml.utils.device.auto import AutoDevice
 from ml.utils.device.base import BaseDevice
 from ml.utils.large_models import init_empty_weights, meta_to_empty_func
 from ml.utils.logging import configure_logging
 from ml.utils.timer import Timer
+from torch import Tensor, nn
 
 logger = logging.getLogger(__name__)
 
 PretrainedRwkvKey = Literal["169m", "430m", "1.5b", "3b", "7b", "14b"]
 
 AttentionState = tuple[Tensor, Tensor, Tensor]
 FeedForwardState = Tensor
@@ -104,160 +109,140 @@
         num_layers=40,
     ),
 }
 
 TOKENIZER_URL = "https://raw.githubusercontent.com/BlinkDL/ChatRWKV/main/20B_tokenizer.json"
 
 
-def get_mask(tsz: int, device: torch.device | None = None, dtype: torch.dtype | None = None) -> Tensor:
-    """Returns the forward mask, used for training.
-
-    Args:
-        tsz: The number of timesteps in the mask
-        device: The mask device
-        dtype: The mask dtype
-
-    Returns:
-        The forward mask, with shape (T, T)
-    """
-    mask = torch.empty(tsz, tsz, device=device, dtype=dtype)
-    mask.fill_(float("-inf"))
-    # mask.triu_(1)
-    mask.tril_(-1)
-    return mask
-
-
-def run_wkv(
-    tsz: int,
+def _wkv_vanilla(
     w: Tensor,
     u: Tensor,
     k: Tensor,
     v: Tensor,
-    last_num: Tensor,
-    last_den: Tensor,
-    mask: Tensor | None = None,
+    num: Tensor,
+    den: Tensor,
 ) -> tuple[Tensor, Tensor, Tensor]:
     """Runs the core WKV computation.
 
-    Args;
-        tsz: The number of timesteps
+    Args:
         w: The decay tensor, with shape (D)
         u: The output multiplier tensor, with shape (D)
         k: The K tensor, with shape (B, T, D)
         v: The V tensor, with shape (B, T, D)
-        last_num: The last numerator, with shape (B, 1, D)
-        last_den: The last denominator, with shape (B, 1, D)
-        mask: The attention mask, with shape (T, T)
+        num: The last numerator, with shape (B, 1, D)
+        den: The last denominator, with shape (B, 1, D)
 
     Returns:
         The WKV tensor, with shape (B, T, D), and the next numerator and
-        denominator tensors, each with shape (B, T, D)
+        denominator tensors, each with shape (B, 1, D)
     """
     assert w.dim() == u.dim() == 1
-    assert mask is None or mask.dim() == 2
-    assert k.dim() == v.dim() == last_num.dim() == last_den.dim() == 3
+    assert k.dim() == v.dim() == num.dim() == den.dim() == 3
+
+    _, tsz, _ = k.shape
+
+    w = -torch.exp(w)  # (D)
+    ew = torch.exp(w)  # (D)
+
+    outs = []
+
+    for t in range(tsz):
+        kt, vt = k[:, t : t + 1], v[:, t : t + 1]  # (B, 1, D), (B, 1, D)
+        ek = torch.exp(kt)  # (B, 1, D)
+        euk = torch.exp(u + kt)  # (B, 1, D)
+        out = (num + euk * vt) / (den + euk)  # (B, 1, D)
+        num = ew * num + ek * vt  # (B, 1, D)
+        den = ew * den + ek  # (B, 1, D)
+        outs.append(out)
 
-    t = torch.arange(tsz + 1, device=w.device)[None, :, None]
-    wt = t[:, None, :-1, :] - t[:, :-1, None, :]
-    w = -torch.exp(w)
-    tw = w * t[:, 1:]
-    twt = w * wt
-    ktw = twt + k[:, :, None]
-    if mask is not None:
-        ktw = ktw + mask[None, :tsz, :tsz, None]
-
-    etw, ektw = torch.exp(tw), torch.exp(ktw)
-    num = etw * last_num + (ektw * v[:, :, None]).sum(1)
-    den = etw * last_den + ektw.sum(1)
+    return torch.cat(outs, 1), num, den
 
-    last_num = torch.cat((last_num, num[..., :-1, :]), dim=-2)
-    last_den = torch.cat((last_den, den[..., :-1, :]), dim=-2)
 
-    out = (last_num + torch.exp(u + k) * v) / (last_den + torch.exp(u + k))
+def get_wkv_fn() -> Callable[[Tensor, Tensor, Tensor, Tensor, Tensor, Tensor], tuple[Tensor, Tensor, Tensor]]:
+    """Returns the WKV function to use.
 
-    return out, num, den
+    The function takes six tensors as input, and returns three tensors as
+    output. The input tensors are ``w``, ``u``, ``k``, ``v``, ``num``, and
+    ``den``, and the output tensors are ``out``, ``num``, and ``den``.
+
+    Returns:
+        The WKV function to use.
+    """
+    if torch.cuda.is_available():
+        from pretrained.triton.rwkv_kernel import triton_wkv
+
+        return triton_wkv
+
+    return _wkv_vanilla
 
 
 class Attention(nn.Module):
     init_x: Tensor
     init_num: Tensor
     init_den: Tensor
-    mask: Tensor
 
     def __init__(self, emb_dim: int, max_tsz: int = 1024, lora_rank: int | None = None) -> None:
         super().__init__()
 
         self.time_decay = nn.Parameter(torch.empty(emb_dim))
         self.time_first = nn.Parameter(torch.empty(emb_dim))
 
         self.time_mix_k = nn.Parameter(torch.empty(1, 1, emb_dim))
         self.time_mix_v = nn.Parameter(torch.empty(1, 1, emb_dim))
         self.time_mix_r = nn.Parameter(torch.empty(1, 1, emb_dim))
 
-        # Disables updating the time parameters if using LoRA.
-        if lora_rank is not None:
-            self.time_decay.requires_grad_(False)
-            self.time_first.requires_grad_(False)
-            self.time_mix_k.requires_grad_(False)
-            self.time_mix_v.requires_grad_(False)
-            self.time_mix_r.requires_grad_(False)
-
         self.key = maybe_lora(nn.Linear(emb_dim, emb_dim, bias=False), lora_rank)
         self.value = maybe_lora(nn.Linear(emb_dim, emb_dim, bias=False), lora_rank)
         self.receptance = maybe_lora(nn.Linear(emb_dim, emb_dim, bias=False), lora_rank)
         self.output = maybe_lora(nn.Linear(emb_dim, emb_dim, bias=False), lora_rank)
 
         self.register_buffer("init_x", torch.zeros(1, 1, emb_dim), persistent=False)
         self.register_buffer("init_num", torch.zeros(1, 1, emb_dim), persistent=False)
         self.register_buffer("init_den", torch.zeros(1, 1, emb_dim), persistent=False)
-        self.register_buffer("mask", get_mask(max_tsz), persistent=False)
+
+        self.wkv_fn = get_wkv_fn()
 
     def time_shift(self, last_x: Tensor, x: Tensor) -> Tensor:
         _, tsz, _ = x.shape
         if tsz > 1:
             last_x = torch.cat((last_x, x[..., :-1, :]), dim=-2)
         return last_x
 
-    def forward(self, x: Tensor, state: AttentionState) -> tuple[Tensor, AttentionState]:
-        bsz, tsz, _ = x.shape
+    def forward(self, x: Tensor, state: AttentionState | None) -> tuple[Tensor, AttentionState]:
+        bsz, _, _ = x.shape
 
         if state is None:
             last_x = self.init_x.repeat(bsz, 1, 1)
-            last_num = self.init_num.repeat(bsz, 1, 1)
-            last_den = self.init_den.repeat(bsz, 1, 1)
+            num = self.init_num.repeat(bsz, 1, 1)
+            den = self.init_den.repeat(bsz, 1, 1)
         else:
-            last_x, last_num, last_den = state
+            last_x, num, den = state
         last_x = self.time_shift(last_x, x)
 
         k = self.key(x * self.time_mix_k + last_x * (1 - self.time_mix_k))
         v = self.value(x * self.time_mix_v + last_x * (1 - self.time_mix_v))
         r = self.receptance(x * self.time_mix_r + last_x * (1 - self.time_mix_r))
         sr = torch.sigmoid(r)
 
         w, u = self.time_decay, self.time_first
-        wkv, num, den = run_wkv(tsz, w, u, k, v, last_num, last_den, self.mask)
+        wkv, num, den = self.wkv_fn(w, u, k, v, num, den)
         rwkv = wkv * sr
 
-        return self.output(rwkv), (x[..., -1:, :], num[..., -1:, :], den[..., -1:, :])
+        return self.output(rwkv), (x[..., -1:, :], num, den)
 
 
 class FeedForward(nn.Module):
     init_state: Tensor
 
     def __init__(self, emb_dim: int, ffn_dim: int, lora_rank: int | None = None) -> None:
         super().__init__()
 
         self.time_mix_k = nn.Parameter(torch.empty(1, 1, emb_dim))
         self.time_mix_r = nn.Parameter(torch.empty(1, 1, emb_dim))
 
-        # Disables updating the time parameters if using LoRA.
-        if lora_rank is not None:
-            self.time_mix_k.requires_grad_(False)
-            self.time_mix_r.requires_grad_(False)
-
         self.key = maybe_lora(nn.Linear(emb_dim, ffn_dim, bias=False), lora_rank)
         self.receptance = maybe_lora(nn.Linear(emb_dim, emb_dim, bias=False), lora_rank)
         self.value = maybe_lora(nn.Linear(ffn_dim, emb_dim, bias=False), lora_rank)
 
         self.register_buffer("init_state", torch.zeros(1, 1, emb_dim), persistent=False)
 
     def time_shift(self, last_x: Tensor, x: Tensor) -> Tensor:
@@ -282,20 +267,14 @@
     def __init__(self, emb_dim: int, pre_norm: bool, lora_rank: int | None = None) -> None:
         super().__init__()
 
         self.ln0 = nn.LayerNorm(emb_dim) if pre_norm else None
         self.ln1 = nn.LayerNorm(emb_dim)
         self.ln2 = nn.LayerNorm(emb_dim)
 
-        if lora_rank is not None:
-            if self.ln0 is not None:
-                self.ln0.requires_grad_(False)
-            self.ln1.requires_grad_(False)
-            self.ln2.requires_grad_(False)
-
         self.att = Attention(emb_dim, lora_rank=lora_rank)
         self.ffn = FeedForward(emb_dim, emb_dim * 4, lora_rank=lora_rank)
 
     def forward(self, x: Tensor, state: State | None = None) -> tuple[Tensor, State]:
         if self.ln0 is not None:
             x = self.ln0(x)
         dx, att_state_out = self.att(self.ln1(x), None if state is None else state[0])
@@ -310,18 +289,14 @@
         super().__init__()
 
         self.emb = maybe_lora(nn.Embedding(num_tokens, emb_dim), lora_rank)
         self.blocks = nn.ModuleList([Block(emb_dim, i == 0, lora_rank=lora_rank) for i in range(num_layers)])
         self.ln_out = nn.LayerNorm(emb_dim)
         self.head = maybe_lora(nn.Linear(emb_dim, num_tokens, bias=False), lora_rank)
 
-        # Disables updating the layer norm parameters if using LoRA.
-        if lora_rank is not None:
-            self.ln_out.requires_grad_(False)
-
     def tensor_to(self, x: Tensor) -> Tensor:
         ref_tensor = self.head.weight
         if x.is_floating_point():
             return x.to(ref_tensor)
         return x.to(ref_tensor.device)
 
     def forward(
@@ -413,58 +388,73 @@
             yield token_str
             if any(e in token_str for e in end_strs_set):
                 break
             if i < max_len - 1:
                 probs, state = self.model(self.model.tensor_to(torch.tensor([[token]])), state)
 
 
-def pretrained_rwkv(key: PretrainedRwkvKey, *, device: BaseDevice | None = None, lora_rank: int | None = None) -> Rwkv:
+def pretrained_rwkv(
+    key: PretrainedRwkvKey,
+    *,
+    device: BaseDevice | None = None,
+    lora_rank: int | None = None,
+    empty: bool = False,
+) -> Rwkv:
     device = AutoDevice.detect_device() if device is None else device
     model_args = PRETRAINED_MODEL_SIZES[key]
+
+    with Timer("building model skeleton", spinner=True), init_empty_weights():
+        model = Rwkv(model_args.emb_dim, 50277, model_args.num_layers, lora_rank=lora_rank)
+
+    if empty:
+        model._apply(meta_to_empty_func(device.get_device(), torch.half))
+        model._apply(lambda x: device.tensor_to(x))
+        return model
+
     ckpt_path = ensure_downloaded(model_args.url, "rwkv", f"{key}.pth", sha256=model_args.sha256)
 
     with Timer("loading model checkpoint", spinner=True):
         ckpt = torch.load(ckpt_path, map_location="cpu")
 
-    with Timer("building model skeleton", spinner=True), init_empty_weights():
-        model = Rwkv(model_args.emb_dim, 50277, model_args.num_layers, lora_rank=lora_rank)
-
     # Build the transformer and loads the checkpoint.
     with Timer("loading state dict", spinner=True):
         model._apply(meta_to_empty_func(device.get_device(), torch.half))
         model.load_state_dict(ckpt)
+        model._apply(lambda x: device.tensor_to(x))
 
     return model
 
 
 def test_rwkv_adhoc() -> None:
     parser = argparse.ArgumentParser()
     parser.add_argument("size", type=str, choices=get_args(PretrainedRwkvKey))
     parser.add_argument("prompt", type=str, nargs="?")
     parser.add_argument("-t", "--tsz", type=int, default=128)
     parser.add_argument("-m", "--temperature", type=float, default=1.0)
     parser.add_argument("-p", "--top-p", type=float, default=0.85)
-    parser.add_argument("-e", "--end-tok", nargs="+", default=[])
+    parser.add_argument("-e", "--end-tok", type=str, nargs="+", default=[])
+    parser.add_argument("-s", "--sep", type=str, default="")
+    parser.add_argument("-y", "--empty", action="store_true")
     args = parser.parse_args()
 
     configure_logging()
 
-    model = pretrained_rwkv(args.size)
+    model = pretrained_rwkv(args.size, empty=args.empty)
     predictor = model.predictor()
 
     def generate_for_prompt(prompt: str) -> None:
         print(prompt, end="")
         for token in predictor.generate(
             prompt,
             max_len=args.tsz,
             temperature=args.temperature,
             top_p=args.top_p,
             end_strs=args.end_tok,
         ):
-            print(token, end="", flush=True)
+            print(token, end=args.sep, flush=True)
         print()
 
     if args.prompt:
         generate_for_prompt(args.prompt)
 
     else:
         prompt = input("Prompt: ")
```

### Comparing `ml-pretrained-0.0.8/pretrained/sam.py` & `ml-pretrained-0.0.9/pretrained/sam.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,21 +34,20 @@
 from pathlib import Path
 from typing import Any, Literal, Type, cast, get_args
 
 import numpy as np
 import PIL.Image
 import torch
 import torch.nn.functional as F
-from torch import Tensor, nn
-from torchvision.transforms.functional import resize, to_pil_image
-
 from ml.utils.checkpoint import ensure_downloaded
 from ml.utils.device.auto import AutoDevice
 from ml.utils.device.base import BaseDevice
 from ml.utils.logging import configure_logging
+from torch import Tensor, nn
+from torchvision.transforms.functional import resize, to_pil_image
 
 PretrainedSamSize = Literal["ViT-H", "ViT-L", "ViT-B"]
 
 ImageFormat = Literal["RGB", "BGR"]
 
 DEFAULT_PIXEL_MEAN = (123.675, 116.28, 103.53)
 DEFAULT_PIXEL_STD = (58.395, 57.12, 57.375)
```

### Comparing `ml-pretrained-0.0.8/pretrained/tacotron2.py` & `ml-pretrained-0.0.9/pretrained/tacotron2.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 .. highlight:: python
 .. code-block:: python
 
     from pretrained.tacotron2 import pretrained_tacotron2_tts
 
     tts = pretrained_tacotron2_tts()
-    audio = tts.generate("Hello, world!")
+    audio, states = tts.generate("Hello, world!")
     write_audio([audio])
 
 You can also interact with this model directly through the command line:
 
 .. highlight:: python
 .. code-block:: python
 
@@ -38,32 +38,32 @@
 import html
 import logging
 import re
 from dataclasses import dataclass
 from math import sqrt
 from numbers import Number
 from pathlib import Path
-from typing import Callable, NamedTuple, cast
+from typing import Callable, Iterable, NamedTuple, cast
 
 import numpy as np
 import torch
 import torch.nn.functional as F
-from torch import Tensor, nn
-from torch.nn.utils.rnn import pad_sequence
-
 from ml.core.config import conf_field
 from ml.models.base import BaseModel, BaseModelConfig
 from ml.models.lora import lora
 from ml.utils.audio import write_audio
 from ml.utils.checkpoint import ensure_downloaded
 from ml.utils.device.auto import AutoDevice
 from ml.utils.device.base import BaseDevice
 from ml.utils.large_models import init_empty_weights, meta_to_empty_func
 from ml.utils.logging import configure_logging
 from ml.utils.timer import Timer
+from torch import Tensor, nn
+from torch.nn.utils.rnn import pad_sequence
+
 from pretrained.vocoder import Vocoder, VocoderType, pretrained_vocoder
 
 logger = logging.getLogger(__name__)
 
 TACOTRON_CKPT_URL = "https://drive.google.com/open?id=1c5ZTuT7J08wLUoVZ2KkUs_VdZuJ86ZqA"
 
 
@@ -657,19 +657,20 @@
         return decoder_inputs
 
     def parse_decoder_outputs(
         self,
         mel_outputs: list[Tensor],
         gate_outputs: list[Tensor],
         alignments: list[Tensor],
-    ) -> tuple[Tensor, Tensor, Tensor]:
+        states: DecoderStates,
+    ) -> tuple[Tensor, Tensor, Tensor, DecoderStates]:
         alignments = torch.stack(alignments, dim=1)
         gate_outputs = torch.stack(gate_outputs, dim=1)
         mel_outputs = torch.stack(mel_outputs, dim=-1)
-        return mel_outputs, gate_outputs, alignments
+        return mel_outputs, gate_outputs, alignments, states
 
     def decode(self, decoder_input: Tensor, states: DecoderStates) -> tuple[Tensor, Tensor, Tensor, DecoderStates]:
         attn_h, attn_c, dec_h, dec_c, attn_weights, attn_weights_cum, attn_ctx, memory, processed_memory, mask = states
 
         cell_input = torch.cat((decoder_input, attn_ctx), -1)
         attn_h, attn_c = self.attention_rnn(cell_input, (attn_h, attn_c))
         attn_h = F.dropout(attn_h, self.p_attention_dropout, self.training)
@@ -698,15 +699,21 @@
             memory=memory,
             processed_memory=processed_memory,
             mask=mask,
         )
 
         return dec_out, gate_pred, attn_weights, new_states
 
-    def forward(self, memory: Tensor, dec_ins: Tensor, memory_lengths: Tensor) -> tuple[Tensor, Tensor, Tensor]:
+    def forward(
+        self,
+        memory: Tensor,
+        dec_ins: Tensor,
+        memory_lengths: Tensor,
+        states: DecoderStates | None = None,
+    ) -> tuple[Tensor, Tensor, Tensor, DecoderStates]:
         dec_in = self.get_go_frame(memory).unsqueeze(0)
         dec_ins = self.parse_decoder_inputs(dec_ins)
         dec_ins = torch.cat((dec_in, dec_ins), dim=0)
         prenet_ins = self.prenet(dec_ins)
 
         states = self.initialize_decoder_states(memory, mask=get_mask_from_lengths(memory_lengths))
 
@@ -716,19 +723,25 @@
         while len(mel_outs) < prenet_ins.size(0) - 1:
             prenet_in = prenet_ins[len(mel_outs)]
             mel_out, gate_out, attn_weights, states = self.decode(prenet_in, states)
             mel_outs += [mel_out.squeeze(1)]
             gate_outs += [gate_out.squeeze(1)]
             alignments += [attn_weights]
 
-        return self.parse_decoder_outputs(mel_outs, gate_outs, alignments)
+        return self.parse_decoder_outputs(mel_outs, gate_outs, alignments, states)
 
-    def infer(self, memory: Tensor, memory_lengths: Tensor) -> tuple[Tensor, Tensor, Tensor]:
+    def infer(
+        self,
+        memory: Tensor,
+        memory_lengths: Tensor,
+        states: DecoderStates | None = None,
+    ) -> tuple[Tensor, Tensor, Tensor, DecoderStates]:
         dec_in = self.get_go_frame(memory)
-        states = self.initialize_decoder_states(memory, mask=get_mask_from_lengths(memory_lengths))
+        if states is None:
+            states = self.initialize_decoder_states(memory, mask=get_mask_from_lengths(memory_lengths))
 
         mel_outs: list[Tensor] = []
         gate_outs: list[Tensor] = []
         alignments: list[Tensor] = []
         while True:
             prenet_in = self.prenet(dec_in)
             mel_out, gate_out, alignment, states = self.decode(prenet_in, states)
@@ -738,15 +751,15 @@
             if (torch.sigmoid(gate_out) > self.gate_threshold).all():
                 break
             elif len(mel_outs) == self.max_decoder_steps:
                 logger.warning("Warning! Reached max decoder steps %d", self.max_decoder_steps)
                 break
             dec_in = mel_out
 
-        return self.parse_decoder_outputs(mel_outs, gate_outs, alignments)
+        return self.parse_decoder_outputs(mel_outs, gate_outs, alignments, states)
 
 
 def window_sumsquare(
     window: str | float,
     n_frames: int,
     hop_length: int = 200,
     win_length: int = 800,
@@ -1006,42 +1019,51 @@
         self.embedding.weight.data.uniform_(-val, val)
         self.encoder = Encoder(config.encoder)
         self.decoder = Decoder(config.decoder)
         self.postnet = Postnet(config.postnet)
 
     def parse_output(
         self,
-        outputs: tuple[Tensor, Tensor, Tensor, Tensor],
+        outputs: tuple[Tensor, Tensor, Tensor, Tensor, DecoderStates],
         output_lengths: Tensor | None = None,
-    ) -> tuple[Tensor, Tensor, Tensor, Tensor]:
+    ) -> tuple[Tensor, Tensor, Tensor, Tensor, DecoderStates]:
         if self.mask_padding and output_lengths is not None:
             mask = ~get_mask_from_lengths(output_lengths)
             mask = mask.expand(self.n_mel_channels, mask.size(0), mask.size(1))
             mask = mask.permute(1, 0, 2)
 
             outputs[0].data.masked_fill_(mask, 0.0)
             outputs[1].data.masked_fill_(mask, 0.0)
             outputs[2].data.masked_fill_(mask[:, 0, :], 1e3)  # gate energies
 
         return outputs
 
-    def forward(self, inputs: tuple[Tensor, Tensor, Tensor, Tensor, Tensor]) -> tuple[Tensor, Tensor, Tensor, Tensor]:
+    def forward(
+        self,
+        inputs: tuple[Tensor, Tensor, Tensor, Tensor, Tensor],
+        states: DecoderStates | None = None,
+    ) -> tuple[Tensor, Tensor, Tensor, Tensor, DecoderStates]:
         text_inputs, text_lengths, mels, _, output_lengths = inputs
         embedded_inputs = self.embedding(text_inputs).transpose(1, 2)
         encoder_outputs = self.encoder(embedded_inputs, text_lengths)
-        mel_outputs, gate_outputs, alignments = self.decoder(encoder_outputs, mels, memory_lengths=text_lengths)
+        mel_outputs, gate_outputs, alignments, states = self.decoder(encoder_outputs, mels, text_lengths, states)
         mel_outputs_postnet = mel_outputs + self.postnet(mel_outputs)
-        return self.parse_output((mel_outputs, mel_outputs_postnet, gate_outputs, alignments), output_lengths)
+        return self.parse_output((mel_outputs, mel_outputs_postnet, gate_outputs, alignments, states), output_lengths)
 
-    def infer(self, inputs: Tensor, input_lengths: Tensor) -> tuple[Tensor, Tensor, Tensor, Tensor]:
+    def infer(
+        self,
+        inputs: Tensor,
+        input_lengths: Tensor,
+        states: DecoderStates | None = None,
+    ) -> tuple[Tensor, Tensor, Tensor, Tensor, DecoderStates]:
         embedded_inputs = self.embedding(inputs).transpose(1, 2)
         encoder_outputs = self.encoder.infer(embedded_inputs, input_lengths)
-        mel_outputs, gate_outputs, alignments = self.decoder.infer(encoder_outputs, input_lengths)
+        mel_outputs, gate_outputs, alignments, states = self.decoder.infer(encoder_outputs, input_lengths, states)
         mel_outputs_postnet = mel_outputs + self.postnet(mel_outputs)
-        return self.parse_output((mel_outputs, mel_outputs_postnet, gate_outputs, alignments))
+        return self.parse_output((mel_outputs, mel_outputs_postnet, gate_outputs, alignments, states))
 
 
 class Tokenizer:
     def __init__(self) -> None:
         super().__init__()
 
         pad = "_"
@@ -1203,37 +1225,47 @@
         self.vocoder.remove_weight_norm()
         self.sampling_rate = self.vocoder.sampling_rate
         self.device.module_to(self.tacotron)
         self.device.module_to(self.vocoder)
         self.tokenizer = Tokenizer()
 
     @torch.inference_mode()
-    def generate_mels(self, text: str | list[str], postnet: bool = True) -> Tensor:
+    def generate_mels(
+        self,
+        text: str | list[str],
+        postnet: bool = True,
+        states: DecoderStates | None = None,
+    ) -> tuple[Tensor, DecoderStates]:
         if isinstance(text, str):
             tokens = self.tokenizer(text).unsqueeze(0)
             token_lengths = tokens.new_full((1,), tokens.shape[1], dtype=torch.int32)
         else:
             token_list = [self.tokenizer(t) for t in text]
             tokens = pad_sequence(token_list, batch_first=True, padding_value=0)
             token_lengths = tokens.new_empty((tokens.shape[0],), dtype=torch.int32)
             for i, t in enumerate(token_list):
                 token_lengths[i] = t.shape[0]
         tokens, token_lengths = self.device.tensor_to(tokens), self.device.tensor_to(token_lengths)
-        mel_outputs, mel_outputs_postnet, _, _ = self.tacotron.infer(tokens, token_lengths)
-        return mel_outputs_postnet if postnet else mel_outputs
+        mel_outputs, mel_outputs_postnet, _, _, states = self.tacotron.infer(tokens, token_lengths, states)
+        return mel_outputs_postnet if postnet else mel_outputs, states
 
     @torch.inference_mode()
     def generate_wave(self, mels: Tensor) -> Tensor:
         return self.vocoder.infer(mels)
 
     @torch.inference_mode()
-    def generate(self, text: str | list[str], postnet: bool = True) -> Tensor:
-        mels = self.generate_mels(text, postnet=postnet)
+    def generate(
+        self,
+        text: str | list[str],
+        postnet: bool = True,
+        states: DecoderStates | None = None,
+    ) -> tuple[Tensor, DecoderStates]:
+        mels, states = self.generate_mels(text, postnet=postnet, states=states)
         audio = self.generate_wave(mels).squeeze(0)
-        return audio
+        return audio, states
 
 
 def pretrained_tacotron2_tts(vocoder_type: VocoderType = "hifigan", *, device: BaseDevice | None = None) -> TTS:
     tacotron = pretrained_tacotron2()
     vocoder = pretrained_vocoder(vocoder_type)
     tts = TTS(tacotron, vocoder, device=device)
     return tts
@@ -1245,39 +1277,44 @@
     parser = argparse.ArgumentParser()
     parser.add_argument("text", type=str, nargs="?", help="The text to synthesize.")
     parser.add_argument("-o", "--out-file", type=str, default=None, help="The output file.")
     args = parser.parse_args()
 
     tts = pretrained_tacotron2_tts()
 
-    def generate_for_text(text: str) -> None:
-        audio = tts.generate(text, postnet=True).cpu()
+    def generate_for_text(texts: Iterable[str]) -> None:
+        states: DecoderStates | None = None
 
-        if args.out_file is None:
-            try:
-                import sounddevice as sd
-            except ImportError:
-                raise ImportError("Please install sounddevice to play audio: pip install sounddevice")
+        for text in texts:
+            audio, states = tts.generate(text, postnet=True, states=states).cpu()
 
-            # Converts audio to the format that sounddevice is expecting.
-            audio = audio.numpy().T
+            if args.out_file is None:
+                try:
+                    import sounddevice as sd
+                except ImportError:
+                    raise ImportError("Please install sounddevice to play audio: pip install sounddevice")
 
-            sd.play(audio, tts.sampling_rate, blocking=True)
+                audio = audio.numpy().T
+                sd.play(audio, tts.sampling_rate, blocking=True)
 
-        else:
-            out_path = Path(args.out_file)
-            out_path.parent.mkdir(exist_ok=True)
-            write_audio(iter([audio]), out_path, tts.sampling_rate)
+            else:
+                out_path = Path(args.out_file)
+                out_path.parent.mkdir(exist_ok=True)
+                write_audio(iter([audio]), out_path, tts.sampling_rate)
 
     if args.text:
-        generate_for_text(args.text)
+        generate_for_text([args.text])
 
     else:
-        text = input("Text: ")
-        while text:
-            generate_for_text(text)
+
+        def gen_texts() -> Iterable[str]:
             text = input("Text: ")
+            while text:
+                yield text
+                text = input("Text: ")
+
+        generate_for_text(gen_texts())
 
 
 if __name__ == "__main__":
     # python -m pretrained.tacotron2
     test_tacotron_adhoc()
```

### Comparing `ml-pretrained-0.0.8/pretrained/vocoder/__init__.py` & `ml-pretrained-0.0.9/pretrained/vocoder/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.8/pretrained/vocoder/hifigan.py` & `ml-pretrained-0.0.9/pretrained/vocoder/hifigan.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,21 +11,20 @@
 """
 
 from dataclasses import dataclass
 from typing import TypeVar, cast
 
 import torch
 import torch.nn.functional as F
-from torch import Tensor, nn
-from torch.nn.utils import remove_weight_norm, weight_norm
-
 from ml.core.config import conf_field
 from ml.models.lora import SupportedModule as LoraModule, lora
 from ml.utils.checkpoint import ensure_downloaded
 from ml.utils.timer import Timer
+from torch import Tensor, nn
+from torch.nn.utils import remove_weight_norm, weight_norm
 
 HIFIGAN_CKPT_URL = "https://huggingface.co/jaketae/hifigan-lj-v1/resolve/main/pytorch_model.bin"
 
 
 @dataclass
 class HiFiGANConfig:
     resblock_kernel_sizes: list[int] = conf_field([3, 7, 11], help="Kernel sizes of ResBlock.")
```

### Comparing `ml-pretrained-0.0.8/pretrained/vocoder/waveglow.py` & `ml-pretrained-0.0.9/pretrained/vocoder/waveglow.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,18 @@
 """
 
 from dataclasses import dataclass
 from typing import cast
 
 import torch
 import torch.nn.functional as F
-from torch import Tensor, nn
-
 from ml.core.config import conf_field
-from ml.models.lora import lora
+from ml.models.lora import maybe_lora
 from ml.utils.checkpoint import ensure_downloaded, get_state_dict_prefix
+from torch import Tensor, nn
 
 WAVEGLOW_CKPT_FP16 = "https://api.ngc.nvidia.com/v2/models/nvidia/waveglow_ckpt_amp/versions/19.09.0/files/nvidia_waveglowpyt_fp16_20190427"
 WAVEGLOW_CKPT_FP32 = "https://api.ngc.nvidia.com/v2/models/nvidia/waveglow_ckpt_fp32/versions/19.09.0/files/nvidia_waveglowpyt_fp32_20190427"
 
 
 @torch.jit.script
 def fused_add_tanh_sigmoid_multiply(input_a: Tensor, input_b: Tensor, n_channels: int) -> Tensor:
@@ -116,47 +115,47 @@
         self.n_channels = config.n_channels
         self.in_layers = nn.ModuleList()
         self.res_skip_layers = nn.ModuleList()
         self.cond_layers = nn.ModuleList()
 
         start = nn.Conv1d(n_in_channels, config.n_channels, 1)
         start = nn.utils.weight_norm(start, name="weight")
-        self.start = start if lora_rank is None else lora(start, r=lora_rank)
+        self.start = maybe_lora(start, lora_rank)
 
         # Initializing last layer to 0 makes the affine coupling layers
         # do nothing at first.  This helps with training stability
         end = nn.Conv1d(config.n_channels, 2 * n_in_channels, 1)
         end.weight.data.zero_()
         if end.bias is not None:
             end.bias.data.zero_()
-        self.end = end if lora_rank is None else lora(end, r=lora_rank)
+        self.end = maybe_lora(end, lora_rank)
 
         for i in range(config.n_layers):
             dilation = 2**i
             padding = int((config.kernel_size * dilation - dilation) / 2)
             in_layer = nn.Conv1d(
                 config.n_channels, 2 * config.n_channels, config.kernel_size, dilation=dilation, padding=padding
             )
             in_layer = nn.utils.weight_norm(in_layer, name="weight")
-            in_layer = in_layer if lora_rank is None else lora(in_layer, r=lora_rank)
+            in_layer = maybe_lora(in_layer, lora_rank)
             self.in_layers.append(in_layer)
 
             cond_layer = nn.Conv1d(n_mel_channels, 2 * config.n_channels, 1)
             cond_layer = nn.utils.weight_norm(cond_layer, name="weight")
-            cond_layer = cond_layer if lora_rank is None else lora(cond_layer, r=lora_rank)
+            cond_layer = maybe_lora(cond_layer, lora_rank)
             self.cond_layers.append(cond_layer)
 
             # last one is not necessary
             if i < config.n_layers - 1:
                 res_skip_channels = 2 * config.n_channels
             else:
                 res_skip_channels = config.n_channels
             res_skip_layer = nn.Conv1d(config.n_channels, res_skip_channels, 1)
             res_skip_layer = nn.utils.weight_norm(res_skip_layer, name="weight")
-            res_skip_layer = res_skip_layer if lora_rank is None else lora(res_skip_layer, r=lora_rank)
+            res_skip_layer = maybe_lora(res_skip_layer, lora_rank)
             self.res_skip_layers.append(res_skip_layer)
 
     def forward(self, audio: Tensor, spect: Tensor) -> Tensor:
         audio = self.start(audio)
 
         output = 0
         layers = zip(self.in_layers, self.cond_layers, self.res_skip_layers)
```

### Comparing `ml-pretrained-0.0.8/pyproject.toml` & `ml-pretrained-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 line-length = 120
 target-version = ["py310"]
 include = '\.pyi?$'
 
 [tool.pytest.ini_options]
 
-timeout = 60
+timeout = 360
 addopts = "-rx -rf -x -q --full-trace"
 testpaths = ["tests"]
 
 markers = [
     "slow: Marks test as being slow",
     "has_gpu: Marks test as requiring a GPU to run",
     "multi_gpu: Marks tests as requiring multiple GPUs to run",
@@ -43,14 +43,15 @@
 
 module = [
     "av.*",
     "cv2.*",
     "ffmpeg.*",
     "matplotlib.*",
     "torchvision.*",
+    "triton.*",
 ]
 
 ignore_missing_imports = true
 
 [tool.isort]
 
 profile = "black"
@@ -73,13 +74,13 @@
 
 [tool.ruff.per-file-ignores]
 
 "__init__.py" = ["E402", "F401", "F403", "F811"]
 
 [tool.ruff.isort]
 
-known-first-party = ["ml", "pretrained", "tests"]
+known-first-party = ["pretrained", "tests"]
 combine-as-imports = true
 
 [tool.ruff.pydocstyle]
 
 convention = "google"
```

### Comparing `ml-pretrained-0.0.8/setup.py` & `ml-pretrained-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.8/tests/test_tacotron2.py` & `ml-pretrained-0.0.9/tests/test_tacotron2.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,10 +7,10 @@
 
 def test_training_matches_inference() -> None:
     model = pretrained_tacotron2(pretrained=False, prenet_dropout=False)
     model.eval()
 
     memory = torch.randn(1, 10, 512)
     memory_lengths = torch.tensor([10])
-    mels_infer, _, _ = model.decoder.infer(memory, memory_lengths)
-    mels_train, _, _ = model.decoder.forward(memory, mels_infer, memory_lengths)
+    mels_infer, _, _, _ = model.decoder.infer(memory, memory_lengths)
+    mels_train, _, _, _ = model.decoder.forward(memory, mels_infer, memory_lengths)
     assert torch.allclose(mels_infer, mels_train)
```

