# Comparing `tmp/pydeseq2-0.3.3.tar.gz` & `tmp/pydeseq2-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/bmuzellec/Documents/Projects/FL_genomics/PyDESeq2/dist/.tmp-2p0keonu/pydeseq2-0.3.3.tar", last modified: Thu Apr  6 14:08:46 2023, max compression
+gzip compressed data, was "/Users/bmuzellec/Documents/Projects/FL_genomics/PyDESeq2/dist/.tmp-ywmm2g4l/pydeseq2-0.3.4.tar", last modified: Thu Jun  1 08:45:02 2023, max compression
```

## Comparing `pydeseq2-0.3.3.tar` & `pydeseq2-0.3.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 bmuzellec   (501) staff       (20)        0 2023-04-06 14:08:46.000000 pydeseq2-0.3.3/
--rw-r--r--   0 bmuzellec   (501) staff       (20)     1062 2022-12-03 17:11:22.000000 pydeseq2-0.3.3/LICENSE
--rw-r--r--   0 bmuzellec   (501) staff       (20)     6066 2023-04-06 14:08:46.000000 pydeseq2-0.3.3/PKG-INFO
--rw-r--r--   0 bmuzellec   (501) staff       (20)     5733 2023-04-06 08:39:13.000000 pydeseq2-0.3.3/README.md
-drwxr-xr-x   0 bmuzellec   (501) staff       (20)        0 2023-04-06 14:08:46.000000 pydeseq2-0.3.3/pydeseq2/
--rw-r--r--   0 bmuzellec   (501) staff       (20)       53 2022-12-28 09:54:14.000000 pydeseq2-0.3.3/pydeseq2/__init__.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)       22 2023-04-06 14:03:10.000000 pydeseq2-0.3.3/pydeseq2/__version__.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)    36609 2023-04-06 14:02:20.000000 pydeseq2-0.3.3/pydeseq2/dds.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)    22038 2023-04-06 14:02:20.000000 pydeseq2-0.3.3/pydeseq2/ds.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)     8480 2023-03-24 14:45:04.000000 pydeseq2-0.3.3/pydeseq2/grid_search.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)     1316 2023-03-15 10:56:22.000000 pydeseq2-0.3.3/pydeseq2/preprocessing.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)    37616 2023-04-06 14:02:20.000000 pydeseq2-0.3.3/pydeseq2/utils.py
-drwxr-xr-x   0 bmuzellec   (501) staff       (20)        0 2023-04-06 14:08:46.000000 pydeseq2-0.3.3/pydeseq2.egg-info/
--rw-r--r--   0 bmuzellec   (501) staff       (20)     6066 2023-04-06 14:08:45.000000 pydeseq2-0.3.3/pydeseq2.egg-info/PKG-INFO
--rw-r--r--   0 bmuzellec   (501) staff       (20)      436 2023-04-06 14:08:45.000000 pydeseq2-0.3.3/pydeseq2.egg-info/SOURCES.txt
--rw-r--r--   0 bmuzellec   (501) staff       (20)        1 2023-04-06 14:08:45.000000 pydeseq2-0.3.3/pydeseq2.egg-info/dependency_links.txt
--rw-r--r--   0 bmuzellec   (501) staff       (20)      190 2023-04-06 14:08:45.000000 pydeseq2-0.3.3/pydeseq2.egg-info/requires.txt
--rw-r--r--   0 bmuzellec   (501) staff       (20)        9 2023-04-06 14:08:45.000000 pydeseq2-0.3.3/pydeseq2.egg-info/top_level.txt
--rw-r--r--   0 bmuzellec   (501) staff       (20)      408 2023-04-05 09:20:58.000000 pydeseq2-0.3.3/pyproject.toml
--rw-r--r--   0 bmuzellec   (501) staff       (20)       38 2023-04-06 14:08:46.000000 pydeseq2-0.3.3/setup.cfg
--rw-r--r--   0 bmuzellec   (501) staff       (20)     1362 2023-02-20 15:16:54.000000 pydeseq2-0.3.3/setup.py
-drwxr-xr-x   0 bmuzellec   (501) staff       (20)        0 2023-04-06 14:08:46.000000 pydeseq2-0.3.3/tests/
--rw-r--r--   0 bmuzellec   (501) staff       (20)     5654 2023-02-16 10:34:42.000000 pydeseq2-0.3.3/tests/test_docstring.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)    11010 2023-04-06 14:02:20.000000 pydeseq2-0.3.3/tests/test_edge_cases.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)    14231 2023-04-06 14:02:20.000000 pydeseq2-0.3.3/tests/test_pydeseq2.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)     1951 2023-02-21 15:32:02.000000 pydeseq2-0.3.3/tests/test_utils.py
+drwxr-xr-x   0 bmuzellec   (501) staff       (20)        0 2023-06-01 08:45:02.000000 pydeseq2-0.3.4/
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     1062 2022-12-03 17:11:22.000000 pydeseq2-0.3.4/LICENSE
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     6216 2023-06-01 08:45:02.000000 pydeseq2-0.3.4/PKG-INFO
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     5883 2023-06-01 08:36:08.000000 pydeseq2-0.3.4/README.md
+drwxr-xr-x   0 bmuzellec   (501) staff       (20)        0 2023-06-01 08:45:02.000000 pydeseq2-0.3.4/pydeseq2/
+-rw-r--r--   0 bmuzellec   (501) staff       (20)       53 2022-12-28 09:54:14.000000 pydeseq2-0.3.4/pydeseq2/__init__.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)       22 2023-06-01 08:37:49.000000 pydeseq2-0.3.4/pydeseq2/__version__.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)    38712 2023-06-01 08:36:08.000000 pydeseq2-0.3.4/pydeseq2/dds.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)    23930 2023-06-01 08:36:10.000000 pydeseq2-0.3.4/pydeseq2/ds.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     8480 2023-03-24 14:45:04.000000 pydeseq2-0.3.4/pydeseq2/grid_search.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     1587 2023-06-01 08:36:08.000000 pydeseq2-0.3.4/pydeseq2/preprocessing.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)    37758 2023-06-01 08:36:08.000000 pydeseq2-0.3.4/pydeseq2/utils.py
+drwxr-xr-x   0 bmuzellec   (501) staff       (20)        0 2023-06-01 08:45:02.000000 pydeseq2-0.3.4/pydeseq2.egg-info/
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     6216 2023-06-01 08:45:02.000000 pydeseq2-0.3.4/pydeseq2.egg-info/PKG-INFO
+-rw-r--r--   0 bmuzellec   (501) staff       (20)      436 2023-06-01 08:45:02.000000 pydeseq2-0.3.4/pydeseq2.egg-info/SOURCES.txt
+-rw-r--r--   0 bmuzellec   (501) staff       (20)        1 2023-06-01 08:45:02.000000 pydeseq2-0.3.4/pydeseq2.egg-info/dependency_links.txt
+-rw-r--r--   0 bmuzellec   (501) staff       (20)      190 2023-06-01 08:45:02.000000 pydeseq2-0.3.4/pydeseq2.egg-info/requires.txt
+-rw-r--r--   0 bmuzellec   (501) staff       (20)        9 2023-06-01 08:45:02.000000 pydeseq2-0.3.4/pydeseq2.egg-info/top_level.txt
+-rw-r--r--   0 bmuzellec   (501) staff       (20)      408 2023-04-05 09:20:58.000000 pydeseq2-0.3.4/pyproject.toml
+-rw-r--r--   0 bmuzellec   (501) staff       (20)       38 2023-06-01 08:45:02.000000 pydeseq2-0.3.4/setup.cfg
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     1362 2023-05-02 08:07:48.000000 pydeseq2-0.3.4/setup.py
+drwxr-xr-x   0 bmuzellec   (501) staff       (20)        0 2023-06-01 08:45:02.000000 pydeseq2-0.3.4/tests/
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     5654 2023-02-16 10:34:42.000000 pydeseq2-0.3.4/tests/test_docstring.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)    11990 2023-06-01 08:36:10.000000 pydeseq2-0.3.4/tests/test_edge_cases.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)    15867 2023-06-01 08:36:08.000000 pydeseq2-0.3.4/tests/test_pydeseq2.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     1951 2023-02-21 15:32:02.000000 pydeseq2-0.3.4/tests/test_utils.py
```

### Comparing `pydeseq2-0.3.3/LICENSE` & `pydeseq2-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydeseq2-0.3.3/PKG-INFO` & `pydeseq2-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydeseq2
-Version: 0.3.3
+Version: 0.3.4
 Summary: A python implementation of DESeq2.
 Author: Boris Muzellec, Maria Telenczuk, Vincent Cabelli and Mathieu Andreux
 Author-email: boris.muzellec@owkin.com
 License: MIT
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -41,26 +41,35 @@
 
 Currently, available features broadly correspond to the default settings of DESeq2 (v1.34.0) for single-factor 
 and paired multi-factor analysis (with categorical factors), but we plan to implement more in the future.
 In case there is a feature you would particularly like to be implemented, feel free to open an issue.
 
 ## Installation
 
-`PyDESeq2` can be installed from PyPI:
+### PyPI
+
+`PyDESeq2` can be installed from PyPI using `pip`:
 
 `pip install pydeseq2`
 
 We recommend installing within a conda environment:
 
 ```
 conda create -n pydeseq2
 conda activate pydeseq2
+conda install pip
 pip install pydeseq2
 ```
 
+### Bioconda
+
+`PyDESeq2` can also be installed from Bioconda with `conda`:
+
+`conda install -c bioconda pydeseq2`
+
 If you're interested in contributing or want access to the development version, please see the [contributing](#contributing) section.
 
 ### Requirements
 
 The list of package version requirements is available in `setup.py`.
 
 For reference, the code is being tested in a github workflow (CI) with python
@@ -104,15 +113,15 @@
 
 ### 1 - Download the repository
 
 `git clone https://github.com/owkin/PyDESeq2.git`
 
 ### 2 - Create a conda environment
 
-Run `conda env create -n pydeseq2 python=3.8` (or higher python version) to create the `pydeseq2` environment and then activate it:
+Run `conda create -n pydeseq2 python=3.8` (or higher python version) to create the `pydeseq2` environment and then activate it:
 `conda activate pydeseq2`.
 
 `cd` to the root of the repo and run `pip install -e ."[dev]"` to install in developer mode.
 
 Then, run `pre-commit install`.
 
 The `pre-commit` tool will automatically run [black](https://black.readthedocs.io/en/stable/)
```

### Comparing `pydeseq2-0.3.3/README.md` & `pydeseq2-0.3.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -29,26 +29,35 @@
 
 Currently, available features broadly correspond to the default settings of DESeq2 (v1.34.0) for single-factor 
 and paired multi-factor analysis (with categorical factors), but we plan to implement more in the future.
 In case there is a feature you would particularly like to be implemented, feel free to open an issue.
 
 ## Installation
 
-`PyDESeq2` can be installed from PyPI:
+### PyPI
+
+`PyDESeq2` can be installed from PyPI using `pip`:
 
 `pip install pydeseq2`
 
 We recommend installing within a conda environment:
 
 ```
 conda create -n pydeseq2
 conda activate pydeseq2
+conda install pip
 pip install pydeseq2
 ```
 
+### Bioconda
+
+`PyDESeq2` can also be installed from Bioconda with `conda`:
+
+`conda install -c bioconda pydeseq2`
+
 If you're interested in contributing or want access to the development version, please see the [contributing](#contributing) section.
 
 ### Requirements
 
 The list of package version requirements is available in `setup.py`.
 
 For reference, the code is being tested in a github workflow (CI) with python
@@ -92,15 +101,15 @@
 
 ### 1 - Download the repository
 
 `git clone https://github.com/owkin/PyDESeq2.git`
 
 ### 2 - Create a conda environment
 
-Run `conda env create -n pydeseq2 python=3.8` (or higher python version) to create the `pydeseq2` environment and then activate it:
+Run `conda create -n pydeseq2 python=3.8` (or higher python version) to create the `pydeseq2` environment and then activate it:
 `conda activate pydeseq2`.
 
 `cd` to the root of the repo and run `pip install -e ."[dev]"` to install in developer mode.
 
 Then, run `pre-commit install`.
 
 The `pre-commit` tool will automatically run [black](https://black.readthedocs.io/en/stable/)
```

### Comparing `pydeseq2-0.3.3/pydeseq2/dds.py` & `pydeseq2-0.3.4/pydeseq2/dds.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import statsmodels.api as sm  # type: ignore
 from joblib import Parallel  # type: ignore
 from joblib import delayed
 from joblib import parallel_backend
 from scipy.optimize import minimize
 from scipy.special import polygamma  # type: ignore
 from scipy.stats import f  # type: ignore
+from scipy.stats import trim_mean  # type: ignore
 from statsmodels.tools.sm_exceptions import DomainWarning  # type: ignore
 
 from pydeseq2.preprocessing import deseq2_norm
 from pydeseq2.utils import build_design_matrix
 from pydeseq2.utils import dispersion_trend
 from pydeseq2.utils import fit_alpha_mle
 from pydeseq2.utils import fit_lin_mu
@@ -171,29 +172,36 @@
         min_replicates: int = 7,
         beta_tol: float = 1e-8,
         n_cpus: Optional[int] = None,
         batch_size: int = 128,
         joblib_verbosity: int = 0,
     ) -> None:
 
-        if adata is None and (counts is None or clinical is None):
-            raise ValueError(
-                "Either adata or both counts and clinical arguments must be provided."
-            )
-
         # Initialize the AnnData part
         if adata is not None:
+            if counts is not None:
+                warnings.warn(
+                    "adata was provided; ignoring counts.", UserWarning, stacklevel=2
+                )
+            if clinical is not None:
+                warnings.warn(
+                    "adata was provided; ignoring clinical.", UserWarning, stacklevel=2
+                )
             # Test counts before going further
             test_valid_counts(adata.X)
             # Copy fields from original AnnData
             self.__dict__.update(adata.__dict__)
-        else:
+        elif counts is not None and clinical is not None:
             # Test counts before going further
             test_valid_counts(counts)
-            super().__init__(X=counts, obs=clinical, dtype=int)
+            super().__init__(X=counts.astype(int), obs=clinical)
+        else:
+            raise ValueError(
+                "Either adata or both counts and clinical arguments must be provided."
+            )
 
         # Convert design_factors to list if a single string was provided.
         self.design_factors = (
             [design_factors] if isinstance(design_factors, str) else design_factors
         )
         if self.obs[self.design_factors].isna().any().any():
             raise ValueError("NaNs are not allowed in the design factors.")
@@ -205,35 +213,47 @@
             clinical_df=self.obs,
             design_factors=self.design_factors,
             ref_level=ref_level,
             expanded=False,
             intercept=True,
         )
 
+        # Check that the design matrix has full rank
+        self._check_full_rank_design()
+
         self.min_mu = min_mu
         self.min_disp = min_disp
         self.max_disp = np.maximum(max_disp, self.n_obs)
         self.refit_cooks = refit_cooks
         self.min_replicates = min_replicates
         self.beta_tol = beta_tol
         self.n_processes = get_num_processes(n_cpus)
         self.batch_size = batch_size
         self.joblib_verbosity = joblib_verbosity
 
-    def vst(self, use_design: bool = False) -> None:
+    def vst(
+        self,
+        use_design: bool = False,
+        fit_type: Literal["parametric", "mean"] = "parametric",
+    ) -> None:
         """
         Fit a variance stabilizing transformation, and apply it to normalized counts.
 
         Results are stored in ``dds.layers["vst_counts"]``.
 
         Parameters
         ----------
         use_design : bool
             Whether to use the full design matrix to fit dispersions and the trend curve.
             If False, only an intercept is used. (default: ``False``).
+        fit_type : str
+            Either "parametric" or "mean" for the type of fitting of dispersions to the
+            mean intensity. parametric - fit a dispersion-mean relation via a robust
+            gamma-family GLM. mean - use the mean of gene-wise dispersion estimates.
+            (default: ``"parametric"``).
         """
 
         # Start by fitting median-of-ratio size factors, if not already present.
         if "size_factors" not in self.obsm:
             self.fit_size_factors()
 
         if use_design:
@@ -245,27 +265,42 @@
             # Reduce the design matrix to an intercept and reconstruct at the end
             self.obsm["design_matrix_buffer"] = self.obsm["design_matrix"].copy()
             self.obsm["design_matrix"] = pd.DataFrame(
                 1, index=self.obs_names, columns=[["intercept"]]
             )
             # Fit the trend curve with an intercept design
             self.fit_genewise_dispersions()
-            self.fit_dispersion_trend()
+            if fit_type == "parametric":
+                self.fit_dispersion_trend()
 
             # Restore the design matrix and free buffer
             self.obsm["design_matrix"] = self.obsm["design_matrix_buffer"].copy()
             del self.obsm["design_matrix_buffer"]
 
         # Apply VST
-        a0, a1 = self.uns["trend_coeffs"]
-        cts = self.layers["normed_counts"]
-        self.layers["vst_counts"] = np.log2(
-            (1 + a1 + 2 * a0 * cts + 2 * np.sqrt(a0 * cts * (1 + a1 + a0 * cts)))
-            / (4 * a0)
-        )
+        if fit_type == "parametric":
+            a0, a1 = self.uns["trend_coeffs"]
+            cts = self.layers["normed_counts"]
+            self.layers["vst_counts"] = np.log2(
+                (1 + a1 + 2 * a0 * cts + 2 * np.sqrt(a0 * cts * (1 + a1 + a0 * cts)))
+                / (4 * a0)
+            )
+        elif fit_type == "mean":
+            gene_dispersions = self.varm["genewise_dispersions"]
+            use_for_mean = gene_dispersions > 10 * self.min_disp
+            mean_disp = trim_mean(gene_dispersions[use_for_mean], proportiontocut=0.001)
+            self.layers["vst_counts"] = (
+                2 * np.arcsinh(np.sqrt(mean_disp * self.layers["normed_counts"]))
+                - np.log(mean_disp)
+                - np.log(4)
+            ) / np.log(2)
+        else:
+            raise NotImplementedError(
+                f"Found fit_type '{fit_type}'. Expected 'parametric' or 'mean'."
+            )
 
     def deseq2(self) -> None:
         """Perform dispersion and log fold-change (LFC) estimation.
 
         Wrapper for the first part of the PyDESeq2 pipeline.
         """
 
@@ -958,7 +993,19 @@
 
         # Restore the design matrix and free buffer
         self.obsm["design_matrix"] = self.obsm["design_matrix_buffer"].copy()
         del self.obsm["design_matrix_buffer"]
 
         # Store normalized counts
         self.layers["normed_counts"] = self.X / self.obsm["size_factors"][:, None]
+
+    def _check_full_rank_design(self):
+        """Check that the design matrix has full column rank."""
+        rank = np.linalg.matrix_rank(self.obsm["design_matrix"])
+        num_vars = self.obsm["design_matrix"].shape[1]
+
+        if rank < num_vars:
+            raise ValueError(
+                "The design matrix is not full rank, so the model cannot be "
+                "fitted. Please remove the design variables that are linear "
+                "combinations of others."
+            )
```

### Comparing `pydeseq2-0.3.3/pydeseq2/ds.py` & `pydeseq2-0.3.4/pydeseq2/ds.py`

 * *Files 7% similar despite different names*

```diff
@@ -263,33 +263,60 @@
 
         # Account for possible all_zeroes due to outlier refitting in DESeqDataSet
         if self.dds.refit_cooks and self.dds.varm["replaced"].sum() > 0:
             self.SE.loc[self.dds.new_all_zeroes_genes] = 0.0
             self.statistics.loc[self.dds.new_all_zeroes_genes] = 0.0
             self.p_values.loc[self.dds.new_all_zeroes_genes] = 1.0
 
-    def lfc_shrink(self, coeff: str) -> None:
+    def lfc_shrink(self, coeff: Optional[str] = None) -> None:
         """LFC shrinkage with an apeGLM prior :cite:p:`DeseqStats-zhu2019heavy`.
 
         Shrinks LFCs using a heavy-tailed Cauchy prior, leaving p-values unchanged.
 
         Parameters
         ----------
-        coeff : str
-            The LFC coefficient to shrink.
+        coeff : str or None
+            The LFC coefficient to shrink. If set to ``None``, the method will try to
+            shrink the coefficient corresponding to the ``contrast`` attribute.
             If the desired coefficient is not available, it may be set from the
             :class:`pydeseq2.dds.DeseqDataSet` argument ``ref_level``.
+            (default: ``None``).
         """
 
-        if coeff not in self.LFC.columns:
+        contrast_level = f"{self.contrast[0]}_{self.contrast[1]}_vs_{self.contrast[2]}"
+
+        if coeff is not None:
+            if coeff not in self.LFC.columns:
+                split_coeff = coeff.split("_")
+                if len(split_coeff) == 4:
+                    raise KeyError(
+                        f"The coeff argument '{coeff}' should be one the LFC columns. "
+                        f"The available LFC coeffs are {self.LFC.columns[1:]}. "
+                        f"If the desired coefficient is not available, please set "
+                        f"`ref_level = [{split_coeff[0]}, {split_coeff[3]}]` "
+                        f"in DeseqDataSet and rerun."
+                    )
+                else:
+                    raise KeyError(
+                        f"The coeff argument '{coeff}' should be one the LFC columns. "
+                        f"The available LFC coeffs are {self.LFC.columns[1:]}. "
+                        f"If the desired coefficient is not available, please set the "
+                        f"appropriate`ref_level` in DeseqDataSet and rerun."
+                    )
+        elif contrast_level not in self.LFC.columns:
             raise KeyError(
-                f"The coeff argument ('{coeff}') should be one the LFC columns. "
-                f"If not available,  it can be set from DeseqDataSet's `ref_level` "
-                f"argument."
+                f"lfc_shrink's coeff argument was set to None, but the coefficient "
+                f"corresponding to the contrast {self.contrast} is not available."
+                f"The available LFC coeffs are {self.LFC.columns[1:]}. "
+                f"If the desired coefficient is not available, please set "
+                f"`ref_level = [{self.contrast[0]}, {self.contrast[2]}]` "
+                f"in DeseqDataSet and rerun."
             )
+        else:
+            coeff = contrast_level
 
         coeff_idx = self.LFC.columns.get_loc(coeff)
 
         size = 1.0 / self.dds.varm["dispersions"]
         offset = np.log(self.dds.obsm["size_factors"])
 
         # Set priors
@@ -352,17 +379,22 @@
         self.shrunk_LFCs = True
 
         # Replace in results dataframe, if it exists
         if hasattr(self, "results_df"):
             self.results_df["log2FoldChange"] = self.LFC.iloc[:, coeff_idx] / np.log(2)
             self.results_df["lfcSE"] = self.SE / np.log(2)
 
+            # Get the corrresponding factor, tested and reference levels of the shrunk
+            # coefficient
+            split_coeff = coeff.split("_")
+            # coeffs are of the form "factor_A_vs_B", hence "factor" is split_coeff[0],
+            # "A" is split_coeff[1] and "B" split_coeff[3]
             print(
                 f"Shrunk Log2 fold change & Wald test p-value: "
-                f"{self.contrast[0]} {self.contrast[1]} vs {self.contrast[2]}"
+                f"{split_coeff[0]} {split_coeff[1]} vs {split_coeff[3]}"
             )
 
             display(self.results_df)
 
     def _independent_filtering(self) -> None:
         """Compute adjusted p-values using independent filtering.
```

### Comparing `pydeseq2-0.3.3/pydeseq2/grid_search.py` & `pydeseq2-0.3.4/pydeseq2/grid_search.py`

 * *Files identical despite different names*

### Comparing `pydeseq2-0.3.3/pydeseq2/preprocessing.py` & `pydeseq2-0.3.4/pydeseq2/preprocessing.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 from typing import Tuple
+from typing import Union
 
 import numpy as np
 import pandas as pd
 
 
-def deseq2_norm(counts: pd.DataFrame) -> Tuple[pd.DataFrame, pd.DataFrame]:
+def deseq2_norm(
+    counts: Union[pd.DataFrame, np.ndarray]
+) -> Tuple[Union[pd.DataFrame, np.ndarray], Union[pd.DataFrame, np.ndarray]]:
     """
     Return normalized counts and size_factors.
 
     Uses the median of ratios method.
 
     Parameters
     ----------
-    counts : ndarray
+    counts : pandas.DataFrame or ndarray
             Raw counts. One column per gene, one row per sample.
 
     Returns
     -------
-    deseq2_counts : pandas.DataFrame
+    deseq2_counts : pandas.DataFrame or ndarray
         DESeq2 normalized counts.
         One column per gene, rows are indexed by sample barcodes.
 
-    size_factors : pandas.DataFrame
+    size_factors : pandas.DataFrame or ndarray
         DESeq2 normalization factors.
     """
 
     # Compute gene-wise mean log counts
     with np.errstate(divide="ignore"):  # ignore division by zero warnings
         log_counts = np.log(counts)
     logmeans = log_counts.mean(0)
     # Filter out genes with -∞ log means
     filtered_genes = ~np.isinf(logmeans)
     # Subtract filtered log means from log counts
-    log_ratios = log_counts[:, filtered_genes] - logmeans[filtered_genes]
+    if isinstance(log_counts, pd.DataFrame):
+        log_ratios = log_counts.loc[:, filtered_genes] - logmeans[filtered_genes]
+    else:
+        log_ratios = log_counts[:, filtered_genes] - logmeans[filtered_genes]
     # Compute sample-wise median of log ratios
     log_medians = np.median(log_ratios, axis=1)
     # Return raw counts divided by size factors (exponential of log ratios)
     # and size factors
     size_factors = np.exp(log_medians)
     deseq2_counts = counts / size_factors[:, None]
     return deseq2_counts, size_factors
```

### Comparing `pydeseq2-0.3.3/pydeseq2/utils.py` & `pydeseq2-0.3.4/pydeseq2/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -459,14 +459,17 @@
 
     # if full rank, estimate initial betas for IRLS below
     if np.linalg.matrix_rank(X) == num_vars:
         Q, R = np.linalg.qr(X)
         y = np.log(counts / size_factors + 0.1)
         beta_init = solve(R, Q.T @ y)
         beta = beta_init
+    else:  # Initialise intercept with log base mean
+        beta = np.zeros(num_vars)
+        beta[0] = np.log(counts / size_factors).mean()
 
     dev = 1000.0
     dev_ratio = 1.0
 
     ridge_factor = np.diag(np.repeat(1e-6, num_vars))
     mu = np.maximum(size_factors * np.exp(X @ beta), min_mu)
```

### Comparing `pydeseq2-0.3.3/pydeseq2.egg-info/PKG-INFO` & `pydeseq2-0.3.4/pydeseq2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydeseq2
-Version: 0.3.3
+Version: 0.3.4
 Summary: A python implementation of DESeq2.
 Author: Boris Muzellec, Maria Telenczuk, Vincent Cabelli and Mathieu Andreux
 Author-email: boris.muzellec@owkin.com
 License: MIT
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -41,26 +41,35 @@
 
 Currently, available features broadly correspond to the default settings of DESeq2 (v1.34.0) for single-factor 
 and paired multi-factor analysis (with categorical factors), but we plan to implement more in the future.
 In case there is a feature you would particularly like to be implemented, feel free to open an issue.
 
 ## Installation
 
-`PyDESeq2` can be installed from PyPI:
+### PyPI
+
+`PyDESeq2` can be installed from PyPI using `pip`:
 
 `pip install pydeseq2`
 
 We recommend installing within a conda environment:
 
 ```
 conda create -n pydeseq2
 conda activate pydeseq2
+conda install pip
 pip install pydeseq2
 ```
 
+### Bioconda
+
+`PyDESeq2` can also be installed from Bioconda with `conda`:
+
+`conda install -c bioconda pydeseq2`
+
 If you're interested in contributing or want access to the development version, please see the [contributing](#contributing) section.
 
 ### Requirements
 
 The list of package version requirements is available in `setup.py`.
 
 For reference, the code is being tested in a github workflow (CI) with python
@@ -104,15 +113,15 @@
 
 ### 1 - Download the repository
 
 `git clone https://github.com/owkin/PyDESeq2.git`
 
 ### 2 - Create a conda environment
 
-Run `conda env create -n pydeseq2 python=3.8` (or higher python version) to create the `pydeseq2` environment and then activate it:
+Run `conda create -n pydeseq2 python=3.8` (or higher python version) to create the `pydeseq2` environment and then activate it:
 `conda activate pydeseq2`.
 
 `cd` to the root of the repo and run `pip install -e ."[dev]"` to install in developer mode.
 
 Then, run `pre-commit install`.
 
 The `pre-commit` tool will automatically run [black](https://black.readthedocs.io/en/stable/)
```

### Comparing `pydeseq2-0.3.3/setup.py` & `pydeseq2-0.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     description="A python implementation of DESeq2.",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Boris Muzellec, Maria Telenczuk, Vincent Cabelli and Mathieu Andreux",
     author_email="boris.muzellec@owkin.com",
     packages=find_packages(exclude=["tests*"]),
     install_requires=[
-        "anndata==0.8.0",
-        "jupyter",
+        "anndata>=0.8.0",
+        "ipython",
         "numpy>=1.23.0",
         "pandas>=1.4.0",
         "scikit-learn>=1.1.0",
         "scipy>=1.8.0",
         "statsmodels",
         "matplotlib>=3.6.2",  # not sure why sphinx_gallery does not work without it
     ],  # external packages as dependencies
```

### Comparing `pydeseq2-0.3.3/tests/test_docstring.py` & `pydeseq2-0.3.4/tests/test_docstring.py`

 * *Files identical despite different names*

### Comparing `pydeseq2-0.3.3/tests/test_edge_cases.py` & `pydeseq2-0.3.4/tests/test_edge_cases.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,24 +112,40 @@
     clinical_df = pd.DataFrame({"condition": [0, np.NaN]}, index=["sample1", "sample2"])
 
     with pytest.raises(ValueError):
         DeseqDataSet(counts=counts_df, clinical=clinical_df, design_factors="condition")
 
 
 def test_one_factor():
-    """Test that a ValueError is thrown when the design factor takes only one value ."""
+    """Test that a ValueError is thrown when the design factor takes only one value."""
     counts_df = pd.DataFrame(
         {"gene1": [0, 1], "gene2": [4, 12]}, index=["sample1", "sample2"]
     )
     clinical_df = pd.DataFrame({"condition": [0, 0]}, index=["sample1", "sample2"])
 
     with pytest.raises(ValueError):
         DeseqDataSet(counts=counts_df, clinical=clinical_df, design_factors="condition")
 
 
+def test_rank_deficient_design():
+    """Test that a ValueError is thrown when the design matrix does not have full column
+    rank."""
+    counts_df = pd.DataFrame(
+        {"gene1": [0, 1], "gene2": [4, 12]}, index=["sample1", "sample2"]
+    )
+    clinical_df = pd.DataFrame(
+        {"condition": [0, 1], "batch": ["A", "B"]}, index=["sample1", "sample2"]
+    )
+
+    with pytest.raises(ValueError):
+        DeseqDataSet(
+            counts=counts_df, clinical=clinical_df, design_factors=["condition", "batch"]
+        )
+
+
 def test_reference_level():
     """Test that a ValueError is thrown when the reference level is not one of the
     design factor values."""
     counts_df = pd.DataFrame(
         {"gene1": [0, 1], "gene2": [4, 12]}, index=["sample1", "sample2"]
     )
     clinical_df = pd.DataFrame({"condition": [0, 1]}, index=["sample1", "sample2"])
@@ -141,15 +157,15 @@
             design_factors="condition",
             ref_level="control",
         )
 
 
 def test_lfc_shrinkage_coeff():
     """Test that a KeyError is thrown when attempting to shrink an unexisting LFC
-    coefficient.
+    coefficient, but that setting coeff=None runs bug-free.
     """
 
     counts_df = load_example_data(
         modality="raw_counts",
         dataset="synthetic",
         debug=False,
     )
@@ -161,18 +177,30 @@
     )
 
     dds = DeseqDataSet(
         counts=counts_df, clinical=clinical_df, design_factors="condition"
     )
     dds.deseq2()
 
-    res = DeseqStats(dds)
-    res.summary()
+    # Check that coeff=None gives the same results as the default
+    # coefficient condition_B_vs_A
+    res_1 = DeseqStats(dds)
+    res_1.summary()
+    res_1.lfc_shrink(coeff=None)
+    shrunk_lfcs_1 = res_1.results_df["log2FoldChange"].copy()
+
+    res_2 = DeseqStats(dds)
+    res_2.summary()
+    res_2.lfc_shrink(coeff="condition_B_vs_A")
+    shrunk_lfcs_2 = res_2.results_df["log2FoldChange"].copy()
+
+    assert (shrunk_lfcs_1 == shrunk_lfcs_2).all()
+
     with pytest.raises(KeyError):
-        res.lfc_shrink(coeff="this_coeff_does_not_exist")
+        res_1.lfc_shrink(coeff="this_coeff_does_not_exist")
 
 
 def test_indexes():
     """Test that a ValueError is thrown when the count matrix and the clinical data
     don't have the same index."""
     counts_df = pd.DataFrame(
         {"gene1": [0, 1], "gene2": [4, 12]}, index=["sample1", "sample2"]
```

### Comparing `pydeseq2-0.3.3/tests/test_pydeseq2.py` & `pydeseq2-0.3.4/tests/test_pydeseq2.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import anndata as ad
 import numpy as np
 import pandas as pd
 
 import tests
 from pydeseq2.dds import DeseqDataSet
 from pydeseq2.ds import DeseqStats
+from pydeseq2.preprocessing import deseq2_norm
 from pydeseq2.utils import load_example_data
 
 # Single-factor tests
 
 
 def test_deseq(tol=0.02):
     """Test that the outputs of the DESeq2 function match those of the original R
@@ -362,15 +363,15 @@
     clinical_df = load_example_data(
         modality="clinical",
         dataset="synthetic",
         debug=False,
     )
 
     # Make an anndata object
-    adata = ad.AnnData(X=counts_df, obs=clinical_df, dtype=int)
+    adata = ad.AnnData(X=counts_df.astype(int), obs=clinical_df)
 
     # Put some dummy data in unused fields
     adata.obsm["dummy_metadata"] = np.random.choice(2, adata.n_obs)
     adata.varm["dummy_param"] = np.random.randn(adata.n_vars)
 
     # Put values in the dispersions field
     adata.varm["dispersions"] = np.random.randn(adata.n_vars) ** 2
@@ -444,14 +445,47 @@
     )
     dds.vst(use_design=True)
     assert (
         np.abs(r_vst_with_design - dds.layers["vst_counts"]) / r_vst_with_design
     ).max().max() < tol
 
 
+def test_mean_vst(tol=0.02):
+    """
+    Test the output of VST with ``fitType="mean"`` compared with DESeq2.
+    """
+
+    # Load data
+    counts_df = load_example_data(
+        modality="raw_counts",
+        dataset="synthetic",
+        debug=False,
+    )
+
+    clinical_df = load_example_data(
+        modality="clinical",
+        dataset="synthetic",
+        debug=False,
+    )
+
+    # Load R data
+    test_path = str(Path(os.path.realpath(tests.__file__)).parent.resolve())
+
+    r_vst = pd.read_csv(
+        os.path.join(test_path, "data/single_factor/r_mean_vst.csv"), index_col=0
+    ).T
+
+    # Test blind design
+    dds = DeseqDataSet(
+        counts=counts_df, clinical=clinical_df, design_factors=["condition"]
+    )
+    dds.vst(use_design=False, fit_type="mean")
+    assert (np.abs(r_vst - dds.layers["vst_counts"]) / r_vst).max().max() < tol
+
+
 def test_ref_level():
     """Test that DeseqDataSet columns are created according to the passed reference
     level, if any.
     """
     counts_df = load_example_data(
         modality="raw_counts",
         dataset="synthetic",
@@ -476,7 +510,38 @@
     # Check that its content is correct
     assert (
         dds.obsm["design_matrix"]["group_X_vs_Y"]
         == clinical_df["group"].apply(
             lambda x: 1 if x == "X" else 0 if x == "Y" else np.NaN
         )
     ).all()
+
+
+def test_deseq2_norm():
+    """Test that deseq2_norm() called on a pandas dataframe outputs the same results as
+    DeseqDataSet.fit_size_factors()
+    """
+    counts_df = load_example_data(
+        modality="raw_counts",
+        dataset="synthetic",
+        debug=False,
+    )
+
+    clinical_df = load_example_data(
+        modality="clinical",
+        dataset="synthetic",
+        debug=False,
+    )
+
+    # Fit size factors from DeseqDataSet
+    dds = DeseqDataSet(counts=counts_df, clinical=clinical_df)
+    dds.fit_size_factors()
+    s1 = dds.obsm["size_factors"]
+
+    # Fit size factors from counts directly
+    s2 = deseq2_norm(counts_df)[1]
+
+    np.testing.assert_almost_equal(
+        s1,
+        s2,
+        decimal=8,
+    )
```

### Comparing `pydeseq2-0.3.3/tests/test_utils.py` & `pydeseq2-0.3.4/tests/test_utils.py`

 * *Files identical despite different names*

