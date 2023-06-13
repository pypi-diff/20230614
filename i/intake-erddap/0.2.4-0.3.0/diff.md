# Comparing `tmp/intake-erddap-0.2.4.tar.gz` & `tmp/intake-erddap-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intake-erddap-0.2.4.tar", last modified: Thu Jan  5 18:28:53 2023, max compression
+gzip compressed data, was "intake-erddap-0.3.0.tar", last modified: Tue Jun 13 22:22:37 2023, max compression
```

## Comparing `intake-erddap-0.2.4.tar` & `intake-erddap-0.3.0.tar`

### file list

```diff
@@ -1,69 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 18:28:53.063310 intake-erddap-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 18:28:53.051310 intake-erddap-0.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 18:28:53.059310 intake-erddap-0.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/.github/workflows/linting.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-01-05 18:28:53.063310 intake-erddap-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/PREV-LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 18:28:53.059310 intake-erddap-0.2.4/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/ci/environment-py3.10.yml
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/ci/environment-py3.8.yml
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/ci/environment-py3.9.yml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 18:28:53.059310 intake-erddap-0.2.4/conda/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/conda/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/dev-environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 18:28:53.059310 intake-erddap-0.2.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/docs/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 18:28:53.059310 intake-erddap-0.2.4/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/docs/examples/wave-height.md
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/docs/examples.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 18:28:53.059310 intake-erddap-0.2.4/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/docs/images/github-mark-white.svg
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/docs/images/github-mark.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 18:28:53.059310 intake-erddap-0.2.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    11523 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/examples/intake-erddap.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 18:28:53.059310 intake-erddap-0.2.4/intake_erddap/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/intake_erddap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-05 18:28:52.000000 intake-erddap-0.2.4/intake_erddap/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/intake_erddap/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    14196 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/intake_erddap/erddap.py
--rw-r--r--   0 runner    (1001) docker     (123)    17463 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/intake_erddap/erddap_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/intake_erddap/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/intake_erddap/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 18:28:53.059310 intake-erddap-0.2.4/intake_erddap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-01-05 18:28:52.000000 intake-erddap-0.2.4/intake_erddap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-01-05 18:28:53.000000 intake-erddap-0.2.4/intake_erddap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 18:28:52.000000 intake-erddap-0.2.4/intake_erddap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-01-05 18:28:52.000000 intake-erddap-0.2.4/intake_erddap.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 18:28:52.000000 intake-erddap-0.2.4/intake_erddap.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-01-05 18:28:52.000000 intake-erddap-0.2.4/intake_erddap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-05 18:28:52.000000 intake-erddap-0.2.4/intake_erddap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-01-05 18:28:53.063310 intake-erddap-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 18:28:53.063310 intake-erddap-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/tests/cat.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/tests/test_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 18:28:53.063310 intake-erddap-0.2.4/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     9327 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/tests/test_data/tabledap_metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)    20541 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/tests/test_erddap_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/tests/test_erddap_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-01-05 18:28:45.000000 intake-erddap-0.2.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:22:37.359988 intake-erddap-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:22:37.351988 intake-erddap-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:22:37.359988 intake-erddap-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/.github/workflows/linting.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-06-13 22:22:37.359988 intake-erddap-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/PREV-LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:22:37.355988 intake-erddap-0.3.0/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/ci/environment-py3.10.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/ci/environment-py3.8.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/ci/environment-py3.9.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:22:37.359988 intake-erddap-0.3.0/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/conda/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/dev-environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:22:37.359988 intake-erddap-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/docs/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:22:37.359988 intake-erddap-0.3.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/docs/examples/wave-height.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/docs/examples.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:22:37.359988 intake-erddap-0.3.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/docs/images/github-mark-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/docs/images/github-mark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:22:37.359988 intake-erddap-0.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    11523 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/examples/intake-erddap.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:22:37.359988 intake-erddap-0.3.0/intake_erddap/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/intake_erddap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-13 22:22:37.000000 intake-erddap-0.3.0/intake_erddap/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/intake_erddap/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17853 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/intake_erddap/erddap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18902 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/intake_erddap/erddap_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/intake_erddap/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/intake_erddap/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:22:37.359988 intake-erddap-0.3.0/intake_erddap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-06-13 22:22:37.000000 intake-erddap-0.3.0/intake_erddap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-13 22:22:37.000000 intake-erddap-0.3.0/intake_erddap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 22:22:37.000000 intake-erddap-0.3.0/intake_erddap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-13 22:22:37.000000 intake-erddap-0.3.0/intake_erddap.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 22:22:37.000000 intake-erddap-0.3.0/intake_erddap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-13 22:22:37.000000 intake-erddap-0.3.0/intake_erddap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 22:22:37.000000 intake-erddap-0.3.0/intake_erddap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-13 22:22:37.359988 intake-erddap-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:22:37.359988 intake-erddap-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/tests/cat.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/tests/test_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:22:37.359988 intake-erddap-0.3.0/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     9327 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/tests/test_data/tabledap_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20541 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/tests/test_erddap_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/tests/test_erddap_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-06-13 22:22:29.000000 intake-erddap-0.3.0/tests/test_utils.py
```

### Comparing `intake-erddap-0.2.4/.github/workflows/test.yaml` & `intake-erddap-0.3.0/.github/workflows/test.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,16 @@
           # Increase this value to reset cache if ci/environment.yml has not changed
           CACHE_NUMBER: 0
         with:
           path: ~/conda_pkgs_dir
           key: ${{ runner.os }}-conda-${{ env.CACHE_NUMBER }}-${{ matrix.python-version}}-${{ hashFiles('ci/environment-py${{ matrix.python-version }}.yml') }}
       - uses: conda-incubator/setup-miniconda@v2
         with:
-          mamba-version: "*" # activate this to build with mamba.
+          python-version: ${{ matrix.python-version }}
+          miniforge-variant: Mambaforge
           channels: conda-forge, defaults # These need to be specified to use mamba
           channel-priority: true
           environment-file: ci/environment-py${{ matrix.python-version }}.yml
 
           activate-environment: test-env
           use-only-tar-bz2: true # IMPORTANT: This needs to be set for caching to work properly!
```

### Comparing `intake-erddap-0.2.4/.gitignore` & `intake-erddap-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `intake-erddap-0.2.4/.pre-commit-config.yaml` & `intake-erddap-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `intake-erddap-0.2.4/LICENSE` & `intake-erddap-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `intake-erddap-0.2.4/PKG-INFO` & `intake-erddap-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intake-erddap
-Version: 0.2.4
+Version: 0.3.0
 Summary: ERDDAP plugin for Intake
 Home-page: https://github.com/axiom-data-science/intake-erddap
 Maintainer: Axiom Data Science
 Maintainer-email: dev@axds.co
 License: BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `intake-erddap-0.2.4/PREV-LICENSE` & `intake-erddap-0.3.0/PREV-LICENSE`

 * *Files identical despite different names*

### Comparing `intake-erddap-0.2.4/README.md` & `intake-erddap-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `intake-erddap-0.2.4/conda/meta.yaml` & `intake-erddap-0.3.0/conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `intake-erddap-0.2.4/docs/Makefile` & `intake-erddap-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `intake-erddap-0.2.4/docs/api.rst` & `intake-erddap-0.3.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `intake-erddap-0.2.4/docs/conf.py` & `intake-erddap-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `intake-erddap-0.2.4/docs/environment.yml` & `intake-erddap-0.3.0/docs/environment.yml`

 * *Files 11% similar despite different names*

```diff
@@ -28,14 +28,15 @@
    - cartopy
    - pip
    - recommonmark
    - pip:
      - git+https://github.com/intake/intake
      - intake-parquet
      - intake-xarray
+     - intake-erddap
     #  - "dask[complete]"
      - docrep<=0.2.7
      - furo
      - nbsphinx>=0.8.7
      - jupyter_client
      - myst-nb
      - sphinx-copybutton
```

### Comparing `intake-erddap-0.2.4/docs/examples/wave-height.md` & `intake-erddap-0.3.0/docs/examples/wave-height.md`

 * *Files identical despite different names*

### Comparing `intake-erddap-0.2.4/docs/examples.rst` & `intake-erddap-0.3.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `intake-erddap-0.2.4/docs/images/github-mark-white.svg` & `intake-erddap-0.3.0/docs/images/github-mark-white.svg`

 * *Files identical despite different names*

### Comparing `intake-erddap-0.2.4/docs/images/github-mark.svg` & `intake-erddap-0.3.0/docs/images/github-mark.svg`

 * *Files identical despite different names*

### Comparing `intake-erddap-0.2.4/docs/index.rst` & `intake-erddap-0.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `intake-erddap-0.2.4/examples/intake-erddap.ipynb` & `intake-erddap-0.3.0/examples/intake-erddap.ipynb`

 * *Files identical despite different names*

### Comparing `intake-erddap-0.2.4/intake_erddap/cache.py` & `intake-erddap-0.3.0/intake_erddap/cache.py`

 * *Files identical despite different names*

### Comparing `intake-erddap-0.2.4/intake_erddap/erddap.py` & `intake-erddap-0.3.0/intake_erddap/erddap.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Source implementations for intake-erddap."""
 import typing
 
 from logging import getLogger
 from typing import List, Optional, Tuple, Type, Union
 
+import cf_pandas  # noqa: F401
+import fsspec
 import numpy as np
 import pandas as pd
 import requests
 import xarray as xr
 
 from erddapy import ERDDAP
 from intake.source import base
@@ -42,14 +44,17 @@
     metadata : dict
     erddap_client : class, optional
         The client object to use for connections to ERDDAP. Must conform to
         the `erddapy.ERDDAP` interface.
     http_client : class, optional
         The client object to use for HTTP requests. Must conform to the
         `requests` interface.
+    open_kwargs : dict, optional
+        Keyword arguments to pass on to the open function like `e.to_pandas`
+        for a DataFrame. For example, {"parse_dates": True}
 
     Note
     ----
     Caches entire dataframe in memory.
     """
 
     name = "erddap"
@@ -62,14 +67,15 @@
         dataset_id: str,
         protocol: str,
         variables: List[str] = None,
         constraints: dict = None,
         metadata: dict = None,
         erddap_client: Optional[Type[ERDDAP]] = None,
         http_client: Optional[Type] = None,
+        open_kwargs: dict = None,
     ):
         variables = variables or []
         constraints = constraints or {}
         metadata = metadata or {}
 
         self._init_args = {
             "dataset_id": dataset_id,
@@ -81,14 +87,15 @@
 
         self._dataset_id = dataset_id
         self._protocol = protocol
         self._variables = variables
         self._constraints = constraints
         self._erddap_client = erddap_client or ERDDAP
         self._http = http_client or requests
+        self.open_kwargs = open_kwargs or {}
 
         super(ERDDAPSource, self).__init__(metadata=metadata)
 
     def get_client(self) -> ERDDAP:
         """Return an initialized ERDDAP Client."""
         e = self._erddap_client(server=self._server)
         e.protocol = self._protocol
@@ -122,14 +129,26 @@
         A class that implements an interface like erdappy's ERDDAP class. The
         source will rely on this client to interface with ERDDAP for most
         requests.
     http_client : module or object, optional
         An object or module that implements an HTTP Client similar to request's
         interface. The source will use this object to make HTTP requests to
         ERDDAP in some cases.
+    mask_failed_qartod : bool, False
+        WARNING ALPHA FEATURE. If True and `*_qc_agg` columns associated with
+        data columns are available, data values associated with QARTOD flags
+        other than 1 and 2 will be nan'ed out. Has not been thoroughly tested.
+    dropna : bool, False.
+        WARNING ALPHA FEATURE. If True, rows with data columns of nans will be
+        dropped from data frame. Has not been thoroughly tested.
+    cache_kwargs : dict, optional
+        WARNING ALPHA FEATURE. If you want to have the data you access stored
+        locally in a cache, use this keyword to input a dictionary of keywords.
+        The cache is set up using ``fsspec``'s simple cache. Example configuration
+        is ``cache_kwargs=dict(cache_storage="/tmp/fnames/", same_names=True)``.
 
     Examples
     --------
     Sources are normally returned from a catalog object, but a source can be instantiated directly:
 
     >>> source = TableDAPSource("https://erddap.senors.axds.co/erddap",
     ... "gov_usgs_waterdata_441759103261203")
@@ -156,18 +175,29 @@
     """
 
     name = "tabledap"
     version = __version__
     container = "dataframe"
     partition_access = True
 
-    def __init__(self, server: str, *args, **kwargs):
+    def __init__(
+        self,
+        server: str,
+        mask_failed_qartod: bool = False,
+        dropna: bool = False,
+        cache_kwargs: Optional[dict] = None,
+        *args,
+        **kwargs,
+    ):
         self._server = server
         self._dataframe: Optional[pd.DataFrame] = None
         self._dataset_metadata: Optional[dict] = None
+        self._mask_failed_qartod = mask_failed_qartod
+        self._dropna = dropna
+        self._cache_kwargs = cache_kwargs
         kwargs.pop("protocol", None)
         # https://github.com/python/mypy/issues/6799
         super().__init__(*args, protocol="tabledap", **kwargs)  # type: ignore
 
     def _get_schema(self) -> base.Schema:
         if self._dataframe is None:
             # TODO: could do partial read with chunksize to get likely schema from
@@ -194,15 +224,72 @@
         return self._get_partition()
 
     def _close(self):
         self._dataframe = None
 
     def _load(self):
         e = self.get_client()
-        self._dataframe: pd.DataFrame = e.to_pandas()
+        if self._cache_kwargs is not None:
+            if "response" in self.open_kwargs:
+                response = self.open_kwargs["response"]
+                self.open_kwargs.pop("response")
+                url = e.get_download_url(response=response)
+            else:
+                url = e.get_download_url(response=response)
+
+            with fsspec.open(f"simplecache::{url}", **self._cache_kwargs) as f:
+                self._dataframe: pd.DataFrame = pd.read_csv(f, **self.open_kwargs)
+        else:
+            self._dataframe: pd.DataFrame = e.to_pandas(
+                requests_kwargs={"timeout": 60}, **self.open_kwargs
+            )
+        if self._mask_failed_qartod:
+            self.run_mask_failed_qartod()
+        if self._dropna:
+            self.run_dropna()
+
+    @property
+    def data_cols(self):
+        """Columns that are not axes, coordinates, nor qc_agg columns."""
+
+        # find data columns which are what we'll use in the final step to drop nan's
+        # don't include dimension/coordinates-type columns (dimcols) nor qc_agg columns (qccols)
+        dimcols = self._dataframe.cf.axes_cols + self._dataframe.cf.coordinates_cols
+        qccols = list(
+            self._dataframe.columns[self._dataframe.columns.str.contains("_qc_agg")]
+        )
+
+        datacols = [
+            col for col in self._dataframe.columns if col not in dimcols + qccols
+        ]
+
+        return datacols
+
+    def run_mask_failed_qartod(self):
+        """Nan data values for which corresponding qc_agg columns is not equal to 1 or 2.
+
+        To get this to work you may need to specify the "qc_agg" columns to come along specifically
+        in the variables input.
+        """
+
+        # if a data column has an associated qc column, use it to weed out bad data by
+        # setting it to nan.
+        for datacol in self.data_cols:
+            qccol = f"{datacol}_qc_agg"
+            if qccol in self._dataframe.columns:
+                self._dataframe.loc[
+                    ~self._dataframe[qccol].isin([1, 2]), datacol
+                ] = pd.NA
+                self._dataframe.drop(columns=[qccol], inplace=True)
+
+    def run_dropna(self):
+        """Drop nan rows based on the data columns."""
+        self._dataframe = self._dataframe.dropna(subset=self.data_cols).reset_index(
+            drop=True
+        )
 
     def _get_dataset_metadata(self) -> dict:
         """Fetch and return the metadata document for the dataset."""
         url = f"{self._server}/info/{self._dataset_id}/index.json"
         resp = self._http.get(url)
         resp.raise_for_status()
         metadata: dict = {"variables": {}}
```

### Comparing `intake-erddap-0.2.4/intake_erddap/erddap_cat.py` & `intake-erddap-0.3.0/intake_erddap/erddap_cat.py`

 * *Files 10% similar despite different names*

```diff
@@ -98,14 +98,26 @@
     query_type : str, default "union"
         Specifies how the catalog should apply the query parameters. Choices are
         ``"union"`` or ``"intersection"``. If the ``query_type`` is set to
         ``"intersection"``, then the set of results will be the intersection of
         each individual query made to ERDDAP. This is equivalent to a logical
         AND of the results. If the value is ``"union"`` then the results will be
         the union of each resulting dataset. This is equivalent to a logical OR.
+    mask_failed_qartod : bool, False
+        WARNING ALPHA FEATURE. If True and `*_qc_agg` columns associated with
+        data columns are available, data values associated with QARTOD flags
+        other than 1 and 2 will be nan'ed out. Has not been thoroughly tested.
+    dropna : bool, False.
+        WARNING ALPHA FEATURE. If True, rows with data columns of nans will be
+        dropped from data frame. Has not been thoroughly tested.
+    cache_kwargs : dict, optional
+        WARNING ALPHA FEATURE. If you want to have the data you access stored
+        locally in a cache, use this keyword to input a dictionary of keywords.
+        The cache is set up using ``fsspec``'s simple cache. Example configuration
+        is ``cache_kwargs=dict(cache_storage="/tmp/fnames/", same_names=True)``.
 
     Attributes
     ----------
     search_url : str
         If a search is performed on the ERDDAP server, the search url is saved as an attribute.
     server : str
         The Base URL of the ERDDAP instance.
@@ -129,27 +141,35 @@
         category_search: Optional[Tuple[str, str]] = None,
         erddap_client: Optional[Type[ERDDAP]] = None,
         use_source_constraints: bool = True,
         protocol: str = "tabledap",
         metadata: dict = None,
         query_type: str = "union",
         cache_period: Optional[Union[int, float]] = 500,
+        open_kwargs: dict = None,
+        mask_failed_qartod: bool = False,
+        dropna: bool = False,
+        cache_kwargs: Optional[dict] = None,
         **kwargs,
     ):
         if server.endswith("/"):
             server = server[:-1]
         self._erddap_client = erddap_client or ERDDAP
         self._entries: Dict[str, LocalCatalogEntry] = {}
         self._use_source_constraints = use_source_constraints
         self._protocol = protocol
         self._dataset_metadata: Optional[Mapping[str, dict]] = None
         self._query_type = query_type
         self.server = server
         self.search_url = None
         self.cache_store = CacheStore(cache_period=cache_period)
+        self.open_kwargs = open_kwargs or {}
+        self._mask_failed_qartod = mask_failed_qartod
+        self._dropna = dropna
+        self._cache_kwargs = cache_kwargs
 
         if kwargs_search is not None:
             checks = [
                 ["min_lon", "max_lon", "min_lat", "max_lat"],
                 ["min_time", "max_time"],
             ]
             for check in checks:
@@ -405,16 +425,24 @@
 
             description = "ERDDAP dataset_id %s from %s" % (dataset_id, self.server)
             args = {
                 "server": self.server,
                 "dataset_id": dataset_id,
                 "protocol": self._protocol,
                 "constraints": {},
+                "open_kwargs": self.open_kwargs,
             }
             if self._protocol == "tabledap":
+                args.update(
+                    {
+                        "mask_failed_qartod": self._mask_failed_qartod,
+                        "dropna": self._dropna,
+                        "cache_kwargs": self._cache_kwargs,
+                    }
+                )
                 args["constraints"].update(self._get_tabledap_constraints())
 
             metadata = all_metadata.get(dataset_id, {})
 
             entry = LocalCatalogEntry(
                 name=dataset_id,
                 description=description,
```

### Comparing `intake-erddap-0.2.4/intake_erddap/utils.py` & `intake-erddap-0.3.0/intake_erddap/utils.py`

 * *Files identical despite different names*

### Comparing `intake-erddap-0.2.4/intake_erddap.egg-info/PKG-INFO` & `intake-erddap-0.3.0/intake_erddap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intake-erddap
-Version: 0.2.4
+Version: 0.3.0
 Summary: ERDDAP plugin for Intake
 Home-page: https://github.com/axiom-data-science/intake-erddap
 Maintainer: Axiom Data Science
 Maintainer-email: dev@axds.co
 License: BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `intake-erddap-0.2.4/intake_erddap.egg-info/SOURCES.txt` & `intake-erddap-0.3.0/intake_erddap.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,20 @@
 MANIFEST.in
 PREV-LICENSE
 README.md
 codecov.yml
 dev-environment.yml
 environment.yml
 pyproject.toml
-readthedocs.yml
 requirements.txt
 setup.cfg
 setup.py
 ./codecov.yml
 ./dev-environment.yml
 ./environment.yml
-./readthedocs.yml
 ./ci/environment-py3.10.yml
 ./ci/environment-py3.8.yml
 ./ci/environment-py3.9.yml
 ./docs/environment.yml
 .github/workflows/linting.yaml
 .github/workflows/release.yaml
 .github/workflows/test.yaml
```

### Comparing `intake-erddap-0.2.4/pyproject.toml` & `intake-erddap-0.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 fail-under = 95
 exclude = ["setup.py", "docs", "tests"]
 verbose = 1
 quiet = false
 color = true
 
 [tool.isort]
-known_third_party = ["appdirs", "cf_pandas", "dask", "erddapy", "intake", "numpy", "pandas", "pkg_resources", "pytest", "requests", "setuptools", "xarray"]
+known_third_party = ["appdirs", "cf_pandas", "dask", "erddapy", "fsspec", "intake", "numpy", "pandas", "pkg_resources", "pytest", "requests", "setuptools", "xarray"]
 skip_glob = ["docs/*", "docs/**/*.py"]
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "-v"
 # only test the root level, otherwise it picks up the tests of the project template
 testpaths = [
```

### Comparing `intake-erddap-0.2.4/setup.py` & `intake-erddap-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `intake-erddap-0.2.4/tests/conftest.py` & `intake-erddap-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `intake-erddap-0.2.4/tests/test_cache.py` & `intake-erddap-0.3.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `intake-erddap-0.2.4/tests/test_data/tabledap_metadata.json` & `intake-erddap-0.3.0/tests/test_data/tabledap_metadata.json`

 * *Files identical despite different names*

### Comparing `intake-erddap-0.2.4/tests/test_erddap_cat.py` & `intake-erddap-0.3.0/tests/test_erddap_cat.py`

 * *Files identical despite different names*

### Comparing `intake-erddap-0.2.4/tests/test_erddap_source.py` & `intake-erddap-0.3.0/tests/test_erddap_source.py`

 * *Files 16% similar despite different names*

```diff
@@ -77,14 +77,43 @@
     assert mock_to_pandas.called
     assert len(df) == 2
 
     source.close()
     assert source._dataframe is None
 
 
+@mock.patch("intake_erddap.erddap.TableDAPSource._get_dataset_metadata")
+@mock.patch("erddapy.ERDDAP.to_pandas")
+def test_erddap_source_read_processing(mock_to_pandas, mock_get_dataset_metadata):
+    """Tests that the source will read from ERDDAP into a pd.DataFrame with processing flag."""
+    df = pd.DataFrame()
+    df["time"] = [
+        "2022-10-21T01:00:00Z",
+        "2022-10-21T02:00:00Z",
+        "2022-10-21T03:00:00Z",
+    ]
+    df["sea_water_temperature"] = [13.4, 13.4, np.nan]
+    df["sea_water_temperature_qc_agg"] = [1, 4, 2]
+    mock_to_pandas.return_value = df
+    mock_get_dataset_metadata.return_value = {}
+
+    source = TableDAPSource(
+        server="http://erddap.invalid/erddap",
+        dataset_id="abc123",
+        protocol="tabledap",
+        mask_failed_qartod=True,
+        dropna=True,
+    )
+    df = source.read()
+    assert df is not None
+    assert mock_to_pandas.called
+    # mask_failed_qartod flag removes 2nd data point and dropna removes 3rd data point
+    assert len(df) == 1
+
+
 @mock.patch("requests.get")
 def test_tabledap_source_get_dataset_metadata(mock_get):
     test_data = Path(__file__).parent / "test_data/tabledap_metadata.json"
     bad = {
         "table": {
             "rows": [
                 ["attribute", "NC_GLOBAL", "blah", "int", ","],
```

### Comparing `intake-erddap-0.2.4/tests/test_utils.py` & `intake-erddap-0.3.0/tests/test_utils.py`

 * *Files identical despite different names*

