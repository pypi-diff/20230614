# Comparing `tmp/pidgan-0.0.0.tar.gz` & `tmp/pidgan-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pidgan-0.0.0.tar", last modified: Sun Feb  5 22:20:06 2023, max compression
+gzip compressed data, was "pidgan-0.0.1.tar", last modified: Wed Jun 14 09:18:23 2023, max compression
```

## Comparing `pidgan-0.0.0.tar` & `pidgan-0.0.1.tar`

### file list

```diff
@@ -1,30 +1,148 @@
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-02-05 22:20:06.143953 pidgan-0.0.0/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)    35148 2023-02-05 20:35:00.000000 pidgan-0.0.0/LICENSE
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     1205 2023-02-05 22:20:06.143953 pidgan-0.0.0/PKG-INFO
--rw-r--r--   0 mabarbet  (1009) z5        (1470)       66 2023-02-05 22:09:01.000000 pidgan-0.0.0/README.md
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     1874 2023-02-05 22:08:44.000000 pidgan-0.0.0/pyproject.toml
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      233 2023-02-05 22:20:06.143953 pidgan-0.0.0/setup.cfg
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-02-05 22:20:06.140953 pidgan-0.0.0/src/
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-02-05 22:20:06.141953 pidgan-0.0.0/src/pidgan/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)       32 2023-02-05 20:37:27.000000 pidgan-0.0.0/src/pidgan/__init__.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-02-05 22:20:06.142953 pidgan-0.0.0/src/pidgan/callbacks/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)        0 2023-02-05 22:10:31.000000 pidgan-0.0.0/src/pidgan/callbacks/__init__.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     8285 2023-02-05 22:10:54.000000 pidgan-0.0.0/src/pidgan/callbacks/schedulers.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-02-05 22:20:06.142953 pidgan-0.0.0/src/pidgan/layers/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      197 2023-02-05 22:14:49.000000 pidgan-0.0.0/src/pidgan/layers/Discriminator.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      193 2023-02-05 22:14:27.000000 pidgan-0.0.0/src/pidgan/layers/Generator.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)       74 2023-02-05 22:15:30.000000 pidgan-0.0.0/src/pidgan/layers/__init__.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-02-05 22:20:06.143953 pidgan-0.0.0/src/pidgan/models/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     5929 2023-02-05 22:16:45.000000 pidgan-0.0.0/src/pidgan/models/BceGAN.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     7488 2023-02-05 22:16:45.000000 pidgan-0.0.0/src/pidgan/models/CramerGAN.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)    18380 2023-02-05 22:16:45.000000 pidgan-0.0.0/src/pidgan/models/GAN.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)    10770 2023-02-05 22:16:45.000000 pidgan-0.0.0/src/pidgan/models/WGAN_ALP.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     5657 2023-02-05 22:16:45.000000 pidgan-0.0.0/src/pidgan/models/WGAN_GP.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      152 2023-02-05 22:16:45.000000 pidgan-0.0.0/src/pidgan/models/__init__.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)       21 2023-02-05 22:19:47.000000 pidgan-0.0.0/src/pidgan/version.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-02-05 22:20:06.142953 pidgan-0.0.0/src/pidgan.egg-info/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     1205 2023-02-05 22:20:06.000000 pidgan-0.0.0/src/pidgan.egg-info/PKG-INFO
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      593 2023-02-05 22:20:06.000000 pidgan-0.0.0/src/pidgan.egg-info/SOURCES.txt
--rw-r--r--   0 mabarbet  (1009) z5        (1470)        1 2023-02-05 22:20:06.000000 pidgan-0.0.0/src/pidgan.egg-info/dependency_links.txt
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      221 2023-02-05 22:20:06.000000 pidgan-0.0.0/src/pidgan.egg-info/requires.txt
--rw-r--r--   0 mabarbet  (1009) z5        (1470)        7 2023-02-05 22:20:06.000000 pidgan-0.0.0/src/pidgan.egg-info/top_level.txt
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.854516 pidgan-0.0.1/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)    35148 2023-02-05 20:35:00.000000 pidgan-0.0.1/LICENSE
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     4121 2023-06-14 09:18:23.854516 pidgan-0.0.1/PKG-INFO
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     3009 2023-06-14 09:16:05.000000 pidgan-0.0.1/README.md
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     1797 2023-06-13 21:30:56.000000 pidgan-0.0.1/pyproject.toml
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      233 2023-06-14 09:18:23.854516 pidgan-0.0.1/setup.cfg
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.803516 pidgan-0.0.1/src/
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.842516 pidgan-0.0.1/src/old_pkg/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)       32 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.842516 pidgan-0.0.1/src/old_pkg/algorithms/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)        0 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/algorithms/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.843516 pidgan-0.0.1/src/old_pkg/algorithms/gan/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     5929 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/algorithms/gan/BceGAN.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     7488 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/algorithms/gan/CramerGAN.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)    18380 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/algorithms/gan/GAN.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)    10770 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/algorithms/gan/WGAN_ALP.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     5657 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/algorithms/gan/WGAN_GP.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      152 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/algorithms/gan/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.843516 pidgan-0.0.1/src/old_pkg/algorithms/norm_flow/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     5562 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/algorithms/norm_flow/LbVAE.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)        0 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/algorithms/norm_flow/NormFlow.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)        0 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/algorithms/norm_flow/VAE_NF.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)       24 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/algorithms/norm_flow/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.843516 pidgan-0.0.1/src/old_pkg/callbacks/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     1431 2023-02-05 22:54:56.000000 pidgan-0.0.1/src/old_pkg/callbacks/HopaasReporter.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      644 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/callbacks/StopWatch.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)       75 2023-02-05 22:54:56.000000 pidgan-0.0.1/src/old_pkg/callbacks/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.844516 pidgan-0.0.1/src/old_pkg/callbacks/gan/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     2096 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/callbacks/gan/HopaasModelSaver.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     2406 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/callbacks/gan/ModelSaver.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      707 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/callbacks/gan/RefereeInitializer.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      205 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/callbacks/gan/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.844516 pidgan-0.0.1/src/old_pkg/callbacks/gan/schedulers/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      951 2023-02-05 22:54:56.000000 pidgan-0.0.1/src/old_pkg/callbacks/gan/schedulers/BaseLrScheduler.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      438 2023-02-05 22:54:56.000000 pidgan-0.0.1/src/old_pkg/callbacks/gan/schedulers/ExpLrScheduler.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      437 2023-02-05 22:54:56.000000 pidgan-0.0.1/src/old_pkg/callbacks/gan/schedulers/PowLrScheduler.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      132 2023-02-05 22:54:56.000000 pidgan-0.0.1/src/old_pkg/callbacks/gan/schedulers/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.844516 pidgan-0.0.1/src/old_pkg/layers/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     2436 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/layers/AddRandomFeatures.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     2020 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/layers/Triangular.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)       90 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/layers/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.845516 pidgan-0.0.1/src/old_pkg/metrics/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     6854 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/metrics/JS_div.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     5772 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/metrics/KL_div.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     4817 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/metrics/KS_test.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)        0 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/metrics/Variance.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      207 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/metrics/__init__.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     4030 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/metrics/chi2_test.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.845516 pidgan-0.0.1/src/old_pkg/preprocessing/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     3058 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/preprocessing/LbColTransformer.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      698 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/preprocessing/WeightedQuantileTransformer.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      126 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/preprocessing/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.846516 pidgan-0.0.1/src/old_pkg/trainers/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)    10011 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/trainers/BaseTrainer.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     7681 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/trainers/DataHandler.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)    30597 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/trainers/GanTrainer.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)        0 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/trainers/NormFlowTrainer.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)    15204 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/trainers/ScikitClassifier.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)    14261 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/trainers/ScikitTrainer.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)    12307 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/trainers/TensorTrainer.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      259 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/trainers/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.847516 pidgan-0.0.1/src/old_pkg/utils/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     1306 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/utils/ParamHandler.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      353 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/utils/__init__.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     1759 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/utils/argparser.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     4218 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/utils/data_from_trees.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     3872 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/utils/getBinCounts.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     1328 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/utils/getModelSummary.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     1340 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/utils/nan_filter.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     2248 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/utils/pre_preprocessing_step.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     7442 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/utils/preprocessor.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     1279 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/utils/warn_message.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)       21 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/version.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.848516 pidgan-0.0.1/src/pidgan/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)       33 2023-06-13 10:49:46.000000 pidgan-0.0.1/src/pidgan/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.849516 pidgan-0.0.1/src/pidgan/algorithms/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     3979 2023-06-13 20:04:03.000000 pidgan-0.0.1/src/pidgan/algorithms/BceGAN.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     7739 2023-06-13 20:30:48.000000 pidgan-0.0.1/src/pidgan/algorithms/CramerGAN.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)    14532 2023-06-13 19:53:55.000000 pidgan-0.0.1/src/pidgan/algorithms/GAN.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     4413 2023-06-13 19:30:36.000000 pidgan-0.0.1/src/pidgan/algorithms/LSGAN.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     5116 2023-06-13 20:36:13.000000 pidgan-0.0.1/src/pidgan/algorithms/WGAN.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     6373 2023-06-13 20:26:51.000000 pidgan-0.0.1/src/pidgan/algorithms/WGAN_ALP.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     5521 2023-06-13 20:23:17.000000 pidgan-0.0.1/src/pidgan/algorithms/WGAN_GP.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      189 2023-06-13 19:30:41.000000 pidgan-0.0.1/src/pidgan/algorithms/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.849516 pidgan-0.0.1/src/pidgan/callbacks/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)        0 2023-06-12 11:42:13.000000 pidgan-0.0.1/src/pidgan/callbacks/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.850516 pidgan-0.0.1/src/pidgan/callbacks/schedulers/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     1823 2023-06-12 11:42:13.000000 pidgan-0.0.1/src/pidgan/callbacks/schedulers/LearnRateBaseScheduler.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     2044 2023-06-12 11:43:16.000000 pidgan-0.0.1/src/pidgan/callbacks/schedulers/LearnRateCosineDecay.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     2125 2023-06-12 11:43:21.000000 pidgan-0.0.1/src/pidgan/callbacks/schedulers/LearnRateExpDecay.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     2140 2023-06-12 11:43:27.000000 pidgan-0.0.1/src/pidgan/callbacks/schedulers/LearnRateInvTimeDecay.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     1422 2023-06-12 11:43:34.000000 pidgan-0.0.1/src/pidgan/callbacks/schedulers/LearnRatePiecewiseConstDecay.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     2177 2023-06-12 11:43:40.000000 pidgan-0.0.1/src/pidgan/callbacks/schedulers/LearnRatePolynomialDecay.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      295 2023-06-12 11:44:17.000000 pidgan-0.0.1/src/pidgan/callbacks/schedulers/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.851516 pidgan-0.0.1/src/pidgan/metrics/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      606 2023-06-13 11:36:24.000000 pidgan-0.0.1/src/pidgan/metrics/Accuracy.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      558 2023-06-12 11:43:57.000000 pidgan-0.0.1/src/pidgan/metrics/BaseMetric.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      696 2023-06-13 11:33:27.000000 pidgan-0.0.1/src/pidgan/metrics/BinaryCrossentropy.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      808 2023-06-13 11:36:24.000000 pidgan-0.0.1/src/pidgan/metrics/JSDivergence.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      526 2023-06-13 11:34:06.000000 pidgan-0.0.1/src/pidgan/metrics/KLDivergence.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      529 2023-06-13 11:34:10.000000 pidgan-0.0.1/src/pidgan/metrics/MeanAbsoluteError.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      527 2023-06-13 11:34:14.000000 pidgan-0.0.1/src/pidgan/metrics/MeanSquaredError.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      524 2023-06-13 11:34:18.000000 pidgan-0.0.1/src/pidgan/metrics/RootMeanSquaredError.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      596 2023-06-13 20:39:48.000000 pidgan-0.0.1/src/pidgan/metrics/WassersteinDistance.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      364 2023-06-12 11:43:57.000000 pidgan-0.0.1/src/pidgan/metrics/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.840516 pidgan-0.0.1/src/pidgan/optimization/
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.851516 pidgan-0.0.1/src/pidgan/optimization/callbacks/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     1661 2023-06-13 11:51:21.000000 pidgan-0.0.1/src/pidgan/optimization/callbacks/HopaasPruner.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)       39 2023-06-12 11:42:19.000000 pidgan-0.0.1/src/pidgan/optimization/callbacks/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.852516 pidgan-0.0.1/src/pidgan/optimization/scores/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      676 2023-06-12 11:46:08.000000 pidgan-0.0.1/src/pidgan/optimization/scores/BaseScore.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      210 2023-06-12 11:46:14.000000 pidgan-0.0.1/src/pidgan/optimization/scores/ChiSquare.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      973 2023-06-12 11:46:19.000000 pidgan-0.0.1/src/pidgan/optimization/scores/EMDistance.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      212 2023-06-12 11:46:24.000000 pidgan-0.0.1/src/pidgan/optimization/scores/JSDivergence.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      212 2023-06-12 11:46:30.000000 pidgan-0.0.1/src/pidgan/optimization/scores/KLDivergence.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      210 2023-06-12 11:46:35.000000 pidgan-0.0.1/src/pidgan/optimization/scores/KSDistance.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)       35 2023-06-12 11:42:19.000000 pidgan-0.0.1/src/pidgan/optimization/scores/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.852516 pidgan-0.0.1/src/pidgan/players/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)        0 2023-06-07 14:02:20.000000 pidgan-0.0.1/src/pidgan/players/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.852516 pidgan-0.0.1/src/pidgan/players/classifiers/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      164 2023-06-13 14:10:29.000000 pidgan-0.0.1/src/pidgan/players/classifiers/Classifier.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)       35 2023-06-13 14:10:43.000000 pidgan-0.0.1/src/pidgan/players/classifiers/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.852516 pidgan-0.0.1/src/pidgan/players/discriminators/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     3682 2023-06-13 19:31:15.000000 pidgan-0.0.1/src/pidgan/players/discriminators/Discriminator.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      235 2023-06-13 10:49:46.000000 pidgan-0.0.1/src/pidgan/players/discriminators/SkipDiscriminator.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)       41 2023-06-13 14:09:10.000000 pidgan-0.0.1/src/pidgan/players/discriminators/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.853516 pidgan-0.0.1/src/pidgan/players/generators/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     4320 2023-06-13 19:31:20.000000 pidgan-0.0.1/src/pidgan/players/generators/Generator.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      219 2023-06-13 10:49:46.000000 pidgan-0.0.1/src/pidgan/players/generators/SkipGenerator.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)       33 2023-06-13 19:30:36.000000 pidgan-0.0.1/src/pidgan/players/generators/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.853516 pidgan-0.0.1/src/pidgan/players/regressors/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      163 2023-06-13 14:09:36.000000 pidgan-0.0.1/src/pidgan/players/regressors/Regressor.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)       33 2023-06-13 14:09:46.000000 pidgan-0.0.1/src/pidgan/players/regressors/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.853516 pidgan-0.0.1/src/pidgan/utils/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     1409 2023-06-13 10:49:51.000000 pidgan-0.0.1/src/pidgan/utils/HPSingleton.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)       84 2023-06-12 11:37:54.000000 pidgan-0.0.1/src/pidgan/utils/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.853516 pidgan-0.0.1/src/pidgan/utils/checks/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)       82 2023-06-12 11:38:35.000000 pidgan-0.0.1/src/pidgan/utils/checks/__init__.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     2097 2023-06-12 11:39:39.000000 pidgan-0.0.1/src/pidgan/utils/checks/checkMetrics.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      816 2023-06-12 11:39:49.000000 pidgan-0.0.1/src/pidgan/utils/checks/checkOptimizer.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     1347 2023-06-13 10:49:46.000000 pidgan-0.0.1/src/pidgan/utils/getSummaryHTML.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)       22 2023-06-13 11:39:52.000000 pidgan-0.0.1/src/pidgan/version.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.848516 pidgan-0.0.1/src/pidgan.egg-info/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     4121 2023-06-14 09:18:23.000000 pidgan-0.0.1/src/pidgan.egg-info/PKG-INFO
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     4479 2023-06-14 09:18:23.000000 pidgan-0.0.1/src/pidgan.egg-info/SOURCES.txt
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)        1 2023-06-14 09:18:23.000000 pidgan-0.0.1/src/pidgan.egg-info/dependency_links.txt
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      163 2023-06-14 09:18:23.000000 pidgan-0.0.1/src/pidgan.egg-info/requires.txt
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)       15 2023-06-14 09:18:23.000000 pidgan-0.0.1/src/pidgan.egg-info/top_level.txt
```

### Comparing `pidgan-0.0.0/LICENSE` & `pidgan-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pidgan-0.0.0/pyproject.toml` & `pidgan-0.0.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
-requires = ["setuptools>=61.0"]
+requires = ["setuptools>=42.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pidgan"
 dynamic = ["version"]
 description = "GAN-based models to fast-simulate the LHCb PID detectors"
 readme = "README.md"
-requires-python = ">=3.7, <=3.10"
+requires-python = ">=3.7, <=3.11"
 license = {text = "GPLv3 License"}
 authors = [
   {name = "Matteo Barbetti", email = "matteo.barbetti@fi.infn.it"},
   {name = "Lucio Anderlini", email = "lucio.anderlini@fi.infn.it"},
 ]
 keywords = [
   "tensorflow",
@@ -26,38 +26,31 @@
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Science/Research",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
-  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "Topic :: Scientific/Engineering :: Physics",
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dependencies = [
   "tensorflow>=2.7",
+  "scikit-learn",
+  # "hopaas-client",   # to be released on PyPI
   "pyyaml"
 ]
 
 [project.optional-dependencies]
-standard = [
-  "numpy",
-  "pandas",
-  "uproot",
-  "matplotlib",
-  "scikit-learn",
-]
-advanced = [
+lamarr = [
   "numpy",
   "pandas",
   "uproot",
   "matplotlib",
-  "scikit-learn",
-  # "hopaas-client",   # to be released on PyPI
   "html-reports>=0.2",
 ]
 style = [
   "black",
   "flake8",
   "isort[colors]",
 ]
@@ -69,15 +62,15 @@
 [project.urls]
 repository = "https://github.com/mbarbetti/pidgan"
 
 [tool.setuptools.dynamic]
 version = {attr = "pidgan.__version__"}
 
 [tool.black]
-target-version = ["py37", "py38", "py39", "py310"]
+target-version = ["py37", "py38", "py39", "py310", "py311"]
 color = true
 skip_magic_trailing_comma = true
 
 [tool.isort]
 profile = "black"
 known_first_party = ["src", "tests"]
 skip_gitignore = true
```

### Comparing `pidgan-0.0.0/src/pidgan/models/BceGAN.py` & `pidgan-0.0.1/src/old_pkg/algorithms/gan/BceGAN.py`

 * *Files identical despite different names*

### Comparing `pidgan-0.0.0/src/pidgan/models/CramerGAN.py` & `pidgan-0.0.1/src/old_pkg/algorithms/gan/CramerGAN.py`

 * *Files identical despite different names*

### Comparing `pidgan-0.0.0/src/pidgan/models/GAN.py` & `pidgan-0.0.1/src/old_pkg/algorithms/gan/GAN.py`

 * *Files identical despite different names*

### Comparing `pidgan-0.0.0/src/pidgan/models/WGAN_ALP.py` & `pidgan-0.0.1/src/old_pkg/algorithms/gan/WGAN_ALP.py`

 * *Files identical despite different names*

### Comparing `pidgan-0.0.0/src/pidgan/models/WGAN_GP.py` & `pidgan-0.0.1/src/old_pkg/algorithms/gan/WGAN_GP.py`

 * *Files identical despite different names*

