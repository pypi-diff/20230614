# Comparing `tmp/scikeras-0.8.0.tar.gz` & `tmp/scikeras-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikeras-0.8.0.tar", max compression
+gzip compressed data, was "scikeras-0.9.0.tar", max compression
```

## Comparing `scikeras-0.8.0.tar` & `scikeras-0.9.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1082 2022-05-11 20:16:16.223238 scikeras-0.8.0/LICENSE
--rw-r--r--   0        0        0     2217 2022-05-11 20:16:16.223238 scikeras-0.8.0/README.md
--rw-r--r--   0        0        0     2354 2022-05-11 20:16:16.227238 scikeras-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1115 2022-05-11 20:16:16.227238 scikeras-0.8.0/scikeras/__init__.py
--rw-r--r--   0        0        0     5997 2022-05-11 20:16:16.227238 scikeras-0.8.0/scikeras/_saving_utils.py
--rw-r--r--   0        0        0     6742 2022-05-11 20:16:16.227238 scikeras-0.8.0/scikeras/_utils.py
--rw-r--r--   0        0        0     3542 2022-05-11 20:16:16.227238 scikeras-0.8.0/scikeras/utils/__init__.py
--rw-r--r--   0        0        0     1303 2022-05-11 20:16:16.227238 scikeras-0.8.0/scikeras/utils/random_state.py
--rw-r--r--   0        0        0    14531 2022-05-11 20:16:16.227238 scikeras-0.8.0/scikeras/utils/transformers.py
--rw-r--r--   0        0        0    69939 2022-05-11 20:16:16.227238 scikeras-0.8.0/scikeras/wrappers.py
--rw-r--r--   0        0        0     3197 2022-05-11 20:16:25.244182 scikeras-0.8.0/setup.py
--rw-r--r--   0        0        0     3750 2022-05-11 20:16:25.244772 scikeras-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2022-07-22 23:47:58.340415 scikeras-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2217 2022-07-22 23:47:58.340415 scikeras-0.9.0/README.md
+-rw-r--r--   0        0        0     2351 2022-07-22 23:47:58.344415 scikeras-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1115 2022-07-22 23:47:58.344415 scikeras-0.9.0/scikeras/__init__.py
+-rw-r--r--   0        0        0     5997 2022-07-22 23:47:58.344415 scikeras-0.9.0/scikeras/_saving_utils.py
+-rw-r--r--   0        0        0     6742 2022-07-22 23:47:58.344415 scikeras-0.9.0/scikeras/_utils.py
+-rw-r--r--   0        0        0     3542 2022-07-22 23:47:58.344415 scikeras-0.9.0/scikeras/utils/__init__.py
+-rw-r--r--   0        0        0     1303 2022-07-22 23:47:58.344415 scikeras-0.9.0/scikeras/utils/random_state.py
+-rw-r--r--   0        0        0    14531 2022-07-22 23:47:58.344415 scikeras-0.9.0/scikeras/utils/transformers.py
+-rw-r--r--   0        0        0    70626 2022-07-22 23:47:58.344415 scikeras-0.9.0/scikeras/wrappers.py
+-rw-r--r--   0        0        0     3191 2022-07-22 23:48:08.990532 scikeras-0.9.0/setup.py
+-rw-r--r--   0        0        0     3744 2022-07-22 23:48:08.991125 scikeras-0.9.0/PKG-INFO
```

### Comparing `scikeras-0.8.0/LICENSE` & `scikeras-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scikeras-0.8.0/README.md` & `scikeras-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `scikeras-0.8.0/pyproject.toml` & `scikeras-0.9.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -23,42 +23,42 @@
   "LICENSE",
 ]
 keywords = ["keras", "tensorflow", "scikit-learn", "deep-learning", "python"]
 license = "MIT"
 name = "scikeras"
 readme = "README.md"
 repository = "https://github.com/adriangb/scikeras"
-version = "0.8.0"
+version = "0.9.0"
 
 [tool.poetry.dependencies]
 importlib-metadata = {version = ">=3", python = "<3.8"}
 python = ">=3.7.0,<3.11.0"
 scikit-learn = ">=1.0.0"
-packaging = ">=0.21,<22.0"
+packaging = ">=0.21"
 tensorflow = {version = ">=2.7.0", optional = true}
 tensorflow-cpu = {version = ">=2.7.0", optional = true}
 
 [tool.poetry.extras]
 tensorflow = ["tensorflow"]
 tensorflow-cpu = ["tensorflow-cpu"]
 
 [tool.poetry.dev-dependencies]
 tensorflow = ">=2.7.0"
-coverage = {extras = ["toml"], version = ">=5.4"}
-insipid-sphinx-theme = ">=0.2.2"
-ipykernel = ">=5.4.2"
+coverage = {extras = ["toml"], version = ">=6.4.2"}
+insipid-sphinx-theme = ">=0.3.2"
+ipykernel = ">=6.15.1"
 jupyter = ">=1.0.0"
-jupytext = ">=1.9.1"
-matplotlib = ">=3.3.3"
-nbsphinx = ">=0.8.1"
-numpydoc = ">=1.1.0"
-pre-commit = ">=2.10.1"
-pytest = ">=6.2.2"
-pytest-cov = ">=2.11.1"
-sphinx = ">=3.2.1"
+jupytext = ">=1.14.0"
+matplotlib = ">=3.5.2"
+nbsphinx = ">=0.8.9"
+numpydoc = ">=1.4.0"
+pre-commit = ">=2.20.0"
+pytest = ">=7.1.2"
+pytest-cov = ">=3.0.0"
+sphinx = ">=5.0.2"
 
 [tool.isort]
 atomic = true
 filter_files = true
 include_trailing_comma = true
 known_first_party = "scikeras"
 known_third_party = [
```

### Comparing `scikeras-0.8.0/scikeras/__init__.py` & `scikeras-0.9.0/scikeras/__init__.py`

 * *Files identical despite different names*

### Comparing `scikeras-0.8.0/scikeras/_saving_utils.py` & `scikeras-0.9.0/scikeras/_saving_utils.py`

 * *Files identical despite different names*

### Comparing `scikeras-0.8.0/scikeras/_utils.py` & `scikeras-0.9.0/scikeras/_utils.py`

 * *Files identical despite different names*

### Comparing `scikeras-0.8.0/scikeras/utils/__init__.py` & `scikeras-0.9.0/scikeras/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scikeras-0.8.0/scikeras/utils/random_state.py` & `scikeras-0.9.0/scikeras/utils/random_state.py`

 * *Files identical despite different names*

### Comparing `scikeras-0.8.0/scikeras/utils/transformers.py` & `scikeras-0.9.0/scikeras/utils/transformers.py`

 * *Files identical despite different names*

### Comparing `scikeras-0.8.0/scikeras/wrappers.py` & `scikeras-0.9.0/scikeras/wrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """Wrapper for using the Scikit-Learn API with Keras models.
 """
+import functools
 import inspect
 import warnings
 
 from collections import defaultdict
 from typing import Any, Callable, Dict, Iterable, List, Mapping, Set, Tuple, Type, Union
 
 import numpy as np
 import tensorflow as tf
 
+from scipy.sparse import isspmatrix, lil_matrix
 from sklearn.base import BaseEstimator, ClassifierMixin, RegressorMixin
 from sklearn.exceptions import NotFittedError
 from sklearn.metrics import accuracy_score as sklearn_accuracy_score
 from sklearn.metrics import r2_score as sklearn_r2_score
 from sklearn.preprocessing import FunctionTransformer
 from sklearn.utils.class_weight import compute_sample_weight
 from sklearn.utils.multiclass import type_of_target
@@ -258,26 +260,35 @@
         if not hasattr(self, "history_"):
             return 0
         return len(self.history_["loss"])
 
     @staticmethod
     def _validate_sample_weight(
         X: np.ndarray,
+        y: np.ndarray,
         sample_weight: Union[np.ndarray, Iterable],
     ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
         """Validate that the passed sample_weight and ensure it is a Numpy array."""
         sample_weight = _check_sample_weight(
             sample_weight, X, dtype=np.dtype(tf.keras.backend.floatx())
         )
         if np.all(sample_weight == 0):
             raise ValueError(
                 "No training samples had any weight; only zeros were passed in sample_weight."
                 " That means there's nothing to train on by definition, so training can not be completed."
             )
-        return X, sample_weight
+        # drop any zero sample weights
+        # this helps mirror the behavior of sklearn estimators
+        # which tend to have higher precisions
+        not_dropped_samples = sample_weight != 0
+        return (
+            X[not_dropped_samples, ...],
+            y[not_dropped_samples, ...],
+            sample_weight[not_dropped_samples, ...],
+        )
 
     def _check_model_param(self):
         """Checks ``model`` and returns model building
         function to use.
 
         Raises
         ------
@@ -300,15 +311,15 @@
                 )
             final_build_fn = self._keras_build_fn
         elif isinstance(model, Model):
             # pre-built Keras Model
             def final_build_fn():
                 return model
 
-        elif inspect.isfunction(model):
+        elif inspect.isfunction(model) or isinstance(model, functools.partial):
             if hasattr(self, "_keras_build_fn"):
                 raise ValueError(
                     "This class cannot implement ``_keras_build_fn`` if"
                     " using the `model` parameter"
                 )
             # a callable method/function
             final_build_fn = model
@@ -565,19 +576,19 @@
     def _validate_data(
         self, X=None, y=None, reset: bool = False, y_numeric: bool = False
     ) -> Tuple[np.ndarray, Union[np.ndarray, None]]:
         """Validate input arrays and set or check their meta-parameters.
 
         Parameters
         ----------
-        X : Union[array-like, sparse matrix, dataframe] of shape \
+        X : Union[array-like, sparse matrix, dataframe, of shape \
            (n_samples, n_features)
             The input samples. If None, ``check_array`` is called on y and
             ``check_X_y`` is called otherwise.
-        y : Union[array-like, sparse matrix, dataframe] of shape \
+        y : Union[array-like, dataframe,, of shape \
             (n_samples,), default=None
             The targets. If None, ``check_array`` is called on X and
             ``check_X_y`` is called otherwise.
         reset : bool, default=False
             If True, override all meta attributes.
             If False, verify that they haven't changed.
         y_numeric : bool, default = False
@@ -603,14 +614,15 @@
                 # instead of float64 (sklearn's default)
                 return tf.keras.backend.floatx()
 
         if X is not None and y is not None:
             X, y = check_X_y(
                 X,
                 y,
+                accept_sparse=True,
                 allow_nd=True,  # allow X to have more than 2 dimensions
                 multi_output=True,  # allow y to be 2D
                 dtype=None,
             )
 
         if y is not None:
             y = check_array(
@@ -634,16 +646,24 @@
                     )
                 if self.y_ndim_ != y_ndim_:
                     raise ValueError(
                         f"y has {y_ndim_} dimensions, but this {self.__name__}"
                         f" is expecting {self.y_ndim_} dimensions in y."
                     )
         if X is not None:
+            if isspmatrix(X):
+                # TensorFlow does not support several of SciPy's sparse formats
+                # use SciPy to reformat here so at least the cost is known
+                X = lil_matrix(X)  # no-copy reformat
+
             X = check_array(
-                X, allow_nd=True, dtype=_check_array_dtype(X, force_numeric=True)
+                X,
+                allow_nd=True,
+                dtype=_check_array_dtype(X, force_numeric=True),
+                accept_sparse=True,
             )
             X_dtype_ = X.dtype
             X_shape_ = X.shape
             n_features_in_ = X.shape[1]
             if reset:
                 self.X_dtype_ = X_dtype_
                 self.X_shape_ = X_shape_
@@ -705,18 +725,18 @@
         return FunctionTransformer()
 
     def fit(self, X, y, sample_weight=None, **kwargs) -> "BaseWrapper":
         """Constructs a new model with ``model`` & fit the model to ``(X, y)``.
 
         Parameters
         ----------
-        X : Union[array-like, sparse matrix, dataframe] of shape (n_samples, n_features)
+        X : Union[array-like, sparse matrix, dataframe, of shape (n_samples, n_features)
             Training samples, where n_samples is the number of samples
             and n_features is the number of features.
-        y : Union[array-like, sparse matrix, dataframe] of shape (n_samples,) or (n_samples, n_outputs)
+        y : Union[array-like, dataframe of shape (n_samples,) or (n_samples, n_outputs)
             True labels for X.
         sample_weight : array-like of shape (n_samples,), default=None
             Array of weights that are assigned to individual samples.
             If not provided, then each sample is given unit weight.
         **kwargs : Dict[str, Any]
             Extra arguments to route to ``Model.fit``.
 
@@ -842,18 +862,18 @@
 
         You only need to call this model if you explicitly do not want to do any fitting
         (for example with a pretrained model). You should _not_ call this
         right before calling ``fit``, calling ``fit`` will do this automatically.
 
         Parameters
         ----------
-        X : Union[array-like, sparse matrix, dataframe] of shape (n_samples, n_features)
+        X : Union[array-like, sparse matrix, dataframe, of shape (n_samples, n_features)
                 Training samples where n_samples is the number of samples
                 and `n_features` is the number of features.
-        y : Union[array-like, sparse matrix, dataframe] of shape \
+        y : Union[array-like, dataframe,, of shape \
             (n_samples,) or (n_samples, n_outputs), default None
             True labels for X.
 
         Returns
         -------
         BaseWrapper
             A reference to the BaseWrapper instance for chained calling.
@@ -871,18 +891,18 @@
         initial_epoch: int,
         **kwargs,
     ) -> None:
         """Constructs a new model with ``model`` & fit the model to ``(X, y)``.
 
         Parameters
         ----------
-        X : Union[array-like, sparse matrix, dataframe] of shape (n_samples, n_features)
+        X : Union[array-like, sparse matrix, dataframe, of shape (n_samples, n_features)
                 Training samples where `n_samples` is the number of samples
                 and `n_features` is the number of features.
-        y :Union[array-like, sparse matrix, dataframe] of shape (n_samples,) or (n_samples, n_outputs)
+        y :Union[array-like, dataframe,, of shape (n_samples,) or (n_samples, n_outputs)
             True labels for X.
         sample_weight : array-like of shape (n_samples,), default=None
             Array of weights that are assigned to individual samples.
             If not provided, then each sample is given unit weight.
         warm_start : bool
             If True, don't rebuild the model.
         epochs : int
@@ -897,15 +917,15 @@
         if not ((self.warm_start or warm_start) and self.initialized_):
             X, y = self._initialize(X, y)
         else:
             X, y = self._validate_data(X, y)
         self._ensure_compiled_model()
 
         if sample_weight is not None:
-            X, sample_weight = self._validate_sample_weight(X, sample_weight)
+            X, y, sample_weight = self._validate_sample_weight(X, y, sample_weight)
 
         y = self.target_encoder_.transform(y)
         X = self.feature_encoder_.transform(X)
 
         self._check_model_compatibility(y)
 
         self._fit_keras_model(
@@ -920,18 +940,18 @@
 
     def partial_fit(self, X, y, sample_weight=None, **kwargs) -> "BaseWrapper":
         """Fit the estimator for a single epoch, preserving the current
         training history and model parameters.
 
         Parameters
         ----------
-        X : Union[array-like, sparse matrix, dataframe] of shape (n_samples, n_features)
+        X : Union[array-like, sparse matrix, dataframe, of shape (n_samples, n_features)
             Training samples where n_samples is the number of samples
             and n_features is the number of features.
-        y : Union[array-like, sparse matrix, dataframe] of shape \
+        y : Union[array-like, dataframe,, of shape \
             (n_samples,) or (n_samples, n_outputs)
             True labels for X.
         sample_weight : array-like of shape (n_samples,), default=None
             Array of weights that are assigned to individual samples.
             If not provided, then each sample is given unit weight.
         **kwargs : Dict[str, Any]
             Extra arguments to route to ``Model.fit``.
@@ -1004,15 +1024,15 @@
         return y_pred
 
     def predict(self, X, **kwargs):
         """Returns predictions for the given test data.
 
         Parameters
         ----------
-        X : Union[array-like, sparse matrix, dataframe] of shape (n_samples, n_features)
+        X : Union[array-like, sparse matrix, dataframe, of shape (n_samples, n_features)
             Training samples where n_samples is the number of samples
             and n_features is the number of features.
         **kwargs : Dict[str, Any]
             Extra arguments to route to ``Model.predict``.
 
         Warnings
         --------
@@ -1062,38 +1082,38 @@
         """Returns the score on the given test data and labels.
 
         No default scoring function is implemented in BaseWrapper,
         you must subclass and implement one.
 
         Parameters
         ----------
-        X : Union[array-like, sparse matrix, dataframe] of shape (n_samples, n_features)
+        X : Union[array-like, sparse matrix, dataframe, of shape (n_samples, n_features)
             Test input samples, where n_samples is the number of samples
             and n_features is the number of features.
-        y : Union[array-like, sparse matrix, dataframe] of shape \
+        y : Union[array-like, dataframe,, of shape \
             (n_samples,) or (n_samples, n_outputs)
             True labels for X.
         sample_weight : array-like of shape (n_samples,), default=None
             Array of weights that are assigned to individual samples.
             If not provided, then each sample is given unit weight.
 
         Returns
         -------
         float
             Score for the test data set.
         """
+        # validate y
+        _, y = self._validate_data(X=None, y=y)
+
         # validate sample weights
         if sample_weight is not None:
-            X, sample_weight = self._validate_sample_weight(
-                X=X, sample_weight=sample_weight
+            X, y, sample_weight = self._validate_sample_weight(
+                X=X, y=y, sample_weight=sample_weight
             )
 
-        # validate y
-        _, y = self._validate_data(X=None, y=y)
-
         # compute Keras model score
         y_pred = self.predict(X)
 
         # filter kwargs and get attributes for score
         params = self.get_params()
         score_args = route_params(params, destination="score", pass_filter=set())
 
@@ -1418,18 +1438,18 @@
         """Initialize the model without any fitting.
         You only need to call this model if you explicitly do not want to do any fitting
         (for example with a pretrained model). You should _not_ call this
         right before calling ``fit``, calling ``fit`` will do this automatically.
 
         Parameters
         ----------
-        X : Union[array-like, sparse matrix, dataframe] of shape (n_samples, n_features)
+        X : Union[array-like, sparse matrix, dataframe, of shape (n_samples, n_features)
                 Training samples where n_samples is the number of samples
                 and `n_features` is the number of features.
-        y : Union[array-like, sparse matrix, dataframe] of shape \
+        y : Union[array-like, dataframe,, of shape \
             (n_samples,) or (n_samples, n_outputs), default None
             True labels for X.
 
         Returns
         -------
         KerasClassifier
             A reference to the KerasClassifier instance for chained calling.
@@ -1439,18 +1459,18 @@
         return self
 
     def fit(self, X, y, sample_weight=None, **kwargs) -> "KerasClassifier":
         """Constructs a new classifier with ``model`` & fit the model to ``(X, y)``.
 
         Parameters
         ----------
-        X : Union[array-like, sparse matrix, dataframe] of shape (n_samples, n_features)
+        X : Union[array-like, sparse matrix, dataframe, of shape (n_samples, n_features)
             Training samples, where n_samples is the number of samples
             and n_features is the number of features.
-        y : Union[array-like, sparse matrix, dataframe] of shape (n_samples,) or (n_samples, n_outputs)
+        y : Union[array-like, dataframe,, of shape (n_samples,) or (n_samples, n_outputs)
             True labels for X.
         sample_weight : array-like of shape (n_samples,), default=None
             Array of weights that are assigned to individual samples.
             If not provided, then each sample is given unit weight.
         **kwargs : Dict[str, Any]
             Extra arguments to route to ``Model.fit``.
 
@@ -1478,18 +1498,18 @@
         self, X, y, classes=None, sample_weight=None, **kwargs
     ) -> "KerasClassifier":
         """Fit classifier for a single epoch, preserving the current epoch
         and all model parameters and state.
 
         Parameters
         ----------
-        X : Union[array-like, sparse matrix, dataframe] of shape (n_samples, n_features)
+        X : Union[array-like, sparse matrix, dataframe, of shape (n_samples, n_features)
             Training samples, where n_samples is the number of samples
             and n_features is the number of features.
-        y : Union[array-like, sparse matrix, dataframe] of shape (n_samples,) or (n_samples, n_outputs)
+        y : Union[array-like, dataframe,, of shape (n_samples,) or (n_samples, n_outputs)
             True labels for X.
         classes: ndarray of shape (n_classes,), default=None
             Classes across all calls to partial_fit. Can be obtained by via
             np.unique(y_all), where y_all is the target vector of the entire dataset.
             This argument is only needed for the first call to partial_fit and can be
             omitted in the subsequent calls. Note that y doesn’t need to contain
             all labels in classes. If you do not pass this argument, SciKeras
@@ -1516,15 +1536,15 @@
         return self
 
     def predict_proba(self, X, **kwargs):
         """Returns class probability estimates for the given test data.
 
         Parameters
         ----------
-        X : Union[array-like, sparse matrix, dataframe] of shape (n_samples, n_features)
+        X : Union[array-like, sparse matrix, dataframe, of shape (n_samples, n_features)
             Training samples, where n_samples is the number of samples
             and n_features is the number of features.
         **kwargs : Dict[str, Any]
             Extra arguments to route to ``Model.predict``.
 
         Warnings
         --------
```

### Comparing `scikeras-0.8.0/setup.py` & `scikeras-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 packages = \
 ['scikeras', 'scikeras.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['packaging>=0.21,<22.0', 'scikit-learn>=1.0.0']
+['packaging>=0.21', 'scikit-learn>=1.0.0']
 
 extras_require = \
 {':python_version < "3.8"': ['importlib-metadata>=3'],
  'tensorflow': ['tensorflow>=2.7.0'],
  'tensorflow-cpu': ['tensorflow-cpu>=2.7.0']}
 
 setup_kwargs = {
     'name': 'scikeras',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Scikit-Learn API wrapper for Keras.',
     'long_description': '# Scikit-Learn Wrapper for Keras\n\n[![Build Status](https://github.com/adriangb/scikeras/workflows/Tests/badge.svg)](https://github.com/adriangb/scikeras/actions?query=workflow%3ATests+branch%3Amaster)\n[![Coverage Status](https://codecov.io/gh/adriangb/scikeras/branch/master/graph/badge.svg)](https://codecov.io/gh/adriangb/scikeras)\n[![Docs](https://github.com/adriangb/scikeras/workflows/Build%20Docs/badge.svg)](https://www.adriangb.com/scikeras/)\n\nScikit-Learn compatible wrappers for Keras Models.\n\n## Why SciKeras\n\nSciKeras is derived from and API compatible with `tf.keras.wrappers.scikit_learn`. The original TensorFlow (TF) wrappers are not actively maintained,\nand [will be removed](https://github.com/tensorflow/tensorflow/pull/36137#issuecomment-726271760) in a future release.\n\nAn overview of the advantages and differences as compared to the TF wrappers can be found in our\n[migration](https://www.adriangb.com/scikeras/stable/migration.html) guide.\n\n## Installation\n\nThis package is available on PyPi:\n\n```bash\n# Normal tensorflow\npip install scikeras[tensorflow]\n\n# or tensorflow-cpu\npip install scikeras[tensorflow-cpu]\n```\n\nSciKeras packages TensorFlow as an optional dependency because there are\nseveral flavors of TensorFlow available (`tensorflow`, `tensorflow-cpu`, etc.).\nDepending on _one_ of them in particular disallows the usage of the other, which is why\nthey need to be optional.\n\n`pip install scikeras[tensorflow]` is basically equivalent to `pip install scikeras tensorflow`\nand is offered just for convenience. You can also install just SciKeras with\n`pip install scikeras`, but you will need a version of tensorflow installed at\nruntime or SciKeras will throw an error when you try to import it.\n\nThe current version of SciKeras depends on `scikit-learn>=1.0.0` and `TensorFlow>=2.7.0`.\n\n### Migrating from `tf.keras.wrappers.scikit_learn`\n\nPlease see the [migration](https://www.adriangb.com/scikeras/stable/migration.html) section of our documentation.\n\n## Documentation\n\nDocumentation is available at [https://www.adriangb.com/scikeras/](https://www.adriangb.com/scikeras/).\n\n## Contributing\n\nSee [CONTRIBUTING.md](https://github.com/adriangb/scikeras/blob/master/CONTRIBUTING.md)\n',
     'author': 'Adrian Garcia Badaracco',
     'author_email': '1755071+adriangb@users.noreply.github.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/adriangb/scikeras',
```

### Comparing `scikeras-0.8.0/PKG-INFO` & `scikeras-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikeras
-Version: 0.8.0
+Version: 0.9.0
 Summary: Scikit-Learn API wrapper for Keras.
 Home-page: https://github.com/adriangb/scikeras
 License: MIT
 Keywords: keras,tensorflow,scikit-learn,deep-learning,python
 Author: Adrian Garcia Badaracco
 Author-email: 1755071+adriangb@users.noreply.github.com
 Requires-Python: >=3.7.0,<3.11.0
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: tensorflow
 Provides-Extra: tensorflow-cpu
 Requires-Dist: importlib-metadata (>=3); python_version < "3.8"
-Requires-Dist: packaging (>=0.21,<22.0)
+Requires-Dist: packaging (>=0.21)
 Requires-Dist: scikit-learn (>=1.0.0)
 Requires-Dist: tensorflow (>=2.7.0); extra == "tensorflow"
 Requires-Dist: tensorflow-cpu (>=2.7.0); extra == "tensorflow-cpu"
 Project-URL: Documentation, https://www.adriangb.com/scikeras/
 Project-URL: Repository, https://github.com/adriangb/scikeras
 Description-Content-Type: text/markdown
```

