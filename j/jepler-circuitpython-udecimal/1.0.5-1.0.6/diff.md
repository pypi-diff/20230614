# Comparing `tmp/jepler-circuitpython-udecimal-1.0.5.tar.gz` & `tmp/jepler-circuitpython-udecimal-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jepler-circuitpython-udecimal-1.0.5.tar", last modified: Tue Feb 15 22:47:29 2022, max compression
+gzip compressed data, was "jepler-circuitpython-udecimal-1.0.6.tar", last modified: Wed Jun  8 10:01:31 2022, max compression
```

## Comparing `jepler-circuitpython-udecimal-1.0.5.tar` & `jepler-circuitpython-udecimal-1.0.6.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 22:47:29.857618 jepler-circuitpython-udecimal-1.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 22:47:29.849618 jepler-circuitpython-udecimal-1.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 22:47:29.853618 jepler-circuitpython-udecimal-1.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     3559 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2719 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      813 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16247 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     3960 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 22:47:29.853618 jepler-circuitpython-udecimal-1.0.5/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    10283 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1288 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/LICENSES/BSD-2-Clause.txt
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     9272 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/LICENSES/Python-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3520 2022-02-15 22:47:29.857618 jepler-circuitpython-udecimal-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2194 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/README.rst.license
--rwxr-xr-x   0 runner    (1001) docker     (121)     1991 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/build.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 22:47:29.853618 jepler-circuitpython-udecimal-1.0.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 22:47:29.853618 jepler-circuitpython-udecimal-1.0.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/docs/api.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 22:47:29.853618 jepler-circuitpython-udecimal-1.0.5/docs/autoapi/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 22:47:29.853618 jepler-circuitpython-udecimal-1.0.5/docs/autoapi/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 22:47:29.853618 jepler-circuitpython-udecimal-1.0.5/docs/autoapi/templates/python/
--rw-r--r--   0 runner    (1001) docker     (121)     2107 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/docs/autoapi/templates/python/module.rst
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/docs/autoapi/templates/python/module.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5547 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      807 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 22:47:29.857618 jepler-circuitpython-udecimal-1.0.5/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     2998 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/examples/test_udecimal.py
--rw-r--r--   0 runner    (1001) docker     (121)     2266 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/examples/udecimal_moneyfmt.py
--rw-r--r--   0 runner    (1001) docker     (121)      521 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/examples/udecimal_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 22:47:29.857618 jepler-circuitpython-udecimal-1.0.5/jepler_circuitpython_udecimal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3520 2022-02-15 22:47:29.000000 jepler-circuitpython-udecimal-1.0.5/jepler_circuitpython_udecimal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1029 2022-02-15 22:47:29.000000 jepler-circuitpython-udecimal-1.0.5/jepler_circuitpython_udecimal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-15 22:47:29.000000 jepler-circuitpython-udecimal-1.0.5/jepler_circuitpython_udecimal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-02-15 22:47:29.000000 jepler-circuitpython-udecimal-1.0.5/jepler_circuitpython_udecimal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 22:47:29.857618 jepler-circuitpython-udecimal-1.0.5/jepler_udecimal/
--rw-r--r--   0 runner    (1001) docker     (121)   186109 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/jepler_udecimal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/jepler_udecimal/test.py
--rw-r--r--   0 runner    (1001) docker     (121)     6145 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/jepler_udecimal/utrig.py
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-15 22:47:29.857618 jepler-circuitpython-udecimal-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2468 2022-02-15 22:47:16.000000 jepler-circuitpython-udecimal-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 10:01:31.494793 jepler-circuitpython-udecimal-1.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 10:01:31.490793 jepler-circuitpython-udecimal-1.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 10:01:31.490793 jepler-circuitpython-udecimal-1.0.6/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 10:01:31.490793 jepler-circuitpython-udecimal-1.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     3544 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2719 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      275 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1219 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    14022 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     3960 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 10:01:31.490793 jepler-circuitpython-udecimal-1.0.6/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    10283 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1288 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/LICENSES/BSD-2-Clause.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     9272 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/LICENSES/Python-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3749 2022-06-08 10:01:31.494793 jepler-circuitpython-udecimal-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2423 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/README.rst.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1991 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 10:01:31.494793 jepler-circuitpython-udecimal-1.0.6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 10:01:31.494793 jepler-circuitpython-udecimal-1.0.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/docs/api.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 10:01:31.490793 jepler-circuitpython-udecimal-1.0.6/docs/autoapi/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 10:01:31.490793 jepler-circuitpython-udecimal-1.0.6/docs/autoapi/templates/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 10:01:31.494793 jepler-circuitpython-udecimal-1.0.6/docs/autoapi/templates/python/
+-rw-r--r--   0 runner    (1001) docker     (121)     2107 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/docs/autoapi/templates/python/module.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/docs/autoapi/templates/python/module.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5547 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      807 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      138 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 10:01:31.494793 jepler-circuitpython-udecimal-1.0.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     2998 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/examples/test_udecimal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2266 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/examples/udecimal_moneyfmt.py
+-rw-r--r--   0 runner    (1001) docker     (121)      521 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/examples/udecimal_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 10:01:31.494793 jepler-circuitpython-udecimal-1.0.6/jepler_circuitpython_udecimal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3749 2022-06-08 10:01:31.000000 jepler-circuitpython-udecimal-1.0.6/jepler_circuitpython_udecimal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-06-08 10:01:31.000000 jepler-circuitpython-udecimal-1.0.6/jepler_circuitpython_udecimal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-08 10:01:31.000000 jepler-circuitpython-udecimal-1.0.6/jepler_circuitpython_udecimal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-06-08 10:01:31.000000 jepler-circuitpython-udecimal-1.0.6/jepler_circuitpython_udecimal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 10:01:31.494793 jepler-circuitpython-udecimal-1.0.6/jepler_udecimal/
+-rw-r--r--   0 runner    (1001) docker     (121)   186123 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/jepler_udecimal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      550 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/jepler_udecimal/test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6145 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/jepler_udecimal/utrig.py
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      393 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-08 10:01:31.494793 jepler-circuitpython-udecimal-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2468 2022-06-08 10:01:21.000000 jepler-circuitpython-udecimal-1.0.6/setup.py
```

### Comparing `jepler-circuitpython-udecimal-1.0.5/.github/workflows/build.yml` & `jepler-circuitpython-udecimal-1.0.6/.github/workflows/build.yml`

 * *Files 4% similar despite different names*

```diff
@@ -38,17 +38,17 @@
       with:
         repository: adafruit/actions-ci-circuitpython-libs
         path: actions-ci
     - name: Install dependencies
       # (e.g. - apt-get: gettext, etc; pip: circuitpython-build-tools, requirements.txt; etc.)
       run: |
         source actions-ci/install.sh
-    - name: Pip install pylint, Sphinx, pre-commit
+    - name: Pip install Sphinx, pre-commit
       run: |
-        pip install --force-reinstall pylint Sphinx sphinx-rtd-theme pre-commit sphinx-autoapi
+        pip install --force-reinstall Sphinx sphinx-rtd-theme pre-commit sphinx-autoapi
     - name: Library version
       run: git describe --dirty --always --tags
     - name: Setup problem matchers
       uses: adafruit/circuitpython-action-library-ci-problem-matchers@v1
     - name: Pre-commit hooks
       run: |
         pre-commit run --all-files
```

### Comparing `jepler-circuitpython-udecimal-1.0.5/.github/workflows/release.yml` & `jepler-circuitpython-udecimal-1.0.6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `jepler-circuitpython-udecimal-1.0.5/.pylintrc` & `jepler-circuitpython-udecimal-1.0.6/.pylintrc`

 * *Files 16% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 # file where it should appear only once).You can also use "--disable=all" to
 # disable everything first and then reenable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use"--disable=all --enable=classes
 # --disable=W"
 # disable=import-error,print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call
-disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation
+disable=raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,import-error,consider-using-f-string,unnecessary-dunder-call
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=
 
@@ -222,20 +222,14 @@
 
 # Maximum number of characters on a single line.
 max-line-length=100
 
 # Maximum number of lines in a module
 max-module-lines=1000
 
-# List of optional constructs for which whitespace checking is disabled. `dict-
-# separator` is used to allow tabulation in dicts, etc.: {1  : 1,\n222: 2}.
-# `trailing-comma` allows a space between comma and closing bracket: (a, ).
-# `empty-line` allows space-only lines.
-no-space-check=trailing-comma,dict-separator
-
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 single-line-class-stmt=no
 
 # Allow the body of an if to be on the same line as the test if there is no
 # else.
 single-line-if-stmt=no
@@ -254,81 +248,53 @@
 
 # Minimum lines number of a similarity.
 min-similarity-lines=4
 
 
 [BASIC]
 
-# Naming hint for argument names
-argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct argument names
 argument-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for attribute names
-attr-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct attribute names
 attr-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Bad variable names which should always be refused, separated by a comma
 bad-names=foo,bar,baz,toto,tutu,tata
 
-# Naming hint for class attribute names
-class-attribute-name-hint=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
-
 # Regular expression matching correct class attribute names
 class-attribute-rgx=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
 
-# Naming hint for class names
-# class-name-hint=[A-Z_][a-zA-Z0-9]+$
-class-name-hint=[A-Z_][a-zA-Z0-9_]+$
-
 # Regular expression matching correct class names
 # class-rgx=[A-Z_][a-zA-Z0-9]+$
 class-rgx=[A-Z_][a-zA-Z0-9_]+$
 
-# Naming hint for constant names
-const-name-hint=(([A-Z_][A-Z0-9_]*)|(__.*__))$
-
 # Regular expression matching correct constant names
 const-rgx=(([A-Z_][A-Z0-9_]*)|(__.*__))$
 
 # Minimum line length for functions/classes that require docstrings, shorter
 # ones are exempt.
 docstring-min-length=-1
 
-# Naming hint for function names
-function-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct function names
 function-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Good variable names which should always be accepted, separated by a comma
 # good-names=i,j,k,ex,Run,_
 good-names=r,g,b,w,i,j,k,n,x,y,z,ex,ok,Run,_
 
 # Include a hint for the correct naming format with invalid-name
 include-naming-hint=no
 
-# Naming hint for inline iteration names
-inlinevar-name-hint=[A-Za-z_][A-Za-z0-9_]*$
-
 # Regular expression matching correct inline iteration names
 inlinevar-rgx=[A-Za-z_][A-Za-z0-9_]*$
 
-# Naming hint for method names
-method-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct method names
 method-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for module names
-module-name-hint=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
-
 # Regular expression matching correct module names
 module-rgx=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
 
 # Colon-delimited sets of names that determine each other's naming style when
 # the name regexes allow several styles.
 name-group=
 
@@ -336,17 +302,14 @@
 # not require a docstring.
 no-docstring-rgx=^_
 
 # List of decorators that produce properties, such as abc.abstractproperty. Add
 # to this list to register other decorators that produce valid properties.
 property-classes=abc.abstractproperty
 
-# Naming hint for variable names
-variable-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct variable names
 variable-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 
 [IMPORTS]
 
 # Allow wildcard imports from modules that define __all__.
```

### Comparing `jepler-circuitpython-udecimal-1.0.5/CODE_OF_CONDUCT.md` & `jepler-circuitpython-udecimal-1.0.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `jepler-circuitpython-udecimal-1.0.5/LICENSE` & `jepler-circuitpython-udecimal-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jepler-circuitpython-udecimal-1.0.5/LICENSES/Apache-2.0.txt` & `jepler-circuitpython-udecimal-1.0.6/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `jepler-circuitpython-udecimal-1.0.5/LICENSES/BSD-2-Clause.txt` & `jepler-circuitpython-udecimal-1.0.6/LICENSES/BSD-2-Clause.txt`

 * *Files identical despite different names*

### Comparing `jepler-circuitpython-udecimal-1.0.5/LICENSES/CC-BY-4.0.txt` & `jepler-circuitpython-udecimal-1.0.6/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `jepler-circuitpython-udecimal-1.0.5/LICENSES/MIT.txt` & `jepler-circuitpython-udecimal-1.0.6/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `jepler-circuitpython-udecimal-1.0.5/LICENSES/Python-2.0.txt` & `jepler-circuitpython-udecimal-1.0.6/LICENSES/Python-2.0.txt`

 * *Files identical despite different names*

### Comparing `jepler-circuitpython-udecimal-1.0.5/LICENSES/Unlicense.txt` & `jepler-circuitpython-udecimal-1.0.6/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `jepler-circuitpython-udecimal-1.0.5/PKG-INFO` & `jepler-circuitpython-udecimal-1.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jepler-circuitpython-udecimal
-Version: 1.0.5
+Version: 1.0.6
 Summary: Reduced version of the decimal library for CircuitPython
 Home-page: https://github.com/jepler/Jepler_CircuitPython_udecimal
 Author: Jeff Epler
 Author-email: jepler@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/jepler/Jepler_CircuitPython_udecimal
 Project-URL: Documentation, https://jepler-udecimal.readthedocs.io/en/latest/api/jepler_udecimal/index.html
@@ -40,14 +40,18 @@
     :target: https://github.com/jepler/Jepler_CircuitPython_udecimal/actions
     :alt: Build Status
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
+.. image:: https://results.pre-commit.ci/badge/github/jepler/Jepler_CircuitPython_udecimal/main.svg
+   :target: https://results.pre-commit.ci/latest/github/jepler/Jepler_CircuitPython_udecimal/main
+   :alt: pre-commit.ci status
+
 Reduced version of the decimal library for CircuitPython
 
 
 Dependencies
 =============
 This library depends on:
```

### Comparing `jepler-circuitpython-udecimal-1.0.5/README.rst` & `jepler-circuitpython-udecimal-1.0.6/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -13,14 +13,18 @@
     :target: https://github.com/jepler/Jepler_CircuitPython_udecimal/actions
     :alt: Build Status
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
+.. image:: https://results.pre-commit.ci/badge/github/jepler/Jepler_CircuitPython_udecimal/main.svg
+   :target: https://results.pre-commit.ci/latest/github/jepler/Jepler_CircuitPython_udecimal/main
+   :alt: pre-commit.ci status
+
 Reduced version of the decimal library for CircuitPython
 
 
 Dependencies
 =============
 This library depends on:
```

### Comparing `jepler-circuitpython-udecimal-1.0.5/build.sh` & `jepler-circuitpython-udecimal-1.0.6/build.sh`

 * *Files identical despite different names*

### Comparing `jepler-circuitpython-udecimal-1.0.5/docs/_static/favicon.ico` & `jepler-circuitpython-udecimal-1.0.6/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `jepler-circuitpython-udecimal-1.0.5/docs/autoapi/templates/python/module.rst` & `jepler-circuitpython-udecimal-1.0.6/docs/autoapi/templates/python/module.rst`

 * *Files identical despite different names*

### Comparing `jepler-circuitpython-udecimal-1.0.5/docs/conf.py` & `jepler-circuitpython-udecimal-1.0.6/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 release = "1.0"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = [
     "_build",
     "Thumbs.db",
```

### Comparing `jepler-circuitpython-udecimal-1.0.5/docs/index.rst` & `jepler-circuitpython-udecimal-1.0.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `jepler-circuitpython-udecimal-1.0.5/examples/test_udecimal.py` & `jepler-circuitpython-udecimal-1.0.6/examples/test_udecimal.py`

 * *Files identical despite different names*

### Comparing `jepler-circuitpython-udecimal-1.0.5/examples/udecimal_moneyfmt.py` & `jepler-circuitpython-udecimal-1.0.6/examples/udecimal_moneyfmt.py`

 * *Files identical despite different names*

### Comparing `jepler-circuitpython-udecimal-1.0.5/examples/udecimal_simpletest.py` & `jepler-circuitpython-udecimal-1.0.6/examples/udecimal_simpletest.py`

 * *Files identical despite different names*

### Comparing `jepler-circuitpython-udecimal-1.0.5/jepler_circuitpython_udecimal.egg-info/PKG-INFO` & `jepler-circuitpython-udecimal-1.0.6/jepler_circuitpython_udecimal.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jepler-circuitpython-udecimal
-Version: 1.0.5
+Version: 1.0.6
 Summary: Reduced version of the decimal library for CircuitPython
 Home-page: https://github.com/jepler/Jepler_CircuitPython_udecimal
 Author: Jeff Epler
 Author-email: jepler@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/jepler/Jepler_CircuitPython_udecimal
 Project-URL: Documentation, https://jepler-udecimal.readthedocs.io/en/latest/api/jepler_udecimal/index.html
@@ -40,14 +40,18 @@
     :target: https://github.com/jepler/Jepler_CircuitPython_udecimal/actions
     :alt: Build Status
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
+.. image:: https://results.pre-commit.ci/badge/github/jepler/Jepler_CircuitPython_udecimal/main.svg
+   :target: https://results.pre-commit.ci/latest/github/jepler/Jepler_CircuitPython_udecimal/main
+   :alt: pre-commit.ci status
+
 Reduced version of the decimal library for CircuitPython
 
 
 Dependencies
 =============
 This library depends on:
```

### Comparing `jepler-circuitpython-udecimal-1.0.5/jepler_circuitpython_udecimal.egg-info/SOURCES.txt` & `jepler-circuitpython-udecimal-1.0.6/jepler_circuitpython_udecimal.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 README.rst
 README.rst.license
 build.sh
 pyproject.toml
 requirements.txt
 requirements_dev.txt
 setup.py
+.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/release.yml
 LICENSES/Apache-2.0.txt
 LICENSES/BSD-2-Clause.txt
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Python-2.0.txt
```

### Comparing `jepler-circuitpython-udecimal-1.0.5/jepler_udecimal/__init__.py` & `jepler-circuitpython-udecimal-1.0.6/jepler_udecimal/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #    and Raymond Hettinger <python at rcn.com>
 #    and Aahz <aahz at pobox.com>
 #    and Tim Peters
 #
 # Adapted to CircuitPython by Jeff Epler <jepler@gmail.com>
 #
 # pylint: disable=line-too-long,superfluous-parens,too-many-lines,redefined-builtin,bare-except
-# pylint: disable=protected-access,invalid-name,no-self-use,self-cls-assignment,no-else-return,no-else-raise,too-many-public-methods,useless-object-inheritance,invalid-unary-operand-type,unused-argument,too-many-branches,too-many-return-statements,no-else-break,unused-variable,arguments-differ,missing-function-docstring,inconsistent-return-statements,global-statement,too-many-statements,attribute-defined-outside-init,consider-using-in,dangerous-default-value,using-constant-test,too-many-locals,too-many-arguments,keyword-arg-before-vararg
+# pylint: disable=protected-access,invalid-name,self-cls-assignment,no-else-return,no-else-raise,too-many-public-methods,useless-object-inheritance,invalid-unary-operand-type,unused-argument,too-many-branches,too-many-return-statements,no-else-break,unused-variable,arguments-differ,missing-function-docstring,inconsistent-return-statements,global-statement,too-many-statements,attribute-defined-outside-init,consider-using-in,dangerous-default-value,using-constant-test,too-many-locals,too-many-arguments,keyword-arg-before-vararg
 """
 Reduced version of the decimal library for CircuitPython.  It runs on
 CircuitPython as well as standard Python, though you should probably
 use the built in decimal module on standard Python.
 
 It still requires a fairly beefy mcu to run.  Importing jepler_udecimal
 on an nRF52840 uses about 52kB of heap.
@@ -137,43 +137,45 @@
 import sys
 
 try:
     from collections import namedtuple as _namedtuple
 
     DecimalTuple = _namedtuple("DecimalTuple", "sign digits exponent")
 except ImportError:
-    DecimalTuple = lambda *args: args
+
+    def DecimalTuple(*args):  # type: ignore
+        return args
+
 
 # Rounding
 ROUND_DOWN = "ROUND_DOWN"
 ROUND_HALF_UP = "ROUND_HALF_UP"
 ROUND_HALF_EVEN = "ROUND_HALF_EVEN"
 ROUND_CEILING = "ROUND_CEILING"
 ROUND_FLOOR = "ROUND_FLOOR"
 ROUND_UP = "ROUND_UP"
 ROUND_HALF_DOWN = "ROUND_HALF_DOWN"
 ROUND_05UP = "ROUND_05UP"
 
 try:
-    NotImplemented
+    NotImplemented  # pylint: disable=used-before-assignment
 except NameError:
     NotImplemented = object()
 
 if sys.implementation.name == "circuitpython":
 
     def _as_integer_ratio(f):
         m, e = _math.frexp(f)
         m = round(m * (1 << 53))
         e = e - 53
         if e > 0:
             return m * (1 << e), 1
         else:
             return m, (1 << (-e))
 
-
 else:
     _as_integer_ratio = float.as_integer_ratio
 
 # Errors
 
 
 class DecimalException(ArithmeticError):
@@ -688,15 +690,15 @@
             return self
 
         if isinstance(value, float):
             if context is None:
                 context = getcontext()
             context._raise_error(
                 FloatOperation,
-                "strict semantics for mixing floats and Decimals are " "enabled",
+                "strict semantics for mixing floats and Decimals are enabled",
             )
             value = Decimal.from_float(value)
             self._exp = value._exp
             self._sign = value._sign
             self._int = value._int
             self._is_special = value._is_special
             return self
@@ -735,15 +737,15 @@
                 return cls(repr(f))
             if _math.copysign(1.0, f) == 1.0:
                 sign = 0
             else:
                 sign = 1
             n, d = _as_integer_ratio(abs(f))
             k = d.bit_length() - 1
-            coeff = str(n * 5 ** k)
+            coeff = str(n * 5**k)
         else:
             raise TypeError("argument must be int or float.")
 
         result = _dec_from_triple(sign, coeff, -k)
         if cls is Decimal:
             return result
         else:
@@ -1345,17 +1347,17 @@
         else:
             # OK, so neither = 0, INF or NaN
             shift = len(other._int) - len(self._int) + context.prec + 1
             exp = self._exp - other._exp - shift
             op1 = _WorkRep(self)
             op2 = _WorkRep(other)
             if shift >= 0:
-                coeff, remainder = divmod(op1.int * 10 ** shift, op2.int)
+                coeff, remainder = divmod(op1.int * 10**shift, op2.int)
             else:
-                coeff, remainder = divmod(op1.int, op2.int * 10 ** -shift)
+                coeff, remainder = divmod(op1.int, op2.int * 10**-shift)
             if remainder:
                 # result is not exact; adjust to ensure correct rounding
                 if coeff % 5 == 0:
                     coeff += 1
             else:
                 # result is exact; get as close to ideal exponent as possible
                 ideal_exp = self._exp - other._exp
@@ -1388,15 +1390,15 @@
             op1 = _WorkRep(self)
             op2 = _WorkRep(other)
             if op1.exp >= op2.exp:
                 op1.int *= 10 ** (op1.exp - op2.exp)
             else:
                 op2.int *= 10 ** (op2.exp - op1.exp)
             q, r = divmod(op1.int, op2.int)
-            if q < 10 ** context.prec:
+            if q < 10**context.prec:
                 return (
                     _dec_from_triple(sign, str(q), 0),
                     _dec_from_triple(self._sign, str(r), ideal_exp),
                 )
 
         # Here the quotient is too large to be representable
         ans = context._raise_error(
@@ -1548,15 +1550,15 @@
         # remainder is r*10**ideal_exponent; other is +/-op2.int *
         # 10**ideal_exponent.   Apply correction to ensure that
         # abs(remainder) <= abs(other)/2
         if 2 * r + (q & 1) > op2.int:
             r -= op2.int
             q += 1
 
-        if q >= 10 ** context.prec:
+        if q >= 10**context.prec:
             return context._raise_error(DivisionImpossible)
 
         # result has same sign as self unless r is negative
         sign = self._sign
         if r < 0:
             sign = 1 - sign
             r = -r
@@ -1615,15 +1617,15 @@
         if self._is_special:
             if self._isnan():
                 raise ValueError("Cannot convert NaN to integer")
             elif self._isinfinity():
                 raise OverflowError("Cannot convert infinity to integer")
         s = (-1) ** self._sign
         if self._exp >= 0:
-            return s * int(self._int) * 10 ** self._exp
+            return s * int(self._int) * 10**self._exp
         else:
             return s * int(self._int[: self._exp] or "0")
 
     __trunc__ = __int__
 
     def _fix_nan(self, context):
         """Decapitate the payload of a NaN to fit the context"""
@@ -1977,15 +1979,15 @@
             xe *= yc
             # result is now 10**(xe * 10**ye);  xe * 10**ye must be integral
             while xe % 10 == 0:
                 xe //= 10
                 ye += 1
             if ye < 0:
                 return None
-            exponent = xe * 10 ** ye
+            exponent = xe * 10**ye
             if y.sign == 1:
                 exponent = -exponent
             # if other is a nonnegative integer, use ideal exponent
             if other._isinteger() and other._sign == 0:
                 ideal_exponent = self._exp * _int(other)
                 zeros = min(exponent - ideal_exponent, p - 1)
             else:
@@ -2036,21 +2038,21 @@
                 e = _decimal_lshift_exact(e * yc, ye)
                 xe = _decimal_lshift_exact(xe * yc, ye)
                 if e is None or xe is None:
                     return None
 
                 if e > emax:
                     return None
-                xc = 5 ** e
+                xc = 5**e
 
             elif last_digit == 5:
                 # e >= log_5(xc) if xc is a power of 5; we have
                 # equality all the way up to xc=5**2658
                 e = _nbits(xc) * 28 // 65
-                xc, remainder = divmod(5 ** e, xc)
+                xc, remainder = divmod(5**e, xc)
                 if remainder:
                     return None
                 while xc % 5 == 0:
                     xc //= 5
                     e -= 1
 
                 # Guard against large values of ye, using the same logic as in
@@ -2063,26 +2065,26 @@
                 e = _decimal_lshift_exact(e * yc, ye)
                 xe = _decimal_lshift_exact(xe * yc, ye)
                 if e is None or xe is None:
                     return None
 
                 if e > emax:
                     return None
-                xc = 2 ** e
+                xc = 2**e
             else:
                 return None
 
-            if xc >= 10 ** p:
+            if xc >= 10**p:
                 return None
             xe = -e - xe
             return _dec_from_triple(0, str(xc), xe)
 
         # now y is positive; find m and n such that y = m/n
         if ye >= 0:
-            m, n = yc * 10 ** ye, 1
+            m, n = yc * 10**ye, 1
         else:
             if xe != 0 and len(str(abs(yc * xe))) <= -ye:
                 return None
             xc_bits = _nbits(xc)
             if xc != 1 and len(str(abs(yc) * xc_bits)) <= -ye:
                 return None
             m, n = yc, 10 ** (-ye)
@@ -2118,17 +2120,17 @@
         # now xc*10**xe is the nth root of the original xc*10**xe
         # compute mth power of xc*10**xe
 
         # if m > p*100//_log10_lb(xc) then m > p/log10(xc), hence xc**m >
         # 10**p and the result is not representable.
         if xc > 1 and m > p * 100 // _log10_lb(xc):
             return None
-        xc = xc ** m
+        xc = xc**m
         xe *= m
-        if xc > 10 ** p:
+        if xc > 10**p:
             return None
 
         # by this point the result *is* exactly representable
         # adjust the exponent to get as close as possible to the ideal
         # exponent, if necessary
         str_xc = str(xc)
         if other._isinteger() and other._sign == 0:
@@ -2565,38 +2567,38 @@
         else:
             c = op.int
             l = len(self._int) + 1 >> 1
 
         # rescale so that c has exactly prec base 100 'digits'
         shift = prec - l
         if shift >= 0:
-            c *= 100 ** shift
+            c *= 100**shift
             exact = True
         else:
-            c, remainder = divmod(c, 100 ** -shift)
+            c, remainder = divmod(c, 100**-shift)
             exact = not remainder
         e -= shift
 
         # find n = floor(sqrt(c)) using Newton's method
-        n = 10 ** prec
+        n = 10**prec
         while True:
             q = c // n
             if n <= q:
                 break
             else:
                 n = n + q >> 1
         exact = exact and n * n == c
 
         if exact:
             # result is exact; rescale to use ideal exponent e
             if shift >= 0:
                 # assert n % 10**shift == 0
-                n //= 10 ** shift
+                n //= 10**shift
             else:
-                n *= 10 ** -shift
+                n *= 10**-shift
             e += shift
         else:
             # result is not exact; fix last digit as described above
             if n % 5 == 0:
                 n += 1
 
         ans = _dec_from_triple(0, str(n), e)
@@ -2808,15 +2810,15 @@
         other = _convert_other(other, raiseit=True)
 
         s = self.copy_abs()
         o = other.copy_abs()
         return s.compare_total(o)
 
     def copy_abs(self):
-        """Returns a copy with the sign set to 0. """
+        """Returns a copy with the sign set to 0."""
         return _dec_from_triple(0, self._int, self._exp, self._is_special)
 
     def copy_negate(self):
         """Returns a copy with the sign inverted."""
         if self._sign:
             return _dec_from_triple(0, self._int, self._exp, self._is_special)
         else:
@@ -2972,19 +2974,19 @@
         if adj <= -2:
             # argument <= 0.1
             return len(str((-1 - adj) * 23 // 10)) - 1
         op = _WorkRep(self)
         c, e = op.int, op.exp
         if adj == 0:
             # 1 < self < 10
-            num = str(c - 10 ** -e)
+            num = str(c - 10**-e)
             den = str(c)
             return len(num) - len(den) - (num < den)
         # adj == -1, 0.1 <= self < 1
-        return e + len(str(10 ** -e - c)) - 1
+        return e + len(str(10**-e - c)) - 1
 
     def ln(self, context=None):
         """Returns the natural (base e) logarithm of self."""
 
         if context is None:
             context = getcontext()
 
@@ -3050,19 +3052,19 @@
         if adj <= -2:
             # self < 0.1
             return len(str(-1 - adj)) - 1
         op = _WorkRep(self)
         c, e = op.int, op.exp
         if adj == 0:
             # 1 < self < 10
-            num = str(c - 10 ** -e)
+            num = str(c - 10**-e)
             den = str(231 * c)
             return len(num) - len(den) - (num < den) + 2
         # adj == -1, 0.1 <= self < 1
-        num = str(10 ** -e - c)
+        num = str(10**-e - c)
         return len(num) + e - (num < "231") - 1
 
     def log10(self, context=None):
         """Returns the base 10 logarithm of self."""
 
         if context is None:
             context = getcontext()
@@ -3108,15 +3110,15 @@
         context = context._shallow_copy()
         rounding = context._set_rounding(ROUND_HALF_EVEN)
         ans = ans._fix(context)
         context.rounding = rounding
         return ans
 
     def logb(self, context=None):
-        """ Returns the exponent of the magnitude of self's MSD.
+        """Returns the exponent of the magnitude of self's MSD.
 
         The result is the integer which is the exponent of the magnitude
         of the most significant digit of self (as though it were truncated
         to a single digit while maintaining the value of that digit and
         without limiting the resulting exponent).
         """
         # logb(NaN) = NaN
@@ -3320,16 +3322,16 @@
 
 ##### Context class #######################################################
 
 
 class _ContextManager(object):
     """Context manager class to support localcontext().
 
-      Sets a copy of the supplied context in __enter__() and restores
-      the previous decimal context in __exit__()
+    Sets a copy of the supplied context in __enter__() and restores
+    the previous decimal context in __exit__()
     """
 
     def __init__(self, new_context):
         self.new_context = new_context.copy()
 
     def __enter__(self):
         self.saved_context = getcontext()
@@ -3571,15 +3573,15 @@
         """Stop ignoring the flags, if they are raised"""
         if flags and isinstance(flags[0], (tuple, list)):
             flags = flags[0]
         for flag in flags:
             self._ignored_flags.remove(flag)
 
     # We inherit object.__hash__, so we must deny this explicitly
-    __hash__ = None
+    __hash__ = None  # type: ignore
 
     def Etiny(self):
         """Returns Etiny (= Emin - prec + 1)"""
         return int(self.Emin - self.prec + 1)
 
     def Etop(self):
         """Returns maximum exponent (= Emax - prec + 1)"""
@@ -3609,15 +3611,15 @@
 
         This method implements the to-number operation of the
         IBM Decimal specification."""
 
         if isinstance(num, str) and (num != num.strip() or "_" in num):
             return self._raise_error(
                 ConversionSyntax,
-                "trailing or leading whitespace and " "underscores are not permitted.",
+                "trailing or leading whitespace and underscores are not permitted.",
             )
 
         d = Decimal(num, context=self)
         if d._isnan() and len(d._int) > self.prec - self.clamp:
             return self._raise_error(
                 ConversionSyntax, "diagnostic info too long in NaN"
             )
@@ -4198,15 +4200,15 @@
         >>> c.log10(1)
         Decimal('0')
         """
         a = _convert_other(a, raiseit=True)
         return a.log10(context=self)
 
     def logb(self, a):
-        """ Returns the exponent of the magnitude of the operand's MSD.
+        """Returns the exponent of the magnitude of the operand's MSD.
 
         The result is the integer which is the exponent of the magnitude
         of the most significant digit of the operand (as though the
         operand were truncated to a single digit while maintaining the
         value of that digit and without limiting the resulting exponent).
 
         >>> ExtendedContext.logb(Decimal('250'))
@@ -4898,33 +4900,33 @@
 
 ##### Integer arithmetic functions used by ln, log10, exp and __pow__ #####
 
 _nbits = int.bit_length
 
 
 def _decimal_lshift_exact(n, e):
-    """ Given integers n and e, return n * 10**e if it's an integer, else None.
+    """Given integers n and e, return n * 10**e if it's an integer, else None.
 
     The computation is designed to avoid computing large powers of 10
     unnecessarily.
 
     >>> _decimal_lshift_exact(3, 4)
     30000
     >>> _decimal_lshift_exact(300, -999999999)  # returns None
 
     """
     if n == 0:
         return 0
     elif e >= 0:
-        return n * 10 ** e
+        return n * 10**e
     else:
         # val_n = largest power of 10 dividing n.
         str_n = str(abs(n))
         val_n = len(str_n) - len(str_n.rstrip("0"))
-        return None if val_n < -e else n // 10 ** -e
+        return None if val_n < -e else n // 10**-e
 
 
 def _sqrt_nearest(n, a):
     """Closest integer to the square root of the positive integer n.  a is
     an initial approximation to the square root.  Any positive integer
     will do for a, but the closer a is to the square root of n the
     faster convergence will be.
@@ -5019,28 +5021,28 @@
     #   f >= 0 and 1 <= d <= 10, or
     #   f <= 0 and 0.1 <= d <= 1.
     # Thus for c*10**e close to 1, f = 0
     l = len(str(c))
     f = e + l - (e + l >= 1)
 
     if p > 0:
-        M = 10 ** p
+        M = 10**p
         k = e + p - f
         if k >= 0:
-            c *= 10 ** k
+            c *= 10**k
         else:
-            c = _div_nearest(c, 10 ** -k)
+            c = _div_nearest(c, 10**-k)
 
         log_d = _ilog(c, M)  # error < 5 + 22 = 27
         log_10 = _log10_digits(p)  # error < 1
         log_d = _div_nearest(log_d * M, log_10)
         log_tenpower = f * M  # exact
     else:
         log_d = 0  # error < 2.31
-        log_tenpower = _div_nearest(f, 10 ** -p)  # error < 0.5
+        log_tenpower = _div_nearest(f, 10**-p)  # error < 0.5
 
     return _div_nearest(log_tenpower + log_d, 100)
 
 
 def _dlog(c, e, p):
     """Given integers c, e and p with c > 0, compute an integer
     approximation to 10**p * log(c*10**e), with an absolute error of
@@ -5056,31 +5058,31 @@
     l = len(str(c))
     f = e + l - (e + l >= 1)
 
     # compute approximation to 10**p*log(d), with error < 27
     if p > 0:
         k = e + p - f
         if k >= 0:
-            c *= 10 ** k
+            c *= 10**k
         else:
-            c = _div_nearest(c, 10 ** -k)  # error of <= 0.5 in c
+            c = _div_nearest(c, 10**-k)  # error of <= 0.5 in c
 
         # _ilog magnifies existing error in c by a factor of at most 10
-        log_d = _ilog(c, 10 ** p)  # error < 5 + 22 = 27
+        log_d = _ilog(c, 10**p)  # error < 5 + 22 = 27
     else:
         # p <= 0: just approximate the whole thing by 0; error < 2.31
         log_d = 0
 
     # compute approximation to f*10**p*log(10), with error < 11.
     if f:
         extra = len(str(abs(f))) - 1
         if p + extra >= 0:
             # error in f * _log10_digits(p+extra) < |f| * 1 = |f|
             # after division, error < |f|/10**extra + 0.5 < 10 + 0.5 < 11
-            f_log_ten = _div_nearest(f * _log10_digits(p + extra), 10 ** extra)
+            f_log_ten = _div_nearest(f * _log10_digits(p + extra), 10**extra)
         else:
             f_log_ten = 0
     else:
         f_log_ten = 0
 
     # error in sum < 11+27 = 38; error after division < 0.38 + 0.5 < 1
     return _div_nearest(f_log_ten + log_d, 100)
@@ -5185,24 +5187,24 @@
     extra = max(0, e + len(str(c)) - 1)
     q = p + extra
 
     # compute quotient c*10**e/(log(10)) = c*10**(e+q)/(log(10)*10**q),
     # rounding down
     shift = e + q
     if shift >= 0:
-        cshift = c * 10 ** shift
+        cshift = c * 10**shift
     else:
-        cshift = c // 10 ** -shift
+        cshift = c // 10**-shift
     quot, rem = divmod(cshift, _log10_digits(q))
 
     # reduce remainder back to original precision
-    rem = _div_nearest(rem, 10 ** extra)
+    rem = _div_nearest(rem, 10**extra)
 
     # error in result of _iexp < 120;  error after division < 0.62
-    return _div_nearest(_iexp(rem, 10 ** p), 1000), quot - p + 3
+    return _div_nearest(_iexp(rem, 10**p), 1000), quot - p + 3
 
 
 def _dpower(xc, xe, yc, ye, p):
     """Given integers xc, xe, yc and ye representing Decimals x = xc*10**xe and
     y = yc*10**ye, compute x**y.  Returns a pair of integers (c, e) such that:
 
       10**(p-1) <= c <= 10**p, and
@@ -5221,25 +5223,25 @@
 
     # log(x) = lxc*10**(-p-b-1), to p+b+1 places after the decimal point
     lxc = _dlog(xc, xe, p + b + 1)
 
     # compute product y*log(x) = yc*lxc*10**(-p-b-1+ye) = pc*10**(-p-1)
     shift = ye - b
     if shift >= 0:
-        pc = lxc * yc * 10 ** shift
+        pc = lxc * yc * 10**shift
     else:
-        pc = _div_nearest(lxc * yc, 10 ** -shift)
+        pc = _div_nearest(lxc * yc, 10**-shift)
 
     if pc == 0:
         # we prefer a result that isn't exactly 1; this makes it
         # easier to compute a correctly rounded result in __pow__
         if (len(str(xc)) + xe >= 1) == (yc > 0):  # if x**y > 1:
             coeff, exp = 10 ** (p - 1) + 1, 1 - p
         else:
-            coeff, exp = 10 ** p - 1, -p
+            coeff, exp = 10**p - 1, -p
     else:
         coeff, exp = _dexp(pc, -(p + 1), p + 1)
         coeff = _div_nearest(coeff, 10)
         exp += 1
 
     return coeff, exp
 
@@ -5344,15 +5346,20 @@
 BasicContext = Context(
     prec=9,
     rounding=ROUND_HALF_UP,
     traps=[DivisionByZero, Overflow, InvalidOperation, Clamped, Underflow],
     flags=[],
 )
 
-ExtendedContext = Context(prec=9, rounding=ROUND_HALF_EVEN, traps=[], flags=[],)
+ExtendedContext = Context(
+    prec=9,
+    rounding=ROUND_HALF_EVEN,
+    traps=[],
+    flags=[],
+)
 
 
 ##### crud for parsing strings #############################################
 #
 # Regular expression used for parsing numeric strings.  Additional
 # comments:
 #
@@ -5364,15 +5371,15 @@
 # number between the optional sign and the optional exponent must have
 # at least one decimal digit, possibly after the decimal point.  The
 # lookahead expression '(?=\d|\.\d)' checks this.
 
 try:
     import re
 except:
-    import ure as re
+    import ure as re  # type: ignore
 
 _parser = re.compile(  # A numeric string consists of:
     r"([-+])?"  # an optional sign, followed by either...    # 1
     r"("  # ...a number                             # 2(
     r"(\d*)"  # having a (possibly empty) integer part  # 3
     r"(\.(\d*))?"  # followed by an optional fractional part # 4(5)
     r"(e([-+]?\d+))?"  # followed by an optional exponent, or... # 6(7)
```

### Comparing `jepler-circuitpython-udecimal-1.0.5/jepler_udecimal/test.py` & `jepler-circuitpython-udecimal-1.0.6/jepler_udecimal/test.py`

 * *Files identical despite different names*

### Comparing `jepler-circuitpython-udecimal-1.0.5/jepler_udecimal/utrig.py` & `jepler-circuitpython-udecimal-1.0.6/jepler_udecimal/utrig.py`

 * *Files identical despite different names*

### Comparing `jepler-circuitpython-udecimal-1.0.5/setup.py` & `jepler-circuitpython-udecimal-1.0.6/setup.py`

 * *Files identical despite different names*

