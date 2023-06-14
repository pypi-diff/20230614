# Comparing `tmp/MEGABYTE-pytorch-0.1.4.tar.gz` & `tmp/MEGABYTE-pytorch-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MEGABYTE-pytorch-0.1.4.tar", last modified: Wed May 31 01:02:21 2023, max compression
+gzip compressed data, was "MEGABYTE-pytorch-0.1.6.tar", last modified: Wed Jun 14 16:51:33 2023, max compression
```

## Comparing `MEGABYTE-pytorch-0.1.4.tar` & `MEGABYTE-pytorch-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:02:21.510444 MEGABYTE-pytorch-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-31 01:02:10.000000 MEGABYTE-pytorch-0.1.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:02:21.510444 MEGABYTE-pytorch-0.1.4/MEGABYTE_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-31 01:02:10.000000 MEGABYTE-pytorch-0.1.4/MEGABYTE_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-05-31 01:02:10.000000 MEGABYTE-pytorch-0.1.4/MEGABYTE_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    13724 2023-05-31 01:02:10.000000 MEGABYTE-pytorch-0.1.4/MEGABYTE_pytorch/megabyte.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:02:21.510444 MEGABYTE-pytorch-0.1.4/MEGABYTE_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-31 01:02:21.000000 MEGABYTE-pytorch-0.1.4/MEGABYTE_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-31 01:02:21.000000 MEGABYTE-pytorch-0.1.4/MEGABYTE_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 01:02:21.000000 MEGABYTE-pytorch-0.1.4/MEGABYTE_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-31 01:02:21.000000 MEGABYTE-pytorch-0.1.4/MEGABYTE_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-31 01:02:21.000000 MEGABYTE-pytorch-0.1.4/MEGABYTE_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-31 01:02:21.510444 MEGABYTE-pytorch-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-05-31 01:02:10.000000 MEGABYTE-pytorch-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 01:02:21.510444 MEGABYTE-pytorch-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-31 01:02:10.000000 MEGABYTE-pytorch-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:51:33.110772 MEGABYTE-pytorch-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-14 16:51:17.000000 MEGABYTE-pytorch-0.1.6/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:51:33.110772 MEGABYTE-pytorch-0.1.6/MEGABYTE_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-14 16:51:17.000000 MEGABYTE-pytorch-0.1.6/MEGABYTE_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-06-14 16:51:17.000000 MEGABYTE-pytorch-0.1.6/MEGABYTE_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13855 2023-06-14 16:51:17.000000 MEGABYTE-pytorch-0.1.6/MEGABYTE_pytorch/megabyte.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:51:33.110772 MEGABYTE-pytorch-0.1.6/MEGABYTE_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-14 16:51:33.000000 MEGABYTE-pytorch-0.1.6/MEGABYTE_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-14 16:51:33.000000 MEGABYTE-pytorch-0.1.6/MEGABYTE_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 16:51:33.000000 MEGABYTE-pytorch-0.1.6/MEGABYTE_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-14 16:51:33.000000 MEGABYTE-pytorch-0.1.6/MEGABYTE_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-14 16:51:33.000000 MEGABYTE-pytorch-0.1.6/MEGABYTE_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-14 16:51:33.110772 MEGABYTE-pytorch-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-06-14 16:51:17.000000 MEGABYTE-pytorch-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 16:51:33.110772 MEGABYTE-pytorch-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-14 16:51:17.000000 MEGABYTE-pytorch-0.1.6/setup.py
```

### Comparing `MEGABYTE-pytorch-0.1.4/LICENSE` & `MEGABYTE-pytorch-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `MEGABYTE-pytorch-0.1.4/MEGABYTE_pytorch/attend.py` & `MEGABYTE-pytorch-0.1.6/MEGABYTE_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `MEGABYTE-pytorch-0.1.4/MEGABYTE_pytorch/megabyte.py` & `MEGABYTE-pytorch-0.1.6/MEGABYTE_pytorch/megabyte.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,15 +214,16 @@
         max_seq_len: Tuple,
         dim_head = 64,
         heads = 8,
         attn_dropout = 0.,
         ff_mult = 4,
         ff_dropout = 0.,
         pad_id = 0,
-        rel_pos_bias = True,
+        rel_pos_bias = False,
+        pos_emb = False,
         flash_attn = False
     ):
         super().__init__()
 
         # simplified configuration for each stage of the hierarchy
         # depth = (2, 2, 4) would translate to depth 2 at first stage, depth 2 second stage, depth 4 third
         # max_seq_len = (16, 8, 4) would translate to max sequence length of 16 at first stage, length of 8 at second stage, length of 4 for last
@@ -238,15 +239,15 @@
         coarsest_dim, *_, fine_dim = dim
 
         self.token_emb = nn.Embedding(num_tokens, fine_dim)
 
         self.max_seq_len = max_seq_len
 
         self.start_tokens = nn.ParameterList([nn.Parameter(torch.randn(h_dim)) for h_dim, seq_len in zip(dim, max_seq_len)])
-        self.pos_embs = nn.ModuleList([nn.Embedding(seq_len, h_dim) for h_dim, seq_len in zip(dim, max_seq_len)])
+        self.pos_embs = nn.ModuleList([nn.Embedding(seq_len, h_dim) for h_dim, seq_len in zip(dim, max_seq_len)]) if pos_emb else None
 
         self.patch_embedders = nn.ModuleList([nn.Sequential(
             Rearrange('... r d -> ... (r d)'),
             nn.LayerNorm(seq_len * dim_in),
             nn.Linear(seq_len * dim_in, dim_out),
             nn.LayerNorm(dim_out)
         ) for dim_in, dim_out, seq_len in zip(dim[1:], dim[:-1], max_seq_len[1:])])
@@ -347,23 +348,27 @@
 
         # get tokens for all hierarchical stages, reducing by appropriate dimensions
         # and adding the absolute positional embeddings
 
         tokens_at_stages = []
         reduced_tokens = tokens
 
-        for ind, pos_emb, patch_emb in zip(range(len(prec_dims)), reversed(self.pos_embs), reversed((*self.patch_embedders, None))):
+        pos_embs = default(self.pos_embs, (None,))
+
+        for ind, pos_emb, patch_emb in zip_longest(range(len(prec_dims)), reversed(pos_embs), reversed((*self.patch_embedders, None))):
             is_first = ind == 0
 
             if not is_first:
                 reduced_tokens = patch_emb(reduced_tokens)
 
-            positions = pos_emb(torch.arange(reduced_tokens.shape[-2], device = device))
-            tokens_with_position = reduced_tokens + positions
-            tokens_at_stages.insert(0, tokens_with_position)
+            if exists(pos_emb):
+                positions = pos_emb(torch.arange(reduced_tokens.shape[-2], device = device))
+                reduced_tokens = reduced_tokens + positions
+
+            tokens_at_stages.insert(0, reduced_tokens)
 
         # the un-pixelshuffled representations of the previous hierarchy, starts with None
 
         prev_stage_tokens_repr = None
 
         # spatial tokens is tokens with depth pos reduced along depth dimension + spatial positions
```

### Comparing `MEGABYTE-pytorch-0.1.4/MEGABYTE_pytorch.egg-info/PKG-INFO` & `MEGABYTE-pytorch-0.1.6/MEGABYTE_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MEGABYTE-pytorch
-Version: 0.1.4
+Version: 0.1.6
 Summary: MEGABYTE - Pytorch
 Home-page: https://github.com/lucidrains/MEGABYTE-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `MEGABYTE-pytorch-0.1.4/PKG-INFO` & `MEGABYTE-pytorch-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MEGABYTE-pytorch
-Version: 0.1.4
+Version: 0.1.6
 Summary: MEGABYTE - Pytorch
 Home-page: https://github.com/lucidrains/MEGABYTE-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `MEGABYTE-pytorch-0.1.4/README.md` & `MEGABYTE-pytorch-0.1.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -106,7 +106,17 @@
     year      = {2021},
     publisher = {Zenodo},
     version   = {0.01},
     doi       = {10.5281/zenodo.5196578},
     url       = {https://doi.org/10.5281/zenodo.5196578}
 }
 ```
+
+```bibtex
+@article{Kazemnejad2023TheIO,
+    title   = {The Impact of Positional Encoding on Length Generalization in Transformers},
+    author  = {Amirhossein Kazemnejad and Inkit Padhi and Karthikeyan Natesan Ramamurthy and Payel Das and Siva Reddy},
+    journal = {ArXiv},
+    year    = {2023},
+    volume  = {abs/2305.19466}
+}
+```
```

#### html2text {}

```diff
@@ -32,8 +32,12 @@
 booktitle = {Advances in Neural Information Processing Systems}, year = {2022}
 } ``` ```bibtex @misc{press2021ALiBi, title = {Train Short, Test Long:
 Attention with Linear Biases Enable Input Length Extrapolation}, author = {Ofir
 Press and Noah A. Smith and Mike Lewis}, year = {2021}, url = {https://ofir.io/
 train_short_test_long.pdf} } ``` ```bibtex @software{peng_bo_2021_5196578,
 author = {PENG Bo}, title = {BlinkDL/RWKV-LM: 0.01}, month = {aug}, year =
 {2021}, publisher = {Zenodo}, version = {0.01}, doi = {10.5281/zenodo.5196578},
-url = {https://doi.org/10.5281/zenodo.5196578} } ```
+url = {https://doi.org/10.5281/zenodo.5196578} } ``` ```bibtex @article
+{Kazemnejad2023TheIO, title = {The Impact of Positional Encoding on Length
+Generalization in Transformers}, author = {Amirhossein Kazemnejad and Inkit
+Padhi and Karthikeyan Natesan Ramamurthy and Payel Das and Siva Reddy}, journal
+= {ArXiv}, year = {2023}, volume = {abs/2305.19466} } ```
```

### Comparing `MEGABYTE-pytorch-0.1.4/setup.py` & `MEGABYTE-pytorch-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'MEGABYTE-pytorch',
   packages = find_packages(),
-  version = '0.1.4',
+  version = '0.1.6',
   license='MIT',
   description = 'MEGABYTE - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/MEGABYTE-pytorch',
   keywords = [
```

