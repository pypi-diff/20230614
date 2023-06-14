# Comparing `tmp/dog-optimizer-1.0.2.tar.gz` & `tmp/dog-optimizer-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dog-optimizer-1.0.2.tar", last modified: Sun Feb 26 18:47:32 2023, max compression
+gzip compressed data, was "dog-optimizer-1.0.3.tar", last modified: Wed Jun 14 18:40:01 2023, max compression
```

## Comparing `dog-optimizer-1.0.2.tar` & `dog-optimizer-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 maorivgi   (501) staff       (20)        0 2023-02-26 18:47:32.579017 dog-optimizer-1.0.2/
--rw-r--r--   0 maorivgi   (501) staff       (20)     1099 2023-02-05 17:09:07.000000 dog-optimizer-1.0.2/LICENSE
--rw-r--r--   0 maorivgi   (501) staff       (20)     4576 2023-02-26 18:47:32.578877 dog-optimizer-1.0.2/PKG-INFO
--rw-r--r--   0 maorivgi   (501) staff       (20)     4009 2023-02-26 18:46:02.000000 dog-optimizer-1.0.2/README.md
--rw-r--r--   0 maorivgi   (501) staff       (20)      664 2023-02-26 18:47:20.000000 dog-optimizer-1.0.2/pyproject.toml
--rw-r--r--   0 maorivgi   (501) staff       (20)       38 2023-02-26 18:47:32.579059 dog-optimizer-1.0.2/setup.cfg
-drwxr-xr-x   0 maorivgi   (501) staff       (20)        0 2023-02-26 18:47:32.577519 dog-optimizer-1.0.2/src/
-drwxr-xr-x   0 maorivgi   (501) staff       (20)        0 2023-02-26 18:47:32.578258 dog-optimizer-1.0.2/src/dog/
--rw-r--r--   0 maorivgi   (501) staff       (20)       72 2023-02-24 09:40:11.000000 dog-optimizer-1.0.2/src/dog/__init__.py
--rw-r--r--   0 maorivgi   (501) staff       (20)     3283 2023-02-24 09:40:11.000000 dog-optimizer-1.0.2/src/dog/averager.py
--rw-r--r--   0 maorivgi   (501) staff       (20)     8926 2023-02-26 18:46:15.000000 dog-optimizer-1.0.2/src/dog/dog.py
-drwxr-xr-x   0 maorivgi   (501) staff       (20)        0 2023-02-26 18:47:32.578712 dog-optimizer-1.0.2/src/dog_optimizer.egg-info/
--rw-r--r--   0 maorivgi   (501) staff       (20)     4576 2023-02-26 18:47:32.000000 dog-optimizer-1.0.2/src/dog_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 maorivgi   (501) staff       (20)      251 2023-02-26 18:47:32.000000 dog-optimizer-1.0.2/src/dog_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 maorivgi   (501) staff       (20)        1 2023-02-26 18:47:32.000000 dog-optimizer-1.0.2/src/dog_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 maorivgi   (501) staff       (20)        4 2023-02-26 18:47:32.000000 dog-optimizer-1.0.2/src/dog_optimizer.egg-info/top_level.txt
+drwxr-xr-x   0 maorivgi   (501) staff       (20)        0 2023-06-14 18:40:01.946078 dog-optimizer-1.0.3/
+-rw-r--r--   0 maorivgi   (501) staff       (20)     1099 2023-02-05 17:09:07.000000 dog-optimizer-1.0.3/LICENSE
+-rw-r--r--   0 maorivgi   (501) staff       (20)     4970 2023-06-14 18:40:01.945959 dog-optimizer-1.0.3/PKG-INFO
+-rw-r--r--   0 maorivgi   (501) staff       (20)     4404 2023-06-14 18:07:20.000000 dog-optimizer-1.0.3/README.md
+-rw-r--r--   0 maorivgi   (501) staff       (20)      664 2023-06-14 18:39:44.000000 dog-optimizer-1.0.3/pyproject.toml
+-rw-r--r--   0 maorivgi   (501) staff       (20)       38 2023-06-14 18:40:01.946111 dog-optimizer-1.0.3/setup.cfg
+drwxr-xr-x   0 maorivgi   (501) staff       (20)        0 2023-06-14 18:40:01.944074 dog-optimizer-1.0.3/src/
+drwxr-xr-x   0 maorivgi   (501) staff       (20)        0 2023-06-14 18:40:01.945182 dog-optimizer-1.0.3/src/dog/
+-rw-r--r--   0 maorivgi   (501) staff       (20)       72 2023-02-24 09:40:11.000000 dog-optimizer-1.0.3/src/dog/__init__.py
+-rw-r--r--   0 maorivgi   (501) staff       (20)     3283 2023-02-24 09:40:11.000000 dog-optimizer-1.0.3/src/dog/averager.py
+-rw-r--r--   0 maorivgi   (501) staff       (20)     9388 2023-06-14 18:07:20.000000 dog-optimizer-1.0.3/src/dog/dog.py
+drwxr-xr-x   0 maorivgi   (501) staff       (20)        0 2023-06-14 18:40:01.945808 dog-optimizer-1.0.3/src/dog_optimizer.egg-info/
+-rw-r--r--   0 maorivgi   (501) staff       (20)     4970 2023-06-14 18:40:01.000000 dog-optimizer-1.0.3/src/dog_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 maorivgi   (501) staff       (20)      251 2023-06-14 18:40:01.000000 dog-optimizer-1.0.3/src/dog_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 maorivgi   (501) staff       (20)        1 2023-06-14 18:40:01.000000 dog-optimizer-1.0.3/src/dog_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 maorivgi   (501) staff       (20)        4 2023-06-14 18:40:01.000000 dog-optimizer-1.0.3/src/dog_optimizer.egg-info/top_level.txt
```

### Comparing `dog-optimizer-1.0.2/LICENSE` & `dog-optimizer-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dog-optimizer-1.0.2/PKG-INFO` & `dog-optimizer-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dog-optimizer
-Version: 1.0.2
+Version: 1.0.3
 Summary: implementation of the algorithms in the paper DoG is SGD's Best Friend: A Parameter-Free Dynamic Step Size Schedule
 Author: Maor Ivgi, Oliver Hinder, Yair Carmon
 Project-URL: Homepage, https://github.com/formll/dog
 Project-URL: Paper, https://arxiv.org/abs/2302.12022
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,14 +14,16 @@
 
 # DoG Optimizer
 
 This repository contains the implementation of the algorithms in the paper 
 [DoG is SGD's Best Friend: A Parameter-Free Dynamic Step Size Schedule](https://arxiv.org/abs/2302.12022)
 by Maor Ivgi, Oliver Hinder and Yair Carmon.
 
+**IMPORTANT:** For best performance (and for fair comparison to other methods) **DoG/L-DoG must be combined with iterate averaging!** This package includes an easy-to-use [averager class](<#iterate-averaging>) - its default configuration should work well out of the box.
+
 ## Algorithm
 DoG ("Distance over Gradients") is a parameter-free stochastic optimizer. 
 DoG updates parameters $x_t$ with stochastic gradients $g_t$ according to:
 ```math
 \begin{aligned}
    \eta_t & = \frac{ \bar{r}_t }{ \sqrt{\sum_{i \le t }{\lVert g_i\rVert ^2 + \epsilon}} } \\   
    x_{t+1} & = x_{t} - \eta_t \cdot g_t
@@ -55,23 +57,24 @@
 from dog import LDoG
 optimizer = LDoG(optimizer args)
 ```
 for LDoG, 
 where `optimizer args` follows the standard pytorch optimizer syntex. 
 To see the list of all available parameters, run `help(DoG)` or `help(LDoG)`.
 
-
-Using the polynomial decay averager is also easy. Simply create it with 
+### Iterate averaging
+We provide an implementation of the polynomial decay averaging used throughout our experimentes. TO use it simply create a `PolynomialDecayAverager` with 
 ```python
 from dog import PolynomialDecayAverager
 averager = PolynomialDecayAverager(model)
 ```
 then, after each `optimizer.step()`, call `averager.step()` as well.
 You can then get both the current model and the averaged model with `averager.base_model` and `averager.averaged_model` respectively.
 
+### Example script
 An example of how to use the above to train a simple CNN on MNIST can be found in `examples/mnist.py` 
 (based on this [pytorch example](https://github.com/pytorch/examples/blob/main/mnist/main.py)).
 
 ### Choosing `reps_rel`
 DoG is parameter-free by design, so there is no need to tune a learning rate parameter. 
 However, as discussed in the paper, DoG has an initial step movement parameter 
 $r_{\epsilon}$ that must be small enough to avoid destructively updates that cause divergence,
```

### Comparing `dog-optimizer-1.0.2/README.md` & `dog-optimizer-1.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # DoG Optimizer
 
 This repository contains the implementation of the algorithms in the paper 
 [DoG is SGD's Best Friend: A Parameter-Free Dynamic Step Size Schedule](https://arxiv.org/abs/2302.12022)
 by Maor Ivgi, Oliver Hinder and Yair Carmon.
 
+**IMPORTANT:** For best performance (and for fair comparison to other methods) **DoG/L-DoG must be combined with iterate averaging!** This package includes an easy-to-use [averager class](<#iterate-averaging>) - its default configuration should work well out of the box.
+
 ## Algorithm
 DoG ("Distance over Gradients") is a parameter-free stochastic optimizer. 
 DoG updates parameters $x_t$ with stochastic gradients $g_t$ according to:
 ```math
 \begin{aligned}
    \eta_t & = \frac{ \bar{r}_t }{ \sqrt{\sum_{i \le t }{\lVert g_i\rVert ^2 + \epsilon}} } \\   
    x_{t+1} & = x_{t} - \eta_t \cdot g_t
@@ -41,23 +43,24 @@
 from dog import LDoG
 optimizer = LDoG(optimizer args)
 ```
 for LDoG, 
 where `optimizer args` follows the standard pytorch optimizer syntex. 
 To see the list of all available parameters, run `help(DoG)` or `help(LDoG)`.
 
-
-Using the polynomial decay averager is also easy. Simply create it with 
+### Iterate averaging
+We provide an implementation of the polynomial decay averaging used throughout our experimentes. TO use it simply create a `PolynomialDecayAverager` with 
 ```python
 from dog import PolynomialDecayAverager
 averager = PolynomialDecayAverager(model)
 ```
 then, after each `optimizer.step()`, call `averager.step()` as well.
 You can then get both the current model and the averaged model with `averager.base_model` and `averager.averaged_model` respectively.
 
+### Example script
 An example of how to use the above to train a simple CNN on MNIST can be found in `examples/mnist.py` 
 (based on this [pytorch example](https://github.com/pytorch/examples/blob/main/mnist/main.py)).
 
 ### Choosing `reps_rel`
 DoG is parameter-free by design, so there is no need to tune a learning rate parameter. 
 However, as discussed in the paper, DoG has an initial step movement parameter 
 $r_{\epsilon}$ that must be small enough to avoid destructively updates that cause divergence, 
@@ -78,8 +81,8 @@
 ```
 @article{ivgi2023dog,
   title={{D}o{G} is {SGD}'s Best Friend: A Parameter-Free Dynamic Step Size Schedule}, 
   author={Maor Ivgi and Oliver Hinder and Yair Carmon}, 
   journal={arXiv:2302.12022}, 
   year={2023},
 }  
-```
+```
```

### Comparing `dog-optimizer-1.0.2/pyproject.toml` & `dog-optimizer-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dog-optimizer"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Maor Ivgi" },
   { name="Oliver Hinder" },
   { name="Yair Carmon" }
 ]
 description = "implementation of the algorithms in the paper DoG is SGD's Best Friend: A Parameter-Free Dynamic Step Size Schedule"
 readme = "README.md"
```

### Comparing `dog-optimizer-1.0.2/src/dog/averager.py` & `dog-optimizer-1.0.3/src/dog/averager.py`

 * *Files identical despite different names*

### Comparing `dog-optimizer-1.0.2/src/dog/dog.py` & `dog-optimizer-1.0.3/src/dog/dog.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,31 +9,35 @@
 
 logger = logging.getLogger(__name__)
 
 
 class DoG(Optimizer):
     """
         DoG (Distance over Gradients) is a parameter-free adaptive optimizer, proposed in
-         `DoG is SGD's Best Friend: A Parameter-Free Dynamic Step Size Schedule` (Ivgi et al., 2023)
+         `DoG is SGD's Best Friend: A Parameter-Free Dynamic Step Size Schedule` (Ivgi et al., 2023).
+       IMPORTANT: for best performance, DoG must be combined with iterate averaging.
     """
 
-    __version__ = '1.0.2'
+    __version__ = '1.0.3'
 
     def __init__(self, params, reps_rel: float = 1e-6, lr: float = 1.0,
                  weight_decay: float = 0.0, eps: float = 1e-8, init_eta: Optional[float] = None):
         r"""Distance over Gradients - an adaptive stochastic optimizer.
 
         DoG updates parameters x_t with stochastic gradients g_t according to:
         .. math::
             \begin{aligned}
                 eta_t & = \frac{ max_{i \le t}{\|x_i - x_0\|} }{ \sqrt{\sum_{i \le t }{\|g_i\|^2 + eps}} }, \\
                 x_{t+1} & = x_{t} - eta_t * g_t,
             \end{aligned}
-
-
+            
+        IMPORTANT: Since we do not employ a step-size decay scheme, ITERATE AVERAGING IS CRUCIAL to obtain 
+        the best performance. This package provides an implementation of the polynomial decay averaging 
+        that is effective and does not require tuning.
+        
         Args:
             params (iterable): iterable of parameters to optimize or dicts defining parameter groups
             reps_rel (float): value to use to compute the  initial distance (r_epsilon in the paper).
                                         Namely, the first step size is given by:
                                         (reps_rel * (1+\|x_0\|)) / (\|g_0\|^2 + eps)^{1/2}  where x_0 are the initial
                                         weights of  the model (or the parameter group), and g_0 is the gradient of the
                                         first step.
@@ -171,14 +175,15 @@
 
 
 class LDoG(DoG):
     """
         Layer-wise DoG, as described in:
        `DoG is SGD's Best Friend: A Parameter-Free Dynamic Step Size Schedule` (Ivgi et al., 2023).
         LDoG applies the DoG formula defined in the DoG class, but for each layer separately.
+        IMPORTANT: for best performance, L-DoG must be combined with iterate averaging.
     """
     def _update_group_state(self, group, init):
         # treat each layer in the group as a separate block
         if self._first_step:
             group['rbar'] = group['reps_rel'] * (1 + torch.stack([p.norm() for p in group['params']]))
             group['G'] = torch.stack([(p.grad ** 2).sum() for p in group['params']]) + group['eps']
         else:
```

### Comparing `dog-optimizer-1.0.2/src/dog_optimizer.egg-info/PKG-INFO` & `dog-optimizer-1.0.3/src/dog_optimizer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dog-optimizer
-Version: 1.0.2
+Version: 1.0.3
 Summary: implementation of the algorithms in the paper DoG is SGD's Best Friend: A Parameter-Free Dynamic Step Size Schedule
 Author: Maor Ivgi, Oliver Hinder, Yair Carmon
 Project-URL: Homepage, https://github.com/formll/dog
 Project-URL: Paper, https://arxiv.org/abs/2302.12022
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,14 +14,16 @@
 
 # DoG Optimizer
 
 This repository contains the implementation of the algorithms in the paper 
 [DoG is SGD's Best Friend: A Parameter-Free Dynamic Step Size Schedule](https://arxiv.org/abs/2302.12022)
 by Maor Ivgi, Oliver Hinder and Yair Carmon.
 
+**IMPORTANT:** For best performance (and for fair comparison to other methods) **DoG/L-DoG must be combined with iterate averaging!** This package includes an easy-to-use [averager class](<#iterate-averaging>) - its default configuration should work well out of the box.
+
 ## Algorithm
 DoG ("Distance over Gradients") is a parameter-free stochastic optimizer. 
 DoG updates parameters $x_t$ with stochastic gradients $g_t$ according to:
 ```math
 \begin{aligned}
    \eta_t & = \frac{ \bar{r}_t }{ \sqrt{\sum_{i \le t }{\lVert g_i\rVert ^2 + \epsilon}} } \\   
    x_{t+1} & = x_{t} - \eta_t \cdot g_t
@@ -55,23 +57,24 @@
 from dog import LDoG
 optimizer = LDoG(optimizer args)
 ```
 for LDoG, 
 where `optimizer args` follows the standard pytorch optimizer syntex. 
 To see the list of all available parameters, run `help(DoG)` or `help(LDoG)`.
 
-
-Using the polynomial decay averager is also easy. Simply create it with 
+### Iterate averaging
+We provide an implementation of the polynomial decay averaging used throughout our experimentes. TO use it simply create a `PolynomialDecayAverager` with 
 ```python
 from dog import PolynomialDecayAverager
 averager = PolynomialDecayAverager(model)
 ```
 then, after each `optimizer.step()`, call `averager.step()` as well.
 You can then get both the current model and the averaged model with `averager.base_model` and `averager.averaged_model` respectively.
 
+### Example script
 An example of how to use the above to train a simple CNN on MNIST can be found in `examples/mnist.py` 
 (based on this [pytorch example](https://github.com/pytorch/examples/blob/main/mnist/main.py)).
 
 ### Choosing `reps_rel`
 DoG is parameter-free by design, so there is no need to tune a learning rate parameter. 
 However, as discussed in the paper, DoG has an initial step movement parameter 
 $r_{\epsilon}$ that must be small enough to avoid destructively updates that cause divergence,
```

