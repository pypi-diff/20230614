# Comparing `tmp/nkululeko-0.47.1.tar.gz` & `tmp/nkululeko-0.48.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkululeko-0.47.1.tar", last modified: Tue Jun 13 14:42:07 2023, max compression
+gzip compressed data, was "nkululeko-0.48.0.tar", last modified: Wed Jun 14 15:18:45 2023, max compression
```

## Comparing `nkululeko-0.47.1.tar` & `nkululeko-0.48.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-06-13 14:42:07.844685 nkululeko-0.47.1/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6308 2023-06-13 14:23:01.000000 nkululeko-0.47.1/CHANGELOG.md
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.47.1/LICENSE
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18034 2023-06-13 14:42:07.844685 nkululeko-0.47.1/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11173 2023-06-13 13:36:10.000000 nkululeko-0.47.1/README.md
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-06-13 14:42:07.844685 nkululeko-0.47.1/nkululeko/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-05-22 09:01:23.000000 nkululeko-0.47.1/nkululeko/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1385 2023-03-07 15:26:22.000000 nkululeko-0.47.1/nkululeko/augment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2399 2023-03-23 15:05:56.000000 nkululeko-0.47.1/nkululeko/augmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       12 2023-01-14 20:36:15.000000 nkululeko-0.47.1/nkululeko/balancer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      955 2023-01-16 11:55:06.000000 nkululeko-0.47.1/nkululeko/cacheddataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       18 2023-06-13 14:22:23.000000 nkululeko-0.47.1/nkululeko/constants.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21627 2023-05-23 12:23:55.000000 nkululeko-0.47.1/nkululeko/dataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2042 2023-05-23 11:18:28.000000 nkululeko-0.47.1/nkululeko/dataset_csv.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      537 2023-01-16 11:56:12.000000 nkululeko-0.47.1/nkululeko/dataset_ravdess.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1815 2023-05-11 13:37:47.000000 nkululeko-0.47.1/nkululeko/demo.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2286 2023-02-15 16:29:45.000000 nkululeko-0.47.1/nkululeko/demo_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    20319 2023-05-23 12:09:53.000000 nkululeko-0.47.1/nkululeko/experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1960 2023-05-11 13:37:32.000000 nkululeko-0.47.1/nkululeko/explore.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3821 2023-05-23 12:00:29.000000 nkululeko-0.47.1/nkululeko/feats_analyser.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2748 2023-05-04 14:30:28.000000 nkululeko-0.47.1/nkululeko/feats_audmodel.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2739 2023-05-04 14:30:21.000000 nkululeko-0.47.1/nkululeko/feats_audmodel_dim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3250 2023-05-04 14:30:36.000000 nkululeko-0.47.1/nkululeko/feats_clap.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2045 2023-05-04 14:08:00.000000 nkululeko-0.47.1/nkululeko/feats_import.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1949 2023-02-09 11:57:32.000000 nkululeko-0.47.1/nkululeko/feats_mld.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2871 2023-06-13 14:22:08.000000 nkululeko-0.47.1/nkululeko/feats_opensmile.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4425 2023-02-09 12:00:41.000000 nkululeko-0.47.1/nkululeko/feats_oxbow.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2130 2023-05-23 11:53:38.000000 nkululeko-0.47.1/nkululeko/feats_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2975 2023-04-19 20:26:13.000000 nkululeko-0.47.1/nkululeko/feats_trill.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4005 2023-02-09 12:01:59.000000 nkululeko-0.47.1/nkululeko/feats_wav2vec2.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3456 2023-05-04 13:43:15.000000 nkululeko-0.47.1/nkululeko/feature_extractor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1319 2023-02-28 14:54:13.000000 nkululeko-0.47.1/nkululeko/featureset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    19509 2023-05-25 16:45:46.000000 nkululeko-0.47.1/nkululeko/feinberg_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1821 2023-01-16 12:04:04.000000 nkululeko-0.47.1/nkululeko/filter_data.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      237 2023-01-16 11:49:55.000000 nkululeko-0.47.1/nkululeko/glob_conf.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      939 2023-01-14 20:36:15.000000 nkululeko-0.47.1/nkululeko/loss_ccc.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1329 2023-01-14 20:36:15.000000 nkululeko-0.47.1/nkululeko/loss_softf1loss.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12074 2023-02-20 12:50:06.000000 nkululeko-0.47.1/nkululeko/model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      432 2023-03-24 08:08:57.000000 nkululeko-0.47.1/nkululeko/model_bayes.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5029 2023-03-24 08:09:03.000000 nkululeko-0.47.1/nkululeko/model_cnn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      603 2023-03-24 08:09:21.000000 nkululeko-0.47.1/nkululeko/model_gmm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      544 2023-03-24 08:10:02.000000 nkululeko-0.47.1/nkululeko/model_knn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      551 2023-03-24 08:09:46.000000 nkululeko-0.47.1/nkululeko/model_knn_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8007 2023-03-24 08:10:19.000000 nkululeko-0.47.1/nkululeko/model_mlp.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8781 2023-03-24 08:10:12.000000 nkululeko-0.47.1/nkululeko/model_mlp_regression.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      522 2023-03-24 08:10:26.000000 nkululeko-0.47.1/nkululeko/model_svm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      505 2023-03-24 08:10:49.000000 nkululeko-0.47.1/nkululeko/model_svr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      382 2023-03-24 08:11:15.000000 nkululeko-0.47.1/nkululeko/model_tree.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      389 2023-03-24 08:10:58.000000 nkululeko-0.47.1/nkululeko/model_tree_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      236 2023-03-24 08:11:22.000000 nkululeko-0.47.1/nkululeko/model_xgb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      242 2023-03-24 08:11:33.000000 nkululeko-0.47.1/nkululeko/model_xgr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5367 2023-03-24 08:13:41.000000 nkululeko-0.47.1/nkululeko/modelrunner.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1540 2023-05-11 13:36:48.000000 nkululeko-0.47.1/nkululeko/nkululeko.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6554 2023-05-23 12:04:34.000000 nkululeko-0.47.1/nkululeko/plots.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10167 2023-05-23 12:24:23.000000 nkululeko-0.47.1/nkululeko/reporter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2023-01-16 11:15:47.000000 nkululeko-0.47.1/nkululeko/result.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6753 2023-02-20 11:58:56.000000 nkululeko-0.47.1/nkululeko/runmanager.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3013 2023-01-16 11:17:07.000000 nkululeko-0.47.1/nkululeko/scaler.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9913 2023-05-25 14:35:43.000000 nkululeko-0.47.1/nkululeko/syllable_nuclei.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1366 2023-05-11 13:41:29.000000 nkululeko-0.47.1/nkululeko/test.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2315 2023-01-16 12:10:32.000000 nkululeko-0.47.1/nkululeko/test_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8967 2023-05-23 11:38:09.000000 nkululeko-0.47.1/nkululeko/util.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-06-13 14:42:07.844685 nkululeko-0.47.1/nkululeko.egg-info/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18034 2023-06-13 14:42:07.000000 nkululeko-0.47.1/nkululeko.egg-info/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1594 2023-06-13 14:42:07.000000 nkululeko-0.47.1/nkululeko.egg-info/SOURCES.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2023-06-13 14:42:07.000000 nkululeko-0.47.1/nkululeko.egg-info/dependency_links.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      259 2023-06-13 14:42:07.000000 nkululeko-0.47.1/nkululeko.egg-info/requires.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2023-06-13 14:42:07.000000 nkululeko-0.47.1/nkululeko.egg-info/top_level.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.47.1/pyproject.toml
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      959 2023-06-13 14:42:07.844685 nkululeko-0.47.1/setup.cfg
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.47.1/setup.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-06-14 15:18:45.754056 nkululeko-0.48.0/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6409 2023-06-14 15:12:40.000000 nkululeko-0.48.0/CHANGELOG.md
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.48.0/LICENSE
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18135 2023-06-14 15:18:45.754056 nkululeko-0.48.0/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11173 2023-06-13 13:36:10.000000 nkululeko-0.48.0/README.md
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-06-14 15:18:45.754056 nkululeko-0.48.0/nkululeko/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-05-22 09:01:23.000000 nkululeko-0.48.0/nkululeko/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1385 2023-03-07 15:26:22.000000 nkululeko-0.48.0/nkululeko/augment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2399 2023-03-23 15:05:56.000000 nkululeko-0.48.0/nkululeko/augmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       12 2023-01-14 20:36:15.000000 nkululeko-0.48.0/nkululeko/balancer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      955 2023-01-16 11:55:06.000000 nkululeko-0.48.0/nkululeko/cacheddataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       18 2023-06-14 14:21:07.000000 nkululeko-0.48.0/nkululeko/constants.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21627 2023-05-23 12:23:55.000000 nkululeko-0.48.0/nkululeko/dataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2042 2023-05-23 11:18:28.000000 nkululeko-0.48.0/nkululeko/dataset_csv.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      537 2023-01-16 11:56:12.000000 nkululeko-0.48.0/nkululeko/dataset_ravdess.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1815 2023-05-11 13:37:47.000000 nkululeko-0.48.0/nkululeko/demo.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2286 2023-02-15 16:29:45.000000 nkululeko-0.48.0/nkululeko/demo_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    20319 2023-05-23 12:09:53.000000 nkululeko-0.48.0/nkululeko/experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1960 2023-05-11 13:37:32.000000 nkululeko-0.48.0/nkululeko/explore.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3821 2023-05-23 12:00:29.000000 nkululeko-0.48.0/nkululeko/feats_analyser.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2748 2023-05-04 14:30:28.000000 nkululeko-0.48.0/nkululeko/feats_audmodel.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2739 2023-05-04 14:30:21.000000 nkululeko-0.48.0/nkululeko/feats_audmodel_dim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3250 2023-05-04 14:30:36.000000 nkululeko-0.48.0/nkululeko/feats_clap.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2045 2023-05-04 14:08:00.000000 nkululeko-0.48.0/nkululeko/feats_import.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1949 2023-02-09 11:57:32.000000 nkululeko-0.48.0/nkululeko/feats_mld.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3756 2023-06-14 14:33:20.000000 nkululeko-0.48.0/nkululeko/feats_opensmile.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4425 2023-02-09 12:00:41.000000 nkululeko-0.48.0/nkululeko/feats_oxbow.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3012 2023-06-14 14:32:32.000000 nkululeko-0.48.0/nkululeko/feats_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2975 2023-04-19 20:26:13.000000 nkululeko-0.48.0/nkululeko/feats_trill.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4005 2023-02-09 12:01:59.000000 nkululeko-0.48.0/nkululeko/feats_wav2vec2.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3456 2023-05-04 13:43:15.000000 nkululeko-0.48.0/nkululeko/feature_extractor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1319 2023-02-28 14:54:13.000000 nkululeko-0.48.0/nkululeko/featureset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    19509 2023-05-25 16:45:46.000000 nkululeko-0.48.0/nkululeko/feinberg_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1821 2023-01-16 12:04:04.000000 nkululeko-0.48.0/nkululeko/filter_data.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      237 2023-01-16 11:49:55.000000 nkululeko-0.48.0/nkululeko/glob_conf.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      939 2023-01-14 20:36:15.000000 nkululeko-0.48.0/nkululeko/loss_ccc.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1329 2023-01-14 20:36:15.000000 nkululeko-0.48.0/nkululeko/loss_softf1loss.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12074 2023-02-20 12:50:06.000000 nkululeko-0.48.0/nkululeko/model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      432 2023-03-24 08:08:57.000000 nkululeko-0.48.0/nkululeko/model_bayes.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5029 2023-03-24 08:09:03.000000 nkululeko-0.48.0/nkululeko/model_cnn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      603 2023-03-24 08:09:21.000000 nkululeko-0.48.0/nkululeko/model_gmm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      544 2023-03-24 08:10:02.000000 nkululeko-0.48.0/nkululeko/model_knn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      551 2023-03-24 08:09:46.000000 nkululeko-0.48.0/nkululeko/model_knn_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8007 2023-03-24 08:10:19.000000 nkululeko-0.48.0/nkululeko/model_mlp.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8781 2023-03-24 08:10:12.000000 nkululeko-0.48.0/nkululeko/model_mlp_regression.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      522 2023-03-24 08:10:26.000000 nkululeko-0.48.0/nkululeko/model_svm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      505 2023-03-24 08:10:49.000000 nkululeko-0.48.0/nkululeko/model_svr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      382 2023-03-24 08:11:15.000000 nkululeko-0.48.0/nkululeko/model_tree.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      389 2023-03-24 08:10:58.000000 nkululeko-0.48.0/nkululeko/model_tree_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      236 2023-03-24 08:11:22.000000 nkululeko-0.48.0/nkululeko/model_xgb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      242 2023-03-24 08:11:33.000000 nkululeko-0.48.0/nkululeko/model_xgr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5367 2023-03-24 08:13:41.000000 nkululeko-0.48.0/nkululeko/modelrunner.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1540 2023-05-11 13:36:48.000000 nkululeko-0.48.0/nkululeko/nkululeko.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6554 2023-05-23 12:04:34.000000 nkululeko-0.48.0/nkululeko/plots.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10167 2023-05-23 12:24:23.000000 nkululeko-0.48.0/nkululeko/reporter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2023-01-16 11:15:47.000000 nkululeko-0.48.0/nkululeko/result.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6753 2023-02-20 11:58:56.000000 nkululeko-0.48.0/nkululeko/runmanager.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3013 2023-01-16 11:17:07.000000 nkululeko-0.48.0/nkululeko/scaler.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9913 2023-05-25 14:35:43.000000 nkululeko-0.48.0/nkululeko/syllable_nuclei.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1366 2023-05-11 13:41:29.000000 nkululeko-0.48.0/nkululeko/test.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2315 2023-01-16 12:10:32.000000 nkululeko-0.48.0/nkululeko/test_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8967 2023-05-23 11:38:09.000000 nkululeko-0.48.0/nkululeko/util.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-06-14 15:18:45.754056 nkululeko-0.48.0/nkululeko.egg-info/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18135 2023-06-14 15:18:45.000000 nkululeko-0.48.0/nkululeko.egg-info/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1594 2023-06-14 15:18:45.000000 nkululeko-0.48.0/nkululeko.egg-info/SOURCES.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2023-06-14 15:18:45.000000 nkululeko-0.48.0/nkululeko.egg-info/dependency_links.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      259 2023-06-14 15:18:45.000000 nkululeko-0.48.0/nkululeko.egg-info/requires.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2023-06-14 15:18:45.000000 nkululeko-0.48.0/nkululeko.egg-info/top_level.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.48.0/pyproject.toml
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      959 2023-06-14 15:18:45.754056 nkululeko-0.48.0/setup.cfg
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.48.0/setup.py
```

### Comparing `nkululeko-0.47.1/CHANGELOG.md` & `nkululeko-0.48.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+Version 0.48.0
+--------------
+* enabled specific feature selection for praat and opensmile features
+
 Version 0.47.1
 --------------
 * enabled feature storage format csv for opensmile features
 
 Version 0.47.0
 --------------
 * added praat speech rate features
```

### Comparing `nkululeko-0.47.1/LICENSE` & `nkululeko-0.48.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/PKG-INFO` & `nkululeko-0.48.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.47.1
+Version: 0.48.0
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -210,14 +210,18 @@
 
 ## License
 Nkululeko can be used under the [MIT license](https://choosealicense.com/licenses/mit/)
 
 Changelog
 =========
 
+Version 0.48.0
+--------------
+* enabled specific feature selection for praat and opensmile features
+
 Version 0.47.1
 --------------
 * enabled feature storage format csv for opensmile features
 
 Version 0.47.0
 --------------
 * added praat speech rate features
```

### Comparing `nkululeko-0.47.1/README.md` & `nkululeko-0.48.0/README.md`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/augment.py` & `nkululeko-0.48.0/nkululeko/augment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/augmenter.py` & `nkululeko-0.48.0/nkululeko/augmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/cacheddataset.py` & `nkululeko-0.48.0/nkululeko/cacheddataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/dataset.py` & `nkululeko-0.48.0/nkululeko/dataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/dataset_csv.py` & `nkululeko-0.48.0/nkululeko/dataset_csv.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/dataset_ravdess.py` & `nkululeko-0.48.0/nkululeko/dataset_ravdess.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/demo.py` & `nkululeko-0.48.0/nkululeko/demo.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/demo_predictor.py` & `nkululeko-0.48.0/nkululeko/demo_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/experiment.py` & `nkululeko-0.48.0/nkululeko/experiment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/explore.py` & `nkululeko-0.48.0/nkululeko/explore.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/feats_analyser.py` & `nkululeko-0.48.0/nkululeko/feats_analyser.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/feats_audmodel.py` & `nkululeko-0.48.0/nkululeko/feats_audmodel.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/feats_audmodel_dim.py` & `nkululeko-0.48.0/nkululeko/feats_audmodel_dim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/feats_clap.py` & `nkululeko-0.48.0/nkululeko/feats_clap.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/feats_import.py` & `nkululeko-0.48.0/nkululeko/feats_import.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/feats_mld.py` & `nkululeko-0.48.0/nkululeko/feats_mld.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/feats_opensmile.py` & `nkululeko-0.48.0/nkululeko/feats_opensmile.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # opensmileset.py
 from nkululeko.featureset import Featureset
 import opensmile
 import os
 import pandas as pd
 import nkululeko.glob_conf as glob_conf
-
+import ast
 
 class Opensmileset(Featureset):
 
     def __init__(self, name, data_df):
         super().__init__(name, data_df)
         self.featset = self.util.config_val('FEATS', 'set', 'eGeMAPSv02')
         try:
@@ -56,8 +56,29 @@
 
 
     def extract_sample(self, signal, sr):
         smile = opensmile.Smile(
                 feature_set=self.feature_set,
                 feature_level=opensmile.FeatureLevel.Functionals,)
         feats = smile.process_signal(signal, sr)
-        return feats.to_numpy()
+        return feats.to_numpy()
+    
+    def filter(self):
+        # use only the features that are indexed in the target dataframes
+        self.df = self.df[self.df.index.isin(self.data_df.index)]
+        try: 
+            # use only some features
+            selected_features = ast.literal_eval(glob_conf.config['FEATS']['os.features'])
+            self.util.debug(f'selecting features from opensmile: {selected_features}')
+            sel_feats_df = pd.DataFrame()
+            hit = False
+            for feat in selected_features:
+                try:
+                    sel_feats_df[feat] = self.df[feat]
+                    hit = True
+                except KeyError:
+                    pass
+            if hit:
+                self.df = sel_feats_df
+                self.util.debug(f'new feats shape after selecting opensmile features: {self.df.shape}')
+        except KeyError:
+            pass
```

### Comparing `nkululeko-0.47.1/nkululeko/feats_oxbow.py` & `nkululeko-0.48.0/nkululeko/feats_oxbow.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/feats_praat.py` & `nkululeko-0.48.0/nkululeko/feats_praat.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # feats_praat.py
 from nkululeko.featureset import Featureset
 import os
 import pandas as pd
 import nkululeko.glob_conf as glob_conf
 from nkululeko import feinberg_praat
+import ast
 
 class Praatset(Featureset):
     """
     a feature extractor for the Praat software, based on 
     David R. Feinberg's Praat scripts for the parselmouth python interface.
     https://osf.io/6dwr3/
 
@@ -43,8 +44,29 @@
         self.df = self.df.astype(float)
 
 
 
     def extract_sample(self, signal, sr):
         self.util.error('feats_praat: extracting single samples not implemented yet')
         feats = None
-        return feats
+        return feats
+    
+    def filter(self):
+        # use only the features that are indexed in the target dataframes
+        self.df = self.df[self.df.index.isin(self.data_df.index)]
+        try: 
+            # use only some features
+            selected_features = ast.literal_eval(glob_conf.config['FEATS']['praat.features'])
+            self.util.debug(f'selecting features from Praat: {selected_features}')
+            sel_feats_df = pd.DataFrame()
+            hit = False
+            for feat in selected_features:
+                try:
+                    sel_feats_df[feat] = self.df[feat]
+                    hit = True
+                except KeyError:
+                    pass
+            if hit:
+                self.df = sel_feats_df
+                self.util.debug(f'new feats shape after selecting Praat features: {self.df.shape}')
+        except KeyError:
+            pass
```

### Comparing `nkululeko-0.47.1/nkululeko/feats_trill.py` & `nkululeko-0.48.0/nkululeko/feats_trill.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/feats_wav2vec2.py` & `nkululeko-0.48.0/nkululeko/feats_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/feature_extractor.py` & `nkululeko-0.48.0/nkululeko/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/featureset.py` & `nkululeko-0.48.0/nkululeko/featureset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/feinberg_praat.py` & `nkululeko-0.48.0/nkululeko/feinberg_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/filter_data.py` & `nkululeko-0.48.0/nkululeko/filter_data.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/loss_ccc.py` & `nkululeko-0.48.0/nkululeko/loss_ccc.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/loss_softf1loss.py` & `nkululeko-0.48.0/nkululeko/loss_softf1loss.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/model.py` & `nkululeko-0.48.0/nkululeko/model.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/model_cnn.py` & `nkululeko-0.48.0/nkululeko/model_cnn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/model_gmm.py` & `nkululeko-0.48.0/nkululeko/model_gmm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/model_knn.py` & `nkululeko-0.48.0/nkululeko/model_knn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/model_knn_reg.py` & `nkululeko-0.48.0/nkululeko/model_knn_reg.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/model_mlp.py` & `nkululeko-0.48.0/nkululeko/model_mlp.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/model_mlp_regression.py` & `nkululeko-0.48.0/nkululeko/model_mlp_regression.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/model_svm.py` & `nkululeko-0.48.0/nkululeko/model_svm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/modelrunner.py` & `nkululeko-0.48.0/nkululeko/modelrunner.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/nkululeko.py` & `nkululeko-0.48.0/nkululeko/nkululeko.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/plots.py` & `nkululeko-0.48.0/nkululeko/plots.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/reporter.py` & `nkululeko-0.48.0/nkululeko/reporter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/runmanager.py` & `nkululeko-0.48.0/nkululeko/runmanager.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/scaler.py` & `nkululeko-0.48.0/nkululeko/scaler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/syllable_nuclei.py` & `nkululeko-0.48.0/nkululeko/syllable_nuclei.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/test.py` & `nkululeko-0.48.0/nkululeko/test.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/test_predictor.py` & `nkululeko-0.48.0/nkululeko/test_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko/util.py` & `nkululeko-0.48.0/nkululeko/util.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/nkululeko.egg-info/PKG-INFO` & `nkululeko-0.48.0/nkululeko.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.47.1
+Version: 0.48.0
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -210,14 +210,18 @@
 
 ## License
 Nkululeko can be used under the [MIT license](https://choosealicense.com/licenses/mit/)
 
 Changelog
 =========
 
+Version 0.48.0
+--------------
+* enabled specific feature selection for praat and opensmile features
+
 Version 0.47.1
 --------------
 * enabled feature storage format csv for opensmile features
 
 Version 0.47.0
 --------------
 * added praat speech rate features
```

### Comparing `nkululeko-0.47.1/nkululeko.egg-info/SOURCES.txt` & `nkululeko-0.48.0/nkululeko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nkululeko-0.47.1/setup.cfg` & `nkululeko-0.48.0/setup.cfg`

 * *Files identical despite different names*

