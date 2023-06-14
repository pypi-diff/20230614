# Comparing `tmp/structured-pruning-adapters-0.5.2.tar.gz` & `tmp/structured-pruning-adapters-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structured-pruning-adapters-0.5.2.tar", last modified: Thu Nov 17 10:56:46 2022, max compression
+gzip compressed data, was "structured-pruning-adapters-0.6.0.tar", last modified: Wed Jun 14 09:13:58 2023, max compression
```

## Comparing `structured-pruning-adapters-0.5.2.tar` & `structured-pruning-adapters-0.6.0.tar`

### file list

```diff
@@ -1,19 +1,26 @@
-drwxr-xr-x   0 au478108 (794351465) 357318537        0 2022-11-17 10:56:46.985006 structured-pruning-adapters-0.5.2/
--rw-r--r--   0 au478108 (794351465) 357318537    11357 2022-06-15 08:39:30.000000 structured-pruning-adapters-0.5.2/LICENSE
--rw-r--r--   0 au478108 (794351465) 357318537     7053 2022-11-17 10:56:46.984453 structured-pruning-adapters-0.5.2/PKG-INFO
--rw-r--r--   0 au478108 (794351465) 357318537     5816 2022-11-17 10:54:09.000000 structured-pruning-adapters-0.5.2/README.md
--rw-r--r--   0 au478108 (794351465) 357318537       38 2022-11-17 10:56:46.985319 structured-pruning-adapters-0.5.2/setup.cfg
--rw-r--r--   0 au478108 (794351465) 357318537     2565 2022-11-17 10:35:57.000000 structured-pruning-adapters-0.5.2/setup.py
-drwxr-xr-x   0 au478108 (794351465) 357318537        0 2022-11-17 10:56:46.979929 structured-pruning-adapters-0.5.2/sp_adapters/
--rw-r--r--   0 au478108 (794351465) 357318537      320 2022-11-17 10:31:11.000000 structured-pruning-adapters-0.5.2/sp_adapters/__init__.py
--rw-r--r--   0 au478108 (794351465) 357318537      116 2022-06-15 13:38:30.000000 structured-pruning-adapters-0.5.2/sp_adapters/base.py
--rw-r--r--   0 au478108 (794351465) 357318537     1445 2022-11-17 10:31:11.000000 structured-pruning-adapters-0.5.2/sp_adapters/lora.py
--rw-r--r--   0 au478108 (794351465) 357318537     7525 2022-11-17 10:31:11.000000 structured-pruning-adapters-0.5.2/sp_adapters/splopa.py
--rw-r--r--   0 au478108 (794351465) 357318537    14139 2022-11-17 10:31:11.000000 structured-pruning-adapters-0.5.2/sp_adapters/splora.py
--rw-r--r--   0 au478108 (794351465) 357318537     2097 2022-09-28 12:45:21.000000 structured-pruning-adapters-0.5.2/sp_adapters/utils.py
-drwxr-xr-x   0 au478108 (794351465) 357318537        0 2022-11-17 10:56:46.983520 structured-pruning-adapters-0.5.2/structured_pruning_adapters.egg-info/
--rw-r--r--   0 au478108 (794351465) 357318537     7053 2022-11-17 10:56:46.000000 structured-pruning-adapters-0.5.2/structured_pruning_adapters.egg-info/PKG-INFO
--rw-r--r--   0 au478108 (794351465) 357318537      409 2022-11-17 10:56:46.000000 structured-pruning-adapters-0.5.2/structured_pruning_adapters.egg-info/SOURCES.txt
--rw-r--r--   0 au478108 (794351465) 357318537        1 2022-11-17 10:56:46.000000 structured-pruning-adapters-0.5.2/structured_pruning_adapters.egg-info/dependency_links.txt
--rw-r--r--   0 au478108 (794351465) 357318537      105 2022-11-17 10:56:46.000000 structured-pruning-adapters-0.5.2/structured_pruning_adapters.egg-info/requires.txt
--rw-r--r--   0 au478108 (794351465) 357318537       12 2022-11-17 10:56:46.000000 structured-pruning-adapters-0.5.2/structured_pruning_adapters.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:13:58.057026 structured-pruning-adapters-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 09:12:04.000000 structured-pruning-adapters-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-06-14 09:13:58.057026 structured-pruning-adapters-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-06-14 09:12:04.000000 structured-pruning-adapters-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 09:13:58.057026 structured-pruning-adapters-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-14 09:12:04.000000 structured-pruning-adapters-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:13:58.053026 structured-pruning-adapters-0.6.0/sp_adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-14 09:12:04.000000 structured-pruning-adapters-0.6.0/sp_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-14 09:12:04.000000 structured-pruning-adapters-0.6.0/sp_adapters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-14 09:12:04.000000 structured-pruning-adapters-0.6.0/sp_adapters/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-06-14 09:12:04.000000 structured-pruning-adapters-0.6.0/sp_adapters/splopa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31876 2023-06-14 09:12:04.000000 structured-pruning-adapters-0.6.0/sp_adapters/splora.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9805 2023-06-14 09:12:04.000000 structured-pruning-adapters-0.6.0/sp_adapters/torch_pruning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-14 09:12:04.000000 structured-pruning-adapters-0.6.0/sp_adapters/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:13:58.057026 structured-pruning-adapters-0.6.0/structured_pruning_adapters.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-06-14 09:13:57.000000 structured-pruning-adapters-0.6.0/structured_pruning_adapters.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-14 09:13:58.000000 structured-pruning-adapters-0.6.0/structured_pruning_adapters.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:13:57.000000 structured-pruning-adapters-0.6.0/structured_pruning_adapters.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-14 09:13:57.000000 structured-pruning-adapters-0.6.0/structured_pruning_adapters.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 09:13:57.000000 structured-pruning-adapters-0.6.0/structured_pruning_adapters.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:13:58.057026 structured-pruning-adapters-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-14 09:12:04.000000 structured-pruning-adapters-0.6.0/tests/test_lin_as_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-14 09:12:04.000000 structured-pruning-adapters-0.6.0/tests/test_splopa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15654 2023-06-14 09:12:04.000000 structured-pruning-adapters-0.6.0/tests/test_splora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-06-14 09:12:04.000000 structured-pruning-adapters-0.6.0/tests/test_torchpruning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-14 09:12:04.000000 structured-pruning-adapters-0.6.0/tests/test_utils.py
```

### Comparing `structured-pruning-adapters-0.5.2/LICENSE` & `structured-pruning-adapters-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.5.2/PKG-INFO` & `structured-pruning-adapters-0.6.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structured-pruning-adapters
-Version: 0.5.2
+Version: 0.6.0
 Summary: Structured Pruning Adapters for PyTorch
 Home-page: https://github.com/lukashedegaard/structured-pruning-adapters
 Author: Lukas Hedegaard
 Author-email: lukasxhedegaard@gmail.com
 License: UNKNOWN
 Keywords: deep learning,pytorch,AI,adapters,pruning,inference
 Platform: UNKNOWN
@@ -27,41 +27,41 @@
 Provides-Extra: build
 Provides-Extra: dev
 License-File: LICENSE
 
 # Structured Pruning Adapters for PyTorch
 
 <div align="left">
-  <!-- <a href="https://pypi.org/project/structured-pruning-adapters/">
+  <a href="https://pypi.org/project/structured-pruning-adapters/">
     <img src="https://img.shields.io/pypi/pyversions/structured-pruning-adapters" height="20" >
   </a>
   <a href="https://badge.fury.io/py/structured-pruning-adapters">
     <img src="https://badge.fury.io/py/structured-pruning-adapters.svg" height="20" >
-  </a> -->
+  </a>
   <!-- <a href="https://structured-pruning-adapters.readthedocs.io/en/latest/?badge=latest">
     <img src="https://readthedocs.org/projects/structured-pruning-adapters/badge/?version=latest" alt="Documentation Status" height="20"/>
   </a> -->
   <!-- <a href="https://pepy.tech/project/structured-pruning-adapters">
     <img src="https://pepy.tech/badge/structured-pruning-adapters" height="20">
   </a> -->
-  <!-- <a href="https://codecov.io/gh/LukasHedegaard/structured-pruning-adapters">
-    <img src="https://codecov.io/gh/LukasHedegaard/structured-pruning-adapters/branch/main/graph/badge.svg?token=????" height="20"/>
-  </a> -->
   <a href="https://opensource.org/licenses/Apache-2.0">
     <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg" height="20">
   </a>
-  <!-- <a href="https://arxiv.org/abs/2204.03418">
-    <img src="http://img.shields.io/badge/paper-arxiv.2204.03418-B31B1B.svg" height="20" >
-  </a> -->
+  <a href="https://arxiv.org/abs/2211.10155">
+    <img src="http://img.shields.io/badge/paper-arxiv.2211.10155-B31B1B.svg" height="20" >
+  </a>
   <a href="https://github.com/psf/black">
     <img src="https://img.shields.io/badge/code%20style-black-000000.svg" height="20">
   </a>
-  <!-- <a href="https://www.codefactor.io/repository/github/lukashedegaard/structured-pruning-adapters/overview/main">
-    <img src="https://www.codefactor.io/repository/github/lukashedegaard/structured-pruning-adapters/badge/main" alt="CodeFactor" height="20" />
-  </a> -->
+    <a href="https://codecov.io/github/LukasHedegaard/structured-pruning-adapters" > 
+    <img src="https://codecov.io/github/LukasHedegaard/structured-pruning-adapters/branch/main/graph/badge.svg?token=WHBSM01TRN"/> 
+  </a>
+  <a href="https://www.codefactor.io/repository/github/lukashedegaard/structured-pruning-adapters">
+    <img src="https://www.codefactor.io/repository/github/lukashedegaard/structured-pruning-adapters/badge" alt="CodeFactor" />
+  </a>
 </div>
 
 ```bash
 pip install structured-pruning-adapters
 ```
 ## A happy mariage 👰‍♀️🤵‍♂️
 
@@ -96,29 +96,33 @@
 
     reg_lin = Linear(256, 512, bias=True)
     spa_lin = SPLoRA(reg_lin, rank=32)
 
     # Or replace all applicable layers in a network
     spa_net = SPLoRA(reg_net, rank=32)
     ```
-3. Employ any Structured Pruning method, e.g [this](https://github.com/huggingface/block_movement_pruning) or [that](https://github.com/seulkiyeom/LRP_Pruning).
+3. Employ any Structured Pruning method. We conducted extensive experimens with multiple [channel-pruning](https://github.com/lukashedegaard/channel-spa-experiments) and [block-pruning](https://github.com/lukashedegaard/block-spa-experiments) methods.
 
 4. Get pruned SP Adapter weights:
     ```python3
-    # Specify mask
-    spa_lin.configure_parameter_read(
+    # Specify mask - learned via your choice of Structured Pruning method
+    in_features_mask=torch.tensor([1, 0, ..., 1], dtype=torch.bool)
+    out_features_mask=torch.tensor([0, 1, ..., 1], dtype=torch.bool)
+
+    # Read parameters
+    params = sp_adapters.splora.parameters(
         adapter_weights_only=True,
         in_features_mask=torch.tensor([1, 0, ..., 1], dtype=torch.bool)
         out_features_mask=torch.tensor([0, 1, ..., 1], dtype=torch.bool),
-    )   # 👆 masks are learned via your choice of Structured Pruning method
-
-    # Read parameters as usual
-    spa_lin.parameters()
-    spa_lin.named_parameters()
-    spa_lin.state_dict()
+    )   
+    named_parameters = sp_adapters.splora.named_parameters(
+        adapter_weights_only=True,
+        in_features_mask=torch.tensor([1, 0, ..., 1], dtype=torch.bool)
+        out_features_mask=torch.tensor([0, 1, ..., 1], dtype=torch.bool),
+    )
     ```
 
 ### Demo
 See also [notebooks/demo.ipynb](notebooks/demo.ipynb) for a hands-on demo.
 
 ### Structured Pruning Low-Rank Adapter (SPLoRA) for _Channel Pruning_ 
 ```python3
@@ -127,32 +131,32 @@
 <div align="center">
 <img src="figures/SPLoRA.png" width="400">
 </div>
 Adds a low-rank bottle-neck projection in projection in parallel with the main weights projection.
 
 <br/>
 
-### Structured Pruning Low-rank PHM Adapter (SPLoPA) for _Block Pruning_
+### Structured Pruning Low-rank PHM Adapter (SPLoPA) for _Block Pruning_ (experimental)
 ```python3
 from sp_adapters import SPLoPA
 ```
 
 <div align="center">
 <img src="figures/SPLoPA.png" width="600">
 </div>
 
 Uses a variation on the Parameterized Hypercomplex Multiplication (PHM) layer [[paper](https://openreview.net/forum?id=rcQdycl0zyk)] with shared low-rank prototypes for block-sparse adaptation.
 
 ## Citation
 If you enjoy this work, please consider citing it
 ```bibtex
-@article{hedegaard2022cotrans,
+@article{hedegaard2022structured,
   title={Structured Pruning Adapters},
-  author={Lukas Hedegaard, Aman Alok, Juby Jose, Alexandros Iosifidis},
-  journal={preprint, arXiv:TBD},
+  author={Lukas Hedegaard and Aman Alok and Juby Jose and Alexandros Iosifidis},
+  journal={preprint, arXiv:2211.10155},
   year={2022}
 }
 ```
 
 ## Acknowledgement
 This work was done in conjunction with a research exchange at [Cactus Communications 🌵](https://cactusglobal.com).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: structured-pruning-adapters Version: 0.5.2 Summary:
+Metadata-Version: 2.1 Name: structured-pruning-adapters Version: 0.6.0 Summary:
 Structured Pruning Adapters for PyTorch Home-page: https://github.com/
 lukashedegaard/structured-pruning-adapters Author: Lukas Hedegaard Author-
 email: lukasxhedegaard@gmail.com License: UNKNOWN Keywords: deep
 learning,pytorch,AI,adapters,pruning,inference Platform: UNKNOWN Classifier:
 Environment :: Console Classifier: Natural Language :: English Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -12,16 +12,20 @@
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Description-Content-Type: text/markdown Provides-Extra: build
 Provides-Extra: dev License-File: LICENSE # Structured Pruning Adapters for
 PyTorch
-    [https://img.shields.io/badge/License-Apache%202.0-blue.svg]  [https://
-img.shields.io/badge/code%20style-black-000000.svg]
+[https://img.shields.io/pypi/pyversions/structured-pruning-adapters] [https://
+badge.fury.io/py/structured-pruning-adapters.svg]   [https://img.shields.io/
+badge/License-Apache%202.0-blue.svg] [http://img.shields.io/badge/paper-
+arxiv.2211.10155-B31B1B.svg] [https://img.shields.io/badge/code%20style-black-
+000000.svg] [https://codecov.io/github/LukasHedegaard/structured-pruning-
+adapters/branch/main/graph/badge.svg?token=WHBSM01TRN] [CodeFactor]
 ```bash pip install structured-pruning-adapters ``` ## A happy mariage
 ð°ââï¸ð¤µââï¸ __Pruning__ is an effective method for reducing the
 size of neural networks. Besides reducing the parameter count, the process
 _can_ accelerate inference as well. CPUs can handle sparse weights just fine,
 but GPUs need structured weights for an acceleration to happen. A structured
 approach to pruning i.e., removing network channels [[paper](https://
 www.sciencedirect.com/science/article/pii/S0031320321000868)] or blocks of
@@ -40,36 +44,40 @@
 parameters (binary pruning mask + masked adapter weights) ð - â
 Accelerated network inference ðð¨ ## How to use this library Use in
 conjunction with any Structured Pruning technique. 1. Install the library:
 ```bash pip install structured-pruning-adapters ``` 2. Replace Linear and Conv
 layers with an SP Adapter: ```python3 from torch.nn import Linear from
 sp_adapter import SPLoRA reg_lin = Linear(256, 512, bias=True) spa_lin = SPLoRA
 (reg_lin, rank=32) # Or replace all applicable layers in a network spa_net =
-SPLoRA(reg_net, rank=32) ``` 3. Employ any Structured Pruning method, e.g
-[this](https://github.com/huggingface/block_movement_pruning) or [that](https:/
-/github.com/seulkiyeom/LRP_Pruning). 4. Get pruned SP Adapter weights:
-```python3 # Specify mask spa_lin.configure_parameter_read
+SPLoRA(reg_net, rank=32) ``` 3. Employ any Structured Pruning method. We
+conducted extensive experimens with multiple [channel-pruning](https://
+github.com/lukashedegaard/channel-spa-experiments) and [block-pruning](https://
+github.com/lukashedegaard/block-spa-experiments) methods. 4. Get pruned SP
+Adapter weights: ```python3 # Specify mask - learned via your choice of
+Structured Pruning method in_features_mask=torch.tensor([1, 0, ..., 1],
+dtype=torch.bool) out_features_mask=torch.tensor([0, 1, ..., 1],
+dtype=torch.bool) # Read parameters params = sp_adapters.splora.parameters
+( adapter_weights_only=True, in_features_mask=torch.tensor([1, 0, ..., 1],
+dtype=torch.bool) out_features_mask=torch.tensor([0, 1, ..., 1],
+dtype=torch.bool), ) named_parameters = sp_adapters.splora.named_parameters
 ( adapter_weights_only=True, in_features_mask=torch.tensor([1, 0, ..., 1],
 dtype=torch.bool) out_features_mask=torch.tensor([0, 1, ..., 1],
-dtype=torch.bool), ) # ð masks are learned via your choice of Structured
-Pruning method # Read parameters as usual spa_lin.parameters()
-spa_lin.named_parameters() spa_lin.state_dict() ``` ### Demo See also
-[notebooks/demo.ipynb](notebooks/demo.ipynb) for a hands-on demo. ###
-Structured Pruning Low-Rank Adapter (SPLoRA) for _Channel Pruning_ ```python3
-from sp_adapters import SPLoRA ```
+dtype=torch.bool), ) ``` ### Demo See also [notebooks/demo.ipynb](notebooks/
+demo.ipynb) for a hands-on demo. ### Structured Pruning Low-Rank Adapter
+(SPLoRA) for _Channel Pruning_ ```python3 from sp_adapters import SPLoRA ```
                              [figures/SPLoRA.png]
 Adds a low-rank bottle-neck projection in projection in parallel with the main
 weights projection.
 ### Structured Pruning Low-rank PHM Adapter (SPLoPA) for _Block Pruning_
-```python3 from sp_adapters import SPLoPA ```
+(experimental) ```python3 from sp_adapters import SPLoPA ```
                              [figures/SPLoPA.png]
 Uses a variation on the Parameterized Hypercomplex Multiplication (PHM) layer [
 [paper](https://openreview.net/forum?id=rcQdycl0zyk)] with shared low-rank
 prototypes for block-sparse adaptation. ## Citation If you enjoy this work,
-please consider citing it ```bibtex @article{hedegaard2022cotrans, title=
-{Structured Pruning Adapters}, author={Lukas Hedegaard, Aman Alok, Juby Jose,
-Alexandros Iosifidis}, journal={preprint, arXiv:TBD}, year={2022} } ``` ##
-Acknowledgement This work was done in conjunction with a research exchange at
-[Cactus Communications ðµ](https://cactusglobal.com). This work has received
-funding from the European Unionâs Horizon 2020 research and innovation
-programme under grant agreement No 871449 [(OpenDR) ðªðº](https://
-opendr.eu).
+please consider citing it ```bibtex @article{hedegaard2022structured, title=
+{Structured Pruning Adapters}, author={Lukas Hedegaard and Aman Alok and Juby
+Jose and Alexandros Iosifidis}, journal={preprint, arXiv:2211.10155}, year=
+{2022} } ``` ## Acknowledgement This work was done in conjunction with a
+research exchange at [Cactus Communications ðµ](https://cactusglobal.com).
+This work has received funding from the European Unionâs Horizon 2020
+research and innovation programme under grant agreement No 871449 [(OpenDR)
+ðªðº](https://opendr.eu).
```

### Comparing `structured-pruning-adapters-0.5.2/README.md` & `structured-pruning-adapters-0.6.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # Structured Pruning Adapters for PyTorch
 
 <div align="left">
-  <!-- <a href="https://pypi.org/project/structured-pruning-adapters/">
+  <a href="https://pypi.org/project/structured-pruning-adapters/">
     <img src="https://img.shields.io/pypi/pyversions/structured-pruning-adapters" height="20" >
   </a>
   <a href="https://badge.fury.io/py/structured-pruning-adapters">
     <img src="https://badge.fury.io/py/structured-pruning-adapters.svg" height="20" >
-  </a> -->
+  </a>
   <!-- <a href="https://structured-pruning-adapters.readthedocs.io/en/latest/?badge=latest">
     <img src="https://readthedocs.org/projects/structured-pruning-adapters/badge/?version=latest" alt="Documentation Status" height="20"/>
   </a> -->
   <!-- <a href="https://pepy.tech/project/structured-pruning-adapters">
     <img src="https://pepy.tech/badge/structured-pruning-adapters" height="20">
   </a> -->
-  <!-- <a href="https://codecov.io/gh/LukasHedegaard/structured-pruning-adapters">
-    <img src="https://codecov.io/gh/LukasHedegaard/structured-pruning-adapters/branch/main/graph/badge.svg?token=????" height="20"/>
-  </a> -->
   <a href="https://opensource.org/licenses/Apache-2.0">
     <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg" height="20">
   </a>
-  <!-- <a href="https://arxiv.org/abs/2204.03418">
-    <img src="http://img.shields.io/badge/paper-arxiv.2204.03418-B31B1B.svg" height="20" >
-  </a> -->
+  <a href="https://arxiv.org/abs/2211.10155">
+    <img src="http://img.shields.io/badge/paper-arxiv.2211.10155-B31B1B.svg" height="20" >
+  </a>
   <a href="https://github.com/psf/black">
     <img src="https://img.shields.io/badge/code%20style-black-000000.svg" height="20">
   </a>
-  <!-- <a href="https://www.codefactor.io/repository/github/lukashedegaard/structured-pruning-adapters/overview/main">
-    <img src="https://www.codefactor.io/repository/github/lukashedegaard/structured-pruning-adapters/badge/main" alt="CodeFactor" height="20" />
-  </a> -->
+    <a href="https://codecov.io/github/LukasHedegaard/structured-pruning-adapters" > 
+    <img src="https://codecov.io/github/LukasHedegaard/structured-pruning-adapters/branch/main/graph/badge.svg?token=WHBSM01TRN"/> 
+  </a>
+  <a href="https://www.codefactor.io/repository/github/lukashedegaard/structured-pruning-adapters">
+    <img src="https://www.codefactor.io/repository/github/lukashedegaard/structured-pruning-adapters/badge" alt="CodeFactor" />
+  </a>
 </div>
 
 ```bash
 pip install structured-pruning-adapters
 ```
 ## A happy mariage 👰‍♀️🤵‍♂️
 
@@ -66,29 +66,33 @@
 
     reg_lin = Linear(256, 512, bias=True)
     spa_lin = SPLoRA(reg_lin, rank=32)
 
     # Or replace all applicable layers in a network
     spa_net = SPLoRA(reg_net, rank=32)
     ```
-3. Employ any Structured Pruning method, e.g [this](https://github.com/huggingface/block_movement_pruning) or [that](https://github.com/seulkiyeom/LRP_Pruning).
+3. Employ any Structured Pruning method. We conducted extensive experimens with multiple [channel-pruning](https://github.com/lukashedegaard/channel-spa-experiments) and [block-pruning](https://github.com/lukashedegaard/block-spa-experiments) methods.
 
 4. Get pruned SP Adapter weights:
     ```python3
-    # Specify mask
-    spa_lin.configure_parameter_read(
+    # Specify mask - learned via your choice of Structured Pruning method
+    in_features_mask=torch.tensor([1, 0, ..., 1], dtype=torch.bool)
+    out_features_mask=torch.tensor([0, 1, ..., 1], dtype=torch.bool)
+
+    # Read parameters
+    params = sp_adapters.splora.parameters(
         adapter_weights_only=True,
         in_features_mask=torch.tensor([1, 0, ..., 1], dtype=torch.bool)
         out_features_mask=torch.tensor([0, 1, ..., 1], dtype=torch.bool),
-    )   # 👆 masks are learned via your choice of Structured Pruning method
-
-    # Read parameters as usual
-    spa_lin.parameters()
-    spa_lin.named_parameters()
-    spa_lin.state_dict()
+    )   
+    named_parameters = sp_adapters.splora.named_parameters(
+        adapter_weights_only=True,
+        in_features_mask=torch.tensor([1, 0, ..., 1], dtype=torch.bool)
+        out_features_mask=torch.tensor([0, 1, ..., 1], dtype=torch.bool),
+    )
     ```
 
 ### Demo
 See also [notebooks/demo.ipynb](notebooks/demo.ipynb) for a hands-on demo.
 
 ### Structured Pruning Low-Rank Adapter (SPLoRA) for _Channel Pruning_ 
 ```python3
@@ -97,32 +101,32 @@
 <div align="center">
 <img src="figures/SPLoRA.png" width="400">
 </div>
 Adds a low-rank bottle-neck projection in projection in parallel with the main weights projection.
 
 <br/>
 
-### Structured Pruning Low-rank PHM Adapter (SPLoPA) for _Block Pruning_
+### Structured Pruning Low-rank PHM Adapter (SPLoPA) for _Block Pruning_ (experimental)
 ```python3
 from sp_adapters import SPLoPA
 ```
 
 <div align="center">
 <img src="figures/SPLoPA.png" width="600">
 </div>
 
 Uses a variation on the Parameterized Hypercomplex Multiplication (PHM) layer [[paper](https://openreview.net/forum?id=rcQdycl0zyk)] with shared low-rank prototypes for block-sparse adaptation.
 
 ## Citation
 If you enjoy this work, please consider citing it
 ```bibtex
-@article{hedegaard2022cotrans,
+@article{hedegaard2022structured,
   title={Structured Pruning Adapters},
-  author={Lukas Hedegaard, Aman Alok, Juby Jose, Alexandros Iosifidis},
-  journal={preprint, arXiv:TBD},
+  author={Lukas Hedegaard and Aman Alok and Juby Jose and Alexandros Iosifidis},
+  journal={preprint, arXiv:2211.10155},
   year={2022}
 }
 ```
 
 ## Acknowledgement
 This work was done in conjunction with a research exchange at [Cactus Communications 🌵](https://cactusglobal.com).
```

#### html2text {}

```diff
@@ -1,10 +1,14 @@
 # Structured Pruning Adapters for PyTorch
-    [https://img.shields.io/badge/License-Apache%202.0-blue.svg]  [https://
-img.shields.io/badge/code%20style-black-000000.svg]
+[https://img.shields.io/pypi/pyversions/structured-pruning-adapters] [https://
+badge.fury.io/py/structured-pruning-adapters.svg]   [https://img.shields.io/
+badge/License-Apache%202.0-blue.svg] [http://img.shields.io/badge/paper-
+arxiv.2211.10155-B31B1B.svg] [https://img.shields.io/badge/code%20style-black-
+000000.svg] [https://codecov.io/github/LukasHedegaard/structured-pruning-
+adapters/branch/main/graph/badge.svg?token=WHBSM01TRN] [CodeFactor]
 ```bash pip install structured-pruning-adapters ``` ## A happy mariage
 ð°ââï¸ð¤µââï¸ __Pruning__ is an effective method for reducing the
 size of neural networks. Besides reducing the parameter count, the process
 _can_ accelerate inference as well. CPUs can handle sparse weights just fine,
 but GPUs need structured weights for an acceleration to happen. A structured
 approach to pruning i.e., removing network channels [[paper](https://
 www.sciencedirect.com/science/article/pii/S0031320321000868)] or blocks of
@@ -23,36 +27,40 @@
 parameters (binary pruning mask + masked adapter weights) ð - â
 Accelerated network inference ðð¨ ## How to use this library Use in
 conjunction with any Structured Pruning technique. 1. Install the library:
 ```bash pip install structured-pruning-adapters ``` 2. Replace Linear and Conv
 layers with an SP Adapter: ```python3 from torch.nn import Linear from
 sp_adapter import SPLoRA reg_lin = Linear(256, 512, bias=True) spa_lin = SPLoRA
 (reg_lin, rank=32) # Or replace all applicable layers in a network spa_net =
-SPLoRA(reg_net, rank=32) ``` 3. Employ any Structured Pruning method, e.g
-[this](https://github.com/huggingface/block_movement_pruning) or [that](https:/
-/github.com/seulkiyeom/LRP_Pruning). 4. Get pruned SP Adapter weights:
-```python3 # Specify mask spa_lin.configure_parameter_read
+SPLoRA(reg_net, rank=32) ``` 3. Employ any Structured Pruning method. We
+conducted extensive experimens with multiple [channel-pruning](https://
+github.com/lukashedegaard/channel-spa-experiments) and [block-pruning](https://
+github.com/lukashedegaard/block-spa-experiments) methods. 4. Get pruned SP
+Adapter weights: ```python3 # Specify mask - learned via your choice of
+Structured Pruning method in_features_mask=torch.tensor([1, 0, ..., 1],
+dtype=torch.bool) out_features_mask=torch.tensor([0, 1, ..., 1],
+dtype=torch.bool) # Read parameters params = sp_adapters.splora.parameters
+( adapter_weights_only=True, in_features_mask=torch.tensor([1, 0, ..., 1],
+dtype=torch.bool) out_features_mask=torch.tensor([0, 1, ..., 1],
+dtype=torch.bool), ) named_parameters = sp_adapters.splora.named_parameters
 ( adapter_weights_only=True, in_features_mask=torch.tensor([1, 0, ..., 1],
 dtype=torch.bool) out_features_mask=torch.tensor([0, 1, ..., 1],
-dtype=torch.bool), ) # ð masks are learned via your choice of Structured
-Pruning method # Read parameters as usual spa_lin.parameters()
-spa_lin.named_parameters() spa_lin.state_dict() ``` ### Demo See also
-[notebooks/demo.ipynb](notebooks/demo.ipynb) for a hands-on demo. ###
-Structured Pruning Low-Rank Adapter (SPLoRA) for _Channel Pruning_ ```python3
-from sp_adapters import SPLoRA ```
+dtype=torch.bool), ) ``` ### Demo See also [notebooks/demo.ipynb](notebooks/
+demo.ipynb) for a hands-on demo. ### Structured Pruning Low-Rank Adapter
+(SPLoRA) for _Channel Pruning_ ```python3 from sp_adapters import SPLoRA ```
                              [figures/SPLoRA.png]
 Adds a low-rank bottle-neck projection in projection in parallel with the main
 weights projection.
 ### Structured Pruning Low-rank PHM Adapter (SPLoPA) for _Block Pruning_
-```python3 from sp_adapters import SPLoPA ```
+(experimental) ```python3 from sp_adapters import SPLoPA ```
                              [figures/SPLoPA.png]
 Uses a variation on the Parameterized Hypercomplex Multiplication (PHM) layer [
 [paper](https://openreview.net/forum?id=rcQdycl0zyk)] with shared low-rank
 prototypes for block-sparse adaptation. ## Citation If you enjoy this work,
-please consider citing it ```bibtex @article{hedegaard2022cotrans, title=
-{Structured Pruning Adapters}, author={Lukas Hedegaard, Aman Alok, Juby Jose,
-Alexandros Iosifidis}, journal={preprint, arXiv:TBD}, year={2022} } ``` ##
-Acknowledgement This work was done in conjunction with a research exchange at
-[Cactus Communications ðµ](https://cactusglobal.com). This work has received
-funding from the European Unionâs Horizon 2020 research and innovation
-programme under grant agreement No 871449 [(OpenDR) ðªðº](https://
-opendr.eu).
+please consider citing it ```bibtex @article{hedegaard2022structured, title=
+{Structured Pruning Adapters}, author={Lukas Hedegaard and Aman Alok and Juby
+Jose and Alexandros Iosifidis}, journal={preprint, arXiv:2211.10155}, year=
+{2022} } ``` ## Acknowledgement This work was done in conjunction with a
+research exchange at [Cactus Communications ðµ](https://cactusglobal.com).
+This work has received funding from the European Unionâs Horizon 2020
+research and innovation programme under grant agreement No 871449 [(OpenDR)
+ðªðº](https://opendr.eu).
```

### Comparing `structured-pruning-adapters-0.5.2/setup.py` & `structured-pruning-adapters-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.5.2/sp_adapters/lora.py` & `structured-pruning-adapters-0.6.0/sp_adapters/lora.py`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.5.2/sp_adapters/splopa.py` & `structured-pruning-adapters-0.6.0/sp_adapters/splopa.py`

 * *Files 10% similar despite different names*

```diff
@@ -75,53 +75,23 @@
             num_prototypes,
             block_shape,
             prototype_rank,
             shared_prototypes,
             shared_pos_weights,
             init_range,
         )
-        if bias:
-            self.adapter_bias = nn.Parameter(
-                torch.empty(out_features, **factory_kwargs)
-            )
-            nn.init.uniform_(self.adapter_bias, -init_range, init_range)
-        else:
-            self.register_parameter("adapter_bias", None)
         self.reset_parameters()
-        self.configure_parameter_read()
 
     def forward(self, input):
-        return nn.functional.linear(input, self.adapted_weight, self.adapted_bias)
+        return nn.functional.linear(input, self.adapted_weight, self.bias)
 
     @property
     def adapted_weight(self) -> nn.Parameter:
         return self.adapter(self.weight)
 
-    @property
-    def adapted_bias(self) -> nn.Parameter:
-        result = None
-        if self.adapter_bias is not None:
-            result = self.bias + self.adapter_bias
-        return result
-
-    def configure_parameter_read(
-        self, adapter_weights_only=True, mask: torch.BoolTensor = None
-    ):
-        self._read_adapter_weights_only = adapter_weights_only
-        self._read_mask = mask
-
-    def named_parameters(
-        self, prefix: str = "", recurse: bool = True
-    ) -> Iterator[Tuple[str, nn.Parameter]]:
-        for name, param in super().named_parameters(prefix, recurse):
-            if not self._read_adapter_weights_only or "adapter" in name:
-                if name == "adapter.pos_weights" and self._read_mask is not None:
-                    param = param[self._read_mask].flatten()
-                yield (name, param)
-
     @classmethod
     def from_module(
         cls,
         module: nn.Linear,
         num_prototypes: int = 64,
         block_shape: Tuple[int, int] = (32, 32),
         prototype_rank: int = 1,
@@ -143,18 +113,42 @@
         copy_linear_params_(module, instance)
         return instance
 
     def to_module(self) -> nn.Linear:
         instance = nn.Linear(self.in_features, self.out_features, self.bias is not None)
         instance.weight = torch.nn.Parameter(self.adapted_weight)
         if self.bias is not None:
-            instance.bias = torch.nn.Parameter(self.adapted_bias)
+            instance.bias = torch.nn.Parameter(self.bias)
         return instance
 
 
+def named_parameters(
+    splopa_model: nn.Module,
+    prefix: str = "",
+    recurse: bool = True,
+    adapter_weights_only: bool = True,
+    mask: torch.BoolTensor = None,
+) -> Iterator[Tuple[str, nn.Parameter]]:
+    for name, param in nn.Module.named_parameters(splopa_model, prefix, recurse):
+        if not adapter_weights_only or "adapter" in name:
+            if name == "adapter.pos_weights" and mask is not None:
+                param = param[mask].flatten()
+            yield (name, param)
+
+
+def parameters(
+    module: nn.Module,
+    recurse: bool = True,
+    adapter_weights_only: bool = True,
+    mask: torch.BoolTensor = None,
+):
+    for _, param in named_parameters(module, "", recurse, adapter_weights_only, mask):
+        yield param
+
+
 class SPLoPAdapter(nn.Module):  # Inherit __setattr__
     def __init__(
         self,
         weight_shape: Tuple[int, int],
         num_prototypes: int = 64,
         block_shape: Tuple[int, int] = (32, 32),
         prototype_rank: int = 1,
```

### Comparing `structured-pruning-adapters-0.5.2/sp_adapters/utils.py` & `structured-pruning-adapters-0.6.0/sp_adapters/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     return res.reshape(siz0 + siz1)
 
 
 def copy_linear_params_(source: nn.Linear, target: nn.Linear, clone=True):
     maybe_clone = torch.clone if clone else lambda x: x
     target.weight = nn.Parameter(maybe_clone(source.weight), requires_grad=False)
     if source.bias is not None:
-        target.bias = nn.Parameter(maybe_clone(source.bias), requires_grad=False)
+        target.bias = nn.Parameter(maybe_clone(source.bias))
 
 
 def recursive_replace(
     module: nn.Module,
     OldModuleType: Type[nn.Module],
     new_module_constructor: Callable[[nn.Module], nn.Module],
     inplace=False,
```

### Comparing `structured-pruning-adapters-0.5.2/structured_pruning_adapters.egg-info/PKG-INFO` & `structured-pruning-adapters-0.6.0/structured_pruning_adapters.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structured-pruning-adapters
-Version: 0.5.2
+Version: 0.6.0
 Summary: Structured Pruning Adapters for PyTorch
 Home-page: https://github.com/lukashedegaard/structured-pruning-adapters
 Author: Lukas Hedegaard
 Author-email: lukasxhedegaard@gmail.com
 License: UNKNOWN
 Keywords: deep learning,pytorch,AI,adapters,pruning,inference
 Platform: UNKNOWN
@@ -27,41 +27,41 @@
 Provides-Extra: build
 Provides-Extra: dev
 License-File: LICENSE
 
 # Structured Pruning Adapters for PyTorch
 
 <div align="left">
-  <!-- <a href="https://pypi.org/project/structured-pruning-adapters/">
+  <a href="https://pypi.org/project/structured-pruning-adapters/">
     <img src="https://img.shields.io/pypi/pyversions/structured-pruning-adapters" height="20" >
   </a>
   <a href="https://badge.fury.io/py/structured-pruning-adapters">
     <img src="https://badge.fury.io/py/structured-pruning-adapters.svg" height="20" >
-  </a> -->
+  </a>
   <!-- <a href="https://structured-pruning-adapters.readthedocs.io/en/latest/?badge=latest">
     <img src="https://readthedocs.org/projects/structured-pruning-adapters/badge/?version=latest" alt="Documentation Status" height="20"/>
   </a> -->
   <!-- <a href="https://pepy.tech/project/structured-pruning-adapters">
     <img src="https://pepy.tech/badge/structured-pruning-adapters" height="20">
   </a> -->
-  <!-- <a href="https://codecov.io/gh/LukasHedegaard/structured-pruning-adapters">
-    <img src="https://codecov.io/gh/LukasHedegaard/structured-pruning-adapters/branch/main/graph/badge.svg?token=????" height="20"/>
-  </a> -->
   <a href="https://opensource.org/licenses/Apache-2.0">
     <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg" height="20">
   </a>
-  <!-- <a href="https://arxiv.org/abs/2204.03418">
-    <img src="http://img.shields.io/badge/paper-arxiv.2204.03418-B31B1B.svg" height="20" >
-  </a> -->
+  <a href="https://arxiv.org/abs/2211.10155">
+    <img src="http://img.shields.io/badge/paper-arxiv.2211.10155-B31B1B.svg" height="20" >
+  </a>
   <a href="https://github.com/psf/black">
     <img src="https://img.shields.io/badge/code%20style-black-000000.svg" height="20">
   </a>
-  <!-- <a href="https://www.codefactor.io/repository/github/lukashedegaard/structured-pruning-adapters/overview/main">
-    <img src="https://www.codefactor.io/repository/github/lukashedegaard/structured-pruning-adapters/badge/main" alt="CodeFactor" height="20" />
-  </a> -->
+    <a href="https://codecov.io/github/LukasHedegaard/structured-pruning-adapters" > 
+    <img src="https://codecov.io/github/LukasHedegaard/structured-pruning-adapters/branch/main/graph/badge.svg?token=WHBSM01TRN"/> 
+  </a>
+  <a href="https://www.codefactor.io/repository/github/lukashedegaard/structured-pruning-adapters">
+    <img src="https://www.codefactor.io/repository/github/lukashedegaard/structured-pruning-adapters/badge" alt="CodeFactor" />
+  </a>
 </div>
 
 ```bash
 pip install structured-pruning-adapters
 ```
 ## A happy mariage 👰‍♀️🤵‍♂️
 
@@ -96,29 +96,33 @@
 
     reg_lin = Linear(256, 512, bias=True)
     spa_lin = SPLoRA(reg_lin, rank=32)
 
     # Or replace all applicable layers in a network
     spa_net = SPLoRA(reg_net, rank=32)
     ```
-3. Employ any Structured Pruning method, e.g [this](https://github.com/huggingface/block_movement_pruning) or [that](https://github.com/seulkiyeom/LRP_Pruning).
+3. Employ any Structured Pruning method. We conducted extensive experimens with multiple [channel-pruning](https://github.com/lukashedegaard/channel-spa-experiments) and [block-pruning](https://github.com/lukashedegaard/block-spa-experiments) methods.
 
 4. Get pruned SP Adapter weights:
     ```python3
-    # Specify mask
-    spa_lin.configure_parameter_read(
+    # Specify mask - learned via your choice of Structured Pruning method
+    in_features_mask=torch.tensor([1, 0, ..., 1], dtype=torch.bool)
+    out_features_mask=torch.tensor([0, 1, ..., 1], dtype=torch.bool)
+
+    # Read parameters
+    params = sp_adapters.splora.parameters(
         adapter_weights_only=True,
         in_features_mask=torch.tensor([1, 0, ..., 1], dtype=torch.bool)
         out_features_mask=torch.tensor([0, 1, ..., 1], dtype=torch.bool),
-    )   # 👆 masks are learned via your choice of Structured Pruning method
-
-    # Read parameters as usual
-    spa_lin.parameters()
-    spa_lin.named_parameters()
-    spa_lin.state_dict()
+    )   
+    named_parameters = sp_adapters.splora.named_parameters(
+        adapter_weights_only=True,
+        in_features_mask=torch.tensor([1, 0, ..., 1], dtype=torch.bool)
+        out_features_mask=torch.tensor([0, 1, ..., 1], dtype=torch.bool),
+    )
     ```
 
 ### Demo
 See also [notebooks/demo.ipynb](notebooks/demo.ipynb) for a hands-on demo.
 
 ### Structured Pruning Low-Rank Adapter (SPLoRA) for _Channel Pruning_ 
 ```python3
@@ -127,32 +131,32 @@
 <div align="center">
 <img src="figures/SPLoRA.png" width="400">
 </div>
 Adds a low-rank bottle-neck projection in projection in parallel with the main weights projection.
 
 <br/>
 
-### Structured Pruning Low-rank PHM Adapter (SPLoPA) for _Block Pruning_
+### Structured Pruning Low-rank PHM Adapter (SPLoPA) for _Block Pruning_ (experimental)
 ```python3
 from sp_adapters import SPLoPA
 ```
 
 <div align="center">
 <img src="figures/SPLoPA.png" width="600">
 </div>
 
 Uses a variation on the Parameterized Hypercomplex Multiplication (PHM) layer [[paper](https://openreview.net/forum?id=rcQdycl0zyk)] with shared low-rank prototypes for block-sparse adaptation.
 
 ## Citation
 If you enjoy this work, please consider citing it
 ```bibtex
-@article{hedegaard2022cotrans,
+@article{hedegaard2022structured,
   title={Structured Pruning Adapters},
-  author={Lukas Hedegaard, Aman Alok, Juby Jose, Alexandros Iosifidis},
-  journal={preprint, arXiv:TBD},
+  author={Lukas Hedegaard and Aman Alok and Juby Jose and Alexandros Iosifidis},
+  journal={preprint, arXiv:2211.10155},
   year={2022}
 }
 ```
 
 ## Acknowledgement
 This work was done in conjunction with a research exchange at [Cactus Communications 🌵](https://cactusglobal.com).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: structured-pruning-adapters Version: 0.5.2 Summary:
+Metadata-Version: 2.1 Name: structured-pruning-adapters Version: 0.6.0 Summary:
 Structured Pruning Adapters for PyTorch Home-page: https://github.com/
 lukashedegaard/structured-pruning-adapters Author: Lukas Hedegaard Author-
 email: lukasxhedegaard@gmail.com License: UNKNOWN Keywords: deep
 learning,pytorch,AI,adapters,pruning,inference Platform: UNKNOWN Classifier:
 Environment :: Console Classifier: Natural Language :: English Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -12,16 +12,20 @@
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Description-Content-Type: text/markdown Provides-Extra: build
 Provides-Extra: dev License-File: LICENSE # Structured Pruning Adapters for
 PyTorch
-    [https://img.shields.io/badge/License-Apache%202.0-blue.svg]  [https://
-img.shields.io/badge/code%20style-black-000000.svg]
+[https://img.shields.io/pypi/pyversions/structured-pruning-adapters] [https://
+badge.fury.io/py/structured-pruning-adapters.svg]   [https://img.shields.io/
+badge/License-Apache%202.0-blue.svg] [http://img.shields.io/badge/paper-
+arxiv.2211.10155-B31B1B.svg] [https://img.shields.io/badge/code%20style-black-
+000000.svg] [https://codecov.io/github/LukasHedegaard/structured-pruning-
+adapters/branch/main/graph/badge.svg?token=WHBSM01TRN] [CodeFactor]
 ```bash pip install structured-pruning-adapters ``` ## A happy mariage
 ð°ââï¸ð¤µââï¸ __Pruning__ is an effective method for reducing the
 size of neural networks. Besides reducing the parameter count, the process
 _can_ accelerate inference as well. CPUs can handle sparse weights just fine,
 but GPUs need structured weights for an acceleration to happen. A structured
 approach to pruning i.e., removing network channels [[paper](https://
 www.sciencedirect.com/science/article/pii/S0031320321000868)] or blocks of
@@ -40,36 +44,40 @@
 parameters (binary pruning mask + masked adapter weights) ð - â
 Accelerated network inference ðð¨ ## How to use this library Use in
 conjunction with any Structured Pruning technique. 1. Install the library:
 ```bash pip install structured-pruning-adapters ``` 2. Replace Linear and Conv
 layers with an SP Adapter: ```python3 from torch.nn import Linear from
 sp_adapter import SPLoRA reg_lin = Linear(256, 512, bias=True) spa_lin = SPLoRA
 (reg_lin, rank=32) # Or replace all applicable layers in a network spa_net =
-SPLoRA(reg_net, rank=32) ``` 3. Employ any Structured Pruning method, e.g
-[this](https://github.com/huggingface/block_movement_pruning) or [that](https:/
-/github.com/seulkiyeom/LRP_Pruning). 4. Get pruned SP Adapter weights:
-```python3 # Specify mask spa_lin.configure_parameter_read
+SPLoRA(reg_net, rank=32) ``` 3. Employ any Structured Pruning method. We
+conducted extensive experimens with multiple [channel-pruning](https://
+github.com/lukashedegaard/channel-spa-experiments) and [block-pruning](https://
+github.com/lukashedegaard/block-spa-experiments) methods. 4. Get pruned SP
+Adapter weights: ```python3 # Specify mask - learned via your choice of
+Structured Pruning method in_features_mask=torch.tensor([1, 0, ..., 1],
+dtype=torch.bool) out_features_mask=torch.tensor([0, 1, ..., 1],
+dtype=torch.bool) # Read parameters params = sp_adapters.splora.parameters
+( adapter_weights_only=True, in_features_mask=torch.tensor([1, 0, ..., 1],
+dtype=torch.bool) out_features_mask=torch.tensor([0, 1, ..., 1],
+dtype=torch.bool), ) named_parameters = sp_adapters.splora.named_parameters
 ( adapter_weights_only=True, in_features_mask=torch.tensor([1, 0, ..., 1],
 dtype=torch.bool) out_features_mask=torch.tensor([0, 1, ..., 1],
-dtype=torch.bool), ) # ð masks are learned via your choice of Structured
-Pruning method # Read parameters as usual spa_lin.parameters()
-spa_lin.named_parameters() spa_lin.state_dict() ``` ### Demo See also
-[notebooks/demo.ipynb](notebooks/demo.ipynb) for a hands-on demo. ###
-Structured Pruning Low-Rank Adapter (SPLoRA) for _Channel Pruning_ ```python3
-from sp_adapters import SPLoRA ```
+dtype=torch.bool), ) ``` ### Demo See also [notebooks/demo.ipynb](notebooks/
+demo.ipynb) for a hands-on demo. ### Structured Pruning Low-Rank Adapter
+(SPLoRA) for _Channel Pruning_ ```python3 from sp_adapters import SPLoRA ```
                              [figures/SPLoRA.png]
 Adds a low-rank bottle-neck projection in projection in parallel with the main
 weights projection.
 ### Structured Pruning Low-rank PHM Adapter (SPLoPA) for _Block Pruning_
-```python3 from sp_adapters import SPLoPA ```
+(experimental) ```python3 from sp_adapters import SPLoPA ```
                              [figures/SPLoPA.png]
 Uses a variation on the Parameterized Hypercomplex Multiplication (PHM) layer [
 [paper](https://openreview.net/forum?id=rcQdycl0zyk)] with shared low-rank
 prototypes for block-sparse adaptation. ## Citation If you enjoy this work,
-please consider citing it ```bibtex @article{hedegaard2022cotrans, title=
-{Structured Pruning Adapters}, author={Lukas Hedegaard, Aman Alok, Juby Jose,
-Alexandros Iosifidis}, journal={preprint, arXiv:TBD}, year={2022} } ``` ##
-Acknowledgement This work was done in conjunction with a research exchange at
-[Cactus Communications ðµ](https://cactusglobal.com). This work has received
-funding from the European Unionâs Horizon 2020 research and innovation
-programme under grant agreement No 871449 [(OpenDR) ðªðº](https://
-opendr.eu).
+please consider citing it ```bibtex @article{hedegaard2022structured, title=
+{Structured Pruning Adapters}, author={Lukas Hedegaard and Aman Alok and Juby
+Jose and Alexandros Iosifidis}, journal={preprint, arXiv:2211.10155}, year=
+{2022} } ``` ## Acknowledgement This work was done in conjunction with a
+research exchange at [Cactus Communications ðµ](https://cactusglobal.com).
+This work has received funding from the European Unionâs Horizon 2020
+research and innovation programme under grant agreement No 871449 [(OpenDR)
+ðªðº](https://opendr.eu).
```

