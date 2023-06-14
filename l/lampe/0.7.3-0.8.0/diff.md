# Comparing `tmp/lampe-0.7.3.tar.gz` & `tmp/lampe-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lampe-0.7.3.tar", last modified: Mon Mar 20 17:11:28 2023, max compression
+gzip compressed data, was "lampe-0.8.0.tar", last modified: Wed Jun 14 14:34:00 2023, max compression
```

## Comparing `lampe-0.7.3.tar` & `lampe-0.8.0.tar`

### file list

```diff
@@ -1,21 +1,30 @@
-drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-03-20 17:11:28.822659 lampe-0.7.3/
--rw-rw-r--   0 francois  (1001) francois  (1001)     1072 2022-12-12 11:28:08.000000 lampe-0.7.3/LICENSE
--rw-rw-r--   0 francois  (1001) francois  (1001)     2603 2023-03-20 17:11:28.822659 lampe-0.7.3/PKG-INFO
--rw-rw-r--   0 francois  (1001) francois  (1001)     1707 2023-01-21 11:58:25.000000 lampe-0.7.3/README.md
-drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-03-20 17:11:28.818659 lampe-0.7.3/lampe/
--rw-rw-r--   0 francois  (1001) francois  (1001)      166 2023-03-20 16:55:52.000000 lampe-0.7.3/lampe/__init__.py
--rw-rw-r--   0 francois  (1001) francois  (1001)    11358 2023-02-28 11:03:47.000000 lampe-0.7.3/lampe/data.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     4692 2022-12-14 21:21:35.000000 lampe-0.7.3/lampe/diagnostics.py
--rw-rw-r--   0 francois  (1001) francois  (1001)    26587 2023-02-28 09:09:15.000000 lampe-0.7.3/lampe/inference.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     3131 2022-12-14 21:21:35.000000 lampe-0.7.3/lampe/masks.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     2532 2023-03-20 16:55:52.000000 lampe-0.7.3/lampe/nn.py
--rw-rw-r--   0 francois  (1001) francois  (1001)    13095 2023-03-20 16:55:52.000000 lampe-0.7.3/lampe/plots.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     3201 2023-03-20 16:55:52.000000 lampe-0.7.3/lampe/utils.py
-drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-03-20 17:11:28.822659 lampe-0.7.3/lampe.egg-info/
--rw-rw-r--   0 francois  (1001) francois  (1001)     2603 2023-03-20 17:11:28.000000 lampe-0.7.3/lampe.egg-info/PKG-INFO
--rw-rw-r--   0 francois  (1001) francois  (1001)      309 2023-03-20 17:11:28.000000 lampe-0.7.3/lampe.egg-info/SOURCES.txt
--rw-rw-r--   0 francois  (1001) francois  (1001)        1 2023-03-20 17:11:28.000000 lampe-0.7.3/lampe.egg-info/dependency_links.txt
--rw-rw-r--   0 francois  (1001) francois  (1001)       82 2023-03-20 17:11:28.000000 lampe-0.7.3/lampe.egg-info/requires.txt
--rw-rw-r--   0 francois  (1001) francois  (1001)        6 2023-03-20 17:11:28.000000 lampe-0.7.3/lampe.egg-info/top_level.txt
--rw-rw-r--   0 francois  (1001) francois  (1001)      978 2023-03-20 17:11:28.822659 lampe-0.7.3/setup.cfg
--rw-rw-r--   0 francois  (1001) francois  (1001)       61 2023-01-21 11:58:25.000000 lampe-0.7.3/setup.py
+drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-06-14 14:34:00.887271 lampe-0.8.0/
+-rw-rw-r--   0 francois  (1001) francois  (1001)     1072 2022-12-12 11:28:08.000000 lampe-0.8.0/LICENSE
+-rw-rw-r--   0 francois  (1001) francois  (1001)     2480 2023-06-14 14:34:00.887271 lampe-0.8.0/PKG-INFO
+-rw-rw-r--   0 francois  (1001) francois  (1001)     1707 2023-01-21 11:58:25.000000 lampe-0.8.0/README.md
+drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-06-14 14:34:00.883270 lampe-0.8.0/lampe/
+-rw-rw-r--   0 francois  (1001) francois  (1001)      166 2023-06-14 14:32:55.000000 lampe-0.8.0/lampe/__init__.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)    11153 2023-06-14 14:17:00.000000 lampe-0.8.0/lampe/data.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     5120 2023-06-14 14:17:00.000000 lampe-0.8.0/lampe/diagnostics.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)    27622 2023-06-14 14:23:38.000000 lampe-0.8.0/lampe/inference.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     3131 2022-12-14 21:21:35.000000 lampe-0.8.0/lampe/masks.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     2532 2023-03-20 17:12:34.000000 lampe-0.8.0/lampe/nn.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)    13107 2023-06-14 14:17:00.000000 lampe-0.8.0/lampe/plots.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     3201 2023-03-20 17:12:34.000000 lampe-0.8.0/lampe/utils.py
+drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-06-14 14:34:00.883270 lampe-0.8.0/lampe.egg-info/
+-rw-rw-r--   0 francois  (1001) francois  (1001)     2480 2023-06-14 14:34:00.000000 lampe-0.8.0/lampe.egg-info/PKG-INFO
+-rw-rw-r--   0 francois  (1001) francois  (1001)      472 2023-06-14 14:34:00.000000 lampe-0.8.0/lampe.egg-info/SOURCES.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)        1 2023-06-14 14:34:00.000000 lampe-0.8.0/lampe.egg-info/dependency_links.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)       83 2023-06-14 14:34:00.000000 lampe-0.8.0/lampe.egg-info/requires.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)        6 2023-06-14 14:34:00.000000 lampe-0.8.0/lampe.egg-info/top_level.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)       83 2023-06-14 14:17:00.000000 lampe-0.8.0/requirements.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)      870 2023-06-14 14:34:00.887271 lampe-0.8.0/setup.cfg
+-rw-rw-r--   0 francois  (1001) francois  (1001)       73 2023-06-14 14:17:00.000000 lampe-0.8.0/setup.py
+drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-06-14 14:34:00.887271 lampe-0.8.0/tests/
+-rw-rw-r--   0 francois  (1001) francois  (1001)     4653 2023-03-20 17:12:34.000000 lampe-0.8.0/tests/test_data.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     1969 2022-12-14 21:21:35.000000 lampe-0.8.0/tests/test_diagnostics.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     4253 2023-06-14 14:23:38.000000 lampe-0.8.0/tests/test_inference.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)      974 2022-12-14 21:21:35.000000 lampe-0.8.0/tests/test_masks.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)      348 2022-12-14 21:21:35.000000 lampe-0.8.0/tests/test_nn.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)      928 2022-12-14 21:21:35.000000 lampe-0.8.0/tests/test_plots.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     1749 2023-02-28 11:00:57.000000 lampe-0.8.0/tests/test_utils.py
```

### Comparing `lampe-0.7.3/LICENSE` & `lampe-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lampe-0.7.3/PKG-INFO` & `lampe-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 Metadata-Version: 2.1
 Name: lampe
-Version: 0.7.3
+Version: 0.8.0
 Summary: Likelihood-free AMortized Posterior Estimation with PyTorch
-Home-page: https://github.com/francois-rozet/lampe
 Author: François Rozet
 Author-email: francois.rozet@outlook.com
-License: MIT License
 Project-URL: Documentation, https://lampe.readthedocs.io
 Project-URL: Source, https://github.com/francois-rozet/lampe
 Project-URL: Tracker, https://github.com/francois-rozet/lampe/issues
 Keywords: torch,simulation-based,inference,amortized,bayesian,posterior,likelihood,mcmc
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `lampe-0.7.3/README.md` & `lampe-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `lampe-0.7.3/lampe/data.py` & `lampe-0.8.0/lampe/data.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         ...     something(theta, x)
     """
 
     def __init__(
         self,
         prior: Distribution,
         simulator: Callable,
-        batch_size: int = 2**10,  # 1024
+        batch_size: int = 2**8,  # 256
         vectorized: bool = False,
         numpy: bool = False,
         **kwargs,
     ):
         super().__init__(
             IterableJointDataset(
                 prior,
@@ -154,33 +154,32 @@
                 return zip(
                     self.theta.split(self.batch_size),
                     self.x.split(self.batch_size),
                 )
 
 
 class H5Dataset(IterableDataset):
-    r"""Creates an iterable dataset of pairs :math:`(\theta, x)` from HDF5 files.
+    r"""Creates an iterable dataset of pairs :math:`(\theta, x)` from an HDF5 file.
 
     As it can be slow to load pairs from disk one by one, :class:`H5Dataset` implements
     a custom :meth:`__iter__` method that loads several contiguous chunks of pairs at
-    once and shuffles their concatenation before yielding the pairs one by one,
-    unless a batch size is provided.
+    once and shuffles their concatenation before yielding the pairs.
 
     :class:`H5Dataset` also implements the :meth:`__len__` and :meth:`__getitem__`
     methods for convenience.
 
     Important:
         When using :class:`H5Dataset` with :class:`torch.utils.data.DataLoader`, it is
         recommended to disable the loader's automatic batching and provide the batch
         size to the dataset, as it significantly improves loading performances.
         In fact, unless using several workers or memory pinning, it is not even
         necessary to wrap the dataset in a :class:`torch.utils.data.DataLoader`.
 
     Arguments:
-        files: HDF5 files containing pairs :math:`(\theta, x)`.
+        file: An HDF5 file containing pairs :math:`(\theta, x)`.
         batch_size: The size of the batches.
         chunk_size: The size of the contiguous chunks.
         chunk_step: The number of chunks loaded at once.
         shuffle: Whether the pairs are shuffled or not when iterating.
 
     Example:
         >>> dataset = H5Dataset('data.h5', batch_size=256, shuffle=True)
@@ -190,62 +189,61 @@
         >>> for theta, x in dataset:
         ...     theta, x = theta.cuda(), x.cuda()
         ...     something(theta, x)
     """
 
     def __init__(
         self,
-        *files: Union[str, Path],
+        file: Union[str, Path],
         batch_size: int = None,
-        chunk_size: int = 2**10,  # 1024
+        chunk_size: int = 2**8,  # 256
         chunk_step: str = 2**8,  # 256
         shuffle: bool = False,
     ):
         super().__init__()
 
-        self.files = [h5py.File(f, mode='r') for f in files]
-        self.sizes = [f['theta'].shape[0] for f in self.files]
-        self.cumsizes = np.cumsum(self.sizes)
+        self.file = h5py.File(file, mode='r')
 
         self.batch_size = batch_size
         self.chunk_size = chunk_size
         self.chunk_step = chunk_step
         self.shuffle = shuffle
 
     def __len__(self) -> int:
-        return self.cumsizes[-1]
+        return len(self.file['theta'])
 
-    def __getitem__(self, i: int) -> Tuple[Tensor, Tensor]:
-        i = i % len(self)
-        j = bisect(self.cumsizes, i)
-        if j > 0:
-            i = i - self.cumsizes[j - 1]
-
-        f = self.files[j]
-        theta, x = f['theta'][i], f['x'][i]
+    def __getitem__(self, i: Union[int, slice]) -> Tuple[Tensor, Tensor]:
+        theta, x = self.file['theta'][i], self.file['x'][i]
 
         return torch.from_numpy(theta), torch.from_numpy(x)
 
     def __iter__(self) -> Iterator[Tuple[Tensor, Tensor]]:
         chunks = torch.tensor([
-            (i, j, j + self.chunk_size)
-            for i, size in enumerate(self.sizes)
-            for j in range(0, size, self.chunk_size)
+            (i, i + self.chunk_size)
+            for i in range(0, len(self), self.chunk_size)
         ])
 
         if self.shuffle:
             order = torch.randperm(len(chunks))
             chunks = chunks[order]
 
         for slices in chunks.split(self.chunk_step):
+            # Merge contiguous slices
             slices = sorted(slices.tolist())
+            stack = []
+
+            for s in slices:
+                if stack and stack[-1][-1] == s[0]:
+                    stack[-1][-1] = s[-1]
+                else:
+                    stack.append(s)
 
             # Load
-            theta = np.concatenate([self.files[i]['theta'][j:k] for i, j, k in slices])
-            x = np.concatenate([self.files[i]['x'][j:k] for i, j, k in slices])
+            theta = np.concatenate([self.file['theta'][i:j] for i, j in stack])
+            x = np.concatenate([self.file['x'][i:j] for i, j in stack])
 
             theta, x = torch.from_numpy(theta), torch.from_numpy(x)
 
             # Shuffle
             if self.shuffle:
                 order = torch.randperm(len(theta))
                 theta, x = theta[order], x[order]
@@ -262,20 +260,17 @@
     def to_memory(self) -> JointDataset:
         r"""Loads all pairs in memory and returns them as a :class:`JointDataset`.
 
         Example:
             >>> dataset = H5Dataset('data.h5').to_memory()
         """
 
-        theta = np.concatenate([f['theta'][:] for f in self.files])
-        x = np.concatenate([f['x'][:] for f in self.files])
-
         return JointDataset(
-            theta,
-            x,
+            self.file['theta'][:],
+            self.file['x'][:],
             batch_size=self.batch_size,
             shuffle=self.shuffle,
         )
 
     @staticmethod
     def store(
         pairs: Iterable[Tuple[Array, Array]],
```

### Comparing `lampe-0.7.3/lampe/diagnostics.py` & `lampe-0.8.0/lampe/diagnostics.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,20 +10,21 @@
 from .utils import gridapply
 
 
 def expected_coverage_mc(
     posterior: Callable[[Tensor], Distribution],
     pairs: Iterable[Tuple[Tensor, Tensor]],
     n: int = 1024,
+    device: str = None,
 ) -> Tuple[Tensor, Tensor]:
     r"""Estimates by Monte Carlo (MC) the expected coverages of a posterior estimator
     :math:`q(\theta | x)` over pairs :math:`(\theta^*, x^*) \sim p(\theta, x)`.
 
-    The expected coverage at credible level :math:`1 - \alpha` is the probability
-    of :math:`\theta^*` to be included in the highest density region of total probability
+    The expected coverage at credible level :math:`1 - \alpha` is the probability of
+    :math:`\theta^*` to be included in the highest density region of total probability
     :math:`1 - \alpha` of the posterior :math:`q(\theta | x^*)`, denoted
     :math:`\Theta_{q(\theta | x^*)}(1 - \alpha)`. To get the coverages, the proportion
     :math:`r^*` of samples :math:`\theta \sim q(\theta | x^*)` having a higher estimated
     density than :math:`\theta^*` is computed for each pair :math:`(\theta^*, x^*)`.
     Formally,
 
     .. math:: r^* = \mathbb{E}_{q(\theta | x^*)}
@@ -41,86 +42,97 @@
         | Averting A Crisis In Simulation-Based Inference (Hermans et al., 2021)
         | https://arxiv.org/abs/2110.06581
 
     Arguments:
         posterior: A posterior estimator :math:`q(\theta | x)`.
         pairs: An iterable of pairs :math:`(\theta^*, x^*) \sim p(\theta, x)`.
         n: The number of samples to draw from the posterior for each pair.
+        device: The device on which the computations are performed.
 
     Returns:
         A vector of increasing credible levels and their respective expected coverages.
 
     Example:
         >>> posterior = lampe.inference.NPE(3, 4)
         >>> testset = lampe.data.H5Dataset('test.h5')
         >>> levels, coverages = expected_coverage_mc(posterior.flow, testset)
     """
 
     ranks = []
 
     with torch.no_grad():
         for theta, x in tqdm(pairs, unit='pair'):
-            dist = posterior(x)
+            if device is not None:
+                theta, x = theta.to(device), x.to(device)
 
+            dist = posterior(x)
             samples = dist.sample((n,))
             mask = dist.log_prob(theta) < dist.log_prob(samples)
             rank = mask.sum() / mask.numel()
 
             ranks.append(rank)
 
     ranks = torch.stack(ranks).cpu()
-    ranks = torch.cat((ranks, torch.tensor([0.0, 1.0])))
+    ranks = torch.cat((ranks, ranks.new_tensor((0.0, 1.0))))
 
     return (
         torch.sort(ranks).values,
-        torch.linspace(0.0, 1.0, len(ranks)),
+        torch.linspace(0, 1, len(ranks)),
     )
 
 
 def expected_coverage_ni(
-    posterior: Callable[[Tensor, Tensor], Tensor],
+    log_p: Callable[[Tensor, Tensor], Tensor],
     pairs: Iterable[Tuple[Tensor, Tensor]],
     domain: Tuple[Tensor, Tensor],
+    device: str = None,
     **kwargs,
 ) -> Tuple[Tensor, Tensor]:
     r"""Estimates by numerical integration (NI) the expected coverages of a posterior
     estimator :math:`q(\theta | x)` over pairs :math:`(\theta^*, x^*) \sim p(\theta, x)`.
 
     Equivalent to :func:`expected_coverage_mc` but the proportions :math:`r^*` are
     approximated by numerical integration over the domain, which is useful when the
     posterior estimator can be evaluated but not be sampled from.
 
     Arguments:
-        posterior: A posterior estimator :math:`\log q(\theta | x)`.
+        log_p: A log-posterior estimator :math:`\log q(\theta | x)`.
         pairs: An iterable of pairs :math:`(\theta^*, x^*) \sim p(\theta, x)`.
         domain: A pair of lower and upper domain bounds for :math:`\theta`.
+        device: The device on which the computations are performed.
         kwargs: Keyword arguments passed to :func:`lampe.utils.gridapply`.
 
     Returns:
         A vector of increasing credible levels and their respective expected coverages.
 
     Example:
         >>> domain = (torch.zeros(3), torch.ones(3))
         >>> prior = lampe.distributions.BoxUniform(*domain)
         >>> ratio = lampe.inference.NRE(3, 4)
-        >>> posterior = lambda theta, x: ratio(theta, x) + prior.log_prob(theta)
+        >>> log_p = lambda theta, x: ratio(theta, x) + prior.log_prob(theta)
         >>> testset = lampe.data.H5Dataset('test.h5')
-        >>> levels, coverages = expected_coverage_ni(posterior, testset, domain)
+        >>> levels, coverages = expected_coverage_ni(log_p, testset, domain)
     """
 
+    if device is not None:
+        domain = tuple(bound.to(device) for bound in domain)
+
     ranks = []
 
     with torch.no_grad():
         for theta, x in tqdm(pairs, unit='pair'):
-            _, log_probs = gridapply(lambda theta: posterior(theta, x), domain, **kwargs)
-            mask = posterior(theta, x) < log_probs
-            rank = log_probs[mask].logsumexp(dim=0) - log_probs.flatten().logsumexp(dim=0)
+            if device is not None:
+                theta, x = theta.to(device), x.to(device)
+
+            _, log_ps = gridapply(lambda theta: log_p(theta, x), domain, **kwargs)
+            mask = log_p(theta, x) < log_ps
+            rank = log_ps[mask].logsumexp(dim=0) - log_ps.flatten().logsumexp(dim=0)
 
             ranks.append(rank.exp())
 
     ranks = torch.stack(ranks).cpu()
-    ranks = torch.cat((ranks, torch.tensor([0.0, 1.0])))
+    ranks = torch.cat((ranks, ranks.new_tensor((0.0, 1.0))))
 
     return (
         torch.sort(ranks).values,
-        torch.linspace(0.0, 1.0, len(ranks)),
+        torch.linspace(0, 1, len(ranks)),
     )
```

### Comparing `lampe-0.7.3/lampe/inference.py` & `lampe-0.8.0/lampe/inference.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 r"""Inference components such as estimators, training losses and MCMC samplers."""
 
 __all__ = [
     'NRE',
     'NRELoss',
     'BNRELoss',
+    'CNRELoss',
+    'BCNRELoss',
     'AMNRE',
     'AMNRELoss',
     'NPE',
     'NPELoss',
-    'AMNPE',
-    'AMNPELoss',
-    'NSE',
-    'NSELoss',
+    'FMPE',
+    'FMPELoss',
     'MetropolisHastings',
 ]
 
 import math
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
@@ -29,15 +29,15 @@
 from zuko.transforms import FreeFormJacobianTransform
 from zuko.utils import broadcast
 
 from .nn import MLP
 
 
 class NRE(nn.Module):
-    r"""Creates a neural ratio estimation (NRE) classifier network.
+    r"""Creates a neural ratio estimation (NRE) network.
 
     The principle of neural ratio estimation is to train a classifier network
     :math:`d_\phi(\theta, x)` to discriminate between pairs :math:`(\theta, x)` equally
     sampled from the joint distribution :math:`p(\theta, x)` and the product of the
     marginals :math:`p(\theta)p(x)`. Formally, the optimization problem is
 
     .. math:: \arg\min_\phi
@@ -99,25 +99,25 @@
 
         theta, x = broadcast(theta, x, ignore=1)
 
         return self.net(torch.cat((theta, x), dim=-1)).squeeze(-1)
 
 
 class NRELoss(nn.Module):
-    r"""Creates a module that calculates the cross-entropy loss for a NRE classifier.
+    r"""Creates a module that calculates the cross-entropy loss for a NRE network.
 
-    Given a batch of :math:`N` pairs :math:`(\theta_i, x_i)`, the module returns
+    Given a batch of :math:`N \geq 2` pairs :math:`(\theta_i, x_i)`, the module returns
 
     .. math:: l = \frac{1}{2N} \sum_{i = 1}^N
         \ell(d_\phi(\theta_i, x_i)) + \ell(1 - d_\phi(\theta_{i+1}, x_i))
 
     where :math:`\ell(p) = -\log p` is the negative log-likelihood.
 
     Arguments:
-        estimator: A classifier network :math:`d_\phi(\theta, x)`.
+        estimator: A log-ratio network :math:`\log r_\phi(\theta, x)`.
     """
 
     def __init__(self, estimator: nn.Module):
         super().__init__()
 
         self.estimator = estimator
 
@@ -142,32 +142,32 @@
         l0 = -F.logsigmoid(-log_r_prime).mean()
 
         return (l1 + l0) / 2
 
 
 class BNRELoss(nn.Module):
     r"""Creates a module that calculates the balanced cross-entropy loss for a balanced
-    NRE (BNRE) classifier.
+    NRE (BNRE) network.
 
-    Given a batch of :math:`N` pairs :math:`(\theta_i, x_i)`, the module returns
+    Given a batch of :math:`N \geq 2` pairs :math:`(\theta_i, x_i)`, the module returns
 
     .. math::
         l & = \frac{1}{2N} \sum_{i = 1}^N
             \ell(d_\phi(\theta_i, x_i)) + \ell(1 - d_\phi(\theta_{i+1}, x_i)) \\
           & + \lambda \left(1 - \frac{1}{N} \sum_{i = 1}^N
             d_\phi(\theta_i, x_i) + d_\phi(\theta_{i+1}, x_i) \right)^2
 
     where :math:`\ell(p) = -\log p` is the negative log-likelihood.
 
     References:
         | Towards Reliable Simulation-Based Inference with Balanced Neural Ratio Estimation (Delaunoy et al., 2022)
         | https://arxiv.org/abs/2208.13624
 
     Arguments:
-        estimator: A classifier network :math:`d_\phi(\theta, x)`.
+        estimator: A log-ratio network :math:`\log r_\phi(\theta, x)`.
         lmbda: The weight :math:`\lambda` controlling the strength of the balancing
             condition.
     """
 
     def __init__(self, estimator: nn.Module, lmbda: float = 100.0):
         super().__init__()
 
@@ -194,17 +194,177 @@
         l1 = -F.logsigmoid(log_r).mean()
         l0 = -F.logsigmoid(-log_r_prime).mean()
         lb = (torch.sigmoid(log_r) + torch.sigmoid(log_r_prime) - 1).mean().square()
 
         return (l1 + l0) / 2 + self.lmbda * lb
 
 
+class CNRELoss(nn.Module):
+    r"""Creates a module that calculates the cross-entropy loss for a contrastive NRE
+    (CNRE) network.
+
+    The principle of contrastive neural ratio estimation (CNRE) is to predict whether a
+    set :math:`\Theta = \{\theta^1, \dots, \theta^K\}` contains or not the parameters
+    that originated an observation :math:`x`. The elements of :math:`\Theta` are drawn
+    independently from the prior :math:`p(\theta)` and the element :math:`\theta^k` that
+    originates the observation :math:`x \sim p(x | \theta^k)` is chosen uniformly within
+    :math:`\Theta`, such that
+
+    .. math:: p(\Theta, x)
+        & = p(\Theta) \, p(x | \Theta) \\
+        & = p(\Theta) \frac{1}{K} \sum_{k = 1}^K p(x | \theta^k) \\
+        & = p(\Theta) \, p(x) \frac{1}{K} \sum_{k = 1}^K r(\theta^k, x)
+
+    where :math:`r(\theta, x)` is the likelihood-to-evidence (LTE) ratio. The task
+    is to discriminate between pairs :math:`(\Theta, x)` for which :math:`\Theta` either
+    does or does not contain the nominal parameters of :math:`x`, similar to the
+    original NRE optimization problem. For this task, the decision function
+    modeling the Bayes optimal classifier is
+
+    .. math:: d(\Theta, x)
+        = \frac{p(\Theta, x)}{p(\Theta, x) + \frac{1}{\gamma} p(\Theta) p(x)}
+        = \frac{\sum_{k = 1}^K r(\theta^k, x)}{\frac{K}{\gamma} + \sum_{k = 1}^K r(\theta^k, x)} \, ,
+
+    where :math:`\gamma \in \mathbb{R}^+` are the odds of :math:`\Theta` containing to
+    not containing the nominal parameters. Consequently, a classifier
+    :math:`d_\phi(\Theta, x)` can be equivalently replaced and trained as a composition
+    of ratios :math:`r_\phi(\theta^k, x)`. Eventually, given a batch of :math:`N \geq
+    2K` pairs :math:`(\theta_i, x_i)`, the module returns
+
+    .. math:: l = \frac{1}{N} \sum_{i = 1}^N
+        \frac{\gamma}{\gamma + 1} \ell(d_\phi(\Theta_i, x_i))
+        + \frac{1}{\gamma + 1} \ell(1 - d_\phi(\Theta_{i+K}, x_i))
+
+    where :math:`\ell(p) = -\log p` is the negative log-likelihood and :math:`\Theta_i =
+    \{\theta_i, \dots, \theta_{i+K-1}\}`.
+
+    Note:
+        The quantity :math:`d_\phi(\Theta, x)` corresponds to :math:`q_\phi(y \neq 0 |
+        \Theta, x)` or :math:`1 - q_\phi(y = 0 | \Theta, x)` in the notations of Miller
+        et al. (2022).
+
+    References:
+        | Contrastive Neural Ratio Estimation (Miller et al., 2022)
+        | https://arxiv.org/abs/2210.06170
+
+    Arguments:
+        estimator: A log-ratio network :math:`\log r_\phi(\theta, x)`.
+        cardinality: The cardinality :math:`K` of :math:`\Theta`.
+        gamma: The odds ratio :math:`\gamma`.
+    """
+
+    def __init__(
+        self,
+        estimator: nn.Module,
+        cardinality: int = 2,
+        gamma: float = 1.0,
+    ):
+        super().__init__()
+
+        self.estimator = estimator
+        self.cardinality = cardinality
+        self.gamma = gamma
+
+    def logits(self, theta: Tensor, x: Tensor) -> Tensor:
+        theta = torch.cat((theta, theta[:self.cardinality - 1]), dim=0)
+        theta = theta.unfold(0, self.cardinality, 1)
+        theta = theta.movedim(-1, 0)
+
+        theta_prime = torch.roll(theta, self.cardinality, dims=1)
+
+        log_r, log_r_prime = self.estimator(
+            torch.stack((theta, theta_prime)),
+            x,
+        )
+
+        shift = math.log(self.gamma / self.cardinality)
+
+        log_r = torch.logsumexp(log_r, dim=0) + shift
+        log_r_prime = torch.logsumexp(log_r_prime, dim=0) + shift
+
+        return log_r, log_r_prime
+
+    def forward(self, theta: Tensor, x: Tensor) -> Tensor:
+        r"""
+        Arguments:
+            theta: The parameters :math:`\theta`, with shape :math:`(N, D)`.
+            x: The observation :math:`x`, with shape :math:`(N, L)`.
+
+        Returns:
+            The scalar loss :math:`l`.
+        """
+
+        log_r, log_r_prime = self.logits(theta, x)
+
+        l1 = -F.logsigmoid(log_r).mean()
+        l0 = -F.logsigmoid(-log_r_prime).mean()
+
+        return (self.gamma * l1 + l0) / (self.gamma + 1)
+
+
+class BCNRELoss(CNRELoss):
+    r"""Creates a module that calculates the balanced cross-entropy loss for a balanced
+    CNRE (BCNRE) network.
+
+    Given a batch of :math:`N \geq 2K` pairs :math:`(\theta_i, x_i)`, the module returns
+
+    .. math::
+        l & = \frac{1}{N} \sum_{i = 1}^N
+            \frac{\gamma}{\gamma + 1} \ell(d_\phi(\Theta_i, x_i))
+            + \frac{1}{\gamma + 1} \ell(1 - d_\phi(\Theta_{i+K}, x_i)) \\
+          & + \lambda \left(1 - \frac{1}{N} \sum_{i = 1}^N
+            d_\phi(\Theta_i, x_i) + d_\phi(\Theta_{i+K}, x_i) \right)^2
+
+    where :math:`\ell(p) = -\log p` is the negative log-likelihood and :math:`\Theta_i =
+    \{\theta_i, \dots, \theta_{i+K-1}\}`.
+
+    References:
+        | Balancing Simulation-based Inference for Conservative Posteriors (Delaunoy et al., 2023)
+        | https://arxiv.org/abs/2304.10978
+
+    Arguments:
+        estimator: A log-ratio network :math:`\log r_\phi(\theta, x)`.
+        cardinality: The cardinality :math:`K` of :math:`\Theta`.
+        gamma: The odds ratio :math:`\gamma`.
+        lmbda: The weight :math:`\lambda` controlling the strength of the balancing
+            condition.
+    """
+
+    def __init__(
+        self,
+        estimator: nn.Module,
+        cardinality: int = 2,
+        gamma: float = 1.0,
+        lmbda: float = 100.0,
+    ):
+        super().__init__(estimator, cardinality, gamma)
+
+        self.lmbda = lmbda
+
+    def forward(self, theta: Tensor, x: Tensor) -> Tensor:
+        r"""
+        Arguments:
+            theta: The parameters :math:`\theta`, with shape :math:`(N, D)`.
+            x: The observation :math:`x`, with shape :math:`(N, L)`.
+
+        Returns:
+            The scalar loss :math:`l`.
+        """
+
+        log_r, log_r_prime = self.logits(theta, x)
+
+        l1 = -F.logsigmoid(log_r).mean()
+        l0 = -F.logsigmoid(-log_r_prime).mean()
+        lb = (torch.sigmoid(log_r) + torch.sigmoid(log_r_prime) - 1).mean().square()
+
+        return (self.gamma * l1 + l0) / (self.gamma + 1) + self.lmbda * lb
+
+
 class AMNRE(NRE):
-    r"""Creates an arbitrary marginal neural ratio estimation (AMNRE) classifier
-    network.
+    r"""Creates an arbitrary marginal neural ratio estimation (AMNRE) network.
 
     The principle of AMNRE is to introduce, as input to the classifier, a binary mask
     :math:`b \in \{0, 1\}^D` indicating a subset of parameters :math:`\theta_b =
     (\theta_i: b_i = 1)` of interest. Intuitively, this allows the classifier to
     distinguish subspaces and to learn a different ratio for each of them. Formally, the
     classifier network takes the form :math:`d_\phi(\theta_b, x, b)` and the
     optimization problem becomes
@@ -262,26 +422,26 @@
 
         theta, x, b = broadcast(theta * b, x, b * 2.0 - 1.0, ignore=1)
 
         return self.net(torch.cat((theta, x, b), dim=-1)).squeeze(-1)
 
 
 class AMNRELoss(nn.Module):
-    r"""Creates a module that calculates the cross-entropy loss for an AMNRE classifier.
+    r"""Creates a module that calculates the cross-entropy loss for an AMNRE network.
 
-    Given a batch of :math:`N` pairs :math:`(\theta_i, x_i)`, the module returns
+    Given a batch of :math:`N \geq 2` pairs :math:`(\theta_i, x_i)`, the module returns
 
     .. math:: l = \frac{1}{2N} \sum_{i = 1}^N
         \ell(d_\phi(\theta_i \odot b_i, x_i, b_i)) +
         \ell(1 - d_\phi(\theta_{i+1} \odot b_i, x_i, b_i))
 
     where the binary masks :math:`b_i` are sampled from a distribution :math:`P(b)`.
 
     Arguments:
-        estimator: A classifier network :math:`d_\phi(\theta, x, b)`.
+        estimator: A log-ratio network :math:`\log r_\phi(\theta, x, b)`.
         mask_dist: A binary mask distribution :math:`P(b)`.
     """
 
     def __init__(
         self,
         estimator: nn.Module,
         mask_dist: Distribution,
@@ -370,28 +530,14 @@
             The log-density :math:`\log p_\phi(\theta | x)`, with shape :math:`(*,)`.
         """
 
         theta, x = broadcast(theta, x, ignore=1)
 
         return self.flow(x).log_prob(theta)
 
-    def sample(self, x: Tensor, shape: Size = ()) -> Tensor:
-        r"""
-        Arguments:
-            x: The observation :math:`x`, with shape :math:`(*, L)`.
-            shape: The shape :math:`S` of the samples.
-
-        Returns:
-            The samples :math:`\theta \sim p_\phi(\theta | x)`,
-            with shape :math:`S + (*, D)`.
-        """
-
-        with torch.no_grad():
-            return self.flow(x).sample(shape)
-
 
 class NPELoss(nn.Module):
     r"""Creates a module that calculates the negative log-likelihood loss for a NPE
     normalizing flow.
 
     Given a batch of :math:`N` pairs :math:`(\theta_i, x_i)`, the module returns
 
@@ -417,153 +563,32 @@
         """
 
         log_p = self.estimator(theta, x)
 
         return -log_p.mean()
 
 
-class AMNPE(NPE):
-    r"""Creates an arbitrary marginal neural posterior estimation (AMNPE)
-    normalizing flow.
+class FMPE(nn.Module):
+    r"""Creates a flow matching posterior estimation (FMPE) network.
 
-    TODO
-
-    Arguments:
-        theta_dim: The dimensionality :math:`D` of the parameter space.
-        x_dim: The dimensionality :math:`L` of the observation space.
-        args: Positional arguments passed to :class:`NPE`.
-        kwargs: Keyword arguments passed to :class:`NPE`.
-    """
-
-    def __init__(
-        self,
-        theta_dim: int,
-        x_dim: int,
-        *args,
-        **kwargs,
-    ):
-        super().__init__(theta_dim, x_dim + theta_dim, *args, **kwargs)
-
-    def forward(self, theta: Tensor, x: Tensor, b: BoolTensor) -> Tensor:
-        r"""
-        Arguments:
-            theta: The parameters :math:`\theta`, with shape :math:`(*, D)`.
-            x: The observation :math:`x`, with shape :math:`(*, L)`.
-            b: A binary mask :math:`b`, with shape :math:`(*, D)`.
-
-        Returns:
-            The log-density :math:`\log p_\phi(\theta | x, b)`, with shape :math:`(*,)`.
-        """
-
-        theta, x, b = broadcast(theta, x, b * 2.0 - 1.0, ignore=1)
-
-        return self.flow(torch.cat((x, b), dim=-1)).log_prob(theta)
-
-    def sample(self, x: Tensor, b: BoolTensor, shape: Size = ()) -> Tensor:
-        r"""
-        Arguments:
-            x: The observation :math:`x`, with shape :math:`(*, L)`.
-            b: A binary mask :math:`b`, with shape :math:`(D,)`.
-            shape: The shape :math:`S` of the samples.
-
-        Returns:
-            The samples :math:`\theta_b \sim p_\phi(\theta_b | x, b)`,
-            with shape :math:`S + (*, D)`.
-        """
-
-        x, b_ = broadcast(x, b * 2.0 - 1.0, ignore=1)
-
-        with torch.no_grad():
-            return self.flow(torch.cat((x, b_), dim=-1)).sample(shape)[..., b]
-
-
-class AMNPELoss(nn.Module):
-    r"""Creates a module that calculates the negative log-likelihood loss for an AMNPE
-    normalizing flow.
-
-    Given a batch of :math:`N` pairs :math:`(\theta_i, x_i)`, the module returns
-
-    .. math:: l = \frac{1}{N} \sum_{i = 1}^N
-        -\log p_\phi(\theta_i \odot b_i + \theta_{i + 1} \odot (1 - b_i) | x_i, b_i)
-
-    where the binary masks :math:`b_i` are sampled from a distribution :math:`P(b)`.
-
-    Arguments:
-        estimator: A normalizing flow :math:`p_\phi(\theta | x, b)`.
-        mask_dist: A binary mask distribution :math:`P(b)`.
-    """
-
-    def __init__(
-        self,
-        estimator: nn.Module,
-        mask_dist: Distribution,
-    ):
-        super().__init__()
-
-        self.estimator = estimator
-        self.mask_dist = mask_dist
-
-    def forward(self, theta: Tensor, x: Tensor) -> Tensor:
-        r"""
-        Arguments:
-            theta: The parameters :math:`\theta`, with shape :math:`(N, D)`.
-            x: The observation :math:`x`, with shape :math:`(N, L)`.
-
-        Returns:
-            The scalar loss :math:`l`.
-        """
-
-        theta_prime = torch.roll(theta, 1, dims=0)
-
-        b = self.mask_dist.sample(theta.shape[:-1])
-        theta = torch.where(b, theta, theta_prime)
-
-        log_prob = self.estimator(theta, x, b)
-
-        return -log_prob.mean()
-
-
-class NSE(nn.Module):
-    r"""Creates a neural score estimation (NSE) regression network.
-
-    The principle of neural score estimation is to train a regression network
-    :math:`s_\phi(\theta_t, x, t)` to approximate the score :math:`\nabla_{\! \theta_t}
-    \log p(\theta_t | x)` of the sub-variance preserving (sub-VP) diffusion process
-
-    .. math:: \mathrm{d} \theta_t = -\frac{1}{2} \beta(t) \theta_t \, \mathrm{d} t +
-        \sqrt{\beta(t) (1 - \alpha(t)^2)} \, \mathrm{d} w
-
-    where :math:`\alpha(t) = \exp(-\int_0^t \beta(u) \, \mathrm{d} u)` and
-    :math:`\beta(t) = (\beta_\max - \beta_\min) \, t + \beta_\min` . The optimization
-    problem is to minimize the rescaled score-matching objective, that is,
-
-    .. math:: \arg\min_\phi \mathbb{E}_{p(\theta, x) p(t) p(\theta_t | \theta)}
-        \Big[ \big\| s_\phi(\theta_t, x, t) - (1 - \alpha(t)) \nabla_{\! \theta_t}
-        \log p(\theta_t | \theta) \big\|_2^2 \Big]
-
-    where :math:`p(\theta_t | \theta) = \mathcal{N}(\theta_t; \sqrt{\alpha(t)} \,
-    \theta, (1 - \alpha(t))^2 I)` is the perturbation kernel corresponding to the
-    diffusion process and for which the optimal regressor is the rescaled score
-
-    .. math:: s(\theta_t, x, t) =
-        (1 - \alpha(t)) \nabla_{\! \theta_t} \log p(\theta_t | x) .
-
-    Given the latter, or an estimator of the latter, the probability flow ODE
-
-    .. math:: \mathrm{d} \theta_t =
-        \left[ -\frac{1}{2} \beta(t) \theta_t - \frac{1}{2} \beta(t) (1 + \alpha(t))
-        s(\theta_t, x, t) \right] \, \mathrm{d} t
-
-    shares the same marginal densities :math:`p(\theta_t | x)` as the diffusion process
-    and can be efficiently integrated (forward for log-density computation and backward
-    for sampling) with black-box ODE solvers.
+    The principle of FMPE is to train a regression network :math:`v_\phi(\theta, x, t)`
+    to approximate a vector field inducing a time-continuous normalizing flow between
+    the posterior distribution :math:`p(\theta | x)` and a standard Gaussian
+    distribution :math:`\mathcal{N}(0, I)`.
+
+    After training, the normalizing flow :math:`p_\phi(\theta | x)` induced by
+    :math:`v_\phi(\theta, x, t)` is used to evaluate the posterior density or generate
+    samples.
 
     References:
-        | Score-Based Generative Modeling through Stochastic Differential Equations (Song et al., 2021)
-        | https://arxiv.org/abs/2011.13456
+        | Flow Matching for Generative Modeling (Lipman et al., 2023)
+        | https://arxiv.org/abs/2210.02747
+
+        | Flow Matching for Scalable Simulation-Based Inference (Dax et al., 2023)
+        | https://arxiv.org/abs/2305.17161
 
     Arguments:
         theta_dim: The dimensionality :math:`D` of the parameter space.
         x_dim: The dimensionality :math:`L` of the observation space.
         freqs: The number of time embedding frequencies.
         build: The network constructor (e.g. :class:`lampe.nn.ResMLP`). It takes the
             number of input and output features as positional arguments.
@@ -590,97 +615,84 @@
         r"""
         Arguments:
             theta: The parameters :math:`\theta`, with shape :math:`(*, D)`.
             x: The observation :math:`x`, with shape :math:`(*, L)`.
             t: The time :math:`t`, with shape :math:`(*,).`
 
         Returns:
-            The rescaled score :math:`s_\phi(\theta, x, t)`, with shape :math:`(*, D)`.
+            The vector field :math:`v_\phi(\theta, x, t)`, with shape :math:`(*, D)`.
         """
 
         t = self.freqs * t[..., None]
         t = torch.cat((t.cos(), t.sin()), dim=-1)
 
         theta, x, t = broadcast(theta, x, t, ignore=1)
 
         return self.net(torch.cat((theta, x, t), dim=-1))
 
-    def alpha(self, t: Tensor) -> Tensor:
-        return torch.exp(-8.0 * t**2)
-
-    def beta(self, t: Tensor) -> Tensor:
-        return 16.0 * t
-
-    def ode(self, theta: Tensor, x: Tensor, t: Tensor) -> Tensor:
-        alpha, beta = self.alpha(t), self.beta(t)
-        score = self.forward(theta, x, t)
-
-        return -beta / 2 * (theta + (1 + alpha) * score)
-
     def flow(self, x: Tensor) -> Distribution:
         r"""
         Arguments:
             x: The observation :math:`x`, with shape :math:`(*, L)`.
 
         Returns:
-            The posterior distribution :math:`p_\phi(\theta | x)` induced by the
-            probability flow ODE.
+            The normalizing flow :math:`p_\phi(\theta | x)`.
         """
 
         return NormalizingFlow(
             transform=FreeFormJacobianTransform(
-                f=lambda t, theta: self.ode(theta, x, t),
-                time=x.new_tensor(1.0),
+                f=lambda t, theta: self(theta, x, t),
+                t0=x.new_tensor(0.0),
+                t1=x.new_tensor(1.0),
                 phi=(x, *self.parameters()),
             ),
             base=DiagNormal(self.zeros, self.ones).expand(x.shape[:-1]),
         )
 
 
-class NSELoss(nn.Module):
-    r"""Creates a module that calculates the rescaled score-matching loss for a NSE
-    regressor.
+class FMPELoss(nn.Module):
+    r"""Creates a module that calculates the flow matching loss for a FMPE regressor.
 
     Given a batch of :math:`N` pairs :math:`(\theta_i, x_i)`, the module returns
 
-    .. math:: l = \frac{1}{N} \sum_{i = 1}^N
-        \| s_\phi(\theta'_i, x_i, t_i) + z_i \|_2^2
+    .. math:: l = \frac{1}{N} \sum_{i = 1}^N\|
+            v_\phi((1 - t_i) \theta_i + (t_i + \eta) \epsilon_i, x_i, t_i)
+            - (\epsilon_i - \theta_i)
+        \|_2^2
 
-    where :math:`t_i \sim \mathcal{U}(0, 1)`, :math:`z_i \sim \mathcal{N}(0,
-    I)` and :math:`\theta'_i = \sqrt{\alpha(t_i)} \, \theta_i + (1 - \alpha(t_i)) \,
-    z_i`.
+    where :math:`t_i \sim \mathcal{U}(0, 1)` and :math:`\epsilon_i \sim \mathcal{N}(0, I)`.
 
     Arguments:
-        estimator: A regression network :math:`s_\phi(\theta, x, t)`.
+        estimator: A regression network :math:`v_\phi(\theta, x, t)`.
     """
 
-    def __init__(self, estimator: nn.Module):
+    def __init__(self, estimator: nn.Module, eta: float = 1e-3):
         super().__init__()
 
         self.estimator = estimator
+        self.eta = eta
 
     def forward(self, theta: Tensor, x: Tensor) -> Tensor:
         r"""
         Arguments:
             theta: The parameters :math:`\theta`, with shape :math:`(N, D)`.
             x: The observation :math:`x`, with shape :math:`(N, L)`.
 
         Returns:
             The scalar loss :math:`l`.
         """
 
-        t = theta.new_empty(theta.shape[:-1]).uniform_(0, 1)
-        alpha = self.estimator.alpha(t)[..., None]
-
-        z = torch.randn_like(theta)
-        theta_prime = alpha.sqrt() * theta + (1 - alpha) * z
+        t = torch.rand(theta.shape[:-1], dtype=theta.dtype, device=theta.device)
+        t_ = t[..., None]
 
-        score = self.estimator(theta_prime, x, t)
+        eps = torch.randn_like(theta)
+        theta_prime = (1 - t_) * theta + (t_ + self.eta) * eps
+        v = eps - theta
 
-        return (score + z).square().mean()
+        return (self.estimator(theta_prime, x, t) - v).square().mean()
 
 
 class MetropolisHastings(object):
     r"""Creates a batched Metropolis-Hastings sampler.
 
     Metropolis-Hastings is a Markov chain Monte Carlo (MCMC) sampling algorithm used to
     sample from intractable distributions :math:`p(x)` whose density is proportional to
```

### Comparing `lampe-0.7.3/lampe/masks.py` & `lampe-0.8.0/lampe/masks.py`

 * *Files identical despite different names*

### Comparing `lampe-0.7.3/lampe/nn.py` & `lampe-0.8.0/lampe/nn.py`

 * *Files identical despite different names*

### Comparing `lampe-0.7.3/lampe/plots.py` & `lampe-0.8.0/lampe/plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -456,15 +456,15 @@
 
     # Plot
     if new:
         ax.plot([0, 1], [0, 1], color='k', linestyle='--')
 
     ax.plot(levels, coverages, color=color, label=legend)
 
-    ax.grid()
+    ax.grid(visible=True)
     ax.set_xlabel(r'Credible level')
     ax.set_ylabel(r'Expected coverage')
 
     if legend is not None:
         ax.legend(loc='upper left')
 
     figure.tight_layout(pad=0.5)
```

### Comparing `lampe-0.7.3/lampe/utils.py` & `lampe-0.8.0/lampe/utils.py`

 * *Files identical despite different names*

### Comparing `lampe-0.7.3/lampe.egg-info/PKG-INFO` & `lampe-0.8.0/lampe.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 Metadata-Version: 2.1
 Name: lampe
-Version: 0.7.3
+Version: 0.8.0
 Summary: Likelihood-free AMortized Posterior Estimation with PyTorch
-Home-page: https://github.com/francois-rozet/lampe
 Author: François Rozet
 Author-email: francois.rozet@outlook.com
-License: MIT License
 Project-URL: Documentation, https://lampe.readthedocs.io
 Project-URL: Source, https://github.com/francois-rozet/lampe
 Project-URL: Tracker, https://github.com/francois-rozet/lampe/issues
 Keywords: torch,simulation-based,inference,amortized,bayesian,posterior,likelihood,mcmc
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `lampe-0.7.3/setup.cfg` & `lampe-0.8.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -11,24 +11,21 @@
 	amortized
 	bayesian
 	posterior
 	likelihood
 	mcmc
 author = François Rozet
 author_email = francois.rozet@outlook.com
-license = MIT License
-url = https://github.com/francois-rozet/lampe
 project_urls = 
 	Documentation = https://lampe.readthedocs.io
 	Source = https://github.com/francois-rozet/lampe
 	Tracker = https://github.com/francois-rozet/lampe/issues
 classifiers = 
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
-	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 
 [options]
 packages = find:
 python_requires = >=3.8
```

