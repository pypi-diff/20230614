# Comparing `tmp/circuitpython-ps2controller-1.2.0.tar.gz` & `tmp/circuitpython-ps2controller-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-ps2controller-1.2.0.tar", last modified: Fri Jun  9 22:34:30 2023, max compression
+gzip compressed data, was "circuitpython-ps2controller-1.2.1.tar", last modified: Wed Jun 14 21:31:33 2023, max compression
```

## Comparing `circuitpython-ps2controller-1.2.0.tar` & `circuitpython-ps2controller-1.2.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:34:30.295277 circuitpython-ps2controller-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:34:30.291277 circuitpython-ps2controller-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:34:30.291277 circuitpython-ps2controller-1.2.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:34:30.291277 circuitpython-ps2controller-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:34:30.295277 circuitpython-ps2controller-1.2.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-06-09 22:34:30.295277 circuitpython-ps2controller-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:34:30.295277 circuitpython-ps2controller-1.2.0/circuitpython_ps2controller.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-06-09 22:34:30.000000 circuitpython-ps2controller-1.2.0/circuitpython_ps2controller.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-09 22:34:30.000000 circuitpython-ps2controller-1.2.0/circuitpython_ps2controller.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 22:34:30.000000 circuitpython-ps2controller-1.2.0/circuitpython_ps2controller.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 22:34:30.000000 circuitpython-ps2controller-1.2.0/circuitpython_ps2controller.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-09 22:34:30.000000 circuitpython-ps2controller-1.2.0/circuitpython_ps2controller.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:34:30.295277 circuitpython-ps2controller-1.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:34:30.295277 circuitpython-ps2controller-1.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)    58754 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/docs/ps2controller_wiring.png
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/docs/ps2controller_wiring.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:34:30.295277 circuitpython-ps2controller-1.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-09 22:34:22.000000 circuitpython-ps2controller-1.2.0/examples/ps2controller_datadump.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-09 22:34:22.000000 circuitpython-ps2controller-1.2.0/examples/ps2controller_digital_only.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-09 22:34:22.000000 circuitpython-ps2controller-1.2.0/examples/ps2controller_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-09 22:34:22.000000 circuitpython-ps2controller-1.2.0/examples/ps2controller_usbkeys.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14199 2023-06-09 22:34:22.000000 circuitpython-ps2controller-1.2.0/ps2controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-09 22:34:22.000000 circuitpython-ps2controller-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-09 22:34:14.000000 circuitpython-ps2controller-1.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 22:34:30.295277 circuitpython-ps2controller-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:31:33.922960 circuitpython-ps2controller-1.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:31:33.914959 circuitpython-ps2controller-1.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:31:33.918959 circuitpython-ps2controller-1.2.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-14 21:31:16.000000 circuitpython-ps2controller-1.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:31:33.918959 circuitpython-ps2controller-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-14 21:31:16.000000 circuitpython-ps2controller-1.2.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-14 21:31:16.000000 circuitpython-ps2controller-1.2.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-14 21:31:16.000000 circuitpython-ps2controller-1.2.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-14 21:31:16.000000 circuitpython-ps2controller-1.2.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-14 21:31:16.000000 circuitpython-ps2controller-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-14 21:31:16.000000 circuitpython-ps2controller-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-06-14 21:31:16.000000 circuitpython-ps2controller-1.2.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-14 21:31:16.000000 circuitpython-ps2controller-1.2.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-06-14 21:31:16.000000 circuitpython-ps2controller-1.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-14 21:31:16.000000 circuitpython-ps2controller-1.2.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:31:33.918959 circuitpython-ps2controller-1.2.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-06-14 21:31:16.000000 circuitpython-ps2controller-1.2.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-14 21:31:16.000000 circuitpython-ps2controller-1.2.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-14 21:31:16.000000 circuitpython-ps2controller-1.2.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-06-14 21:31:33.922960 circuitpython-ps2controller-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-06-14 21:31:16.000000 circuitpython-ps2controller-1.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-14 21:31:16.000000 circuitpython-ps2controller-1.2.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:31:33.918959 circuitpython-ps2controller-1.2.1/circuitpython_ps2controller.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-06-14 21:31:33.000000 circuitpython-ps2controller-1.2.1/circuitpython_ps2controller.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-14 21:31:33.000000 circuitpython-ps2controller-1.2.1/circuitpython_ps2controller.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 21:31:33.000000 circuitpython-ps2controller-1.2.1/circuitpython_ps2controller.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-14 21:31:33.000000 circuitpython-ps2controller-1.2.1/circuitpython_ps2controller.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-14 21:31:33.000000 circuitpython-ps2controller-1.2.1/circuitpython_ps2controller.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:31:33.922960 circuitpython-ps2controller-1.2.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:31:33.922960 circuitpython-ps2controller-1.2.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-14 21:31:16.000000 circuitpython-ps2controller-1.2.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-14 21:31:16.000000 circuitpython-ps2controller-1.2.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-14 21:31:16.000000 circuitpython-ps2controller-1.2.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-14 21:31:16.000000 circuitpython-ps2controller-1.2.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-14 21:31:16.000000 circuitpython-ps2controller-1.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-14 21:31:16.000000 circuitpython-ps2controller-1.2.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-14 21:31:16.000000 circuitpython-ps2controller-1.2.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-14 21:31:16.000000 circuitpython-ps2controller-1.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-14 21:31:16.000000 circuitpython-ps2controller-1.2.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)    58754 2023-06-14 21:31:16.000000 circuitpython-ps2controller-1.2.1/docs/ps2controller_wiring.png
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-14 21:31:16.000000 circuitpython-ps2controller-1.2.1/docs/ps2controller_wiring.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-14 21:31:16.000000 circuitpython-ps2controller-1.2.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:31:33.922960 circuitpython-ps2controller-1.2.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-14 21:31:26.000000 circuitpython-ps2controller-1.2.1/examples/ps2controller_datadump.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-14 21:31:26.000000 circuitpython-ps2controller-1.2.1/examples/ps2controller_digital_only.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-14 21:31:26.000000 circuitpython-ps2controller-1.2.1/examples/ps2controller_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-14 21:31:26.000000 circuitpython-ps2controller-1.2.1/examples/ps2controller_usbkeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-14 21:31:16.000000 circuitpython-ps2controller-1.2.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14160 2023-06-14 21:31:26.000000 circuitpython-ps2controller-1.2.1/ps2controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-14 21:31:26.000000 circuitpython-ps2controller-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-14 21:31:16.000000 circuitpython-ps2controller-1.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 21:31:33.922960 circuitpython-ps2controller-1.2.1/setup.cfg
```

### Comparing `circuitpython-ps2controller-1.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `circuitpython-ps2controller-1.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.2.0/.github/workflows/release_gh.yml` & `circuitpython-ps2controller-1.2.1/.github/workflows/release_gh.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.2.0/.gitignore` & `circuitpython-ps2controller-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.2.0/.pre-commit-config.yaml` & `circuitpython-ps2controller-1.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.2.0/.pylintrc` & `circuitpython-ps2controller-1.2.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.2.0/CODE_OF_CONDUCT.md` & `circuitpython-ps2controller-1.2.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.2.0/LICENSE` & `circuitpython-ps2controller-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.2.0/LICENSES/CC-BY-4.0.txt` & `circuitpython-ps2controller-1.2.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.2.0/LICENSES/MIT.txt` & `circuitpython-ps2controller-1.2.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.2.0/LICENSES/Unlicense.txt` & `circuitpython-ps2controller-1.2.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.2.0/PKG-INFO` & `circuitpython-ps2controller-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-ps2controller
-Version: 1.2.0
+Version: 1.2.1
 Summary: CircuitPython library to read Sony PS2 game controllers
 Author-email: Tod Kurt <tod@todbot.com>
 License: MIT
 Project-URL: Homepage, https://github.com/todbot/CircuitPython_PS2Controller
 Keywords: adafruit,blinka,circuitpython,micropython,ps2controller,ps2,psx,controller,gamepad,sony,dualshock
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-ps2controller-1.2.0/README.rst` & `circuitpython-ps2controller-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.2.0/circuitpython_ps2controller.egg-info/PKG-INFO` & `circuitpython-ps2controller-1.2.1/circuitpython_ps2controller.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-ps2controller
-Version: 1.2.0
+Version: 1.2.1
 Summary: CircuitPython library to read Sony PS2 game controllers
 Author-email: Tod Kurt <tod@todbot.com>
 License: MIT
 Project-URL: Homepage, https://github.com/todbot/CircuitPython_PS2Controller
 Keywords: adafruit,blinka,circuitpython,micropython,ps2controller,ps2,psx,controller,gamepad,sony,dualshock
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-ps2controller-1.2.0/circuitpython_ps2controller.egg-info/SOURCES.txt` & `circuitpython-ps2controller-1.2.1/circuitpython_ps2controller.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.2.0/docs/_static/favicon.ico` & `circuitpython-ps2controller-1.2.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.2.0/docs/conf.py` & `circuitpython-ps2controller-1.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.2.0/docs/examples.rst` & `circuitpython-ps2controller-1.2.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.2.0/docs/index.rst` & `circuitpython-ps2controller-1.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.2.0/docs/ps2controller_wiring.png` & `circuitpython-ps2controller-1.2.1/docs/ps2controller_wiring.png`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.2.0/examples/ps2controller_datadump.py` & `circuitpython-ps2controller-1.2.1/examples/ps2controller_datadump.py`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.2.0/examples/ps2controller_digital_only.py` & `circuitpython-ps2controller-1.2.1/examples/ps2controller_digital_only.py`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.2.0/examples/ps2controller_usbkeys.py` & `circuitpython-ps2controller-1.2.1/examples/ps2controller_usbkeys.py`

 * *Files identical despite different names*

### Comparing `circuitpython-ps2controller-1.2.0/ps2controller.py` & `circuitpython-ps2controller-1.2.1/ps2controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 """
 
 from collections import namedtuple
 import time
 from micropython import const
 import digitalio
 
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 __repo__ = "https://github.com/todbot/CircuitPython_PS2Controller.git"
 
 
 # Time between att being issues to control and first clock edge
 _ATTN_DELAY_MICROS = const(40)
 # hold time for dat/cmd pins after clk
 _HOLD_TIME_MICROS = const(2)
@@ -285,18 +285,18 @@
         """Bit-bang out a single byte on cmd_pin, while reading in a single byte on dat_pin"""
         byte_in = 0
         # clock is held high until a byte is to be sent
         for i in range(8):
             self.cmd_pin.value = (byte_out & (1 << i)) != 0  # send OUT data on cmd pin
             self.clk_pin.value = False  # clock LOW
             _delay_micros(_HOLD_TIME_MICROS)
-            self.clk_pin.value = True  # clock HIGH
-            _delay_micros(_HOLD_TIME_MICROS)  # seems uneeded in CirPy because slow
             if self.dat_pin.value:  # read IN data on dat pin
                 byte_in |= 1 << i
+            self.clk_pin.value = True  # clock HIGH
+            _delay_micros(_HOLD_TIME_MICROS)
         return byte_in
 
     def _shift_inout_buf(self, bytes_out):
         """
         Send out a buffer of bytes on cmd_pin,
         while reading in a same-sized buffer on dat_pin
         """
```

### Comparing `circuitpython-ps2controller-1.2.0/pyproject.toml` & `circuitpython-ps2controller-1.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-ps2controller"
 description = "CircuitPython library to read Sony PS2 game controllers"
-version = "1.2.0"
+version = "1.2.1"
 readme = "README.rst"
 authors = [
     {name = "Tod Kurt", email = "tod@todbot.com"}
 ]
 urls = {Homepage = "https://github.com/todbot/CircuitPython_PS2Controller"}
 keywords = [
     "adafruit",
```

