# Comparing `tmp/gmltools-0.0.80.tar.gz` & `tmp/gmltools-0.0.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmltools-0.0.80.tar", last modified: Wed Jun 14 08:50:22 2023, max compression
+gzip compressed data, was "gmltools-0.0.81.tar", last modified: Wed Jun 14 08:54:29 2023, max compression
```

## Comparing `gmltools-0.0.80.tar` & `gmltools-0.0.81.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 08:50:22.484146 gmltools-0.0.80/
--rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.80/LICENSE
--rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.80/Models.ipynb
--rw-rw-rw-   0        0        0     1021 2023-06-14 08:50:22.483060 gmltools-0.0.80/PKG-INFO
--rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.80/README.md
--rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.80/gmltools.yml
--rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.80/mltools.yml
--rw-rw-rw-   0        0        0      618 2023-06-14 08:50:03.000000 gmltools-0.0.80/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-14 08:50:22.484146 gmltools-0.0.80/setup.cfg
--rw-rw-rw-   0        0        0     1746 2023-06-14 08:49:55.000000 gmltools-0.0.80/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:50:22.447423 gmltools-0.0.80/src/
-drwxrwxrwx   0        0        0        0 2023-06-14 08:50:22.461352 gmltools-0.0.80/src/gmltools/
--rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.80/src/gmltools/To_Do.txt
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.80/src/gmltools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:50:22.468518 gmltools-0.0.80/src/gmltools/eda/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.80/src/gmltools/eda/__init__.py
--rw-rw-rw-   0        0        0    42538 2023-05-29 11:18:21.000000 gmltools-0.0.80/src/gmltools/eda/eda.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:50:22.475291 gmltools-0.0.80/src/gmltools/models/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.80/src/gmltools/models/__init__.py
--rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.80/src/gmltools/models/bayes.py
--rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.80/src/gmltools/models/custom_scorings.py
--rw-rw-rw-   0        0        0     5653 2023-05-24 10:54:18.000000 gmltools-0.0.80/src/gmltools/models/dummy_model.py
--rw-rw-rw-   0        0        0   160691 2023-06-14 08:43:11.000000 gmltools-0.0.80/src/gmltools/models/model.py
--rw-rw-rw-   0        0        0     7038 2023-06-06 11:25:02.000000 gmltools-0.0.80/src/gmltools/models/models_info.py
--rw-rw-rw-   0        0        0    13212 2023-05-12 09:20:42.000000 gmltools-0.0.80/src/gmltools/models/timeseriesplit.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:50:22.478578 gmltools-0.0.80/src/gmltools/models_analysis/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.80/src/gmltools/models_analysis/__init__.py
--rw-rw-rw-   0        0        0    73636 2023-04-30 15:51:16.000000 gmltools-0.0.80/src/gmltools/models_analysis/classification_analysis.py
--rw-rw-rw-   0        0        0     5653 2023-04-30 15:57:34.000000 gmltools-0.0.80/src/gmltools/models_analysis/xai.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:50:22.483060 gmltools-0.0.80/src/gmltools/preprocess/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.80/src/gmltools/preprocess/__init__.py
--rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.80/src/gmltools/preprocess/autoregressive_features.py
--rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.80/src/gmltools/preprocess/manage_holidays.py
--rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.80/src/gmltools/preprocess/preprocess.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:50:22.467255 gmltools-0.0.80/src/gmltools.egg-info/
--rw-rw-rw-   0        0        0     1021 2023-06-14 08:50:22.000000 gmltools-0.0.80/src/gmltools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      906 2023-06-14 08:50:22.000000 gmltools-0.0.80/src/gmltools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 08:50:22.000000 gmltools-0.0.80/src/gmltools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      137 2023-06-14 08:50:22.000000 gmltools-0.0.80/src/gmltools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-14 08:50:22.000000 gmltools-0.0.80/src/gmltools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 08:54:29.523493 gmltools-0.0.81/
+-rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.81/LICENSE
+-rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.81/Models.ipynb
+-rw-rw-rw-   0        0        0     1021 2023-06-14 08:54:29.522419 gmltools-0.0.81/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.81/README.md
+-rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.81/gmltools.yml
+-rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.81/mltools.yml
+-rw-rw-rw-   0        0        0      618 2023-06-14 08:54:20.000000 gmltools-0.0.81/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-14 08:54:29.523493 gmltools-0.0.81/setup.cfg
+-rw-rw-rw-   0        0        0     1746 2023-06-14 08:54:18.000000 gmltools-0.0.81/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:54:29.486267 gmltools-0.0.81/src/
+drwxrwxrwx   0        0        0        0 2023-06-14 08:54:29.498153 gmltools-0.0.81/src/gmltools/
+-rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.81/src/gmltools/To_Do.txt
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.81/src/gmltools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:54:29.503714 gmltools-0.0.81/src/gmltools/eda/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.81/src/gmltools/eda/__init__.py
+-rw-rw-rw-   0        0        0    42538 2023-05-29 11:18:21.000000 gmltools-0.0.81/src/gmltools/eda/eda.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:54:29.515690 gmltools-0.0.81/src/gmltools/models/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.81/src/gmltools/models/__init__.py
+-rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.81/src/gmltools/models/bayes.py
+-rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.81/src/gmltools/models/custom_scorings.py
+-rw-rw-rw-   0        0        0     5653 2023-05-24 10:54:18.000000 gmltools-0.0.81/src/gmltools/models/dummy_model.py
+-rw-rw-rw-   0        0        0   160613 2023-06-14 08:54:19.000000 gmltools-0.0.81/src/gmltools/models/model.py
+-rw-rw-rw-   0        0        0     7038 2023-06-06 11:25:02.000000 gmltools-0.0.81/src/gmltools/models/models_info.py
+-rw-rw-rw-   0        0        0    13212 2023-05-12 09:20:42.000000 gmltools-0.0.81/src/gmltools/models/timeseriesplit.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:54:29.518680 gmltools-0.0.81/src/gmltools/models_analysis/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.81/src/gmltools/models_analysis/__init__.py
+-rw-rw-rw-   0        0        0    73636 2023-04-30 15:51:16.000000 gmltools-0.0.81/src/gmltools/models_analysis/classification_analysis.py
+-rw-rw-rw-   0        0        0     5653 2023-04-30 15:57:34.000000 gmltools-0.0.81/src/gmltools/models_analysis/xai.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:54:29.522419 gmltools-0.0.81/src/gmltools/preprocess/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.81/src/gmltools/preprocess/__init__.py
+-rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.81/src/gmltools/preprocess/autoregressive_features.py
+-rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.81/src/gmltools/preprocess/manage_holidays.py
+-rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.81/src/gmltools/preprocess/preprocess.py
+drwxrwxrwx   0        0        0        0 2023-06-14 08:54:29.502258 gmltools-0.0.81/src/gmltools.egg-info/
+-rw-rw-rw-   0        0        0     1021 2023-06-14 08:54:29.000000 gmltools-0.0.81/src/gmltools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      906 2023-06-14 08:54:29.000000 gmltools-0.0.81/src/gmltools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 08:54:29.000000 gmltools-0.0.81/src/gmltools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      137 2023-06-14 08:54:29.000000 gmltools-0.0.81/src/gmltools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-14 08:54:29.000000 gmltools-0.0.81/src/gmltools.egg-info/top_level.txt
```

### Comparing `gmltools-0.0.80/LICENSE` & `gmltools-0.0.81/LICENSE`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.80/Models.ipynb` & `gmltools-0.0.81/Models.ipynb`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.80/PKG-INFO` & `gmltools-0.0.81/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.80
+Version: 0.0.81
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.80/README.md` & `gmltools-0.0.81/README.md`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.80/gmltools.yml` & `gmltools-0.0.81/gmltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.80/mltools.yml` & `gmltools-0.0.81/mltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.80/pyproject.toml` & `gmltools-0.0.81/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gmltools"
-version = "0.0.80"
+version = "0.0.81"
 description = "Machine Learning library aiming for a higher level programming, organizing best tools"
 authors = ["Diego Sanz-Gadea Sánchez"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gmltools-0.0.80/setup.py` & `gmltools-0.0.81/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6.3,<4.0.0', 'numpy>=1.21.6,<2.0.0', 'pandas>=1.5.0,<2.0.0', 'xgboost==1.5.0', 'lightgbm>=3.3.5', 'linear-tree>=0.3.5', 'scikit-learn>=1.2.1']
 
 setup_kwargs = {
     'name': 'gmltools',
-    'version': '0.0.80',
+    'version': '0.0.81',
     'description': 'Machine Learning library aiming for a higher level programming, organizing best tools',
     'long_description': '# gmltools\n\nMachine Learning library aiming for a higher level programming, organizing best tools\n\n```bash\n$ pip install gmltools\n```\n\n## Usage\n\n- TODO\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`gmltutils` was created by Diego Sanz-Gadea Sánchez. It is licensed under the terms of the GNU General Public License v3.0 license.\n\n## Credits\n\n`gmltutils` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
     'author': 'Diego Sanz-Gadea Sánchez',
     'author_email': 'dsanzgadeasanchez@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `gmltools-0.0.80/src/gmltools/To_Do.txt` & `gmltools-0.0.81/src/gmltools/To_Do.txt`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.80/src/gmltools/eda/eda.py` & `gmltools-0.0.81/src/gmltools/eda/eda.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.80/src/gmltools/models/bayes.py` & `gmltools-0.0.81/src/gmltools/models/bayes.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.80/src/gmltools/models/custom_scorings.py` & `gmltools-0.0.81/src/gmltools/models/custom_scorings.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.80/src/gmltools/models/dummy_model.py` & `gmltools-0.0.81/src/gmltools/models/dummy_model.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.80/src/gmltools/models/model.py` & `gmltools-0.0.81/src/gmltools/models/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -469,15 +469,15 @@
         select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
         self.model=select_searchcv.fit()
         
         #generate a dictionary with all the parameters used in the model
         self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
         
         self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), "Class_Weights":str(class_weight), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
-                                    'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
+                                    'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape),
                                     'scoring':str(scoring), 'cv':str(self.cv), 'criterion':str(criterion), 'sample_weight':str(sample_weight)}
         
 
     
     def XGBoost_Classifier( self, ordinal_cat_cols:list=None,
                             scoring='accuracy', eval_metric='merror',
                             objective='multi:softmax', grid_params:dict={},
```

### Comparing `gmltools-0.0.80/src/gmltools/models/models_info.py` & `gmltools-0.0.81/src/gmltools/models/models_info.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.80/src/gmltools/models/timeseriesplit.py` & `gmltools-0.0.81/src/gmltools/models/timeseriesplit.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.80/src/gmltools/models_analysis/classification_analysis.py` & `gmltools-0.0.81/src/gmltools/models_analysis/classification_analysis.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.80/src/gmltools/models_analysis/xai.py` & `gmltools-0.0.81/src/gmltools/models_analysis/xai.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.80/src/gmltools/preprocess/autoregressive_features.py` & `gmltools-0.0.81/src/gmltools/preprocess/autoregressive_features.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.80/src/gmltools/preprocess/manage_holidays.py` & `gmltools-0.0.81/src/gmltools/preprocess/manage_holidays.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.80/src/gmltools/preprocess/preprocess.py` & `gmltools-0.0.81/src/gmltools/preprocess/preprocess.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.80/src/gmltools.egg-info/PKG-INFO` & `gmltools-0.0.81/src/gmltools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.80
+Version: 0.0.81
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.80/src/gmltools.egg-info/SOURCES.txt` & `gmltools-0.0.81/src/gmltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

