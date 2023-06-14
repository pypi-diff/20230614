# Comparing `tmp/prolint2-0.0.7.tar.gz` & `tmp/prolint2-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prolint2-0.0.7.tar", last modified: Mon Feb 27 20:17:41 2023, max compression
+gzip compressed data, was "prolint2-0.0.8.tar", last modified: Mon Mar 27 21:45:22 2023, max compression
```

## Comparing `prolint2-0.0.7.tar` & `prolint2-0.0.8.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:17:41.090980 prolint2-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-02-27 20:17:32.000000 prolint2-0.0.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-02-27 20:17:32.000000 prolint2-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-27 20:17:32.000000 prolint2-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-02-27 20:17:41.090980 prolint2-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-02-27 20:17:32.000000 prolint2-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:17:41.078980 prolint2-0.0.7/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3209 2023-02-27 20:17:32.000000 prolint2-0.0.7/bin/prolint2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:17:41.094980 prolint2-0.0.7/prolint2/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-02-27 20:17:32.000000 prolint2-0.0.7/prolint2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-27 20:17:41.094980 prolint2-0.0.7/prolint2/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-02-27 20:17:32.000000 prolint2-0.0.7/prolint2/config.ini
--rw-r--r--   0 runner    (1001) docker     (123)    16840 2023-02-27 20:17:32.000000 prolint2-0.0.7/prolint2/contacts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:17:41.082980 prolint2-0.0.7/prolint2/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-02-27 20:17:32.000000 prolint2-0.0.7/prolint2/data/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)  1643625 2023-02-27 20:17:32.000000 prolint2-0.0.7/prolint2/data/coordinates.gro
--rw-r--r--   0 runner    (1001) docker     (123)   966276 2023-02-27 20:17:32.000000 prolint2-0.0.7/prolint2/data/trajectory.xtc
--rw-r--r--   0 runner    (1001) docker     (123)    13222 2023-02-27 20:17:32.000000 prolint2-0.0.7/prolint2/interactive_sel.py
--rw-r--r--   0 runner    (1001) docker     (123)    12908 2023-02-27 20:17:32.000000 prolint2-0.0.7/prolint2/prolint2.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-02-27 20:17:32.000000 prolint2-0.0.7/prolint2/sampledata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:17:41.082980 prolint2-0.0.7/prolint2/server/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-02-27 20:17:32.000000 prolint2-0.0.7/prolint2/server/app.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     9469 2023-02-27 20:17:32.000000 prolint2-0.0.7/prolint2/server/chord_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-02-27 20:17:32.000000 prolint2-0.0.7/prolint2/server/get_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    71086 2023-02-27 20:17:32.000000 prolint2-0.0.7/prolint2/server/girk.json
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-02-27 20:17:32.000000 prolint2-0.0.7/prolint2/server/home.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-02-27 20:17:32.000000 prolint2-0.0.7/prolint2/server/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    12153 2023-02-27 20:17:32.000000 prolint2-0.0.7/prolint2/server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:17:41.078980 prolint2-0.0.7/prolint2/server/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:17:41.086980 prolint2-0.0.7/prolint2/server/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-02-27 20:17:32.000000 prolint2-0.0.7/prolint2/server/static/css/main.css
--rw-r--r--   0 runner    (1001) docker     (123)    66916 2023-02-27 20:17:32.000000 prolint2-0.0.7/prolint2/server/static/css/pdbe-molstar-3.1.0_vendor.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:17:41.086980 prolint2-0.0.7/prolint2/server/static/images/
--rwxr-xr-x   0 runner    (1001) docker     (123)    12211 2023-02-27 20:17:32.000000 prolint2-0.0.7/prolint2/server/static/images/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:17:41.090980 prolint2-0.0.7/prolint2/server/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-02-27 20:17:32.000000 prolint2-0.0.7/prolint2/server/static/js/app.js
--rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-02-27 20:17:32.000000 prolint2-0.0.7/prolint2/server/static/js/ganttApp.js
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-02-27 20:17:32.000000 prolint2-0.0.7/prolint2/server/static/js/heatmapApp.js
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-02-27 20:17:32.000000 prolint2-0.0.7/prolint2/server/static/js/mol.js
--rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-02-27 20:17:32.000000 prolint2-0.0.7/prolint2/server/static/js/network.js
--rw-r--r--   0 runner    (1001) docker     (123)  4346110 2023-02-27 20:17:32.000000 prolint2-0.0.7/prolint2/server/static/js/pdbe-molstar-plugin-3.1.0_vendor.js
--rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-02-27 20:17:32.000000 prolint2-0.0.7/prolint2/server/static/js/pie.js
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-02-27 20:17:32.000000 prolint2-0.0.7/prolint2/server/static/js/radialApp.js
--rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-02-27 20:17:32.000000 prolint2-0.0.7/prolint2/server/static/js/table.js
--rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-02-27 20:17:32.000000 prolint2-0.0.7/prolint2/server/static/js/timeseries.js
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-02-27 20:17:32.000000 prolint2-0.0.7/prolint2/server/static/js/utils.js
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-02-27 20:17:32.000000 prolint2-0.0.7/prolint2/server/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:17:41.090980 prolint2-0.0.7/prolint2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-02-27 20:17:32.000000 prolint2-0.0.7/prolint2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-02-27 20:17:32.000000 prolint2-0.0.7/prolint2/tests/test_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-02-27 20:17:32.000000 prolint2-0.0.7/prolint2/tests/test_prolint2.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-02-27 20:17:32.000000 prolint2-0.0.7/prolint2/tests/test_sampledata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:17:41.078980 prolint2-0.0.7/prolint2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-02-27 20:17:41.000000 prolint2-0.0.7/prolint2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-02-27 20:17:41.000000 prolint2-0.0.7/prolint2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 20:17:41.000000 prolint2-0.0.7/prolint2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-27 20:17:41.000000 prolint2-0.0.7/prolint2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-27 20:17:41.000000 prolint2-0.0.7/prolint2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-02-27 20:17:41.094980 prolint2-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-02-27 20:17:32.000000 prolint2-0.0.7/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68277 2023-02-27 20:17:32.000000 prolint2-0.0.7/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:45:22.390018 prolint2-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-03-27 21:45:12.000000 prolint2-0.0.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-03-27 21:45:12.000000 prolint2-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-27 21:45:12.000000 prolint2-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-03-27 21:45:22.390018 prolint2-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-03-27 21:45:12.000000 prolint2-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:45:22.374018 prolint2-0.0.8/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3209 2023-03-27 21:45:12.000000 prolint2-0.0.8/bin/prolint2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:45:22.390018 prolint2-0.0.8/prolint2/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-27 21:45:22.390018 prolint2-0.0.8/prolint2/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    16840 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/contacts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:45:22.378018 prolint2-0.0.8/prolint2/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/data/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1643625 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/data/coordinates.gro
+-rw-r--r--   0 runner    (1001) docker     (123)   966276 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/data/trajectory.xtc
+-rw-r--r--   0 runner    (1001) docker     (123)    13222 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/interactive_sel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12908 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/prolint2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/sampledata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:45:22.382018 prolint2-0.0.8/prolint2/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/app.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     9469 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/chord_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/get_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71086 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/girk.json
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/home.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12153 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:45:22.374018 prolint2-0.0.8/prolint2/server/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:45:22.382018 prolint2-0.0.8/prolint2/server/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/static/css/main.css
+-rw-r--r--   0 runner    (1001) docker     (123)    66916 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/static/css/pdbe-molstar-3.1.0_vendor.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:45:22.382018 prolint2-0.0.8/prolint2/server/static/images/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12211 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/static/images/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:45:22.386018 prolint2-0.0.8/prolint2/server/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/static/js/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/static/js/ganttApp.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/static/js/heatmapApp.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/static/js/mol.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/static/js/network.js
+-rw-r--r--   0 runner    (1001) docker     (123)  4346110 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/static/js/pdbe-molstar-plugin-3.1.0_vendor.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/static/js/pie.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/static/js/radialApp.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/static/js/table.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/static/js/timeseries.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/static/js/utils.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/server/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:45:22.390018 prolint2-0.0.8/prolint2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/tests/test_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/tests/test_prolint2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-27 21:45:12.000000 prolint2-0.0.8/prolint2/tests/test_sampledata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:45:22.374018 prolint2-0.0.8/prolint2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-03-27 21:45:22.000000 prolint2-0.0.8/prolint2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-03-27 21:45:22.000000 prolint2-0.0.8/prolint2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 21:45:22.000000 prolint2-0.0.8/prolint2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-27 21:45:22.000000 prolint2-0.0.8/prolint2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-27 21:45:22.000000 prolint2-0.0.8/prolint2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-27 21:45:22.390018 prolint2-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-03-27 21:45:12.000000 prolint2-0.0.8/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68277 2023-03-27 21:45:12.000000 prolint2-0.0.8/versioneer.py
```

### Comparing `prolint2-0.0.7/CODE_OF_CONDUCT.md` & `prolint2-0.0.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/LICENSE` & `prolint2-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/PKG-INFO` & `prolint2-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prolint2
-Version: 0.0.7
+Version: 0.0.8
 Summary: ProLint2: Lipid-Protein Interaction Analysis.
 Home-page: https://github.com/ProLint/prolint2
 Author: Daniel P. Ramirez & Besian I. Sejdiu
 Author-email: daniel.ramirezecheme@ucalgary.ca
 License: MIT
 Platform: Linux
 Platform: Mac OS-X
```

### Comparing `prolint2-0.0.7/README.md` & `prolint2-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/bin/prolint2` & `prolint2-0.0.8/bin/prolint2`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/prolint2/__init__.py` & `prolint2-0.0.8/prolint2/__init__.py`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/prolint2/config.ini` & `prolint2-0.0.8/prolint2/config.ini`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/prolint2/contacts.py` & `prolint2-0.0.8/prolint2/contacts.py`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/prolint2/data/README.md` & `prolint2-0.0.8/prolint2/data/README.md`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/prolint2/data/coordinates.gro` & `prolint2-0.0.8/prolint2/data/coordinates.gro`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/prolint2/data/trajectory.xtc` & `prolint2-0.0.8/prolint2/data/trajectory.xtc`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/prolint2/interactive_sel.py` & `prolint2-0.0.8/prolint2/interactive_sel.py`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/prolint2/prolint2.py` & `prolint2-0.0.8/prolint2/prolint2.py`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/prolint2/sampledata.py` & `prolint2-0.0.8/prolint2/sampledata.py`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/prolint2/server/chord_utils.py` & `prolint2-0.0.8/prolint2/server/chord_utils.py`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/prolint2/server/get_json.py` & `prolint2-0.0.8/prolint2/server/get_json.py`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/prolint2/server/girk.json` & `prolint2-0.0.8/prolint2/server/girk.json`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/prolint2/server/index.html` & `prolint2-0.0.8/prolint2/server/index.html`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/prolint2/server/server.py` & `prolint2-0.0.8/prolint2/server/server.py`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/prolint2/server/static/css/main.css` & `prolint2-0.0.8/prolint2/server/static/css/main.css`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/prolint2/server/static/css/pdbe-molstar-3.1.0_vendor.css` & `prolint2-0.0.8/prolint2/server/static/css/pdbe-molstar-3.1.0_vendor.css`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/prolint2/server/static/images/logo.png` & `prolint2-0.0.8/prolint2/server/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/prolint2/server/static/js/app.js` & `prolint2-0.0.8/prolint2/server/static/js/app.js`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/prolint2/server/static/js/ganttApp.js` & `prolint2-0.0.8/prolint2/server/static/js/ganttApp.js`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/prolint2/server/static/js/heatmapApp.js` & `prolint2-0.0.8/prolint2/server/static/js/heatmapApp.js`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/prolint2/server/static/js/mol.js` & `prolint2-0.0.8/prolint2/server/static/js/mol.js`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/prolint2/server/static/js/network.js` & `prolint2-0.0.8/prolint2/server/static/js/network.js`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/prolint2/server/static/js/pdbe-molstar-plugin-3.1.0_vendor.js` & `prolint2-0.0.8/prolint2/server/static/js/pdbe-molstar-plugin-3.1.0_vendor.js`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/prolint2/server/static/js/pie.js` & `prolint2-0.0.8/prolint2/server/static/js/pie.js`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/prolint2/server/static/js/radialApp.js` & `prolint2-0.0.8/prolint2/server/static/js/radialApp.js`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/prolint2/server/static/js/table.js` & `prolint2-0.0.8/prolint2/server/static/js/table.js`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/prolint2/server/static/js/timeseries.js` & `prolint2-0.0.8/prolint2/server/static/js/timeseries.js`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/prolint2/server/static/js/utils.js` & `prolint2-0.0.8/prolint2/server/static/js/utils.js`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/prolint2/server/utils.py` & `prolint2-0.0.8/prolint2/server/utils.py`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/prolint2/tests/test_contacts.py` & `prolint2-0.0.8/prolint2/tests/test_contacts.py`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/prolint2/tests/test_prolint2.py` & `prolint2-0.0.8/prolint2/tests/test_prolint2.py`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/prolint2.egg-info/PKG-INFO` & `prolint2-0.0.8/prolint2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prolint2
-Version: 0.0.7
+Version: 0.0.8
 Summary: ProLint2: Lipid-Protein Interaction Analysis.
 Home-page: https://github.com/ProLint/prolint2
 Author: Daniel P. Ramirez & Besian I. Sejdiu
 Author-email: daniel.ramirezecheme@ucalgary.ca
 License: MIT
 Platform: Linux
 Platform: Mac OS-X
```

### Comparing `prolint2-0.0.7/prolint2.egg-info/SOURCES.txt` & `prolint2-0.0.8/prolint2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/setup.py` & `prolint2-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `prolint2-0.0.7/versioneer.py` & `prolint2-0.0.8/versioneer.py`

 * *Files identical despite different names*

