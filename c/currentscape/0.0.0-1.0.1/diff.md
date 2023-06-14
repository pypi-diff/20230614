# Comparing `tmp/currentscape-0.0.0.tar.gz` & `tmp/currentscape-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "currentscape-0.0.0.tar", last modified: Wed Jun 14 12:11:10 2023, max compression
+gzip compressed data, was "currentscape-1.0.1.tar", last modified: Wed Jun 14 15:26:21 2023, max compression
```

## Comparing `currentscape-0.0.0.tar` & `currentscape-1.0.1.tar`

### file list

```diff
@@ -1,40 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:11:10.909452 currentscape-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-14 12:11:07.000000 currentscape-0.0.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-06-14 12:11:07.000000 currentscape-0.0.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-14 12:11:07.000000 currentscape-0.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-14 12:11:07.000000 currentscape-0.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10036 2023-06-14 12:11:10.909452 currentscape-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-06-14 12:11:07.000000 currentscape-0.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:11:10.905452 currentscape-0.0.0/currentscape/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-14 12:11:07.000000 currentscape-0.0.0/currentscape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-06-14 12:11:07.000000 currentscape-0.0.0/currentscape/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    23183 2023-06-14 12:11:07.000000 currentscape-0.0.0/currentscape/currents.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-06-14 12:11:07.000000 currentscape-0.0.0/currentscape/currentscape.py
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-06-14 12:11:07.000000 currentscape-0.0.0/currentscape/data_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-06-14 12:11:07.000000 currentscape-0.0.0/currentscape/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-06-14 12:11:07.000000 currentscape-0.0.0/currentscape/ions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-06-14 12:11:07.000000 currentscape-0.0.0/currentscape/legends.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-06-14 12:11:07.000000 currentscape-0.0.0/currentscape/mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    18165 2023-06-14 12:11:07.000000 currentscape-0.0.0/currentscape/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-14 12:11:07.000000 currentscape-0.0.0/currentscape/voltages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:11:10.905452 currentscape-0.0.0/currentscape.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10036 2023-06-14 12:11:10.000000 currentscape-0.0.0/currentscape.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-14 12:11:10.000000 currentscape-0.0.0/currentscape.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 12:11:10.000000 currentscape-0.0.0/currentscape.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-14 12:11:10.000000 currentscape-0.0.0/currentscape.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 12:11:10.000000 currentscape-0.0.0/currentscape.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 12:11:10.909452 currentscape-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-14 12:11:07.000000 currentscape-0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:11:10.909452 currentscape-0.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 12:11:07.000000 currentscape-0.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-14 12:11:07.000000 currentscape-0.0.0/tests/extract_bNAC_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-14 12:11:07.000000 currentscape-0.0.0/tests/test_currentscape_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-14 12:11:07.000000 currentscape-0.0.0/tests/test_currentscape_currents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-14 12:11:07.000000 currentscape-0.0.0/tests/test_currentscape_dataprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-14 12:11:07.000000 currentscape-0.0.0/tests/test_currentscape_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-14 12:11:07.000000 currentscape-0.0.0/tests/test_currentscape_from_paper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-14 12:11:07.000000 currentscape-0.0.0/tests/test_currentscape_ions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-14 12:11:07.000000 currentscape-0.0.0/tests/test_currentscape_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-06-14 12:11:07.000000 currentscape-0.0.0/tests/test_currentscape_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-14 12:11:07.000000 currentscape-0.0.0/tests/test_use_case_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-14 12:11:07.000000 currentscape-0.0.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.796502 currentscape-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.776502 currentscape-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.780502 currentscape-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-14 15:26:14.000000 currentscape-1.0.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-14 15:26:14.000000 currentscape-1.0.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-14 15:26:14.000000 currentscape-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-14 15:26:14.000000 currentscape-1.0.1/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-14 15:26:14.000000 currentscape-1.0.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-14 15:26:14.000000 currentscape-1.0.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-14 15:26:14.000000 currentscape-1.0.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-14 15:26:14.000000 currentscape-1.0.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-06-14 15:26:14.000000 currentscape-1.0.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-06-14 15:26:14.000000 currentscape-1.0.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-14 15:26:14.000000 currentscape-1.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-14 15:26:14.000000 currentscape-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-14 15:26:14.000000 currentscape-1.0.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-06-14 15:26:21.796502 currentscape-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9237 2023-06-14 15:26:14.000000 currentscape-1.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15156 2023-06-14 15:26:14.000000 currentscape-1.0.1/Tutorial.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.780502 currentscape-1.0.1/currentscape/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-14 15:26:14.000000 currentscape-1.0.1/currentscape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-06-14 15:26:14.000000 currentscape-1.0.1/currentscape/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23209 2023-06-14 15:26:14.000000 currentscape-1.0.1/currentscape/currents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-06-14 15:26:14.000000 currentscape-1.0.1/currentscape/currentscape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-06-14 15:26:14.000000 currentscape-1.0.1/currentscape/data_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-06-14 15:26:14.000000 currentscape-1.0.1/currentscape/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-06-14 15:26:14.000000 currentscape-1.0.1/currentscape/ions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-06-14 15:26:14.000000 currentscape-1.0.1/currentscape/legends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-06-14 15:26:14.000000 currentscape-1.0.1/currentscape/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18165 2023-06-14 15:26:14.000000 currentscape-1.0.1/currentscape/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-14 15:26:14.000000 currentscape-1.0.1/currentscape/voltages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.780502 currentscape-1.0.1/currentscape.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-06-14 15:26:21.000000 currentscape-1.0.1/currentscape.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-14 15:26:21.000000 currentscape-1.0.1/currentscape.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 15:26:21.000000 currentscape-1.0.1/currentscape.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-14 15:26:21.000000 currentscape-1.0.1/currentscape.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 15:26:21.000000 currentscape-1.0.1/currentscape.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.784502 currentscape-1.0.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-14 15:26:14.000000 currentscape-1.0.1/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.784502 currentscape-1.0.1/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-14 15:26:14.000000 currentscape-1.0.1/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-14 15:26:14.000000 currentscape-1.0.1/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-14 15:26:14.000000 currentscape-1.0.1/doc/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.784502 currentscape-1.0.1/doc/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   170626 2023-06-14 15:26:14.000000 currentscape-1.0.1/doc/source/images/plot.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46597 2023-06-14 15:26:14.000000 currentscape-1.0.1/doc/source/images/quickstart_plot.png
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-14 15:26:14.000000 currentscape-1.0.1/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-14 15:26:14.000000 currentscape-1.0.1/doc/source/tutorial.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.776502 currentscape-1.0.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.784502 currentscape-1.0.1/examples/original_paper_plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/original_paper_plot/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/original_paper_plot/LICENSE_CC0-1.0
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/original_paper_plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/original_paper_plot/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/original_paper_plot/get_currents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/original_paper_plot/integrate_single_compartment_and_plot_currentscape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.788502 currentscape-1.0.1/examples/original_paper_plot/parameters-and-initial-conditions/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/original_paper_plot/parameters-and-initial-conditions/initial-conditions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/original_paper_plot/parameters-and-initial-conditions/model-A-name-HZFTSB.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/original_paper_plot/parameters-and-initial-conditions/model-B-name-8XCUQE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/original_paper_plot/parameters-and-initial-conditions/model-C-name-C1L1R0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/original_paper_plot/parameters-and-initial-conditions/model-D-name-KI47XV.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/original_paper_plot/parameters-and-initial-conditions/model-E-name-OG1RE2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/original_paper_plot/parameters-and-initial-conditions/model-F-name-B7S21N.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG2-name-1BLGMA.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/original_paper_plot/parameters-and-initial-conditions/model-FIG3-name-VVECT5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/original_paper_plot/single_compartment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.788502 currentscape-1.0.1/examples/use_case/
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/LICENSE_CC-BY-CA-SA-4.0
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.776502 currentscape-1.0.1/examples/use_case/config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.788502 currentscape-1.0.1/examples/use_case/config/params/
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/config/params/final.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/config/params/pyr.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.792502 currentscape-1.0.1/examples/use_case/mechanisms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/mechanisms/CaDynamics_DC0.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/mechanisms/Ca_HVA2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/mechanisms/Ca_LVAst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/mechanisms/Ih.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/mechanisms/K_Pst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/mechanisms/K_Tst.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/mechanisms/NaTg.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/mechanisms/Nap_Et2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/mechanisms/SK_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/mechanisms/SKv3_1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/mechanisms/notes.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.792502 currentscape-1.0.1/examples/use_case/morphology/
+-rw-r--r--   0 runner    (1001) docker     (123)   135189 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/morphology/dend-C231296A-P4B2_axon-C200897C-P2_-_Scale_x1.000_y0.975_z1.000.asc
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.792502 currentscape-1.0.1/examples/use_case/python_recordings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/python_recordings/.keep
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-06-14 15:26:14.000000 currentscape-1.0.1/examples/use_case/run_py.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.776502 currentscape-1.0.1/extra/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.792502 currentscape-1.0.1/extra/jjb-cells/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-14 15:26:14.000000 currentscape-1.0.1/extra/jjb-cells/cells.currentscape.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.776502 currentscape-1.0.1/extra/spack/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.776502 currentscape-1.0.1/extra/spack/var/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.776502 currentscape-1.0.1/extra/spack/var/spack/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.776502 currentscape-1.0.1/extra/spack/var/spack/repos/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.776502 currentscape-1.0.1/extra/spack/var/spack/repos/builtin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.776502 currentscape-1.0.1/extra/spack/var/spack/repos/builtin/packages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.792502 currentscape-1.0.1/extra/spack/var/spack/repos/builtin/packages/py-currentscape/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-14 15:26:14.000000 currentscape-1.0.1/extra/spack/var/spack/repos/builtin/packages/py-currentscape/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-14 15:26:14.000000 currentscape-1.0.1/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 15:26:21.796502 currentscape-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-14 15:26:14.000000 currentscape-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:21.796502 currentscape-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:26:14.000000 currentscape-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-14 15:26:14.000000 currentscape-1.0.1/tests/extract_bNAC_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-14 15:26:14.000000 currentscape-1.0.1/tests/test_currentscape_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-14 15:26:14.000000 currentscape-1.0.1/tests/test_currentscape_currents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-14 15:26:14.000000 currentscape-1.0.1/tests/test_currentscape_dataprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-14 15:26:14.000000 currentscape-1.0.1/tests/test_currentscape_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-14 15:26:14.000000 currentscape-1.0.1/tests/test_currentscape_from_paper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-14 15:26:14.000000 currentscape-1.0.1/tests/test_currentscape_ions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-14 15:26:14.000000 currentscape-1.0.1/tests/test_currentscape_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-06-14 15:26:14.000000 currentscape-1.0.1/tests/test_currentscape_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-14 15:26:14.000000 currentscape-1.0.1/tests/test_use_case_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-14 15:26:14.000000 currentscape-1.0.1/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-14 15:26:14.000000 currentscape-1.0.1/tox.ini
```

### Comparing `currentscape-0.0.0/COPYING` & `currentscape-1.0.1/COPYING`

 * *Files identical despite different names*

### Comparing `currentscape-0.0.0/LICENSE.txt` & `currentscape-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `currentscape-0.0.0/PKG-INFO` & `currentscape-1.0.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6375 7272  : 2.1.Name: curr
 00000020: 656e 7473 6361 7065 0a56 6572 7369 6f6e  entscape.Version
-00000030: 3a20 302e 302e 300a 5375 6d6d 6172 793a  : 0.0.0.Summary:
+00000030: 3a20 312e 302e 310a 5375 6d6d 6172 793a  : 1.0.1.Summary:
 00000040: 204d 6f64 756c 6520 746f 2065 6173 696c   Module to easil
 00000050: 7920 706c 6f74 2063 7572 7265 6e74 7363  y plot currentsc
 00000060: 6170 652e 0a48 6f6d 652d 7061 6765 3a20  ape..Home-page: 
 00000070: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
 00000080: 6f6d 2f42 6c75 6542 7261 696e 2f43 7572  om/BlueBrain/Cur
 00000090: 7265 6e74 7363 6170 650a 4175 7468 6f72  rentscape.Author
 000000a0: 3a20 426c 7565 2042 7261 696e 2050 726f  : Blue Brain Pro
@@ -52,577 +52,593 @@
 00000330: 7373 6966 6965 723a 2054 6f70 6963 203a  ssifier: Topic :
 00000340: 3a20 5363 6965 6e74 6966 6963 2f45 6e67  : Scientific/Eng
 00000350: 696e 6565 7269 6e67 203a 3a20 4269 6f2d  ineering :: Bio-
 00000360: 496e 666f 726d 6174 6963 730a 5265 7175  Informatics.Requ
 00000370: 6972 6573 2d50 7974 686f 6e3a 203e 3d33  ires-Python: >=3
 00000380: 2e37 0a44 6573 6372 6970 7469 6f6e 2d43  .7.Description-C
 00000390: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
-000003a0: 742f 6d61 726b 646f 776e 0a50 726f 7669  t/markdown.Provi
-000003b0: 6465 732d 4578 7472 613a 2064 6f63 730a  des-Extra: docs.
-000003c0: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
-000003d0: 6578 616d 706c 650a 4c69 6365 6e73 652d  example.License-
-000003e0: 4669 6c65 3a20 4c49 4345 4e53 452e 7478  File: LICENSE.tx
-000003f0: 740a 4c69 6365 6e73 652d 4669 6c65 3a20  t.License-File: 
-00000400: 434f 5059 494e 470a 4c69 6365 6e73 652d  COPYING.License-
-00000410: 4669 6c65 3a20 4155 5448 4f52 532e 7273  File: AUTHORS.rs
-00000420: 740a 0a43 7572 7265 6e74 7363 6170 650a  t..Currentscape.
-00000430: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a 2e2e  ============....
-00000440: 2072 6177 3a3a 2068 746d 6c0a 0a09 3c74   raw:: html...<t
-00000450: 6162 6c65 3e0a 093c 7472 3e0a 0920 203c  able>..<tr>..  <
-00000460: 7464 3e4c 6174 6573 7420 5265 6c65 6173  td>Latest Releas
-00000470: 653c 2f74 643e 0a09 2020 3c74 643e 0a09  e</td>..  <td>..
-00000480: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
-00000490: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
-000004a0: 6f6a 6563 742f 6375 7272 656e 7473 6361  oject/currentsca
-000004b0: 7065 2f22 3e0a 0920 2020 203c 696d 6720  pe/">..    <img 
-000004c0: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
-000004d0: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
-000004e0: 2f76 2f63 7572 7265 6e74 7363 6170 652e  /v/currentscape.
-000004f0: 7376 6722 2061 6c74 3d22 6c61 7465 7374  svg" alt="latest
-00000500: 2072 656c 6561 7365 2220 2f3e 0a09 2020   release" />..  
-00000510: 2020 3c2f 613e 0a09 2020 3c2f 7464 3e0a    </a>..  </td>.
-00000520: 093c 2f74 723e 0a09 3c74 723e 0a09 2020  .</tr>..<tr>..  
-00000530: 3c74 643e 446f 6375 6d65 6e74 6174 696f  <td>Documentatio
-00000540: 6e3c 2f74 643e 0a09 2020 3c74 643e 0a09  n</td>..  <td>..
-00000550: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
-00000560: 7073 3a2f 2f63 7572 7265 6e74 7363 6170  ps://currentscap
-00000570: 652e 7265 6164 7468 6564 6f63 732e 696f  e.readthedocs.io
-00000580: 2f22 3e0a 0920 2020 203c 696d 6720 7372  /">..    <img sr
-00000590: 633d 2268 7474 7073 3a2f 2f72 6561 6474  c="https://readt
-000005a0: 6865 646f 6373 2e6f 7267 2f70 726f 6a65  hedocs.org/proje
-000005b0: 6374 732f 6375 7272 656e 7473 6361 7065  cts/currentscape
-000005c0: 2f62 6164 6765 2f3f 7665 7273 696f 6e3d  /badge/?version=
-000005d0: 6c61 7465 7374 2220 616c 743d 226c 6174  latest" alt="lat
-000005e0: 6573 7420 646f 6375 6d65 6e74 6174 696f  est documentatio
-000005f0: 6e22 202f 3e0a 0920 2020 203c 2f61 3e0a  n" />..    </a>.
-00000600: 0920 203c 2f74 643e 0a09 3c2f 7472 3e0a  .  </td>..</tr>.
-00000610: 093c 7472 3e0a 0920 203c 7464 3e4c 6963  .<tr>..  <td>Lic
-00000620: 656e 7365 3c2f 7464 3e0a 0920 203c 7464  ense</td>..  <td
-00000630: 3e0a 0920 2020 203c 6120 6872 6566 3d22  >..    <a href="
-00000640: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000650: 6f6d 2f42 6c75 6542 7261 696e 2f43 7572  om/BlueBrain/Cur
-00000660: 7265 6e74 7363 6170 652f 626c 6f62 2f6d  rentscape/blob/m
-00000670: 6169 6e2f 4c49 4345 4e53 452e 7478 7422  ain/LICENSE.txt"
-00000680: 3e0a 0920 2020 203c 696d 6720 7372 633d  >..    <img src=
-00000690: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
-000006a0: 656c 6473 2e69 6f2f 7079 7069 2f6c 2f63  elds.io/pypi/l/c
-000006b0: 7572 7265 6e74 7363 6170 652e 7376 6722  urrentscape.svg"
-000006c0: 2061 6c74 3d22 6c69 6365 6e73 6522 202f   alt="license" /
-000006d0: 3e0a 0920 2020 203c 2f61 3e0a 093c 2f74  >..    </a>..</t
-000006e0: 643e 0a09 3c2f 7472 3e0a 093c 7472 3e0a  d>..</tr>..<tr>.
-000006f0: 0920 203c 7464 3e42 7569 6c64 2053 7461  .  <td>Build Sta
-00000700: 7475 733c 2f74 643e 0a09 2020 3c74 643e  tus</td>..  <td>
-00000710: 0a09 2020 2020 3c61 2068 7265 663d 2268  ..    <a href="h
-00000720: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000730: 6d2f 426c 7565 4272 6169 6e2f 4375 7272  m/BlueBrain/Curr
-00000740: 656e 7473 6361 7065 2f61 6374 696f 6e73  entscape/actions
-00000750: 223e 0a09 2020 2020 3c69 6d67 2073 7263  ">..    <img src
-00000760: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
-00000770: 2e63 6f6d 2f42 6c75 6542 7261 696e 2f43  .com/BlueBrain/C
-00000780: 7572 7265 6e74 7363 6170 652f 776f 726b  urrentscape/work
-00000790: 666c 6f77 732f 5465 7374 2f62 6164 6765  flows/Test/badge
-000007a0: 2e73 7667 3f62 7261 6e63 683d 6d61 696e  .svg?branch=main
-000007b0: 2220 616c 743d 2241 6374 696f 6e73 2062  " alt="Actions b
-000007c0: 7569 6c64 2073 7461 7475 7322 202f 3e0a  uild status" />.
-000007d0: 0920 2020 203c 2f61 3e0a 0920 203c 2f74  .    </a>..  </t
-000007e0: 643e 0a09 3c2f 7472 3e0a 093c 7472 3e0a  d>..</tr>..<tr>.
-000007f0: 0920 203c 7464 3e43 6f76 6572 6167 653c  .  <td>Coverage<
-00000800: 2f74 643e 0a09 2020 3c74 643e 0a09 2020  /td>..  <td>..  
-00000810: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-00000820: 3a2f 2f63 6f64 6563 6f76 2e69 6f2f 6768  ://codecov.io/gh
-00000830: 2f42 6c75 6542 7261 696e 2f63 7572 7265  /BlueBrain/curre
-00000840: 6e74 7363 6170 6522 3e0a 0920 2020 203c  ntscape">..    <
-00000850: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00000860: 2f63 6f64 6563 6f76 2e69 6f2f 6769 7468  /codecov.io/gith
-00000870: 7562 2f42 6c75 6542 7261 696e 2f43 7572  ub/BlueBrain/Cur
-00000880: 7265 6e74 7363 6170 652f 636f 7665 7261  rentscape/covera
-00000890: 6765 2e73 7667 3f62 7261 6e63 683d 6d61  ge.svg?branch=ma
-000008a0: 696e 2220 616c 743d 2263 6f76 6572 6167  in" alt="coverag
-000008b0: 6522 202f 3e0a 0920 2020 203c 2f61 3e0a  e" />..    </a>.
-000008c0: 0920 203c 2f74 643e 0a09 3c2f 7472 3e0a  .  </td>..</tr>.
-000008d0: 093c 7472 3e0a 0909 3c74 643e 4769 7474  .<tr>...<td>Gitt
-000008e0: 6572 3c2f 7464 3e0a 0909 3c74 643e 0a09  er</td>...<td>..
-000008f0: 0909 3c61 2068 7265 663d 2268 7474 7073  ..<a href="https
-00000900: 3a2f 2f67 6974 7465 722e 696d 2f62 6c75  ://gitter.im/blu
-00000910: 6562 7261 696e 2f63 7572 7265 6e74 7363  ebrain/currentsc
-00000920: 6170 6522 3e0a 0909 093c 696d 6720 7372  ape">....<img sr
-00000930: 633d 2268 7474 7073 3a2f 2f62 6164 6765  c="https://badge
-00000940: 732e 6769 7474 6572 2e69 6d2f 4a6f 696e  s.gitter.im/Join
-00000950: 2532 3043 6861 742e 7376 6722 0a09 093c  %20Chat.svg"...<
-00000960: 2f61 3e0a 0909 3c2f 7464 3e0a 093c 2f74  /a>...</td>..</t
-00000970: 723e 0a09 3c2f 7461 626c 653e 0a0a 496e  r>..</table>..In
-00000980: 7472 6f64 7563 7469 6f6e 0a3d 3d3d 3d3d  troduction.=====
-00000990: 3d3d 3d3d 3d3d 3d0a 0a43 7572 7265 6e74  =======..Current
-000009a0: 7363 6170 6520 6973 2061 2050 7974 686f  scape is a Pytho
-000009b0: 6e20 746f 6f6c 2065 6e61 626c 696e 6720  n tool enabling 
-000009c0: 7363 6965 6e74 6973 7473 2074 6f20 6561  scientists to ea
-000009d0: 7369 6c79 2070 6c6f 7420 7468 6520 6375  sily plot the cu
-000009e0: 7272 656e 7473 2069 6e20 656c 6563 7472  rrents in electr
-000009f0: 6963 616c 206e 6575 726f 6e20 6d6f 6465  ical neuron mode
-00000a00: 6c73 2e0a 5468 6520 636f 6465 2069 7320  ls..The code is 
-00000a10: 6261 7365 6420 6f6e 2074 6865 2070 6170  based on the pap
-00000a20: 6572 2060 416c 6f6e 736f 2061 6e64 204d  er `Alonso and M
-00000a30: 6172 6465 722c 2032 3031 3920 3c68 7474  arder, 2019 <htt
-00000a40: 7073 3a2f 2f64 6f69 2e6f 7267 2f31 302e  ps://doi.org/10.
-00000a50: 3735 3534 2f65 4c69 6665 2e34 3237 3232  7554/eLife.42722
-00000a60: 3e60 5f2e 0a0a 4375 7272 656e 7473 6361  >`_...Currentsca
-00000a70: 7065 2066 6967 7572 6573 2070 6c6f 7420  pe figures plot 
-00000a80: 7468 6520 7065 7263 656e 7461 6765 206f  the percentage o
-00000a90: 6620 696e 7761 7264 2061 6e64 206f 7574  f inward and out
-00000aa0: 7761 7264 2069 6f6e 6963 206d 656d 6272  ward ionic membr
-00000ab0: 616e 6520 6375 7272 656e 7473 2c0a 7468  ane currents,.th
-00000ac0: 6520 746f 7461 6c20 696e 7761 7264 2061  e total inward a
-00000ad0: 6e64 206f 7574 7761 7264 2063 7572 7265  nd outward curre
-00000ae0: 6e74 732c 2061 7320 7765 6c6c 2061 7320  nts, as well as 
-00000af0: 7468 6520 766f 6c74 6167 6520 696e 2066  the voltage in f
-00000b00: 756e 6374 696f 6e20 6f66 2074 696d 652e  unction of time.
-00000b10: 0a49 7420 616c 6c6f 7773 206d 6f64 656c  .It allows model
-00000b20: 6c65 7273 2074 6f20 7365 6520 7768 6963  lers to see whic
-00000b30: 6820 6375 7272 656e 7473 2070 6c61 7920  h currents play 
-00000b40: 6120 726f 6c65 2061 7420 616e 7920 6769  a role at any gi
-00000b50: 7665 6e20 7469 6d65 2064 7572 696e 6720  ven time during 
-00000b60: 6120 7369 6d75 6c61 7469 6f6e 2c20 616e  a simulation, an
-00000b70: 6420 6368 6563 6b20 696e 2064 6570 7468  d check in depth
-00000b80: 2074 6865 2063 7572 7265 6e74 2064 796e   the current dyn
-00000b90: 616d 6963 732e 0a0a 2e2e 2069 6d61 6765  amics..... image
-00000ba0: 3a3a 2064 6f63 2f73 6f75 7263 652f 696d  :: doc/source/im
-00000bb0: 6167 6573 2f70 6c6f 742e 706e 670a 0a43  ages/plot.png..C
-00000bc0: 6974 6174 696f 6e0a 3d3d 3d3d 3d3d 3d3d  itation.========
-00000bd0: 0a0a 5768 656e 2079 6f75 2075 7365 2074  ..When you use t
-00000be0: 6869 7320 4375 7272 656e 7473 6361 7065  his Currentscape
-00000bf0: 2073 6f66 7477 6172 6520 666f 7220 796f   software for yo
-00000c00: 7572 2072 6573 6561 7263 682c 2077 6520  ur research, we 
-00000c10: 6173 6b20 796f 7520 746f 2063 6974 6520  ask you to cite 
-00000c20: 7468 6520 666f 6c6c 6f77 696e 6720 7075  the following pu
-00000c30: 626c 6963 6174 696f 6e20 2874 6869 7320  blication (this 
-00000c40: 696e 636c 7564 6573 2070 6f73 7465 7220  includes poster 
-00000c50: 7072 6573 656e 7461 7469 6f6e 7329 3a0a  presentations):.
-00000c60: 0a2e 2e20 636f 6465 2d62 6c6f 636b 3a3a  ... code-block::
-00000c70: 200a 0a20 2020 2040 6172 7469 636c 6520   ..    @article 
-00000c80: 7b31 302e 3735 3534 2f65 4c69 6665 2e34  {10.7554/eLife.4
-00000c90: 3237 3232 2c0a 2020 2020 6172 7469 636c  2722,.    articl
-00000ca0: 655f 7479 7065 203d 207b 6a6f 7572 6e61  e_type = {journa
-00000cb0: 6c7d 2c0a 2020 2020 7469 746c 6520 3d20  l},.    title = 
-00000cc0: 7b56 6973 7561 6c69 7a61 7469 6f6e 206f  {Visualization o
-00000cd0: 6620 6375 7272 656e 7473 2069 6e20 6e65  f currents in ne
-00000ce0: 7572 616c 206d 6f64 656c 7320 7769 7468  ural models with
-00000cf0: 2073 696d 696c 6172 2062 6568 6176 696f   similar behavio
-00000d00: 7220 616e 6420 6469 6666 6572 656e 7420  r and different 
-00000d10: 636f 6e64 7563 7461 6e63 6520 6465 6e73  conductance dens
-00000d20: 6974 6965 737d 2c0a 2020 2020 6175 7468  ities},.    auth
-00000d30: 6f72 203d 207b 416c 6f6e 736f 2c20 4c65  or = {Alonso, Le
-00000d40: 616e 6472 6f20 4d20 616e 6420 4d61 7264  andro M and Mard
-00000d50: 6572 2c20 4576 657d 2c0a 2020 2020 6564  er, Eve},.    ed
-00000d60: 6974 6f72 203d 207b 5765 7374 6272 6f6f  itor = {Westbroo
-00000d70: 6b2c 2047 6172 7920 4c20 616e 6420 536b  k, Gary L and Sk
-00000d80: 696e 6e65 722c 2046 7261 6e63 6573 204b  inner, Frances K
-00000d90: 2061 6e64 204c 616e 6b61 7261 6e79 2c20   and Lankarany, 
-00000da0: 4d69 6c61 6420 616e 6420 4272 6974 746f  Milad and Britto
-00000db0: 6e2c 204f 6c69 7665 727d 2c0a 2020 2020  n, Oliver},.    
-00000dc0: 766f 6c75 6d65 203d 2038 2c0a 2020 2020  volume = 8,.    
-00000dd0: 7965 6172 203d 2032 3031 392c 0a20 2020  year = 2019,.   
-00000de0: 206d 6f6e 7468 203d 207b 6a61 6e7d 2c0a   month = {jan},.
-00000df0: 2020 2020 7075 625f 6461 7465 203d 207b      pub_date = {
-00000e00: 3230 3139 2d30 312d 3331 7d2c 0a20 2020  2019-01-31},.   
-00000e10: 2070 6167 6573 203d 207b 6534 3237 3232   pages = {e42722
-00000e20: 7d2c 0a20 2020 2063 6974 6174 696f 6e20  },.    citation 
-00000e30: 3d20 7b65 4c69 6665 2032 3031 393b 383a  = {eLife 2019;8:
-00000e40: 6534 3237 3232 7d2c 0a20 2020 2064 6f69  e42722},.    doi
-00000e50: 203d 207b 3130 2e37 3535 342f 654c 6966   = {10.7554/eLif
-00000e60: 652e 3432 3732 327d 2c0a 2020 2020 7572  e.42722},.    ur
-00000e70: 6c20 3d20 7b68 7474 7073 3a2f 2f64 6f69  l = {https://doi
-00000e80: 2e6f 7267 2f31 302e 3735 3534 2f65 4c69  .org/10.7554/eLi
-00000e90: 6665 2e34 3237 3232 7d2c 0a20 2020 2061  fe.42722},.    a
-00000ea0: 6273 7472 6163 7420 3d20 7b43 6f6e 6475  bstract = {Condu
-00000eb0: 6374 616e 6365 2d62 6173 6564 206d 6f64  ctance-based mod
-00000ec0: 656c 7320 6f66 206e 6575 7261 6c20 6163  els of neural ac
-00000ed0: 7469 7669 7479 2070 726f 6475 6365 206c  tivity produce l
-00000ee0: 6172 6765 2061 6d6f 756e 7473 206f 6620  arge amounts of 
-00000ef0: 6461 7461 2074 6861 7420 6361 6e20 6265  data that can be
-00000f00: 2068 6172 6420 746f 2076 6973 7561 6c69   hard to visuali
-00000f10: 7a65 2061 6e64 2069 6e74 6572 7072 6574  ze and interpret
-00000f20: 2e20 5765 2069 6e74 726f 6475 6365 2076  . We introduce v
-00000f30: 6973 7561 6c69 7a61 7469 6f6e 206d 6574  isualization met
-00000f40: 686f 6473 2074 6f20 6469 7370 6c61 7920  hods to display 
-00000f50: 7468 6520 6479 6e61 6d69 6373 206f 6620  the dynamics of 
-00000f60: 7468 6520 696f 6e69 6320 6375 7272 656e  the ionic curren
-00000f70: 7473 2061 6e64 2074 6f20 6469 7370 6c61  ts and to displa
-00000f80: 7920 7468 6520 6d6f 6465 6c73 e280 9920  y the models... 
-00000f90: 7265 7370 6f6e 7365 2074 6f20 7065 7274  response to pert
-00000fa0: 7572 6261 7469 6f6e 732e 2054 6f20 7669  urbations. To vi
-00000fb0: 7375 616c 697a 6520 7468 6520 6375 7272  sualize the curr
-00000fc0: 656e 7473 e280 9920 6479 6e61 6d69 6373  ents... dynamics
-00000fd0: 2c20 7765 2063 6f6d 7075 7465 2074 6865  , we compute the
-00000fe0: 2070 6572 6365 6e74 2063 6f6e 7472 6962   percent contrib
-00000ff0: 7574 696f 6e20 6f66 2065 6163 6820 6375  ution of each cu
-00001000: 7272 656e 7420 616e 6420 6469 7370 6c61  rrent and displa
-00001010: 7920 7468 656d 206f 7665 7220 7469 6d65  y them over time
-00001020: 2075 7369 6e67 2073 7461 636b 6564 2d61   using stacked-a
-00001030: 7265 6120 706c 6f74 732e 2054 6865 2077  rea plots. The w
-00001040: 6176 6566 6f72 6d20 6f66 2074 6865 206d  aveform of the m
-00001050: 656d 6272 616e 6520 706f 7465 6e74 6961  embrane potentia
-00001060: 6c20 616e 6420 7468 6520 636f 6e74 7269  l and the contri
-00001070: 6275 7469 6f6e 206f 6620 6561 6368 2063  bution of each c
-00001080: 7572 7265 6e74 2063 6861 6e67 6520 6173  urrent change as
-00001090: 2074 6865 206d 6f64 656c 7320 6172 6520   the models are 
-000010a0: 7065 7274 7572 6265 642e 2054 6f20 7265  perturbed. To re
-000010b0: 7072 6573 656e 7420 7468 6573 6520 6368  present these ch
-000010c0: 616e 6765 7320 6f76 6572 2061 2072 616e  anges over a ran
-000010d0: 6765 206f 6620 7468 6520 7065 7274 7572  ge of the pertur
-000010e0: 6261 7469 6f6e 2063 6f6e 7472 6f6c 2070  bation control p
-000010f0: 6172 616d 6574 6572 2c20 7765 2063 6f6d  arameter, we com
-00001100: 7075 7465 2061 6e64 2064 6973 706c 6179  pute and display
-00001110: 2074 6865 2064 6973 7472 6962 7574 696f   the distributio
-00001120: 6e73 206f 6620 7468 6573 6520 7761 7665  ns of these wave
-00001130: 666f 726d 732e 2057 6520 696c 6c75 7374  forms. We illust
-00001140: 7261 7465 2074 6865 7365 2070 726f 6365  rate these proce
-00001150: 6475 7265 7320 696e 2073 6978 2065 7861  dures in six exa
-00001160: 6d70 6c65 7320 6f66 2062 7572 7374 696e  mples of burstin
-00001170: 6720 6d6f 6465 6c20 6e65 7572 6f6e 7320  g model neurons 
-00001180: 7769 7468 2073 696d 696c 6172 2061 6374  with similar act
-00001190: 6976 6974 7920 6275 7420 7468 6174 2064  ivity but that d
-000011a0: 6966 6665 7220 6173 206d 7563 6820 6173  iffer as much as
-000011b0: 2074 6872 6565 666f 6c64 2069 6e20 7468   threefold in th
-000011c0: 6569 7220 636f 6e64 7563 7461 6e63 6520  eir conductance 
-000011d0: 6465 6e73 6974 6965 732e 2054 6865 7365  densities. These
-000011e0: 2076 6973 7561 6c69 7a61 7469 6f6e 206d   visualization m
-000011f0: 6574 686f 6473 2070 726f 7669 6465 2068  ethods provide h
-00001200: 6575 7269 7374 6963 2069 6e73 6967 6874  euristic insight
-00001210: 2069 6e74 6f20 7768 7920 696e 6469 7669   into why indivi
-00001220: 6475 616c 206e 6575 726f 6e73 206f 7220  dual neurons or 
-00001230: 6e65 7477 6f72 6b73 2077 6974 6820 7369  networks with si
-00001240: 6d69 6c61 7220 6265 6861 7669 6f72 2063  milar behavior c
-00001250: 616e 2072 6573 706f 6e64 2077 6964 656c  an respond widel
-00001260: 7920 6469 6666 6572 656e 746c 7920 746f  y differently to
-00001270: 2070 6572 7475 7262 6174 696f 6e73 2e7d   perturbations.}
-00001280: 2c0a 2020 2020 6b65 7977 6f72 6473 203d  ,.    keywords =
-00001290: 207b 6e65 7572 6f6e 616c 206f 7363 696c   {neuronal oscil
-000012a0: 6c61 746f 7273 2c20 4e61 2b20 6368 616e  lators, Na+ chan
-000012b0: 6e65 6c73 2c20 4361 2b2b 2063 6861 6e6e  nels, Ca++ chann
-000012c0: 656c 732c 204b 2b20 6368 616e 6e65 6c73  els, K+ channels
-000012d0: 2c20 636f 6e64 7563 7461 6e63 652d 6261  , conductance-ba
-000012e0: 7365 642c 2069 6f6e 6963 2063 6861 6e6e  sed, ionic chann
-000012f0: 656c 737d 2c0a 2020 2020 6a6f 7572 6e61  els},.    journa
-00001300: 6c20 3d20 7b65 4c69 6665 7d2c 0a20 2020  l = {eLife},.   
-00001310: 2069 7373 6e20 3d20 7b32 3035 302d 3038   issn = {2050-08
-00001320: 3458 7d2c 0a20 2020 2070 7562 6c69 7368  4X},.    publish
-00001330: 6572 203d 207b 654c 6966 6520 5363 6965  er = {eLife Scie
-00001340: 6e63 6573 2050 7562 6c69 6361 7469 6f6e  nces Publication
-00001350: 732c 204c 7464 7d2c 0a20 2020 207d 0a0a  s, Ltd},.    }..
-00001360: 5375 7070 6f72 740a 3d3d 3d3d 3d3d 3d0a  Support.=======.
-00001370: 0a57 6520 6172 6520 7072 6f76 6964 696e  .We are providin
-00001380: 6720 7375 7070 6f72 7420 6f6e 2060 4769  g support on `Gi
-00001390: 7474 6572 203c 6874 7470 733a 2f2f 6769  tter <https://gi
-000013a0: 7474 6572 2e69 6d2f 426c 7565 4272 6169  tter.im/BlueBrai
-000013b0: 6e2f 4375 7272 656e 7473 6361 7065 3e60  n/Currentscape>`
-000013c0: 5f2e 2057 6520 7375 6767 6573 7420 796f  _. We suggest yo
-000013d0: 7520 6372 6561 7465 2074 6963 6b65 7473  u create tickets
-000013e0: 206f 6e20 7468 6520 6047 6974 6875 6220   on the `Github 
-000013f0: 6973 7375 6520 7472 6163 6b65 7220 3c68  issue tracker <h
-00001400: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001410: 6d2f 426c 7565 4272 6169 6e2f 4375 7272  m/BlueBrain/Curr
-00001420: 656e 7473 6361 7065 2f69 7373 7565 733e  entscape/issues>
-00001430: 605f 2069 6e20 6361 7365 2079 6f75 2065  `_ in case you e
-00001440: 6e63 6f75 6e74 6572 2070 726f 626c 656d  ncounter problem
-00001450: 7320 7768 696c 6520 7573 696e 6720 7468  s while using th
-00001460: 6520 736f 6674 7761 7265 206f 7220 6966  e software or if
-00001470: 2079 6f75 2068 6176 6520 736f 6d65 2073   you have some s
-00001480: 7567 6765 7374 696f 6e73 2e0a 0a4d 6169  uggestions...Mai
-00001490: 6e20 6465 7065 6e64 656e 6369 6573 0a3d  n dependencies.=
-000014a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000014b0: 0a0a 2d20 6050 7974 686f 6e20 332e 372b  ..- `Python 3.7+
-000014c0: 203c 6874 7470 733a 2f2f 7777 772e 7079   <https://www.py
-000014d0: 7468 6f6e 2e6f 7267 2f64 6f77 6e6c 6f61  thon.org/downloa
-000014e0: 6473 2f72 656c 6561 7365 2f70 7974 686f  ds/release/pytho
-000014f0: 6e2d 3337 302f 3e60 5f0a 2d20 604e 756d  n-370/>`_.- `Num
-00001500: 7079 203c 6874 7470 733a 2f2f 6e75 6d70  py <https://nump
-00001510: 792e 6f72 672f 3e60 5f20 2861 7574 6f6d  y.org/>`_ (autom
-00001520: 6174 6963 616c 6c79 2069 6e73 7461 6c6c  atically install
-00001530: 6564 2062 7920 7069 7029 0a2d 2060 5061  ed by pip).- `Pa
-00001540: 6c65 7474 6162 6c65 203c 6874 7470 733a  lettable <https:
-00001550: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 6966  //github.com/jif
-00001560: 6679 636c 7562 2f70 616c 6574 7461 626c  fyclub/palettabl
-00001570: 653e 605f 2028 6175 746f 6d61 7469 6361  e>`_ (automatica
-00001580: 6c6c 7920 696e 7374 616c 6c65 6420 6279  lly installed by
-00001590: 2070 6970 290a 0a49 6e73 7461 6c6c 6174   pip)..Installat
-000015a0: 696f 6e0a 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ion.============
-000015b0: 0a0a 4375 7272 656e 7473 6361 7065 2063  ..Currentscape c
-000015c0: 616e 2062 6520 7069 7020 696e 7374 616c  an be pip instal
-000015d0: 6c65 6420 7769 7468 2074 6865 2066 6f6c  led with the fol
-000015e0: 6c6f 7769 6e67 2063 6f6d 6d61 6e64 3a0a  lowing command:.
-000015f0: 0a2e 2e20 636f 6465 2d62 6c6f 636b 3a3a  ... code-block::
-00001600: 2070 7974 686f 6e0a 0a20 2020 2070 6970   python..    pip
-00001610: 2069 6e73 7461 6c6c 2063 7572 7265 6e74   install current
-00001620: 7363 6170 650a 0a49 6620 796f 7520 7761  scape..If you wa
-00001630: 6e74 2074 6f20 6265 2061 626c 6520 746f  nt to be able to
-00001640: 2072 756e 2074 6865 2043 7572 7265 6e74   run the Current
-00001650: 7363 6170 6520 6578 616d 706c 6573 2c20  scape examples, 
-00001660: 796f 7520 7769 6c6c 206e 6565 6420 746f  you will need to
-00001670: 2061 6c73 6f20 696e 7374 616c 6c20 7468   also install th
-00001680: 6520 6578 616d 706c 6520 6465 7065 6e64  e example depend
-00001690: 656e 6369 6573 3a0a 0a2e 2e20 636f 6465  encies:.... code
-000016a0: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0a  -block:: python.
-000016b0: 0a20 2020 2070 6970 2069 6e73 7461 6c6c  .    pip install
-000016c0: 2063 7572 7265 6e74 7363 6170 655b 6578   currentscape[ex
-000016d0: 616d 706c 655d 0a0a 5175 6963 6b20 5374  ample]..Quick St
-000016e0: 6172 740a 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a  art.===========.
-000016f0: 0a42 656c 6f77 2069 7320 616e 2065 7861  .Below is an exa
-00001700: 6d70 6c65 206f 6620 6120 6261 6c6c 2061  mple of a ball a
-00001710: 6e64 2073 7469 636b 206d 6f64 656c 2069  nd stick model i
-00001720: 6e20 4e45 5552 4f4e 2077 6974 6820 7369  n NEURON with si
-00001730: 6d70 6c65 2048 6f64 676b 696e 2d48 7578  mple Hodgkin-Hux
-00001740: 6c65 7920 6d65 6368 616e 6973 6d73 2c20  ley mechanisms, 
-00001750: 746f 2077 6869 6368 2061 2073 7465 7020  to which a step 
-00001760: 7374 696d 756c 7573 2069 7320 6170 706c  stimulus is appl
-00001770: 6965 642e 0a0a 5468 6520 766f 6c74 6167  ied...The voltag
-00001780: 6520 616e 6420 696f 6e69 6320 6375 7272  e and ionic curr
-00001790: 656e 7473 2061 7265 2072 6563 6f72 6465  ents are recorde
-000017a0: 6420 616e 6420 6665 6420 746f 2043 7572  d and fed to Cur
-000017b0: 7265 6e74 7363 6170 652c 2061 6c6f 6e67  rentscape, along
-000017c0: 2077 6974 6820 6120 636f 6e66 6967 7572   with a configur
-000017d0: 6174 696f 6e20 6469 6374 696f 6e61 7279  ation dictionary
-000017e0: 2063 6f6e 7461 696e 696e 6720 7468 6520   containing the 
-000017f0: 6375 7272 656e 7420 6e61 6d65 7320 746f  current names to
-00001800: 2062 6520 6469 7370 6c61 7965 6420 696e   be displayed in
-00001810: 2074 6865 206c 6567 656e 642e 0a0a 546f   the legend...To
-00001820: 2072 756e 2074 6865 2063 6f64 6520 796f   run the code yo
-00001830: 7520 7769 6c6c 2066 6972 7374 2068 6176  u will first hav
-00001840: 6520 746f 2069 6e73 7461 6c6c 204e 4555  e to install NEU
-00001850: 524f 4e20 7061 636b 6167 653a 0a0a 2e2e  RON package:....
-00001860: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
-00001870: 7468 6f6e 0a0a 2020 2020 7069 7020 696e  thon..    pip in
-00001880: 7374 616c 6c20 6e65 7572 6f6e 0a0a 5768  stall neuron..Wh
-00001890: 656e 2079 6f75 2074 6865 6e20 6578 6563  en you then exec
-000018a0: 7574 6520 7468 6520 666f 6c6c 6f77 696e  ute the followin
-000018b0: 6720 7079 7468 6f6e 2063 6f64 652c 2061  g python code, a
-000018c0: 2077 696e 646f 7720 7368 6f75 6c64 206f   window should o
-000018d0: 7065 6e20 7769 7468 2074 6865 2063 7572  pen with the cur
-000018e0: 7265 6e74 7363 6170 6520 706c 6f74 3a0a  rentscape plot:.
-000018f0: 0a2e 2e20 636f 6465 2d62 6c6f 636b 3a3a  ... code-block::
-00001900: 2070 7974 686f 6e0a 0a20 2020 2069 6d70   python..    imp
-00001910: 6f72 7420 6e75 6d70 7920 6173 206e 700a  ort numpy as np.
-00001920: 2020 2020 6672 6f6d 206e 6575 726f 6e20      from neuron 
-00001930: 696d 706f 7274 2068 0a20 2020 2066 726f  import h.    fro
-00001940: 6d20 6e65 7572 6f6e 2e75 6e69 7473 2069  m neuron.units i
-00001950: 6d70 6f72 7420 6d73 2c20 6d56 0a20 2020  mport ms, mV.   
-00001960: 2066 726f 6d20 6375 7272 656e 7473 6361   from currentsca
-00001970: 7065 2e63 7572 7265 6e74 7363 6170 6520  pe.currentscape 
-00001980: 696d 706f 7274 2070 6c6f 745f 6375 7272  import plot_curr
-00001990: 656e 7473 6361 7065 0a0a 2020 2020 682e  entscape..    h.
-000019a0: 6c6f 6164 5f66 696c 6528 2773 7464 7275  load_file('stdru
-000019b0: 6e2e 686f 6327 290a 0a20 2020 2073 6f6d  n.hoc')..    som
-000019c0: 6120 3d20 682e 5365 6374 696f 6e28 6e61  a = h.Section(na
-000019d0: 6d65 3d27 736f 6d61 2729 0a20 2020 2064  me='soma').    d
-000019e0: 656e 6420 3d20 682e 5365 6374 696f 6e28  end = h.Section(
-000019f0: 6e61 6d65 3d27 6465 6e64 2729 0a0a 2020  name='dend')..  
-00001a00: 2020 6465 6e64 2e63 6f6e 6e65 6374 2873    dend.connect(s
-00001a10: 6f6d 6128 3129 290a 0a20 2020 2073 6f6d  oma(1))..    som
-00001a20: 612e 4c20 3d20 736f 6d61 2e64 6961 6d20  a.L = soma.diam 
-00001a30: 3d20 3132 2e36 3135 370a 2020 2020 6465  = 12.6157.    de
-00001a40: 6e64 2e4c 203d 2032 3030 0a20 2020 2064  nd.L = 200.    d
-00001a50: 656e 642e 6469 616d 203d 2031 0a0a 2020  end.diam = 1..  
-00001a60: 2020 666f 7220 7365 6320 696e 2068 2e61    for sec in h.a
-00001a70: 6c6c 7365 6328 293a 0a20 2020 2020 2020  llsec():.       
-00001a80: 2073 6563 2e52 6120 3d20 3130 3020 2020   sec.Ra = 100   
-00001a90: 2023 2041 7869 616c 2072 6573 6973 7461   # Axial resista
-00001aa0: 6e63 6520 696e 204f 686d 202a 2063 6d0a  nce in Ohm * cm.
-00001ab0: 2020 2020 2020 2020 7365 632e 636d 203d          sec.cm =
-00001ac0: 2031 2020 2020 2020 2320 4d65 6d62 7261   1      # Membra
-00001ad0: 6e65 2063 6170 6163 6974 616e 6365 2069  ne capacitance i
-00001ae0: 6e20 6d69 6372 6f20 4661 7261 6473 202f  n micro Farads /
-00001af0: 2063 6d5e 320a 0a20 2020 2023 2049 6e73   cm^2..    # Ins
-00001b00: 6572 7420 6163 7469 7665 2048 6f64 676b  ert active Hodgk
-00001b10: 696e 2d48 7578 6c65 7920 6375 7272 656e  in-Huxley curren
-00001b20: 7420 696e 2074 6865 2073 6f6d 610a 2020  t in the soma.  
-00001b30: 2020 736f 6d61 2e69 6e73 6572 7428 2768    soma.insert('h
-00001b40: 6827 290a 2020 2020 666f 7220 7365 6720  h').    for seg 
-00001b50: 696e 2073 6f6d 613a 0a20 2020 2020 2020  in soma:.       
-00001b60: 2073 6567 2e68 682e 676e 6162 6172 203d   seg.hh.gnabar =
-00001b70: 2030 2e31 3220 2023 2053 6f64 6975 6d20   0.12  # Sodium 
-00001b80: 636f 6e64 7563 7461 6e63 6520 696e 2053  conductance in S
-00001b90: 2f63 6d32 0a20 2020 2020 2020 2073 6567  /cm2.        seg
-00001ba0: 2e68 682e 676b 6261 7220 3d20 302e 3033  .hh.gkbar = 0.03
-00001bb0: 3620 2023 2050 6f74 6173 7369 756d 2063  6  # Potassium c
-00001bc0: 6f6e 6475 6374 616e 6365 2069 6e20 532f  onductance in S/
-00001bd0: 636d 320a 2020 2020 2020 2020 7365 672e  cm2.        seg.
-00001be0: 6868 2e67 6c20 3d20 302e 3030 3033 2020  hh.gl = 0.0003  
-00001bf0: 2020 2320 4c65 616b 2063 6f6e 6475 6374    # Leak conduct
-00001c00: 616e 6365 2069 6e20 532f 636d 320a 2020  ance in S/cm2.  
-00001c10: 2020 2020 2020 7365 672e 6868 2e65 6c20        seg.hh.el 
-00001c20: 3d20 2d35 342e 3320 2020 2020 2320 5265  = -54.3     # Re
-00001c30: 7665 7273 616c 2070 6f74 656e 7469 616c  versal potential
-00001c40: 2069 6e20 6d56 0a0a 2020 2020 2320 496e   in mV..    # In
-00001c50: 7365 7274 2070 6173 7369 7665 2063 7572  sert passive cur
-00001c60: 7265 6e74 2069 6e20 7468 6520 6465 6e64  rent in the dend
-00001c70: 7269 7465 0a20 2020 2064 656e 642e 696e  rite.    dend.in
-00001c80: 7365 7274 2827 7061 7327 290a 2020 2020  sert('pas').    
-00001c90: 666f 7220 7365 6720 696e 2064 656e 643a  for seg in dend:
-00001ca0: 0a20 2020 2020 2020 2073 6567 2e70 6173  .        seg.pas
-00001cb0: 2e67 203d 2030 2e30 3031 2020 2320 5061  .g = 0.001  # Pa
-00001cc0: 7373 6976 6520 636f 6e64 7563 7461 6e63  ssive conductanc
-00001cd0: 6520 696e 2053 2f63 6d32 0a20 2020 2020  e in S/cm2.     
-00001ce0: 2020 2073 6567 2e70 6173 2e65 203d 202d     seg.pas.e = -
-00001cf0: 3635 2020 2020 2320 4c65 616b 2072 6576  65    # Leak rev
-00001d00: 6572 7361 6c20 706f 7465 6e74 6961 6c20  ersal potential 
-00001d10: 6d56 0a0a 2020 2020 7374 696d 203d 2068  mV..    stim = h
-00001d20: 2e49 436c 616d 7028 6465 6e64 2831 2929  .IClamp(dend(1))
-00001d30: 0a20 2020 2073 7469 6d2e 6465 6c61 7920  .    stim.delay 
-00001d40: 3d20 350a 2020 2020 7374 696d 2e64 7572  = 5.    stim.dur
-00001d50: 203d 2031 300a 2020 2020 7374 696d 2e61   = 10.    stim.a
-00001d60: 6d70 203d 2030 2e31 0a0a 2020 2020 6375  mp = 0.1..    cu
-00001d70: 7272 656e 745f 6e61 6d65 7320 3d20 5b22  rrent_names = ["
-00001d80: 696b 222c 2022 696e 6122 2c20 2269 6c5f  ik", "ina", "il_
-00001d90: 6868 225d 0a20 2020 2074 5f76 6563 203d  hh"].    t_vec =
-00001da0: 2068 2e56 6563 746f 7228 290a 2020 2020   h.Vector().    
-00001db0: 765f 7665 6320 3d20 682e 5665 6374 6f72  v_vec = h.Vector
-00001dc0: 2829 0a20 2020 2069 6b5f 7665 6320 3d20  ().    ik_vec = 
-00001dd0: 682e 5665 6374 6f72 2829 0a20 2020 2069  h.Vector().    i
-00001de0: 6e61 5f76 6563 203d 2068 2e56 6563 746f  na_vec = h.Vecto
-00001df0: 7228 290a 2020 2020 696c 5f76 6563 203d  r().    il_vec =
-00001e00: 2068 2e56 6563 746f 7228 290a 2020 2020   h.Vector().    
-00001e10: 745f 7665 632e 7265 636f 7264 2868 2e5f  t_vec.record(h._
-00001e20: 7265 665f 7429 0a20 2020 2076 5f76 6563  ref_t).    v_vec
-00001e30: 2e72 6563 6f72 6428 736f 6d61 2830 2e35  .record(soma(0.5
-00001e40: 292e 5f72 6566 5f76 290a 2020 2020 696b  )._ref_v).    ik
-00001e50: 5f76 6563 2e72 6563 6f72 6428 736f 6d61  _vec.record(soma
-00001e60: 2830 2e35 292e 5f72 6566 5f69 6b29 0a20  (0.5)._ref_ik). 
-00001e70: 2020 2069 6e61 5f76 6563 2e72 6563 6f72     ina_vec.recor
-00001e80: 6428 736f 6d61 2830 2e35 292e 5f72 6566  d(soma(0.5)._ref
-00001e90: 5f69 6e61 290a 2020 2020 696c 5f76 6563  _ina).    il_vec
-00001ea0: 2e72 6563 6f72 6428 736f 6d61 2830 2e35  .record(soma(0.5
-00001eb0: 292e 5f72 6566 5f69 6c5f 6868 290a 0a20  )._ref_il_hh).. 
-00001ec0: 2020 2068 2e66 696e 6974 6961 6c69 7a65     h.finitialize
-00001ed0: 282d 3635 202a 206d 5629 0a20 2020 2068  (-65 * mV).    h
-00001ee0: 2e63 6f6e 7469 6e75 6572 756e 2832 3520  .continuerun(25 
-00001ef0: 2a20 6d73 290a 0a20 2020 2074 6f5f 7041  * ms)..    to_pA
-00001f00: 203d 2031 3020 2a20 736f 6d61 2830 2e35   = 10 * soma(0.5
-00001f10: 292e 6172 6561 2829 2023 2074 7572 6e20  ).area() # turn 
-00001f20: 6d41 2f63 6d32 2028 2a75 6d32 2920 696e  mA/cm2 (*um2) in
-00001f30: 746f 2070 410a 2020 2020 766f 6c74 6167  to pA.    voltag
-00001f40: 6520 3d20 6e70 2e61 7361 7272 6179 2876  e = np.asarray(v
-00001f50: 5f76 6563 290a 2020 2020 706f 7461 7373  _vec).    potass
-00001f60: 6975 6d20 3d20 6e70 2e61 7361 7272 6179  ium = np.asarray
-00001f70: 2869 6b5f 7665 6329 202a 2074 6f5f 7041  (ik_vec) * to_pA
-00001f80: 0a20 2020 2073 6f64 6975 6d20 3d20 6e70  .    sodium = np
-00001f90: 2e61 7361 7272 6179 2869 6e61 5f76 6563  .asarray(ina_vec
-00001fa0: 2920 2a20 746f 5f70 410a 2020 2020 6c65  ) * to_pA.    le
-00001fb0: 616b 203d 206e 702e 6173 6172 7261 7928  ak = np.asarray(
-00001fc0: 696c 5f76 6563 2920 2a20 746f 5f70 410a  il_vec) * to_pA.
-00001fd0: 0a20 2020 2063 6f6e 6669 6720 3d20 7b0a  .    config = {.
-00001fe0: 2020 2020 2020 2020 226f 7574 7075 7422          "output"
-00001ff0: 3a20 7b20 2020 2020 2020 2020 2020 2020  : {             
-00002000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002030: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00002040: 2020 2273 6176 6566 6967 223a 2054 7275    "savefig": Tru
-00002050: 652c 2020 2020 2020 2020 2020 2020 2020  e,              
-00002060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002080: 2020 2020 2020 2020 2020 2020 200a 2020               .  
-00002090: 2020 2020 2020 2020 2264 6972 223a 2022          "dir": "
-000020a0: 2e22 2c20 2020 2020 2020 2020 2020 2020  .",             
-000020b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020e0: 2020 200a 2020 2020 2020 2020 2020 2266     .          "f
-000020f0: 6e61 6d65 223a 2022 7175 6963 6b73 7461  name": "quicksta
-00002100: 7274 5f70 6c6f 7422 2c20 2020 2020 2020  rt_plot",       
-00002110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002130: 2020 2020 2020 2020 200a 2020 2020 2020           .      
-00002140: 2020 2020 2265 7874 656e 7369 6f6e 223a      "extension":
-00002150: 2022 706e 6722 2c20 2020 2020 2020 2020   "png",         
-00002160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002180: 2020 2020 2020 2020 2020 2020 2020 200a                 .
-00002190: 2020 2020 2020 2020 2020 2264 7069 223a            "dpi":
-000021a0: 2033 3030 2c20 2020 2020 2020 2020 2020   300,           
-000021b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021e0: 2020 2020 200a 2020 2020 2020 2020 2020       .          
-000021f0: 2274 7261 6e73 7061 7265 6e74 223a 2046  "transparent": F
-00002200: 616c 7365 2020 2020 2020 2020 2020 2020  alse            
-00002210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002230: 2020 2020 2020 2020 2020 200a 2020 2020             .    
-00002240: 2020 2020 7d2c 2020 200a 2020 2020 2020      },   .      
-00002250: 2020 2263 7572 7265 6e74 223a 207b 226e    "current": {"n
-00002260: 616d 6573 223a 2063 7572 7265 6e74 5f6e  ames": current_n
-00002270: 616d 6573 7d2c 0a20 2020 2020 2020 2022  ames},.        "
-00002280: 766f 6c74 6167 6522 3a20 7b22 796c 696d  voltage": {"ylim
-00002290: 223a 205b 2d39 302c 2035 305d 7d2c 0a20  ": [-90, 50]},. 
-000022a0: 2020 2020 2020 2022 6c65 6765 6e64 7465         "legendte
-000022b0: 7874 7369 7a65 223a 2035 2c0a 2020 2020  xtsize": 5,.    
-000022c0: 7d0a 2020 2020 6669 6720 3d20 706c 6f74  }.    fig = plot
-000022d0: 5f63 7572 7265 6e74 7363 6170 6528 766f  _currentscape(vo
-000022e0: 6c74 6167 652c 205b 706f 7461 7373 6975  ltage, [potassiu
-000022f0: 6d2c 2073 6f64 6975 6d2c 206c 6561 6b5d  m, sodium, leak]
-00002300: 2c20 636f 6e66 6967 290a 2020 2020 6669  , config).    fi
-00002310: 672e 7368 6f77 2829 0a0a 5768 656e 2079  g.show()..When y
-00002320: 6f75 2072 756e 2074 6869 7320 636f 6465  ou run this code
-00002330: 2069 6e20 5079 7468 6f6e 2c20 6974 2077   in Python, it w
-00002340: 696c 6c20 6765 6e65 7261 7465 2074 6865  ill generate the
-00002350: 2066 6f6c 6c6f 7769 6e67 2063 7572 7265   following curre
-00002360: 6e74 7363 6170 6520 706c 6f74 2028 696e  ntscape plot (in
-00002370: 2061 2077 696e 646f 772c 2061 6e64 206f   a window, and o
-00002380: 6e20 6469 736b 2061 7320 7175 6963 6b73  n disk as quicks
-00002390: 7461 7274 5f70 6c6f 742e 706e 6729 3a0a  tart_plot.png):.
-000023a0: 0a2e 2e20 696d 6167 653a 3a20 646f 632f  ... image:: doc/
-000023b0: 736f 7572 6365 2f69 6d61 6765 732f 7175  source/images/qu
-000023c0: 6963 6b73 7461 7274 5f70 6c6f 742e 706e  ickstart_plot.pn
-000023d0: 670a 0a54 7574 6f72 6961 6c0a 3d3d 3d3d  g..Tutorial.====
-000023e0: 3d3d 3d3d 0a0a 4120 6d6f 7265 2064 6574  ====..A more det
-000023f0: 6169 6c65 6420 6578 706c 616e 6174 696f  ailed explanatio
-00002400: 6e20 6f6e 2068 6f77 2074 6f20 7573 6520  n on how to use 
-00002410: 4375 7272 656e 7473 6361 7065 2c20 6173  Currentscape, as
-00002420: 2077 656c 6c20 6173 206f 7468 6572 2065   well as other e
-00002430: 7861 6d70 6c65 7320 6361 6e20 6265 2066  xamples can be f
-00002440: 6f75 6e64 206f 6e20 7468 6520 6074 7574  ound on the `tut
-00002450: 6f72 6961 6c20 7061 6765 203c 5475 746f  orial page <Tuto
-00002460: 7269 616c 2e72 7374 3e60 5f2e 0a0a 4150  rial.rst>`_...AP
-00002470: 4920 446f 6375 6d65 6e74 6174 696f 6e0a  I Documentation.
-00002480: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00002490: 3d0a 0a54 6865 2041 5049 2064 6f63 756d  =..The API docum
-000024a0: 656e 7461 7469 6f6e 2063 616e 2062 6520  entation can be 
-000024b0: 666f 756e 6420 6f6e 2060 5265 6164 5468  found on `ReadTh
-000024c0: 6544 6f63 7320 3c22 6874 7470 733a 2f2f  eDocs <"https://
-000024d0: 6375 7272 656e 7473 6361 7065 2e72 6561  currentscape.rea
-000024e0: 6474 6865 646f 6373 2e69 6f22 3e60 5f2e  dthedocs.io">`_.
-000024f0: 0a0a 4675 6e64 696e 6720 2620 4163 6b6e  ..Funding & Ackn
-00002500: 6f77 6c65 6467 656d 656e 7473 0a3d 3d3d  owledgements.===
-00002510: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00002520: 3d3d 3d3d 3d3d 3d0a 0a57 6520 7769 7368  =======..We wish
-00002530: 2074 6f20 7468 616e 6b20 7468 6520 6175   to thank the au
-00002540: 7468 6f72 7320 6f66 2060 416c 6f6e 736f  thors of `Alonso
-00002550: 2061 6e64 204d 6172 6465 722c 2032 3031   and Marder, 201
-00002560: 3920 3c68 7474 7073 3a2f 2f64 6f69 2e6f  9 <https://doi.o
-00002570: 7267 2f31 302e 3735 3534 2f65 4c69 6665  rg/10.7554/eLife
-00002580: 2e34 3237 3232 3e60 5f20 746f 206c 6574  .42722>`_ to let
-00002590: 2075 7320 696e 7465 6772 6174 6520 6120   us integrate a 
-000025a0: 7061 7274 206f 6620 7468 6569 7220 6063  part of their `c
-000025b0: 6f64 6520 3c68 7474 7073 3a2f 2f64 6174  ode <https://dat
-000025c0: 6164 7279 6164 2e6f 7267 2f73 7461 7368  adryad.org/stash
-000025d0: 2f64 6174 6173 6574 2f64 6f69 3a31 302e  /dataset/doi:10.
-000025e0: 3530 3631 2f64 7279 6164 2e64 3037 3739  5061/dryad.d0779
-000025f0: 6d62 3e60 5f20 696e 746f 2074 6869 7320  mb>`_ into this 
-00002600: 7265 706f 7369 746f 7279 2e0a 0a54 6865  repository...The
-00002610: 2070 6172 7420 6f66 2074 6865 2063 6f64   part of the cod
-00002620: 6520 696e 2074 6869 7320 7265 706f 7369  e in this reposi
-00002630: 746f 7279 2064 6576 656c 6f70 6564 2062  tory developed b
-00002640: 7920 7468 6520 4550 464c 2042 6c75 6520  y the EPFL Blue 
-00002650: 4272 6169 6e20 5072 6f6a 6563 7420 7761  Brain Project wa
-00002660: 7320 7375 7070 6f72 7465 6420 6279 2066  s supported by f
-00002670: 756e 6469 6e67 2074 6f20 7468 6520 426c  unding to the Bl
-00002680: 7565 2042 7261 696e 2050 726f 6a65 6374  ue Brain Project
-00002690: 2c20 6120 7265 7365 6172 6368 2063 656e  , a research cen
-000026a0: 7465 7220 6f66 2074 6865 20c3 8963 6f6c  ter of the ..col
-000026b0: 6520 706f 6c79 7465 6368 6e69 7175 6520  e polytechnique 
-000026c0: 66c3 a964 c3a9 7261 6c65 2064 6520 4c61  f..d..rale de La
-000026d0: 7573 616e 6e65 2028 4550 464c 292c 2066  usanne (EPFL), f
-000026e0: 726f 6d20 7468 6520 5377 6973 7320 676f  rom the Swiss go
-000026f0: 7665 726e 6d65 6e74 2773 2045 5448 2042  vernment's ETH B
-00002700: 6f61 7264 206f 6620 7468 6520 5377 6973  oard of the Swis
-00002710: 7320 4665 6465 7261 6c20 496e 7374 6974  s Federal Instit
-00002720: 7574 6573 206f 6620 5465 6368 6e6f 6c6f  utes of Technolo
-00002730: 6779 2e0a                                gy..
+000003a0: 742f 782d 7273 740a 5072 6f76 6964 6573  t/x-rst.Provides
+000003b0: 2d45 7874 7261 3a20 646f 6373 0a50 726f  -Extra: docs.Pro
+000003c0: 7669 6465 732d 4578 7472 613a 2065 7861  vides-Extra: exa
+000003d0: 6d70 6c65 0a4c 6963 656e 7365 2d46 696c  mple.License-Fil
+000003e0: 653a 204c 4943 454e 5345 2e74 7874 0a4c  e: LICENSE.txt.L
+000003f0: 6963 656e 7365 2d46 696c 653a 2043 4f50  icense-File: COP
+00000400: 5949 4e47 0a4c 6963 656e 7365 2d46 696c  YING.License-Fil
+00000410: 653a 2041 5554 484f 5253 2e72 7374 0a0a  e: AUTHORS.rst..
+00000420: 4375 7272 656e 7473 6361 7065 0a3d 3d3d  Currentscape.===
+00000430: 3d3d 3d3d 3d3d 3d3d 3d0a 0a0a 2b2d 2d2d  =========...+---
+00000440: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+00000450: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 4c61  ----------+.| La
+00000460: 7465 7374 2052 656c 6561 7365 207c 207c  test Release | |
+00000470: 7079 7069 7c20 2020 2020 7c0a 2b2d 2d2d  pypi|     |.+---
+00000480: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+00000490: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 446f  ----------+.| Do
+000004a0: 6375 6d65 6e74 6174 696f 6e20 207c 207c  cumentation  | |
+000004b0: 646f 6373 7c20 2020 2020 7c0a 2b2d 2d2d  docs|     |.+---
+000004c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+000004d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 4c69  ----------+.| Li
+000004e0: 6365 6e73 6520 2020 2020 2020 207c 207c  cense        | |
+000004f0: 6c69 6365 6e73 657c 2020 7c0a 2b2d 2d2d  license|  |.+---
+00000500: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+00000510: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 4275  ----------+.| Bu
+00000520: 696c 6420 5374 6174 7573 2009 207c 207c  ild Status . | |
+00000530: 6275 696c 647c 2020 2020 7c0a 2b2d 2d2d  build|    |.+---
+00000540: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+00000550: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 436f  ----------+.| Co
+00000560: 7665 7261 6765 2020 2020 2020 207c 207c  verage       | |
+00000570: 636f 7665 7261 6765 7c20 7c0a 2b2d 2d2d  coverage| |.+---
+00000580: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+00000590: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 4769  ----------+.| Gi
+000005a0: 7474 6572 2020 2020 2020 2020 207c 207c  tter         | |
+000005b0: 6769 7474 6572 7c20 2020 7c0a 2b2d 2d2d  gitter|   |.+---
+000005c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+000005d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 0a49 6e74  ----------+..Int
+000005e0: 726f 6475 6374 696f 6e0a 3d3d 3d3d 3d3d  roduction.======
+000005f0: 3d3d 3d3d 3d3d 0a0a 4375 7272 656e 7473  ======..Currents
+00000600: 6361 7065 2069 7320 6120 5079 7468 6f6e  cape is a Python
+00000610: 2074 6f6f 6c20 656e 6162 6c69 6e67 2073   tool enabling s
+00000620: 6369 656e 7469 7374 7320 746f 2065 6173  cientists to eas
+00000630: 696c 7920 706c 6f74 2074 6865 2063 7572  ily plot the cur
+00000640: 7265 6e74 7320 696e 2065 6c65 6374 7269  rents in electri
+00000650: 6361 6c20 6e65 7572 6f6e 206d 6f64 656c  cal neuron model
+00000660: 732e 0a54 6865 2063 6f64 6520 6973 2062  s..The code is b
+00000670: 6173 6564 206f 6e20 7468 6520 7061 7065  ased on the pape
+00000680: 7220 6041 6c6f 6e73 6f20 616e 6420 4d61  r `Alonso and Ma
+00000690: 7264 6572 2c20 3230 3139 203c 6874 7470  rder, 2019 <http
+000006a0: 733a 2f2f 646f 692e 6f72 672f 3130 2e37  s://doi.org/10.7
+000006b0: 3535 342f 654c 6966 652e 3432 3732 323e  554/eLife.42722>
+000006c0: 605f 5f2e 0a0a 4375 7272 656e 7473 6361  `__...Currentsca
+000006d0: 7065 2066 6967 7572 6573 2070 6c6f 7420  pe figures plot 
+000006e0: 7468 6520 7065 7263 656e 7461 6765 206f  the percentage o
+000006f0: 6620 696e 7761 7264 2061 6e64 206f 7574  f inward and out
+00000700: 7761 7264 2069 6f6e 6963 206d 656d 6272  ward ionic membr
+00000710: 616e 6520 6375 7272 656e 7473 2c0a 7468  ane currents,.th
+00000720: 6520 746f 7461 6c20 696e 7761 7264 2061  e total inward a
+00000730: 6e64 206f 7574 7761 7264 2063 7572 7265  nd outward curre
+00000740: 6e74 732c 2061 7320 7765 6c6c 2061 7320  nts, as well as 
+00000750: 7468 6520 766f 6c74 6167 6520 696e 2066  the voltage in f
+00000760: 756e 6374 696f 6e20 6f66 2074 696d 652e  unction of time.
+00000770: 0a49 7420 616c 6c6f 7773 206d 6f64 656c  .It allows model
+00000780: 6c65 7273 2074 6f20 7365 6520 7768 6963  lers to see whic
+00000790: 6820 6375 7272 656e 7473 2070 6c61 7920  h currents play 
+000007a0: 6120 726f 6c65 2061 7420 616e 7920 6769  a role at any gi
+000007b0: 7665 6e20 7469 6d65 2064 7572 696e 6720  ven time during 
+000007c0: 6120 7369 6d75 6c61 7469 6f6e 2c20 616e  a simulation, an
+000007d0: 6420 6368 6563 6b20 696e 2064 6570 7468  d check in depth
+000007e0: 2074 6865 2063 7572 7265 6e74 2064 796e   the current dyn
+000007f0: 616d 6963 732e 0a0a 2e2e 2069 6d61 6765  amics..... image
+00000800: 3a3a 2064 6f63 2f73 6f75 7263 652f 696d  :: doc/source/im
+00000810: 6167 6573 2f70 6c6f 742e 706e 670a 0a43  ages/plot.png..C
+00000820: 6974 6174 696f 6e0a 3d3d 3d3d 3d3d 3d3d  itation.========
+00000830: 0a0a 5768 656e 2079 6f75 2075 7365 2074  ..When you use t
+00000840: 6869 7320 4375 7272 656e 7473 6361 7065  his Currentscape
+00000850: 2073 6f66 7477 6172 6520 666f 7220 796f   software for yo
+00000860: 7572 2072 6573 6561 7263 682c 2077 6520  ur research, we 
+00000870: 6173 6b20 796f 7520 746f 2063 6974 6520  ask you to cite 
+00000880: 7468 6520 666f 6c6c 6f77 696e 6720 7075  the following pu
+00000890: 626c 6963 6174 696f 6e20 2874 6869 7320  blication (this 
+000008a0: 696e 636c 7564 6573 2070 6f73 7465 7220  includes poster 
+000008b0: 7072 6573 656e 7461 7469 6f6e 7329 3a0a  presentations):.
+000008c0: 0a2e 2e20 636f 6465 2d62 6c6f 636b 3a3a  ... code-block::
+000008d0: 200a 0a20 2020 2040 6172 7469 636c 6520   ..    @article 
+000008e0: 7b31 302e 3735 3534 2f65 4c69 6665 2e34  {10.7554/eLife.4
+000008f0: 3237 3232 2c0a 2020 2020 6172 7469 636c  2722,.    articl
+00000900: 655f 7479 7065 203d 207b 6a6f 7572 6e61  e_type = {journa
+00000910: 6c7d 2c0a 2020 2020 7469 746c 6520 3d20  l},.    title = 
+00000920: 7b56 6973 7561 6c69 7a61 7469 6f6e 206f  {Visualization o
+00000930: 6620 6375 7272 656e 7473 2069 6e20 6e65  f currents in ne
+00000940: 7572 616c 206d 6f64 656c 7320 7769 7468  ural models with
+00000950: 2073 696d 696c 6172 2062 6568 6176 696f   similar behavio
+00000960: 7220 616e 6420 6469 6666 6572 656e 7420  r and different 
+00000970: 636f 6e64 7563 7461 6e63 6520 6465 6e73  conductance dens
+00000980: 6974 6965 737d 2c0a 2020 2020 6175 7468  ities},.    auth
+00000990: 6f72 203d 207b 416c 6f6e 736f 2c20 4c65  or = {Alonso, Le
+000009a0: 616e 6472 6f20 4d20 616e 6420 4d61 7264  andro M and Mard
+000009b0: 6572 2c20 4576 657d 2c0a 2020 2020 6564  er, Eve},.    ed
+000009c0: 6974 6f72 203d 207b 5765 7374 6272 6f6f  itor = {Westbroo
+000009d0: 6b2c 2047 6172 7920 4c20 616e 6420 536b  k, Gary L and Sk
+000009e0: 696e 6e65 722c 2046 7261 6e63 6573 204b  inner, Frances K
+000009f0: 2061 6e64 204c 616e 6b61 7261 6e79 2c20   and Lankarany, 
+00000a00: 4d69 6c61 6420 616e 6420 4272 6974 746f  Milad and Britto
+00000a10: 6e2c 204f 6c69 7665 727d 2c0a 2020 2020  n, Oliver},.    
+00000a20: 766f 6c75 6d65 203d 2038 2c0a 2020 2020  volume = 8,.    
+00000a30: 7965 6172 203d 2032 3031 392c 0a20 2020  year = 2019,.   
+00000a40: 206d 6f6e 7468 203d 207b 6a61 6e7d 2c0a   month = {jan},.
+00000a50: 2020 2020 7075 625f 6461 7465 203d 207b      pub_date = {
+00000a60: 3230 3139 2d30 312d 3331 7d2c 0a20 2020  2019-01-31},.   
+00000a70: 2070 6167 6573 203d 207b 6534 3237 3232   pages = {e42722
+00000a80: 7d2c 0a20 2020 2063 6974 6174 696f 6e20  },.    citation 
+00000a90: 3d20 7b65 4c69 6665 2032 3031 393b 383a  = {eLife 2019;8:
+00000aa0: 6534 3237 3232 7d2c 0a20 2020 2064 6f69  e42722},.    doi
+00000ab0: 203d 207b 3130 2e37 3535 342f 654c 6966   = {10.7554/eLif
+00000ac0: 652e 3432 3732 327d 2c0a 2020 2020 7572  e.42722},.    ur
+00000ad0: 6c20 3d20 7b68 7474 7073 3a2f 2f64 6f69  l = {https://doi
+00000ae0: 2e6f 7267 2f31 302e 3735 3534 2f65 4c69  .org/10.7554/eLi
+00000af0: 6665 2e34 3237 3232 7d2c 0a20 2020 2061  fe.42722},.    a
+00000b00: 6273 7472 6163 7420 3d20 7b43 6f6e 6475  bstract = {Condu
+00000b10: 6374 616e 6365 2d62 6173 6564 206d 6f64  ctance-based mod
+00000b20: 656c 7320 6f66 206e 6575 7261 6c20 6163  els of neural ac
+00000b30: 7469 7669 7479 2070 726f 6475 6365 206c  tivity produce l
+00000b40: 6172 6765 2061 6d6f 756e 7473 206f 6620  arge amounts of 
+00000b50: 6461 7461 2074 6861 7420 6361 6e20 6265  data that can be
+00000b60: 2068 6172 6420 746f 2076 6973 7561 6c69   hard to visuali
+00000b70: 7a65 2061 6e64 2069 6e74 6572 7072 6574  ze and interpret
+00000b80: 2e20 5765 2069 6e74 726f 6475 6365 2076  . We introduce v
+00000b90: 6973 7561 6c69 7a61 7469 6f6e 206d 6574  isualization met
+00000ba0: 686f 6473 2074 6f20 6469 7370 6c61 7920  hods to display 
+00000bb0: 7468 6520 6479 6e61 6d69 6373 206f 6620  the dynamics of 
+00000bc0: 7468 6520 696f 6e69 6320 6375 7272 656e  the ionic curren
+00000bd0: 7473 2061 6e64 2074 6f20 6469 7370 6c61  ts and to displa
+00000be0: 7920 7468 6520 6d6f 6465 6c73 e280 9920  y the models... 
+00000bf0: 7265 7370 6f6e 7365 2074 6f20 7065 7274  response to pert
+00000c00: 7572 6261 7469 6f6e 732e 2054 6f20 7669  urbations. To vi
+00000c10: 7375 616c 697a 6520 7468 6520 6375 7272  sualize the curr
+00000c20: 656e 7473 e280 9920 6479 6e61 6d69 6373  ents... dynamics
+00000c30: 2c20 7765 2063 6f6d 7075 7465 2074 6865  , we compute the
+00000c40: 2070 6572 6365 6e74 2063 6f6e 7472 6962   percent contrib
+00000c50: 7574 696f 6e20 6f66 2065 6163 6820 6375  ution of each cu
+00000c60: 7272 656e 7420 616e 6420 6469 7370 6c61  rrent and displa
+00000c70: 7920 7468 656d 206f 7665 7220 7469 6d65  y them over time
+00000c80: 2075 7369 6e67 2073 7461 636b 6564 2d61   using stacked-a
+00000c90: 7265 6120 706c 6f74 732e 2054 6865 2077  rea plots. The w
+00000ca0: 6176 6566 6f72 6d20 6f66 2074 6865 206d  aveform of the m
+00000cb0: 656d 6272 616e 6520 706f 7465 6e74 6961  embrane potentia
+00000cc0: 6c20 616e 6420 7468 6520 636f 6e74 7269  l and the contri
+00000cd0: 6275 7469 6f6e 206f 6620 6561 6368 2063  bution of each c
+00000ce0: 7572 7265 6e74 2063 6861 6e67 6520 6173  urrent change as
+00000cf0: 2074 6865 206d 6f64 656c 7320 6172 6520   the models are 
+00000d00: 7065 7274 7572 6265 642e 2054 6f20 7265  perturbed. To re
+00000d10: 7072 6573 656e 7420 7468 6573 6520 6368  present these ch
+00000d20: 616e 6765 7320 6f76 6572 2061 2072 616e  anges over a ran
+00000d30: 6765 206f 6620 7468 6520 7065 7274 7572  ge of the pertur
+00000d40: 6261 7469 6f6e 2063 6f6e 7472 6f6c 2070  bation control p
+00000d50: 6172 616d 6574 6572 2c20 7765 2063 6f6d  arameter, we com
+00000d60: 7075 7465 2061 6e64 2064 6973 706c 6179  pute and display
+00000d70: 2074 6865 2064 6973 7472 6962 7574 696f   the distributio
+00000d80: 6e73 206f 6620 7468 6573 6520 7761 7665  ns of these wave
+00000d90: 666f 726d 732e 2057 6520 696c 6c75 7374  forms. We illust
+00000da0: 7261 7465 2074 6865 7365 2070 726f 6365  rate these proce
+00000db0: 6475 7265 7320 696e 2073 6978 2065 7861  dures in six exa
+00000dc0: 6d70 6c65 7320 6f66 2062 7572 7374 696e  mples of burstin
+00000dd0: 6720 6d6f 6465 6c20 6e65 7572 6f6e 7320  g model neurons 
+00000de0: 7769 7468 2073 696d 696c 6172 2061 6374  with similar act
+00000df0: 6976 6974 7920 6275 7420 7468 6174 2064  ivity but that d
+00000e00: 6966 6665 7220 6173 206d 7563 6820 6173  iffer as much as
+00000e10: 2074 6872 6565 666f 6c64 2069 6e20 7468   threefold in th
+00000e20: 6569 7220 636f 6e64 7563 7461 6e63 6520  eir conductance 
+00000e30: 6465 6e73 6974 6965 732e 2054 6865 7365  densities. These
+00000e40: 2076 6973 7561 6c69 7a61 7469 6f6e 206d   visualization m
+00000e50: 6574 686f 6473 2070 726f 7669 6465 2068  ethods provide h
+00000e60: 6575 7269 7374 6963 2069 6e73 6967 6874  euristic insight
+00000e70: 2069 6e74 6f20 7768 7920 696e 6469 7669   into why indivi
+00000e80: 6475 616c 206e 6575 726f 6e73 206f 7220  dual neurons or 
+00000e90: 6e65 7477 6f72 6b73 2077 6974 6820 7369  networks with si
+00000ea0: 6d69 6c61 7220 6265 6861 7669 6f72 2063  milar behavior c
+00000eb0: 616e 2072 6573 706f 6e64 2077 6964 656c  an respond widel
+00000ec0: 7920 6469 6666 6572 656e 746c 7920 746f  y differently to
+00000ed0: 2070 6572 7475 7262 6174 696f 6e73 2e7d   perturbations.}
+00000ee0: 2c0a 2020 2020 6b65 7977 6f72 6473 203d  ,.    keywords =
+00000ef0: 207b 6e65 7572 6f6e 616c 206f 7363 696c   {neuronal oscil
+00000f00: 6c61 746f 7273 2c20 4e61 2b20 6368 616e  lators, Na+ chan
+00000f10: 6e65 6c73 2c20 4361 2b2b 2063 6861 6e6e  nels, Ca++ chann
+00000f20: 656c 732c 204b 2b20 6368 616e 6e65 6c73  els, K+ channels
+00000f30: 2c20 636f 6e64 7563 7461 6e63 652d 6261  , conductance-ba
+00000f40: 7365 642c 2069 6f6e 6963 2063 6861 6e6e  sed, ionic chann
+00000f50: 656c 737d 2c0a 2020 2020 6a6f 7572 6e61  els},.    journa
+00000f60: 6c20 3d20 7b65 4c69 6665 7d2c 0a20 2020  l = {eLife},.   
+00000f70: 2069 7373 6e20 3d20 7b32 3035 302d 3038   issn = {2050-08
+00000f80: 3458 7d2c 0a20 2020 2070 7562 6c69 7368  4X},.    publish
+00000f90: 6572 203d 207b 654c 6966 6520 5363 6965  er = {eLife Scie
+00000fa0: 6e63 6573 2050 7562 6c69 6361 7469 6f6e  nces Publication
+00000fb0: 732c 204c 7464 7d2c 0a20 2020 207d 0a0a  s, Ltd},.    }..
+00000fc0: 5375 7070 6f72 740a 3d3d 3d3d 3d3d 3d0a  Support.=======.
+00000fd0: 0a57 6520 6172 6520 7072 6f76 6964 696e  .We are providin
+00000fe0: 6720 7375 7070 6f72 7420 6f6e 2060 4769  g support on `Gi
+00000ff0: 7474 6572 203c 6874 7470 733a 2f2f 6769  tter <https://gi
+00001000: 7474 6572 2e69 6d2f 426c 7565 4272 6169  tter.im/BlueBrai
+00001010: 6e2f 4375 7272 656e 7473 6361 7065 3e60  n/Currentscape>`
+00001020: 5f2e 2057 6520 7375 6767 6573 7420 796f  _. We suggest yo
+00001030: 7520 6372 6561 7465 2074 6963 6b65 7473  u create tickets
+00001040: 206f 6e20 7468 6520 6047 6974 6875 6220   on the `Github 
+00001050: 6973 7375 6520 7472 6163 6b65 7220 3c68  issue tracker <h
+00001060: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001070: 6d2f 426c 7565 4272 6169 6e2f 4375 7272  m/BlueBrain/Curr
+00001080: 656e 7473 6361 7065 2f69 7373 7565 733e  entscape/issues>
+00001090: 605f 2069 6e20 6361 7365 2079 6f75 2065  `_ in case you e
+000010a0: 6e63 6f75 6e74 6572 2070 726f 626c 656d  ncounter problem
+000010b0: 7320 7768 696c 6520 7573 696e 6720 7468  s while using th
+000010c0: 6520 736f 6674 7761 7265 206f 7220 6966  e software or if
+000010d0: 2079 6f75 2068 6176 6520 736f 6d65 2073   you have some s
+000010e0: 7567 6765 7374 696f 6e73 2e0a 0a4d 6169  uggestions...Mai
+000010f0: 6e20 6465 7065 6e64 656e 6369 6573 0a3d  n dependencies.=
+00001100: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00001110: 0a0a 2d20 6050 7974 686f 6e20 332e 372b  ..- `Python 3.7+
+00001120: 203c 6874 7470 733a 2f2f 7777 772e 7079   <https://www.py
+00001130: 7468 6f6e 2e6f 7267 2f64 6f77 6e6c 6f61  thon.org/downloa
+00001140: 6473 2f72 656c 6561 7365 2f70 7974 686f  ds/release/pytho
+00001150: 6e2d 3337 302f 3e60 5f0a 2d20 604e 756d  n-370/>`_.- `Num
+00001160: 7079 203c 6874 7470 733a 2f2f 6e75 6d70  py <https://nump
+00001170: 792e 6f72 672f 3e60 5f20 2861 7574 6f6d  y.org/>`_ (autom
+00001180: 6174 6963 616c 6c79 2069 6e73 7461 6c6c  atically install
+00001190: 6564 2062 7920 7069 7029 0a2d 2060 5061  ed by pip).- `Pa
+000011a0: 6c65 7474 6162 6c65 203c 6874 7470 733a  lettable <https:
+000011b0: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 6966  //github.com/jif
+000011c0: 6679 636c 7562 2f70 616c 6574 7461 626c  fyclub/palettabl
+000011d0: 653e 605f 2028 6175 746f 6d61 7469 6361  e>`_ (automatica
+000011e0: 6c6c 7920 696e 7374 616c 6c65 6420 6279  lly installed by
+000011f0: 2070 6970 290a 0a49 6e73 7461 6c6c 6174   pip)..Installat
+00001200: 696f 6e0a 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ion.============
+00001210: 0a0a 4375 7272 656e 7473 6361 7065 2063  ..Currentscape c
+00001220: 616e 2062 6520 7069 7020 696e 7374 616c  an be pip instal
+00001230: 6c65 6420 7769 7468 2074 6865 2066 6f6c  led with the fol
+00001240: 6c6f 7769 6e67 2063 6f6d 6d61 6e64 3a0a  lowing command:.
+00001250: 0a2e 2e20 636f 6465 2d62 6c6f 636b 3a3a  ... code-block::
+00001260: 2070 7974 686f 6e0a 0a20 2020 2070 6970   python..    pip
+00001270: 2069 6e73 7461 6c6c 2063 7572 7265 6e74   install current
+00001280: 7363 6170 650a 0a49 6620 796f 7520 7761  scape..If you wa
+00001290: 6e74 2074 6f20 6265 2061 626c 6520 746f  nt to be able to
+000012a0: 2072 756e 2074 6865 2043 7572 7265 6e74   run the Current
+000012b0: 7363 6170 6520 6578 616d 706c 6573 2c20  scape examples, 
+000012c0: 796f 7520 7769 6c6c 206e 6565 6420 746f  you will need to
+000012d0: 2061 6c73 6f20 696e 7374 616c 6c20 7468   also install th
+000012e0: 6520 6578 616d 706c 6520 6465 7065 6e64  e example depend
+000012f0: 656e 6369 6573 3a0a 0a2e 2e20 636f 6465  encies:.... code
+00001300: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0a  -block:: python.
+00001310: 0a20 2020 2070 6970 2069 6e73 7461 6c6c  .    pip install
+00001320: 2063 7572 7265 6e74 7363 6170 655b 6578   currentscape[ex
+00001330: 616d 706c 655d 0a0a 5175 6963 6b20 5374  ample]..Quick St
+00001340: 6172 740a 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a  art.===========.
+00001350: 0a42 656c 6f77 2069 7320 616e 2065 7861  .Below is an exa
+00001360: 6d70 6c65 206f 6620 6120 6261 6c6c 2061  mple of a ball a
+00001370: 6e64 2073 7469 636b 206d 6f64 656c 2069  nd stick model i
+00001380: 6e20 4e45 5552 4f4e 2077 6974 6820 7369  n NEURON with si
+00001390: 6d70 6c65 2048 6f64 676b 696e 2d48 7578  mple Hodgkin-Hux
+000013a0: 6c65 7920 6d65 6368 616e 6973 6d73 2c20  ley mechanisms, 
+000013b0: 746f 2077 6869 6368 2061 2073 7465 7020  to which a step 
+000013c0: 7374 696d 756c 7573 2069 7320 6170 706c  stimulus is appl
+000013d0: 6965 642e 0a0a 5468 6520 766f 6c74 6167  ied...The voltag
+000013e0: 6520 616e 6420 696f 6e69 6320 6375 7272  e and ionic curr
+000013f0: 656e 7473 2061 7265 2072 6563 6f72 6465  ents are recorde
+00001400: 6420 616e 6420 6665 6420 746f 2043 7572  d and fed to Cur
+00001410: 7265 6e74 7363 6170 652c 2061 6c6f 6e67  rentscape, along
+00001420: 2077 6974 6820 6120 636f 6e66 6967 7572   with a configur
+00001430: 6174 696f 6e20 6469 6374 696f 6e61 7279  ation dictionary
+00001440: 2063 6f6e 7461 696e 696e 6720 7468 6520   containing the 
+00001450: 6375 7272 656e 7420 6e61 6d65 7320 746f  current names to
+00001460: 2062 6520 6469 7370 6c61 7965 6420 696e   be displayed in
+00001470: 2074 6865 206c 6567 656e 642e 0a0a 546f   the legend...To
+00001480: 2072 756e 2074 6865 2063 6f64 6520 796f   run the code yo
+00001490: 7520 7769 6c6c 2066 6972 7374 2068 6176  u will first hav
+000014a0: 6520 746f 2069 6e73 7461 6c6c 204e 4555  e to install NEU
+000014b0: 524f 4e20 7061 636b 6167 653a 0a0a 2e2e  RON package:....
+000014c0: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
+000014d0: 7468 6f6e 0a0a 2020 2020 7069 7020 696e  thon..    pip in
+000014e0: 7374 616c 6c20 6e65 7572 6f6e 0a0a 5768  stall neuron..Wh
+000014f0: 656e 2079 6f75 2074 6865 6e20 6578 6563  en you then exec
+00001500: 7574 6520 7468 6520 666f 6c6c 6f77 696e  ute the followin
+00001510: 6720 7079 7468 6f6e 2063 6f64 652c 2061  g python code, a
+00001520: 2077 696e 646f 7720 7368 6f75 6c64 206f   window should o
+00001530: 7065 6e20 7769 7468 2074 6865 2063 7572  pen with the cur
+00001540: 7265 6e74 7363 6170 6520 706c 6f74 3a0a  rentscape plot:.
+00001550: 0a2e 2e20 636f 6465 2d62 6c6f 636b 3a3a  ... code-block::
+00001560: 2070 7974 686f 6e0a 0a20 2020 2069 6d70   python..    imp
+00001570: 6f72 7420 6e75 6d70 7920 6173 206e 700a  ort numpy as np.
+00001580: 2020 2020 6672 6f6d 206e 6575 726f 6e20      from neuron 
+00001590: 696d 706f 7274 2068 0a20 2020 2066 726f  import h.    fro
+000015a0: 6d20 6e65 7572 6f6e 2e75 6e69 7473 2069  m neuron.units i
+000015b0: 6d70 6f72 7420 6d73 2c20 6d56 0a20 2020  mport ms, mV.   
+000015c0: 2066 726f 6d20 6375 7272 656e 7473 6361   from currentsca
+000015d0: 7065 2e63 7572 7265 6e74 7363 6170 6520  pe.currentscape 
+000015e0: 696d 706f 7274 2070 6c6f 745f 6375 7272  import plot_curr
+000015f0: 656e 7473 6361 7065 0a0a 2020 2020 682e  entscape..    h.
+00001600: 6c6f 6164 5f66 696c 6528 2773 7464 7275  load_file('stdru
+00001610: 6e2e 686f 6327 290a 0a20 2020 2073 6f6d  n.hoc')..    som
+00001620: 6120 3d20 682e 5365 6374 696f 6e28 6e61  a = h.Section(na
+00001630: 6d65 3d27 736f 6d61 2729 0a20 2020 2064  me='soma').    d
+00001640: 656e 6420 3d20 682e 5365 6374 696f 6e28  end = h.Section(
+00001650: 6e61 6d65 3d27 6465 6e64 2729 0a0a 2020  name='dend')..  
+00001660: 2020 6465 6e64 2e63 6f6e 6e65 6374 2873    dend.connect(s
+00001670: 6f6d 6128 3129 290a 0a20 2020 2073 6f6d  oma(1))..    som
+00001680: 612e 4c20 3d20 736f 6d61 2e64 6961 6d20  a.L = soma.diam 
+00001690: 3d20 3132 2e36 3135 370a 2020 2020 6465  = 12.6157.    de
+000016a0: 6e64 2e4c 203d 2032 3030 0a20 2020 2064  nd.L = 200.    d
+000016b0: 656e 642e 6469 616d 203d 2031 0a0a 2020  end.diam = 1..  
+000016c0: 2020 666f 7220 7365 6320 696e 2068 2e61    for sec in h.a
+000016d0: 6c6c 7365 6328 293a 0a20 2020 2020 2020  llsec():.       
+000016e0: 2073 6563 2e52 6120 3d20 3130 3020 2020   sec.Ra = 100   
+000016f0: 2023 2041 7869 616c 2072 6573 6973 7461   # Axial resista
+00001700: 6e63 6520 696e 204f 686d 202a 2063 6d0a  nce in Ohm * cm.
+00001710: 2020 2020 2020 2020 7365 632e 636d 203d          sec.cm =
+00001720: 2031 2020 2020 2020 2320 4d65 6d62 7261   1      # Membra
+00001730: 6e65 2063 6170 6163 6974 616e 6365 2069  ne capacitance i
+00001740: 6e20 6d69 6372 6f20 4661 7261 6473 202f  n micro Farads /
+00001750: 2063 6d5e 320a 0a20 2020 2023 2049 6e73   cm^2..    # Ins
+00001760: 6572 7420 6163 7469 7665 2048 6f64 676b  ert active Hodgk
+00001770: 696e 2d48 7578 6c65 7920 6375 7272 656e  in-Huxley curren
+00001780: 7420 696e 2074 6865 2073 6f6d 610a 2020  t in the soma.  
+00001790: 2020 736f 6d61 2e69 6e73 6572 7428 2768    soma.insert('h
+000017a0: 6827 290a 2020 2020 666f 7220 7365 6720  h').    for seg 
+000017b0: 696e 2073 6f6d 613a 0a20 2020 2020 2020  in soma:.       
+000017c0: 2073 6567 2e68 682e 676e 6162 6172 203d   seg.hh.gnabar =
+000017d0: 2030 2e31 3220 2023 2053 6f64 6975 6d20   0.12  # Sodium 
+000017e0: 636f 6e64 7563 7461 6e63 6520 696e 2053  conductance in S
+000017f0: 2f63 6d32 0a20 2020 2020 2020 2073 6567  /cm2.        seg
+00001800: 2e68 682e 676b 6261 7220 3d20 302e 3033  .hh.gkbar = 0.03
+00001810: 3620 2023 2050 6f74 6173 7369 756d 2063  6  # Potassium c
+00001820: 6f6e 6475 6374 616e 6365 2069 6e20 532f  onductance in S/
+00001830: 636d 320a 2020 2020 2020 2020 7365 672e  cm2.        seg.
+00001840: 6868 2e67 6c20 3d20 302e 3030 3033 2020  hh.gl = 0.0003  
+00001850: 2020 2320 4c65 616b 2063 6f6e 6475 6374    # Leak conduct
+00001860: 616e 6365 2069 6e20 532f 636d 320a 2020  ance in S/cm2.  
+00001870: 2020 2020 2020 7365 672e 6868 2e65 6c20        seg.hh.el 
+00001880: 3d20 2d35 342e 3320 2020 2020 2320 5265  = -54.3     # Re
+00001890: 7665 7273 616c 2070 6f74 656e 7469 616c  versal potential
+000018a0: 2069 6e20 6d56 0a0a 2020 2020 2320 496e   in mV..    # In
+000018b0: 7365 7274 2070 6173 7369 7665 2063 7572  sert passive cur
+000018c0: 7265 6e74 2069 6e20 7468 6520 6465 6e64  rent in the dend
+000018d0: 7269 7465 0a20 2020 2064 656e 642e 696e  rite.    dend.in
+000018e0: 7365 7274 2827 7061 7327 290a 2020 2020  sert('pas').    
+000018f0: 666f 7220 7365 6720 696e 2064 656e 643a  for seg in dend:
+00001900: 0a20 2020 2020 2020 2073 6567 2e70 6173  .        seg.pas
+00001910: 2e67 203d 2030 2e30 3031 2020 2320 5061  .g = 0.001  # Pa
+00001920: 7373 6976 6520 636f 6e64 7563 7461 6e63  ssive conductanc
+00001930: 6520 696e 2053 2f63 6d32 0a20 2020 2020  e in S/cm2.     
+00001940: 2020 2073 6567 2e70 6173 2e65 203d 202d     seg.pas.e = -
+00001950: 3635 2020 2020 2320 4c65 616b 2072 6576  65    # Leak rev
+00001960: 6572 7361 6c20 706f 7465 6e74 6961 6c20  ersal potential 
+00001970: 6d56 0a0a 2020 2020 7374 696d 203d 2068  mV..    stim = h
+00001980: 2e49 436c 616d 7028 6465 6e64 2831 2929  .IClamp(dend(1))
+00001990: 0a20 2020 2073 7469 6d2e 6465 6c61 7920  .    stim.delay 
+000019a0: 3d20 350a 2020 2020 7374 696d 2e64 7572  = 5.    stim.dur
+000019b0: 203d 2031 300a 2020 2020 7374 696d 2e61   = 10.    stim.a
+000019c0: 6d70 203d 2030 2e31 0a0a 2020 2020 6375  mp = 0.1..    cu
+000019d0: 7272 656e 745f 6e61 6d65 7320 3d20 5b22  rrent_names = ["
+000019e0: 696b 222c 2022 696e 6122 2c20 2269 6c5f  ik", "ina", "il_
+000019f0: 6868 225d 0a20 2020 2074 5f76 6563 203d  hh"].    t_vec =
+00001a00: 2068 2e56 6563 746f 7228 290a 2020 2020   h.Vector().    
+00001a10: 765f 7665 6320 3d20 682e 5665 6374 6f72  v_vec = h.Vector
+00001a20: 2829 0a20 2020 2069 6b5f 7665 6320 3d20  ().    ik_vec = 
+00001a30: 682e 5665 6374 6f72 2829 0a20 2020 2069  h.Vector().    i
+00001a40: 6e61 5f76 6563 203d 2068 2e56 6563 746f  na_vec = h.Vecto
+00001a50: 7228 290a 2020 2020 696c 5f76 6563 203d  r().    il_vec =
+00001a60: 2068 2e56 6563 746f 7228 290a 2020 2020   h.Vector().    
+00001a70: 745f 7665 632e 7265 636f 7264 2868 2e5f  t_vec.record(h._
+00001a80: 7265 665f 7429 0a20 2020 2076 5f76 6563  ref_t).    v_vec
+00001a90: 2e72 6563 6f72 6428 736f 6d61 2830 2e35  .record(soma(0.5
+00001aa0: 292e 5f72 6566 5f76 290a 2020 2020 696b  )._ref_v).    ik
+00001ab0: 5f76 6563 2e72 6563 6f72 6428 736f 6d61  _vec.record(soma
+00001ac0: 2830 2e35 292e 5f72 6566 5f69 6b29 0a20  (0.5)._ref_ik). 
+00001ad0: 2020 2069 6e61 5f76 6563 2e72 6563 6f72     ina_vec.recor
+00001ae0: 6428 736f 6d61 2830 2e35 292e 5f72 6566  d(soma(0.5)._ref
+00001af0: 5f69 6e61 290a 2020 2020 696c 5f76 6563  _ina).    il_vec
+00001b00: 2e72 6563 6f72 6428 736f 6d61 2830 2e35  .record(soma(0.5
+00001b10: 292e 5f72 6566 5f69 6c5f 6868 290a 0a20  )._ref_il_hh).. 
+00001b20: 2020 2068 2e66 696e 6974 6961 6c69 7a65     h.finitialize
+00001b30: 282d 3635 202a 206d 5629 0a20 2020 2068  (-65 * mV).    h
+00001b40: 2e63 6f6e 7469 6e75 6572 756e 2832 3520  .continuerun(25 
+00001b50: 2a20 6d73 290a 0a20 2020 2074 6f5f 7041  * ms)..    to_pA
+00001b60: 203d 2031 3020 2a20 736f 6d61 2830 2e35   = 10 * soma(0.5
+00001b70: 292e 6172 6561 2829 2023 2074 7572 6e20  ).area() # turn 
+00001b80: 6d41 2f63 6d32 2028 2a75 6d32 2920 696e  mA/cm2 (*um2) in
+00001b90: 746f 2070 410a 2020 2020 766f 6c74 6167  to pA.    voltag
+00001ba0: 6520 3d20 6e70 2e61 7361 7272 6179 2876  e = np.asarray(v
+00001bb0: 5f76 6563 290a 2020 2020 706f 7461 7373  _vec).    potass
+00001bc0: 6975 6d20 3d20 6e70 2e61 7361 7272 6179  ium = np.asarray
+00001bd0: 2869 6b5f 7665 6329 202a 2074 6f5f 7041  (ik_vec) * to_pA
+00001be0: 0a20 2020 2073 6f64 6975 6d20 3d20 6e70  .    sodium = np
+00001bf0: 2e61 7361 7272 6179 2869 6e61 5f76 6563  .asarray(ina_vec
+00001c00: 2920 2a20 746f 5f70 410a 2020 2020 6c65  ) * to_pA.    le
+00001c10: 616b 203d 206e 702e 6173 6172 7261 7928  ak = np.asarray(
+00001c20: 696c 5f76 6563 2920 2a20 746f 5f70 410a  il_vec) * to_pA.
+00001c30: 0a20 2020 2063 6f6e 6669 6720 3d20 7b0a  .    config = {.
+00001c40: 2020 2020 2020 2020 226f 7574 7075 7422          "output"
+00001c50: 3a20 7b20 2020 2020 2020 2020 2020 2020  : {             
+00001c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c90: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00001ca0: 2020 2273 6176 6566 6967 223a 2054 7275    "savefig": Tru
+00001cb0: 652c 2020 2020 2020 2020 2020 2020 2020  e,              
+00001cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ce0: 2020 2020 2020 2020 2020 2020 200a 2020               .  
+00001cf0: 2020 2020 2020 2020 2264 6972 223a 2022          "dir": "
+00001d00: 2e22 2c20 2020 2020 2020 2020 2020 2020  .",             
+00001d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d40: 2020 200a 2020 2020 2020 2020 2020 2266     .          "f
+00001d50: 6e61 6d65 223a 2022 7175 6963 6b73 7461  name": "quicksta
+00001d60: 7274 5f70 6c6f 7422 2c20 2020 2020 2020  rt_plot",       
+00001d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d90: 2020 2020 2020 2020 200a 2020 2020 2020           .      
+00001da0: 2020 2020 2265 7874 656e 7369 6f6e 223a      "extension":
+00001db0: 2022 706e 6722 2c20 2020 2020 2020 2020   "png",         
+00001dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001de0: 2020 2020 2020 2020 2020 2020 2020 200a                 .
+00001df0: 2020 2020 2020 2020 2020 2264 7069 223a            "dpi":
+00001e00: 2033 3030 2c20 2020 2020 2020 2020 2020   300,           
+00001e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e40: 2020 2020 200a 2020 2020 2020 2020 2020       .          
+00001e50: 2274 7261 6e73 7061 7265 6e74 223a 2046  "transparent": F
+00001e60: 616c 7365 2020 2020 2020 2020 2020 2020  alse            
+00001e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e90: 2020 2020 2020 2020 2020 200a 2020 2020             .    
+00001ea0: 2020 2020 7d2c 2020 200a 2020 2020 2020      },   .      
+00001eb0: 2020 2263 7572 7265 6e74 223a 207b 226e    "current": {"n
+00001ec0: 616d 6573 223a 2063 7572 7265 6e74 5f6e  ames": current_n
+00001ed0: 616d 6573 7d2c 0a20 2020 2020 2020 2022  ames},.        "
+00001ee0: 766f 6c74 6167 6522 3a20 7b22 796c 696d  voltage": {"ylim
+00001ef0: 223a 205b 2d39 302c 2035 305d 7d2c 0a20  ": [-90, 50]},. 
+00001f00: 2020 2020 2020 2022 6c65 6765 6e64 7465         "legendte
+00001f10: 7874 7369 7a65 223a 2035 2c0a 2020 2020  xtsize": 5,.    
+00001f20: 7d0a 2020 2020 6669 6720 3d20 706c 6f74  }.    fig = plot
+00001f30: 5f63 7572 7265 6e74 7363 6170 6528 766f  _currentscape(vo
+00001f40: 6c74 6167 652c 205b 706f 7461 7373 6975  ltage, [potassiu
+00001f50: 6d2c 2073 6f64 6975 6d2c 206c 6561 6b5d  m, sodium, leak]
+00001f60: 2c20 636f 6e66 6967 290a 2020 2020 6669  , config).    fi
+00001f70: 672e 7368 6f77 2829 0a0a 5768 656e 2079  g.show()..When y
+00001f80: 6f75 2072 756e 2074 6869 7320 636f 6465  ou run this code
+00001f90: 2069 6e20 5079 7468 6f6e 2c20 6974 2077   in Python, it w
+00001fa0: 696c 6c20 6765 6e65 7261 7465 2074 6865  ill generate the
+00001fb0: 2066 6f6c 6c6f 7769 6e67 2063 7572 7265   following curre
+00001fc0: 6e74 7363 6170 6520 706c 6f74 2028 696e  ntscape plot (in
+00001fd0: 2061 2077 696e 646f 772c 2061 6e64 206f   a window, and o
+00001fe0: 6e20 6469 736b 2061 7320 7175 6963 6b73  n disk as quicks
+00001ff0: 7461 7274 5f70 6c6f 742e 706e 6729 3a0a  tart_plot.png):.
+00002000: 0a2e 2e20 696d 6167 653a 3a20 646f 632f  ... image:: doc/
+00002010: 736f 7572 6365 2f69 6d61 6765 732f 7175  source/images/qu
+00002020: 6963 6b73 7461 7274 5f70 6c6f 742e 706e  ickstart_plot.pn
+00002030: 670a 0a54 7574 6f72 6961 6c0a 3d3d 3d3d  g..Tutorial.====
+00002040: 3d3d 3d3d 0a0a 4120 6d6f 7265 2064 6574  ====..A more det
+00002050: 6169 6c65 6420 6578 706c 616e 6174 696f  ailed explanatio
+00002060: 6e20 6f6e 2068 6f77 2074 6f20 7573 6520  n on how to use 
+00002070: 4375 7272 656e 7473 6361 7065 2c20 6173  Currentscape, as
+00002080: 2077 656c 6c20 6173 206f 7468 6572 2065   well as other e
+00002090: 7861 6d70 6c65 7320 6361 6e20 6265 2066  xamples can be f
+000020a0: 6f75 6e64 206f 6e20 7468 6520 6074 7574  ound on the `tut
+000020b0: 6f72 6961 6c20 7061 6765 203c 5475 746f  orial page <Tuto
+000020c0: 7269 616c 2e72 7374 3e60 5f2e 0a0a 4150  rial.rst>`_...AP
+000020d0: 4920 446f 6375 6d65 6e74 6174 696f 6e0a  I Documentation.
+000020e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000020f0: 3d0a 0a54 6865 2041 5049 2064 6f63 756d  =..The API docum
+00002100: 656e 7461 7469 6f6e 2063 616e 2062 6520  entation can be 
+00002110: 666f 756e 6420 6f6e 2060 5265 6164 5468  found on `ReadTh
+00002120: 6544 6f63 7320 3c22 6874 7470 733a 2f2f  eDocs <"https://
+00002130: 6375 7272 656e 7473 6361 7065 2e72 6561  currentscape.rea
+00002140: 6474 6865 646f 6373 2e69 6f22 3e60 5f2e  dthedocs.io">`_.
+00002150: 0a0a 4675 6e64 696e 6720 2620 4163 6b6e  ..Funding & Ackn
+00002160: 6f77 6c65 6467 656d 656e 7473 0a3d 3d3d  owledgements.===
+00002170: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00002180: 3d3d 3d3d 3d3d 3d0a 0a57 6520 7769 7368  =======..We wish
+00002190: 2074 6f20 7468 616e 6b20 7468 6520 6175   to thank the au
+000021a0: 7468 6f72 7320 6f66 2060 416c 6f6e 736f  thors of `Alonso
+000021b0: 2061 6e64 204d 6172 6465 722c 2032 3031   and Marder, 201
+000021c0: 3920 3c68 7474 7073 3a2f 2f64 6f69 2e6f  9 <https://doi.o
+000021d0: 7267 2f31 302e 3735 3534 2f65 4c69 6665  rg/10.7554/eLife
+000021e0: 2e34 3237 3232 3e60 5f5f 2074 6f20 6c65  .42722>`__ to le
+000021f0: 7420 7573 2069 6e74 6567 7261 7465 2061  t us integrate a
+00002200: 2070 6172 7420 6f66 2074 6865 6972 2060   part of their `
+00002210: 636f 6465 203c 6874 7470 733a 2f2f 6461  code <https://da
+00002220: 7461 6472 7961 642e 6f72 672f 7374 6173  tadryad.org/stas
+00002230: 682f 6461 7461 7365 742f 646f 693a 3130  h/dataset/doi:10
+00002240: 2e35 3036 312f 6472 7961 642e 6430 3737  .5061/dryad.d077
+00002250: 396d 623e 605f 2069 6e74 6f20 7468 6973  9mb>`_ into this
+00002260: 2072 6570 6f73 6974 6f72 792e 0a0a 5468   repository...Th
+00002270: 6520 7061 7274 206f 6620 7468 6520 636f  e part of the co
+00002280: 6465 2069 6e20 7468 6973 2072 6570 6f73  de in this repos
+00002290: 6974 6f72 7920 6465 7665 6c6f 7065 6420  itory developed 
+000022a0: 6279 2074 6865 2045 5046 4c20 426c 7565  by the EPFL Blue
+000022b0: 2042 7261 696e 2050 726f 6a65 6374 2077   Brain Project w
+000022c0: 6173 2073 7570 706f 7274 6564 2062 7920  as supported by 
+000022d0: 6675 6e64 696e 6720 746f 2074 6865 2042  funding to the B
+000022e0: 6c75 6520 4272 6169 6e20 5072 6f6a 6563  lue Brain Projec
+000022f0: 742c 2061 2072 6573 6561 7263 6820 6365  t, a research ce
+00002300: 6e74 6572 206f 6620 7468 6520 c389 636f  nter of the ..co
+00002310: 6c65 2070 6f6c 7974 6563 686e 6971 7565  le polytechnique
+00002320: 2066 c3a9 64c3 a972 616c 6520 6465 204c   f..d..rale de L
+00002330: 6175 7361 6e6e 6520 2845 5046 4c29 2c20  ausanne (EPFL), 
+00002340: 6672 6f6d 2074 6865 2053 7769 7373 2067  from the Swiss g
+00002350: 6f76 6572 6e6d 656e 7427 7320 4554 4820  overnment's ETH 
+00002360: 426f 6172 6420 6f66 2074 6865 2053 7769  Board of the Swi
+00002370: 7373 2046 6564 6572 616c 2049 6e73 7469  ss Federal Insti
+00002380: 7475 7465 7320 6f66 2054 6563 686e 6f6c  tutes of Technol
+00002390: 6f67 792e 0a0a 0a2e 2e20 7c70 7970 697c  ogy...... |pypi|
+000023a0: 2069 6d61 6765 3a3a 2068 7474 7073 3a2f   image:: https:/
+000023b0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+000023c0: 7079 7069 2f76 2f63 7572 7265 6e74 7363  pypi/v/currentsc
+000023d0: 6170 652e 7376 670a 2020 2020 2020 2020  ape.svg.        
+000023e0: 2020 2020 2020 203a 7461 7267 6574 3a20         :target: 
+000023f0: 6874 7470 733a 2f2f 7465 7374 2e70 7970  https://test.pyp
+00002400: 692e 6f72 672f 7072 6f6a 6563 742f 6375  i.org/project/cu
+00002410: 7272 656e 7473 6361 7065 2f0a 2020 2020  rrentscape/.    
+00002420: 2020 2020 2020 2020 2020 203a 616c 743a             :alt:
+00002430: 206c 6174 6573 7420 7265 6c65 6173 650a   latest release.
+00002440: 0a2e 2e20 7c64 6f63 737c 2069 6d61 6765  ... |docs| image
+00002450: 3a3a 2068 7474 7073 3a2f 2f72 6561 6474  :: https://readt
+00002460: 6865 646f 6373 2e6f 7267 2f70 726f 6a65  hedocs.org/proje
+00002470: 6374 732f 6375 7272 656e 7473 6361 7065  cts/currentscape
+00002480: 2f62 6164 6765 2f3f 7665 7273 696f 6e3d  /badge/?version=
+00002490: 6c61 7465 7374 0a20 2020 2020 2020 2020  latest.         
+000024a0: 2020 2020 2020 3a74 6172 6765 743a 2068        :target: h
+000024b0: 7474 7073 3a2f 2f63 7572 7265 6e74 7363  ttps://currentsc
+000024c0: 6170 652e 7265 6164 7468 6564 6f63 732e  ape.readthedocs.
+000024d0: 696f 2f0a 2020 2020 2020 2020 2020 2020  io/.            
+000024e0: 2020 203a 616c 743a 206c 6174 6573 7420     :alt: latest 
+000024f0: 646f 6375 6d65 6e74 6174 696f 6e0a 0a2e  documentation...
+00002500: 2e20 7c6c 6963 656e 7365 7c20 696d 6167  . |license| imag
+00002510: 653a 3a20 6874 7470 733a 2f2f 696d 672e  e:: https://img.
+00002520: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+00002530: 6c2f 6375 7272 656e 7473 6361 7065 2e73  l/currentscape.s
+00002540: 7667 0a20 2020 2020 2020 2020 2020 2020  vg.             
+00002550: 2020 2020 203a 7461 7267 6574 3a20 6874       :target: ht
+00002560: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00002570: 2f42 6c75 6542 7261 696e 2f43 7572 7265  /BlueBrain/Curre
+00002580: 6e74 7363 6170 652f 626c 6f62 2f6d 6169  ntscape/blob/mai
+00002590: 6e2f 4c49 4345 4e53 452e 7478 740a 2020  n/LICENSE.txt.  
+000025a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025b0: 3a61 6c74 3a20 6c69 6365 6e73 650a 0a2e  :alt: license...
+000025c0: 2e20 7c62 7569 6c64 7c20 696d 6167 653a  . |build| image:
+000025d0: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+000025e0: 2e63 6f6d 2f42 6c75 6542 7261 696e 2f43  .com/BlueBrain/C
+000025f0: 7572 7265 6e74 7363 6170 652f 776f 726b  urrentscape/work
+00002600: 666c 6f77 732f 5465 7374 2f62 6164 6765  flows/Test/badge
+00002610: 2e73 7667 3f62 7261 6e63 683d 6d61 696e  .svg?branch=main
+00002620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002630: 203a 7461 7267 6574 3a20 6874 7470 733a   :target: https:
+00002640: 2f2f 6769 7468 7562 2e63 6f6d 2f42 6c75  //github.com/Blu
+00002650: 6542 7261 696e 2f43 7572 7265 6e74 7363  eBrain/Currentsc
+00002660: 6170 652f 6163 7469 6f6e 730a 2020 2020  ape/actions.    
+00002670: 2020 2020 2020 2020 2020 2020 3a61 6c74              :alt
+00002680: 3a20 6163 7469 6f6e 7320 6275 696c 6420  : actions build 
+00002690: 7374 6174 7573 0a0a 2e2e 207c 636f 7665  status.... |cove
+000026a0: 7261 6765 7c20 696d 6167 653a 3a20 6874  rage| image:: ht
+000026b0: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
+000026c0: 2f67 6974 6875 622f 426c 7565 4272 6169  /github/BlueBrai
+000026d0: 6e2f 4375 7272 656e 7473 6361 7065 2f63  n/Currentscape/c
+000026e0: 6f76 6572 6167 652e 7376 673f 6272 616e  overage.svg?bran
+000026f0: 6368 3d6d 6169 6e0a 2020 2020 2020 2020  ch=main.        
+00002700: 2020 2020 2020 2020 2020 203a 7461 7267             :targ
+00002710: 6574 3a20 6874 7470 733a 2f2f 636f 6465  et: https://code
+00002720: 636f 762e 696f 2f67 682f 426c 7565 4272  cov.io/gh/BlueBr
+00002730: 6169 6e2f 6375 7272 656e 7473 6361 7065  ain/currentscape
+00002740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002750: 2020 2020 3a61 6c74 3a20 636f 7665 7261      :alt: covera
+00002760: 6765 0a0a 2e2e 207c 6769 7474 6572 7c20  ge.... |gitter| 
+00002770: 696d 6167 653a 3a20 6874 7470 733a 2f2f  image:: https://
+00002780: 6261 6467 6573 2e67 6974 7465 722e 696d  badges.gitter.im
+00002790: 2f4a 6f69 6e25 3230 4368 6174 2e73 7667  /Join%20Chat.svg
+000027a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000027b0: 2020 3a74 6172 6765 743a 2068 7474 7073    :target: https
+000027c0: 3a2f 2f67 6974 7465 722e 696d 2f62 6c75  ://gitter.im/blu
+000027d0: 6562 7261 696e 2f63 7572 7265 6e74 7363  ebrain/currentsc
+000027e0: 6170 650a 2020 2020 2020 2020 2020 2020  ape.            
+000027f0: 2020 2020 203a 616c 743a 204a 6f69 6e20       :alt: Join 
+00002800: 7468 6520 6368 6174 2061 7420 6874 7470  the chat at http
+00002810: 733a 2f2f 6769 7474 6572 2e69 6d2f 626c  s://gitter.im/bl
+00002820: 7565 6272 6169 6e2f 6375 7272 656e 7473  uebrain/currents
+00002830: 6361 7065 0a                             cape.
```

### Comparing `currentscape-0.0.0/README.rst` & `currentscape-1.0.1/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,562 +1,578 @@
 00000000: 4375 7272 656e 7473 6361 7065 0a3d 3d3d  Currentscape.===
-00000010: 3d3d 3d3d 3d3d 3d3d 3d0a 0a2e 2e20 7261  =========.... ra
-00000020: 773a 3a20 6874 6d6c 0a0a 093c 7461 626c  w:: html...<tabl
-00000030: 653e 0a09 3c74 723e 0a09 2020 3c74 643e  e>..<tr>..  <td>
-00000040: 4c61 7465 7374 2052 656c 6561 7365 3c2f  Latest Release</
-00000050: 7464 3e0a 0920 203c 7464 3e0a 0920 2020  td>..  <td>..   
-00000060: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-00000070: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
-00000080: 6374 2f63 7572 7265 6e74 7363 6170 652f  ct/currentscape/
-00000090: 223e 0a09 2020 2020 3c69 6d67 2073 7263  ">..    <img src
-000000a0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
-000000b0: 6965 6c64 732e 696f 2f70 7970 692f 762f  ields.io/pypi/v/
-000000c0: 6375 7272 656e 7473 6361 7065 2e73 7667  currentscape.svg
-000000d0: 2220 616c 743d 226c 6174 6573 7420 7265  " alt="latest re
-000000e0: 6c65 6173 6522 202f 3e0a 0920 2020 203c  lease" />..    <
-000000f0: 2f61 3e0a 0920 203c 2f74 643e 0a09 3c2f  /a>..  </td>..</
-00000100: 7472 3e0a 093c 7472 3e0a 0920 203c 7464  tr>..<tr>..  <td
-00000110: 3e44 6f63 756d 656e 7461 7469 6f6e 3c2f  >Documentation</
-00000120: 7464 3e0a 0920 203c 7464 3e0a 0920 2020  td>..  <td>..   
-00000130: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-00000140: 2f2f 6375 7272 656e 7473 6361 7065 2e72  //currentscape.r
-00000150: 6561 6474 6865 646f 6373 2e69 6f2f 223e  eadthedocs.io/">
-00000160: 0a09 2020 2020 3c69 6d67 2073 7263 3d22  ..    <img src="
-00000170: 6874 7470 733a 2f2f 7265 6164 7468 6564  https://readthed
-00000180: 6f63 732e 6f72 672f 7072 6f6a 6563 7473  ocs.org/projects
-00000190: 2f63 7572 7265 6e74 7363 6170 652f 6261  /currentscape/ba
-000001a0: 6467 652f 3f76 6572 7369 6f6e 3d6c 6174  dge/?version=lat
-000001b0: 6573 7422 2061 6c74 3d22 6c61 7465 7374  est" alt="latest
-000001c0: 2064 6f63 756d 656e 7461 7469 6f6e 2220   documentation" 
-000001d0: 2f3e 0a09 2020 2020 3c2f 613e 0a09 2020  />..    </a>..  
-000001e0: 3c2f 7464 3e0a 093c 2f74 723e 0a09 3c74  </td>..</tr>..<t
-000001f0: 723e 0a09 2020 3c74 643e 4c69 6365 6e73  r>..  <td>Licens
-00000200: 653c 2f74 643e 0a09 2020 3c74 643e 0a09  e</td>..  <td>..
-00000210: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
-00000220: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000230: 426c 7565 4272 6169 6e2f 4375 7272 656e  BlueBrain/Curren
-00000240: 7473 6361 7065 2f62 6c6f 622f 6d61 696e  tscape/blob/main
-00000250: 2f4c 4943 454e 5345 2e74 7874 223e 0a09  /LICENSE.txt">..
-00000260: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
-00000270: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000280: 732e 696f 2f70 7970 692f 6c2f 6375 7272  s.io/pypi/l/curr
-00000290: 656e 7473 6361 7065 2e73 7667 2220 616c  entscape.svg" al
-000002a0: 743d 226c 6963 656e 7365 2220 2f3e 0a09  t="license" />..
-000002b0: 2020 2020 3c2f 613e 0a09 3c2f 7464 3e0a      </a>..</td>.
-000002c0: 093c 2f74 723e 0a09 3c74 723e 0a09 2020  .</tr>..<tr>..  
-000002d0: 3c74 643e 4275 696c 6420 5374 6174 7573  <td>Build Status
-000002e0: 3c2f 7464 3e0a 0920 203c 7464 3e0a 0920  </td>..  <td>.. 
-000002f0: 2020 203c 6120 6872 6566 3d22 6874 7470     <a href="http
-00000300: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f42  s://github.com/B
-00000310: 6c75 6542 7261 696e 2f43 7572 7265 6e74  lueBrain/Current
-00000320: 7363 6170 652f 6163 7469 6f6e 7322 3e0a  scape/actions">.
-00000330: 0920 2020 203c 696d 6720 7372 633d 2268  .    <img src="h
-00000340: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000350: 6d2f 426c 7565 4272 6169 6e2f 4375 7272  m/BlueBrain/Curr
-00000360: 656e 7473 6361 7065 2f77 6f72 6b66 6c6f  entscape/workflo
-00000370: 7773 2f54 6573 742f 6261 6467 652e 7376  ws/Test/badge.sv
-00000380: 673f 6272 616e 6368 3d6d 6169 6e22 2061  g?branch=main" a
-00000390: 6c74 3d22 4163 7469 6f6e 7320 6275 696c  lt="Actions buil
-000003a0: 6420 7374 6174 7573 2220 2f3e 0a09 2020  d status" />..  
-000003b0: 2020 3c2f 613e 0a09 2020 3c2f 7464 3e0a    </a>..  </td>.
-000003c0: 093c 2f74 723e 0a09 3c74 723e 0a09 2020  .</tr>..<tr>..  
-000003d0: 3c74 643e 436f 7665 7261 6765 3c2f 7464  <td>Coverage</td
-000003e0: 3e0a 0920 203c 7464 3e0a 0920 2020 203c  >..  <td>..    <
-000003f0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00000400: 636f 6465 636f 762e 696f 2f67 682f 426c  codecov.io/gh/Bl
-00000410: 7565 4272 6169 6e2f 6375 7272 656e 7473  ueBrain/currents
-00000420: 6361 7065 223e 0a09 2020 2020 3c69 6d67  cape">..    <img
-00000430: 2073 7263 3d22 6874 7470 733a 2f2f 636f   src="https://co
-00000440: 6465 636f 762e 696f 2f67 6974 6875 622f  decov.io/github/
-00000450: 426c 7565 4272 6169 6e2f 4375 7272 656e  BlueBrain/Curren
-00000460: 7473 6361 7065 2f63 6f76 6572 6167 652e  tscape/coverage.
-00000470: 7376 673f 6272 616e 6368 3d6d 6169 6e22  svg?branch=main"
-00000480: 2061 6c74 3d22 636f 7665 7261 6765 2220   alt="coverage" 
-00000490: 2f3e 0a09 2020 2020 3c2f 613e 0a09 2020  />..    </a>..  
-000004a0: 3c2f 7464 3e0a 093c 2f74 723e 0a09 3c74  </td>..</tr>..<t
-000004b0: 723e 0a09 093c 7464 3e47 6974 7465 723c  r>...<td>Gitter<
-000004c0: 2f74 643e 0a09 093c 7464 3e0a 0909 093c  /td>...<td>....<
-000004d0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-000004e0: 6769 7474 6572 2e69 6d2f 626c 7565 6272  gitter.im/bluebr
-000004f0: 6169 6e2f 6375 7272 656e 7473 6361 7065  ain/currentscape
-00000500: 223e 0a09 0909 3c69 6d67 2073 7263 3d22  ">....<img src="
-00000510: 6874 7470 733a 2f2f 6261 6467 6573 2e67  https://badges.g
-00000520: 6974 7465 722e 696d 2f4a 6f69 6e25 3230  itter.im/Join%20
-00000530: 4368 6174 2e73 7667 220a 0909 3c2f 613e  Chat.svg"...</a>
-00000540: 0a09 093c 2f74 643e 0a09 3c2f 7472 3e0a  ...</td>..</tr>.
-00000550: 093c 2f74 6162 6c65 3e0a 0a49 6e74 726f  .</table>..Intro
-00000560: 6475 6374 696f 6e0a 3d3d 3d3d 3d3d 3d3d  duction.========
-00000570: 3d3d 3d3d 0a0a 4375 7272 656e 7473 6361  ====..Currentsca
-00000580: 7065 2069 7320 6120 5079 7468 6f6e 2074  pe is a Python t
-00000590: 6f6f 6c20 656e 6162 6c69 6e67 2073 6369  ool enabling sci
-000005a0: 656e 7469 7374 7320 746f 2065 6173 696c  entists to easil
-000005b0: 7920 706c 6f74 2074 6865 2063 7572 7265  y plot the curre
-000005c0: 6e74 7320 696e 2065 6c65 6374 7269 6361  nts in electrica
-000005d0: 6c20 6e65 7572 6f6e 206d 6f64 656c 732e  l neuron models.
-000005e0: 0a54 6865 2063 6f64 6520 6973 2062 6173  .The code is bas
-000005f0: 6564 206f 6e20 7468 6520 7061 7065 7220  ed on the paper 
-00000600: 6041 6c6f 6e73 6f20 616e 6420 4d61 7264  `Alonso and Mard
-00000610: 6572 2c20 3230 3139 203c 6874 7470 733a  er, 2019 <https:
-00000620: 2f2f 646f 692e 6f72 672f 3130 2e37 3535  //doi.org/10.755
-00000630: 342f 654c 6966 652e 3432 3732 323e 605f  4/eLife.42722>`_
-00000640: 2e0a 0a43 7572 7265 6e74 7363 6170 6520  ...Currentscape 
-00000650: 6669 6775 7265 7320 706c 6f74 2074 6865  figures plot the
-00000660: 2070 6572 6365 6e74 6167 6520 6f66 2069   percentage of i
-00000670: 6e77 6172 6420 616e 6420 6f75 7477 6172  nward and outwar
-00000680: 6420 696f 6e69 6320 6d65 6d62 7261 6e65  d ionic membrane
-00000690: 2063 7572 7265 6e74 732c 0a74 6865 2074   currents,.the t
-000006a0: 6f74 616c 2069 6e77 6172 6420 616e 6420  otal inward and 
-000006b0: 6f75 7477 6172 6420 6375 7272 656e 7473  outward currents
-000006c0: 2c20 6173 2077 656c 6c20 6173 2074 6865  , as well as the
-000006d0: 2076 6f6c 7461 6765 2069 6e20 6675 6e63   voltage in func
-000006e0: 7469 6f6e 206f 6620 7469 6d65 2e0a 4974  tion of time..It
-000006f0: 2061 6c6c 6f77 7320 6d6f 6465 6c6c 6572   allows modeller
-00000700: 7320 746f 2073 6565 2077 6869 6368 2063  s to see which c
-00000710: 7572 7265 6e74 7320 706c 6179 2061 2072  urrents play a r
-00000720: 6f6c 6520 6174 2061 6e79 2067 6976 656e  ole at any given
-00000730: 2074 696d 6520 6475 7269 6e67 2061 2073   time during a s
-00000740: 696d 756c 6174 696f 6e2c 2061 6e64 2063  imulation, and c
-00000750: 6865 636b 2069 6e20 6465 7074 6820 7468  heck in depth th
-00000760: 6520 6375 7272 656e 7420 6479 6e61 6d69  e current dynami
-00000770: 6373 2e0a 0a2e 2e20 696d 6167 653a 3a20  cs..... image:: 
-00000780: 646f 632f 736f 7572 6365 2f69 6d61 6765  doc/source/image
-00000790: 732f 706c 6f74 2e70 6e67 0a0a 4369 7461  s/plot.png..Cita
-000007a0: 7469 6f6e 0a3d 3d3d 3d3d 3d3d 3d0a 0a57  tion.========..W
-000007b0: 6865 6e20 796f 7520 7573 6520 7468 6973  hen you use this
-000007c0: 2043 7572 7265 6e74 7363 6170 6520 736f   Currentscape so
-000007d0: 6674 7761 7265 2066 6f72 2079 6f75 7220  ftware for your 
-000007e0: 7265 7365 6172 6368 2c20 7765 2061 736b  research, we ask
-000007f0: 2079 6f75 2074 6f20 6369 7465 2074 6865   you to cite the
-00000800: 2066 6f6c 6c6f 7769 6e67 2070 7562 6c69   following publi
-00000810: 6361 7469 6f6e 2028 7468 6973 2069 6e63  cation (this inc
-00000820: 6c75 6465 7320 706f 7374 6572 2070 7265  ludes poster pre
-00000830: 7365 6e74 6174 696f 6e73 293a 0a0a 2e2e  sentations):....
-00000840: 2063 6f64 652d 626c 6f63 6b3a 3a20 0a0a   code-block:: ..
-00000850: 2020 2020 4061 7274 6963 6c65 207b 3130      @article {10
-00000860: 2e37 3535 342f 654c 6966 652e 3432 3732  .7554/eLife.4272
-00000870: 322c 0a20 2020 2061 7274 6963 6c65 5f74  2,.    article_t
-00000880: 7970 6520 3d20 7b6a 6f75 726e 616c 7d2c  ype = {journal},
-00000890: 0a20 2020 2074 6974 6c65 203d 207b 5669  .    title = {Vi
-000008a0: 7375 616c 697a 6174 696f 6e20 6f66 2063  sualization of c
-000008b0: 7572 7265 6e74 7320 696e 206e 6575 7261  urrents in neura
-000008c0: 6c20 6d6f 6465 6c73 2077 6974 6820 7369  l models with si
-000008d0: 6d69 6c61 7220 6265 6861 7669 6f72 2061  milar behavior a
-000008e0: 6e64 2064 6966 6665 7265 6e74 2063 6f6e  nd different con
-000008f0: 6475 6374 616e 6365 2064 656e 7369 7469  ductance densiti
-00000900: 6573 7d2c 0a20 2020 2061 7574 686f 7220  es},.    author 
-00000910: 3d20 7b41 6c6f 6e73 6f2c 204c 6561 6e64  = {Alonso, Leand
-00000920: 726f 204d 2061 6e64 204d 6172 6465 722c  ro M and Marder,
-00000930: 2045 7665 7d2c 0a20 2020 2065 6469 746f   Eve},.    edito
-00000940: 7220 3d20 7b57 6573 7462 726f 6f6b 2c20  r = {Westbrook, 
-00000950: 4761 7279 204c 2061 6e64 2053 6b69 6e6e  Gary L and Skinn
-00000960: 6572 2c20 4672 616e 6365 7320 4b20 616e  er, Frances K an
-00000970: 6420 4c61 6e6b 6172 616e 792c 204d 696c  d Lankarany, Mil
-00000980: 6164 2061 6e64 2042 7269 7474 6f6e 2c20  ad and Britton, 
-00000990: 4f6c 6976 6572 7d2c 0a20 2020 2076 6f6c  Oliver},.    vol
-000009a0: 756d 6520 3d20 382c 0a20 2020 2079 6561  ume = 8,.    yea
-000009b0: 7220 3d20 3230 3139 2c0a 2020 2020 6d6f  r = 2019,.    mo
-000009c0: 6e74 6820 3d20 7b6a 616e 7d2c 0a20 2020  nth = {jan},.   
-000009d0: 2070 7562 5f64 6174 6520 3d20 7b32 3031   pub_date = {201
-000009e0: 392d 3031 2d33 317d 2c0a 2020 2020 7061  9-01-31},.    pa
-000009f0: 6765 7320 3d20 7b65 3432 3732 327d 2c0a  ges = {e42722},.
-00000a00: 2020 2020 6369 7461 7469 6f6e 203d 207b      citation = {
-00000a10: 654c 6966 6520 3230 3139 3b38 3a65 3432  eLife 2019;8:e42
-00000a20: 3732 327d 2c0a 2020 2020 646f 6920 3d20  722},.    doi = 
-00000a30: 7b31 302e 3735 3534 2f65 4c69 6665 2e34  {10.7554/eLife.4
-00000a40: 3237 3232 7d2c 0a20 2020 2075 726c 203d  2722},.    url =
-00000a50: 207b 6874 7470 733a 2f2f 646f 692e 6f72   {https://doi.or
-00000a60: 672f 3130 2e37 3535 342f 654c 6966 652e  g/10.7554/eLife.
-00000a70: 3432 3732 327d 2c0a 2020 2020 6162 7374  42722},.    abst
-00000a80: 7261 6374 203d 207b 436f 6e64 7563 7461  ract = {Conducta
-00000a90: 6e63 652d 6261 7365 6420 6d6f 6465 6c73  nce-based models
-00000aa0: 206f 6620 6e65 7572 616c 2061 6374 6976   of neural activ
-00000ab0: 6974 7920 7072 6f64 7563 6520 6c61 7267  ity produce larg
-00000ac0: 6520 616d 6f75 6e74 7320 6f66 2064 6174  e amounts of dat
-00000ad0: 6120 7468 6174 2063 616e 2062 6520 6861  a that can be ha
-00000ae0: 7264 2074 6f20 7669 7375 616c 697a 6520  rd to visualize 
-00000af0: 616e 6420 696e 7465 7270 7265 742e 2057  and interpret. W
-00000b00: 6520 696e 7472 6f64 7563 6520 7669 7375  e introduce visu
-00000b10: 616c 697a 6174 696f 6e20 6d65 7468 6f64  alization method
-00000b20: 7320 746f 2064 6973 706c 6179 2074 6865  s to display the
-00000b30: 2064 796e 616d 6963 7320 6f66 2074 6865   dynamics of the
-00000b40: 2069 6f6e 6963 2063 7572 7265 6e74 7320   ionic currents 
-00000b50: 616e 6420 746f 2064 6973 706c 6179 2074  and to display t
-00000b60: 6865 206d 6f64 656c 73e2 8099 2072 6573  he models... res
-00000b70: 706f 6e73 6520 746f 2070 6572 7475 7262  ponse to perturb
-00000b80: 6174 696f 6e73 2e20 546f 2076 6973 7561  ations. To visua
-00000b90: 6c69 7a65 2074 6865 2063 7572 7265 6e74  lize the current
-00000ba0: 73e2 8099 2064 796e 616d 6963 732c 2077  s... dynamics, w
-00000bb0: 6520 636f 6d70 7574 6520 7468 6520 7065  e compute the pe
-00000bc0: 7263 656e 7420 636f 6e74 7269 6275 7469  rcent contributi
-00000bd0: 6f6e 206f 6620 6561 6368 2063 7572 7265  on of each curre
-00000be0: 6e74 2061 6e64 2064 6973 706c 6179 2074  nt and display t
-00000bf0: 6865 6d20 6f76 6572 2074 696d 6520 7573  hem over time us
-00000c00: 696e 6720 7374 6163 6b65 642d 6172 6561  ing stacked-area
-00000c10: 2070 6c6f 7473 2e20 5468 6520 7761 7665   plots. The wave
-00000c20: 666f 726d 206f 6620 7468 6520 6d65 6d62  form of the memb
-00000c30: 7261 6e65 2070 6f74 656e 7469 616c 2061  rane potential a
-00000c40: 6e64 2074 6865 2063 6f6e 7472 6962 7574  nd the contribut
-00000c50: 696f 6e20 6f66 2065 6163 6820 6375 7272  ion of each curr
-00000c60: 656e 7420 6368 616e 6765 2061 7320 7468  ent change as th
-00000c70: 6520 6d6f 6465 6c73 2061 7265 2070 6572  e models are per
-00000c80: 7475 7262 6564 2e20 546f 2072 6570 7265  turbed. To repre
-00000c90: 7365 6e74 2074 6865 7365 2063 6861 6e67  sent these chang
-00000ca0: 6573 206f 7665 7220 6120 7261 6e67 6520  es over a range 
-00000cb0: 6f66 2074 6865 2070 6572 7475 7262 6174  of the perturbat
-00000cc0: 696f 6e20 636f 6e74 726f 6c20 7061 7261  ion control para
-00000cd0: 6d65 7465 722c 2077 6520 636f 6d70 7574  meter, we comput
-00000ce0: 6520 616e 6420 6469 7370 6c61 7920 7468  e and display th
-00000cf0: 6520 6469 7374 7269 6275 7469 6f6e 7320  e distributions 
-00000d00: 6f66 2074 6865 7365 2077 6176 6566 6f72  of these wavefor
-00000d10: 6d73 2e20 5765 2069 6c6c 7573 7472 6174  ms. We illustrat
-00000d20: 6520 7468 6573 6520 7072 6f63 6564 7572  e these procedur
-00000d30: 6573 2069 6e20 7369 7820 6578 616d 706c  es in six exampl
-00000d40: 6573 206f 6620 6275 7273 7469 6e67 206d  es of bursting m
-00000d50: 6f64 656c 206e 6575 726f 6e73 2077 6974  odel neurons wit
-00000d60: 6820 7369 6d69 6c61 7220 6163 7469 7669  h similar activi
-00000d70: 7479 2062 7574 2074 6861 7420 6469 6666  ty but that diff
-00000d80: 6572 2061 7320 6d75 6368 2061 7320 7468  er as much as th
-00000d90: 7265 6566 6f6c 6420 696e 2074 6865 6972  reefold in their
-00000da0: 2063 6f6e 6475 6374 616e 6365 2064 656e   conductance den
-00000db0: 7369 7469 6573 2e20 5468 6573 6520 7669  sities. These vi
-00000dc0: 7375 616c 697a 6174 696f 6e20 6d65 7468  sualization meth
-00000dd0: 6f64 7320 7072 6f76 6964 6520 6865 7572  ods provide heur
-00000de0: 6973 7469 6320 696e 7369 6768 7420 696e  istic insight in
-00000df0: 746f 2077 6879 2069 6e64 6976 6964 7561  to why individua
-00000e00: 6c20 6e65 7572 6f6e 7320 6f72 206e 6574  l neurons or net
-00000e10: 776f 726b 7320 7769 7468 2073 696d 696c  works with simil
-00000e20: 6172 2062 6568 6176 696f 7220 6361 6e20  ar behavior can 
-00000e30: 7265 7370 6f6e 6420 7769 6465 6c79 2064  respond widely d
-00000e40: 6966 6665 7265 6e74 6c79 2074 6f20 7065  ifferently to pe
-00000e50: 7274 7572 6261 7469 6f6e 732e 7d2c 0a20  rturbations.},. 
-00000e60: 2020 206b 6579 776f 7264 7320 3d20 7b6e     keywords = {n
-00000e70: 6575 726f 6e61 6c20 6f73 6369 6c6c 6174  euronal oscillat
-00000e80: 6f72 732c 204e 612b 2063 6861 6e6e 656c  ors, Na+ channel
-00000e90: 732c 2043 612b 2b20 6368 616e 6e65 6c73  s, Ca++ channels
-00000ea0: 2c20 4b2b 2063 6861 6e6e 656c 732c 2063  , K+ channels, c
-00000eb0: 6f6e 6475 6374 616e 6365 2d62 6173 6564  onductance-based
-00000ec0: 2c20 696f 6e69 6320 6368 616e 6e65 6c73  , ionic channels
-00000ed0: 7d2c 0a20 2020 206a 6f75 726e 616c 203d  },.    journal =
-00000ee0: 207b 654c 6966 657d 2c0a 2020 2020 6973   {eLife},.    is
-00000ef0: 736e 203d 207b 3230 3530 2d30 3834 587d  sn = {2050-084X}
-00000f00: 2c0a 2020 2020 7075 626c 6973 6865 7220  ,.    publisher 
-00000f10: 3d20 7b65 4c69 6665 2053 6369 656e 6365  = {eLife Science
-00000f20: 7320 5075 626c 6963 6174 696f 6e73 2c20  s Publications, 
-00000f30: 4c74 647d 2c0a 2020 2020 7d0a 0a53 7570  Ltd},.    }..Sup
-00000f40: 706f 7274 0a3d 3d3d 3d3d 3d3d 0a0a 5765  port.=======..We
-00000f50: 2061 7265 2070 726f 7669 6469 6e67 2073   are providing s
-00000f60: 7570 706f 7274 206f 6e20 6047 6974 7465  upport on `Gitte
-00000f70: 7220 3c68 7474 7073 3a2f 2f67 6974 7465  r <https://gitte
-00000f80: 722e 696d 2f42 6c75 6542 7261 696e 2f43  r.im/BlueBrain/C
-00000f90: 7572 7265 6e74 7363 6170 653e 605f 2e20  urrentscape>`_. 
-00000fa0: 5765 2073 7567 6765 7374 2079 6f75 2063  We suggest you c
-00000fb0: 7265 6174 6520 7469 636b 6574 7320 6f6e  reate tickets on
-00000fc0: 2074 6865 2060 4769 7468 7562 2069 7373   the `Github iss
-00000fd0: 7565 2074 7261 636b 6572 203c 6874 7470  ue tracker <http
-00000fe0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f42  s://github.com/B
-00000ff0: 6c75 6542 7261 696e 2f43 7572 7265 6e74  lueBrain/Current
-00001000: 7363 6170 652f 6973 7375 6573 3e60 5f20  scape/issues>`_ 
-00001010: 696e 2063 6173 6520 796f 7520 656e 636f  in case you enco
-00001020: 756e 7465 7220 7072 6f62 6c65 6d73 2077  unter problems w
-00001030: 6869 6c65 2075 7369 6e67 2074 6865 2073  hile using the s
-00001040: 6f66 7477 6172 6520 6f72 2069 6620 796f  oftware or if yo
-00001050: 7520 6861 7665 2073 6f6d 6520 7375 6767  u have some sugg
-00001060: 6573 7469 6f6e 732e 0a0a 4d61 696e 2064  estions...Main d
-00001070: 6570 656e 6465 6e63 6965 730a 3d3d 3d3d  ependencies.====
-00001080: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 0a2d  =============..-
-00001090: 2060 5079 7468 6f6e 2033 2e37 2b20 3c68   `Python 3.7+ <h
-000010a0: 7474 7073 3a2f 2f77 7777 2e70 7974 686f  ttps://www.pytho
-000010b0: 6e2e 6f72 672f 646f 776e 6c6f 6164 732f  n.org/downloads/
-000010c0: 7265 6c65 6173 652f 7079 7468 6f6e 2d33  release/python-3
-000010d0: 3730 2f3e 605f 0a2d 2060 4e75 6d70 7920  70/>`_.- `Numpy 
-000010e0: 3c68 7474 7073 3a2f 2f6e 756d 7079 2e6f  <https://numpy.o
-000010f0: 7267 2f3e 605f 2028 6175 746f 6d61 7469  rg/>`_ (automati
-00001100: 6361 6c6c 7920 696e 7374 616c 6c65 6420  cally installed 
-00001110: 6279 2070 6970 290a 2d20 6050 616c 6574  by pip).- `Palet
-00001120: 7461 626c 6520 3c68 7474 7073 3a2f 2f67  table <https://g
-00001130: 6974 6875 622e 636f 6d2f 6a69 6666 7963  ithub.com/jiffyc
-00001140: 6c75 622f 7061 6c65 7474 6162 6c65 3e60  lub/palettable>`
-00001150: 5f20 2861 7574 6f6d 6174 6963 616c 6c79  _ (automatically
-00001160: 2069 6e73 7461 6c6c 6564 2062 7920 7069   installed by pi
-00001170: 7029 0a0a 496e 7374 616c 6c61 7469 6f6e  p)..Installation
-00001180: 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 0a43  .============..C
-00001190: 7572 7265 6e74 7363 6170 6520 6361 6e20  urrentscape can 
-000011a0: 6265 2070 6970 2069 6e73 7461 6c6c 6564  be pip installed
-000011b0: 2077 6974 6820 7468 6520 666f 6c6c 6f77   with the follow
-000011c0: 696e 6720 636f 6d6d 616e 643a 0a0a 2e2e  ing command:....
-000011d0: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
-000011e0: 7468 6f6e 0a0a 2020 2020 7069 7020 696e  thon..    pip in
-000011f0: 7374 616c 6c20 6375 7272 656e 7473 6361  stall currentsca
-00001200: 7065 0a0a 4966 2079 6f75 2077 616e 7420  pe..If you want 
-00001210: 746f 2062 6520 6162 6c65 2074 6f20 7275  to be able to ru
-00001220: 6e20 7468 6520 4375 7272 656e 7473 6361  n the Currentsca
-00001230: 7065 2065 7861 6d70 6c65 732c 2079 6f75  pe examples, you
-00001240: 2077 696c 6c20 6e65 6564 2074 6f20 616c   will need to al
-00001250: 736f 2069 6e73 7461 6c6c 2074 6865 2065  so install the e
-00001260: 7861 6d70 6c65 2064 6570 656e 6465 6e63  xample dependenc
-00001270: 6965 733a 0a0a 2e2e 2063 6f64 652d 626c  ies:.... code-bl
-00001280: 6f63 6b3a 3a20 7079 7468 6f6e 0a0a 2020  ock:: python..  
-00001290: 2020 7069 7020 696e 7374 616c 6c20 6375    pip install cu
-000012a0: 7272 656e 7473 6361 7065 5b65 7861 6d70  rrentscape[examp
-000012b0: 6c65 5d0a 0a51 7569 636b 2053 7461 7274  le]..Quick Start
-000012c0: 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a 4265  .===========..Be
-000012d0: 6c6f 7720 6973 2061 6e20 6578 616d 706c  low is an exampl
-000012e0: 6520 6f66 2061 2062 616c 6c20 616e 6420  e of a ball and 
-000012f0: 7374 6963 6b20 6d6f 6465 6c20 696e 204e  stick model in N
-00001300: 4555 524f 4e20 7769 7468 2073 696d 706c  EURON with simpl
-00001310: 6520 486f 6467 6b69 6e2d 4875 786c 6579  e Hodgkin-Huxley
-00001320: 206d 6563 6861 6e69 736d 732c 2074 6f20   mechanisms, to 
-00001330: 7768 6963 6820 6120 7374 6570 2073 7469  which a step sti
-00001340: 6d75 6c75 7320 6973 2061 7070 6c69 6564  mulus is applied
-00001350: 2e0a 0a54 6865 2076 6f6c 7461 6765 2061  ...The voltage a
-00001360: 6e64 2069 6f6e 6963 2063 7572 7265 6e74  nd ionic current
-00001370: 7320 6172 6520 7265 636f 7264 6564 2061  s are recorded a
-00001380: 6e64 2066 6564 2074 6f20 4375 7272 656e  nd fed to Curren
-00001390: 7473 6361 7065 2c20 616c 6f6e 6720 7769  tscape, along wi
-000013a0: 7468 2061 2063 6f6e 6669 6775 7261 7469  th a configurati
-000013b0: 6f6e 2064 6963 7469 6f6e 6172 7920 636f  on dictionary co
-000013c0: 6e74 6169 6e69 6e67 2074 6865 2063 7572  ntaining the cur
-000013d0: 7265 6e74 206e 616d 6573 2074 6f20 6265  rent names to be
-000013e0: 2064 6973 706c 6179 6564 2069 6e20 7468   displayed in th
-000013f0: 6520 6c65 6765 6e64 2e0a 0a54 6f20 7275  e legend...To ru
-00001400: 6e20 7468 6520 636f 6465 2079 6f75 2077  n the code you w
-00001410: 696c 6c20 6669 7273 7420 6861 7665 2074  ill first have t
-00001420: 6f20 696e 7374 616c 6c20 4e45 5552 4f4e  o install NEURON
-00001430: 2070 6163 6b61 6765 3a0a 0a2e 2e20 636f   package:.... co
-00001440: 6465 2d62 6c6f 636b 3a3a 2070 7974 686f  de-block:: pytho
-00001450: 6e0a 0a20 2020 2070 6970 2069 6e73 7461  n..    pip insta
-00001460: 6c6c 206e 6575 726f 6e0a 0a57 6865 6e20  ll neuron..When 
-00001470: 796f 7520 7468 656e 2065 7865 6375 7465  you then execute
-00001480: 2074 6865 2066 6f6c 6c6f 7769 6e67 2070   the following p
-00001490: 7974 686f 6e20 636f 6465 2c20 6120 7769  ython code, a wi
-000014a0: 6e64 6f77 2073 686f 756c 6420 6f70 656e  ndow should open
-000014b0: 2077 6974 6820 7468 6520 6375 7272 656e   with the curren
-000014c0: 7473 6361 7065 2070 6c6f 743a 0a0a 2e2e  tscape plot:....
-000014d0: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
-000014e0: 7468 6f6e 0a0a 2020 2020 696d 706f 7274  thon..    import
-000014f0: 206e 756d 7079 2061 7320 6e70 0a20 2020   numpy as np.   
-00001500: 2066 726f 6d20 6e65 7572 6f6e 2069 6d70   from neuron imp
-00001510: 6f72 7420 680a 2020 2020 6672 6f6d 206e  ort h.    from n
-00001520: 6575 726f 6e2e 756e 6974 7320 696d 706f  euron.units impo
-00001530: 7274 206d 732c 206d 560a 2020 2020 6672  rt ms, mV.    fr
-00001540: 6f6d 2063 7572 7265 6e74 7363 6170 652e  om currentscape.
-00001550: 6375 7272 656e 7473 6361 7065 2069 6d70  currentscape imp
-00001560: 6f72 7420 706c 6f74 5f63 7572 7265 6e74  ort plot_current
-00001570: 7363 6170 650a 0a20 2020 2068 2e6c 6f61  scape..    h.loa
-00001580: 645f 6669 6c65 2827 7374 6472 756e 2e68  d_file('stdrun.h
-00001590: 6f63 2729 0a0a 2020 2020 736f 6d61 203d  oc')..    soma =
-000015a0: 2068 2e53 6563 7469 6f6e 286e 616d 653d   h.Section(name=
-000015b0: 2773 6f6d 6127 290a 2020 2020 6465 6e64  'soma').    dend
-000015c0: 203d 2068 2e53 6563 7469 6f6e 286e 616d   = h.Section(nam
-000015d0: 653d 2764 656e 6427 290a 0a20 2020 2064  e='dend')..    d
-000015e0: 656e 642e 636f 6e6e 6563 7428 736f 6d61  end.connect(soma
-000015f0: 2831 2929 0a0a 2020 2020 736f 6d61 2e4c  (1))..    soma.L
-00001600: 203d 2073 6f6d 612e 6469 616d 203d 2031   = soma.diam = 1
-00001610: 322e 3631 3537 0a20 2020 2064 656e 642e  2.6157.    dend.
-00001620: 4c20 3d20 3230 300a 2020 2020 6465 6e64  L = 200.    dend
-00001630: 2e64 6961 6d20 3d20 310a 0a20 2020 2066  .diam = 1..    f
-00001640: 6f72 2073 6563 2069 6e20 682e 616c 6c73  or sec in h.alls
-00001650: 6563 2829 3a0a 2020 2020 2020 2020 7365  ec():.        se
-00001660: 632e 5261 203d 2031 3030 2020 2020 2320  c.Ra = 100    # 
-00001670: 4178 6961 6c20 7265 7369 7374 616e 6365  Axial resistance
-00001680: 2069 6e20 4f68 6d20 2a20 636d 0a20 2020   in Ohm * cm.   
-00001690: 2020 2020 2073 6563 2e63 6d20 3d20 3120       sec.cm = 1 
-000016a0: 2020 2020 2023 204d 656d 6272 616e 6520       # Membrane 
-000016b0: 6361 7061 6369 7461 6e63 6520 696e 206d  capacitance in m
-000016c0: 6963 726f 2046 6172 6164 7320 2f20 636d  icro Farads / cm
-000016d0: 5e32 0a0a 2020 2020 2320 496e 7365 7274  ^2..    # Insert
-000016e0: 2061 6374 6976 6520 486f 6467 6b69 6e2d   active Hodgkin-
-000016f0: 4875 786c 6579 2063 7572 7265 6e74 2069  Huxley current i
-00001700: 6e20 7468 6520 736f 6d61 0a20 2020 2073  n the soma.    s
-00001710: 6f6d 612e 696e 7365 7274 2827 6868 2729  oma.insert('hh')
-00001720: 0a20 2020 2066 6f72 2073 6567 2069 6e20  .    for seg in 
-00001730: 736f 6d61 3a0a 2020 2020 2020 2020 7365  soma:.        se
-00001740: 672e 6868 2e67 6e61 6261 7220 3d20 302e  g.hh.gnabar = 0.
-00001750: 3132 2020 2320 536f 6469 756d 2063 6f6e  12  # Sodium con
-00001760: 6475 6374 616e 6365 2069 6e20 532f 636d  ductance in S/cm
-00001770: 320a 2020 2020 2020 2020 7365 672e 6868  2.        seg.hh
-00001780: 2e67 6b62 6172 203d 2030 2e30 3336 2020  .gkbar = 0.036  
-00001790: 2320 506f 7461 7373 6975 6d20 636f 6e64  # Potassium cond
-000017a0: 7563 7461 6e63 6520 696e 2053 2f63 6d32  uctance in S/cm2
-000017b0: 0a20 2020 2020 2020 2073 6567 2e68 682e  .        seg.hh.
-000017c0: 676c 203d 2030 2e30 3030 3320 2020 2023  gl = 0.0003    #
-000017d0: 204c 6561 6b20 636f 6e64 7563 7461 6e63   Leak conductanc
-000017e0: 6520 696e 2053 2f63 6d32 0a20 2020 2020  e in S/cm2.     
-000017f0: 2020 2073 6567 2e68 682e 656c 203d 202d     seg.hh.el = -
-00001800: 3534 2e33 2020 2020 2023 2052 6576 6572  54.3     # Rever
-00001810: 7361 6c20 706f 7465 6e74 6961 6c20 696e  sal potential in
-00001820: 206d 560a 0a20 2020 2023 2049 6e73 6572   mV..    # Inser
-00001830: 7420 7061 7373 6976 6520 6375 7272 656e  t passive curren
-00001840: 7420 696e 2074 6865 2064 656e 6472 6974  t in the dendrit
-00001850: 650a 2020 2020 6465 6e64 2e69 6e73 6572  e.    dend.inser
-00001860: 7428 2770 6173 2729 0a20 2020 2066 6f72  t('pas').    for
-00001870: 2073 6567 2069 6e20 6465 6e64 3a0a 2020   seg in dend:.  
-00001880: 2020 2020 2020 7365 672e 7061 732e 6720        seg.pas.g 
-00001890: 3d20 302e 3030 3120 2023 2050 6173 7369  = 0.001  # Passi
-000018a0: 7665 2063 6f6e 6475 6374 616e 6365 2069  ve conductance i
-000018b0: 6e20 532f 636d 320a 2020 2020 2020 2020  n S/cm2.        
-000018c0: 7365 672e 7061 732e 6520 3d20 2d36 3520  seg.pas.e = -65 
-000018d0: 2020 2023 204c 6561 6b20 7265 7665 7273     # Leak revers
-000018e0: 616c 2070 6f74 656e 7469 616c 206d 560a  al potential mV.
-000018f0: 0a20 2020 2073 7469 6d20 3d20 682e 4943  .    stim = h.IC
-00001900: 6c61 6d70 2864 656e 6428 3129 290a 2020  lamp(dend(1)).  
-00001910: 2020 7374 696d 2e64 656c 6179 203d 2035    stim.delay = 5
-00001920: 0a20 2020 2073 7469 6d2e 6475 7220 3d20  .    stim.dur = 
-00001930: 3130 0a20 2020 2073 7469 6d2e 616d 7020  10.    stim.amp 
-00001940: 3d20 302e 310a 0a20 2020 2063 7572 7265  = 0.1..    curre
-00001950: 6e74 5f6e 616d 6573 203d 205b 2269 6b22  nt_names = ["ik"
-00001960: 2c20 2269 6e61 222c 2022 696c 5f68 6822  , "ina", "il_hh"
-00001970: 5d0a 2020 2020 745f 7665 6320 3d20 682e  ].    t_vec = h.
-00001980: 5665 6374 6f72 2829 0a20 2020 2076 5f76  Vector().    v_v
-00001990: 6563 203d 2068 2e56 6563 746f 7228 290a  ec = h.Vector().
-000019a0: 2020 2020 696b 5f76 6563 203d 2068 2e56      ik_vec = h.V
-000019b0: 6563 746f 7228 290a 2020 2020 696e 615f  ector().    ina_
-000019c0: 7665 6320 3d20 682e 5665 6374 6f72 2829  vec = h.Vector()
-000019d0: 0a20 2020 2069 6c5f 7665 6320 3d20 682e  .    il_vec = h.
-000019e0: 5665 6374 6f72 2829 0a20 2020 2074 5f76  Vector().    t_v
-000019f0: 6563 2e72 6563 6f72 6428 682e 5f72 6566  ec.record(h._ref
-00001a00: 5f74 290a 2020 2020 765f 7665 632e 7265  _t).    v_vec.re
-00001a10: 636f 7264 2873 6f6d 6128 302e 3529 2e5f  cord(soma(0.5)._
-00001a20: 7265 665f 7629 0a20 2020 2069 6b5f 7665  ref_v).    ik_ve
-00001a30: 632e 7265 636f 7264 2873 6f6d 6128 302e  c.record(soma(0.
-00001a40: 3529 2e5f 7265 665f 696b 290a 2020 2020  5)._ref_ik).    
-00001a50: 696e 615f 7665 632e 7265 636f 7264 2873  ina_vec.record(s
-00001a60: 6f6d 6128 302e 3529 2e5f 7265 665f 696e  oma(0.5)._ref_in
-00001a70: 6129 0a20 2020 2069 6c5f 7665 632e 7265  a).    il_vec.re
-00001a80: 636f 7264 2873 6f6d 6128 302e 3529 2e5f  cord(soma(0.5)._
-00001a90: 7265 665f 696c 5f68 6829 0a0a 2020 2020  ref_il_hh)..    
-00001aa0: 682e 6669 6e69 7469 616c 697a 6528 2d36  h.finitialize(-6
-00001ab0: 3520 2a20 6d56 290a 2020 2020 682e 636f  5 * mV).    h.co
-00001ac0: 6e74 696e 7565 7275 6e28 3235 202a 206d  ntinuerun(25 * m
-00001ad0: 7329 0a0a 2020 2020 746f 5f70 4120 3d20  s)..    to_pA = 
-00001ae0: 3130 202a 2073 6f6d 6128 302e 3529 2e61  10 * soma(0.5).a
-00001af0: 7265 6128 2920 2320 7475 726e 206d 412f  rea() # turn mA/
-00001b00: 636d 3220 282a 756d 3229 2069 6e74 6f20  cm2 (*um2) into 
-00001b10: 7041 0a20 2020 2076 6f6c 7461 6765 203d  pA.    voltage =
-00001b20: 206e 702e 6173 6172 7261 7928 765f 7665   np.asarray(v_ve
-00001b30: 6329 0a20 2020 2070 6f74 6173 7369 756d  c).    potassium
-00001b40: 203d 206e 702e 6173 6172 7261 7928 696b   = np.asarray(ik
-00001b50: 5f76 6563 2920 2a20 746f 5f70 410a 2020  _vec) * to_pA.  
-00001b60: 2020 736f 6469 756d 203d 206e 702e 6173    sodium = np.as
-00001b70: 6172 7261 7928 696e 615f 7665 6329 202a  array(ina_vec) *
-00001b80: 2074 6f5f 7041 0a20 2020 206c 6561 6b20   to_pA.    leak 
-00001b90: 3d20 6e70 2e61 7361 7272 6179 2869 6c5f  = np.asarray(il_
-00001ba0: 7665 6329 202a 2074 6f5f 7041 0a0a 2020  vec) * to_pA..  
-00001bb0: 2020 636f 6e66 6967 203d 207b 0a20 2020    config = {.   
-00001bc0: 2020 2020 2022 6f75 7470 7574 223a 207b       "output": {
-00001bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c10: 2020 2020 0a20 2020 2020 2020 2020 2022      .          "
-00001c20: 7361 7665 6669 6722 3a20 5472 7565 2c20  savefig": True, 
-00001c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c60: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
-00001c70: 2020 2020 2022 6469 7222 3a20 222e 222c       "dir": ".",
-00001c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001cc0: 0a20 2020 2020 2020 2020 2022 666e 616d  .          "fnam
-00001cd0: 6522 3a20 2271 7569 636b 7374 6172 745f  e": "quickstart_
-00001ce0: 706c 6f74 222c 2020 2020 2020 2020 2020  plot",          
-00001cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d10: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
-00001d20: 2022 6578 7465 6e73 696f 6e22 3a20 2270   "extension": "p
-00001d30: 6e67 222c 2020 2020 2020 2020 2020 2020  ng",            
-00001d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d60: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
-00001d70: 2020 2020 2020 2022 6470 6922 3a20 3330         "dpi": 30
-00001d80: 302c 2020 2020 2020 2020 2020 2020 2020  0,              
-00001d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001dc0: 2020 0a20 2020 2020 2020 2020 2022 7472    .          "tr
-00001dd0: 616e 7370 6172 656e 7422 3a20 4661 6c73  ansparent": Fals
-00001de0: 6520 2020 2020 2020 2020 2020 2020 2020  e               
-00001df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e10: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00001e20: 207d 2c20 2020 0a20 2020 2020 2020 2022   },   .        "
-00001e30: 6375 7272 656e 7422 3a20 7b22 6e61 6d65  current": {"name
-00001e40: 7322 3a20 6375 7272 656e 745f 6e61 6d65  s": current_name
-00001e50: 737d 2c0a 2020 2020 2020 2020 2276 6f6c  s},.        "vol
-00001e60: 7461 6765 223a 207b 2279 6c69 6d22 3a20  tage": {"ylim": 
-00001e70: 5b2d 3930 2c20 3530 5d7d 2c0a 2020 2020  [-90, 50]},.    
-00001e80: 2020 2020 226c 6567 656e 6474 6578 7473      "legendtexts
-00001e90: 697a 6522 3a20 352c 0a20 2020 207d 0a20  ize": 5,.    }. 
-00001ea0: 2020 2066 6967 203d 2070 6c6f 745f 6375     fig = plot_cu
-00001eb0: 7272 656e 7473 6361 7065 2876 6f6c 7461  rrentscape(volta
-00001ec0: 6765 2c20 5b70 6f74 6173 7369 756d 2c20  ge, [potassium, 
-00001ed0: 736f 6469 756d 2c20 6c65 616b 5d2c 2063  sodium, leak], c
-00001ee0: 6f6e 6669 6729 0a20 2020 2066 6967 2e73  onfig).    fig.s
-00001ef0: 686f 7728 290a 0a57 6865 6e20 796f 7520  how()..When you 
-00001f00: 7275 6e20 7468 6973 2063 6f64 6520 696e  run this code in
-00001f10: 2050 7974 686f 6e2c 2069 7420 7769 6c6c   Python, it will
-00001f20: 2067 656e 6572 6174 6520 7468 6520 666f   generate the fo
-00001f30: 6c6c 6f77 696e 6720 6375 7272 656e 7473  llowing currents
-00001f40: 6361 7065 2070 6c6f 7420 2869 6e20 6120  cape plot (in a 
-00001f50: 7769 6e64 6f77 2c20 616e 6420 6f6e 2064  window, and on d
-00001f60: 6973 6b20 6173 2071 7569 636b 7374 6172  isk as quickstar
-00001f70: 745f 706c 6f74 2e70 6e67 293a 0a0a 2e2e  t_plot.png):....
-00001f80: 2069 6d61 6765 3a3a 2064 6f63 2f73 6f75   image:: doc/sou
-00001f90: 7263 652f 696d 6167 6573 2f71 7569 636b  rce/images/quick
-00001fa0: 7374 6172 745f 706c 6f74 2e70 6e67 0a0a  start_plot.png..
-00001fb0: 5475 746f 7269 616c 0a3d 3d3d 3d3d 3d3d  Tutorial.=======
-00001fc0: 3d0a 0a41 206d 6f72 6520 6465 7461 696c  =..A more detail
-00001fd0: 6564 2065 7870 6c61 6e61 7469 6f6e 206f  ed explanation o
-00001fe0: 6e20 686f 7720 746f 2075 7365 2043 7572  n how to use Cur
-00001ff0: 7265 6e74 7363 6170 652c 2061 7320 7765  rentscape, as we
-00002000: 6c6c 2061 7320 6f74 6865 7220 6578 616d  ll as other exam
-00002010: 706c 6573 2063 616e 2062 6520 666f 756e  ples can be foun
-00002020: 6420 6f6e 2074 6865 2060 7475 746f 7269  d on the `tutori
-00002030: 616c 2070 6167 6520 3c54 7574 6f72 6961  al page <Tutoria
-00002040: 6c2e 7273 743e 605f 2e0a 0a41 5049 2044  l.rst>`_...API D
-00002050: 6f63 756d 656e 7461 7469 6f6e 0a3d 3d3d  ocumentation.===
-00002060: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a  ==============..
-00002070: 5468 6520 4150 4920 646f 6375 6d65 6e74  The API document
-00002080: 6174 696f 6e20 6361 6e20 6265 2066 6f75  ation can be fou
-00002090: 6e64 206f 6e20 6052 6561 6454 6865 446f  nd on `ReadTheDo
-000020a0: 6373 203c 2268 7474 7073 3a2f 2f63 7572  cs <"https://cur
-000020b0: 7265 6e74 7363 6170 652e 7265 6164 7468  rentscape.readth
-000020c0: 6564 6f63 732e 696f 223e 605f 2e0a 0a46  edocs.io">`_...F
-000020d0: 756e 6469 6e67 2026 2041 636b 6e6f 776c  unding & Acknowl
-000020e0: 6564 6765 6d65 6e74 730a 3d3d 3d3d 3d3d  edgements.======
-000020f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00002100: 3d3d 3d3d 0a0a 5765 2077 6973 6820 746f  ====..We wish to
-00002110: 2074 6861 6e6b 2074 6865 2061 7574 686f   thank the autho
-00002120: 7273 206f 6620 6041 6c6f 6e73 6f20 616e  rs of `Alonso an
-00002130: 6420 4d61 7264 6572 2c20 3230 3139 203c  d Marder, 2019 <
-00002140: 6874 7470 733a 2f2f 646f 692e 6f72 672f  https://doi.org/
-00002150: 3130 2e37 3535 342f 654c 6966 652e 3432  10.7554/eLife.42
-00002160: 3732 323e 605f 2074 6f20 6c65 7420 7573  722>`_ to let us
-00002170: 2069 6e74 6567 7261 7465 2061 2070 6172   integrate a par
-00002180: 7420 6f66 2074 6865 6972 2060 636f 6465  t of their `code
-00002190: 203c 6874 7470 733a 2f2f 6461 7461 6472   <https://datadr
-000021a0: 7961 642e 6f72 672f 7374 6173 682f 6461  yad.org/stash/da
-000021b0: 7461 7365 742f 646f 693a 3130 2e35 3036  taset/doi:10.506
-000021c0: 312f 6472 7961 642e 6430 3737 396d 623e  1/dryad.d0779mb>
-000021d0: 605f 2069 6e74 6f20 7468 6973 2072 6570  `_ into this rep
-000021e0: 6f73 6974 6f72 792e 0a0a 5468 6520 7061  ository...The pa
-000021f0: 7274 206f 6620 7468 6520 636f 6465 2069  rt of the code i
-00002200: 6e20 7468 6973 2072 6570 6f73 6974 6f72  n this repositor
-00002210: 7920 6465 7665 6c6f 7065 6420 6279 2074  y developed by t
-00002220: 6865 2045 5046 4c20 426c 7565 2042 7261  he EPFL Blue Bra
-00002230: 696e 2050 726f 6a65 6374 2077 6173 2073  in Project was s
-00002240: 7570 706f 7274 6564 2062 7920 6675 6e64  upported by fund
-00002250: 696e 6720 746f 2074 6865 2042 6c75 6520  ing to the Blue 
-00002260: 4272 6169 6e20 5072 6f6a 6563 742c 2061  Brain Project, a
-00002270: 2072 6573 6561 7263 6820 6365 6e74 6572   research center
-00002280: 206f 6620 7468 6520 c389 636f 6c65 2070   of the ..cole p
-00002290: 6f6c 7974 6563 686e 6971 7565 2066 c3a9  olytechnique f..
-000022a0: 64c3 a972 616c 6520 6465 204c 6175 7361  d..rale de Lausa
-000022b0: 6e6e 6520 2845 5046 4c29 2c20 6672 6f6d  nne (EPFL), from
-000022c0: 2074 6865 2053 7769 7373 2067 6f76 6572   the Swiss gover
-000022d0: 6e6d 656e 7427 7320 4554 4820 426f 6172  nment's ETH Boar
-000022e0: 6420 6f66 2074 6865 2053 7769 7373 2046  d of the Swiss F
-000022f0: 6564 6572 616c 2049 6e73 7469 7475 7465  ederal Institute
-00002300: 7320 6f66 2054 6563 686e 6f6c 6f67 792e  s of Technology.
-00002310: 0a                                       .
+00000010: 3d3d 3d3d 3d3d 3d3d 3d0a 0a0a 2b2d 2d2d  =========...+---
+00000020: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+00000030: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 4c61  ----------+.| La
+00000040: 7465 7374 2052 656c 6561 7365 207c 207c  test Release | |
+00000050: 7079 7069 7c20 2020 2020 7c0a 2b2d 2d2d  pypi|     |.+---
+00000060: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+00000070: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 446f  ----------+.| Do
+00000080: 6375 6d65 6e74 6174 696f 6e20 207c 207c  cumentation  | |
+00000090: 646f 6373 7c20 2020 2020 7c0a 2b2d 2d2d  docs|     |.+---
+000000a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+000000b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 4c69  ----------+.| Li
+000000c0: 6365 6e73 6520 2020 2020 2020 207c 207c  cense        | |
+000000d0: 6c69 6365 6e73 657c 2020 7c0a 2b2d 2d2d  license|  |.+---
+000000e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+000000f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 4275  ----------+.| Bu
+00000100: 696c 6420 5374 6174 7573 2009 207c 207c  ild Status . | |
+00000110: 6275 696c 647c 2020 2020 7c0a 2b2d 2d2d  build|    |.+---
+00000120: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+00000130: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 436f  ----------+.| Co
+00000140: 7665 7261 6765 2020 2020 2020 207c 207c  verage       | |
+00000150: 636f 7665 7261 6765 7c20 7c0a 2b2d 2d2d  coverage| |.+---
+00000160: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+00000170: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 4769  ----------+.| Gi
+00000180: 7474 6572 2020 2020 2020 2020 207c 207c  tter         | |
+00000190: 6769 7474 6572 7c20 2020 7c0a 2b2d 2d2d  gitter|   |.+---
+000001a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+000001b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 0a49 6e74  ----------+..Int
+000001c0: 726f 6475 6374 696f 6e0a 3d3d 3d3d 3d3d  roduction.======
+000001d0: 3d3d 3d3d 3d3d 0a0a 4375 7272 656e 7473  ======..Currents
+000001e0: 6361 7065 2069 7320 6120 5079 7468 6f6e  cape is a Python
+000001f0: 2074 6f6f 6c20 656e 6162 6c69 6e67 2073   tool enabling s
+00000200: 6369 656e 7469 7374 7320 746f 2065 6173  cientists to eas
+00000210: 696c 7920 706c 6f74 2074 6865 2063 7572  ily plot the cur
+00000220: 7265 6e74 7320 696e 2065 6c65 6374 7269  rents in electri
+00000230: 6361 6c20 6e65 7572 6f6e 206d 6f64 656c  cal neuron model
+00000240: 732e 0a54 6865 2063 6f64 6520 6973 2062  s..The code is b
+00000250: 6173 6564 206f 6e20 7468 6520 7061 7065  ased on the pape
+00000260: 7220 6041 6c6f 6e73 6f20 616e 6420 4d61  r `Alonso and Ma
+00000270: 7264 6572 2c20 3230 3139 203c 6874 7470  rder, 2019 <http
+00000280: 733a 2f2f 646f 692e 6f72 672f 3130 2e37  s://doi.org/10.7
+00000290: 3535 342f 654c 6966 652e 3432 3732 323e  554/eLife.42722>
+000002a0: 605f 5f2e 0a0a 4375 7272 656e 7473 6361  `__...Currentsca
+000002b0: 7065 2066 6967 7572 6573 2070 6c6f 7420  pe figures plot 
+000002c0: 7468 6520 7065 7263 656e 7461 6765 206f  the percentage o
+000002d0: 6620 696e 7761 7264 2061 6e64 206f 7574  f inward and out
+000002e0: 7761 7264 2069 6f6e 6963 206d 656d 6272  ward ionic membr
+000002f0: 616e 6520 6375 7272 656e 7473 2c0a 7468  ane currents,.th
+00000300: 6520 746f 7461 6c20 696e 7761 7264 2061  e total inward a
+00000310: 6e64 206f 7574 7761 7264 2063 7572 7265  nd outward curre
+00000320: 6e74 732c 2061 7320 7765 6c6c 2061 7320  nts, as well as 
+00000330: 7468 6520 766f 6c74 6167 6520 696e 2066  the voltage in f
+00000340: 756e 6374 696f 6e20 6f66 2074 696d 652e  unction of time.
+00000350: 0a49 7420 616c 6c6f 7773 206d 6f64 656c  .It allows model
+00000360: 6c65 7273 2074 6f20 7365 6520 7768 6963  lers to see whic
+00000370: 6820 6375 7272 656e 7473 2070 6c61 7920  h currents play 
+00000380: 6120 726f 6c65 2061 7420 616e 7920 6769  a role at any gi
+00000390: 7665 6e20 7469 6d65 2064 7572 696e 6720  ven time during 
+000003a0: 6120 7369 6d75 6c61 7469 6f6e 2c20 616e  a simulation, an
+000003b0: 6420 6368 6563 6b20 696e 2064 6570 7468  d check in depth
+000003c0: 2074 6865 2063 7572 7265 6e74 2064 796e   the current dyn
+000003d0: 616d 6963 732e 0a0a 2e2e 2069 6d61 6765  amics..... image
+000003e0: 3a3a 2064 6f63 2f73 6f75 7263 652f 696d  :: doc/source/im
+000003f0: 6167 6573 2f70 6c6f 742e 706e 670a 0a43  ages/plot.png..C
+00000400: 6974 6174 696f 6e0a 3d3d 3d3d 3d3d 3d3d  itation.========
+00000410: 0a0a 5768 656e 2079 6f75 2075 7365 2074  ..When you use t
+00000420: 6869 7320 4375 7272 656e 7473 6361 7065  his Currentscape
+00000430: 2073 6f66 7477 6172 6520 666f 7220 796f   software for yo
+00000440: 7572 2072 6573 6561 7263 682c 2077 6520  ur research, we 
+00000450: 6173 6b20 796f 7520 746f 2063 6974 6520  ask you to cite 
+00000460: 7468 6520 666f 6c6c 6f77 696e 6720 7075  the following pu
+00000470: 626c 6963 6174 696f 6e20 2874 6869 7320  blication (this 
+00000480: 696e 636c 7564 6573 2070 6f73 7465 7220  includes poster 
+00000490: 7072 6573 656e 7461 7469 6f6e 7329 3a0a  presentations):.
+000004a0: 0a2e 2e20 636f 6465 2d62 6c6f 636b 3a3a  ... code-block::
+000004b0: 200a 0a20 2020 2040 6172 7469 636c 6520   ..    @article 
+000004c0: 7b31 302e 3735 3534 2f65 4c69 6665 2e34  {10.7554/eLife.4
+000004d0: 3237 3232 2c0a 2020 2020 6172 7469 636c  2722,.    articl
+000004e0: 655f 7479 7065 203d 207b 6a6f 7572 6e61  e_type = {journa
+000004f0: 6c7d 2c0a 2020 2020 7469 746c 6520 3d20  l},.    title = 
+00000500: 7b56 6973 7561 6c69 7a61 7469 6f6e 206f  {Visualization o
+00000510: 6620 6375 7272 656e 7473 2069 6e20 6e65  f currents in ne
+00000520: 7572 616c 206d 6f64 656c 7320 7769 7468  ural models with
+00000530: 2073 696d 696c 6172 2062 6568 6176 696f   similar behavio
+00000540: 7220 616e 6420 6469 6666 6572 656e 7420  r and different 
+00000550: 636f 6e64 7563 7461 6e63 6520 6465 6e73  conductance dens
+00000560: 6974 6965 737d 2c0a 2020 2020 6175 7468  ities},.    auth
+00000570: 6f72 203d 207b 416c 6f6e 736f 2c20 4c65  or = {Alonso, Le
+00000580: 616e 6472 6f20 4d20 616e 6420 4d61 7264  andro M and Mard
+00000590: 6572 2c20 4576 657d 2c0a 2020 2020 6564  er, Eve},.    ed
+000005a0: 6974 6f72 203d 207b 5765 7374 6272 6f6f  itor = {Westbroo
+000005b0: 6b2c 2047 6172 7920 4c20 616e 6420 536b  k, Gary L and Sk
+000005c0: 696e 6e65 722c 2046 7261 6e63 6573 204b  inner, Frances K
+000005d0: 2061 6e64 204c 616e 6b61 7261 6e79 2c20   and Lankarany, 
+000005e0: 4d69 6c61 6420 616e 6420 4272 6974 746f  Milad and Britto
+000005f0: 6e2c 204f 6c69 7665 727d 2c0a 2020 2020  n, Oliver},.    
+00000600: 766f 6c75 6d65 203d 2038 2c0a 2020 2020  volume = 8,.    
+00000610: 7965 6172 203d 2032 3031 392c 0a20 2020  year = 2019,.   
+00000620: 206d 6f6e 7468 203d 207b 6a61 6e7d 2c0a   month = {jan},.
+00000630: 2020 2020 7075 625f 6461 7465 203d 207b      pub_date = {
+00000640: 3230 3139 2d30 312d 3331 7d2c 0a20 2020  2019-01-31},.   
+00000650: 2070 6167 6573 203d 207b 6534 3237 3232   pages = {e42722
+00000660: 7d2c 0a20 2020 2063 6974 6174 696f 6e20  },.    citation 
+00000670: 3d20 7b65 4c69 6665 2032 3031 393b 383a  = {eLife 2019;8:
+00000680: 6534 3237 3232 7d2c 0a20 2020 2064 6f69  e42722},.    doi
+00000690: 203d 207b 3130 2e37 3535 342f 654c 6966   = {10.7554/eLif
+000006a0: 652e 3432 3732 327d 2c0a 2020 2020 7572  e.42722},.    ur
+000006b0: 6c20 3d20 7b68 7474 7073 3a2f 2f64 6f69  l = {https://doi
+000006c0: 2e6f 7267 2f31 302e 3735 3534 2f65 4c69  .org/10.7554/eLi
+000006d0: 6665 2e34 3237 3232 7d2c 0a20 2020 2061  fe.42722},.    a
+000006e0: 6273 7472 6163 7420 3d20 7b43 6f6e 6475  bstract = {Condu
+000006f0: 6374 616e 6365 2d62 6173 6564 206d 6f64  ctance-based mod
+00000700: 656c 7320 6f66 206e 6575 7261 6c20 6163  els of neural ac
+00000710: 7469 7669 7479 2070 726f 6475 6365 206c  tivity produce l
+00000720: 6172 6765 2061 6d6f 756e 7473 206f 6620  arge amounts of 
+00000730: 6461 7461 2074 6861 7420 6361 6e20 6265  data that can be
+00000740: 2068 6172 6420 746f 2076 6973 7561 6c69   hard to visuali
+00000750: 7a65 2061 6e64 2069 6e74 6572 7072 6574  ze and interpret
+00000760: 2e20 5765 2069 6e74 726f 6475 6365 2076  . We introduce v
+00000770: 6973 7561 6c69 7a61 7469 6f6e 206d 6574  isualization met
+00000780: 686f 6473 2074 6f20 6469 7370 6c61 7920  hods to display 
+00000790: 7468 6520 6479 6e61 6d69 6373 206f 6620  the dynamics of 
+000007a0: 7468 6520 696f 6e69 6320 6375 7272 656e  the ionic curren
+000007b0: 7473 2061 6e64 2074 6f20 6469 7370 6c61  ts and to displa
+000007c0: 7920 7468 6520 6d6f 6465 6c73 e280 9920  y the models... 
+000007d0: 7265 7370 6f6e 7365 2074 6f20 7065 7274  response to pert
+000007e0: 7572 6261 7469 6f6e 732e 2054 6f20 7669  urbations. To vi
+000007f0: 7375 616c 697a 6520 7468 6520 6375 7272  sualize the curr
+00000800: 656e 7473 e280 9920 6479 6e61 6d69 6373  ents... dynamics
+00000810: 2c20 7765 2063 6f6d 7075 7465 2074 6865  , we compute the
+00000820: 2070 6572 6365 6e74 2063 6f6e 7472 6962   percent contrib
+00000830: 7574 696f 6e20 6f66 2065 6163 6820 6375  ution of each cu
+00000840: 7272 656e 7420 616e 6420 6469 7370 6c61  rrent and displa
+00000850: 7920 7468 656d 206f 7665 7220 7469 6d65  y them over time
+00000860: 2075 7369 6e67 2073 7461 636b 6564 2d61   using stacked-a
+00000870: 7265 6120 706c 6f74 732e 2054 6865 2077  rea plots. The w
+00000880: 6176 6566 6f72 6d20 6f66 2074 6865 206d  aveform of the m
+00000890: 656d 6272 616e 6520 706f 7465 6e74 6961  embrane potentia
+000008a0: 6c20 616e 6420 7468 6520 636f 6e74 7269  l and the contri
+000008b0: 6275 7469 6f6e 206f 6620 6561 6368 2063  bution of each c
+000008c0: 7572 7265 6e74 2063 6861 6e67 6520 6173  urrent change as
+000008d0: 2074 6865 206d 6f64 656c 7320 6172 6520   the models are 
+000008e0: 7065 7274 7572 6265 642e 2054 6f20 7265  perturbed. To re
+000008f0: 7072 6573 656e 7420 7468 6573 6520 6368  present these ch
+00000900: 616e 6765 7320 6f76 6572 2061 2072 616e  anges over a ran
+00000910: 6765 206f 6620 7468 6520 7065 7274 7572  ge of the pertur
+00000920: 6261 7469 6f6e 2063 6f6e 7472 6f6c 2070  bation control p
+00000930: 6172 616d 6574 6572 2c20 7765 2063 6f6d  arameter, we com
+00000940: 7075 7465 2061 6e64 2064 6973 706c 6179  pute and display
+00000950: 2074 6865 2064 6973 7472 6962 7574 696f   the distributio
+00000960: 6e73 206f 6620 7468 6573 6520 7761 7665  ns of these wave
+00000970: 666f 726d 732e 2057 6520 696c 6c75 7374  forms. We illust
+00000980: 7261 7465 2074 6865 7365 2070 726f 6365  rate these proce
+00000990: 6475 7265 7320 696e 2073 6978 2065 7861  dures in six exa
+000009a0: 6d70 6c65 7320 6f66 2062 7572 7374 696e  mples of burstin
+000009b0: 6720 6d6f 6465 6c20 6e65 7572 6f6e 7320  g model neurons 
+000009c0: 7769 7468 2073 696d 696c 6172 2061 6374  with similar act
+000009d0: 6976 6974 7920 6275 7420 7468 6174 2064  ivity but that d
+000009e0: 6966 6665 7220 6173 206d 7563 6820 6173  iffer as much as
+000009f0: 2074 6872 6565 666f 6c64 2069 6e20 7468   threefold in th
+00000a00: 6569 7220 636f 6e64 7563 7461 6e63 6520  eir conductance 
+00000a10: 6465 6e73 6974 6965 732e 2054 6865 7365  densities. These
+00000a20: 2076 6973 7561 6c69 7a61 7469 6f6e 206d   visualization m
+00000a30: 6574 686f 6473 2070 726f 7669 6465 2068  ethods provide h
+00000a40: 6575 7269 7374 6963 2069 6e73 6967 6874  euristic insight
+00000a50: 2069 6e74 6f20 7768 7920 696e 6469 7669   into why indivi
+00000a60: 6475 616c 206e 6575 726f 6e73 206f 7220  dual neurons or 
+00000a70: 6e65 7477 6f72 6b73 2077 6974 6820 7369  networks with si
+00000a80: 6d69 6c61 7220 6265 6861 7669 6f72 2063  milar behavior c
+00000a90: 616e 2072 6573 706f 6e64 2077 6964 656c  an respond widel
+00000aa0: 7920 6469 6666 6572 656e 746c 7920 746f  y differently to
+00000ab0: 2070 6572 7475 7262 6174 696f 6e73 2e7d   perturbations.}
+00000ac0: 2c0a 2020 2020 6b65 7977 6f72 6473 203d  ,.    keywords =
+00000ad0: 207b 6e65 7572 6f6e 616c 206f 7363 696c   {neuronal oscil
+00000ae0: 6c61 746f 7273 2c20 4e61 2b20 6368 616e  lators, Na+ chan
+00000af0: 6e65 6c73 2c20 4361 2b2b 2063 6861 6e6e  nels, Ca++ chann
+00000b00: 656c 732c 204b 2b20 6368 616e 6e65 6c73  els, K+ channels
+00000b10: 2c20 636f 6e64 7563 7461 6e63 652d 6261  , conductance-ba
+00000b20: 7365 642c 2069 6f6e 6963 2063 6861 6e6e  sed, ionic chann
+00000b30: 656c 737d 2c0a 2020 2020 6a6f 7572 6e61  els},.    journa
+00000b40: 6c20 3d20 7b65 4c69 6665 7d2c 0a20 2020  l = {eLife},.   
+00000b50: 2069 7373 6e20 3d20 7b32 3035 302d 3038   issn = {2050-08
+00000b60: 3458 7d2c 0a20 2020 2070 7562 6c69 7368  4X},.    publish
+00000b70: 6572 203d 207b 654c 6966 6520 5363 6965  er = {eLife Scie
+00000b80: 6e63 6573 2050 7562 6c69 6361 7469 6f6e  nces Publication
+00000b90: 732c 204c 7464 7d2c 0a20 2020 207d 0a0a  s, Ltd},.    }..
+00000ba0: 5375 7070 6f72 740a 3d3d 3d3d 3d3d 3d0a  Support.=======.
+00000bb0: 0a57 6520 6172 6520 7072 6f76 6964 696e  .We are providin
+00000bc0: 6720 7375 7070 6f72 7420 6f6e 2060 4769  g support on `Gi
+00000bd0: 7474 6572 203c 6874 7470 733a 2f2f 6769  tter <https://gi
+00000be0: 7474 6572 2e69 6d2f 426c 7565 4272 6169  tter.im/BlueBrai
+00000bf0: 6e2f 4375 7272 656e 7473 6361 7065 3e60  n/Currentscape>`
+00000c00: 5f2e 2057 6520 7375 6767 6573 7420 796f  _. We suggest yo
+00000c10: 7520 6372 6561 7465 2074 6963 6b65 7473  u create tickets
+00000c20: 206f 6e20 7468 6520 6047 6974 6875 6220   on the `Github 
+00000c30: 6973 7375 6520 7472 6163 6b65 7220 3c68  issue tracker <h
+00000c40: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000c50: 6d2f 426c 7565 4272 6169 6e2f 4375 7272  m/BlueBrain/Curr
+00000c60: 656e 7473 6361 7065 2f69 7373 7565 733e  entscape/issues>
+00000c70: 605f 2069 6e20 6361 7365 2079 6f75 2065  `_ in case you e
+00000c80: 6e63 6f75 6e74 6572 2070 726f 626c 656d  ncounter problem
+00000c90: 7320 7768 696c 6520 7573 696e 6720 7468  s while using th
+00000ca0: 6520 736f 6674 7761 7265 206f 7220 6966  e software or if
+00000cb0: 2079 6f75 2068 6176 6520 736f 6d65 2073   you have some s
+00000cc0: 7567 6765 7374 696f 6e73 2e0a 0a4d 6169  uggestions...Mai
+00000cd0: 6e20 6465 7065 6e64 656e 6369 6573 0a3d  n dependencies.=
+00000ce0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000cf0: 0a0a 2d20 6050 7974 686f 6e20 332e 372b  ..- `Python 3.7+
+00000d00: 203c 6874 7470 733a 2f2f 7777 772e 7079   <https://www.py
+00000d10: 7468 6f6e 2e6f 7267 2f64 6f77 6e6c 6f61  thon.org/downloa
+00000d20: 6473 2f72 656c 6561 7365 2f70 7974 686f  ds/release/pytho
+00000d30: 6e2d 3337 302f 3e60 5f0a 2d20 604e 756d  n-370/>`_.- `Num
+00000d40: 7079 203c 6874 7470 733a 2f2f 6e75 6d70  py <https://nump
+00000d50: 792e 6f72 672f 3e60 5f20 2861 7574 6f6d  y.org/>`_ (autom
+00000d60: 6174 6963 616c 6c79 2069 6e73 7461 6c6c  atically install
+00000d70: 6564 2062 7920 7069 7029 0a2d 2060 5061  ed by pip).- `Pa
+00000d80: 6c65 7474 6162 6c65 203c 6874 7470 733a  lettable <https:
+00000d90: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 6966  //github.com/jif
+00000da0: 6679 636c 7562 2f70 616c 6574 7461 626c  fyclub/palettabl
+00000db0: 653e 605f 2028 6175 746f 6d61 7469 6361  e>`_ (automatica
+00000dc0: 6c6c 7920 696e 7374 616c 6c65 6420 6279  lly installed by
+00000dd0: 2070 6970 290a 0a49 6e73 7461 6c6c 6174   pip)..Installat
+00000de0: 696f 6e0a 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ion.============
+00000df0: 0a0a 4375 7272 656e 7473 6361 7065 2063  ..Currentscape c
+00000e00: 616e 2062 6520 7069 7020 696e 7374 616c  an be pip instal
+00000e10: 6c65 6420 7769 7468 2074 6865 2066 6f6c  led with the fol
+00000e20: 6c6f 7769 6e67 2063 6f6d 6d61 6e64 3a0a  lowing command:.
+00000e30: 0a2e 2e20 636f 6465 2d62 6c6f 636b 3a3a  ... code-block::
+00000e40: 2070 7974 686f 6e0a 0a20 2020 2070 6970   python..    pip
+00000e50: 2069 6e73 7461 6c6c 2063 7572 7265 6e74   install current
+00000e60: 7363 6170 650a 0a49 6620 796f 7520 7761  scape..If you wa
+00000e70: 6e74 2074 6f20 6265 2061 626c 6520 746f  nt to be able to
+00000e80: 2072 756e 2074 6865 2043 7572 7265 6e74   run the Current
+00000e90: 7363 6170 6520 6578 616d 706c 6573 2c20  scape examples, 
+00000ea0: 796f 7520 7769 6c6c 206e 6565 6420 746f  you will need to
+00000eb0: 2061 6c73 6f20 696e 7374 616c 6c20 7468   also install th
+00000ec0: 6520 6578 616d 706c 6520 6465 7065 6e64  e example depend
+00000ed0: 656e 6369 6573 3a0a 0a2e 2e20 636f 6465  encies:.... code
+00000ee0: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0a  -block:: python.
+00000ef0: 0a20 2020 2070 6970 2069 6e73 7461 6c6c  .    pip install
+00000f00: 2063 7572 7265 6e74 7363 6170 655b 6578   currentscape[ex
+00000f10: 616d 706c 655d 0a0a 5175 6963 6b20 5374  ample]..Quick St
+00000f20: 6172 740a 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a  art.===========.
+00000f30: 0a42 656c 6f77 2069 7320 616e 2065 7861  .Below is an exa
+00000f40: 6d70 6c65 206f 6620 6120 6261 6c6c 2061  mple of a ball a
+00000f50: 6e64 2073 7469 636b 206d 6f64 656c 2069  nd stick model i
+00000f60: 6e20 4e45 5552 4f4e 2077 6974 6820 7369  n NEURON with si
+00000f70: 6d70 6c65 2048 6f64 676b 696e 2d48 7578  mple Hodgkin-Hux
+00000f80: 6c65 7920 6d65 6368 616e 6973 6d73 2c20  ley mechanisms, 
+00000f90: 746f 2077 6869 6368 2061 2073 7465 7020  to which a step 
+00000fa0: 7374 696d 756c 7573 2069 7320 6170 706c  stimulus is appl
+00000fb0: 6965 642e 0a0a 5468 6520 766f 6c74 6167  ied...The voltag
+00000fc0: 6520 616e 6420 696f 6e69 6320 6375 7272  e and ionic curr
+00000fd0: 656e 7473 2061 7265 2072 6563 6f72 6465  ents are recorde
+00000fe0: 6420 616e 6420 6665 6420 746f 2043 7572  d and fed to Cur
+00000ff0: 7265 6e74 7363 6170 652c 2061 6c6f 6e67  rentscape, along
+00001000: 2077 6974 6820 6120 636f 6e66 6967 7572   with a configur
+00001010: 6174 696f 6e20 6469 6374 696f 6e61 7279  ation dictionary
+00001020: 2063 6f6e 7461 696e 696e 6720 7468 6520   containing the 
+00001030: 6375 7272 656e 7420 6e61 6d65 7320 746f  current names to
+00001040: 2062 6520 6469 7370 6c61 7965 6420 696e   be displayed in
+00001050: 2074 6865 206c 6567 656e 642e 0a0a 546f   the legend...To
+00001060: 2072 756e 2074 6865 2063 6f64 6520 796f   run the code yo
+00001070: 7520 7769 6c6c 2066 6972 7374 2068 6176  u will first hav
+00001080: 6520 746f 2069 6e73 7461 6c6c 204e 4555  e to install NEU
+00001090: 524f 4e20 7061 636b 6167 653a 0a0a 2e2e  RON package:....
+000010a0: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
+000010b0: 7468 6f6e 0a0a 2020 2020 7069 7020 696e  thon..    pip in
+000010c0: 7374 616c 6c20 6e65 7572 6f6e 0a0a 5768  stall neuron..Wh
+000010d0: 656e 2079 6f75 2074 6865 6e20 6578 6563  en you then exec
+000010e0: 7574 6520 7468 6520 666f 6c6c 6f77 696e  ute the followin
+000010f0: 6720 7079 7468 6f6e 2063 6f64 652c 2061  g python code, a
+00001100: 2077 696e 646f 7720 7368 6f75 6c64 206f   window should o
+00001110: 7065 6e20 7769 7468 2074 6865 2063 7572  pen with the cur
+00001120: 7265 6e74 7363 6170 6520 706c 6f74 3a0a  rentscape plot:.
+00001130: 0a2e 2e20 636f 6465 2d62 6c6f 636b 3a3a  ... code-block::
+00001140: 2070 7974 686f 6e0a 0a20 2020 2069 6d70   python..    imp
+00001150: 6f72 7420 6e75 6d70 7920 6173 206e 700a  ort numpy as np.
+00001160: 2020 2020 6672 6f6d 206e 6575 726f 6e20      from neuron 
+00001170: 696d 706f 7274 2068 0a20 2020 2066 726f  import h.    fro
+00001180: 6d20 6e65 7572 6f6e 2e75 6e69 7473 2069  m neuron.units i
+00001190: 6d70 6f72 7420 6d73 2c20 6d56 0a20 2020  mport ms, mV.   
+000011a0: 2066 726f 6d20 6375 7272 656e 7473 6361   from currentsca
+000011b0: 7065 2e63 7572 7265 6e74 7363 6170 6520  pe.currentscape 
+000011c0: 696d 706f 7274 2070 6c6f 745f 6375 7272  import plot_curr
+000011d0: 656e 7473 6361 7065 0a0a 2020 2020 682e  entscape..    h.
+000011e0: 6c6f 6164 5f66 696c 6528 2773 7464 7275  load_file('stdru
+000011f0: 6e2e 686f 6327 290a 0a20 2020 2073 6f6d  n.hoc')..    som
+00001200: 6120 3d20 682e 5365 6374 696f 6e28 6e61  a = h.Section(na
+00001210: 6d65 3d27 736f 6d61 2729 0a20 2020 2064  me='soma').    d
+00001220: 656e 6420 3d20 682e 5365 6374 696f 6e28  end = h.Section(
+00001230: 6e61 6d65 3d27 6465 6e64 2729 0a0a 2020  name='dend')..  
+00001240: 2020 6465 6e64 2e63 6f6e 6e65 6374 2873    dend.connect(s
+00001250: 6f6d 6128 3129 290a 0a20 2020 2073 6f6d  oma(1))..    som
+00001260: 612e 4c20 3d20 736f 6d61 2e64 6961 6d20  a.L = soma.diam 
+00001270: 3d20 3132 2e36 3135 370a 2020 2020 6465  = 12.6157.    de
+00001280: 6e64 2e4c 203d 2032 3030 0a20 2020 2064  nd.L = 200.    d
+00001290: 656e 642e 6469 616d 203d 2031 0a0a 2020  end.diam = 1..  
+000012a0: 2020 666f 7220 7365 6320 696e 2068 2e61    for sec in h.a
+000012b0: 6c6c 7365 6328 293a 0a20 2020 2020 2020  llsec():.       
+000012c0: 2073 6563 2e52 6120 3d20 3130 3020 2020   sec.Ra = 100   
+000012d0: 2023 2041 7869 616c 2072 6573 6973 7461   # Axial resista
+000012e0: 6e63 6520 696e 204f 686d 202a 2063 6d0a  nce in Ohm * cm.
+000012f0: 2020 2020 2020 2020 7365 632e 636d 203d          sec.cm =
+00001300: 2031 2020 2020 2020 2320 4d65 6d62 7261   1      # Membra
+00001310: 6e65 2063 6170 6163 6974 616e 6365 2069  ne capacitance i
+00001320: 6e20 6d69 6372 6f20 4661 7261 6473 202f  n micro Farads /
+00001330: 2063 6d5e 320a 0a20 2020 2023 2049 6e73   cm^2..    # Ins
+00001340: 6572 7420 6163 7469 7665 2048 6f64 676b  ert active Hodgk
+00001350: 696e 2d48 7578 6c65 7920 6375 7272 656e  in-Huxley curren
+00001360: 7420 696e 2074 6865 2073 6f6d 610a 2020  t in the soma.  
+00001370: 2020 736f 6d61 2e69 6e73 6572 7428 2768    soma.insert('h
+00001380: 6827 290a 2020 2020 666f 7220 7365 6720  h').    for seg 
+00001390: 696e 2073 6f6d 613a 0a20 2020 2020 2020  in soma:.       
+000013a0: 2073 6567 2e68 682e 676e 6162 6172 203d   seg.hh.gnabar =
+000013b0: 2030 2e31 3220 2023 2053 6f64 6975 6d20   0.12  # Sodium 
+000013c0: 636f 6e64 7563 7461 6e63 6520 696e 2053  conductance in S
+000013d0: 2f63 6d32 0a20 2020 2020 2020 2073 6567  /cm2.        seg
+000013e0: 2e68 682e 676b 6261 7220 3d20 302e 3033  .hh.gkbar = 0.03
+000013f0: 3620 2023 2050 6f74 6173 7369 756d 2063  6  # Potassium c
+00001400: 6f6e 6475 6374 616e 6365 2069 6e20 532f  onductance in S/
+00001410: 636d 320a 2020 2020 2020 2020 7365 672e  cm2.        seg.
+00001420: 6868 2e67 6c20 3d20 302e 3030 3033 2020  hh.gl = 0.0003  
+00001430: 2020 2320 4c65 616b 2063 6f6e 6475 6374    # Leak conduct
+00001440: 616e 6365 2069 6e20 532f 636d 320a 2020  ance in S/cm2.  
+00001450: 2020 2020 2020 7365 672e 6868 2e65 6c20        seg.hh.el 
+00001460: 3d20 2d35 342e 3320 2020 2020 2320 5265  = -54.3     # Re
+00001470: 7665 7273 616c 2070 6f74 656e 7469 616c  versal potential
+00001480: 2069 6e20 6d56 0a0a 2020 2020 2320 496e   in mV..    # In
+00001490: 7365 7274 2070 6173 7369 7665 2063 7572  sert passive cur
+000014a0: 7265 6e74 2069 6e20 7468 6520 6465 6e64  rent in the dend
+000014b0: 7269 7465 0a20 2020 2064 656e 642e 696e  rite.    dend.in
+000014c0: 7365 7274 2827 7061 7327 290a 2020 2020  sert('pas').    
+000014d0: 666f 7220 7365 6720 696e 2064 656e 643a  for seg in dend:
+000014e0: 0a20 2020 2020 2020 2073 6567 2e70 6173  .        seg.pas
+000014f0: 2e67 203d 2030 2e30 3031 2020 2320 5061  .g = 0.001  # Pa
+00001500: 7373 6976 6520 636f 6e64 7563 7461 6e63  ssive conductanc
+00001510: 6520 696e 2053 2f63 6d32 0a20 2020 2020  e in S/cm2.     
+00001520: 2020 2073 6567 2e70 6173 2e65 203d 202d     seg.pas.e = -
+00001530: 3635 2020 2020 2320 4c65 616b 2072 6576  65    # Leak rev
+00001540: 6572 7361 6c20 706f 7465 6e74 6961 6c20  ersal potential 
+00001550: 6d56 0a0a 2020 2020 7374 696d 203d 2068  mV..    stim = h
+00001560: 2e49 436c 616d 7028 6465 6e64 2831 2929  .IClamp(dend(1))
+00001570: 0a20 2020 2073 7469 6d2e 6465 6c61 7920  .    stim.delay 
+00001580: 3d20 350a 2020 2020 7374 696d 2e64 7572  = 5.    stim.dur
+00001590: 203d 2031 300a 2020 2020 7374 696d 2e61   = 10.    stim.a
+000015a0: 6d70 203d 2030 2e31 0a0a 2020 2020 6375  mp = 0.1..    cu
+000015b0: 7272 656e 745f 6e61 6d65 7320 3d20 5b22  rrent_names = ["
+000015c0: 696b 222c 2022 696e 6122 2c20 2269 6c5f  ik", "ina", "il_
+000015d0: 6868 225d 0a20 2020 2074 5f76 6563 203d  hh"].    t_vec =
+000015e0: 2068 2e56 6563 746f 7228 290a 2020 2020   h.Vector().    
+000015f0: 765f 7665 6320 3d20 682e 5665 6374 6f72  v_vec = h.Vector
+00001600: 2829 0a20 2020 2069 6b5f 7665 6320 3d20  ().    ik_vec = 
+00001610: 682e 5665 6374 6f72 2829 0a20 2020 2069  h.Vector().    i
+00001620: 6e61 5f76 6563 203d 2068 2e56 6563 746f  na_vec = h.Vecto
+00001630: 7228 290a 2020 2020 696c 5f76 6563 203d  r().    il_vec =
+00001640: 2068 2e56 6563 746f 7228 290a 2020 2020   h.Vector().    
+00001650: 745f 7665 632e 7265 636f 7264 2868 2e5f  t_vec.record(h._
+00001660: 7265 665f 7429 0a20 2020 2076 5f76 6563  ref_t).    v_vec
+00001670: 2e72 6563 6f72 6428 736f 6d61 2830 2e35  .record(soma(0.5
+00001680: 292e 5f72 6566 5f76 290a 2020 2020 696b  )._ref_v).    ik
+00001690: 5f76 6563 2e72 6563 6f72 6428 736f 6d61  _vec.record(soma
+000016a0: 2830 2e35 292e 5f72 6566 5f69 6b29 0a20  (0.5)._ref_ik). 
+000016b0: 2020 2069 6e61 5f76 6563 2e72 6563 6f72     ina_vec.recor
+000016c0: 6428 736f 6d61 2830 2e35 292e 5f72 6566  d(soma(0.5)._ref
+000016d0: 5f69 6e61 290a 2020 2020 696c 5f76 6563  _ina).    il_vec
+000016e0: 2e72 6563 6f72 6428 736f 6d61 2830 2e35  .record(soma(0.5
+000016f0: 292e 5f72 6566 5f69 6c5f 6868 290a 0a20  )._ref_il_hh).. 
+00001700: 2020 2068 2e66 696e 6974 6961 6c69 7a65     h.finitialize
+00001710: 282d 3635 202a 206d 5629 0a20 2020 2068  (-65 * mV).    h
+00001720: 2e63 6f6e 7469 6e75 6572 756e 2832 3520  .continuerun(25 
+00001730: 2a20 6d73 290a 0a20 2020 2074 6f5f 7041  * ms)..    to_pA
+00001740: 203d 2031 3020 2a20 736f 6d61 2830 2e35   = 10 * soma(0.5
+00001750: 292e 6172 6561 2829 2023 2074 7572 6e20  ).area() # turn 
+00001760: 6d41 2f63 6d32 2028 2a75 6d32 2920 696e  mA/cm2 (*um2) in
+00001770: 746f 2070 410a 2020 2020 766f 6c74 6167  to pA.    voltag
+00001780: 6520 3d20 6e70 2e61 7361 7272 6179 2876  e = np.asarray(v
+00001790: 5f76 6563 290a 2020 2020 706f 7461 7373  _vec).    potass
+000017a0: 6975 6d20 3d20 6e70 2e61 7361 7272 6179  ium = np.asarray
+000017b0: 2869 6b5f 7665 6329 202a 2074 6f5f 7041  (ik_vec) * to_pA
+000017c0: 0a20 2020 2073 6f64 6975 6d20 3d20 6e70  .    sodium = np
+000017d0: 2e61 7361 7272 6179 2869 6e61 5f76 6563  .asarray(ina_vec
+000017e0: 2920 2a20 746f 5f70 410a 2020 2020 6c65  ) * to_pA.    le
+000017f0: 616b 203d 206e 702e 6173 6172 7261 7928  ak = np.asarray(
+00001800: 696c 5f76 6563 2920 2a20 746f 5f70 410a  il_vec) * to_pA.
+00001810: 0a20 2020 2063 6f6e 6669 6720 3d20 7b0a  .    config = {.
+00001820: 2020 2020 2020 2020 226f 7574 7075 7422          "output"
+00001830: 3a20 7b20 2020 2020 2020 2020 2020 2020  : {             
+00001840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001870: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00001880: 2020 2273 6176 6566 6967 223a 2054 7275    "savefig": Tru
+00001890: 652c 2020 2020 2020 2020 2020 2020 2020  e,              
+000018a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018c0: 2020 2020 2020 2020 2020 2020 200a 2020               .  
+000018d0: 2020 2020 2020 2020 2264 6972 223a 2022          "dir": "
+000018e0: 2e22 2c20 2020 2020 2020 2020 2020 2020  .",             
+000018f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001920: 2020 200a 2020 2020 2020 2020 2020 2266     .          "f
+00001930: 6e61 6d65 223a 2022 7175 6963 6b73 7461  name": "quicksta
+00001940: 7274 5f70 6c6f 7422 2c20 2020 2020 2020  rt_plot",       
+00001950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001970: 2020 2020 2020 2020 200a 2020 2020 2020           .      
+00001980: 2020 2020 2265 7874 656e 7369 6f6e 223a      "extension":
+00001990: 2022 706e 6722 2c20 2020 2020 2020 2020   "png",         
+000019a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019c0: 2020 2020 2020 2020 2020 2020 2020 200a                 .
+000019d0: 2020 2020 2020 2020 2020 2264 7069 223a            "dpi":
+000019e0: 2033 3030 2c20 2020 2020 2020 2020 2020   300,           
+000019f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a20: 2020 2020 200a 2020 2020 2020 2020 2020       .          
+00001a30: 2274 7261 6e73 7061 7265 6e74 223a 2046  "transparent": F
+00001a40: 616c 7365 2020 2020 2020 2020 2020 2020  alse            
+00001a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a70: 2020 2020 2020 2020 2020 200a 2020 2020             .    
+00001a80: 2020 2020 7d2c 2020 200a 2020 2020 2020      },   .      
+00001a90: 2020 2263 7572 7265 6e74 223a 207b 226e    "current": {"n
+00001aa0: 616d 6573 223a 2063 7572 7265 6e74 5f6e  ames": current_n
+00001ab0: 616d 6573 7d2c 0a20 2020 2020 2020 2022  ames},.        "
+00001ac0: 766f 6c74 6167 6522 3a20 7b22 796c 696d  voltage": {"ylim
+00001ad0: 223a 205b 2d39 302c 2035 305d 7d2c 0a20  ": [-90, 50]},. 
+00001ae0: 2020 2020 2020 2022 6c65 6765 6e64 7465         "legendte
+00001af0: 7874 7369 7a65 223a 2035 2c0a 2020 2020  xtsize": 5,.    
+00001b00: 7d0a 2020 2020 6669 6720 3d20 706c 6f74  }.    fig = plot
+00001b10: 5f63 7572 7265 6e74 7363 6170 6528 766f  _currentscape(vo
+00001b20: 6c74 6167 652c 205b 706f 7461 7373 6975  ltage, [potassiu
+00001b30: 6d2c 2073 6f64 6975 6d2c 206c 6561 6b5d  m, sodium, leak]
+00001b40: 2c20 636f 6e66 6967 290a 2020 2020 6669  , config).    fi
+00001b50: 672e 7368 6f77 2829 0a0a 5768 656e 2079  g.show()..When y
+00001b60: 6f75 2072 756e 2074 6869 7320 636f 6465  ou run this code
+00001b70: 2069 6e20 5079 7468 6f6e 2c20 6974 2077   in Python, it w
+00001b80: 696c 6c20 6765 6e65 7261 7465 2074 6865  ill generate the
+00001b90: 2066 6f6c 6c6f 7769 6e67 2063 7572 7265   following curre
+00001ba0: 6e74 7363 6170 6520 706c 6f74 2028 696e  ntscape plot (in
+00001bb0: 2061 2077 696e 646f 772c 2061 6e64 206f   a window, and o
+00001bc0: 6e20 6469 736b 2061 7320 7175 6963 6b73  n disk as quicks
+00001bd0: 7461 7274 5f70 6c6f 742e 706e 6729 3a0a  tart_plot.png):.
+00001be0: 0a2e 2e20 696d 6167 653a 3a20 646f 632f  ... image:: doc/
+00001bf0: 736f 7572 6365 2f69 6d61 6765 732f 7175  source/images/qu
+00001c00: 6963 6b73 7461 7274 5f70 6c6f 742e 706e  ickstart_plot.pn
+00001c10: 670a 0a54 7574 6f72 6961 6c0a 3d3d 3d3d  g..Tutorial.====
+00001c20: 3d3d 3d3d 0a0a 4120 6d6f 7265 2064 6574  ====..A more det
+00001c30: 6169 6c65 6420 6578 706c 616e 6174 696f  ailed explanatio
+00001c40: 6e20 6f6e 2068 6f77 2074 6f20 7573 6520  n on how to use 
+00001c50: 4375 7272 656e 7473 6361 7065 2c20 6173  Currentscape, as
+00001c60: 2077 656c 6c20 6173 206f 7468 6572 2065   well as other e
+00001c70: 7861 6d70 6c65 7320 6361 6e20 6265 2066  xamples can be f
+00001c80: 6f75 6e64 206f 6e20 7468 6520 6074 7574  ound on the `tut
+00001c90: 6f72 6961 6c20 7061 6765 203c 5475 746f  orial page <Tuto
+00001ca0: 7269 616c 2e72 7374 3e60 5f2e 0a0a 4150  rial.rst>`_...AP
+00001cb0: 4920 446f 6375 6d65 6e74 6174 696f 6e0a  I Documentation.
+00001cc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00001cd0: 3d0a 0a54 6865 2041 5049 2064 6f63 756d  =..The API docum
+00001ce0: 656e 7461 7469 6f6e 2063 616e 2062 6520  entation can be 
+00001cf0: 666f 756e 6420 6f6e 2060 5265 6164 5468  found on `ReadTh
+00001d00: 6544 6f63 7320 3c22 6874 7470 733a 2f2f  eDocs <"https://
+00001d10: 6375 7272 656e 7473 6361 7065 2e72 6561  currentscape.rea
+00001d20: 6474 6865 646f 6373 2e69 6f22 3e60 5f2e  dthedocs.io">`_.
+00001d30: 0a0a 4675 6e64 696e 6720 2620 4163 6b6e  ..Funding & Ackn
+00001d40: 6f77 6c65 6467 656d 656e 7473 0a3d 3d3d  owledgements.===
+00001d50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00001d60: 3d3d 3d3d 3d3d 3d0a 0a57 6520 7769 7368  =======..We wish
+00001d70: 2074 6f20 7468 616e 6b20 7468 6520 6175   to thank the au
+00001d80: 7468 6f72 7320 6f66 2060 416c 6f6e 736f  thors of `Alonso
+00001d90: 2061 6e64 204d 6172 6465 722c 2032 3031   and Marder, 201
+00001da0: 3920 3c68 7474 7073 3a2f 2f64 6f69 2e6f  9 <https://doi.o
+00001db0: 7267 2f31 302e 3735 3534 2f65 4c69 6665  rg/10.7554/eLife
+00001dc0: 2e34 3237 3232 3e60 5f5f 2074 6f20 6c65  .42722>`__ to le
+00001dd0: 7420 7573 2069 6e74 6567 7261 7465 2061  t us integrate a
+00001de0: 2070 6172 7420 6f66 2074 6865 6972 2060   part of their `
+00001df0: 636f 6465 203c 6874 7470 733a 2f2f 6461  code <https://da
+00001e00: 7461 6472 7961 642e 6f72 672f 7374 6173  tadryad.org/stas
+00001e10: 682f 6461 7461 7365 742f 646f 693a 3130  h/dataset/doi:10
+00001e20: 2e35 3036 312f 6472 7961 642e 6430 3737  .5061/dryad.d077
+00001e30: 396d 623e 605f 2069 6e74 6f20 7468 6973  9mb>`_ into this
+00001e40: 2072 6570 6f73 6974 6f72 792e 0a0a 5468   repository...Th
+00001e50: 6520 7061 7274 206f 6620 7468 6520 636f  e part of the co
+00001e60: 6465 2069 6e20 7468 6973 2072 6570 6f73  de in this repos
+00001e70: 6974 6f72 7920 6465 7665 6c6f 7065 6420  itory developed 
+00001e80: 6279 2074 6865 2045 5046 4c20 426c 7565  by the EPFL Blue
+00001e90: 2042 7261 696e 2050 726f 6a65 6374 2077   Brain Project w
+00001ea0: 6173 2073 7570 706f 7274 6564 2062 7920  as supported by 
+00001eb0: 6675 6e64 696e 6720 746f 2074 6865 2042  funding to the B
+00001ec0: 6c75 6520 4272 6169 6e20 5072 6f6a 6563  lue Brain Projec
+00001ed0: 742c 2061 2072 6573 6561 7263 6820 6365  t, a research ce
+00001ee0: 6e74 6572 206f 6620 7468 6520 c389 636f  nter of the ..co
+00001ef0: 6c65 2070 6f6c 7974 6563 686e 6971 7565  le polytechnique
+00001f00: 2066 c3a9 64c3 a972 616c 6520 6465 204c   f..d..rale de L
+00001f10: 6175 7361 6e6e 6520 2845 5046 4c29 2c20  ausanne (EPFL), 
+00001f20: 6672 6f6d 2074 6865 2053 7769 7373 2067  from the Swiss g
+00001f30: 6f76 6572 6e6d 656e 7427 7320 4554 4820  overnment's ETH 
+00001f40: 426f 6172 6420 6f66 2074 6865 2053 7769  Board of the Swi
+00001f50: 7373 2046 6564 6572 616c 2049 6e73 7469  ss Federal Insti
+00001f60: 7475 7465 7320 6f66 2054 6563 686e 6f6c  tutes of Technol
+00001f70: 6f67 792e 0a0a 0a2e 2e20 7c70 7970 697c  ogy...... |pypi|
+00001f80: 2069 6d61 6765 3a3a 2068 7474 7073 3a2f   image:: https:/
+00001f90: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00001fa0: 7079 7069 2f76 2f63 7572 7265 6e74 7363  pypi/v/currentsc
+00001fb0: 6170 652e 7376 670a 2020 2020 2020 2020  ape.svg.        
+00001fc0: 2020 2020 2020 203a 7461 7267 6574 3a20         :target: 
+00001fd0: 6874 7470 733a 2f2f 7465 7374 2e70 7970  https://test.pyp
+00001fe0: 692e 6f72 672f 7072 6f6a 6563 742f 6375  i.org/project/cu
+00001ff0: 7272 656e 7473 6361 7065 2f0a 2020 2020  rrentscape/.    
+00002000: 2020 2020 2020 2020 2020 203a 616c 743a             :alt:
+00002010: 206c 6174 6573 7420 7265 6c65 6173 650a   latest release.
+00002020: 0a2e 2e20 7c64 6f63 737c 2069 6d61 6765  ... |docs| image
+00002030: 3a3a 2068 7474 7073 3a2f 2f72 6561 6474  :: https://readt
+00002040: 6865 646f 6373 2e6f 7267 2f70 726f 6a65  hedocs.org/proje
+00002050: 6374 732f 6375 7272 656e 7473 6361 7065  cts/currentscape
+00002060: 2f62 6164 6765 2f3f 7665 7273 696f 6e3d  /badge/?version=
+00002070: 6c61 7465 7374 0a20 2020 2020 2020 2020  latest.         
+00002080: 2020 2020 2020 3a74 6172 6765 743a 2068        :target: h
+00002090: 7474 7073 3a2f 2f63 7572 7265 6e74 7363  ttps://currentsc
+000020a0: 6170 652e 7265 6164 7468 6564 6f63 732e  ape.readthedocs.
+000020b0: 696f 2f0a 2020 2020 2020 2020 2020 2020  io/.            
+000020c0: 2020 203a 616c 743a 206c 6174 6573 7420     :alt: latest 
+000020d0: 646f 6375 6d65 6e74 6174 696f 6e0a 0a2e  documentation...
+000020e0: 2e20 7c6c 6963 656e 7365 7c20 696d 6167  . |license| imag
+000020f0: 653a 3a20 6874 7470 733a 2f2f 696d 672e  e:: https://img.
+00002100: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+00002110: 6c2f 6375 7272 656e 7473 6361 7065 2e73  l/currentscape.s
+00002120: 7667 0a20 2020 2020 2020 2020 2020 2020  vg.             
+00002130: 2020 2020 203a 7461 7267 6574 3a20 6874       :target: ht
+00002140: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00002150: 2f42 6c75 6542 7261 696e 2f43 7572 7265  /BlueBrain/Curre
+00002160: 6e74 7363 6170 652f 626c 6f62 2f6d 6169  ntscape/blob/mai
+00002170: 6e2f 4c49 4345 4e53 452e 7478 740a 2020  n/LICENSE.txt.  
+00002180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002190: 3a61 6c74 3a20 6c69 6365 6e73 650a 0a2e  :alt: license...
+000021a0: 2e20 7c62 7569 6c64 7c20 696d 6167 653a  . |build| image:
+000021b0: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+000021c0: 2e63 6f6d 2f42 6c75 6542 7261 696e 2f43  .com/BlueBrain/C
+000021d0: 7572 7265 6e74 7363 6170 652f 776f 726b  urrentscape/work
+000021e0: 666c 6f77 732f 5465 7374 2f62 6164 6765  flows/Test/badge
+000021f0: 2e73 7667 3f62 7261 6e63 683d 6d61 696e  .svg?branch=main
+00002200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002210: 203a 7461 7267 6574 3a20 6874 7470 733a   :target: https:
+00002220: 2f2f 6769 7468 7562 2e63 6f6d 2f42 6c75  //github.com/Blu
+00002230: 6542 7261 696e 2f43 7572 7265 6e74 7363  eBrain/Currentsc
+00002240: 6170 652f 6163 7469 6f6e 730a 2020 2020  ape/actions.    
+00002250: 2020 2020 2020 2020 2020 2020 3a61 6c74              :alt
+00002260: 3a20 6163 7469 6f6e 7320 6275 696c 6420  : actions build 
+00002270: 7374 6174 7573 0a0a 2e2e 207c 636f 7665  status.... |cove
+00002280: 7261 6765 7c20 696d 6167 653a 3a20 6874  rage| image:: ht
+00002290: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
+000022a0: 2f67 6974 6875 622f 426c 7565 4272 6169  /github/BlueBrai
+000022b0: 6e2f 4375 7272 656e 7473 6361 7065 2f63  n/Currentscape/c
+000022c0: 6f76 6572 6167 652e 7376 673f 6272 616e  overage.svg?bran
+000022d0: 6368 3d6d 6169 6e0a 2020 2020 2020 2020  ch=main.        
+000022e0: 2020 2020 2020 2020 2020 203a 7461 7267             :targ
+000022f0: 6574 3a20 6874 7470 733a 2f2f 636f 6465  et: https://code
+00002300: 636f 762e 696f 2f67 682f 426c 7565 4272  cov.io/gh/BlueBr
+00002310: 6169 6e2f 6375 7272 656e 7473 6361 7065  ain/currentscape
+00002320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002330: 2020 2020 3a61 6c74 3a20 636f 7665 7261      :alt: covera
+00002340: 6765 0a0a 2e2e 207c 6769 7474 6572 7c20  ge.... |gitter| 
+00002350: 696d 6167 653a 3a20 6874 7470 733a 2f2f  image:: https://
+00002360: 6261 6467 6573 2e67 6974 7465 722e 696d  badges.gitter.im
+00002370: 2f4a 6f69 6e25 3230 4368 6174 2e73 7667  /Join%20Chat.svg
+00002380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002390: 2020 3a74 6172 6765 743a 2068 7474 7073    :target: https
+000023a0: 3a2f 2f67 6974 7465 722e 696d 2f62 6c75  ://gitter.im/blu
+000023b0: 6562 7261 696e 2f63 7572 7265 6e74 7363  ebrain/currentsc
+000023c0: 6170 650a 2020 2020 2020 2020 2020 2020  ape.            
+000023d0: 2020 2020 203a 616c 743a 204a 6f69 6e20       :alt: Join 
+000023e0: 7468 6520 6368 6174 2061 7420 6874 7470  the chat at http
+000023f0: 733a 2f2f 6769 7474 6572 2e69 6d2f 626c  s://gitter.im/bl
+00002400: 7565 6272 6169 6e2f 6375 7272 656e 7473  uebrain/currents
+00002410: 6361 7065 0a                             cape.
```

### Comparing `currentscape-0.0.0/currentscape/__init__.py` & `currentscape-1.0.1/currentscape/__init__.py`

 * *Files identical despite different names*

### Comparing `currentscape-0.0.0/currentscape/config_parser.py` & `currentscape-1.0.1/currentscape/config_parser.py`

 * *Files identical despite different names*

### Comparing `currentscape-0.0.0/currentscape/currents.py` & `currentscape-1.0.1/currentscape/currents.py`

 * *Files 0% similar despite different names*

```diff
@@ -495,20 +495,21 @@
 
         Remove 0s arrays. Reorder if asked. Record reordered name indexes.
         Return the sum and the fraction with its reordered indexes.
 
         Args:
             reorder_ (bool): whether to reorder the currents or not
 
-        Returns:
-            pos_norm (ndarray of ndarrays): arrays containing norm
-                of positive currents
-            neg_norm (ndarray of ndarrays): arrays containing (-1)* norm
-                of negative currents
+        Returns: A tuple (pos_norm, neg_norm, normapos, normaneg), with
+            pos_norm (ndarray of ndarrays): arrays containing norm of positive currents
+
+            neg_norm (ndarray of ndarrays): arrays containing (-1)* norm of negative currents
+
             normapos (ndarray): summed positive currents
+
             normaneg (ndarray): summed (absolute values of) negative currents
         """
         cpos = self.get_positive_data()
         cneg = self.get_negative_data()
 
         normapos = np.sum(np.abs(np.asarray(cpos)), axis=0)
         normaneg = np.sum(np.abs(np.asarray(cneg)), axis=0)
```

### Comparing `currentscape-0.0.0/currentscape/currentscape.py` & `currentscape-1.0.1/currentscape/currentscape.py`

 * *Files identical despite different names*

### Comparing `currentscape-0.0.0/currentscape/data_processing.py` & `currentscape-1.0.1/currentscape/data_processing.py`

 * *Files identical despite different names*

### Comparing `currentscape-0.0.0/currentscape/datasets.py` & `currentscape-1.0.1/currentscape/datasets.py`

 * *Files identical despite different names*

### Comparing `currentscape-0.0.0/currentscape/ions.py` & `currentscape-1.0.1/currentscape/ions.py`

 * *Files identical despite different names*

### Comparing `currentscape-0.0.0/currentscape/legends.py` & `currentscape-1.0.1/currentscape/legends.py`

 * *Files identical despite different names*

### Comparing `currentscape-0.0.0/currentscape/mapper.py` & `currentscape-1.0.1/currentscape/mapper.py`

 * *Files identical despite different names*

### Comparing `currentscape-0.0.0/currentscape/plotting.py` & `currentscape-1.0.1/currentscape/plotting.py`

 * *Files identical despite different names*

### Comparing `currentscape-0.0.0/currentscape/voltages.py` & `currentscape-1.0.1/currentscape/voltages.py`

 * *Files identical despite different names*

### Comparing `currentscape-0.0.0/currentscape.egg-info/PKG-INFO` & `currentscape-1.0.1/currentscape.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6375 7272  : 2.1.Name: curr
 00000020: 656e 7473 6361 7065 0a56 6572 7369 6f6e  entscape.Version
-00000030: 3a20 302e 302e 300a 5375 6d6d 6172 793a  : 0.0.0.Summary:
+00000030: 3a20 312e 302e 310a 5375 6d6d 6172 793a  : 1.0.1.Summary:
 00000040: 204d 6f64 756c 6520 746f 2065 6173 696c   Module to easil
 00000050: 7920 706c 6f74 2063 7572 7265 6e74 7363  y plot currentsc
 00000060: 6170 652e 0a48 6f6d 652d 7061 6765 3a20  ape..Home-page: 
 00000070: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
 00000080: 6f6d 2f42 6c75 6542 7261 696e 2f43 7572  om/BlueBrain/Cur
 00000090: 7265 6e74 7363 6170 650a 4175 7468 6f72  rentscape.Author
 000000a0: 3a20 426c 7565 2042 7261 696e 2050 726f  : Blue Brain Pro
@@ -52,577 +52,593 @@
 00000330: 7373 6966 6965 723a 2054 6f70 6963 203a  ssifier: Topic :
 00000340: 3a20 5363 6965 6e74 6966 6963 2f45 6e67  : Scientific/Eng
 00000350: 696e 6565 7269 6e67 203a 3a20 4269 6f2d  ineering :: Bio-
 00000360: 496e 666f 726d 6174 6963 730a 5265 7175  Informatics.Requ
 00000370: 6972 6573 2d50 7974 686f 6e3a 203e 3d33  ires-Python: >=3
 00000380: 2e37 0a44 6573 6372 6970 7469 6f6e 2d43  .7.Description-C
 00000390: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
-000003a0: 742f 6d61 726b 646f 776e 0a50 726f 7669  t/markdown.Provi
-000003b0: 6465 732d 4578 7472 613a 2064 6f63 730a  des-Extra: docs.
-000003c0: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
-000003d0: 6578 616d 706c 650a 4c69 6365 6e73 652d  example.License-
-000003e0: 4669 6c65 3a20 4c49 4345 4e53 452e 7478  File: LICENSE.tx
-000003f0: 740a 4c69 6365 6e73 652d 4669 6c65 3a20  t.License-File: 
-00000400: 434f 5059 494e 470a 4c69 6365 6e73 652d  COPYING.License-
-00000410: 4669 6c65 3a20 4155 5448 4f52 532e 7273  File: AUTHORS.rs
-00000420: 740a 0a43 7572 7265 6e74 7363 6170 650a  t..Currentscape.
-00000430: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a 2e2e  ============....
-00000440: 2072 6177 3a3a 2068 746d 6c0a 0a09 3c74   raw:: html...<t
-00000450: 6162 6c65 3e0a 093c 7472 3e0a 0920 203c  able>..<tr>..  <
-00000460: 7464 3e4c 6174 6573 7420 5265 6c65 6173  td>Latest Releas
-00000470: 653c 2f74 643e 0a09 2020 3c74 643e 0a09  e</td>..  <td>..
-00000480: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
-00000490: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
-000004a0: 6f6a 6563 742f 6375 7272 656e 7473 6361  oject/currentsca
-000004b0: 7065 2f22 3e0a 0920 2020 203c 696d 6720  pe/">..    <img 
-000004c0: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
-000004d0: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
-000004e0: 2f76 2f63 7572 7265 6e74 7363 6170 652e  /v/currentscape.
-000004f0: 7376 6722 2061 6c74 3d22 6c61 7465 7374  svg" alt="latest
-00000500: 2072 656c 6561 7365 2220 2f3e 0a09 2020   release" />..  
-00000510: 2020 3c2f 613e 0a09 2020 3c2f 7464 3e0a    </a>..  </td>.
-00000520: 093c 2f74 723e 0a09 3c74 723e 0a09 2020  .</tr>..<tr>..  
-00000530: 3c74 643e 446f 6375 6d65 6e74 6174 696f  <td>Documentatio
-00000540: 6e3c 2f74 643e 0a09 2020 3c74 643e 0a09  n</td>..  <td>..
-00000550: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
-00000560: 7073 3a2f 2f63 7572 7265 6e74 7363 6170  ps://currentscap
-00000570: 652e 7265 6164 7468 6564 6f63 732e 696f  e.readthedocs.io
-00000580: 2f22 3e0a 0920 2020 203c 696d 6720 7372  /">..    <img sr
-00000590: 633d 2268 7474 7073 3a2f 2f72 6561 6474  c="https://readt
-000005a0: 6865 646f 6373 2e6f 7267 2f70 726f 6a65  hedocs.org/proje
-000005b0: 6374 732f 6375 7272 656e 7473 6361 7065  cts/currentscape
-000005c0: 2f62 6164 6765 2f3f 7665 7273 696f 6e3d  /badge/?version=
-000005d0: 6c61 7465 7374 2220 616c 743d 226c 6174  latest" alt="lat
-000005e0: 6573 7420 646f 6375 6d65 6e74 6174 696f  est documentatio
-000005f0: 6e22 202f 3e0a 0920 2020 203c 2f61 3e0a  n" />..    </a>.
-00000600: 0920 203c 2f74 643e 0a09 3c2f 7472 3e0a  .  </td>..</tr>.
-00000610: 093c 7472 3e0a 0920 203c 7464 3e4c 6963  .<tr>..  <td>Lic
-00000620: 656e 7365 3c2f 7464 3e0a 0920 203c 7464  ense</td>..  <td
-00000630: 3e0a 0920 2020 203c 6120 6872 6566 3d22  >..    <a href="
-00000640: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000650: 6f6d 2f42 6c75 6542 7261 696e 2f43 7572  om/BlueBrain/Cur
-00000660: 7265 6e74 7363 6170 652f 626c 6f62 2f6d  rentscape/blob/m
-00000670: 6169 6e2f 4c49 4345 4e53 452e 7478 7422  ain/LICENSE.txt"
-00000680: 3e0a 0920 2020 203c 696d 6720 7372 633d  >..    <img src=
-00000690: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
-000006a0: 656c 6473 2e69 6f2f 7079 7069 2f6c 2f63  elds.io/pypi/l/c
-000006b0: 7572 7265 6e74 7363 6170 652e 7376 6722  urrentscape.svg"
-000006c0: 2061 6c74 3d22 6c69 6365 6e73 6522 202f   alt="license" /
-000006d0: 3e0a 0920 2020 203c 2f61 3e0a 093c 2f74  >..    </a>..</t
-000006e0: 643e 0a09 3c2f 7472 3e0a 093c 7472 3e0a  d>..</tr>..<tr>.
-000006f0: 0920 203c 7464 3e42 7569 6c64 2053 7461  .  <td>Build Sta
-00000700: 7475 733c 2f74 643e 0a09 2020 3c74 643e  tus</td>..  <td>
-00000710: 0a09 2020 2020 3c61 2068 7265 663d 2268  ..    <a href="h
-00000720: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000730: 6d2f 426c 7565 4272 6169 6e2f 4375 7272  m/BlueBrain/Curr
-00000740: 656e 7473 6361 7065 2f61 6374 696f 6e73  entscape/actions
-00000750: 223e 0a09 2020 2020 3c69 6d67 2073 7263  ">..    <img src
-00000760: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
-00000770: 2e63 6f6d 2f42 6c75 6542 7261 696e 2f43  .com/BlueBrain/C
-00000780: 7572 7265 6e74 7363 6170 652f 776f 726b  urrentscape/work
-00000790: 666c 6f77 732f 5465 7374 2f62 6164 6765  flows/Test/badge
-000007a0: 2e73 7667 3f62 7261 6e63 683d 6d61 696e  .svg?branch=main
-000007b0: 2220 616c 743d 2241 6374 696f 6e73 2062  " alt="Actions b
-000007c0: 7569 6c64 2073 7461 7475 7322 202f 3e0a  uild status" />.
-000007d0: 0920 2020 203c 2f61 3e0a 0920 203c 2f74  .    </a>..  </t
-000007e0: 643e 0a09 3c2f 7472 3e0a 093c 7472 3e0a  d>..</tr>..<tr>.
-000007f0: 0920 203c 7464 3e43 6f76 6572 6167 653c  .  <td>Coverage<
-00000800: 2f74 643e 0a09 2020 3c74 643e 0a09 2020  /td>..  <td>..  
-00000810: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-00000820: 3a2f 2f63 6f64 6563 6f76 2e69 6f2f 6768  ://codecov.io/gh
-00000830: 2f42 6c75 6542 7261 696e 2f63 7572 7265  /BlueBrain/curre
-00000840: 6e74 7363 6170 6522 3e0a 0920 2020 203c  ntscape">..    <
-00000850: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00000860: 2f63 6f64 6563 6f76 2e69 6f2f 6769 7468  /codecov.io/gith
-00000870: 7562 2f42 6c75 6542 7261 696e 2f43 7572  ub/BlueBrain/Cur
-00000880: 7265 6e74 7363 6170 652f 636f 7665 7261  rentscape/covera
-00000890: 6765 2e73 7667 3f62 7261 6e63 683d 6d61  ge.svg?branch=ma
-000008a0: 696e 2220 616c 743d 2263 6f76 6572 6167  in" alt="coverag
-000008b0: 6522 202f 3e0a 0920 2020 203c 2f61 3e0a  e" />..    </a>.
-000008c0: 0920 203c 2f74 643e 0a09 3c2f 7472 3e0a  .  </td>..</tr>.
-000008d0: 093c 7472 3e0a 0909 3c74 643e 4769 7474  .<tr>...<td>Gitt
-000008e0: 6572 3c2f 7464 3e0a 0909 3c74 643e 0a09  er</td>...<td>..
-000008f0: 0909 3c61 2068 7265 663d 2268 7474 7073  ..<a href="https
-00000900: 3a2f 2f67 6974 7465 722e 696d 2f62 6c75  ://gitter.im/blu
-00000910: 6562 7261 696e 2f63 7572 7265 6e74 7363  ebrain/currentsc
-00000920: 6170 6522 3e0a 0909 093c 696d 6720 7372  ape">....<img sr
-00000930: 633d 2268 7474 7073 3a2f 2f62 6164 6765  c="https://badge
-00000940: 732e 6769 7474 6572 2e69 6d2f 4a6f 696e  s.gitter.im/Join
-00000950: 2532 3043 6861 742e 7376 6722 0a09 093c  %20Chat.svg"...<
-00000960: 2f61 3e0a 0909 3c2f 7464 3e0a 093c 2f74  /a>...</td>..</t
-00000970: 723e 0a09 3c2f 7461 626c 653e 0a0a 496e  r>..</table>..In
-00000980: 7472 6f64 7563 7469 6f6e 0a3d 3d3d 3d3d  troduction.=====
-00000990: 3d3d 3d3d 3d3d 3d0a 0a43 7572 7265 6e74  =======..Current
-000009a0: 7363 6170 6520 6973 2061 2050 7974 686f  scape is a Pytho
-000009b0: 6e20 746f 6f6c 2065 6e61 626c 696e 6720  n tool enabling 
-000009c0: 7363 6965 6e74 6973 7473 2074 6f20 6561  scientists to ea
-000009d0: 7369 6c79 2070 6c6f 7420 7468 6520 6375  sily plot the cu
-000009e0: 7272 656e 7473 2069 6e20 656c 6563 7472  rrents in electr
-000009f0: 6963 616c 206e 6575 726f 6e20 6d6f 6465  ical neuron mode
-00000a00: 6c73 2e0a 5468 6520 636f 6465 2069 7320  ls..The code is 
-00000a10: 6261 7365 6420 6f6e 2074 6865 2070 6170  based on the pap
-00000a20: 6572 2060 416c 6f6e 736f 2061 6e64 204d  er `Alonso and M
-00000a30: 6172 6465 722c 2032 3031 3920 3c68 7474  arder, 2019 <htt
-00000a40: 7073 3a2f 2f64 6f69 2e6f 7267 2f31 302e  ps://doi.org/10.
-00000a50: 3735 3534 2f65 4c69 6665 2e34 3237 3232  7554/eLife.42722
-00000a60: 3e60 5f2e 0a0a 4375 7272 656e 7473 6361  >`_...Currentsca
-00000a70: 7065 2066 6967 7572 6573 2070 6c6f 7420  pe figures plot 
-00000a80: 7468 6520 7065 7263 656e 7461 6765 206f  the percentage o
-00000a90: 6620 696e 7761 7264 2061 6e64 206f 7574  f inward and out
-00000aa0: 7761 7264 2069 6f6e 6963 206d 656d 6272  ward ionic membr
-00000ab0: 616e 6520 6375 7272 656e 7473 2c0a 7468  ane currents,.th
-00000ac0: 6520 746f 7461 6c20 696e 7761 7264 2061  e total inward a
-00000ad0: 6e64 206f 7574 7761 7264 2063 7572 7265  nd outward curre
-00000ae0: 6e74 732c 2061 7320 7765 6c6c 2061 7320  nts, as well as 
-00000af0: 7468 6520 766f 6c74 6167 6520 696e 2066  the voltage in f
-00000b00: 756e 6374 696f 6e20 6f66 2074 696d 652e  unction of time.
-00000b10: 0a49 7420 616c 6c6f 7773 206d 6f64 656c  .It allows model
-00000b20: 6c65 7273 2074 6f20 7365 6520 7768 6963  lers to see whic
-00000b30: 6820 6375 7272 656e 7473 2070 6c61 7920  h currents play 
-00000b40: 6120 726f 6c65 2061 7420 616e 7920 6769  a role at any gi
-00000b50: 7665 6e20 7469 6d65 2064 7572 696e 6720  ven time during 
-00000b60: 6120 7369 6d75 6c61 7469 6f6e 2c20 616e  a simulation, an
-00000b70: 6420 6368 6563 6b20 696e 2064 6570 7468  d check in depth
-00000b80: 2074 6865 2063 7572 7265 6e74 2064 796e   the current dyn
-00000b90: 616d 6963 732e 0a0a 2e2e 2069 6d61 6765  amics..... image
-00000ba0: 3a3a 2064 6f63 2f73 6f75 7263 652f 696d  :: doc/source/im
-00000bb0: 6167 6573 2f70 6c6f 742e 706e 670a 0a43  ages/plot.png..C
-00000bc0: 6974 6174 696f 6e0a 3d3d 3d3d 3d3d 3d3d  itation.========
-00000bd0: 0a0a 5768 656e 2079 6f75 2075 7365 2074  ..When you use t
-00000be0: 6869 7320 4375 7272 656e 7473 6361 7065  his Currentscape
-00000bf0: 2073 6f66 7477 6172 6520 666f 7220 796f   software for yo
-00000c00: 7572 2072 6573 6561 7263 682c 2077 6520  ur research, we 
-00000c10: 6173 6b20 796f 7520 746f 2063 6974 6520  ask you to cite 
-00000c20: 7468 6520 666f 6c6c 6f77 696e 6720 7075  the following pu
-00000c30: 626c 6963 6174 696f 6e20 2874 6869 7320  blication (this 
-00000c40: 696e 636c 7564 6573 2070 6f73 7465 7220  includes poster 
-00000c50: 7072 6573 656e 7461 7469 6f6e 7329 3a0a  presentations):.
-00000c60: 0a2e 2e20 636f 6465 2d62 6c6f 636b 3a3a  ... code-block::
-00000c70: 200a 0a20 2020 2040 6172 7469 636c 6520   ..    @article 
-00000c80: 7b31 302e 3735 3534 2f65 4c69 6665 2e34  {10.7554/eLife.4
-00000c90: 3237 3232 2c0a 2020 2020 6172 7469 636c  2722,.    articl
-00000ca0: 655f 7479 7065 203d 207b 6a6f 7572 6e61  e_type = {journa
-00000cb0: 6c7d 2c0a 2020 2020 7469 746c 6520 3d20  l},.    title = 
-00000cc0: 7b56 6973 7561 6c69 7a61 7469 6f6e 206f  {Visualization o
-00000cd0: 6620 6375 7272 656e 7473 2069 6e20 6e65  f currents in ne
-00000ce0: 7572 616c 206d 6f64 656c 7320 7769 7468  ural models with
-00000cf0: 2073 696d 696c 6172 2062 6568 6176 696f   similar behavio
-00000d00: 7220 616e 6420 6469 6666 6572 656e 7420  r and different 
-00000d10: 636f 6e64 7563 7461 6e63 6520 6465 6e73  conductance dens
-00000d20: 6974 6965 737d 2c0a 2020 2020 6175 7468  ities},.    auth
-00000d30: 6f72 203d 207b 416c 6f6e 736f 2c20 4c65  or = {Alonso, Le
-00000d40: 616e 6472 6f20 4d20 616e 6420 4d61 7264  andro M and Mard
-00000d50: 6572 2c20 4576 657d 2c0a 2020 2020 6564  er, Eve},.    ed
-00000d60: 6974 6f72 203d 207b 5765 7374 6272 6f6f  itor = {Westbroo
-00000d70: 6b2c 2047 6172 7920 4c20 616e 6420 536b  k, Gary L and Sk
-00000d80: 696e 6e65 722c 2046 7261 6e63 6573 204b  inner, Frances K
-00000d90: 2061 6e64 204c 616e 6b61 7261 6e79 2c20   and Lankarany, 
-00000da0: 4d69 6c61 6420 616e 6420 4272 6974 746f  Milad and Britto
-00000db0: 6e2c 204f 6c69 7665 727d 2c0a 2020 2020  n, Oliver},.    
-00000dc0: 766f 6c75 6d65 203d 2038 2c0a 2020 2020  volume = 8,.    
-00000dd0: 7965 6172 203d 2032 3031 392c 0a20 2020  year = 2019,.   
-00000de0: 206d 6f6e 7468 203d 207b 6a61 6e7d 2c0a   month = {jan},.
-00000df0: 2020 2020 7075 625f 6461 7465 203d 207b      pub_date = {
-00000e00: 3230 3139 2d30 312d 3331 7d2c 0a20 2020  2019-01-31},.   
-00000e10: 2070 6167 6573 203d 207b 6534 3237 3232   pages = {e42722
-00000e20: 7d2c 0a20 2020 2063 6974 6174 696f 6e20  },.    citation 
-00000e30: 3d20 7b65 4c69 6665 2032 3031 393b 383a  = {eLife 2019;8:
-00000e40: 6534 3237 3232 7d2c 0a20 2020 2064 6f69  e42722},.    doi
-00000e50: 203d 207b 3130 2e37 3535 342f 654c 6966   = {10.7554/eLif
-00000e60: 652e 3432 3732 327d 2c0a 2020 2020 7572  e.42722},.    ur
-00000e70: 6c20 3d20 7b68 7474 7073 3a2f 2f64 6f69  l = {https://doi
-00000e80: 2e6f 7267 2f31 302e 3735 3534 2f65 4c69  .org/10.7554/eLi
-00000e90: 6665 2e34 3237 3232 7d2c 0a20 2020 2061  fe.42722},.    a
-00000ea0: 6273 7472 6163 7420 3d20 7b43 6f6e 6475  bstract = {Condu
-00000eb0: 6374 616e 6365 2d62 6173 6564 206d 6f64  ctance-based mod
-00000ec0: 656c 7320 6f66 206e 6575 7261 6c20 6163  els of neural ac
-00000ed0: 7469 7669 7479 2070 726f 6475 6365 206c  tivity produce l
-00000ee0: 6172 6765 2061 6d6f 756e 7473 206f 6620  arge amounts of 
-00000ef0: 6461 7461 2074 6861 7420 6361 6e20 6265  data that can be
-00000f00: 2068 6172 6420 746f 2076 6973 7561 6c69   hard to visuali
-00000f10: 7a65 2061 6e64 2069 6e74 6572 7072 6574  ze and interpret
-00000f20: 2e20 5765 2069 6e74 726f 6475 6365 2076  . We introduce v
-00000f30: 6973 7561 6c69 7a61 7469 6f6e 206d 6574  isualization met
-00000f40: 686f 6473 2074 6f20 6469 7370 6c61 7920  hods to display 
-00000f50: 7468 6520 6479 6e61 6d69 6373 206f 6620  the dynamics of 
-00000f60: 7468 6520 696f 6e69 6320 6375 7272 656e  the ionic curren
-00000f70: 7473 2061 6e64 2074 6f20 6469 7370 6c61  ts and to displa
-00000f80: 7920 7468 6520 6d6f 6465 6c73 e280 9920  y the models... 
-00000f90: 7265 7370 6f6e 7365 2074 6f20 7065 7274  response to pert
-00000fa0: 7572 6261 7469 6f6e 732e 2054 6f20 7669  urbations. To vi
-00000fb0: 7375 616c 697a 6520 7468 6520 6375 7272  sualize the curr
-00000fc0: 656e 7473 e280 9920 6479 6e61 6d69 6373  ents... dynamics
-00000fd0: 2c20 7765 2063 6f6d 7075 7465 2074 6865  , we compute the
-00000fe0: 2070 6572 6365 6e74 2063 6f6e 7472 6962   percent contrib
-00000ff0: 7574 696f 6e20 6f66 2065 6163 6820 6375  ution of each cu
-00001000: 7272 656e 7420 616e 6420 6469 7370 6c61  rrent and displa
-00001010: 7920 7468 656d 206f 7665 7220 7469 6d65  y them over time
-00001020: 2075 7369 6e67 2073 7461 636b 6564 2d61   using stacked-a
-00001030: 7265 6120 706c 6f74 732e 2054 6865 2077  rea plots. The w
-00001040: 6176 6566 6f72 6d20 6f66 2074 6865 206d  aveform of the m
-00001050: 656d 6272 616e 6520 706f 7465 6e74 6961  embrane potentia
-00001060: 6c20 616e 6420 7468 6520 636f 6e74 7269  l and the contri
-00001070: 6275 7469 6f6e 206f 6620 6561 6368 2063  bution of each c
-00001080: 7572 7265 6e74 2063 6861 6e67 6520 6173  urrent change as
-00001090: 2074 6865 206d 6f64 656c 7320 6172 6520   the models are 
-000010a0: 7065 7274 7572 6265 642e 2054 6f20 7265  perturbed. To re
-000010b0: 7072 6573 656e 7420 7468 6573 6520 6368  present these ch
-000010c0: 616e 6765 7320 6f76 6572 2061 2072 616e  anges over a ran
-000010d0: 6765 206f 6620 7468 6520 7065 7274 7572  ge of the pertur
-000010e0: 6261 7469 6f6e 2063 6f6e 7472 6f6c 2070  bation control p
-000010f0: 6172 616d 6574 6572 2c20 7765 2063 6f6d  arameter, we com
-00001100: 7075 7465 2061 6e64 2064 6973 706c 6179  pute and display
-00001110: 2074 6865 2064 6973 7472 6962 7574 696f   the distributio
-00001120: 6e73 206f 6620 7468 6573 6520 7761 7665  ns of these wave
-00001130: 666f 726d 732e 2057 6520 696c 6c75 7374  forms. We illust
-00001140: 7261 7465 2074 6865 7365 2070 726f 6365  rate these proce
-00001150: 6475 7265 7320 696e 2073 6978 2065 7861  dures in six exa
-00001160: 6d70 6c65 7320 6f66 2062 7572 7374 696e  mples of burstin
-00001170: 6720 6d6f 6465 6c20 6e65 7572 6f6e 7320  g model neurons 
-00001180: 7769 7468 2073 696d 696c 6172 2061 6374  with similar act
-00001190: 6976 6974 7920 6275 7420 7468 6174 2064  ivity but that d
-000011a0: 6966 6665 7220 6173 206d 7563 6820 6173  iffer as much as
-000011b0: 2074 6872 6565 666f 6c64 2069 6e20 7468   threefold in th
-000011c0: 6569 7220 636f 6e64 7563 7461 6e63 6520  eir conductance 
-000011d0: 6465 6e73 6974 6965 732e 2054 6865 7365  densities. These
-000011e0: 2076 6973 7561 6c69 7a61 7469 6f6e 206d   visualization m
-000011f0: 6574 686f 6473 2070 726f 7669 6465 2068  ethods provide h
-00001200: 6575 7269 7374 6963 2069 6e73 6967 6874  euristic insight
-00001210: 2069 6e74 6f20 7768 7920 696e 6469 7669   into why indivi
-00001220: 6475 616c 206e 6575 726f 6e73 206f 7220  dual neurons or 
-00001230: 6e65 7477 6f72 6b73 2077 6974 6820 7369  networks with si
-00001240: 6d69 6c61 7220 6265 6861 7669 6f72 2063  milar behavior c
-00001250: 616e 2072 6573 706f 6e64 2077 6964 656c  an respond widel
-00001260: 7920 6469 6666 6572 656e 746c 7920 746f  y differently to
-00001270: 2070 6572 7475 7262 6174 696f 6e73 2e7d   perturbations.}
-00001280: 2c0a 2020 2020 6b65 7977 6f72 6473 203d  ,.    keywords =
-00001290: 207b 6e65 7572 6f6e 616c 206f 7363 696c   {neuronal oscil
-000012a0: 6c61 746f 7273 2c20 4e61 2b20 6368 616e  lators, Na+ chan
-000012b0: 6e65 6c73 2c20 4361 2b2b 2063 6861 6e6e  nels, Ca++ chann
-000012c0: 656c 732c 204b 2b20 6368 616e 6e65 6c73  els, K+ channels
-000012d0: 2c20 636f 6e64 7563 7461 6e63 652d 6261  , conductance-ba
-000012e0: 7365 642c 2069 6f6e 6963 2063 6861 6e6e  sed, ionic chann
-000012f0: 656c 737d 2c0a 2020 2020 6a6f 7572 6e61  els},.    journa
-00001300: 6c20 3d20 7b65 4c69 6665 7d2c 0a20 2020  l = {eLife},.   
-00001310: 2069 7373 6e20 3d20 7b32 3035 302d 3038   issn = {2050-08
-00001320: 3458 7d2c 0a20 2020 2070 7562 6c69 7368  4X},.    publish
-00001330: 6572 203d 207b 654c 6966 6520 5363 6965  er = {eLife Scie
-00001340: 6e63 6573 2050 7562 6c69 6361 7469 6f6e  nces Publication
-00001350: 732c 204c 7464 7d2c 0a20 2020 207d 0a0a  s, Ltd},.    }..
-00001360: 5375 7070 6f72 740a 3d3d 3d3d 3d3d 3d0a  Support.=======.
-00001370: 0a57 6520 6172 6520 7072 6f76 6964 696e  .We are providin
-00001380: 6720 7375 7070 6f72 7420 6f6e 2060 4769  g support on `Gi
-00001390: 7474 6572 203c 6874 7470 733a 2f2f 6769  tter <https://gi
-000013a0: 7474 6572 2e69 6d2f 426c 7565 4272 6169  tter.im/BlueBrai
-000013b0: 6e2f 4375 7272 656e 7473 6361 7065 3e60  n/Currentscape>`
-000013c0: 5f2e 2057 6520 7375 6767 6573 7420 796f  _. We suggest yo
-000013d0: 7520 6372 6561 7465 2074 6963 6b65 7473  u create tickets
-000013e0: 206f 6e20 7468 6520 6047 6974 6875 6220   on the `Github 
-000013f0: 6973 7375 6520 7472 6163 6b65 7220 3c68  issue tracker <h
-00001400: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001410: 6d2f 426c 7565 4272 6169 6e2f 4375 7272  m/BlueBrain/Curr
-00001420: 656e 7473 6361 7065 2f69 7373 7565 733e  entscape/issues>
-00001430: 605f 2069 6e20 6361 7365 2079 6f75 2065  `_ in case you e
-00001440: 6e63 6f75 6e74 6572 2070 726f 626c 656d  ncounter problem
-00001450: 7320 7768 696c 6520 7573 696e 6720 7468  s while using th
-00001460: 6520 736f 6674 7761 7265 206f 7220 6966  e software or if
-00001470: 2079 6f75 2068 6176 6520 736f 6d65 2073   you have some s
-00001480: 7567 6765 7374 696f 6e73 2e0a 0a4d 6169  uggestions...Mai
-00001490: 6e20 6465 7065 6e64 656e 6369 6573 0a3d  n dependencies.=
-000014a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000014b0: 0a0a 2d20 6050 7974 686f 6e20 332e 372b  ..- `Python 3.7+
-000014c0: 203c 6874 7470 733a 2f2f 7777 772e 7079   <https://www.py
-000014d0: 7468 6f6e 2e6f 7267 2f64 6f77 6e6c 6f61  thon.org/downloa
-000014e0: 6473 2f72 656c 6561 7365 2f70 7974 686f  ds/release/pytho
-000014f0: 6e2d 3337 302f 3e60 5f0a 2d20 604e 756d  n-370/>`_.- `Num
-00001500: 7079 203c 6874 7470 733a 2f2f 6e75 6d70  py <https://nump
-00001510: 792e 6f72 672f 3e60 5f20 2861 7574 6f6d  y.org/>`_ (autom
-00001520: 6174 6963 616c 6c79 2069 6e73 7461 6c6c  atically install
-00001530: 6564 2062 7920 7069 7029 0a2d 2060 5061  ed by pip).- `Pa
-00001540: 6c65 7474 6162 6c65 203c 6874 7470 733a  lettable <https:
-00001550: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 6966  //github.com/jif
-00001560: 6679 636c 7562 2f70 616c 6574 7461 626c  fyclub/palettabl
-00001570: 653e 605f 2028 6175 746f 6d61 7469 6361  e>`_ (automatica
-00001580: 6c6c 7920 696e 7374 616c 6c65 6420 6279  lly installed by
-00001590: 2070 6970 290a 0a49 6e73 7461 6c6c 6174   pip)..Installat
-000015a0: 696f 6e0a 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ion.============
-000015b0: 0a0a 4375 7272 656e 7473 6361 7065 2063  ..Currentscape c
-000015c0: 616e 2062 6520 7069 7020 696e 7374 616c  an be pip instal
-000015d0: 6c65 6420 7769 7468 2074 6865 2066 6f6c  led with the fol
-000015e0: 6c6f 7769 6e67 2063 6f6d 6d61 6e64 3a0a  lowing command:.
-000015f0: 0a2e 2e20 636f 6465 2d62 6c6f 636b 3a3a  ... code-block::
-00001600: 2070 7974 686f 6e0a 0a20 2020 2070 6970   python..    pip
-00001610: 2069 6e73 7461 6c6c 2063 7572 7265 6e74   install current
-00001620: 7363 6170 650a 0a49 6620 796f 7520 7761  scape..If you wa
-00001630: 6e74 2074 6f20 6265 2061 626c 6520 746f  nt to be able to
-00001640: 2072 756e 2074 6865 2043 7572 7265 6e74   run the Current
-00001650: 7363 6170 6520 6578 616d 706c 6573 2c20  scape examples, 
-00001660: 796f 7520 7769 6c6c 206e 6565 6420 746f  you will need to
-00001670: 2061 6c73 6f20 696e 7374 616c 6c20 7468   also install th
-00001680: 6520 6578 616d 706c 6520 6465 7065 6e64  e example depend
-00001690: 656e 6369 6573 3a0a 0a2e 2e20 636f 6465  encies:.... code
-000016a0: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0a  -block:: python.
-000016b0: 0a20 2020 2070 6970 2069 6e73 7461 6c6c  .    pip install
-000016c0: 2063 7572 7265 6e74 7363 6170 655b 6578   currentscape[ex
-000016d0: 616d 706c 655d 0a0a 5175 6963 6b20 5374  ample]..Quick St
-000016e0: 6172 740a 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a  art.===========.
-000016f0: 0a42 656c 6f77 2069 7320 616e 2065 7861  .Below is an exa
-00001700: 6d70 6c65 206f 6620 6120 6261 6c6c 2061  mple of a ball a
-00001710: 6e64 2073 7469 636b 206d 6f64 656c 2069  nd stick model i
-00001720: 6e20 4e45 5552 4f4e 2077 6974 6820 7369  n NEURON with si
-00001730: 6d70 6c65 2048 6f64 676b 696e 2d48 7578  mple Hodgkin-Hux
-00001740: 6c65 7920 6d65 6368 616e 6973 6d73 2c20  ley mechanisms, 
-00001750: 746f 2077 6869 6368 2061 2073 7465 7020  to which a step 
-00001760: 7374 696d 756c 7573 2069 7320 6170 706c  stimulus is appl
-00001770: 6965 642e 0a0a 5468 6520 766f 6c74 6167  ied...The voltag
-00001780: 6520 616e 6420 696f 6e69 6320 6375 7272  e and ionic curr
-00001790: 656e 7473 2061 7265 2072 6563 6f72 6465  ents are recorde
-000017a0: 6420 616e 6420 6665 6420 746f 2043 7572  d and fed to Cur
-000017b0: 7265 6e74 7363 6170 652c 2061 6c6f 6e67  rentscape, along
-000017c0: 2077 6974 6820 6120 636f 6e66 6967 7572   with a configur
-000017d0: 6174 696f 6e20 6469 6374 696f 6e61 7279  ation dictionary
-000017e0: 2063 6f6e 7461 696e 696e 6720 7468 6520   containing the 
-000017f0: 6375 7272 656e 7420 6e61 6d65 7320 746f  current names to
-00001800: 2062 6520 6469 7370 6c61 7965 6420 696e   be displayed in
-00001810: 2074 6865 206c 6567 656e 642e 0a0a 546f   the legend...To
-00001820: 2072 756e 2074 6865 2063 6f64 6520 796f   run the code yo
-00001830: 7520 7769 6c6c 2066 6972 7374 2068 6176  u will first hav
-00001840: 6520 746f 2069 6e73 7461 6c6c 204e 4555  e to install NEU
-00001850: 524f 4e20 7061 636b 6167 653a 0a0a 2e2e  RON package:....
-00001860: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
-00001870: 7468 6f6e 0a0a 2020 2020 7069 7020 696e  thon..    pip in
-00001880: 7374 616c 6c20 6e65 7572 6f6e 0a0a 5768  stall neuron..Wh
-00001890: 656e 2079 6f75 2074 6865 6e20 6578 6563  en you then exec
-000018a0: 7574 6520 7468 6520 666f 6c6c 6f77 696e  ute the followin
-000018b0: 6720 7079 7468 6f6e 2063 6f64 652c 2061  g python code, a
-000018c0: 2077 696e 646f 7720 7368 6f75 6c64 206f   window should o
-000018d0: 7065 6e20 7769 7468 2074 6865 2063 7572  pen with the cur
-000018e0: 7265 6e74 7363 6170 6520 706c 6f74 3a0a  rentscape plot:.
-000018f0: 0a2e 2e20 636f 6465 2d62 6c6f 636b 3a3a  ... code-block::
-00001900: 2070 7974 686f 6e0a 0a20 2020 2069 6d70   python..    imp
-00001910: 6f72 7420 6e75 6d70 7920 6173 206e 700a  ort numpy as np.
-00001920: 2020 2020 6672 6f6d 206e 6575 726f 6e20      from neuron 
-00001930: 696d 706f 7274 2068 0a20 2020 2066 726f  import h.    fro
-00001940: 6d20 6e65 7572 6f6e 2e75 6e69 7473 2069  m neuron.units i
-00001950: 6d70 6f72 7420 6d73 2c20 6d56 0a20 2020  mport ms, mV.   
-00001960: 2066 726f 6d20 6375 7272 656e 7473 6361   from currentsca
-00001970: 7065 2e63 7572 7265 6e74 7363 6170 6520  pe.currentscape 
-00001980: 696d 706f 7274 2070 6c6f 745f 6375 7272  import plot_curr
-00001990: 656e 7473 6361 7065 0a0a 2020 2020 682e  entscape..    h.
-000019a0: 6c6f 6164 5f66 696c 6528 2773 7464 7275  load_file('stdru
-000019b0: 6e2e 686f 6327 290a 0a20 2020 2073 6f6d  n.hoc')..    som
-000019c0: 6120 3d20 682e 5365 6374 696f 6e28 6e61  a = h.Section(na
-000019d0: 6d65 3d27 736f 6d61 2729 0a20 2020 2064  me='soma').    d
-000019e0: 656e 6420 3d20 682e 5365 6374 696f 6e28  end = h.Section(
-000019f0: 6e61 6d65 3d27 6465 6e64 2729 0a0a 2020  name='dend')..  
-00001a00: 2020 6465 6e64 2e63 6f6e 6e65 6374 2873    dend.connect(s
-00001a10: 6f6d 6128 3129 290a 0a20 2020 2073 6f6d  oma(1))..    som
-00001a20: 612e 4c20 3d20 736f 6d61 2e64 6961 6d20  a.L = soma.diam 
-00001a30: 3d20 3132 2e36 3135 370a 2020 2020 6465  = 12.6157.    de
-00001a40: 6e64 2e4c 203d 2032 3030 0a20 2020 2064  nd.L = 200.    d
-00001a50: 656e 642e 6469 616d 203d 2031 0a0a 2020  end.diam = 1..  
-00001a60: 2020 666f 7220 7365 6320 696e 2068 2e61    for sec in h.a
-00001a70: 6c6c 7365 6328 293a 0a20 2020 2020 2020  llsec():.       
-00001a80: 2073 6563 2e52 6120 3d20 3130 3020 2020   sec.Ra = 100   
-00001a90: 2023 2041 7869 616c 2072 6573 6973 7461   # Axial resista
-00001aa0: 6e63 6520 696e 204f 686d 202a 2063 6d0a  nce in Ohm * cm.
-00001ab0: 2020 2020 2020 2020 7365 632e 636d 203d          sec.cm =
-00001ac0: 2031 2020 2020 2020 2320 4d65 6d62 7261   1      # Membra
-00001ad0: 6e65 2063 6170 6163 6974 616e 6365 2069  ne capacitance i
-00001ae0: 6e20 6d69 6372 6f20 4661 7261 6473 202f  n micro Farads /
-00001af0: 2063 6d5e 320a 0a20 2020 2023 2049 6e73   cm^2..    # Ins
-00001b00: 6572 7420 6163 7469 7665 2048 6f64 676b  ert active Hodgk
-00001b10: 696e 2d48 7578 6c65 7920 6375 7272 656e  in-Huxley curren
-00001b20: 7420 696e 2074 6865 2073 6f6d 610a 2020  t in the soma.  
-00001b30: 2020 736f 6d61 2e69 6e73 6572 7428 2768    soma.insert('h
-00001b40: 6827 290a 2020 2020 666f 7220 7365 6720  h').    for seg 
-00001b50: 696e 2073 6f6d 613a 0a20 2020 2020 2020  in soma:.       
-00001b60: 2073 6567 2e68 682e 676e 6162 6172 203d   seg.hh.gnabar =
-00001b70: 2030 2e31 3220 2023 2053 6f64 6975 6d20   0.12  # Sodium 
-00001b80: 636f 6e64 7563 7461 6e63 6520 696e 2053  conductance in S
-00001b90: 2f63 6d32 0a20 2020 2020 2020 2073 6567  /cm2.        seg
-00001ba0: 2e68 682e 676b 6261 7220 3d20 302e 3033  .hh.gkbar = 0.03
-00001bb0: 3620 2023 2050 6f74 6173 7369 756d 2063  6  # Potassium c
-00001bc0: 6f6e 6475 6374 616e 6365 2069 6e20 532f  onductance in S/
-00001bd0: 636d 320a 2020 2020 2020 2020 7365 672e  cm2.        seg.
-00001be0: 6868 2e67 6c20 3d20 302e 3030 3033 2020  hh.gl = 0.0003  
-00001bf0: 2020 2320 4c65 616b 2063 6f6e 6475 6374    # Leak conduct
-00001c00: 616e 6365 2069 6e20 532f 636d 320a 2020  ance in S/cm2.  
-00001c10: 2020 2020 2020 7365 672e 6868 2e65 6c20        seg.hh.el 
-00001c20: 3d20 2d35 342e 3320 2020 2020 2320 5265  = -54.3     # Re
-00001c30: 7665 7273 616c 2070 6f74 656e 7469 616c  versal potential
-00001c40: 2069 6e20 6d56 0a0a 2020 2020 2320 496e   in mV..    # In
-00001c50: 7365 7274 2070 6173 7369 7665 2063 7572  sert passive cur
-00001c60: 7265 6e74 2069 6e20 7468 6520 6465 6e64  rent in the dend
-00001c70: 7269 7465 0a20 2020 2064 656e 642e 696e  rite.    dend.in
-00001c80: 7365 7274 2827 7061 7327 290a 2020 2020  sert('pas').    
-00001c90: 666f 7220 7365 6720 696e 2064 656e 643a  for seg in dend:
-00001ca0: 0a20 2020 2020 2020 2073 6567 2e70 6173  .        seg.pas
-00001cb0: 2e67 203d 2030 2e30 3031 2020 2320 5061  .g = 0.001  # Pa
-00001cc0: 7373 6976 6520 636f 6e64 7563 7461 6e63  ssive conductanc
-00001cd0: 6520 696e 2053 2f63 6d32 0a20 2020 2020  e in S/cm2.     
-00001ce0: 2020 2073 6567 2e70 6173 2e65 203d 202d     seg.pas.e = -
-00001cf0: 3635 2020 2020 2320 4c65 616b 2072 6576  65    # Leak rev
-00001d00: 6572 7361 6c20 706f 7465 6e74 6961 6c20  ersal potential 
-00001d10: 6d56 0a0a 2020 2020 7374 696d 203d 2068  mV..    stim = h
-00001d20: 2e49 436c 616d 7028 6465 6e64 2831 2929  .IClamp(dend(1))
-00001d30: 0a20 2020 2073 7469 6d2e 6465 6c61 7920  .    stim.delay 
-00001d40: 3d20 350a 2020 2020 7374 696d 2e64 7572  = 5.    stim.dur
-00001d50: 203d 2031 300a 2020 2020 7374 696d 2e61   = 10.    stim.a
-00001d60: 6d70 203d 2030 2e31 0a0a 2020 2020 6375  mp = 0.1..    cu
-00001d70: 7272 656e 745f 6e61 6d65 7320 3d20 5b22  rrent_names = ["
-00001d80: 696b 222c 2022 696e 6122 2c20 2269 6c5f  ik", "ina", "il_
-00001d90: 6868 225d 0a20 2020 2074 5f76 6563 203d  hh"].    t_vec =
-00001da0: 2068 2e56 6563 746f 7228 290a 2020 2020   h.Vector().    
-00001db0: 765f 7665 6320 3d20 682e 5665 6374 6f72  v_vec = h.Vector
-00001dc0: 2829 0a20 2020 2069 6b5f 7665 6320 3d20  ().    ik_vec = 
-00001dd0: 682e 5665 6374 6f72 2829 0a20 2020 2069  h.Vector().    i
-00001de0: 6e61 5f76 6563 203d 2068 2e56 6563 746f  na_vec = h.Vecto
-00001df0: 7228 290a 2020 2020 696c 5f76 6563 203d  r().    il_vec =
-00001e00: 2068 2e56 6563 746f 7228 290a 2020 2020   h.Vector().    
-00001e10: 745f 7665 632e 7265 636f 7264 2868 2e5f  t_vec.record(h._
-00001e20: 7265 665f 7429 0a20 2020 2076 5f76 6563  ref_t).    v_vec
-00001e30: 2e72 6563 6f72 6428 736f 6d61 2830 2e35  .record(soma(0.5
-00001e40: 292e 5f72 6566 5f76 290a 2020 2020 696b  )._ref_v).    ik
-00001e50: 5f76 6563 2e72 6563 6f72 6428 736f 6d61  _vec.record(soma
-00001e60: 2830 2e35 292e 5f72 6566 5f69 6b29 0a20  (0.5)._ref_ik). 
-00001e70: 2020 2069 6e61 5f76 6563 2e72 6563 6f72     ina_vec.recor
-00001e80: 6428 736f 6d61 2830 2e35 292e 5f72 6566  d(soma(0.5)._ref
-00001e90: 5f69 6e61 290a 2020 2020 696c 5f76 6563  _ina).    il_vec
-00001ea0: 2e72 6563 6f72 6428 736f 6d61 2830 2e35  .record(soma(0.5
-00001eb0: 292e 5f72 6566 5f69 6c5f 6868 290a 0a20  )._ref_il_hh).. 
-00001ec0: 2020 2068 2e66 696e 6974 6961 6c69 7a65     h.finitialize
-00001ed0: 282d 3635 202a 206d 5629 0a20 2020 2068  (-65 * mV).    h
-00001ee0: 2e63 6f6e 7469 6e75 6572 756e 2832 3520  .continuerun(25 
-00001ef0: 2a20 6d73 290a 0a20 2020 2074 6f5f 7041  * ms)..    to_pA
-00001f00: 203d 2031 3020 2a20 736f 6d61 2830 2e35   = 10 * soma(0.5
-00001f10: 292e 6172 6561 2829 2023 2074 7572 6e20  ).area() # turn 
-00001f20: 6d41 2f63 6d32 2028 2a75 6d32 2920 696e  mA/cm2 (*um2) in
-00001f30: 746f 2070 410a 2020 2020 766f 6c74 6167  to pA.    voltag
-00001f40: 6520 3d20 6e70 2e61 7361 7272 6179 2876  e = np.asarray(v
-00001f50: 5f76 6563 290a 2020 2020 706f 7461 7373  _vec).    potass
-00001f60: 6975 6d20 3d20 6e70 2e61 7361 7272 6179  ium = np.asarray
-00001f70: 2869 6b5f 7665 6329 202a 2074 6f5f 7041  (ik_vec) * to_pA
-00001f80: 0a20 2020 2073 6f64 6975 6d20 3d20 6e70  .    sodium = np
-00001f90: 2e61 7361 7272 6179 2869 6e61 5f76 6563  .asarray(ina_vec
-00001fa0: 2920 2a20 746f 5f70 410a 2020 2020 6c65  ) * to_pA.    le
-00001fb0: 616b 203d 206e 702e 6173 6172 7261 7928  ak = np.asarray(
-00001fc0: 696c 5f76 6563 2920 2a20 746f 5f70 410a  il_vec) * to_pA.
-00001fd0: 0a20 2020 2063 6f6e 6669 6720 3d20 7b0a  .    config = {.
-00001fe0: 2020 2020 2020 2020 226f 7574 7075 7422          "output"
-00001ff0: 3a20 7b20 2020 2020 2020 2020 2020 2020  : {             
-00002000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002030: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00002040: 2020 2273 6176 6566 6967 223a 2054 7275    "savefig": Tru
-00002050: 652c 2020 2020 2020 2020 2020 2020 2020  e,              
-00002060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002080: 2020 2020 2020 2020 2020 2020 200a 2020               .  
-00002090: 2020 2020 2020 2020 2264 6972 223a 2022          "dir": "
-000020a0: 2e22 2c20 2020 2020 2020 2020 2020 2020  .",             
-000020b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020e0: 2020 200a 2020 2020 2020 2020 2020 2266     .          "f
-000020f0: 6e61 6d65 223a 2022 7175 6963 6b73 7461  name": "quicksta
-00002100: 7274 5f70 6c6f 7422 2c20 2020 2020 2020  rt_plot",       
-00002110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002130: 2020 2020 2020 2020 200a 2020 2020 2020           .      
-00002140: 2020 2020 2265 7874 656e 7369 6f6e 223a      "extension":
-00002150: 2022 706e 6722 2c20 2020 2020 2020 2020   "png",         
-00002160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002180: 2020 2020 2020 2020 2020 2020 2020 200a                 .
-00002190: 2020 2020 2020 2020 2020 2264 7069 223a            "dpi":
-000021a0: 2033 3030 2c20 2020 2020 2020 2020 2020   300,           
-000021b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021e0: 2020 2020 200a 2020 2020 2020 2020 2020       .          
-000021f0: 2274 7261 6e73 7061 7265 6e74 223a 2046  "transparent": F
-00002200: 616c 7365 2020 2020 2020 2020 2020 2020  alse            
-00002210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002230: 2020 2020 2020 2020 2020 200a 2020 2020             .    
-00002240: 2020 2020 7d2c 2020 200a 2020 2020 2020      },   .      
-00002250: 2020 2263 7572 7265 6e74 223a 207b 226e    "current": {"n
-00002260: 616d 6573 223a 2063 7572 7265 6e74 5f6e  ames": current_n
-00002270: 616d 6573 7d2c 0a20 2020 2020 2020 2022  ames},.        "
-00002280: 766f 6c74 6167 6522 3a20 7b22 796c 696d  voltage": {"ylim
-00002290: 223a 205b 2d39 302c 2035 305d 7d2c 0a20  ": [-90, 50]},. 
-000022a0: 2020 2020 2020 2022 6c65 6765 6e64 7465         "legendte
-000022b0: 7874 7369 7a65 223a 2035 2c0a 2020 2020  xtsize": 5,.    
-000022c0: 7d0a 2020 2020 6669 6720 3d20 706c 6f74  }.    fig = plot
-000022d0: 5f63 7572 7265 6e74 7363 6170 6528 766f  _currentscape(vo
-000022e0: 6c74 6167 652c 205b 706f 7461 7373 6975  ltage, [potassiu
-000022f0: 6d2c 2073 6f64 6975 6d2c 206c 6561 6b5d  m, sodium, leak]
-00002300: 2c20 636f 6e66 6967 290a 2020 2020 6669  , config).    fi
-00002310: 672e 7368 6f77 2829 0a0a 5768 656e 2079  g.show()..When y
-00002320: 6f75 2072 756e 2074 6869 7320 636f 6465  ou run this code
-00002330: 2069 6e20 5079 7468 6f6e 2c20 6974 2077   in Python, it w
-00002340: 696c 6c20 6765 6e65 7261 7465 2074 6865  ill generate the
-00002350: 2066 6f6c 6c6f 7769 6e67 2063 7572 7265   following curre
-00002360: 6e74 7363 6170 6520 706c 6f74 2028 696e  ntscape plot (in
-00002370: 2061 2077 696e 646f 772c 2061 6e64 206f   a window, and o
-00002380: 6e20 6469 736b 2061 7320 7175 6963 6b73  n disk as quicks
-00002390: 7461 7274 5f70 6c6f 742e 706e 6729 3a0a  tart_plot.png):.
-000023a0: 0a2e 2e20 696d 6167 653a 3a20 646f 632f  ... image:: doc/
-000023b0: 736f 7572 6365 2f69 6d61 6765 732f 7175  source/images/qu
-000023c0: 6963 6b73 7461 7274 5f70 6c6f 742e 706e  ickstart_plot.pn
-000023d0: 670a 0a54 7574 6f72 6961 6c0a 3d3d 3d3d  g..Tutorial.====
-000023e0: 3d3d 3d3d 0a0a 4120 6d6f 7265 2064 6574  ====..A more det
-000023f0: 6169 6c65 6420 6578 706c 616e 6174 696f  ailed explanatio
-00002400: 6e20 6f6e 2068 6f77 2074 6f20 7573 6520  n on how to use 
-00002410: 4375 7272 656e 7473 6361 7065 2c20 6173  Currentscape, as
-00002420: 2077 656c 6c20 6173 206f 7468 6572 2065   well as other e
-00002430: 7861 6d70 6c65 7320 6361 6e20 6265 2066  xamples can be f
-00002440: 6f75 6e64 206f 6e20 7468 6520 6074 7574  ound on the `tut
-00002450: 6f72 6961 6c20 7061 6765 203c 5475 746f  orial page <Tuto
-00002460: 7269 616c 2e72 7374 3e60 5f2e 0a0a 4150  rial.rst>`_...AP
-00002470: 4920 446f 6375 6d65 6e74 6174 696f 6e0a  I Documentation.
-00002480: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00002490: 3d0a 0a54 6865 2041 5049 2064 6f63 756d  =..The API docum
-000024a0: 656e 7461 7469 6f6e 2063 616e 2062 6520  entation can be 
-000024b0: 666f 756e 6420 6f6e 2060 5265 6164 5468  found on `ReadTh
-000024c0: 6544 6f63 7320 3c22 6874 7470 733a 2f2f  eDocs <"https://
-000024d0: 6375 7272 656e 7473 6361 7065 2e72 6561  currentscape.rea
-000024e0: 6474 6865 646f 6373 2e69 6f22 3e60 5f2e  dthedocs.io">`_.
-000024f0: 0a0a 4675 6e64 696e 6720 2620 4163 6b6e  ..Funding & Ackn
-00002500: 6f77 6c65 6467 656d 656e 7473 0a3d 3d3d  owledgements.===
-00002510: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00002520: 3d3d 3d3d 3d3d 3d0a 0a57 6520 7769 7368  =======..We wish
-00002530: 2074 6f20 7468 616e 6b20 7468 6520 6175   to thank the au
-00002540: 7468 6f72 7320 6f66 2060 416c 6f6e 736f  thors of `Alonso
-00002550: 2061 6e64 204d 6172 6465 722c 2032 3031   and Marder, 201
-00002560: 3920 3c68 7474 7073 3a2f 2f64 6f69 2e6f  9 <https://doi.o
-00002570: 7267 2f31 302e 3735 3534 2f65 4c69 6665  rg/10.7554/eLife
-00002580: 2e34 3237 3232 3e60 5f20 746f 206c 6574  .42722>`_ to let
-00002590: 2075 7320 696e 7465 6772 6174 6520 6120   us integrate a 
-000025a0: 7061 7274 206f 6620 7468 6569 7220 6063  part of their `c
-000025b0: 6f64 6520 3c68 7474 7073 3a2f 2f64 6174  ode <https://dat
-000025c0: 6164 7279 6164 2e6f 7267 2f73 7461 7368  adryad.org/stash
-000025d0: 2f64 6174 6173 6574 2f64 6f69 3a31 302e  /dataset/doi:10.
-000025e0: 3530 3631 2f64 7279 6164 2e64 3037 3739  5061/dryad.d0779
-000025f0: 6d62 3e60 5f20 696e 746f 2074 6869 7320  mb>`_ into this 
-00002600: 7265 706f 7369 746f 7279 2e0a 0a54 6865  repository...The
-00002610: 2070 6172 7420 6f66 2074 6865 2063 6f64   part of the cod
-00002620: 6520 696e 2074 6869 7320 7265 706f 7369  e in this reposi
-00002630: 746f 7279 2064 6576 656c 6f70 6564 2062  tory developed b
-00002640: 7920 7468 6520 4550 464c 2042 6c75 6520  y the EPFL Blue 
-00002650: 4272 6169 6e20 5072 6f6a 6563 7420 7761  Brain Project wa
-00002660: 7320 7375 7070 6f72 7465 6420 6279 2066  s supported by f
-00002670: 756e 6469 6e67 2074 6f20 7468 6520 426c  unding to the Bl
-00002680: 7565 2042 7261 696e 2050 726f 6a65 6374  ue Brain Project
-00002690: 2c20 6120 7265 7365 6172 6368 2063 656e  , a research cen
-000026a0: 7465 7220 6f66 2074 6865 20c3 8963 6f6c  ter of the ..col
-000026b0: 6520 706f 6c79 7465 6368 6e69 7175 6520  e polytechnique 
-000026c0: 66c3 a964 c3a9 7261 6c65 2064 6520 4c61  f..d..rale de La
-000026d0: 7573 616e 6e65 2028 4550 464c 292c 2066  usanne (EPFL), f
-000026e0: 726f 6d20 7468 6520 5377 6973 7320 676f  rom the Swiss go
-000026f0: 7665 726e 6d65 6e74 2773 2045 5448 2042  vernment's ETH B
-00002700: 6f61 7264 206f 6620 7468 6520 5377 6973  oard of the Swis
-00002710: 7320 4665 6465 7261 6c20 496e 7374 6974  s Federal Instit
-00002720: 7574 6573 206f 6620 5465 6368 6e6f 6c6f  utes of Technolo
-00002730: 6779 2e0a                                gy..
+000003a0: 742f 782d 7273 740a 5072 6f76 6964 6573  t/x-rst.Provides
+000003b0: 2d45 7874 7261 3a20 646f 6373 0a50 726f  -Extra: docs.Pro
+000003c0: 7669 6465 732d 4578 7472 613a 2065 7861  vides-Extra: exa
+000003d0: 6d70 6c65 0a4c 6963 656e 7365 2d46 696c  mple.License-Fil
+000003e0: 653a 204c 4943 454e 5345 2e74 7874 0a4c  e: LICENSE.txt.L
+000003f0: 6963 656e 7365 2d46 696c 653a 2043 4f50  icense-File: COP
+00000400: 5949 4e47 0a4c 6963 656e 7365 2d46 696c  YING.License-Fil
+00000410: 653a 2041 5554 484f 5253 2e72 7374 0a0a  e: AUTHORS.rst..
+00000420: 4375 7272 656e 7473 6361 7065 0a3d 3d3d  Currentscape.===
+00000430: 3d3d 3d3d 3d3d 3d3d 3d0a 0a0a 2b2d 2d2d  =========...+---
+00000440: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+00000450: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 4c61  ----------+.| La
+00000460: 7465 7374 2052 656c 6561 7365 207c 207c  test Release | |
+00000470: 7079 7069 7c20 2020 2020 7c0a 2b2d 2d2d  pypi|     |.+---
+00000480: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+00000490: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 446f  ----------+.| Do
+000004a0: 6375 6d65 6e74 6174 696f 6e20 207c 207c  cumentation  | |
+000004b0: 646f 6373 7c20 2020 2020 7c0a 2b2d 2d2d  docs|     |.+---
+000004c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+000004d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 4c69  ----------+.| Li
+000004e0: 6365 6e73 6520 2020 2020 2020 207c 207c  cense        | |
+000004f0: 6c69 6365 6e73 657c 2020 7c0a 2b2d 2d2d  license|  |.+---
+00000500: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+00000510: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 4275  ----------+.| Bu
+00000520: 696c 6420 5374 6174 7573 2009 207c 207c  ild Status . | |
+00000530: 6275 696c 647c 2020 2020 7c0a 2b2d 2d2d  build|    |.+---
+00000540: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+00000550: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 436f  ----------+.| Co
+00000560: 7665 7261 6765 2020 2020 2020 207c 207c  verage       | |
+00000570: 636f 7665 7261 6765 7c20 7c0a 2b2d 2d2d  coverage| |.+---
+00000580: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+00000590: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 4769  ----------+.| Gi
+000005a0: 7474 6572 2020 2020 2020 2020 207c 207c  tter         | |
+000005b0: 6769 7474 6572 7c20 2020 7c0a 2b2d 2d2d  gitter|   |.+---
+000005c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+000005d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 0a49 6e74  ----------+..Int
+000005e0: 726f 6475 6374 696f 6e0a 3d3d 3d3d 3d3d  roduction.======
+000005f0: 3d3d 3d3d 3d3d 0a0a 4375 7272 656e 7473  ======..Currents
+00000600: 6361 7065 2069 7320 6120 5079 7468 6f6e  cape is a Python
+00000610: 2074 6f6f 6c20 656e 6162 6c69 6e67 2073   tool enabling s
+00000620: 6369 656e 7469 7374 7320 746f 2065 6173  cientists to eas
+00000630: 696c 7920 706c 6f74 2074 6865 2063 7572  ily plot the cur
+00000640: 7265 6e74 7320 696e 2065 6c65 6374 7269  rents in electri
+00000650: 6361 6c20 6e65 7572 6f6e 206d 6f64 656c  cal neuron model
+00000660: 732e 0a54 6865 2063 6f64 6520 6973 2062  s..The code is b
+00000670: 6173 6564 206f 6e20 7468 6520 7061 7065  ased on the pape
+00000680: 7220 6041 6c6f 6e73 6f20 616e 6420 4d61  r `Alonso and Ma
+00000690: 7264 6572 2c20 3230 3139 203c 6874 7470  rder, 2019 <http
+000006a0: 733a 2f2f 646f 692e 6f72 672f 3130 2e37  s://doi.org/10.7
+000006b0: 3535 342f 654c 6966 652e 3432 3732 323e  554/eLife.42722>
+000006c0: 605f 5f2e 0a0a 4375 7272 656e 7473 6361  `__...Currentsca
+000006d0: 7065 2066 6967 7572 6573 2070 6c6f 7420  pe figures plot 
+000006e0: 7468 6520 7065 7263 656e 7461 6765 206f  the percentage o
+000006f0: 6620 696e 7761 7264 2061 6e64 206f 7574  f inward and out
+00000700: 7761 7264 2069 6f6e 6963 206d 656d 6272  ward ionic membr
+00000710: 616e 6520 6375 7272 656e 7473 2c0a 7468  ane currents,.th
+00000720: 6520 746f 7461 6c20 696e 7761 7264 2061  e total inward a
+00000730: 6e64 206f 7574 7761 7264 2063 7572 7265  nd outward curre
+00000740: 6e74 732c 2061 7320 7765 6c6c 2061 7320  nts, as well as 
+00000750: 7468 6520 766f 6c74 6167 6520 696e 2066  the voltage in f
+00000760: 756e 6374 696f 6e20 6f66 2074 696d 652e  unction of time.
+00000770: 0a49 7420 616c 6c6f 7773 206d 6f64 656c  .It allows model
+00000780: 6c65 7273 2074 6f20 7365 6520 7768 6963  lers to see whic
+00000790: 6820 6375 7272 656e 7473 2070 6c61 7920  h currents play 
+000007a0: 6120 726f 6c65 2061 7420 616e 7920 6769  a role at any gi
+000007b0: 7665 6e20 7469 6d65 2064 7572 696e 6720  ven time during 
+000007c0: 6120 7369 6d75 6c61 7469 6f6e 2c20 616e  a simulation, an
+000007d0: 6420 6368 6563 6b20 696e 2064 6570 7468  d check in depth
+000007e0: 2074 6865 2063 7572 7265 6e74 2064 796e   the current dyn
+000007f0: 616d 6963 732e 0a0a 2e2e 2069 6d61 6765  amics..... image
+00000800: 3a3a 2064 6f63 2f73 6f75 7263 652f 696d  :: doc/source/im
+00000810: 6167 6573 2f70 6c6f 742e 706e 670a 0a43  ages/plot.png..C
+00000820: 6974 6174 696f 6e0a 3d3d 3d3d 3d3d 3d3d  itation.========
+00000830: 0a0a 5768 656e 2079 6f75 2075 7365 2074  ..When you use t
+00000840: 6869 7320 4375 7272 656e 7473 6361 7065  his Currentscape
+00000850: 2073 6f66 7477 6172 6520 666f 7220 796f   software for yo
+00000860: 7572 2072 6573 6561 7263 682c 2077 6520  ur research, we 
+00000870: 6173 6b20 796f 7520 746f 2063 6974 6520  ask you to cite 
+00000880: 7468 6520 666f 6c6c 6f77 696e 6720 7075  the following pu
+00000890: 626c 6963 6174 696f 6e20 2874 6869 7320  blication (this 
+000008a0: 696e 636c 7564 6573 2070 6f73 7465 7220  includes poster 
+000008b0: 7072 6573 656e 7461 7469 6f6e 7329 3a0a  presentations):.
+000008c0: 0a2e 2e20 636f 6465 2d62 6c6f 636b 3a3a  ... code-block::
+000008d0: 200a 0a20 2020 2040 6172 7469 636c 6520   ..    @article 
+000008e0: 7b31 302e 3735 3534 2f65 4c69 6665 2e34  {10.7554/eLife.4
+000008f0: 3237 3232 2c0a 2020 2020 6172 7469 636c  2722,.    articl
+00000900: 655f 7479 7065 203d 207b 6a6f 7572 6e61  e_type = {journa
+00000910: 6c7d 2c0a 2020 2020 7469 746c 6520 3d20  l},.    title = 
+00000920: 7b56 6973 7561 6c69 7a61 7469 6f6e 206f  {Visualization o
+00000930: 6620 6375 7272 656e 7473 2069 6e20 6e65  f currents in ne
+00000940: 7572 616c 206d 6f64 656c 7320 7769 7468  ural models with
+00000950: 2073 696d 696c 6172 2062 6568 6176 696f   similar behavio
+00000960: 7220 616e 6420 6469 6666 6572 656e 7420  r and different 
+00000970: 636f 6e64 7563 7461 6e63 6520 6465 6e73  conductance dens
+00000980: 6974 6965 737d 2c0a 2020 2020 6175 7468  ities},.    auth
+00000990: 6f72 203d 207b 416c 6f6e 736f 2c20 4c65  or = {Alonso, Le
+000009a0: 616e 6472 6f20 4d20 616e 6420 4d61 7264  andro M and Mard
+000009b0: 6572 2c20 4576 657d 2c0a 2020 2020 6564  er, Eve},.    ed
+000009c0: 6974 6f72 203d 207b 5765 7374 6272 6f6f  itor = {Westbroo
+000009d0: 6b2c 2047 6172 7920 4c20 616e 6420 536b  k, Gary L and Sk
+000009e0: 696e 6e65 722c 2046 7261 6e63 6573 204b  inner, Frances K
+000009f0: 2061 6e64 204c 616e 6b61 7261 6e79 2c20   and Lankarany, 
+00000a00: 4d69 6c61 6420 616e 6420 4272 6974 746f  Milad and Britto
+00000a10: 6e2c 204f 6c69 7665 727d 2c0a 2020 2020  n, Oliver},.    
+00000a20: 766f 6c75 6d65 203d 2038 2c0a 2020 2020  volume = 8,.    
+00000a30: 7965 6172 203d 2032 3031 392c 0a20 2020  year = 2019,.   
+00000a40: 206d 6f6e 7468 203d 207b 6a61 6e7d 2c0a   month = {jan},.
+00000a50: 2020 2020 7075 625f 6461 7465 203d 207b      pub_date = {
+00000a60: 3230 3139 2d30 312d 3331 7d2c 0a20 2020  2019-01-31},.   
+00000a70: 2070 6167 6573 203d 207b 6534 3237 3232   pages = {e42722
+00000a80: 7d2c 0a20 2020 2063 6974 6174 696f 6e20  },.    citation 
+00000a90: 3d20 7b65 4c69 6665 2032 3031 393b 383a  = {eLife 2019;8:
+00000aa0: 6534 3237 3232 7d2c 0a20 2020 2064 6f69  e42722},.    doi
+00000ab0: 203d 207b 3130 2e37 3535 342f 654c 6966   = {10.7554/eLif
+00000ac0: 652e 3432 3732 327d 2c0a 2020 2020 7572  e.42722},.    ur
+00000ad0: 6c20 3d20 7b68 7474 7073 3a2f 2f64 6f69  l = {https://doi
+00000ae0: 2e6f 7267 2f31 302e 3735 3534 2f65 4c69  .org/10.7554/eLi
+00000af0: 6665 2e34 3237 3232 7d2c 0a20 2020 2061  fe.42722},.    a
+00000b00: 6273 7472 6163 7420 3d20 7b43 6f6e 6475  bstract = {Condu
+00000b10: 6374 616e 6365 2d62 6173 6564 206d 6f64  ctance-based mod
+00000b20: 656c 7320 6f66 206e 6575 7261 6c20 6163  els of neural ac
+00000b30: 7469 7669 7479 2070 726f 6475 6365 206c  tivity produce l
+00000b40: 6172 6765 2061 6d6f 756e 7473 206f 6620  arge amounts of 
+00000b50: 6461 7461 2074 6861 7420 6361 6e20 6265  data that can be
+00000b60: 2068 6172 6420 746f 2076 6973 7561 6c69   hard to visuali
+00000b70: 7a65 2061 6e64 2069 6e74 6572 7072 6574  ze and interpret
+00000b80: 2e20 5765 2069 6e74 726f 6475 6365 2076  . We introduce v
+00000b90: 6973 7561 6c69 7a61 7469 6f6e 206d 6574  isualization met
+00000ba0: 686f 6473 2074 6f20 6469 7370 6c61 7920  hods to display 
+00000bb0: 7468 6520 6479 6e61 6d69 6373 206f 6620  the dynamics of 
+00000bc0: 7468 6520 696f 6e69 6320 6375 7272 656e  the ionic curren
+00000bd0: 7473 2061 6e64 2074 6f20 6469 7370 6c61  ts and to displa
+00000be0: 7920 7468 6520 6d6f 6465 6c73 e280 9920  y the models... 
+00000bf0: 7265 7370 6f6e 7365 2074 6f20 7065 7274  response to pert
+00000c00: 7572 6261 7469 6f6e 732e 2054 6f20 7669  urbations. To vi
+00000c10: 7375 616c 697a 6520 7468 6520 6375 7272  sualize the curr
+00000c20: 656e 7473 e280 9920 6479 6e61 6d69 6373  ents... dynamics
+00000c30: 2c20 7765 2063 6f6d 7075 7465 2074 6865  , we compute the
+00000c40: 2070 6572 6365 6e74 2063 6f6e 7472 6962   percent contrib
+00000c50: 7574 696f 6e20 6f66 2065 6163 6820 6375  ution of each cu
+00000c60: 7272 656e 7420 616e 6420 6469 7370 6c61  rrent and displa
+00000c70: 7920 7468 656d 206f 7665 7220 7469 6d65  y them over time
+00000c80: 2075 7369 6e67 2073 7461 636b 6564 2d61   using stacked-a
+00000c90: 7265 6120 706c 6f74 732e 2054 6865 2077  rea plots. The w
+00000ca0: 6176 6566 6f72 6d20 6f66 2074 6865 206d  aveform of the m
+00000cb0: 656d 6272 616e 6520 706f 7465 6e74 6961  embrane potentia
+00000cc0: 6c20 616e 6420 7468 6520 636f 6e74 7269  l and the contri
+00000cd0: 6275 7469 6f6e 206f 6620 6561 6368 2063  bution of each c
+00000ce0: 7572 7265 6e74 2063 6861 6e67 6520 6173  urrent change as
+00000cf0: 2074 6865 206d 6f64 656c 7320 6172 6520   the models are 
+00000d00: 7065 7274 7572 6265 642e 2054 6f20 7265  perturbed. To re
+00000d10: 7072 6573 656e 7420 7468 6573 6520 6368  present these ch
+00000d20: 616e 6765 7320 6f76 6572 2061 2072 616e  anges over a ran
+00000d30: 6765 206f 6620 7468 6520 7065 7274 7572  ge of the pertur
+00000d40: 6261 7469 6f6e 2063 6f6e 7472 6f6c 2070  bation control p
+00000d50: 6172 616d 6574 6572 2c20 7765 2063 6f6d  arameter, we com
+00000d60: 7075 7465 2061 6e64 2064 6973 706c 6179  pute and display
+00000d70: 2074 6865 2064 6973 7472 6962 7574 696f   the distributio
+00000d80: 6e73 206f 6620 7468 6573 6520 7761 7665  ns of these wave
+00000d90: 666f 726d 732e 2057 6520 696c 6c75 7374  forms. We illust
+00000da0: 7261 7465 2074 6865 7365 2070 726f 6365  rate these proce
+00000db0: 6475 7265 7320 696e 2073 6978 2065 7861  dures in six exa
+00000dc0: 6d70 6c65 7320 6f66 2062 7572 7374 696e  mples of burstin
+00000dd0: 6720 6d6f 6465 6c20 6e65 7572 6f6e 7320  g model neurons 
+00000de0: 7769 7468 2073 696d 696c 6172 2061 6374  with similar act
+00000df0: 6976 6974 7920 6275 7420 7468 6174 2064  ivity but that d
+00000e00: 6966 6665 7220 6173 206d 7563 6820 6173  iffer as much as
+00000e10: 2074 6872 6565 666f 6c64 2069 6e20 7468   threefold in th
+00000e20: 6569 7220 636f 6e64 7563 7461 6e63 6520  eir conductance 
+00000e30: 6465 6e73 6974 6965 732e 2054 6865 7365  densities. These
+00000e40: 2076 6973 7561 6c69 7a61 7469 6f6e 206d   visualization m
+00000e50: 6574 686f 6473 2070 726f 7669 6465 2068  ethods provide h
+00000e60: 6575 7269 7374 6963 2069 6e73 6967 6874  euristic insight
+00000e70: 2069 6e74 6f20 7768 7920 696e 6469 7669   into why indivi
+00000e80: 6475 616c 206e 6575 726f 6e73 206f 7220  dual neurons or 
+00000e90: 6e65 7477 6f72 6b73 2077 6974 6820 7369  networks with si
+00000ea0: 6d69 6c61 7220 6265 6861 7669 6f72 2063  milar behavior c
+00000eb0: 616e 2072 6573 706f 6e64 2077 6964 656c  an respond widel
+00000ec0: 7920 6469 6666 6572 656e 746c 7920 746f  y differently to
+00000ed0: 2070 6572 7475 7262 6174 696f 6e73 2e7d   perturbations.}
+00000ee0: 2c0a 2020 2020 6b65 7977 6f72 6473 203d  ,.    keywords =
+00000ef0: 207b 6e65 7572 6f6e 616c 206f 7363 696c   {neuronal oscil
+00000f00: 6c61 746f 7273 2c20 4e61 2b20 6368 616e  lators, Na+ chan
+00000f10: 6e65 6c73 2c20 4361 2b2b 2063 6861 6e6e  nels, Ca++ chann
+00000f20: 656c 732c 204b 2b20 6368 616e 6e65 6c73  els, K+ channels
+00000f30: 2c20 636f 6e64 7563 7461 6e63 652d 6261  , conductance-ba
+00000f40: 7365 642c 2069 6f6e 6963 2063 6861 6e6e  sed, ionic chann
+00000f50: 656c 737d 2c0a 2020 2020 6a6f 7572 6e61  els},.    journa
+00000f60: 6c20 3d20 7b65 4c69 6665 7d2c 0a20 2020  l = {eLife},.   
+00000f70: 2069 7373 6e20 3d20 7b32 3035 302d 3038   issn = {2050-08
+00000f80: 3458 7d2c 0a20 2020 2070 7562 6c69 7368  4X},.    publish
+00000f90: 6572 203d 207b 654c 6966 6520 5363 6965  er = {eLife Scie
+00000fa0: 6e63 6573 2050 7562 6c69 6361 7469 6f6e  nces Publication
+00000fb0: 732c 204c 7464 7d2c 0a20 2020 207d 0a0a  s, Ltd},.    }..
+00000fc0: 5375 7070 6f72 740a 3d3d 3d3d 3d3d 3d0a  Support.=======.
+00000fd0: 0a57 6520 6172 6520 7072 6f76 6964 696e  .We are providin
+00000fe0: 6720 7375 7070 6f72 7420 6f6e 2060 4769  g support on `Gi
+00000ff0: 7474 6572 203c 6874 7470 733a 2f2f 6769  tter <https://gi
+00001000: 7474 6572 2e69 6d2f 426c 7565 4272 6169  tter.im/BlueBrai
+00001010: 6e2f 4375 7272 656e 7473 6361 7065 3e60  n/Currentscape>`
+00001020: 5f2e 2057 6520 7375 6767 6573 7420 796f  _. We suggest yo
+00001030: 7520 6372 6561 7465 2074 6963 6b65 7473  u create tickets
+00001040: 206f 6e20 7468 6520 6047 6974 6875 6220   on the `Github 
+00001050: 6973 7375 6520 7472 6163 6b65 7220 3c68  issue tracker <h
+00001060: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001070: 6d2f 426c 7565 4272 6169 6e2f 4375 7272  m/BlueBrain/Curr
+00001080: 656e 7473 6361 7065 2f69 7373 7565 733e  entscape/issues>
+00001090: 605f 2069 6e20 6361 7365 2079 6f75 2065  `_ in case you e
+000010a0: 6e63 6f75 6e74 6572 2070 726f 626c 656d  ncounter problem
+000010b0: 7320 7768 696c 6520 7573 696e 6720 7468  s while using th
+000010c0: 6520 736f 6674 7761 7265 206f 7220 6966  e software or if
+000010d0: 2079 6f75 2068 6176 6520 736f 6d65 2073   you have some s
+000010e0: 7567 6765 7374 696f 6e73 2e0a 0a4d 6169  uggestions...Mai
+000010f0: 6e20 6465 7065 6e64 656e 6369 6573 0a3d  n dependencies.=
+00001100: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00001110: 0a0a 2d20 6050 7974 686f 6e20 332e 372b  ..- `Python 3.7+
+00001120: 203c 6874 7470 733a 2f2f 7777 772e 7079   <https://www.py
+00001130: 7468 6f6e 2e6f 7267 2f64 6f77 6e6c 6f61  thon.org/downloa
+00001140: 6473 2f72 656c 6561 7365 2f70 7974 686f  ds/release/pytho
+00001150: 6e2d 3337 302f 3e60 5f0a 2d20 604e 756d  n-370/>`_.- `Num
+00001160: 7079 203c 6874 7470 733a 2f2f 6e75 6d70  py <https://nump
+00001170: 792e 6f72 672f 3e60 5f20 2861 7574 6f6d  y.org/>`_ (autom
+00001180: 6174 6963 616c 6c79 2069 6e73 7461 6c6c  atically install
+00001190: 6564 2062 7920 7069 7029 0a2d 2060 5061  ed by pip).- `Pa
+000011a0: 6c65 7474 6162 6c65 203c 6874 7470 733a  lettable <https:
+000011b0: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 6966  //github.com/jif
+000011c0: 6679 636c 7562 2f70 616c 6574 7461 626c  fyclub/palettabl
+000011d0: 653e 605f 2028 6175 746f 6d61 7469 6361  e>`_ (automatica
+000011e0: 6c6c 7920 696e 7374 616c 6c65 6420 6279  lly installed by
+000011f0: 2070 6970 290a 0a49 6e73 7461 6c6c 6174   pip)..Installat
+00001200: 696f 6e0a 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ion.============
+00001210: 0a0a 4375 7272 656e 7473 6361 7065 2063  ..Currentscape c
+00001220: 616e 2062 6520 7069 7020 696e 7374 616c  an be pip instal
+00001230: 6c65 6420 7769 7468 2074 6865 2066 6f6c  led with the fol
+00001240: 6c6f 7769 6e67 2063 6f6d 6d61 6e64 3a0a  lowing command:.
+00001250: 0a2e 2e20 636f 6465 2d62 6c6f 636b 3a3a  ... code-block::
+00001260: 2070 7974 686f 6e0a 0a20 2020 2070 6970   python..    pip
+00001270: 2069 6e73 7461 6c6c 2063 7572 7265 6e74   install current
+00001280: 7363 6170 650a 0a49 6620 796f 7520 7761  scape..If you wa
+00001290: 6e74 2074 6f20 6265 2061 626c 6520 746f  nt to be able to
+000012a0: 2072 756e 2074 6865 2043 7572 7265 6e74   run the Current
+000012b0: 7363 6170 6520 6578 616d 706c 6573 2c20  scape examples, 
+000012c0: 796f 7520 7769 6c6c 206e 6565 6420 746f  you will need to
+000012d0: 2061 6c73 6f20 696e 7374 616c 6c20 7468   also install th
+000012e0: 6520 6578 616d 706c 6520 6465 7065 6e64  e example depend
+000012f0: 656e 6369 6573 3a0a 0a2e 2e20 636f 6465  encies:.... code
+00001300: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0a  -block:: python.
+00001310: 0a20 2020 2070 6970 2069 6e73 7461 6c6c  .    pip install
+00001320: 2063 7572 7265 6e74 7363 6170 655b 6578   currentscape[ex
+00001330: 616d 706c 655d 0a0a 5175 6963 6b20 5374  ample]..Quick St
+00001340: 6172 740a 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a  art.===========.
+00001350: 0a42 656c 6f77 2069 7320 616e 2065 7861  .Below is an exa
+00001360: 6d70 6c65 206f 6620 6120 6261 6c6c 2061  mple of a ball a
+00001370: 6e64 2073 7469 636b 206d 6f64 656c 2069  nd stick model i
+00001380: 6e20 4e45 5552 4f4e 2077 6974 6820 7369  n NEURON with si
+00001390: 6d70 6c65 2048 6f64 676b 696e 2d48 7578  mple Hodgkin-Hux
+000013a0: 6c65 7920 6d65 6368 616e 6973 6d73 2c20  ley mechanisms, 
+000013b0: 746f 2077 6869 6368 2061 2073 7465 7020  to which a step 
+000013c0: 7374 696d 756c 7573 2069 7320 6170 706c  stimulus is appl
+000013d0: 6965 642e 0a0a 5468 6520 766f 6c74 6167  ied...The voltag
+000013e0: 6520 616e 6420 696f 6e69 6320 6375 7272  e and ionic curr
+000013f0: 656e 7473 2061 7265 2072 6563 6f72 6465  ents are recorde
+00001400: 6420 616e 6420 6665 6420 746f 2043 7572  d and fed to Cur
+00001410: 7265 6e74 7363 6170 652c 2061 6c6f 6e67  rentscape, along
+00001420: 2077 6974 6820 6120 636f 6e66 6967 7572   with a configur
+00001430: 6174 696f 6e20 6469 6374 696f 6e61 7279  ation dictionary
+00001440: 2063 6f6e 7461 696e 696e 6720 7468 6520   containing the 
+00001450: 6375 7272 656e 7420 6e61 6d65 7320 746f  current names to
+00001460: 2062 6520 6469 7370 6c61 7965 6420 696e   be displayed in
+00001470: 2074 6865 206c 6567 656e 642e 0a0a 546f   the legend...To
+00001480: 2072 756e 2074 6865 2063 6f64 6520 796f   run the code yo
+00001490: 7520 7769 6c6c 2066 6972 7374 2068 6176  u will first hav
+000014a0: 6520 746f 2069 6e73 7461 6c6c 204e 4555  e to install NEU
+000014b0: 524f 4e20 7061 636b 6167 653a 0a0a 2e2e  RON package:....
+000014c0: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
+000014d0: 7468 6f6e 0a0a 2020 2020 7069 7020 696e  thon..    pip in
+000014e0: 7374 616c 6c20 6e65 7572 6f6e 0a0a 5768  stall neuron..Wh
+000014f0: 656e 2079 6f75 2074 6865 6e20 6578 6563  en you then exec
+00001500: 7574 6520 7468 6520 666f 6c6c 6f77 696e  ute the followin
+00001510: 6720 7079 7468 6f6e 2063 6f64 652c 2061  g python code, a
+00001520: 2077 696e 646f 7720 7368 6f75 6c64 206f   window should o
+00001530: 7065 6e20 7769 7468 2074 6865 2063 7572  pen with the cur
+00001540: 7265 6e74 7363 6170 6520 706c 6f74 3a0a  rentscape plot:.
+00001550: 0a2e 2e20 636f 6465 2d62 6c6f 636b 3a3a  ... code-block::
+00001560: 2070 7974 686f 6e0a 0a20 2020 2069 6d70   python..    imp
+00001570: 6f72 7420 6e75 6d70 7920 6173 206e 700a  ort numpy as np.
+00001580: 2020 2020 6672 6f6d 206e 6575 726f 6e20      from neuron 
+00001590: 696d 706f 7274 2068 0a20 2020 2066 726f  import h.    fro
+000015a0: 6d20 6e65 7572 6f6e 2e75 6e69 7473 2069  m neuron.units i
+000015b0: 6d70 6f72 7420 6d73 2c20 6d56 0a20 2020  mport ms, mV.   
+000015c0: 2066 726f 6d20 6375 7272 656e 7473 6361   from currentsca
+000015d0: 7065 2e63 7572 7265 6e74 7363 6170 6520  pe.currentscape 
+000015e0: 696d 706f 7274 2070 6c6f 745f 6375 7272  import plot_curr
+000015f0: 656e 7473 6361 7065 0a0a 2020 2020 682e  entscape..    h.
+00001600: 6c6f 6164 5f66 696c 6528 2773 7464 7275  load_file('stdru
+00001610: 6e2e 686f 6327 290a 0a20 2020 2073 6f6d  n.hoc')..    som
+00001620: 6120 3d20 682e 5365 6374 696f 6e28 6e61  a = h.Section(na
+00001630: 6d65 3d27 736f 6d61 2729 0a20 2020 2064  me='soma').    d
+00001640: 656e 6420 3d20 682e 5365 6374 696f 6e28  end = h.Section(
+00001650: 6e61 6d65 3d27 6465 6e64 2729 0a0a 2020  name='dend')..  
+00001660: 2020 6465 6e64 2e63 6f6e 6e65 6374 2873    dend.connect(s
+00001670: 6f6d 6128 3129 290a 0a20 2020 2073 6f6d  oma(1))..    som
+00001680: 612e 4c20 3d20 736f 6d61 2e64 6961 6d20  a.L = soma.diam 
+00001690: 3d20 3132 2e36 3135 370a 2020 2020 6465  = 12.6157.    de
+000016a0: 6e64 2e4c 203d 2032 3030 0a20 2020 2064  nd.L = 200.    d
+000016b0: 656e 642e 6469 616d 203d 2031 0a0a 2020  end.diam = 1..  
+000016c0: 2020 666f 7220 7365 6320 696e 2068 2e61    for sec in h.a
+000016d0: 6c6c 7365 6328 293a 0a20 2020 2020 2020  llsec():.       
+000016e0: 2073 6563 2e52 6120 3d20 3130 3020 2020   sec.Ra = 100   
+000016f0: 2023 2041 7869 616c 2072 6573 6973 7461   # Axial resista
+00001700: 6e63 6520 696e 204f 686d 202a 2063 6d0a  nce in Ohm * cm.
+00001710: 2020 2020 2020 2020 7365 632e 636d 203d          sec.cm =
+00001720: 2031 2020 2020 2020 2320 4d65 6d62 7261   1      # Membra
+00001730: 6e65 2063 6170 6163 6974 616e 6365 2069  ne capacitance i
+00001740: 6e20 6d69 6372 6f20 4661 7261 6473 202f  n micro Farads /
+00001750: 2063 6d5e 320a 0a20 2020 2023 2049 6e73   cm^2..    # Ins
+00001760: 6572 7420 6163 7469 7665 2048 6f64 676b  ert active Hodgk
+00001770: 696e 2d48 7578 6c65 7920 6375 7272 656e  in-Huxley curren
+00001780: 7420 696e 2074 6865 2073 6f6d 610a 2020  t in the soma.  
+00001790: 2020 736f 6d61 2e69 6e73 6572 7428 2768    soma.insert('h
+000017a0: 6827 290a 2020 2020 666f 7220 7365 6720  h').    for seg 
+000017b0: 696e 2073 6f6d 613a 0a20 2020 2020 2020  in soma:.       
+000017c0: 2073 6567 2e68 682e 676e 6162 6172 203d   seg.hh.gnabar =
+000017d0: 2030 2e31 3220 2023 2053 6f64 6975 6d20   0.12  # Sodium 
+000017e0: 636f 6e64 7563 7461 6e63 6520 696e 2053  conductance in S
+000017f0: 2f63 6d32 0a20 2020 2020 2020 2073 6567  /cm2.        seg
+00001800: 2e68 682e 676b 6261 7220 3d20 302e 3033  .hh.gkbar = 0.03
+00001810: 3620 2023 2050 6f74 6173 7369 756d 2063  6  # Potassium c
+00001820: 6f6e 6475 6374 616e 6365 2069 6e20 532f  onductance in S/
+00001830: 636d 320a 2020 2020 2020 2020 7365 672e  cm2.        seg.
+00001840: 6868 2e67 6c20 3d20 302e 3030 3033 2020  hh.gl = 0.0003  
+00001850: 2020 2320 4c65 616b 2063 6f6e 6475 6374    # Leak conduct
+00001860: 616e 6365 2069 6e20 532f 636d 320a 2020  ance in S/cm2.  
+00001870: 2020 2020 2020 7365 672e 6868 2e65 6c20        seg.hh.el 
+00001880: 3d20 2d35 342e 3320 2020 2020 2320 5265  = -54.3     # Re
+00001890: 7665 7273 616c 2070 6f74 656e 7469 616c  versal potential
+000018a0: 2069 6e20 6d56 0a0a 2020 2020 2320 496e   in mV..    # In
+000018b0: 7365 7274 2070 6173 7369 7665 2063 7572  sert passive cur
+000018c0: 7265 6e74 2069 6e20 7468 6520 6465 6e64  rent in the dend
+000018d0: 7269 7465 0a20 2020 2064 656e 642e 696e  rite.    dend.in
+000018e0: 7365 7274 2827 7061 7327 290a 2020 2020  sert('pas').    
+000018f0: 666f 7220 7365 6720 696e 2064 656e 643a  for seg in dend:
+00001900: 0a20 2020 2020 2020 2073 6567 2e70 6173  .        seg.pas
+00001910: 2e67 203d 2030 2e30 3031 2020 2320 5061  .g = 0.001  # Pa
+00001920: 7373 6976 6520 636f 6e64 7563 7461 6e63  ssive conductanc
+00001930: 6520 696e 2053 2f63 6d32 0a20 2020 2020  e in S/cm2.     
+00001940: 2020 2073 6567 2e70 6173 2e65 203d 202d     seg.pas.e = -
+00001950: 3635 2020 2020 2320 4c65 616b 2072 6576  65    # Leak rev
+00001960: 6572 7361 6c20 706f 7465 6e74 6961 6c20  ersal potential 
+00001970: 6d56 0a0a 2020 2020 7374 696d 203d 2068  mV..    stim = h
+00001980: 2e49 436c 616d 7028 6465 6e64 2831 2929  .IClamp(dend(1))
+00001990: 0a20 2020 2073 7469 6d2e 6465 6c61 7920  .    stim.delay 
+000019a0: 3d20 350a 2020 2020 7374 696d 2e64 7572  = 5.    stim.dur
+000019b0: 203d 2031 300a 2020 2020 7374 696d 2e61   = 10.    stim.a
+000019c0: 6d70 203d 2030 2e31 0a0a 2020 2020 6375  mp = 0.1..    cu
+000019d0: 7272 656e 745f 6e61 6d65 7320 3d20 5b22  rrent_names = ["
+000019e0: 696b 222c 2022 696e 6122 2c20 2269 6c5f  ik", "ina", "il_
+000019f0: 6868 225d 0a20 2020 2074 5f76 6563 203d  hh"].    t_vec =
+00001a00: 2068 2e56 6563 746f 7228 290a 2020 2020   h.Vector().    
+00001a10: 765f 7665 6320 3d20 682e 5665 6374 6f72  v_vec = h.Vector
+00001a20: 2829 0a20 2020 2069 6b5f 7665 6320 3d20  ().    ik_vec = 
+00001a30: 682e 5665 6374 6f72 2829 0a20 2020 2069  h.Vector().    i
+00001a40: 6e61 5f76 6563 203d 2068 2e56 6563 746f  na_vec = h.Vecto
+00001a50: 7228 290a 2020 2020 696c 5f76 6563 203d  r().    il_vec =
+00001a60: 2068 2e56 6563 746f 7228 290a 2020 2020   h.Vector().    
+00001a70: 745f 7665 632e 7265 636f 7264 2868 2e5f  t_vec.record(h._
+00001a80: 7265 665f 7429 0a20 2020 2076 5f76 6563  ref_t).    v_vec
+00001a90: 2e72 6563 6f72 6428 736f 6d61 2830 2e35  .record(soma(0.5
+00001aa0: 292e 5f72 6566 5f76 290a 2020 2020 696b  )._ref_v).    ik
+00001ab0: 5f76 6563 2e72 6563 6f72 6428 736f 6d61  _vec.record(soma
+00001ac0: 2830 2e35 292e 5f72 6566 5f69 6b29 0a20  (0.5)._ref_ik). 
+00001ad0: 2020 2069 6e61 5f76 6563 2e72 6563 6f72     ina_vec.recor
+00001ae0: 6428 736f 6d61 2830 2e35 292e 5f72 6566  d(soma(0.5)._ref
+00001af0: 5f69 6e61 290a 2020 2020 696c 5f76 6563  _ina).    il_vec
+00001b00: 2e72 6563 6f72 6428 736f 6d61 2830 2e35  .record(soma(0.5
+00001b10: 292e 5f72 6566 5f69 6c5f 6868 290a 0a20  )._ref_il_hh).. 
+00001b20: 2020 2068 2e66 696e 6974 6961 6c69 7a65     h.finitialize
+00001b30: 282d 3635 202a 206d 5629 0a20 2020 2068  (-65 * mV).    h
+00001b40: 2e63 6f6e 7469 6e75 6572 756e 2832 3520  .continuerun(25 
+00001b50: 2a20 6d73 290a 0a20 2020 2074 6f5f 7041  * ms)..    to_pA
+00001b60: 203d 2031 3020 2a20 736f 6d61 2830 2e35   = 10 * soma(0.5
+00001b70: 292e 6172 6561 2829 2023 2074 7572 6e20  ).area() # turn 
+00001b80: 6d41 2f63 6d32 2028 2a75 6d32 2920 696e  mA/cm2 (*um2) in
+00001b90: 746f 2070 410a 2020 2020 766f 6c74 6167  to pA.    voltag
+00001ba0: 6520 3d20 6e70 2e61 7361 7272 6179 2876  e = np.asarray(v
+00001bb0: 5f76 6563 290a 2020 2020 706f 7461 7373  _vec).    potass
+00001bc0: 6975 6d20 3d20 6e70 2e61 7361 7272 6179  ium = np.asarray
+00001bd0: 2869 6b5f 7665 6329 202a 2074 6f5f 7041  (ik_vec) * to_pA
+00001be0: 0a20 2020 2073 6f64 6975 6d20 3d20 6e70  .    sodium = np
+00001bf0: 2e61 7361 7272 6179 2869 6e61 5f76 6563  .asarray(ina_vec
+00001c00: 2920 2a20 746f 5f70 410a 2020 2020 6c65  ) * to_pA.    le
+00001c10: 616b 203d 206e 702e 6173 6172 7261 7928  ak = np.asarray(
+00001c20: 696c 5f76 6563 2920 2a20 746f 5f70 410a  il_vec) * to_pA.
+00001c30: 0a20 2020 2063 6f6e 6669 6720 3d20 7b0a  .    config = {.
+00001c40: 2020 2020 2020 2020 226f 7574 7075 7422          "output"
+00001c50: 3a20 7b20 2020 2020 2020 2020 2020 2020  : {             
+00001c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c90: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00001ca0: 2020 2273 6176 6566 6967 223a 2054 7275    "savefig": Tru
+00001cb0: 652c 2020 2020 2020 2020 2020 2020 2020  e,              
+00001cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ce0: 2020 2020 2020 2020 2020 2020 200a 2020               .  
+00001cf0: 2020 2020 2020 2020 2264 6972 223a 2022          "dir": "
+00001d00: 2e22 2c20 2020 2020 2020 2020 2020 2020  .",             
+00001d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d40: 2020 200a 2020 2020 2020 2020 2020 2266     .          "f
+00001d50: 6e61 6d65 223a 2022 7175 6963 6b73 7461  name": "quicksta
+00001d60: 7274 5f70 6c6f 7422 2c20 2020 2020 2020  rt_plot",       
+00001d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d90: 2020 2020 2020 2020 200a 2020 2020 2020           .      
+00001da0: 2020 2020 2265 7874 656e 7369 6f6e 223a      "extension":
+00001db0: 2022 706e 6722 2c20 2020 2020 2020 2020   "png",         
+00001dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001de0: 2020 2020 2020 2020 2020 2020 2020 200a                 .
+00001df0: 2020 2020 2020 2020 2020 2264 7069 223a            "dpi":
+00001e00: 2033 3030 2c20 2020 2020 2020 2020 2020   300,           
+00001e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e40: 2020 2020 200a 2020 2020 2020 2020 2020       .          
+00001e50: 2274 7261 6e73 7061 7265 6e74 223a 2046  "transparent": F
+00001e60: 616c 7365 2020 2020 2020 2020 2020 2020  alse            
+00001e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e90: 2020 2020 2020 2020 2020 200a 2020 2020             .    
+00001ea0: 2020 2020 7d2c 2020 200a 2020 2020 2020      },   .      
+00001eb0: 2020 2263 7572 7265 6e74 223a 207b 226e    "current": {"n
+00001ec0: 616d 6573 223a 2063 7572 7265 6e74 5f6e  ames": current_n
+00001ed0: 616d 6573 7d2c 0a20 2020 2020 2020 2022  ames},.        "
+00001ee0: 766f 6c74 6167 6522 3a20 7b22 796c 696d  voltage": {"ylim
+00001ef0: 223a 205b 2d39 302c 2035 305d 7d2c 0a20  ": [-90, 50]},. 
+00001f00: 2020 2020 2020 2022 6c65 6765 6e64 7465         "legendte
+00001f10: 7874 7369 7a65 223a 2035 2c0a 2020 2020  xtsize": 5,.    
+00001f20: 7d0a 2020 2020 6669 6720 3d20 706c 6f74  }.    fig = plot
+00001f30: 5f63 7572 7265 6e74 7363 6170 6528 766f  _currentscape(vo
+00001f40: 6c74 6167 652c 205b 706f 7461 7373 6975  ltage, [potassiu
+00001f50: 6d2c 2073 6f64 6975 6d2c 206c 6561 6b5d  m, sodium, leak]
+00001f60: 2c20 636f 6e66 6967 290a 2020 2020 6669  , config).    fi
+00001f70: 672e 7368 6f77 2829 0a0a 5768 656e 2079  g.show()..When y
+00001f80: 6f75 2072 756e 2074 6869 7320 636f 6465  ou run this code
+00001f90: 2069 6e20 5079 7468 6f6e 2c20 6974 2077   in Python, it w
+00001fa0: 696c 6c20 6765 6e65 7261 7465 2074 6865  ill generate the
+00001fb0: 2066 6f6c 6c6f 7769 6e67 2063 7572 7265   following curre
+00001fc0: 6e74 7363 6170 6520 706c 6f74 2028 696e  ntscape plot (in
+00001fd0: 2061 2077 696e 646f 772c 2061 6e64 206f   a window, and o
+00001fe0: 6e20 6469 736b 2061 7320 7175 6963 6b73  n disk as quicks
+00001ff0: 7461 7274 5f70 6c6f 742e 706e 6729 3a0a  tart_plot.png):.
+00002000: 0a2e 2e20 696d 6167 653a 3a20 646f 632f  ... image:: doc/
+00002010: 736f 7572 6365 2f69 6d61 6765 732f 7175  source/images/qu
+00002020: 6963 6b73 7461 7274 5f70 6c6f 742e 706e  ickstart_plot.pn
+00002030: 670a 0a54 7574 6f72 6961 6c0a 3d3d 3d3d  g..Tutorial.====
+00002040: 3d3d 3d3d 0a0a 4120 6d6f 7265 2064 6574  ====..A more det
+00002050: 6169 6c65 6420 6578 706c 616e 6174 696f  ailed explanatio
+00002060: 6e20 6f6e 2068 6f77 2074 6f20 7573 6520  n on how to use 
+00002070: 4375 7272 656e 7473 6361 7065 2c20 6173  Currentscape, as
+00002080: 2077 656c 6c20 6173 206f 7468 6572 2065   well as other e
+00002090: 7861 6d70 6c65 7320 6361 6e20 6265 2066  xamples can be f
+000020a0: 6f75 6e64 206f 6e20 7468 6520 6074 7574  ound on the `tut
+000020b0: 6f72 6961 6c20 7061 6765 203c 5475 746f  orial page <Tuto
+000020c0: 7269 616c 2e72 7374 3e60 5f2e 0a0a 4150  rial.rst>`_...AP
+000020d0: 4920 446f 6375 6d65 6e74 6174 696f 6e0a  I Documentation.
+000020e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000020f0: 3d0a 0a54 6865 2041 5049 2064 6f63 756d  =..The API docum
+00002100: 656e 7461 7469 6f6e 2063 616e 2062 6520  entation can be 
+00002110: 666f 756e 6420 6f6e 2060 5265 6164 5468  found on `ReadTh
+00002120: 6544 6f63 7320 3c22 6874 7470 733a 2f2f  eDocs <"https://
+00002130: 6375 7272 656e 7473 6361 7065 2e72 6561  currentscape.rea
+00002140: 6474 6865 646f 6373 2e69 6f22 3e60 5f2e  dthedocs.io">`_.
+00002150: 0a0a 4675 6e64 696e 6720 2620 4163 6b6e  ..Funding & Ackn
+00002160: 6f77 6c65 6467 656d 656e 7473 0a3d 3d3d  owledgements.===
+00002170: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00002180: 3d3d 3d3d 3d3d 3d0a 0a57 6520 7769 7368  =======..We wish
+00002190: 2074 6f20 7468 616e 6b20 7468 6520 6175   to thank the au
+000021a0: 7468 6f72 7320 6f66 2060 416c 6f6e 736f  thors of `Alonso
+000021b0: 2061 6e64 204d 6172 6465 722c 2032 3031   and Marder, 201
+000021c0: 3920 3c68 7474 7073 3a2f 2f64 6f69 2e6f  9 <https://doi.o
+000021d0: 7267 2f31 302e 3735 3534 2f65 4c69 6665  rg/10.7554/eLife
+000021e0: 2e34 3237 3232 3e60 5f5f 2074 6f20 6c65  .42722>`__ to le
+000021f0: 7420 7573 2069 6e74 6567 7261 7465 2061  t us integrate a
+00002200: 2070 6172 7420 6f66 2074 6865 6972 2060   part of their `
+00002210: 636f 6465 203c 6874 7470 733a 2f2f 6461  code <https://da
+00002220: 7461 6472 7961 642e 6f72 672f 7374 6173  tadryad.org/stas
+00002230: 682f 6461 7461 7365 742f 646f 693a 3130  h/dataset/doi:10
+00002240: 2e35 3036 312f 6472 7961 642e 6430 3737  .5061/dryad.d077
+00002250: 396d 623e 605f 2069 6e74 6f20 7468 6973  9mb>`_ into this
+00002260: 2072 6570 6f73 6974 6f72 792e 0a0a 5468   repository...Th
+00002270: 6520 7061 7274 206f 6620 7468 6520 636f  e part of the co
+00002280: 6465 2069 6e20 7468 6973 2072 6570 6f73  de in this repos
+00002290: 6974 6f72 7920 6465 7665 6c6f 7065 6420  itory developed 
+000022a0: 6279 2074 6865 2045 5046 4c20 426c 7565  by the EPFL Blue
+000022b0: 2042 7261 696e 2050 726f 6a65 6374 2077   Brain Project w
+000022c0: 6173 2073 7570 706f 7274 6564 2062 7920  as supported by 
+000022d0: 6675 6e64 696e 6720 746f 2074 6865 2042  funding to the B
+000022e0: 6c75 6520 4272 6169 6e20 5072 6f6a 6563  lue Brain Projec
+000022f0: 742c 2061 2072 6573 6561 7263 6820 6365  t, a research ce
+00002300: 6e74 6572 206f 6620 7468 6520 c389 636f  nter of the ..co
+00002310: 6c65 2070 6f6c 7974 6563 686e 6971 7565  le polytechnique
+00002320: 2066 c3a9 64c3 a972 616c 6520 6465 204c   f..d..rale de L
+00002330: 6175 7361 6e6e 6520 2845 5046 4c29 2c20  ausanne (EPFL), 
+00002340: 6672 6f6d 2074 6865 2053 7769 7373 2067  from the Swiss g
+00002350: 6f76 6572 6e6d 656e 7427 7320 4554 4820  overnment's ETH 
+00002360: 426f 6172 6420 6f66 2074 6865 2053 7769  Board of the Swi
+00002370: 7373 2046 6564 6572 616c 2049 6e73 7469  ss Federal Insti
+00002380: 7475 7465 7320 6f66 2054 6563 686e 6f6c  tutes of Technol
+00002390: 6f67 792e 0a0a 0a2e 2e20 7c70 7970 697c  ogy...... |pypi|
+000023a0: 2069 6d61 6765 3a3a 2068 7474 7073 3a2f   image:: https:/
+000023b0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+000023c0: 7079 7069 2f76 2f63 7572 7265 6e74 7363  pypi/v/currentsc
+000023d0: 6170 652e 7376 670a 2020 2020 2020 2020  ape.svg.        
+000023e0: 2020 2020 2020 203a 7461 7267 6574 3a20         :target: 
+000023f0: 6874 7470 733a 2f2f 7465 7374 2e70 7970  https://test.pyp
+00002400: 692e 6f72 672f 7072 6f6a 6563 742f 6375  i.org/project/cu
+00002410: 7272 656e 7473 6361 7065 2f0a 2020 2020  rrentscape/.    
+00002420: 2020 2020 2020 2020 2020 203a 616c 743a             :alt:
+00002430: 206c 6174 6573 7420 7265 6c65 6173 650a   latest release.
+00002440: 0a2e 2e20 7c64 6f63 737c 2069 6d61 6765  ... |docs| image
+00002450: 3a3a 2068 7474 7073 3a2f 2f72 6561 6474  :: https://readt
+00002460: 6865 646f 6373 2e6f 7267 2f70 726f 6a65  hedocs.org/proje
+00002470: 6374 732f 6375 7272 656e 7473 6361 7065  cts/currentscape
+00002480: 2f62 6164 6765 2f3f 7665 7273 696f 6e3d  /badge/?version=
+00002490: 6c61 7465 7374 0a20 2020 2020 2020 2020  latest.         
+000024a0: 2020 2020 2020 3a74 6172 6765 743a 2068        :target: h
+000024b0: 7474 7073 3a2f 2f63 7572 7265 6e74 7363  ttps://currentsc
+000024c0: 6170 652e 7265 6164 7468 6564 6f63 732e  ape.readthedocs.
+000024d0: 696f 2f0a 2020 2020 2020 2020 2020 2020  io/.            
+000024e0: 2020 203a 616c 743a 206c 6174 6573 7420     :alt: latest 
+000024f0: 646f 6375 6d65 6e74 6174 696f 6e0a 0a2e  documentation...
+00002500: 2e20 7c6c 6963 656e 7365 7c20 696d 6167  . |license| imag
+00002510: 653a 3a20 6874 7470 733a 2f2f 696d 672e  e:: https://img.
+00002520: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+00002530: 6c2f 6375 7272 656e 7473 6361 7065 2e73  l/currentscape.s
+00002540: 7667 0a20 2020 2020 2020 2020 2020 2020  vg.             
+00002550: 2020 2020 203a 7461 7267 6574 3a20 6874       :target: ht
+00002560: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00002570: 2f42 6c75 6542 7261 696e 2f43 7572 7265  /BlueBrain/Curre
+00002580: 6e74 7363 6170 652f 626c 6f62 2f6d 6169  ntscape/blob/mai
+00002590: 6e2f 4c49 4345 4e53 452e 7478 740a 2020  n/LICENSE.txt.  
+000025a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025b0: 3a61 6c74 3a20 6c69 6365 6e73 650a 0a2e  :alt: license...
+000025c0: 2e20 7c62 7569 6c64 7c20 696d 6167 653a  . |build| image:
+000025d0: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+000025e0: 2e63 6f6d 2f42 6c75 6542 7261 696e 2f43  .com/BlueBrain/C
+000025f0: 7572 7265 6e74 7363 6170 652f 776f 726b  urrentscape/work
+00002600: 666c 6f77 732f 5465 7374 2f62 6164 6765  flows/Test/badge
+00002610: 2e73 7667 3f62 7261 6e63 683d 6d61 696e  .svg?branch=main
+00002620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002630: 203a 7461 7267 6574 3a20 6874 7470 733a   :target: https:
+00002640: 2f2f 6769 7468 7562 2e63 6f6d 2f42 6c75  //github.com/Blu
+00002650: 6542 7261 696e 2f43 7572 7265 6e74 7363  eBrain/Currentsc
+00002660: 6170 652f 6163 7469 6f6e 730a 2020 2020  ape/actions.    
+00002670: 2020 2020 2020 2020 2020 2020 3a61 6c74              :alt
+00002680: 3a20 6163 7469 6f6e 7320 6275 696c 6420  : actions build 
+00002690: 7374 6174 7573 0a0a 2e2e 207c 636f 7665  status.... |cove
+000026a0: 7261 6765 7c20 696d 6167 653a 3a20 6874  rage| image:: ht
+000026b0: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
+000026c0: 2f67 6974 6875 622f 426c 7565 4272 6169  /github/BlueBrai
+000026d0: 6e2f 4375 7272 656e 7473 6361 7065 2f63  n/Currentscape/c
+000026e0: 6f76 6572 6167 652e 7376 673f 6272 616e  overage.svg?bran
+000026f0: 6368 3d6d 6169 6e0a 2020 2020 2020 2020  ch=main.        
+00002700: 2020 2020 2020 2020 2020 203a 7461 7267             :targ
+00002710: 6574 3a20 6874 7470 733a 2f2f 636f 6465  et: https://code
+00002720: 636f 762e 696f 2f67 682f 426c 7565 4272  cov.io/gh/BlueBr
+00002730: 6169 6e2f 6375 7272 656e 7473 6361 7065  ain/currentscape
+00002740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002750: 2020 2020 3a61 6c74 3a20 636f 7665 7261      :alt: covera
+00002760: 6765 0a0a 2e2e 207c 6769 7474 6572 7c20  ge.... |gitter| 
+00002770: 696d 6167 653a 3a20 6874 7470 733a 2f2f  image:: https://
+00002780: 6261 6467 6573 2e67 6974 7465 722e 696d  badges.gitter.im
+00002790: 2f4a 6f69 6e25 3230 4368 6174 2e73 7667  /Join%20Chat.svg
+000027a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000027b0: 2020 3a74 6172 6765 743a 2068 7474 7073    :target: https
+000027c0: 3a2f 2f67 6974 7465 722e 696d 2f62 6c75  ://gitter.im/blu
+000027d0: 6562 7261 696e 2f63 7572 7265 6e74 7363  ebrain/currentsc
+000027e0: 6170 650a 2020 2020 2020 2020 2020 2020  ape.            
+000027f0: 2020 2020 203a 616c 743a 204a 6f69 6e20       :alt: Join 
+00002800: 7468 6520 6368 6174 2061 7420 6874 7470  the chat at http
+00002810: 733a 2f2f 6769 7474 6572 2e69 6d2f 626c  s://gitter.im/bl
+00002820: 7565 6272 6169 6e2f 6375 7272 656e 7473  uebrain/currents
+00002830: 6361 7065 0a                             cape.
```

### Comparing `currentscape-0.0.0/setup.py` & `currentscape-1.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import imp
 import sys
 
 from setuptools import setup, find_packages
 
 if sys.version_info < (3, 7):
     sys.exit("Sorry, Python < 3.7 is not supported")
 
@@ -28,17 +27,18 @@
 
 EXTRA_EXAMPLE = ["scipy", "bluepyopt", "emodelrunner>=1.1.5"]
 
 setup(
     name="currentscape",
     author="Blue Brain Project, EPFL",
     use_scm_version=True,
+    setup_requires=["setuptools_scm"],
     description="Module to easily plot currentscape.",
     long_description=README,
-    long_description_content_type="text/markdown",
+    long_description_content_type="text/x-rst",
     url="https://github.com/BlueBrain/Currentscape",
     project_urls={
         "Tracker": "https://github.com/BlueBrain/Currentscape",
         "Source": "https://github.com/BlueBrain/Currentscape",
     },
     license="Apache 2.0",
     install_requires=[
```

### Comparing `currentscape-0.0.0/tests/extract_bNAC_config.json` & `currentscape-1.0.1/tests/extract_bNAC_config.json`

 * *Files identical despite different names*

### Comparing `currentscape-0.0.0/tests/test_currentscape_config_parser.py` & `currentscape-1.0.1/tests/test_currentscape_config_parser.py`

 * *Files identical despite different names*

### Comparing `currentscape-0.0.0/tests/test_currentscape_currents.py` & `currentscape-1.0.1/tests/test_currentscape_currents.py`

 * *Files identical despite different names*

### Comparing `currentscape-0.0.0/tests/test_currentscape_dataprocessing.py` & `currentscape-1.0.1/tests/test_currentscape_dataprocessing.py`

 * *Files identical despite different names*

### Comparing `currentscape-0.0.0/tests/test_currentscape_datasets.py` & `currentscape-1.0.1/tests/test_currentscape_datasets.py`

 * *Files identical despite different names*

### Comparing `currentscape-0.0.0/tests/test_currentscape_from_paper.py` & `currentscape-1.0.1/tests/test_currentscape_from_paper.py`

 * *Files identical despite different names*

### Comparing `currentscape-0.0.0/tests/test_currentscape_ions.py` & `currentscape-1.0.1/tests/test_currentscape_ions.py`

 * *Files identical despite different names*

### Comparing `currentscape-0.0.0/tests/test_currentscape_mapper.py` & `currentscape-1.0.1/tests/test_currentscape_mapper.py`

 * *Files identical despite different names*

### Comparing `currentscape-0.0.0/tests/test_currentscape_plotting.py` & `currentscape-1.0.1/tests/test_currentscape_plotting.py`

 * *Files identical despite different names*

### Comparing `currentscape-0.0.0/tests/test_use_case_example.py` & `currentscape-1.0.1/tests/test_use_case_example.py`

 * *Files identical despite different names*

