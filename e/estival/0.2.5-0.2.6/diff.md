# Comparing `tmp/estival-0.2.5.tar.gz` & `tmp/estival-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "estival-0.2.5.tar", max compression
+gzip compressed data, was "estival-0.2.6.tar", max compression
```

## Comparing `estival-0.2.5.tar` & `estival-0.2.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     3458 2023-05-18 00:47:35.180316 estival-0.2.5/estival/calibration/__pycache__/pymc.cpython-310.pyc
--rw-r--r--   0        0        0     4772 2023-05-06 03:26:51.437183 estival-0.2.5/estival/calibration/__pycache__/pymc.cpython-311.pyc
--rw-r--r--   0        0        0    14995 2023-05-05 04:48:51.863477 estival-0.2.5/estival/calibration/mcmc/__pycache__/adaptive.cpython-310.pyc
--rw-r--r--   0        0        0    25353 2023-05-05 05:24:17.406283 estival-0.2.5/estival/calibration/mcmc/__pycache__/adaptive.cpython-311.pyc
--rw-r--r--   0        0        0    14860 2023-02-20 23:46:02.295570 estival-0.2.5/estival/calibration/mcmc/__pycache__/adaptive.cpython-39.pyc
--rw-r--r--   0        0        0     2324 2023-05-05 04:48:54.568004 estival-0.2.5/estival/calibration/mcmc/__pycache__/covariance.cpython-310.pyc
--rw-r--r--   0        0        0     3213 2023-05-05 05:24:18.633294 estival-0.2.5/estival/calibration/mcmc/__pycache__/covariance.cpython-311.pyc
--rw-r--r--   0        0        0     2328 2023-02-21 00:23:32.275795 estival-0.2.5/estival/calibration/mcmc/__pycache__/covariance.cpython-39.pyc
--rw-r--r--   0        0        0     3211 2023-05-05 04:48:54.551505 estival-0.2.5/estival/calibration/mcmc/__pycache__/transformations.cpython-310.pyc
--rw-r--r--   0        0        0     5303 2023-05-05 05:24:18.606294 estival-0.2.5/estival/calibration/mcmc/__pycache__/transformations.cpython-311.pyc
--rw-r--r--   0        0        0     3288 2022-11-22 23:17:43.763620 estival-0.2.5/estival/calibration/mcmc/__pycache__/transformations.cpython-39.pyc
--rw-r--r--   0        0        0    23290 2023-05-03 06:12:36.018586 estival-0.2.5/estival/calibration/mcmc/adaptive.py
--rw-r--r--   0        0        0     1916 2023-02-21 00:23:01.508628 estival-0.2.5/estival/calibration/mcmc/covariance.py
--rw-r--r--   0        0        0     3408 2023-03-27 20:16:03.557131 estival-0.2.5/estival/calibration/mcmc/transformations.py
--rw-r--r--   0        0        0     3080 2023-05-11 03:41:35.661930 estival-0.2.5/estival/calibration/pymc.py
--rw-r--r--   0        0        0     2683 2023-05-11 02:56:54.916427 estival-0.2.5/estival/model.py
--rw-r--r--   0        0        0     2666 2023-05-03 21:37:51.092087 estival-0.2.5/estival/optimization/__pycache__/nevergrad.cpython-310.pyc
--rw-r--r--   0        0        0     4511 2023-05-05 05:24:18.926797 estival-0.2.5/estival/optimization/__pycache__/nevergrad.cpython-311.pyc
--rw-r--r--   0        0        0     2635 2023-05-03 21:00:19.800964 estival-0.2.5/estival/optimization/nevergrad.py
--rw-r--r--   0        0        0     4222 2023-05-10 03:48:52.052508 estival-0.2.5/estival/priors.py
--rw-r--r--   0        0        0    11486 2023-05-19 02:24:52.265480 estival-0.2.5/estival/targets.py
--rw-r--r--   0        0        0     2806 2023-03-29 04:09:12.012193 estival-0.2.5/estival/utils.py
--rw-r--r--   0        0        0     1320 2022-11-20 23:56:33.173670 estival-0.2.5/LICENSE
--rw-r--r--   0        0        0     1034 2023-05-19 02:26:27.177228 estival-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      588 2023-05-19 02:26:51.906422 estival-0.2.5/README.md
--rw-r--r--   0        0        0     1718 1970-01-01 00:00:00.000000 estival-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     3458 2023-05-18 00:47:35.180316 estival-0.2.6/estival/calibration/__pycache__/pymc.cpython-310.pyc
+-rw-r--r--   0        0        0     4772 2023-05-06 03:26:51.437183 estival-0.2.6/estival/calibration/__pycache__/pymc.cpython-311.pyc
+-rw-r--r--   0        0        0    14995 2023-05-05 04:48:51.863477 estival-0.2.6/estival/calibration/mcmc/__pycache__/adaptive.cpython-310.pyc
+-rw-r--r--   0        0        0    25353 2023-05-05 05:24:17.406283 estival-0.2.6/estival/calibration/mcmc/__pycache__/adaptive.cpython-311.pyc
+-rw-r--r--   0        0        0    14860 2023-02-20 23:46:02.295570 estival-0.2.6/estival/calibration/mcmc/__pycache__/adaptive.cpython-39.pyc
+-rw-r--r--   0        0        0     2324 2023-05-05 04:48:54.568004 estival-0.2.6/estival/calibration/mcmc/__pycache__/covariance.cpython-310.pyc
+-rw-r--r--   0        0        0     3213 2023-05-05 05:24:18.633294 estival-0.2.6/estival/calibration/mcmc/__pycache__/covariance.cpython-311.pyc
+-rw-r--r--   0        0        0     2328 2023-02-21 00:23:32.275795 estival-0.2.6/estival/calibration/mcmc/__pycache__/covariance.cpython-39.pyc
+-rw-r--r--   0        0        0     3211 2023-05-05 04:48:54.551505 estival-0.2.6/estival/calibration/mcmc/__pycache__/transformations.cpython-310.pyc
+-rw-r--r--   0        0        0     5303 2023-05-05 05:24:18.606294 estival-0.2.6/estival/calibration/mcmc/__pycache__/transformations.cpython-311.pyc
+-rw-r--r--   0        0        0     3288 2022-11-22 23:17:43.763620 estival-0.2.6/estival/calibration/mcmc/__pycache__/transformations.cpython-39.pyc
+-rw-r--r--   0        0        0    23290 2023-05-03 06:12:36.018586 estival-0.2.6/estival/calibration/mcmc/adaptive.py
+-rw-r--r--   0        0        0     1916 2023-02-21 00:23:01.508628 estival-0.2.6/estival/calibration/mcmc/covariance.py
+-rw-r--r--   0        0        0     3408 2023-03-27 20:16:03.557131 estival-0.2.6/estival/calibration/mcmc/transformations.py
+-rw-r--r--   0        0        0     3080 2023-05-11 03:41:35.661930 estival-0.2.6/estival/calibration/pymc.py
+-rw-r--r--   0        0        0     3957 2023-06-14 03:12:11.683431 estival-0.2.6/estival/model.py
+-rw-r--r--   0        0        0     2666 2023-05-03 21:37:51.092087 estival-0.2.6/estival/optimization/__pycache__/nevergrad.cpython-310.pyc
+-rw-r--r--   0        0        0     4511 2023-05-05 05:24:18.926797 estival-0.2.6/estival/optimization/__pycache__/nevergrad.cpython-311.pyc
+-rw-r--r--   0        0        0     2635 2023-05-03 21:00:19.800964 estival-0.2.6/estival/optimization/nevergrad.py
+-rw-r--r--   0        0        0     4192 2023-06-14 03:24:25.980234 estival-0.2.6/estival/priors.py
+-rw-r--r--   0        0        0    11486 2023-05-19 02:24:52.265480 estival-0.2.6/estival/targets.py
+-rw-r--r--   0        0        0     2806 2023-03-29 04:09:12.012193 estival-0.2.6/estival/utils.py
+-rw-r--r--   0        0        0     1320 2022-11-20 23:56:33.173670 estival-0.2.6/LICENSE
+-rw-r--r--   0        0        0     1034 2023-06-14 03:13:47.826686 estival-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      669 2023-06-14 03:14:19.151101 estival-0.2.6/README.md
+-rw-r--r--   0        0        0     1799 1970-01-01 00:00:00.000000 estival-0.2.6/PKG-INFO
```

### Comparing `estival-0.2.5/estival/calibration/__pycache__/pymc.cpython-310.pyc` & `estival-0.2.6/estival/calibration/__pycache__/pymc.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.5/estival/calibration/__pycache__/pymc.cpython-311.pyc` & `estival-0.2.6/estival/calibration/__pycache__/pymc.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.5/estival/calibration/mcmc/__pycache__/adaptive.cpython-310.pyc` & `estival-0.2.6/estival/calibration/mcmc/__pycache__/adaptive.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.5/estival/calibration/mcmc/__pycache__/adaptive.cpython-311.pyc` & `estival-0.2.6/estival/calibration/mcmc/__pycache__/adaptive.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.5/estival/calibration/mcmc/__pycache__/adaptive.cpython-39.pyc` & `estival-0.2.6/estival/calibration/mcmc/__pycache__/adaptive.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.5/estival/calibration/mcmc/__pycache__/covariance.cpython-310.pyc` & `estival-0.2.6/estival/calibration/mcmc/__pycache__/covariance.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.5/estival/calibration/mcmc/__pycache__/covariance.cpython-311.pyc` & `estival-0.2.6/estival/calibration/mcmc/__pycache__/covariance.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.5/estival/calibration/mcmc/__pycache__/covariance.cpython-39.pyc` & `estival-0.2.6/estival/calibration/mcmc/__pycache__/covariance.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.5/estival/calibration/mcmc/__pycache__/transformations.cpython-310.pyc` & `estival-0.2.6/estival/calibration/mcmc/__pycache__/transformations.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.5/estival/calibration/mcmc/__pycache__/transformations.cpython-311.pyc` & `estival-0.2.6/estival/calibration/mcmc/__pycache__/transformations.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.5/estival/calibration/mcmc/__pycache__/transformations.cpython-39.pyc` & `estival-0.2.6/estival/calibration/mcmc/__pycache__/transformations.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.5/estival/calibration/mcmc/adaptive.py` & `estival-0.2.6/estival/calibration/mcmc/adaptive.py`

 * *Files identical despite different names*

### Comparing `estival-0.2.5/estival/calibration/mcmc/covariance.py` & `estival-0.2.6/estival/calibration/mcmc/covariance.py`

 * *Files identical despite different names*

### Comparing `estival-0.2.5/estival/calibration/mcmc/transformations.py` & `estival-0.2.6/estival/calibration/mcmc/transformations.py`

 * *Files identical despite different names*

### Comparing `estival-0.2.5/estival/calibration/pymc.py` & `estival-0.2.6/estival/calibration/pymc.py`

 * *Files identical despite different names*

### Comparing `estival-0.2.5/estival/model.py` & `estival-0.2.6/estival/model.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,38 +4,46 @@
 from summer2 import CompartmentalModel
 
 from jax import jit
 
 import pandas as pd
 
 
+@dataclass
+class ResultsData:
+    derived_outputs: pd.DataFrame
+
+
 class BayesianCompartmentalModel:
     def __init__(
         self,
         model: CompartmentalModel,
         parameters: dict,
         priors: list,
         targets: list,
         extra_ll=None,
     ):
         self.model = model
+
+        self._model_parameters = model.get_input_parameters()
+
         self.parameters = parameters
         self.targets = {t.name: t for t in targets}
 
         for t in targets:
             priors = priors + t.get_priors()
         self.priors = {p.name: p for p in priors}
 
         self._ref_idx = self.model._get_ref_idx()
+        if not isinstance(self._ref_idx, pd.Index):
+            self._ref_idx = pd.Index(self._ref_idx)
         self.epoch = self.model.get_epoch()
 
         self.loglikelihood = self._build_logll_func(extra_ll)
 
-
-
     def _build_logll_func(self, extra_ll=None):
         model_params = self.model.get_input_parameters()
         dyn_params = list(model_params.intersection(set(self.priors)))
         self.model.set_derived_outputs_whitelist(list(self.targets))
 
         self._ll_runner = self.model.get_runner(self.parameters, dyn_params)
 
@@ -58,36 +66,56 @@
                 logdens += te(modelled, kwargs)
 
             if extra_ll:
                 logdens += extra_ll(kwargs)
 
             return logdens
 
+        logll.__doc__ = f"""logll({', '.join([k for k in self.priors])})\n
+        Run the model for a given set of parameters, and 
+        return the loglikelihood of its outputs, including any values from extrall"""
+
         return logll
 
     def logprior(self, **parameters):
         lp = 0.0
         for k, p in self.priors.items():
             lp += p.logpdf(parameters[k])
         return lp
 
     def logposterior(self, **parameters):
         return self.loglikelihood(**parameters) + self.logprior(**parameters)
 
-    def run(self, parameters):
-        results = self._full_runner._run_func(parameters)
+    def run(self, parameters: dict) -> ResultsData:
+        """Run the model for a given set of parameters.
+        Note that only parameters specified as priors affect the outputs; other parameters
+        are in-filled from the initial arguments supplied to BayesianCompartmentalModel
+
+        Args:
+            parameters: Dict of parameter key/values (as specified in priors)
+
+        Returns:
+            ResultsData, an extensible container with derived_outputs as a DataFrame
+        """
+        run_params = {k: v for k, v in parameters.items() if k in self._model_parameters}
+        results = self._full_runner._run_func(run_params)
+
         return ResultsData(
             derived_outputs=pd.DataFrame(results["derived_outputs"], index=self._ref_idx)
         )
 
-    def run_jax(self, parameters):
+    def run_jax(self, parameters: dict) -> dict:
+        """Run the jax run function for the model directly with the supplied parameters;
+        meaning bcm.run_jax can be included in JIT calls
+
+        Args:
+            parameters: Dict of parameter key/values (as specified in priors)
+
+        Returns:
+            Results as per the summer2 jax runner
+        """
         return self._full_runner._run_func(parameters)
 
 
-@dataclass
-class ResultsData:
-    derived_outputs: pd.DataFrame
-
-
 def capture_model_kwargs(model: CompartmentalModel, **kwargs) -> dict:
     model_params = model.get_input_parameters()
     return {k: kwargs[k] for k in kwargs if k in model_params}
```

### Comparing `estival-0.2.5/estival/optimization/__pycache__/nevergrad.cpython-310.pyc` & `estival-0.2.6/estival/optimization/__pycache__/nevergrad.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.5/estival/optimization/__pycache__/nevergrad.cpython-311.pyc` & `estival-0.2.6/estival/optimization/__pycache__/nevergrad.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `estival-0.2.5/estival/optimization/nevergrad.py` & `estival-0.2.6/estival/optimization/nevergrad.py`

 * *Files identical despite different names*

### Comparing `estival-0.2.5/estival/priors.py` & `estival-0.2.6/estival/priors.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,16 +54,16 @@
 
 
 class BetaPrior(BasePrior):
     """
     A beta distributed prior.
     """
 
-    def __init__(self, name: str, mean: float, ci: Tuple[float, float]):
-        super().__init__(name)
+    def __init__(self, name: str, mean: float, ci: Tuple[float, float], size=1):
+        super().__init__(name, size)
         self.mean = mean
         self.ci = ci
         self.name = name
         self._find_distri_params()
         self.rv = stats.beta(**self.distri_params)
 
     def bounds(self, ci=1.0) -> Tuple[float, float]:
@@ -116,29 +116,29 @@
 
 
 class TruncNormalPrior(BasePrior):
     """
     A prior with a truncated normal distribution.
     """
 
-    def __init__(self, name: str, mean: float, stdev: float, trunc_range: Tuple[float, float]):
-        super().__init__(name)
+    def __init__(
+        self, name: str, mean: float, stdev: float, trunc_range: Tuple[float, float], size=1
+    ):
+        super().__init__(name, size)
         self.mean, self.stdev = mean, stdev
         self.trunc_range = tuple(trunc_range)
         self.distri_params = {
             "loc": self.mean,
             "scale": self.stdev,
             "a": (trunc_range[0] - mean) / stdev,
             "b": (trunc_range[1] - mean) / stdev,
         }
         self.rv = stats.truncnorm(**self.distri_params)
 
     def to_pymc(self):
         lower, upper = self.trunc_range
         if self.size > 1:
-            lower = np.repeat(self.start, self.size)
-            upper = np.repeat(self.start, self.size)
-        else:
-            lower, upper = self.start, self.end
+            lower = np.repeat(lower, self.size)
+            upper = np.repeat(upper, self.size)
         return pm.TruncatedNormal(
             self.name, mu=self.mean, sigma=self.stdev, lower=lower, upper=upper
         )
```

### Comparing `estival-0.2.5/estival/targets.py` & `estival-0.2.6/estival/targets.py`

 * *Files identical despite different names*

### Comparing `estival-0.2.5/estival/utils.py` & `estival-0.2.6/estival/utils.py`

 * *Files identical despite different names*

### Comparing `estival-0.2.5/LICENSE` & `estival-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `estival-0.2.5/pyproject.toml` & `estival-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "estival"
-version = "0.2.5"
+version = "0.2.6"
 readme = "README.md"
 license = "BSD-2-Clause"
 homepage = "https://github.com/monash-emu/estival"
 repository = "https://github.com/monash-emu/estival"
 documentation = "https://github.com/monash-emu/estival"
 keywords = [
     "calibration",
```

### Comparing `estival-0.2.5/PKG-INFO` & `estival-0.2.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: estival
-Version: 0.2.5
+Version: 0.2.6
 Summary: A set of calibration and probabilistic programming tools for use with summerepi2
 Home-page: https://github.com/monash-emu/estival
 License: BSD-2-Clause
 Keywords: calibration,optimization,bayesian,compartmental modelling,summerepi
 Author: David Shipman
 Author-email: dshipman@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
@@ -41,7 +41,9 @@
 - 0.2.3  
 Include tensorflow-probability(jax) for more (and better tested) stats modules
 - 0.2.4
 Bugfix (vector priors were not exported to pymc correctly)
 Add Epoch support to allow DatetimeIndex targets
 - 0.2.5
 Bugfix for BinomialTarget (wasn't indexing modelled data)
+- 0.2.6
+Bugfix (reference index for models without date returned incorrect type)
```

