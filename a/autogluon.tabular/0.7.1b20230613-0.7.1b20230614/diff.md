# Comparing `tmp/autogluon.tabular-0.7.1b20230613.tar.gz` & `tmp/autogluon.tabular-0.7.1b20230614.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.tabular-0.7.1b20230613.tar", last modified: Tue Jun 13 09:04:13 2023, max compression
+gzip compressed data, was "autogluon.tabular-0.7.1b20230614.tar", last modified: Wed Jun 14 09:04:06 2023, max compression
```

## Comparing `autogluon.tabular-0.7.1b20230613.tar` & `autogluon.tabular-0.7.1b20230614.tar`

### file list

```diff
@@ -1,173 +1,173 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.622498 autogluon.tabular-0.7.1b20230613/
--rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-06-13 09:04:13.622498 autogluon.tabular-0.7.1b20230613/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 09:04:13.622498 autogluon.tabular-0.7.1b20230613/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.606497 autogluon.tabular-0.7.1b20230613/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.606497 autogluon.tabular-0.7.1b20230613/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.610497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.610497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21133 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/configs/config_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/configs/feature_generator_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/configs/hyperparameter_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.610497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/learner/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/learner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52502 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/learner/abstract_learner.py
--rw-r--r--   0 runner    (1001) docker     (123)    24172 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/learner/default_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.610497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.610497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/_utils/rapids_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/_utils/torch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.610497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/automm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/automm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/automm/automm_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/automm/ft_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.610497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/catboost/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/catboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/catboost/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/catboost/catboost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/catboost/catboost_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.610497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/catboost/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/catboost/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.610497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fastainn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fastainn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fastainn/callbacks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1370 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fastainn/fastai_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.610497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fastainn/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fastainn/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fastainn/imports_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fastainn/quantile_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25566 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.610497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fasttext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fasttext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fasttext/fasttext_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.610497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fasttext/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fasttext/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.614497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/image_prediction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/image_prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/image_prediction/image_predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.614497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/imodels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/imodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/imodels/imodels_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.614497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/knn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/knn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/knn/_knn_loo_variants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/knn/knn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/knn/knn_rapids_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/knn/knn_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.614497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lgb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lgb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lgb/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.614497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lgb/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lgb/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    18414 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lgb/lgb_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lgb/lgb_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.614497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.614497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lr/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lr/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lr/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lr/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    13640 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lr/lr_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lr/lr_rapids_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.614497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/rf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/rf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.614497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/rf/compilers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/rf/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/rf/compilers/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/rf/compilers/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)    20649 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/rf/rf_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    36291 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/rf/rf_quantile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/rf/rf_rapids_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.614497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.618497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    23173 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/modified_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/pretexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/tab_model_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/tab_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    22608 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.618497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabpfn/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabpfn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabpfn/tabpfn_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.618497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.618497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/compilers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/compilers/native.py
--rw-r--r--   0 runner    (1001) docker     (123)    17109 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.618497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.618497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33156 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13347 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.618497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35716 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.618497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/text_prediction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/text_prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.618497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/vowpalwabbit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/vowpalwabbit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.618497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/xgboost/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/xgboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/xgboost/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.618497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/xgboost/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/xgboost/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/xgboost/xgboost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/xgboost/xgboost_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.618497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/xt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/xt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/xt/xt_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.618497 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/predictor/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/predictor/interpretable_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)   266100 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/predictor/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.622498 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.622498 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/trainer/model_presets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/trainer/model_presets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17878 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/trainer/model_presets/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/trainer/model_presets/presets_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/trainer/model_presets/presets_distill.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.622498 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-06-13 09:03:45.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/tuning/feature_pruner.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-13 09:04:13.000000 autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:04:13.610497 autogluon.tabular-0.7.1b20230613/src/autogluon.tabular.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-06-13 09:04:13.000000 autogluon.tabular-0.7.1b20230613/src/autogluon.tabular.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-06-13 09:04:13.000000 autogluon.tabular-0.7.1b20230613/src/autogluon.tabular.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:04:13.000000 autogluon.tabular-0.7.1b20230613/src/autogluon.tabular.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-13 09:04:13.000000 autogluon.tabular-0.7.1b20230613/src/autogluon.tabular.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-13 09:04:13.000000 autogluon.tabular-0.7.1b20230613/src/autogluon.tabular.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-13 09:04:13.000000 autogluon.tabular-0.7.1b20230613/src/autogluon.tabular.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:04:13.000000 autogluon.tabular-0.7.1b20230613/src/autogluon.tabular.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.970643 autogluon.tabular-0.7.1b20230614/
+-rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-06-14 09:04:06.970643 autogluon.tabular-0.7.1b20230614/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 09:04:06.970643 autogluon.tabular-0.7.1b20230614/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.942643 autogluon.tabular-0.7.1b20230614/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.942643 autogluon.tabular-0.7.1b20230614/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.946643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.946643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21133 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/configs/config_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/configs/feature_generator_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/configs/hyperparameter_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.950643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/learner/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/learner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52502 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/learner/abstract_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24172 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/learner/default_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.950643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.950643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/_utils/rapids_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/_utils/torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.950643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/automm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/automm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/automm/automm_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/automm/ft_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.950643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/catboost/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/catboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/catboost/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/catboost/catboost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/catboost/catboost_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.950643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/catboost/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/catboost/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.950643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/fastainn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/fastainn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/fastainn/callbacks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1370 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/fastainn/fastai_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.954643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/fastainn/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/fastainn/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/fastainn/imports_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/fastainn/quantile_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25566 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.954643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/fasttext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/fasttext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/fasttext/fasttext_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.954643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/fasttext/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/fasttext/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.954643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/image_prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/image_prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/image_prediction/image_predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.954643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/imodels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/imodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/imodels/imodels_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.954643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/knn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/knn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/knn/_knn_loo_variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/knn/knn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/knn/knn_rapids_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/knn/knn_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.954643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/lgb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/lgb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/lgb/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.954643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/lgb/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/lgb/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18414 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/lgb/lgb_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/lgb/lgb_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.954643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/lr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/lr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.958643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/lr/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/lr/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/lr/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/lr/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13640 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/lr/lr_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/lr/lr_rapids_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.958643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/rf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/rf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.958643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/rf/compilers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/rf/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/rf/compilers/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/rf/compilers/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20649 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/rf/rf_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36291 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/rf/rf_quantile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/rf/rf_rapids_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.962643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tab_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tab_transformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.962643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tab_transformer/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tab_transformer/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23173 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tab_transformer/modified_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tab_transformer/pretexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tab_transformer/tab_model_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tab_transformer/tab_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22608 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tab_transformer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.962643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tabpfn/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tabpfn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tabpfn/tabpfn_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.962643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tabular_nn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tabular_nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.962643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tabular_nn/compilers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tabular_nn/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tabular_nn/compilers/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17109 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.962643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tabular_nn/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tabular_nn/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.962643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tabular_nn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tabular_nn/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33156 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13347 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.966643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tabular_nn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tabular_nn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35716 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.966643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/text_prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/text_prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.966643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/vowpalwabbit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/vowpalwabbit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.966643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/xgboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/xgboost/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.966643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/xgboost/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/xgboost/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/xgboost/xgboost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/xgboost/xgboost_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.966643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/xt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/xt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/xt/xt_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.966643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/predictor/interpretable_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267286 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/predictor/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.966643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.970643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/trainer/model_presets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/trainer/model_presets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17878 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/trainer/model_presets/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/trainer/model_presets/presets_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/trainer/model_presets/presets_distill.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.970643 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-06-14 09:03:34.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/tuning/feature_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-14 09:04:06.000000 autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:04:06.946643 autogluon.tabular-0.7.1b20230614/src/autogluon.tabular.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-06-14 09:04:06.000000 autogluon.tabular-0.7.1b20230614/src/autogluon.tabular.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-06-14 09:04:06.000000 autogluon.tabular-0.7.1b20230614/src/autogluon.tabular.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:04:06.000000 autogluon.tabular-0.7.1b20230614/src/autogluon.tabular.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-14 09:04:06.000000 autogluon.tabular-0.7.1b20230614/src/autogluon.tabular.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-14 09:04:06.000000 autogluon.tabular-0.7.1b20230614/src/autogluon.tabular.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-14 09:04:06.000000 autogluon.tabular-0.7.1b20230614/src/autogluon.tabular.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:04:06.000000 autogluon.tabular-0.7.1b20230614/src/autogluon.tabular.egg-info/zip-safe
```

### Comparing `autogluon.tabular-0.7.1b20230613/PKG-INFO` & `autogluon.tabular-0.7.1b20230614/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.tabular
-Version: 0.7.1b20230613
+Version: 0.7.1b20230614
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.tabular-0.7.1b20230613/setup.py` & `autogluon.tabular-0.7.1b20230614/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/configs/config_helper.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/configs/config_helper.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/configs/feature_generator_presets.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/configs/feature_generator_presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/configs/hyperparameter_configs.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/configs/hyperparameter_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/configs/presets_configs.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/configs/presets_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/learner/abstract_learner.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/learner/abstract_learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/learner/default_learner.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/learner/default_learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/__init__.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/_utils/rapids_utils.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/_utils/rapids_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/_utils/torch_utils.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/_utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/automm/automm_model.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/automm/automm_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/automm/ft_transformer.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/automm/ft_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/catboost/callbacks.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/catboost/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/catboost/catboost_model.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/catboost/catboost_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/catboost/catboost_utils.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/catboost/catboost_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fastainn/callbacks.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/fastainn/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fastainn/fastai_helpers.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/fastainn/fastai_helpers.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fastainn/quantile_helpers.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/fastainn/quantile_helpers.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fasttext/fasttext_model.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/fasttext/fasttext_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/image_prediction/image_predictor.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/image_prediction/image_predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/imodels/imodels_models.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/imodels/imodels_models.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/knn/_knn_loo_variants.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/knn/_knn_loo_variants.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/knn/knn_model.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/knn/knn_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/knn/knn_rapids_model.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/knn/knn_rapids_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/knn/knn_utils.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/knn/knn_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lgb/callbacks.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/lgb/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lgb/lgb_model.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/lgb/lgb_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lgb/lgb_utils.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/lgb/lgb_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lr/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/lr/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lr/lr_model.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/lr/lr_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/lr/lr_rapids_model.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/lr/lr_rapids_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/rf/compilers/native.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/rf/compilers/native.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/rf/compilers/onnx.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/rf/compilers/onnx.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/rf/rf_model.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/rf/rf_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/rf/rf_quantile.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/rf/rf_quantile.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/rf/rf_rapids_model.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/rf/rf_rapids_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/modified_transformer.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tab_transformer/modified_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/pretexts.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tab_transformer/pretexts.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/tab_model_base.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tab_transformer/tab_model_base.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/tab_transformer.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tab_transformer/tab_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tab_transformer/utils.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tab_transformer/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabpfn/tabpfn_model.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tabpfn/tabpfn_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/compilers/native.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tabular_nn/compilers/native.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/xgboost/callbacks.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/xgboost/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/xgboost/xgboost_model.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/xgboost/xgboost_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/xgboost/xgboost_utils.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/xgboost/xgboost_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/models/xt/xt_model.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/models/xt/xt_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/predictor/interpretable_predictor.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/predictor/interpretable_predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/predictor/predictor.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/predictor/predictor.py`

 * *Files 1% similar despite different names*

```diff
@@ -655,18 +655,35 @@
                 This held-out data is only used to score models and determine weighted ensemble weights.
                 Enable this if there is a large gap between score_val and score_test in stack models.
                 Note: If `tuning_data` was specified, `tuning_data` is used as the holdout data.
                 Disabled if not bagging.
             hyperparameter_tune_kwargs : str or dict, default = None
                 Hyperparameter tuning strategy and kwargs (for example, how many HPO trials to run).
                 If None, then hyperparameter tuning will not be performed.
-                Valid preset values:
-                    'auto': Uses the 'random' preset.
-                    'random': Performs HPO via random search using local scheduler.
-                The 'searcher' key is required when providing a dict.
+                You can either choose to provide a preset
+                    Valid preset values:
+                        'auto': Performs HPO via bayesian optimization search on NN_TORCH and FASTAI models, and random search on other models using local scheduler.
+                        'random': Performs HPO via random search using local scheduler.
+                Or provide a dict to specify searchers and schedulers
+                    Valid keys:
+                        'num_trials': How many HPO trials to run
+                        'scheduler': Which scheduler to use
+                            Valid values:
+                                'local': Local shceduler that schedule trials FIFO
+                        'searcher': Which searching algorithm to use
+                            'local_random': Uses the 'random' searcher
+                            'random': Perform random search
+                            'auto': Perform bayesian optimization search on NN_TORCH and FASTAI models. Perform random search on other models.
+                    The 'scheduler' and 'searcher' key are required when providing a dict.
+                    An example of a valid dict:
+                        hyperparameter_tune_kwargs = {
+                            'num_trials': 5,
+                            'scheduler' : 'local',
+                            'searcher': 'auto',
+                        }
             feature_prune_kwargs: dict, default = None
                 Performs layer-wise feature pruning via recursive feature elimination with permutation feature importance.
                 This fits all models in a stack layer once, discovers a pruned set of features, fits all models in the stack layer
                 again with the pruned set of features, and updates input feature lists for models whose validation score improved.
                 If None, do not perform feature pruning. If empty dictionary, perform feature pruning with default configurations.
                 For valid dictionary keys, refer to :class:`autogluon.core.utils.feature_selection.FeatureSelector` and
                 `autogluon.core.trainer.abstract_trainer.AbstractTrainer._proxy_model_feature_prune` documentation.
@@ -3531,14 +3548,15 @@
             A list containing lines of the log file
         """
         file_path = log_file_path
         if file_path is None:
             assert predictor_path is not None, "Please either provide `predictor_path` or `log_file_path` to load the log file"
             file_path = os.path.join(predictor_path, "logs", cls._predictor_log_file_name)
         assert os.path.isfile(file_path), f"Log file does not exist at {file_path}"
+        lines = []
         with open(file_path, "r") as f:
             lines = f.readlines()
         return lines
 
     def _setup_log_to_file(self, path, log_to_file, log_file_path):
         if log_to_file:
             if log_file_path == "auto":
```

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/trainer/auto_trainer.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/trainer/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/trainer/model_presets/presets.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/trainer/model_presets/presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/trainer/model_presets/presets_custom.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/trainer/model_presets/presets_custom.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/trainer/model_presets/presets_distill.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/trainer/model_presets/presets_distill.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon/tabular/tuning/feature_pruner.py` & `autogluon.tabular-0.7.1b20230614/src/autogluon/tabular/tuning/feature_pruner.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon.tabular.egg-info/PKG-INFO` & `autogluon.tabular-0.7.1b20230614/src/autogluon.tabular.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.tabular
-Version: 0.7.1b20230613
+Version: 0.7.1b20230614
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon.tabular.egg-info/SOURCES.txt` & `autogluon.tabular-0.7.1b20230614/src/autogluon.tabular.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230613/src/autogluon.tabular.egg-info/requires.txt` & `autogluon.tabular-0.7.1b20230614/src/autogluon.tabular.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 numpy<1.27,>=1.21
 scipy<1.12,>=1.5.4
 pandas<1.6,>=1.4.1
 scikit-learn<1.3,>=1.0
 networkx<3.0,>=2.3
-autogluon.core==0.7.1b20230613
-autogluon.features==0.7.1b20230613
+autogluon.core==0.7.1b20230614
+autogluon.features==0.7.1b20230614
 
 [all]
-catboost<1.3,>=1.1
-fastai<2.8,>=2.3.1
 lightgbm<3.4,>=3.3
-autogluon.core[all]==0.7.1b20230613
-torch<1.14,>=1.9
+fastai<2.8,>=2.3.1
+catboost<1.3,>=1.1
+autogluon.core[all]==0.7.1b20230614
 xgboost<1.8,>=1.6
+torch<1.14,>=1.9
 
 [all:sys_platform == "darwin"]
 catboost<1.2,>=1.1
 
 [catboost]
 catboost<1.3,>=1.1
 
@@ -30,15 +30,15 @@
 [imodels]
 imodels<1.4.0,>=1.3.10
 
 [lightgbm]
 lightgbm<3.4,>=3.3
 
 [ray]
-autogluon.core[all]==0.7.1b20230613
+autogluon.core[all]==0.7.1b20230614
 
 [skex]
 scikit-learn-intelex<2023.2,>=2021.7
 
 [skl2onnx]
 skl2onnx<1.14.0,>=1.13.0
 onnxruntime-gpu<1.14.0,>=1.13.0
```

