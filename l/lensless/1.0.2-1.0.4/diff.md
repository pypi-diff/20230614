# Comparing `tmp/lensless-1.0.2.tar.gz` & `tmp/lensless-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lensless-1.0.2.tar", last modified: Tue May 31 12:02:32 2022, max compression
+gzip compressed data, was "lensless-1.0.4.tar", last modified: Wed Jun 14 08:13:17 2023, max compression
```

## Comparing `lensless-1.0.2.tar` & `lensless-1.0.4.tar`

### file list

```diff
@@ -1,30 +1,36 @@
-drwxrwxr-x   0 bezzam    (1009) bezzam    (1009)        0 2022-05-31 12:02:32.711920 lensless-1.0.2/
--rw-rw-r--   0 bezzam    (1009) bezzam    (1009)    35149 2022-04-13 11:58:01.000000 lensless-1.0.2/LICENSE
--rw-rw-r--   0 bezzam    (1009) bezzam    (1009)    12278 2022-05-31 12:02:32.711920 lensless-1.0.2/PKG-INFO
--rw-rw-r--   0 bezzam    (1009) bezzam    (1009)    11819 2022-05-31 11:49:38.000000 lensless-1.0.2/README.md
-drwxrwxr-x   0 bezzam    (1009) bezzam    (1009)        0 2022-05-31 12:02:32.711920 lensless-1.0.2/lensless/
--rw-rw-r--   0 bezzam    (1009) bezzam    (1009)      300 2022-04-24 21:40:17.000000 lensless-1.0.2/lensless/__init__.py
--rw-rw-r--   0 bezzam    (1009) bezzam    (1009)     7981 2022-05-31 11:49:38.000000 lensless-1.0.2/lensless/admm.py
--rw-rw-r--   0 bezzam    (1009) bezzam    (1009)     7202 2022-05-31 11:49:38.000000 lensless-1.0.2/lensless/apgd.py
--rw-rw-r--   0 bezzam    (1009) bezzam    (1009)      510 2022-04-13 11:58:02.000000 lensless-1.0.2/lensless/autocorr.py
--rw-rw-r--   0 bezzam    (1009) bezzam    (1009)      311 2022-04-13 11:58:02.000000 lensless-1.0.2/lensless/constants.py
--rw-rw-r--   0 bezzam    (1009) bezzam    (1009)     5371 2022-05-31 11:49:38.000000 lensless-1.0.2/lensless/gradient_descent.py
--rw-rw-r--   0 bezzam    (1009) bezzam    (1009)     8911 2022-05-31 11:49:38.000000 lensless-1.0.2/lensless/io.py
--rw-rw-r--   0 bezzam    (1009) bezzam    (1009)     5093 2022-04-13 11:58:02.000000 lensless-1.0.2/lensless/metric.py
--rw-rw-r--   0 bezzam    (1009) bezzam    (1009)     1134 2022-04-13 11:58:02.000000 lensless-1.0.2/lensless/mirflickr.py
--rw-rw-r--   0 bezzam    (1009) bezzam    (1009)     6415 2022-04-13 11:58:02.000000 lensless-1.0.2/lensless/plot.py
--rw-rw-r--   0 bezzam    (1009) bezzam    (1009)     1242 2022-04-13 11:58:02.000000 lensless-1.0.2/lensless/realfftconv.py
--rw-rw-r--   0 bezzam    (1009) bezzam    (1009)     3020 2022-05-31 09:58:37.000000 lensless-1.0.2/lensless/realfftconv_sol.py
--rw-rw-r--   0 bezzam    (1009) bezzam    (1009)     7038 2022-04-13 11:58:02.000000 lensless-1.0.2/lensless/recon.py
--rw-rw-r--   0 bezzam    (1009) bezzam    (1009)     6211 2022-04-26 12:27:20.000000 lensless-1.0.2/lensless/util.py
-drwxrwxr-x   0 bezzam    (1009) bezzam    (1009)        0 2022-05-31 12:02:32.711920 lensless-1.0.2/lensless.egg-info/
--rw-rw-r--   0 bezzam    (1009) bezzam    (1009)    12278 2022-05-31 12:02:32.000000 lensless-1.0.2/lensless.egg-info/PKG-INFO
--rw-rw-r--   0 bezzam    (1009) bezzam    (1009)      507 2022-05-31 12:02:32.000000 lensless-1.0.2/lensless.egg-info/SOURCES.txt
--rw-rw-r--   0 bezzam    (1009) bezzam    (1009)        1 2022-05-31 12:02:32.000000 lensless-1.0.2/lensless.egg-info/dependency_links.txt
--rw-rw-r--   0 bezzam    (1009) bezzam    (1009)      112 2022-05-31 12:02:32.000000 lensless-1.0.2/lensless.egg-info/requires.txt
--rw-rw-r--   0 bezzam    (1009) bezzam    (1009)        9 2022-05-31 12:02:32.000000 lensless-1.0.2/lensless.egg-info/top_level.txt
--rw-rw-r--   0 bezzam    (1009) bezzam    (1009)       38 2022-05-31 12:02:32.711920 lensless-1.0.2/setup.cfg
--rw-rw-r--   0 bezzam    (1009) bezzam    (1009)      905 2022-05-31 11:50:09.000000 lensless-1.0.2/setup.py
-drwxrwxr-x   0 bezzam    (1009) bezzam    (1009)        0 2022-05-31 12:02:32.711920 lensless-1.0.2/test/
--rw-rw-r--   0 bezzam    (1009) bezzam    (1009)     1217 2022-05-31 11:49:38.000000 lensless-1.0.2/test/test_algos.py
--rw-rw-r--   0 bezzam    (1009) bezzam    (1009)      762 2022-04-24 21:40:17.000000 lensless-1.0.2/test/test_io.py
+drwxr-xr-x   0 eric       (502) staff       (20)        0 2023-06-14 08:13:17.311448 lensless-1.0.4/
+-rw-r--r--   0 eric       (502) staff       (20)    35149 2022-05-23 14:51:06.000000 lensless-1.0.4/LICENSE
+-rw-r--r--   0 eric       (502) staff       (20)     6575 2023-06-14 08:13:17.311047 lensless-1.0.4/PKG-INFO
+-rw-r--r--   0 eric       (502) staff       (20)     6117 2023-06-14 08:10:04.000000 lensless-1.0.4/README.rst
+drwxr-xr-x   0 eric       (502) staff       (20)        0 2023-06-14 08:13:17.302353 lensless-1.0.4/lensless/
+-rw-r--r--   0 eric       (502) staff       (20)      893 2023-06-05 06:50:13.000000 lensless-1.0.4/lensless/__init__.py
+-rw-r--r--   0 eric       (502) staff       (20)    11474 2023-06-05 06:50:13.000000 lensless-1.0.4/lensless/admm.py
+-rw-r--r--   0 eric       (502) staff       (20)     8178 2023-06-05 06:50:13.000000 lensless-1.0.4/lensless/apgd.py
+-rw-r--r--   0 eric       (502) staff       (20)    11607 2023-06-05 06:50:13.000000 lensless-1.0.4/lensless/benchmark.py
+-rw-r--r--   0 eric       (502) staff       (20)      311 2022-05-23 14:51:08.000000 lensless-1.0.4/lensless/constants.py
+-rw-r--r--   0 eric       (502) staff       (20)     7627 2023-06-05 06:50:13.000000 lensless-1.0.4/lensless/gradient_descent.py
+-rw-r--r--   0 eric       (502) staff       (20)    12798 2023-06-14 08:09:41.000000 lensless-1.0.4/lensless/io.py
+-rw-r--r--   0 eric       (502) staff       (20)    10302 2023-06-05 06:50:13.000000 lensless-1.0.4/lensless/metric.py
+-rw-r--r--   0 eric       (502) staff       (20)     1134 2022-05-23 14:51:08.000000 lensless-1.0.4/lensless/mirflickr.py
+-rw-r--r--   0 eric       (502) staff       (20)     7271 2023-06-05 06:50:13.000000 lensless-1.0.4/lensless/plot.py
+-rw-r--r--   0 eric       (502) staff       (20)    19373 2023-06-05 06:50:13.000000 lensless-1.0.4/lensless/recon.py
+-rw-r--r--   0 eric       (502) staff       (20)     5888 2023-06-05 06:50:13.000000 lensless-1.0.4/lensless/rfft_convolve.py
+-rw-r--r--   0 eric       (502) staff       (20)        1 2023-06-14 08:10:00.000000 lensless-1.0.4/lensless/secrets.py
+-rw-r--r--   0 eric       (502) staff       (20)     4973 2023-06-05 06:50:13.000000 lensless-1.0.4/lensless/trainable_recon.py
+-rw-r--r--   0 eric       (502) staff       (20)     8637 2023-06-05 06:50:13.000000 lensless-1.0.4/lensless/unrolled_admm.py
+-rw-r--r--   0 eric       (502) staff       (20)     4713 2023-06-05 06:50:13.000000 lensless-1.0.4/lensless/unrolled_fista.py
+-rw-r--r--   0 eric       (502) staff       (20)     8073 2023-06-14 08:09:41.000000 lensless-1.0.4/lensless/util.py
+-rw-r--r--   0 eric       (502) staff       (20)       22 2023-06-14 08:12:53.000000 lensless-1.0.4/lensless/version.py
+drwxr-xr-x   0 eric       (502) staff       (20)        0 2023-06-14 08:13:17.307338 lensless-1.0.4/lensless.egg-info/
+-rw-r--r--   0 eric       (502) staff       (20)     6575 2023-06-14 08:13:16.000000 lensless-1.0.4/lensless.egg-info/PKG-INFO
+-rw-r--r--   0 eric       (502) staff       (20)      642 2023-06-14 08:13:17.000000 lensless-1.0.4/lensless.egg-info/SOURCES.txt
+-rw-r--r--   0 eric       (502) staff       (20)        1 2023-06-14 08:13:16.000000 lensless-1.0.4/lensless.egg-info/dependency_links.txt
+-rw-r--r--   0 eric       (502) staff       (20)      104 2023-06-14 08:13:16.000000 lensless-1.0.4/lensless.egg-info/requires.txt
+-rw-r--r--   0 eric       (502) staff       (20)        9 2023-06-14 08:13:17.000000 lensless-1.0.4/lensless.egg-info/top_level.txt
+-rw-r--r--   0 eric       (502) staff       (20)      113 2023-06-05 06:50:14.000000 lensless-1.0.4/pyproject.toml
+-rw-r--r--   0 eric       (502) staff       (20)       38 2023-06-14 08:13:17.311647 lensless-1.0.4/setup.cfg
+-rw-r--r--   0 eric       (502) staff       (20)     1062 2023-06-14 08:10:04.000000 lensless-1.0.4/setup.py
+drwxr-xr-x   0 eric       (502) staff       (20)        0 2023-06-14 08:13:17.310143 lensless-1.0.4/test/
+-rw-r--r--   0 eric       (502) staff       (20)     7491 2023-06-05 06:50:14.000000 lensless-1.0.4/test/test_algos.py
+-rw-r--r--   0 eric       (502) staff       (20)     2114 2023-06-05 06:50:14.000000 lensless-1.0.4/test/test_convolver.py
+-rw-r--r--   0 eric       (502) staff       (20)      814 2023-06-05 06:50:14.000000 lensless-1.0.4/test/test_io.py
```

### Comparing `lensless-1.0.2/LICENSE` & `lensless-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lensless-1.0.2/lensless/apgd.py` & `lensless-1.0.4/lensless/gradient_descent.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,197 +1,218 @@
+import numpy as np
 from lensless.recon import ReconstructionAlgorithm
 import inspect
-import numpy as np
-from pycsou.linop.conv import Convolve2D
-from pycsou.func.loss import SquaredL2Loss
-from pycsou.func.penalty import NonNegativeOrthant, SquaredL2Norm, L1Norm
-from pycsou.opt.proxalgs import APGD as APGD_pyc
-from copy import deepcopy
 
 try:
-    from lensless.realfftconv_sol import RealFFTConvolve2D
-except:
-    from lensless.realfftconv import RealFFTConvolve2D
+    import torch
 
+    torch_available = True
+except ImportError:
+    torch_available = False
 
-class APGDPriors:
-    """
-    Priors (compatible with Pycsou) for APGD.
 
-    See Pycsou documentation for available penalties:
-    https://matthieumeo.github.io/pycsou/html/api/functionals/pycsou.func.penalty.html?highlight=penalty#module-pycsou.func.penalty
-    """
+class GradientDescentUpdate:
+    """Gradient descent update techniques."""
 
-    L2 = "l2"
-    NONNEG = "nonneg"
-    L1 = "l1"
+    VANILLA = "vanilla"
+    NESTEROV = "nesterov"
+    FISTA = "fista"
 
     @staticmethod
     def all_values():
         vals = []
-        for i in inspect.getmembers(APGDPriors):
+        for i in inspect.getmembers(GradientDescentUpdate):
             # remove private and protected functions, and this function
             if not i[0].startswith("_") and not callable(i[1]):
                 vals.append(i[1])
         return vals
 
 
-class APGD(ReconstructionAlgorithm):
-    def __init__(
-        self,
-        psf,
-        max_iter=500,
-        dtype=np.float32,
-        diff_penalty=None,
-        prox_penalty=APGDPriors.NONNEG,
-        acceleration="BT",
-        diff_lambda=0.001,
-        prox_lambda=0.001,
-        realconv=True,
-        **kwargs
-    ):
-        """
-        Wrapper for Pycsou's APGD (accelerated proximal gradient descent)
-        applied to lensless imaging.
+def non_neg(xi):
+    """
+    Clip input so that it is non-negative.
 
-        Pycsou APGD documentation: https://matthieumeo.github.io/pycsou/html/api/algorithms/pycsou.opt.proxalgs.html?highlight=apgd#pycsou.opt.proxalgs.AcceleratedProximalGradientDescent
+    Parameters
+    ----------
+    xi : :py:class:`~numpy.ndarray`
+        Data to clip.
+
+    Returns
+    -------
+    nonneg : :py:class:`~numpy.ndarray`
+        Non-negative projection of input.
+
+    """
+    if torch_available and isinstance(xi, torch.Tensor):
+        return torch.maximum(xi, torch.zeros_like(xi))
+    else:
+        return np.maximum(xi, 0)
+
+
+class GradientDescent(ReconstructionAlgorithm):
+    """
+    Object for applying projected gradient descent.
+    """
+
+    def __init__(self, psf, dtype=None, proj=non_neg, **kwargs):
+        """
 
         Parameters
         ----------
-        psf :py:class:`~numpy.ndarray`
-            PSF that models forward propagation.
-        max_iter : int, optional
-            Maximal number of iterations.
+        psf : :py:class:`~numpy.ndarray` or :py:class:`~torch.Tensor`
+            Point spread function (PSF) that models forward propagation.
+            Must be of shape (depth, height, width, channels) even if
+            depth = 1 and channels = 1. You can use :py:func:`~lensless.io.load_psf`
+            to load a PSF from a file such that it is in the correct format.
         dtype : float32 or float64
-            Data type to use for optimization.
-        diff_penalty : None or str or :py:class:`~pycsou.func.penalty`
-            Differentiable functional to serve as prior / regularization term.
-            Default is None. See Pycsou documentation for available
-            penalties: https://matthieumeo.github.io/pycsou/html/api/functionals/pycsou.func.penalty.html?highlight=penalty#module-pycsou.func.penalty
-        prox_penalty : None or str or :py:class:`~pycsou.func.penalty`
-            Proximal functional to serve as prior / regularization term. Default
-            is non-negative prior. See Pycsou documentation for available
-            penalties: https://matthieumeo.github.io/pycsou/html/api/functionals/pycsou.func.penalty.html?highlight=penalty#module-pycsou.func.penalty
-        acceleration : [None, 'BT', 'CD']
-            Which acceleration scheme should be used (None for no acceleration).
-            "BT" (Beck and Teboule) has convergence `O(1/k^2)`, while "CD"
-            (Chambolle and Dossal) has convergence `o(1/K^2)`. So "CD" should be
-            faster. but from our experience "BT" gives better results.
-        diff_lambda : float
-            Weight of differentiable penalty.
-        prox_lambda : float
-            Weight of proximal penalty.
-        realconv : bool
-            Whether to apply convolution for real signals (if available).
-        """
-
-        # PSF and data are the same size / shape
-        self._original_shape = psf.shape
-        self._original_size = psf.size
-
-        self._apgd = None
-        self._gen = None
-
-        super(APGD, self).__init__(psf, dtype)
-
-        self._max_iter = max_iter
-
-        # Convolution operator
-        if realconv:
-            self._H = RealFFTConvolve2D(self._psf, dtype=dtype)
-        else:
-            assert self._is_rgb is False, "RGB not supported for `Convolve2D`."
-            self._H = Convolve2D(size=psf.size, filter=psf, shape=psf.shape, dtype=dtype)
-        self._H.compute_lipschitz_cst()
-
-        # initialize solvers which will be created when data is set
-        if diff_penalty is not None:
-            if diff_penalty == APGDPriors.L2:
-                self._diff_penalty = diff_lambda * SquaredL2Norm(dim=self._H.shape[1])
-            else:
-                assert hasattr(diff_penalty, "jacobianT")
-                self._diff_penalty = diff_lambda * diff_penalty(dim=self._H.shape[1])
-        else:
-            self._diff_penalty = None
+            Data type to use for optimization. Default is float32.
+        proj : :py:class:`function`
+            Projection function to apply at each iteration. Default is
+            non-negative.
+        """
+
+        assert callable(proj)
+        self._proj = proj
+        super(GradientDescent, self).__init__(psf, dtype, **kwargs)
 
-        if prox_penalty is not None:
-            if prox_penalty == APGDPriors.L1:
-                self._prox_penalty = prox_lambda * L1Norm(dim=self._H.shape[1])
-            elif prox_penalty == APGDPriors.NONNEG:
-                self._prox_penalty = prox_lambda * NonNegativeOrthant(dim=self._H.shape[1])
+    def reset(self):
+        if self.is_torch:
+            if self._initial_est is not None:
+                self._image_est = self._initial_est
             else:
-                try:
-                    self._prox_penalty = prox_lambda * prox_penalty(dim=self._H.shape[1])
-                except:
-                    raise ValueError("Unexpected prior.")
+                # initial guess, half intensity image
+                psf_flat = self._psf.reshape(-1, self._psf_shape[3])
+                pixel_start = (
+                    torch.max(psf_flat, axis=0).values + torch.min(psf_flat, axis=0).values
+                ) / 2
+                # initialize image estimate as [Batch, Depth, Height, Width, Channels]
+                self._image_est = torch.ones_like(self._psf[None, ...]) * pixel_start
+
+            # set step size as < 2 / lipschitz
+            Hadj_flat = self._convolver._Hadj.reshape(-1, self._psf_shape[3])
+            H_flat = self._convolver._H.reshape(-1, self._psf_shape[3])
+            self._alpha = torch.real(1.8 / torch.max(torch.abs(Hadj_flat * H_flat), axis=0).values)
+
         else:
-            self._prox_penalty = None
+            if self._initial_est is not None:
+                self._image_est = self._initial_est
+            else:
+                psf_flat = self._psf.reshape(-1, self._psf_shape[3])
+                pixel_start = (np.max(psf_flat, axis=0) + np.min(psf_flat, axis=0)) / 2
+                # initialize image estimate as [Batch, Depth, Height, Width, Channels]
+                self._image_est = np.ones_like(self._psf[None, ...]) * pixel_start
+
+            # set step size as < 2 / lipschitz
+            Hadj_flat = self._convolver._Hadj.reshape(-1, self._psf_shape[3])
+            H_flat = self._convolver._H.reshape(-1, self._psf_shape[3])
+            self._alpha = np.real(1.8 / np.max(Hadj_flat * H_flat, axis=0))
+
+    def _grad(self):
+        diff = self._convolver.convolve(self._image_est) - self._data
+        return self._convolver.deconvolve(diff)
+
+    def _update(self, iter):
+        self._image_est -= self._alpha * self._grad()
+        self._image_est = self._proj(self._image_est)
+
+    def _form_image(self):
+        return self._proj(self._image_est)
+
+
+class NesterovGradientDescent(GradientDescent):
+    """
+    Object for applying projected gradient descent with Nesterov momentum for
+    acceleration.
+
+    A nice tutorial/ blog post on Nesterov momentum can be found
+    `here <https://machinelearningmastery.com/gradient-descent-with-nesterov-momentum-from-scratch/>`_.
 
-        self._acc = acceleration
+    """
 
-    def set_data(self, data):
+    def __init__(self, psf, dtype=None, proj=non_neg, p=0, mu=0.9, **kwargs):
         """
-        For `APGD`, we use data to initialize problem for Pycsou.
 
         Parameters
         ----------
-        data : :py:class:`~numpy.ndarray`
-            Lensless data on which to iterate to recover an estimate of the
-             scene. Should match provide PSF, i.e. shape and 2D (grayscale) or
-             3D (RGB).
-
-        """
-        if not self._is_rgb:
-            assert len(data.shape) == 2
-            data = data[:, :, np.newaxis]
-        assert len(self._psf_shape) == len(data.shape)
-        self._data = data
-
-        """ Set up problem """
-        # Cost function
-        loss = (1 / 2) * SquaredL2Loss(dim=self._H.shape[0], data=self._data.ravel())
-        F = loss * self._H
-        if self._diff_penalty is not None:
-            F += self._diff_penalty
-
-        if self._prox_penalty is not None:
-            G = self._prox_penalty
-            dim = G.shape[1]
-        else:
-            G = None
-            dim = self._data.size
-
-        self._apgd = APGD_pyc(dim=dim, F=F, G=G, acceleration=self._acc)
+        psf : :py:class:`~numpy.ndarray` or :py:class:`~torch.Tensor`
+            Point spread function (PSF) that models forward propagation.
+            Must be of shape (depth, height, width, channels) even if
+            depth = 1 and channels = 1. You can use :py:func:`~lensless.io.load_psf`
+            to load a PSF from a file such that it is in the correct format.
+        dtype : float32 or float64
+            Data type to use for optimization. Default is float32.
+        proj : :py:class:`function`
+            Projection function to apply at each iteration. Default is
+            non-negative.
+        p : float
+            Momentum parameter that keeps track of changes. By default, this
+            is initialized to 0.
+        mu : float
+            Momentum parameter. Default is 0.9.
+        """
+        self._p = p
+        self._mu = mu
+        super(NesterovGradientDescent, self).__init__(psf, dtype, proj, **kwargs)
+
+    def reset(self, p=0, mu=0.9):
+        self._p = p
+        self._mu = mu
+        super(NesterovGradientDescent, self).reset()
+
+    def _update(self, iter):
+        p_prev = self._p
+        self._p = self._mu * self._p - self._alpha * self._grad()
+        self._image_est += -self._mu * p_prev + (1 + self._mu) * self._p
+        self._image_est = self._proj(self._image_est)
 
-        # -- setup to print progress report
-        self._apgd.old_iterand = deepcopy(self._apgd.init_iterand)
-        self._apgd.update_diagnostics()
-        self._gen = self._apgd.iterates(n=self._max_iter)
 
-    def reset(self):
-        self._image_est = np.zeros(self._original_size, dtype=self._dtype)
-        if self._apgd is not None:
-            self._apgd.reset()
+class FISTA(GradientDescent):
+    """
+    Object for applying projected gradient descent with FISTA (Fast Iterative
+    Shrinkage-Thresholding Algorithm) for acceleration.
 
-            # -- setup to print progress report
-            self._apgd.old_iterand = deepcopy(self._apgd.init_iterand)
-            self._apgd.update_diagnostics()
-            self._gen = self._apgd.iterates(n=self._max_iter)
+    Paper: https://www.ceremade.dauphine.fr/~carlier/FISTA
 
-    def _progress(self):
-        """
-        Pycsou has functionality for printing progress that we will make use of
-        here.
+    """
 
+    def __init__(self, psf, dtype=None, proj=non_neg, tk=1.0, **kwargs):
         """
-        self._apgd.update_diagnostics()
-        self._apgd.old_iterand = deepcopy(self._apgd.iterand)
-        self._apgd.print_diagnostics()
 
-    def _update(self):
-        next(self._gen)
-        self._image_est[:] = self._apgd.iterand["iterand"]
+        Parameters
+        ----------
+        psf : :py:class:`~numpy.ndarray` or :py:class:`~torch.Tensor`
+            Point spread function (PSF) that models forward propagation.
+            Must be of shape (depth, height, width, channels) even if
+            depth = 1 and channels = 1. You can use :py:func:`~lensless.io.load_psf`
+            to load a PSF from a file such that it is in the correct format.
+        dtype : float32 or float64
+            Data type to use for optimization. Default is float32.
+        proj : :py:class:`function`
+            Projection function to apply at each iteration. Default is
+            non-negative.
+        tk : float
+            Initial step size parameter for FISTA. It is updated at each iteration
+            according to Eq. 4.2 of paper. By default, initialized to 1.0.
+
+        """
+        self._initial_tk = tk
+
+        super(FISTA, self).__init__(psf, dtype, proj, **kwargs)
+
+        self._tk = tk
+        self._xk = self._image_est
+
+    def reset(self, tk=None):
+        super(FISTA, self).reset()
+        if tk:
+            self._tk = tk
+        else:
+            self._tk = self._initial_tk
+        self._xk = self._image_est
 
-    def _form_image(self):
-        image = self._image_est.reshape(self._original_shape)
-        image[image < 0] = 0
-        return image
+    def _update(self, iter):
+        self._image_est -= self._alpha * self._grad()
+        xk = self._proj(self._image_est)
+        tk = (1 + np.sqrt(1 + 4 * self._tk**2)) / 2
+        self._image_est = xk + (self._tk - 1) / tk * (xk - self._xk)
+        self._tk = tk
+        self._xk = xk
```

### Comparing `lensless-1.0.2/lensless/io.py` & `lensless-1.0.4/lensless/apgd.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,323 +1,223 @@
-import os.path
-import rawpy
-import cv2
+from lensless.recon import ReconstructionAlgorithm
+import inspect
 import numpy as np
-from lensless.util import resize, bayer2rgb, rgb2gray, print_image_info
-from lensless.plot import plot_image
-from lensless.constants import RPI_HQ_CAMERA_CCM_MATRIX, RPI_HQ_CAMERA_BLACK_LEVEL
-
-
-def load_image(
-    fp,
-    verbose=False,
-    flip=False,
-    bayer=False,
-    black_level=RPI_HQ_CAMERA_BLACK_LEVEL,
-    blue_gain=None,
-    red_gain=None,
-    ccm=RPI_HQ_CAMERA_CCM_MATRIX,
-    back=None,
-    nbits_out=None,
-):
-    """
-    Load image as numpy array.
+from typing import Optional
+from lensless.rfft_convolve import RealFFTConvolve2D as Convolver
 
-    Parameters
-    ----------
-    fp : str
-        Full path to file.
-    verbose : bool, optional
-        Whether to plot into about file.
-    flip : bool
-        Whether to flip data (vertical and horizontal).
-    bayer : bool
-        Whether input data is Bayer.
-    blue_gain : float
-        Blue gain for color correction.
-    red_gain : float
-        Red gain for color correction.
-    black_level : float
-        Black level. Default is to use that of Raspberry Pi HQ camera.
-    ccm : :py:class:`~numpy.ndarray`
-        Color correction matrix. Default is to use that of Raspberry Pi HQ camera.
-    back : array_like
-        Background level to subtract.
-    nbits_out : int
-        Output bit depth. Default is to use that of input.
-
-    Returns
-    -------
-    img :py:class:`~numpy.ndarray`
-        RGB image of dimension (height, width, 3).
-    """
-    assert os.path.isfile(fp)
-    if "dng" in fp:
-        assert bayer
-        raw = rawpy.imread(fp)
-        img = raw.raw_image
-        # TODO : use raw.postprocess?
-        ccm = raw.color_matrix[:, :3]
-        black_level = np.array(raw.black_level_per_channel[:3]).astype(np.float32)
-    else:
-        img = cv2.imread(fp, cv2.IMREAD_UNCHANGED)
-
-    if bayer:
-        assert len(img.shape) == 2, img.shape
-        if img.max() > 255:
-            # HQ camera
-            n_bits = 12
+import pycsou.abc as pyca
+import pycsou.operator.func as func
+import pycsou.opt.solver as solver
+import pycsou.opt.stop as stop
+import pycsou.runtime as pycrt
+import pycsou.util as pycu
+import pycsou.util.ptype as pyct
+
+
+class APGDPriors:
+    """
+    Priors (compatible with Pycsou) for APGD.
+
+    """
+
+    L2 = "l2"
+    NONNEG = "nonneg"
+    L1 = "l1"
+
+    @staticmethod
+    def all_values():
+        vals = []
+        for i in inspect.getmembers(APGDPriors):
+            # remove private and protected functions, and this function
+            if not i[0].startswith("_") and not callable(i[1]):
+                vals.append(i[1])
+        return vals
+
+
+class RealFFTConvolve2D(pyca.LinOp):
+    def __init__(
+        self, filter: pyct.NDArray, dtype: Optional[type] = None, norm: str = "ortho", **kwargs
+    ):
+        """
+        Linear operator that performs convolution in Fourier domain, and assumes
+        real-valued signals.
+
+        Parameters
+        ----------
+        filter :py:class:`~numpy.ndarray`
+            2D filter to use. Must be of shape (height, width, channels) even if
+            only one channel.
+        dtype : float32 or float64
+            Data type to use for optimization.
+        norm : str
+            Normalization to use for convolution. See :py:class:`~lensless.rfft_convolve.RealFFTConvolve2D`
+        """
+        assert len(filter.shape) == 4, "Filter must be of shape (depth, height, width, channels)"
+        self._filter_shape = np.array(filter.shape)
+        self._convolver = Convolver(filter, dtype=dtype, norm=norm)
+
+        shape = (int(np.prod(self._filter_shape)), int(np.prod(self._filter_shape)))
+        super(RealFFTConvolve2D, self).__init__(shape=shape)
+
+    @pycrt.enforce_precision(i="x")
+    @pycu.vectorize(i="x")
+    def apply(self, x: pyct.NDArray) -> pyct.NDArray:
+        y = self._convolver.convolve(np.reshape(x, self._filter_shape))
+        return y.ravel()
+
+    @pycrt.enforce_precision(i="y")
+    @pycu.vectorize(i="y")
+    def adjoint(self, y: pyct.NDArray) -> pyct.NDArray:
+        x = self._convolver.deconvolve(np.reshape(y, self._filter_shape))
+        return x.ravel()
+
+
+class APGD(ReconstructionAlgorithm):
+    def __init__(
+        self,
+        psf,
+        max_iter=500,
+        dtype=np.float32,
+        diff_penalty=None,
+        prox_penalty=APGDPriors.NONNEG,
+        acceleration=True,
+        diff_lambda=0.001,
+        prox_lambda=0.001,
+        disp=100,
+        rel_error=None,
+        lipschitz_tight=True,
+        lipschitz_tol=1.0,
+        **kwargs
+    ):
+        """
+        Wrapper for `Pycsou's PGD <https://github.com/matthieumeo/pycsou/blob/a74b714192821501371c89dbd44eac15a5456a0f/src/pycsou/opt/solver/pgd.py#L17>`__
+        (accelerated proximal gradient descent) applied to lensless imaging.
+
+        Parameters
+        ----------
+        psf : :py:class:`~numpy.ndarray`
+            Point spread function (PSF) that models forward propagation.
+            Must be of shape (depth, height, width, channels) even if
+            depth = 1 and channels = 1. You can use :py:func:`~lensless.io.load_psf`
+            to load a PSF from a file such that it is in the correct format.
+        max_iter : int, optional
+            Maximal number of iterations.
+        dtype : float32 or float64
+            Data type to use for optimization.
+        diff_penalty : None or str or `DiffFunc`
+            Differentiable functional to serve as prior / regularization term.
+            Default is None. See `DiffFunc <https://github.com/matthieumeo/pycsou/blob/a74b714192821501371c89dbd44eac15a5456a0f/src/pycsou/abc/operator.py#L980>`_.
+        prox_penalty : None or str or `ProxFunc`
+            Proximal functional to serve as prior / regularization term. Default
+            is non-negative prior. See `ProxFunc <https://github.com/matthieumeo/pycsou/blob/a74b714192821501371c89dbd44eac15a5456a0f/src/pycsou/abc/operator.py#L741>`_.
+        acceleration : bool, optional
+            Whether to use acceleration or not. Default is True.
+        diff_lambda : float
+            Weight of differentiable penalty.
+        prox_lambda : float
+            Weight of proximal penalty.
+        disp : int, optional
+            Display frequency. Default is 100.
+        rel_error : float, optional
+            Relative error to stop optimization. Default is 1e-6.
+        lipschitz_tight : bool, optional
+            Whether to use tight Lipschitz constant or not. Default is True.
+        lipschitz_tol : float, optional
+            Tolerance to compute Lipschitz constant. Default is 1.
+        """
+
+        assert isinstance(psf, np.ndarray), "PSF must be a numpy array"
+
+        # PSF and data are the same size / shape
+        self._original_shape = psf.shape
+        self._original_size = psf.size
+
+        self._apgd = None
+        self._gen = None
+
+        super(APGD, self).__init__(psf, dtype, n_iter=max_iter, **kwargs)
+
+        self._stop_crit = stop.MaxIter(max_iter)
+        if rel_error is not None:
+            self._stop_crit = self._stop_crit | stop.RelError(eps=rel_error)
+        self._disp = disp
+
+        # Convolution operator
+
+        self._H = RealFFTConvolve2D(self._psf, dtype=dtype)
+        self._H.lipschitz(tol=lipschitz_tol, tight=lipschitz_tight)
+
+        # initialize solvers which will be created when data is set
+        if diff_penalty is not None:
+            if diff_penalty == APGDPriors.L2:
+                self._diff_penalty = diff_lambda * func.SquaredL2Norm(dim=self._H.shape[1])
+            else:
+                assert hasattr(diff_penalty, "jacobian")
+                self._diff_penalty = diff_lambda * diff_penalty(dim=self._H.shape[1])
         else:
-            n_bits = 8
-
-        if back:
-            back_img = cv2.imread(back, cv2.IMREAD_UNCHANGED)
-            dtype = img.dtype
-            img = img.astype(np.float32) - back_img.astype(np.float32)
-            img = np.clip(img, a_min=0, a_max=img.max())
-            img = img.astype(dtype)
-        if nbits_out is None:
-            nbits_out = n_bits
-        img = bayer2rgb(
-            img,
-            nbits=n_bits,
-            blue_gain=blue_gain,
-            red_gain=red_gain,
-            black_level=black_level,
-            ccm=ccm,
-            nbits_out=nbits_out,
-        )
+            self._diff_penalty = None
 
-    else:
-        if len(img.shape) == 3:
-            img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
-
-    if flip:
-        img = np.flipud(img)
-        img = np.fliplr(img)
-
-    if verbose:
-        print_image_info(img)
-
-    return img
-
-
-def load_psf(
-    fp,
-    downsample=1,
-    return_float=True,
-    bg_pix=(5, 25),
-    return_bg=False,
-    flip=False,
-    verbose=False,
-    bayer=False,
-    blue_gain=None,
-    red_gain=None,
-    dtype=np.float32,
-    nbits_out=None,
-    single_psf=False,
-    shape=None,
-):
-    """
-    Load and process PSF for analysis or for reconstruction.
+        if prox_penalty is not None:
+            if prox_penalty == APGDPriors.L1:
+                self._prox_penalty = prox_lambda * func.L1Norm(dim=self._H.shape[1])
+            elif prox_penalty == APGDPriors.NONNEG:
+                self._prox_penalty = prox_lambda * func.PositiveOrthant(dim=self._H.shape[1])
+            else:
+                try:
+                    self._prox_penalty = prox_lambda * prox_penalty(dim=self._H.shape[1])
+                except ValueError:
+                    print("Unexpected prior.")
+        else:
+            self._prox_penalty = None
 
-    Basic steps are:
-    - Load image.
-    - (Optionally) subtract background. Recommended.
-    - (Optionally) resize to more manageable size
-    - (Optionally) normalize within [0, 1] if using for reconstruction; otherwise cast back to uint for analysis.
-
-    Parameters
-    ----------
-    fp : str
-        Full path to file.
-    downsample : int, optional
-        Downsampling factor. Recommended for image reconstruction.
-    return_float : bool, optional
-        Whether to return PSF as float array, or unsigned int.
-    bg_pix : tuple, optional
-        Section of pixels to take from top left corner to remove background level. Set to `None` to omit this
-        step, althrough it is highly recommended.
-    return_bg : bool, optional
-        Whether to return background level, for removing from data for reconstruction.
-    flip : bool, optional
-        Whether to flip up-down and left-right.
-    verbose : bool
-        Whether to print metadata.
-    bayer : bool
-        Whether input data is Bayer.
-    blue_gain : float
-        Blue gain for color correction.
-    red_gain : float
-        Red gain for color correction.
-    dtype : float32 or float64
-        Data type of returned data.
-    nbits_out : int
-        Output bit depth. Default is to use that of input.
-    single_psf : bool
-        Whether to sum RGB channels into single PSF, same across channels. Done
-        in "Learned reconstructions for practical mask-based lensless imaging"
-        of Kristina Monakhova et. al.
-
-    Returns
-    -------
-    psf :py:class:`~numpy.ndarray`
-        2-D array of PSF.
-    """
+        self._acc = acceleration
 
-    # load image data and extract necessary channels
-    psf = load_image(
-        fp,
-        verbose=verbose,
-        flip=flip,
-        bayer=bayer,
-        blue_gain=blue_gain,
-        red_gain=red_gain,
-        nbits_out=nbits_out,
-    )
-
-    original_dtype = psf.dtype
-    psf = np.array(psf, dtype=dtype)
-
-    # subtract background, assume black edges
-    bg = np.zeros(3)
-    if bg_pix is not None:
-        bg = []
-        for i in range(3):
-            bg_i = np.mean(psf[bg_pix[0] : bg_pix[1], bg_pix[0] : bg_pix[1], i])
-            psf[:, :, i] -= bg_i
-            bg.append(bg_i)
-        psf = np.clip(psf, a_min=0, a_max=psf.max())
-        bg = np.array(bg)
-
-    # resize
-    if shape:
-        psf = resize(psf, shape=shape)
-    elif downsample != 1:
-        psf = resize(psf, factor=1 / downsample)
-
-    if single_psf:
-        assert len(psf.shape) == 3
-        # TODO : in Lensless Learning, they sum channels --> `psf_diffuser = np.sum(psf_diffuser,2)`
-        # https://github.com/Waller-Lab/LenslessLearning/blob/master/pre-trained%20reconstructions.ipynb
-        psf = np.sum(psf, 2)
-        psf = psf[:, :, np.newaxis]
-
-    # normalize
-    if return_float:
-        # psf /= psf.max()
-        psf /= np.linalg.norm(psf.ravel())
-    else:
-        psf = psf.astype(original_dtype)
-
-    if return_bg:
-        return psf, bg
-    else:
-        return psf
-
-
-def load_data(
-    psf_fp,
-    data_fp,
-    downsample=None,
-    bg_pix=(5, 25),
-    plot=True,
-    flip=False,
-    bayer=False,
-    blue_gain=None,
-    red_gain=None,
-    gamma=None,
-    gray=False,
-    dtype=np.float32,
-    single_psf=False,
-    shape=None,
-):
-    """
-    Load data for image reconstruction.
+    def set_data(self, data):
+        """
+        For ``APGD``, we use data to initialize problem for Pycsou.
+
+        Parameters
+        ----------
+        data : :py:class:`~numpy.ndarray`
+            Lensless data on which to iterate to recover an estimate of the
+             scene. Should match provide PSF, i.e. shape and 2D (grayscale) or
+             3D (RGB).
+
+        """
+        super(APGD, self).set_data(
+            np.repeat(data, self._original_shape[-4], axis=0)
+        )  # we repeat the data for each depth to match the size of the PSF
+
+        """ Set up problem """
+        # Cost function
+        loss = (1 / 2) * func.SquaredL2Norm(dim=self._H.shape[0]).asloss(self._data.ravel())
+        F = loss * self._H
+        if self._diff_penalty is not None:
+            F += self._diff_penalty
 
-    Parameters
-    ----------
-    psf_fp : str
-        Full path to PSF file.
-    data_fp : str
-        Full path to measurement file.
-    downsample : int or float
-        Downsampling factor.
-    bg_pix : tuple, optional
-        Section of pixels to take from top left corner to remove background
-        level. Set to `None` to omit this step, although it is highly
-        recommended.
-    plot : bool, optional
-        Whether or not to plot PSF and raw data.
-    flip : bool
-        Whether to flip data (vertical and horizontal).
-    bayer : bool
-        Whether input data is Bayer.
-    blue_gain : float
-        Blue gain for color correction.
-    red_gain : float
-        Red gain for color correction.
-    gamma : float, optional
-        Optional gamma factor to apply, ONLY for plotting. Default is None.
-    gray : bool
-        Whether to load as grayscale or RGB.
-    dtype : float32 or float64
-        Data type of returned data.
-    single_psf : bool
-        Whether to sum RGB channels into single PSF, same across channels. Done
-        in "Learned reconstructions for practical mask-based lensless imaging"
-        of Kristina Monakhova et. al.
-
-    Returns
-    -------
-    psf :py:class:`~numpy.ndarray`
-        2-D array of PSF.
-    data :py:class:`~numpy.ndarray`
-        2-D array of raw measurement data.
-    """
+        self._apgd = solver.PGD(
+            f=F, g=self._prox_penalty, show_progress=False, verbosity=self._disp
+        )
 
-    assert os.path.isfile(psf_fp)
-    assert os.path.isfile(data_fp)
-    if shape is None:
-        assert downsample is not None
-
-    # load and process PSF data
-    psf, bg = load_psf(
-        psf_fp,
-        downsample=downsample,
-        return_float=True,
-        bg_pix=bg_pix,
-        return_bg=True,
-        flip=flip,
-        bayer=bayer,
-        blue_gain=blue_gain,
-        red_gain=red_gain,
-        dtype=dtype,
-        single_psf=single_psf,
-        shape=shape,
-    )
-
-    # load and process raw measurement
-    data = load_image(data_fp, flip=flip, bayer=bayer, blue_gain=blue_gain, red_gain=red_gain)
-    data = np.array(data, dtype=dtype)
-
-    data -= bg
-    data = np.clip(data, a_min=0, a_max=data.max())
-    if data.shape != psf.shape:
-        # in DiffuserCam dataset, images are already reshaped
-        data = resize(data, shape=psf.shape[:2])
-    data /= np.linalg.norm(data.ravel())
-
-    if gray:
-        psf = rgb2gray(psf)
-        data = rgb2gray(data)
-
-    if plot:
-        ax = plot_image(psf, gamma=gamma)
-        ax.set_title("PSF")
-        ax = plot_image(data, gamma=gamma)
-        ax.set_title("Raw data")
+        self._apgd.fit(
+            x0=np.zeros(F.shape[1]),
+            # x0=np.random.normal(size=F.shape[1]),
+            stop_crit=self._stop_crit,
+            track_objective=True,
+            mode=pyca.solver.Mode.MANUAL,
+            acceleration=self._acc,
+        )
 
-    psf = np.array(psf, dtype=dtype)
-    data = np.array(data, dtype=dtype)
+    def reset(self):
+        if self._initial_est is not None:
+            self._image_est = self._initial_est
+        else:
+            self._image_est = np.zeros(self._original_size, dtype=self._dtype)
 
-    return psf, data
+    def _update(self, iter):
+        res = next(self._apgd.steps())
+        self._image_est[:] = res["x"]
+
+    def _form_image(self):
+        image = self._image_est.reshape(self._original_shape)
+        image[image < 0] = 0
+        return image
```

### Comparing `lensless-1.0.2/lensless/mirflickr.py` & `lensless-1.0.4/lensless/mirflickr.py`

 * *Files identical despite different names*

### Comparing `lensless-1.0.2/lensless/plot.py` & `lensless-1.0.4/lensless/plot.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 import numpy as np
 import warnings
 import matplotlib.pyplot as plt
 
-from lensless.util import FLOAT_DTYPES, get_max_val, gamma_correction
+from lensless.util import FLOAT_DTYPES, get_max_val, gamma_correction, autocorr2d
 
-try:
-    from lensless.autocorr_sol import autocorr2d
-except:
-    from lensless.autocorr import autocorr2d
 
-
-def plot_image(img, ax=None, gamma=None, normalize=True):
+def plot_image(img, ax=None, gamma=None, normalize=True, axis=0):
     """
     Plot image data.
 
     Parameters
     ----------
     img : :py:class:`~numpy.ndarray`
         Data to plot.
-    ax :py:class:`~matplotlib.axes.Axes`, optional
+    ax : :py:class:`~matplotlib.axes.Axes`, optional
         `Axes` object to fill for plotting/saving, default is to create one.
     gamma : float, optional
-            Gamma correction factor to apply for plots. Default is None.
+        Gamma correction factor to apply for plots. Default is None.
     normalize : bool
         Whether to normalize data to maximum range. Default is True.
+    axis : int
+        For 3D data, the axis on which to project the data
 
     Returns
     -------
-    ax :py:class:`~matplotlib.axes.Axes`, optional
-        `Axes` object to fill for plotting/saving, default is to create one.
-
+    ax : :py:class:`~matplotlib.axes.Axes`
+        Axes on which image is plot.
     """
 
     if ax is None:
         _, ax = plt.subplots()
 
     max_val = img.max()
     if not normalize:
@@ -43,20 +39,41 @@
             max_val = 1
 
     # need float image for gamma correction and plotting
     img_norm = img / max_val
     if gamma and gamma > 1:
         img_norm = gamma_correction(img_norm, gamma=gamma)
 
-    if len(img.shape) == 3 and img.shape[2] == 3:
-        ax.imshow(img_norm)
-    elif len(img.shape) == 3 and img.shape[2] == 1:
-        ax.imshow(img_norm[:, :, 0], cmap="gray")
-    elif len(img.shape) == 2:
+    # full data format : [depth, width, height, color]
+    if len(img.shape) == 4:
+        if img.shape[3] == 3:  # 3d rgb
+            sum_img = np.sum(img_norm, axis=axis)
+            ax.imshow(sum_img)
+
+        else:
+            assert img.shape[3] == 1  # 3d grayscale with color channel extended
+            sum_img = np.sum(img_norm[:, :, :, 0], axis=axis)
+            ax.imshow(sum_img, cmap="gray")
+
+    # data of length 3 means we have to infer whichever depth or color is missing, based on shape.
+    elif len(img.shape) == 3:
+        if img.shape[2] == 3:  # 2D rgb
+            ax.imshow(img_norm)
+
+        elif img.shape[2] == 1:  # 2D grayscale with color channel extended
+            ax.imshow(img_norm[:, :, 0], cmap="gray")
+
+        else:  # 3D grayscale
+            sum_img = np.sum(img_norm, axis=axis)
+            ax.imshow(sum_img, cmap="gray")
+
+    # data of length 2 means we have only width and height
+    elif len(img.shape) == 2:  # 2D grayscale
         ax.imshow(img_norm, cmap="gray")
+
     else:
         raise ValueError(f"Unexpected data shape : {img_norm.shape}")
 
     return ax
 
 
 def pixel_histogram(img, nbits=None, ax=None, log_scale=True):
@@ -73,14 +90,15 @@
             `Axes` object to fill, default is to create one.
     log_scale : bool, optional
         Whether to use log scale in counting number of pixels.
 
     Return
     ------
     ax : :py:class:`~matplotlib.axes.Axes`
+        Axes on which histogram is plot.
     """
     if ax is None:
         _, ax = plt.subplots()
 
     if nbits:
         # max_val = get_max_val(img, nbits)
         max_val = 2**nbits - 1
@@ -132,14 +150,15 @@
         `Axes` object to fill, default is to create one.
     dB : bool, optional
         Whether to plot in dB scale.
 
     Return
     ------
     ax : :py:class:`~matplotlib.axes.Axes`
+        Axes on which cross-section is plot.
     """
 
     if ax is None:
         _, ax = plt.subplots()
 
     # get cross-section
     if idx is None:
@@ -200,15 +219,17 @@
         Desired padding. See NumPy documentation: https://numpy.org/doc/stable/reference/generated/numpy.pad.html
     ax : :py:class:`~matplotlib.axes.Axes`, optional
             `Axes` object to fill, default is to create one.
 
     Return
     ------
     ax : :py:class:`~matplotlib.axes.Axes`
+        Axes on which auto-correlation is plot.
     autocorr : py:class:`~numpy.ndarray`
+        Auto-correlation.
     """
 
     nbit_plot = 8
     max_val_plot = 2**nbit_plot - 1
 
     # compute autocorrelation
     autocorr = autocorr2d(vals, pad_mode=pad_mode)
```

### Comparing `lensless-1.0.2/lensless/util.py` & `lensless-1.0.4/lensless/util.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,110 +1,143 @@
 import cv2
 import csv
 import numpy as np
 from lensless.constants import RPI_HQ_CAMERA_CCM_MATRIX, RPI_HQ_CAMERA_BLACK_LEVEL
 
+try:
+    import torch
+    import torchvision.transforms as tf
+
+    torch_available = True
+except ImportError:
+    torch_available = False
 
 SUPPORTED_BIT_DEPTH = np.array([8, 10, 12, 16])
 FLOAT_DTYPES = [np.float32, np.float64]
 
 
 def resize(img, factor=None, shape=None, interpolation=cv2.INTER_CUBIC):
     """
     Resize by given factor.
 
     Parameters
     ----------
-    img :py:class:`~numpy.ndarray`
+    img : :py:class:`~numpy.ndarray`
         Downsampled image.
     factor : int or float
         Resizing factor.
     shape : tuple
         (Height, width).
     interpolation : OpenCV interpolation method
         See https://docs.opencv.org/2.4/modules/imgproc/doc/geometric_transformations.html#cv2.resize
 
     Returns
     -------
-    img :py:class:`~numpy.ndarray`
+    img : :py:class:`~numpy.ndarray`
         Resized image.
     """
     min_val = img.min()
     max_val = img.max()
-    img_shape = np.array(img.shape)[:2]
-    if shape is None:
-        assert factor is not None
-        new_shape = tuple((img_shape * factor).astype(int))
-        new_shape = new_shape[::-1]
-        resized = cv2.resize(img, dsize=new_shape, interpolation=interpolation)
+    img_shape = np.array(img.shape)[-3:-1]
+
+    assert not ((factor is None) and (shape is None)), "Must specify either factor or shape"
+    new_shape = tuple((img_shape * factor).astype(int)) if (shape is None) else shape[-3:-1]
+
+    if np.array_equal(img_shape, new_shape):
+        return img
+
+    if torch_available:
+        # torch resize expects an input of form [color, depth, width, height]
+        tmp = np.moveaxis(img, -1, 0)
+        resized = tf.Resize(size=new_shape, interpolation=interpolation)(
+            torch.from_numpy(tmp)
+        ).numpy()
+        resized = np.moveaxis(resized, 0, -1)
+
     else:
-        if np.array_equal(img_shape, shape[::-1]):
-            return img
-        resized = cv2.resize(img, dsize=shape[::-1], interpolation=interpolation)
+        resized = np.array(
+            [
+                cv2.resize(img[i], dsize=new_shape[::-1], interpolation=interpolation)
+                for i in range(img.shape[-4])
+            ]
+        )
+        # OpenCV discards channel dimension if it is 1, put it back
+        if len(resized.shape) == 3:
+            # resized = resized[:, :, :, np.newaxis]
+            resized = np.expand_dims(resized, axis=-1)
+
     return np.clip(resized, min_val, max_val)
 
 
 def rgb2gray(rgb, weights=None):
     """
     Convert RGB array to grayscale.
 
     Parameters
     ----------
     rgb : :py:class:`~numpy.ndarray`
-        (N_height, N_width, N_channel) image.
+        (Depth, Height, Width, Channel) image.
     weights : :py:class:`~numpy.ndarray`
         [Optional] (3,) weights to convert from RGB to grayscale.
 
     Returns
     -------
     img :py:class:`~numpy.ndarray`
-        Grayscale image of dimension (height, width).
+        Grayscale image of dimension (depth, height, width, 1).
 
     """
+    assert len(rgb.shape) == 4, "Input must be (depth, height, width, channel)"
     if weights is None:
-        weights = np.array([0.299, 0.587, 0.144])
+        weights = np.array([0.299, 0.587, 0.114])
     assert len(weights) == 3
-    return np.tensordot(rgb, weights, axes=((2,), 0))
+    return np.tensordot(rgb, weights, axes=((3,), 0))[:, :, :, np.newaxis]
 
 
 def gamma_correction(vals, gamma=2.2):
     """
-    Tutorials
-    - https://www.cambridgeincolour.com/tutorials/gamma-correction.htm
-    - (code, for images) https://www.pyimagesearch.com/2015/10/05/opencv-gamma-correction/
-        https://lindevs.com/apply-gamma-correction-to-an-image-using-opencv/
-    - (code) http://www.fourmilab.ch/documents/specrend/specrend.c
+    Apply `gamma correction <https://www.cambridgeincolour.com/tutorials/gamma-correction.htm>`__.
 
     Parameters
     ----------
-    vals : array_like
+    vals : :py:class:`~numpy.ndarray`
         RGB values to gamma correct.
     gamma : float, optional
-            Gamma correction factor to apply for plots. Default is None.
+        Gamma correction factor.
 
     Returns
     -------
-    vals : array_like
+    vals : :py:class:`~numpy.ndarray`
         Gamma-corrected data.
 
     """
 
-    # simple approach
-    # return np.power(vals, 1 / gamma)
-
     # Rec. 709 gamma correction
     # http://www.fourmilab.ch/documents/specrend/specrend.c
     cc = 0.018
     inv_gam = 1 / gamma
     clip_val = (1.099 * np.power(cc, inv_gam) - 0.099) / cc
     return np.where(vals < cc, vals * clip_val, 1.099 * np.power(vals, inv_gam) - 0.099)
 
 
 def get_max_val(img, nbits=None):
-    """For uint image"""
+    """
+    For uint image.
+
+    Parameters
+    ----------
+    img : :py:class:`~numpy.ndarray`
+        Image array.
+    nbits : int, optional
+        Number of bits per pixel. Detect if not provided.
+
+    Returns
+    -------
+    max_val : int
+        Maximum pixel value.
+    """
     assert img.dtype not in FLOAT_DTYPES
     if nbits is None:
         nbits = int(np.ceil(np.log2(img.max())))
 
     if nbits not in SUPPORTED_BIT_DEPTH:
         nbits = SUPPORTED_BIT_DEPTH[nbits < SUPPORTED_BIT_DEPTH][0]
     max_val = 2**nbits - 1
@@ -122,19 +155,20 @@
     red_gain=None,
     black_level=RPI_HQ_CAMERA_BLACK_LEVEL,
     ccm=RPI_HQ_CAMERA_CCM_MATRIX,
     nbits_out=None,
 ):
     """
     Convert raw Bayer data to RGB with the following steps:
-    - Demosaic with bi-linear interpolation, mapping the Bayer array to RGB.
-    - Black level removal.
-    - White balancing, applying gains to red and blue channels.
-    - Color correction matrix.
-    - Clip
+
+    #. Demosaic with bi-linear interpolation, mapping the Bayer array to RGB.
+    #. Black level removal.
+    #. White balancing, applying gains to red and blue channels.
+    #. Color correction matrix.
+    #. Clip.
 
     Parameters
     ----------
     img : :py:class:`~numpy.ndarray`
         2D Bayer data to convert to RGB.
     nbits : int
         Bit depth of input data.
@@ -176,14 +210,22 @@
     img = (img.reshape(-1, 3, order="F") @ ccm.T).reshape(img.shape, order="F")
     img[img < 0] = 0
     img[img > 1] = 1
     return (img * (2**nbits_out - 1)).astype(dtype)
 
 
 def get_distro():
+    """
+    Get current OS distribution.
+
+    Returns
+    -------
+    result : str
+        Name and version of OS.
+    """
     # https://majornetwork.net/2019/11/get-linux-distribution-name-and-version-with-python/
     RELEASE_DATA = {}
     with open("/etc/os-release") as f:
         reader = csv.reader(f, delimiter="=")
         for row in reader:
             if row:
                 RELEASE_DATA[row[0]] = row[1]
@@ -195,12 +237,49 @@
         if version_split[0] == major_version:
             # Just major version shown, replace it with the full version
             RELEASE_DATA["VERSION"] = " ".join([DEBIAN_VERSION] + version_split[1:])
     return f"{RELEASE_DATA['NAME']} {RELEASE_DATA['VERSION']}"
 
 
 def print_image_info(img):
+    """
+    Print dimensions, data type, max, min, mean.
+    """
     print("dimensions : {}".format(img.shape))
     print("data type : {}".format(img.dtype))
     print("max  : {}".format(img.max()))
     print("min  : {}".format(img.min()))
     print("mean : {}".format(img.mean()))
+
+
+def autocorr2d(vals, pad_mode="reflect"):
+    """
+    Compute 2-D autocorrelation of image via the FFT.
+
+    Parameters
+    ----------
+    vals : :py:class:`~numpy.ndarray`
+        2-D image.
+    pad_mode : str
+        Desired padding. See NumPy documentation: https://numpy.org/doc/stable/reference/generated/numpy.pad.html
+
+    Return
+    ------
+    autocorr : :py:class:`~numpy.ndarray`
+    """
+
+    shape = vals.shape
+    assert len(shape) == 2
+
+    # pad
+    vals_padded = np.pad(
+        vals,
+        pad_width=((shape[0] // 2, shape[0] // 2), (shape[1] // 2, shape[1] // 2)),
+        mode=pad_mode,
+    )
+
+    # compute autocorrelation via DFT
+    X = np.fft.rfft2(vals_padded)
+    autocorr = np.fft.ifftshift(np.fft.irfft2(X * X.conj()))
+
+    # remove padding
+    return autocorr[shape[0] // 2 : -shape[0] // 2, shape[1] // 2 : -shape[1] // 2]
```

### Comparing `lensless-1.0.2/setup.py` & `lensless-1.0.4/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 import setuptools
 
-with open("README.md", "r") as fh:
+# import version from file -> `__version__`
+__version__ = None
+with open("lensless/version.py") as f:
+    exec(f.read())
+assert __version__ is not None
+
+with open("README.rst", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lensless",
-    version="1.0.2",
+    version=__version__,
     author="Eric Bezzam",
     author_email="ebezzam@gmail.com",
     description="Package to control and image with a lensless camera running on a Raspberry Pi.",
     long_description=long_description,
-    long_description_content_type="text/markdown",
+    long_description_content_type="text/x-rst",
     url="https://github.com/LCAV/LenslessPiCam",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.6",
+    python_requires=">=3.8.1",
     install_requires=[
-        "opencv-python==4.5.1.48",
-        "numpy>=1.21",
-        "scipy==1.7.0",
-        "click==8.0.1",
-        "image==1.5.33",
-        "picamerax==20.9.1",
-        "matplotlib==3.4.2",
+        "opencv-python>=4.5.1.48",
+        "numpy>=1.22, <=1.23.5",
+        "scipy>=1.7.0",
+        "image>=1.5.33",
+        "matplotlib>=3.4.2",
+        "rawpy>=0.16.0",
     ],
     extra_requires={"dev": ["pudb", "black"]},
 )
```

### Comparing `lensless-1.0.2/test/test_io.py` & `lensless-1.0.4/test/test_io.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 psf_fp = "data/psf/tape_rgb.png"
 data_fp = "data/raw_data/thumbs_up_rgb.png"
 downsample = 8
 
 
 def test_load_data():
     for gray in [True, False]:
-        for dtype in [np.float32, np.float64]:
+        for dtype in ["float32", "float64"]:
             psf, data = load_data(
                 psf_fp=psf_fp,
                 data_fp=data_fp,
                 downsample=downsample,
                 plot=False,
                 gray=gray,
                 dtype=dtype,
             )
-            if gray:
-                assert len(psf.shape) == 2
-            else:
-                assert len(psf.shape) == 3
-            assert psf.shape == data.shape
+            assert psf.shape[3] == (1 if gray else 3)
+            assert len(psf.shape) == 4
+            assert len(data.shape) == 4
+            assert data.shape[0] == 1
+            assert psf.shape[1:] == data.shape[1:]
             assert psf.dtype == dtype, dtype
             assert data.dtype == dtype, dtype
 
 
 test_load_data()
```

