# Comparing `tmp/vector_quantize_pytorch-1.6.7.tar.gz` & `tmp/vector_quantize_pytorch-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_quantize_pytorch-1.6.7.tar", last modified: Tue May 30 19:54:17 2023, max compression
+gzip compressed data, was "vector_quantize_pytorch-1.6.9.tar", last modified: Tue May 30 20:04:00 2023, max compression
```

## Comparing `vector_quantize_pytorch-1.6.7.tar` & `vector_quantize_pytorch-1.6.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:54:17.210549 vector_quantize_pytorch-1.6.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-30 19:54:05.000000 vector_quantize_pytorch-1.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-30 19:54:17.210549 vector_quantize_pytorch-1.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-05-30 19:54:05.000000 vector_quantize_pytorch-1.6.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 19:54:17.210549 vector_quantize_pytorch-1.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-30 19:54:05.000000 vector_quantize_pytorch-1.6.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:54:17.206549 vector_quantize_pytorch-1.6.7/vector_quantize_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-30 19:54:05.000000 vector_quantize_pytorch-1.6.7/vector_quantize_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-30 19:54:05.000000 vector_quantize_pytorch-1.6.7/vector_quantize_pytorch/random_projection_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-05-30 19:54:05.000000 vector_quantize_pytorch-1.6.7/vector_quantize_pytorch/residual_vq.py
--rw-r--r--   0 runner    (1001) docker     (123)    30174 2023-05-30 19:54:05.000000 vector_quantize_pytorch-1.6.7/vector_quantize_pytorch/vector_quantize_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:54:17.210549 vector_quantize_pytorch-1.6.7/vector_quantize_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-30 19:54:17.000000 vector_quantize_pytorch-1.6.7/vector_quantize_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-30 19:54:17.000000 vector_quantize_pytorch-1.6.7/vector_quantize_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 19:54:17.000000 vector_quantize_pytorch-1.6.7/vector_quantize_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 19:54:17.000000 vector_quantize_pytorch-1.6.7/vector_quantize_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-30 19:54:17.000000 vector_quantize_pytorch-1.6.7/vector_quantize_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:04:00.195877 vector_quantize_pytorch-1.6.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-30 20:03:47.000000 vector_quantize_pytorch-1.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-30 20:04:00.195877 vector_quantize_pytorch-1.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16116 2023-05-30 20:03:47.000000 vector_quantize_pytorch-1.6.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 20:04:00.195877 vector_quantize_pytorch-1.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-30 20:03:47.000000 vector_quantize_pytorch-1.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:04:00.195877 vector_quantize_pytorch-1.6.9/vector_quantize_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-30 20:03:47.000000 vector_quantize_pytorch-1.6.9/vector_quantize_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-30 20:03:47.000000 vector_quantize_pytorch-1.6.9/vector_quantize_pytorch/random_projection_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-05-30 20:03:47.000000 vector_quantize_pytorch-1.6.9/vector_quantize_pytorch/residual_vq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31994 2023-05-30 20:03:47.000000 vector_quantize_pytorch-1.6.9/vector_quantize_pytorch/vector_quantize_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:04:00.195877 vector_quantize_pytorch-1.6.9/vector_quantize_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-30 20:04:00.000000 vector_quantize_pytorch-1.6.9/vector_quantize_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-30 20:04:00.000000 vector_quantize_pytorch-1.6.9/vector_quantize_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 20:04:00.000000 vector_quantize_pytorch-1.6.9/vector_quantize_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 20:04:00.000000 vector_quantize_pytorch-1.6.9/vector_quantize_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-30 20:04:00.000000 vector_quantize_pytorch-1.6.9/vector_quantize_pytorch.egg-info/top_level.txt
```

### Comparing `vector_quantize_pytorch-1.6.7/LICENSE` & `vector_quantize_pytorch-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.6.7/PKG-INFO` & `vector_quantize_pytorch-1.6.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_quantize_pytorch
-Version: 1.6.7
+Version: 1.6.9
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vector_quantize_pytorch-1.6.7/README.md` & `vector_quantize_pytorch-1.6.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -178,14 +178,36 @@
     threshold_ema_dead_code = 2  # should actively replace any codes that have an exponential moving average cluster size less than 2
 )
 
 x = torch.randn(1, 1024, 256)
 quantized, indices, commit_loss = vq(x)
 ```
 
+### Orthogonal regularization loss
+
+VQ-VAE / VQ-GAN is quickly gaining popularity. A <a href="https://arxiv.org/abs/2112.00384">recent paper</a> proposes that when using vector quantization on images, enforcing the codebook to be orthogonal leads to translation equivariance of the discretized codes, leading to large improvements in downstream text to image generation tasks.
+
+You can use this feature by simply setting the `orthogonal_reg_weight` to be greater than `0`, in which case the orthogonal regularization will be added to the auxiliary loss outputted by the module.
+
+```python
+import torch
+from vector_quantize_pytorch import VectorQuantize
+vq = VectorQuantize(
+    dim = 256,
+    codebook_size = 256,
+    accept_image_fmap = True,                   # set this true to be able to pass in an image feature map
+    orthogonal_reg_weight = 10,                 # in paper, they recommended a value of 10
+    orthogonal_reg_max_codes = 128,             # this would randomly sample from the codebook for the orthogonal regularization loss, for limiting memory usage
+    orthogonal_reg_active_codes_only = False    # set this to True if you have a very large codebook, and would only like to enforce the loss on the activated codes per batch
+)
+img_fmap = torch.randn(1, 256, 32, 32)
+quantized, indices, loss = vq(img_fmap) # (1, 256, 32, 32), (1, 32, 32), (1,)
+# loss now contains the orthogonal regularization loss with the weight as assigned
+```
+
 ### Multi-headed VQ
 
 There has been a number of papers that proposes variants of discrete latent representations with a multi-headed approach (multiple codes per feature). I have decided to offer one variant where the same codebook is used to vector quantize across the input dimension `head` times.
 
 You can also use a more proven approach (memcodes) from <a href="https://github.com/lucidrains/nwt-pytorch">NWT paper</a>
 
 ```python
@@ -395,7 +417,18 @@
     title   = {Einops: Clear and Reliable Tensor Manipulations with Einstein-like Notation},
     author  = {Alex Rogozhnikov},
     booktitle = {International Conference on Learning Representations},
     year    = {2022},
     url     = {https://openreview.net/forum?id=oapKSVM2bcj}
 }
 ```
+
+```bibtex
+@misc{shin2021translationequivariant,
+    title   = {Translation-equivariant Image Quantizer for Bi-directional Image-Text Generation},
+    author  = {Woncheol Shin and Gyubok Lee and Jiyoung Lee and Joonseok Lee and Edward Choi},
+    year    = {2021},
+    eprint  = {2112.00384},
+    archivePrefix = {arXiv},
+    primaryClass = {cs.CV}
+}
+```
```

#### html2text {}

```diff
@@ -71,78 +71,95 @@
 codes Finally, the SoundStream paper has a scheme where they replace codes that
 have hits below a certain threshold with randomly selected vector from the
 current batch. You can set this threshold with `threshold_ema_dead_code`
 keyword. ```python import torch from vector_quantize_pytorch import
 VectorQuantize vq = VectorQuantize( dim = 256, codebook_size = 512,
 threshold_ema_dead_code = 2 # should actively replace any codes that have an
 exponential moving average cluster size less than 2 ) x = torch.randn(1, 1024,
-256) quantized, indices, commit_loss = vq(x) ``` ### Multi-headed VQ There has
-been a number of papers that proposes variants of discrete latent
-representations with a multi-headed approach (multiple codes per feature). I
-have decided to offer one variant where the same codebook is used to vector
-quantize across the input dimension `head` times. You can also use a more
-proven approach (memcodes) from NWT_paper ```python import torch from
+256) quantized, indices, commit_loss = vq(x) ``` ### Orthogonal regularization
+loss VQ-VAE / VQ-GAN is quickly gaining popularity. A recent_paper proposes
+that when using vector quantization on images, enforcing the codebook to be
+orthogonal leads to translation equivariance of the discretized codes, leading
+to large improvements in downstream text to image generation tasks. You can use
+this feature by simply setting the `orthogonal_reg_weight` to be greater than
+`0`, in which case the orthogonal regularization will be added to the auxiliary
+loss outputted by the module. ```python import torch from
 vector_quantize_pytorch import VectorQuantize vq = VectorQuantize( dim = 256,
-codebook_dim = 32, # a number of papers have shown smaller codebook dimension
-to be acceptable heads = 8, # number of heads to vector quantize, codebook
-shared across all heads separate_codebook_per_head = True, # whether to have a
-separate codebook per head. False would mean 1 shared codebook codebook_size =
-8196, accept_image_fmap = True ) img_fmap = torch.randn(1, 256, 32, 32)
-quantized, indices, loss = vq(img_fmap) # (1, 256, 32, 32), (1, 32, 32, 8),
-(1,) # indices shape - (batch, height, width, heads) ``` ### Random Projection
-Quantizer This_paper first proposed to use a random projection quantizer for
-masked speech modeling, where signals are projected with a randomly initialized
-matrix and then matched with a random initialized codebook. One therefore does
-not need to learn the quantizer. This technique was used by Google's Universal
-Speech_Model to achieve SOTA for speech-to-text modeling. USM further proposes
-to use multiple codebook, and the masked speech modeling with a multi-softmax
-objective. You can do this easily by setting `num_codebooks` to be greater than
-1 ```python import torch from vector_quantize_pytorch import
-RandomProjectionQuantizer quantizer = RandomProjectionQuantizer( dim = 512, #
-input dimensions num_codebooks = 16, # in USM, they used up to 16 for 5% gain
-codebook_dim = 256, # codebook dimension codebook_size = 1024 # codebook size )
-x = torch.randn(1, 1024, 512) indices = quantizer(x) # (1, 1024, 16) - (batch,
-seq, num_codebooks) ``` ### DDP This repository also supports synchronizing the
-codebooks in a distributed settings. Below should be a working script, and also
-shows which flag you need to enable for it to work as expected. ```python
-import torch from torch import nn from vector_quantize_pytorch import
-VectorQuantize # ddp related imports import os import torch.distributed as dist
-import torch.multiprocessing as mp from torch.nn.parallel import
-DistributedDataParallel as DDP def setup(rank, world_size): os.environ
-['MASTER_ADDR'] = 'localhost' os.environ['MASTER_PORT'] = '12355'
-dist.init_process_group("gloo", rank=rank, world_size=world_size) def cleanup
-(): dist.destroy_process_group() def start(rank, world_size): setup(rank,
-world_size) net = nn.Sequential( nn.Conv2d(256, 256, 1), VectorQuantize( dim =
-256, codebook_size = 1024, accept_image_fmap = True, sync_codebook = True #
-this needs to be set to True ) ).cuda(rank) ddp_mp_model = DDP(net, device_ids
-= [rank]) img_fmap = torch.randn(1, 256, 32, 32).cuda(rank) quantized, indices,
-loss = ddp_mp_model(img_fmap) cleanup() if __name__ == '__main__': world_size =
-torch.cuda.device_count() assert world_size >= 2, f"requires at least 2 GPUs to
-run, but got {n_gpus}" mp.spawn(start, args=(world_size,), nprocs=world_size,
-join=True) ``` ## Todo - [x] allow for multi-headed codebooks - [x] support
-masking - [x] make sure affine param works with (`sync_affine_param` set to
-`True`) ## Citations ```bibtex @misc{oord2018neural, title = {Neural Discrete
-Representation Learning}, author = {Aaron van den Oord and Oriol Vinyals and
-Koray Kavukcuoglu}, year = {2018}, eprint = {1711.00937}, archivePrefix =
-{arXiv}, primaryClass = {cs.LG} } ``` ```bibtex @misc{zeghidour2021soundstream,
-title = {SoundStream: An End-to-End Neural Audio Codec}, author = {Neil
-Zeghidour and Alejandro Luebs and Ahmed Omran and Jan Skoglund and Marco
-Tagliasacchi}, year = {2021}, eprint = {2107.03312}, archivePrefix = {arXiv},
-primaryClass = {cs.SD} } ``` ```bibtex @inproceedings
-{anonymous2022vectorquantized, title = {Vector-quantized Image Modeling with
-Improved {VQGAN}}, author = {Anonymous}, booktitle = {Submitted to The Tenth
-International Conference on Learning Representations }, year = {2022}, url =
-{https://openreview.net/forum?id=pfNyExj7z2}, note = {under review} } ```
-```bibtex @unknown{unknown, author = {Lee, Doyup and Kim, Chiheon and Kim,
-Saehoon and Cho, Minsu and Han, Wook-Shin}, year = {2022}, month = {03}, title
-= {Autoregressive Image Generation using Residual Quantization} } ``` ```bibtex
-@article{Defossez2022HighFN, title = {High Fidelity Neural Audio Compression},
-author = {Alexandre D'efossez and Jade Copet and Gabriel Synnaeve and Yossi
-Adi}, journal = {ArXiv}, year = {2022}, volume = {abs/2210.13438} } ```
-```bibtex @inproceedings{Chiu2022SelfsupervisedLW, title = {Self-supervised
+codebook_size = 256, accept_image_fmap = True, # set this true to be able to
+pass in an image feature map orthogonal_reg_weight = 10, # in paper, they
+recommended a value of 10 orthogonal_reg_max_codes = 128, # this would randomly
+sample from the codebook for the orthogonal regularization loss, for limiting
+memory usage orthogonal_reg_active_codes_only = False # set this to True if you
+have a very large codebook, and would only like to enforce the loss on the
+activated codes per batch ) img_fmap = torch.randn(1, 256, 32, 32) quantized,
+indices, loss = vq(img_fmap) # (1, 256, 32, 32), (1, 32, 32), (1,) # loss now
+contains the orthogonal regularization loss with the weight as assigned ``` ###
+Multi-headed VQ There has been a number of papers that proposes variants of
+discrete latent representations with a multi-headed approach (multiple codes
+per feature). I have decided to offer one variant where the same codebook is
+used to vector quantize across the input dimension `head` times. You can also
+use a more proven approach (memcodes) from NWT_paper ```python import torch
+from vector_quantize_pytorch import VectorQuantize vq = VectorQuantize( dim =
+256, codebook_dim = 32, # a number of papers have shown smaller codebook
+dimension to be acceptable heads = 8, # number of heads to vector quantize,
+codebook shared across all heads separate_codebook_per_head = True, # whether
+to have a separate codebook per head. False would mean 1 shared codebook
+codebook_size = 8196, accept_image_fmap = True ) img_fmap = torch.randn(1, 256,
+32, 32) quantized, indices, loss = vq(img_fmap) # (1, 256, 32, 32), (1, 32, 32,
+8), (1,) # indices shape - (batch, height, width, heads) ``` ### Random
+Projection Quantizer This_paper first proposed to use a random projection
+quantizer for masked speech modeling, where signals are projected with a
+randomly initialized matrix and then matched with a random initialized
+codebook. One therefore does not need to learn the quantizer. This technique
+was used by Google's Universal_Speech_Model to achieve SOTA for speech-to-text
+modeling. USM further proposes to use multiple codebook, and the masked speech
+modeling with a multi-softmax objective. You can do this easily by setting
+`num_codebooks` to be greater than 1 ```python import torch from
+vector_quantize_pytorch import RandomProjectionQuantizer quantizer =
+RandomProjectionQuantizer( dim = 512, # input dimensions num_codebooks = 16, #
+in USM, they used up to 16 for 5% gain codebook_dim = 256, # codebook dimension
+codebook_size = 1024 # codebook size ) x = torch.randn(1, 1024, 512) indices =
+quantizer(x) # (1, 1024, 16) - (batch, seq, num_codebooks) ``` ### DDP This
+repository also supports synchronizing the codebooks in a distributed settings.
+Below should be a working script, and also shows which flag you need to enable
+for it to work as expected. ```python import torch from torch import nn from
+vector_quantize_pytorch import VectorQuantize # ddp related imports import os
+import torch.distributed as dist import torch.multiprocessing as mp from
+torch.nn.parallel import DistributedDataParallel as DDP def setup(rank,
+world_size): os.environ['MASTER_ADDR'] = 'localhost' os.environ['MASTER_PORT']
+= '12355' dist.init_process_group("gloo", rank=rank, world_size=world_size) def
+cleanup(): dist.destroy_process_group() def start(rank, world_size): setup
+(rank, world_size) net = nn.Sequential( nn.Conv2d(256, 256, 1), VectorQuantize
+( dim = 256, codebook_size = 1024, accept_image_fmap = True, sync_codebook =
+True # this needs to be set to True ) ).cuda(rank) ddp_mp_model = DDP(net,
+device_ids = [rank]) img_fmap = torch.randn(1, 256, 32, 32).cuda(rank)
+quantized, indices, loss = ddp_mp_model(img_fmap) cleanup() if __name__ ==
+'__main__': world_size = torch.cuda.device_count() assert world_size >= 2,
+f"requires at least 2 GPUs to run, but got {n_gpus}" mp.spawn(start, args=
+(world_size,), nprocs=world_size, join=True) ``` ## Todo - [x] allow for multi-
+headed codebooks - [x] support masking - [x] make sure affine param works with
+(`sync_affine_param` set to `True`) ## Citations ```bibtex @misc
+{oord2018neural, title = {Neural Discrete Representation Learning}, author =
+{Aaron van den Oord and Oriol Vinyals and Koray Kavukcuoglu}, year = {2018},
+eprint = {1711.00937}, archivePrefix = {arXiv}, primaryClass = {cs.LG} } ```
+```bibtex @misc{zeghidour2021soundstream, title = {SoundStream: An End-to-End
+Neural Audio Codec}, author = {Neil Zeghidour and Alejandro Luebs and Ahmed
+Omran and Jan Skoglund and Marco Tagliasacchi}, year = {2021}, eprint =
+{2107.03312}, archivePrefix = {arXiv}, primaryClass = {cs.SD} } ``` ```bibtex
+@inproceedings{anonymous2022vectorquantized, title = {Vector-quantized Image
+Modeling with Improved {VQGAN}}, author = {Anonymous}, booktitle = {Submitted
+to The Tenth International Conference on Learning Representations }, year =
+{2022}, url = {https://openreview.net/forum?id=pfNyExj7z2}, note = {under
+review} } ``` ```bibtex @unknown{unknown, author = {Lee, Doyup and Kim, Chiheon
+and Kim, Saehoon and Cho, Minsu and Han, Wook-Shin}, year = {2022}, month =
+{03}, title = {Autoregressive Image Generation using Residual Quantization} }
+``` ```bibtex @article{Defossez2022HighFN, title = {High Fidelity Neural Audio
+Compression}, author = {Alexandre D'efossez and Jade Copet and Gabriel Synnaeve
+and Yossi Adi}, journal = {ArXiv}, year = {2022}, volume = {abs/2210.13438} }
+``` ```bibtex @inproceedings{Chiu2022SelfsupervisedLW, title = {Self-supervised
 Learning with Random-projection Quantizer for Speech Recognition}, author =
 {Chung-Cheng Chiu and James Qin and Yu Zhang and Jiahui Yu and Yonghui Wu},
 booktitle = {International Conference on Machine Learning}, year = {2022} } ```
 ```bibtex @inproceedings{Zhang2023GoogleUS, title = {Google USM: Scaling
 Automatic Speech Recognition Beyond 100 Languages}, author = {Yu Zhang and Wei
 Han and James Qin and Yongqiang Wang and Ankur Bapna and Zhehuai Chen and
 Nanxin Chen and Bo Li and Vera Axelrod and Gary Wang and Zhong Meng and Ke Hu
@@ -166,8 +183,12 @@
 Challenges in Vector Quantized Networks}, author = {Huh, Minyoung and Cheung,
 Brian and Agrawal, Pulkit and Isola, Phillip}, booktitle = {International
 Conference on Machine Learning}, year = {2023}, organization = {PMLR} } ```
 ```bibtex @inproceedings{rogozhnikov2022einops, title = {Einops: Clear and
 Reliable Tensor Manipulations with Einstein-like Notation}, author = {Alex
 Rogozhnikov}, booktitle = {International Conference on Learning
 Representations}, year = {2022}, url = {https://openreview.net/
-forum?id=oapKSVM2bcj} } ```
+forum?id=oapKSVM2bcj} } ``` ```bibtex @misc{shin2021translationequivariant,
+title = {Translation-equivariant Image Quantizer for Bi-directional Image-Text
+Generation}, author = {Woncheol Shin and Gyubok Lee and Jiyoung Lee and
+Joonseok Lee and Edward Choi}, year = {2021}, eprint = {2112.00384},
+archivePrefix = {arXiv}, primaryClass = {cs.CV} } ```
```

### Comparing `vector_quantize_pytorch-1.6.7/setup.py` & `vector_quantize_pytorch-1.6.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'vector_quantize_pytorch',
   packages = find_packages(),
-  version = '1.6.7',
+  version = '1.6.9',
   license='MIT',
   description = 'Vector Quantization - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/vector-quantizer-pytorch',
   keywords = [
```

### Comparing `vector_quantize_pytorch-1.6.7/vector_quantize_pytorch/random_projection_quantizer.py` & `vector_quantize_pytorch-1.6.9/vector_quantize_pytorch/random_projection_quantizer.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.6.7/vector_quantize_pytorch/residual_vq.py` & `vector_quantize_pytorch-1.6.9/vector_quantize_pytorch/residual_vq.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.6.7/vector_quantize_pytorch/vector_quantize_pytorch.py` & `vector_quantize_pytorch-1.6.9/vector_quantize_pytorch/vector_quantize_pytorch.py`

 * *Files 4% similar despite different names*

```diff
@@ -207,14 +207,23 @@
 
 def batched_embedding(indices, embeds):
     batch, dim = indices.shape[1], embeds.shape[-1]
     indices = repeat(indices, 'h b n -> h b n d', d = dim)
     embeds = repeat(embeds, 'h c d -> h b c d', b = batch)
     return embeds.gather(2, indices)
 
+# regularization losses
+
+def orthogonal_loss_fn(t):
+    # eq (2) from https://arxiv.org/abs/2112.00384
+    h, n = t.shape[:2]
+    normed_codes = l2norm(t)
+    cosine_sim = einsum('h i d, h j d -> h i j', normed_codes, normed_codes)
+    return (cosine_sim ** 2).sum() / (h * n ** 2) - (1 / n)
+
 # distance types
 
 class EuclideanCodebook(nn.Module):
     def __init__(
         self,
         dim,
         codebook_size,
@@ -626,14 +635,17 @@
         sync_kmeans = True,
         use_cosine_sim = False,
         threshold_ema_dead_code = 0,
         channel_last = True,
         accept_image_fmap = False,
         commitment_weight = 1.,
         commitment_use_cross_entropy_loss = False,
+        orthogonal_reg_weight = 0.,
+        orthogonal_reg_active_codes_only = False,
+        orthogonal_reg_max_codes = None,
         stochastic_sample_codes = False,
         sample_codebook_temp = 1.,
         straight_through = False,
         reinmax = False,  # using reinmax for improved straight-through, assuming straight through helps at all
         sync_codebook = False,
         sync_affine_param = False,
         ema_update = True,
@@ -655,14 +667,20 @@
         self.project_in = nn.Linear(dim, codebook_input_dim) if requires_projection else nn.Identity()
         self.project_out = nn.Linear(codebook_input_dim, dim) if requires_projection else nn.Identity()
 
         self.eps = eps
         self.commitment_weight = commitment_weight
         self.commitment_use_cross_entropy_loss = commitment_use_cross_entropy_loss # whether to use cross entropy loss to codebook as commitment loss
 
+        has_codebook_orthogonal_loss = orthogonal_reg_weight > 0
+        self.has_codebook_orthogonal_loss = has_codebook_orthogonal_loss
+        self.orthogonal_reg_weight = orthogonal_reg_weight
+        self.orthogonal_reg_active_codes_only = orthogonal_reg_active_codes_only
+        self.orthogonal_reg_max_codes = orthogonal_reg_max_codes
+
         assert not (ema_update and learnable_codebook), 'learnable codebook not compatible with EMA update'
 
         assert 0 <= sync_update_v <= 1.
         assert not (sync_update_v > 0. and not learnable_codebook), 'learnable codebook must be turned on'
 
         self.sync_update_v = sync_update_v
 
@@ -682,15 +700,15 @@
             kmeans_init = kmeans_init,
             kmeans_iters = kmeans_iters,
             sync_kmeans = sync_kmeans,
             decay = decay,
             eps = eps,
             threshold_ema_dead_code = threshold_ema_dead_code,
             use_ddp = sync_codebook,
-            learnable_codebook = learnable_codebook,
+            learnable_codebook = has_codebook_orthogonal_loss or learnable_codebook,
             sample_codebook_temp = sample_codebook_temp,
             gumbel_sample = gumbel_sample_fn,
             ema_update = ema_update
         )
 
         if affine_param:
             assert not use_cosine_sim
@@ -850,14 +868,33 @@
 
                         commit_loss = commit_loss[mask].mean()
                     else:
                         commit_loss = F.mse_loss(detached_quantize, x)
 
                 loss = loss + commit_loss * self.commitment_weight
 
+            if self.has_codebook_orthogonal_loss:
+                codebook = self._codebook.embed
+
+                # only calculate orthogonal loss for the activated codes for this batch
+
+                if self.orthogonal_reg_active_codes_only:
+                    assert not (is_multiheaded and self.separate_codebook_per_head), 'orthogonal regularization for only active codes not compatible with multi-headed with separate codebooks yet'
+                    unique_code_ids = torch.unique(embed_ind)
+                    codebook = codebook[:, unique_code_ids]
+
+                num_codes = codebook.shape[-2]
+
+                if exists(self.orthogonal_reg_max_codes) and num_codes > self.orthogonal_reg_max_codes:
+                    rand_ids = torch.randperm(num_codes, device = device)[:self.orthogonal_reg_max_codes]
+                    codebook = codebook[:, rand_ids]
+
+                orthogonal_reg_loss = orthogonal_loss_fn(codebook)
+                loss = loss + orthogonal_reg_loss * self.orthogonal_reg_weight
+
         # handle multi-headed quantized embeddings
 
         if is_multiheaded:
             if self.separate_codebook_per_head:
                 quantize = rearrange(quantize, 'h b n d -> b n (h d)', h = heads)
             else:
                 quantize = rearrange(quantize, '1 (b h) n d -> b n (h d)', h = heads)
```

### Comparing `vector_quantize_pytorch-1.6.7/vector_quantize_pytorch.egg-info/PKG-INFO` & `vector_quantize_pytorch-1.6.9/vector_quantize_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-quantize-pytorch
-Version: 1.6.7
+Version: 1.6.9
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

