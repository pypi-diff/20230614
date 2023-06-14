# Comparing `tmp/ib2influx-0.9.tar.gz` & `tmp/ib2influx-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ib2influx-0.9.tar", last modified: Wed Jan  4 02:29:20 2023, max compression
+gzip compressed data, was "ib2influx-1.1.0.tar", last modified: Wed Jun 14 07:02:06 2023, max compression
```

## Comparing `ib2influx-0.9.tar` & `ib2influx-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 02:29:20.194037 ib2influx-0.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 02:29:20.190037 ib2influx-0.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 02:29:20.190037 ib2influx-0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-01-04 02:29:10.000000 ib2influx-0.9/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-01-04 02:29:10.000000 ib2influx-0.9/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-04 02:29:10.000000 ib2influx-0.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-01-04 02:29:10.000000 ib2influx-0.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-04 02:29:10.000000 ib2influx-0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-01-04 02:29:20.194037 ib2influx-0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-01-04 02:29:10.000000 ib2influx-0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-01-04 02:29:10.000000 ib2influx-0.9/config_example.yml
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-01-04 02:29:10.000000 ib2influx-0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-01-04 02:29:20.194037 ib2influx-0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 02:29:20.190037 ib2influx-0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 02:29:20.194037 ib2influx-0.9/src/ib2influx/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-04 02:29:10.000000 ib2influx-0.9/src/ib2influx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-01-04 02:29:10.000000 ib2influx-0.9/src/ib2influx/loader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      411 2023-01-04 02:29:10.000000 ib2influx-0.9/src/ib2influx/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-01-04 02:29:10.000000 ib2influx-0.9/src/ib2influx/opa.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-01-04 02:29:10.000000 ib2influx-0.9/src/ib2influx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 02:29:20.194037 ib2influx-0.9/src/ib2influx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-01-04 02:29:20.000000 ib2influx-0.9/src/ib2influx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-01-04 02:29:20.000000 ib2influx-0.9/src/ib2influx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-04 02:29:20.000000 ib2influx-0.9/src/ib2influx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-04 02:29:20.000000 ib2influx-0.9/src/ib2influx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-01-04 02:29:20.000000 ib2influx-0.9/src/ib2influx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-04 02:29:20.000000 ib2influx-0.9/src/ib2influx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:02:06.948424 ib2influx-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:02:06.944424 ib2influx-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:02:06.944424 ib2influx-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-14 07:01:55.000000 ib2influx-1.1.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-14 07:01:55.000000 ib2influx-1.1.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-14 07:01:55.000000 ib2influx-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-14 07:01:55.000000 ib2influx-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-14 07:01:55.000000 ib2influx-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-14 07:02:06.948424 ib2influx-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-14 07:01:55.000000 ib2influx-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-14 07:01:55.000000 ib2influx-1.1.0/config_example.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-14 07:01:55.000000 ib2influx-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-14 07:02:06.948424 ib2influx-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:02:06.944424 ib2influx-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:02:06.948424 ib2influx-1.1.0/src/ib2influx/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-14 07:01:55.000000 ib2influx-1.1.0/src/ib2influx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-14 07:01:55.000000 ib2influx-1.1.0/src/ib2influx/loader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      881 2023-06-14 07:01:55.000000 ib2influx-1.1.0/src/ib2influx/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-06-14 07:01:55.000000 ib2influx-1.1.0/src/ib2influx/mlx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-14 07:01:55.000000 ib2influx-1.1.0/src/ib2influx/opa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-14 07:01:55.000000 ib2influx-1.1.0/src/ib2influx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:02:06.948424 ib2influx-1.1.0/src/ib2influx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-14 07:02:06.000000 ib2influx-1.1.0/src/ib2influx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-14 07:02:06.000000 ib2influx-1.1.0/src/ib2influx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 07:02:06.000000 ib2influx-1.1.0/src/ib2influx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-14 07:02:06.000000 ib2influx-1.1.0/src/ib2influx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-14 07:02:06.000000 ib2influx-1.1.0/src/ib2influx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-14 07:02:06.000000 ib2influx-1.1.0/src/ib2influx.egg-info/top_level.txt
```

### Comparing `ib2influx-0.9/.github/workflows/publish.yml` & `ib2influx-1.1.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `ib2influx-0.9/.pre-commit-config.yaml` & `ib2influx-1.1.0/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 ---
 
 repos:
   - repo: https://github.com/ambv/black
-    rev: 22.12.0
+    rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/PyCQA/flake8
     rev: 6.0.0
     hooks:
       - id: flake8
 
   - repo: https://github.com/adrienverge/yamllint
-    rev: v1.28.0
+    rev: v1.32.0
     hooks:
       - id: yamllint
         args: ['-d relaxed']
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: check-merge-conflict
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.11.2
+    rev: 5.12.0
     hooks:
       - id: isort
```

### Comparing `ib2influx-0.9/LICENSE` & `ib2influx-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ib2influx-0.9/PKG-INFO` & `ib2influx-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: ib2influx
-Version: 0.9
+Version: 1.1.0
 Summary: Collect IB statistics and push them to InfluxDB
 Author-email: Conrad Chan <conradchan@hotmail.com.au>
 Project-URL: Homepage, https://github.com/conradtchan/ib2influx
 Project-URL: Bug Tracker, https://github.com/conradtchan/ib2influx/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.11
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ib2influx
 Collect IB network measurements to InfluxDB
```

### Comparing `ib2influx-0.9/pyproject.toml` & `ib2influx-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "ib2influx"
 dynamic = ["version"]
 authors = [
     { name="Conrad Chan", email="conradchan@hotmail.com.au" },
 ]
 description = "Collect IB statistics and push them to InfluxDB"
 readme = "README.md"
-requires-python = ">=3.11"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
     "Development Status :: 4 - Beta",
 ]
 dependencies = [
```

### Comparing `ib2influx-0.9/src/ib2influx/loader.py` & `ib2influx-1.1.0/src/ib2influx/loader.py`

 * *Files identical despite different names*

### Comparing `ib2influx-0.9/src/ib2influx/opa.py` & `ib2influx-1.1.0/src/ib2influx/opa.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,15 +75,18 @@
                 data[host] = {}
 
                 for influx_key, opa_key in self.KEYS.items():
                     # Convert from string to int
                     value = int(row[key_col[opa_key]])
 
                     # Perform conversion and add to dict using the InfluxDB key
-                    data[host][influx_key] = self.convert_opa_units(value)
+                    if "Data" in opa_key:
+                        data[host][influx_key] = self.convert_opa_units(value)
+                    else:
+                        data[host][influx_key] = value
 
         return data
 
     @staticmethod
     def convert_opa_units(x):
         """
         opaextractperf's rates are in units of 8 bytes
```

### Comparing `ib2influx-0.9/src/ib2influx.egg-info/PKG-INFO` & `ib2influx-1.1.0/src/ib2influx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: ib2influx
-Version: 0.9
+Version: 1.1.0
 Summary: Collect IB statistics and push them to InfluxDB
 Author-email: Conrad Chan <conradchan@hotmail.com.au>
 Project-URL: Homepage, https://github.com/conradtchan/ib2influx
 Project-URL: Bug Tracker, https://github.com/conradtchan/ib2influx/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.11
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ib2influx
 Collect IB network measurements to InfluxDB
```

