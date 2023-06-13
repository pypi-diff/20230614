# Comparing `tmp/gtnet-0.0.1.tar.gz` & `tmp/gtnet-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gtnet-0.0.1.tar", last modified: Mon Jun 12 18:16:05 2023, max compression
+gzip compressed data, was "gtnet-0.0.2.tar", last modified: Tue Jun 13 23:00:26 2023, max compression
```

## Comparing `gtnet-0.0.1.tar` & `gtnet-0.0.2.tar`

### file list

```diff
@@ -1,82 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:16:05.787259 gtnet-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-12 18:15:53.000000 gtnet-0.0.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:16:05.767258 gtnet-0.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-06-12 18:15:53.000000 gtnet-0.0.1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-12 18:15:53.000000 gtnet-0.0.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:16:05.767258 gtnet-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-12 18:15:53.000000 gtnet-0.0.1/.github/workflows/codespell.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-12 18:15:53.000000 gtnet-0.0.1/.github/workflows/deploy_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-12 18:15:53.000000 gtnet-0.0.1/.github/workflows/ruff.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-12 18:15:53.000000 gtnet-0.0.1/.github/workflows/run_coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-12 18:15:53.000000 gtnet-0.0.1/.github/workflows/run_tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-12 18:15:53.000000 gtnet-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-12 18:15:53.000000 gtnet-0.0.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-12 18:15:53.000000 gtnet-0.0.1/Legal.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-06-12 18:16:05.787259 gtnet-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-06-12 18:15:53.000000 gtnet-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:16:05.775259 gtnet-0.0.1/data/
--rw-r--r--   0 runner    (1001) docker     (123)  5437423 2023-06-12 18:15:53.000000 gtnet-0.0.1/data/GCA_000006155.2.fna
--rw-r--r--   0 runner    (1001) docker     (123)    61553 2023-06-12 18:15:53.000000 gtnet-0.0.1/data/small.fna
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-12 18:15:53.000000 gtnet-0.0.1/data/small.raw.csv
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-12 18:15:53.000000 gtnet-0.0.1/data/small.tax.0.05.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:16:05.775259 gtnet-0.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-06-12 18:15:53.000000 gtnet-0.0.1/docs/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-12 18:15:53.000000 gtnet-0.0.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:16:05.775259 gtnet-0.0.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)    35955 2023-06-12 18:15:53.000000 gtnet-0.0.1/docs/source/accuracy.png
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-12 18:15:53.000000 gtnet-0.0.1/docs/source/api_docs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9929 2023-06-12 18:15:53.000000 gtnet-0.0.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-12 18:15:53.000000 gtnet-0.0.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-12 18:15:53.000000 gtnet-0.0.1/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-12 18:15:53.000000 gtnet-0.0.1/docs/source/legal.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-12 18:15:53.000000 gtnet-0.0.1/docs/source/performance.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18491 2023-06-12 18:15:53.000000 gtnet-0.0.1/docs/source/runtime.png
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-12 18:15:53.000000 gtnet-0.0.1/docs/source/training.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-12 18:15:53.000000 gtnet-0.0.1/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-06-12 18:15:53.000000 gtnet-0.0.1/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-12 18:15:53.000000 gtnet-0.0.1/fetch_model.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-12 18:15:53.000000 gtnet-0.0.1/license.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-12 18:15:53.000000 gtnet-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-12 18:15:53.000000 gtnet-0.0.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-12 18:15:53.000000 gtnet-0.0.1/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 18:15:53.000000 gtnet-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 18:16:05.787259 gtnet-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:16:05.763258 gtnet-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:16:05.779259 gtnet-0.0.1/src/gtnet/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/classify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:16:05.779259 gtnet-0.0.1/src/gtnet/data/
--rw-r--r--   0 runner    (1001) docker     (123)  5437423 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/data/GCA_000006155.2.fna
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:16:05.787259 gtnet-0.0.1/src/gtnet/deploy_pkg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/deploy_pkg/class.roc.npz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/deploy_pkg/class.score.pt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/deploy_pkg/domain.roc.npz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/deploy_pkg/domain.score.pt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/deploy_pkg/family.roc.npz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/deploy_pkg/family.score.pt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/deploy_pkg/genus.roc.npz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/deploy_pkg/genus.score.pt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/deploy_pkg/last.pt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/deploy_pkg/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/deploy_pkg/order.roc.npz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/deploy_pkg/order.score.pt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/deploy_pkg/phylum.roc.npz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/deploy_pkg/phylum.score.pt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/deploy_pkg/species.roc.npz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/deploy_pkg/species.score.pt
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-12 18:15:53.000000 gtnet-0.0.1/src/gtnet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:16:05.779259 gtnet-0.0.1/src/gtnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-06-12 18:16:05.000000 gtnet-0.0.1/src/gtnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-12 18:16:05.000000 gtnet-0.0.1/src/gtnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 18:16:05.000000 gtnet-0.0.1/src/gtnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 18:16:05.000000 gtnet-0.0.1/src/gtnet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 18:16:05.000000 gtnet-0.0.1/src/gtnet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 18:16:05.000000 gtnet-0.0.1/src/gtnet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:16:05.787259 gtnet-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:15:53.000000 gtnet-0.0.1/tests/test_lca.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:15:53.000000 gtnet-0.0.1/tests/test_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-12 18:15:53.000000 gtnet-0.0.1/tests/test_sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:26.695192 gtnet-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-13 23:00:14.000000 gtnet-0.0.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:26.675191 gtnet-0.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-06-13 23:00:14.000000 gtnet-0.0.2/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-13 23:00:14.000000 gtnet-0.0.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:26.675191 gtnet-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-13 23:00:14.000000 gtnet-0.0.2/.github/workflows/codespell.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-13 23:00:14.000000 gtnet-0.0.2/.github/workflows/deploy_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-13 23:00:14.000000 gtnet-0.0.2/.github/workflows/ruff.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-13 23:00:14.000000 gtnet-0.0.2/.github/workflows/run_coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-13 23:00:14.000000 gtnet-0.0.2/.github/workflows/run_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-13 23:00:14.000000 gtnet-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-13 23:00:14.000000 gtnet-0.0.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-13 23:00:14.000000 gtnet-0.0.2/Legal.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-13 23:00:26.695192 gtnet-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-13 23:00:14.000000 gtnet-0.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:26.683191 gtnet-0.0.2/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  5437423 2023-06-13 23:00:14.000000 gtnet-0.0.2/data/GCA_000006155.2.fna
+-rw-r--r--   0 runner    (1001) docker     (123)    61553 2023-06-13 23:00:14.000000 gtnet-0.0.2/data/small.fna
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-13 23:00:14.000000 gtnet-0.0.2/data/small.raw.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-13 23:00:14.000000 gtnet-0.0.2/data/small.tax.0.05.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:26.683191 gtnet-0.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-06-13 23:00:14.000000 gtnet-0.0.2/docs/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-13 23:00:14.000000 gtnet-0.0.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:26.683191 gtnet-0.0.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)    35955 2023-06-13 23:00:14.000000 gtnet-0.0.2/docs/source/accuracy.png
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-13 23:00:14.000000 gtnet-0.0.2/docs/source/api_docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-06-13 23:00:14.000000 gtnet-0.0.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27508 2023-06-13 23:00:14.000000 gtnet-0.0.2/docs/source/gtnet-favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32999 2023-06-13 23:00:14.000000 gtnet-0.0.2/docs/source/gtnet.png
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-13 23:00:14.000000 gtnet-0.0.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-13 23:00:14.000000 gtnet-0.0.2/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-13 23:00:14.000000 gtnet-0.0.2/docs/source/legal.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-13 23:00:14.000000 gtnet-0.0.2/docs/source/performance.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18491 2023-06-13 23:00:14.000000 gtnet-0.0.2/docs/source/runtime.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-13 23:00:14.000000 gtnet-0.0.2/docs/source/training.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-13 23:00:14.000000 gtnet-0.0.2/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-06-13 23:00:14.000000 gtnet-0.0.2/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-13 23:00:14.000000 gtnet-0.0.2/fetch_model.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-13 23:00:14.000000 gtnet-0.0.2/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-13 23:00:14.000000 gtnet-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-13 23:00:14.000000 gtnet-0.0.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-13 23:00:14.000000 gtnet-0.0.2/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-13 23:00:14.000000 gtnet-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 23:00:26.695192 gtnet-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:26.671190 gtnet-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:26.683191 gtnet-0.0.2/src/gtnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:26.687192 gtnet-0.0.2/src/gtnet/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  5437423 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/data/GCA_000006155.2.fna
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:26.695192 gtnet-0.0.2/src/gtnet/deploy_pkg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/deploy_pkg/class.roc.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/deploy_pkg/class.score.pt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/deploy_pkg/domain.roc.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/deploy_pkg/domain.score.pt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/deploy_pkg/family.roc.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/deploy_pkg/family.score.pt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/deploy_pkg/genus.roc.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/deploy_pkg/genus.score.pt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/deploy_pkg/last.pt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/deploy_pkg/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/deploy_pkg/order.roc.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/deploy_pkg/order.score.pt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/deploy_pkg/phylum.roc.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/deploy_pkg/phylum.score.pt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/deploy_pkg/species.roc.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/deploy_pkg/species.score.pt
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:26.687192 gtnet-0.0.2/src/gtnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-13 23:00:26.000000 gtnet-0.0.2/src/gtnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-13 23:00:26.000000 gtnet-0.0.2/src/gtnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 23:00:26.000000 gtnet-0.0.2/src/gtnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-13 23:00:26.000000 gtnet-0.0.2/src/gtnet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-13 23:00:26.000000 gtnet-0.0.2/src/gtnet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 23:00:26.000000 gtnet-0.0.2/src/gtnet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:26.695192 gtnet-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:14.000000 gtnet-0.0.2/tests/test_lca.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:14.000000 gtnet-0.0.2/tests/test_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-13 23:00:14.000000 gtnet-0.0.2/tests/test_sequence.py
```

### Comparing `gtnet-0.0.1/.github/CODE_OF_CONDUCT.md` & `gtnet-0.0.2/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.1/.github/pull_request_template.md` & `gtnet-0.0.2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.1/.github/workflows/deploy_release.yml` & `gtnet-0.0.2/.github/workflows/deploy_release.yml`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.1/.github/workflows/run_coverage.yml` & `gtnet-0.0.2/.github/workflows/run_coverage.yml`

 * *Files 15% similar despite different names*

```diff
@@ -51,14 +51,17 @@
         run: |
           python -m pip install -e .  # must install in editable mode for coverage to find sources
           python -m pip list
 
       - name: Run tests and generate coverage report
         run: |
           pytest --cov
+          gtnet predict data/small.fna > data/small.raw.test.csv
+          gtnet filter --fpr 0.05 data/small.raw.csv > data/small.tax.test.csv
+          gtnet classify --fpr 0.05 data/small.fna > data/small.tax.test.csv
           python -m coverage xml  # codecov uploader requires xml format
           python -m coverage report -m
 
       - name: Upload coverage to Codecov
         uses: codecov/codecov-action@v3
         with:
           fail_ci_if_error: true
```

### Comparing `gtnet-0.0.1/.github/workflows/run_tests.yml` & `gtnet-0.0.2/.github/workflows/run_tests.yml`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.1/.gitignore` & `gtnet-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.1/.readthedocs.yaml` & `gtnet-0.0.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.1/Legal.txt` & `gtnet-0.0.2/Legal.txt`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.1/README.md` & `gtnet-0.0.2/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,33 @@
+=====
 GTNet
 =====
-The Genome Taxonomy Network for assigning microbial taxonomy to DNA sequences
+The Genome Taxonomy Network for assigning GTDB microbial taxonomy to DNA sequences.
+
+Documentation can be found at https://gtnet.readthedocs.io.
+
+Latest Release
+==============
+
+.. image:: https://badge.fury.io/py/gtnet.svg
+    :target: https://badge.fury.io/py/gtnet
+
+Overall Health
+==============
+
+.. image:: https://codecov.io/gh/exabiome/gtnet/branch/main/graph/badge.svg?token=AFJH59YZ3U
+    :target: https://codecov.io/gh/exabiome/gtnet
+
+.. image:: https://readthedocs.org/projects/hdmf/badge/?version=stable
+    :target: https://hdmf.readthedocs.io/en/stable/?badge=stable
+
+Installation
+============
 
-## Getting started
-Installing GTNet from PyPI
-```bash
-pip install gtnet
-```
-
-Installing GTNet from source
-```bash
-pip install git+https://github.com/exabiome/gtnet.git
-```
-
-## Running GTNet
-Getting taxonomic classifications for all sequences in a Fasta file.
-```bash
-gtnet classify data/small.fna > data/small.tax.csv
-```
-
-### GTNet steps
-GTNet consists of two main steps: 1) get scored predictions of taxonoimc assignments and 2) filter
-scored predictions. The previous command combines these two commands into a single command with a 
-default false-positive rate. The two steps have been separated into two commands for those who
-want to experiment with different false-positive rates.
-
-Getting predictions for all sequences in a Fasta file.
-```bash
-gtnet predict data/small.fna > data/small.tax.raw.csv
-```
-The first time you run `predict`, the model file will be downloaded and stored in the
-same directory that the `gtnet` package is installed in. Therefore, for the this to be successful,
-you must have write privileges on the directory that `gtnet` is installed in.
-
-Filtering predictions 
-```bash
-gtnet filter --fpr 0.05 data/small.tax.raw.csv > data/small.tax.csv
-```
+See the `GTNet documentation <https://gtnet.readthedocs.io/en/stable/installation.html>`_.
 
 LICENSE
 =======
 
 The Genome Taxonomy Network (GTNet) Copyright (c) 2022, The
 Regents of the University of California, through Lawrence Berkeley
 National Laboratory (subject to receipt of any required approvals
@@ -97,9 +84,9 @@
 please contact Berkeley Lab's Intellectual Property Office at
 IPO@lbl.gov.
 
 NOTICE.  This Software was developed under funding from the U.S. Department
 of Energy and the U.S. Government consequently retains certain rights.  As
 such, the U.S. Government has been granted for itself and others acting on
 its behalf a paid-up, nonexclusive, irrevocable, worldwide license in the
-Software to reproduce, distribute copies to the public, prepare derivative 
+Software to reproduce, distribute copies to the public, prepare derivative
 works, and perform publicly and display publicly, and to permit others to do so.
```

### Comparing `gtnet-0.0.1/data/GCA_000006155.2.fna` & `gtnet-0.0.2/data/GCA_000006155.2.fna`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.1/data/small.fna` & `gtnet-0.0.2/data/small.fna`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.1/data/small.raw.csv` & `gtnet-0.0.2/data/small.raw.csv`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.1/docs/CONTRIBUTING.rst` & `gtnet-0.0.2/docs/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.1/docs/Makefile` & `gtnet-0.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.1/docs/source/accuracy.png` & `gtnet-0.0.2/docs/source/accuracy.png`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.1/docs/source/conf.py` & `gtnet-0.0.2/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,32 +132,37 @@
 html_theme_path = [sphinx_rtd_theme.get_html_theme_path()]
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 # html_theme_options = {}
 
+html_theme_options = {
+    'logo_only': True,
+}
+
 # Add any paths that contain custom themes here, relative to this directory.
 # html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
 # html_title = None
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
 # html_short_title = None
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
-# html_logo = None
+html_logo = "gtnet.png"
 
 # The name of an image file (within the static path) to use as favicon of the
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
-# html_favicon = None
+html_favicon = "gtnet-favicon.png"
+
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 # html_static_path = ["_static"]
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
```

### Comparing `gtnet-0.0.1/docs/source/index.rst` & `gtnet-0.0.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.1/docs/source/performance.rst` & `gtnet-0.0.2/docs/source/performance.rst`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.1/docs/source/runtime.png` & `gtnet-0.0.2/docs/source/runtime.png`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.1/docs/source/training.rst` & `gtnet-0.0.2/docs/source/training.rst`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.1/docs/source/usage.rst` & `gtnet-0.0.2/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.1/environment.yml` & `gtnet-0.0.2/environment.yml`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.1/license.txt` & `gtnet-0.0.2/license.txt`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.1/pyproject.toml` & `gtnet-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.1/requirements-dev.txt` & `gtnet-0.0.2/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.1/src/gtnet/classify.py` & `gtnet-0.0.2/src/gtnet/classify.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,16 +16,17 @@
 
     Parameters
     ----------
 
     argv : Namespace, default=sys.argv
         The command-line arguments to use for running this command
     """
-    desc = "Get taxonomic classification for each sequence in a Fasta file."
-    epi = ()
+    desc = "Get filtered taxonomic classification for each sequence in a Fasta file."
+    epi = ("This command will output a taxonomic classification filtered to a specified false-positive rate "
+           "for each sequence")
 
     parser = argparse.ArgumentParser(description=desc, epilog=epi)
     parser.add_argument('fasta', type=str, help='the Fasta files to do taxonomic classification on')
     parser.add_argument('-c', '--n_chunks', type=int, default=DEFAULT_N_CHUNKS,
                         help='the number of sequence chunks to process at a time')
     parser.add_argument('-o', '--output', type=str, default=None, help='the output file to save classifications to')
     check_cuda(parser)
```

### Comparing `gtnet-0.0.1/src/gtnet/data/GCA_000006155.2.fna` & `gtnet-0.0.2/src/gtnet/data/GCA_000006155.2.fna`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.1/src/gtnet/filter.py` & `gtnet-0.0.2/src/gtnet/filter.py`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.1/src/gtnet/main.py` & `gtnet-0.0.2/src/gtnet/main.py`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.1/src/gtnet/predict.py` & `gtnet-0.0.2/src/gtnet/predict.py`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.1/src/gtnet/sequence.py` & `gtnet-0.0.2/src/gtnet/sequence.py`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.1/src/gtnet/utils.py` & `gtnet-0.0.2/src/gtnet/utils.py`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.1/src/gtnet.egg-info/SOURCES.txt` & `gtnet-0.0.2/src/gtnet.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 .gitattributes
 .gitignore
 .readthedocs.yaml
 Legal.txt
-README.md
+README.rst
 environment.yml
 fetch_model.sh
 license.txt
 pyproject.toml
 requirements-dev.txt
 requirements-doc.txt
 requirements.txt
@@ -22,14 +22,16 @@
 data/small.raw.csv
 data/small.tax.0.05.csv
 docs/CONTRIBUTING.rst
 docs/Makefile
 docs/source/accuracy.png
 docs/source/api_docs.rst
 docs/source/conf.py
+docs/source/gtnet-favicon.png
+docs/source/gtnet.png
 docs/source/index.rst
 docs/source/installation.rst
 docs/source/legal.rst
 docs/source/performance.rst
 docs/source/runtime.png
 docs/source/training.rst
 docs/source/usage.rst
```

### Comparing `gtnet-0.0.1/tests/test_sequence.py` & `gtnet-0.0.2/tests/test_sequence.py`

 * *Files identical despite different names*

