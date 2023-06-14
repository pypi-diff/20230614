# Comparing `tmp/srecli-0.0.6.tar.gz` & `tmp/srecli-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srecli-0.0.6.tar", last modified: Mon May 29 15:58:11 2023, max compression
+gzip compressed data, was "srecli-0.0.7.tar", last modified: Wed Jun 14 03:54:18 2023, max compression
```

## Comparing `srecli-0.0.6.tar` & `srecli-0.0.7.tar`

### file list

```diff
@@ -1,30 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:58:11.803555 srecli-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:58:11.803555 srecli-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:58:11.803555 srecli-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-05-29 15:58:00.000000 srecli-0.0.6/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-29 15:58:00.000000 srecli-0.0.6/.github/workflows/pypi_publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-29 15:58:00.000000 srecli-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-29 15:58:00.000000 srecli-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-29 15:58:11.803555 srecli-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-29 15:58:00.000000 srecli-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-29 15:58:00.000000 srecli-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-29 15:58:00.000000 srecli-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 15:58:11.803555 srecli-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-29 15:58:00.000000 srecli-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:58:11.803555 srecli-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:58:11.803555 srecli-0.0.6/src/srecli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:58:00.000000 srecli-0.0.6/src/srecli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-29 15:58:00.000000 srecli-0.0.6/src/srecli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:58:11.803555 srecli-0.0.6/src/srecli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:58:00.000000 srecli-0.0.6/src/srecli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-29 15:58:00.000000 srecli-0.0.6/src/srecli/commands/cmd_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:58:11.803555 srecli-0.0.6/src/srecli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-29 15:58:11.000000 srecli-0.0.6/src/srecli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-29 15:58:11.000000 srecli-0.0.6/src/srecli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 15:58:11.000000 srecli-0.0.6/src/srecli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-29 15:58:11.000000 srecli-0.0.6/src/srecli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-29 15:58:11.000000 srecli-0.0.6/src/srecli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 15:58:11.000000 srecli-0.0.6/src/srecli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:58:11.803555 srecli-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:58:00.000000 srecli-0.0.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-29 15:58:00.000000 srecli-0.0.6/tests/test_status_show.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:54:18.146398 srecli-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:54:18.138398 srecli-0.0.7/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-14 03:54:00.000000 srecli-0.0.7/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:54:18.138398 srecli-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-06-14 03:54:00.000000 srecli-0.0.7/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-14 03:54:00.000000 srecli-0.0.7/.github/workflows/pypi_publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-14 03:54:00.000000 srecli-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-14 03:54:00.000000 srecli-0.0.7/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-14 03:54:00.000000 srecli-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-14 03:54:18.142398 srecli-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-14 03:54:00.000000 srecli-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:54:18.142398 srecli-0.0.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-14 03:54:00.000000 srecli-0.0.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-14 03:54:00.000000 srecli-0.0.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-14 03:54:00.000000 srecli-0.0.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-14 03:54:00.000000 srecli-0.0.7/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:54:18.142398 srecli-0.0.7/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-14 03:54:00.000000 srecli-0.0.7/docs/reference/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-14 03:54:00.000000 srecli-0.0.7/docs/reference/srecli.cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-14 03:54:00.000000 srecli-0.0.7/docs/reference/srecli.commands.cmd_status.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-14 03:54:00.000000 srecli-0.0.7/docs/reference/srecli.commands.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-14 03:54:00.000000 srecli-0.0.7/docs/reference/srecli.options.common.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-14 03:54:00.000000 srecli-0.0.7/docs/reference/srecli.options.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-14 03:54:00.000000 srecli-0.0.7/docs/reference/srecli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-14 03:54:00.000000 srecli-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-14 03:54:00.000000 srecli-0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 03:54:18.146398 srecli-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-14 03:54:00.000000 srecli-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:54:18.138398 srecli-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:54:18.142398 srecli-0.0.7/src/srecli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 03:54:00.000000 srecli-0.0.7/src/srecli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-14 03:54:00.000000 srecli-0.0.7/src/srecli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:54:18.142398 srecli-0.0.7/src/srecli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 03:54:00.000000 srecli-0.0.7/src/srecli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-14 03:54:00.000000 srecli-0.0.7/src/srecli/commands/cmd_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:54:18.142398 srecli-0.0.7/src/srecli/options/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 03:54:00.000000 srecli-0.0.7/src/srecli/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-14 03:54:00.000000 srecli-0.0.7/src/srecli/options/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:54:18.142398 srecli-0.0.7/src/srecli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-14 03:54:18.000000 srecli-0.0.7/src/srecli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-14 03:54:18.000000 srecli-0.0.7/src/srecli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 03:54:18.000000 srecli-0.0.7/src/srecli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-14 03:54:18.000000 srecli-0.0.7/src/srecli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-14 03:54:18.000000 srecli-0.0.7/src/srecli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 03:54:18.000000 srecli-0.0.7/src/srecli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:54:18.142398 srecli-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 03:54:00.000000 srecli-0.0.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-14 03:54:00.000000 srecli-0.0.7/tests/test_status_show.py
```

### Comparing `srecli-0.0.6/.github/workflows/build.yaml` & `srecli-0.0.7/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `srecli-0.0.6/.github/workflows/pypi_publish.yaml` & `srecli-0.0.7/.github/workflows/pypi_publish.yaml`

 * *Files identical despite different names*

### Comparing `srecli-0.0.6/.gitignore` & `srecli-0.0.7/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -155,7 +155,10 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
+#
+src/version.py
+src/_version.py
```

### Comparing `srecli-0.0.6/LICENSE` & `srecli-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `srecli-0.0.6/PKG-INFO` & `srecli-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: srecli
-Version: 0.0.6
-Summary: CLI tool for common SRE related work
+Version: 0.0.7
+Summary: srecli is a click based CLI tool to cater common SRE related system automation tasks.
 Author-email: Shibhikkiran D <shibhikkiran@example.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `srecli-0.0.6/README.md` & `srecli-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `srecli-0.0.6/pyproject.toml` & `srecli-0.0.7/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [project]
 name = "srecli"
-version = "0.0.6"
-description = "CLI tool for common SRE related work"
+#version = "0.0.6"
+dynamic = ["version"]
+description = "srecli is a click based CLI tool to cater common SRE related system automation tasks."
 authors = [
     {name = "Shibhikkiran D", email = "shibhikkiran@example.com"},
 ]
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -18,20 +19,27 @@
 ]
 
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = [
     "setuptools ~=63.2.0",
     "wheel ~=0.37.1",
-    "setuptools_scm[toml]",
+    "setuptools_scm[toml] ~=7.1.0",
 ]
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
+
+[tool.setuptools_scm]
+write_to = "src/_version.py"
+version_scheme = "python-simplified-semver"
+local_scheme = "no-local-version"
+
+
 [project.scripts]
 srecli = 'srecli.cli:cli'
 
 [project.optional-dependencies]
 dev = [
     "pylint ~=2.14.0",
     "toml ~=0.10.2",
@@ -89,14 +97,15 @@
     env_list =
         py310
         py39
         py38
         typecheck
         format 
         lint
+        docs
 
     [testenv]
     deps = 
         pytest
         pytest-cov
     commands = pytest tests
 
@@ -116,8 +125,27 @@
     [testenv:lint]
     skip_install = True
     deps =
         flake8
         flake8-bugbear
     commands =
         flake8 --extend-ignore E501 --exclude .tox,.git,__pycache__docs,build,dist --show-source --statistics {posargs:src tests}
+
+    [testenv:docs]
+    deps =
+        importlib
+        sphinx
+        sphinx-nested-apidoc
+    commands =
+        sphinx-apidoc --force --implicit-namespaces --module-first --separate -o docs/reference/ src/srecli src/srecli/*.c src/srecli/*.so
+        sphinx-build -n --keep-going -b html docs/ docs/_build/
+
+    [testenv:devdocs]
+    deps =
+        importlib
+        sphinx
+        sphinx-nested-apidoc
+        sphinx-autobuild
+    commands =
+        sphinx-apidoc --force --implicit-namespaces --module-first --separate -o docs/reference/ src/srecli src/srecli/*.c src/srecli/*.so
+        sphinx-autobuild -n -b html --port 9876 docs/ docs/_build/
 """
```

### Comparing `srecli-0.0.6/src/srecli.egg-info/PKG-INFO` & `srecli-0.0.7/src/srecli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: srecli
-Version: 0.0.6
-Summary: CLI tool for common SRE related work
+Version: 0.0.7
+Summary: srecli is a click based CLI tool to cater common SRE related system automation tasks.
 Author-email: Shibhikkiran D <shibhikkiran@example.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `srecli-0.0.6/tests/test_status_show.py` & `srecli-0.0.7/tests/test_status_show.py`

 * *Files identical despite different names*

