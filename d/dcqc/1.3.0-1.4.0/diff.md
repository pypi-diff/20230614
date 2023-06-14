# Comparing `tmp/dcqc-1.3.0.tar.gz` & `tmp/dcqc-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcqc-1.3.0.tar", last modified: Wed Apr 12 07:28:55 2023, max compression
+gzip compressed data, was "dcqc-1.4.0.tar", last modified: Tue May 30 18:18:39 2023, max compression
```

## Comparing `dcqc-1.3.0.tar` & `dcqc-1.4.0.tar`

### file list

```diff
@@ -1,96 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:28:55.424489 dcqc-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-12 07:28:01.000000 dcqc-1.3.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:28:55.412489 dcqc-1.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:28:55.416489 dcqc-1.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-04-12 07:28:01.000000 dcqc-1.3.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-12 07:28:01.000000 dcqc-1.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-12 07:28:01.000000 dcqc-1.3.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-12 07:28:01.000000 dcqc-1.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-12 07:28:01.000000 dcqc-1.3.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-12 07:28:01.000000 dcqc-1.3.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-12 07:28:01.000000 dcqc-1.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-04-12 07:28:01.000000 dcqc-1.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-12 07:28:01.000000 dcqc-1.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-12 07:28:55.424489 dcqc-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-12 07:28:01.000000 dcqc-1.3.0/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)   102584 2023-04-12 07:28:01.000000 dcqc-1.3.0/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-12 07:28:01.000000 dcqc-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:28:55.416489 dcqc-1.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-12 07:28:01.000000 dcqc-1.3.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:28:55.416489 dcqc-1.3.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 07:28:01.000000 dcqc-1.3.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-12 07:28:01.000000 dcqc-1.3.0/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-12 07:28:01.000000 dcqc-1.3.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-04-12 07:28:01.000000 dcqc-1.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-12 07:28:01.000000 dcqc-1.3.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-12 07:28:01.000000 dcqc-1.3.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-12 07:28:01.000000 dcqc-1.3.0/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-12 07:28:01.000000 dcqc-1.3.0/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-12 07:28:01.000000 dcqc-1.3.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-12 07:28:01.000000 dcqc-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-12 07:28:55.424489 dcqc-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-12 07:28:01.000000 dcqc-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:28:55.412489 dcqc-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:28:55.416489 dcqc-1.3.0/src/dcqc/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-12 07:28:01.000000 dcqc-1.3.0/src/dcqc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-12 07:28:01.000000 dcqc-1.3.0/src/dcqc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12514 2023-04-12 07:28:01.000000 dcqc-1.3.0/src/dcqc/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-04-12 07:28:01.000000 dcqc-1.3.0/src/dcqc/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-04-12 07:28:01.000000 dcqc-1.3.0/src/dcqc/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-04-12 07:28:01.000000 dcqc-1.3.0/src/dcqc/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-04-12 07:28:01.000000 dcqc-1.3.0/src/dcqc/reports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:28:55.420489 dcqc-1.3.0/src/dcqc/suites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:28:01.000000 dcqc-1.3.0/src/dcqc/suites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10380 2023-04-12 07:28:01.000000 dcqc-1.3.0/src/dcqc/suites/suite_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-12 07:28:01.000000 dcqc-1.3.0/src/dcqc/suites/suites.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-12 07:28:01.000000 dcqc-1.3.0/src/dcqc/target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:28:55.420489 dcqc-1.3.0/src/dcqc/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:28:01.000000 dcqc-1.3.0/src/dcqc/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-04-12 07:28:01.000000 dcqc-1.3.0/src/dcqc/tests/test_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-04-12 07:28:01.000000 dcqc-1.3.0/src/dcqc/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-12 07:28:01.000000 dcqc-1.3.0/src/dcqc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:28:55.420489 dcqc-1.3.0/src/dcqc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-12 07:28:55.000000 dcqc-1.3.0/src/dcqc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-12 07:28:55.000000 dcqc-1.3.0/src/dcqc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 07:28:55.000000 dcqc-1.3.0/src/dcqc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-12 07:28:55.000000 dcqc-1.3.0/src/dcqc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 07:28:55.000000 dcqc-1.3.0/src/dcqc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-12 07:28:55.000000 dcqc-1.3.0/src/dcqc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 07:28:55.000000 dcqc-1.3.0/src/dcqc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:28:55.420489 dcqc-1.3.0/src/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-12 07:28:01.000000 dcqc-1.3.0/src/docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-12 07:28:01.000000 dcqc-1.3.0/src/docker/build.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:28:55.420489 dcqc-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:28:55.420489 dcqc-1.3.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    76770 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/circuit.tif
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/example.bam
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/example.fastq
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/example.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/example.jsonld
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/example.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/file.json
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/files.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)     1671 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/small.csv
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/suite.json
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/target.json
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/test.computed.json
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/test.external.json
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/test.internal.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/test_contains_word_date.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/tests.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:28:55.424489 dcqc-1.3.0/tests/data/tiffinfo/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/tiffinfo/exit_code.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/tiffinfo/std_err.txt
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/tiffinfo/std_out.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/test_acceptance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/test_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/test_suites.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/test_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/test_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-12 07:28:01.000000 dcqc-1.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:18:39.891348 dcqc-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-30 18:17:45.000000 dcqc-1.4.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:18:39.879347 dcqc-1.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:18:39.883348 dcqc-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-05-30 18:17:45.000000 dcqc-1.4.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-30 18:17:45.000000 dcqc-1.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-30 18:17:45.000000 dcqc-1.4.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-30 18:17:45.000000 dcqc-1.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-30 18:17:45.000000 dcqc-1.4.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-30 18:17:45.000000 dcqc-1.4.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-30 18:17:45.000000 dcqc-1.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-05-30 18:17:45.000000 dcqc-1.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-30 18:17:45.000000 dcqc-1.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-05-30 18:18:39.891348 dcqc-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-30 18:17:45.000000 dcqc-1.4.0/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)   102584 2023-05-30 18:17:45.000000 dcqc-1.4.0/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-30 18:17:45.000000 dcqc-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:18:39.883348 dcqc-1.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-30 18:17:45.000000 dcqc-1.4.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:18:39.883348 dcqc-1.4.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-30 18:17:45.000000 dcqc-1.4.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-30 18:17:45.000000 dcqc-1.4.0/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-30 18:17:45.000000 dcqc-1.4.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-05-30 18:17:45.000000 dcqc-1.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-30 18:17:45.000000 dcqc-1.4.0/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-30 18:17:45.000000 dcqc-1.4.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-30 18:17:45.000000 dcqc-1.4.0/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-30 18:17:45.000000 dcqc-1.4.0/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-30 18:17:45.000000 dcqc-1.4.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-30 18:17:45.000000 dcqc-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-30 18:18:39.891348 dcqc-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-30 18:17:45.000000 dcqc-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:18:39.879347 dcqc-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:18:39.883348 dcqc-1.4.0/src/dcqc/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-30 18:17:45.000000 dcqc-1.4.0/src/dcqc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-30 18:17:45.000000 dcqc-1.4.0/src/dcqc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12514 2023-05-30 18:17:45.000000 dcqc-1.4.0/src/dcqc/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-05-30 18:17:45.000000 dcqc-1.4.0/src/dcqc/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-30 18:17:45.000000 dcqc-1.4.0/src/dcqc/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-05-30 18:17:45.000000 dcqc-1.4.0/src/dcqc/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-05-30 18:17:45.000000 dcqc-1.4.0/src/dcqc/reports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:18:39.887348 dcqc-1.4.0/src/dcqc/suites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:17:45.000000 dcqc-1.4.0/src/dcqc/suites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10380 2023-05-30 18:17:45.000000 dcqc-1.4.0/src/dcqc/suites/suite_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-30 18:17:45.000000 dcqc-1.4.0/src/dcqc/suites/suites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-30 18:17:45.000000 dcqc-1.4.0/src/dcqc/target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:18:39.887348 dcqc-1.4.0/src/dcqc/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:17:45.000000 dcqc-1.4.0/src/dcqc/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-05-30 18:17:45.000000 dcqc-1.4.0/src/dcqc/tests/test_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-05-30 18:17:45.000000 dcqc-1.4.0/src/dcqc/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-30 18:17:45.000000 dcqc-1.4.0/src/dcqc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:18:39.883348 dcqc-1.4.0/src/dcqc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-05-30 18:18:39.000000 dcqc-1.4.0/src/dcqc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-30 18:18:39.000000 dcqc-1.4.0/src/dcqc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 18:18:39.000000 dcqc-1.4.0/src/dcqc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-30 18:18:39.000000 dcqc-1.4.0/src/dcqc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 18:18:39.000000 dcqc-1.4.0/src/dcqc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-30 18:18:39.000000 dcqc-1.4.0/src/dcqc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-30 18:18:39.000000 dcqc-1.4.0/src/dcqc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:18:39.887348 dcqc-1.4.0/src/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-30 18:17:45.000000 dcqc-1.4.0/src/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-30 18:17:45.000000 dcqc-1.4.0/src/docker/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:18:39.887348 dcqc-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-30 18:17:45.000000 dcqc-1.4.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:18:39.887348 dcqc-1.4.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    76770 2023-05-30 18:17:45.000000 dcqc-1.4.0/tests/data/circuit.tif
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-30 18:17:45.000000 dcqc-1.4.0/tests/data/example.bam
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-30 18:17:45.000000 dcqc-1.4.0/tests/data/example.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-30 18:17:45.000000 dcqc-1.4.0/tests/data/example.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-30 18:17:45.000000 dcqc-1.4.0/tests/data/example.jsonld
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-30 18:17:45.000000 dcqc-1.4.0/tests/data/example.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-30 18:17:45.000000 dcqc-1.4.0/tests/data/file.json
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-30 18:17:45.000000 dcqc-1.4.0/tests/data/files.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1671 2023-05-30 18:17:45.000000 dcqc-1.4.0/tests/data/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-30 18:17:45.000000 dcqc-1.4.0/tests/data/small.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-30 18:17:45.000000 dcqc-1.4.0/tests/data/suite.json
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-30 18:17:45.000000 dcqc-1.4.0/tests/data/target.json
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-30 18:17:45.000000 dcqc-1.4.0/tests/data/test.computed.json
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-30 18:17:45.000000 dcqc-1.4.0/tests/data/test.external.json
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-30 18:17:45.000000 dcqc-1.4.0/tests/data/test.internal.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-30 18:17:45.000000 dcqc-1.4.0/tests/data/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-30 18:17:45.000000 dcqc-1.4.0/tests/data/test_contains_word_date.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   262517 2023-05-30 18:17:45.000000 dcqc-1.4.0/tests/data/test_image_dirty_datetime.tif
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-30 18:17:45.000000 dcqc-1.4.0/tests/data/tests.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:18:39.891348 dcqc-1.4.0/tests/data/tiffinfo/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-30 18:17:45.000000 dcqc-1.4.0/tests/data/tiffinfo/exit_code.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:17:45.000000 dcqc-1.4.0/tests/data/tiffinfo/std_err.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-30 18:17:45.000000 dcqc-1.4.0/tests/data/tiffinfo/std_out.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-30 18:17:45.000000 dcqc-1.4.0/tests/test_acceptance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-05-30 18:17:45.000000 dcqc-1.4.0/tests/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-30 18:17:45.000000 dcqc-1.4.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-30 18:17:45.000000 dcqc-1.4.0/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-30 18:17:45.000000 dcqc-1.4.0/tests/test_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-30 18:17:45.000000 dcqc-1.4.0/tests/test_suites.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-30 18:17:45.000000 dcqc-1.4.0/tests/test_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-05-30 18:17:45.000000 dcqc-1.4.0/tests/test_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-30 18:17:45.000000 dcqc-1.4.0/tox.ini
```

### Comparing `dcqc-1.3.0/.coveragerc` & `dcqc-1.4.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `dcqc-1.3.0/.github/workflows/ci.yml` & `dcqc-1.4.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `dcqc-1.3.0/.gitignore` & `dcqc-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dcqc-1.3.0/.pre-commit-config.yaml` & `dcqc-1.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dcqc-1.3.0/CONTRIBUTING.md` & `dcqc-1.4.0/CONTRIBUTING.md`

 * *Files 14% similar despite different names*

```diff
@@ -182,14 +182,44 @@
 2. Go to the web page of your fork and click "Create pull request"
    to send your changes for review.
 
    Find more detailed information in [creating a PR]. You might also want to open
    the PR as a draft first and mark it as ready for review after the feedbacks
    from the continuous integration (CI) system or any required fixes.
 
+### Special Considerations for Contributing External Tests
+
+In `py-dcqc`, any test where the primary business logic is executed outside of this package itself is considered to be external. One example is the `LibTiffInfoTest`. For these tests, `py-dcqc` is responsible for packaging up a Nextflow process which is then executed in an [nf-dcqc](https://github.com/Sage-Bionetworks-Workflows/nf-dcqc) workflow run. Such tests are not possible to run in `py-dcqc` alone at this time. This makes contributing, testing, debugging, and using external tests a little more complicated that internal tests such as the `Md5ChecksumTest` which has all of its logic built into this package.
+
+When contributing an external test, following these steps may be helpful:
+
+1. Follow the steps above to set up `py-dcqc` and create your contribution.
+
+2. Follow the instructions in the [README.md](https://github.com/Sage-Bionetworks-Workflows/nf-dcqc/blob/dev/README.md)
+   file in the `nf-dcqc` respository to set up the workflow on your local machine.
+   - Run `git checkout dev` to switch to the developer branch
+
+3. Build your local version of `py-dcqc` with your new changes with:
+   ```console
+   src/docker/build.sh
+   ```
+   NOTE: This step assumes that you have docker installed and that it is running, and that you have `pipx` installed.
+
+4. Follow `nf-dcqc` instructions to create a `nextflow run` command that tests your contribution.
+   - You should include at least two files in your `nf-dcqc` input file ([example](https://github.com/Sage-Bionetworks-Workflows/nf-dcqc/blob/dev/testdata/input_full.csv)), one that you expect to pass your contributed test, and one that you expect to fail.
+   - Include the `local` profile so that the workflow leverages your locally built `py-orca` container
+
+   Example command (executed from within your local `nf-dcqc` repo clone):
+   ```
+   nextflow run main.nf -profile local,docker --input path/to/your/input.csv -- outdir output --required_tests <YOUR_TEST_NAME>
+   ```
+
+5. Examine the final `suites.json` that is exported by the Nextflow workflow, if your contributed test bahaved as
+   expected, you're done! If not, debug and make changes to your contribution and re-run the workflow.
+
 ### Troubleshooting
 
 The following tips can be used when facing problems to build or test the
 package:
 
 1. Make sure to fetch all the tags from the upstream [repository].
    The command `git describe --abbrev=0 --tags` should return the version you
```

### Comparing `dcqc-1.3.0/LICENSE.txt` & `dcqc-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcqc-1.3.0/PKG-INFO` & `dcqc-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcqc
-Version: 1.3.0
+Version: 1.4.0
 Summary: Python package for performing quality control (QC) for data coordination (DC)
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Bruno Grande
 Author-email: bruno.grande@sagebase.org
 License: Apache-2.0
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `dcqc-1.3.0/Pipfile.lock` & `dcqc-1.4.0/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `dcqc-1.3.0/README.md` & `dcqc-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `dcqc-1.3.0/docs/Makefile` & `dcqc-1.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dcqc-1.3.0/docs/conf.py` & `dcqc-1.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.3.0/docs/index.md` & `dcqc-1.4.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `dcqc-1.3.0/pyproject.toml` & `dcqc-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dcqc-1.3.0/setup.cfg` & `dcqc-1.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `dcqc-1.3.0/setup.py` & `dcqc-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.3.0/src/dcqc/__init__.py` & `dcqc-1.4.0/src/dcqc/__init__.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.3.0/src/dcqc/file.py` & `dcqc-1.4.0/src/dcqc/file.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.3.0/src/dcqc/main.py` & `dcqc-1.4.0/src/dcqc/main.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.3.0/src/dcqc/mixins.py` & `dcqc-1.4.0/src/dcqc/mixins.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.3.0/src/dcqc/parsers.py` & `dcqc-1.4.0/src/dcqc/parsers.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.3.0/src/dcqc/reports.py` & `dcqc-1.4.0/src/dcqc/reports.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.3.0/src/dcqc/suites/suite_abc.py` & `dcqc-1.4.0/src/dcqc/suites/suite_abc.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.3.0/src/dcqc/suites/suites.py` & `dcqc-1.4.0/src/dcqc/suites/suites.py`

 * *Files 27% similar despite different names*

```diff
@@ -18,15 +18,19 @@
 class JsonLdSuite(JsonSuite):
     file_type = FileType.get_file_type("JSON-LD")
     add_tests = (tests.JsonLdLoadTest,)
 
 
 class TiffSuite(FileSuite):
     file_type = FileType.get_file_type("TIFF")
-    add_tests = (tests.LibTiffInfoTest, tests.GrepDateTest)
+    add_tests = (
+        tests.LibTiffInfoTest,
+        tests.GrepDateTest,
+        tests.TiffTag306DateTimeTest,
+    )
 
 
 class OmeTiffSuite(TiffSuite):
     file_type = FileType.get_file_type("OME-TIFF")
     add_tests = (tests.OmeXmlSchemaTest, tests.BioFormatsInfoTest)
```

### Comparing `dcqc-1.3.0/src/dcqc/target.py` & `dcqc-1.4.0/src/dcqc/target.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.3.0/src/dcqc/tests/test_abc.py` & `dcqc-1.4.0/src/dcqc/tests/test_abc.py`

 * *Files identical despite different names*

```diff
@@ -181,15 +181,15 @@
     _serialized_properties = ["command"]
 
     def __post_init__(self, command_args: Sequence[str]):
         self._command_args = command_args
 
     @property
     def command(self) -> str:
-        return shlex.join(self._command_args)
+        return " ".join(self._command_args)
 
     @classmethod
     def from_dict(cls, dictionary: SerializedObject) -> Process:
         """Deserialize a dictionary into a process.
 
         Args:
             dictionary: A serialized proces object.
```

### Comparing `dcqc-1.3.0/src/dcqc/tests/tests.py` & `dcqc-1.4.0/src/dcqc/tests/tests.py`

 * *Files 14% similar despite different names*

```diff
@@ -141,19 +141,45 @@
 class GrepDateTest(ExternalTestMixin, TestABC):
     tier = 4
 
     def generate_process(self) -> Process:
         file = self.get_file()
         path = file.local_path.as_posix()
         command_args = [
+            "!",  # negate exit status
             "grep",
-            "-E",
-            "-w",
-            "-i",
-            "'date|time'",
+            "-E",  # extended regular expression
+            "-i",  # case insensitive
+            "-a",  # treat input as text
+            "-q",  # suppress output
+            "'date|time'",  # match date or time
             path,
         ]
         process = Process(
             container="quay.io/biocontainers/coreutils:8.30--h14c3975_1000",
             command_args=command_args,
         )
         return process
+
+
+class TiffTag306DateTimeTest(ExternalTestMixin, TestABC):
+    tier = 4
+
+    def generate_process(self) -> Process:
+        file = self.get_file()
+        path = file.local_path.as_posix()
+        command_args = [
+            "!",  # negate exit status
+            "tifftools",
+            "dump",
+            path,
+            "|",
+            "grep",  # pipe the output
+            "-a",  # treat input as text
+            "-q",  # suppress output
+            "'DateTime 306 (0x132) ASCII'",  # match the DateTime 306 tag
+        ]
+        process = Process(
+            container="ghcr.io/sage-bionetworks-workflows/tifftools:latest",
+            command_args=command_args,
+        )
+        return process
```

### Comparing `dcqc-1.3.0/src/dcqc/utils.py` & `dcqc-1.4.0/src/dcqc/utils.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.3.0/src/dcqc.egg-info/PKG-INFO` & `dcqc-1.4.0/src/dcqc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcqc
-Version: 1.3.0
+Version: 1.4.0
 Summary: Python package for performing quality control (QC) for data coordination (DC)
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Bruno Grande
 Author-email: bruno.grande@sagebase.org
 License: Apache-2.0
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `dcqc-1.3.0/src/dcqc.egg-info/SOURCES.txt` & `dcqc-1.4.0/src/dcqc.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -71,11 +71,12 @@
 tests/data/suite.json
 tests/data/target.json
 tests/data/test.computed.json
 tests/data/test.external.json
 tests/data/test.internal.json
 tests/data/test.txt
 tests/data/test_contains_word_date.txt
+tests/data/test_image_dirty_datetime.tif
 tests/data/tests.json
 tests/data/tiffinfo/exit_code.txt
 tests/data/tiffinfo/std_err.txt
 tests/data/tiffinfo/std_out.txt
```

### Comparing `dcqc-1.3.0/tests/conftest.py` & `dcqc-1.4.0/tests/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 
 @pytest.fixture
 def test_files(get_data):
     txt_path = get_data("test.txt")
     jsonld_path = get_data("example.jsonld")
     tiff_path = get_data("circuit.tif")
     syn_path = "syn://syn50555279"
+    tiff_dirty_datetime_path = get_data("test_image_dirty_datetime.tif")
     good_metadata = {
         "file_type": "txt",
         "md5_checksum": "14758f1afd44c09b7992073ccf00b43d",
     }
     bad_metadata = {
         "file_type": "tiff",
         "md5_checksum": "definitelynottherightmd5checksum",
@@ -69,20 +70,27 @@
         "file_type": "JSON-LD",
         "md5_checksum": "56bb5f34da6d6df2ade3ac37e25586b7",
     }
     tiff_metadata = {
         "file_type": "tiff",
         "md5_checksum": "c7b08f6decb5e7572efbe6074926a843",
     }
+    tiff_dirty_datetime_metadata = {
+        "file_type": "tiff",
+        "md5_checksum": "28a9ee7d0e994d494068ce8d6cda0268",
+    }
     test_files = {
         "good": File(txt_path.as_posix(), good_metadata),
         "bad": File(txt_path.as_posix(), bad_metadata),
         "tiff": File(tiff_path.as_posix(), tiff_metadata),
         "jsonld": File(jsonld_path.as_posix(), jsonld_metadata),
         "synapse": File(syn_path, good_metadata),
+        "tiff_dirty_datetime": File(
+            tiff_dirty_datetime_path.as_posix(), tiff_dirty_datetime_metadata
+        ),
     }
 
     # Create an in-memory remote file based on the good file
     remote_file = File(f"mem://{txt_path.name}", good_metadata)
     remote_file.fs.writetext(remote_file.fs_path, txt_path.read_text())
     test_files["remote"] = remote_file
```

### Comparing `dcqc-1.3.0/tests/data/circuit.tif` & `dcqc-1.4.0/tests/data/circuit.tif`

 * *Files identical despite different names*

### Comparing `dcqc-1.3.0/tests/data/example.jsonld` & `dcqc-1.4.0/tests/data/example.jsonld`

 * *Files identical despite different names*

### Comparing `dcqc-1.3.0/tests/data/files.csv` & `dcqc-1.4.0/tests/data/files.csv`

 * *Files identical despite different names*

### Comparing `dcqc-1.3.0/tests/data/generate.py` & `dcqc-1.4.0/tests/data/generate.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.3.0/tests/data/suite.json` & `dcqc-1.4.0/tests/data/suite.json`

 * *Files identical despite different names*

### Comparing `dcqc-1.3.0/tests/data/tests.json` & `dcqc-1.4.0/tests/data/tests.json`

 * *Files identical despite different names*

### Comparing `dcqc-1.3.0/tests/test_acceptance.py` & `dcqc-1.4.0/tests/test_acceptance.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.3.0/tests/test_file.py` & `dcqc-1.4.0/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.3.0/tests/test_main.py` & `dcqc-1.4.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.3.0/tests/test_parsers.py` & `dcqc-1.4.0/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.3.0/tests/test_reports.py` & `dcqc-1.4.0/tests/test_reports.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.3.0/tests/test_suites.py` & `dcqc-1.4.0/tests/test_suites.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import pytest
 
 from dcqc.file import FileType
 from dcqc.suites.suite_abc import SuiteABC
 from dcqc.suites.suites import FileSuite, OmeTiffSuite, TiffSuite
 from dcqc.tests.test_abc import TestABC, TestStatus
-from dcqc.tests.tests import FileExtensionTest, GrepDateTest, LibTiffInfoTest
+from dcqc.tests.tests import (
+    FileExtensionTest,
+    GrepDateTest,
+    LibTiffInfoTest,
+    TiffTag306DateTimeTest,
+)
 
 FileType("None", ())
 FileType("Unpaired", ())
 
 
 class RedundantFileSuite(TiffSuite):
     file_type = FileType.get_file_type("None")
-    del_tests = (
-        LibTiffInfoTest,
-        GrepDateTest,
-    )
+    del_tests = (LibTiffInfoTest, GrepDateTest, TiffTag306DateTimeTest)
 
 
 class DummyTest(TestABC):
     def compute_status(self) -> TestStatus:
         return TestStatus.NONE
 
 
@@ -96,24 +98,24 @@
     with pytest.raises(ValueError):
         SuiteABC.from_tests(tests)
 
 
 def test_that_a_suite_will_not_consider_unrequired_tests(test_targets):
     target = test_targets["bad"]
     required_tests = []
-    skipped_tests = ["LibTiffInfoTest", "GrepDateTest"]
+    skipped_tests = ["LibTiffInfoTest", "GrepDateTest", "TiffTag306DateTimeTest"]
     suite = SuiteABC.from_target(target, required_tests, skipped_tests)
     suite_status = suite.compute_status()
     assert suite_status == TestStatus.PASS
 
 
 def test_that_a_suite_will_consider_required_tests_when_failing(test_targets):
     target = test_targets["bad"]
     required_tests = ["FileExtensionTest"]
-    skipped_tests = ["LibTiffInfoTest", "GrepDateTest"]
+    skipped_tests = ["LibTiffInfoTest", "GrepDateTest", "TiffTag306DateTimeTest"]
     suite = SuiteABC.from_target(target, required_tests, skipped_tests)
     suite_status = suite.compute_status()
     assert suite_status == TestStatus.FAIL
 
 
 def test_that_a_suite_will_consider_required_tests_when_passing(test_targets):
     target = test_targets["good"]
```

### Comparing `dcqc-1.3.0/tests/test_target.py` & `dcqc-1.4.0/tests/test_target.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.3.0/tests/test_tests.py` & `dcqc-1.4.0/tests/test_tests.py`

 * *Files 10% similar despite different names*

```diff
@@ -225,7 +225,38 @@
 
 def test_for_an_error_when_getting_one_file_from_multi_file_target(test_files):
     file = test_files["good"]
     target = Target(file, file)
     test = tests.FileExtensionTest(target)
     with pytest.raises(ValueError):
         test.get_file()
+
+
+def test_that_the_tifftag306datetimetest_command_is_produced(test_targets):
+    target = test_targets["tiff"]
+    test = tests.TiffTag306DateTimeTest(target)
+    process = test.generate_process()
+    assert "grep" in process.command
+
+
+def test_that_the_tifftag306datetimetest_correctly_interprets_exit_code_0_and_1(
+    test_files, mocker
+):
+    tiff_file = test_files["tiff"]
+    target = Target(tiff_file)
+    with TemporaryDirectory() as tmp_dir:
+        path_0 = Path(tmp_dir, "code_0.txt")
+        path_1 = Path(tmp_dir, "code_1.txt")
+        path_0.write_text("0")
+        path_1.write_text("1")
+        good_outputs = {"std_out": path_1, "std_err": path_1, "exit_code": path_0}
+        bad_outputs = {"std_out": path_0, "std_err": path_0, "exit_code": path_1}
+
+        test = tests.TiffTag306DateTimeTest(target)
+        mocker.patch.object(test, "_find_process_outputs", return_value=good_outputs)
+        test_status = test.get_status()
+        assert test_status == TestStatus.PASS
+
+        test = tests.LibTiffInfoTest(target)
+        mocker.patch.object(test, "_find_process_outputs", return_value=bad_outputs)
+        test_status = test.get_status()
+        assert test_status == TestStatus.FAIL
```

### Comparing `dcqc-1.3.0/tox.ini` & `dcqc-1.4.0/tox.ini`

 * *Files identical despite different names*

