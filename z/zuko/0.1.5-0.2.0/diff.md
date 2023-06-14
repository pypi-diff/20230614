# Comparing `tmp/zuko-0.1.5.tar.gz` & `tmp/zuko-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zuko-0.1.5.tar", last modified: Mon Mar 20 17:08:52 2023, max compression
+gzip compressed data, was "zuko-0.2.0.tar", last modified: Mon Apr 10 15:31:18 2023, max compression
```

## Comparing `zuko-0.1.5.tar` & `zuko-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-03-20 17:08:52.164630 zuko-0.1.5/
--rw-rw-r--   0 francois  (1001) francois  (1001)     1072 2022-12-13 12:43:25.000000 zuko-0.1.5/LICENSE
--rw-rw-r--   0 francois  (1001) francois  (1001)     4270 2023-03-20 17:08:52.164630 zuko-0.1.5/PKG-INFO
--rw-rw-r--   0 francois  (1001) francois  (1001)     3419 2023-02-07 15:10:30.000000 zuko-0.1.5/README.md
--rw-rw-r--   0 francois  (1001) francois  (1001)      930 2023-03-20 17:08:52.164630 zuko-0.1.5/setup.cfg
--rw-rw-r--   0 francois  (1001) francois  (1001)       61 2023-01-21 11:03:48.000000 zuko-0.1.5/setup.py
-drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-03-20 17:08:52.164630 zuko-0.1.5/zuko/
--rw-rw-r--   0 francois  (1001) francois  (1001)      177 2023-03-20 17:08:26.000000 zuko-0.1.5/zuko/__init__.py
--rw-rw-r--   0 francois  (1001) francois  (1001)    20362 2023-02-07 15:31:17.000000 zuko-0.1.5/zuko/distributions.py
--rw-rw-r--   0 francois  (1001) francois  (1001)    28104 2023-03-20 17:08:26.000000 zuko-0.1.5/zuko/flows.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     9172 2023-03-20 17:08:26.000000 zuko-0.1.5/zuko/nn.py
--rw-rw-r--   0 francois  (1001) francois  (1001)    21619 2023-03-03 16:17:55.000000 zuko-0.1.5/zuko/transforms.py
--rw-rw-r--   0 francois  (1001) francois  (1001)    12928 2023-03-20 17:08:26.000000 zuko-0.1.5/zuko/utils.py
-drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-03-20 17:08:52.164630 zuko-0.1.5/zuko.egg-info/
--rw-rw-r--   0 francois  (1001) francois  (1001)     4270 2023-03-20 17:08:52.000000 zuko-0.1.5/zuko.egg-info/PKG-INFO
--rw-rw-r--   0 francois  (1001) francois  (1001)      272 2023-03-20 17:08:52.000000 zuko-0.1.5/zuko.egg-info/SOURCES.txt
--rw-rw-r--   0 francois  (1001) francois  (1001)        1 2023-03-20 17:08:52.000000 zuko-0.1.5/zuko.egg-info/dependency_links.txt
--rw-rw-r--   0 francois  (1001) francois  (1001)       27 2023-03-20 17:08:52.000000 zuko-0.1.5/zuko.egg-info/requires.txt
--rw-rw-r--   0 francois  (1001) francois  (1001)        5 2023-03-20 17:08:52.000000 zuko-0.1.5/zuko.egg-info/top_level.txt
+drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-04-10 15:31:18.386393 zuko-0.2.0/
+-rw-rw-r--   0 francois  (1001) francois  (1001)     1072 2022-12-13 12:43:25.000000 zuko-0.2.0/LICENSE
+-rw-rw-r--   0 francois  (1001) francois  (1001)     4262 2023-04-10 15:31:18.386393 zuko-0.2.0/PKG-INFO
+-rw-rw-r--   0 francois  (1001) francois  (1001)     3411 2023-04-10 15:30:49.000000 zuko-0.2.0/README.md
+-rw-rw-r--   0 francois  (1001) francois  (1001)      930 2023-04-10 15:31:18.386393 zuko-0.2.0/setup.cfg
+-rw-rw-r--   0 francois  (1001) francois  (1001)       61 2023-01-21 11:03:48.000000 zuko-0.2.0/setup.py
+drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-04-10 15:31:18.386393 zuko-0.2.0/zuko/
+-rw-rw-r--   0 francois  (1001) francois  (1001)      177 2023-04-10 15:30:49.000000 zuko-0.2.0/zuko/__init__.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)    20798 2023-04-10 15:30:49.000000 zuko-0.2.0/zuko/distributions.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)    28104 2023-04-10 13:44:16.000000 zuko-0.2.0/zuko/flows.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     9172 2023-03-20 17:08:26.000000 zuko-0.2.0/zuko/nn.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)    23270 2023-04-10 15:30:49.000000 zuko-0.2.0/zuko/transforms.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)    12928 2023-03-20 17:08:26.000000 zuko-0.2.0/zuko/utils.py
+drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-04-10 15:31:18.386393 zuko-0.2.0/zuko.egg-info/
+-rw-rw-r--   0 francois  (1001) francois  (1001)     4262 2023-04-10 15:31:18.000000 zuko-0.2.0/zuko.egg-info/PKG-INFO
+-rw-rw-r--   0 francois  (1001) francois  (1001)      272 2023-04-10 15:31:18.000000 zuko-0.2.0/zuko.egg-info/SOURCES.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)        1 2023-04-10 15:31:18.000000 zuko-0.2.0/zuko.egg-info/dependency_links.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)       28 2023-04-10 15:31:18.000000 zuko-0.2.0/zuko.egg-info/requires.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)        5 2023-04-10 15:31:18.000000 zuko-0.2.0/zuko.egg-info/top_level.txt
```

### Comparing `zuko-0.1.5/LICENSE` & `zuko-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zuko-0.1.5/PKG-INFO` & `zuko-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zuko
-Version: 0.1.5
+Version: 0.2.0
 Summary: Normalizing flows in PyTorch
 Home-page: https://github.com/francois-rozet/zuko
 Author: François Rozet
 Author-email: francois.rozet@outlook.com
 License: MIT License
 Project-URL: Documentation, https://zuko.readthedocs.io
 Project-URL: Source, https://github.com/francois-rozet/zuko
@@ -22,15 +22,15 @@
 
 ![Zuko's banner](https://raw.githubusercontent.com/francois-rozet/zuko/master/docs/images/banner.svg)
 
 # Zuko - Normalizing flows in PyTorch
 
 Zuko is a Python package that implements normalizing flows in PyTorch. It relies as much as possible on distributions and transformations already provided by PyTorch. Unfortunately, the `Distribution` and `Transform` classes of `torch` are not sub-classes of `torch.nn.Module`, which means you cannot send their internal tensors to GPU with `.to('cuda')` or retrieve their parameters with `.parameters()`.
 
-To solve this problem, `zuko` defines two abstract classes: `DistributionModule` and `TransformModule`. The former is any `Module` whose forward pass returns a `Distribution` and the latter is any `Module` whose forward pass returns a `Transform`. Then, a normalizing flow is the composition of a list of `TransformModule` and a base `DistributionModule`. This design allows for flows that behave like distributions while retaining the benefits of `Module`. It also makes the implementations easy to understand and extend.
+To solve this problem, `zuko` defines two abstract classes: `DistributionModule` and `TransformModule`. The former is any `Module` whose forward pass returns a `Distribution` and the latter is any `Module` whose forward pass returns a `Transform`. A normalizing flow is just a `DistributionModule` which contains a list of `TransformModule` and a base `DistributionModule`. This design allows for flows that behave like distributions while retaining the benefits of `Module`. It also makes the implementations easier to understand and extend.
 
 > In the [Avatar](https://wikipedia.org/wiki/Avatar:_The_Last_Airbender) cartoon, [Zuko](https://wikipedia.org/wiki/Zuko) is a powerful firebender 🔥
 
 ## Installation
 
 The `zuko` package is available on [PyPI](https://pypi.org/project/zuko), which means it is installable via `pip`.
 
@@ -66,15 +66,15 @@
     loss.backward()
     optimizer.step()
 
 # Sample 64 points x ~ p(x | y*)
 x = flow(y_star).sample((64,))
 ```
 
-For more information about the available features check out the documentation at [zuko.readthedocs.io](https://zuko.readthedocs.io).
+For more information, check out the documentation at [zuko.readthedocs.io](https://zuko.readthedocs.io).
 
 ### Available flows
 
 | Class   | Year | Reference |
 |:-------:|:----:|-----------|
 | `MAF`   | 2017 | [Masked Autoregressive Flow for Density Estimation](https://arxiv.org/abs/1705.07057) |
 | `NSF`   | 2019 | [Neural Spline Flows](https://arxiv.org/abs/1906.04032) |
```

### Comparing `zuko-0.1.5/README.md` & `zuko-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ![Zuko's banner](https://raw.githubusercontent.com/francois-rozet/zuko/master/docs/images/banner.svg)
 
 # Zuko - Normalizing flows in PyTorch
 
 Zuko is a Python package that implements normalizing flows in PyTorch. It relies as much as possible on distributions and transformations already provided by PyTorch. Unfortunately, the `Distribution` and `Transform` classes of `torch` are not sub-classes of `torch.nn.Module`, which means you cannot send their internal tensors to GPU with `.to('cuda')` or retrieve their parameters with `.parameters()`.
 
-To solve this problem, `zuko` defines two abstract classes: `DistributionModule` and `TransformModule`. The former is any `Module` whose forward pass returns a `Distribution` and the latter is any `Module` whose forward pass returns a `Transform`. Then, a normalizing flow is the composition of a list of `TransformModule` and a base `DistributionModule`. This design allows for flows that behave like distributions while retaining the benefits of `Module`. It also makes the implementations easy to understand and extend.
+To solve this problem, `zuko` defines two abstract classes: `DistributionModule` and `TransformModule`. The former is any `Module` whose forward pass returns a `Distribution` and the latter is any `Module` whose forward pass returns a `Transform`. A normalizing flow is just a `DistributionModule` which contains a list of `TransformModule` and a base `DistributionModule`. This design allows for flows that behave like distributions while retaining the benefits of `Module`. It also makes the implementations easier to understand and extend.
 
 > In the [Avatar](https://wikipedia.org/wiki/Avatar:_The_Last_Airbender) cartoon, [Zuko](https://wikipedia.org/wiki/Zuko) is a powerful firebender 🔥
 
 ## Installation
 
 The `zuko` package is available on [PyPI](https://pypi.org/project/zuko), which means it is installable via `pip`.
 
@@ -44,15 +44,15 @@
     loss.backward()
     optimizer.step()
 
 # Sample 64 points x ~ p(x | y*)
 x = flow(y_star).sample((64,))
 ```
 
-For more information about the available features check out the documentation at [zuko.readthedocs.io](https://zuko.readthedocs.io).
+For more information, check out the documentation at [zuko.readthedocs.io](https://zuko.readthedocs.io).
 
 ### Available flows
 
 | Class   | Year | Reference |
 |:-------:|:----:|-----------|
 | `MAF`   | 2017 | [Masked Autoregressive Flow for Density Estimation](https://arxiv.org/abs/1705.07057) |
 | `NSF`   | 2019 | [Neural Spline Flows](https://arxiv.org/abs/1906.04032) |
```

### Comparing `zuko-0.1.5/setup.cfg` & `zuko-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `zuko-0.1.5/zuko/distributions.py` & `zuko-0.2.0/zuko/distributions.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,25 @@
         if self.base.has_rsample:
             z = self.base.rsample(shape)
         else:
             z = self.base.sample(shape)
 
         return self.transform.inv(z)
 
+    def rsample_and_log_prob(self, shape: Size = ()) -> Tuple[Tensor, Tensor]:
+        if self.base.has_rsample:
+            z = self.base.rsample(shape)
+        else:
+            z = self.base.sample(shape)
+
+        x, ladj = self.transform.inv.call_and_ladj(z)
+        ladj = _sum_rightmost(ladj, self.reinterpreted)
+
+        return x, self.base.log_prob(z) - ladj
+
 
 class Joint(Distribution):
     r"""Creates a distribution for a multivariate random variable :math:`X` which
     is the concatenation of :math:`n` independent random variables :math:`Z_i`.
 
     .. math:: p(X = x) = \prod_i p(Z_i = x_i)
 
@@ -336,15 +347,15 @@
         >>> d.event_shape
         torch.Size([3])
         >>> d.sample()
         tensor([ 0.7304, -0.1976, -1.7591])
     """
 
     def __init__(self, loc: Tensor, scale: Tensor, ndims: int = 1):
-        super().__init__(Normal(loc, scale), ndims)
+        super().__init__(Normal(torch.as_tensor(loc), torch.as_tensor(scale)), ndims)
 
     def __repr__(self) -> str:
         return 'Diag' + repr(self.base_dist)
 
     def expand(self, batch_shape: Size, new: Distribution = None) -> Distribution:
         new = self._get_checked_instance(DiagNormal, new)
         return super().expand(batch_shape, new)
@@ -369,15 +380,15 @@
         >>> d.event_shape
         torch.Size([3])
         >>> d.sample()
         tensor([ 0.1859, -0.9698,  0.0665])
     """
 
     def __init__(self, lower: Tensor, upper: Tensor, ndims: int = 1):
-        super().__init__(Uniform(lower, upper), ndims)
+        super().__init__(Uniform(torch.as_tensor(lower), torch.as_tensor(upper)), ndims)
 
     def __repr__(self) -> str:
         return 'Box' + repr(self.base_dist)
 
     def expand(self, batch_shape: Size, new: Distribution = None) -> Distribution:
         new = self._get_checked_instance(BoxUniform, new)
         return super().expand(batch_shape, new)
```

### Comparing `zuko-0.1.5/zuko/flows.py` & `zuko-0.2.0/zuko/flows.py`

 * *Files identical despite different names*

### Comparing `zuko-0.1.5/zuko/nn.py` & `zuko-0.2.0/zuko/nn.py`

 * *Files identical despite different names*

### Comparing `zuko-0.1.5/zuko/transforms.py` & `zuko-0.2.0/zuko/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     'MonotonicAffineTransform',
     'MonotonicRQSTransform',
     'MonotonicTransform',
     'UnconstrainedMonotonicTransform',
     'SOSPolynomialTransform',
     'FreeFormJacobianTransform',
     'AutoregressiveTransform',
+    'LULinearTransform',
     'PermutationTransform',
 ]
 
 import math
 import torch
 import torch.nn.functional as F
 
@@ -103,14 +104,25 @@
         return all(t.bijective for t in self.transforms)
 
     def _call(self, x: Tensor) -> Tensor:
         for t in self.transforms:
             x = t(x)
         return x
 
+    @property
+    def inv(self) -> Transform:
+        new = self.__new__(ComposedTransform)
+        new.transforms = [t.inv for t in reversed(self.transforms)]
+        new.domain_dim = self.codomain_dim
+        new.codomain_dim = self.domain_dim
+
+        Transform.__init__(new)
+
+        return new
+
     def _inverse(self, y: Tensor) -> Tensor:
         for t in reversed(self.transforms):
             y = t.inv(y)
         return y
 
     def log_abs_det_jacobian(self, x: Tensor, y: Tensor) -> Tensor:
         _, ladj = self.call_and_ladj(x)
@@ -581,15 +593,15 @@
 
 class FreeFormJacobianTransform(Transform):
     r"""Creates a free-form Jacobian transformation.
 
     The transformation is the integration of a system of first-order ordinary
     differential equations
 
-    .. math:: x(T) = \int_0^T f_\phi(t, x(t)) ~ dt .
+    .. math:: x(T) = x(0) + \int_0^T f_\phi(t, x(t)) ~ dt .
 
     References:
         | FFJORD: Free-form Continuous Dynamics for Scalable Reversible Generative Models (Grathwohl et al., 2018)
         | https://arxiv.org/abs/1810.01367
 
     Arguments:
         f: A system of first-order ODEs :math:`f_\phi`.
@@ -619,47 +631,55 @@
         self.phi = tuple(filter(lambda p: p.requires_grad, phi))
         self.exact = exact
         self.trace_scale = 1e-2  # relax jacobian tolerances
 
     def _call(self, x: Tensor) -> Tensor:
         return odeint(self.f, x, self.t0, self.t1, self.phi)
 
+    @property
+    def inv(self) -> Transform:
+        new = self.__new__(FreeFormJacobianTransform)
+        new.f = self.f
+        new.t0 = self.t1
+        new.t1 = self.t0
+        new.phi = self.phi
+        new.exact = self.exact
+        new.trace_scale = self.trace_scale
+
+        Transform.__init__(new)
+
+        return new
+
     def _inverse(self, y: Tensor) -> Tensor:
         return odeint(self.f, y, self.t1, self.t0, self.phi)
 
     def log_abs_det_jacobian(self, x: Tensor, y: Tensor) -> Tensor:
         _, ladj = self.call_and_ladj(x)
         return ladj
 
     def call_and_ladj(self, x: Tensor) -> Tuple[Tensor, Tensor]:
         if self.exact:
             I = torch.eye(x.shape[-1], dtype=x.dtype, device=x.device)
             I = I.expand(*x.shape, x.shape[-1]).movedim(-1, 0)
-
-            def f_aug(t: Tensor, x: Tensor, ladj: Tensor) -> Tensor:
-                with torch.enable_grad():
-                    x = x.requires_grad_().expand(I.shape)
-                    dx = self.f(t, x)
-
-                jacobian = torch.autograd.grad(dx, x, I, create_graph=True)[0]
-                trace = torch.einsum('i...i', jacobian)
-
-                return dx[0], trace * self.trace_scale
         else:
             eps = torch.randn_like(x)
 
-            def f_aug(t: Tensor, x: Tensor, ladj: Tensor) -> Tensor:
-                with torch.enable_grad():
-                    x = x.requires_grad_()
-                    dx = self.f(t, x)
+        def f_aug(t: Tensor, x: Tensor, ladj: Tensor) -> Tensor:
+            with torch.enable_grad():
+                x = x.requires_grad_()
+                dx = self.f(t, x)
 
+            if self.exact:
+                jacobian = torch.autograd.grad(dx, x, I, create_graph=True, is_grads_batched=True)[0]
+                trace = torch.einsum('i...i', jacobian)
+            else:
                 epsjp = torch.autograd.grad(dx, x, eps, create_graph=True)[0]
                 trace = (epsjp * eps).sum(dim=-1)
 
-                return dx, trace * self.trace_scale
+            return dx, trace * self.trace_scale
 
         ladj = torch.zeros_like(x[..., 0])
         y, ladj = odeint(f_aug, (x, ladj), self.t0, self.t1, self.phi)
 
         return y, ladj * (1 / self.trace_scale)
 
 
@@ -702,14 +722,54 @@
         return self.meta(x).log_abs_det_jacobian(x, y).sum(dim=-1)
 
     def call_and_ladj(self, x: Tensor) -> Tuple[Tensor, Tensor]:
         y, ladj = self.meta(x).call_and_ladj(x)
         return y, ladj.sum(dim=-1)
 
 
+class LULinearTransform(Transform):
+    r"""Creates a transformation :math:`f(x) = L U x`.
+
+    Arguments:
+        LU: A matrix whose lower and upper triangular parts are the non-zero elements
+            of :math:`L` and :math:`U`, with shape :math:`(*, D, D)`.
+    """
+
+    domain = constraints.real_vector
+    codomain = constraints.real_vector
+    bijective = True
+
+    def __init__(self, LU: Tensor, **kwargs):
+        super().__init__(**kwargs)
+
+        I = torch.eye(LU.shape[-1], dtype=LU.dtype, device=LU.device)
+
+        self.L = torch.tril(LU, diagonal=-1) + I
+        self.U = torch.triu(LU, diagonal=+1) + I
+
+    def _call(self, x: Tensor) -> Tensor:
+        return (self.L @ self.U @ x.unsqueeze(-1)).squeeze(-1)
+
+    def _inverse(self, y: Tensor) -> Tensor:
+        return torch.linalg.solve_triangular(
+            self.U,
+            torch.linalg.solve_triangular(
+                self.L,
+                y.unsqueeze(-1),
+                upper=False,
+                unitriangular=True,
+            ),
+            upper=True,
+            unitriangular=True,
+        ).squeeze(-1)
+
+    def log_abs_det_jacobian(self, x: Tensor, y: Tensor) -> Tensor:
+        return x.new_zeros(x.shape[:-1])
+
+
 class PermutationTransform(Transform):
     r"""Creates a transformation that permutes the elements.
 
     Arguments:
         order: The permutation order, with shape :math:`(*, D)`.
     """
```

### Comparing `zuko-0.1.5/zuko/utils.py` & `zuko-0.2.0/zuko/utils.py`

 * *Files identical despite different names*

### Comparing `zuko-0.1.5/zuko.egg-info/PKG-INFO` & `zuko-0.2.0/zuko.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zuko
-Version: 0.1.5
+Version: 0.2.0
 Summary: Normalizing flows in PyTorch
 Home-page: https://github.com/francois-rozet/zuko
 Author: François Rozet
 Author-email: francois.rozet@outlook.com
 License: MIT License
 Project-URL: Documentation, https://zuko.readthedocs.io
 Project-URL: Source, https://github.com/francois-rozet/zuko
@@ -22,15 +22,15 @@
 
 ![Zuko's banner](https://raw.githubusercontent.com/francois-rozet/zuko/master/docs/images/banner.svg)
 
 # Zuko - Normalizing flows in PyTorch
 
 Zuko is a Python package that implements normalizing flows in PyTorch. It relies as much as possible on distributions and transformations already provided by PyTorch. Unfortunately, the `Distribution` and `Transform` classes of `torch` are not sub-classes of `torch.nn.Module`, which means you cannot send their internal tensors to GPU with `.to('cuda')` or retrieve their parameters with `.parameters()`.
 
-To solve this problem, `zuko` defines two abstract classes: `DistributionModule` and `TransformModule`. The former is any `Module` whose forward pass returns a `Distribution` and the latter is any `Module` whose forward pass returns a `Transform`. Then, a normalizing flow is the composition of a list of `TransformModule` and a base `DistributionModule`. This design allows for flows that behave like distributions while retaining the benefits of `Module`. It also makes the implementations easy to understand and extend.
+To solve this problem, `zuko` defines two abstract classes: `DistributionModule` and `TransformModule`. The former is any `Module` whose forward pass returns a `Distribution` and the latter is any `Module` whose forward pass returns a `Transform`. A normalizing flow is just a `DistributionModule` which contains a list of `TransformModule` and a base `DistributionModule`. This design allows for flows that behave like distributions while retaining the benefits of `Module`. It also makes the implementations easier to understand and extend.
 
 > In the [Avatar](https://wikipedia.org/wiki/Avatar:_The_Last_Airbender) cartoon, [Zuko](https://wikipedia.org/wiki/Zuko) is a powerful firebender 🔥
 
 ## Installation
 
 The `zuko` package is available on [PyPI](https://pypi.org/project/zuko), which means it is installable via `pip`.
 
@@ -66,15 +66,15 @@
     loss.backward()
     optimizer.step()
 
 # Sample 64 points x ~ p(x | y*)
 x = flow(y_star).sample((64,))
 ```
 
-For more information about the available features check out the documentation at [zuko.readthedocs.io](https://zuko.readthedocs.io).
+For more information, check out the documentation at [zuko.readthedocs.io](https://zuko.readthedocs.io).
 
 ### Available flows
 
 | Class   | Year | Reference |
 |:-------:|:----:|-----------|
 | `MAF`   | 2017 | [Masked Autoregressive Flow for Density Estimation](https://arxiv.org/abs/1705.07057) |
 | `NSF`   | 2019 | [Neural Spline Flows](https://arxiv.org/abs/1906.04032) |
```

