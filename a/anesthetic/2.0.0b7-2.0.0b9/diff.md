# Comparing `tmp/anesthetic-2.0.0b7.tar.gz` & `tmp/anesthetic-2.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anesthetic-2.0.0b7.tar", last modified: Wed Mar 10 18:49:11 2021, max compression
+gzip compressed data, was "anesthetic-2.0.0b9.tar", last modified: Thu Jul 15 13:19:18 2021, max compression
```

## Comparing `anesthetic-2.0.0b7.tar` & `anesthetic-2.0.0b9.tar`

### file list

```diff
@@ -1,121 +1,126 @@
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2021-03-10 18:49:11.215136 anesthetic-2.0.0b7/
--rw-r--r--   0 will      (1000) will      (1000)       42 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/.coveragerc
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2021-03-10 18:49:11.198470 anesthetic-2.0.0b7/.github/
--rw-r--r--   0 will      (1000) will      (1000)     3367 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 will      (1000) will      (1000)      836 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/.github/CONTRIBUTING.md
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2021-03-10 18:49:11.198470 anesthetic-2.0.0b7/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 will      (1000) will      (1000)      438 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 will      (1000) will      (1000)      569 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 will      (1000) will      (1000)      531 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2021-03-10 18:49:11.201804 anesthetic-2.0.0b7/.github/workflows/
--rw-r--r--   0 will      (1000) will      (1000)     2279 2021-03-05 09:25:55.000000 anesthetic-2.0.0b7/.github/workflows/CI.yml
--rw-r--r--   0 will      (1000) will      (1000)      262 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/.gitignore
--rw-r--r--   0 will      (1000) will      (1000)      540 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/.readthedocs.yml
--rw-r--r--   0 will      (1000) will      (1000)     1069 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/LICENSE
--rw-r--r--   0 will      (1000) will      (1000)    11481 2021-03-10 18:49:11.215136 anesthetic-2.0.0b7/PKG-INFO
--rw-r--r--   0 will      (1000) will      (1000)     8643 2021-03-10 18:48:07.000000 anesthetic-2.0.0b7/README.rst
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2021-03-10 18:49:11.201804 anesthetic-2.0.0b7/anesthetic/
--rw-r--r--   0 will      (1000) will      (1000)      400 2021-03-05 09:25:55.000000 anesthetic-2.0.0b7/anesthetic/__init__.py
--rw-r--r--   0 will      (1000) will      (1000)      919 2020-05-31 10:39:15.000000 anesthetic-2.0.0b7/anesthetic/boundary.py
--rw-r--r--   0 will      (1000) will      (1000)      886 2021-03-05 09:25:55.000000 anesthetic-2.0.0b7/anesthetic/convert.py
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2021-03-10 18:49:11.201804 anesthetic-2.0.0b7/anesthetic/gui/
--rw-r--r--   0 will      (1000) will      (1000)       68 2020-05-31 09:10:19.000000 anesthetic-2.0.0b7/anesthetic/gui/__init__.py
--rw-r--r--   0 will      (1000) will      (1000)     9211 2021-03-05 09:25:55.000000 anesthetic-2.0.0b7/anesthetic/gui/plot.py
--rw-r--r--   0 will      (1000) will      (1000)     8255 2021-03-05 09:25:55.000000 anesthetic-2.0.0b7/anesthetic/gui/widgets.py
--rw-r--r--   0 will      (1000) will      (1000)     2751 2020-05-31 10:39:15.000000 anesthetic-2.0.0b7/anesthetic/kde.py
--rw-r--r--   0 will      (1000) will      (1000)    31128 2021-03-10 18:48:07.000000 anesthetic-2.0.0b7/anesthetic/plot.py
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2021-03-10 18:49:11.201804 anesthetic-2.0.0b7/anesthetic/read/
--rw-r--r--   0 will      (1000) will      (1000)       44 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/anesthetic/read/__init__.py
--rw-r--r--   0 will      (1000) will      (1000)      442 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/anesthetic/read/chainreader.py
--rw-r--r--   0 will      (1000) will      (1000)     3605 2021-03-05 09:25:55.000000 anesthetic-2.0.0b7/anesthetic/read/getdistreader.py
--rw-r--r--   0 will      (1000) will      (1000)     5747 2021-03-05 09:25:55.000000 anesthetic-2.0.0b7/anesthetic/read/montepythonreader.py
--rw-r--r--   0 will      (1000) will      (1000)     2219 2020-05-31 10:39:15.000000 anesthetic-2.0.0b7/anesthetic/read/multinestreader.py
--rw-r--r--   0 will      (1000) will      (1000)     1042 2020-05-31 10:39:15.000000 anesthetic-2.0.0b7/anesthetic/read/polychordreader.py
--rw-r--r--   0 will      (1000) will      (1000)     1187 2020-06-23 10:24:18.000000 anesthetic-2.0.0b7/anesthetic/read/samplereader.py
--rw-r--r--   0 will      (1000) will      (1000)    30778 2021-03-05 09:25:55.000000 anesthetic-2.0.0b7/anesthetic/samples.py
--rw-r--r--   0 will      (1000) will      (1000)    14078 2021-03-10 18:48:03.000000 anesthetic-2.0.0b7/anesthetic/utils.py
--rw-r--r--   0 will      (1000) will      (1000)    11168 2021-03-10 18:46:37.000000 anesthetic-2.0.0b7/anesthetic/weighted_pandas.py
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2021-03-10 18:49:11.201804 anesthetic-2.0.0b7/anesthetic.egg-info/
--rw-r--r--   0 will      (1000) will      (1000)    11481 2021-03-10 18:49:11.000000 anesthetic-2.0.0b7/anesthetic.egg-info/PKG-INFO
--rw-r--r--   0 will      (1000) will      (1000)     2768 2021-03-10 18:49:11.000000 anesthetic-2.0.0b7/anesthetic.egg-info/SOURCES.txt
--rw-r--r--   0 will      (1000) will      (1000)        1 2021-03-10 18:49:11.000000 anesthetic-2.0.0b7/anesthetic.egg-info/dependency_links.txt
--rw-r--r--   0 will      (1000) will      (1000)      165 2021-03-10 18:49:11.000000 anesthetic-2.0.0b7/anesthetic.egg-info/requires.txt
--rw-r--r--   0 will      (1000) will      (1000)       11 2021-03-10 18:49:11.000000 anesthetic-2.0.0b7/anesthetic.egg-info/top_level.txt
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2021-03-10 18:49:11.201804 anesthetic-2.0.0b7/bin/
--rwxr-xr-x   0 will      (1000) will      (1000)     5625 2020-05-31 10:39:15.000000 anesthetic-2.0.0b7/bin/gen_data.py
--rw-r--r--   0 will      (1000) will      (1000)     3348 2020-05-31 10:39:15.000000 anesthetic-2.0.0b7/bin/plot.py
--rwxr-xr-x   0 will      (1000) will      (1000)      214 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/bin/run_tests
--rw-r--r--   0 will      (1000) will      (1000)    11766 2020-07-29 19:08:13.000000 anesthetic-2.0.0b7/demo.ipynb
--rw-r--r--   0 will      (1000) will      (1000)     5623 2020-07-29 19:08:13.000000 anesthetic-2.0.0b7/demo.py
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2021-03-10 18:49:11.201804 anesthetic-2.0.0b7/docs/
--rw-r--r--   0 will      (1000) will      (1000)      584 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/docs/Makefile
--rw-r--r--   0 will      (1000) will      (1000)      791 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/docs/make.bat
--rw-r--r--   0 will      (1000) will      (1000)       47 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/docs/requirements.txt
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2021-03-10 18:49:11.205137 anesthetic-2.0.0b7/docs/source/
--rw-r--r--   0 will      (1000) will      (1000)      499 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/docs/source/anesthetic.gui.rst
--rw-r--r--   0 will      (1000) will      (1000)     1000 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/docs/source/anesthetic.read.rst
--rw-r--r--   0 will      (1000) will      (1000)      988 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/docs/source/anesthetic.rst
--rw-r--r--   0 will      (1000) will      (1000)     6272 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/docs/source/conf.py
--rw-r--r--   0 will      (1000) will      (1000)      187 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/docs/source/index.rst
--rw-r--r--   0 will      (1000) will      (1000)       55 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/docs/source/intro.rst
--rw-r--r--   0 will      (1000) will      (1000)       67 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/docs/source/modules.rst
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2021-03-10 18:49:11.205137 anesthetic-2.0.0b7/images/
--rw-r--r--   0 will      (1000) will      (1000)   224235 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/images/anim_1.gif
--rw-r--r--   0 will      (1000) will      (1000)      669 2020-05-31 10:39:15.000000 anesthetic-2.0.0b7/images/animate.py
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2021-03-10 18:49:11.205137 anesthetic-2.0.0b7/paper/
--rw-r--r--   0 will      (1000) will      (1000)    50898 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/paper/2d.png
--rw-r--r--   0 will      (1000) will      (1000)     1728 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/paper/Makefile
--rw-r--r--   0 will      (1000) will      (1000)    13970 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/paper/paper.bib
--rw-r--r--   0 will      (1000) will      (1000)     5900 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/paper/paper.md
--rw-r--r--   0 will      (1000) will      (1000)       44 2021-03-05 09:25:55.000000 anesthetic-2.0.0b7/requirements.txt
--rw-r--r--   0 will      (1000) will      (1000)       68 2021-03-05 09:25:55.000000 anesthetic-2.0.0b7/requirements_extras.txt
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2021-03-10 18:49:11.205137 anesthetic-2.0.0b7/scripts/
--rwxr-xr-x   0 will      (1000) will      (1000)      582 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/scripts/anesthetic
--rw-r--r--   0 will      (1000) will      (1000)       38 2021-03-10 18:49:11.215136 anesthetic-2.0.0b7/setup.cfg
--rw-r--r--   0 will      (1000) will      (1000)     2226 2021-03-05 09:25:55.000000 anesthetic-2.0.0b7/setup.py
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2021-03-10 18:49:11.205137 anesthetic-2.0.0b7/tests/
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2021-03-10 18:49:11.211803 anesthetic-2.0.0b7/tests/example_data/
--rw-r--r--   0 will      (1000) will      (1000)       35 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/tests/example_data/gd.paramnames
--rw-r--r--   0 will      (1000) will      (1000)       43 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/tests/example_data/gd.ranges
--rw-r--r--   0 will      (1000) will      (1000)   601100 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/tests/example_data/gd_1.txt
--rw-r--r--   0 will      (1000) will      (1000)   601123 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/tests/example_data/gd_2.txt
--rw-r--r--   0 will      (1000) will      (1000)       35 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/tests/example_data/gd_single.paramnames
--rw-r--r--   0 will      (1000) will      (1000)       43 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/tests/example_data/gd_single.ranges
--rw-r--r--   0 will      (1000) will      (1000)  1202223 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/tests/example_data/gd_single.txt
--rw-r--r--   0 will      (1000) will      (1000)       35 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/tests/example_data/mn.paramnames
--rw-r--r--   0 will      (1000) will      (1000)       43 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/tests/example_data/mn.ranges
--rw-r--r--   0 will      (1000) will      (1000)       35 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/tests/example_data/mn_old.paramnames
--rw-r--r--   0 will      (1000) will      (1000)       43 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/tests/example_data/mn_old.ranges
--rw-r--r--   0 will      (1000) will      (1000)   190401 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/tests/example_data/mn_oldev.dat
--rw-r--r--   0 will      (1000) will      (1000)   163747 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/tests/example_data/mn_oldphys_live.points
--rw-r--r--   0 will      (1000) will      (1000)   214684 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/tests/example_data/mndead-birth.txt
--rw-r--r--   0 will      (1000) will      (1000)   190401 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/tests/example_data/mnev.dat
--rw-r--r--   0 will      (1000) will      (1000)    17375 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/tests/example_data/mnphys_live-birth.txt
--rw-r--r--   0 will      (1000) will      (1000)    15120 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/tests/example_data/mnphys_live.points
-drwxr-xr-x   0 will      (1000) will      (1000)        0 2021-03-10 18:49:11.215136 anesthetic-2.0.0b7/tests/example_data/mp/
--rw-r--r--   0 will      (1000) will      (1000)      679 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/tests/example_data/mp/2019-01-24_200000_.paramnames
--rw-r--r--   0 will      (1000) will      (1000)   699801 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/tests/example_data/mp/2019-01-24_200000__1.txt
--rw-r--r--   0 will      (1000) will      (1000)   699771 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/tests/example_data/mp/2019-01-24_200000__2.txt
--rw-r--r--   0 will      (1000) will      (1000)     7017 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/tests/example_data/mp/log.param
--rw-r--r--   0 will      (1000) will      (1000)      834 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/tests/example_data/mp/mp.bestfit
--rw-r--r--   0 will      (1000) will      (1000)     9959 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/tests/example_data/mp/mp.covmat
--rw-r--r--   0 will      (1000) will      (1000)     6301 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/tests/example_data/mp/mp.h_info
--rw-r--r--   0 will      (1000) will      (1000)      212 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/tests/example_data/mp/mp.log
--rw-r--r--   0 will      (1000) will      (1000)     2161 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/tests/example_data/mp/mp.tex
--rw-r--r--   0 will      (1000) will      (1000)     4363 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/tests/example_data/mp/mp.v_info
--rw-r--r--   0 will      (1000) will      (1000)       35 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/tests/example_data/pc.paramnames
--rw-r--r--   0 will      (1000) will      (1000)       30 2020-05-22 11:57:06.000000 anesthetic-2.0.0b7/tests/example_data/pc.ranges
--rw-r--r--   0 will      (1000) will      (1000)       35 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/tests/example_data/pc_250.paramnames
--rw-r--r--   0 will      (1000) will      (1000)       43 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/tests/example_data/pc_250.ranges
--rw-r--r--   0 will      (1000) will      (1000)   370744 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/tests/example_data/pc_250_dead-birth.txt
--rw-r--r--   0 will      (1000) will      (1000)    34233 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/tests/example_data/pc_250_phys_live-birth.txt
--rw-r--r--   0 will      (1000) will      (1000)   185280 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/tests/example_data/pc_dead-birth.txt
--rw-r--r--   0 will      (1000) will      (1000)    17125 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/tests/example_data/pc_phys_live-birth.txt
--rw-r--r--   0 will      (1000) will      (1000)       40 2020-05-21 17:26:53.000000 anesthetic-2.0.0b7/tests/matplotlib_agg.py
--rw-r--r--   0 will      (1000) will      (1000)      644 2021-03-05 09:25:55.000000 anesthetic-2.0.0b7/tests/test_convert.py
--rw-r--r--   0 will      (1000) will      (1000)     1278 2021-03-05 09:25:55.000000 anesthetic-2.0.0b7/tests/test_gui.py
--rw-r--r--   0 will      (1000) will      (1000)    18562 2021-03-10 18:48:07.000000 anesthetic-2.0.0b7/tests/test_plot.py
--rw-r--r--   0 will      (1000) will      (1000)    31338 2021-03-10 18:48:07.000000 anesthetic-2.0.0b7/tests/test_samples.py
--rw-r--r--   0 will      (1000) will      (1000)     4310 2021-03-10 18:48:03.000000 anesthetic-2.0.0b7/tests/test_utils.py
--rw-r--r--   0 will      (1000) will      (1000)    14411 2021-03-05 09:25:55.000000 anesthetic-2.0.0b7/tests/test_weighted_pandas.py
--rw-r--r--   0 will      (1000) will      (1000)     3080 2021-03-05 09:25:55.000000 anesthetic-2.0.0b7/tests/wedding_cake.py
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2021-07-15 13:19:17.999222 anesthetic-2.0.0b9/
+-rw-r--r--   0 will      (1000) will      (1000)       42 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/.coveragerc
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2021-07-15 13:19:17.985889 anesthetic-2.0.0b9/.github/
+-rw-r--r--   0 will      (1000) will      (1000)     3367 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 will      (1000) will      (1000)      836 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/.github/CONTRIBUTING.md
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2021-07-15 13:19:17.985889 anesthetic-2.0.0b9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 will      (1000) will      (1000)      438 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 will      (1000) will      (1000)      569 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 will      (1000) will      (1000)      531 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2021-07-15 13:19:17.985889 anesthetic-2.0.0b9/.github/workflows/
+-rw-r--r--   0 will      (1000) will      (1000)     2325 2021-07-14 10:25:30.000000 anesthetic-2.0.0b9/.github/workflows/CI.yml
+-rw-r--r--   0 will      (1000) will      (1000)      262 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/.gitignore
+-rw-r--r--   0 will      (1000) will      (1000)      540 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/.readthedocs.yml
+-rw-r--r--   0 will      (1000) will      (1000)     1069 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/LICENSE
+-rw-r--r--   0 will      (1000) will      (1000)     9674 2021-07-15 13:19:17.999222 anesthetic-2.0.0b9/PKG-INFO
+-rw-r--r--   0 will      (1000) will      (1000)     8553 2021-07-14 10:12:54.000000 anesthetic-2.0.0b9/README.rst
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2021-07-15 13:19:17.989223 anesthetic-2.0.0b9/anesthetic/
+-rw-r--r--   0 will      (1000) will      (1000)      400 2021-03-05 09:25:55.000000 anesthetic-2.0.0b9/anesthetic/__init__.py
+-rw-r--r--   0 will      (1000) will      (1000)      919 2020-05-31 10:39:15.000000 anesthetic-2.0.0b9/anesthetic/boundary.py
+-rw-r--r--   0 will      (1000) will      (1000)      886 2021-07-15 13:17:19.000000 anesthetic-2.0.0b9/anesthetic/convert.py
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2021-07-15 13:19:17.989223 anesthetic-2.0.0b9/anesthetic/gui/
+-rw-r--r--   0 will      (1000) will      (1000)       68 2020-05-31 09:10:19.000000 anesthetic-2.0.0b9/anesthetic/gui/__init__.py
+-rw-r--r--   0 will      (1000) will      (1000)     9211 2021-03-05 09:25:55.000000 anesthetic-2.0.0b9/anesthetic/gui/plot.py
+-rw-r--r--   0 will      (1000) will      (1000)     8255 2021-03-05 09:25:55.000000 anesthetic-2.0.0b9/anesthetic/gui/widgets.py
+-rw-r--r--   0 will      (1000) will      (1000)     2787 2021-07-06 16:58:04.000000 anesthetic-2.0.0b9/anesthetic/kde.py
+-rw-r--r--   0 will      (1000) will      (1000)    37395 2021-07-15 13:17:22.000000 anesthetic-2.0.0b9/anesthetic/plot.py
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2021-07-15 13:19:17.989223 anesthetic-2.0.0b9/anesthetic/read/
+-rw-r--r--   0 will      (1000) will      (1000)       44 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/anesthetic/read/__init__.py
+-rw-r--r--   0 will      (1000) will      (1000)      442 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/anesthetic/read/chainreader.py
+-rw-r--r--   0 will      (1000) will      (1000)     2850 2021-07-15 13:17:22.000000 anesthetic-2.0.0b9/anesthetic/read/cobayamcmcreader.py
+-rw-r--r--   0 will      (1000) will      (1000)     3484 2021-07-15 13:17:22.000000 anesthetic-2.0.0b9/anesthetic/read/getdistreader.py
+-rw-r--r--   0 will      (1000) will      (1000)     5747 2021-03-05 09:25:55.000000 anesthetic-2.0.0b9/anesthetic/read/montepythonreader.py
+-rw-r--r--   0 will      (1000) will      (1000)     2219 2020-05-31 10:39:15.000000 anesthetic-2.0.0b9/anesthetic/read/multinestreader.py
+-rw-r--r--   0 will      (1000) will      (1000)     1042 2020-05-31 10:39:15.000000 anesthetic-2.0.0b9/anesthetic/read/polychordreader.py
+-rw-r--r--   0 will      (1000) will      (1000)     1408 2021-07-15 13:17:22.000000 anesthetic-2.0.0b9/anesthetic/read/samplereader.py
+-rw-r--r--   0 will      (1000) will      (1000)    31526 2021-07-15 13:17:22.000000 anesthetic-2.0.0b9/anesthetic/samples.py
+-rw-r--r--   0 will      (1000) will      (1000)    14122 2021-07-14 10:43:38.000000 anesthetic-2.0.0b9/anesthetic/utils.py
+-rw-r--r--   0 will      (1000) will      (1000)    11588 2021-07-14 10:43:38.000000 anesthetic-2.0.0b9/anesthetic/weighted_pandas.py
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2021-07-15 13:19:17.989223 anesthetic-2.0.0b9/anesthetic.egg-info/
+-rw-r--r--   0 will      (1000) will      (1000)     9674 2021-07-15 13:19:17.000000 anesthetic-2.0.0b9/anesthetic.egg-info/PKG-INFO
+-rw-r--r--   0 will      (1000) will      (1000)     2928 2021-07-15 13:19:17.000000 anesthetic-2.0.0b9/anesthetic.egg-info/SOURCES.txt
+-rw-r--r--   0 will      (1000) will      (1000)        1 2021-07-15 13:19:17.000000 anesthetic-2.0.0b9/anesthetic.egg-info/dependency_links.txt
+-rw-r--r--   0 will      (1000) will      (1000)      172 2021-07-15 13:19:17.000000 anesthetic-2.0.0b9/anesthetic.egg-info/requires.txt
+-rw-r--r--   0 will      (1000) will      (1000)       11 2021-07-15 13:19:17.000000 anesthetic-2.0.0b9/anesthetic.egg-info/top_level.txt
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2021-07-15 13:19:17.989223 anesthetic-2.0.0b9/bin/
+-rwxr-xr-x   0 will      (1000) will      (1000)     5625 2020-05-31 10:39:15.000000 anesthetic-2.0.0b9/bin/gen_data.py
+-rw-r--r--   0 will      (1000) will      (1000)     3348 2020-05-31 10:39:15.000000 anesthetic-2.0.0b9/bin/plot.py
+-rwxr-xr-x   0 will      (1000) will      (1000)      214 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/bin/run_tests
+-rw-r--r--   0 will      (1000) will      (1000)    11766 2020-07-29 19:08:13.000000 anesthetic-2.0.0b9/demo.ipynb
+-rw-r--r--   0 will      (1000) will      (1000)     5623 2020-07-29 19:08:13.000000 anesthetic-2.0.0b9/demo.py
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2021-07-15 13:19:17.989223 anesthetic-2.0.0b9/docs/
+-rw-r--r--   0 will      (1000) will      (1000)      584 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/docs/Makefile
+-rw-r--r--   0 will      (1000) will      (1000)      791 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/docs/make.bat
+-rw-r--r--   0 will      (1000) will      (1000)       47 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/docs/requirements.txt
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2021-07-15 13:19:17.989223 anesthetic-2.0.0b9/docs/source/
+-rw-r--r--   0 will      (1000) will      (1000)      499 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/docs/source/anesthetic.gui.rst
+-rw-r--r--   0 will      (1000) will      (1000)     1000 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/docs/source/anesthetic.read.rst
+-rw-r--r--   0 will      (1000) will      (1000)      988 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/docs/source/anesthetic.rst
+-rw-r--r--   0 will      (1000) will      (1000)     6272 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/docs/source/conf.py
+-rw-r--r--   0 will      (1000) will      (1000)      187 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/docs/source/index.rst
+-rw-r--r--   0 will      (1000) will      (1000)       55 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/docs/source/intro.rst
+-rw-r--r--   0 will      (1000) will      (1000)       67 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/docs/source/modules.rst
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2021-07-15 13:19:17.989223 anesthetic-2.0.0b9/images/
+-rw-r--r--   0 will      (1000) will      (1000)   224235 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/images/anim_1.gif
+-rw-r--r--   0 will      (1000) will      (1000)      669 2020-05-31 10:39:15.000000 anesthetic-2.0.0b9/images/animate.py
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2021-07-15 13:19:17.992556 anesthetic-2.0.0b9/paper/
+-rw-r--r--   0 will      (1000) will      (1000)    50898 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/paper/2d.png
+-rw-r--r--   0 will      (1000) will      (1000)     1728 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/paper/Makefile
+-rw-r--r--   0 will      (1000) will      (1000)    13970 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/paper/paper.bib
+-rw-r--r--   0 will      (1000) will      (1000)     5900 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/paper/paper.md
+-rw-r--r--   0 will      (1000) will      (1000)       51 2021-07-06 16:58:04.000000 anesthetic-2.0.0b9/requirements.txt
+-rw-r--r--   0 will      (1000) will      (1000)       75 2021-07-06 16:58:04.000000 anesthetic-2.0.0b9/requirements_extras.txt
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2021-07-15 13:19:17.992556 anesthetic-2.0.0b9/scripts/
+-rwxr-xr-x   0 will      (1000) will      (1000)      582 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/scripts/anesthetic
+-rw-r--r--   0 will      (1000) will      (1000)       38 2021-07-15 13:19:17.999222 anesthetic-2.0.0b9/setup.cfg
+-rw-r--r--   0 will      (1000) will      (1000)     2239 2021-07-06 16:58:04.000000 anesthetic-2.0.0b9/setup.py
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2021-07-15 13:19:17.992556 anesthetic-2.0.0b9/tests/
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2021-07-15 13:19:17.995889 anesthetic-2.0.0b9/tests/example_data/
+-rw-r--r--   0 will      (1000) will      (1000)   268449 2021-07-15 13:17:22.000000 anesthetic-2.0.0b9/tests/example_data/cb.1.txt
+-rw-r--r--   0 will      (1000) will      (1000)   293862 2021-07-15 13:17:22.000000 anesthetic-2.0.0b9/tests/example_data/cb.2.txt
+-rw-r--r--   0 will      (1000) will      (1000)      258 2021-07-15 13:17:22.000000 anesthetic-2.0.0b9/tests/example_data/cb.input.yaml
+-rw-r--r--   0 will      (1000) will      (1000)     1156 2021-07-15 13:17:22.000000 anesthetic-2.0.0b9/tests/example_data/cb.updated.yaml
+-rw-r--r--   0 will      (1000) will      (1000)       35 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/tests/example_data/gd.paramnames
+-rw-r--r--   0 will      (1000) will      (1000)       43 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/tests/example_data/gd.ranges
+-rw-r--r--   0 will      (1000) will      (1000)   601100 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/tests/example_data/gd_1.txt
+-rw-r--r--   0 will      (1000) will      (1000)   601123 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/tests/example_data/gd_2.txt
+-rw-r--r--   0 will      (1000) will      (1000)       35 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/tests/example_data/gd_single.paramnames
+-rw-r--r--   0 will      (1000) will      (1000)       43 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/tests/example_data/gd_single.ranges
+-rw-r--r--   0 will      (1000) will      (1000)  1202223 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/tests/example_data/gd_single.txt
+-rw-r--r--   0 will      (1000) will      (1000)       35 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/tests/example_data/mn.paramnames
+-rw-r--r--   0 will      (1000) will      (1000)       43 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/tests/example_data/mn.ranges
+-rw-r--r--   0 will      (1000) will      (1000)       35 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/tests/example_data/mn_old.paramnames
+-rw-r--r--   0 will      (1000) will      (1000)       43 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/tests/example_data/mn_old.ranges
+-rw-r--r--   0 will      (1000) will      (1000)   190401 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/tests/example_data/mn_oldev.dat
+-rw-r--r--   0 will      (1000) will      (1000)   163747 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/tests/example_data/mn_oldphys_live.points
+-rw-r--r--   0 will      (1000) will      (1000)   214684 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/tests/example_data/mndead-birth.txt
+-rw-r--r--   0 will      (1000) will      (1000)   190401 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/tests/example_data/mnev.dat
+-rw-r--r--   0 will      (1000) will      (1000)    17375 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/tests/example_data/mnphys_live-birth.txt
+-rw-r--r--   0 will      (1000) will      (1000)    15120 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/tests/example_data/mnphys_live.points
+drwxr-xr-x   0 will      (1000) will      (1000)        0 2021-07-15 13:19:17.999222 anesthetic-2.0.0b9/tests/example_data/mp/
+-rw-r--r--   0 will      (1000) will      (1000)      679 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/tests/example_data/mp/2019-01-24_200000_.paramnames
+-rw-r--r--   0 will      (1000) will      (1000)   699801 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/tests/example_data/mp/2019-01-24_200000__1.txt
+-rw-r--r--   0 will      (1000) will      (1000)   699771 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/tests/example_data/mp/2019-01-24_200000__2.txt
+-rw-r--r--   0 will      (1000) will      (1000)     7017 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/tests/example_data/mp/log.param
+-rw-r--r--   0 will      (1000) will      (1000)      834 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/tests/example_data/mp/mp.bestfit
+-rw-r--r--   0 will      (1000) will      (1000)     9959 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/tests/example_data/mp/mp.covmat
+-rw-r--r--   0 will      (1000) will      (1000)     6301 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/tests/example_data/mp/mp.h_info
+-rw-r--r--   0 will      (1000) will      (1000)      212 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/tests/example_data/mp/mp.log
+-rw-r--r--   0 will      (1000) will      (1000)     2161 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/tests/example_data/mp/mp.tex
+-rw-r--r--   0 will      (1000) will      (1000)     4363 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/tests/example_data/mp/mp.v_info
+-rw-r--r--   0 will      (1000) will      (1000)       35 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/tests/example_data/pc.paramnames
+-rw-r--r--   0 will      (1000) will      (1000)       30 2020-05-22 11:57:06.000000 anesthetic-2.0.0b9/tests/example_data/pc.ranges
+-rw-r--r--   0 will      (1000) will      (1000)       35 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/tests/example_data/pc_250.paramnames
+-rw-r--r--   0 will      (1000) will      (1000)       43 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/tests/example_data/pc_250.ranges
+-rw-r--r--   0 will      (1000) will      (1000)   370744 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/tests/example_data/pc_250_dead-birth.txt
+-rw-r--r--   0 will      (1000) will      (1000)    34233 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/tests/example_data/pc_250_phys_live-birth.txt
+-rw-r--r--   0 will      (1000) will      (1000)   185280 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/tests/example_data/pc_dead-birth.txt
+-rw-r--r--   0 will      (1000) will      (1000)    17125 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/tests/example_data/pc_phys_live-birth.txt
+-rw-r--r--   0 will      (1000) will      (1000)       40 2020-05-21 17:26:53.000000 anesthetic-2.0.0b9/tests/matplotlib_agg.py
+-rw-r--r--   0 will      (1000) will      (1000)      644 2021-03-05 09:25:55.000000 anesthetic-2.0.0b9/tests/test_convert.py
+-rw-r--r--   0 will      (1000) will      (1000)     1582 2021-07-06 16:58:04.000000 anesthetic-2.0.0b9/tests/test_gui.py
+-rw-r--r--   0 will      (1000) will      (1000)    24128 2021-07-15 13:17:22.000000 anesthetic-2.0.0b9/tests/test_plot.py
+-rw-r--r--   0 will      (1000) will      (1000)    32383 2021-07-15 13:17:22.000000 anesthetic-2.0.0b9/tests/test_samples.py
+-rw-r--r--   0 will      (1000) will      (1000)     4310 2021-07-14 09:37:42.000000 anesthetic-2.0.0b9/tests/test_utils.py
+-rw-r--r--   0 will      (1000) will      (1000)    14587 2021-07-14 10:25:30.000000 anesthetic-2.0.0b9/tests/test_weighted_pandas.py
+-rw-r--r--   0 will      (1000) will      (1000)     3081 2021-07-15 13:17:22.000000 anesthetic-2.0.0b9/tests/wedding_cake.py
```

### Comparing `anesthetic-2.0.0b7/.github/CODE_OF_CONDUCT.md` & `anesthetic-2.0.0b9/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/.github/CONTRIBUTING.md` & `anesthetic-2.0.0b9/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/.github/ISSUE_TEMPLATE/feature_request.md` & `anesthetic-2.0.0b9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/.github/PULL_REQUEST_TEMPLATE.md` & `anesthetic-2.0.0b9/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/.github/workflows/CI.yml` & `anesthetic-2.0.0b9/.github/workflows/CI.yml`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 name: CI
 
 on:
   push:
     branches: [ master ]
   pull_request:
     branches: [ master ]
+  schedule:
+    - cron: "0 0 * * *"
 
   workflow_dispatch:
 
 jobs:
   lint:
     runs-on: ubuntu-latest
     steps:
@@ -74,11 +76,11 @@
       shell: bash -l {0}
       run: |
         conda install pytest pytest-cov pytest-xdist
         conda install --file requirements.txt
 
     - name: Test with pytest
       shell: bash -l {0}
-      run: pytest --cov=anesthetic -n auto tests
+      run: python -m pytest --cov=anesthetic -n auto tests
 
     - name: Upload coverage to Codecov
       uses: codecov/codecov-action@v1
```

### Comparing `anesthetic-2.0.0b7/.readthedocs.yml` & `anesthetic-2.0.0b9/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/LICENSE` & `anesthetic-2.0.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/PKG-INFO` & `anesthetic-2.0.0b9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,232 +1,15 @@
 Metadata-Version: 2.1
 Name: anesthetic
-Version: 2.0.0b7
+Version: 2.0.0b9
 Summary: anesthetic: nested sampling visualisation
 Home-page: https://github.com/williamjameshandley/anesthetic
 Author: Will Handley
 Author-email: wh260@cam.ac.uk
 License: MIT
-Description: =========================================
-        anesthetic: nested sampling visualisation
-        =========================================
-        :anesthetic: nested sampling visualisation
-        :Author: Will Handley and Lukas Hergt
-        :Version: 2.0.0-beta.7
-        :Homepage: https://github.com/williamjameshandley/anesthetic
-        :Documentation: http://anesthetic.readthedocs.io/
-        
-        .. image:: https://travis-ci.com/williamjameshandley/anesthetic.svg?branch=master
-           :target: https://travis-ci.com/williamjameshandley/anesthetic
-           :alt: Build Status
-        .. image:: https://circleci.com/gh/williamjameshandley/anesthetic.svg?style=svg
-           :target: https://circleci.com/gh/williamjameshandley/anesthetic
-        .. image:: https://codecov.io/gh/williamjameshandley/anesthetic/branch/master/graph/badge.svg
-           :target: https://codecov.io/gh/williamjameshandley/anesthetic
-           :alt: Test Coverage Status
-        .. image:: https://readthedocs.org/projects/anesthetic/badge/?version=latest
-           :target: https://anesthetic.readthedocs.io/en/latest/?badge=latest
-           :alt: Documentation Status
-        .. image:: https://badge.fury.io/py/anesthetic.svg
-           :target: https://badge.fury.io/py/anesthetic
-           :alt: PyPi location
-        .. image:: https://zenodo.org/badge/175663535.svg
-           :target: https://zenodo.org/badge/latestdoi/175663535
-           :alt: Permanent DOI for this release
-        .. image:: http://joss.theoj.org/papers/8c51bffda75d122cf4a8b991e18d3e45/status.svg
-           :target: http://joss.theoj.org/papers/8c51bffda75d122cf4a8b991e18d3e45
-           :alt: Review Status
-        .. image:: https://img.shields.io/badge/license-MIT-blue.svg
-           :target: https://github.com/williamjameshandley/anesthetic/blob/master/LICENSE
-           :alt: License information
-        .. image:: https://mybinder.org/badge_logo.svg
-           :target: https://mybinder.org/v2/gh/williamjameshandley/anesthetic/1.0.0?filepath=demo.ipynb
-           :alt: Online interactive notebook
-        
-        
-        
-        
-        
-        ``anesthetic`` brings together tools for processing nested sampling chains, leveraging standard scientific python libraries.
-        
-        You can see example usage and plots in the `plot gallery <http://htmlpreview.github.io/?https://github.com/williamjameshandley/cosmo_example/blob/master/demos/demo.html>`_, or in the corresponding `Jupyter notebook <https://mybinder.org/v2/gh/williamjameshandley/anesthetic/master?filepath=demo.ipynb>`_.
-        
-        Current functionality includes:
-        
-        - Computation of Bayesian evidences, Kullback-Liebler divergences and Bayesian model dimensionalities.
-        - Marginalised 1d and 2d plots.
-        - Dynamic replaying of nested sampling.
-        
-        This tool was designed primarily for use with nested sampling outputs, although it can be used for normal MCMC chains.
-        
-        For an interactive view of a nested sampling run, you can use the ``anesthetic`` script.
-        
-        .. code:: bash
-        
-           $ anesthetic <ns file root>
-        
-        .. image:: https://github.com/williamjameshandley/anesthetic/raw/master/images/anim_1.gif
-        
-        Features
-        --------
-        
-        - Both samples and plotting axes are stored as a ``pandas.DataFrame``, with parameter names as indices, which makes for easy access and modification.
-        - Sensible color scheme for plotting nearly flat distributions.
-        - For easy extension/modification, uses the standard python libraries:
-          `numpy <https://www.numpy.org/>`__,
-          `scipy <https://www.scipy.org/>`__,
-          `matplotlib <https://matplotlib.org/>`__
-          and `pandas <https://pandas.pydata.org/>`__.
-        
-        Installation
-        ------------
-        
-        ``anesthetic`` can be installed via pip
-        
-        .. code:: bash
-        
-            pip install anesthetic
-        
-        or via the setup.py
-        
-        .. code:: bash
-        
-            git clone https://github.com/williamjameshandley/anesthetic
-            cd anesthetic
-            python setup.py install --user
-        
-        You can check that things are working by running the test suite:
-        
-        .. code:: bash
-        
-            export MPLBACKEND=Agg     # only necessary for OSX users
-            python -m pytest
-            flake8 anesthetic tests
-            pydocstyle --convention=numpy anesthetic
-        
-        
-        Dependencies
-        ~~~~~~~~~~~~
-        
-        Basic requirements:
-        
-        - Python 3.6+
-        - `matplotlib <https://pypi.org/project/matplotlib/>`__
-        - `numpy <https://pypi.org/project/numpy/>`__
-        - `scipy <https://pypi.org/project/scipy/>`__
-        - `pandas <https://pypi.org/project/pandas/>`__
-        - `fastKDE <https://pypi.org/project/fastkde/>`__
-        
-        Documentation:
-        
-        - `sphinx <https://pypi.org/project/Sphinx/>`__
-        - `numpydoc <https://pypi.org/project/numpydoc/>`__
-        
-        Tests:
-        
-        - `pytest <https://pypi.org/project/pytest/>`__
-        
-        Documentation
-        -------------
-        
-        Full Documentation is hosted at `ReadTheDocs <http://anesthetic.readthedocs.io/>`__.  To build your own local copy of the documentation you'll need to install `sphinx <https://pypi.org/project/Sphinx/>`__. You can then run:
-        
-        .. code:: bash
-        
-           cd docs
-           make html
-        
-        
-        Citation
-        --------
-        
-        If you use ``anesthetic`` to generate plots for a publication, please cite
-        as: ::
-        
-           Handley, (2019). anesthetic: nested sampling visualisation. Journal of Open
-           Source Software, 4(37), 1414, https://doi.org/10.21105/joss.01414
-        
-        or using the BibTeX:
-        
-        .. code:: bibtex
-        
-           @article{anesthetic,
-               doi = {10.21105/joss.01414},
-               url = {http://dx.doi.org/10.21105/joss.01414},
-               year  = {2019},
-               month = {Jun},
-               publisher = {The Open Journal},
-               volume = {4},
-               number = {37},
-               pages = {1414},
-               author = {Will Handley},
-               title = {anesthetic: nested sampling visualisation},
-               journal = {The Journal of Open Source Software}
-           }
-        
-        
-        Contributing
-        ------------
-        There are many ways you can contribute via the `GitHub repository <https://github.com/williamjameshandley/anesthetic>`__.
-        
-        - You can `open an issue <https://github.com/williamjameshandley/anesthetic/issues>`__ to report bugs or to propose new features.
-        - Pull requests are very welcome. Note that if you are going to propose major changes, be sure to open an issue for discussion first, to make sure that your PR will be accepted before you spend effort coding it.
-        
-        
-        Questions/Comments
-        ------------------
-        Another posterior plotting tool?
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-            This is my posterior plotter. There are many like it, but this one is mine.
-        
-        There are several excellent tools for plotting marginalised posteriors:
-        
-        - `getdist <http://getdist.readthedocs.io/en/latest/intro.html>`__
-        - `corner <https://corner.readthedocs.io>`__
-        - `pygtc <https://pygtc.readthedocs.io>`__
-        - `dynesty <https://dynesty.readthedocs.io>`__
-        - `MontePython <http://baudren.github.io/montepython.html>`__
-        
-        Why create another one? In general, any dedicated user of software will find that there is some functionality that in their use case is lacking, and the designs of previous codes make such extensions challenging. In my case this was:
-        
-        1. For large numbers of samples, kernel density estimation is slow, or inaccurate (particularly for samples generated from nested sampling). There are kernel density estimators, such as `fastKDE <https://pypi.org/project/fastkde/>`__, which ameliorate many of these difficulties.
-        
-        2. Existing tools can make it difficult to define new parameters. For example, the default cosmomc chain defines ``omegabh2``, but not ``omegab``. The transformation is easy, since ``omegab = omegabh2/ (H0/100)**2``, but implementing this transformation in existing packages is not so trivial. ``anesthetic`` solves this issue by storing the samples as a pandas array, for which the relevant code for defining the above new parameter would be
-        
-        .. code:: python
-        
-            from anesthetic import MCMCSamples
-            samples = MCMCSamples(root=file_root)                         # Load the samples
-            samples['omegab'] = samples.omegabh2/(samples.H0/100)**2      # Define omegab
-            samples.tex['omegab'] = '$\Omega_b$'                          # Label omegab
-            samples.plot_1d('omegab')                                     # Simple 1D plot
-        
-        3. Many KDE plotting tools have conventions that don't play well with uniformly distributed parameters, which presents a problem if you are trying to plot priors along with your posteriors. ``anesthetic`` has a sensible mechanism, by defining the contours by the amount of iso-probability mass they contain, but colouring the fill in relation to the probability density of the contour.
-        
-        What's in a name?
-        ~~~~~~~~~~~~~~~~~
-        
-        There is an emerging convention for naming nested sampling packages with words that have nest in them (`nestle and dynesty <https://dynesty.readthedocs.io/en/latest/>`__, `nestorflow <https://github.com/tomcharnock/NestorFlow>`__). Doing a UNIX grep:
-        
-        .. code:: bash
-        
-            grep nest /usr/share/dict/words
-        
-        yields a lot of superlatives (e.g. greenest), but a few other cool names for future projects:
-        
-        - amnesty
-        - defenestrate
-        - dishonestly
-        - inestimable
-        - minestrone
-        - rhinestone
-        
-        I chose ``anesthetic`` because I liked the soft 'th', and in spite of the US spelling.
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
@@ -237,7 +20,225 @@
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Provides-Extra: docs
 Provides-Extra: automated bins calculation
 Provides-Extra: fast kernel density estimation
+License-File: LICENSE
+
+=========================================
+anesthetic: nested sampling visualisation
+=========================================
+:anesthetic: nested sampling visualisation
+:Author: Will Handley and Lukas Hergt
+:Version: 2.0.0-beta.9
+:Homepage: https://github.com/williamjameshandley/anesthetic
+:Documentation: http://anesthetic.readthedocs.io/
+
+.. image:: https://github.com/williamjameshandley/anesthetic/workflows/CI/badge.svg?branch=master
+   :target: https://github.com/williamjameshandley/anesthetic/actions?query=workflow%3ACI+branch%3Amaster
+   :alt: Build Status
+.. image:: https://codecov.io/gh/williamjameshandley/anesthetic/branch/master/graph/badge.svg
+   :target: https://codecov.io/gh/williamjameshandley/anesthetic
+   :alt: Test Coverage Status
+.. image:: https://readthedocs.org/projects/anesthetic/badge/?version=latest
+   :target: https://anesthetic.readthedocs.io/en/latest/?badge=latest
+   :alt: Documentation Status
+.. image:: https://badge.fury.io/py/anesthetic.svg
+   :target: https://badge.fury.io/py/anesthetic
+   :alt: PyPi location
+.. image:: https://zenodo.org/badge/175663535.svg
+   :target: https://zenodo.org/badge/latestdoi/175663535
+   :alt: Permanent DOI for this release
+.. image:: http://joss.theoj.org/papers/8c51bffda75d122cf4a8b991e18d3e45/status.svg
+   :target: http://joss.theoj.org/papers/8c51bffda75d122cf4a8b991e18d3e45
+   :alt: Review Status
+.. image:: https://img.shields.io/badge/license-MIT-blue.svg
+   :target: https://github.com/williamjameshandley/anesthetic/blob/master/LICENSE
+   :alt: License information
+.. image:: https://mybinder.org/badge_logo.svg
+   :target: https://mybinder.org/v2/gh/williamjameshandley/anesthetic/1.0.0?filepath=demo.ipynb
+   :alt: Online interactive notebook
+
+
+
+
+
+``anesthetic`` brings together tools for processing nested sampling chains, leveraging standard scientific python libraries.
+
+You can see example usage and plots in the `plot gallery <http://htmlpreview.github.io/?https://github.com/williamjameshandley/cosmo_example/blob/master/demos/demo.html>`_, or in the corresponding `Jupyter notebook <https://mybinder.org/v2/gh/williamjameshandley/anesthetic/master?filepath=demo.ipynb>`_.
+
+Current functionality includes:
+
+- Computation of Bayesian evidences, Kullback-Liebler divergences and Bayesian model dimensionalities.
+- Marginalised 1d and 2d plots.
+- Dynamic replaying of nested sampling.
+
+This tool was designed primarily for use with nested sampling outputs, although it can be used for normal MCMC chains.
+
+For an interactive view of a nested sampling run, you can use the ``anesthetic`` script.
+
+.. code:: bash
+
+   $ anesthetic <ns file root>
+
+.. image:: https://github.com/williamjameshandley/anesthetic/raw/master/images/anim_1.gif
+
+Features
+--------
+
+- Both samples and plotting axes are stored as a ``pandas.DataFrame``, with parameter names as indices, which makes for easy access and modification.
+- Sensible color scheme for plotting nearly flat distributions.
+- For easy extension/modification, uses the standard python libraries:
+  `numpy <https://www.numpy.org/>`__,
+  `scipy <https://www.scipy.org/>`__,
+  `matplotlib <https://matplotlib.org/>`__
+  and `pandas <https://pandas.pydata.org/>`__.
+
+Installation
+------------
+
+``anesthetic`` can be installed via pip
+
+.. code:: bash
+
+    pip install anesthetic
+
+or via the setup.py
+
+.. code:: bash
+
+    git clone https://github.com/williamjameshandley/anesthetic
+    cd anesthetic
+    python setup.py install --user
+
+You can check that things are working by running the test suite:
+
+.. code:: bash
+
+    export MPLBACKEND=Agg     # only necessary for OSX users
+    python -m pytest
+    flake8 anesthetic tests
+    pydocstyle --convention=numpy anesthetic
+
+
+Dependencies
+~~~~~~~~~~~~
+
+Basic requirements:
+
+- Python 3.6+
+- `matplotlib <https://pypi.org/project/matplotlib/>`__
+- `numpy <https://pypi.org/project/numpy/>`__
+- `scipy <https://pypi.org/project/scipy/>`__
+- `pandas <https://pypi.org/project/pandas/>`__
+- `fastKDE <https://pypi.org/project/fastkde/>`__
+
+Documentation:
+
+- `sphinx <https://pypi.org/project/Sphinx/>`__
+- `numpydoc <https://pypi.org/project/numpydoc/>`__
+
+Tests:
+
+- `pytest <https://pypi.org/project/pytest/>`__
+
+Documentation
+-------------
+
+Full Documentation is hosted at `ReadTheDocs <http://anesthetic.readthedocs.io/>`__.  To build your own local copy of the documentation you'll need to install `sphinx <https://pypi.org/project/Sphinx/>`__. You can then run:
+
+.. code:: bash
+
+   cd docs
+   make html
+
+
+Citation
+--------
+
+If you use ``anesthetic`` to generate plots for a publication, please cite
+as: ::
+
+   Handley, (2019). anesthetic: nested sampling visualisation. Journal of Open
+   Source Software, 4(37), 1414, https://doi.org/10.21105/joss.01414
+
+or using the BibTeX:
+
+.. code:: bibtex
+
+   @article{anesthetic,
+       doi = {10.21105/joss.01414},
+       url = {http://dx.doi.org/10.21105/joss.01414},
+       year  = {2019},
+       month = {Jun},
+       publisher = {The Open Journal},
+       volume = {4},
+       number = {37},
+       pages = {1414},
+       author = {Will Handley},
+       title = {anesthetic: nested sampling visualisation},
+       journal = {The Journal of Open Source Software}
+   }
+
+
+Contributing
+------------
+There are many ways you can contribute via the `GitHub repository <https://github.com/williamjameshandley/anesthetic>`__.
+
+- You can `open an issue <https://github.com/williamjameshandley/anesthetic/issues>`__ to report bugs or to propose new features.
+- Pull requests are very welcome. Note that if you are going to propose major changes, be sure to open an issue for discussion first, to make sure that your PR will be accepted before you spend effort coding it.
+
+
+Questions/Comments
+------------------
+Another posterior plotting tool?
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+    This is my posterior plotter. There are many like it, but this one is mine.
+
+There are several excellent tools for plotting marginalised posteriors:
+
+- `getdist <http://getdist.readthedocs.io/en/latest/intro.html>`__
+- `corner <https://corner.readthedocs.io>`__
+- `pygtc <https://pygtc.readthedocs.io>`__
+- `dynesty <https://dynesty.readthedocs.io>`__
+- `MontePython <http://baudren.github.io/montepython.html>`__
+
+Why create another one? In general, any dedicated user of software will find that there is some functionality that in their use case is lacking, and the designs of previous codes make such extensions challenging. In my case this was:
+
+1. For large numbers of samples, kernel density estimation is slow, or inaccurate (particularly for samples generated from nested sampling). There are kernel density estimators, such as `fastKDE <https://pypi.org/project/fastkde/>`__, which ameliorate many of these difficulties.
+
+2. Existing tools can make it difficult to define new parameters. For example, the default cosmomc chain defines ``omegabh2``, but not ``omegab``. The transformation is easy, since ``omegab = omegabh2/ (H0/100)**2``, but implementing this transformation in existing packages is not so trivial. ``anesthetic`` solves this issue by storing the samples as a pandas array, for which the relevant code for defining the above new parameter would be
+
+.. code:: python
+
+    from anesthetic import MCMCSamples
+    samples = MCMCSamples(root=file_root)                         # Load the samples
+    samples['omegab'] = samples.omegabh2/(samples.H0/100)**2      # Define omegab
+    samples.tex['omegab'] = '$\Omega_b$'                          # Label omegab
+    samples.plot_1d('omegab')                                     # Simple 1D plot
+
+3. Many KDE plotting tools have conventions that don't play well with uniformly distributed parameters, which presents a problem if you are trying to plot priors along with your posteriors. ``anesthetic`` has a sensible mechanism, by defining the contours by the amount of iso-probability mass they contain, but colouring the fill in relation to the probability density of the contour.
+
+What's in a name?
+~~~~~~~~~~~~~~~~~
+
+There is an emerging convention for naming nested sampling packages with words that have nest in them (`nestle and dynesty <https://dynesty.readthedocs.io/en/latest/>`__, `nestorflow <https://github.com/tomcharnock/NestorFlow>`__). Doing a UNIX grep:
+
+.. code:: bash
+
+    grep nest /usr/share/dict/words
+
+yields a lot of superlatives (e.g. greenest), but a few other cool names for future projects:
+
+- amnesty
+- defenestrate
+- dishonestly
+- inestimable
+- minestrone
+- rhinestone
+
+I chose ``anesthetic`` because I liked the soft 'th', and in spite of the US spelling.
+
+
```

### Comparing `anesthetic-2.0.0b7/README.rst` & `anesthetic-2.0.0b9/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 =========================================
 anesthetic: nested sampling visualisation
 =========================================
 :anesthetic: nested sampling visualisation
 :Author: Will Handley and Lukas Hergt
-:Version: 2.0.0-beta.7
+:Version: 2.0.0-beta.9
 :Homepage: https://github.com/williamjameshandley/anesthetic
 :Documentation: http://anesthetic.readthedocs.io/
 
-.. image:: https://travis-ci.com/williamjameshandley/anesthetic.svg?branch=master
-   :target: https://travis-ci.com/williamjameshandley/anesthetic
+.. image:: https://github.com/williamjameshandley/anesthetic/workflows/CI/badge.svg?branch=master
+   :target: https://github.com/williamjameshandley/anesthetic/actions?query=workflow%3ACI+branch%3Amaster
    :alt: Build Status
-.. image:: https://circleci.com/gh/williamjameshandley/anesthetic.svg?style=svg
-   :target: https://circleci.com/gh/williamjameshandley/anesthetic
 .. image:: https://codecov.io/gh/williamjameshandley/anesthetic/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/williamjameshandley/anesthetic
    :alt: Test Coverage Status
 .. image:: https://readthedocs.org/projects/anesthetic/badge/?version=latest
    :target: https://anesthetic.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 .. image:: https://badge.fury.io/py/anesthetic.svg
```

### Comparing `anesthetic-2.0.0b7/anesthetic/boundary.py` & `anesthetic-2.0.0b9/anesthetic/boundary.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/anesthetic/convert.py` & `anesthetic-2.0.0b9/anesthetic/convert.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/anesthetic/gui/plot.py` & `anesthetic-2.0.0b9/anesthetic/gui/plot.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/anesthetic/gui/widgets.py` & `anesthetic-2.0.0b9/anesthetic/gui/widgets.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/anesthetic/kde.py` & `anesthetic-2.0.0b9/anesthetic/kde.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         p = p[x >= xmin]
         x = x[x >= xmin]
 
     if xmax is not None:
         p = p[x <= xmax]
         x = x[x <= xmax]
 
-    return x, p
+    return x, p, xmin, xmax
 
 
 def fastkde_2d(d_x, d_y, xmin=None, xmax=None, ymin=None, ymax=None):
     """Perform a two-dimensional kernel density estimation.
 
     Wrapper round fastkde.fastKDE. Boundary corrections implemented by
     reflecting boundary conditions.
@@ -99,8 +99,8 @@
         p = p[y >= ymin, :]
         y = y[y >= ymin]
 
     if ymax is not None:
         p = p[y <= ymax, :]
         y = y[y <= ymax]
 
-    return x, y, p
+    return x, y, p, xmin, xmax, ymin, ymax
```

### Comparing `anesthetic-2.0.0b7/anesthetic/plot.py` & `anesthetic-2.0.0b9/anesthetic/plot.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,14 +32,102 @@
                               triangular_sample_compression_2d,
                               iso_probability_contours,
                               iso_probability_contours_from_samples,
                               scaled_triangulation, match_contour_to_contourf)
 from anesthetic.boundary import cut_and_normalise_gaussian
 
 
+class AxesSeries(pandas.Series):
+    """Anesthetic's axes version of `pandas.Series`."""
+
+    @property
+    def _constructor(self):
+        return AxesSeries
+
+    @property
+    def _constructor_expanddim(self):
+        return AxesDataFrame
+
+
+class AxesDataFrame(pandas.DataFrame):
+    """Anesthetic's axes version of `pandas.DataFrame`."""
+
+    @property
+    def _constructor(self):
+        return AxesDataFrame
+
+    @property
+    def _constructor_sliced(self):
+        return AxesSeries
+
+    def axlines(self, params, values, **kwargs):
+        """Add vertical and horizontal lines across all axes.
+
+        Parameters
+        ----------
+            params : str or list(str)
+                parameter label(s).
+                Should match the size of `values`.
+            values : float or list(float)
+                value(s) at which vertical and horizontal lines shall be added.
+                Should match the size of `params`.
+            kwargs
+                Any kwarg that can be passed to `plt.axvline` or `plt.axhline`.
+
+        """
+        params = np.ravel(params)
+        values = np.ravel(values)
+        if params.size != values.size:
+            raise ValueError("The sizes of `params` and `values` must match "
+                             "exactly, but params.size=%s and values.size=%s."
+                             % (params.size, values.size))
+        for i, param in enumerate(params):
+            if param in self.columns:
+                for ax in self.loc[:, param]:
+                    ax.axvline(values[i], **kwargs)
+            if param in self.index:
+                for ax in self.loc[param, self.columns != param]:
+                    ax.axhline(values[i], **kwargs)
+
+    def axspans(self, params, vmins, vmaxs, **kwargs):
+        """Add vertical and horizontal spans across all axes.
+
+        Parameters
+        ----------
+            params : str or list(str)
+                parameter label(s).
+                Should match the size of `vmins` and `vmaxs`.
+            vmins : float or list(float)
+                Minimum value of the vertical and horizontal axes spans.
+                Should match the size of `params`.
+            vmaxs : float or list(float)
+                Maximum value of the vertical and horizontal axes spans.
+                Should match the size of `params`.
+            kwargs
+                Any kwarg that can be passed to `plt.axvspan` or `plt.axhspan`.
+
+        """
+        kwargs = normalize_kwargs(kwargs, dict(color=['c']))
+        params = np.ravel(params)
+        vmins = np.ravel(vmins)
+        vmaxs = np.ravel(vmaxs)
+        if params.size != vmins.size:
+            raise ValueError("The sizes of `params`, `vmins` and `vmaxs` must "
+                             "match exactly, but params.size=%s, "
+                             "vmins.size=%s and vmaxs.size=%s."
+                             % (params.size, vmins.size, vmaxs.size))
+        for i, param in enumerate(params):
+            if param in self.columns:
+                for ax in self.loc[:, param]:
+                    ax.axvspan(vmins[i], vmaxs[i], **kwargs)
+            if param in self.index:
+                for ax in self.loc[param, self.columns != param]:
+                    ax.axhspan(vmins[i], vmaxs[i], **kwargs)
+
+
 def make_1d_axes(params, **kwargs):
     """Create a set of axes for plotting 1D marginalised posteriors.
 
     Parameters
     ----------
         params: list(str)
             names of parameters.
@@ -64,15 +152,15 @@
     fig: matplotlib.figure.Figure
         New or original (if supplied) figure object
 
     axes: pandas.Series(matplotlib.axes.Axes)
         Pandas array of axes objects
 
     """
-    axes = pandas.Series(index=np.atleast_1d(params), dtype=object)
+    axes = AxesSeries(index=np.atleast_1d(params), dtype=object)
     axes[:] = None
     tex = kwargs.pop('tex', {})
     fig = kwargs.pop('fig') if 'fig' in kwargs else plt.figure()
     ncols = kwargs.pop('ncols', int(np.ceil(np.sqrt(len(axes)))))
     nrows = int(np.ceil(len(axes)/float(ncols)))
     if 'subplot_spec' in kwargs:
         grid = SGS(nrows, ncols, wspace=0,
@@ -116,14 +204,20 @@
             diagonal, or to create a 1D marginalised plot on the diagonal.
             Default: True
 
         fig: matplotlib.figure.Figure, optional
             Figure to plot on.
             Default: matplotlib.pyplot.figure()
 
+        ticks: str
+            If 'outer', plot ticks only on the very left and very bottom.
+            If 'inner', plot ticks also in inner subplots.
+            If None, plot no ticks at all.
+            Default: 'outer'
+
         subplot_spec: matplotlib.gridspec.GridSpec, optional
             gridspec to plot array as part of a subfigure.
             Default: None
 
     Returns
     -------
     fig: matplotlib.figure.Figure
@@ -134,21 +228,22 @@
 
     """
     if nest_level(params) == 2:
         xparams, yparams = params
     else:
         xparams = yparams = params
 
+    ticks = kwargs.pop('ticks', 'outer')
     upper = kwargs.pop('upper', True)
     lower = kwargs.pop('lower', True)
     diagonal = kwargs.pop('diagonal', True)
 
-    axes = pandas.DataFrame(index=np.atleast_1d(yparams),
-                            columns=np.atleast_1d(xparams),
-                            dtype=object)
+    axes = AxesDataFrame(index=np.atleast_1d(yparams),
+                         columns=np.atleast_1d(xparams),
+                         dtype=object)
     axes[:][:] = None
     all_params = list(axes.columns) + list(axes.index)
 
     for j, y in enumerate(axes.index):
         for i, x in enumerate(axes.columns):
             if all_params.index(x) < all_params.index(y):
                 if lower:
@@ -175,63 +270,107 @@
     if kwargs:
         raise TypeError('Unexpected **kwargs: %r' % kwargs)
 
     if axes.size == 0:
         return fig, axes
     position = axes.copy()
     axes[:][:] = None
-    for j, y in enumerate(axes.index):
+    for j, y in enumerate(axes.index[::-1]):
         for i, x in enumerate(axes.columns):
             if position[x][y] is not None:
                 sx = list(axes[x].dropna())
                 sx = sx[0] if sx else None
                 sy = list(axes.T[y].dropna())
                 sy = sy[0] if sy else None
-                axes[x][y] = fig.add_subplot(grid[j, i],
+                axes[x][y] = fig.add_subplot(grid[axes.index.size-1-j, i],
                                              sharex=sx, sharey=sy)
 
                 if position[x][y] == 0:
                     axes[x][y].twin = axes[x][y].twinx()
                     axes[x][y].twin.set_yticks([])
                     axes[x][y].twin.set_ylim(0, 1.1)
                     axes[x][y].set_zorder(axes[x][y].twin.get_zorder() + 1)
                     axes[x][y].lines = axes[x][y].twin.lines
                     axes[x][y].patches = axes[x][y].twin.patches
                     axes[x][y].collections = axes[x][y].twin.collections
                     axes[x][y].containers = axes[x][y].twin.containers
                     make_diagonal(axes[x][y])
                     axes[x][y].position = 'diagonal'
-                elif position[x][y] == 1:
-                    axes[x][y].position = 'upper'
-                elif position[x][y] == -1:
-                    axes[x][y].position = 'lower'
+                    axes[x][y].twin.xaxis.set_major_locator(
+                        MaxNLocator(3, prune='both'))
+                else:
+                    if position[x][y] == 1:
+                        axes[x][y].position = 'upper'
+                    elif position[x][y] == -1:
+                        axes[x][y].position = 'lower'
+                    axes[x][y].yaxis.set_major_locator(
+                        MaxNLocator(3, prune='both'))
+                axes[x][y].xaxis.set_major_locator(
+                    MaxNLocator(3, prune='both'))
 
     for y, ax in axes.bfill(axis=1).iloc[:, 0].dropna().iteritems():
         ax.set_ylabel(tex[y])
 
     for x, ax in axes.ffill(axis=0).iloc[-1, :].dropna().iteritems():
         ax.set_xlabel(tex[x])
 
+    # left and right ticks and labels
     for y, ax in axes.iterrows():
         ax_ = ax.dropna()
-        if len(ax_):
+        if len(ax_) and ticks == 'inner':
+            for i, a in enumerate(ax_):
+                if i == 0:  # first column
+                    if a.position == 'diagonal' and len(ax_) == 1:
+                        a.tick_params('y', left=False, labelleft=False)
+                    else:
+                        a.tick_params('y', left=True, labelleft=True)
+                elif a.position == 'diagonal':  # not first column
+                    tl = a.yaxis.majorTicks[0].tick1line.get_markersize()
+                    a.tick_params('y', direction='out', length=tl/2,
+                                  left=True, labelleft=False)
+                else:  # not diagonal and not first column
+                    a.tick_params('y', direction='inout',
+                                  left=True, labelleft=False)
+        elif len(ax_) and ticks == 'outer':  # no inner ticks
             for a in ax_[1:]:
                 a.tick_params('y', left=False, labelleft=False)
+        elif len(ax_) and ticks is None:  # no ticks at all
+            for a in ax_:
+                a.tick_params('y', left=False, right=False,
+                              labelleft=False, labelright=False)
+        else:
+            raise ValueError(
+                "ticks=%s was requested, but ticks can only be one of "
+                "['outer', 'inner', None]." % ticks)
 
+    # bottom and top ticks and labels
     for x, ax in axes.iteritems():
         ax_ = ax.dropna()
         if len(ax_):
-            for a in ax_[:-1]:
-                a.tick_params('x', bottom=False, labelbottom=False)
-
-    for y, ax in axes.bfill(axis=1).iloc[:, 0].dropna().iteritems():
-        ax.yaxis.set_major_locator(MaxNLocator(3, prune='both'))
-
-    for x, ax in axes.ffill(axis=0).iloc[-1, :].dropna().iteritems():
-        ax.xaxis.set_major_locator(MaxNLocator(3, prune='both'))
+            if ticks == 'inner':
+                for i, a in enumerate(ax_):
+                    if i == len(ax_) - 1:  # bottom row
+                        a.tick_params('x', bottom=True, labelbottom=True)
+                    else:  # not bottom row
+                        a.tick_params('x', direction='inout',
+                                      bottom=True, labelbottom=False)
+                        if a.position == 'diagonal':
+                            a.twin.tick_params('x', direction='inout',
+                                               bottom=True, labelbottom=False)
+            elif ticks == 'outer':  # no inner ticks
+                for a in ax_[:-1]:
+                    a.tick_params('x', bottom=False, labelbottom=False)
+            elif ticks is None:  # no ticks at all
+                for a in ax_:
+                    a.tick_params('x', bottom=False, top=False,
+                                  labelbottom=False, labeltop=False)
+            else:
+                raise ValueError(
+                    "ticks=%s was requested, but ticks can only be one of "
+                    "['outer', 'inner', None]." % ticks)
 
     return fig, axes
 
 
 def fastkde_plot_1d(ax, data, *args, **kwargs):
     """Plot a 1d marginalised distribution.
 
@@ -279,14 +418,15 @@
     if data.max()-data.min() <= 0:
         return
 
     levels = kwargs.pop('levels', [0.68, 0.95])
 
     xmin = kwargs.pop('xmin', None)
     xmax = kwargs.pop('xmax', None)
+    density = kwargs.pop('density', False)
     cmap = kwargs.pop('cmap', None)
     color = kwargs.pop('color', (next(ax._get_lines.prop_cycler)['color']
                                  if cmap is None else cmap(0.68)))
     facecolor = kwargs.pop('facecolor', False)
 
     if 'edgecolor' in kwargs:
         edgecolor = kwargs.pop('edgecolor')
@@ -295,22 +435,23 @@
     else:
         edgecolor = color
 
     q = kwargs.pop('q', '5sigma')
     q = quantile_plot_interval(q=q)
 
     try:
-        x, p = fastkde_1d(data, xmin, xmax)
+        x, p, xmin, xmax = fastkde_1d(data, xmin, xmax)
     except NameError:
         raise ImportError("You need to install fastkde to use fastkde")
     p /= p.max()
     i = ((x > quantile(x, q[0], p)) & (x < quantile(x, q[1], p)))
 
-    ans = ax.plot(x[i], p[i], color=color, *args, **kwargs)
-    ax.set_xlim(*check_bounds(x[i], xmin, xmax), auto=True)
+    area = np.trapz(x=x[i], y=p[i]) if density else 1
+    ans = ax.plot(x[i], p[i]/area, color=color, *args, **kwargs)
+    ax.set_xlim(xmin, xmax, auto=True)
 
     if facecolor and facecolor not in [None, 'None', 'none']:
         if facecolor is True:
             facecolor = color
         c = iso_probability_contours(p[i], contours=levels)
         cmap = basic_cmap(facecolor)
         fill = []
@@ -378,14 +519,15 @@
 
     levels = kwargs.pop('levels', [0.68, 0.95])
 
     xmin = kwargs.pop('xmin', None)
     xmax = kwargs.pop('xmax', None)
     weights = kwargs.pop('weights', None)
     ncompress = kwargs.pop('ncompress', 1000)
+    density = kwargs.pop('density', False)
     cmap = kwargs.pop('cmap', None)
     color = kwargs.pop('color', (next(ax._get_lines.prop_cycler)['color']
                                  if cmap is None else cmap(0.68)))
     facecolor = kwargs.pop('facecolor', False)
 
     if 'edgecolor' in kwargs:
         edgecolor = kwargs.pop('edgecolor')
@@ -409,15 +551,16 @@
     if xmin is not None:
         i = i & (x > xmin)
     if xmax is not None:
         i = i & (x < xmax)
     sigma = np.sqrt(kde.covariance[0, 0])
     pp = cut_and_normalise_gaussian(x[i], p[i], sigma, xmin, xmax)
     pp /= pp.max()
-    ans = ax.plot(x[i], pp, color=color, *args, **kwargs)
+    area = np.trapz(x=x[i], y=pp) if density else 1
+    ans = ax.plot(x[i], pp/area, color=color, *args, **kwargs)
     ax.set_xlim(*check_bounds(x[i], xmin, xmax), auto=True)
 
     if facecolor and facecolor not in [None, 'None', 'none']:
         if facecolor is True:
             facecolor = color
         c = iso_probability_contours_from_samples(pp, contours=levels,
                                                   weights=w)
@@ -473,14 +616,15 @@
     plotter = kwargs.pop('plotter', '')
     weights = kwargs.pop('weights', None)
     if xmin is None or not np.isfinite(xmin):
         xmin = quantile(data, 0.01, weights)
     if xmax is None or not np.isfinite(xmax):
         xmax = quantile(data, 0.99, weights)
     histtype = kwargs.pop('histtype', 'bar')
+    density = kwargs.get('density', False)
     cmap = kwargs.pop('cmap', None)
     color = kwargs.pop('color', (next(ax._get_lines.prop_cycler)['color']
                                  if cmap is None else cmap(0.68)))
 
     if plotter == 'astropyhist':
         try:
             h, edges, bars = hist(data, ax=ax, color=color, range=(xmin, xmax),
@@ -488,23 +632,24 @@
         except NameError:
             raise ImportError("You need to install astropy to use astropyhist")
     else:
         h, edges, bars = ax.hist(data, color=color, range=(xmin, xmax),
                                  histtype=histtype, weights=weights,
                                  *args, **kwargs)
 
-    if histtype == 'bar':
+    if histtype == 'bar' and not density:
         for b in bars:
             b.set_height(b.get_height() / h.max())
-    elif histtype == 'step' or histtype == 'stepfilled':
+    elif (histtype == 'step' or histtype == 'stepfilled') and not density:
         trans = Affine2D().scale(sx=1, sy=1./h.max()) + ax.transData
         bars[0].set_transform(trans)
 
     ax.set_xlim(*check_bounds(edges, xmin, xmax), auto=True)
-    ax.set_ylim(0, 1.1)
+    if not density:
+        ax.set_ylim(0, 1.1)
     return bars
 
 
 def fastkde_contour_plot_2d(ax, data_x, data_y, *args, **kwargs):
     """Plot a 2d marginalised distribution as contours.
 
     This functions as a wrapper around matplotlib.axes.Axes.contour, and
@@ -545,24 +690,24 @@
     ymin = kwargs.pop('ymin', None)
     ymax = kwargs.pop('ymax', None)
     label = kwargs.pop('label', None)
     zorder = kwargs.pop('zorder', 1)
     levels = kwargs.pop('levels', [0.68, 0.95])
     color = kwargs.pop('color', next(ax._get_lines.prop_cycler)['color'])
     facecolor = kwargs.pop('facecolor', color)
-    edgecolor = kwargs.pop(
-        'edgecolor', color if facecolor in [None, 'None', 'none'] else 'k')
+    edgecolor = kwargs.pop('edgecolor', color)
     kwargs.pop('q', None)
 
     if len(data_x) == 0 or len(data_y) == 0:
         return np.zeros(0), np.zeros(0), np.zeros((0, 0))
 
     try:
-        x, y, pdf = fastkde_2d(data_x, data_y,
-                               xmin=xmin, xmax=xmax, ymin=ymin, ymax=ymax)
+        x, y, pdf, xmin, xmax, ymin, ymax = fastkde_2d(data_x, data_y,
+                                                       xmin=xmin, xmax=xmax,
+                                                       ymin=ymin, ymax=ymax)
     except NameError:
         raise ImportError("You need to install fastkde to use fastkde")
 
     levels = iso_probability_contours(pdf, contours=levels)
 
     i = (pdf >= levels[0]*0.5).any(axis=0)
     j = (pdf >= levels[0]*0.5).any(axis=1)
@@ -591,16 +736,16 @@
         edgecolor = edgecolor if cmap is None else None
 
     vmin, vmax = match_contour_to_contourf(levels, vmin=0, vmax=pdf.max())
     cont = ax.contour(x[i], y[j], pdf[np.ix_(j, i)], levels, zorder=zorder,
                       vmin=vmin, vmax=vmax, linewidths=linewidths,
                       colors=edgecolor, cmap=cmap, *args, **kwargs)
 
-    ax.set_xlim(*check_bounds(x[i], xmin, xmax), auto=True)
-    ax.set_ylim(*check_bounds(y[j], ymin, ymax), auto=True)
+    ax.set_xlim(xmin, xmax, auto=True)
+    ax.set_ylim(ymin, ymax, auto=True)
     return contf, cont
 
 
 def kde_contour_plot_2d(ax, data_x, data_y, *args, **kwargs):
     """Plot a 2d marginalised distribution as contours.
 
     This functions as a wrapper around matplotlib.axes.Axes.tricontour, and
@@ -645,16 +790,15 @@
     ymax = kwargs.pop('ymax', None)
     weights = kwargs.pop('weights', None)
     ncompress = kwargs.pop('ncompress', 1000)
     label = kwargs.pop('label', None)
     zorder = kwargs.pop('zorder', 1)
     color = kwargs.pop('color', next(ax._get_lines.prop_cycler)['color'])
     facecolor = kwargs.pop('facecolor', color)
-    edgecolor = kwargs.pop(
-        'edgecolor', color if facecolor in [None, 'None', 'none'] else 'k')
+    edgecolor = kwargs.pop('edgecolor', color)
     kwargs.pop('q', None)
 
     if len(data_x) == 0 or len(data_y) == 0:
         return np.zeros(0), np.zeros(0), np.zeros((0, 0))
 
     if weights is not None:
         data_x = data_x[weights != 0]
@@ -742,14 +886,15 @@
         A set of colors
 
     """
     xmin = kwargs.pop('xmin', None)
     xmax = kwargs.pop('xmax', None)
     ymin = kwargs.pop('ymin', None)
     ymax = kwargs.pop('ymax', None)
+    vmin = kwargs.pop('vmin', 0)
     label = kwargs.pop('label', None)
     levels = kwargs.pop('levels', None)
     color = kwargs.pop('color', next(ax._get_lines.prop_cycler)['color'])
     weights = kwargs.pop('weights', None)
 
     if xmin is None or not np.isfinite(xmin):
         xmin = quantile(data_x, 0.01, weights)
@@ -765,15 +910,15 @@
     if len(data_x) == 0 or len(data_y) == 0:
         return np.zeros(0), np.zeros(0), np.zeros((0, 0))
 
     cmap = kwargs.pop('cmap', basic_cmap(color))
 
     if levels is None:
         pdf, x, y, image = ax.hist2d(data_x, data_y, weights=weights,
-                                     cmap=cmap, range=rge,
+                                     cmap=cmap, range=rge, vmin=vmin,
                                      *args, **kwargs)
     else:
         bins = kwargs.pop('bins', 10)
         density = kwargs.pop('density', False)
         cmin = kwargs.pop('cmin', None)
         cmax = kwargs.pop('cmax', None)
         pdf, x, y = np.histogram2d(data_x, data_y, bins, rge,
@@ -782,15 +927,15 @@
         pdf = np.digitize(pdf, levels, right=True)
         pdf = np.array(levels)[pdf]
         pdf = np.ma.masked_array(pdf, pdf < levels[1])
         if cmin is not None:
             pdf[pdf < cmin] = np.ma.masked
         if cmax is not None:
             pdf[pdf > cmax] = np.ma.masked
-        image = ax.pcolormesh(x, y, pdf.T, cmap=cmap, vmin=0, vmax=pdf.max(),
+        image = ax.pcolormesh(x, y, pdf.T, cmap=cmap, vmin=vmin,
                               *args, **kwargs)
 
     ax.patches += [plt.Rectangle((0, 0), 0, 0, fc=cmap(0.999), ec=cmap(0.32),
                                  lw=2, label=label)]
 
     ax.set_xlim(*check_bounds(x, xmin, xmax), auto=True)
     ax.set_ylim(*check_bounds(y, ymin, ymax), auto=True)
```

### Comparing `anesthetic-2.0.0b7/anesthetic/read/getdistreader.py` & `anesthetic-2.0.0b9/anesthetic/read/getdistreader.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,26 +79,20 @@
 
     @property
     def paramnames_file(self):
         """File containing parameter names."""
         return self.root + '.paramnames'
 
     @property
-    def yaml_file(self):
-        """Cobaya parameter file."""
-        return self.root + '.updated.yaml'
-
-    @property
     def ranges_file(self):
         """File containing parameter names."""
         return self.root + '.ranges'
 
     @property
     def chains_files(self):
         """File containing parameter names."""
         files = glob.glob(self.root + '_[0-9].txt')
         if not files:
             files = glob.glob(self.root + '.[0-9].txt')
         if not files:
             files = [self.root + '.txt']
-
         return files
```

### Comparing `anesthetic-2.0.0b7/anesthetic/read/montepythonreader.py` & `anesthetic-2.0.0b9/anesthetic/read/montepythonreader.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/anesthetic/read/multinestreader.py` & `anesthetic-2.0.0b9/anesthetic/read/multinestreader.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/anesthetic/read/polychordreader.py` & `anesthetic-2.0.0b9/anesthetic/read/polychordreader.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/anesthetic/read/samplereader.py` & `anesthetic-2.0.0b9/anesthetic/read/samplereader.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Generic sampling reading tools."""
 import os
 from anesthetic.read.getdistreader import GetDistReader
+from anesthetic.read.cobayamcmcreader import CobayaMCMCReader
 from anesthetic.read.montepythonreader import MontePythonReader
 from anesthetic.read.polychordreader import PolyChordReader
 from anesthetic.read.multinestreader import MultiNestReader
 
 
 def SampleReader(root):
     """Read from a variety of sampling chains."""
@@ -13,19 +14,25 @@
         return mn
 
     pc = PolyChordReader(root)
     if os.path.isfile(pc.birth_file):
         return pc
 
     gd = GetDistReader(root)
-    if ((os.path.isfile(gd.paramnames_file) or os.path.isfile(gd.yaml_file))
+    if (os.path.isfile(gd.paramnames_file)
             and os.path.isfile(gd.chains_files[0])
             and os.path.isfile(gd.chains_files[-1])):
         return gd
 
+    cb = CobayaMCMCReader(root)
+    if (os.path.isfile(cb.yaml_file)
+            and os.path.isfile(cb.chains_files[0])
+            and os.path.isfile(cb.chains_files[-1])):
+        return cb
+
     mp = MontePythonReader(root)
     if (os.path.isfile(mp.log_param_file)
             and os.path.isfile(mp.log_file)
             and os.path.isfile(mp.paramnames_file)):
         mp._init()
         return mp
```

### Comparing `anesthetic-2.0.0b7/anesthetic/samples.py` & `anesthetic-2.0.0b9/anesthetic/samples.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 - ``MCMCSamples``
 - ``NestedSamples``
 """
 import os
 import numpy as np
 import pandas
 import copy
+import warnings
 from collections.abc import Sequence
 from anesthetic.plot import (make_1d_axes, make_2d_axes, fastkde_plot_1d,
                              kde_plot_1d, hist_plot_1d, scatter_plot_2d,
                              fastkde_contour_plot_2d,
                              kde_contour_plot_2d, hist_plot_2d)
 from anesthetic.read.samplereader import SampleReader
 from anesthetic.utils import (compute_nlive, compute_insertion_indexes,
@@ -154,14 +155,15 @@
         fig: matplotlib.figure.Figure
             New or original (if supplied) figure object
 
         axes: pandas.DataFrame or pandas.Series of matplotlib.axes.Axes
             Pandas array of axes objects
 
         """
+        self._set_automatic_limits()
         plot_type = kwargs.pop('plot_type', 'kde')
         do_1d_plot = paramname_y is None or paramname_x == paramname_y
         kwargs['label'] = kwargs.get('label', self.label)
         ncompress = kwargs.pop('ncompress', None)
 
         if do_1d_plot:
             if paramname_x in self and plot_type is not None:
@@ -614,28 +616,29 @@
         ----------
         logL: float or int, optional
             Loglikelihood or iteration number to return live points.
             If not provided, return the last set of active live points.
 
         Returns
         -------
-        live_points: NestedSamples
+        live_points: MCMCSamples
             Live points at either:
                 - contour logL (if input is float)
-                - ith contour (if input is integer)
-                - last generation contour if logL not provided
+                - ith iteration (if input is integer)
+                - last set of live points if no argument provided
         """
         if logL is None:
             logL = self.logL_birth.max()
         else:
             try:
                 logL = float(self.logL[logL])
             except KeyError:
                 pass
-        return self[(self.logL > logL) & (self.logL_birth <= logL)]
+        i = (self.logL >= logL) & (self.logL_birth < logL)
+        return MCMCSamples(self[i], weights=np.ones(i.sum()))
 
     def posterior_points(self, beta=1):
         """Get equally weighted posterior points at temperature beta."""
         return self.set_beta(beta).compress(-1)
 
     def prior_points(self, params=None):
         """Get equally weighted prior points."""
@@ -734,17 +737,28 @@
                 samples['logL_birth'] = logL_birth
                 samples.tex['logL_birth'] = r'$\log\mathcal{L}_{\rm birth}$'
 
             if 'logL_birth' not in samples:
                 raise RuntimeError("Cannot recompute run without "
                                    "birth contours logL_birth.")
 
-            if (samples.logL <= samples.logL_birth).any():
-                raise RuntimeError("Not a valid nested sampling run. "
-                                   "Require logL > logL_birth.")
+            invalid = samples.logL <= samples.logL_birth
+            n_bad = invalid.sum()
+            n_equal = (samples.logL == samples.logL_birth).sum()
+            if n_bad:
+                warnings.warn("%i out of %i samples have logL <= logL_birth,"
+                              "\n%i of which have logL == logL_birth."
+                              "\nThis may just indicate numerical rounding "
+                              "errors at the peak of the likelihood, but "
+                              "further investigation of the chains files is "
+                              "recommended."
+                              "\nDropping the invalid samples." %
+                              (n_bad, len(samples), n_equal),
+                              RuntimeWarning)
+                samples = samples[~invalid].reset_index()
 
             samples['nlive'] = compute_nlive(samples.logL, samples.logL_birth)
 
         samples.tex['nlive'] = r'$n_{\rm live}$'
         samples.beta = samples._beta
         return modify_inplace(self, samples, inplace)
```

### Comparing `anesthetic-2.0.0b7/anesthetic/utils.py` & `anesthetic-2.0.0b9/anesthetic/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,25 +64,25 @@
         W = w * nsamples / w.sum()
 
     fraction, integer = np.modf(W)
     extra = (u < fraction).astype(int)
     return (integer + extra).astype(int)
 
 
-def quantile(a, q, w=None):
+def quantile(a, q, w=None, interpolation='linear'):
     """Compute the weighted quantile for a one dimensional array."""
     if w is None:
         w = np.ones_like(a)
     a = np.array(list(a))  # Necessary to convert pandas arrays
     w = np.array(list(w))  # Necessary to convert pandas arrays
     i = np.argsort(a)
     c = np.cumsum(w[i[1:]]+w[i[:-1]])
     c /= c[-1]
     c = np.concatenate(([0.], c))
-    icdf = interp1d(c, a[i])
+    icdf = interp1d(c, a[i], kind=interpolation)
     quant = icdf(q)
     if isinstance(q, float):
         quant = float(quant)
     return quant
 
 
 def check_bounds(d, xmin=None, xmax=None):
```

### Comparing `anesthetic-2.0.0b7/anesthetic/weighted_pandas.py` & `anesthetic-2.0.0b9/anesthetic/weighted_pandas.py`

 * *Files 11% similar despite different names*

```diff
@@ -123,17 +123,19 @@
         return np.average(masked_array(abs(self-mean), null),
                           weights=self.weights)
 
     def sem(self, skipna=True):
         """Weighted standard error of the mean."""
         return np.sqrt(self.var(skipna=skipna)/self.neff())
 
-    def quantile(self, q=0.5):
+    def quantile(self, q=0.5, numeric_only=True, interpolation='linear'):
         """Weighted quantile of the sampled distribution."""
-        return quantile(self.values, q, self.weights)
+        if not numeric_only:
+            raise NotImplementedError("numeric_only kwarg not implemented")
+        return quantile(self.values, q, self.weights, interpolation)
 
     def compress(self, nsamples=None):
         """Reduce the number of samples by discarding low-weights.
 
         Parameters
         ----------
         neff: int, optional
@@ -262,24 +264,28 @@
             return super().var(axis=axis, skipna=skipna)
 
     def sem(self, axis=0, skipna=True):
         """Weighted standard error of the mean."""
         n = self.neff() if axis == 0 else self.shape[1]
         return np.sqrt(self.var(axis=axis, skipna=skipna)/n)
 
-    def quantile(self, q=0.5, axis=0):
+    def quantile(self, q=0.5, axis=0, numeric_only=True,
+                 interpolation='linear'):
         """Weighted quantile of the sampled distribution."""
+        if not numeric_only:
+            raise NotImplementedError("numeric_only kwarg not implemented")
         if axis == 0:
             data = np.array([c.quantile(q) for _, c in self.iteritems()])
             if np.isscalar(q):
                 return Series(data, index=self.columns)
             else:
                 return DataFrame(data.T, columns=self.columns, index=q)
         else:
-            return super().quantile(q=q, axis=axis)
+            return super().quantile(q=q, axis=axis, numeric_only=numeric_only,
+                                    interpolation=interpolation)
 
     def compress(self, nsamples=None):
         """Reduce the number of samples by discarding low-weights.
 
         Parameters
         ----------
         neff: int, optional
```

### Comparing `anesthetic-2.0.0b7/anesthetic.egg-info/PKG-INFO` & `anesthetic-2.0.0b9/anesthetic.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,232 +1,15 @@
 Metadata-Version: 2.1
 Name: anesthetic
-Version: 2.0.0b7
+Version: 2.0.0b9
 Summary: anesthetic: nested sampling visualisation
 Home-page: https://github.com/williamjameshandley/anesthetic
 Author: Will Handley
 Author-email: wh260@cam.ac.uk
 License: MIT
-Description: =========================================
-        anesthetic: nested sampling visualisation
-        =========================================
-        :anesthetic: nested sampling visualisation
-        :Author: Will Handley and Lukas Hergt
-        :Version: 2.0.0-beta.7
-        :Homepage: https://github.com/williamjameshandley/anesthetic
-        :Documentation: http://anesthetic.readthedocs.io/
-        
-        .. image:: https://travis-ci.com/williamjameshandley/anesthetic.svg?branch=master
-           :target: https://travis-ci.com/williamjameshandley/anesthetic
-           :alt: Build Status
-        .. image:: https://circleci.com/gh/williamjameshandley/anesthetic.svg?style=svg
-           :target: https://circleci.com/gh/williamjameshandley/anesthetic
-        .. image:: https://codecov.io/gh/williamjameshandley/anesthetic/branch/master/graph/badge.svg
-           :target: https://codecov.io/gh/williamjameshandley/anesthetic
-           :alt: Test Coverage Status
-        .. image:: https://readthedocs.org/projects/anesthetic/badge/?version=latest
-           :target: https://anesthetic.readthedocs.io/en/latest/?badge=latest
-           :alt: Documentation Status
-        .. image:: https://badge.fury.io/py/anesthetic.svg
-           :target: https://badge.fury.io/py/anesthetic
-           :alt: PyPi location
-        .. image:: https://zenodo.org/badge/175663535.svg
-           :target: https://zenodo.org/badge/latestdoi/175663535
-           :alt: Permanent DOI for this release
-        .. image:: http://joss.theoj.org/papers/8c51bffda75d122cf4a8b991e18d3e45/status.svg
-           :target: http://joss.theoj.org/papers/8c51bffda75d122cf4a8b991e18d3e45
-           :alt: Review Status
-        .. image:: https://img.shields.io/badge/license-MIT-blue.svg
-           :target: https://github.com/williamjameshandley/anesthetic/blob/master/LICENSE
-           :alt: License information
-        .. image:: https://mybinder.org/badge_logo.svg
-           :target: https://mybinder.org/v2/gh/williamjameshandley/anesthetic/1.0.0?filepath=demo.ipynb
-           :alt: Online interactive notebook
-        
-        
-        
-        
-        
-        ``anesthetic`` brings together tools for processing nested sampling chains, leveraging standard scientific python libraries.
-        
-        You can see example usage and plots in the `plot gallery <http://htmlpreview.github.io/?https://github.com/williamjameshandley/cosmo_example/blob/master/demos/demo.html>`_, or in the corresponding `Jupyter notebook <https://mybinder.org/v2/gh/williamjameshandley/anesthetic/master?filepath=demo.ipynb>`_.
-        
-        Current functionality includes:
-        
-        - Computation of Bayesian evidences, Kullback-Liebler divergences and Bayesian model dimensionalities.
-        - Marginalised 1d and 2d plots.
-        - Dynamic replaying of nested sampling.
-        
-        This tool was designed primarily for use with nested sampling outputs, although it can be used for normal MCMC chains.
-        
-        For an interactive view of a nested sampling run, you can use the ``anesthetic`` script.
-        
-        .. code:: bash
-        
-           $ anesthetic <ns file root>
-        
-        .. image:: https://github.com/williamjameshandley/anesthetic/raw/master/images/anim_1.gif
-        
-        Features
-        --------
-        
-        - Both samples and plotting axes are stored as a ``pandas.DataFrame``, with parameter names as indices, which makes for easy access and modification.
-        - Sensible color scheme for plotting nearly flat distributions.
-        - For easy extension/modification, uses the standard python libraries:
-          `numpy <https://www.numpy.org/>`__,
-          `scipy <https://www.scipy.org/>`__,
-          `matplotlib <https://matplotlib.org/>`__
-          and `pandas <https://pandas.pydata.org/>`__.
-        
-        Installation
-        ------------
-        
-        ``anesthetic`` can be installed via pip
-        
-        .. code:: bash
-        
-            pip install anesthetic
-        
-        or via the setup.py
-        
-        .. code:: bash
-        
-            git clone https://github.com/williamjameshandley/anesthetic
-            cd anesthetic
-            python setup.py install --user
-        
-        You can check that things are working by running the test suite:
-        
-        .. code:: bash
-        
-            export MPLBACKEND=Agg     # only necessary for OSX users
-            python -m pytest
-            flake8 anesthetic tests
-            pydocstyle --convention=numpy anesthetic
-        
-        
-        Dependencies
-        ~~~~~~~~~~~~
-        
-        Basic requirements:
-        
-        - Python 3.6+
-        - `matplotlib <https://pypi.org/project/matplotlib/>`__
-        - `numpy <https://pypi.org/project/numpy/>`__
-        - `scipy <https://pypi.org/project/scipy/>`__
-        - `pandas <https://pypi.org/project/pandas/>`__
-        - `fastKDE <https://pypi.org/project/fastkde/>`__
-        
-        Documentation:
-        
-        - `sphinx <https://pypi.org/project/Sphinx/>`__
-        - `numpydoc <https://pypi.org/project/numpydoc/>`__
-        
-        Tests:
-        
-        - `pytest <https://pypi.org/project/pytest/>`__
-        
-        Documentation
-        -------------
-        
-        Full Documentation is hosted at `ReadTheDocs <http://anesthetic.readthedocs.io/>`__.  To build your own local copy of the documentation you'll need to install `sphinx <https://pypi.org/project/Sphinx/>`__. You can then run:
-        
-        .. code:: bash
-        
-           cd docs
-           make html
-        
-        
-        Citation
-        --------
-        
-        If you use ``anesthetic`` to generate plots for a publication, please cite
-        as: ::
-        
-           Handley, (2019). anesthetic: nested sampling visualisation. Journal of Open
-           Source Software, 4(37), 1414, https://doi.org/10.21105/joss.01414
-        
-        or using the BibTeX:
-        
-        .. code:: bibtex
-        
-           @article{anesthetic,
-               doi = {10.21105/joss.01414},
-               url = {http://dx.doi.org/10.21105/joss.01414},
-               year  = {2019},
-               month = {Jun},
-               publisher = {The Open Journal},
-               volume = {4},
-               number = {37},
-               pages = {1414},
-               author = {Will Handley},
-               title = {anesthetic: nested sampling visualisation},
-               journal = {The Journal of Open Source Software}
-           }
-        
-        
-        Contributing
-        ------------
-        There are many ways you can contribute via the `GitHub repository <https://github.com/williamjameshandley/anesthetic>`__.
-        
-        - You can `open an issue <https://github.com/williamjameshandley/anesthetic/issues>`__ to report bugs or to propose new features.
-        - Pull requests are very welcome. Note that if you are going to propose major changes, be sure to open an issue for discussion first, to make sure that your PR will be accepted before you spend effort coding it.
-        
-        
-        Questions/Comments
-        ------------------
-        Another posterior plotting tool?
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-            This is my posterior plotter. There are many like it, but this one is mine.
-        
-        There are several excellent tools for plotting marginalised posteriors:
-        
-        - `getdist <http://getdist.readthedocs.io/en/latest/intro.html>`__
-        - `corner <https://corner.readthedocs.io>`__
-        - `pygtc <https://pygtc.readthedocs.io>`__
-        - `dynesty <https://dynesty.readthedocs.io>`__
-        - `MontePython <http://baudren.github.io/montepython.html>`__
-        
-        Why create another one? In general, any dedicated user of software will find that there is some functionality that in their use case is lacking, and the designs of previous codes make such extensions challenging. In my case this was:
-        
-        1. For large numbers of samples, kernel density estimation is slow, or inaccurate (particularly for samples generated from nested sampling). There are kernel density estimators, such as `fastKDE <https://pypi.org/project/fastkde/>`__, which ameliorate many of these difficulties.
-        
-        2. Existing tools can make it difficult to define new parameters. For example, the default cosmomc chain defines ``omegabh2``, but not ``omegab``. The transformation is easy, since ``omegab = omegabh2/ (H0/100)**2``, but implementing this transformation in existing packages is not so trivial. ``anesthetic`` solves this issue by storing the samples as a pandas array, for which the relevant code for defining the above new parameter would be
-        
-        .. code:: python
-        
-            from anesthetic import MCMCSamples
-            samples = MCMCSamples(root=file_root)                         # Load the samples
-            samples['omegab'] = samples.omegabh2/(samples.H0/100)**2      # Define omegab
-            samples.tex['omegab'] = '$\Omega_b$'                          # Label omegab
-            samples.plot_1d('omegab')                                     # Simple 1D plot
-        
-        3. Many KDE plotting tools have conventions that don't play well with uniformly distributed parameters, which presents a problem if you are trying to plot priors along with your posteriors. ``anesthetic`` has a sensible mechanism, by defining the contours by the amount of iso-probability mass they contain, but colouring the fill in relation to the probability density of the contour.
-        
-        What's in a name?
-        ~~~~~~~~~~~~~~~~~
-        
-        There is an emerging convention for naming nested sampling packages with words that have nest in them (`nestle and dynesty <https://dynesty.readthedocs.io/en/latest/>`__, `nestorflow <https://github.com/tomcharnock/NestorFlow>`__). Doing a UNIX grep:
-        
-        .. code:: bash
-        
-            grep nest /usr/share/dict/words
-        
-        yields a lot of superlatives (e.g. greenest), but a few other cool names for future projects:
-        
-        - amnesty
-        - defenestrate
-        - dishonestly
-        - inestimable
-        - minestrone
-        - rhinestone
-        
-        I chose ``anesthetic`` because I liked the soft 'th', and in spite of the US spelling.
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
@@ -237,7 +20,225 @@
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Provides-Extra: docs
 Provides-Extra: automated bins calculation
 Provides-Extra: fast kernel density estimation
+License-File: LICENSE
+
+=========================================
+anesthetic: nested sampling visualisation
+=========================================
+:anesthetic: nested sampling visualisation
+:Author: Will Handley and Lukas Hergt
+:Version: 2.0.0-beta.9
+:Homepage: https://github.com/williamjameshandley/anesthetic
+:Documentation: http://anesthetic.readthedocs.io/
+
+.. image:: https://github.com/williamjameshandley/anesthetic/workflows/CI/badge.svg?branch=master
+   :target: https://github.com/williamjameshandley/anesthetic/actions?query=workflow%3ACI+branch%3Amaster
+   :alt: Build Status
+.. image:: https://codecov.io/gh/williamjameshandley/anesthetic/branch/master/graph/badge.svg
+   :target: https://codecov.io/gh/williamjameshandley/anesthetic
+   :alt: Test Coverage Status
+.. image:: https://readthedocs.org/projects/anesthetic/badge/?version=latest
+   :target: https://anesthetic.readthedocs.io/en/latest/?badge=latest
+   :alt: Documentation Status
+.. image:: https://badge.fury.io/py/anesthetic.svg
+   :target: https://badge.fury.io/py/anesthetic
+   :alt: PyPi location
+.. image:: https://zenodo.org/badge/175663535.svg
+   :target: https://zenodo.org/badge/latestdoi/175663535
+   :alt: Permanent DOI for this release
+.. image:: http://joss.theoj.org/papers/8c51bffda75d122cf4a8b991e18d3e45/status.svg
+   :target: http://joss.theoj.org/papers/8c51bffda75d122cf4a8b991e18d3e45
+   :alt: Review Status
+.. image:: https://img.shields.io/badge/license-MIT-blue.svg
+   :target: https://github.com/williamjameshandley/anesthetic/blob/master/LICENSE
+   :alt: License information
+.. image:: https://mybinder.org/badge_logo.svg
+   :target: https://mybinder.org/v2/gh/williamjameshandley/anesthetic/1.0.0?filepath=demo.ipynb
+   :alt: Online interactive notebook
+
+
+
+
+
+``anesthetic`` brings together tools for processing nested sampling chains, leveraging standard scientific python libraries.
+
+You can see example usage and plots in the `plot gallery <http://htmlpreview.github.io/?https://github.com/williamjameshandley/cosmo_example/blob/master/demos/demo.html>`_, or in the corresponding `Jupyter notebook <https://mybinder.org/v2/gh/williamjameshandley/anesthetic/master?filepath=demo.ipynb>`_.
+
+Current functionality includes:
+
+- Computation of Bayesian evidences, Kullback-Liebler divergences and Bayesian model dimensionalities.
+- Marginalised 1d and 2d plots.
+- Dynamic replaying of nested sampling.
+
+This tool was designed primarily for use with nested sampling outputs, although it can be used for normal MCMC chains.
+
+For an interactive view of a nested sampling run, you can use the ``anesthetic`` script.
+
+.. code:: bash
+
+   $ anesthetic <ns file root>
+
+.. image:: https://github.com/williamjameshandley/anesthetic/raw/master/images/anim_1.gif
+
+Features
+--------
+
+- Both samples and plotting axes are stored as a ``pandas.DataFrame``, with parameter names as indices, which makes for easy access and modification.
+- Sensible color scheme for plotting nearly flat distributions.
+- For easy extension/modification, uses the standard python libraries:
+  `numpy <https://www.numpy.org/>`__,
+  `scipy <https://www.scipy.org/>`__,
+  `matplotlib <https://matplotlib.org/>`__
+  and `pandas <https://pandas.pydata.org/>`__.
+
+Installation
+------------
+
+``anesthetic`` can be installed via pip
+
+.. code:: bash
+
+    pip install anesthetic
+
+or via the setup.py
+
+.. code:: bash
+
+    git clone https://github.com/williamjameshandley/anesthetic
+    cd anesthetic
+    python setup.py install --user
+
+You can check that things are working by running the test suite:
+
+.. code:: bash
+
+    export MPLBACKEND=Agg     # only necessary for OSX users
+    python -m pytest
+    flake8 anesthetic tests
+    pydocstyle --convention=numpy anesthetic
+
+
+Dependencies
+~~~~~~~~~~~~
+
+Basic requirements:
+
+- Python 3.6+
+- `matplotlib <https://pypi.org/project/matplotlib/>`__
+- `numpy <https://pypi.org/project/numpy/>`__
+- `scipy <https://pypi.org/project/scipy/>`__
+- `pandas <https://pypi.org/project/pandas/>`__
+- `fastKDE <https://pypi.org/project/fastkde/>`__
+
+Documentation:
+
+- `sphinx <https://pypi.org/project/Sphinx/>`__
+- `numpydoc <https://pypi.org/project/numpydoc/>`__
+
+Tests:
+
+- `pytest <https://pypi.org/project/pytest/>`__
+
+Documentation
+-------------
+
+Full Documentation is hosted at `ReadTheDocs <http://anesthetic.readthedocs.io/>`__.  To build your own local copy of the documentation you'll need to install `sphinx <https://pypi.org/project/Sphinx/>`__. You can then run:
+
+.. code:: bash
+
+   cd docs
+   make html
+
+
+Citation
+--------
+
+If you use ``anesthetic`` to generate plots for a publication, please cite
+as: ::
+
+   Handley, (2019). anesthetic: nested sampling visualisation. Journal of Open
+   Source Software, 4(37), 1414, https://doi.org/10.21105/joss.01414
+
+or using the BibTeX:
+
+.. code:: bibtex
+
+   @article{anesthetic,
+       doi = {10.21105/joss.01414},
+       url = {http://dx.doi.org/10.21105/joss.01414},
+       year  = {2019},
+       month = {Jun},
+       publisher = {The Open Journal},
+       volume = {4},
+       number = {37},
+       pages = {1414},
+       author = {Will Handley},
+       title = {anesthetic: nested sampling visualisation},
+       journal = {The Journal of Open Source Software}
+   }
+
+
+Contributing
+------------
+There are many ways you can contribute via the `GitHub repository <https://github.com/williamjameshandley/anesthetic>`__.
+
+- You can `open an issue <https://github.com/williamjameshandley/anesthetic/issues>`__ to report bugs or to propose new features.
+- Pull requests are very welcome. Note that if you are going to propose major changes, be sure to open an issue for discussion first, to make sure that your PR will be accepted before you spend effort coding it.
+
+
+Questions/Comments
+------------------
+Another posterior plotting tool?
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+    This is my posterior plotter. There are many like it, but this one is mine.
+
+There are several excellent tools for plotting marginalised posteriors:
+
+- `getdist <http://getdist.readthedocs.io/en/latest/intro.html>`__
+- `corner <https://corner.readthedocs.io>`__
+- `pygtc <https://pygtc.readthedocs.io>`__
+- `dynesty <https://dynesty.readthedocs.io>`__
+- `MontePython <http://baudren.github.io/montepython.html>`__
+
+Why create another one? In general, any dedicated user of software will find that there is some functionality that in their use case is lacking, and the designs of previous codes make such extensions challenging. In my case this was:
+
+1. For large numbers of samples, kernel density estimation is slow, or inaccurate (particularly for samples generated from nested sampling). There are kernel density estimators, such as `fastKDE <https://pypi.org/project/fastkde/>`__, which ameliorate many of these difficulties.
+
+2. Existing tools can make it difficult to define new parameters. For example, the default cosmomc chain defines ``omegabh2``, but not ``omegab``. The transformation is easy, since ``omegab = omegabh2/ (H0/100)**2``, but implementing this transformation in existing packages is not so trivial. ``anesthetic`` solves this issue by storing the samples as a pandas array, for which the relevant code for defining the above new parameter would be
+
+.. code:: python
+
+    from anesthetic import MCMCSamples
+    samples = MCMCSamples(root=file_root)                         # Load the samples
+    samples['omegab'] = samples.omegabh2/(samples.H0/100)**2      # Define omegab
+    samples.tex['omegab'] = '$\Omega_b$'                          # Label omegab
+    samples.plot_1d('omegab')                                     # Simple 1D plot
+
+3. Many KDE plotting tools have conventions that don't play well with uniformly distributed parameters, which presents a problem if you are trying to plot priors along with your posteriors. ``anesthetic`` has a sensible mechanism, by defining the contours by the amount of iso-probability mass they contain, but colouring the fill in relation to the probability density of the contour.
+
+What's in a name?
+~~~~~~~~~~~~~~~~~
+
+There is an emerging convention for naming nested sampling packages with words that have nest in them (`nestle and dynesty <https://dynesty.readthedocs.io/en/latest/>`__, `nestorflow <https://github.com/tomcharnock/NestorFlow>`__). Doing a UNIX grep:
+
+.. code:: bash
+
+    grep nest /usr/share/dict/words
+
+yields a lot of superlatives (e.g. greenest), but a few other cool names for future projects:
+
+- amnesty
+- defenestrate
+- dishonestly
+- inestimable
+- minestrone
+- rhinestone
+
+I chose ``anesthetic`` because I liked the soft 'th', and in spite of the US spelling.
+
+
```

### Comparing `anesthetic-2.0.0b7/anesthetic.egg-info/SOURCES.txt` & `anesthetic-2.0.0b9/anesthetic.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 anesthetic.egg-info/requires.txt
 anesthetic.egg-info/top_level.txt
 anesthetic/gui/__init__.py
 anesthetic/gui/plot.py
 anesthetic/gui/widgets.py
 anesthetic/read/__init__.py
 anesthetic/read/chainreader.py
+anesthetic/read/cobayamcmcreader.py
 anesthetic/read/getdistreader.py
 anesthetic/read/montepythonreader.py
 anesthetic/read/multinestreader.py
 anesthetic/read/polychordreader.py
 anesthetic/read/samplereader.py
 bin/gen_data.py
 bin/plot.py
@@ -61,14 +62,18 @@
 tests/test_convert.py
 tests/test_gui.py
 tests/test_plot.py
 tests/test_samples.py
 tests/test_utils.py
 tests/test_weighted_pandas.py
 tests/wedding_cake.py
+tests/example_data/cb.1.txt
+tests/example_data/cb.2.txt
+tests/example_data/cb.input.yaml
+tests/example_data/cb.updated.yaml
 tests/example_data/gd.paramnames
 tests/example_data/gd.ranges
 tests/example_data/gd_1.txt
 tests/example_data/gd_2.txt
 tests/example_data/gd_single.paramnames
 tests/example_data/gd_single.ranges
 tests/example_data/gd_single.txt
```

### Comparing `anesthetic-2.0.0b7/bin/gen_data.py` & `anesthetic-2.0.0b9/bin/gen_data.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/bin/plot.py` & `anesthetic-2.0.0b9/bin/plot.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/demo.ipynb` & `anesthetic-2.0.0b9/demo.ipynb`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/demo.py` & `anesthetic-2.0.0b9/demo.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/docs/Makefile` & `anesthetic-2.0.0b9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/docs/make.bat` & `anesthetic-2.0.0b9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/docs/source/anesthetic.read.rst` & `anesthetic-2.0.0b9/docs/source/anesthetic.read.rst`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/docs/source/anesthetic.rst` & `anesthetic-2.0.0b9/docs/source/anesthetic.rst`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/docs/source/conf.py` & `anesthetic-2.0.0b9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/images/anim_1.gif` & `anesthetic-2.0.0b9/images/anim_1.gif`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/images/animate.py` & `anesthetic-2.0.0b9/images/animate.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/paper/2d.png` & `anesthetic-2.0.0b9/paper/2d.png`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/paper/Makefile` & `anesthetic-2.0.0b9/paper/Makefile`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/paper/paper.bib` & `anesthetic-2.0.0b9/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/paper/paper.md` & `anesthetic-2.0.0b9/paper/paper.md`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/scripts/anesthetic` & `anesthetic-2.0.0b9/scripts/anesthetic`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/setup.py` & `anesthetic-2.0.0b9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
       install_requires=open('requirements.txt').read().splitlines(),
       setup_requires=['pytest-runner'],
       extras_require={
           'docs': ['sphinx', 'sphinx_rtd_theme', 'numpydoc'],
           'automated bins calculation': ['astropy'],
           'fast kernel density estimation': ['fastkde'],
           },
-      tests_require=['pytest'],
+      tests_require=['pytest', 'packaging'],
       include_package_data=True,
       license='MIT',
       classifiers=[
                    'Development Status :: 5 - Production/Stable',
                    'Intended Audience :: Developers',
                    'Intended Audience :: Science/Research',
                    'Natural Language :: English',
```

### Comparing `anesthetic-2.0.0b7/tests/example_data/gd_1.txt` & `anesthetic-2.0.0b9/tests/example_data/gd_1.txt`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/tests/example_data/gd_2.txt` & `anesthetic-2.0.0b9/tests/example_data/gd_2.txt`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/tests/example_data/gd_single.txt` & `anesthetic-2.0.0b9/tests/example_data/gd_single.txt`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/tests/example_data/mn_oldev.dat` & `anesthetic-2.0.0b9/tests/example_data/mn_oldev.dat`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/tests/example_data/mn_oldphys_live.points` & `anesthetic-2.0.0b9/tests/example_data/mn_oldphys_live.points`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/tests/example_data/mndead-birth.txt` & `anesthetic-2.0.0b9/tests/example_data/mndead-birth.txt`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/tests/example_data/mnev.dat` & `anesthetic-2.0.0b9/tests/example_data/mnev.dat`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/tests/example_data/mnphys_live-birth.txt` & `anesthetic-2.0.0b9/tests/example_data/mnphys_live-birth.txt`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/tests/example_data/mnphys_live.points` & `anesthetic-2.0.0b9/tests/example_data/mnphys_live.points`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/tests/example_data/mp/2019-01-24_200000_.paramnames` & `anesthetic-2.0.0b9/tests/example_data/mp/2019-01-24_200000_.paramnames`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/tests/example_data/mp/2019-01-24_200000__1.txt` & `anesthetic-2.0.0b9/tests/example_data/mp/2019-01-24_200000__1.txt`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/tests/example_data/mp/2019-01-24_200000__2.txt` & `anesthetic-2.0.0b9/tests/example_data/mp/2019-01-24_200000__2.txt`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/tests/example_data/mp/log.param` & `anesthetic-2.0.0b9/tests/example_data/mp/log.param`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/tests/example_data/mp/mp.bestfit` & `anesthetic-2.0.0b9/tests/example_data/mp/mp.bestfit`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/tests/example_data/mp/mp.covmat` & `anesthetic-2.0.0b9/tests/example_data/mp/mp.covmat`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/tests/example_data/mp/mp.h_info` & `anesthetic-2.0.0b9/tests/example_data/mp/mp.h_info`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/tests/example_data/mp/mp.tex` & `anesthetic-2.0.0b9/tests/example_data/mp/mp.tex`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/tests/example_data/mp/mp.v_info` & `anesthetic-2.0.0b9/tests/example_data/mp/mp.v_info`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/tests/example_data/pc_250_dead-birth.txt` & `anesthetic-2.0.0b9/tests/example_data/pc_250_dead-birth.txt`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/tests/example_data/pc_250_phys_live-birth.txt` & `anesthetic-2.0.0b9/tests/example_data/pc_250_phys_live-birth.txt`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/tests/example_data/pc_dead-birth.txt` & `anesthetic-2.0.0b9/tests/example_data/pc_dead-birth.txt`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/tests/example_data/pc_phys_live-birth.txt` & `anesthetic-2.0.0b9/tests/example_data/pc_phys_live-birth.txt`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/tests/test_convert.py` & `anesthetic-2.0.0b9/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/tests/test_gui.py` & `anesthetic-2.0.0b9/tests/test_gui.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import matplotlib_agg  # noqa: F401
+from packaging import version
+from matplotlib import __version__ as mpl_version
 from anesthetic import NestedSamples
 
 
 def test_gui():
     plotter = NestedSamples(root='./tests/example_data/pc').gui()
 
     # Type buttons
@@ -30,12 +32,19 @@
     assert(plotter.temperature() == 1)
     plotter.temperature.slider.set_val(1)
     assert(plotter.temperature() == 10)
     plotter.temperature.slider.set_val(2)
     assert(plotter.temperature() == 100)
     plotter.type.buttons.set_active(0)
 
-    # Reload button
-    plotter.reload.button.observers[0](None)
+    if version.parse(mpl_version) >= version.parse('3.4.0'):
+        # Reload button
+        plotter.reload.button.observers[0]()
+
+        # Reset button
+        plotter.reset.button.observers[0]()
+    else:
+        # Reload button
+        plotter.reload.button.observers[0](None)
 
-    # Reset button
-    plotter.reset.button.observers[0](None)
+        # Reset button
+        plotter.reset.button.observers[0](None)
```

### Comparing `anesthetic-2.0.0b7/tests/test_plot.py` & `anesthetic-2.0.0b9/tests/test_plot.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 from matplotlib.tri import TriContourSet
 from matplotlib.lines import Line2D
 from matplotlib.patches import Patch, Polygon
 from matplotlib.colors import ColorConverter, to_rgba
 from matplotlib.figure import Figure
 from pandas.core.series import Series
 from pandas.core.frame import DataFrame
+from scipy.special import erf
+from scipy.interpolate import interp1d
 
 
 def test_make_1d_axes():
     paramnames = ['A', 'B', 'C', 'D', 'E']
     tex = {'A': 'tA', 'B': 'tB', 'C': 'tC', 'D': 'tD', 'E': 'tE'}
 
     # Check no optional arguments
@@ -166,14 +168,41 @@
                     ns = calc_n(axes)
                     assert(ns['upper'] == upper * nu)
                     assert(ns['lower'] == lower * nl)
                     assert(ns['diagonal'] == diagonal * nd)
         plt.close("all")
 
 
+@pytest.mark.parametrize('upper', [False, True])
+@pytest.mark.parametrize('ticks', ['inner', 'outer', None])
+def test_make_2d_axes_ticks(upper, ticks):
+    xticks = [0.1, 0.4, 0.7]
+    yticks = [0.2, 0.5, 0.8]
+    paramnames = ["x0", "x1", "x2", "x3"]
+    for k in paramnames:
+        fig, axes = make_2d_axes(paramnames, upper=upper, ticks=ticks)
+        axes[k][k].set_xticks(xticks)
+        axes[k][k].set_yticks(yticks)
+        for i, row in axes.iterrows():
+            for j, ax in row.iteritems():
+                if ax is None:
+                    break
+                if i == k:
+                    assert np.array_equal(yticks, ax.get_yticks())
+                else:
+                    assert not np.array_equal(yticks, ax.get_yticks())
+                if j == k:
+                    assert np.array_equal(xticks, ax.get_xticks())
+                else:
+                    assert not np.array_equal(xticks, ax.get_xticks())
+        plt.close("all")
+    with pytest.raises(ValueError):
+        make_2d_axes(paramnames, upper=upper, ticks='spam')
+
+
 def test_2d_axes_limits():
     np.random.seed(0)
     paramnames = ['A', 'B', 'C', 'D']
     fig, axes = make_2d_axes(paramnames)
     for x in paramnames:
         for y in paramnames:
             a, b, c, d = np.random.rand(4)
@@ -184,14 +213,45 @@
 
             axes[x][y].set_ylim(c, d)
             for z in paramnames:
                 assert(axes[y][z].get_xlim() == (c, d))
                 assert(axes[z][y].get_ylim() == (c, d))
 
 
+@pytest.mark.parametrize('axesparams', [['A', 'B', 'C', 'D'],
+                                        [['A', 'B', 'C', 'D'], ['A', 'B']],
+                                        [['A', 'B'], ['A', 'B', 'C', 'D']]])
+@pytest.mark.parametrize('params, values', [('A', 0),
+                                            (['A', 'C', 'E'], [0, 0, 0]),
+                                            (['A', 'C', 'C'], [0, 0, 0.5])])
+def test_2d_axlines_axspans(axesparams, params, values):
+    values = np.array(values)
+    line_kwargs = dict(c='k', ls='--', lw=0.5)
+    span_kwargs = dict(c='k', alpha=0.5)
+    fig, axes = make_2d_axes(axesparams)
+    axes.axlines(params, values, **line_kwargs)
+    axes.axspans(params, values-0.1, values+0.1, **span_kwargs)
+    plt.close("all")
+
+
+@pytest.mark.parametrize('params, values', [('A', [0, 0]),
+                                            (['A', 'C'], 0),
+                                            (['A', 'C'], [0, 0, 0.5]),
+                                            (['A', 'C', 'C'], [0, 0])])
+def test_2d_axlines_axspans_error(params, values):
+    values = np.array(values)
+    axesparams = ['A', 'B', 'C', 'D']
+    fig, axes = make_2d_axes(axesparams)
+    with pytest.raises(ValueError):
+        axes.axlines(params, values)
+    with pytest.raises(ValueError):
+        axes.axspans(params, values-0.1, values+0.1)
+    plt.close("all")
+
+
 @pytest.mark.parametrize('plot_1d', [kde_plot_1d, fastkde_plot_1d])
 def test_kde_plot_1d(plot_1d):
     fig, ax = plt.subplots()
     np.random.seed(0)
     data = np.random.randn(1000)
 
     try:
@@ -235,14 +295,32 @@
         plot_1d(ax, data, facecolor=True, levels=[0.2, 0.6, 0.8])
         line, fill = plot_1d(ax, data, fc='blue', color='k', ec='r')
         assert(np.all(fill[0].get_edgecolor()[0] == to_rgba('r')))
         assert (to_rgba(line[0].get_color()) == to_rgba('r'))
         line, fill = plot_1d(ax, data, fc=True, color='k', ec=None)
         assert(len(fill[0].get_edgecolor()) == 0)
         assert (to_rgba(line[0].get_color()) == to_rgba('k'))
+        plt.close("all")
+
+        # Check xlim, Gaussian (i.e. limits reduced to relevant data range)
+        fig, ax = plt.subplots()
+        data = np.random.randn(1000) * 0.01 + 0.5
+        plot_1d(ax, data, xmin=0, xmax=1)
+        xmin, xmax = ax.get_xlim()
+        assert(xmin > 0.4)
+        assert(xmax < 0.6)
+        plt.close("all")
+        # Check xlim, Uniform (i.e. data and limits span entire prior boundary)
+        fig, ax = plt.subplots()
+        data = np.random.uniform(size=1000)
+        plot_1d(ax, data, xmin=0, xmax=1)
+        xmin, xmax = ax.get_xlim()
+        assert(xmin == 0)
+        assert(xmax == 1)
+        plt.close("all")
 
     except ImportError:
         if 'fastkde' not in sys.modules:
             pass
 
 
 def test_hist_plot_1d():
@@ -340,14 +418,52 @@
     weights = np.exp(-(data_x**2 + data_y**2)/2)
     hist_plot_2d(ax, data_x, data_y, weights=weights, bins=30)
     xmin, xmax = ax.get_xlim()
     ymin, ymax = ax.get_ylim()
     assert xmin > -3 and xmax < 3 and ymin > -3 and ymax < 3
 
 
+@pytest.mark.parametrize('plot_1d', [kde_plot_1d, fastkde_plot_1d])
+@pytest.mark.parametrize('s', [1, 2])
+def test_1d_density_kwarg(plot_1d, s):
+    try:
+        np.random.seed(0)
+        x = np.random.normal(scale=s, size=2000)
+        fig, ax = plt.subplots()
+
+        # hist density = False:
+        h = hist_plot_1d(ax, x, density=False, bins=np.linspace(-5.5, 5.5, 12))
+        bar_height = h.get_children()[len(h.get_children()) // 2].get_height()
+        assert(bar_height == pytest.approx(1, rel=0.1))
+
+        # kde density = False:
+        k = plot_1d(ax, x, density=False)[0]
+        f = interp1d(k.get_xdata(), k.get_ydata(), 'cubic', assume_sorted=True)
+        kde_height = f(0)
+        assert(kde_height == pytest.approx(1, rel=0.1))
+
+        # hist density = True:
+        h = hist_plot_1d(ax, x, density=True, bins=np.linspace(-5.5, 5.5, 12))
+        bar_height = h.get_children()[len(h.get_children()) // 2].get_height()
+        assert(bar_height == pytest.approx(erf(0.5 / np.sqrt(2) / s), rel=0.1))
+
+        # kde density = True:
+        k = plot_1d(ax, x, density=True)[0]
+        f = interp1d(k.get_xdata(), k.get_ydata(), 'cubic', assume_sorted=True)
+        kde_height = f(0)
+        gauss_norm = 1 / np.sqrt(2 * np.pi * s**2)
+        assert(kde_height == pytest.approx(gauss_norm, rel=0.1))
+
+        plt.close("all")
+
+    except ImportError:
+        if 'fastkde' not in sys.modules:
+            pass
+
+
 @pytest.mark.parametrize('contour_plot_2d', [kde_contour_plot_2d,
                                              fastkde_contour_plot_2d])
 def test_contour_plot_2d(contour_plot_2d):
     try:
         ax = plt.gca()
         np.random.seed(1)
         data_x = np.random.randn(1000)
@@ -421,15 +537,40 @@
         cf, ct = contour_plot_2d(ax, data_x, data_y, fc=None, ec='C1')
         assert cf is None
         assert ct.colors == 'C1'
         cf, ct = contour_plot_2d(ax, data_x, data_y, fc=None, cmap=plt.cm.Reds)
         assert cf is None
         assert ct.get_cmap() == plt.cm.Reds
         assert ct.colors is None
-        plt.close()
+        plt.close("all")
+
+        # Check limits, Gaussian (i.e. limits reduced to relevant data range)
+        fig, ax = plt.subplots()
+        data_x = np.random.randn(1000) * 0.01 + 0.5
+        data_y = np.random.randn(1000) * 0.01 + 0.5
+        contour_plot_2d(ax, data_x, data_y, xmin=0, xmax=1, ymin=0, ymax=1)
+        xmin, xmax = ax.get_xlim()
+        ymin, ymax = ax.get_ylim()
+        assert(xmin > 0.4)
+        assert(xmax < 0.6)
+        assert(ymin > 0.4)
+        assert(ymax < 0.6)
+        plt.close("all")
+        # Check limits, Uniform (i.e. data & limits span entire prior boundary)
+        fig, ax = plt.subplots()
+        data_x = np.random.uniform(size=1000)
+        data_y = np.random.uniform(size=1000)
+        contour_plot_2d(ax, data_x, data_y, xmin=0, xmax=1, ymin=0, ymax=1)
+        xmin, xmax = ax.get_xlim()
+        ymin, ymax = ax.get_ylim()
+        assert(xmin == 0)
+        assert(xmax == 1)
+        assert(ymin == 0)
+        assert(ymax == 1)
+        plt.close("all")
 
     except ImportError:
         if 'fastkde' not in sys.modules:
             pass
 
 
 def test_scatter_plot_2d():
```

### Comparing `anesthetic-2.0.0b7/tests/test_samples.py` & `anesthetic-2.0.0b9/tests/test_samples.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,29 +96,46 @@
 
     mcmc = MCMCSamples(root='./tests/example_data/gd_single')
     mcmc.plot_2d(['x0', 'x1', 'x2', 'x3'])
     mcmc.plot_1d(['x0', 'x1', 'x2', 'x3'])
     plt.close("all")
 
 
-def test_read_getdist_discard_burn_in():
+@pytest.mark.xfail('getdist' not in sys.modules,
+                   raises=NameError,
+                   reason="requires getdist package")
+@pytest.mark.parametrize('root', ['gd', 'cb'])
+def test_read_discard_burn_in(root):
     np.random.seed(3)
-    mcmc = MCMCSamples(burn_in=0.3, root='./tests/example_data/gd')
+    mcmc = MCMCSamples(burn_in=0.3, root='./tests/example_data/' + root)
     mcmc.plot_2d(['x0', 'x1', 'x2', 'x3'])
     mcmc.plot_1d(['x0', 'x1', 'x2', 'x3'])
 
-    # for 2 getdist chains of length 5000
-    mcmc0 = MCMCSamples(root='./tests/example_data/gd')
-    mcmc1 = MCMCSamples(burn_in=1000, root='./tests/example_data/gd')
+    # for 2 chains of length 5000
+    mcmc0 = MCMCSamples(root='./tests/example_data/' + root)
+    mcmc1 = MCMCSamples(burn_in=1000, root='./tests/example_data/' + root)
     for key in ['x0', 'x1', 'x2', 'x3', 'x4']:
-        assert_array_equal(mcmc0[key][1000:5000], mcmc1[key][:4000])
+        if key in mcmc0:
+            assert key in mcmc1
+            assert_array_equal(mcmc0[key][1000:2000], mcmc1[key][:1000])
     mcmc1.plot_2d(['x0', 'x1', 'x2', 'x3', 'x4'])
     mcmc1.plot_1d(['x0', 'x1', 'x2', 'x3', 'x4'])
 
 
+@pytest.mark.xfail('getdist' not in sys.modules,
+                   raises=NameError,
+                   reason="requires getdist package")
+def test_read_cobayamcmc():
+    np.random.seed(3)
+    mcmc = MCMCSamples(root='./tests/example_data/cb')
+    mcmc.plot_2d(['x0', 'x1'])
+    mcmc.plot_1d(['x0', 'x1'])
+    plt.close("all")
+
+
 @pytest.mark.xfail('montepython' not in sys.modules,
                    raises=ImportError,
                    reason="requires montepython package")
 def test_read_montepython():
     np.random.seed(3)
     mcmc = MCMCSamples(root='./tests/example_data/mp')
     mcmc.plot_2d(['x0', 'x1', 'x2', 'x3'])
@@ -592,27 +609,29 @@
     assert_frame_equal(prior, ns.set_beta(0))
 
 
 def test_live_points():
     np.random.seed(4)
     pc = NestedSamples(root="./tests/example_data/pc")
 
-    for i, logL in pc.logL.iloc[:-1].iteritems():
+    for i, logL in pc.logL.iloc[::49].iteritems():
         live_points = pc.live_points(logL)
-        assert len(live_points) == int(pc.nlive[i[0]+1])
+        assert len(live_points) == int(pc.nlive[i[0]])
 
         live_points_from_int = pc.live_points(i[0])
         assert_array_equal(live_points_from_int, live_points)
 
         live_points_from_index = pc.live_points(i)
         assert_array_equal(live_points_from_index, live_points)
 
+    assert pc.live_points(0).index[0][0] == 0
+
     last_live_points = pc.live_points()
     logL = pc.logL_birth.max()
-    assert (last_live_points.logL > logL).all()
+    assert (last_live_points.logL >= logL).all()
     assert len(last_live_points) == pc.nlive.mode()[0]
 
 
 def test_limit_assignment():
     np.random.seed(3)
     ns = NestedSamples(root='./tests/example_data/pc')
     # `None` in .ranges file:
@@ -628,14 +647,23 @@
     assert ns.limits['x3'][0] == 0
     assert ns.limits['x3'][1] == 1
     # limits for logL, weights, nlive
     assert ns.limits['logL'][0] == -777.0115456428716
     assert ns.limits['logL'][1] == 5.748335384373301
     assert ns.limits['nlive'][0] == 1
     assert ns.limits['nlive'][1] == 125
+    # limits for derived parameters:
+    ns['x5'] = ns.x0 + ns.x1
+    assert 'x5' in ns.columns and 'x5' not in ns.limits
+    ns.plot_1d(['x5'])
+    assert 'x5' in ns.columns and 'x5' in ns.limits
+    ns['x6'] = ns.x2 + ns.x3
+    assert 'x6' in ns.columns and 'x6' not in ns.limits
+    ns.plot_2d(['x5', 'x6'])
+    assert 'x6' in ns.columns and 'x6' in ns.limits
 
 
 def test_xmin_xmax_1d():
     """Test to provide a solution to #89"""
     np.random.seed(3)
     ns = NestedSamples(root='./tests/example_data/pc')
     fig, ax = ns.plot_1d('x0', plot_type='hist')
@@ -865,16 +893,17 @@
 def test_recompute():
     np.random.seed(3)
     pc = NestedSamples(root='./tests/example_data/pc')
     recompute = pc.recompute()
     assert recompute is not pc
 
     pc.loc[1000, 'logL'] = pc.logL_birth.iloc[1000]-1
-    with pytest.raises(RuntimeError):
-        pc.recompute()
+    with pytest.warns(RuntimeWarning):
+        recompute = pc.recompute()
+    assert len(recompute) == len(pc) - 1
 
     mn = NestedSamples(root='./tests/example_data/mn_old')
     with pytest.raises(RuntimeError):
         mn.recompute()
 
 
 def test_copy():
```

### Comparing `anesthetic-2.0.0b7/tests/test_utils.py` & `anesthetic-2.0.0b9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.0.0b7/tests/test_weighted_pandas.py` & `anesthetic-2.0.0b9/tests/test_weighted_pandas.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,14 +199,17 @@
         quantile = df.quantile(q, axis=1)
         assert isinstance(quantile, WeightedSeries)
 
     assert_allclose(df.quantile(qs), np.transpose([qs, qs, qs]), atol=1e-2)
     quantile = df.quantile(qs, axis=1)
     assert isinstance(quantile, WeightedDataFrame)
 
+    with pytest.raises(NotImplementedError):
+        df.quantile(numeric_only=False)
+
 
 def test_WeightedDataFrame_hist():
     plt.figure()
     df = test_WeightedDataFrame_constructor()
     axes = df[['A', 'B']].hist(bins=20, density=True)
     for ax in axes.flatten():
         assert len(ax.patches) == 20
@@ -401,14 +404,17 @@
     for q in qs:
         quantile = series.quantile(q)
         assert isinstance(quantile, float)
         assert_allclose(quantile, q, atol=1e-2)
 
     assert_allclose(series.quantile(qs), qs, atol=1e-2)
 
+    with pytest.raises(NotImplementedError):
+        series.quantile(numeric_only=False)
+
 
 def test_WeightedSeries_hist():
     plt.figure()
     series = test_WeightedSeries_constructor()
     ax = series.hist(bins=20, density=True)
     assert len(ax.patches) == 20
     norm = 0
```

### Comparing `anesthetic-2.0.0b7/tests/wedding_cake.py` & `anesthetic-2.0.0b9/tests/wedding_cake.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,16 @@
             x_ = np.random.uniform(0.5-r_, 0.5+r_, size=(j.sum(), self.D))
             live_birth_likes[j] = logL_
             live_points[j] = x_
             live_likes[j] = self.logL(x_)
 
             samps = NestedSamples(points, logL=death_likes,
                                   logL_birth=birth_likes)
-            if samps.live_points().weights.sum()/samps.weights.sum() < 0.001:
+
+            if samps.iloc[-nlive:].weights.sum()/samps.weights.sum() < 0.001:
                 break
 
         death_likes = np.concatenate([death_likes, live_likes])
         birth_likes = np.concatenate([birth_likes, live_birth_likes])
         points = np.concatenate([points, live_points])
 
         return NestedSamples(points, logL=death_likes, logL_birth=birth_likes)
```

