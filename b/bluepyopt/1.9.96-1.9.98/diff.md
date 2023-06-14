# Comparing `tmp/bluepyopt-1.9.96.tar.gz` & `tmp/bluepyopt-1.9.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bluepyopt-1.9.96.tar", last modified: Thu Dec 10 17:43:24 2020, max compression
+gzip compressed data, was "dist/bluepyopt-1.9.98.tar", last modified: Fri Dec 11 13:48:46 2020, max compression
```

## Comparing `bluepyopt-1.9.96.tar` & `bluepyopt-1.9.98.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-10 17:43:24.000000 bluepyopt-1.9.96/
--rw-rw-r--   0 travis    (2000) travis    (2000)      201 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    69513 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/versioneer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1042 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/LICENSE.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      179 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/AUTHORS.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1189 2020-12-10 17:43:24.000000 bluepyopt-1.9.96/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     7970 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-10 17:43:24.000000 bluepyopt-1.9.96/bluepyopt.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1189 2020-12-10 17:43:24.000000 bluepyopt-1.9.96/bluepyopt.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-12-10 17:43:24.000000 bluepyopt-1.9.96/bluepyopt.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       10 2020-12-10 17:43:24.000000 bluepyopt-1.9.96/bluepyopt.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     3415 2020-12-10 17:43:24.000000 bluepyopt-1.9.96/bluepyopt.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      116 2020-12-10 17:43:24.000000 bluepyopt-1.9.96/bluepyopt.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       69 2020-12-10 17:43:24.000000 bluepyopt-1.9.96/bluepyopt.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     7651 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/LGPL.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      202 2020-12-10 17:43:24.000000 bluepyopt-1.9.96/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-10 17:43:24.000000 bluepyopt-1.9.96/bluepyopt/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-10 17:43:24.000000 bluepyopt-1.9.96/bluepyopt/ipyp/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/ipyp/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4571 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/ipyp/bpopt_tasksdb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      498 2020-12-10 17:43:24.000000 bluepyopt-1.9.96/bluepyopt/_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      218 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tools.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-10 17:43:24.000000 bluepyopt-1.9.96/bluepyopt/ephys/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6856 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/ephys/create_hoc.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-10 17:43:24.000000 bluepyopt-1.9.96/bluepyopt/ephys/examples/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-10 17:43:24.000000 bluepyopt-1.9.96/bluepyopt/ephys/examples/simplecell/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2560 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/ephys/examples/simplecell/simplecell.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      100 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/ephys/examples/simplecell/simple.swc
--rw-rw-r--   0 travis    (2000) travis    (2000)       46 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/ephys/examples/simplecell/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       45 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/ephys/examples/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9967 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/ephys/protocols.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1525 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/ephys/objectivescalculators.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-10 17:43:24.000000 bluepyopt-1.9.96/bluepyopt/ephys/templates/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4985 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/ephys/templates/cell_template.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)    10039 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/ephys/mechanisms.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6073 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/ephys/parameterscalers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9462 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/ephys/locations.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15998 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/ephys/models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2513 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/ephys/serializer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3261 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/ephys/objectives.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7516 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/ephys/morphologies.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7882 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/ephys/evaluators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12265 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/ephys/parameters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      341 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/ephys/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1515 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/ephys/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3018 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/ephys/recordings.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10321 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/ephys/stimuli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7658 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/ephys/efeatures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2300 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/ephys/responses.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4821 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/ephys/simulators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      999 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/optimisations.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1008 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/objectives.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2341 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/evaluators.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-10 17:43:24.000000 bluepyopt-1.9.96/bluepyopt/deapext/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6446 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/deapext/algorithms.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10523 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/deapext/optimisations.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-10 17:43:24.000000 bluepyopt-1.9.96/bluepyopt/deapext/tools/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4774 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/deapext/tools/selIBEA.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       43 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/deapext/tools/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       18 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/deapext/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1404 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/deapext/stoppingCriteria.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4722 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/parameters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      963 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/api.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1677 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-10 17:43:24.000000 bluepyopt-1.9.96/bluepyopt/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)      904 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_tools.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-10 17:43:24.000000 bluepyopt-1.9.96/bluepyopt/tests/test_ephys/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2076 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_ephys/test_parameters.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-10 17:43:24.000000 bluepyopt-1.9.96/bluepyopt/tests/test_ephys/testmodels/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1483 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_ephys/testmodels/dummycells.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_ephys/testmodels/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7773 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_ephys/test_models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3591 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_ephys/test_evaluators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3825 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_ephys/test_morphologies.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6839 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_ephys/test_locations.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2276 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_ephys/test_recordings.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9761 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_ephys/test_features.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-10 17:43:24.000000 bluepyopt-1.9.96/bluepyopt/tests/test_ephys/testdata/
--rw-rw-r--   0 travis    (2000) travis    (2000)      100 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_ephys/testdata/simple.swc
--rw-rw-r--   0 travis    (2000) travis    (2000)     4835 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_ephys/testdata/test.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)      137 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_ephys/testdata/apic.swc
--rw-rw-r--   0 travis    (2000) travis    (2000)      387 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_ephys/testdata/simple_ax2.asc
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_ephys/testdata/simple.wrong
--rw-rw-r--   0 travis    (2000) travis    (2000)      145 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_ephys/testdata/simple_ax1.swc
--rw-rw-r--   0 travis    (2000) travis    (2000)      169 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_ephys/testdata/simple_ax2.swc
--rw-rw-r--   0 travis    (2000) travis    (2000)   202089 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_ephys/testdata/TimeVoltageResponse.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     1770 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_ephys/test_parameterscalers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11552 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_ephys/test_protocols.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2223 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_ephys/test_serializer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4962 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_ephys/test_simulators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1496 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_ephys/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2615 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_ephys/test_create_hoc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6093 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_ephys/test_objectives.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5889 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_ephys/test_mechanisms.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6706 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_ephys/test_stimuli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1245 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_ephys/test_init.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5295 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_l5pc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3589 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_stochkv.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-10 17:43:24.000000 bluepyopt-1.9.96/bluepyopt/tests/test_deapext/
--rw-rw-r--   0 travis    (2000) travis    (2000)      577 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_deapext/test_stoppingCriteria.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1381 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_deapext/deapext_test_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3122 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_deapext/test_optimisations.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2193 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_deapext/test_selIBEA.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4222 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_deapext/test_algorithms.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4330 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_parameters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1134 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_evaluators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5535 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/disable_simplecell_scoop.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       41 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/.gitignore
--rw-rw-r--   0 travis    (2000) travis    (2000)     1175 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_simplecell.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      997 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/test_bluepyopt.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1971 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/tests/expected_results.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1127 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/bluepyopt/stoppingCriteria.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2848 2020-12-10 17:38:43.000000 bluepyopt-1.9.96/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-11 13:48:46.000000 bluepyopt-1.9.98/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      201 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69513 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/versioneer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1042 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/LICENSE.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      179 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/AUTHORS.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1189 2020-12-11 13:48:46.000000 bluepyopt-1.9.98/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7970 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-11 13:48:46.000000 bluepyopt-1.9.98/bluepyopt.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1189 2020-12-11 13:48:46.000000 bluepyopt-1.9.98/bluepyopt.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-12-11 13:48:46.000000 bluepyopt-1.9.98/bluepyopt.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       10 2020-12-11 13:48:46.000000 bluepyopt-1.9.98/bluepyopt.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3415 2020-12-11 13:48:46.000000 bluepyopt-1.9.98/bluepyopt.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      116 2020-12-11 13:48:46.000000 bluepyopt-1.9.98/bluepyopt.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       69 2020-12-11 13:48:46.000000 bluepyopt-1.9.98/bluepyopt.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7651 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/LGPL.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      202 2020-12-11 13:48:46.000000 bluepyopt-1.9.98/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-11 13:48:46.000000 bluepyopt-1.9.98/bluepyopt/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-11 13:48:46.000000 bluepyopt-1.9.98/bluepyopt/ipyp/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/ipyp/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4571 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/ipyp/bpopt_tasksdb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      498 2020-12-11 13:48:46.000000 bluepyopt-1.9.98/bluepyopt/_version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      218 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tools.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-11 13:48:46.000000 bluepyopt-1.9.98/bluepyopt/ephys/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6856 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/ephys/create_hoc.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-11 13:48:46.000000 bluepyopt-1.9.98/bluepyopt/ephys/examples/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-11 13:48:46.000000 bluepyopt-1.9.98/bluepyopt/ephys/examples/simplecell/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2560 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/ephys/examples/simplecell/simplecell.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      100 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/ephys/examples/simplecell/simple.swc
+-rw-rw-r--   0 travis    (2000) travis    (2000)       46 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/ephys/examples/simplecell/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       45 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/ephys/examples/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9967 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/ephys/protocols.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1525 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/ephys/objectivescalculators.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-11 13:48:46.000000 bluepyopt-1.9.98/bluepyopt/ephys/templates/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4985 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/ephys/templates/cell_template.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10039 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/ephys/mechanisms.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6073 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/ephys/parameterscalers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9462 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/ephys/locations.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15998 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/ephys/models.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2513 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/ephys/serializer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3261 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/ephys/objectives.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7516 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/ephys/morphologies.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7882 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/ephys/evaluators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12265 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/ephys/parameters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      341 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/ephys/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1515 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/ephys/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3018 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/ephys/recordings.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10321 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/ephys/stimuli.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7658 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/ephys/efeatures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2300 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/ephys/responses.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4821 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/ephys/simulators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      999 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/optimisations.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1008 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/objectives.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2341 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/evaluators.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-11 13:48:46.000000 bluepyopt-1.9.98/bluepyopt/deapext/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6446 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/deapext/algorithms.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10523 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/deapext/optimisations.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-11 13:48:46.000000 bluepyopt-1.9.98/bluepyopt/deapext/tools/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4774 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/deapext/tools/selIBEA.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       43 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/deapext/tools/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       18 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/deapext/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1404 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/deapext/stoppingCriteria.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4722 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/parameters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      963 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/api.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1677 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-11 13:48:46.000000 bluepyopt-1.9.98/bluepyopt/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      904 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_tools.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-11 13:48:46.000000 bluepyopt-1.9.98/bluepyopt/tests/test_ephys/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2076 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_ephys/test_parameters.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-11 13:48:46.000000 bluepyopt-1.9.98/bluepyopt/tests/test_ephys/testmodels/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1483 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_ephys/testmodels/dummycells.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_ephys/testmodels/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7773 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_ephys/test_models.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3591 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_ephys/test_evaluators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3825 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_ephys/test_morphologies.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6839 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_ephys/test_locations.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2276 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_ephys/test_recordings.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9761 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_ephys/test_features.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-11 13:48:46.000000 bluepyopt-1.9.98/bluepyopt/tests/test_ephys/testdata/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      100 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_ephys/testdata/simple.swc
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4835 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_ephys/testdata/test.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)      137 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_ephys/testdata/apic.swc
+-rw-rw-r--   0 travis    (2000) travis    (2000)      387 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_ephys/testdata/simple_ax2.asc
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_ephys/testdata/simple.wrong
+-rw-rw-r--   0 travis    (2000) travis    (2000)      145 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_ephys/testdata/simple_ax1.swc
+-rw-rw-r--   0 travis    (2000) travis    (2000)      169 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_ephys/testdata/simple_ax2.swc
+-rw-rw-r--   0 travis    (2000) travis    (2000)   202089 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_ephys/testdata/TimeVoltageResponse.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1770 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_ephys/test_parameterscalers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11552 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_ephys/test_protocols.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2223 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_ephys/test_serializer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4962 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_ephys/test_simulators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1496 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_ephys/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2615 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_ephys/test_create_hoc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6093 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_ephys/test_objectives.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5889 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_ephys/test_mechanisms.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6706 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_ephys/test_stimuli.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1245 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_ephys/test_init.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5295 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_l5pc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3589 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_stochkv.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-11 13:48:46.000000 bluepyopt-1.9.98/bluepyopt/tests/test_deapext/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      577 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_deapext/test_stoppingCriteria.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1381 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_deapext/deapext_test_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3122 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_deapext/test_optimisations.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2193 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_deapext/test_selIBEA.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4222 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_deapext/test_algorithms.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4330 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_parameters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1134 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_evaluators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5535 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/disable_simplecell_scoop.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       41 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/.gitignore
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1175 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_simplecell.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      997 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/test_bluepyopt.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1971 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/tests/expected_results.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1127 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/bluepyopt/stoppingCriteria.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2848 2020-12-11 13:43:39.000000 bluepyopt-1.9.98/setup.py
```

### Comparing `bluepyopt-1.9.96/versioneer.py` & `bluepyopt-1.9.98/versioneer.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/LICENSE.txt` & `bluepyopt-1.9.98/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/PKG-INFO` & `bluepyopt-1.9.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bluepyopt
-Version: 1.9.96
+Version: 1.9.98
 Summary: Bluebrain Python Optimisation Library (bluepyopt)
 Home-page: https://github.com/BlueBrain/BluePyOpt
 Author: BlueBrain Project, EPFL
 Author-email: werner.vangeit@epfl.ch
 License: LGPLv3
 Description: The Blue Brain Python Optimisation Library (BluePyOpt) is an extensible framework for data-driven model parameter optimisation that wraps and standardises several existing open-source tools. It simplifies the task of creating and sharing these optimisations, and the associated techniques and knowledge. This is achieved by abstracting the optimisation and evaluation tasks into various reusable and flexible discrete elements according to established best-practices.
 Keywords: optimisation,neuroscience,BlueBrainProject
```

### Comparing `bluepyopt-1.9.96/README.md` & `bluepyopt-1.9.98/README.md`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt.egg-info/PKG-INFO` & `bluepyopt-1.9.98/bluepyopt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bluepyopt
-Version: 1.9.96
+Version: 1.9.98
 Summary: Bluebrain Python Optimisation Library (bluepyopt)
 Home-page: https://github.com/BlueBrain/BluePyOpt
 Author: BlueBrain Project, EPFL
 Author-email: werner.vangeit@epfl.ch
 License: LGPLv3
 Description: The Blue Brain Python Optimisation Library (BluePyOpt) is an extensible framework for data-driven model parameter optimisation that wraps and standardises several existing open-source tools. It simplifies the task of creating and sharing these optimisations, and the associated techniques and knowledge. This is achieved by abstracting the optimisation and evaluation tasks into various reusable and flexible discrete elements according to established best-practices.
 Keywords: optimisation,neuroscience,BlueBrainProject
```

### Comparing `bluepyopt-1.9.96/bluepyopt.egg-info/SOURCES.txt` & `bluepyopt-1.9.98/bluepyopt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/LGPL.txt` & `bluepyopt-1.9.98/LGPL.txt`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/ipyp/bpopt_tasksdb.py` & `bluepyopt-1.9.98/bluepyopt/ipyp/bpopt_tasksdb.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/ephys/create_hoc.py` & `bluepyopt-1.9.98/bluepyopt/ephys/create_hoc.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/ephys/examples/simplecell/simplecell.py` & `bluepyopt-1.9.98/bluepyopt/ephys/examples/simplecell/simplecell.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/ephys/protocols.py` & `bluepyopt-1.9.98/bluepyopt/ephys/protocols.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/ephys/objectivescalculators.py` & `bluepyopt-1.9.98/bluepyopt/ephys/objectivescalculators.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/ephys/templates/cell_template.jinja2` & `bluepyopt-1.9.98/bluepyopt/ephys/templates/cell_template.jinja2`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/ephys/mechanisms.py` & `bluepyopt-1.9.98/bluepyopt/ephys/mechanisms.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/ephys/parameterscalers.py` & `bluepyopt-1.9.98/bluepyopt/ephys/parameterscalers.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/ephys/locations.py` & `bluepyopt-1.9.98/bluepyopt/ephys/locations.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/ephys/models.py` & `bluepyopt-1.9.98/bluepyopt/ephys/models.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/ephys/serializer.py` & `bluepyopt-1.9.98/bluepyopt/ephys/serializer.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/ephys/objectives.py` & `bluepyopt-1.9.98/bluepyopt/ephys/objectives.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/ephys/morphologies.py` & `bluepyopt-1.9.98/bluepyopt/ephys/morphologies.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/ephys/evaluators.py` & `bluepyopt-1.9.98/bluepyopt/ephys/evaluators.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/ephys/parameters.py` & `bluepyopt-1.9.98/bluepyopt/ephys/parameters.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/ephys/__init__.py` & `bluepyopt-1.9.98/bluepyopt/ephys/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/ephys/recordings.py` & `bluepyopt-1.9.98/bluepyopt/ephys/recordings.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/ephys/stimuli.py` & `bluepyopt-1.9.98/bluepyopt/ephys/stimuli.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/ephys/efeatures.py` & `bluepyopt-1.9.98/bluepyopt/ephys/efeatures.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/ephys/responses.py` & `bluepyopt-1.9.98/bluepyopt/ephys/responses.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/ephys/simulators.py` & `bluepyopt-1.9.98/bluepyopt/ephys/simulators.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/optimisations.py` & `bluepyopt-1.9.98/bluepyopt/optimisations.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/objectives.py` & `bluepyopt-1.9.98/bluepyopt/objectives.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/evaluators.py` & `bluepyopt-1.9.98/bluepyopt/evaluators.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/deapext/algorithms.py` & `bluepyopt-1.9.98/bluepyopt/deapext/algorithms.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/deapext/optimisations.py` & `bluepyopt-1.9.98/bluepyopt/deapext/optimisations.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/deapext/tools/selIBEA.py` & `bluepyopt-1.9.98/bluepyopt/deapext/tools/selIBEA.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/deapext/stoppingCriteria.py` & `bluepyopt-1.9.98/bluepyopt/deapext/stoppingCriteria.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/parameters.py` & `bluepyopt-1.9.98/bluepyopt/parameters.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/api.py` & `bluepyopt-1.9.98/bluepyopt/api.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/__init__.py` & `bluepyopt-1.9.98/bluepyopt/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/tests/test_tools.py` & `bluepyopt-1.9.98/bluepyopt/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/tests/test_ephys/test_parameters.py` & `bluepyopt-1.9.98/bluepyopt/tests/test_ephys/test_parameters.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/tests/test_ephys/testmodels/dummycells.py` & `bluepyopt-1.9.98/bluepyopt/tests/test_ephys/testmodels/dummycells.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/tests/test_ephys/test_models.py` & `bluepyopt-1.9.98/bluepyopt/tests/test_ephys/test_models.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/tests/test_ephys/test_evaluators.py` & `bluepyopt-1.9.98/bluepyopt/tests/test_ephys/test_evaluators.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/tests/test_ephys/test_morphologies.py` & `bluepyopt-1.9.98/bluepyopt/tests/test_ephys/test_morphologies.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/tests/test_ephys/test_locations.py` & `bluepyopt-1.9.98/bluepyopt/tests/test_ephys/test_locations.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/tests/test_ephys/test_recordings.py` & `bluepyopt-1.9.98/bluepyopt/tests/test_ephys/test_recordings.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/tests/test_ephys/test_features.py` & `bluepyopt-1.9.98/bluepyopt/tests/test_ephys/test_features.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/tests/test_ephys/testdata/test.jinja2` & `bluepyopt-1.9.98/bluepyopt/tests/test_ephys/testdata/test.jinja2`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/tests/test_ephys/testdata/TimeVoltageResponse.csv` & `bluepyopt-1.9.98/bluepyopt/tests/test_ephys/testdata/TimeVoltageResponse.csv`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/tests/test_ephys/test_parameterscalers.py` & `bluepyopt-1.9.98/bluepyopt/tests/test_ephys/test_parameterscalers.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/tests/test_ephys/test_protocols.py` & `bluepyopt-1.9.98/bluepyopt/tests/test_ephys/test_protocols.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/tests/test_ephys/test_serializer.py` & `bluepyopt-1.9.98/bluepyopt/tests/test_ephys/test_serializer.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/tests/test_ephys/test_simulators.py` & `bluepyopt-1.9.98/bluepyopt/tests/test_ephys/test_simulators.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/tests/test_ephys/utils.py` & `bluepyopt-1.9.98/bluepyopt/tests/test_ephys/utils.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/tests/test_ephys/test_create_hoc.py` & `bluepyopt-1.9.98/bluepyopt/tests/test_ephys/test_create_hoc.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/tests/test_ephys/test_objectives.py` & `bluepyopt-1.9.98/bluepyopt/tests/test_ephys/test_objectives.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/tests/test_ephys/test_mechanisms.py` & `bluepyopt-1.9.98/bluepyopt/tests/test_ephys/test_mechanisms.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/tests/test_ephys/test_stimuli.py` & `bluepyopt-1.9.98/bluepyopt/tests/test_ephys/test_stimuli.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/tests/test_ephys/test_init.py` & `bluepyopt-1.9.98/bluepyopt/tests/test_ephys/test_init.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/tests/test_l5pc.py` & `bluepyopt-1.9.98/bluepyopt/tests/test_l5pc.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/tests/test_stochkv.py` & `bluepyopt-1.9.98/bluepyopt/tests/test_stochkv.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/tests/test_deapext/test_stoppingCriteria.py` & `bluepyopt-1.9.98/bluepyopt/tests/test_deapext/test_stoppingCriteria.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/tests/test_deapext/deapext_test_utils.py` & `bluepyopt-1.9.98/bluepyopt/tests/test_deapext/deapext_test_utils.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/tests/test_deapext/test_optimisations.py` & `bluepyopt-1.9.98/bluepyopt/tests/test_deapext/test_optimisations.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/tests/test_deapext/test_selIBEA.py` & `bluepyopt-1.9.98/bluepyopt/tests/test_deapext/test_selIBEA.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/tests/test_deapext/test_algorithms.py` & `bluepyopt-1.9.98/bluepyopt/tests/test_deapext/test_algorithms.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/tests/test_parameters.py` & `bluepyopt-1.9.98/bluepyopt/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/tests/test_evaluators.py` & `bluepyopt-1.9.98/bluepyopt/tests/test_evaluators.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/tests/disable_simplecell_scoop.py` & `bluepyopt-1.9.98/bluepyopt/tests/disable_simplecell_scoop.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/tests/test_simplecell.py` & `bluepyopt-1.9.98/bluepyopt/tests/test_simplecell.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/tests/test_bluepyopt.py` & `bluepyopt-1.9.98/bluepyopt/tests/test_bluepyopt.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/tests/expected_results.json` & `bluepyopt-1.9.98/bluepyopt/tests/expected_results.json`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/bluepyopt/stoppingCriteria.py` & `bluepyopt-1.9.98/bluepyopt/stoppingCriteria.py`

 * *Files identical despite different names*

### Comparing `bluepyopt-1.9.96/setup.py` & `bluepyopt-1.9.98/setup.py`

 * *Files identical despite different names*

