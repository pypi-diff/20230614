# Comparing `tmp/pe-sunat-1.2.1.tar.gz` & `tmp/pe-sunat-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pe-sunat-1.2.1.tar", last modified: Tue Feb  7 21:08:32 2023, max compression
+gzip compressed data, was "pe-sunat-1.3.0.tar", last modified: Mon Feb 27 21:50:05 2023, max compression
```

## Comparing `pe-sunat-1.2.1.tar` & `pe-sunat-1.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 21:08:32.227755 pe-sunat-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-02-07 21:08:09.000000 pe-sunat-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      370 2023-02-07 21:08:09.000000 pe-sunat-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     5309 2023-02-07 21:08:32.227755 pe-sunat-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-02-07 21:08:09.000000 pe-sunat-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 21:08:32.227755 pe-sunat-1.2.1/cordada/
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-02-07 21:08:09.000000 pe-sunat-1.2.1/cordada/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 21:08:32.227755 pe-sunat-1.2.1/cordada/pe_sunat/
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-02-07 21:08:09.000000 pe-sunat-1.2.1/cordada/pe_sunat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-07 21:08:09.000000 pe-sunat-1.2.1/cordada/pe_sunat/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 21:08:32.227755 pe-sunat-1.2.1/cordada/pe_sunat/ruc/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-07 21:08:09.000000 pe-sunat-1.2.1/cordada/pe_sunat/ruc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      441 2023-02-07 21:08:09.000000 pe-sunat-1.2.1/cordada/pe_sunat/ruc/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     5634 2023-02-07 21:08:09.000000 pe-sunat-1.2.1/cordada/pe_sunat/ruc/entities.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-07 21:08:32.227755 pe-sunat-1.2.1/pe_sunat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5309 2023-02-07 21:08:32.000000 pe-sunat-1.2.1/pe_sunat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      382 2023-02-07 21:08:32.000000 pe-sunat-1.2.1/pe_sunat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-07 21:08:32.000000 pe-sunat-1.2.1/pe_sunat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-07 21:08:31.000000 pe-sunat-1.2.1/pe_sunat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-02-07 21:08:32.000000 pe-sunat-1.2.1/pe_sunat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      942 2023-02-07 21:08:32.227755 pe-sunat-1.2.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)       85 2023-02-07 21:08:09.000000 pe-sunat-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 21:50:05.182329 pe-sunat-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-02-27 21:49:35.000000 pe-sunat-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      370 2023-02-27 21:49:35.000000 pe-sunat-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6358 2023-02-27 21:50:05.182329 pe-sunat-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1826 2023-02-27 21:49:35.000000 pe-sunat-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 21:50:05.182329 pe-sunat-1.3.0/cordada/
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-02-27 21:49:35.000000 pe-sunat-1.3.0/cordada/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 21:50:05.182329 pe-sunat-1.3.0/cordada/pe_sunat/
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-02-27 21:49:35.000000 pe-sunat-1.3.0/cordada/pe_sunat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-27 21:49:35.000000 pe-sunat-1.3.0/cordada/pe_sunat/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 21:50:05.182329 pe-sunat-1.3.0/cordada/pe_sunat/ruc/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-27 21:49:35.000000 pe-sunat-1.3.0/cordada/pe_sunat/ruc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      441 2023-02-27 21:49:35.000000 pe-sunat-1.3.0/cordada/pe_sunat/ruc/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5634 2023-02-27 21:49:35.000000 pe-sunat-1.3.0/cordada/pe_sunat/ruc/entities.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 21:50:05.182329 pe-sunat-1.3.0/pe_sunat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6358 2023-02-27 21:50:05.000000 pe-sunat-1.3.0/pe_sunat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      382 2023-02-27 21:50:05.000000 pe-sunat-1.3.0/pe_sunat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-27 21:50:05.000000 pe-sunat-1.3.0/pe_sunat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-27 21:50:04.000000 pe-sunat-1.3.0/pe_sunat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-02-27 21:50:05.000000 pe-sunat-1.3.0/pe_sunat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      942 2023-02-27 21:50:05.182329 pe-sunat-1.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)       85 2023-02-27 21:49:35.000000 pe-sunat-1.3.0/setup.py
```

### Comparing `pe-sunat-1.2.1/LICENSE` & `pe-sunat-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pe-sunat-1.2.1/PKG-INFO` & `pe-sunat-1.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pe-sunat
-Version: 1.2.1
+Version: 1.3.0
 Summary: Python library for Superintendencia Nacional de Aduanas y de Administración Tributaria (SUNAT) of Peru.
 Home-page: https://github.com/cordada/lib-pe-sunat-python/
 Author: Cordada SpA
 Author-email: no-reply@cordada.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -26,18 +26,18 @@
 Tributaria* (SUNAT) of *Perú*.
 
 
 ## Dashboard
 
 ### Development
 
-| VCS Branch | Deployment Environment | VCS Repository | CI Status |
-| ---------- | ---------------------- | -------------- | --------- |
-| `develop` | Staging | [GitHub](https://github.com/cordada/lib-pe-sunat-python/tree/develop) | [![GitHub Actions](https://github.com/cordada/lib-pe-sunat-python/actions/workflows/ci.yaml/badge.svg?branch=develop)](https://github.com/cordada/lib-pe-sunat-python/actions/workflows/ci.yaml?query=branch:develop) |
-| `master` | Production | [GitHub](https://github.com/cordada/lib-pe-sunat-python/tree/master) | [![GitHub Actions](https://github.com/cordada/lib-pe-sunat-python/actions/workflows/ci.yaml/badge.svg?branch=master)](https://github.com/cordada/lib-pe-sunat-python/actions/workflows/ci.yaml?query=branch:master) |
+| VCS Branch | Deployment Environment | VCS Repository | CI/CD Status |
+| ---------- | ---------------------- | -------------- | ------------ |
+| `develop` | Staging | [GitHub](https://github.com/cordada/lib-pe-sunat-python/tree/develop) | [![GitHub Actions](https://github.com/cordada/lib-pe-sunat-python/actions/workflows/ci-cd.yaml/badge.svg?branch=develop)](https://github.com/cordada/lib-pe-sunat-python/actions/workflows/ci-cd.yaml?query=branch:develop) |
+| `master` | Production | [GitHub](https://github.com/cordada/lib-pe-sunat-python/tree/master) | [![GitHub Actions](https://github.com/cordada/lib-pe-sunat-python/actions/workflows/ci-cd.yaml/badge.svg?branch=master)](https://github.com/cordada/lib-pe-sunat-python/actions/workflows/ci-cd.yaml?query=branch:master) |
 
 
 | Code Climate | Project Analysis |
 | ------------ | ---------------- |
 | [![Maintainability](https://api.codeclimate.com/v1/badges/ede6619f0d7dc4a0f0bc/maintainability)](https://codeclimate.com/github/cordada/lib-pe-sunat-python/maintainability) | [Open Source Insights](https://deps.dev/pypi/pe-sunat) |
 
 
@@ -72,14 +72,32 @@
 
 ## Additional Documentation
 
 [Documentation](docs/)
 
 # Changelog
 
+## 1.3.0 (2023-02-27)
+
+- (PR #44, 2023-02-08) chore: bump tox from 3.27.1 to 4.4.4
+- (PR #46, 2023-02-08) chore: bump isort from 5.10.1 to 5.12.0
+- (PR #45, 2023-02-08) chore: bump black from 22.12.0 to 23.1.0
+- (PR #56, 2023-02-08) chore: bump cryptography from 38.0.3 to 39.0.1
+- (PR #43, 2023-02-09) chore: bump flake8 from 4.0.1 to 6.0.0
+- (PR #58, 2023-02-13) Improve Super-Linter GitHub Actions workflow
+- (PR #59, 2023-02-13) Add Make files to cache key used for Python dependencies in CI/CD
+- (PR #60, 2023-02-13) Get PyPI username from GitHub Actions variable instead of secret
+- (PR #61, 2023-02-13) Fix deprecation of GitHub Actions `set-output`
+- (PR #62, 2023-02-13) Pin versions of actions used in GitHub Actions workflows
+- (PR #63, 2023-02-13) Remove unnecessary permissions from GitHub Actions workflows
+- (PR #66, 2023-02-13) Update CI/CD information in readme
+- (PR #65, 2023-02-17) chore: bump tox from 4.4.4 to 4.4.5
+- (PR #67, 2023-02-19) Change cache key of release & deploy workflows to match CI workflow
+
+
 ## 1.2.1 (2023-02-07)
 
 - (PR #31, 2023-01-26) chore: bump certifi from 2022.6.15 to 2022.12.7
 - (PR #40, 2023-01-26) Add GitHub Dependency Review
 - (PR #34, 2023-01-26) chore: bump black from 22.10.0 to 22.12.0
 - (PR #41, 2023-01-26) Improve GitHub Dependency Review
 - (PR #42, 2023-01-27) Update Markdownlint configuration
```

### Comparing `pe-sunat-1.2.1/README.md` & `pe-sunat-1.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 Tributaria* (SUNAT) of *Perú*.
 
 
 ## Dashboard
 
 ### Development
 
-| VCS Branch | Deployment Environment | VCS Repository | CI Status |
-| ---------- | ---------------------- | -------------- | --------- |
-| `develop` | Staging | [GitHub](https://github.com/cordada/lib-pe-sunat-python/tree/develop) | [![GitHub Actions](https://github.com/cordada/lib-pe-sunat-python/actions/workflows/ci.yaml/badge.svg?branch=develop)](https://github.com/cordada/lib-pe-sunat-python/actions/workflows/ci.yaml?query=branch:develop) |
-| `master` | Production | [GitHub](https://github.com/cordada/lib-pe-sunat-python/tree/master) | [![GitHub Actions](https://github.com/cordada/lib-pe-sunat-python/actions/workflows/ci.yaml/badge.svg?branch=master)](https://github.com/cordada/lib-pe-sunat-python/actions/workflows/ci.yaml?query=branch:master) |
+| VCS Branch | Deployment Environment | VCS Repository | CI/CD Status |
+| ---------- | ---------------------- | -------------- | ------------ |
+| `develop` | Staging | [GitHub](https://github.com/cordada/lib-pe-sunat-python/tree/develop) | [![GitHub Actions](https://github.com/cordada/lib-pe-sunat-python/actions/workflows/ci-cd.yaml/badge.svg?branch=develop)](https://github.com/cordada/lib-pe-sunat-python/actions/workflows/ci-cd.yaml?query=branch:develop) |
+| `master` | Production | [GitHub](https://github.com/cordada/lib-pe-sunat-python/tree/master) | [![GitHub Actions](https://github.com/cordada/lib-pe-sunat-python/actions/workflows/ci-cd.yaml/badge.svg?branch=master)](https://github.com/cordada/lib-pe-sunat-python/actions/workflows/ci-cd.yaml?query=branch:master) |
 
 
 | Code Climate | Project Analysis |
 | ------------ | ---------------- |
 | [![Maintainability](https://api.codeclimate.com/v1/badges/ede6619f0d7dc4a0f0bc/maintainability)](https://codeclimate.com/github/cordada/lib-pe-sunat-python/maintainability) | [Open Source Insights](https://deps.dev/pypi/pe-sunat) |
```

### Comparing `pe-sunat-1.2.1/cordada/pe_sunat/ruc/entities.py` & `pe-sunat-1.3.0/cordada/pe_sunat/ruc/entities.py`

 * *Files identical despite different names*

### Comparing `pe-sunat-1.2.1/pe_sunat.egg-info/PKG-INFO` & `pe-sunat-1.3.0/pe_sunat.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pe-sunat
-Version: 1.2.1
+Version: 1.3.0
 Summary: Python library for Superintendencia Nacional de Aduanas y de Administración Tributaria (SUNAT) of Peru.
 Home-page: https://github.com/cordada/lib-pe-sunat-python/
 Author: Cordada SpA
 Author-email: no-reply@cordada.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -26,18 +26,18 @@
 Tributaria* (SUNAT) of *Perú*.
 
 
 ## Dashboard
 
 ### Development
 
-| VCS Branch | Deployment Environment | VCS Repository | CI Status |
-| ---------- | ---------------------- | -------------- | --------- |
-| `develop` | Staging | [GitHub](https://github.com/cordada/lib-pe-sunat-python/tree/develop) | [![GitHub Actions](https://github.com/cordada/lib-pe-sunat-python/actions/workflows/ci.yaml/badge.svg?branch=develop)](https://github.com/cordada/lib-pe-sunat-python/actions/workflows/ci.yaml?query=branch:develop) |
-| `master` | Production | [GitHub](https://github.com/cordada/lib-pe-sunat-python/tree/master) | [![GitHub Actions](https://github.com/cordada/lib-pe-sunat-python/actions/workflows/ci.yaml/badge.svg?branch=master)](https://github.com/cordada/lib-pe-sunat-python/actions/workflows/ci.yaml?query=branch:master) |
+| VCS Branch | Deployment Environment | VCS Repository | CI/CD Status |
+| ---------- | ---------------------- | -------------- | ------------ |
+| `develop` | Staging | [GitHub](https://github.com/cordada/lib-pe-sunat-python/tree/develop) | [![GitHub Actions](https://github.com/cordada/lib-pe-sunat-python/actions/workflows/ci-cd.yaml/badge.svg?branch=develop)](https://github.com/cordada/lib-pe-sunat-python/actions/workflows/ci-cd.yaml?query=branch:develop) |
+| `master` | Production | [GitHub](https://github.com/cordada/lib-pe-sunat-python/tree/master) | [![GitHub Actions](https://github.com/cordada/lib-pe-sunat-python/actions/workflows/ci-cd.yaml/badge.svg?branch=master)](https://github.com/cordada/lib-pe-sunat-python/actions/workflows/ci-cd.yaml?query=branch:master) |
 
 
 | Code Climate | Project Analysis |
 | ------------ | ---------------- |
 | [![Maintainability](https://api.codeclimate.com/v1/badges/ede6619f0d7dc4a0f0bc/maintainability)](https://codeclimate.com/github/cordada/lib-pe-sunat-python/maintainability) | [Open Source Insights](https://deps.dev/pypi/pe-sunat) |
 
 
@@ -72,14 +72,32 @@
 
 ## Additional Documentation
 
 [Documentation](docs/)
 
 # Changelog
 
+## 1.3.0 (2023-02-27)
+
+- (PR #44, 2023-02-08) chore: bump tox from 3.27.1 to 4.4.4
+- (PR #46, 2023-02-08) chore: bump isort from 5.10.1 to 5.12.0
+- (PR #45, 2023-02-08) chore: bump black from 22.12.0 to 23.1.0
+- (PR #56, 2023-02-08) chore: bump cryptography from 38.0.3 to 39.0.1
+- (PR #43, 2023-02-09) chore: bump flake8 from 4.0.1 to 6.0.0
+- (PR #58, 2023-02-13) Improve Super-Linter GitHub Actions workflow
+- (PR #59, 2023-02-13) Add Make files to cache key used for Python dependencies in CI/CD
+- (PR #60, 2023-02-13) Get PyPI username from GitHub Actions variable instead of secret
+- (PR #61, 2023-02-13) Fix deprecation of GitHub Actions `set-output`
+- (PR #62, 2023-02-13) Pin versions of actions used in GitHub Actions workflows
+- (PR #63, 2023-02-13) Remove unnecessary permissions from GitHub Actions workflows
+- (PR #66, 2023-02-13) Update CI/CD information in readme
+- (PR #65, 2023-02-17) chore: bump tox from 4.4.4 to 4.4.5
+- (PR #67, 2023-02-19) Change cache key of release & deploy workflows to match CI workflow
+
+
 ## 1.2.1 (2023-02-07)
 
 - (PR #31, 2023-01-26) chore: bump certifi from 2022.6.15 to 2022.12.7
 - (PR #40, 2023-01-26) Add GitHub Dependency Review
 - (PR #34, 2023-01-26) chore: bump black from 22.10.0 to 22.12.0
 - (PR #41, 2023-01-26) Improve GitHub Dependency Review
 - (PR #42, 2023-01-27) Update Markdownlint configuration
```

### Comparing `pe-sunat-1.2.1/setup.cfg` & `pe-sunat-1.3.0/setup.cfg`

 * *Files identical despite different names*

