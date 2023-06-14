# Comparing `tmp/absplit-1.1.0.tar.gz` & `tmp/absplit-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "absplit-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "absplit-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `absplit-1.1.0.tar` & `absplit-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     4958 2023-06-05 23:23:06.124000 absplit-1.1.0/.gitignore
--rw-r--r--   0        0        0       50 2023-02-18 09:46:26.039000 absplit-1.1.0/.idea/.gitignore
--rw-r--r--   0        0        0      331 2023-06-12 08:10:41.536000 absplit-1.1.0/.idea/genetic_algorithm.iml
--rw-r--r--   0        0        0      179 2023-02-18 09:46:26.072000 absplit-1.1.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      305 2023-06-12 08:10:39.408000 absplit-1.1.0/.idea/misc.xml
--rw-r--r--   0        0        0      293 2023-02-18 09:46:26.093000 absplit-1.1.0/.idea/modules.xml
--rw-r--r--   0        0        0      185 2023-02-18 09:46:26.104000 absplit-1.1.0/.idea/vcs.xml
--rw-r--r--   0        0        0     1026 2023-02-18 09:46:26.114000 absplit-1.1.0/LICENSE
--rw-r--r--   0        0        0      152 2023-02-18 09:46:26.124000 absplit-1.1.0/MANIFEST.in
--rw-r--r--   0        0        0     7015 2023-06-12 08:39:50.161000 absplit-1.1.0/README.md
--rw-r--r--   0        0        0       62 2023-06-12 08:39:50.092000 absplit-1.1.0/absplit/__init__.py
--rw-r--r--   0        0        0     8275 2023-06-11 11:49:29.241000 absplit-1.1.0/absplit/data.py
--rw-r--r--   0        0        0    23169 2023-06-12 08:36:15.539000 absplit-1.1.0/absplit/ga.py
--rw-r--r--   0        0        0     1866 2023-02-18 09:46:26.177000 absplit-1.1.0/absplit/param.py
--rw-r--r--   0        0        0    29186 2023-02-18 09:46:26.190000 absplit-1.1.0/images/logo.jpeg
--rw-r--r--   0        0        0     1531 2023-06-12 08:39:50.213000 absplit-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       50 2023-06-05 23:23:06.260000 absplit-1.1.0/requirements.txt
--rw-r--r--   0        0        0        0 2023-02-18 09:46:26.220000 absplit-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0     5925 2023-02-18 09:46:26.238000 absplit-1.1.0/tests/test_data.py
--rw-r--r--   0        0        0     2125 2023-06-12 08:32:24.989000 absplit-1.1.0/tests/test_ga.py
--rw-r--r--   0        0        0     8064 1970-01-01 00:00:00.000000 absplit-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4958 2023-06-05 23:23:06.124000 absplit-1.2.0/.gitignore
+-rw-r--r--   0        0        0       50 2023-02-18 09:46:26.039000 absplit-1.2.0/.idea/.gitignore
+-rw-r--r--   0        0        0      291 2023-06-12 08:40:13.087000 absplit-1.2.0/.idea/genetic_algorithm.iml
+-rw-r--r--   0        0        0      179 2023-02-18 09:46:26.072000 absplit-1.2.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      303 2023-06-12 08:40:13.168000 absplit-1.2.0/.idea/misc.xml
+-rw-r--r--   0        0        0      293 2023-02-18 09:46:26.093000 absplit-1.2.0/.idea/modules.xml
+-rw-r--r--   0        0        0      185 2023-02-18 09:46:26.104000 absplit-1.2.0/.idea/vcs.xml
+-rw-r--r--   0        0        0     1026 2023-02-18 09:46:26.114000 absplit-1.2.0/LICENSE
+-rw-r--r--   0        0        0      152 2023-02-18 09:46:26.124000 absplit-1.2.0/MANIFEST.in
+-rw-r--r--   0        0        0     7387 2023-06-14 16:57:57.554000 absplit-1.2.0/README.md
+-rw-r--r--   0        0        0       62 2023-06-14 16:57:57.570000 absplit-1.2.0/absplit/__init__.py
+-rw-r--r--   0        0        0     8654 2023-06-14 16:57:57.585000 absplit-1.2.0/absplit/data.py
+-rw-r--r--   0        0        0    23681 2023-06-14 16:57:57.601000 absplit-1.2.0/absplit/ga.py
+-rw-r--r--   0        0        0     1866 2023-02-18 09:46:26.177000 absplit-1.2.0/absplit/param.py
+-rw-r--r--   0        0        0    29186 2023-02-18 09:46:26.190000 absplit-1.2.0/images/logo.jpeg
+-rw-r--r--   0        0        0     1531 2023-06-14 16:57:57.617000 absplit-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-06-05 23:23:06.260000 absplit-1.2.0/requirements.txt
+-rw-r--r--   0        0        0        0 2023-02-18 09:46:26.220000 absplit-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     5925 2023-02-18 09:46:26.238000 absplit-1.2.0/tests/test_data.py
+-rw-r--r--   0        0        0     2125 2023-06-12 08:32:24.989000 absplit-1.2.0/tests/test_ga.py
+-rw-r--r--   0        0        0     8425 1970-01-01 00:00:00.000000 absplit-1.2.0/PKG-INFO
```

### Comparing `absplit-1.1.0/.gitignore` & `absplit-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `absplit-1.1.0/LICENSE` & `absplit-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `absplit-1.1.0/README.md` & `absplit-1.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg" width="460" height="140">
 <h3><strong>ABSplit</strong></h3>
 Split your data into matching A/B/n groups
 
 ![license](https://img.shields.io/badge/License-MIT-blue.svg)
-![version](https://img.shields.io/badge/version-1.1.0-blue.svg)
+![version](https://img.shields.io/badge/version-1.2.0-blue.svg)
 ![version](https://img.shields.io/badge/python-3-orange.svg)
 
 </div>
 
 <details open>
   <summary>Table of Contents</summary>
   <ol>
@@ -114,16 +114,25 @@
 
 # Visualise generation fitness
 ab.fitness()
 
 # Visualise data
 ab.visualise()
 
-# Extract results
+# Extract bin splits
 df = ab.results
+
+# Extract distributions summary
+df_dist = ab.distributions
+
+# Extract data aggregated by bins
+df_agg = ab.aggregations
+
+# Extract RMSE summary
+df_rmse = ab.rmse
 ```
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ## API Reference
 ### Absplit 
 `ABSplit(df, metrics, splitting, date_col=None, ga_params={}, metric_weights={}, splits=[0.5, 0.5], size_penalty=0)`
 
@@ -138,14 +147,16 @@
 * `ga_params` (dict, optional): Parameters for the genetic algorithm `pygad.GA` module parameters, see 
 [here](https://pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html#pygad-ga-class) for arguments you can pass
 (default: `{}`)
 * `splits` (list, optional): How many groups to split into, and relative size of the groups (default: `[0.5, 0.5]`,
 2 groups of equal size)
 * `size_penalty` (float, optional): Penalty weighting for differences in the population count between groups 
 (default: `0`)
+* `cutoff_date` (str, optional): Cutoff date between fitting and validation data. If `None`, it will fit on all 
+available data. If cutoff date provided, RMSE scores will be for validation period
 * `metric_weights` (dict, optional): Weights for each metric in the data. If you want the splitting to focus on 
 one metrics more than the other, you can prioritise this here (default: `{}`)
 
 
 ### Match 
 `Match(population, sample, metrics, splitting, date_col=None, ga_params={}, metric_weights={})`
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 [https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg]
                                **** ABSplit ****
  Split your data into matching A/B/n groups ![license](https://img.shields.io/
  badge/License-MIT-blue.svg) ![version](https://img.shields.io/badge/version-
- 1.1.0-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
+ 1.2.0-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
  Table of Contents
    1. About_The_Project
    2. Getting_Started
           o Installation
    3. Tutorials
           o Do_it_yourself
    4. Usage
@@ -43,16 +43,18 @@
 'y']] for item in sublist] + ['x']*3, 'city': [item for sublist in [[x]*3 for x
 in ['a', 'b', 'c', 'd', 'e']] for item in sublist], 'metric1': np.arange(0, 15,
 1), 'metric2': np.arange(0, 150, 10) } df = pd.DataFrame(data_dct) # Identify
 which columns are metrics, which is the time period, and what to split on
 kwargs = { 'metrics': ['metric1', 'metric2'], 'date_col': 'date', 'splitting':
 'city' } # Initialise ab = ABSplit( df=df, split=[.5, .5], # Split into 2
 groups of equal size **kwargs, ) # Generate split ab.run() # Visualise
-generation fitness ab.fitness() # Visualise data ab.visualise() # Extract
-results df = ab.results ```
+generation fitness ab.fitness() # Visualise data ab.visualise() # Extract bin
+splits df = ab.results # Extract distributions summary df_dist =
+ab.distributions # Extract data aggregated by bins df_agg = ab.aggregations #
+Extract RMSE summary df_rmse = ab.rmse ```
                                                                   (back_to_top)
 ## API Reference ### Absplit `ABSplit(df, metrics, splitting, date_col=None,
 ga_params={}, metric_weights={}, splits=[0.5, 0.5], size_penalty=0)` Splits
 population into 2 groups. Mutually exclusive, completely exhaustive Arguments:
 * `df` (pd.DataFrame): Dataframe to be split * `metrics` (str, list): Name of,
 or list of names of, metric columns in DataFrame * `splitting` (str): Name of
 column that represents individuals in the population that is getting split *
@@ -61,34 +63,36 @@
 timeseries, (default `None`) * `ga_params` (dict, optional): Parameters for the
 genetic algorithm `pygad.GA` module parameters, see [here](https://
 pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html#pygad-ga-class)
 for arguments you can pass (default: `{}`) * `splits` (list, optional): How
 many groups to split into, and relative size of the groups (default: `[0.5,
 0.5]`, 2 groups of equal size) * `size_penalty` (float, optional): Penalty
 weighting for differences in the population count between groups (default: `0`)
-* `metric_weights` (dict, optional): Weights for each metric in the data. If
-you want the splitting to focus on one metrics more than the other, you can
-prioritise this here (default: `{}`) ### Match `Match(population, sample,
-metrics, splitting, date_col=None, ga_params={}, metric_weights={})` Takes
-DataFrame `sample` and finds a comparable group in `population`. Arguments: *
-`population` (pd.DataFrame): Population to search for comparable group (**Must
-exclude sample data**) * `sample` (pd.DataFrame): Sample we are looking to find
-a match for. * `metrics` (str, list): Name of, or list of names of, metric
-columns in DataFrame * `splitting` (str): Name of column that represents
-individuals in the population that is getting split * `date_col` (str,
-optional): Name of column that represents time periods, if applicable. If left
-empty, it will perform a static split, i.e. not across timeseries, (default
-`None`) * `ga_params` (dict, optional): Parameters for the genetic algorithm
-`pygad.GA` module parameters, see [here](https://pygad.readthedocs.io/en/
-latest/README_pygad_ReadTheDocs.html#pygad-ga-class) for arguments you can pass
-(default: `{}`) * `splits` (list, optional): How many groups to split into, and
-relative size of the groups (default: `[0.5, 0.5]`, 2 groups of equal size) *
-`metric_weights` (dict, optional): Weights for each metric in the data. If you
-want the splitting to focus on one metrics more than the other, you can
-prioritise this here (default: `{}`)
+* `cutoff_date` (str, optional): Cutoff date between fitting and validation
+data. If `None`, it will fit on all available data. If cutoff date provided,
+RMSE scores will be for validation period * `metric_weights` (dict, optional):
+Weights for each metric in the data. If you want the splitting to focus on one
+metrics more than the other, you can prioritise this here (default: `{}`) ###
+Match `Match(population, sample, metrics, splitting, date_col=None, ga_params=
+{}, metric_weights={})` Takes DataFrame `sample` and finds a comparable group
+in `population`. Arguments: * `population` (pd.DataFrame): Population to search
+for comparable group (**Must exclude sample data**) * `sample` (pd.DataFrame):
+Sample we are looking to find a match for. * `metrics` (str, list): Name of, or
+list of names of, metric columns in DataFrame * `splitting` (str): Name of
+column that represents individuals in the population that is getting split *
+`date_col` (str, optional): Name of column that represents time periods, if
+applicable. If left empty, it will perform a static split, i.e. not across
+timeseries, (default `None`) * `ga_params` (dict, optional): Parameters for the
+genetic algorithm `pygad.GA` module parameters, see [here](https://
+pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html#pygad-ga-class)
+for arguments you can pass (default: `{}`) * `splits` (list, optional): How
+many groups to split into, and relative size of the groups (default: `[0.5,
+0.5]`, 2 groups of equal size) * `metric_weights` (dict, optional): Weights for
+each metric in the data. If you want the splitting to focus on one metrics more
+than the other, you can prioritise this here (default: `{}`)
                                                                   (back_to_top)
 ## Contributing I welcome contributions to ABSplit! For major changes, please
 open an issue first to discuss what you would like to change. Please make sure
 to update tests as appropriate.
                                                                   (back_to_top)
 ## License [MIT](https://choosealicense.com/licenses/mit/)
                                                                   (back_to_top)
```

### Comparing `absplit-1.1.0/absplit/data.py` & `absplit-1.2.0/absplit/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,28 +42,30 @@
         _set_indexes(): Sets indexes for data passed
         _unstack(): Unstacks data by time periods (if applicable)
         _scale(): Scales the metrics
         filter(index): Uses index to filter dataframe
         assign(solution): Maps solution (binary numpy array) to unstacked dataframe index
     """
 
-    def __init__(self, df, scaler=None, scale=True, **kwargs):
+    def __init__(self, df, scaler=None, scale=True, cutoff_date=None, **kwargs):
         """Initializes the class and sets the attributes
 
         Args:
             df (pd.DataFrame): Dataframe to process
             scaler (object, optional): Scaling function object. Default None
             scale (bool, optional): To apply scaling to data or not. Default True
             **kwargs: Additional keyword arguments
         """
-
+        # print(f'data: {cutoff_date}')
         super().__init__(**kwargs)
         self._df_stacked = df
         self._pre_fit_scaler = scaler
         self._scaler_flag = scale
+        self._cutoff_date = cutoff_date
+
         self.remainder_cols = [x for x in self._df_stacked.columns if x not in self.all_spec_columns]
         self._df_unstacked = None
         self._df_index = None
         self.num_metrics = None
         self.time_periods = None
         self.pop_size = None
         self.splitting_values = None
@@ -134,17 +136,23 @@
 
     def _unstack(self):
         """Unstack date column if date columns is passed
 
         Returns:
             pd.DataFrame
         """
-
-        self._df_unstacked = self._df_unstacked.unstack(self.date_col, fill_value=0) if self.date_col \
-            else self._df_unstacked
+        df_unstacked = self._df_unstacked
+        if self.date_col and self._cutoff_date:
+            df_unstacked = df_unstacked[
+                df_unstacked.index.get_level_values(self.date_col) <= pd.to_datetime(self._cutoff_date)
+            ]
+
+        df_unstacked = df_unstacked.unstack(self.date_col, fill_value=0) if self.date_col \
+            else df_unstacked
+        self._df_unstacked = df_unstacked
 
     def _scale(self):
         """Standardise all metrics so all metrics weighted as equally as possible
 
         Returns:
             pd.DataFrame
         """
```

### Comparing `absplit-1.1.0/absplit/ga.py` & `absplit-1.2.0/absplit/ga.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,48 +153,52 @@
     Methods:
         _cost_weighting(): Modifies cost weighting array
         run(): Runs the genetic algorithm
         fitness(): Plot generation fitness graph
         visualise(): Plots metrics using results from genetic algorithm output
     """
 
-    def __init__(self, ga_params={}, metric_weights={}, runs=1, splits=[0.5, 0.5], size_penalty=1, **kwargs):
+    def __init__(self, ga_params={}, metric_weights={}, runs=1, splits=[0.5, 0.5], size_penalty=1, cutoff_date=None,
+                 **kwargs):
         """Initializes the class and sets the attributes
 
         Args:
             ga_params (dict, optional): Genetic algorithm parameters to add/modify
             metric_weights (dict, optional): Cost weightings to apply to metrics
             runs (int, optional): How many runs to try
             **kwargs: Additional keyword arguments
         """
         super().__init__(**kwargs)
         global size_penalty_global
         size_penalty_global = size_penalty
-
+        # print(cutoff_date)
         if ga_params:
             assert isinstance(ga_params, dict), 'ga_params must be a dictionary'
         self._runs = runs
         self._splits = splits
         self._splits_num = len(self._splits)
         self._ga_params = GAParams(splits=splits, **ga_params)
         self._best_score = -1
         self._metric_weights = metric_weights
+        self._cutoff_date = cutoff_date
         self._df = None
         self._population = None
         self._df_result = None  # Final results dataframe
         self._df_dist = None  # Group count distribution
         self._df_agg = None  # Group aggregated data
         self._ga = None  # Genetic algorithm instance
         self._df_vis = None  # Visualisation dataframe
         self._df_rmse = None  # RMSE between groups
         self._best_ga = None
         self._solution = None
 
         self._cost_weighting()
 
+        # print(self._cutoff_date)
+
     def _cost_weighting(self):
         """Set relative cost weights for each metric. Defaults to 1 unless specified.
 
         Used if you want the genetic algorithm to penalise the MSE cost of some metrics
         over others. Particularly useful if one metric is quite volatile, as the MSE cost can
         end up with it prioritising this over others.
 
@@ -285,30 +289,33 @@
 
     def _build_rmse(self):
         df_agg = self._df_agg.copy()
 
         if self.date_col is None:
             df_agg.index = [0]*df_agg.shape[0]
 
+        if self.date_col and self._cutoff_date:
+            df_agg = df_agg[
+                df_agg[self.date_col] > pd.to_datetime(self._cutoff_date)
+            ]
+
         df_ = df_agg.pivot(index=self.date_col, columns='bin', values=self.metrics)
         df_.columns = df_.columns.map('_'.join).str.lower()
 
         groups = self._df_agg['bin'].unique()
         combinations_lst = list(combinations(groups, 2))
 
         df_lst = []
 
         for metric in self.metrics:
             df_metric = pd.DataFrame()
             for a, b in combinations_lst:
-                # print(metric, a, b)
                 col_a = f'{metric}_{a}'
                 col_b = f'{metric}_{b}'
                 rmse = np.sqrt(((df_[col_a] - df_[col_b]) ** 2).mean())
-                # print(mse)
                 df_metric.loc[a, b] = rmse
                 df_metric.loc[b, a] = rmse
             df_metric = df_metric.reindex(sorted(df_metric.columns), axis=1)
             columns = pd.MultiIndex.from_tuples([(metric, col) for col in df_metric.columns])
             df_metric.columns = columns
             df_lst.append(df_metric)
 
@@ -369,20 +376,23 @@
 
         # Plot each metric
         for i, metric in enumerate(self.metrics):
 
             # If over time, plot line graph, else bar
             if self.date_col:
                 sns.lineplot(data=self._df_agg, x=self.date_col, y=metric, hue='bin', ax=ax[i], palette='Dark2')
+                if self._cutoff_date:
+                    ax[i].axvline(pd.to_datetime(self._cutoff_date), label='Cutoff', linestyle='--')
             else:
                 self._df_agg['metric'] = metric
                 sns.barplot(data=self._df_agg, x='metric', y=metric, hue='bin', ax=ax[i])
 
             ax[i].set_title(f'{metric.title()}')
             ax[i].tick_params(axis='x', labelrotation=45)
+            ax[i].legend()
 
         plt.show()
 
 
 class ABSplit(SplitBase):
     """Splits data into A/B groups based on specified parameters. All members of the population will be in one bin or
     the other.
@@ -406,26 +416,27 @@
     Methods:
         _cost_weighting(): Modifies cost weighting array
         run(): Runs the genetic algorithm
         fitness(): Plot generation fitness graph
         visualise(): Plots metrics using results from genetic algorithm output
     """
 
-    def __init__(self, df, ga_params={}, metric_weights={}, **kwargs):
+    def __init__(self, df, ga_params={}, metric_weights={}, cutoff_date=None, **kwargs):
         """Initializes the class and sets the attributes
 
         Args:
             df (pd.DataFrame): Dataframe to be split
             ga_params (dict): Parameters for the genetic algorithm (default: {})
             metric_weights (dict): Weights for each metric in the data (default: {})
             **kwargs: Additional keyword arguments
         """
-        super().__init__(ga_params=ga_params, metric_weights=metric_weights, **kwargs)
+        # print(cutoff_date)
+        super().__init__(ga_params=ga_params, metric_weights=metric_weights, cutoff_date=cutoff_date, **kwargs)
         self.df = df
-        self._population = Data(self.df.copy(), **kwargs)
+        self._population = Data(self.df.copy(), cutoff_date=cutoff_date, **kwargs)
 
     def _build_df_vis(self):
         # Merge solution results (_df_results) onto input data (metrics) so that data can be visualised
         self._df_vis = self._population.stacked.merge(
             self._df_result,
             left_index=True,
             right_index=True
```

### Comparing `absplit-1.1.0/absplit/param.py` & `absplit-1.2.0/absplit/param.py`

 * *Files identical despite different names*

### Comparing `absplit-1.1.0/images/logo.jpeg` & `absplit-1.2.0/images/logo.jpeg`

 * *Files identical despite different names*

### Comparing `absplit-1.1.0/pyproject.toml` & `absplit-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "absplit"
-version = "1.1.0"
+version = "1.2.0"
 description = "Generates A/B test groups"
 readme = "README.md"
 authors = [{name = "Cormac Rynne", email = "cormac.ry@gmail.com"}]
 license = {file = "LICENSE"}
 repository = "https://github.com/cormac-rynne/absplit"
 requires-python = "<=3.11"
 classifiers = [
```

### Comparing `absplit-1.1.0/tests/test_data.py` & `absplit-1.2.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `absplit-1.1.0/tests/test_ga.py` & `absplit-1.2.0/tests/test_ga.py`

 * *Files identical despite different names*

### Comparing `absplit-1.1.0/PKG-INFO` & `absplit-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: absplit
-Version: 1.1.0
+Version: 1.2.0
 Summary: Generates A/B test groups
 Keywords: absplit,a/b test,ab test,ab split,split,set formation,group formation
 Author-email: Cormac Rynne <cormac.ry@gmail.com>
 Requires-Python: <=3.11
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -31,15 +31,15 @@
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg" width="460" height="140">
 <h3><strong>ABSplit</strong></h3>
 Split your data into matching A/B/n groups
 
 ![license](https://img.shields.io/badge/License-MIT-blue.svg)
-![version](https://img.shields.io/badge/version-1.1.0-blue.svg)
+![version](https://img.shields.io/badge/version-1.2.0-blue.svg)
 ![version](https://img.shields.io/badge/python-3-orange.svg)
 
 </div>
 
 <details open>
   <summary>Table of Contents</summary>
   <ol>
@@ -143,16 +143,25 @@
 
 # Visualise generation fitness
 ab.fitness()
 
 # Visualise data
 ab.visualise()
 
-# Extract results
+# Extract bin splits
 df = ab.results
+
+# Extract distributions summary
+df_dist = ab.distributions
+
+# Extract data aggregated by bins
+df_agg = ab.aggregations
+
+# Extract RMSE summary
+df_rmse = ab.rmse
 ```
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ## API Reference
 ### Absplit 
 `ABSplit(df, metrics, splitting, date_col=None, ga_params={}, metric_weights={}, splits=[0.5, 0.5], size_penalty=0)`
 
@@ -167,14 +176,16 @@
 * `ga_params` (dict, optional): Parameters for the genetic algorithm `pygad.GA` module parameters, see 
 [here](https://pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html#pygad-ga-class) for arguments you can pass
 (default: `{}`)
 * `splits` (list, optional): How many groups to split into, and relative size of the groups (default: `[0.5, 0.5]`,
 2 groups of equal size)
 * `size_penalty` (float, optional): Penalty weighting for differences in the population count between groups 
 (default: `0`)
+* `cutoff_date` (str, optional): Cutoff date between fitting and validation data. If `None`, it will fit on all 
+available data. If cutoff date provided, RMSE scores will be for validation period
 * `metric_weights` (dict, optional): Weights for each metric in the data. If you want the splitting to focus on 
 one metrics more than the other, you can prioritise this here (default: `{}`)
 
 
 ### Match 
 `Match(population, sample, metrics, splitting, date_col=None, ga_params={}, metric_weights={})`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: absplit Version: 1.1.0 Summary: Generates A/B test
+Metadata-Version: 2.1 Name: absplit Version: 1.2.0 Summary: Generates A/B test
 groups Keywords: absplit,a/b test,ab test,ab split,split,set formation,group
 formation Author-email: Cormac Rynne
 ry@gmail.com> Requires-Python: <=3.11 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
@@ -15,15 +15,15 @@
 Libraries :: Python Modules Requires-Dist: pygad==3.0.1 Requires-Dist: scikit-
 learn Requires-Dist: numpy Requires-Dist: pandas Requires-Dist: seaborn
 Project-URL: Home, https://github.com/cormac-rynne/absplit
 [https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg]
                                **** ABSplit ****
  Split your data into matching A/B/n groups ![license](https://img.shields.io/
  badge/License-MIT-blue.svg) ![version](https://img.shields.io/badge/version-
- 1.1.0-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
+ 1.2.0-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
  Table of Contents
    1. About_The_Project
    2. Getting_Started
           o Installation
    3. Tutorials
           o Do_it_yourself
    4. Usage
@@ -60,16 +60,18 @@
 'y']] for item in sublist] + ['x']*3, 'city': [item for sublist in [[x]*3 for x
 in ['a', 'b', 'c', 'd', 'e']] for item in sublist], 'metric1': np.arange(0, 15,
 1), 'metric2': np.arange(0, 150, 10) } df = pd.DataFrame(data_dct) # Identify
 which columns are metrics, which is the time period, and what to split on
 kwargs = { 'metrics': ['metric1', 'metric2'], 'date_col': 'date', 'splitting':
 'city' } # Initialise ab = ABSplit( df=df, split=[.5, .5], # Split into 2
 groups of equal size **kwargs, ) # Generate split ab.run() # Visualise
-generation fitness ab.fitness() # Visualise data ab.visualise() # Extract
-results df = ab.results ```
+generation fitness ab.fitness() # Visualise data ab.visualise() # Extract bin
+splits df = ab.results # Extract distributions summary df_dist =
+ab.distributions # Extract data aggregated by bins df_agg = ab.aggregations #
+Extract RMSE summary df_rmse = ab.rmse ```
                                                                   (back_to_top)
 ## API Reference ### Absplit `ABSplit(df, metrics, splitting, date_col=None,
 ga_params={}, metric_weights={}, splits=[0.5, 0.5], size_penalty=0)` Splits
 population into 2 groups. Mutually exclusive, completely exhaustive Arguments:
 * `df` (pd.DataFrame): Dataframe to be split * `metrics` (str, list): Name of,
 or list of names of, metric columns in DataFrame * `splitting` (str): Name of
 column that represents individuals in the population that is getting split *
@@ -78,34 +80,36 @@
 timeseries, (default `None`) * `ga_params` (dict, optional): Parameters for the
 genetic algorithm `pygad.GA` module parameters, see [here](https://
 pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html#pygad-ga-class)
 for arguments you can pass (default: `{}`) * `splits` (list, optional): How
 many groups to split into, and relative size of the groups (default: `[0.5,
 0.5]`, 2 groups of equal size) * `size_penalty` (float, optional): Penalty
 weighting for differences in the population count between groups (default: `0`)
-* `metric_weights` (dict, optional): Weights for each metric in the data. If
-you want the splitting to focus on one metrics more than the other, you can
-prioritise this here (default: `{}`) ### Match `Match(population, sample,
-metrics, splitting, date_col=None, ga_params={}, metric_weights={})` Takes
-DataFrame `sample` and finds a comparable group in `population`. Arguments: *
-`population` (pd.DataFrame): Population to search for comparable group (**Must
-exclude sample data**) * `sample` (pd.DataFrame): Sample we are looking to find
-a match for. * `metrics` (str, list): Name of, or list of names of, metric
-columns in DataFrame * `splitting` (str): Name of column that represents
-individuals in the population that is getting split * `date_col` (str,
-optional): Name of column that represents time periods, if applicable. If left
-empty, it will perform a static split, i.e. not across timeseries, (default
-`None`) * `ga_params` (dict, optional): Parameters for the genetic algorithm
-`pygad.GA` module parameters, see [here](https://pygad.readthedocs.io/en/
-latest/README_pygad_ReadTheDocs.html#pygad-ga-class) for arguments you can pass
-(default: `{}`) * `splits` (list, optional): How many groups to split into, and
-relative size of the groups (default: `[0.5, 0.5]`, 2 groups of equal size) *
-`metric_weights` (dict, optional): Weights for each metric in the data. If you
-want the splitting to focus on one metrics more than the other, you can
-prioritise this here (default: `{}`)
+* `cutoff_date` (str, optional): Cutoff date between fitting and validation
+data. If `None`, it will fit on all available data. If cutoff date provided,
+RMSE scores will be for validation period * `metric_weights` (dict, optional):
+Weights for each metric in the data. If you want the splitting to focus on one
+metrics more than the other, you can prioritise this here (default: `{}`) ###
+Match `Match(population, sample, metrics, splitting, date_col=None, ga_params=
+{}, metric_weights={})` Takes DataFrame `sample` and finds a comparable group
+in `population`. Arguments: * `population` (pd.DataFrame): Population to search
+for comparable group (**Must exclude sample data**) * `sample` (pd.DataFrame):
+Sample we are looking to find a match for. * `metrics` (str, list): Name of, or
+list of names of, metric columns in DataFrame * `splitting` (str): Name of
+column that represents individuals in the population that is getting split *
+`date_col` (str, optional): Name of column that represents time periods, if
+applicable. If left empty, it will perform a static split, i.e. not across
+timeseries, (default `None`) * `ga_params` (dict, optional): Parameters for the
+genetic algorithm `pygad.GA` module parameters, see [here](https://
+pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html#pygad-ga-class)
+for arguments you can pass (default: `{}`) * `splits` (list, optional): How
+many groups to split into, and relative size of the groups (default: `[0.5,
+0.5]`, 2 groups of equal size) * `metric_weights` (dict, optional): Weights for
+each metric in the data. If you want the splitting to focus on one metrics more
+than the other, you can prioritise this here (default: `{}`)
                                                                   (back_to_top)
 ## Contributing I welcome contributions to ABSplit! For major changes, please
 open an issue first to discuss what you would like to change. Please make sure
 to update tests as appropriate.
                                                                   (back_to_top)
 ## License [MIT](https://choosealicense.com/licenses/mit/)
                                                                   (back_to_top)
```

