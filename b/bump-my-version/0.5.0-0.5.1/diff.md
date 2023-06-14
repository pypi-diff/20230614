# Comparing `tmp/bump-my-version-0.5.0.tar.gz` & `tmp/bump-my-version-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bump-my-version-0.5.0.tar", last modified: Mon Jun 12 14:03:04 2023, max compression
+gzip compressed data, was "bump-my-version-0.5.1.tar", last modified: Wed Jun 14 15:03:24 2023, max compression
```

## Comparing `bump-my-version-0.5.0.tar` & `bump-my-version-0.5.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:03:04.421677 bump-my-version-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    13404 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-06-12 14:03:04.421677 bump-my-version-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:03:04.417677 bump-my-version-0.5.0/bump_my_version.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-06-12 14:03:04.000000 bump-my-version-0.5.0/bump_my_version.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-12 14:03:04.000000 bump-my-version-0.5.0/bump_my_version.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 14:03:04.000000 bump-my-version-0.5.0/bump_my_version.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-12 14:03:04.000000 bump-my-version-0.5.0/bump_my_version.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-12 14:03:04.000000 bump-my-version-0.5.0/bump_my_version.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-12 14:03:04.000000 bump-my-version-0.5.0/bump_my_version.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:03:04.421677 bump-my-version-0.5.0/bumpversion/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/bumpversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/bumpversion/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/bumpversion/aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/bumpversion/autocast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/bumpversion/bump.py
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/bumpversion/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/bumpversion/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/bumpversion/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/bumpversion/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/bumpversion/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/bumpversion/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/bumpversion/scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/bumpversion/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/bumpversion/version_part.py
--rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-12 14:03:04.421677 bump-my-version-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:03:04.421677 bump-my-version-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:03:04.421677 bump-my-version-0.5.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/fixtures/basic_cfg.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/fixtures/basic_cfg.toml
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/fixtures/basic_cfg_expected.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:03:04.421677 bump-my-version-0.5.0/tests/fixtures/glob/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:03:04.421677 bump-my-version-0.5.0/tests/fixtures/glob/directory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/fixtures/glob/directory/file3.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/fixtures/glob/file1.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/fixtures/glob/file2.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/fixtures/glob/not-text.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:03:04.421677 bump-my-version-0.5.0/tests/fixtures/interpolation/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/fixtures/interpolation/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/fixtures/interpolation/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/fixtures/interpolation/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/test_autocast.py
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/test_bump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9844 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13258 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-06-12 14:02:44.000000 bump-my-version-0.5.0/tests/test_version_part.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:03:24.470339 bump-my-version-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    14356 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-06-14 15:03:24.470339 bump-my-version-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:03:24.466339 bump-my-version-0.5.1/bump_my_version.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-06-14 15:03:24.000000 bump-my-version-0.5.1/bump_my_version.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-14 15:03:24.000000 bump-my-version-0.5.1/bump_my_version.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 15:03:24.000000 bump-my-version-0.5.1/bump_my_version.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-14 15:03:24.000000 bump-my-version-0.5.1/bump_my_version.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-14 15:03:24.000000 bump-my-version-0.5.1/bump_my_version.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-14 15:03:24.000000 bump-my-version-0.5.1/bump_my_version.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:03:24.466339 bump-my-version-0.5.1/bumpversion/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/bumpversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/bumpversion/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/bumpversion/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/bumpversion/autocast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/bumpversion/bump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/bumpversion/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/bumpversion/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/bumpversion/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/bumpversion/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/bumpversion/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/bumpversion/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/bumpversion/scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/bumpversion/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/bumpversion/version_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-14 15:03:24.470339 bump-my-version-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:03:24.470339 bump-my-version-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:03:24.470339 bump-my-version-0.5.1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/tests/fixtures/basic_cfg.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/tests/fixtures/basic_cfg.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/tests/fixtures/basic_cfg_expected.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:03:24.470339 bump-my-version-0.5.1/tests/fixtures/glob/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:03:24.470339 bump-my-version-0.5.1/tests/fixtures/glob/directory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/tests/fixtures/glob/directory/file3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/tests/fixtures/glob/file1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/tests/fixtures/glob/file2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/tests/fixtures/glob/not-text.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:03:24.470339 bump-my-version-0.5.1/tests/fixtures/interpolation/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/tests/fixtures/interpolation/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/tests/fixtures/interpolation/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/tests/fixtures/interpolation/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/tests/test_autocast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/tests/test_bump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9844 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-06-14 15:03:04.000000 bump-my-version-0.5.1/tests/test_version_part.py
```

### Comparing `bump-my-version-0.5.0/CHANGELOG.md` & `bump-my-version-0.5.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,28 @@
 # Changelog
 
+## 0.5.1 (2023-06-14)
+[Compare the full difference.](https://github.com/callowayproject/bump-my-version/compare/0.5.0...0.5.1)
+
+### Fixes
+
+- Fixes reporting the wrong version missing in a file. [efb04e9](https://github.com/callowayproject/bump-my-version/commit/efb04e94a07fa886253bbfc9cf801040e4c03895)
+    
+  - Fixes issue #20
+  - Renders the correct `current_version` for each file being modified.
+### Other
+
+- [pre-commit.ci] auto fixes from pre-commit.com hooks. [5476cdf](https://github.com/callowayproject/bump-my-version/commit/5476cdf8b66666e06e9bfd4d71eaf2610103079a)
+    
+  for more information, see https://pre-commit.ci
+- [pre-commit.ci] pre-commit autoupdate. [6e500c2](https://github.com/callowayproject/bump-my-version/commit/6e500c24592f1688cbb13d3fcb6071aa0815ffe8)
+    
+  **updates:** - [github.com/charliermarsh/ruff-pre-commit: v0.0.270 → v0.0.272](https://github.com/charliermarsh/ruff-pre-commit/compare/v0.0.270...v0.0.272)
+
+
 ## 0.5.0 (2023-06-12)
 [Compare the full difference.](https://github.com/callowayproject/bump-my-version/compare/0.4.1...0.5.0)
 
 ### Fixes
 
 - Fixed ruff complaints about subprocess. [c429c68](https://github.com/callowayproject/bump-my-version/commit/c429c682515455558095836cb108a93fa23aa67f)
```

### Comparing `bump-my-version-0.5.0/CODE_OF_CONDUCT.md` & `bump-my-version-0.5.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.5.0/CONTRIBUTING.md` & `bump-my-version-0.5.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.5.0/LICENSE` & `bump-my-version-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.5.0/PKG-INFO` & `bump-my-version-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bump-my-version
-Version: 0.5.0
+Version: 0.5.1
 Summary: Version bump your Python project
 Author-email: Corey Oordt <coreyoordt@gmail.com>
 License: MIT License
         
         Copyright (c) 2013-2014 Filip Noetzel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `bump-my-version-0.5.0/README.md` & `bump-my-version-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.5.0/bump_my_version.egg-info/PKG-INFO` & `bump-my-version-0.5.1/bump_my_version.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bump-my-version
-Version: 0.5.0
+Version: 0.5.1
 Summary: Version bump your Python project
 Author-email: Corey Oordt <coreyoordt@gmail.com>
 License: MIT License
         
         Copyright (c) 2013-2014 Filip Noetzel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `bump-my-version-0.5.0/bump_my_version.egg-info/SOURCES.txt` & `bump-my-version-0.5.1/bump_my_version.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.5.0/bumpversion/aliases.py` & `bump-my-version-0.5.1/bumpversion/aliases.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.5.0/bumpversion/autocast.py` & `bump-my-version-0.5.1/bumpversion/autocast.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.5.0/bumpversion/bump.py` & `bump-my-version-0.5.1/bumpversion/bump.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.5.0/bumpversion/cli.py` & `bump-my-version-0.5.1/bumpversion/cli.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.5.0/bumpversion/config.py` & `bump-my-version-0.5.1/bumpversion/config.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.5.0/bumpversion/exceptions.py` & `bump-my-version-0.5.1/bumpversion/exceptions.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.5.0/bumpversion/files.py` & `bump-my-version-0.5.1/bumpversion/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,8 +205,9 @@
 ) -> None:
     """Make sure files exist and contain version string."""
     logger.info(
         "Asserting files %s contain the version string...",
         ", ".join({str(f.path) for f in files}),
     )
     for f in files:
+        context["current_version"] = f.version_config.serialize(current_version, context)
         f.contains_version(current_version, context)
```

### Comparing `bump-my-version-0.5.0/bumpversion/functions.py` & `bump-my-version-0.5.1/bumpversion/functions.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.5.0/bumpversion/logging.py` & `bump-my-version-0.5.1/bumpversion/logging.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.5.0/bumpversion/scm.py` & `bump-my-version-0.5.1/bumpversion/scm.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.5.0/bumpversion/utils.py` & `bump-my-version-0.5.1/bumpversion/utils.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.5.0/bumpversion/version_part.py` & `bump-my-version-0.5.1/bumpversion/version_part.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,15 +224,15 @@
         try:
             # test whether all parts required in the format have values
             serialized = serialize_format.format(**values)
 
         except KeyError as e:
             missing_key = getattr(e, "message", e.args[0])
             raise MissingValueError(
-                f"Did not find key {missing_key!r} in {repr(version)} when serializing version number"
+                f"Did not find key {missing_key!r} in {version!r} when serializing version number"
             ) from e
 
         keys_needing_representation = set()
 
         keys = list(self.order)
         for i, k in enumerate(keys):
             v = values[k]
```

### Comparing `bump-my-version-0.5.0/pyproject.toml` & `bump-my-version-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,15 @@
 [tool.ruff.isort]
 order-by-type = true
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.bumpversion]
-current_version = "0.5.0"
+current_version = "0.5.1"
 commit = true
 commit_args = "--no-verify"
 tag = true
 tag_name = "{new_version}"
 allow_dirty = true
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)(\\.(?P<dev>dev\\d+))?"
 serialize = [
```

### Comparing `bump-my-version-0.5.0/tests/conftest.py` & `bump-my-version-0.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.5.0/tests/fixtures/basic_cfg.cfg` & `bump-my-version-0.5.1/tests/fixtures/basic_cfg.cfg`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.5.0/tests/fixtures/basic_cfg.toml` & `bump-my-version-0.5.1/tests/fixtures/basic_cfg.toml`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.5.0/tests/fixtures/basic_cfg_expected.json` & `bump-my-version-0.5.1/tests/fixtures/basic_cfg_expected.json`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.5.0/tests/test_autocast.py` & `bump-my-version-0.5.1/tests/test_autocast.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.5.0/tests/test_bump.py` & `bump-my-version-0.5.1/tests/test_bump.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.5.0/tests/test_cli.py` & `bump-my-version-0.5.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.5.0/tests/test_config.py` & `bump-my-version-0.5.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.5.0/tests/test_files.py` & `bump-my-version-0.5.1/tests/test_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from textwrap import dedent
 
 import pytest
 from pytest import param
 
 from bumpversion import exceptions, files
 from bumpversion.utils import get_context
+from bumpversion.exceptions import VersionNotFoundError
 from tests.conftest import get_config_data, inside_dir
 
 
 @pytest.mark.parametrize(
     ["glob_pattern", "file_list"],
     [
         param("*.txt", {Path("file1.txt"), Path("file2.txt")}, id="simple-glob"),
@@ -149,23 +150,23 @@
 
     assert full_vers_path.read_text() == "2.0.1"
     assert maj_vers_path.read_text() == "2"
     assert readme_path.read_text() == "MyAwesomeSoftware(TM) v2.0"
     assert build_num_path.read_text() == "2.0.1+jane+38945"
 
 
-def test_issue_14(tmp_path: Path):
+def test_raises_correct_missing_version_string(tmp_path: Path):
     full_vers_path = tmp_path / "FULL_VERSION.txt"
     full_vers_path.write_text("3.1.0-rc+build.1031")
     assembly_path = tmp_path / "AssemblyInfo.cs"
     assembly_path.write_text(
         '[assembly: AssemblyFileVersion("3.1.0-rc+build.1031")]\n' '[assembly: AssemblyVersion("3.1.1031.0")]'
     )
     csv_path = tmp_path / "Version.csv"
-    csv_path.write_text("1;3;1;0;rc;build.1031")
+    csv_path.write_text("1;3-1;0;rc;build.1031")
 
     overrides = {
         "current_version": "3.1.0-rc+build.1031",
         "parse": r"(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(-(?P<release>[0-9A-Za-z]+))?(\+build\.(?P<build>.[0-9A-Za-z]+))?",
         "serialize": ["{major}.{minor}.{patch}-{release}+build.{build}", "{major}.{minor}.{patch}+build.{build}"],
         "commit": True,
         "message": "Bump version: {current_version} -> {new_version}",
@@ -209,22 +210,19 @@
         },
     }
     conf, version_config, current_version = get_config_data(overrides)
     major_version = current_version.bump("patch", version_config.order)
 
     ctx = get_context(conf)
 
-    for file_cfg in conf.files:
-        cfg_file = files.ConfiguredFile(file_cfg, version_config)
-        cfg_file.replace_version(current_version, major_version, ctx)
+    configured_files = [files.ConfiguredFile(file_cfg, version_config) for file_cfg in conf.files]
 
-    assert full_vers_path.read_text() == "3.1.1-beta+build.1031"
-    expected = '[assembly: AssemblyFileVersion("3.1.1-beta+build.1031")]\n[assembly: AssemblyVersion("3.1.1031.1")]'
-    assert assembly_path.read_text() == expected
-    assert csv_path.read_text() == "1;3;1;1;beta;build.1031"
+    with pytest.raises(VersionNotFoundError) as e:
+        files.modify_files(configured_files, current_version, major_version, ctx)
+        assert e.message.startswith("Did not find '1;3;1;0;rc;build.1031'")
 
 
 def test_search_replace_to_avoid_updating_unconcerned_lines(tmp_path: Path):
     req_path = tmp_path / "requirements.txt"
     req_path.write_text("Django>=1.5.6,<1.6\nMyProject==1.5.6")
 
     changelog_path = tmp_path / "CHANGELOG.md"
```

### Comparing `bump-my-version-0.5.0/tests/test_functions.py` & `bump-my-version-0.5.1/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.5.0/tests/test_scm.py` & `bump-my-version-0.5.1/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `bump-my-version-0.5.0/tests/test_version_part.py` & `bump-my-version-0.5.1/tests/test_version_part.py`

 * *Files identical despite different names*

