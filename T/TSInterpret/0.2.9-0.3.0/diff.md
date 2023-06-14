# Comparing `tmp/TSInterpret-0.2.9.tar.gz` & `tmp/TSInterpret-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TSInterpret-0.2.9.tar", last modified: Tue Jun 13 14:47:08 2023, max compression
+gzip compressed data, was "TSInterpret-0.3.0.tar", last modified: Wed Jun 14 07:56:24 2023, max compression
```

## Comparing `TSInterpret-0.2.9.tar` & `TSInterpret-0.3.0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:08.229413 TSInterpret-0.2.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:08.221413 TSInterpret-0.2.9/ClassificationModels/
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-13 14:46:55.000000 TSInterpret-0.2.9/ClassificationModels/CNN.py
--rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-06-13 14:46:55.000000 TSInterpret-0.2.9/ClassificationModels/CNN_T.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-06-13 14:46:55.000000 TSInterpret-0.2.9/ClassificationModels/DecisionTree.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-13 14:46:55.000000 TSInterpret-0.2.9/ClassificationModels/LSTM.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-13 14:46:55.000000 TSInterpret-0.2.9/ClassificationModels/LSTM_T.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-06-13 14:46:55.000000 TSInterpret-0.2.9/ClassificationModels/ResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:46:55.000000 TSInterpret-0.2.9/ClassificationModels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/ClassificationModels/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-06-13 14:47:08.229413 TSInterpret-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:08.221413 TSInterpret-0.2.9/TSInterpret/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:08.221413 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/FeatureAttribution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:08.221413 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/GradCam/
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/GradCam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/InstanceBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/InterpretabilityBase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:08.221413 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/Saliency/
--rw-r--r--   0 runner    (1001) docker     (123)    16172 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py
--rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/Saliency/TSR.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/Saliency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:08.225413 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/counterfactual/
--rw-r--r--   0 runner    (1001) docker     (123)    22784 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/counterfactual/Ates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/counterfactual/CF.py
--rw-r--r--   0 runner    (1001) docker     (123)    11302 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:08.225413 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/
--rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/counterfactual/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:08.225413 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:08.225413 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/learning_process/
--rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/learning_process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:08.225413 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10995 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/leftist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/neighbors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:08.225413 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:08.229413 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:08.229413 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:08.229413 TSInterpret-0.2.9/TSInterpret/Models/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/Models/PyTorchModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/Models/SklearnModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/Models/TensorflowModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/Models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/Models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:08.221413 TSInterpret-0.2.9/TSInterpret.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-06-13 14:47:08.000000 TSInterpret-0.2.9/TSInterpret.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-06-13 14:47:08.000000 TSInterpret-0.2.9/TSInterpret.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:47:08.000000 TSInterpret-0.2.9/TSInterpret.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-06-13 14:47:08.000000 TSInterpret-0.2.9/TSInterpret.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 14:47:08.000000 TSInterpret-0.2.9/TSInterpret.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 14:47:08.229413 TSInterpret-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:56:24.220639 TSInterpret-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:56:24.212639 TSInterpret-0.3.0/ClassificationModels/
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-14 07:56:10.000000 TSInterpret-0.3.0/ClassificationModels/CNN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-06-14 07:56:10.000000 TSInterpret-0.3.0/ClassificationModels/CNN_T.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-06-14 07:56:10.000000 TSInterpret-0.3.0/ClassificationModels/DecisionTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-14 07:56:10.000000 TSInterpret-0.3.0/ClassificationModels/LSTM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-14 07:56:10.000000 TSInterpret-0.3.0/ClassificationModels/LSTM_T.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-06-14 07:56:10.000000 TSInterpret-0.3.0/ClassificationModels/ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 07:56:10.000000 TSInterpret-0.3.0/ClassificationModels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/ClassificationModels/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-06-14 07:56:24.220639 TSInterpret-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:56:24.212639 TSInterpret-0.3.0/TSInterpret/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:56:24.212639 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/FeatureAttribution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:56:24.212639 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/GradCam/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/GradCam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/InstanceBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/InterpretabilityBase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:56:24.216639 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/Saliency/
+-rw-r--r--   0 runner    (1001) docker     (123)    16172 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/Saliency/TSR.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/Saliency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:56:24.216639 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/counterfactual/
+-rw-r--r--   0 runner    (1001) docker     (123)    22784 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/counterfactual/Ates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/counterfactual/CF.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12504 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:56:24.216639 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/
+-rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/counterfactual/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:56:24.216639 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:56:24.216639 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/learning_process/
+-rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/learning_process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:56:24.216639 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10995 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/leftist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/neighbors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:56:24.216639 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:56:24.220639 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:56:24.220639 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:56:24.220639 TSInterpret-0.3.0/TSInterpret/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/Models/PyTorchModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/Models/SklearnModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/Models/TensorflowModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/Models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/TSInterpret/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:56:24.212639 TSInterpret-0.3.0/TSInterpret.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-06-14 07:56:24.000000 TSInterpret-0.3.0/TSInterpret.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-06-14 07:56:24.000000 TSInterpret-0.3.0/TSInterpret.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 07:56:24.000000 TSInterpret-0.3.0/TSInterpret.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-06-14 07:56:24.000000 TSInterpret-0.3.0/TSInterpret.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-14 07:56:24.000000 TSInterpret-0.3.0/TSInterpret.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 07:56:24.220639 TSInterpret-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-06-14 07:56:11.000000 TSInterpret-0.3.0/setup.py
```

### Comparing `TSInterpret-0.2.9/ClassificationModels/CNN.py` & `TSInterpret-0.3.0/ClassificationModels/CNN.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/ClassificationModels/CNN_T.py` & `TSInterpret-0.3.0/ClassificationModels/CNN_T.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/ClassificationModels/DecisionTree.py` & `TSInterpret-0.3.0/ClassificationModels/DecisionTree.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/ClassificationModels/LSTM.py` & `TSInterpret-0.3.0/ClassificationModels/LSTM.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/ClassificationModels/LSTM_T.py` & `TSInterpret-0.3.0/ClassificationModels/LSTM_T.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/ClassificationModels/ResNet.py` & `TSInterpret-0.3.0/ClassificationModels/ResNet.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/ClassificationModels/utils.py` & `TSInterpret-0.3.0/ClassificationModels/utils.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/LICENSE` & `TSInterpret-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/PKG-INFO` & `TSInterpret-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSInterpret
-Version: 0.2.9
+Version: 0.3.0
 Summary: todo
 Home-page: https://ipe-wim-gitlab.fzi.de/hoellig/interpretabilitytimeseries
 Author: Jacqueline Hoellig
 Author-email: hoellig@fzi.de
 License: BSD-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TSInterpret Version: 0.2.9 Summary: todo Home-page:
+Metadata-Version: 2.1 Name: TSInterpret Version: 0.3.0 Summary: todo Home-page:
 https://ipe-wim-gitlab.fzi.de/hoellig/interpretabilitytimeseries Author:
 Jacqueline Hoellig Author-email: hoellig@fzi.de License: BSD-3 Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
```

### Comparing `TSInterpret-0.2.9/README.md` & `TSInterpret-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/FeatureAttribution.py` & `TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/FeatureAttribution.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py` & `TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/InterpretabilityBase.py` & `TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/InterpretabilityBase.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py` & `TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py` & `TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py` & `TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/Saliency/TSR.py` & `TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/Saliency/TSR.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/counterfactual/Ates.py` & `TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/counterfactual/Ates.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/counterfactual/CF.py` & `TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/counterfactual/CF.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py` & `TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 """Implementation after Delaney et al . https://github.com/e-delaney/Instance-Based_CFE_TSC"""
 import warnings
 from typing import Tuple
+from collections import OrderedDict
+from typing import Dict, Callable
+
+
+import torch
 
 import numpy as np
 from torchcam.methods import CAM
 from tslearn.barycenters import dtw_barycenter_averaging
 from tslearn.neighbors import KNeighborsTimeSeries
 
 from TSInterpret.InterpretabilityModels.counterfactual.CF import CF
@@ -29,54 +34,54 @@
         Science.
     ----------
     """
 
     def __init__(
         self,
         model,
-        shape,
         data,
         backend="PYT",
         mode="feat",
         method="NUN-CF",
         distance_measure="dtw",
         n_neighbors=1,
         max_iter=500,
     ) -> None:
         """
         In this case differentiation between time & feat not necessary as implicitly given by CNN. Only works for CNNs due to the attribution methods.
         Arguments:
             model [torch.nn.Module, Callable, tf.keras.model]: classification model to explain
-            shape Tuple: input shape
             data Tuple: reference set as tuple (x,y)
             backend str: 'PYT' or  'TF'
             mode str: model either 'time' or 'feat'. `time` -> `(-1, time, feature)` or `feat` -> `(-1, feature, time)`
             method str: 'Nun_CF', 'dtw_bary_center' or 'native_guide'.
             distance_measure str: sklearn appreviation for distance of knn.
             n_neighbore int: # neighbors to select from.
             max_iter int : max number of runs
         """
         super().__init__(model, mode)
+
         self.backend = backend
         test_x, test_y = data
         test_x = np.array(test_x)  # , dtype=np.float32)
-
+        shape = (test_x.shape[-2], test_x.shape[-1])
+        print(shape)
         if mode == "time":
             # Parse test data into (1, feat, time):
-            self.ts_length = shape[-2]
+            self.ts_length = test_x.shape[-2]
             test_x = test_x.reshape(test_x.shape[0], test_x.shape[2], test_x.shape[1])
         elif mode == "feat":
-            self.ts_length = shape[-1]
+            self.ts_length = test_x.shape[-1]
 
         if backend == "PYT":
-
-            try:
-                self.cam_extractor = CAM(self.model, input_shape=(shape[1], shape[2]))
-            except:
-                print("GradCam Hook already registered")
+            self.remove_all_hooks(self.model)
+            # try:
+            self.cam_extractor = CAM(self.model, input_shape=shape)
+            # except:
+            #    print("GradCam Hook already registered")
             change = False
             if self.mode == "time":
                 change = True
             self.predict = PyTorchModel(self.model, change).predict
             y_pred = np.argmax(self.predict(test_x), axis=1)
 
         elif backend == "TF":
@@ -84,21 +89,40 @@
             y_pred = np.argmax(
                 self.model.predict(test_x.reshape(-1, self.ts_length, 1)), axis=1
             )
             self.predict = TensorFlowModel(self.model, change=True).predict
         else:
             print("Only Compatible with Tensorflow (TF) or Pytorch (PYT)!")
 
-        self.reference_set = (test_x, y_pred)
+        self.data = (test_x, y_pred)
         self.method = method
         self.distance_measure = distance_measure
         self.max_iter = max_iter
         self.n_neighbors = n_neighbors
         # Manipulate reference set replace original y with predicted y
 
+    def remove_all_hooks(self, model: torch.nn.Module) -> None:
+        # TODO Move THIS TO TSINTERPRET !
+        if hasattr(model, "_forward_hooks"):
+            if model._forward_hooks != OrderedDict():
+                model._forward_hooks: Dict[int, Callable] = OrderedDict()
+            elif hasattr(model, "_forward_pre_hooks"):
+                model._forward_pre_hooks: Dict[int, Callable] = OrderedDict()
+            elif hasattr(model, "_backward_hooks"):
+                model._backward_hooks: Dict[int, Callable] = OrderedDict()
+        for name, child in model._modules.items():
+            if child is not None:
+                if hasattr(child, "_forward_hooks"):
+                    child._forward_hooks: Dict[int, Callable] = OrderedDict()
+                elif hasattr(child, "_forward_pre_hooks"):
+                    child._forward_pre_hooks: Dict[int, Callable] = OrderedDict()
+                elif hasattr(child, "_backward_hooks"):
+                    child._backward_hooks: Dict[int, Callable] = OrderedDict()
+                self.remove_all_hooks(child)
+
     def _native_guide_retrieval(self, query, predicted_label, distance, n_neighbors):
         """
         This gets the nearest unlike neighbors.
         Arguments:
             query (np.array): The instance to explain.
             predicted_label (np.array): Label of instance.
             reference_set (np.array): Set of addtional labeled data (could be training or test set)
@@ -107,15 +131,15 @@
         Returns:
             [np.array]: Returns K_Nearest_Neighbors of input query with different classification label.
 
         """
         if type(predicted_label) != int:
             predicted_label = np.argmax(predicted_label)
 
-        x_train, y = self.reference_set
+        x_train, y = self.data
         if len(y.shape) == 2:
             y = np.argmax(y, axis=1)
         ts_length = self.ts_length
         knn = KNeighborsTimeSeries(n_neighbors=n_neighbors, metric=distance)
         knn.fit(x_train[list(np.where(y != predicted_label))].reshape(-1, ts_length, 1))
         dist, ind = knn.kneighbors(query.reshape(1, ts_length, 1), return_distance=True)
         x_train.reshape(-1, 1, ts_length)
@@ -158,15 +182,15 @@
         self, instance, label, subarray_length=1, max_iter=500
     ):
         print(label)
         _, nun = self._native_guide_retrieval(instance, label, self.distance_measure, 1)
         if np.count_nonzero(nun.reshape(-1) - instance.reshape(-1)) == 0:
             print("Starting and nun are Identical !")
 
-        test_x, test_y = self.reference_set
+        test_x, test_y = self.data
         train_x = test_x
         individual = np.array(nun.tolist())  # , dtype=np.float64)
         out = self.predict(individual)
         if self.backend == "PYT":
             training_weights = (
                 self.cam_extractor(out.squeeze(0).argmax().item(), out)[0]
                 .detach()
```

### Comparing `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py` & `TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py` & `TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py` & `TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py` & `TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py` & `TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py` & `TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py` & `TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py` & `TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py` & `TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py` & `TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py` & `TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/leftist.py` & `TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/leftist.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/neighbors.py` & `TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/neighbors.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py` & `TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py` & `TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py` & `TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py` & `TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py` & `TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py` & `TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py` & `TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py` & `TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py` & `TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/transform.py` & `TSInterpret-0.3.0/TSInterpret/InterpretabilityModels/leftist/transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret/Models/PyTorchModel.py` & `TSInterpret-0.3.0/TSInterpret/Models/PyTorchModel.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret/Models/SklearnModel.py` & `TSInterpret-0.3.0/TSInterpret/Models/SklearnModel.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret/Models/TensorflowModel.py` & `TSInterpret-0.3.0/TSInterpret/Models/TensorflowModel.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret/Models/base_model.py` & `TSInterpret-0.3.0/TSInterpret/Models/base_model.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret.egg-info/PKG-INFO` & `TSInterpret-0.3.0/TSInterpret.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSInterpret
-Version: 0.2.9
+Version: 0.3.0
 Summary: todo
 Home-page: https://ipe-wim-gitlab.fzi.de/hoellig/interpretabilitytimeseries
 Author: Jacqueline Hoellig
 Author-email: hoellig@fzi.de
 License: BSD-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TSInterpret Version: 0.2.9 Summary: todo Home-page:
+Metadata-Version: 2.1 Name: TSInterpret Version: 0.3.0 Summary: todo Home-page:
 https://ipe-wim-gitlab.fzi.de/hoellig/interpretabilitytimeseries Author:
 Jacqueline Hoellig Author-email: hoellig@fzi.de License: BSD-3 Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
```

### Comparing `TSInterpret-0.2.9/TSInterpret.egg-info/SOURCES.txt` & `TSInterpret-0.3.0/TSInterpret.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/TSInterpret.egg-info/requires.txt` & `TSInterpret-0.3.0/TSInterpret.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.9/setup.py` & `TSInterpret-0.3.0/setup.py`

 * *Files identical despite different names*

