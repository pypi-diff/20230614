# Comparing `tmp/mozregression-5.5.0.dev0.tar.gz` & `tmp/mozregression-5.5.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozregression-5.5.0.dev0.tar", last modified: Thu Jun  8 18:43:26 2023, max compression
+gzip compressed data, was "mozregression-5.5.0.dev1.tar", last modified: Wed Jun 14 19:06:33 2023, max compression
```

## Comparing `mozregression-5.5.0.dev0.tar` & `mozregression-5.5.0.dev1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:43:26.785893 mozregression-5.5.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/.coveralls.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:43:26.777892 mozregression-5.5.0.dev0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:43:26.777892 mozregression-5.5.0.dev0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/.github/workflows/compile-requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/.github/workflows/deploy-gui.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/.github/workflows/glean-probe-scraper.yml
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/.github/workflows/run-compile-requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-08 18:43:26.781892 mozregression-5.5.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:43:26.781892 mozregression-5.5.0.dev0/mozregression/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/approx_persist.py
--rw-r--r--   0 runner    (1001) docker     (123)    25458 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/bisector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/branches.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/bugzilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/build_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11266 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/build_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/class_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    23201 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/download_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/fetch_build_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    21598 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/fetch_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/json_pushes.py
--rw-r--r--   0 runner    (1001) docker     (123)    19190 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/launchers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/mach_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    14567 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/persist_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/pings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/releases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/tc_authenticate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/tempdir.py
--rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-08 18:43:26.000000 mozregression-5.5.0.dev0/mozregression/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:43:26.781892 mozregression-5.5.0.dev0/mozregression.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-08 18:43:26.000000 mozregression-5.5.0.dev0/mozregression.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-08 18:43:26.000000 mozregression-5.5.0.dev0/mozregression.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 18:43:26.000000 mozregression-5.5.0.dev0/mozregression.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-08 18:43:26.000000 mozregression-5.5.0.dev0/mozregression.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-08 18:43:26.000000 mozregression-5.5.0.dev0/mozregression.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 18:43:26.000000 mozregression-5.5.0.dev0/mozregression.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 18:43:26.785893 mozregression-5.5.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:06:33.220715 mozregression-5.5.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/.coveralls.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:06:33.212715 mozregression-5.5.0.dev1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:06:33.212715 mozregression-5.5.0.dev1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/.github/workflows/compile-requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/.github/workflows/deploy-gui.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/.github/workflows/glean-probe-scraper.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/.github/workflows/run-compile-requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-14 19:06:33.220715 mozregression-5.5.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:06:33.216715 mozregression-5.5.0.dev1/mozregression/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/mozregression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/mozregression/approx_persist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25458 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/mozregression/bisector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/mozregression/branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/mozregression/bugzilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/mozregression/build_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11266 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/mozregression/build_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/mozregression/class_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23201 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/mozregression/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/mozregression/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/mozregression/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/mozregression/download_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/mozregression/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/mozregression/fetch_build_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21598 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/mozregression/fetch_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/mozregression/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/mozregression/json_pushes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19190 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/mozregression/launchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/mozregression/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/mozregression/mach_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14567 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/mozregression/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/mozregression/metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/mozregression/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/mozregression/persist_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/mozregression/pings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/mozregression/releases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/mozregression/tc_authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/mozregression/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/mozregression/tempdir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/mozregression/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-14 19:06:33.000000 mozregression-5.5.0.dev1/mozregression/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:06:33.220715 mozregression-5.5.0.dev1/mozregression.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-14 19:06:33.000000 mozregression-5.5.0.dev1/mozregression.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-14 19:06:33.000000 mozregression-5.5.0.dev1/mozregression.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 19:06:33.000000 mozregression-5.5.0.dev1/mozregression.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-14 19:06:33.000000 mozregression-5.5.0.dev1/mozregression.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-14 19:06:33.000000 mozregression-5.5.0.dev1/mozregression.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-14 19:06:33.000000 mozregression-5.5.0.dev1/mozregression.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 19:06:33.220715 mozregression-5.5.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-14 19:05:37.000000 mozregression-5.5.0.dev1/setup.py
```

### Comparing `mozregression-5.5.0.dev0/.github/workflows/build.yml` & `mozregression-5.5.0.dev1/.github/workflows/build.yml`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,21 @@
   lint:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python
         uses: actions/setup-python@v2
         with:
-          python-version: "3.10"
+          python-version: 3.9
       - name: Install dependencies
         run: |
           python -m venv env
           source env/bin/activate
           python -m pip install --upgrade pip
-          python -m pip install -r requirements/requirements-3.10-Linux.txt
+          python -m pip install -r requirements/requirements-3.9-Linux.txt
           python -m pip install -e .
       - name: Lint
         run: |
           source env/bin/activate
           ./bin/lint-check.sh || (echo "Lint fix results:" && ./bin/lint-fix.sh && git diff && false)
 
   build-and-test-linux-base:
@@ -125,15 +125,15 @@
           python -m pip install --upgrade pip
           python -m pip install -r requirements/requirements-3.11-macOS.txt
           python -m pip install -e .
       - name: Build
         run: |
           source env/bin/activate
           python gui/build.py bundle
-          ls -alh gui/dist/mozregression-gui.dmg
+          ls -alh gui/mozregression-gui-app-bundle.tar.gz
       - name: Test
         run: |
           source env/bin/activate
           coverage run -m pytest -v gui/tests
           coveralls --service=github
   build-and-test-windows-gui:
     runs-on: windows-latest
```

### Comparing `mozregression-5.5.0.dev0/.github/workflows/compile-requirements.yml` & `mozregression-5.5.0.dev1/.github/workflows/compile-requirements.yml`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev0/.github/workflows/deploy-gui.yml` & `mozregression-5.5.0.dev1/.github/workflows/deploy-gui.yml`

 * *Files 6% similar despite different names*

```diff
@@ -72,21 +72,21 @@
           python -m pip install --upgrade pip
           python -m pip install -r requirements/requirements-3.11-macOS.txt
           python -m pip install -e .
       - name: Build
         run: |
           source env/bin/activate
           python gui/build.py bundle
-          ls -alh gui/dist/mozregression-gui.dmg
+          ls -alh gui/mozregression-gui-app-bundle.tar.gz
       - name: Upload
         uses: actions/upload-release-asset@v1
         with:
           upload_url: ${{ github.event.release.upload_url }}
-          asset_path: ./gui/dist/mozregression-gui.dmg
-          asset_name: mozregression-gui.dmg
+          asset_path: ./gui/dist/mozregression-gui-app-bundle.tar.gz
+          asset_name: mozregression-gui-app-bundle.tar.gz
           asset_content_type: application/octet-stream
   build-and-publish-windows-gui:
     runs-on: windows-latest
     env:
       GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
     steps:
       - uses: actions/checkout@v2
```

### Comparing `mozregression-5.5.0.dev0/.github/workflows/deploy.yml` & `mozregression-5.5.0.dev1/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev0/.github/workflows/run-compile-requirements.yml` & `mozregression-5.5.0.dev1/.github/workflows/run-compile-requirements.yml`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev0/LICENSE` & `mozregression-5.5.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev0/PKG-INFO` & `mozregression-5.5.0.dev1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozregression
-Version: 5.5.0.dev0
+Version: 5.5.0.dev1
 Summary: Regression range finder for Mozilla nightly builds
 Home-page: http://github.com/mozilla/mozregression
 Author: Mozilla Automation and Tools Team
 Author-email: tools@lists.mozilla.org
 License: MPL 2.0
 Platform: Any
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `mozregression-5.5.0.dev0/README.md` & `mozregression-5.5.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev0/mozregression/approx_persist.py` & `mozregression-5.5.0.dev1/mozregression/approx_persist.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev0/mozregression/bisector.py` & `mozregression-5.5.0.dev1/mozregression/bisector.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev0/mozregression/branches.py` & `mozregression-5.5.0.dev1/mozregression/branches.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev0/mozregression/bugzilla.py` & `mozregression-5.5.0.dev1/mozregression/bugzilla.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev0/mozregression/build_info.py` & `mozregression-5.5.0.dev1/mozregression/build_info.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev0/mozregression/build_range.py` & `mozregression-5.5.0.dev1/mozregression/build_range.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev0/mozregression/class_registry.py` & `mozregression-5.5.0.dev1/mozregression/class_registry.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev0/mozregression/cli.py` & `mozregression-5.5.0.dev1/mozregression/cli.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev0/mozregression/config.py` & `mozregression-5.5.0.dev1/mozregression/config.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev0/mozregression/dates.py` & `mozregression-5.5.0.dev1/mozregression/dates.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev0/mozregression/download_manager.py` & `mozregression-5.5.0.dev1/mozregression/download_manager.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev0/mozregression/errors.py` & `mozregression-5.5.0.dev1/mozregression/errors.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev0/mozregression/fetch_build_info.py` & `mozregression-5.5.0.dev1/mozregression/fetch_build_info.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev0/mozregression/fetch_configs.py` & `mozregression-5.5.0.dev1/mozregression/fetch_configs.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev0/mozregression/history.py` & `mozregression-5.5.0.dev1/mozregression/history.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev0/mozregression/json_pushes.py` & `mozregression-5.5.0.dev1/mozregression/json_pushes.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev0/mozregression/launchers.py` & `mozregression-5.5.0.dev1/mozregression/launchers.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev0/mozregression/log.py` & `mozregression-5.5.0.dev1/mozregression/log.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev0/mozregression/mach_interface.py` & `mozregression-5.5.0.dev1/mozregression/mach_interface.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev0/mozregression/main.py` & `mozregression-5.5.0.dev1/mozregression/main.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev0/mozregression/metrics.yaml` & `mozregression-5.5.0.dev1/mozregression/metrics.yaml`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev0/mozregression/network.py` & `mozregression-5.5.0.dev1/mozregression/network.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev0/mozregression/persist_limit.py` & `mozregression-5.5.0.dev1/mozregression/persist_limit.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev0/mozregression/pings.yaml` & `mozregression-5.5.0.dev1/mozregression/pings.yaml`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev0/mozregression/releases.py` & `mozregression-5.5.0.dev1/mozregression/releases.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev0/mozregression/tc_authenticate.py` & `mozregression-5.5.0.dev1/mozregression/tc_authenticate.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev0/mozregression/telemetry.py` & `mozregression-5.5.0.dev1/mozregression/telemetry.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,43 +32,45 @@
         "python_version",
     ],
 )
 
 
 def get_system_info():
     """Return a dictionary with various information about the system."""
+    UNKNOWN = "unknown"
     info = {
         "windows_version": None,
         "mac_version": None,
         "linux_version": None,
         "linux_distro": None,
         "python_version": None,
     }
 
     if mozinfo.os == "mac":
         try:
             # Fetch the "release" from tuple containing macOS version information.
             # See https://docs.python.org/3/library/platform.html#macos-platform.
             info["mac_version"] = platform.mac_ver()[0]
         except (AttributeError, IndexError):
-            pass
+            info["mac_version"] = UNKNOWN
     elif mozinfo.os == "windows":
         try:
             # Fetch "version" from tuple containing Windows version information.
             # See https://docs.python.org/3/library/platform.html#windows-platform.
             info["windows_version"] = platform.win32_ver()[1]
         except (AttributeError, IndexError):
-            pass
-    else:
+            info["windows_version"] = UNKNOWN
+    elif mozinfo.os == "linux":
         distro_info = distro.info()
         try:
             info["linux_version"] = distro_info["version"]
             info["linux_distro"] = distro_info["id"]
         except KeyError:
-            pass
+            info["linux_version"] = UNKNOWN
+            info["linux_distro"] = UNKNOWN
     info["python_version"] = platform.python_version()
     return info
 
 
 def initialize_telemetry(upload_enabled, allow_multiprocessing=False):
     mozregression_path = Path.home() / ".mozilla" / "mozregression"
     Glean.initialize(
```

### Comparing `mozregression-5.5.0.dev0/mozregression/tempdir.py` & `mozregression-5.5.0.dev1/mozregression/tempdir.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev0/mozregression/test_runner.py` & `mozregression-5.5.0.dev1/mozregression/test_runner.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev0/mozregression.egg-info/PKG-INFO` & `mozregression-5.5.0.dev1/mozregression.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozregression
-Version: 5.5.0.dev0
+Version: 5.5.0.dev1
 Summary: Regression range finder for Mozilla nightly builds
 Home-page: http://github.com/mozilla/mozregression
 Author: Mozilla Automation and Tools Team
 Author-email: tools@lists.mozilla.org
 License: MPL 2.0
 Platform: Any
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `mozregression-5.5.0.dev0/mozregression.egg-info/SOURCES.txt` & `mozregression-5.5.0.dev1/mozregression.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev0/pyproject.toml` & `mozregression-5.5.0.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.0.dev0/setup.py` & `mozregression-5.5.0.dev1/setup.py`

 * *Files identical despite different names*

