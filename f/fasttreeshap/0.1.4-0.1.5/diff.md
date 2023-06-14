# Comparing `tmp/fasttreeshap-0.1.4.tar.gz` & `tmp/fasttreeshap-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fasttreeshap-0.1.4.tar", last modified: Thu May 18 06:42:21 2023, max compression
+gzip compressed data, was "fasttreeshap-0.1.5.tar", last modified: Wed Jun 14 06:36:21 2023, max compression
```

## Comparing `fasttreeshap-0.1.4.tar` & `fasttreeshap-0.1.5.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-05-18 06:42:21.935241 fasttreeshap-0.1.4/
--rw-r--r--   0 jlyang   (26356) staff       (20)     1315 2021-11-05 18:22:53.000000 fasttreeshap-0.1.4/LICENSE
--rw-r--r--   0 jlyang   (26356) staff       (20)       31 2021-11-05 18:22:53.000000 fasttreeshap-0.1.4/MANIFEST.in
--rw-r--r--   0 jlyang   (26356) staff       (20)      301 2021-11-05 18:22:53.000000 fasttreeshap-0.1.4/NOTICE
--rw-r--r--   0 jlyang   (26356) staff       (20)     1149 2023-05-18 06:42:21.934740 fasttreeshap-0.1.4/PKG-INFO
--rw-r--r--   0 jlyang   (26356) staff       (20)    12973 2022-10-20 10:28:10.000000 fasttreeshap-0.1.4/README.md
-drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-05-18 06:42:21.873720 fasttreeshap-0.1.4/fasttreeshap/
--rw-r--r--   0 jlyang   (26356) staff       (20)     2154 2023-05-18 06:38:55.000000 fasttreeshap-0.1.4/fasttreeshap/__init__.py
--rw-r--r--   0 jlyang   (26356) staff       (20)    31324 2023-05-18 05:47:46.000000 fasttreeshap-0.1.4/fasttreeshap/_explanation.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     8702 2021-11-05 18:22:53.000000 fasttreeshap-0.1.4/fasttreeshap/_serializable.py
-drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-05-18 06:42:21.879672 fasttreeshap-0.1.4/fasttreeshap/cext/
--rw-r--r--   0 jlyang   (26356) staff       (20)    25950 2021-12-22 23:39:22.000000 fasttreeshap-0.1.4/fasttreeshap/cext/_cext.cc
--rw-r--r--   0 jlyang   (26356) staff       (20)    96965 2022-01-26 19:51:12.000000 fasttreeshap-0.1.4/fasttreeshap/cext/tree_shap.h
--rw-r--r--   0 jlyang   (26356) staff       (20)     9105 2023-05-18 05:47:46.000000 fasttreeshap-0.1.4/fasttreeshap/datasets.py
-drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-05-18 06:42:21.883154 fasttreeshap-0.1.4/fasttreeshap/explainers/
--rw-r--r--   0 jlyang   (26356) staff       (20)       23 2022-01-26 19:51:12.000000 fasttreeshap-0.1.4/fasttreeshap/explainers/__init__.py
--rw-r--r--   0 jlyang   (26356) staff       (20)    16708 2023-05-18 05:47:46.000000 fasttreeshap-0.1.4/fasttreeshap/explainers/_explainer.py
--rw-r--r--   0 jlyang   (26356) staff       (20)    98158 2023-05-18 05:47:46.000000 fasttreeshap-0.1.4/fasttreeshap/explainers/_tree.py
--rw-r--r--   0 jlyang   (26356) staff       (20)      443 2021-11-05 18:22:53.000000 fasttreeshap-0.1.4/fasttreeshap/links.py
-drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-05-18 06:42:21.891281 fasttreeshap-0.1.4/fasttreeshap/maskers/
--rw-r--r--   0 jlyang   (26356) staff       (20)      283 2021-12-22 23:04:49.000000 fasttreeshap-0.1.4/fasttreeshap/maskers/__init__.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     5144 2021-11-05 18:22:53.000000 fasttreeshap-0.1.4/fasttreeshap/maskers/_composite.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     1008 2021-11-05 18:22:53.000000 fasttreeshap-0.1.4/fasttreeshap/maskers/_fixed.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     2401 2021-11-05 18:22:53.000000 fasttreeshap-0.1.4/fasttreeshap/maskers/_fixed_composite.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     8218 2023-05-18 05:47:46.000000 fasttreeshap-0.1.4/fasttreeshap/maskers/_image.py
--rw-r--r--   0 jlyang   (26356) staff       (20)      753 2023-05-18 05:47:46.000000 fasttreeshap-0.1.4/fasttreeshap/maskers/_masker.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     2672 2021-11-05 18:22:53.000000 fasttreeshap-0.1.4/fasttreeshap/maskers/_output_composite.py
--rw-r--r--   0 jlyang   (26356) staff       (20)    14011 2023-05-18 05:47:46.000000 fasttreeshap-0.1.4/fasttreeshap/maskers/_tabular.py
--rw-r--r--   0 jlyang   (26356) staff       (20)    21420 2023-05-18 05:47:46.000000 fasttreeshap-0.1.4/fasttreeshap/maskers/_text.py
-drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-05-18 06:42:21.893597 fasttreeshap-0.1.4/fasttreeshap/models/
--rw-r--r--   0 jlyang   (26356) staff       (20)       26 2022-01-26 19:51:12.000000 fasttreeshap-0.1.4/fasttreeshap/models/__init__.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     1178 2021-12-21 08:43:12.000000 fasttreeshap-0.1.4/fasttreeshap/models/_model.py
-drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-05-18 06:42:21.915852 fasttreeshap-0.1.4/fasttreeshap/plots/
--rw-r--r--   0 jlyang   (26356) staff       (20)      512 2021-12-20 22:31:41.000000 fasttreeshap-0.1.4/fasttreeshap/plots/__init__.py
--rw-r--r--   0 jlyang   (26356) staff       (20)    17284 2021-11-05 18:22:53.000000 fasttreeshap-0.1.4/fasttreeshap/plots/_bar.py
--rw-r--r--   0 jlyang   (26356) staff       (20)    41053 2023-05-18 06:03:46.000000 fasttreeshap-0.1.4/fasttreeshap/plots/_beeswarm.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     8827 2021-11-05 18:22:53.000000 fasttreeshap-0.1.4/fasttreeshap/plots/_benchmark.py
--rw-r--r--   0 jlyang   (26356) staff       (20)    25998 2021-11-05 18:22:53.000000 fasttreeshap-0.1.4/fasttreeshap/plots/_decision.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     2813 2021-11-05 18:22:53.000000 fasttreeshap-0.1.4/fasttreeshap/plots/_embedding.py
--rw-r--r--   0 jlyang   (26356) staff       (20)    19403 2021-11-05 18:22:53.000000 fasttreeshap-0.1.4/fasttreeshap/plots/_force.py
--rw-r--r--   0 jlyang   (26356) staff       (20)    14787 2021-11-05 18:22:53.000000 fasttreeshap-0.1.4/fasttreeshap/plots/_force_matplotlib.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     3121 2023-05-18 05:47:46.000000 fasttreeshap-0.1.4/fasttreeshap/plots/_group_difference.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     6392 2021-11-05 18:22:53.000000 fasttreeshap-0.1.4/fasttreeshap/plots/_heatmap.py
--rw-r--r--   0 jlyang   (26356) staff       (20)    24258 2021-11-05 18:22:53.000000 fasttreeshap-0.1.4/fasttreeshap/plots/_image.py
--rw-r--r--   0 jlyang   (26356) staff       (20)      608 2021-11-05 18:22:53.000000 fasttreeshap-0.1.4/fasttreeshap/plots/_labels.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     2825 2021-11-05 18:22:53.000000 fasttreeshap-0.1.4/fasttreeshap/plots/_monitoring.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     9521 2021-11-05 18:22:53.000000 fasttreeshap-0.1.4/fasttreeshap/plots/_partial_dependence.py
--rw-r--r--   0 jlyang   (26356) staff       (20)    32609 2023-05-18 06:04:06.000000 fasttreeshap-0.1.4/fasttreeshap/plots/_scatter.py
--rw-r--r--   0 jlyang   (26356) staff       (20)    58223 2021-11-05 18:22:53.000000 fasttreeshap-0.1.4/fasttreeshap/plots/_text.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     7616 2021-11-05 18:22:53.000000 fasttreeshap-0.1.4/fasttreeshap/plots/_utils.py
--rw-r--r--   0 jlyang   (26356) staff       (20)    23938 2021-11-05 18:22:53.000000 fasttreeshap-0.1.4/fasttreeshap/plots/_violin.py
--rw-r--r--   0 jlyang   (26356) staff       (20)    26292 2021-11-05 18:22:53.000000 fasttreeshap-0.1.4/fasttreeshap/plots/_waterfall.py
-drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-05-18 06:42:21.919469 fasttreeshap-0.1.4/fasttreeshap/plots/colors/
--rw-r--r--   0 jlyang   (26356) staff       (20)      262 2021-11-05 18:22:53.000000 fasttreeshap-0.1.4/fasttreeshap/plots/colors/__init__.py
--rw-r--r--   0 jlyang   (26356) staff       (20)    36767 2021-11-05 18:22:53.000000 fasttreeshap-0.1.4/fasttreeshap/plots/colors/_colorconv.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     5096 2021-11-05 18:22:53.000000 fasttreeshap-0.1.4/fasttreeshap/plots/colors/_colors.py
-drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-05-18 06:42:21.923570 fasttreeshap-0.1.4/fasttreeshap/plots/resources/
--rw-r--r--   0 jlyang   (26356) staff       (20)   370829 2021-11-05 18:22:53.000000 fasttreeshap-0.1.4/fasttreeshap/plots/resources/bundle.js
--rw-r--r--   0 jlyang   (26356) staff       (20)      570 2021-11-05 18:22:53.000000 fasttreeshap-0.1.4/fasttreeshap/plots/resources/logoSmallGray.png
-drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-05-18 06:42:21.933594 fasttreeshap-0.1.4/fasttreeshap/utils/
--rw-r--r--   0 jlyang   (26356) staff       (20)      449 2021-11-05 18:22:53.000000 fasttreeshap-0.1.4/fasttreeshap/utils/__init__.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     8508 2021-11-05 18:22:53.000000 fasttreeshap-0.1.4/fasttreeshap/utils/_clustering.py
--rw-r--r--   0 jlyang   (26356) staff       (20)    10640 2023-05-18 05:47:46.000000 fasttreeshap-0.1.4/fasttreeshap/utils/_general.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     2576 2021-12-22 23:06:09.000000 fasttreeshap-0.1.4/fasttreeshap/utils/_keras.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     7329 2021-11-05 18:22:53.000000 fasttreeshap-0.1.4/fasttreeshap/utils/_legacy.py
--rw-r--r--   0 jlyang   (26356) staff       (20)    20509 2023-05-18 05:47:46.000000 fasttreeshap-0.1.4/fasttreeshap/utils/_masked_model.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     1227 2021-11-05 18:22:53.000000 fasttreeshap-0.1.4/fasttreeshap/utils/_show_progress.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     5552 2021-12-22 23:06:09.000000 fasttreeshap-0.1.4/fasttreeshap/utils/image.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     6494 2021-12-22 23:06:09.000000 fasttreeshap-0.1.4/fasttreeshap/utils/transformers.py
-drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-05-18 06:42:21.877828 fasttreeshap-0.1.4/fasttreeshap.egg-info/
--rwx------   0 jlyang   (26356) staff       (20)     1149 2023-05-18 06:42:21.000000 fasttreeshap-0.1.4/fasttreeshap.egg-info/PKG-INFO
--rwx------   0 jlyang   (26356) staff       (20)     2045 2023-05-18 06:42:21.000000 fasttreeshap-0.1.4/fasttreeshap.egg-info/SOURCES.txt
--rwx------   0 jlyang   (26356) staff       (20)        1 2023-05-18 06:42:21.000000 fasttreeshap-0.1.4/fasttreeshap.egg-info/dependency_links.txt
--rwx------   0 jlyang   (26356) staff       (20)        1 2021-11-04 04:21:15.000000 fasttreeshap-0.1.4/fasttreeshap.egg-info/not-zip-safe
--rwx------   0 jlyang   (26356) staff       (20)      526 2023-05-18 06:42:21.000000 fasttreeshap-0.1.4/fasttreeshap.egg-info/requires.txt
--rwx------   0 jlyang   (26356) staff       (20)       13 2023-05-18 06:42:21.000000 fasttreeshap-0.1.4/fasttreeshap.egg-info/top_level.txt
--rw-r--r--   0 jlyang   (26356) staff       (20)      115 2021-11-05 18:22:53.000000 fasttreeshap-0.1.4/pyproject.toml
--rw-r--r--   0 jlyang   (26356) staff       (20)       38 2023-05-18 06:42:21.935534 fasttreeshap-0.1.4/setup.cfg
--rw-r--r--   0 jlyang   (26356) staff       (20)     8524 2022-11-29 01:22:57.000000 fasttreeshap-0.1.4/setup.py
+drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-06-14 06:36:21.727641 fasttreeshap-0.1.5/
+-rw-r--r--   0 jlyang   (26356) staff       (20)     1315 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/LICENSE
+-rw-r--r--   0 jlyang   (26356) staff       (20)       31 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/MANIFEST.in
+-rw-r--r--   0 jlyang   (26356) staff       (20)      301 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/NOTICE
+-rw-r--r--   0 jlyang   (26356) staff       (20)     1149 2023-06-14 06:36:21.726746 fasttreeshap-0.1.5/PKG-INFO
+-rw-r--r--   0 jlyang   (26356) staff       (20)    12973 2022-10-20 10:28:10.000000 fasttreeshap-0.1.5/README.md
+drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-06-14 06:36:21.643332 fasttreeshap-0.1.5/fasttreeshap/
+-rw-r--r--   0 jlyang   (26356) staff       (20)     2154 2023-06-14 06:34:38.000000 fasttreeshap-0.1.5/fasttreeshap/__init__.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)    31324 2023-05-18 05:47:46.000000 fasttreeshap-0.1.5/fasttreeshap/_explanation.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     8702 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/_serializable.py
+drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-06-14 06:36:21.650435 fasttreeshap-0.1.5/fasttreeshap/cext/
+-rw-r--r--   0 jlyang   (26356) staff       (20)    25950 2021-12-22 23:39:22.000000 fasttreeshap-0.1.5/fasttreeshap/cext/_cext.cc
+-rw-r--r--   0 jlyang   (26356) staff       (20)    96965 2022-01-26 19:51:12.000000 fasttreeshap-0.1.5/fasttreeshap/cext/tree_shap.h
+-rw-r--r--   0 jlyang   (26356) staff       (20)     9105 2023-05-18 05:47:46.000000 fasttreeshap-0.1.5/fasttreeshap/datasets.py
+drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-06-14 06:36:21.654719 fasttreeshap-0.1.5/fasttreeshap/explainers/
+-rw-r--r--   0 jlyang   (26356) staff       (20)       23 2022-01-26 19:51:12.000000 fasttreeshap-0.1.5/fasttreeshap/explainers/__init__.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)    16708 2023-05-18 05:47:46.000000 fasttreeshap-0.1.5/fasttreeshap/explainers/_explainer.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)    98158 2023-05-18 05:47:46.000000 fasttreeshap-0.1.5/fasttreeshap/explainers/_tree.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)      433 2023-06-14 06:34:15.000000 fasttreeshap-0.1.5/fasttreeshap/links.py
+drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-06-14 06:36:21.665366 fasttreeshap-0.1.5/fasttreeshap/maskers/
+-rw-r--r--   0 jlyang   (26356) staff       (20)      283 2021-12-22 23:04:49.000000 fasttreeshap-0.1.5/fasttreeshap/maskers/__init__.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     5144 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/maskers/_composite.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     1008 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/maskers/_fixed.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     2401 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/maskers/_fixed_composite.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     8218 2023-05-18 05:47:46.000000 fasttreeshap-0.1.5/fasttreeshap/maskers/_image.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)      753 2023-05-18 05:47:46.000000 fasttreeshap-0.1.5/fasttreeshap/maskers/_masker.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     2672 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/maskers/_output_composite.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)    14014 2023-06-14 06:34:15.000000 fasttreeshap-0.1.5/fasttreeshap/maskers/_tabular.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)    21420 2023-05-18 05:47:46.000000 fasttreeshap-0.1.5/fasttreeshap/maskers/_text.py
+drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-06-14 06:36:21.668428 fasttreeshap-0.1.5/fasttreeshap/models/
+-rw-r--r--   0 jlyang   (26356) staff       (20)       26 2022-01-26 19:51:12.000000 fasttreeshap-0.1.5/fasttreeshap/models/__init__.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     1178 2021-12-21 08:43:12.000000 fasttreeshap-0.1.5/fasttreeshap/models/_model.py
+drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-06-14 06:36:21.695413 fasttreeshap-0.1.5/fasttreeshap/plots/
+-rw-r--r--   0 jlyang   (26356) staff       (20)      512 2021-12-20 22:31:41.000000 fasttreeshap-0.1.5/fasttreeshap/plots/__init__.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)    17284 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/_bar.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)    41053 2023-05-18 06:03:46.000000 fasttreeshap-0.1.5/fasttreeshap/plots/_beeswarm.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     8827 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/_benchmark.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)    25998 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/_decision.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     2813 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/_embedding.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)    19403 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/_force.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)    14787 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/_force_matplotlib.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     3121 2023-05-18 05:47:46.000000 fasttreeshap-0.1.5/fasttreeshap/plots/_group_difference.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     6392 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/_heatmap.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)    24258 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/_image.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)      608 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/_labels.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     2825 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/_monitoring.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     9521 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/_partial_dependence.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)    32609 2023-05-18 06:04:06.000000 fasttreeshap-0.1.5/fasttreeshap/plots/_scatter.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)    58223 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/_text.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     7616 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/_utils.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)    23938 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/_violin.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)    26292 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/_waterfall.py
+drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-06-14 06:36:21.701339 fasttreeshap-0.1.5/fasttreeshap/plots/colors/
+-rw-r--r--   0 jlyang   (26356) staff       (20)      262 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/colors/__init__.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)    36759 2023-05-30 19:28:57.000000 fasttreeshap-0.1.5/fasttreeshap/plots/colors/_colorconv.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     5096 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/colors/_colors.py
+drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-06-14 06:36:21.709052 fasttreeshap-0.1.5/fasttreeshap/plots/resources/
+-rw-r--r--   0 jlyang   (26356) staff       (20)   370829 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/resources/bundle.js
+-rw-r--r--   0 jlyang   (26356) staff       (20)      570 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/resources/logoSmallGray.png
+drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-06-14 06:36:21.725118 fasttreeshap-0.1.5/fasttreeshap/utils/
+-rw-r--r--   0 jlyang   (26356) staff       (20)      449 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/utils/__init__.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     8514 2023-06-14 06:34:15.000000 fasttreeshap-0.1.5/fasttreeshap/utils/_clustering.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)    10640 2023-05-18 05:47:46.000000 fasttreeshap-0.1.5/fasttreeshap/utils/_general.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     2576 2021-12-22 23:06:09.000000 fasttreeshap-0.1.5/fasttreeshap/utils/_keras.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     7329 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/utils/_legacy.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)    20513 2023-06-14 06:34:15.000000 fasttreeshap-0.1.5/fasttreeshap/utils/_masked_model.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     1227 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/utils/_show_progress.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     5552 2021-12-22 23:06:09.000000 fasttreeshap-0.1.5/fasttreeshap/utils/image.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     6494 2021-12-22 23:06:09.000000 fasttreeshap-0.1.5/fasttreeshap/utils/transformers.py
+drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-06-14 06:36:21.647973 fasttreeshap-0.1.5/fasttreeshap.egg-info/
+-rwx------   0 jlyang   (26356) staff       (20)     1149 2023-06-14 06:36:21.000000 fasttreeshap-0.1.5/fasttreeshap.egg-info/PKG-INFO
+-rwx------   0 jlyang   (26356) staff       (20)     2045 2023-06-14 06:36:21.000000 fasttreeshap-0.1.5/fasttreeshap.egg-info/SOURCES.txt
+-rwx------   0 jlyang   (26356) staff       (20)        1 2023-06-14 06:36:21.000000 fasttreeshap-0.1.5/fasttreeshap.egg-info/dependency_links.txt
+-rwx------   0 jlyang   (26356) staff       (20)        1 2021-11-04 04:21:15.000000 fasttreeshap-0.1.5/fasttreeshap.egg-info/not-zip-safe
+-rwx------   0 jlyang   (26356) staff       (20)      526 2023-06-14 06:36:21.000000 fasttreeshap-0.1.5/fasttreeshap.egg-info/requires.txt
+-rwx------   0 jlyang   (26356) staff       (20)       13 2023-06-14 06:36:21.000000 fasttreeshap-0.1.5/fasttreeshap.egg-info/top_level.txt
+-rw-r--r--   0 jlyang   (26356) staff       (20)      115 2023-05-18 18:21:26.000000 fasttreeshap-0.1.5/pyproject.toml
+-rw-r--r--   0 jlyang   (26356) staff       (20)       38 2023-06-14 06:36:21.727887 fasttreeshap-0.1.5/setup.cfg
+-rw-r--r--   0 jlyang   (26356) staff       (20)     8524 2023-05-18 18:27:08.000000 fasttreeshap-0.1.5/setup.py
```

### Comparing `fasttreeshap-0.1.4/LICENSE` & `fasttreeshap-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/PKG-INFO` & `fasttreeshap-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fasttreeshap
-Version: 0.1.4
+Version: 0.1.5
 Summary: A fast implementation of TreeSHAP algorithm.
 Home-page: http://github.com/linkedin/fasttreeshap
 Author: Jilei Yang
 Author-email: jlyang0712@gmail.com
 License: BSD 2-CLAUSE
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
```

### Comparing `fasttreeshap-0.1.4/README.md` & `fasttreeshap-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/__init__.py` & `fasttreeshap-0.1.5/fasttreeshap/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # flake8: noqa
 
 import warnings
 import sys
 
-__version__ = '0.1.4'
+__version__ = '0.1.5'
 
 # check python version
 if (sys.version_info < (3, 0)):
     warnings.warn("fasttreeshap only supports Python 3 (not 2)!")
 
 from ._explanation import Explanation, Cohorts
```

### Comparing `fasttreeshap-0.1.4/fasttreeshap/_explanation.py` & `fasttreeshap-0.1.5/fasttreeshap/_explanation.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/_serializable.py` & `fasttreeshap-0.1.5/fasttreeshap/_serializable.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/cext/_cext.cc` & `fasttreeshap-0.1.5/fasttreeshap/cext/_cext.cc`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/cext/tree_shap.h` & `fasttreeshap-0.1.5/fasttreeshap/cext/tree_shap.h`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/datasets.py` & `fasttreeshap-0.1.5/fasttreeshap/datasets.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/explainers/_explainer.py` & `fasttreeshap-0.1.5/fasttreeshap/explainers/_explainer.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/explainers/_tree.py` & `fasttreeshap-0.1.5/fasttreeshap/explainers/_tree.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/maskers/_composite.py` & `fasttreeshap-0.1.5/fasttreeshap/maskers/_composite.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/maskers/_fixed.py` & `fasttreeshap-0.1.5/fasttreeshap/maskers/_fixed.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/maskers/_fixed_composite.py` & `fasttreeshap-0.1.5/fasttreeshap/maskers/_fixed_composite.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/maskers/_image.py` & `fasttreeshap-0.1.5/fasttreeshap/maskers/_image.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/maskers/_masker.py` & `fasttreeshap-0.1.5/fasttreeshap/maskers/_masker.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/maskers/_output_composite.py` & `fasttreeshap-0.1.5/fasttreeshap/maskers/_output_composite.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/maskers/_tabular.py` & `fasttreeshap-0.1.5/fasttreeshap/maskers/_tabular.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import pandas as pd
 import numpy as np
-from numba import jit
+from numba import njit
 from .. import utils
 from ..utils import safe_isinstance, MaskedModel
 from ._masker import Masker
 from .._serializable import Serializer, Deserializer
 
 log = logging.getLogger('shap')
 
@@ -177,26 +177,26 @@
         kwargs = super().load(in_file, instantiate=False)
         with Deserializer(in_file, "shap.maskers.Tabular", min_version=0, max_version=0) as s:
             kwargs["data"] = s.load("data")
             kwargs["max_samples"] = s.load("max_samples")
             kwargs["clustering"] = s.load("clustering")
         return kwargs
 
-@jit
+@njit
 def _single_delta_mask(dind, masked_inputs, last_mask, data, x, noop_code):
     if dind == noop_code:
         pass
     elif last_mask[dind]:
         masked_inputs[:, dind] = data[:, dind]
         last_mask[dind] = False
     else:
         masked_inputs[:, dind] = x[dind]
         last_mask[dind] = True
 
-@jit
+@njit
 def _delta_masking(masks, x, curr_delta_inds, varying_rows_out,
                    masked_inputs_tmp, last_mask, data, variants, masked_inputs_out, noop_code):
     """ Implements the special (high speed) delta masking API that only flips the positions we need to.
 
     Note that we attempt to avoid doing any allocation inside this function for speed reasons.
     """
```

### Comparing `fasttreeshap-0.1.4/fasttreeshap/maskers/_text.py` & `fasttreeshap-0.1.5/fasttreeshap/maskers/_text.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/models/_model.py` & `fasttreeshap-0.1.5/fasttreeshap/models/_model.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/plots/__init__.py` & `fasttreeshap-0.1.5/fasttreeshap/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/plots/_bar.py` & `fasttreeshap-0.1.5/fasttreeshap/plots/_bar.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/plots/_beeswarm.py` & `fasttreeshap-0.1.5/fasttreeshap/plots/_beeswarm.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/plots/_benchmark.py` & `fasttreeshap-0.1.5/fasttreeshap/plots/_benchmark.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/plots/_decision.py` & `fasttreeshap-0.1.5/fasttreeshap/plots/_decision.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/plots/_embedding.py` & `fasttreeshap-0.1.5/fasttreeshap/plots/_embedding.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/plots/_force.py` & `fasttreeshap-0.1.5/fasttreeshap/plots/_force.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/plots/_force_matplotlib.py` & `fasttreeshap-0.1.5/fasttreeshap/plots/_force_matplotlib.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/plots/_group_difference.py` & `fasttreeshap-0.1.5/fasttreeshap/plots/_group_difference.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/plots/_heatmap.py` & `fasttreeshap-0.1.5/fasttreeshap/plots/_heatmap.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/plots/_image.py` & `fasttreeshap-0.1.5/fasttreeshap/plots/_image.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/plots/_labels.py` & `fasttreeshap-0.1.5/fasttreeshap/plots/_labels.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/plots/_monitoring.py` & `fasttreeshap-0.1.5/fasttreeshap/plots/_monitoring.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/plots/_partial_dependence.py` & `fasttreeshap-0.1.5/fasttreeshap/plots/_partial_dependence.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/plots/_scatter.py` & `fasttreeshap-0.1.5/fasttreeshap/plots/_scatter.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/plots/_text.py` & `fasttreeshap-0.1.5/fasttreeshap/plots/_text.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/plots/_utils.py` & `fasttreeshap-0.1.5/fasttreeshap/plots/_utils.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/plots/_violin.py` & `fasttreeshap-0.1.5/fasttreeshap/plots/_violin.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/plots/_waterfall.py` & `fasttreeshap-0.1.5/fasttreeshap/plots/_waterfall.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/plots/colors/_colorconv.py` & `fasttreeshap-0.1.5/fasttreeshap/plots/colors/_colorconv.py`

 * *Files 1% similar despite different names*

```diff
@@ -609,16 +609,16 @@
 _integer_types = (np.byte, np.ubyte,          # 8 bits
                   np.short, np.ushort,        # 16 bits
                   np.intc, np.uintc,          # 16 or 32 or 64 bits
                   np.int_, np.uint,           # 32 or 64 bits
                   np.longlong, np.ulonglong)  # 64 bits
 _integer_ranges = {t: (np.iinfo(t).min, np.iinfo(t).max)
                    for t in _integer_types}
-dtype_range = {np.bool_: (False, True),
-               np.bool8: (False, True),
+dtype_range = {bool: (False, True),
+               bool: (False, True),
                np.float16: (-1, 1),
                np.float32: (-1, 1),
                np.float64: (-1, 1)}
 dtype_range.update(_integer_ranges)
 
 _supported_types = list(dtype_range.keys())
```

### Comparing `fasttreeshap-0.1.4/fasttreeshap/plots/colors/_colors.py` & `fasttreeshap-0.1.5/fasttreeshap/plots/colors/_colors.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/plots/resources/bundle.js` & `fasttreeshap-0.1.5/fasttreeshap/plots/resources/bundle.js`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/plots/resources/logoSmallGray.png` & `fasttreeshap-0.1.5/fasttreeshap/plots/resources/logoSmallGray.png`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/utils/_clustering.py` & `fasttreeshap-0.1.5/fasttreeshap/utils/_clustering.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import scipy as sp
 from scipy.spatial.distance import pdist
-from numba import jit
+from numba import njit
 import sklearn
 import warnings
 from ._general import safe_isinstance
 from ._show_progress import show_progress
 
 
 def partition_tree(X, metric="correlation"):
@@ -27,15 +27,15 @@
 
     partition_tree: np.array
         The partition tree we should follow.
     """
     M = len(index_mask)
     #switch = np.random.randn(M) < 0
     _pt_shuffle_rec(partition_tree.shape[0]-1, indexes, index_mask, partition_tree, M, 0)
-@jit
+@njit
 def _pt_shuffle_rec(i, indexes, index_mask, partition_tree, M, pos):
     if i < 0:
         # see if we should include this index in the ordering
         if index_mask[i + M]: 
             indexes[pos] = i + M
             return pos + 1
         else:
@@ -46,38 +46,38 @@
         pos = _pt_shuffle_rec(left, indexes, index_mask, partition_tree, M, pos)
         pos = _pt_shuffle_rec(right, indexes, index_mask, partition_tree, M, pos)
     else:
         pos = _pt_shuffle_rec(right, indexes, index_mask, partition_tree, M, pos)
         pos = _pt_shuffle_rec(left, indexes, index_mask, partition_tree, M, pos)
     return pos
 
-@jit
+@njit
 def delta_minimization_order(all_masks, max_swap_size=100, num_passes=2):
     order = np.arange(len(all_masks))
     for _ in range(num_passes):
         for length in list(range(2, max_swap_size)): 
             for i in range(1, len(order)-length):
                 if _reverse_window_score_gain(all_masks, order, i, length) > 0:
                     _reverse_window(order, i, length)
     return order
-@jit
+@njit
 def _reverse_window(order, start, length):
     for i in range(length // 2):
         tmp = order[start + i]
         order[start + i] = order[start + length - i - 1]
         order[start + length - i - 1] = tmp
-@jit
+@njit
 def _reverse_window_score_gain(masks, order, start, length):
     forward_score = _mask_delta_score(masks[order[start - 1]], masks[order[start]]) + \
                     _mask_delta_score(masks[order[start + length-1]], masks[order[start + length]])
     reverse_score = _mask_delta_score(masks[order[start - 1]], masks[order[start + length-1]]) + \
                     _mask_delta_score(masks[order[start]], masks[order[start + length]])
     
     return forward_score - reverse_score
-@jit
+@njit
 def _mask_delta_score(m1, m2):
     return (m1 ^ m2).sum()
 
 
 def hclust_ordering(X, metric="sqeuclidean", anchor_first=False):
     """ A leaf ordering is under-defined, this picks the ordering that keeps nearby samples similar.
     """
```

### Comparing `fasttreeshap-0.1.4/fasttreeshap/utils/_general.py` & `fasttreeshap-0.1.5/fasttreeshap/utils/_general.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/utils/_keras.py` & `fasttreeshap-0.1.5/fasttreeshap/utils/_keras.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/utils/_legacy.py` & `fasttreeshap-0.1.5/fasttreeshap/utils/_legacy.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/utils/_masked_model.py` & `fasttreeshap-0.1.5/fasttreeshap/utils/_masked_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import copy
 import numpy as np
 import scipy.sparse
-from numba import jit
+from numba import njit
 from .. import links
 
 
 class MaskedModel():
     """ This is a utility class that combines a model, a masker object, and a current input.
 
     The combination of a model, a masker object, and a current input produces a binary set
@@ -283,15 +283,15 @@
             full_masks[i,-masks[masks_pos]-1] = ~full_masks[i,-masks[masks_pos]-1] # -value - 1 is the original index that needs flipped
             masks_pos += 1
 
         if masks[masks_pos] != MaskedModel.delta_mask_noop_value:
             full_masks[i,masks[masks_pos]] = ~full_masks[i,masks[masks_pos]]
         masks_pos += 1
 
-#@jit # TODO: figure out how to jit this function, or most of it
+#@njit # TODO: figure out how to jit this function, or most of it
 def _build_delta_masked_inputs(masks, batch_positions, num_mask_samples, num_varying_rows, delta_indexes,
                                varying_rows, args, masker, variants, variants_column_sums):
     all_masked_inputs = [[] for a in args]
     dpos = 0
     i = -1
     masks_pos = 0
     while masks_pos < len(masks):
@@ -354,15 +354,15 @@
 
 def _build_fixed_output(averaged_outs, last_outs, outputs, batch_positions, varying_rows, num_varying_rows, link, linearizing_weights):
     if len(last_outs.shape) == 1:
         _build_fixed_single_output(averaged_outs, last_outs, outputs, batch_positions, varying_rows, num_varying_rows, link, linearizing_weights)
     else:
         _build_fixed_multi_output(averaged_outs, last_outs, outputs, batch_positions, varying_rows, num_varying_rows, link, linearizing_weights)
 
-@jit # we can't use this when using a custom link function...
+@njit # we can't use this when using a custom link function...
 def _build_fixed_single_output(averaged_outs, last_outs, outputs, batch_positions, varying_rows, num_varying_rows, link, linearizing_weights):
     # here we can assume that the outputs will always be the same size, and we need
     # to carry over evaluation outputs
     sample_count = last_outs.shape[0]
     # if linearizing_weights is not None:
     #     averaged_outs[0] = np.mean(linearizing_weights * link(last_outs))
     # else:
@@ -376,15 +376,15 @@
             if linearizing_weights is not None:
                 averaged_outs[i] = np.mean(linearizing_weights * link(last_outs))
             else:
                 averaged_outs[i] = link(np.mean(last_outs))
         else:
             averaged_outs[i] = averaged_outs[i-1]
 
-@jit
+@njit
 def _build_fixed_multi_output(averaged_outs, last_outs, outputs, batch_positions, varying_rows, num_varying_rows, link, linearizing_weights):
     # here we can assume that the outputs will always be the same size, and we need
     # to carry over evaluation outputs
     sample_count = last_outs.shape[0]
     for i in range(0, len(averaged_outs)):
         if batch_positions[i] < batch_positions[i+1]:
             if num_varying_rows[i] == sample_count:
```

### Comparing `fasttreeshap-0.1.4/fasttreeshap/utils/_show_progress.py` & `fasttreeshap-0.1.5/fasttreeshap/utils/_show_progress.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/utils/image.py` & `fasttreeshap-0.1.5/fasttreeshap/utils/image.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap/utils/transformers.py` & `fasttreeshap-0.1.5/fasttreeshap/utils/transformers.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap.egg-info/PKG-INFO` & `fasttreeshap-0.1.5/fasttreeshap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fasttreeshap
-Version: 0.1.4
+Version: 0.1.5
 Summary: A fast implementation of TreeSHAP algorithm.
 Home-page: http://github.com/linkedin/fasttreeshap
 Author: Jilei Yang
 Author-email: jlyang0712@gmail.com
 License: BSD 2-CLAUSE
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
```

### Comparing `fasttreeshap-0.1.4/fasttreeshap.egg-info/SOURCES.txt` & `fasttreeshap-0.1.5/fasttreeshap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.4/fasttreeshap.egg-info/requires.txt` & `fasttreeshap-0.1.5/fasttreeshap.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -7,33 +7,33 @@
 slicer==0.0.7
 numba
 cloudpickle
 psutil
 shap
 
 [all]
-torch
-sphinx
-pytest-cov
-catboost
 xgboost
+pyspark
 transformers
+sphinx_rtd_theme
+catboost
+nbsphinx
+ipython
 numpydoc
 pytest-mpl
-lightgbm
-sphinx_rtd_theme
 matplotlib
-pyspark
-ipython
-pytest
 pyod
-nbsphinx
-opencv-python
+sphinx
 lime
+opencv-python
+pytest-cov
 sentencepiece
+lightgbm
+pytest
+torch
 
 [docs]
 matplotlib
 ipython
 numpydoc
 sphinx_rtd_theme
 sphinx
```

### Comparing `fasttreeshap-0.1.4/setup.py` & `fasttreeshap-0.1.5/setup.py`

 * *Files identical despite different names*

