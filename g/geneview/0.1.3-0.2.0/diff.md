# Comparing `tmp/geneview-0.1.3.tar.gz` & `tmp/geneview-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/geneview-0.1.3.tar", last modified: Thu Jun 23 13:01:54 2022, max compression
+gzip compressed data, was "dist/geneview-0.2.0.tar", last modified: Wed Jun 14 02:16:55 2023, max compression
```

## Comparing `geneview-0.1.3.tar` & `geneview-0.2.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2022-06-23 13:01:54.214746 geneview-0.1.3/
--rw-r--r--   0 huangshujia   (501) staff       (20)    15605 2022-06-23 13:01:54.213809 geneview-0.1.3/PKG-INFO
--rw-r--r--   0 huangshujia   (501) staff       (20)    11899 2021-08-23 07:04:21.000000 geneview-0.1.3/README.md
-drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2022-06-23 13:01:54.093280 geneview-0.1.3/geneview/
--rw-r--r--   0 huangshujia   (501) staff       (20)      457 2022-06-23 08:13:34.000000 geneview-0.1.3/geneview/__init__.py
-drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2022-06-23 13:01:54.107716 geneview-0.1.3/geneview/algorithm/
--rw-r--r--   0 huangshujia   (501) staff       (20)       42 2021-04-30 15:11:56.000000 geneview-0.1.3/geneview/algorithm/__init__.py
--rw-r--r--   0 huangshujia   (501) staff       (20)     4790 2021-06-02 00:32:31.000000 geneview-0.1.3/geneview/algorithm/_cluster.py
-drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2022-06-23 13:01:54.115498 geneview-0.1.3/geneview/baseplot/
--rw-r--r--   0 huangshujia   (501) staff       (20)       47 2021-05-06 07:48:03.000000 geneview-0.1.3/geneview/baseplot/__init__.py
--rw-r--r--   0 huangshujia   (501) staff       (20)        0 2021-05-13 09:00:18.000000 geneview-0.1.3/geneview/baseplot/_forest.py
--rw-r--r--   0 huangshujia   (501) staff       (20)    21012 2021-05-27 09:15:06.000000 geneview-0.1.3/geneview/baseplot/_venn.py
--rw-r--r--   0 huangshujia   (501) staff       (20)     5443 2021-05-13 02:30:08.000000 geneview-0.1.3/geneview/conftest.py
-drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2022-06-23 13:01:54.119699 geneview-0.1.3/geneview/genome_tracks/
--rw-r--r--   0 huangshujia   (501) staff       (20)      209 2021-05-25 08:54:56.000000 geneview-0.1.3/geneview/genome_tracks/__init__.py
-drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2022-06-23 13:01:54.138483 geneview-0.1.3/geneview/gwas/
--rw-r--r--   0 huangshujia   (501) staff       (20)       70 2021-05-11 03:58:13.000000 geneview-0.1.3/geneview/gwas/__init__.py
--rw-r--r--   0 huangshujia   (501) staff       (20)       78 2021-05-13 09:06:32.000000 geneview-0.1.3/geneview/gwas/_locuszoom.py
--rw-r--r--   0 huangshujia   (501) staff       (20)    15647 2021-05-13 06:11:47.000000 geneview-0.1.3/geneview/gwas/_manhattan.py
--rw-r--r--   0 huangshujia   (501) staff       (20)    11066 2022-01-10 13:44:21.000000 geneview-0.1.3/geneview/gwas/_qq.py
-drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2022-06-23 13:01:54.144512 geneview-0.1.3/geneview/karyotype/
--rw-r--r--   0 huangshujia   (501) staff       (20)       34 2021-02-04 01:48:57.000000 geneview-0.1.3/geneview/karyotype/__init__.py
--rw-r--r--   0 huangshujia   (501) staff       (20)     3149 2021-05-13 05:13:25.000000 geneview-0.1.3/geneview/karyotype/_karyotype.py
-drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2022-06-23 13:01:54.159767 geneview-0.1.3/geneview/palette/
--rw-r--r--   0 huangshujia   (501) staff       (20)      234 2021-05-02 15:17:42.000000 geneview-0.1.3/geneview/palette/__init__.py
--rw-r--r--   0 huangshujia   (501) staff       (20)     6932 2021-02-04 01:48:57.000000 geneview-0.1.3/geneview/palette/_circos.py
--rw-r--r--   0 huangshujia   (501) staff       (20)      494 2021-05-05 03:00:12.000000 geneview-0.1.3/geneview/palette/_palettes.py
--rw-r--r--   0 huangshujia   (501) staff       (20)    35446 2021-02-04 01:48:57.000000 geneview-0.1.3/geneview/palette/_xkcd_rgb.py
-drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2022-06-23 13:01:54.168635 geneview-0.1.3/geneview/popgene/
--rw-r--r--   0 huangshujia   (501) staff       (20)       37 2021-05-01 09:02:22.000000 geneview-0.1.3/geneview/popgene/__init__.py
--rw-r--r--   0 huangshujia   (501) staff       (20)    13293 2021-05-13 05:41:27.000000 geneview-0.1.3/geneview/popgene/_admixture.py
--rw-r--r--   0 huangshujia   (501) staff       (20)        0 2021-06-03 02:43:17.000000 geneview-0.1.3/geneview/popgene/_ldblock.py
-drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2022-06-23 13:01:54.172930 geneview-0.1.3/geneview/tests/
--rw-r--r--   0 huangshujia   (501) staff       (20)        0 2021-02-04 01:48:57.000000 geneview-0.1.3/geneview/tests/__init__.py
--rw-r--r--   0 huangshujia   (501) staff       (20)        0 2021-05-11 03:56:07.000000 geneview-0.1.3/geneview/tests/test_algorithms.py
--rw-r--r--   0 huangshujia   (501) staff       (20)     2370 2021-05-11 03:54:37.000000 geneview-0.1.3/geneview/tests/test_decorators.py
-drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2022-06-23 13:01:54.205670 geneview-0.1.3/geneview/utils/
--rw-r--r--   0 huangshujia   (501) staff       (20)      612 2021-05-14 06:52:45.000000 geneview-0.1.3/geneview/utils/__init__.py
--rw-r--r--   0 huangshujia   (501) staff       (20)    26871 2021-04-27 08:42:56.000000 geneview-0.1.3/geneview/utils/_adjust_text.py
--rw-r--r--   0 huangshujia   (501) staff       (20)     2842 2021-05-14 06:18:34.000000 geneview-0.1.3/geneview/utils/_dataset.py
--rw-r--r--   0 huangshujia   (501) staff       (20)     2153 2021-05-14 06:43:50.000000 geneview-0.1.3/geneview/utils/_decorators.py
--rw-r--r--   0 huangshujia   (501) staff       (20)      922 2021-05-14 06:41:43.000000 geneview-0.1.3/geneview/utils/_misc.py
-drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2022-06-23 13:01:54.101116 geneview-0.1.3/geneview.egg-info/
--rw-r--r--   0 huangshujia   (501) staff       (20)    15605 2022-06-23 13:01:52.000000 geneview-0.1.3/geneview.egg-info/PKG-INFO
--rw-r--r--   0 huangshujia   (501) staff       (20)     1009 2022-06-23 13:01:53.000000 geneview-0.1.3/geneview.egg-info/SOURCES.txt
--rw-r--r--   0 huangshujia   (501) staff       (20)        1 2022-06-23 13:01:52.000000 geneview-0.1.3/geneview.egg-info/dependency_links.txt
--rw-r--r--   0 huangshujia   (501) staff       (20)       38 2022-06-23 13:01:52.000000 geneview-0.1.3/geneview.egg-info/requires.txt
--rw-r--r--   0 huangshujia   (501) staff       (20)        9 2022-06-23 13:01:52.000000 geneview-0.1.3/geneview.egg-info/top_level.txt
--rw-r--r--   0 huangshujia   (501) staff       (20)       38 2022-06-23 13:01:54.215070 geneview-0.1.3/setup.cfg
--rw-r--r--   0 huangshujia   (501) staff       (20)     2325 2022-06-23 13:01:32.000000 geneview-0.1.3/setup.py
+drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-06-14 02:16:55.975234 geneview-0.2.0/
+-rw-r--r--   0 huangshujia   (501) staff       (20)    15671 2023-06-14 02:16:55.974323 geneview-0.2.0/PKG-INFO
+-rw-r--r--   0 huangshujia   (501) staff       (20)    11957 2023-06-14 02:12:24.000000 geneview-0.2.0/README.md
+drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-06-14 02:16:55.831253 geneview-0.2.0/geneview/
+-rw-r--r--   0 huangshujia   (501) staff       (20)      508 2023-06-14 01:55:50.000000 geneview-0.2.0/geneview/__init__.py
+drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-06-14 02:16:55.851199 geneview-0.2.0/geneview/algorithm/
+-rw-r--r--   0 huangshujia   (501) staff       (20)       42 2021-04-30 15:11:56.000000 geneview-0.2.0/geneview/algorithm/__init__.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)     4790 2021-06-02 00:32:31.000000 geneview-0.2.0/geneview/algorithm/_cluster.py
+drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-06-14 02:16:55.864070 geneview-0.2.0/geneview/baseplot/
+-rw-r--r--   0 huangshujia   (501) staff       (20)       47 2021-05-06 07:48:03.000000 geneview-0.2.0/geneview/baseplot/__init__.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)        0 2021-05-13 09:00:18.000000 geneview-0.2.0/geneview/baseplot/_forest.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)    21012 2021-05-27 09:15:06.000000 geneview-0.2.0/geneview/baseplot/_venn.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)     5443 2021-05-13 02:30:08.000000 geneview-0.2.0/geneview/conftest.py
+drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-06-14 02:16:55.868054 geneview-0.2.0/geneview/genome_tracks/
+-rw-r--r--   0 huangshujia   (501) staff       (20)      209 2021-05-25 08:54:56.000000 geneview-0.2.0/geneview/genome_tracks/__init__.py
+drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-06-14 02:16:55.894755 geneview-0.2.0/geneview/gwas/
+-rw-r--r--   0 huangshujia   (501) staff       (20)       70 2021-05-11 03:58:13.000000 geneview-0.2.0/geneview/gwas/__init__.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)       78 2021-05-13 09:06:32.000000 geneview-0.2.0/geneview/gwas/_locuszoom.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)    15669 2022-08-18 13:19:47.000000 geneview-0.2.0/geneview/gwas/_manhattan.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)    11066 2022-01-10 13:44:21.000000 geneview-0.2.0/geneview/gwas/_qq.py
+drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-06-14 02:16:55.901201 geneview-0.2.0/geneview/karyotype/
+-rw-r--r--   0 huangshujia   (501) staff       (20)       34 2021-02-04 01:48:57.000000 geneview-0.2.0/geneview/karyotype/__init__.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)     3149 2021-05-13 05:13:25.000000 geneview-0.2.0/geneview/karyotype/_karyotype.py
+drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-06-14 02:16:55.914605 geneview-0.2.0/geneview/palette/
+-rw-r--r--   0 huangshujia   (501) staff       (20)      234 2021-05-02 15:17:42.000000 geneview-0.2.0/geneview/palette/__init__.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)     6932 2021-02-04 01:48:57.000000 geneview-0.2.0/geneview/palette/_circos.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)      494 2021-05-05 03:00:12.000000 geneview-0.2.0/geneview/palette/_palettes.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)    35446 2021-02-04 01:48:57.000000 geneview-0.2.0/geneview/palette/_xkcd_rgb.py
+drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-06-14 02:16:55.937636 geneview-0.2.0/geneview/popgene/
+-rw-r--r--   0 huangshujia   (501) staff       (20)       38 2023-06-13 16:36:36.000000 geneview-0.2.0/geneview/popgene/__init__.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)    13782 2023-06-14 01:50:37.000000 geneview-0.2.0/geneview/popgene/_admixture.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)        0 2021-06-03 02:43:17.000000 geneview-0.2.0/geneview/popgene/_ldblock.py
+drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-06-14 02:16:55.940419 geneview-0.2.0/geneview/tests/
+-rw-r--r--   0 huangshujia   (501) staff       (20)        0 2021-02-04 01:48:57.000000 geneview-0.2.0/geneview/tests/__init__.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)        0 2021-05-11 03:56:07.000000 geneview-0.2.0/geneview/tests/test_algorithms.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)     2370 2021-05-11 03:54:37.000000 geneview-0.2.0/geneview/tests/test_decorators.py
+drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-06-14 02:16:55.968981 geneview-0.2.0/geneview/utils/
+-rw-r--r--   0 huangshujia   (501) staff       (20)      612 2021-05-14 06:52:45.000000 geneview-0.2.0/geneview/utils/__init__.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)    26871 2021-04-27 08:42:56.000000 geneview-0.2.0/geneview/utils/_adjust_text.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)     2842 2021-05-14 06:18:34.000000 geneview-0.2.0/geneview/utils/_dataset.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)     2153 2021-05-14 06:43:50.000000 geneview-0.2.0/geneview/utils/_decorators.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)      922 2021-05-14 06:41:43.000000 geneview-0.2.0/geneview/utils/_misc.py
+drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-06-14 02:16:55.841642 geneview-0.2.0/geneview.egg-info/
+-rw-r--r--   0 huangshujia   (501) staff       (20)    15671 2023-06-14 02:16:54.000000 geneview-0.2.0/geneview.egg-info/PKG-INFO
+-rw-r--r--   0 huangshujia   (501) staff       (20)     1009 2023-06-14 02:16:54.000000 geneview-0.2.0/geneview.egg-info/SOURCES.txt
+-rw-r--r--   0 huangshujia   (501) staff       (20)        1 2023-06-14 02:16:54.000000 geneview-0.2.0/geneview.egg-info/dependency_links.txt
+-rw-r--r--   0 huangshujia   (501) staff       (20)       38 2023-06-14 02:16:54.000000 geneview-0.2.0/geneview.egg-info/requires.txt
+-rw-r--r--   0 huangshujia   (501) staff       (20)        9 2023-06-14 02:16:54.000000 geneview-0.2.0/geneview.egg-info/top_level.txt
+-rw-r--r--   0 huangshujia   (501) staff       (20)       38 2023-06-14 02:16:55.975676 geneview-0.2.0/setup.cfg
+-rw-r--r--   0 huangshujia   (501) staff       (20)     2325 2023-06-14 02:13:16.000000 geneview-0.2.0/setup.py
```

### Comparing `geneview-0.1.3/PKG-INFO` & `geneview-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: geneview
-Version: 0.1.3
+Version: 0.2.0
 Summary: Geneview: A python package for genomics data visualization.
 Home-page: https://github.com/ShujiaHuang/geneview
 Author: Shujia Huang
 Author-email: huangshujia9@gmail.com
 Maintainer: Shujia Huang
 Maintainer-email: huangshujia9@gmail.com
 License: BSD (3-clause)
 Download-URL: https://github.com/ShujiaHuang/geneview
-Description: # geneview: A python package for genomics data visualization
+Description: # geneview: A python package for visualizing genomics data
         
         [![PyPI Version](https://img.shields.io/pypi/v/geneview.svg)](https://pypi.org/project/geneview/)
         [![Python](https://img.shields.io/pypi/pyversions/geneview.svg?style=plastic)](https://badge.fury.io/py/geneview)
         ![Tests](https://github.com/ShujiaHuang/geneview/workflows/CI/badge.svg)
         [![Code Coverage](https://codecov.io/gh/ShujiaHuang/geneview/branch/master/graph/badge.svg)](https://codecov.io/gh/ShujiaHuang/geneview)
         
-        **geneview** is a library for making attractive and informative genomic graphics in Python.
-        It is built on top of matplotlib and tightly integrated with the PyData stack, including
-        support for `numpy` and `pandas` data structures. And now it is actively developed.
+        **geneview** is a library for making attractive and informative genomics graphics in Python.
+        It is built on top of [matplotlib](https://matplotlib.org/) and tightly integrated with the PyData 
+        stack, including support for `numpy` and `pandas` data structures. And now it is actively developed.
         
         Some of the features that geneview offers are:
         
         - High-level abstractions for structuring grids of plots that let you easily build complex visualizations.
-        - Functions for visualizing general genomic plots.
+        - Functions for visualizing general genomics plots.
         
         
         ## Installation
         
         To install the released version, just do
         
         ```bash
@@ -74,15 +74,15 @@
         defaulting to a darkblue and lightblue color scheme.
         
         ```python
         import matplotlib.pyplot as plt
         import geneview as gv
         
         # load data
-        df = gv.utils.load_dataset("gwas")
+        df = gv.load_dataset("gwas")
         # Plot a basic manhattan plot with horizontal xtick labels and the figure will display in screen.
         ax = gv.manhattanplot(data=df)
         plt.show()
         ```
         
         ![manhattan_plot.png](./examples/figures/manhattan_plot.png)
         
@@ -202,15 +202,15 @@
         
         ```python
         
         import matplotlib.pyplot as plt
         import geneview as gv
         
         # load data
-        df = gv.utils.load_dataset("gwas")
+        df = gv.load_dataset("gwas")
         # Plot a basic manhattan plot with horizontal xtick labels and the figure will display in screen.
         ax = gv.qqplot(data=df["P"])
         plt.show()
         
         ```
         
         ![qq.png](./examples/figures/qq.png)
@@ -239,15 +239,15 @@
         ### Admixture plot
         Generate **Admixture** plot from the raw admixture output result:
         
         #### simple example for admixtureplot
         
         ```python
         import matplotlib.pyplot as plt
-        from geneview.utils import load_dataset
+        from geneview import load_dataset
         from geneview import admixtureplot
         
         f, ax = plt.subplots(1, 1, figsize=(14, 2), facecolor="w", constrained_layout=True, dpi=300)
         admixtureplot(data=load_dataset("admixture_output.Q"), 
                       population_info=load_dataset("admixture_population.info"),
                       ylabel_kws={"rotation": 45, "ha": "right"},
                       ax=ax)
@@ -256,34 +256,35 @@
         
         or
         
         ```python
         import matplotlib.pyplot as plt
         import geneview as gv
         
-        admixture_output_fn = gv.utils.load_dataset("admixture_output.Q")
-        population_group_fn = gv.utils.load_dataset("admixture_population.info")
+        admixture_output_fn = gv.load_dataset("admixture_output.Q")
+        population_group_fn = gv.load_dataset("admixture_population.info")
         
         # define the order for population to plot
         pop_group_1kg = ["KHV", "CDX", "CHS", "CHB", "JPT", "BEB", "STU", "ITU", "GIH", "PJL", "FIN", 
                          "CEU", "GBR", "IBS", "TSI", "PEL", "PUR", "MXL", "CLM", "ASW", "ACB", "GWD", 
                          "MSL", "YRI", "ESN", "LWK"]
         
         f, ax = plt.subplots(1, 1, figsize=(14, 2), facecolor="w", constrained_layout=True, dpi=300)
         gv.popgen.admixtureplot(data=admixture_output_fn, 
                                 population_info=population_group_fn,
+                                edgewidth=2.0,
                                 group_order=pop_group_1kg,
                                 shuffle_popsample_kws={"frac": 0.5},
                                 ylabel_kws={"rotation": 45, "ha": "right"},
                                 ax=ax)
         ```
         
         ![admixtureplot](./examples/figures/admixture.png)
         
-        - [More tutorials about admixtureplot](./docs/tutorial/admixture.ipynb)
+        - [The format of input files and more details about admixtureplot](./docs/tutorial/admixture.ipynb)
         
         
         ### Venn plots
         
         **Venn diagrams for 2, 3, 4, 5, 6 sets.**
         
         ![Venn.png](./examples/figures/venn.png)
@@ -345,15 +346,15 @@
         We need the data structures: `DataFrame` and `Series` in **pandas**. 
         It's easy and worth to learn, click 
         [here](http://pda.readthedocs.org/en/latest/chp5.html) to see more detail 
         tutorial for these two data type.
         
         ## License
         
-        Released under a BSD (3-clause) license
+        Released under a GPL-3.0 license
         
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `geneview-0.1.3/README.md` & `geneview-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# geneview: A python package for genomics data visualization
+# geneview: A python package for visualizing genomics data
 
 [![PyPI Version](https://img.shields.io/pypi/v/geneview.svg)](https://pypi.org/project/geneview/)
 [![Python](https://img.shields.io/pypi/pyversions/geneview.svg?style=plastic)](https://badge.fury.io/py/geneview)
 ![Tests](https://github.com/ShujiaHuang/geneview/workflows/CI/badge.svg)
 [![Code Coverage](https://codecov.io/gh/ShujiaHuang/geneview/branch/master/graph/badge.svg)](https://codecov.io/gh/ShujiaHuang/geneview)
 
-**geneview** is a library for making attractive and informative genomic graphics in Python.
-It is built on top of matplotlib and tightly integrated with the PyData stack, including
-support for `numpy` and `pandas` data structures. And now it is actively developed.
+**geneview** is a library for making attractive and informative genomics graphics in Python.
+It is built on top of [matplotlib](https://matplotlib.org/) and tightly integrated with the PyData 
+stack, including support for `numpy` and `pandas` data structures. And now it is actively developed.
 
 Some of the features that geneview offers are:
 
 - High-level abstractions for structuring grids of plots that let you easily build complex visualizations.
-- Functions for visualizing general genomic plots.
+- Functions for visualizing general genomics plots.
 
 
 ## Installation
 
 To install the released version, just do
 
 ```bash
@@ -63,15 +63,15 @@
 defaulting to a darkblue and lightblue color scheme.
 
 ```python
 import matplotlib.pyplot as plt
 import geneview as gv
 
 # load data
-df = gv.utils.load_dataset("gwas")
+df = gv.load_dataset("gwas")
 # Plot a basic manhattan plot with horizontal xtick labels and the figure will display in screen.
 ax = gv.manhattanplot(data=df)
 plt.show()
 ```
 
 ![manhattan_plot.png](./examples/figures/manhattan_plot.png)
 
@@ -191,15 +191,15 @@
 
 ```python
 
 import matplotlib.pyplot as plt
 import geneview as gv
 
 # load data
-df = gv.utils.load_dataset("gwas")
+df = gv.load_dataset("gwas")
 # Plot a basic manhattan plot with horizontal xtick labels and the figure will display in screen.
 ax = gv.qqplot(data=df["P"])
 plt.show()
 
 ```
 
 ![qq.png](./examples/figures/qq.png)
@@ -228,15 +228,15 @@
 ### Admixture plot
 Generate **Admixture** plot from the raw admixture output result:
 
 #### simple example for admixtureplot
 
 ```python
 import matplotlib.pyplot as plt
-from geneview.utils import load_dataset
+from geneview import load_dataset
 from geneview import admixtureplot
 
 f, ax = plt.subplots(1, 1, figsize=(14, 2), facecolor="w", constrained_layout=True, dpi=300)
 admixtureplot(data=load_dataset("admixture_output.Q"), 
               population_info=load_dataset("admixture_population.info"),
               ylabel_kws={"rotation": 45, "ha": "right"},
               ax=ax)
@@ -245,34 +245,35 @@
 
 or
 
 ```python
 import matplotlib.pyplot as plt
 import geneview as gv
 
-admixture_output_fn = gv.utils.load_dataset("admixture_output.Q")
-population_group_fn = gv.utils.load_dataset("admixture_population.info")
+admixture_output_fn = gv.load_dataset("admixture_output.Q")
+population_group_fn = gv.load_dataset("admixture_population.info")
 
 # define the order for population to plot
 pop_group_1kg = ["KHV", "CDX", "CHS", "CHB", "JPT", "BEB", "STU", "ITU", "GIH", "PJL", "FIN", 
                  "CEU", "GBR", "IBS", "TSI", "PEL", "PUR", "MXL", "CLM", "ASW", "ACB", "GWD", 
                  "MSL", "YRI", "ESN", "LWK"]
 
 f, ax = plt.subplots(1, 1, figsize=(14, 2), facecolor="w", constrained_layout=True, dpi=300)
 gv.popgen.admixtureplot(data=admixture_output_fn, 
                         population_info=population_group_fn,
+                        edgewidth=2.0,
                         group_order=pop_group_1kg,
                         shuffle_popsample_kws={"frac": 0.5},
                         ylabel_kws={"rotation": 45, "ha": "right"},
                         ax=ax)
 ```
 
 ![admixtureplot](./examples/figures/admixture.png)
 
-- [More tutorials about admixtureplot](./docs/tutorial/admixture.ipynb)
+- [The format of input files and more details about admixtureplot](./docs/tutorial/admixture.ipynb)
 
 
 ### Venn plots
 
 **Venn diagrams for 2, 3, 4, 5, 6 sets.**
 
 ![Venn.png](./examples/figures/venn.png)
@@ -334,8 +335,8 @@
 We need the data structures: `DataFrame` and `Series` in **pandas**. 
 It's easy and worth to learn, click 
 [here](http://pda.readthedocs.org/en/latest/chp5.html) to see more detail 
 tutorial for these two data type.
 
 ## License
 
-Released under a BSD (3-clause) license
+Released under a GPL-3.0 license
```

### Comparing `geneview-0.1.3/geneview/algorithm/_cluster.py` & `geneview-0.2.0/geneview/algorithm/_cluster.py`

 * *Files identical despite different names*

### Comparing `geneview-0.1.3/geneview/baseplot/_venn.py` & `geneview-0.2.0/geneview/baseplot/_venn.py`

 * *Files identical despite different names*

### Comparing `geneview-0.1.3/geneview/conftest.py` & `geneview-0.2.0/geneview/conftest.py`

 * *Files identical despite different names*

### Comparing `geneview-0.1.3/geneview/gwas/_manhattan.py` & `geneview-0.2.0/geneview/gwas/_manhattan.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,15 +251,15 @@
         for i, (site, p_value) in enumerate(zip(group_data[pos], group_data[pv])):
             y_value = -np.log10(p_value) if logp else p_value
 
             x.append(last_xpos + site)
             y.append(y_value)
 
             c.append(sign_marker_color if ((sign_marker_p is not None) and (p_value <= sign_marker_p)) else color)
-            if (sign_marker_p is not None) and (p_value <= sign_marker_p):
+            if (snp is not None) and (sign_marker_p is not None) and (p_value <= sign_marker_p):
                 snp_id = group_data[snp].iloc[i]
                 sign_snp_sites.append([last_xpos + site, y_value, snp_id])  # x_pos, y_value, text
 
         # ``xs_by_id`` is for setting up positions and ticks. Ticks should
         # be placed in the middle of a chromosome. The a new pos column is 
         # added that keeps a running sum of the positions of each successive 
         # chromsome.
```

### Comparing `geneview-0.1.3/geneview/gwas/_qq.py` & `geneview-0.2.0/geneview/gwas/_qq.py`

 * *Files identical despite different names*

### Comparing `geneview-0.1.3/geneview/karyotype/_karyotype.py` & `geneview-0.2.0/geneview/karyotype/_karyotype.py`

 * *Files identical despite different names*

### Comparing `geneview-0.1.3/geneview/palette/_circos.py` & `geneview-0.2.0/geneview/palette/_circos.py`

 * *Files identical despite different names*

### Comparing `geneview-0.1.3/geneview/palette/_xkcd_rgb.py` & `geneview-0.2.0/geneview/palette/_xkcd_rgb.py`

 * *Files identical despite different names*

### Comparing `geneview-0.1.3/geneview/popgene/_admixture.py` & `geneview-0.2.0/geneview/popgene/_admixture.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from ..palette import generate_colors_palette
 
 
 def _draw_admixtureplot(
         data=None,
         group_order=None,
         linewidth=1.0,
+        edgewidth=1.0,
         palette="tab10",
         xticklabels=None,
         xticklabel_kws=None,
         ylabel=None,
         ylabel_kws=None,
         hierarchical_kws=None,
         ax=None
@@ -50,39 +51,43 @@
 
     if group_order is None:
         group_order = list(set(data.keys()))
 
     n = 0
     for g in group_order:
         n += len(data[g])
-        hc = hierarchical_cluster(data=data[g], **hierarchical_kws)
-        data[g] = hc.data.iloc[hc.reordered_index]  # re-order the data.
+        if len(data[g]) > 1:
+            # Only for the group sample larger than 1 need cluster.
+            hc = hierarchical_cluster(data=data[g], **hierarchical_kws)
+            data[g] = hc.data.iloc[hc.reordered_index]  # re-order data.
 
     x = np.arange(n)
     base_y = np.zeros(len(x))
 
-    column_names = data[group_order[0]].columns
-    colors = generate_colors_palette(cmap=palette, n_colors=len(column_names))
+    k_names = data[group_order[0]].columns
+    colors = generate_colors_palette(cmap=palette, n_colors=len(k_names))
     palette = cycle(colors)
-    if len(colors) < len(column_names):
+    if len(colors) < len(k_names):
         msg = ("The categories of colors setting by `palette` is less than "
                "the number of estimating sub populations (K) in admixture, "
                "which could cause a confuse plot. Please reset the palette.")
         warnings.warn(msg)
 
-    for k in column_names:
+    bar_width = 1.0
+    for k in k_names:
         c = next(palette)  # one color for one 'k'
         start_g_pos = 0
         add_y = []
         for g in group_order:  # keep group order
             try:
                 y = data[g][k]
                 end_g_pos = start_g_pos + len(y)
-                ax.bar(x[start_g_pos:end_g_pos], y, bottom=base_y[start_g_pos:end_g_pos],
-                       color=c, width=1.0, linewidth=0)
+                ax.bar(x[start_g_pos:end_g_pos] + 0.5 * bar_width, y,
+                       bottom=base_y[start_g_pos:end_g_pos],
+                       color=c, width=bar_width, linewidth=0)
 
                 start_g_pos = end_g_pos
                 add_y.append(y)
             except KeyError:
                 raise KeyError("KeyError: '%s'. Missing in 'group_order'." % g)
 
         base_y += np.array(pd.concat(add_y, axis=0))
@@ -92,20 +97,20 @@
     for g in group_order:  # make group order
         g_size = len(data[g])
         xticks_pos.append(g_pos + 0.5 * g_size)
 
         g_pos += g_size
         ax.axvline(x=g_pos, color="k", lw=linewidth)
 
-    ax.spines["left"].set_linewidth(linewidth)
-    ax.spines["top"].set_linewidth(linewidth)
-    ax.spines["right"].set_linewidth(linewidth)
-    ax.spines["bottom"].set_linewidth(linewidth)
+    ax.spines["left"].set_linewidth(edgewidth)
+    ax.spines["top"].set_linewidth(edgewidth)
+    ax.spines["right"].set_linewidth(edgewidth)
+    ax.spines["bottom"].set_linewidth(edgewidth)
 
-    ax.set_xlim([x[0], x[-1]])
+    ax.set_xlim([x[0], x[-1]+bar_width])
     ax.set_ylim([0, 1.0])
     ax.tick_params(bottom=False, top=False, left=False, right=False)
 
     if xticklabel_kws is None:
         xticklabel_kws = {}
 
     if xticklabels and (len(group_order) != len(xticklabels)):
@@ -136,36 +141,37 @@
 
     if len(sample_info) != len(df):
         raise ValueError("The size of sample_info(%d) and input admixture result(%d) "
                          "must be the same." % (len(sample_info), len(df)))
 
     data = {}
     for g in popset:
-        g_data = df[sample_info["Group"] == g].copy()
+        g_data = df[sample_info["Group"] == g].copy()  # Get specify group data according to the order of sample_info
         g_size = len(g_data)
         if shuffle_popsample_kws:
             shuffle_raw_n = shuffle_popsample_kws["n"] if "n" in shuffle_popsample_kws else None
             if shuffle_raw_n and shuffle_raw_n > g_size:
                 shuffle_popsample_kws["n"] = g_size
                 data[g] = g_data.sample(**shuffle_popsample_kws)
-                shuffle_popsample_kws["n"] = shuffle_raw_n  # reset to the raw N
+                shuffle_popsample_kws["n"] = shuffle_raw_n  # reset to the raw shuffle N
             else:
                 data[g] = g_data.sample(**shuffle_popsample_kws)
         else:
             data[g] = g_data
 
     return data
 
 
 def admixtureplot(
         data,
         population_info=None,
         shuffle_popsample_kws=None,
         group_order=None,
         linewidth=1.0,
+        edgewidth=1.0,
         palette="tab10",
         xticklabels=None,
         xticklabel_kws=None,
         ylabel=None,
         ylabel_kws=None,
         hierarchical_kws=None,
         ax=None
@@ -192,14 +198,17 @@
 
         group_order : vector of strings, optional
             Specify the order of processing and plotting for the estimating sub populations.
 
         linewidth : float, optional, default: 1.0
             Set the line width in plot
 
+        edgewidth : float, optional, default: 1.0
+            Set the frame edge width in plot
+
         palette : string, list, or :class:`matplotlib.colors.Colormap`, optional, default: tab10.
             String values are passed to :func:`generate_colors`. List values imply categorical
             mapping, while a colormap object implies numeric mapping.
 
         xticklabels : list, optional
             The label texts of x-axis.
 
@@ -256,15 +265,15 @@
         Setting the ``shuffle_popsample_kws`` argument if you wish to sample some samples for each
         population group in the admixture plot.
 
         only sampling 80 samples for each population group.
         .. plot::
             :context: close-figs
 
-            >>> ax = admixtureplot(data=admixture_fn,
+            >>> ax = admixtureplot(data=admixture_fn, edgewidth=1.0,
             ...                    population_info=population_fn,
             ...                    shuffle_popsample_kws={"n": 80},
             ...                    group_order=pop_group_1kg)
 
         Or specifies the fraction of each group population.
 
         .. plot::
@@ -293,14 +302,15 @@
             ...     data[g] = g_data.sample(n=140, random_state=100) if len(g_data)>140 else g_data
 
             # Plot the figure
             >>> import matplotlib.pyplot as plt
             >>> f, ax = plt.subplots(1, 1, figsize=(14, 3), facecolor="w", constrained_layout=True, dpi=300)
             >>> ax = admixtureplot(data=data,
             ...                    group_order=pop_group_1kg,
+            ...                    edgewidth=2.0,
             ...                    palette="Set1",
             ...                    xticklabel_kws={"rotation": "vertical"},
             ...                    ylabel="K=11",
             ...                    ylabel_kws={"rotation": 0, "ha": "right"},
             ...                    ax=ax)
 
     """
@@ -329,14 +339,15 @@
     if ylabel is None:
         g = list(data.keys())[0]
         ylabel = "K=%d" % len(data[g].columns)
 
     return _draw_admixtureplot(data=data,
                                group_order=group_order,
                                linewidth=linewidth,
+                               edgewidth=edgewidth,
                                palette=palette,
                                xticklabels=xticklabels,
                                xticklabel_kws=xticklabel_kws,
                                ylabel=ylabel,
                                ylabel_kws=ylabel_kws,
                                hierarchical_kws=hierarchical_kws,
                                ax=ax)
```

### Comparing `geneview-0.1.3/geneview/tests/test_decorators.py` & `geneview-0.2.0/geneview/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `geneview-0.1.3/geneview/utils/__init__.py` & `geneview-0.2.0/geneview/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `geneview-0.1.3/geneview/utils/_adjust_text.py` & `geneview-0.2.0/geneview/utils/_adjust_text.py`

 * *Files identical despite different names*

### Comparing `geneview-0.1.3/geneview/utils/_dataset.py` & `geneview-0.2.0/geneview/utils/_dataset.py`

 * *Files identical despite different names*

### Comparing `geneview-0.1.3/geneview/utils/_decorators.py` & `geneview-0.2.0/geneview/utils/_decorators.py`

 * *Files identical despite different names*

### Comparing `geneview-0.1.3/geneview/utils/_misc.py` & `geneview-0.2.0/geneview/utils/_misc.py`

 * *Files identical despite different names*

### Comparing `geneview-0.1.3/geneview.egg-info/PKG-INFO` & `geneview-0.2.0/geneview.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: geneview
-Version: 0.1.3
+Version: 0.2.0
 Summary: Geneview: A python package for genomics data visualization.
 Home-page: https://github.com/ShujiaHuang/geneview
 Author: Shujia Huang
 Author-email: huangshujia9@gmail.com
 Maintainer: Shujia Huang
 Maintainer-email: huangshujia9@gmail.com
 License: BSD (3-clause)
 Download-URL: https://github.com/ShujiaHuang/geneview
-Description: # geneview: A python package for genomics data visualization
+Description: # geneview: A python package for visualizing genomics data
         
         [![PyPI Version](https://img.shields.io/pypi/v/geneview.svg)](https://pypi.org/project/geneview/)
         [![Python](https://img.shields.io/pypi/pyversions/geneview.svg?style=plastic)](https://badge.fury.io/py/geneview)
         ![Tests](https://github.com/ShujiaHuang/geneview/workflows/CI/badge.svg)
         [![Code Coverage](https://codecov.io/gh/ShujiaHuang/geneview/branch/master/graph/badge.svg)](https://codecov.io/gh/ShujiaHuang/geneview)
         
-        **geneview** is a library for making attractive and informative genomic graphics in Python.
-        It is built on top of matplotlib and tightly integrated with the PyData stack, including
-        support for `numpy` and `pandas` data structures. And now it is actively developed.
+        **geneview** is a library for making attractive and informative genomics graphics in Python.
+        It is built on top of [matplotlib](https://matplotlib.org/) and tightly integrated with the PyData 
+        stack, including support for `numpy` and `pandas` data structures. And now it is actively developed.
         
         Some of the features that geneview offers are:
         
         - High-level abstractions for structuring grids of plots that let you easily build complex visualizations.
-        - Functions for visualizing general genomic plots.
+        - Functions for visualizing general genomics plots.
         
         
         ## Installation
         
         To install the released version, just do
         
         ```bash
@@ -74,15 +74,15 @@
         defaulting to a darkblue and lightblue color scheme.
         
         ```python
         import matplotlib.pyplot as plt
         import geneview as gv
         
         # load data
-        df = gv.utils.load_dataset("gwas")
+        df = gv.load_dataset("gwas")
         # Plot a basic manhattan plot with horizontal xtick labels and the figure will display in screen.
         ax = gv.manhattanplot(data=df)
         plt.show()
         ```
         
         ![manhattan_plot.png](./examples/figures/manhattan_plot.png)
         
@@ -202,15 +202,15 @@
         
         ```python
         
         import matplotlib.pyplot as plt
         import geneview as gv
         
         # load data
-        df = gv.utils.load_dataset("gwas")
+        df = gv.load_dataset("gwas")
         # Plot a basic manhattan plot with horizontal xtick labels and the figure will display in screen.
         ax = gv.qqplot(data=df["P"])
         plt.show()
         
         ```
         
         ![qq.png](./examples/figures/qq.png)
@@ -239,15 +239,15 @@
         ### Admixture plot
         Generate **Admixture** plot from the raw admixture output result:
         
         #### simple example for admixtureplot
         
         ```python
         import matplotlib.pyplot as plt
-        from geneview.utils import load_dataset
+        from geneview import load_dataset
         from geneview import admixtureplot
         
         f, ax = plt.subplots(1, 1, figsize=(14, 2), facecolor="w", constrained_layout=True, dpi=300)
         admixtureplot(data=load_dataset("admixture_output.Q"), 
                       population_info=load_dataset("admixture_population.info"),
                       ylabel_kws={"rotation": 45, "ha": "right"},
                       ax=ax)
@@ -256,34 +256,35 @@
         
         or
         
         ```python
         import matplotlib.pyplot as plt
         import geneview as gv
         
-        admixture_output_fn = gv.utils.load_dataset("admixture_output.Q")
-        population_group_fn = gv.utils.load_dataset("admixture_population.info")
+        admixture_output_fn = gv.load_dataset("admixture_output.Q")
+        population_group_fn = gv.load_dataset("admixture_population.info")
         
         # define the order for population to plot
         pop_group_1kg = ["KHV", "CDX", "CHS", "CHB", "JPT", "BEB", "STU", "ITU", "GIH", "PJL", "FIN", 
                          "CEU", "GBR", "IBS", "TSI", "PEL", "PUR", "MXL", "CLM", "ASW", "ACB", "GWD", 
                          "MSL", "YRI", "ESN", "LWK"]
         
         f, ax = plt.subplots(1, 1, figsize=(14, 2), facecolor="w", constrained_layout=True, dpi=300)
         gv.popgen.admixtureplot(data=admixture_output_fn, 
                                 population_info=population_group_fn,
+                                edgewidth=2.0,
                                 group_order=pop_group_1kg,
                                 shuffle_popsample_kws={"frac": 0.5},
                                 ylabel_kws={"rotation": 45, "ha": "right"},
                                 ax=ax)
         ```
         
         ![admixtureplot](./examples/figures/admixture.png)
         
-        - [More tutorials about admixtureplot](./docs/tutorial/admixture.ipynb)
+        - [The format of input files and more details about admixtureplot](./docs/tutorial/admixture.ipynb)
         
         
         ### Venn plots
         
         **Venn diagrams for 2, 3, 4, 5, 6 sets.**
         
         ![Venn.png](./examples/figures/venn.png)
@@ -345,15 +346,15 @@
         We need the data structures: `DataFrame` and `Series` in **pandas**. 
         It's easy and worth to learn, click 
         [here](http://pda.readthedocs.org/en/latest/chp5.html) to see more detail 
         tutorial for these two data type.
         
         ## License
         
-        Released under a BSD (3-clause) license
+        Released under a GPL-3.0 license
         
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `geneview-0.1.3/geneview.egg-info/SOURCES.txt` & `geneview-0.2.0/geneview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geneview-0.1.3/setup.py` & `geneview-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 meta = Namespace(
     __DISTNAME__     = "geneview",
     __AUTHOR__       = "Shujia Huang",
     __AUTHOR_EMAIL__ = "huangshujia9@gmail.com",
     __URL__          = "https://github.com/ShujiaHuang/geneview",
     __LICENSE__      = "BSD (3-clause)",
     __DOWNLOAD_URL__ = "https://github.com/ShujiaHuang/geneview",
-    __VERSION__      = "0.1.3",
+    __VERSION__      = "0.2.0",
 )
 
 try:
     from setuptools import setup, find_packages
     _has_setuptools = True
 except ImportError:
     from distutils.core import setup, find_packages
```

