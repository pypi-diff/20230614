# Comparing `tmp/bayesianbandits-0.4.1.tar.gz` & `tmp/bayesianbandits-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayesianbandits-0.4.1.tar", max compression
+gzip compressed data, was "bayesianbandits-0.4.2.tar", max compression
```

## Comparing `bayesianbandits-0.4.1.tar` & `bayesianbandits-0.4.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1074 2023-06-09 17:22:40.840365 bayesianbandits-0.4.1/LICENSE
--rw-r--r--   0        0        0     1093 2023-06-09 17:22:40.840365 bayesianbandits-0.4.1/README.md
--rw-r--r--   0        0        0     2740 2023-06-09 17:22:40.844365 bayesianbandits-0.4.1/bayesianbandits/__init__.py
--rw-r--r--   0        0        0     3538 2023-06-09 17:22:40.844365 bayesianbandits-0.4.1/bayesianbandits/_arm.py
--rw-r--r--   0        0        0    20408 2023-06-09 17:22:40.844365 bayesianbandits-0.4.1/bayesianbandits/_basebandit.py
--rw-r--r--   0        0        0    29470 2023-06-09 17:22:40.844365 bayesianbandits-0.4.1/bayesianbandits/_estimators.py
--rw-r--r--   0        0        0     1304 2023-06-09 17:22:40.844365 bayesianbandits-0.4.1/bayesianbandits/_np_utils.py
--rw-r--r--   0        0        0     5036 2023-06-09 17:22:40.844365 bayesianbandits-0.4.1/bayesianbandits/_policy_decorators.py
--rw-r--r--   0        0        0     2634 2023-06-09 17:22:40.844365 bayesianbandits-0.4.1/bayesianbandits/_typing.py
--rw-r--r--   0        0        0      705 2023-06-09 17:22:40.852366 bayesianbandits-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1627 1970-01-01 00:00:00.000000 bayesianbandits-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-14 01:38:50.705377 bayesianbandits-0.4.2/LICENSE
+-rw-r--r--   0        0        0     1093 2023-06-14 01:38:50.705377 bayesianbandits-0.4.2/README.md
+-rw-r--r--   0        0        0     2740 2023-06-14 01:38:50.705377 bayesianbandits-0.4.2/bayesianbandits/__init__.py
+-rw-r--r--   0        0        0     3538 2023-06-14 01:38:50.705377 bayesianbandits-0.4.2/bayesianbandits/_arm.py
+-rw-r--r--   0        0        0    20408 2023-06-14 01:38:50.705377 bayesianbandits-0.4.2/bayesianbandits/_basebandit.py
+-rw-r--r--   0        0        0    29847 2023-06-14 01:38:50.705377 bayesianbandits-0.4.2/bayesianbandits/_estimators.py
+-rw-r--r--   0        0        0     1304 2023-06-14 01:38:50.705377 bayesianbandits-0.4.2/bayesianbandits/_np_utils.py
+-rw-r--r--   0        0        0     5036 2023-06-14 01:38:50.705377 bayesianbandits-0.4.2/bayesianbandits/_policy_decorators.py
+-rw-r--r--   0        0        0     2634 2023-06-14 01:38:50.705377 bayesianbandits-0.4.2/bayesianbandits/_typing.py
+-rw-r--r--   0        0        0      705 2023-06-14 01:38:50.709377 bayesianbandits-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1627 1970-01-01 00:00:00.000000 bayesianbandits-0.4.2/PKG-INFO
```

### Comparing `bayesianbandits-0.4.1/LICENSE` & `bayesianbandits-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.4.1/README.md` & `bayesianbandits-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.4.1/bayesianbandits/__init__.py` & `bayesianbandits-0.4.2/bayesianbandits/__init__.py`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.4.1/bayesianbandits/_arm.py` & `bayesianbandits-0.4.2/bayesianbandits/_arm.py`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.4.1/bayesianbandits/_basebandit.py` & `bayesianbandits-0.4.2/bayesianbandits/_basebandit.py`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.4.1/bayesianbandits/_estimators.py` & `bayesianbandits-0.4.2/bayesianbandits/_estimators.py`

 * *Files 2% similar despite different names*

```diff
@@ -506,30 +506,30 @@
         random_state: Union[int, np.random.Generator, None] = None,
     ) -> None:
         self.alpha = alpha
         self.beta = beta
         self.learning_rate = learning_rate
         self.random_state = random_state
 
-    def fit(self, X: NDArray[Any], y: NDArray[Any]) -> Self:
+    def fit(self, X_fit: NDArray[Any], y: NDArray[Any]) -> Self:
         """
         Fit the model using X as training data and y as target values. y must be
         count data.
         """
-        X, y = check_X_y(
-            X,
+        X_fit, y = check_X_y(
+            X_fit,
             y,
             copy=True,
             ensure_2d=True,
             dtype=np.float_,
         )
 
-        self._initialize_prior(X)
+        self._initialize_prior(X_fit)
 
-        self._fit_helper(X, y)
+        self._fit_helper(X_fit, y)
 
         return self
 
     def _initialize_prior(self, X: NDArray[Any]) -> None:
         if isinstance(self.random_state, int) or self.random_state is None:
             self.random_state_ = np.random.default_rng(self.random_state)
         else:
@@ -642,14 +642,17 @@
 
         # Decay the prior without making an update. Because we're only
         # increasing the prior variance, we do not need to update the
         # mean.
         cov_inv = prior_decay * self.cov_inv_
 
         self.cov_inv_ = cov_inv
+        # Delete the cached covariance matrix, since it is no longer valid
+        if hasattr(self, "cov_"):
+            del self.cov_
 
 
 class NormalInverseGammaRegressor(NormalRegressor):
     """
     Bayesian linear regression with unknown variance.
 
     Default prior values correspond to ridge regression with alpha = 1.
@@ -740,17 +743,17 @@
     """
 
     def __init__(
         self,
         *,
         mu: ArrayLike = 0.0,
         lam: ArrayLike = 1.0,
-        a=0.1,
-        b=0.1,
-        learning_rate=1.0,
+        a: float = 0.1,
+        b: float = 0.1,
+        learning_rate: float = 1.0,
         random_state: Union[int, np.random.Generator, None] = None,
     ):
         self.mu = mu
         self.lam = lam
         self.a = a
         self.b = b
         self.learning_rate = learning_rate
@@ -761,15 +764,15 @@
             self.random_state_ = np.random.default_rng(self.random_state)
         else:
             self.random_state_ = self.random_state
 
         self.n_features_ = X.shape[1]
         if np.isscalar(self.mu):
             self.coef_ = np.full(self.n_features_, self.mu, dtype=np.float_)
-        elif cast(NDArray, self.mu).ndim == 1:
+        elif cast(NDArray[np.float_], self.mu).ndim == 1:
             self.coef_ = cast(NDArray[np.float_], self.mu)
         else:
             raise ValueError("The prior mean must be a scalar or vector.")
 
         if np.isscalar(self.lam):
             self.cov_inv_ = cast(np.float_, self.lam) * np.eye(self.n_features_)
         elif cast(NDArray[np.float_], self.lam).ndim == 1:
@@ -822,14 +825,16 @@
         )
 
         # Posteriors become priors for the next batch
         self.cov_inv_ = V_n
         # Delete the cached shape_ property so it is recalculated
         if hasattr(self, "shape_"):
             del self.shape_
+        if hasattr(self, "cov_"):
+            del self.cov_
         self.coef_ = m_n
         self.a_ = a_n
         self.b_ = b_n
 
     @cached_property
     def shape_(self) -> Covariance:
         extra_var = self.b_ / self.a_ * np.eye(self.n_features_)
@@ -895,9 +900,13 @@
         V_n = prior_decay * self.cov_inv_
 
         a_n = prior_decay * self.a_
 
         b_n = prior_decay * self.b_
 
         self.cov_inv_ = V_n
+        if hasattr(self, "shape_"):
+            del self.shape_
+        if hasattr(self, "cov_"):
+            del self.cov_
         self.a_ = a_n
         self.b_ = b_n
```

### Comparing `bayesianbandits-0.4.1/bayesianbandits/_np_utils.py` & `bayesianbandits-0.4.2/bayesianbandits/_np_utils.py`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.4.1/bayesianbandits/_policy_decorators.py` & `bayesianbandits-0.4.2/bayesianbandits/_policy_decorators.py`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.4.1/bayesianbandits/_typing.py` & `bayesianbandits-0.4.2/bayesianbandits/_typing.py`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.4.1/pyproject.toml` & `bayesianbandits-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "bayesianbandits"
-version = "0.4.1"
+version = "0.4.2"
 description = ""
 authors = ["Rishi Kulkarni <rishi@kulkarni.science>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9, <3.12"
 scipy = "^1.10.0"
 scikit-learn = "^1.2.1"
-typing-extensions = "^4.5.0"
+typing-extensions = "^4.6.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 black = "^23.1.0"
 flake8 = "^6.0.0"
 ipython = "^8.10.0"
```

### Comparing `bayesianbandits-0.4.1/PKG-INFO` & `bayesianbandits-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: bayesianbandits
-Version: 0.4.1
+Version: 0.4.2
 Summary: 
 Author: Rishi Kulkarni
 Author-email: rishi@kulkarni.science
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: scikit-learn (>=1.2.1,<2.0.0)
 Requires-Dist: scipy (>=1.10.0,<2.0.0)
-Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
+Requires-Dist: typing-extensions (>=4.6.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # `bayesianbandits`
 
 bayesianbandits is a Pythonic framework for building agents to maximize rewards in multi-armed bandit (MAB) problems. These agents can handle a number of MAB subproblems, such as contextual, restless, and delayed reward bandits.
 
 Building an agent is as simple as defining arms and using the necessary decorators. For example, to create an agent for a Bernoulli bandit:
```

