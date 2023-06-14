# Comparing `tmp/discotime-0.0.1.tar.gz` & `tmp/discotime-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discotime-0.0.1.tar", last modified: Tue Jun 13 13:44:43 2023, max compression
+gzip compressed data, was "discotime-0.0.2.tar", last modified: Wed Jun 14 08:00:19 2023, max compression
```

## Comparing `discotime-0.0.1.tar` & `discotime-0.0.2.tar`

### file list

```diff
@@ -1,40 +1,43 @@
-drwxr-xr-x   0 pechris   (1000) pechris   (1000)        0 2023-06-13 13:44:43.162091 discotime-0.0.1/
--rw-r--r--   0 pechris   (1000) pechris   (1000)     1079 2022-12-20 15:34:43.000000 discotime-0.0.1/LICENSE
--rw-r--r--   0 pechris   (1000) pechris   (1000)       62 2023-01-18 09:20:28.000000 discotime-0.0.1/MANIFEST.in
--rw-r--r--   0 pechris   (1000) pechris   (1000)     1306 2023-06-13 13:44:43.162091 discotime-0.0.1/PKG-INFO
--rw-r--r--   0 pechris   (1000) pechris   (1000)      907 2023-06-13 11:52:54.000000 discotime-0.0.1/README.md
--rw-r--r--   0 pechris   (1000) pechris   (1000)      122 2023-06-13 13:32:17.000000 discotime-0.0.1/pyproject.toml
--rw-r--r--   0 pechris   (1000) pechris   (1000)     2333 2023-06-13 13:44:43.162091 discotime-0.0.1/setup.cfg
-drwxr-xr-x   0 pechris   (1000) pechris   (1000)        0 2023-06-13 13:44:43.162091 discotime-0.0.1/src/
-drwxr-xr-x   0 pechris   (1000) pechris   (1000)        0 2023-06-13 13:44:43.162091 discotime-0.0.1/src/discotime/
--rw-r--r--   0 pechris   (1000) pechris   (1000)      106 2023-05-20 12:38:12.000000 discotime-0.0.1/src/discotime/__init__.py
-drwxr-xr-x   0 pechris   (1000) pechris   (1000)        0 2023-06-13 13:44:43.162091 discotime-0.0.1/src/discotime/datasets/
--rw-r--r--   0 pechris   (1000) pechris   (1000)      152 2023-06-13 13:01:51.000000 discotime-0.0.1/src/discotime/datasets/__init__.py
--rw-r--r--   0 pechris   (1000) pechris   (1000)     5675 2023-06-06 19:25:55.000000 discotime-0.0.1/src/discotime/datasets/from_rstats.py
--rw-r--r--   0 pechris   (1000) pechris   (1000)    11265 2023-06-06 19:53:02.000000 discotime-0.0.1/src/discotime/datasets/utils.py
-drwxr-xr-x   0 pechris   (1000) pechris   (1000)        0 2023-06-13 13:44:43.162091 discotime-0.0.1/src/discotime/metrics/
--rw-r--r--   0 pechris   (1000) pechris   (1000)       91 2023-02-23 14:14:46.000000 discotime-0.0.1/src/discotime/metrics/__init__.py
--rw-r--r--   0 pechris   (1000) pechris   (1000)     4635 2023-06-12 13:59:45.000000 discotime-0.0.1/src/discotime/metrics/brier_score.py
--rw-r--r--   0 pechris   (1000) pechris   (1000)     1922 2023-05-30 10:17:34.000000 discotime-0.0.1/src/discotime/metrics/ipa.py
-drwxr-xr-x   0 pechris   (1000) pechris   (1000)        0 2023-06-13 13:44:43.162091 discotime-0.0.1/src/discotime/models/
--rw-r--r--   0 pechris   (1000) pechris   (1000)       63 2023-05-23 08:03:53.000000 discotime-0.0.1/src/discotime/models/__init__.py
--rw-r--r--   0 pechris   (1000) pechris   (1000)     5105 2023-05-23 12:44:07.000000 discotime-0.0.1/src/discotime/models/components.py
--rw-r--r--   0 pechris   (1000) pechris   (1000)    10384 2023-06-12 12:40:34.000000 discotime-0.0.1/src/discotime/models/models.py
-drwxr-xr-x   0 pechris   (1000) pechris   (1000)        0 2023-06-13 13:44:43.162091 discotime-0.0.1/src/discotime/utils/
--rw-r--r--   0 pechris   (1000) pechris   (1000)      112 2023-03-08 13:10:12.000000 discotime-0.0.1/src/discotime/utils/__init__.py
--rw-r--r--   0 pechris   (1000) pechris   (1000)     5798 2023-06-12 13:58:39.000000 discotime-0.0.1/src/discotime/utils/estimators.py
--rw-r--r--   0 pechris   (1000) pechris   (1000)     6455 2023-06-13 09:24:05.000000 discotime-0.0.1/src/discotime/utils/misc.py
--rw-r--r--   0 pechris   (1000) pechris   (1000)     1246 2023-06-06 19:52:29.000000 discotime-0.0.1/src/discotime/utils/typing.py
-drwxr-xr-x   0 pechris   (1000) pechris   (1000)        0 2023-06-13 13:44:43.162091 discotime-0.0.1/src/discotime.egg-info/
--rw-r--r--   0 pechris   (1000) pechris   (1000)     1306 2023-06-13 13:44:43.000000 discotime-0.0.1/src/discotime.egg-info/PKG-INFO
--rw-r--r--   0 pechris   (1000) pechris   (1000)      834 2023-06-13 13:44:43.000000 discotime-0.0.1/src/discotime.egg-info/SOURCES.txt
--rw-r--r--   0 pechris   (1000) pechris   (1000)        1 2023-06-13 13:44:43.000000 discotime-0.0.1/src/discotime.egg-info/dependency_links.txt
--rw-r--r--   0 pechris   (1000) pechris   (1000)      183 2023-06-13 13:44:43.000000 discotime-0.0.1/src/discotime.egg-info/requires.txt
--rw-r--r--   0 pechris   (1000) pechris   (1000)       10 2023-06-13 13:44:43.000000 discotime-0.0.1/src/discotime.egg-info/top_level.txt
-drwxr-xr-x   0 pechris   (1000) pechris   (1000)        0 2023-06-13 13:44:43.162091 discotime-0.0.1/tests/
--rw-r--r--   0 pechris   (1000) pechris   (1000)      934 2023-06-13 13:03:24.000000 discotime-0.0.1/tests/test_lightning_module.py
--rw-r--r--   0 pechris   (1000) pechris   (1000)     3521 2023-05-30 10:38:15.000000 discotime-0.0.1/tests/test_metrics.py
--rw-r--r--   0 pechris   (1000) pechris   (1000)     1411 2023-06-12 11:19:51.000000 discotime-0.0.1/tests/test_mgus2.py
--rw-r--r--   0 pechris   (1000) pechris   (1000)     1867 2023-06-12 11:21:21.000000 discotime-0.0.1/tests/test_models.py
--rw-r--r--   0 pechris   (1000) pechris   (1000)     1989 2023-06-06 19:49:32.000000 discotime-0.0.1/tests/test_preprocessing.py
--rw-r--r--   0 pechris   (1000) pechris   (1000)     3487 2023-05-22 14:09:38.000000 discotime-0.0.1/tests/test_utils.py
+drwxr-xr-x   0 pechris   (1000) pechris   (1000)        0 2023-06-14 08:00:19.864440 discotime-0.0.2/
+-rw-r--r--   0 pechris   (1000) pechris   (1000)     1079 2022-12-20 15:34:43.000000 discotime-0.0.2/LICENSE
+-rw-r--r--   0 pechris   (1000) pechris   (1000)       62 2023-01-18 09:20:28.000000 discotime-0.0.2/MANIFEST.in
+-rw-r--r--   0 pechris   (1000) pechris   (1000)     1463 2023-06-14 08:00:19.864440 discotime-0.0.2/PKG-INFO
+-rw-r--r--   0 pechris   (1000) pechris   (1000)     1064 2023-06-14 06:33:22.000000 discotime-0.0.2/README.md
+-rw-r--r--   0 pechris   (1000) pechris   (1000)      122 2023-06-13 13:32:17.000000 discotime-0.0.2/pyproject.toml
+-rw-r--r--   0 pechris   (1000) pechris   (1000)     2333 2023-06-14 08:00:19.864440 discotime-0.0.2/setup.cfg
+drwxr-xr-x   0 pechris   (1000) pechris   (1000)        0 2023-06-14 08:00:19.854440 discotime-0.0.2/src/
+drwxr-xr-x   0 pechris   (1000) pechris   (1000)        0 2023-06-14 08:00:19.854440 discotime-0.0.2/src/discotime/
+-rw-r--r--   0 pechris   (1000) pechris   (1000)      106 2023-05-20 12:38:12.000000 discotime-0.0.2/src/discotime/__init__.py
+drwxr-xr-x   0 pechris   (1000) pechris   (1000)        0 2023-06-14 08:00:19.854440 discotime-0.0.2/src/discotime/datasets/
+-rw-r--r--   0 pechris   (1000) pechris   (1000)      152 2023-06-13 13:01:51.000000 discotime-0.0.2/src/discotime/datasets/__init__.py
+drwxr-xr-x   0 pechris   (1000) pechris   (1000)        0 2023-06-14 08:00:19.854440 discotime-0.0.2/src/discotime/datasets/_data/
+-rw-r--r--   0 pechris   (1000) pechris   (1000)        1 2023-06-13 14:19:52.000000 discotime-0.0.2/src/discotime/datasets/_data/.gitignore
+-rw-r--r--   0 pechris   (1000) pechris   (1000)    49998 2023-06-13 14:17:42.000000 discotime-0.0.2/src/discotime/datasets/_data/mgus2.csv
+-rw-r--r--   0 pechris   (1000) pechris   (1000)     5775 2023-06-13 14:17:31.000000 discotime-0.0.2/src/discotime/datasets/from_rstats.py
+-rw-r--r--   0 pechris   (1000) pechris   (1000)    11275 2023-06-13 18:44:19.000000 discotime-0.0.2/src/discotime/datasets/utils.py
+drwxr-xr-x   0 pechris   (1000) pechris   (1000)        0 2023-06-14 08:00:19.854440 discotime-0.0.2/src/discotime/metrics/
+-rw-r--r--   0 pechris   (1000) pechris   (1000)       91 2023-02-23 14:14:46.000000 discotime-0.0.2/src/discotime/metrics/__init__.py
+-rw-r--r--   0 pechris   (1000) pechris   (1000)     4635 2023-06-12 13:59:45.000000 discotime-0.0.2/src/discotime/metrics/brier_score.py
+-rw-r--r--   0 pechris   (1000) pechris   (1000)     1922 2023-05-30 10:17:34.000000 discotime-0.0.2/src/discotime/metrics/ipa.py
+drwxr-xr-x   0 pechris   (1000) pechris   (1000)        0 2023-06-14 08:00:19.864440 discotime-0.0.2/src/discotime/models/
+-rw-r--r--   0 pechris   (1000) pechris   (1000)       63 2023-05-23 08:03:53.000000 discotime-0.0.2/src/discotime/models/__init__.py
+-rw-r--r--   0 pechris   (1000) pechris   (1000)     5105 2023-05-23 12:44:07.000000 discotime-0.0.2/src/discotime/models/components.py
+-rw-r--r--   0 pechris   (1000) pechris   (1000)    10384 2023-06-12 12:40:34.000000 discotime-0.0.2/src/discotime/models/models.py
+drwxr-xr-x   0 pechris   (1000) pechris   (1000)        0 2023-06-14 08:00:19.864440 discotime-0.0.2/src/discotime/utils/
+-rw-r--r--   0 pechris   (1000) pechris   (1000)      112 2023-03-08 13:10:12.000000 discotime-0.0.2/src/discotime/utils/__init__.py
+-rw-r--r--   0 pechris   (1000) pechris   (1000)     5802 2023-06-13 17:44:35.000000 discotime-0.0.2/src/discotime/utils/estimators.py
+-rw-r--r--   0 pechris   (1000) pechris   (1000)     6566 2023-06-13 17:48:04.000000 discotime-0.0.2/src/discotime/utils/misc.py
+-rw-r--r--   0 pechris   (1000) pechris   (1000)     1274 2023-06-13 18:42:48.000000 discotime-0.0.2/src/discotime/utils/typing.py
+drwxr-xr-x   0 pechris   (1000) pechris   (1000)        0 2023-06-14 08:00:19.854440 discotime-0.0.2/src/discotime.egg-info/
+-rw-r--r--   0 pechris   (1000) pechris   (1000)     1463 2023-06-14 08:00:19.000000 discotime-0.0.2/src/discotime.egg-info/PKG-INFO
+-rw-r--r--   0 pechris   (1000) pechris   (1000)      913 2023-06-14 08:00:19.000000 discotime-0.0.2/src/discotime.egg-info/SOURCES.txt
+-rw-r--r--   0 pechris   (1000) pechris   (1000)        1 2023-06-14 08:00:19.000000 discotime-0.0.2/src/discotime.egg-info/dependency_links.txt
+-rw-r--r--   0 pechris   (1000) pechris   (1000)      183 2023-06-14 08:00:19.000000 discotime-0.0.2/src/discotime.egg-info/requires.txt
+-rw-r--r--   0 pechris   (1000) pechris   (1000)       10 2023-06-14 08:00:19.000000 discotime-0.0.2/src/discotime.egg-info/top_level.txt
+drwxr-xr-x   0 pechris   (1000) pechris   (1000)        0 2023-06-14 08:00:19.864440 discotime-0.0.2/tests/
+-rw-r--r--   0 pechris   (1000) pechris   (1000)      934 2023-06-13 13:03:24.000000 discotime-0.0.2/tests/test_lightning_module.py
+-rw-r--r--   0 pechris   (1000) pechris   (1000)     3521 2023-05-30 10:38:15.000000 discotime-0.0.2/tests/test_metrics.py
+-rw-r--r--   0 pechris   (1000) pechris   (1000)     1427 2023-06-13 17:48:41.000000 discotime-0.0.2/tests/test_mgus2.py
+-rw-r--r--   0 pechris   (1000) pechris   (1000)     1867 2023-06-12 11:21:21.000000 discotime-0.0.2/tests/test_models.py
+-rw-r--r--   0 pechris   (1000) pechris   (1000)     1989 2023-06-06 19:49:32.000000 discotime-0.0.2/tests/test_preprocessing.py
+-rw-r--r--   0 pechris   (1000) pechris   (1000)     3487 2023-05-22 14:09:38.000000 discotime-0.0.2/tests/test_utils.py
```

### Comparing `discotime-0.0.1/LICENSE` & `discotime-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `discotime-0.0.1/PKG-INFO` & `discotime-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: discotime
-Version: 0.0.1
+Version: 0.0.2
 Summary: Discrete-time competing risk analysis with neural networks
 Home-page: https://github.com/peterchristofferholm/discotime
 Author: Peter Holm
 Author-email: "Peter Holm" <petchdk@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![Documentation Status](https://readthedocs.org/projects/discotime/badge/?version=latest)](https://discotime.readthedocs.io/en/latest/?badge=latest)
+
 # Discotime: Discrete-time Competing Risks Models with PyTorch Lightning
 
-[**Docs**](https://optuna.readthedocs.io/en/stable/)
-| [**Installation**](https://optuna.readthedocs.io/en/stable/installation.html)
-| [**Tutorial**](https://optuna.readthedocs.io/en/stable/tutorial/index.html)
-| [**Examples**](https://github.com/optuna/optuna-examples)
+[**Docs**](https://discotime.readthedocs.io/en/stable/)
+| [**Installation**](https://discotime.readthedocs.io/en/stable/installation.html)
+| [**Tutorial**](https://discotime.readthedocs.io/en/stable/tutorial/index.html)
+| [**Examples**](https://github.com/discotime/examples)
 
 *Discotime* is a python package for discrete-time survival analysis 
 with neural networks that have been designed to handle competing risk models.
 The package relies on PyTorch Lightning to provide an easy-to-use interface,
 that still can be customized to your heart's content. 
 The packages contains an implementation of discrete time-to-event models
 for neural networks (using PyTorch), different evaluation metrics,
 and a couple of different competing risk datasets. 
+
 **The package is currently under development,**
 **Breaking changes are to be expected.**
```

### Comparing `discotime-0.0.1/setup.cfg` & `discotime-0.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = discotime
-version = 0.0.1
+version = 0.0.2
 url = https://github.com/peterchristofferholm/discotime
 author = Peter Holm
 author_email = "Peter Holm" <petchdk@gmail.com>
 description = Discrete-time competing risk analysis with neural networks
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
```

### Comparing `discotime-0.0.1/src/discotime/datasets/from_rstats.py` & `discotime-0.0.2/src/discotime/datasets/from_rstats.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     default_fts_transformer,
     SurvDataset,
 )
 from discotime.datasets.utils import LabelDiscretizer
 
 
 _ROOT_PATH = Path(discotime.__file__).parent
-_DATA_PATH = _ROOT_PATH / "datasets" / "_data" / "_downloads"
+_DATA_PATH = _ROOT_PATH / "datasets" / "_data"
 
 
 class Mgus2(LitSurvDataModule):
     """
     Natural history of 1341 sequential patients with monoclonal gammopathy of
     undetermined significance (MGUS).
 
@@ -70,14 +70,16 @@
         available, then the download logic is skipped.
 
         [1]: Therneau T (2023). A Package for Survival Analysis in R.
         """
         url = "https://github.com/therneau/survival/raw/649851/data/cancer.rda"
 
         if not self.mgus2_csv.is_file():
+            # create data directory if needed
+            self.mgus2_csv.parent.mkdir(parents=True, exist_ok=True)
             # download and parse rdata file
             r = requests.get(url)
             parsed = rdata.parser.parse_data(r.content)
             df = rdata.conversion.convert(parsed)["mgus2"]
             # slight reformatting
             x = df.loc[:, "age":"mspike"]  # type: ignore
             t = df[["futime", "ptime"]].min(axis=1)
```

### Comparing `discotime-0.0.1/src/discotime/datasets/utils.py` & `discotime-0.0.2/src/discotime/datasets/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,18 +31,18 @@
     and :math:`\mathbf{x}_{i} \in \mathbb{R}^d` is a :math:`d`-dimensional
     vector of time-independent predictors or covariates.
 
     Args:
         features: time-independent features.
         event_time: follow-up time (continuous).
         event_status: event indicator (0=censored, 1/2/...=competing risks).
-        discretizer: discretizer that follows the :obj:`LabelTransformer`
+        discretizer: discretizer that follows the :py:class:`LabelTransformer`
             protocol that convert continuous time/event tuples to their
             respective discretized versions. Typically this would be
-            :obj:`LabelDiscretizer` unless a custom discretization object is
+            :py:class:`LabelDiscretizer` unless a custom discretization object is
             used.
     """
 
     def __init__(
         self,
         features: npt.ArrayLike,
         event_time: npt.ArrayLike,
```

### Comparing `discotime-0.0.1/src/discotime/metrics/brier_score.py` & `discotime-0.0.2/src/discotime/metrics/brier_score.py`

 * *Files identical despite different names*

### Comparing `discotime-0.0.1/src/discotime/metrics/ipa.py` & `discotime-0.0.2/src/discotime/metrics/ipa.py`

 * *Files identical despite different names*

### Comparing `discotime-0.0.1/src/discotime/models/components.py` & `discotime-0.0.2/src/discotime/models/components.py`

 * *Files identical despite different names*

### Comparing `discotime-0.0.1/src/discotime/models/models.py` & `discotime-0.0.2/src/discotime/models/models.py`

 * *Files identical despite different names*

### Comparing `discotime-0.0.1/src/discotime/utils/estimators.py` & `discotime-0.0.2/src/discotime/utils/estimators.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             then all observed causes are include.
     """
 
     def __init__(
         self,
         time: npt.ArrayLike,
         event: npt.ArrayLike,
-        n_causes: Optional[int] = None,
+        n_causes: Optional[Int] = None,
     ) -> None:
         time, event = map(np.asarray, (time, event))
 
         if time.ndim != 1:
             raise ValueError(f"`time` is a {time.ndim}D array.")
 
         if event.ndim != 1:
@@ -129,15 +129,15 @@
         # lagged survival which starts with P(0) = 1
         sj = np.cumprod((nj - mj) / nj)[:-1]
         sj = np.pad(sj, (1, 0), constant_values=1)
 
         # cause-specific incidences
         n_risks = n_causes if n_causes else np.max(event)
         ci = np.zeros((tj.size, n_risks))
-        for e in range(1, n_risks):
+        for e in range(1, n_risks + 1):
             mcj = _pad(_tabulate(tj, time[event == e]))
             ci[:, e - 1] = np.cumsum(sj * (mcj / nj))
 
         self._tj = tj
         self._sj = sj
         self._ci = ci
```

### Comparing `discotime-0.0.1/src/discotime/utils/misc.py` & `discotime-0.0.2/src/discotime/utils/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     Args:
         d (Mapping): dictionary/mapping of things.
         u (Mapping): other dictionary/mapping of things to update `d` with.
 
     Example:
         >>> foo = {"dog" : {"color" : "black", "age" : 10}}
         >>> bar = {"dog" : {"age" : 11}, "cat" : None}
-        >>> recursive_update(foo, bar)
+        >>> update_mapping(foo, bar)
         {'dog': {'color': 'black', 'age': 11}, 'cat': None}
     """
     for k, v in u.items():
         if isinstance(v, Mapping):
             d[k] = update_mapping(d.get(k, {}), v)  # type: ignore
         else:
             d[k] = v  # type: ignore
@@ -82,14 +82,17 @@
         train_dl = self.fabric.setup_dataloaders(self.train_dl)
         valid_dl = self.fabric.setup_dataloaders(self.valid_dl)
         module, optimizer = self.fabric.setup(
             self.module,
             self.module.configure_optimizers(),
         )
 
+        assert isinstance(train_dl, DataLoader)
+        assert isinstance(valid_dl, DataLoader)
+
         while True:
             self.module.train()
             with torch.set_grad_enabled(True):
                 for batch_idx, batch in enumerate(train_dl):
                     loss = module.training_step(batch, batch_idx)
                     optimizer.zero_grad()
                     self.fabric.backward(loss)
@@ -97,15 +100,15 @@
 
             with torch.set_grad_enabled(False):
                 module.eval()
                 losses = (
                     module.validation_step(batch, idx) * len(batch[1])
                     for idx, batch in enumerate(valid_dl)
                 )
-                yield sum(losses) / len(valid_dl.sampler)
+                yield sum(losses) / len(valid_dl.sampler)  # type: ignore
 
 
 def split_dataset(
     dataset: Dataset[T], k: int = 5
 ) -> Generator[tuple[ConcatDataset[T], Subset[T]], None, None]:
     """Split dataset into k train/validation splits"""
     splits = deque(random_split(dataset, lengths=[1 / k] * k))
```

### Comparing `discotime-0.0.1/src/discotime/utils/typing.py` & `discotime-0.0.2/src/discotime/utils/typing.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,16 @@
         ...
 
     def fit_transform(self, *args, **kwargs) -> Any:
         ...
 
 
 class LabelTransformer(Transformer, Protocol):
+    """LabelTransformer"""
+
     def fit(self, time: Iterable[Num], event: Iterable[Int]) -> None:
         ...
 
     def transform(
         self,
         time: Iterable[Num],
         event: Iterable[Int],
```

### Comparing `discotime-0.0.1/src/discotime.egg-info/PKG-INFO` & `discotime-0.0.2/src/discotime.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: discotime
-Version: 0.0.1
+Version: 0.0.2
 Summary: Discrete-time competing risk analysis with neural networks
 Home-page: https://github.com/peterchristofferholm/discotime
 Author: Peter Holm
 Author-email: "Peter Holm" <petchdk@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![Documentation Status](https://readthedocs.org/projects/discotime/badge/?version=latest)](https://discotime.readthedocs.io/en/latest/?badge=latest)
+
 # Discotime: Discrete-time Competing Risks Models with PyTorch Lightning
 
-[**Docs**](https://optuna.readthedocs.io/en/stable/)
-| [**Installation**](https://optuna.readthedocs.io/en/stable/installation.html)
-| [**Tutorial**](https://optuna.readthedocs.io/en/stable/tutorial/index.html)
-| [**Examples**](https://github.com/optuna/optuna-examples)
+[**Docs**](https://discotime.readthedocs.io/en/stable/)
+| [**Installation**](https://discotime.readthedocs.io/en/stable/installation.html)
+| [**Tutorial**](https://discotime.readthedocs.io/en/stable/tutorial/index.html)
+| [**Examples**](https://github.com/discotime/examples)
 
 *Discotime* is a python package for discrete-time survival analysis 
 with neural networks that have been designed to handle competing risk models.
 The package relies on PyTorch Lightning to provide an easy-to-use interface,
 that still can be customized to your heart's content. 
 The packages contains an implementation of discrete time-to-event models
 for neural networks (using PyTorch), different evaluation metrics,
 and a couple of different competing risk datasets. 
+
 **The package is currently under development,**
 **Breaking changes are to be expected.**
```

### Comparing `discotime-0.0.1/src/discotime.egg-info/SOURCES.txt` & `discotime-0.0.2/src/discotime.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 src/discotime.egg-info/SOURCES.txt
 src/discotime.egg-info/dependency_links.txt
 src/discotime.egg-info/requires.txt
 src/discotime.egg-info/top_level.txt
 src/discotime/datasets/__init__.py
 src/discotime/datasets/from_rstats.py
 src/discotime/datasets/utils.py
+src/discotime/datasets/_data/.gitignore
+src/discotime/datasets/_data/mgus2.csv
 src/discotime/metrics/__init__.py
 src/discotime/metrics/brier_score.py
 src/discotime/metrics/ipa.py
 src/discotime/models/__init__.py
 src/discotime/models/components.py
 src/discotime/models/models.py
 src/discotime/utils/__init__.py
```

### Comparing `discotime-0.0.1/tests/test_lightning_module.py` & `discotime-0.0.2/tests/test_lightning_module.py`

 * *Files identical despite different names*

### Comparing `discotime-0.0.1/tests/test_metrics.py` & `discotime-0.0.2/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `discotime-0.0.1/tests/test_mgus2.py` & `discotime-0.0.2/tests/test_mgus2.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     assert len(mgus2_dm.dset_train[0]) == 5
     assert len(mgus2_dm.dset_test[0]) == 5
 
     assert len(next(iter(mgus2_dm.train_dataloader()))) == 5
     assert len(next(iter(mgus2_dm.test_dataloader()))) == 5
 
     # number of cuts is n_time_bins + 1
-    assert len(mgus2_dm.cuts) == (mgus2_dm.hparams.data_config.n_time_bins + 1)
+    assert len(mgus2_dm.cuts) == (mgus2_dm.hparams.data_config.n_time_bins + 1)  # type: ignore
 
 
 @mark.filterwarnings("ignore")
 def test_model_integration(mgus2_dm: Mgus2):
     model = LitSurvModule(ModelConfig())
     trainer = Trainer(
         accelerator="cpu",
```

### Comparing `discotime-0.0.1/tests/test_models.py` & `discotime-0.0.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `discotime-0.0.1/tests/test_preprocessing.py` & `discotime-0.0.2/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `discotime-0.0.1/tests/test_utils.py` & `discotime-0.0.2/tests/test_utils.py`

 * *Files identical despite different names*

