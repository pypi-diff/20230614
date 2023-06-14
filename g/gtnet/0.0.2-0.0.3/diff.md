# Comparing `tmp/gtnet-0.0.2.tar.gz` & `tmp/gtnet-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gtnet-0.0.2.tar", last modified: Tue Jun 13 23:00:26 2023, max compression
+gzip compressed data, was "gtnet-0.0.3.tar", last modified: Wed Jun 14 18:38:35 2023, max compression
```

## Comparing `gtnet-0.0.2.tar` & `gtnet-0.0.3.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:26.695192 gtnet-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-13 23:00:14.000000 gtnet-0.0.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:26.675191 gtnet-0.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-06-13 23:00:14.000000 gtnet-0.0.2/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-13 23:00:14.000000 gtnet-0.0.2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:26.675191 gtnet-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-13 23:00:14.000000 gtnet-0.0.2/.github/workflows/codespell.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-13 23:00:14.000000 gtnet-0.0.2/.github/workflows/deploy_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-13 23:00:14.000000 gtnet-0.0.2/.github/workflows/ruff.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-13 23:00:14.000000 gtnet-0.0.2/.github/workflows/run_coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-13 23:00:14.000000 gtnet-0.0.2/.github/workflows/run_tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-13 23:00:14.000000 gtnet-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-13 23:00:14.000000 gtnet-0.0.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-13 23:00:14.000000 gtnet-0.0.2/Legal.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-13 23:00:26.695192 gtnet-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-13 23:00:14.000000 gtnet-0.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:26.683191 gtnet-0.0.2/data/
--rw-r--r--   0 runner    (1001) docker     (123)  5437423 2023-06-13 23:00:14.000000 gtnet-0.0.2/data/GCA_000006155.2.fna
--rw-r--r--   0 runner    (1001) docker     (123)    61553 2023-06-13 23:00:14.000000 gtnet-0.0.2/data/small.fna
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-13 23:00:14.000000 gtnet-0.0.2/data/small.raw.csv
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-13 23:00:14.000000 gtnet-0.0.2/data/small.tax.0.05.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:26.683191 gtnet-0.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-06-13 23:00:14.000000 gtnet-0.0.2/docs/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-13 23:00:14.000000 gtnet-0.0.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:26.683191 gtnet-0.0.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)    35955 2023-06-13 23:00:14.000000 gtnet-0.0.2/docs/source/accuracy.png
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-13 23:00:14.000000 gtnet-0.0.2/docs/source/api_docs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-06-13 23:00:14.000000 gtnet-0.0.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    27508 2023-06-13 23:00:14.000000 gtnet-0.0.2/docs/source/gtnet-favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)    32999 2023-06-13 23:00:14.000000 gtnet-0.0.2/docs/source/gtnet.png
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-13 23:00:14.000000 gtnet-0.0.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-13 23:00:14.000000 gtnet-0.0.2/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-13 23:00:14.000000 gtnet-0.0.2/docs/source/legal.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-13 23:00:14.000000 gtnet-0.0.2/docs/source/performance.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18491 2023-06-13 23:00:14.000000 gtnet-0.0.2/docs/source/runtime.png
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-13 23:00:14.000000 gtnet-0.0.2/docs/source/training.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-13 23:00:14.000000 gtnet-0.0.2/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-06-13 23:00:14.000000 gtnet-0.0.2/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-13 23:00:14.000000 gtnet-0.0.2/fetch_model.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-13 23:00:14.000000 gtnet-0.0.2/license.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-13 23:00:14.000000 gtnet-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-13 23:00:14.000000 gtnet-0.0.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-13 23:00:14.000000 gtnet-0.0.2/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-13 23:00:14.000000 gtnet-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 23:00:26.695192 gtnet-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:26.671190 gtnet-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:26.683191 gtnet-0.0.2/src/gtnet/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/classify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:26.687192 gtnet-0.0.2/src/gtnet/data/
--rw-r--r--   0 runner    (1001) docker     (123)  5437423 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/data/GCA_000006155.2.fna
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:26.695192 gtnet-0.0.2/src/gtnet/deploy_pkg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/deploy_pkg/class.roc.npz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/deploy_pkg/class.score.pt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/deploy_pkg/domain.roc.npz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/deploy_pkg/domain.score.pt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/deploy_pkg/family.roc.npz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/deploy_pkg/family.score.pt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/deploy_pkg/genus.roc.npz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/deploy_pkg/genus.score.pt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/deploy_pkg/last.pt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/deploy_pkg/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/deploy_pkg/order.roc.npz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/deploy_pkg/order.score.pt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/deploy_pkg/phylum.roc.npz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/deploy_pkg/phylum.score.pt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/deploy_pkg/species.roc.npz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/deploy_pkg/species.score.pt
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-13 23:00:14.000000 gtnet-0.0.2/src/gtnet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:26.687192 gtnet-0.0.2/src/gtnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-13 23:00:26.000000 gtnet-0.0.2/src/gtnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-13 23:00:26.000000 gtnet-0.0.2/src/gtnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 23:00:26.000000 gtnet-0.0.2/src/gtnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-13 23:00:26.000000 gtnet-0.0.2/src/gtnet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-13 23:00:26.000000 gtnet-0.0.2/src/gtnet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 23:00:26.000000 gtnet-0.0.2/src/gtnet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:26.695192 gtnet-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:14.000000 gtnet-0.0.2/tests/test_lca.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:00:14.000000 gtnet-0.0.2/tests/test_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-13 23:00:14.000000 gtnet-0.0.2/tests/test_sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:35.765445 gtnet-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-14 18:38:25.000000 gtnet-0.0.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:35.749445 gtnet-0.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-06-14 18:38:25.000000 gtnet-0.0.3/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-14 18:38:25.000000 gtnet-0.0.3/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:35.749445 gtnet-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-14 18:38:25.000000 gtnet-0.0.3/.github/workflows/codespell.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-14 18:38:25.000000 gtnet-0.0.3/.github/workflows/deploy_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-14 18:38:25.000000 gtnet-0.0.3/.github/workflows/ruff.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-14 18:38:25.000000 gtnet-0.0.3/.github/workflows/run_coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-14 18:38:25.000000 gtnet-0.0.3/.github/workflows/run_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-14 18:38:25.000000 gtnet-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-14 18:38:25.000000 gtnet-0.0.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-14 18:38:25.000000 gtnet-0.0.3/Legal.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-14 18:38:35.765445 gtnet-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-14 18:38:25.000000 gtnet-0.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:35.757445 gtnet-0.0.3/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  5437423 2023-06-14 18:38:26.000000 gtnet-0.0.3/data/GCA_000006155.2.fna
+-rw-r--r--   0 runner    (1001) docker     (123)    61553 2023-06-14 18:38:26.000000 gtnet-0.0.3/data/small.fna
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-14 18:38:26.000000 gtnet-0.0.3/data/small.raw.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-14 18:38:26.000000 gtnet-0.0.3/data/small.tax.0.05.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:35.757445 gtnet-0.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-06-14 18:38:26.000000 gtnet-0.0.3/docs/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-14 18:38:26.000000 gtnet-0.0.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:35.757445 gtnet-0.0.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)    35955 2023-06-14 18:38:26.000000 gtnet-0.0.3/docs/source/accuracy.png
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-14 18:38:26.000000 gtnet-0.0.3/docs/source/api_docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-06-14 18:38:26.000000 gtnet-0.0.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27508 2023-06-14 18:38:26.000000 gtnet-0.0.3/docs/source/gtnet-favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32999 2023-06-14 18:38:26.000000 gtnet-0.0.3/docs/source/gtnet.png
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-14 18:38:26.000000 gtnet-0.0.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-14 18:38:26.000000 gtnet-0.0.3/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-14 18:38:26.000000 gtnet-0.0.3/docs/source/legal.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-14 18:38:26.000000 gtnet-0.0.3/docs/source/performance.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18491 2023-06-14 18:38:26.000000 gtnet-0.0.3/docs/source/runtime.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-14 18:38:26.000000 gtnet-0.0.3/docs/source/training.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-14 18:38:26.000000 gtnet-0.0.3/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-06-14 18:38:26.000000 gtnet-0.0.3/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-14 18:38:26.000000 gtnet-0.0.3/fetch_model.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-06-14 18:38:26.000000 gtnet-0.0.3/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-14 18:38:26.000000 gtnet-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-14 18:38:26.000000 gtnet-0.0.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-14 18:38:26.000000 gtnet-0.0.3/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-14 18:38:26.000000 gtnet-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 18:38:35.765445 gtnet-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:35.749445 gtnet-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:35.757445 gtnet-0.0.3/src/gtnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:35.757445 gtnet-0.0.3/src/gtnet/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  5437423 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/data/GCA_000006155.2.fna
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:35.765445 gtnet-0.0.3/src/gtnet/deploy_pkg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/deploy_pkg/class.roc.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/deploy_pkg/class.score.pt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/deploy_pkg/domain.roc.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/deploy_pkg/domain.score.pt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/deploy_pkg/family.roc.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/deploy_pkg/family.score.pt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/deploy_pkg/genus.roc.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/deploy_pkg/genus.score.pt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/deploy_pkg/last.pt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/deploy_pkg/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/deploy_pkg/order.roc.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/deploy_pkg/order.score.pt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/deploy_pkg/phylum.roc.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/deploy_pkg/phylum.score.pt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/deploy_pkg/species.roc.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/deploy_pkg/species.score.pt
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-06-14 18:38:26.000000 gtnet-0.0.3/src/gtnet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:35.757445 gtnet-0.0.3/src/gtnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-14 18:38:35.000000 gtnet-0.0.3/src/gtnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-14 18:38:35.000000 gtnet-0.0.3/src/gtnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 18:38:35.000000 gtnet-0.0.3/src/gtnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-14 18:38:35.000000 gtnet-0.0.3/src/gtnet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-14 18:38:35.000000 gtnet-0.0.3/src/gtnet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-14 18:38:35.000000 gtnet-0.0.3/src/gtnet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:35.765445 gtnet-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:26.000000 gtnet-0.0.3/tests/test_lca.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:38:26.000000 gtnet-0.0.3/tests/test_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-14 18:38:26.000000 gtnet-0.0.3/tests/test_sequence.py
```

### Comparing `gtnet-0.0.2/.github/CODE_OF_CONDUCT.md` & `gtnet-0.0.3/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.2/.github/pull_request_template.md` & `gtnet-0.0.3/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.2/.github/workflows/deploy_release.yml` & `gtnet-0.0.3/.github/workflows/deploy_release.yml`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.2/.github/workflows/run_coverage.yml` & `gtnet-0.0.3/.github/workflows/run_coverage.yml`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.2/.github/workflows/run_tests.yml` & `gtnet-0.0.3/.github/workflows/run_tests.yml`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.2/.gitignore` & `gtnet-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.2/.readthedocs.yaml` & `gtnet-0.0.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.2/Legal.txt` & `gtnet-0.0.3/Legal.txt`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.2/PKG-INFO` & `gtnet-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtnet
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for running Genome Taxonomy Network predictions
 Author-email: Andrew Tritt <ajtritt@lbl.gov>, Ryan Ly <rly@lbl.gov>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/exabiome/gtnet
 Project-URL: Bug Tracker, https://github.com/exabiome/gtnet/issues
 Keywords: python,microbiome,microbial-taxonomy,cross-platform,open-data,data-format,open-source,open-science,reproducible-research,machine-learning
 Classifier: Programming Language :: Python
```

### Comparing `gtnet-0.0.2/README.rst` & `gtnet-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.2/data/GCA_000006155.2.fna` & `gtnet-0.0.3/data/GCA_000006155.2.fna`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.2/data/small.fna` & `gtnet-0.0.3/data/small.fna`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.2/data/small.raw.csv` & `gtnet-0.0.3/data/small.raw.csv`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.2/docs/CONTRIBUTING.rst` & `gtnet-0.0.3/docs/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.2/docs/Makefile` & `gtnet-0.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.2/docs/source/accuracy.png` & `gtnet-0.0.3/docs/source/accuracy.png`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.2/docs/source/conf.py` & `gtnet-0.0.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.2/docs/source/gtnet-favicon.png` & `gtnet-0.0.3/docs/source/gtnet-favicon.png`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.2/docs/source/gtnet.png` & `gtnet-0.0.3/docs/source/gtnet.png`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.2/docs/source/index.rst` & `gtnet-0.0.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.2/docs/source/performance.rst` & `gtnet-0.0.3/docs/source/performance.rst`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.2/docs/source/runtime.png` & `gtnet-0.0.3/docs/source/runtime.png`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.2/docs/source/training.rst` & `gtnet-0.0.3/docs/source/training.rst`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.2/docs/source/usage.rst` & `gtnet-0.0.3/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.2/environment.yml` & `gtnet-0.0.3/environment.yml`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.2/pyproject.toml` & `gtnet-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.2/requirements-dev.txt` & `gtnet-0.0.3/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.2/src/gtnet/classify.py` & `gtnet-0.0.3/src/gtnet/classify.py`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.2/src/gtnet/data/GCA_000006155.2.fna` & `gtnet-0.0.3/src/gtnet/data/GCA_000006155.2.fna`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.2/src/gtnet/filter.py` & `gtnet-0.0.3/src/gtnet/filter.py`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.2/src/gtnet/main.py` & `gtnet-0.0.3/src/gtnet/main.py`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.2/src/gtnet/predict.py` & `gtnet-0.0.3/src/gtnet/predict.py`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.2/src/gtnet/sequence.py` & `gtnet-0.0.3/src/gtnet/sequence.py`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.2/src/gtnet/utils.py` & `gtnet-0.0.3/src/gtnet/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import glob
 import hashlib
+from importlib.resources import files
 import json
 import logging
 import os
 import sys
 import urllib
 import warnings
 import zipfile
 
 import numpy as np
-from pkg_resources import resource_filename
 import torch
 import torch.nn as nn
 
 
 def parse_logger(string):
     if not string:
         ret = logging.getLogger()
@@ -36,23 +36,23 @@
 
     _deploy_pkg_url = "https://osf.io/download/mwgb9/"
 
     _checksum = "0245fcf825bfe4de0770fcb46798ca90"
 
     @classmethod
     def check_pkg(cls):
-        deploy_dir = resource_filename(__name__, 'deploy_pkg')
+        deploy_dir = files(__package__).joinpath('deploy_pkg')
         total = 0
         for path in glob.glob(f"{deploy_dir}/*"):
             total += os.path.getsize(path)
         if total == 0:
             msg = ("Downloading GTNet deployment package. This will only happen on the first invocation "
                    "of gtnet predict or gtnet classify")
             warnings.warn(msg)
-            zip_path = resource_filename(__name__, 'deploy_pkg.zip')
+            zip_path = files(__package__).joinpath('deploy_pkg.zip')
             urllib.request.urlretrieve(cls._deploy_pkg_url, zip_path)
             dl_checksum = hashlib.md5(open(zip_path,'rb').read()).hexdigest()
             if dl_checksum != cls._checksum:
                 raise ValueError(f"Downloaded deployment package {zip_path} does not match expected checksum")
             with zipfile.ZipFile(zip_path) as zip_ref:
                 zip_ref.extractall(os.path.dirname(deploy_dir))
             os.remove(zip_path)
```

### Comparing `gtnet-0.0.2/src/gtnet.egg-info/PKG-INFO` & `gtnet-0.0.3/src/gtnet.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtnet
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for running Genome Taxonomy Network predictions
 Author-email: Andrew Tritt <ajtritt@lbl.gov>, Ryan Ly <rly@lbl.gov>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/exabiome/gtnet
 Project-URL: Bug Tracker, https://github.com/exabiome/gtnet/issues
 Keywords: python,microbiome,microbial-taxonomy,cross-platform,open-data,data-format,open-source,open-science,reproducible-research,machine-learning
 Classifier: Programming Language :: Python
```

### Comparing `gtnet-0.0.2/src/gtnet.egg-info/SOURCES.txt` & `gtnet-0.0.3/src/gtnet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gtnet-0.0.2/tests/test_sequence.py` & `gtnet-0.0.3/tests/test_sequence.py`

 * *Files identical despite different names*

