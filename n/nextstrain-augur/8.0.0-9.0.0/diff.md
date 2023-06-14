# Comparing `tmp/nextstrain-augur-8.0.0.tar.gz` & `tmp/nextstrain-augur-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nextstrain-augur-8.0.0.tar", last modified: Mon Jun  8 21:49:27 2020, max compression
+gzip compressed data, was "dist/nextstrain-augur-9.0.0.tar", last modified: Mon Jun 29 20:01:41 2020, max compression
```

## Comparing `nextstrain-augur-8.0.0.tar` & `nextstrain-augur-9.0.0.tar`

### file list

```diff
@@ -1,53 +1,57 @@
-drwxr-xr-x   0 jlhudd     (501) staff       (20)        0 2020-06-08 21:49:27.000000 nextstrain-augur-8.0.0/
--rw-r--r--   0 jlhudd     (501) staff       (20)     7788 2020-06-08 21:49:27.000000 nextstrain-augur-8.0.0/PKG-INFO
--rw-r--r--   0 jlhudd     (501) staff       (20)     5805 2020-04-07 18:09:51.000000 nextstrain-augur-8.0.0/README.md
-drwxr-xr-x   0 jlhudd     (501) staff       (20)        0 2020-06-08 21:49:27.000000 nextstrain-augur-8.0.0/augur/
--rw-r--r--   0 jlhudd     (501) staff       (20)      489 2020-03-24 19:21:38.000000 nextstrain-augur-8.0.0/augur/import.py
--rw-r--r--   0 jlhudd     (501) staff       (20)     7899 2020-06-08 21:49:25.000000 nextstrain-augur-8.0.0/augur/mask.py
--rw-r--r--   0 jlhudd     (501) staff       (20)     9154 2020-06-08 21:49:25.000000 nextstrain-augur-8.0.0/augur/ancestral.py
--rw-r--r--   0 jlhudd     (501) staff       (20)    15890 2020-06-08 21:49:25.000000 nextstrain-augur-8.0.0/augur/tree.py
--rw-r--r--   0 jlhudd     (501) staff       (20)    26944 2020-06-08 21:49:25.000000 nextstrain-augur-8.0.0/augur/import_beast.py
--rw-r--r--   0 jlhudd     (501) staff       (20)    17714 2020-06-08 21:49:25.000000 nextstrain-augur-8.0.0/augur/translate.py
--rw-r--r--   0 jlhudd     (501) staff       (20)      177 2020-03-24 19:21:38.000000 nextstrain-augur-8.0.0/augur/version.py
--rw-r--r--   0 jlhudd     (501) staff       (20)    17525 2020-06-08 21:49:25.000000 nextstrain-augur-8.0.0/augur/align.py
--rw-r--r--   0 jlhudd     (501) staff       (20)     4073 2020-06-08 21:49:25.000000 nextstrain-augur-8.0.0/augur/reconstruct_sequences.py
--rw-r--r--   0 jlhudd     (501) staff       (20)    15740 2020-03-24 19:21:38.000000 nextstrain-augur-8.0.0/augur/export_v1.py
--rw-r--r--   0 jlhudd     (501) staff       (20)       41 2020-03-24 19:21:38.000000 nextstrain-augur-8.0.0/augur/filenames.py
--rw-r--r--   0 jlhudd     (501) staff       (20)    14111 2020-06-08 21:49:25.000000 nextstrain-augur-8.0.0/augur/refine.py
--rw-r--r--   0 jlhudd     (501) staff       (20)     3183 2020-03-24 19:21:38.000000 nextstrain-augur-8.0.0/augur/__init__.py
--rw-r--r--   0 jlhudd     (501) staff       (20)       22 2020-06-08 21:49:25.000000 nextstrain-augur-8.0.0/augur/__version__.py
--rw-r--r--   0 jlhudd     (501) staff       (20)      669 2020-03-24 19:21:38.000000 nextstrain-augur-8.0.0/augur/export.py
--rw-r--r--   0 jlhudd     (501) staff       (20)    23401 2020-06-08 21:49:25.000000 nextstrain-augur-8.0.0/augur/distance.py
--rw-r--r--   0 jlhudd     (501) staff       (20)     7796 2020-06-08 21:49:25.000000 nextstrain-augur-8.0.0/augur/clades.py
--rw-r--r--   0 jlhudd     (501) staff       (20)     5389 2020-06-08 21:49:25.000000 nextstrain-augur-8.0.0/augur/validate.py
--rw-r--r--   0 jlhudd     (501) staff       (20)     5215 2020-06-08 21:49:25.000000 nextstrain-augur-8.0.0/augur/lbi.py
--rw-r--r--   0 jlhudd     (501) staff       (20)    12728 2020-03-30 20:15:18.000000 nextstrain-augur-8.0.0/augur/validate_export.py
--rw-r--r--   0 jlhudd     (501) staff       (20)    33580 2020-06-08 21:49:25.000000 nextstrain-augur-8.0.0/augur/utils.py
--rw-r--r--   0 jlhudd     (501) staff       (20)    48676 2020-03-24 19:21:38.000000 nextstrain-augur-8.0.0/augur/titer_model.py
--rw-r--r--   0 jlhudd     (501) staff       (20)    40301 2020-06-08 21:49:25.000000 nextstrain-augur-8.0.0/augur/export_v2.py
--rw-r--r--   0 jlhudd     (501) staff       (20)    18716 2020-06-08 21:49:25.000000 nextstrain-augur-8.0.0/augur/filter.py
--rw-r--r--   0 jlhudd     (501) staff       (20)     9112 2020-06-08 21:49:25.000000 nextstrain-augur-8.0.0/augur/traits.py
--rw-r--r--   0 jlhudd     (501) staff       (20)    49102 2020-03-24 19:21:38.000000 nextstrain-augur-8.0.0/augur/frequency_estimators.py
--rw-r--r--   0 jlhudd     (501) staff       (20)     5528 2020-03-24 19:21:38.000000 nextstrain-augur-8.0.0/augur/titers.py
--rw-r--r--   0 jlhudd     (501) staff       (20)     4413 2020-06-08 21:49:25.000000 nextstrain-augur-8.0.0/augur/parse.py
--rw-r--r--   0 jlhudd     (501) staff       (20)    13199 2020-04-07 18:09:51.000000 nextstrain-augur-8.0.0/augur/sequence_traits.py
-drwxr-xr-x   0 jlhudd     (501) staff       (20)        0 2020-06-08 21:49:27.000000 nextstrain-augur-8.0.0/augur/data/
--rw-r--r--   0 jlhudd     (501) staff       (20)    14038 2020-03-24 19:21:38.000000 nextstrain-augur-8.0.0/augur/data/lat_longs.tsv
--rw-r--r--   0 jlhudd     (501) staff       (20)      420 2020-03-24 19:21:38.000000 nextstrain-augur-8.0.0/augur/data/colors.tsv
--rw-r--r--   0 jlhudd     (501) staff       (20)     1452 2020-03-24 19:21:38.000000 nextstrain-augur-8.0.0/augur/data/schema-annotations.json
--rw-r--r--   0 jlhudd     (501) staff       (20)     6638 2020-06-08 21:49:25.000000 nextstrain-augur-8.0.0/augur/data/schema-auspice-config-v2.json
--rw-r--r--   0 jlhudd     (501) staff       (20)    25006 2020-06-08 21:49:25.000000 nextstrain-augur-8.0.0/augur/data/schema-export-v2.json
--rw-r--r--   0 jlhudd     (501) staff       (20)    11235 2020-03-24 19:21:38.000000 nextstrain-augur-8.0.0/augur/data/schema-export-v1-meta.json
--rw-r--r--   0 jlhudd     (501) staff       (20)     6476 2020-03-24 19:21:38.000000 nextstrain-augur-8.0.0/augur/data/schema-export-v1-tree.json
--rw-r--r--   0 jlhudd     (501) staff       (20)      337 2020-03-24 19:21:38.000000 nextstrain-augur-8.0.0/augur/__main__.py
--rw-r--r--   0 jlhudd     (501) staff       (20)    11778 2020-06-08 21:49:25.000000 nextstrain-augur-8.0.0/augur/frequencies.py
--rw-r--r--   0 jlhudd     (501) staff       (20)     3361 2020-06-08 21:49:25.000000 nextstrain-augur-8.0.0/setup.py
--rw-r--r--   0 jlhudd     (501) staff       (20)       38 2020-06-08 21:49:27.000000 nextstrain-augur-8.0.0/setup.cfg
-drwxr-xr-x   0 jlhudd     (501) staff       (20)        0 2020-06-08 21:49:27.000000 nextstrain-augur-8.0.0/nextstrain_augur.egg-info/
--rw-r--r--   0 jlhudd     (501) staff       (20)     7788 2020-06-08 21:49:26.000000 nextstrain-augur-8.0.0/nextstrain_augur.egg-info/PKG-INFO
--rw-r--r--   0 jlhudd     (501) staff       (20)     1082 2020-06-08 21:49:26.000000 nextstrain-augur-8.0.0/nextstrain_augur.egg-info/SOURCES.txt
--rw-r--r--   0 jlhudd     (501) staff       (20)       47 2020-06-08 21:49:26.000000 nextstrain-augur-8.0.0/nextstrain_augur.egg-info/entry_points.txt
--rw-r--r--   0 jlhudd     (501) staff       (20)      582 2020-06-08 21:49:26.000000 nextstrain-augur-8.0.0/nextstrain_augur.egg-info/requires.txt
--rw-r--r--   0 jlhudd     (501) staff       (20)        6 2020-06-08 21:49:26.000000 nextstrain-augur-8.0.0/nextstrain_augur.egg-info/top_level.txt
--rw-r--r--   0 jlhudd     (501) staff       (20)        1 2020-06-08 21:49:26.000000 nextstrain-augur-8.0.0/nextstrain_augur.egg-info/dependency_links.txt
--rw-r--r--   0 jlhudd     (501) staff       (20)    32387 2020-03-24 19:21:38.000000 nextstrain-augur-8.0.0/LICENSE.txt
+drwxr-xr-x   0 jlhudd     (501) staff       (20)        0 2020-06-29 20:01:41.000000 nextstrain-augur-9.0.0/
+-rw-r--r--   0 jlhudd     (501) staff       (20)     6624 2020-06-29 20:01:41.000000 nextstrain-augur-9.0.0/PKG-INFO
+-rw-r--r--   0 jlhudd     (501) staff       (20)     4897 2020-06-29 20:01:39.000000 nextstrain-augur-9.0.0/README.md
+drwxr-xr-x   0 jlhudd     (501) staff       (20)        0 2020-06-29 20:01:41.000000 nextstrain-augur-9.0.0/augur/
+-rw-r--r--   0 jlhudd     (501) staff       (20)      489 2020-03-24 19:21:38.000000 nextstrain-augur-9.0.0/augur/import.py
+-rw-r--r--   0 jlhudd     (501) staff       (20)     7899 2020-06-29 19:01:48.000000 nextstrain-augur-9.0.0/augur/mask.py
+-rw-r--r--   0 jlhudd     (501) staff       (20)     9154 2020-06-29 19:01:48.000000 nextstrain-augur-9.0.0/augur/ancestral.py
+-rw-r--r--   0 jlhudd     (501) staff       (20)    15764 2020-06-29 20:01:40.000000 nextstrain-augur-9.0.0/augur/tree.py
+-rw-r--r--   0 jlhudd     (501) staff       (20)    26944 2020-06-29 19:01:48.000000 nextstrain-augur-9.0.0/augur/import_beast.py
+-rw-r--r--   0 jlhudd     (501) staff       (20)    17714 2020-06-29 19:01:48.000000 nextstrain-augur-9.0.0/augur/translate.py
+-rw-r--r--   0 jlhudd     (501) staff       (20)      177 2020-03-24 19:21:38.000000 nextstrain-augur-9.0.0/augur/version.py
+-rw-r--r--   0 jlhudd     (501) staff       (20)    18935 2020-06-29 20:01:40.000000 nextstrain-augur-9.0.0/augur/align.py
+-rw-r--r--   0 jlhudd     (501) staff       (20)     4073 2020-06-29 19:01:48.000000 nextstrain-augur-9.0.0/augur/reconstruct_sequences.py
+-rw-r--r--   0 jlhudd     (501) staff       (20)    15740 2020-03-24 19:21:38.000000 nextstrain-augur-9.0.0/augur/export_v1.py
+-rw-r--r--   0 jlhudd     (501) staff       (20)       41 2020-03-24 19:21:38.000000 nextstrain-augur-9.0.0/augur/filenames.py
+-rw-r--r--   0 jlhudd     (501) staff       (20)    14111 2020-06-29 19:01:48.000000 nextstrain-augur-9.0.0/augur/refine.py
+-rw-r--r--   0 jlhudd     (501) staff       (20)     3183 2020-03-24 19:21:38.000000 nextstrain-augur-9.0.0/augur/__init__.py
+-rw-r--r--   0 jlhudd     (501) staff       (20)       22 2020-06-29 20:01:39.000000 nextstrain-augur-9.0.0/augur/__version__.py
+-rw-r--r--   0 jlhudd     (501) staff       (20)      669 2020-03-24 19:21:38.000000 nextstrain-augur-9.0.0/augur/export.py
+-rw-r--r--   0 jlhudd     (501) staff       (20)    23401 2020-06-29 19:01:48.000000 nextstrain-augur-9.0.0/augur/distance.py
+-rw-r--r--   0 jlhudd     (501) staff       (20)     7796 2020-06-29 19:01:48.000000 nextstrain-augur-9.0.0/augur/clades.py
+-rw-r--r--   0 jlhudd     (501) staff       (20)     5389 2020-06-29 19:01:48.000000 nextstrain-augur-9.0.0/augur/validate.py
+drwxr-xr-x   0 jlhudd     (501) staff       (20)        0 2020-06-29 20:01:41.000000 nextstrain-augur-9.0.0/augur/util_support/
+-rw-r--r--   0 jlhudd     (501) staff       (20)        0 2020-06-29 20:01:40.000000 nextstrain-augur-9.0.0/augur/util_support/__init__.py
+-rw-r--r--   0 jlhudd     (501) staff       (20)     2687 2020-06-29 20:01:40.000000 nextstrain-augur-9.0.0/augur/util_support/shell_command_runner.py
+-rw-r--r--   0 jlhudd     (501) staff       (20)     4101 2020-06-29 20:01:40.000000 nextstrain-augur-9.0.0/augur/util_support/date_disambiguator.py
+-rw-r--r--   0 jlhudd     (501) staff       (20)     5215 2020-06-29 19:01:48.000000 nextstrain-augur-9.0.0/augur/lbi.py
+-rw-r--r--   0 jlhudd     (501) staff       (20)    12728 2020-03-30 20:15:18.000000 nextstrain-augur-9.0.0/augur/validate_export.py
+-rw-r--r--   0 jlhudd     (501) staff       (20)    30733 2020-06-29 20:01:40.000000 nextstrain-augur-9.0.0/augur/utils.py
+-rw-r--r--   0 jlhudd     (501) staff       (20)    48676 2020-03-24 19:21:38.000000 nextstrain-augur-9.0.0/augur/titer_model.py
+-rw-r--r--   0 jlhudd     (501) staff       (20)    41628 2020-06-29 20:01:40.000000 nextstrain-augur-9.0.0/augur/export_v2.py
+-rw-r--r--   0 jlhudd     (501) staff       (20)    19417 2020-06-29 20:01:40.000000 nextstrain-augur-9.0.0/augur/filter.py
+-rw-r--r--   0 jlhudd     (501) staff       (20)     9112 2020-06-29 19:01:48.000000 nextstrain-augur-9.0.0/augur/traits.py
+-rw-r--r--   0 jlhudd     (501) staff       (20)    49103 2020-06-29 20:01:40.000000 nextstrain-augur-9.0.0/augur/frequency_estimators.py
+-rw-r--r--   0 jlhudd     (501) staff       (20)     5528 2020-03-24 19:21:38.000000 nextstrain-augur-9.0.0/augur/titers.py
+-rw-r--r--   0 jlhudd     (501) staff       (20)     4445 2020-06-29 20:01:40.000000 nextstrain-augur-9.0.0/augur/parse.py
+-rw-r--r--   0 jlhudd     (501) staff       (20)    13199 2020-04-07 18:09:51.000000 nextstrain-augur-9.0.0/augur/sequence_traits.py
+drwxr-xr-x   0 jlhudd     (501) staff       (20)        0 2020-06-29 20:01:41.000000 nextstrain-augur-9.0.0/augur/data/
+-rw-r--r--   0 jlhudd     (501) staff       (20)    14038 2020-03-24 19:21:38.000000 nextstrain-augur-9.0.0/augur/data/lat_longs.tsv
+-rw-r--r--   0 jlhudd     (501) staff       (20)      420 2020-03-24 19:21:38.000000 nextstrain-augur-9.0.0/augur/data/colors.tsv
+-rw-r--r--   0 jlhudd     (501) staff       (20)     1452 2020-03-24 19:21:38.000000 nextstrain-augur-9.0.0/augur/data/schema-annotations.json
+-rw-r--r--   0 jlhudd     (501) staff       (20)     6638 2020-06-29 19:01:48.000000 nextstrain-augur-9.0.0/augur/data/schema-auspice-config-v2.json
+-rw-r--r--   0 jlhudd     (501) staff       (20)    25006 2020-06-29 19:01:48.000000 nextstrain-augur-9.0.0/augur/data/schema-export-v2.json
+-rw-r--r--   0 jlhudd     (501) staff       (20)    11235 2020-03-24 19:21:38.000000 nextstrain-augur-9.0.0/augur/data/schema-export-v1-meta.json
+-rw-r--r--   0 jlhudd     (501) staff       (20)     6476 2020-03-24 19:21:38.000000 nextstrain-augur-9.0.0/augur/data/schema-export-v1-tree.json
+-rw-r--r--   0 jlhudd     (501) staff       (20)      337 2020-03-24 19:21:38.000000 nextstrain-augur-9.0.0/augur/__main__.py
+-rw-r--r--   0 jlhudd     (501) staff       (20)    11778 2020-06-29 19:01:48.000000 nextstrain-augur-9.0.0/augur/frequencies.py
+-rw-r--r--   0 jlhudd     (501) staff       (20)     3428 2020-06-29 20:01:40.000000 nextstrain-augur-9.0.0/setup.py
+-rw-r--r--   0 jlhudd     (501) staff       (20)       38 2020-06-29 20:01:41.000000 nextstrain-augur-9.0.0/setup.cfg
+drwxr-xr-x   0 jlhudd     (501) staff       (20)        0 2020-06-29 20:01:41.000000 nextstrain-augur-9.0.0/nextstrain_augur.egg-info/
+-rw-r--r--   0 jlhudd     (501) staff       (20)     6624 2020-06-29 20:01:41.000000 nextstrain-augur-9.0.0/nextstrain_augur.egg-info/PKG-INFO
+-rw-r--r--   0 jlhudd     (501) staff       (20)     1197 2020-06-29 20:01:41.000000 nextstrain-augur-9.0.0/nextstrain_augur.egg-info/SOURCES.txt
+-rw-r--r--   0 jlhudd     (501) staff       (20)       47 2020-06-29 20:01:41.000000 nextstrain-augur-9.0.0/nextstrain_augur.egg-info/entry_points.txt
+-rw-r--r--   0 jlhudd     (501) staff       (20)      614 2020-06-29 20:01:41.000000 nextstrain-augur-9.0.0/nextstrain_augur.egg-info/requires.txt
+-rw-r--r--   0 jlhudd     (501) staff       (20)        6 2020-06-29 20:01:41.000000 nextstrain-augur-9.0.0/nextstrain_augur.egg-info/top_level.txt
+-rw-r--r--   0 jlhudd     (501) staff       (20)        1 2020-06-29 20:01:41.000000 nextstrain-augur-9.0.0/nextstrain_augur.egg-info/dependency_links.txt
+-rw-r--r--   0 jlhudd     (501) staff       (20)    32387 2020-03-24 19:21:38.000000 nextstrain-augur-9.0.0/LICENSE.txt
```

### Comparing `nextstrain-augur-8.0.0/PKG-INFO` & `nextstrain-augur-9.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,85 +1,53 @@
 Metadata-Version: 2.1
 Name: nextstrain-augur
-Version: 8.0.0
+Version: 9.0.0
 Summary: A bioinformatics toolkit for phylogenetic analysis
 Home-page: https://github.com/nextstrain/augur
 Author: Nextstrain developers
 Author-email: trevor@bedford.io, richard.neher@unibas.ch
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/nextstrain/augur/issues
 Project-URL: Change Log, https://github.com/nextstrain/augur/blob/master/CHANGES.md#next
 Project-URL: Source, https://github.com/nextstrain/augur
 Description: [![Build Status](https://travis-ci.com/nextstrain/augur.svg?branch=master)](https://travis-ci.com/nextstrain/augur)
         [![PyPI version](https://badge.fury.io/py/nextstrain-augur.svg)](https://pypi.org/project/nextstrain-augur/)
-        [![Documentation Status](https://readthedocs.org/projects/nextstrain-augur/badge/?version=latest)](https://nextstrain-augur.readthedocs.io/en/stable/?badge=latest)     
+        [![Documentation Status](https://readthedocs.org/projects/nextstrain-augur/badge/?version=latest)](https://nextstrain-augur.readthedocs.io/en/stable/?badge=latest)
         [![License: AGPL v3](https://img.shields.io/badge/License-AGPL%20v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
         
         ## About Nextstrain
         
         Nextstrain is an open-source project to harness the scientific and public health potential of pathogen genome data.
         We provide a continually-updated view of publicly available data with powerful analytics and visualizations showing pathogen evolution and epidemic spread.
         Our goal is to aid epidemiological understanding and improve outbreak response.
         
         Resulting data and inferences are available live at the website [nextstrain.org](https://nextstrain.org).
         
         ## About Augur
+        
         *Definition: One held to foretell events by omens.*
         
         Augur is the bioinformatics toolkit we use to track evolution from sequence and serological data.
         It provides a collection of commands which are designed to be composable into larger processing pipelines.
         
         The output of augur is a series of JSONs that can be used to visualize your results using [Auspice](https://github.com/nextstrain/auspice).
         
-        
         ## Documentation
-        * [Overview of how Augur fits together with other Nextstrain tools](https://nextstrain.org/docs/getting-started/introduction#open-source-tools-for-the-community)  
-        * [Overview of Augur usage](https://nextstrain.org/docs/bioinformatics/introduction-to-augur)  
-        * [Technical documentation for Augur](https://nextstrain-augur.readthedocs.io/en/stable/installation/installation.html)  
-        * [Contributor guide](https://github.com/nextstrain/.github/blob/master/CONTRIBUTING.md)  
-        * [Project board with available issues](https://github.com/orgs/nextstrain/projects/6)   
-        * [Developer docs for Augur](./DEV_DOCS.md)  
-        
-        
-        
-        # Quickstart
-        
-        ## Installation
-        
-        Augur is written in Python 3 and requires at least Python 3.6.
-        
-        To install, run:
-        ```bash
-            pip install nextstrain-augur[full]
-        ```
-        
-        Augur uses some common external bioinformatics programs which you'll need to install to have a fully functioning toolkit:
-        
-        * `augur align` requires [mafft](https://mafft.cbrc.jp/alignment/software/)
-        
-        * `augur tree` requires at least one of:
-           - [IQ-TREE](http://www.iqtree.org/) (used by default)
-           - [RAxML](https://sco.h-its.org/exelixis/web/software/raxml/) (optional alternative)
-           - [FastTree](http://www.microbesonline.org/fasttree/) (optional alternative)
-        
-        * Bacterial data (or any VCF usage) requires [vcftools](https://vcftools.github.io/)
-        
-        On macOS, you can install these external programs using Homebrew with:
-        ```bash
-        brew tap brewsci/bio
-        brew install mafft iqtree raxml fasttree vcftools
-        ```
         
-        On Debian/Ubuntu, you can install them via:
+        * [Overview of how Augur fits together with other Nextstrain tools](https://nextstrain.org/docs/getting-started/introduction#open-source-tools-for-the-community)
+        * [Overview of Augur usage](https://nextstrain.org/docs/bioinformatics/introduction-to-augur)
+        * [Technical documentation for Augur](https://nextstrain-augur.readthedocs.io/en/stable/installation/installation.html)
+        * [Contributor guide](https://github.com/nextstrain/.github/blob/master/CONTRIBUTING.md)
+        * [Project board with available issues](https://github.com/orgs/nextstrain/projects/6)
+        * [Developer docs for Augur](./DEV_DOCS.md)
         
-        ```bash
-        sudo apt install mafft iqtree raxml fasttree vcftools
-        ```
+        ## Quickstart
         
-        [For more extensive installation instructions, please see the technical docs](https://nextstrain-augur.readthedocs.io/en/stable/installation/installation.html)
+        [Follow instructions to install augur](https://nextstrain-augur.readthedocs.io/en/stable/installation/installation.html).
+        Try out an analysis of real virus data by [completing the Zika tutorial](https://nextstrain.org/docs/tutorials/zika).
         
         ## Basic Usage
         
         All of Augur's commands are accessed through the `augur` program.
         For example, to infer ancestral sequences from a tree, you'd run `augur ancestral`.
         If you've installed the `nextstrain-augur` package, you can just run `augur`.
         Otherwise, you can run `./bin/augur` from a copy of the source code.
```

### Comparing `nextstrain-augur-8.0.0/README.md` & `nextstrain-augur-9.0.0/nextstrain_augur.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,117 +1,110 @@
-[![Build Status](https://travis-ci.com/nextstrain/augur.svg?branch=master)](https://travis-ci.com/nextstrain/augur)
-[![PyPI version](https://badge.fury.io/py/nextstrain-augur.svg)](https://pypi.org/project/nextstrain-augur/)
-[![Documentation Status](https://readthedocs.org/projects/nextstrain-augur/badge/?version=latest)](https://nextstrain-augur.readthedocs.io/en/stable/?badge=latest)     
-[![License: AGPL v3](https://img.shields.io/badge/License-AGPL%20v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
-
-## About Nextstrain
-
-Nextstrain is an open-source project to harness the scientific and public health potential of pathogen genome data.
-We provide a continually-updated view of publicly available data with powerful analytics and visualizations showing pathogen evolution and epidemic spread.
-Our goal is to aid epidemiological understanding and improve outbreak response.
-
-Resulting data and inferences are available live at the website [nextstrain.org](https://nextstrain.org).
-
-## About Augur
-*Definition: One held to foretell events by omens.*
-
-Augur is the bioinformatics toolkit we use to track evolution from sequence and serological data.
-It provides a collection of commands which are designed to be composable into larger processing pipelines.
-
-The output of augur is a series of JSONs that can be used to visualize your results using [Auspice](https://github.com/nextstrain/auspice).
-
-
-## Documentation
-* [Overview of how Augur fits together with other Nextstrain tools](https://nextstrain.org/docs/getting-started/introduction#open-source-tools-for-the-community)  
-* [Overview of Augur usage](https://nextstrain.org/docs/bioinformatics/introduction-to-augur)  
-* [Technical documentation for Augur](https://nextstrain-augur.readthedocs.io/en/stable/installation/installation.html)  
-* [Contributor guide](https://github.com/nextstrain/.github/blob/master/CONTRIBUTING.md)  
-* [Project board with available issues](https://github.com/orgs/nextstrain/projects/6)   
-* [Developer docs for Augur](./DEV_DOCS.md)  
-
-
-
-# Quickstart
-
-## Installation
-
-Augur is written in Python 3 and requires at least Python 3.6.
-
-To install, run:
-```bash
-    pip install nextstrain-augur[full]
-```
-
-Augur uses some common external bioinformatics programs which you'll need to install to have a fully functioning toolkit:
-
-* `augur align` requires [mafft](https://mafft.cbrc.jp/alignment/software/)
-
-* `augur tree` requires at least one of:
-   - [IQ-TREE](http://www.iqtree.org/) (used by default)
-   - [RAxML](https://sco.h-its.org/exelixis/web/software/raxml/) (optional alternative)
-   - [FastTree](http://www.microbesonline.org/fasttree/) (optional alternative)
-
-* Bacterial data (or any VCF usage) requires [vcftools](https://vcftools.github.io/)
-
-On macOS, you can install these external programs using Homebrew with:
-```bash
-brew tap brewsci/bio
-brew install mafft iqtree raxml fasttree vcftools
-```
-
-On Debian/Ubuntu, you can install them via:
-
-```bash
-sudo apt install mafft iqtree raxml fasttree vcftools
-```
-
-[For more extensive installation instructions, please see the technical docs](https://nextstrain-augur.readthedocs.io/en/stable/installation/installation.html)
-
-## Basic Usage
-
-All of Augur's commands are accessed through the `augur` program.
-For example, to infer ancestral sequences from a tree, you'd run `augur ancestral`.
-If you've installed the `nextstrain-augur` package, you can just run `augur`.
-Otherwise, you can run `./bin/augur` from a copy of the source code.
-
-```
-usage: augur [-h] {parse,filter,mask,align,tree,refine,ancestral,translate,clades,traits,sequence-traits,titers,export,validate,version} ...
-
-Augur: A bioinformatics toolkit for phylogenetic analysis.
-
-positional arguments:
-  {parse,filter,mask,align,tree,refine,ancestral,translate,clades,traits,sequence-traits,titers,export,validate,version}
-    parse               Parse delimited fields from FASTA sequence names into
-                        a TSV and FASTA file.
-    filter              Filter and subsample a sequence set.
-    mask                Mask specified sites from a VCF file.
-    align               Align multiple sequences from FASTA or VCF.
-    tree                Build a tree using a variety of methods.
-    refine              Refine an initial tree using sequence metadata.
-    ancestral           Infer ancestral sequences based on a tree.
-    translate           Translate gene regions from nucleotides to amino
-                        acids.
-    clades              Assign clades to nodes in a tree based on amino-acid
-                        or nucleotide signatures.
-    traits              Infer ancestral traits based on a tree.
-    sequence-traits     Annotate sequences based on amino-acid or nucleotide
-                        signatures.
-    titers              Annotate a tree with actual and inferred titer
-                        measurements.
-    export              Export JSON files suitable for visualization with
-                        auspice.
-    validate            Validate a set of JSON files intended for
-                        visualization in auspice.
-    version             Print the version of augur.
-
-optional arguments:
-  -h, --help            show this help message and exit
-```
-
-For more information on a specific command, you can run it with the `--help` option, for example, `augur tree --help`.
-
-
-## License and copyright
-
-Copyright 2014-2019 Trevor Bedford and Richard Neher.
-
-Source code to Nextstrain is made available under the terms of the [GNU Affero General Public License](LICENSE.txt) (AGPL). Nextstrain is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU Affero General Public License for more details.
+Metadata-Version: 2.1
+Name: nextstrain-augur
+Version: 9.0.0
+Summary: A bioinformatics toolkit for phylogenetic analysis
+Home-page: https://github.com/nextstrain/augur
+Author: Nextstrain developers
+Author-email: trevor@bedford.io, richard.neher@unibas.ch
+License: UNKNOWN
+Project-URL: Bug Reports, https://github.com/nextstrain/augur/issues
+Project-URL: Change Log, https://github.com/nextstrain/augur/blob/master/CHANGES.md#next
+Project-URL: Source, https://github.com/nextstrain/augur
+Description: [![Build Status](https://travis-ci.com/nextstrain/augur.svg?branch=master)](https://travis-ci.com/nextstrain/augur)
+        [![PyPI version](https://badge.fury.io/py/nextstrain-augur.svg)](https://pypi.org/project/nextstrain-augur/)
+        [![Documentation Status](https://readthedocs.org/projects/nextstrain-augur/badge/?version=latest)](https://nextstrain-augur.readthedocs.io/en/stable/?badge=latest)
+        [![License: AGPL v3](https://img.shields.io/badge/License-AGPL%20v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
+        
+        ## About Nextstrain
+        
+        Nextstrain is an open-source project to harness the scientific and public health potential of pathogen genome data.
+        We provide a continually-updated view of publicly available data with powerful analytics and visualizations showing pathogen evolution and epidemic spread.
+        Our goal is to aid epidemiological understanding and improve outbreak response.
+        
+        Resulting data and inferences are available live at the website [nextstrain.org](https://nextstrain.org).
+        
+        ## About Augur
+        
+        *Definition: One held to foretell events by omens.*
+        
+        Augur is the bioinformatics toolkit we use to track evolution from sequence and serological data.
+        It provides a collection of commands which are designed to be composable into larger processing pipelines.
+        
+        The output of augur is a series of JSONs that can be used to visualize your results using [Auspice](https://github.com/nextstrain/auspice).
+        
+        ## Documentation
+        
+        * [Overview of how Augur fits together with other Nextstrain tools](https://nextstrain.org/docs/getting-started/introduction#open-source-tools-for-the-community)
+        * [Overview of Augur usage](https://nextstrain.org/docs/bioinformatics/introduction-to-augur)
+        * [Technical documentation for Augur](https://nextstrain-augur.readthedocs.io/en/stable/installation/installation.html)
+        * [Contributor guide](https://github.com/nextstrain/.github/blob/master/CONTRIBUTING.md)
+        * [Project board with available issues](https://github.com/orgs/nextstrain/projects/6)
+        * [Developer docs for Augur](./DEV_DOCS.md)
+        
+        ## Quickstart
+        
+        [Follow instructions to install augur](https://nextstrain-augur.readthedocs.io/en/stable/installation/installation.html).
+        Try out an analysis of real virus data by [completing the Zika tutorial](https://nextstrain.org/docs/tutorials/zika).
+        
+        ## Basic Usage
+        
+        All of Augur's commands are accessed through the `augur` program.
+        For example, to infer ancestral sequences from a tree, you'd run `augur ancestral`.
+        If you've installed the `nextstrain-augur` package, you can just run `augur`.
+        Otherwise, you can run `./bin/augur` from a copy of the source code.
+        
+        ```
+        usage: augur [-h] {parse,filter,mask,align,tree,refine,ancestral,translate,clades,traits,sequence-traits,titers,export,validate,version} ...
+        
+        Augur: A bioinformatics toolkit for phylogenetic analysis.
+        
+        positional arguments:
+          {parse,filter,mask,align,tree,refine,ancestral,translate,clades,traits,sequence-traits,titers,export,validate,version}
+            parse               Parse delimited fields from FASTA sequence names into
+                                a TSV and FASTA file.
+            filter              Filter and subsample a sequence set.
+            mask                Mask specified sites from a VCF file.
+            align               Align multiple sequences from FASTA or VCF.
+            tree                Build a tree using a variety of methods.
+            refine              Refine an initial tree using sequence metadata.
+            ancestral           Infer ancestral sequences based on a tree.
+            translate           Translate gene regions from nucleotides to amino
+                                acids.
+            clades              Assign clades to nodes in a tree based on amino-acid
+                                or nucleotide signatures.
+            traits              Infer ancestral traits based on a tree.
+            sequence-traits     Annotate sequences based on amino-acid or nucleotide
+                                signatures.
+            titers              Annotate a tree with actual and inferred titer
+                                measurements.
+            export              Export JSON files suitable for visualization with
+                                auspice.
+            validate            Validate a set of JSON files intended for
+                                visualization in auspice.
+            version             Print the version of augur.
+        
+        optional arguments:
+          -h, --help            show this help message and exit
+        ```
+        
+        For more information on a specific command, you can run it with the `--help` option, for example, `augur tree --help`.
+        
+        
+        ## License and copyright
+        
+        Copyright 2014-2019 Trevor Bedford and Richard Neher.
+        
+        Source code to Nextstrain is made available under the terms of the [GNU Affero General Public License](LICENSE.txt) (AGPL). Nextstrain is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU Affero General Public License for more details.
+        
+Keywords: nextstrain,molecular epidemiology
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: full
+Provides-Extra: dev
```

### Comparing `nextstrain-augur-8.0.0/augur/mask.py` & `nextstrain-augur-9.0.0/augur/mask.py`

 * *Files identical despite different names*

### Comparing `nextstrain-augur-8.0.0/augur/ancestral.py` & `nextstrain-augur-9.0.0/augur/ancestral.py`

 * *Files identical despite different names*

### Comparing `nextstrain-augur-8.0.0/augur/tree.py` & `nextstrain-augur-9.0.0/augur/tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,14 @@
     try:
         run_shell_command(cmd, raise_errors = True)
         shutil.copy("RAxML_bestTree.%s"%(random_string), out_file)
         T = Phylo.read(out_file, 'newick')
         if clean_up:
             os.remove("RAxML_bestTree.%s"%(random_string))
             os.remove("RAxML_info.%s"%(random_string))
-            os.remove("RAxML_log.%s"%(random_string))
             os.remove("RAxML_parsimonyTree.%s"%(random_string))
             os.remove("RAxML_result.%s"%(random_string))
 
     except:
         print("ERROR: TREE BUILDING FAILED")
         if os.path.isfile("RAxML_log.%s"%(random_string)):
             print("Please see the log file for more details: {}".format("RAxML_log.%s"%(random_string)))
@@ -114,16 +113,14 @@
     cmd = " ".join(call)
     print("Building a tree via:\n\t" + cmd +
           "\n\tPrice et al: FastTree 2 - Approximately Maximum-Likelihood Trees for Large Alignments." +
           "\n\tPLoS ONE 5(3): e9490. https://doi.org/10.1371/journal.pone.0009490\n")
     try:
         run_shell_command(cmd, raise_errors = True, extra_env = extra_env)
         T = Phylo.read(out_file, 'newick')
-        if clean_up:
-            os.remove(log_file)
     except:
         print("ERROR: TREE BUILDING FAILED")
         if os.path.isfile(log_file):
             print("Please see the log file for more details: {}".format(log_file))
         T=None
 
     return T
@@ -185,19 +182,18 @@
             n.name = n.name.replace('_X_X_','/').replace('_Y_Y_','|').replace("_X_Y_","(").replace("_Y_X_",")")
         #this allows the user to check intermediate output, as tree.nwk will be
         if clean_up:
             #allow user to see chosen model if modeltest was run
             if substitution_model.lower() == 'none':
                 shutil.copyfile(log_file, out_file.replace(out_file.split('/')[-1],"iqtree.log"))
 
-            for f in [log_file, tmp_aln_file]:
-                if os.path.isfile(f):
-                    os.remove(f)
+            if os.path.isfile(tmp_aln_file):
+                os.remove(tmp_aln_file)
 
-            for ext in [".bionj",".ckp.gz",".iqtree",".log",".mldist",".model.gz",".treefile",".uniqueseq.phy",".model"]:
+            for ext in [".bionj",".ckp.gz",".iqtree",".mldist",".model.gz",".treefile",".uniqueseq.phy",".model"]:
                 if os.path.isfile(tmp_aln_file + ext):
                     os.remove(tmp_aln_file + ext)
     except:
         print("ERROR: TREE BUILDING FAILED")
         if os.path.isfile(log_file):
             print("Please see the log file for more details: {}".format(log_file))
         T=None
@@ -210,15 +206,15 @@
     from Bio.Seq import Seq
 
     sequences = compress_seq['sequences']
     ref = compress_seq['reference']
     positions = compress_seq['positions']
 
     #If want to exclude sites from initial treebuild, read in here
-    strip_pos = load_mask_sites(stripFile)
+    strip_pos = load_mask_sites(stripFile) if stripFile else []
 
     #Get sequence names
     seqNames = list(sequences.keys())
 
     #Check non-ref sites to see if informative
     printPositionMap = False    #If true, prints file mapping Fasta position to real position
     sites = []
```

### Comparing `nextstrain-augur-8.0.0/augur/import_beast.py` & `nextstrain-augur-9.0.0/augur/import_beast.py`

 * *Files identical despite different names*

### Comparing `nextstrain-augur-8.0.0/augur/translate.py` & `nextstrain-augur-9.0.0/augur/translate.py`

 * *Files identical despite different names*

### Comparing `nextstrain-augur-8.0.0/augur/align.py` & `nextstrain-augur-9.0.0/augur/align.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,72 @@
     parser.add_argument('--reference-name', metavar="NAME", type=str, help="strip insertions relative to reference sequence; use if the reference is already in the input sequences")
     parser.add_argument('--reference-sequence', metavar="PATH", type=str, help="Add this reference sequence to the dataset & strip insertions relative to this. Use if the reference is NOT already in the input sequences")
     parser.add_argument('--remove-reference', action="store_true", default=False, help="remove reference sequence from the alignment")
     parser.add_argument('--fill-gaps', action="store_true", default=False, help="If gaps represent missing data rather than true indels, replace by N after aligning.")
     parser.add_argument('--existing-alignment', metavar="FASTA", default=False, help="An existing alignment to which the sequences will be added. The ouput alignment will be the same length as this existing alignment.")
     parser.add_argument('--debug', action="store_true", default=False, help="Produce extra files (e.g. pre- and post-aligner files) which can help with debugging poor alignments.")
 
+def prepare(sequences, existing_aln_fname, output, ref_name, ref_seq_fname):
+    """Prepare the sequences, existing alignment, and reference sequence for alignment.
+
+    This function:
+        1. Combines all given input sequences into a single file
+        2. Checks to make sure the input sequences don't overlap with the existing alignment, if one exists.
+        3. If given a reference name, check that sequence exists in either the existing alignment, if given, or the input sequences.
+        4. If given a reference sequence, either add it to the existing alignment or prepend it to the input seqeunces.
+        5. Write the input sequences to a single file, and write the alignment back out if we added the reference sequence to it.
+
+    Parameters
+    ----------
+    sequences : list[str]
+        List of paths to FASTA-formatted sequences to align.
+    existing_aln_fname : str
+        Path of an existing alignment to use, or None
+    output: str
+        Path the aligned sequences will be written out to.
+    ref_name: str
+        The name of the reference sequence, if provided
+    ref_seq_fname: str
+        The path to the reference sequence file. If this is provided, it overrides ref_name.
+
+    Returns
+    -------
+        tuple: The existing alignment filename, the new sequences filename, and the name of the reference sequence.
+    """
+    seqs = read_sequences(*sequences)
+    seqs_to_align_fname = output + ".to_align.fasta"
+
+    if existing_aln_fname:
+        existing_aln = read_alignment(existing_aln_fname)
+        seqs = prune_seqs_matching_alignment(seqs, existing_aln)
+    else:
+        existing_aln = None
+
+    if ref_seq_fname:
+        ref_seq = read_reference(ref_seq_fname)
+        ref_name = ref_seq.id
+        if existing_aln:
+            if len(ref_seq) != existing_aln.get_alignment_length():
+                raise AlignmentError("ERROR: Provided existing alignment ({}bp) is not the same length as the reference sequence ({}bp)".format(existing_aln.get_alignment_length(), len(ref_seq)))
+            existing_aln_fname = existing_aln_fname + ".ref.fasta"
+            existing_aln.append(ref_seq)
+            write_seqs(existing_aln, existing_aln_fname)
+        else:
+            # reference sequence needs to be the first one for auto direction
+            # adjustment (auto reverse-complement)
+            seqs.insert(0, ref_seq)
+    elif ref_name:
+        ensure_reference_strain_present(ref_name, existing_aln, seqs)
+
+    write_seqs(seqs, seqs_to_align_fname)
+
+    # 90% sure this is only ever going to catch ref_seq was a dupe
+    check_duplicates(existing_aln, seqs)
+    return existing_aln_fname, seqs_to_align_fname, ref_name
+
 def run(args):
     '''
     Parameters
     ----------
     args : namespace
         arguments passed in via the command-line from augur
 
@@ -40,112 +98,102 @@
     int
         returns 0 for success, 1 for general error
     '''
     temp_files_to_remove = []
 
     try:
         check_arguments(args)
-        seqs = read_sequences(*args.sequences)
-        existing_aln = read_alignment(args.existing_alignment) if args.existing_alignment else None
-
-        # if we have been given a reference (strain) name, make sure it is present
-        ref_name = args.reference_name
-        if args.reference_name:
-            ensure_reference_strain_present(ref_name, existing_aln, seqs)
-
-        # If given an existing alignment, then add the reference sequence to this if desired (and if it is the same length)
-        if existing_aln and args.reference_sequence:
-            existing_aln_fname = args.existing_alignment + ".ref.fasta"
-            ref_seq = read_reference(args.reference_sequence)
-            if len(ref_seq) != existing_aln.get_alignment_length():
-                raise AlignmentError("ERROR: Provided existing alignment ({}bp) is not the same length as the reference sequence ({}bp)".format(existing_aln.get_alignment_length(), len(ref_seq)))
-            existing_aln.append(ref_seq)
-            write_seqs(existing_aln, existing_aln_fname)
-            temp_files_to_remove.append(existing_aln_fname)
-            ref_name = ref_seq.id
-        else:
-            existing_aln_fname = args.existing_alignment # may be False
-
-        ## Create a single file of sequences for alignment (or to be added to the alignment).
-        ## Add in the reference file to the sequences _if_ we don't have an existing alignment
-        if args.reference_sequence and not existing_aln:
-            seqs_to_align_fname = args.output+".to_align.fasta"
-            ref_seq = read_reference(args.reference_sequence)
-            # reference sequence needs to be the first one for auto direction adjustment (auto reverse-complement)
-            write_seqs([ref_seq] + list(seqs.values()), seqs_to_align_fname)
-            ref_name = ref_seq.id
-        elif existing_aln:
-            seqs_to_align_fname = args.output+".new_seqs_to_align.fasta"
-            seqs = prune_seqs_matching_alignment(seqs, existing_aln)
-            write_seqs(list(seqs.values()), seqs_to_align_fname)
-        else:
-            seqs_to_align_fname = args.output+".to_align.fasta"
-            write_seqs(list(seqs.values()), seqs_to_align_fname)
+        existing_aln_fname, seqs_to_align_fname, ref_name = prepare(args.sequences, args.existing_alignment, args.output, args.reference_name, args.reference_sequence)
         temp_files_to_remove.append(seqs_to_align_fname)
-
-        check_duplicates(existing_aln, ref_name, seqs)
+        if existing_aln_fname != args.existing_alignment:
+            temp_files_to_remove.append(existing_aln_fname)
+        # -- existing_aln_fname, seqs_to_align_fname, ref_name --
 
         # before aligning, make a copy of the data that the aligner receives as input (very useful for debugging purposes)
-        if args.debug and not existing_aln:
+        if args.debug and not existing_aln_fname:
             copyfile(seqs_to_align_fname, args.output+".pre_aligner.fasta")
 
         # generate alignment command & run
         cmd = generate_alignment_cmd(args.method, args.nthreads, existing_aln_fname, seqs_to_align_fname, args.output, args.output+".log")
         success = run_shell_command(cmd)
         if not success:
             raise AlignmentError("Error during alignment")
 
         # after aligning, make a copy of the data that the aligner produced (useful for debugging)
         if args.debug:
             copyfile(args.output, args.output+".post_aligner.fasta")
 
-        # reads the new alignment
-        seqs = read_alignment(args.output)
-
-        # convert the aligner output to upper case and remove auto reverse-complement prefix
-        prettify_alignment(seqs)
-
-        # if we've specified a reference, strip out all the columns not present in the reference
-        # this will overwrite the alignment file
-        if ref_name:
-            seqs = strip_non_reference(seqs, ref_name, insertion_csv=args.output+".insertions.csv")
-            if args.remove_reference:
-                seqs = remove_reference_sequence(seqs, ref_name)
-            write_seqs(seqs, args.output)
-        if args.fill_gaps:
-            make_gaps_ambiguous(seqs)
-
-        # write the modified sequences back to the alignment file
-        write_seqs(seqs, args.output)
+        postprocess(args.output, ref_name, not args.remove_reference, args.fill_gaps)
 
 
     except AlignmentError as e:
         print(str(e))
         return 1
 
     # finally, remove any temporary files
     for fname in temp_files_to_remove:
         os.remove(fname)
 
+
+def postprocess(output_file, ref_name, keep_reference, fill_gaps):
+    """Postprocessing of the combined alignment file.
+
+    Parameters
+    ----------
+    output_file: str
+        The file the new alignment was written to
+    ref_name: str
+        If provided, the name of the reference strain used in the alignment
+    keep_reference: bool
+        If the reference was provided, whether it should be kept in the alignment
+    fill_gaps: bool
+        Replace all gaps in the alignment with "N" to indicate ambiguous sites.
+
+    Returns
+    -------
+        None - the modified alignment is written directly to output_file
+    """
+    # -- ref_name --
+    # reads the new alignment
+    seqs = read_alignment(output_file)
+    # convert the aligner output to upper case and remove auto reverse-complement prefix
+    prettify_alignment(seqs)
+
+    # if we've specified a reference, strip out all the columns not present in the reference
+    # this will overwrite the alignment file
+    if ref_name:
+        seqs = strip_non_reference(seqs, ref_name, insertion_csv=output_file+".insertions.csv")
+        if not keep_reference:
+            seqs = remove_reference_sequence(seqs, ref_name)
+
+    if fill_gaps:
+        make_gaps_ambiguous(seqs)
+
+    # write the modified sequences back to the alignment file
+    write_seqs(seqs, output_file)
+
+
+
 #####################################################################################################
 
 def read_sequences(*fnames):
+    """return list of sequences from all fnames"""
     seqs = {}
     try:
         for fname in fnames:
             for record in SeqIO.parse(fname, 'fasta'):
                 if record.name in seqs and record.seq != seqs[record.name].seq:
                     raise AlignmentError("Detected duplicate input strains \"%s\" but the sequences are different." % record.name)
                     # if the same sequence then we can proceed (and we only take one)
                 seqs[record.name] = record
     except FileNotFoundError:
         raise AlignmentError("\nCannot read sequences -- make sure the file %s exists and contains sequences in fasta format" % fname)
     except ValueError as error:
         raise AlignmentError("\nERROR: Problem reading in {}: {}".format(fname, str(error)))
-    return seqs
+    return list(seqs.values())
 
 def check_arguments(args):
     # Simple error checking related to a reference name/sequence
     if args.reference_name and args.reference_sequence:
         raise AlignmentError("ERROR: You cannot provide both --reference-name and --reference-sequence")
     if args.remove_reference and not (args.reference_name or args.reference_sequence):
         raise AlignmentError("ERROR: You've asked to remove the reference but haven't specified one!")
@@ -157,15 +205,15 @@
         raise AlignmentError("\nERROR: Problem reading in {}: {}".format(fname, str(error)))
 
 def ensure_reference_strain_present(ref_name, existing_alignment, seqs):
     if existing_alignment:
         if ref_name not in {x.name for x in existing_alignment}:
             raise AlignmentError("ERROR: Specified reference name %s (via --reference-name) is not in the supplied alignment."%ref_name)
     else:
-        if ref_name not in seqs:
+        if ref_name not in {x.name for x in seqs}:
             raise AlignmentError("ERROR: Specified reference name %s (via --reference-name) is not in the sequence sample."%ref_name)
 
 
     # align
     # if args.method=='mafft':
     #     shoutput = shquote(output)
     #     shname = shquote(seq_fname)
@@ -341,45 +389,41 @@
 
 def check_duplicates(*values):
     names = set()
     def add(name):
         if name in names:
             raise AlignmentError("Duplicate strains of \"{}\" detected".format(name))
         names.add(name)
-
     for sample in values:
         if not sample:
             # allows false-like values (e.g. always provide existing_alignment, allowing
             # the default which is `False`)
             continue
-        elif type(sample) == dict:
-            for s in sample:
-                add(s)
-        elif type(sample) == Align.MultipleSeqAlignment:
+        elif isinstance(sample, (list, Align.MultipleSeqAlignment)):
             for s in sample:
                 add(s.name)
-        elif type(sample) == str:
+        elif isinstance(sample, str):
             add(sample)
         else:
             raise TypeError()
 
 def write_seqs(seqs, fname):
     """A wrapper around SeqIO.write with error handling"""
     try:
         SeqIO.write(seqs, fname, 'fasta')
     except FileNotFoundError:
         raise AlignmentError('ERROR: Couldn\'t write "{}" -- perhaps the directory doesn\'t exist?'.format(fname))
 
 
 def prune_seqs_matching_alignment(seqs, aln):
     """
-    Return a set of seqs excluding those set via `exclude` & print a warning
+    Return a set of seqs excluding those already in the alignment & print a warning
     message for each sequence which is exluded.
     """
-    ret = {}
-    exclude_names = {s.name for s in aln}
-    for name, seq in seqs.items():
-        if name in exclude_names:
-            print("Excluding {} as it is already present in the alignment".format(name))
+    ret = []
+    aln_names = {s.name for s in aln}
+    for seq in seqs:
+        if seq.name in aln_names:
+            print("Excluding {} as it is already present in the alignment".format(seq.name))
         else:
-            ret[name] = seq
+            ret.append(seq)
     return ret
```

### Comparing `nextstrain-augur-8.0.0/augur/reconstruct_sequences.py` & `nextstrain-augur-9.0.0/augur/reconstruct_sequences.py`

 * *Files identical despite different names*

### Comparing `nextstrain-augur-8.0.0/augur/export_v1.py` & `nextstrain-augur-9.0.0/augur/export_v1.py`

 * *Files identical despite different names*

### Comparing `nextstrain-augur-8.0.0/augur/refine.py` & `nextstrain-augur-9.0.0/augur/refine.py`

 * *Files identical despite different names*

### Comparing `nextstrain-augur-8.0.0/augur/__init__.py` & `nextstrain-augur-9.0.0/augur/__init__.py`

 * *Files identical despite different names*

### Comparing `nextstrain-augur-8.0.0/augur/export.py` & `nextstrain-augur-9.0.0/augur/export.py`

 * *Files identical despite different names*

### Comparing `nextstrain-augur-8.0.0/augur/distance.py` & `nextstrain-augur-9.0.0/augur/distance.py`

 * *Files identical despite different names*

### Comparing `nextstrain-augur-8.0.0/augur/clades.py` & `nextstrain-augur-9.0.0/augur/clades.py`

 * *Files identical despite different names*

### Comparing `nextstrain-augur-8.0.0/augur/validate.py` & `nextstrain-augur-9.0.0/augur/validate.py`

 * *Files identical despite different names*

### Comparing `nextstrain-augur-8.0.0/augur/lbi.py` & `nextstrain-augur-9.0.0/augur/lbi.py`

 * *Files identical despite different names*

### Comparing `nextstrain-augur-8.0.0/augur/validate_export.py` & `nextstrain-augur-9.0.0/augur/validate_export.py`

 * *Files identical despite different names*

### Comparing `nextstrain-augur-8.0.0/augur/utils.py` & `nextstrain-augur-9.0.0/augur/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,22 +7,26 @@
 import subprocess
 import shlex
 from contextlib import contextmanager
 from treetime.utils import numeric_date
 from collections import defaultdict
 from pkg_resources import resource_stream
 from io import TextIOWrapper
-from textwrap import dedent
 from .__version__ import __version__
 import packaging.version as packaging_version
 from .validate import validate, ValidateError, load_json_schema
 
+from augur.util_support.date_disambiguator import DateDisambiguator
+from augur.util_support.shell_command_runner import ShellCommandRunner
+
+
 class AugurException(Exception):
     pass
 
+
 @contextmanager
 def open_file(fname, mode):
     """Open a file using either gzip.open() or open() depending on file name. Semantics identical to open()"""
     if fname.endswith('.gz'):
         if "t" not in mode:
             # For interoperability, gzip needs to open files in "text" mode
             mode = mode + "t"
@@ -58,46 +62,16 @@
         if default:
             print("WARNING: no name for the output file was specified. Writing results to %s."%default, file=sys.stderr)
             return default
         else:
             raise ValueError("Please specify a name for the JSON file containing the results.")
 
 
-def ambiguous_date_to_date_range(mydate, fmt, min_max_year=None):
-    from datetime import datetime
-    sep = fmt.split('%')[1][-1]
-    min_date, max_date = {}, {}
-    today = datetime.today().date()
-
-    for val, field  in zip(mydate.split(sep), fmt.split(sep+'%')):
-        f = 'year' if 'y' in field.lower() else ('day' if 'd' in field.lower() else 'month')
-        if 'XX' in val:
-            if f=='year':
-                if min_max_year:
-                    min_date[f]=min_max_year[0]
-                    if len(min_max_year)>1:
-                        max_date[f]=min_max_year[1]
-                    elif len(min_max_year)==1:
-                        max_date[f]=4000 #will be replaced by 'today' below.
-                else:
-                    return None, None
-            elif f=='month':
-                min_date[f]=1
-                max_date[f]=12
-            elif f=='day':
-                min_date[f]=1
-                max_date[f]=31
-        else:
-            min_date[f]=int(val)
-            max_date[f]=int(val)
-    max_date['day'] = min(max_date['day'], 31 if max_date['month'] in [1,3,5,7,8,10,12]
-                                           else 28 if max_date['month']==2 else 30)
-    lower_bound = datetime(year=min_date['year'], month=min_date['month'], day=min_date['day']).date()
-    upper_bound = datetime(year=max_date['year'], month=max_date['month'], day=max_date['day']).date()
-    return (lower_bound, upper_bound if upper_bound<today else today)
+def ambiguous_date_to_date_range(uncertain_date, fmt, min_max_year=None):
+    return DateDisambiguator(uncertain_date, fmt=fmt, min_max_year=min_max_year).range()
 
 def read_metadata(fname, query=None):
     if not fname:
         print("ERROR: read_metadata called without a filename")
         return {}, []
     if os.path.isfile(fname):
         try:
@@ -119,14 +93,15 @@
         meta_dict = {}
         for ii, val in metadata.iterrows():
             if hasattr(val, "strain"):
                 if val.strain in meta_dict:
                     raise ValueError("Duplicate strain '{}'".format(val.strain))
                 meta_dict[val.strain] = val.to_dict()
             elif hasattr(val, "name"):
+                val = val.rename(val["name"])
                 if val.name in meta_dict:
                     raise ValueError("Duplicate name '{}'".format(val.name))
                 meta_dict[val.name] = val.to_dict()
             else:
                 print("ERROR: meta data file needs 'name' or 'strain' column")
 
         return meta_dict, list(metadata.columns)
@@ -563,85 +538,26 @@
         #must temporarily remove .gz ending, or gzip won't zip it!
         os.rename(vcf_file_name, vcf_file_name[:-3])
         call = ["gzip", vcf_file_name[:-3]]
         run_shell_command(" ".join(call), raise_errors = True)
 
 shquote = shlex.quote
 
-def run_shell_command(cmd, raise_errors = False, extra_env = None):
+def run_shell_command(cmd, raise_errors=False, extra_env=None):
     """
     Run the given command string via Bash with error checking.
 
     Returns True if the command exits normally.  Returns False if the command
     exits with failure and "raise_errors" is False (the default).  When
     "raise_errors" is True, exceptions are rethrown.
 
     If an *extra_env* mapping is passed, the provided keys and values are
     overlayed onto the default subprocess environment.
     """
-    env = os.environ.copy()
-
-    if extra_env:
-        env.update(extra_env)
-
-    shargs = ['-c', "set -euo pipefail; " + cmd]
-
-    if os.name == 'posix':
-        shellexec = ['/bin/bash']
-    else:
-        # We try best effort on other systems. For now that means nt/java.
-        shellexec = ['env', 'bash']
-
-    try:
-        # Use check_call() instead of run() since the latter was added only in Python 3.5.
-        subprocess.check_output(
-            shellexec + shargs,
-            shell = False,
-            stderr = subprocess.STDOUT,
-            env = env)
-
-    except subprocess.CalledProcessError as error:
-        print_error(
-            "{out}\nshell exited {rc} when running: {cmd}{extra}",
-            out = error.output,
-            rc  = error.returncode,
-            cmd = cmd,
-            extra = "\nAre you sure this program is installed?" if error.returncode==127 else "",
-        )
-        if raise_errors:
-            raise
-        else:
-            return False
-
-    except FileNotFoundError as error:
-        print_error(
-            """
-            Unable to run shell commands using {shell}!
-
-            Augur requires {shell} to be installed.  Please open an issue on GitHub
-            <https://github.com/nextstrain/augur/issues/new> if you need assistance.
-            """,
-            shell = ' and '.join(shellexec)
-        )
-        if raise_errors:
-            raise
-        else:
-            return False
-
-    else:
-        return True
-
-
-def print_error(message, **kwargs):
-    """
-    Formats *message* with *kwargs* using :meth:`str.format` and
-    :func:`textwrap.dedent` and uses it to print an error message to
-    ``sys.stderr``.
-    """
-    print("\nERROR: " + dedent(message.format(**kwargs)).lstrip("\n")+"\n", file = sys.stderr)
+    return ShellCommandRunner(cmd, raise_errors=raise_errors, extra_env=extra_env).run()
 
 
 def first_line(text):
     """
     Returns the first line of the given text, ignoring leading and trailing
     whitespace.
     """
```

### Comparing `nextstrain-augur-8.0.0/augur/titer_model.py` & `nextstrain-augur-9.0.0/augur/titer_model.py`

 * *Files identical despite different names*

### Comparing `nextstrain-augur-8.0.0/augur/export_v2.py` & `nextstrain-augur-9.0.0/augur/export_v2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Export JSON files suitable for visualization with auspice.
 """
 from pathlib import Path
 import os, sys
 import time
-from collections import defaultdict
+from collections import defaultdict, deque
 import warnings
 import re
 from Bio import Phylo
 from .utils import read_metadata, read_node_data, write_json, read_config, read_lat_longs, read_colors
 from .validate import export_v2 as validate_v2, auspice_config_v2 as validate_auspice_config_v2, ValidateError
 
 # Set up warnings & exceptions
@@ -429,14 +429,55 @@
     if "map" in panels:
         if "geo_resolutions" not in data_json["meta"] or not data_json["meta"]["geo_resolutions"]:
             panels.remove("map")
 
     data_json['meta']["panels"] = panels
 
 
+def counter_to_disambiguation_suffix(count):
+    """Given a numeric count of author papers, return a distinct alphabetical
+    disambiguation suffix.
+
+    >>> counter_to_disambiguation_suffix(0)
+    'A'
+    >>> counter_to_disambiguation_suffix(25)
+    'Z'
+    >>> counter_to_disambiguation_suffix(26)
+    'AA'
+    >>> counter_to_disambiguation_suffix(51)
+    'AZ'
+    >>> counter_to_disambiguation_suffix(52)
+    'BA'
+    """
+    letters = "ABCDEFGHIJKLMNOPQRSTUVWXYZ"
+    base = len(letters)
+    suffix = deque()
+
+    # Find the appropriate combination of letters for the given count. This
+    # closely resembles the steps required to calculate the base 26 value of the
+    # given base 10 number.
+    while True:
+        quotient = count // base
+        remainder = count % base
+
+        # Collect remainders from right to left. Letters are zero-indexed such
+        # that a count of 0 returns an "A".
+        suffix.appendleft(letters[remainder])
+
+        # Stop when we've accounted for all possible quotient and remainder
+        # values.
+        if quotient == 0:
+            break
+
+        # Convert counts to zero-indexed values such that the next place value
+        # starts with the letter "A" instead of the letter "B".
+        count = quotient - 1
+
+    return "".join(suffix)
+
 def create_author_data(node_attrs):
     """Gather the authors which appear in the metadata and create the author
     info structure with unique keys
     """
 
     def node_to_author_tuple(data):
         # make a unique list of citations to disambiguate
@@ -484,15 +525,16 @@
         if node_name not in node_author_info:
             continue # internal node / terminal node without authors
 
         author_tuple = node_to_author_tuple(node_author_info[node_name])
         author = node_author_info[node_name]["author"]
         if len(author_to_unique_tuples[author]) > 1:
             index = author_to_unique_tuples[author].index(author_tuple)
-            node_author_info[node_name]["value"] = author + " {}".format("ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz"[index])
+            disambiguation_suffix = counter_to_disambiguation_suffix(index)
+            node_author_info[node_name]["value"] = f"{author} {disambiguation_suffix}"
         else:
             node_author_info[node_name]["value"] = author
 
     return node_author_info
 
 
 def set_node_attrs_on_tree(data_json, node_attrs):
```

### Comparing `nextstrain-augur-8.0.0/augur/filter.py` & `nextstrain-augur-9.0.0/augur/filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 from Bio import SeqIO
 import pandas as pd
 from collections import defaultdict
 import random, os, re
 import numpy as np
 import sys
+import datetime
+import treetime.utils
 from .utils import read_metadata, get_numerical_dates, run_shell_command, shquote
 
 comment_char = '#'
 
 
 def read_vcf(filename):
     if filename.lower().endswith(".gz"):
@@ -83,16 +85,16 @@
     """
     filtered_meta_dict, _ = read_metadata(metadata_file, query)
     return [seq for seq in sequences if seq in filtered_meta_dict]
 
 def register_arguments(parser):
     parser.add_argument('--sequences', '-s', required=True, help="sequences in fasta or VCF format")
     parser.add_argument('--metadata', required=True, help="metadata associated with sequences")
-    parser.add_argument('--min-date', type=float, help="minimal cutoff for numerical date")
-    parser.add_argument('--max-date', type=float, help="maximal cutoff for numerical date")
+    parser.add_argument('--min-date', type=numeric_date, help="minimal cutoff for date; may be specified as an Augur-style numeric date (with the year as the integer part) or YYYY-MM-DD")
+    parser.add_argument('--max-date', type=numeric_date, help="maximal cutoff for date; may be specified as an Augur-style numeric date (with the year as the integer part) or YYYY-MM-DD")
     parser.add_argument('--min-length', type=int, help="minimal length of the sequences")
     parser.add_argument('--non-nucleotide', action='store_true', help="exclude sequences that contain illegal characters")
     parser.add_argument('--exclude', type=str, help="file with list of strains that are to be excluded")
     parser.add_argument('--include', type=str, help="file with list of strains that are to be included regardless of priorities or subsampling")
     parser.add_argument('--priority', type=str, help="file with list of priority scores for sequences (strain\tpriority)")
     parser.add_argument('--sequences-per-group', type=int, help="subsample to no more than this number of sequences per category")
     parser.add_argument('--group-by', nargs='+', help="categories with respect to subsample; two virtual fields, \"month\" and \"year\", are supported if they don't already exist as real fields but a \"date\" field does exist")
@@ -406,7 +408,25 @@
         print("\t%i sequences were added back because of '%s'" % (num_included_by_metadata, args.include_where))
 
     print("%i sequences have been written out to %s" % (len(seq_keep), args.output))
 
 
 def _filename_gz(filename):
     return filename.lower().endswith(".gz")
+
+
+def numeric_date(date):
+    """
+    Converts the given *date* string to a :py:class:`float`.
+
+    *date* may be given as a number (a float) with year as the integer part, or
+    in the YYYY-MM-DD (ISO 8601) syntax.
+
+    >>> numeric_date("2020.42")
+    2020.42
+    >>> numeric_date("2020-06-04")
+    2020.42486...
+    """
+    try:
+        return float(date)
+    except ValueError:
+        return treetime.utils.numeric_date(datetime.date(*map(int, date.split("-", 2))))
```

### Comparing `nextstrain-augur-8.0.0/augur/traits.py` & `nextstrain-augur-9.0.0/augur/traits.py`

 * *Files identical despite different names*

### Comparing `nextstrain-augur-8.0.0/augur/frequency_estimators.py` & `nextstrain-augur-9.0.0/augur/frequency_estimators.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,15 @@
         self.pc = pc
         self.ws = ws
         self.verbose = 0
         self.method = method
 
         self.pivots = make_pivots(pivots, self.tps)
 
-        good_tps = (self.tps>self.pivots[0])&(self.tps<self.pivots[-1])
+        good_tps = (self.tps>=self.pivots[0])&(self.tps<self.pivots[-1])
         self.tps = self.tps[good_tps]
         self.obs = self.obs[good_tps]
 
 
     def initial_guess(self, pc=0.01):
         # generate a useful initial guess from a running average of the counts
         if self.ws<len(self.obs):
```

### Comparing `nextstrain-augur-8.0.0/augur/titers.py` & `nextstrain-augur-9.0.0/augur/titers.py`

 * *Files identical despite different names*

### Comparing `nextstrain-augur-8.0.0/augur/parse.py` & `nextstrain-augur-9.0.0/augur/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,18 +48,18 @@
 
     if camelCase:
         words = map(str.capitalize, words)
 
     res = ' '.join(words)
 
     if removeComma:
-        res.replace(',', '')
+        res = res.replace(',', '')
 
     if etal == 'lower':
-        res = res.replace('Et Al', 'et al').replace('Et Al.', 'et al.')
+        res = res.replace('Et Al', 'et al').replace('Et Al.', 'et al.').replace('Et al', 'et al')
     elif etal == 'strip':
         res = res.replace('et al.', '').replace('Et Al.', '').replace('et al', '').replace('Et Al', '')
 
     return res
 
 
 def register_arguments(parser):
```

### Comparing `nextstrain-augur-8.0.0/augur/sequence_traits.py` & `nextstrain-augur-9.0.0/augur/sequence_traits.py`

 * *Files identical despite different names*

### Comparing `nextstrain-augur-8.0.0/augur/data/lat_longs.tsv` & `nextstrain-augur-9.0.0/augur/data/lat_longs.tsv`

 * *Files identical despite different names*

### Comparing `nextstrain-augur-8.0.0/augur/data/schema-annotations.json` & `nextstrain-augur-9.0.0/augur/data/schema-annotations.json`

 * *Files identical despite different names*

### Comparing `nextstrain-augur-8.0.0/augur/data/schema-auspice-config-v2.json` & `nextstrain-augur-9.0.0/augur/data/schema-auspice-config-v2.json`

 * *Files identical despite different names*

### Comparing `nextstrain-augur-8.0.0/augur/data/schema-export-v2.json` & `nextstrain-augur-9.0.0/augur/data/schema-export-v2.json`

 * *Files identical despite different names*

### Comparing `nextstrain-augur-8.0.0/augur/data/schema-export-v1-meta.json` & `nextstrain-augur-9.0.0/augur/data/schema-export-v1-meta.json`

 * *Files identical despite different names*

### Comparing `nextstrain-augur-8.0.0/augur/data/schema-export-v1-tree.json` & `nextstrain-augur-9.0.0/augur/data/schema-export-v1-tree.json`

 * *Files identical despite different names*

### Comparing `nextstrain-augur-8.0.0/augur/frequencies.py` & `nextstrain-augur-9.0.0/augur/frequencies.py`

 * *Files identical despite different names*

### Comparing `nextstrain-augur-8.0.0/setup.py` & `nextstrain-augur-9.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib    import Path
-from setuptools import setup
+import setuptools
 import sys
 
 min_version = (3, 6)
 
 if sys.version_info < min_version:
     error = """
 Beginning with augur 7.0.0, Python {0} or above is required.
@@ -22,30 +22,32 @@
 with version_file.open() as f:
     exec(f.read())
 
 # Get the long description from the README file
 with readme_file.open(encoding = "utf-8") as f:
     long_description = f.read()
 
-setup(
+
+
+setuptools.setup(
     name = "nextstrain-augur",
     version = __version__,
     author = "Nextstrain developers",
     author_email = "trevor@bedford.io, richard.neher@unibas.ch",
     description = "A bioinformatics toolkit for phylogenetic analysis",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     keywords = "nextstrain, molecular epidemiology",
     url = "https://github.com/nextstrain/augur",
     project_urls = {
         "Bug Reports": "https://github.com/nextstrain/augur/issues",
         "Change Log": "https://github.com/nextstrain/augur/blob/master/CHANGES.md#next",
         "Source": "https://github.com/nextstrain/augur",
     },
-    packages = ['augur'],
+    packages = setuptools.find_packages(),
     package_data = {'augur': ['data/*']},
     data_files = [("", ["LICENSE.txt"])],
     python_requires = '>={}'.format('.'.join(str(n) for n in min_version)),
     install_requires = [
         "bcbio-gff >=0.6.0, ==0.6.*",
         "biopython >=1.67, ==1.*",
         "jsonschema >=3.0.0, ==3.*",
@@ -60,14 +62,15 @@
             "matplotlib >=2.0, ==2.*",
             "seaborn >=0.9.0, ==0.9.*"
         ],
         'dev': [
             "cram >=0.7, ==0.*",
             "deepdiff >=4.3.2, ==4.3.*",
             "freezegun >=0.3.15, ==0.3.*",
+            "nextstrain-sphinx-theme >=2020.3",
             "pylint >=1.7.6, ==1.7.*",
             "pytest >=5.4.1, ==5.4.*",
             "pytest-cov >=2.8.1, ==2.8.*",
             "pytest-mock >= 2.0.0, ==2.0.*",
             "recommonmark >=0.5.0, ==0.*",
             "Sphinx >=2.0.1, ==2.*",
             "sphinx-argparse >=0.2.5, ==0.*",
```

### Comparing `nextstrain-augur-8.0.0/nextstrain_augur.egg-info/SOURCES.txt` & `nextstrain-augur-9.0.0/nextstrain_augur.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -35,13 +35,16 @@
 augur/data/colors.tsv
 augur/data/lat_longs.tsv
 augur/data/schema-annotations.json
 augur/data/schema-auspice-config-v2.json
 augur/data/schema-export-v1-meta.json
 augur/data/schema-export-v1-tree.json
 augur/data/schema-export-v2.json
+augur/util_support/__init__.py
+augur/util_support/date_disambiguator.py
+augur/util_support/shell_command_runner.py
 nextstrain_augur.egg-info/PKG-INFO
 nextstrain_augur.egg-info/SOURCES.txt
 nextstrain_augur.egg-info/dependency_links.txt
 nextstrain_augur.egg-info/entry_points.txt
 nextstrain_augur.egg-info/requires.txt
 nextstrain_augur.egg-info/top_level.txt
```

### Comparing `nextstrain-augur-8.0.0/nextstrain_augur.egg-info/requires.txt` & `nextstrain-augur-9.0.0/nextstrain_augur.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 phylo-treetime==0.7.*,>=0.7.4
 snakemake<5.11,>=5.4.0
 
 [dev]
 cram==0.*,>=0.7
 deepdiff==4.3.*,>=4.3.2
 freezegun==0.3.*,>=0.3.15
+nextstrain-sphinx-theme>=2020.3
 pylint==1.7.*,>=1.7.6
 pytest==5.4.*,>=5.4.1
 pytest-cov==2.8.*,>=2.8.1
 pytest-mock==2.0.*,>=2.0.0
 recommonmark==0.*,>=0.5.0
 Sphinx==2.*,>=2.0.1
 sphinx-argparse==0.*,>=0.2.5
```

### Comparing `nextstrain-augur-8.0.0/LICENSE.txt` & `nextstrain-augur-9.0.0/LICENSE.txt`

 * *Files identical despite different names*

