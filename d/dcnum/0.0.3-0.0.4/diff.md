# Comparing `tmp/dcnum-0.0.3.tar.gz` & `tmp/dcnum-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcnum-0.0.3.tar", last modified: Tue Jun 13 11:32:22 2023, max compression
+gzip compressed data, was "dcnum-0.0.4.tar", last modified: Tue Jun 13 16:31:28 2023, max compression
```

## Comparing `dcnum-0.0.3.tar` & `dcnum-0.0.4.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:32:22.636705 dcnum-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:32:22.620705 dcnum-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:32:22.624705 dcnum-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-13 11:32:06.000000 dcnum-0.0.3/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-13 11:32:06.000000 dcnum-0.0.3/.github/workflows/deploy_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-13 11:32:06.000000 dcnum-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-13 11:32:06.000000 dcnum-0.0.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-13 11:32:06.000000 dcnum-0.0.3/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-13 11:32:06.000000 dcnum-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-13 11:32:22.636705 dcnum-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-13 11:32:06.000000 dcnum-0.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:32:22.624705 dcnum-0.0.3/dcnum/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 11:32:22.000000 dcnum-0.0.3/dcnum/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:32:22.628705 dcnum-0.0.3/dcnum/feat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/feat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:32:22.628705 dcnum-0.0.3/dcnum/feat/background/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/feat/background/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/feat/background/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/feat/background/bg_roll_median.py
--rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/feat/background/bg_sparse_median.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:32:22.628705 dcnum-0.0.3/dcnum/feat/brightness/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/feat/brightness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/feat/brightness/bright_all.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:32:22.628705 dcnum-0.0.3/dcnum/feat/haralick/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/feat/haralick/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/feat/haralick/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/feat/haralick/tex_all.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:32:22.628705 dcnum-0.0.3/dcnum/feat/moments/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/feat/moments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/feat/moments/ct_opencv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/feat/moments/mt_legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:32:22.628705 dcnum-0.0.3/dcnum/meta/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/meta/ppid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:32:22.632705 dcnum-0.0.3/dcnum/read/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/read/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/read/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/read/hdf5_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:32:22.632705 dcnum-0.0.3/dcnum/segm/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/segm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/segm/segm_thresh.py
--rw-r--r--   0 runner    (1001) docker     (123)    17565 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/segm/segmenter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:32:22.628705 dcnum-0.0.3/dcnum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-13 11:32:22.000000 dcnum-0.0.3/dcnum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-06-13 11:32:22.000000 dcnum-0.0.3/dcnum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 11:32:22.000000 dcnum-0.0.3/dcnum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-13 11:32:22.000000 dcnum-0.0.3/dcnum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-13 11:32:22.000000 dcnum-0.0.3/dcnum.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:32:22.632705 dcnum-0.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-13 11:32:06.000000 dcnum-0.0.3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:32:22.632705 dcnum-0.0.3/docs/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-13 11:32:06.000000 dcnum-0.0.3/docs/extensions/github_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-13 11:32:06.000000 dcnum-0.0.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-13 11:32:06.000000 dcnum-0.0.3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-13 11:32:06.000000 dcnum-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 11:32:22.636705 dcnum-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:32:22.636705 dcnum-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-13 11:32:06.000000 dcnum-0.0.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:32:22.636705 dcnum-0.0.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   650653 2023-06-13 11:32:06.000000 dcnum-0.0.3/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
--rw-r--r--   0 runner    (1001) docker     (123)   154010 2023-06-13 11:32:06.000000 dcnum-0.0.3/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-13 11:32:06.000000 dcnum-0.0.3/tests/helper_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-13 11:32:06.000000 dcnum-0.0.3/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-13 11:32:06.000000 dcnum-0.0.3/tests/test_feat_background_bg_roll_median.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-13 11:32:06.000000 dcnum-0.0.3/tests/test_feat_brightness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-13 11:32:06.000000 dcnum-0.0.3/tests/test_feat_haralick.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-13 11:32:06.000000 dcnum-0.0.3/tests/test_feat_moments_based.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-13 11:32:06.000000 dcnum-0.0.3/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-13 11:32:06.000000 dcnum-0.0.3/tests/test_ppid.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-13 11:32:06.000000 dcnum-0.0.3/tests/test_ppid_segm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-06-13 11:32:06.000000 dcnum-0.0.3/tests/test_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-06-13 11:32:06.000000 dcnum-0.0.3/tests/test_segm_thresh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:31:28.587839 dcnum-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:31:28.579838 dcnum-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:31:28.579838 dcnum-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-13 16:31:16.000000 dcnum-0.0.4/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-13 16:31:16.000000 dcnum-0.0.4/.github/workflows/deploy_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-13 16:31:16.000000 dcnum-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-13 16:31:16.000000 dcnum-0.0.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-13 16:31:16.000000 dcnum-0.0.4/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-13 16:31:16.000000 dcnum-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-13 16:31:28.587839 dcnum-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-13 16:31:16.000000 dcnum-0.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:31:28.579838 dcnum-0.0.4/dcnum/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-13 16:31:16.000000 dcnum-0.0.4/dcnum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 16:31:28.000000 dcnum-0.0.4/dcnum/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:31:28.579838 dcnum-0.0.4/dcnum/feat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:31:16.000000 dcnum-0.0.4/dcnum/feat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:31:28.583839 dcnum-0.0.4/dcnum/feat/background/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-13 16:31:16.000000 dcnum-0.0.4/dcnum/feat/background/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-06-13 16:31:16.000000 dcnum-0.0.4/dcnum/feat/background/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-06-13 16:31:16.000000 dcnum-0.0.4/dcnum/feat/background/bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-06-13 16:31:16.000000 dcnum-0.0.4/dcnum/feat/background/bg_sparse_median.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:31:28.583839 dcnum-0.0.4/dcnum/feat/brightness/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-13 16:31:16.000000 dcnum-0.0.4/dcnum/feat/brightness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-13 16:31:16.000000 dcnum-0.0.4/dcnum/feat/brightness/bright_all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:31:28.583839 dcnum-0.0.4/dcnum/feat/haralick/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-13 16:31:16.000000 dcnum-0.0.4/dcnum/feat/haralick/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-13 16:31:16.000000 dcnum-0.0.4/dcnum/feat/haralick/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-13 16:31:16.000000 dcnum-0.0.4/dcnum/feat/haralick/tex_all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:31:28.583839 dcnum-0.0.4/dcnum/feat/moments/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-13 16:31:16.000000 dcnum-0.0.4/dcnum/feat/moments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-13 16:31:16.000000 dcnum-0.0.4/dcnum/feat/moments/ct_opencv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-13 16:31:16.000000 dcnum-0.0.4/dcnum/feat/moments/mt_legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:31:28.583839 dcnum-0.0.4/dcnum/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-13 16:31:16.000000 dcnum-0.0.4/dcnum/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-06-13 16:31:16.000000 dcnum-0.0.4/dcnum/meta/ppid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:31:28.583839 dcnum-0.0.4/dcnum/read/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-13 16:31:16.000000 dcnum-0.0.4/dcnum/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-13 16:31:16.000000 dcnum-0.0.4/dcnum/read/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-13 16:31:16.000000 dcnum-0.0.4/dcnum/read/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-06-13 16:31:16.000000 dcnum-0.0.4/dcnum/read/hdf5_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:31:28.583839 dcnum-0.0.4/dcnum/segm/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-13 16:31:16.000000 dcnum-0.0.4/dcnum/segm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-13 16:31:16.000000 dcnum-0.0.4/dcnum/segm/segm_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17565 2023-06-13 16:31:16.000000 dcnum-0.0.4/dcnum/segm/segmenter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:31:28.579838 dcnum-0.0.4/dcnum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-13 16:31:28.000000 dcnum-0.0.4/dcnum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-13 16:31:28.000000 dcnum-0.0.4/dcnum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:31:28.000000 dcnum-0.0.4/dcnum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-13 16:31:28.000000 dcnum-0.0.4/dcnum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-13 16:31:28.000000 dcnum-0.0.4/dcnum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:31:28.583839 dcnum-0.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-13 16:31:16.000000 dcnum-0.0.4/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:31:28.583839 dcnum-0.0.4/docs/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-13 16:31:16.000000 dcnum-0.0.4/docs/extensions/github_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-13 16:31:16.000000 dcnum-0.0.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-13 16:31:16.000000 dcnum-0.0.4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-13 16:31:16.000000 dcnum-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 16:31:28.587839 dcnum-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:31:28.583839 dcnum-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-13 16:31:16.000000 dcnum-0.0.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:31:28.587839 dcnum-0.0.4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   650653 2023-06-13 16:31:16.000000 dcnum-0.0.4/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (123)   154010 2023-06-13 16:31:16.000000 dcnum-0.0.4/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-13 16:31:16.000000 dcnum-0.0.4/tests/helper_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-13 16:31:16.000000 dcnum-0.0.4/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-13 16:31:16.000000 dcnum-0.0.4/tests/test_feat_background_bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-13 16:31:16.000000 dcnum-0.0.4/tests/test_feat_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-13 16:31:16.000000 dcnum-0.0.4/tests/test_feat_haralick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-13 16:31:16.000000 dcnum-0.0.4/tests/test_feat_moments_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-13 16:31:16.000000 dcnum-0.0.4/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-13 16:31:16.000000 dcnum-0.0.4/tests/test_ppid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-13 16:31:16.000000 dcnum-0.0.4/tests/test_ppid_segm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-13 16:31:16.000000 dcnum-0.0.4/tests/test_read_concat_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-06-13 16:31:16.000000 dcnum-0.0.4/tests/test_read_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-06-13 16:31:16.000000 dcnum-0.0.4/tests/test_segm_thresh.py
```

### Comparing `dcnum-0.0.3/.github/workflows/check.yml` & `dcnum-0.0.4/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.3/.github/workflows/deploy_pypi.yml` & `dcnum-0.0.4/.github/workflows/deploy_pypi.yml`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.3/.gitignore` & `dcnum-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.3/LICENSE` & `dcnum-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.3/PKG-INFO` & `dcnum-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.0.3
+Version: 0.0.4
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
```

### Comparing `dcnum-0.0.3/README.rst` & `dcnum-0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.3/dcnum/feat/background/base.py` & `dcnum-0.0.4/dcnum/feat/background/base.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.3/dcnum/feat/background/bg_roll_median.py` & `dcnum-0.0.4/dcnum/feat/background/bg_roll_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.3/dcnum/feat/background/bg_sparse_median.py` & `dcnum-0.0.4/dcnum/feat/background/bg_sparse_median.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
             if "frame" in self.h5in["/events"]:
                 # compute time from frame rate and frame numbers
                 self.time = self.h5in["/events/frame"] / fr
                 self.time -= self.time[0]
             else:
                 # compute time using frame rate (approximate)
                 dur = self.event_count / fr * 1.5
-                logger.info(f"Approximating duration: {dur / 60:.1fmin}")
+                logger.info(f"Approximating duration: {dur / 60:.1f}min")
                 self.time = np.linspace(0, dur, self.event_count)
         else:
             # make an educated guess
             dur = self.event_count / 3600 * 1.5
             logger.info(f"Guessing duration: {dur/60:.1fmin}")
             self.time = np.linspace(0, dur, self.event_count)
```

### Comparing `dcnum-0.0.3/dcnum/feat/brightness/bright_all.py` & `dcnum-0.0.4/dcnum/feat/brightness/bright_all.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.3/dcnum/feat/haralick/tex_all.py` & `dcnum-0.0.4/dcnum/feat/haralick/tex_all.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.3/dcnum/feat/moments/ct_opencv.py` & `dcnum-0.0.4/dcnum/feat/moments/ct_opencv.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.3/dcnum/feat/moments/mt_legacy.py` & `dcnum-0.0.4/dcnum/feat/moments/mt_legacy.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.3/dcnum/meta/ppid.py` & `dcnum-0.0.4/dcnum/meta/ppid.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.3/dcnum/read/cache.py` & `dcnum-0.0.4/dcnum/read/cache.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.3/dcnum/segm/segm_thresh.py` & `dcnum-0.0.4/dcnum/segm/segm_thresh.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.3/dcnum/segm/segmenter.py` & `dcnum-0.0.4/dcnum/segm/segmenter.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.3/dcnum.egg-info/PKG-INFO` & `dcnum-0.0.4/dcnum.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.0.3
+Version: 0.0.4
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
```

### Comparing `dcnum-0.0.3/dcnum.egg-info/SOURCES.txt` & `dcnum-0.0.4/dcnum.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -45,11 +45,12 @@
 tests/test_feat_background_bg_roll_median.py
 tests/test_feat_brightness.py
 tests/test_feat_haralick.py
 tests/test_feat_moments_based.py
 tests/test_init.py
 tests/test_ppid.py
 tests/test_ppid_segm.py
-tests/test_read.py
+tests/test_read_concat_hdf5.py
+tests/test_read_hdf5.py
 tests/test_segm_thresh.py
 tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
 tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
```

### Comparing `dcnum-0.0.3/docs/conf.py` & `dcnum-0.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.3/docs/extensions/github_changelog.py` & `dcnum-0.0.4/docs/extensions/github_changelog.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.3/pyproject.toml` & `dcnum-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.3/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip` & `dcnum-0.0.4/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.3/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip` & `dcnum-0.0.4/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.3/tests/helper_methods.py` & `dcnum-0.0.4/tests/helper_methods.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.3/tests/test_feat_background_bg_roll_median.py` & `dcnum-0.0.4/tests/test_feat_background_bg_roll_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.3/tests/test_feat_brightness.py` & `dcnum-0.0.4/tests/test_feat_brightness.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.3/tests/test_feat_haralick.py` & `dcnum-0.0.4/tests/test_feat_haralick.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.3/tests/test_feat_moments_based.py` & `dcnum-0.0.4/tests/test_feat_moments_based.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.3/tests/test_ppid.py` & `dcnum-0.0.4/tests/test_ppid.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.3/tests/test_read.py` & `dcnum-0.0.4/tests/test_read_hdf5.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.3/tests/test_segm_thresh.py` & `dcnum-0.0.4/tests/test_segm_thresh.py`

 * *Files identical despite different names*

