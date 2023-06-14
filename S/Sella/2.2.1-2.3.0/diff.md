# Comparing `tmp/Sella-2.2.1.tar.gz` & `tmp/Sella-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Sella-2.2.1.tar", last modified: Fri Jan 13 20:18:22 2023, max compression
+gzip compressed data, was "Sella-2.3.0.tar", last modified: Wed Jun 14 21:21:12 2023, max compression
```

## Comparing `Sella-2.2.1.tar` & `Sella-2.3.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 20:18:22.644090 Sella-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-01-13 20:18:00.000000 Sella-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-01-13 20:18:00.000000 Sella-2.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-01-13 20:18:22.644090 Sella-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-01-13 20:18:00.000000 Sella-2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 20:18:22.640090 Sella-2.2.1/Sella.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-01-13 20:18:22.000000 Sella-2.2.1/Sella.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-01-13 20:18:22.000000 Sella-2.2.1/Sella.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 20:18:22.000000 Sella-2.2.1/Sella.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-13 20:18:22.000000 Sella-2.2.1/Sella.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-13 20:18:22.000000 Sella-2.2.1/Sella.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-01-13 20:18:00.000000 Sella-2.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-01-13 20:18:00.000000 Sella-2.2.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 20:18:22.644090 Sella-2.2.1/sella/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-01-13 20:18:00.000000 Sella-2.2.1/sella/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-01-13 20:18:00.000000 Sella-2.2.1/sella/eigensolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)    21272 2023-01-13 20:18:00.000000 Sella-2.2.1/sella/force_match.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-01-13 20:18:00.000000 Sella-2.2.1/sella/hessian_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    54069 2023-01-13 20:18:00.000000 Sella-2.2.1/sella/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)    10531 2023-01-13 20:18:00.000000 Sella-2.2.1/sella/linalg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 20:18:22.644090 Sella-2.2.1/sella/optimize/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-13 20:18:00.000000 Sella-2.2.1/sella/optimize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-01-13 20:18:00.000000 Sella-2.2.1/sella/optimize/irc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-01-13 20:18:00.000000 Sella-2.2.1/sella/optimize/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-01-13 20:18:00.000000 Sella-2.2.1/sella/optimize/restricted_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-01-13 20:18:00.000000 Sella-2.2.1/sella/optimize/stepper.py
--rw-r--r--   0 runner    (1001) docker     (123)    18883 2023-01-13 20:18:00.000000 Sella-2.2.1/sella/peswrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-01-13 20:18:00.000000 Sella-2.2.1/sella/samd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 20:18:22.644090 Sella-2.2.1/sella/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-13 20:18:00.000000 Sella-2.2.1/sella/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-01-13 20:18:00.000000 Sella-2.2.1/sella/utilities/blas.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-01-13 20:18:00.000000 Sella-2.2.1/sella/utilities/math.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-13 20:18:22.644090 Sella-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-01-13 20:18:00.000000 Sella-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:21:12.060397 Sella-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-06-14 21:20:40.000000 Sella-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-14 21:20:40.000000 Sella-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-14 21:21:12.060397 Sella-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-14 21:20:40.000000 Sella-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:21:12.060397 Sella-2.3.0/Sella.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-14 21:21:11.000000 Sella-2.3.0/Sella.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-14 21:21:12.000000 Sella-2.3.0/Sella.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 21:21:11.000000 Sella-2.3.0/Sella.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-14 21:21:11.000000 Sella-2.3.0/Sella.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-14 21:21:11.000000 Sella-2.3.0/Sella.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-14 21:20:40.000000 Sella-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-14 21:20:40.000000 Sella-2.3.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:21:12.060397 Sella-2.3.0/sella/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-14 21:20:40.000000 Sella-2.3.0/sella/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-06-14 21:20:40.000000 Sella-2.3.0/sella/eigensolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21272 2023-06-14 21:20:40.000000 Sella-2.3.0/sella/force_match.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-06-14 21:20:40.000000 Sella-2.3.0/sella/hessian_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56037 2023-06-14 21:20:40.000000 Sella-2.3.0/sella/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10618 2023-06-14 21:20:40.000000 Sella-2.3.0/sella/linalg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:21:12.060397 Sella-2.3.0/sella/optimize/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-14 21:20:40.000000 Sella-2.3.0/sella/optimize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-06-14 21:20:40.000000 Sella-2.3.0/sella/optimize/irc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-06-14 21:20:40.000000 Sella-2.3.0/sella/optimize/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-06-14 21:20:40.000000 Sella-2.3.0/sella/optimize/restricted_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-14 21:20:40.000000 Sella-2.3.0/sella/optimize/stepper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20857 2023-06-14 21:20:40.000000 Sella-2.3.0/sella/peswrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-14 21:20:40.000000 Sella-2.3.0/sella/samd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:21:12.060397 Sella-2.3.0/sella/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 21:20:40.000000 Sella-2.3.0/sella/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-06-14 21:20:40.000000 Sella-2.3.0/sella/utilities/blas.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-06-14 21:20:40.000000 Sella-2.3.0/sella/utilities/math.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-14 21:21:12.060397 Sella-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-14 21:20:40.000000 Sella-2.3.0/setup.py
```

### Comparing `Sella-2.2.1/LICENSE` & `Sella-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Sella-2.2.1/PKG-INFO` & `Sella-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sella
-Version: 2.2.1
+Version: 2.3.0
 Author: Eric Hermes
 Author-email: ehermes@sandia.gov
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Natural Language :: English
```

### Comparing `Sella-2.2.1/README.md` & `Sella-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `Sella-2.2.1/Sella.egg-info/PKG-INFO` & `Sella-2.3.0/Sella.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sella
-Version: 2.2.1
+Version: 2.3.0
 Author: Eric Hermes
 Author-email: ehermes@sandia.gov
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Natural Language :: English
```

### Comparing `Sella-2.2.1/Sella.egg-info/SOURCES.txt` & `Sella-2.3.0/Sella.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Sella-2.2.1/sella/eigensolvers.py` & `Sella-2.3.0/sella/eigensolvers.py`

 * *Files identical despite different names*

### Comparing `Sella-2.2.1/sella/force_match.pyx` & `Sella-2.3.0/sella/force_match.pyx`

 * *Files identical despite different names*

### Comparing `Sella-2.2.1/sella/hessian_update.py` & `Sella-2.3.0/sella/hessian_update.py`

 * *Files identical despite different names*

### Comparing `Sella-2.2.1/sella/internal.py` & `Sella-2.3.0/sella/internal.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import (
-    Tuple, Callable, Iterator, Union, TypeVar, Optional, List, Dict
+    Tuple, Callable, Iterator, Union, TypeVar, Optional, List, Dict, Type
 )
 from itertools import (
     product,
     combinations,
     combinations_with_replacement as cwr
 )
 from functools import partialmethod
@@ -49,58 +49,157 @@
 
 def _hessian(
     func: Callable[[jnp.ndarray, jnp.ndarray, jnp.ndarray], float]
 ) -> Callable[[jnp.ndarray, jnp.ndarray, jnp.ndarray], jnp.ndarray]:
     return jit(jacfwd(jacrev(func, argnums=0), argnums=0))
 
 
-class Internal:
+class Coordinate:
     nindices = None
-    union = None
-    diff = None
+    kwargs = None
 
     def __init__(
         self,
         indices: Tuple[int, ...],
-        ncvecs: Tuple[IVec, ...] = None
     ) -> None:
         if self.nindices is not None:
             assert len(indices) == self.nindices
         self.indices = np.array(indices, dtype=np.int32)
+        self.kwargs = dict()
+
+    def reverse(self) -> 'Coordinate':
+        raise NotImplementedError
+
+    def __eq__(self, other: 'Coordinate') -> bool:
+        if not isinstance(other, self.__class__):
+            return NotImplemented
+        if len(self.indices) != len(other.indices):
+            return False
+        if np.all(self.indices == other.indices):
+            return True
+        return False
+
+    def __add__(self, other: 'Coordinate') -> 'Coordinate':
+        raise NotImplementedError
+
+    def split(self) -> Tuple['Coordinate', 'Coordinate']:
+        raise NotImplementedError
+
+    def __repr__(self) -> str:
+        out = [f'indices={self.indices}']
+        out += [f'{key}={val}' for key, val in self.kwargs.items()]
+        str_out = ', '.join(out)
+        return f'{self.__class__.__name__}({str_out})'
+
+    @staticmethod
+    def _eval0(pos: jnp.ndarray, **kwargs) -> float:
+        raise NotImplementedError
+
+    @staticmethod
+    def _eval1(pos: jnp.ndarray, **kwargs) -> jnp.ndarray:
+        raise NotImplementedError
+
+    @staticmethod
+    def _eval2(pos: jnp.ndarray, **kwargs) -> jnp.ndarray:
+        raise NotImplementedError
+
+    def calc(self, atoms: Atoms) -> float:
+        return float(self._eval0(
+            atoms[self.indices].positions, **self.kwargs
+        ))
+
+    def calc_gradient(self, atoms: Atoms) -> np.ndarray:
+        return np.array(self._eval1(
+            atoms[self.indices].positions, **self.kwargs
+        ))
+
+    def calc_hessian(self, atoms: Atoms) -> jnp.ndarray:
+        return np.array(self._eval2(
+            atoms[self.indices].positions, **self.kwargs
+        ))
+
+    def _check_derivative(
+        self, atoms: Atoms, delta: float, atol: float, order: int
+    ) -> bool:
+        if order == 1:
+            derivative = 'Gradient'
+            f0 = self.calc
+            f1 = self.calc_gradient
+        elif order == 2:
+            derivative = 'Hessian'
+            f0 = self.calc_gradient
+            f1 = self.calc_hessian
+        else:
+            raise ValueError(f'Order {order} gradients are not implemented')
+
+        atoms0 = atoms.copy()
+        g_ref = f1(atoms0)
+        g_numer = np.zeros_like(g_ref)
+        atoms = atoms0.copy()
+        for i, idx in enumerate(self.indices):
+            for j in range(3):
+                atoms.positions[idx, j] = atoms0.positions[idx, j] + delta
+                fplus = f0(atoms)
+                atoms.positions[idx, j] = atoms0.positions[idx, j] - delta
+                fminus = f0(atoms)
+                g_numer[i, j] = (fplus - fminus) / (2 * delta)
+                atoms.positions[idx, j] = atoms0.positions[idx, j]
+        if np.max(np.abs(g_numer - g_ref)) > atol:
+            warnings.warn(f'{derivative}s for {self} failed numerical test!')
+            return False
+        return True
+
+    def check_gradient(
+        self, atoms: Atoms, delta: float = 1e-4, atol: float = 1e-6
+    ) -> bool:
+        return self._check_derivative(atoms, delta, atol, order=1)
+
+    def check_hessian(
+        self, atoms: Atoms, delta: float = 1e-4, atol: float = 1e-6
+    ) -> bool:
+        return self._check_derivative(atoms, delta, atol, order=2)
+
+
+class Internal(Coordinate):
+    union = None
+    diff = None
+
+    def __init__(
+        self,
+        indices: Tuple[int, ...],
+        ncvecs: Tuple[IVec, ...] = None
+    ) -> None:
+        Coordinate.__init__(self, indices)
 
         if self.nindices is not None:
             if ncvecs is None:
                 ncvecs = np.zeros((self.nindices - 1, 3), dtype=np.int32)
             else:
                 ncvecs = np.asarray(ncvecs).reshape((self.nindices - 1, 3))
         else:
             if ncvecs is not None:
                 raise ValueError(
                     "{} does not support ncvecs"
                     .format(self.__class__.__name__)
                 )
             ncvecs = np.empty((0, 3), dtype=np.int32)
-        self.ncvecs = ncvecs
+        self.kwargs['ncvecs'] = ncvecs
 
     def reverse(self) -> 'Internal':
-        return self.__class__(self.indices[::-1], -self.ncvecs[::-1])
+        return self.__class__(self.indices[::-1], -self.kwargs['ncvecs'][::-1])
 
     def __eq__(self, other: object) -> bool:
-        if not isinstance(other, self.__class__):
-            return NotImplemented
-        if (
-            np.all(self.indices == other.indices)
-            and np.all(self.ncvecs == other.ncvecs)
-        ):
-            return True
+        if not Coordinate.__eq__(self, other):
+            return False
         srev = self.reverse()
-        if (
-            np.all(srev.indices == other.indices)
-            and np.all(srev.ncvecs == other.ncvecs)
-        ):
+        if not Coordinate.__eq__(srev, other):
+            return False
+        if np.all(self.kwargs['ncvecs'] == other.kwargs['ncvecs']):
+            return True
+        if np.all(srev.kwargs['ncvecs'] == other.kwargs['ncvecs']):
             return True
         return False
 
     def __add__(self, other: object) -> 'Internal':
         if self.union is None:
             return NotImplemented
         if not isinstance(other, self.__class__):
@@ -110,38 +209,31 @@
                 'Cannot add {} object to itself.'
                 .format(self.__class__.__name__)
             )
 
         for s, o in product([self, self.reverse()], [other, other.reverse()]):
             if (
                 np.all(s.indices[1:] == o.indices[:-1])
-                and np.all(s.ncvecs[1:] == o.ncvecs[:-1])
+                and np.all(s.kwargs['ncvecs'][1:] == o.kwargs['ncvecs'][:-1])
             ):
                 new_indices = [*s.indices, o.indices[-1]]
-                new_ncvecs = [*s.ncvecs, o.ncvecs[-1]]
+                new_ncvecs = [*s.kwargs['ncvecs'], o.kwargs['ncvecs'][-1]]
                 return self.union(new_indices, new_ncvecs)
         raise NoValidInternalError(
             '{} indices do not overlap!'.format(self.__class__.__name__)
         )
 
     def split(self) -> Tuple['Internal', 'Internal']:
         if self.diff is None:
             raise RuntimeError(
                 "Don't know how to split a {}!".format(self.__class__.__name__)
             )
         return (
-            self.diff(self.indices[:-1], self.ncvecs[:-1]),
-            self.diff(self.indices[1:], self.ncvecs[1:])
-        )
-
-    def __repr__(self) -> str:
-        return "{}(indices={}, ncvecs={})".format(
-            self.__class__.__name__,
-            tuple(self.indices),
-            tuple([tuple(vec) for vec in self.ncvecs])
+            self.diff(self.indices[:-1], self.kwargs['ncvecs'][:-1]),
+            self.diff(self.indices[1:], self.kwargs['ncvecs'][1:])
         )
 
     @staticmethod
     def _eval0(
         pos: jnp.ndarray, tvecs: jnp.ndarray
     ) -> float:
         raise NotImplementedError
@@ -155,88 +247,56 @@
     @staticmethod
     def _eval2(
         pos: jnp.ndarray, tvecs: jnp.ndarray
     ) -> jnp.ndarray:
         raise NotImplementedError
 
     def calc(self, atoms: Atoms) -> float:
-        tvecs = jnp.asarray(self.ncvecs @ atoms.cell, dtype=np.float64)
+        tvecs = jnp.asarray(
+            self.kwargs['ncvecs'] @ atoms.cell, dtype=np.float64
+        )
         return float(self._eval0(atoms[self.indices].positions, tvecs))
 
     def calc_gradient(self, atoms: Atoms) -> np.ndarray:
-        tvecs = jnp.asarray(self.ncvecs @ atoms.cell, dtype=np.float64)
+        tvecs = jnp.asarray(
+            self.kwargs['ncvecs'] @ atoms.cell, dtype=np.float64
+        )
         return np.array(self._eval1(atoms[self.indices].positions, tvecs))
 
     def calc_hessian(self, atoms: Atoms) -> jnp.ndarray:
-        tvecs = jnp.asarray(self.ncvecs @ atoms.cell, dtype=np.float64)
+        tvecs = jnp.asarray(
+            self.kwargs['ncvecs'] @ atoms.cell, dtype=np.float64
+        )
         return np.array(self._eval2(atoms[self.indices].positions, tvecs))
 
 
 def _translation(
     pos: jnp.ndarray,
     dim: int,
-    tvecs: jnp.ndarray
 ) -> float:
     return pos[:, dim].mean()
 
 
-class Translation(Internal):
+class Translation(Coordinate):
     def __init__(
         self,
         indices: Tuple[int, ...],
         dim: int,
     ) -> None:
-        self.indices = np.array(sorted(indices), dtype=np.int32)
-        self.ncvecs = np.empty((0, 3), dtype=np.int32)
-        self.dim = dim
-
-    def reverse(self) -> 'Internal':
-        raise NotImplementedError
+        Coordinate.__init__(self, indices)
+        self.kwargs['dim'] = dim
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, self.__class__):
             return NotImplemented
-        # JAX seems subtlely broken. Accessing the last element of a
-        # large jax.numpy.ndarray object is something like 5 orders of
-        # magnitude slower than accessing the last element of a
-        # numpy.ndarray objects, so we convert to numpy.ndarray here.
-        sidx = np.asarray(self.indices, dtype=np.int32)
-        oidx = np.asarray(other.indices, dtype=np.int32)
-        if self.dim != other.dim:
+        if self.kwargs['dim'] != other.kwargs['dim']:
             return False
-        if len(sidx) != len(oidx):
+        if set(self.indices) != set(other.indices):
             return False
-        if np.all(sidx == oidx):
-            return True
-        return False
-
-    def __repr__(self) -> str:
-        return "{}(indices={}, dim={})".format(
-            self.__class__.__name__,
-            tuple(self.indices),
-            self.dim
-        )
-
-    def calc(self, atoms: Atoms) -> float:
-        tvecs = jnp.asarray(self.ncvecs @ atoms.cell, dtype=np.float64)
-        return float(self._eval0(
-            atoms.positions[self.indices], self.dim, tvecs
-        ))
-
-    def calc_gradient(self, atoms: Atoms) -> np.ndarray:
-        tvecs = jnp.asarray(self.ncvecs @ atoms.cell, dtype=np.float64)
-        return np.array(self._eval1(
-            atoms.positions[self.indices], self.dim, tvecs
-            ))
-
-    def calc_hessian(self, atoms: Atoms) -> jnp.ndarray:
-        tvecs = jnp.asarray(self.ncvecs @ atoms.cell, dtype=np.float64)
-        return np.array(self._eval2(
-            atoms.positions[self.indices], self.dim, tvecs
-        ))
+        return True
 
     _eval0 = staticmethod(jit(_translation))
     _eval1 = staticmethod(_gradient(_translation))
     _eval2 = staticmethod(_hessian(_translation))
 
 
 # Nominally, jax.numpy.linalg.eigh supports auto-differentiation,
@@ -325,119 +385,69 @@
     axis: int,
     refpos: jnp.ndarray
 ) -> float:
     q = _rotation_q(pos, refpos)
     return 2 * q[axis + 1] * asinc(q[0])
 
 
-class Rotation(Internal):
+class Rotation(Coordinate):
     def __init__(
         self,
         indices: Tuple[int, ...],
         axis: int,
         refpos: np.ndarray,
     ) -> None:
         assert len(indices) >= 2
-        self.indices = np.array(indices, dtype=np.int32)
-        self.refpos = refpos.copy() - refpos.mean(0)
-        self.axis = axis
-
-    def reverse(self) -> 'Internal':
-        raise NotImplementedError
+        Coordinate.__init__(self, indices)
+        self.kwargs['axis'] = axis
+        self.kwargs['refpos'] = refpos.copy() - refpos.mean(0)
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, self.__class__):
             return NotImplemented
-        if self.axis != other.axis:
+        if self.kwargs['axis'] != other.kwargs['axis']:
             return False
         if len(self.indices) != len(other.indices):
             return False
         if set(self.indices) != set(other.indices):
             return False
+        if np.any(self.kwargs['refpos'] != other.kwargs['refpos']):
+            return False
         return True
 
-    def __repr__(self) -> str:
-        return "{}(indices={}, axis={}, refpos={})".format(
-            self.__class__.__name__,
-            tuple(self.indices),
-            self.axis,
-            self.refpos,
-        )
-
-    def calc(self, atoms: Atoms) -> float:
-        return float(self._eval0(
-            atoms.positions[self.indices], self.axis, self.refpos
-        ))
-
-    def calc_gradient(self, atoms: Atoms) -> np.ndarray:
-        return np.array(self._eval1(
-            atoms.positions[self.indices], self.axis, self.refpos
-        ))
-
-    def calc_hessian(self, atoms: Atoms) -> np.ndarray:
-        return np.array(self._eval2(
-            atoms.positions[self.indices], self.axis, self.refpos
-        ))
-
     _eval0 = staticmethod(jit(_rotation))
     _eval1 = staticmethod(jit(jacfwd(_rotation, argnums=0)))
     _eval2 = staticmethod(jit(jacfwd(jacfwd(_rotation, argnums=0), argnums=0)))
 
 
 def _displacement(
     pos: jnp.ndarray,
     refpos: jnp.ndarray,
     W: jnp.ndarray
 ) -> float:
     dx = (pos - refpos).ravel()
     return dx @ W @ dx
 
 
-class Displacement(Internal):
+class Displacement(Coordinate):
     def __init__(
         self,
         indices: np.ndarray,
         refpos: np.ndarray,
         W: np.ndarray,
     ) -> None:
-        self.indices = indices.copy()
-        self.refpos = refpos.copy()
-        self.W = W.copy()
+        Coordinate.__init__(self, indices)
+        self.kwargs['refpos'] = refpos.copy()
+        self.kwargs['W'] = W.copy()
 
-    def reverse(self) -> 'Internal':
-        raise NotImplementedError
-
-    def __eq__(self, other: object) -> bool:
-        if not isinstance(other, self.__class__):
-            return NotImplemented
+    def __eq__(self, other: Coordinate) -> bool:
+        if not Coordinate.__eq__(self, other):
+            return False
         return np.all(self.refpos == other.refpos)
 
-    def __repr__(self) -> str:
-        return "{}(indices={}, refpos={}, W={})".format(
-            self.__class__.__name__,
-            self.indices,
-            self.refpos,
-            self.W,
-        )
-
-    def calc(self, atoms: Atoms) -> float:
-        return float(self._eval0(
-            atoms.positions[self.indices], self.refpos, self.W
-        ))
-
-    def calc_gradient(self, atoms: Atoms) -> np.ndarray:
-        return np.array(self._eval1(
-            atoms.positions[self.indices], self.refpos, self.W
-        ))
-
-    def calc_hessian(self, atoms: Atoms) -> np.ndarray:
-        return np.array(self._eval2(
-            atoms.positions[self.indices], self.refpos, self.W
-        ))
-
     _eval0 = staticmethod(jit(_displacement))
     _eval1 = staticmethod(jit(_gradient(_displacement)))
     _eval2 = staticmethod(jit(_hessian(_displacement)))
 
 
 def _bond(
     pos: jnp.ndarray,
@@ -451,15 +461,17 @@
 class Bond(Internal):
     nindices = 2
     _eval0 = staticmethod(jit(_bond))
     _eval1 = staticmethod(_gradient(_bond))
     _eval2 = staticmethod(_hessian(_bond))
 
     def calc_vec(self, atoms: Atoms) -> np.ndarray:
-        tvecs = np.asarray(self.ncvecs @ atoms.cell, dtype=np.float64)
+        tvecs = np.asarray(
+            self.kwargs['ncvecs'] @ atoms.cell, dtype=np.float64
+        )
         i, j = self.indices
         return atoms.positions[j] - atoms.positions[i] + tvecs[0]
 
 
 def _angle(
     pos: jnp.ndarray,
     tvecs: jnp.ndarray
@@ -499,14 +511,42 @@
 
 Bond.union = Angle
 Angle.union = Dihedral
 Angle.diff = Bond
 Dihedral.diff = Angle
 
 
+def make_internal(
+    name: str,
+    fun: Callable[[jnp.ndarray, ...], float],
+    nindices: int,
+    use_jit: bool = True,
+    jac: Callable[[jnp.ndarray, ...], jnp.ndarray] = None,
+    hess: Callable[[jnp.ndarray, ...], jnp.ndarray] = None,
+    **kwargs,
+) -> Type[Coordinate]:
+    if jac is None:
+        jac = _gradient(fun)
+    if hess is None:
+        hess = _hessian(fun)
+
+    if use_jit:
+        fun = jit(fun)
+        jac = jit(jac)
+        hess = jit(hess)
+
+    return type(name, (Coordinate,), dict(
+        nindices=nindices,
+        kwargs=kwargs,
+        _eval0=staticmethod(fun),
+        _eval1=staticmethod(jac),
+        _eval2=staticmethod(hess)
+    ))
+
+
 class BaseInternals:
     _names = (
         'translations', 'bonds', 'angles', 'dihedrals', 'other', 'rotations'
     )
 
     def __init__(
         self,
@@ -611,42 +651,53 @@
 
     def calc(self) -> np.ndarray:
         """Calculates the internal coordinate vector."""
         self._cache_check()
         if 'coords' not in self._cache:
             atoms = self.all_atoms
             self._cache['coords'] = np.array([c.calc(atoms) for c in self])
-        return np.array([x for x, a in zip(self._cache['coords'], self._active_mask) if a])
+        return np.array([
+            x for x, a in zip(self._cache['coords'], self._active_mask) if a
+        ])
 
     def jacobian(self) -> np.ndarray:
         """Calculates the internal coordinate Jacobian matrix."""
         self._cache_check()
         if 'jacobian' not in self._cache:
             atoms = self.all_atoms
             self._cache['jacobian'] = [
                 np.array(c.calc_gradient(atoms)) for c in self
             ]
-        indices = [np.array(c.indices) for c, a in zip(self, self._active_mask) if a]
+        indices = []
+        jacs = []
+        for coord, jac, active in zip(
+            self, self._cache['jacobian'], self._active_mask
+        ):
+            if active:
+                indices.append(np.array(coord.indices))
+                jacs.append(jac)
         return SparseInternalJacobian(
             self.natoms + self.ndummies,
             indices,
-            [j for j, a in zip(self._cache['jacobian'], self._active_mask) if a]
+            jacs,
         ).asarray()
 
     def hessian(self) -> np.ndarray:
         """Calculates the Hessian matrix for each internal coordinate."""
         self._cache_check()
         if 'hessian' not in self._cache:
             atoms = self.all_atoms
             self._cache['hessian'] = [
                 np.array(c.calc_hessian(atoms)) for c in self
             ]
         indices = [np.array(c.indices) for c in self]
         hessians = []
-        for idx, vals, active in zip(indices, self._cache['hessian'], self._active_mask):
+        for idx, vals, active in zip(
+            indices, self._cache['hessian'], self._active_mask
+        ):
             if not active:
                 continue
             hessians.append(SparseInternalHessian(
                 self.natoms + self.ndummies, idx, vals.copy()
             ))
         return SparseInternalHessians(hessians, self.ndof)
 
@@ -659,21 +710,18 @@
             if name == 'dihedrals':
                 end = start + len(self.internals[name])
                 break
             start += len(self.internals[name])
         vec[start:end] = (vec[start:end] + np.pi) % (2 * np.pi) - np.pi
         return vec
 
-    def __iter__(self) -> Iterator[Internal]:
+    def __iter__(self) -> Iterator[Coordinate]:
         for name in self._names:
             for coord in self.internals[name]:
                 yield coord
-            #for coord, active in zip(self.internals[name], self._active[name]):
-            #    if active:
-            #        yield coord
 
     def _get_neighbors(self, dx: np.ndarray) -> Iterator[np.ndarray]:
         pbc = self.atoms.pbc
         if self.cell is None or not np.all(self.cell == self.atoms.cell):
             self.cell = self.atoms.cell.array.copy()
             rcell, self.op = minkowski_reduce(
                 complete_cell(self.cell), pbc=pbc
@@ -761,14 +809,30 @@
                 new_indices = (*rot.indices[:-1], didx)
                 new_rot = Rotation(
                     new_indices, rot.axis,
                     self.all_atoms[new_indices].positions
                 )
                 self.internals['rotations'][i] = new_rot
 
+    def check_all_gradients(
+        self, delta: float = 1e-4, atol: float = 1e-6
+    ) -> bool:
+        success = True
+        for coord in self:
+            success &= coord.check_gradient(self.all_atoms, delta, atol)
+        return success
+
+    def check_all_hessians(
+        self, delta: float = 1e-4, atol: float = 1e-6,
+    ) -> bool:
+        success = True
+        for coord in self:
+            success &= coord.check_hessian(self.all_atoms, delta, atol)
+        return success
+
 
 class Constraints(BaseInternals):
     def __init__(
         self,
         atoms: Atoms,
         dummies: Atoms = None,
         dinds: np.ndarray = None,
@@ -914,18 +978,18 @@
             raise DuplicateConstraintError(
                 "Coordinate {} is already fixed to target {}"
                 .format(new, self._targets['translations'][idx])
             )
 
     def _fix_internal(
         self,
-        kind: TypeVar('Internal', bound=Internal),
+        kind: TypeVar('Coordinate', bound=Coordinate),
         name: str,
         conv: float,
-        indices: Union[Tuple[int, ...], Internal],
+        indices: Union[Tuple[int, ...], Coordinate],
         ncvecs: Tuple[IVec, ...] = None,
         mic: bool = None,
         target: float = None,
         comparator: str = 'eq',
         replace_ok: bool = True,
     ) -> None:
         if isinstance(indices, kind):
@@ -963,15 +1027,15 @@
     fix_angle = partialmethod(_fix_internal, Angle, 'angles', np.pi / 180.)
     fix_dihedral = partialmethod(
         _fix_internal, Dihedral, 'dihedrals', np.pi / 180.
     )
 
     def fix_other(
         self,
-        coord: Internal,
+        coord: Coordinate,
         target: float = None,
         comparator: str = 'eq',
         replace_ok: bool = True,
     ) -> None:
         if target is None:
             target = coord.calc(self.all_atoms)
         try:
@@ -1068,15 +1132,15 @@
                 )
             self.dummies = cons.dummies
             self.dinds = cons.dinds
         self.cons = cons
 
         for kind, adder in zip(self._names, (
             self.add_translation, self.add_bond, self.add_angle,
-            self.add_dihedral, self.add_rotation
+            self.add_dihedral, self.add_other, self.add_rotation
         )):
             for coord in self.cons.internals[kind]:
                 adder(coord)
         self.allow_fragments = allow_fragments
 
     def copy(self) -> 'Internals':
         new = self.__class__(
@@ -1152,17 +1216,17 @@
         ):
             raise DuplicateInternalError
         self.internals['translations'].append(new)
         self._active['translations'].append(True)
 
     def _add_internal(
         self,
-        kind: TypeVar('Internal', bound=Internal),
+        kind: TypeVar('Coordinate', bound=Coordinate),
         name: str,
-        indices: Union[Tuple[int, ...], Internal],
+        indices: Union[Tuple[int, ...], Coordinate],
         ncvecs: Tuple[IVec, ...] = None,
         mic: bool = None,
     ) -> None:
         if isinstance(indices, kind):
             if ncvecs is not None or mic is not None:
                 raise ValueError(
                     '"ncvecs" and "mic" keywords cannot be used '
@@ -1180,14 +1244,25 @@
         self.internals[name].append(new)
         self._active[name].append(True)
 
     add_bond = partialmethod(_add_internal, Bond, 'bonds')
     add_angle = partialmethod(_add_internal, Angle, 'angles')
     add_dihedral = partialmethod(_add_internal, Dihedral, 'dihedrals')
 
+    def add_other(
+        self,
+        coord: Coordinate,
+    ) -> None:
+        try:
+            idx = self.internals['other'].index(coord)
+        except ValueError:
+            self.internals['other'].append(coord)
+        else:
+            raise DuplicateCoordinateError()
+
     def forbid_translation(
         self,
         index: Union[int, Tuple[int, ...], Translation] = None,
         dim: int = None
     ) -> None:
         if isinstance(index, Translation):
             if dim is not None:
@@ -1210,17 +1285,17 @@
         except ValueError:
             pass
         if new not in self.forbidden['translations']:
             self.forbidden['translations'].append(new)
 
     def _forbid_internal(
         self,
-        kind: TypeVar('Internal', bound=Internal),
+        kind: TypeVar('Coordinate', bound=Coordinate),
         name: str,
-        indices: Union[Tuple[int, ...], Internal],
+        indices: Union[Tuple[int, ...], Coordinate],
         ncvecs: Tuple[IVec, ...] = None,
         mic: bool = None,
     ) -> None:
         if isinstance(indices, kind):
             if ncvecs is not None or mic is not None:
                 raise ValueError(
                     '"ncvecs" and "mic" keywords cannot be used '
@@ -1354,15 +1429,14 @@
                     try:
                         self.add_angle(new)
                     except DuplicateInternalError:
                         pass
                 else:
                     self.forbid_angle(new)
                     linear.append((b1, b2))
-            #if linear and self.dinds[j] < 0:
             if linear:
                 if len(jbonds) == 2:
                     # Add a dummy atom to an atom center with only 2 bonds
                     # sort bonds from shortest to longest to ensure
                     # permutational invariance
                     b1, b2 = sorted(jbonds, key=lambda x: x.calc(self.atoms))
                     # First try to take the cross product of the two bond
@@ -1376,16 +1450,16 @@
                         dx2 = b2.calc_vec(self.atoms)
                         dx2 /= np.linalg.norm(dx2)
                         dpos = np.cross(dx1, dx2)
                         dpos_norm = np.linalg.norm(dpos)
                         if dpos_norm < 1e-4:
                             # the aforementioned backup strategy
                             # pick the cartesian basis vector that is maximally
-                            # orthogonal with the shorter of the two displacement
-                            # vectors.
+                            # orthogonal with the shorter of the two
+                            # displacement vectors.
                             # note: this is not rotationally invariant, but
                             # there's not much we can do about that
                             dim = np.argmin(np.abs(dx1))
                             dpos[:] = 0.
                             dpos[dim] = 1.
                             dpos -= dx1 * (dpos @ dx1)
                             dpos /= np.linalg.norm(dpos)
@@ -1402,15 +1476,17 @@
                     dangle1 = b1 + dbond
                     self.cons.fix_angle(dangle1, replace_ok=False)
                     dangle2 = b2 + dbond
                     self.cons.fix_angle(dangle2, replace_ok=False)
                     # Fix the improper dihedral and update relevant internals
                     if b2.indices[1] == j:
                         b2 = b2.reverse()
-                    dbond2 = Bond((self.dinds[j], b2.indices[1]), b2.ncvecs)
+                    dbond2 = Bond(
+                        (self.dinds[j], b2.indices[1]), b2.kwargs['ncvecs']
+                    )
                     dangle3 = dbond + dbond2
                     ddihedral = dangle1 + dangle3
                     self.add_dihedral(ddihedral)
                     self.add_dummy_to_internals(j)
                     self.cons.add_dummy_to_internals(j)
                     # Add relevant angles
                     for b1 in jbonds:
@@ -1429,17 +1505,17 @@
                         for b3 in jbonds:
                             if b3 in (b1, b2):
                                 continue
                             indices = (
                                 b1.indices[1], j, b3.indices[1], b2.indices[1]
                             )
                             ncvecs = (
-                                -b1.ncvecs[0],
-                                b3.ncvecs[0],
-                                b2.ncvecs[0] - b3.ncvecs[0]
+                                -b1.kwargs['ncvecs'][0],
+                                b3.kwargs['ncvecs'][0],
+                                b2.kwargs['ncvecs'][0] - b3.kwargs['ncvecs'][0]
                             )
                             try:
                                 self.add_dihedral(indices, ncvecs)
                             except DuplicateInternalError:
                                 pass
                             break
                         else:
@@ -1454,15 +1530,15 @@
                 new = a1 + a2
             except NoValidInternalError:
                 continue
             # this is a dihedral that has the same exact atom as both
             # the first and last atom.
             if (
                 new.indices[0] == new.indices[3]
-                and np.all(np.sum(new.ncvecs, axis=0) == np.array((0, 0, 0)))
+                and np.all(np.sum(new.kwargs['ncvecs'], axis=0) == np.array((0, 0, 0)))
             ):
                 continue
             try:
                 self.add_dihedral(new)
             except DuplicateInternalError:
                 continue
 
@@ -1472,15 +1548,15 @@
         ndeloc = np.sum(S > 1e-8)
         ndof = 3 * (self.natoms + self.ndummies) - 6
         if ndeloc != ndof:
             warnings.warn(
                 f'{ndeloc} coords found! Expected {ndof}.'
             )
 
-    def check_for_bad_internals(self) -> Optional[Dict[str, List[Internal]]]:
+    def check_for_bad_internals(self) -> Optional[Dict[str, List[Coordinate]]]:
         bad = {'bonds': [], 'angles': []}
         for a in self.internals['angles']:
             if not (self.atol < a.calc(self.all_atoms) < np.pi - self.atol):
                 bad['angles'].append(a)
 
         for ints in bad.values():
             if ints:
```

### Comparing `Sella-2.2.1/sella/linalg.py` & `Sella-2.3.0/sella/linalg.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,17 +155,20 @@
         self.set_B(B0)
 
     def set_B(self, target):
         if target is None:
             self.B = None
             self.evals = None
             self.evecs = None
+            self.initialized = False
             return
         elif np.isscalar(target):
             target = target * np.eye(self.dim)
+        else:
+            self.initialized = True
         assert target.shape == self.shape
         self.B = target
         self.evals, self.evecs = eigh(self.B)
 
     def update(self, dx, dg):
         """Perform a quasi-Newton update on B"""
         if self.B is None:
```

### Comparing `Sella-2.2.1/sella/optimize/irc.py` & `Sella-2.3.0/sella/optimize/irc.py`

 * *Files identical despite different names*

### Comparing `Sella-2.2.1/sella/optimize/optimize.py` & `Sella-2.3.0/sella/optimize/optimize.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 import warnings
 from time import localtime, strftime
-from typing import Union
+from typing import Union, Callable, Optional
 
 import numpy as np
 from ase import Atoms
 from ase.optimize.optimize import Optimizer
 from ase.utils import basestring
 from ase.io.trajectory import Trajectory
 
@@ -59,14 +59,16 @@
         constraints: Constraints = None,
         constraints_tol: float = 1e-5,
         v0: np.ndarray = None,
         internal: Union[bool, Internals] = False,
         append_trajectory: bool = False,
         rs: str = None,
         nsteps_per_diag: int = 3,
+        diag_every_n: Optional[int] = None,
+        hessian_function: Optional[Callable[[Atoms], np.ndarray]] = None,
         **kwargs
     ):
         if order == 0:
             default = _default_kwargs['minimum']
         else:
             default = _default_kwargs['saddle']
 
@@ -76,15 +78,23 @@
                 trajectory = Trajectory(trajectory, mode=mode,
                                         atoms=atoms, master=master)
 
         asetraj = None
         self.peskwargs = kwargs.copy()
         self.user_internal = internal
         self.initialize_pes(
-            atoms, trajectory, order, eta, constraints, v0, internal, **kwargs
+            atoms,
+            trajectory,
+            order,
+            eta,
+            constraints,
+            v0,
+            internal,
+            hessian_function,
+            **kwargs
         )
 
         if rs is None:
             rs = 'mis' if internal else 'ras'
         self.rs = get_restricted_step(rs)
         Optimizer.__init__(self, atoms, restart, logfile, asetraj, master,
                            force_consistent)
@@ -138,24 +148,26 @@
                           "most likely fail!\n Proceeding anyway, but you "
                           "shouldn't be optimistic.")
 
         self.initialized = False
         self.xi = 1.
         self.nsteps_per_diag = nsteps_per_diag
         self.nsteps_since_diag = 0
+        self.diag_every_n = np.infty if diag_every_n is None else diag_every_n
 
     def initialize_pes(
         self,
         atoms: Atoms,
         trajectory: str = None,
         order: int = 1,
         eta: float = 1e-4,
         constraints: Constraints = None,
         v0: np.ndarray = None,
         internal: Union[bool, Internals] = False,
+        hessian_function: Optional[Callable[[Atoms], np.ndarray]] = None,
         **kwargs
     ):
         if internal:
             if isinstance(internal, Internals):
                 auto_find_internals = False
                 if constraints is not None:
                     raise ValueError(
@@ -172,35 +184,41 @@
             self.pes = InternalPES(
                 atoms,
                 internals=internal,
                 trajectory=trajectory,
                 eta=eta,
                 v0=v0,
                 auto_find_internals=auto_find_internals,
+                hessian_function=hessian_function,
                 **kwargs
             )
         else:
             self.internal = None
             if constraints is None:
                 constraints = Constraints(atoms)
             self.constraints = constraints
             self.pes = PES(
                 atoms,
                 constraints=constraints,
                 trajectory=trajectory,
                 eta=eta,
                 v0=v0,
+                hessian_function=hessian_function,
                 **kwargs
             )
 
     def _predict_step(self):
         if not self.initialized:
             self.pes.get_g()
             if self.eig:
-                self.pes.diag(**self.diagkwargs)
+                if self.pes.hessian_function is not None:
+                    self.pes.calculate_hessian()
+                else:
+                    self.pes.diag(**self.diagkwargs)
+                self.nsteps_since_diag = -1
             self.initialized = True
 
         self.pes.cons.disable_satisfied_inequalities()
         self.pes._update_basis()
         self.pes.save()
         all_valid = False
         x0 = self.pes.get_x()
@@ -215,40 +233,45 @@
         self.pes._update_basis()
         return s, smag
 
     def step(self):
         s, smag = self._predict_step()
 
         # Determine if we need to call the eigensolver, then step
-        if self.eig and self.nsteps_since_diag >= self.nsteps_per_diag:
+        if self.nsteps_since_diag >= self.diag_every_n:
+            ev = True
+        elif self.eig and self.nsteps_since_diag >= self.nsteps_per_diag:
             if self.pes.H.evals is None:
                 ev = True
             else:
                 Unred = self.pes.get_Unred()
                 ev = (self.pes.get_HL().project(Unred)
                                        .evals[:self.ord] > 0).any()
         else:
             ev = False
+
         if ev:
             self.nsteps_since_diag = 0
         else:
             self.nsteps_since_diag += 1
+
         rho = self.pes.kick(s, ev, **self.diagkwargs)
 
         # Check for bad internals, and if found, reset PES object.
         # This skips the trust radius update.
         if self.internal and self.pes.int.check_for_bad_internals():
             self.initialize_pes(
                 atoms=self.pes.atoms,
                 trajectory=self.pes.traj,
                 order=self.ord,
                 eta=self.pes.eta,
                 constraints=self.constraints,
                 v0=None,  # TODO: use leftmost eigenvector from old H
                 internal=self.user_internal,
+                hessian_function=self.pes.hessian_function,
             )
             self.initialized = False
             self.rho = 1
             return
 
         # Update trust radius
         if rho is None:
```

### Comparing `Sella-2.2.1/sella/optimize/restricted_step.py` & `Sella-2.3.0/sella/optimize/restricted_step.py`

 * *Files identical despite different names*

### Comparing `Sella-2.2.1/sella/optimize/stepper.py` & `Sella-2.3.0/sella/optimize/stepper.py`

 * *Files identical despite different names*

### Comparing `Sella-2.2.1/sella/peswrapper.py` & `Sella-2.3.0/sella/peswrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union
+from typing import Union, Callable
 
 import numpy as np
 from scipy.linalg import eigh
 from scipy.integrate import LSODA
 from ase import Atoms
 from ase.utils import basestring
 from ase.visualize import view
@@ -23,15 +23,16 @@
         H0: np.ndarray = None,
         constraints: Constraints = None,
         eigensolver: str = 'jd0',
         trajectory: Union[str, Trajectory] = None,
         eta: float = 1e-4,
         v0: np.ndarray = None,
         proj_trans: bool = None,
-        proj_rot: bool = None
+        proj_rot: bool = None,
+        hessian_function: Callable[[Atoms], np.ndarray] = None,
     ) -> None:
         self.atoms = atoms
         if constraints is None:
             constraints = Constraints(self.atoms)
         if proj_trans is None:
             if constraints.internals['translations']:
                 proj_trans = False
@@ -85,14 +86,16 @@
             self.set_H(None, initialized=False)
         else:
             self.set_H(H0, initialized=True)
 
         self.savepoint = dict(apos=None, dpos=None)
         self.first_diag = True
 
+        self.hessian_function = hessian_function
+
     apos = property(lambda self: self.atoms.positions.copy())
     dpos = property(lambda self: None)
 
     def save(self):
         self.savepoint = dict(apos=self.apos, dpos=self.dpos)
 
     def restore(self):
@@ -323,18 +326,25 @@
             ratio = None
         else:
             ratio = df_actual / df_pred
 
         self._update_H(dx_final, dg_actual)
 
         if diag:
-            self.diag(**diag_kwargs)
+            if self.hessian_function is not None:
+                self.calculate_hessian()
+            else:
+                self.diag(**diag_kwargs)
 
         return ratio
 
+    def calculate_hessian(self):
+        assert self.hessian_function is not None
+        self.H.set_B(self.hessian_function(self.atoms))
+
 
 class InternalPES(PES):
     def __init__(
         self,
         atoms: Atoms,
         internals: Internals,
         *args,
@@ -622,7 +632,50 @@
         if not PES._update(self, feval=feval):
             return
 
         B = self.int.jacobian()
         Binv = np.linalg.pinv(B)
         self.curr.update(B=B, Binv=Binv)
         return True
+
+    def _convert_cartesian_hessian_to_internal(
+        self,
+        Hcart: np.ndarray,
+    ) -> np.ndarray:
+        ncart = 3 * len(self.atoms)
+        # Get Jacobian and calculate redundant and non-redundant spaces
+        B = self.int.jacobian()[:, :ncart]
+        Ui, Si, VTi = np.linalg.svd(B)
+        nnred = np.sum(Si > 1e-6)
+        Unred = Ui[:, :nnred]
+        Ured = Ui[:, nnred:]
+
+        # Calculate inverse Jacobian in non-redundant space
+        Bnred_inv = VTi[:nnred].T @ np.diag(1 / Si[:nnred])
+
+        # Convert Cartesian Hessian to non-redundant internal Hessian
+        Hcart_coupled = self.int.hessian().ldot(self.get_g())[:ncart, :ncart]
+        Hcart_corr = Hcart - Hcart_coupled
+        Hnred = Bnred_inv.T @ Hcart_corr @ Bnred_inv
+
+        # Find eigenvalues of non-redundant internal Hessian
+        lnred, _ = np.linalg.eigh(Hnred)
+
+        # The redundant part of the Hessian will be initialized to the
+        # geometric mean of the non-redundant eigenvalues
+        lnred_mean = np.exp(np.log(np.abs(lnred)).mean())
+
+        # finish reconstructing redundant internal Hessian
+        return Unred @ Hnred @ Unred.T + lnred_mean * Ured @ Ured.T
+
+    def _convert_internal_hessian_to_cartesian(
+        self,
+        Hint: np.ndarray,
+    ) -> np.ndarray:
+        B = self.int.jacobian()
+        return B.T @ Hint @ B + self.int.hessian().ldot(self.get_g())
+
+    def calculate_hessian(self):
+        assert self.hessian_function is not None
+        self.H.set_B(self._convert_cartesian_hessian_to_internal(
+            self.hessian_function(self.atoms)
+        ))
```

### Comparing `Sella-2.2.1/sella/samd.py` & `Sella-2.3.0/sella/samd.py`

 * *Files identical despite different names*

### Comparing `Sella-2.2.1/sella/utilities/blas.pyx` & `Sella-2.3.0/sella/utilities/blas.pyx`

 * *Files identical despite different names*

### Comparing `Sella-2.2.1/sella/utilities/math.pyx` & `Sella-2.3.0/sella/utilities/math.pyx`

 * *Files identical despite different names*

### Comparing `Sella-2.2.1/setup.py` & `Sella-2.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 import os
 
 import numpy as np
 
 from setuptools import setup, Extension, find_packages
 
-VERSION = '2.2.1'
+VERSION = '2.3.0'
 
 debug = '--debug' in sys.argv or '-g' in sys.argv
 
 try:
     from Cython.Build import cythonize
 except ImportError:
     use_cython = False
```

