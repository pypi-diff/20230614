# Comparing `tmp/semver-3.0.0rc1.tar.gz` & `tmp/semver-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semver-3.0.0rc1.tar", last modified: Sun Mar 19 16:48:46 2023, max compression
+gzip compressed data, was "semver-3.0.1.tar", last modified: Wed Jun 14 11:43:01 2023, max compression
```

## Comparing `semver-3.0.0rc1.tar` & `semver-3.0.1.tar`

### file list

```diff
@@ -1,116 +1,118 @@
-drwxr-xr-x   0 tom       (1003) users      (100)        0 2023-03-19 16:48:46.593373 semver-3.0.0rc1/
--rw-r--r--   0 tom       (1003) users      (100)      229 2022-12-14 15:46:31.000000 semver-3.0.0rc1/.coveragerc
--rw-r--r--   0 tom       (1003) users      (100)      217 2023-02-22 12:09:12.000000 semver-3.0.0rc1/.editorconfig
--rw-r--r--   0 tom       (1003) users      (100)     4585 2023-03-07 06:55:28.000000 semver-3.0.0rc1/.gitignore
--rw-r--r--   0 tom       (1003) users      (100)    10356 2023-03-19 16:40:05.000000 semver-3.0.0rc1/CHANGELOG.rst
--rw-r--r--   0 tom       (1003) users      (100)     1891 2023-03-19 16:40:05.000000 semver-3.0.0rc1/CONTRIBUTING.rst
--rw-r--r--   0 tom       (1003) users      (100)     1749 2023-03-19 16:40:05.000000 semver-3.0.0rc1/CONTRIBUTORS
--rw-r--r--   0 tom       (1003) users      (100)     1496 2020-02-16 20:02:48.000000 semver-3.0.0rc1/LICENSE.txt
--rw-r--r--   0 tom       (1003) users      (100)      128 2023-02-22 12:09:12.000000 semver-3.0.0rc1/MANIFEST.in
--rw-r--r--   0 tom       (1003) users      (100)       69 2020-02-16 20:02:48.000000 semver-3.0.0rc1/Makefile
--rw-r--r--   0 tom       (1003) users      (100)     5545 2023-03-19 16:48:46.593373 semver-3.0.0rc1/PKG-INFO
--rw-r--r--   0 tom       (1003) users      (100)     4174 2023-03-19 16:40:05.000000 semver-3.0.0rc1/README.rst
-drwxr-xr-x   0 tom       (1003) users      (100)        0 2023-03-19 16:48:46.237372 semver-3.0.0rc1/changelog.d/
--rw-r--r--   0 tom       (1003) users      (100)       12 2023-02-22 12:09:12.000000 semver-3.0.0rc1/changelog.d/.gitignore
--rw-r--r--   0 tom       (1003) users      (100)     2501 2023-02-22 12:09:12.000000 semver-3.0.0rc1/changelog.d/README.rst
--rw-r--r--   0 tom       (1003) users      (100)      964 2023-02-22 12:09:12.000000 semver-3.0.0rc1/changelog.d/_template.rst
-drwxr-xr-x   0 tom       (1003) users      (100)        0 2023-03-19 16:48:46.281372 semver-3.0.0rc1/docs/
--rw-r--r--   0 tom       (1003) users      (100)      604 2020-02-16 20:02:48.000000 semver-3.0.0rc1/docs/Makefile
-drwxr-xr-x   0 tom       (1003) users      (100)        0 2023-03-19 16:48:46.281372 semver-3.0.0rc1/docs/_static/
-drwxr-xr-x   0 tom       (1003) users      (100)        0 2023-03-19 16:48:46.293372 semver-3.0.0rc1/docs/_static/css/
--rw-r--r--   0 tom       (1003) users      (100)     1193 2023-02-22 12:09:12.000000 semver-3.0.0rc1/docs/_static/css/custom.css
--rw-r--r--   0 tom       (1003) users      (100)     7754 2023-02-22 12:09:12.000000 semver-3.0.0rc1/docs/_static/logo.svg
-drwxr-xr-x   0 tom       (1003) users      (100)        0 2023-03-19 16:48:46.301372 semver-3.0.0rc1/docs/_templates/
--rw-r--r--   0 tom       (1003) users      (100)     1924 2023-02-22 12:09:12.000000 semver-3.0.0rc1/docs/_templates/layout.html
-drwxr-xr-x   0 tom       (1003) users      (100)        0 2023-03-19 16:48:46.321372 semver-3.0.0rc1/docs/advanced/
--rw-r--r--   0 tom       (1003) users      (100)     1208 2023-02-22 12:09:12.000000 semver-3.0.0rc1/docs/advanced/coerce.py
--rw-r--r--   0 tom       (1003) users      (100)     1822 2023-03-07 06:55:23.000000 semver-3.0.0rc1/docs/advanced/combine-pydantic-and-semver.rst
--rw-r--r--   0 tom       (1003) users      (100)     6185 2023-03-19 16:40:05.000000 semver-3.0.0rc1/docs/advanced/convert-pypi-to-semver.rst
--rw-r--r--   0 tom       (1003) users      (100)     1092 2023-03-19 16:40:05.000000 semver-3.0.0rc1/docs/advanced/create-subclasses-from-version.rst
--rw-r--r--   0 tom       (1003) users      (100)     1131 2023-02-22 12:09:12.000000 semver-3.0.0rc1/docs/advanced/deal-with-invalid-versions.rst
--rw-r--r--   0 tom       (1003) users      (100)     1102 2023-02-22 12:09:12.000000 semver-3.0.0rc1/docs/advanced/display-deprecation-warnings.rst
--rw-r--r--   0 tom       (1003) users      (100)      245 2023-03-19 16:40:05.000000 semver-3.0.0rc1/docs/advanced/index.rst
--rw-r--r--   0 tom       (1003) users      (100)      819 2023-03-19 16:40:05.000000 semver-3.0.0rc1/docs/advanced/semverwithvprefix.py
--rw-r--r--   0 tom       (1003) users      (100)      719 2023-03-19 16:40:05.000000 semver-3.0.0rc1/docs/advanced/version-from-file.rst
--rw-r--r--   0 tom       (1003) users      (100)     1802 2023-03-19 16:40:05.000000 semver-3.0.0rc1/docs/api.rst
--rw-r--r--   0 tom       (1003) users      (100)     2117 2023-03-19 16:40:05.000000 semver-3.0.0rc1/docs/build-semver.rst
--rw-r--r--   0 tom       (1003) users      (100)    12616 2023-02-22 12:09:13.000000 semver-3.0.0rc1/docs/changelog-semver2.rst
--rw-r--r--   0 tom       (1003) users      (100)    10410 2023-03-19 16:40:05.000000 semver-3.0.0rc1/docs/changelog-semver3-devel.rst
--rw-r--r--   0 tom       (1003) users      (100)       47 2023-02-22 12:09:13.000000 semver-3.0.0rc1/docs/changelog.rst
--rw-r--r--   0 tom       (1003) users      (100)     8057 2023-03-07 06:55:28.000000 semver-3.0.0rc1/docs/conf.py
-drwxr-xr-x   0 tom       (1003) users      (100)        0 2023-03-19 16:48:46.325372 semver-3.0.0rc1/docs/contribute/
--rw-r--r--   0 tom       (1003) users      (100)      143 2023-03-19 16:40:05.000000 semver-3.0.0rc1/docs/contribute/add-changelog-entry.rst
--rw-r--r--   0 tom       (1003) users      (100)     2565 2023-03-19 16:40:05.000000 semver-3.0.0rc1/docs/contribute/doc-semver.rst
--rw-r--r--   0 tom       (1003) users      (100)      580 2023-03-19 16:40:05.000000 semver-3.0.0rc1/docs/contribute/finish-release.rst
--rw-r--r--   0 tom       (1003) users      (100)      525 2023-03-19 16:40:05.000000 semver-3.0.0rc1/docs/contribute/index.rst
--rw-r--r--   0 tom       (1003) users      (100)      432 2023-03-19 16:40:05.000000 semver-3.0.0rc1/docs/contribute/prerequisites.rst
--rw-r--r--   0 tom       (1003) users      (100)     3227 2023-03-19 16:40:05.000000 semver-3.0.0rc1/docs/contribute/release-procedure.rst
--rw-r--r--   0 tom       (1003) users      (100)      577 2023-03-19 16:40:05.000000 semver-3.0.0rc1/docs/contribute/report-bugs.rst
--rw-r--r--   0 tom       (1003) users      (100)     1934 2023-03-19 16:40:05.000000 semver-3.0.0rc1/docs/contribute/run-test-suite.rst
--rw-r--r--   0 tom       (1003) users      (100)      559 2023-03-19 16:40:05.000000 semver-3.0.0rc1/docs/index.rst
--rw-r--r--   0 tom       (1003) users      (100)     2586 2023-02-22 12:09:13.000000 semver-3.0.0rc1/docs/install.rst
--rw-r--r--   0 tom       (1003) users      (100)      804 2020-02-16 20:02:48.000000 semver-3.0.0rc1/docs/make.bat
-drwxr-xr-x   0 tom       (1003) users      (100)        0 2023-03-19 16:48:46.329373 semver-3.0.0rc1/docs/migration/
--rw-r--r--   0 tom       (1003) users      (100)      133 2023-02-22 12:09:13.000000 semver-3.0.0rc1/docs/migration/index.rst
--rw-r--r--   0 tom       (1003) users      (100)     1572 2023-03-19 16:40:05.000000 semver-3.0.0rc1/docs/migration/migratetosemver3.rst
--rw-r--r--   0 tom       (1003) users      (100)     3147 2023-03-19 16:40:05.000000 semver-3.0.0rc1/docs/migration/replace-deprecated-functions.rst
--rw-r--r--   0 tom       (1003) users      (100)     3738 2020-04-29 05:30:13.000000 semver-3.0.0rc1/docs/pysemver.rst
--rw-r--r--   0 tom       (1003) users      (100)      120 2023-02-22 12:09:13.000000 semver-3.0.0rc1/docs/readme.rst
--rw-r--r--   0 tom       (1003) users      (100)       88 2023-02-22 12:09:13.000000 semver-3.0.0rc1/docs/requirements.txt
-drwxr-xr-x   0 tom       (1003) users      (100)        0 2023-03-19 16:48:46.361373 semver-3.0.0rc1/docs/usage/
--rw-r--r--   0 tom       (1003) users      (100)     1105 2023-02-22 12:09:13.000000 semver-3.0.0rc1/docs/usage/access-parts-of-a-version.rst
--rw-r--r--   0 tom       (1003) users      (100)     1236 2023-03-19 16:40:05.000000 semver-3.0.0rc1/docs/usage/access-parts-through-index.rst
--rw-r--r--   0 tom       (1003) users      (100)     2224 2023-03-19 16:40:05.000000 semver-3.0.0rc1/docs/usage/check-compatible-semver-version.rst
--rw-r--r--   0 tom       (1003) users      (100)      312 2023-03-19 16:40:05.000000 semver-3.0.0rc1/docs/usage/check-valid-semver-version.rst
--rw-r--r--   0 tom       (1003) users      (100)     1126 2023-03-19 16:40:05.000000 semver-3.0.0rc1/docs/usage/compare-versions-through-expression.rst
--rw-r--r--   0 tom       (1003) users      (100)     2447 2023-03-19 16:40:05.000000 semver-3.0.0rc1/docs/usage/compare-versions.rst
--rw-r--r--   0 tom       (1003) users      (100)      883 2023-03-19 16:40:05.000000 semver-3.0.0rc1/docs/usage/convert-version-into-different-types.rst
--rw-r--r--   0 tom       (1003) users      (100)     3458 2023-03-19 16:40:05.000000 semver-3.0.0rc1/docs/usage/create-a-version.rst
--rw-r--r--   0 tom       (1003) users      (100)      636 2023-02-22 12:09:13.000000 semver-3.0.0rc1/docs/usage/determine-version-equality.rst
--rw-r--r--   0 tom       (1003) users      (100)     1669 2023-03-19 16:40:05.000000 semver-3.0.0rc1/docs/usage/get-min-and-max-of-multiple-versions.rst
--rw-r--r--   0 tom       (1003) users      (100)      787 2023-03-19 16:40:05.000000 semver-3.0.0rc1/docs/usage/increase-parts-of-a-version_prereleases.rst
--rw-r--r--   0 tom       (1003) users      (100)      519 2023-03-07 06:55:28.000000 semver-3.0.0rc1/docs/usage/index.rst
--rw-r--r--   0 tom       (1003) users      (100)      651 2023-03-19 16:40:05.000000 semver-3.0.0rc1/docs/usage/parse-version-string.rst
--rw-r--r--   0 tom       (1003) users      (100)     2421 2023-03-19 16:40:05.000000 semver-3.0.0rc1/docs/usage/raise-parts-of-a-version.rst
--rw-r--r--   0 tom       (1003) users      (100)      672 2023-03-19 16:40:05.000000 semver-3.0.0rc1/docs/usage/replace-parts-of-a-version.rst
--rw-r--r--   0 tom       (1003) users      (100)      172 2023-03-19 16:40:05.000000 semver-3.0.0rc1/docs/usage/semver-version.rst
--rw-r--r--   0 tom       (1003) users      (100)      330 2023-02-22 12:09:13.000000 semver-3.0.0rc1/docs/usage/semver_org-version.rst
--rw-r--r--   0 tom       (1003) users      (100)     1208 2023-02-22 12:09:13.000000 semver-3.0.0rc1/pyproject.toml
--rw-r--r--   0 tom       (1003) users      (100)     3480 2023-02-22 12:09:13.000000 semver-3.0.0rc1/release-procedure.md
--rw-r--r--   0 tom       (1003) users      (100)     2156 2023-03-19 16:48:46.645373 semver-3.0.0rc1/setup.cfg
-drwxr-xr-x   0 tom       (1003) users      (100)        0 2023-03-19 16:48:46.185372 semver-3.0.0rc1/src/
-drwxr-xr-x   0 tom       (1003) users      (100)        0 2023-03-19 16:48:46.397373 semver-3.0.0rc1/src/semver/
--rw-r--r--   0 tom       (1003) users      (100)      820 2023-03-19 16:40:05.000000 semver-3.0.0rc1/src/semver/__about__.py
--rw-r--r--   0 tom       (1003) users      (100)      688 2023-02-22 12:09:13.000000 semver-3.0.0rc1/src/semver/__init__.py
--rw-r--r--   0 tom       (1003) users      (100)      592 2023-03-07 06:55:23.000000 semver-3.0.0rc1/src/semver/__main__.py
--rw-r--r--   0 tom       (1003) users      (100)    10931 2023-03-19 16:40:05.000000 semver-3.0.0rc1/src/semver/_deprecated.py
--rw-r--r--   0 tom       (1003) users      (100)      422 2023-02-28 06:58:41.000000 semver-3.0.0rc1/src/semver/_types.py
--rw-r--r--   0 tom       (1003) users      (100)     5188 2023-03-07 06:55:28.000000 semver-3.0.0rc1/src/semver/cli.py
--rw-r--r--   0 tom       (1003) users      (100)        0 2023-02-22 12:09:13.000000 semver-3.0.0rc1/src/semver/py.typed
--rw-r--r--   0 tom       (1003) users      (100)    24094 2023-03-19 16:40:05.000000 semver-3.0.0rc1/src/semver/version.py
-drwxr-xr-x   0 tom       (1003) users      (100)        0 2023-03-19 16:48:46.397373 semver-3.0.0rc1/src/semver.egg-info/
--rw-r--r--   0 tom       (1003) users      (100)     5545 2023-03-19 16:48:46.000000 semver-3.0.0rc1/src/semver.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1003) users      (100)     2751 2023-03-19 16:48:46.000000 semver-3.0.0rc1/src/semver.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1003) users      (100)        1 2023-03-19 16:48:46.000000 semver-3.0.0rc1/src/semver.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1003) users      (100)       45 2023-03-19 16:48:46.000000 semver-3.0.0rc1/src/semver.egg-info/entry_points.txt
--rw-r--r--   0 tom       (1003) users      (100)        7 2023-03-19 16:48:46.000000 semver-3.0.0rc1/src/semver.egg-info/top_level.txt
-drwxr-xr-x   0 tom       (1003) users      (100)        0 2023-03-19 16:48:46.585373 semver-3.0.0rc1/tests/
--rw-r--r--   0 tom       (1003) users      (100)     1208 2023-02-22 12:09:12.000000 semver-3.0.0rc1/tests/coerce.py
--rw-r--r--   0 tom       (1003) users      (100)      739 2023-03-07 06:55:23.000000 semver-3.0.0rc1/tests/conftest.py
--rw-r--r--   0 tom       (1003) users      (100)      819 2023-03-19 16:40:05.000000 semver-3.0.0rc1/tests/semverwithvprefix.py
--rw-r--r--   0 tom       (1003) users      (100)     3667 2023-03-07 06:55:23.000000 semver-3.0.0rc1/tests/test_bump.py
--rw-r--r--   0 tom       (1003) users      (100)     8068 2023-02-22 12:09:13.000000 semver-3.0.0rc1/tests/test_compare.py
--rw-r--r--   0 tom       (1003) users      (100)     2153 2023-02-22 12:09:13.000000 semver-3.0.0rc1/tests/test_deprecated_functions.py
--rw-r--r--   0 tom       (1003) users      (100)     1062 2023-02-22 12:09:13.000000 semver-3.0.0rc1/tests/test_docstrings.py
--rw-r--r--   0 tom       (1003) users      (100)     2207 2023-02-22 12:09:13.000000 semver-3.0.0rc1/tests/test_format.py
--rw-r--r--   0 tom       (1003) users      (100)      965 2023-02-22 12:09:13.000000 semver-3.0.0rc1/tests/test_immutable.py
--rw-r--r--   0 tom       (1003) users      (100)     2988 2023-02-22 12:09:13.000000 semver-3.0.0rc1/tests/test_index.py
--rw-r--r--   0 tom       (1003) users      (100)     1651 2023-02-22 12:09:13.000000 semver-3.0.0rc1/tests/test_match.py
--rw-r--r--   0 tom       (1003) users      (100)     1356 2023-02-22 12:09:13.000000 semver-3.0.0rc1/tests/test_max-min.py
--rw-r--r--   0 tom       (1003) users      (100)     5503 2023-02-22 12:09:13.000000 semver-3.0.0rc1/tests/test_parsing.py
--rw-r--r--   0 tom       (1003) users      (100)     4182 2023-02-22 12:09:13.000000 semver-3.0.0rc1/tests/test_pysemver-cli.py
--rw-r--r--   0 tom       (1003) users      (100)     1789 2023-02-22 12:09:13.000000 semver-3.0.0rc1/tests/test_replace.py
--rw-r--r--   0 tom       (1003) users      (100)     3684 2023-03-07 06:55:28.000000 semver-3.0.0rc1/tests/test_semver.py
--rw-r--r--   0 tom       (1003) users      (100)      563 2023-02-22 12:09:13.000000 semver-3.0.0rc1/tests/test_subclass.py
--rw-r--r--   0 tom       (1003) users      (100)      341 2023-02-22 12:09:13.000000 semver-3.0.0rc1/tests/test_typeerror-274.py
--rw-r--r--   0 tom       (1003) users      (100)     2380 2023-03-19 16:40:05.000000 semver-3.0.0rc1/tox.ini
+drwxr-xr-x   0 tom       (1003) users      (100)        0 2023-06-14 11:43:01.207531 semver-3.0.1/
+-rw-r--r--   0 tom       (1003) users      (100)      229 2022-12-14 15:46:31.000000 semver-3.0.1/.coveragerc
+-rw-r--r--   0 tom       (1003) users      (100)      217 2023-02-22 12:09:12.000000 semver-3.0.1/.editorconfig
+-rw-r--r--   0 tom       (1003) users      (100)     4585 2023-03-07 06:55:28.000000 semver-3.0.1/.gitignore
+-rw-r--r--   0 tom       (1003) users      (100)    11033 2023-06-14 11:41:46.000000 semver-3.0.1/CHANGELOG.rst
+-rw-r--r--   0 tom       (1003) users      (100)     2311 2023-06-14 10:38:31.000000 semver-3.0.1/CITATION.cff
+-rw-r--r--   0 tom       (1003) users      (100)     1891 2023-03-19 16:40:05.000000 semver-3.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 tom       (1003) users      (100)     1749 2023-03-19 16:40:05.000000 semver-3.0.1/CONTRIBUTORS
+-rw-r--r--   0 tom       (1003) users      (100)     1496 2020-02-16 20:02:48.000000 semver-3.0.1/LICENSE.txt
+-rw-r--r--   0 tom       (1003) users      (100)      128 2023-02-22 12:09:12.000000 semver-3.0.1/MANIFEST.in
+-rw-r--r--   0 tom       (1003) users      (100)       69 2020-02-16 20:02:48.000000 semver-3.0.1/Makefile
+-rw-r--r--   0 tom       (1003) users      (100)     5542 2023-06-14 11:43:01.207531 semver-3.0.1/PKG-INFO
+-rw-r--r--   0 tom       (1003) users      (100)     4174 2023-03-19 16:40:05.000000 semver-3.0.1/README.rst
+drwxr-xr-x   0 tom       (1003) users      (100)        0 2023-06-14 11:43:01.203531 semver-3.0.1/changelog.d/
+-rw-r--r--   0 tom       (1003) users      (100)       12 2023-02-22 12:09:12.000000 semver-3.0.1/changelog.d/.gitignore
+-rw-r--r--   0 tom       (1003) users      (100)     2501 2023-02-22 12:09:12.000000 semver-3.0.1/changelog.d/README.rst
+-rw-r--r--   0 tom       (1003) users      (100)      964 2023-02-22 12:09:12.000000 semver-3.0.1/changelog.d/_template.rst
+drwxr-xr-x   0 tom       (1003) users      (100)        0 2023-06-14 11:43:01.203531 semver-3.0.1/docs/
+-rw-r--r--   0 tom       (1003) users      (100)      604 2020-02-16 20:02:48.000000 semver-3.0.1/docs/Makefile
+drwxr-xr-x   0 tom       (1003) users      (100)        0 2023-06-14 11:43:01.203531 semver-3.0.1/docs/_static/
+drwxr-xr-x   0 tom       (1003) users      (100)        0 2023-06-14 11:43:01.203531 semver-3.0.1/docs/_static/css/
+-rw-r--r--   0 tom       (1003) users      (100)     1193 2023-02-22 12:09:12.000000 semver-3.0.1/docs/_static/css/custom.css
+-rw-r--r--   0 tom       (1003) users      (100)     7754 2023-02-22 12:09:12.000000 semver-3.0.1/docs/_static/logo.svg
+drwxr-xr-x   0 tom       (1003) users      (100)        0 2023-06-14 11:43:01.203531 semver-3.0.1/docs/_templates/
+-rw-r--r--   0 tom       (1003) users      (100)     1924 2023-04-03 12:15:56.000000 semver-3.0.1/docs/_templates/layout.html
+drwxr-xr-x   0 tom       (1003) users      (100)        0 2023-06-14 11:43:01.203531 semver-3.0.1/docs/advanced/
+-rw-r--r--   0 tom       (1003) users      (100)     1208 2023-02-22 12:09:12.000000 semver-3.0.1/docs/advanced/coerce.py
+-rw-r--r--   0 tom       (1003) users      (100)     1822 2023-03-07 06:55:23.000000 semver-3.0.1/docs/advanced/combine-pydantic-and-semver.rst
+-rw-r--r--   0 tom       (1003) users      (100)     6185 2023-03-19 16:40:05.000000 semver-3.0.1/docs/advanced/convert-pypi-to-semver.rst
+-rw-r--r--   0 tom       (1003) users      (100)     1092 2023-03-19 16:40:05.000000 semver-3.0.1/docs/advanced/create-subclasses-from-version.rst
+-rw-r--r--   0 tom       (1003) users      (100)     1131 2023-02-22 12:09:12.000000 semver-3.0.1/docs/advanced/deal-with-invalid-versions.rst
+-rw-r--r--   0 tom       (1003) users      (100)     1102 2023-02-22 12:09:12.000000 semver-3.0.1/docs/advanced/display-deprecation-warnings.rst
+-rw-r--r--   0 tom       (1003) users      (100)      245 2023-03-19 16:40:05.000000 semver-3.0.1/docs/advanced/index.rst
+-rw-r--r--   0 tom       (1003) users      (100)      819 2023-03-19 16:40:05.000000 semver-3.0.1/docs/advanced/semverwithvprefix.py
+-rw-r--r--   0 tom       (1003) users      (100)      719 2023-03-19 16:40:05.000000 semver-3.0.1/docs/advanced/version-from-file.rst
+-rw-r--r--   0 tom       (1003) users      (100)     1802 2023-04-02 13:11:55.000000 semver-3.0.1/docs/api.rst
+-rw-r--r--   0 tom       (1003) users      (100)     2117 2023-03-19 16:40:05.000000 semver-3.0.1/docs/build-semver.rst
+-rw-r--r--   0 tom       (1003) users      (100)    10410 2023-03-19 16:40:05.000000 semver-3.0.1/docs/changelog-semver3-devel.rst
+-rw-r--r--   0 tom       (1003) users      (100)       47 2023-02-22 12:09:13.000000 semver-3.0.1/docs/changelog.rst
+-rw-r--r--   0 tom       (1003) users      (100)     8557 2023-04-03 12:15:56.000000 semver-3.0.1/docs/conf.py
+drwxr-xr-x   0 tom       (1003) users      (100)        0 2023-06-14 11:43:01.203531 semver-3.0.1/docs/contribute/
+-rw-r--r--   0 tom       (1003) users      (100)      143 2023-03-19 16:40:05.000000 semver-3.0.1/docs/contribute/add-changelog-entry.rst
+-rw-r--r--   0 tom       (1003) users      (100)     2565 2023-03-19 16:40:05.000000 semver-3.0.1/docs/contribute/doc-semver.rst
+-rw-r--r--   0 tom       (1003) users      (100)      580 2023-03-19 16:40:05.000000 semver-3.0.1/docs/contribute/finish-release.rst
+-rw-r--r--   0 tom       (1003) users      (100)      525 2023-03-19 16:40:05.000000 semver-3.0.1/docs/contribute/index.rst
+-rw-r--r--   0 tom       (1003) users      (100)      432 2023-03-19 16:40:05.000000 semver-3.0.1/docs/contribute/prerequisites.rst
+-rw-r--r--   0 tom       (1003) users      (100)     3227 2023-03-19 16:40:05.000000 semver-3.0.1/docs/contribute/release-procedure.rst
+-rw-r--r--   0 tom       (1003) users      (100)      577 2023-03-19 16:40:05.000000 semver-3.0.1/docs/contribute/report-bugs.rst
+-rw-r--r--   0 tom       (1003) users      (100)     1934 2023-03-19 16:40:05.000000 semver-3.0.1/docs/contribute/run-test-suite.rst
+-rw-r--r--   0 tom       (1003) users      (100)      565 2023-04-02 13:11:55.000000 semver-3.0.1/docs/index.rst
+-rw-r--r--   0 tom       (1003) users      (100)     2586 2023-02-22 12:09:13.000000 semver-3.0.1/docs/install.rst
+drwxr-xr-x   0 tom       (1003) users      (100)        0 2023-06-14 11:43:01.203531 semver-3.0.1/docs/inventories/
+-rw-r--r--   0 tom       (1003) users      (100)   130055 2023-04-02 13:11:55.000000 semver-3.0.1/docs/inventories/python-objects.inv
+-rw-r--r--   0 tom       (1003) users      (100)      804 2020-02-16 20:02:48.000000 semver-3.0.1/docs/make.bat
+drwxr-xr-x   0 tom       (1003) users      (100)        0 2023-06-14 11:43:01.203531 semver-3.0.1/docs/migration/
+-rw-r--r--   0 tom       (1003) users      (100)      133 2023-02-22 12:09:13.000000 semver-3.0.1/docs/migration/index.rst
+-rw-r--r--   0 tom       (1003) users      (100)     1572 2023-03-19 16:40:05.000000 semver-3.0.1/docs/migration/migratetosemver3.rst
+-rw-r--r--   0 tom       (1003) users      (100)     3147 2023-03-19 16:40:05.000000 semver-3.0.1/docs/migration/replace-deprecated-functions.rst
+-rw-r--r--   0 tom       (1003) users      (100)     3738 2020-04-29 05:30:13.000000 semver-3.0.1/docs/pysemver.rst
+-rw-r--r--   0 tom       (1003) users      (100)      120 2023-02-22 12:09:13.000000 semver-3.0.1/docs/readme.rst
+-rw-r--r--   0 tom       (1003) users      (100)       88 2023-04-03 12:15:56.000000 semver-3.0.1/docs/requirements.txt
+drwxr-xr-x   0 tom       (1003) users      (100)        0 2023-06-14 11:43:01.207531 semver-3.0.1/docs/usage/
+-rw-r--r--   0 tom       (1003) users      (100)     1105 2023-02-22 12:09:13.000000 semver-3.0.1/docs/usage/access-parts-of-a-version.rst
+-rw-r--r--   0 tom       (1003) users      (100)     1236 2023-03-19 16:40:05.000000 semver-3.0.1/docs/usage/access-parts-through-index.rst
+-rw-r--r--   0 tom       (1003) users      (100)     2224 2023-03-19 16:40:05.000000 semver-3.0.1/docs/usage/check-compatible-semver-version.rst
+-rw-r--r--   0 tom       (1003) users      (100)      312 2023-03-19 16:40:05.000000 semver-3.0.1/docs/usage/check-valid-semver-version.rst
+-rw-r--r--   0 tom       (1003) users      (100)     1126 2023-03-19 16:40:05.000000 semver-3.0.1/docs/usage/compare-versions-through-expression.rst
+-rw-r--r--   0 tom       (1003) users      (100)     2476 2023-04-02 13:11:55.000000 semver-3.0.1/docs/usage/compare-versions.rst
+-rw-r--r--   0 tom       (1003) users      (100)      883 2023-03-19 16:40:05.000000 semver-3.0.1/docs/usage/convert-version-into-different-types.rst
+-rw-r--r--   0 tom       (1003) users      (100)     3458 2023-03-19 16:40:05.000000 semver-3.0.1/docs/usage/create-a-version.rst
+-rw-r--r--   0 tom       (1003) users      (100)      636 2023-02-22 12:09:13.000000 semver-3.0.1/docs/usage/determine-version-equality.rst
+-rw-r--r--   0 tom       (1003) users      (100)     1669 2023-03-19 16:40:05.000000 semver-3.0.1/docs/usage/get-min-and-max-of-multiple-versions.rst
+-rw-r--r--   0 tom       (1003) users      (100)      787 2023-03-19 16:40:05.000000 semver-3.0.1/docs/usage/increase-parts-of-a-version_prereleases.rst
+-rw-r--r--   0 tom       (1003) users      (100)      519 2023-03-07 06:55:28.000000 semver-3.0.1/docs/usage/index.rst
+-rw-r--r--   0 tom       (1003) users      (100)      651 2023-03-19 16:40:05.000000 semver-3.0.1/docs/usage/parse-version-string.rst
+-rw-r--r--   0 tom       (1003) users      (100)     2421 2023-03-19 16:40:05.000000 semver-3.0.1/docs/usage/raise-parts-of-a-version.rst
+-rw-r--r--   0 tom       (1003) users      (100)      672 2023-03-19 16:40:05.000000 semver-3.0.1/docs/usage/replace-parts-of-a-version.rst
+-rw-r--r--   0 tom       (1003) users      (100)      167 2023-06-14 11:41:46.000000 semver-3.0.1/docs/usage/semver-version.rst
+-rw-r--r--   0 tom       (1003) users      (100)      330 2023-02-22 12:09:13.000000 semver-3.0.1/docs/usage/semver_org-version.rst
+-rw-r--r--   0 tom       (1003) users      (100)     1349 2023-06-14 11:07:38.000000 semver-3.0.1/pyproject.toml
+-rw-r--r--   0 tom       (1003) users      (100)     3515 2023-06-14 11:41:46.000000 semver-3.0.1/release-procedure.md
+-rw-r--r--   0 tom       (1003) users      (100)     2156 2023-06-14 11:43:01.207531 semver-3.0.1/setup.cfg
+drwxr-xr-x   0 tom       (1003) users      (100)        0 2023-06-14 11:43:01.199531 semver-3.0.1/src/
+drwxr-xr-x   0 tom       (1003) users      (100)        0 2023-06-14 11:43:01.207531 semver-3.0.1/src/semver/
+-rw-r--r--   0 tom       (1003) users      (100)      815 2023-06-14 11:41:46.000000 semver-3.0.1/src/semver/__about__.py
+-rw-r--r--   0 tom       (1003) users      (100)     1269 2023-06-14 10:38:31.000000 semver-3.0.1/src/semver/__init__.py
+-rw-r--r--   0 tom       (1003) users      (100)      592 2023-03-07 06:55:23.000000 semver-3.0.1/src/semver/__main__.py
+-rw-r--r--   0 tom       (1003) users      (100)    11272 2023-04-02 13:11:55.000000 semver-3.0.1/src/semver/_deprecated.py
+-rw-r--r--   0 tom       (1003) users      (100)      422 2023-02-28 06:58:41.000000 semver-3.0.1/src/semver/_types.py
+-rw-r--r--   0 tom       (1003) users      (100)     5189 2023-06-14 10:38:31.000000 semver-3.0.1/src/semver/cli.py
+-rw-r--r--   0 tom       (1003) users      (100)        0 2023-02-22 12:09:13.000000 semver-3.0.1/src/semver/py.typed
+-rw-r--r--   0 tom       (1003) users      (100)    24075 2023-06-14 11:20:42.000000 semver-3.0.1/src/semver/version.py
+drwxr-xr-x   0 tom       (1003) users      (100)        0 2023-06-14 11:43:01.207531 semver-3.0.1/src/semver.egg-info/
+-rw-r--r--   0 tom       (1003) users      (100)     5542 2023-06-14 11:43:01.000000 semver-3.0.1/src/semver.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1003) users      (100)     2773 2023-06-14 11:43:01.000000 semver-3.0.1/src/semver.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1003) users      (100)        1 2023-06-14 11:43:01.000000 semver-3.0.1/src/semver.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1003) users      (100)       45 2023-06-14 11:43:01.000000 semver-3.0.1/src/semver.egg-info/entry_points.txt
+-rw-r--r--   0 tom       (1003) users      (100)        7 2023-06-14 11:43:01.000000 semver-3.0.1/src/semver.egg-info/top_level.txt
+drwxr-xr-x   0 tom       (1003) users      (100)        0 2023-06-14 11:43:01.207531 semver-3.0.1/tests/
+-rw-r--r--   0 tom       (1003) users      (100)     1208 2023-02-22 12:09:12.000000 semver-3.0.1/tests/coerce.py
+-rw-r--r--   0 tom       (1003) users      (100)      739 2023-03-07 06:55:23.000000 semver-3.0.1/tests/conftest.py
+-rw-r--r--   0 tom       (1003) users      (100)      819 2023-03-19 16:40:05.000000 semver-3.0.1/tests/semverwithvprefix.py
+-rw-r--r--   0 tom       (1003) users      (100)     3667 2023-03-07 06:55:23.000000 semver-3.0.1/tests/test_bump.py
+-rw-r--r--   0 tom       (1003) users      (100)     8068 2023-02-22 12:09:13.000000 semver-3.0.1/tests/test_compare.py
+-rw-r--r--   0 tom       (1003) users      (100)     2097 2023-04-02 13:11:55.000000 semver-3.0.1/tests/test_deprecated_functions.py
+-rw-r--r--   0 tom       (1003) users      (100)     1062 2023-02-22 12:09:13.000000 semver-3.0.1/tests/test_docstrings.py
+-rw-r--r--   0 tom       (1003) users      (100)     2207 2023-02-22 12:09:13.000000 semver-3.0.1/tests/test_format.py
+-rw-r--r--   0 tom       (1003) users      (100)      965 2023-02-22 12:09:13.000000 semver-3.0.1/tests/test_immutable.py
+-rw-r--r--   0 tom       (1003) users      (100)     2988 2023-02-22 12:09:13.000000 semver-3.0.1/tests/test_index.py
+-rw-r--r--   0 tom       (1003) users      (100)     1651 2023-02-22 12:09:13.000000 semver-3.0.1/tests/test_match.py
+-rw-r--r--   0 tom       (1003) users      (100)     1356 2023-02-22 12:09:13.000000 semver-3.0.1/tests/test_max-min.py
+-rw-r--r--   0 tom       (1003) users      (100)     5503 2023-02-22 12:09:13.000000 semver-3.0.1/tests/test_parsing.py
+-rw-r--r--   0 tom       (1003) users      (100)     4182 2023-02-22 12:09:13.000000 semver-3.0.1/tests/test_pysemver-cli.py
+-rw-r--r--   0 tom       (1003) users      (100)     1789 2023-02-22 12:09:13.000000 semver-3.0.1/tests/test_replace.py
+-rw-r--r--   0 tom       (1003) users      (100)     3684 2023-03-07 06:55:28.000000 semver-3.0.1/tests/test_semver.py
+-rw-r--r--   0 tom       (1003) users      (100)      563 2023-02-22 12:09:13.000000 semver-3.0.1/tests/test_subclass.py
+-rw-r--r--   0 tom       (1003) users      (100)      341 2023-02-22 12:09:13.000000 semver-3.0.1/tests/test_typeerror-274.py
+-rw-r--r--   0 tom       (1003) users      (100)     2319 2023-06-14 11:41:46.000000 semver-3.0.1/tox.ini
```

### Comparing `semver-3.0.0rc1/.gitignore` & `semver-3.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/CHANGELOG.rst` & `semver-3.0.1/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -14,18 +14,35 @@
    This changelog is managed by towncrier and is compiled at release time.
 
    See https://python-semver.rtd.io/en/latest/development.html#changelog
    for details.
 
 .. towncrier release notes start
 
+Version 3.0.1
+=============
+
+:Released: 2023-06-14
+:Maintainer: Tom Schraitle
+
+
+Bug Fixes
+---------
+
+* :gh:`410`: Export functions properly using ``__all__`` in ``__init__.py``.
+
+
+
+----
+
+
 Version 3.0.0
 =============
 
-:Released: 2023-03-19
+:Released: 2023-04-02
 :Maintainer: Tom Schraitle
 
 
 Bug Fixes
 ---------
 
 * :gh:`291`: Disallow negative numbers in VersionInfo arguments
@@ -91,14 +108,22 @@
   Python 3.6 reached its end of life and isn't supported anymore.
   At the time of writing (Dec 2022), the lowest version is 3.7.
 
   Although the `poll <https://github.com/python-semver/python-semver/discussions/371>`_
   didn't cast many votes, the majority agreed to remove support for
   Python 3.6.
 
+* :pr:`402`: Keep :func:`semver.compare <semver._deprecated.compare>`.
+   Although it breaks consistency with module level functions, it seems it's
+   a much needed/used function. It's still unclear if we should deprecate
+   this function or not (that's why we use :py:exc:`PendingDeprecationWarning`).
+
+   As we don't have a uniform initializer yet, this function stays in the
+   :file:`_deprecated.py` file for the time being until we find a better solution. See :gh:`258` for details.
+
 
 Features
 --------
 
 * :gh:`169`: Create semver package and split code among different modules in the packages:
 
   * Remove :file:`semver.py`
```

### Comparing `semver-3.0.0rc1/CONTRIBUTING.rst` & `semver-3.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/CONTRIBUTORS` & `semver-3.0.1/CONTRIBUTORS`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/LICENSE.txt` & `semver-3.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/PKG-INFO` & `semver-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semver
-Version: 3.0.0rc1
+Version: 3.0.1
 Summary: Python helper for Semantic Versioning (https://semver.org)
 Home-page: https://github.com/python-semver/python-semver
 Author: Kostiantyn Rybnikov
 Author-email: k-bx@k-bx.com
 Maintainer: Sebastien Celles, Tom Schraitle
 Maintainer-email: s.celles@gmail.com
 License: BSD
```

### Comparing `semver-3.0.0rc1/README.rst` & `semver-3.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/changelog.d/README.rst` & `semver-3.0.1/changelog.d/README.rst`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/changelog.d/_template.rst` & `semver-3.0.1/changelog.d/_template.rst`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/Makefile` & `semver-3.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/_static/css/custom.css` & `semver-3.0.1/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/_static/logo.svg` & `semver-3.0.1/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/_templates/layout.html` & `semver-3.0.1/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/advanced/coerce.py` & `semver-3.0.1/docs/advanced/coerce.py`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/advanced/combine-pydantic-and-semver.rst` & `semver-3.0.1/docs/advanced/combine-pydantic-and-semver.rst`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/advanced/convert-pypi-to-semver.rst` & `semver-3.0.1/docs/advanced/convert-pypi-to-semver.rst`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/advanced/create-subclasses-from-version.rst` & `semver-3.0.1/docs/advanced/create-subclasses-from-version.rst`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/advanced/deal-with-invalid-versions.rst` & `semver-3.0.1/docs/advanced/deal-with-invalid-versions.rst`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/advanced/display-deprecation-warnings.rst` & `semver-3.0.1/docs/advanced/display-deprecation-warnings.rst`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/advanced/semverwithvprefix.py` & `semver-3.0.1/docs/advanced/semverwithvprefix.py`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/advanced/version-from-file.rst` & `semver-3.0.1/docs/advanced/version-from-file.rst`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/api.rst` & `semver-3.0.1/docs/api.rst`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 
 
 Deprecated Functions in :mod:`semver._deprecated`
 -------------------------------------------------
 
 .. automodule:: semver._deprecated
 
+.. autofunction:: semver._deprecated.compare
+
 .. autofunction:: semver._deprecated.bump_build
 
 .. autofunction:: semver._deprecated.bump_major
 
 .. autofunction:: semver._deprecated.bump_minor
 
 .. autofunction:: semver._deprecated.bump_patch
 
 .. autofunction:: semver._deprecated.bump_prerelease
 
-.. autofunction:: semver._deprecated.compare
-
 .. autofunction:: semver._deprecated.deprecated
 
 .. autofunction:: semver._deprecated.finalize_version
 
 .. autofunction:: semver._deprecated.format_version
 
 .. autofunction:: semver._deprecated.match
```

### Comparing `semver-3.0.0rc1/docs/build-semver.rst` & `semver-3.0.1/docs/build-semver.rst`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/changelog-semver3-devel.rst` & `semver-3.0.1/docs/changelog-semver3-devel.rst`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/conf.py` & `semver-3.0.1/docs/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -118,14 +118,25 @@
 # Markup to shorten external links
 # See https://www.sphinx-doc.org/en/master/usage/extensions/extlinks.html
 extlinks = {
     "gh": ("https://github.com/python-semver/python-semver/issues/%s", "#%s"),
     "pr": ("https://github.com/python-semver/python-semver/pull/%s", "PR #%s"),
 }
 
+# Link to other projects’ documentation
+# See https://www.sphinx-doc.org/en/master/usage/extensions/intersphinx.html
+intersphinx_mapping = {
+    # Download it from the root with:
+    # wget -O docs/python-objects.inv https://docs.python.org/3/objects.inv
+    "python": ("https://docs.python.org/3", (None, "inventories/python-objects.inv")),
+}
+# Avoid side-effects (namely that documentations local references can
+# suddenly resolve to an external location.)
+intersphinx_disabled_reftypes = ["*"]
+
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
 html_theme = "alabaster"
 templates_path = ["_templates"]
```

### Comparing `semver-3.0.0rc1/docs/contribute/doc-semver.rst` & `semver-3.0.1/docs/contribute/doc-semver.rst`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/contribute/finish-release.rst` & `semver-3.0.1/docs/contribute/finish-release.rst`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/contribute/index.rst` & `semver-3.0.1/docs/contribute/index.rst`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/contribute/release-procedure.rst` & `semver-3.0.1/docs/contribute/release-procedure.rst`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/contribute/report-bugs.rst` & `semver-3.0.1/docs/contribute/report-bugs.rst`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/contribute/run-test-suite.rst` & `semver-3.0.1/docs/contribute/run-test-suite.rst`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/index.rst` & `semver-3.0.1/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 .. toctree::
    :maxdepth: 1
    :caption: Development
    :hidden:
 
    changelog
-   changelog-semver2
+   changelog-semver3-devel
 
 
 Indices and Tables
 ==================
 
 * :ref:`genindex`
 * :ref:`modindex`
```

### Comparing `semver-3.0.0rc1/docs/install.rst` & `semver-3.0.1/docs/install.rst`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/make.bat` & `semver-3.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/migration/migratetosemver3.rst` & `semver-3.0.1/docs/migration/migratetosemver3.rst`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/migration/replace-deprecated-functions.rst` & `semver-3.0.1/docs/migration/replace-deprecated-functions.rst`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/pysemver.rst` & `semver-3.0.1/docs/pysemver.rst`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/usage/access-parts-of-a-version.rst` & `semver-3.0.1/docs/usage/access-parts-of-a-version.rst`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/usage/access-parts-through-index.rst` & `semver-3.0.1/docs/usage/access-parts-through-index.rst`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/usage/check-compatible-semver-version.rst` & `semver-3.0.1/docs/usage/check-compatible-semver-version.rst`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/usage/compare-versions-through-expression.rst` & `semver-3.0.1/docs/usage/compare-versions-through-expression.rst`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/usage/compare-versions.rst` & `semver-3.0.1/docs/usage/compare-versions.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Comparing Versions
 ==================
 
 To compare two versions depends on your type:
 
 * **Two strings**
 
-  Use :func:`semver.compare`::
+  Use :func:`semver.compare <semver._deprecated.compare>`::
 
     >>> semver.compare("1.0.0", "2.0.0")
     -1
     >>> semver.compare("2.0.0", "1.0.0")
     1
     >>> semver.compare("2.0.0", "2.0.0")
     0
```

### Comparing `semver-3.0.0rc1/docs/usage/convert-version-into-different-types.rst` & `semver-3.0.1/docs/usage/convert-version-into-different-types.rst`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/usage/create-a-version.rst` & `semver-3.0.1/docs/usage/create-a-version.rst`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/usage/determine-version-equality.rst` & `semver-3.0.1/docs/usage/determine-version-equality.rst`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/usage/get-min-and-max-of-multiple-versions.rst` & `semver-3.0.1/docs/usage/get-min-and-max-of-multiple-versions.rst`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/usage/increase-parts-of-a-version_prereleases.rst` & `semver-3.0.1/docs/usage/increase-parts-of-a-version_prereleases.rst`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/usage/index.rst` & `semver-3.0.1/docs/usage/index.rst`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/usage/parse-version-string.rst` & `semver-3.0.1/docs/usage/parse-version-string.rst`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/usage/raise-parts-of-a-version.rst` & `semver-3.0.1/docs/usage/raise-parts-of-a-version.rst`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/docs/usage/replace-parts-of-a-version.rst` & `semver-3.0.1/docs/usage/replace-parts-of-a-version.rst`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/pyproject.toml` & `semver-3.0.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -6,27 +6,34 @@
 # https://godatadriven.com/blog/a-practical-guide-to-setuptools-and-pyproject-toml/
 
 [build-system]
 requires = [
   # sync with setup.py until we discard non-pep-517/518
   "setuptools",
   "setuptools-scm",
-  "wheel",
-  "build",
 ]
 build-backend = "setuptools.build_meta"
 
 
 
 [tool.black]
 line-length = 88
 target-version = ['py37', 'py38', 'py39', 'py310', 'py311']
 # diff = true
 
 
+[tool.docformatter]
+wrap-summaries = 80
+close-quotes-on-newline = true
+# make-summary-multi-line = true
+black = true
+pre-summary-newline = true
+recursive = true
+
+
 [tool.towncrier]
 package = "semver"
 package_dir = "src"
 filename = "CHANGELOG.rst"
 directory = "changelog.d/"
 title_format = "Version {version}"
 template = "changelog.d/_template.rst"
```

### Comparing `semver-3.0.0rc1/release-procedure.md` & `semver-3.0.1/release-procedure.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,20 +16,21 @@
 
 1. Create a new branch `release/<VERSION>`.
 
 1. If one or several supported Python versions have been removed or added, verify that the 3 following files have been updated:
    * `setup.cfg`
    * `tox.ini`
    * `.git/workflows/pythonpackage.yml`
+   * `CITATION.cff`
 
 1. Verify that the version has been updated and follow
    <https://semver.org>:
 
    * `src/semver/__about__.py`
-   * `docs/usage.rst`
+   * `docs/usage/semver-version.rst`
 
 1. Add eventually new contributor(s) to [CONTRIBUTORS](https://github.com/python-semver/python-semver/blob/master/CONTRIBUTORS).
 
 
 1. Check if all changelog entries are created. If some are missing, [create them](https://python-semver.readthedocs.io/en/latest/development.html#adding-a-changelog-entry).
 
 1. Show the new draft [CHANGELOG](https://github.com/python-semver/python-semver/blob/master/CHANGELOG.rst) entry for the latest release with:
```

### Comparing `semver-3.0.0rc1/setup.cfg` & `semver-3.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/src/semver/__about__.py` & `semver-3.0.1/src/semver/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 .. autodata:: __version__
 
 .. autodata:: SEMVER_SPEC_VERSION
 """
 
 #: Semver version
-__version__ = "3.0.0-rc.1"
+__version__ = "3.0.1"
 
 #: Original semver author
 __author__ = "Kostiantyn Rybnikov"
 
 #: Author's email address
 __author_email__ = "k-bx@k-bx.com"
```

### Comparing `semver-3.0.0rc1/src/semver/__main__.py` & `semver-3.0.1/src/semver/__main__.py`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/src/semver/_deprecated.py` & `semver-3.0.1/src/semver/_deprecated.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 import warnings
 from functools import partial, wraps
 from types import FrameType
 from typing import Type, Callable, Optional, cast
 
 from . import cli
 from .version import Version
-from ._types import Decorator, F, String
+from ._types import Decorator, F
 
 
 def deprecated(
     func: Optional[F] = None,
+    *,
     replace: Optional[str] = None,
     version: Optional[str] = None,
+    remove: Optional[str] = None,
     category: Type[Warning] = DeprecationWarning,
 ) -> Decorator:
     """
     Decorates a function to output a deprecation warning.
 
     :param func: the function to decorate
     :param replace: the function to replace (use the full qualified
@@ -30,23 +32,34 @@
     :param category: allow you to specify the deprecation warning class
         of your choice. By default, it's  :class:`DeprecationWarning`, but
         you can choose :class:`PendingDeprecationWarning` or a custom class.
     :return: decorated function which is marked as deprecated
     """
 
     if func is None:
-        return partial(deprecated, replace=replace, version=version, category=category)
+        return partial(
+            deprecated,
+            replace=replace,
+            version=version,
+            remove=remove,
+            category=category,
+        )
 
     @wraps(func)
     def wrapper(*args, **kwargs) -> Callable[..., F]:
         msg_list = ["Function 'semver.{f}' is deprecated."]
 
         if version:
             msg_list.append("Deprecated since version {v}. ")
-        msg_list.append("This function will be removed in semver 3.")
+
+        if not remove:
+            msg_list.append("This function will be removed in semver 3.")
+        else:
+            msg_list.append(str(remove))
+
         if replace:
             msg_list.append("Use {r!r} instead.")
         else:
             msg_list.append("Use the respective 'semver.Version.{r}' instead.")
 
         f = cast(F, func).__qualname__
         r = replace or f
@@ -65,14 +78,44 @@
         # better remove the interpreter stack:
         del frame
         return func(*args, **kwargs)  # type: ignore
 
     return wrapper
 
 
+@deprecated(
+    version="3.0.0",
+    remove="Still under investigation, see #258.",
+    category=PendingDeprecationWarning,
+)
+def compare(ver1: str, ver2: str) -> int:
+    """
+    Compare two versions strings.
+
+    .. deprecated:: 3.0.0
+       The situation of this function is unclear and it might
+       disappear in the future.
+       If possible, use :meth:`semver.version.Version.compare`.
+       See :gh:`258` for details.
+
+    :param ver1: first version string
+    :param ver2: second version string
+    :return: The return value is negative if ver1 < ver2,
+             zero if ver1 == ver2 and strictly positive if ver1 > ver2
+
+    >>> semver.compare("1.0.0", "2.0.0")
+    -1
+    >>> semver.compare("2.0.0", "1.0.0")
+    1
+    >>> semver.compare("2.0.0", "2.0.0")
+    0
+    """
+    return Version.parse(ver1).compare(ver2)
+
+
 @deprecated(version="2.10.0")
 def parse(version):
     """
     Parse version to major, minor, patch, pre-release, build parts.
 
     .. deprecated:: 2.10.0
        Use :meth:`~semver.version.Version.parse` instead.
@@ -123,36 +166,14 @@
     >>> version_info.build
     'build.4'
     """
     return Version.parse(version)
 
 
 @deprecated(version="2.10.0")
-def compare(ver1, ver2):
-    """
-    Compare two versions strings.
-
-    :param ver1: version string 1
-    :param ver2: version string 2
-    :return: The return value is negative if ver1 < ver2,
-             zero if ver1 == ver2 and strictly positive if ver1 > ver2
-    :rtype: int
-
-    >>> semver.compare("1.0.0", "2.0.0")
-    -1
-    >>> semver.compare("2.0.0", "1.0.0")
-    1
-    >>> semver.compare("2.0.0", "2.0.0")
-    0
-    """
-    v1 = Version.parse(ver1)
-    return v1.compare(ver2)
-
-
-@deprecated(version="2.10.0")
 def match(version, match_expr):
     """
     Compare two versions strings through a comparison.
 
     .. deprecated:: 2.10.0
        Use :meth:`~semver.version.Version.match` instead.
 
@@ -188,23 +209,15 @@
     :param ver2: version string 2
     :return: the greater version of the two
     :rtype: :class:`Version`
 
     >>> semver.max_ver("1.0.0", "2.0.0")
     '2.0.0'
     """
-    if isinstance(ver1, String.__args__):  # type: ignore
-        ver1 = Version.parse(ver1)
-    elif not isinstance(ver1, Version):
-        raise TypeError()
-    cmp_res = ver1.compare(ver2)
-    if cmp_res >= 0:
-        return str(ver1)
-    else:
-        return ver2
+    return str(max(ver1, ver2, key=Version.parse))
 
 
 @deprecated(replace="min", version="2.10.2")
 def min_ver(ver1, ver2):
     """
     Returns the smaller version of two versions strings.
 
@@ -215,20 +228,15 @@
     :param ver2: version string 2
     :return: the smaller version of the two
     :rtype: :class:`Version`
 
     >>> semver.min_ver("1.0.0", "2.0.0")
     '1.0.0'
     """
-    ver1 = Version.parse(ver1)
-    cmp_res = ver1.compare(ver2)
-    if cmp_res <= 0:
-        return str(ver1)
-    else:
-        return ver2
+    return str(min(ver1, ver2, key=Version.parse))
 
 
 @deprecated(replace="str(versionobject)", version="2.10.0")
 def format_version(major, minor, patch, prerelease=None, build=None):
     """
     Format a version string according to the Semantic Versioning specification.
 
@@ -383,14 +391,20 @@
     >>> semver.replace("1.2.3", major=2, patch=10)
     '2.2.10'
     """
     return str(Version.parse(version).replace(**parts))
 
 
 # CLI
-cmd_bump = deprecated(cli.cmd_bump, "semver.cli.cmd_bump", "3.0.0")
-cmd_check = deprecated(cli.cmd_check, "semver.cli.cmd_check", "3.0.0")
-cmd_compare = deprecated(cli.cmd_compare, "semver.cli.cmd_compare", "3.0.0")
-cmd_nextver = deprecated(cli.cmd_nextver, "semver.cli.cmd_nextver", "3.0.0")
-createparser = deprecated(cli.createparser, "semver.cli.createparser", "3.0.0")
-process = deprecated(cli.process, "semver.cli.process", "3.0.0")
-main = deprecated(cli.main, "semver.cli.main", "3.0.0")
+cmd_bump = deprecated(cli.cmd_bump, replace="semver.cli.cmd_bump", version="3.0.0")
+cmd_check = deprecated(cli.cmd_check, replace="semver.cli.cmd_check", version="3.0.0")
+cmd_compare = deprecated(
+    cli.cmd_compare, replace="semver.cli.cmd_compare", version="3.0.0"
+)
+cmd_nextver = deprecated(
+    cli.cmd_nextver, replace="semver.cli.cmd_nextver", version="3.0.0"
+)
+createparser = deprecated(
+    cli.createparser, replace="semver.cli.createparser", version="3.0.0"
+)
+process = deprecated(cli.process, replace="semver.cli.process", version="3.0.0")
+main = deprecated(cli.main, replace="semver.cli.main", version="3.0.0")
```

### Comparing `semver-3.0.0rc1/src/semver/cli.py` & `semver-3.0.1/src/semver/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     if Version.is_valid(args.version):
         return None
     raise ValueError("Invalid version %r" % args.version)
 
 
 def cmd_compare(args: argparse.Namespace) -> str:
     """
-    Subcommand: Compare two versions
+    Subcommand: Compare two versions.
 
     Synopsis: compare <VERSION1> <VERSION2>
 
     :param args: The parsed arguments
     """
     ver1 = Version.parse(args.version1)
     return str(ver1.compare(args.version2))
```

### Comparing `semver-3.0.0rc1/src/semver/version.py` & `semver-3.0.1/src/semver/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,16 +60,15 @@
 class Version:
     """
     A semver compatible version class.
 
     See specification at https://semver.org.
 
     :param major: version when you make incompatible API changes.
-    :param minor: version when you add functionality in
-                  a backwards-compatible manner.
+    :param minor: version when you add functionality in a backwards-compatible manner.
     :param patch: version when you make backwards-compatible bug fixes.
     :param prerelease: an optional prerelease string
     :param build: an optional build string
     """
 
     __slots__ = ("_major", "_minor", "_patch", "_prerelease", "_build")
 
@@ -428,15 +427,15 @@
         Determines next version, preserving natural order.
 
         .. versionadded:: 2.10.0
 
         This function is taking prereleases into account.
         The "major", "minor", and "patch" raises the respective parts like
         the ``bump_*`` functions. The real difference is using the
-        "preprelease" part. It gives you the next patch version of the
+        "prerelease" part. It gives you the next patch version of the
         prerelease, for example:
 
         >>> str(semver.parse("0.1.4").next_version("prerelease"))
         '0.1.5-rc.1'
 
         :param part: One of "major", "minor", "patch", or "prerelease"
         :param prerelease_token: prefix string of prerelease, defaults to 'rc'
```

### Comparing `semver-3.0.0rc1/src/semver.egg-info/PKG-INFO` & `semver-3.0.1/src/semver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semver
-Version: 3.0.0rc1
+Version: 3.0.1
 Summary: Python helper for Semantic Versioning (https://semver.org)
 Home-page: https://github.com/python-semver/python-semver
 Author: Kostiantyn Rybnikov
 Author-email: k-bx@k-bx.com
 Maintainer: Sebastien Celles, Tom Schraitle
 Maintainer-email: s.celles@gmail.com
 License: BSD
```

### Comparing `semver-3.0.0rc1/src/semver.egg-info/SOURCES.txt` & `semver-3.0.1/src/semver.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .coveragerc
 .editorconfig
 .gitignore
 CHANGELOG.rst
+CITATION.cff
 CONTRIBUTING.rst
 CONTRIBUTORS
 LICENSE.txt
 MANIFEST.in
 Makefile
 README.rst
 pyproject.toml
@@ -14,15 +15,14 @@
 tox.ini
 changelog.d/.gitignore
 changelog.d/README.rst
 changelog.d/_template.rst
 docs/Makefile
 docs/api.rst
 docs/build-semver.rst
-docs/changelog-semver2.rst
 docs/changelog-semver3-devel.rst
 docs/changelog.rst
 docs/conf.py
 docs/index.rst
 docs/install.rst
 docs/make.bat
 docs/pysemver.rst
@@ -44,14 +44,15 @@
 docs/contribute/doc-semver.rst
 docs/contribute/finish-release.rst
 docs/contribute/index.rst
 docs/contribute/prerequisites.rst
 docs/contribute/release-procedure.rst
 docs/contribute/report-bugs.rst
 docs/contribute/run-test-suite.rst
+docs/inventories/python-objects.inv
 docs/migration/index.rst
 docs/migration/migratetosemver3.rst
 docs/migration/replace-deprecated-functions.rst
 docs/usage/access-parts-of-a-version.rst
 docs/usage/access-parts-through-index.rst
 docs/usage/check-compatible-semver-version.rst
 docs/usage/check-valid-semver-version.rst
```

### Comparing `semver-3.0.0rc1/tests/coerce.py` & `semver-3.0.1/tests/coerce.py`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/tests/conftest.py` & `semver-3.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/tests/semverwithvprefix.py` & `semver-3.0.1/tests/semverwithvprefix.py`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/tests/test_bump.py` & `semver-3.0.1/tests/test_bump.py`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/tests/test_compare.py` & `semver-3.0.1/tests/test_compare.py`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/tests/test_deprecated_functions.py` & `semver-3.0.1/tests/test_deprecated_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from argparse import Namespace
 
 import pytest
 
 from semver import (
     parse,
     parse_version_info,
-    compare,
     match,
     max_ver,
     min_ver,
     format_version,
     bump_major,
     bump_minor,
     bump_patch,
@@ -32,15 +31,14 @@
     "func, args, kwargs",
     [
         (bump_build, ("1.2.3",), {}),
         (bump_major, ("1.2.3",), {}),
         (bump_minor, ("1.2.3",), {}),
         (bump_patch, ("1.2.3",), {}),
         (bump_prerelease, ("1.2.3",), {}),
-        (compare, ("1.2.1", "1.2.2"), {}),
         (format_version, (3, 4, 5), {}),
         (finalize_version, ("1.2.3-rc.5",), {}),
         (match, ("1.0.0", ">=1.0.0"), {}),
         (parse, ("1.2.3",), {}),
         (parse_version_info, ("1.2.3",), {}),
         (replace, ("1.2.3",), dict(major=2, patch=10)),
         (max_ver, ("1.2.3", "1.2.4"), {}),
```

### Comparing `semver-3.0.0rc1/tests/test_docstrings.py` & `semver-3.0.1/tests/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/tests/test_format.py` & `semver-3.0.1/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/tests/test_immutable.py` & `semver-3.0.1/tests/test_immutable.py`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/tests/test_index.py` & `semver-3.0.1/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/tests/test_match.py` & `semver-3.0.1/tests/test_match.py`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/tests/test_max-min.py` & `semver-3.0.1/tests/test_max-min.py`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/tests/test_parsing.py` & `semver-3.0.1/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/tests/test_pysemver-cli.py` & `semver-3.0.1/tests/test_pysemver-cli.py`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/tests/test_replace.py` & `semver-3.0.1/tests/test_replace.py`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/tests/test_semver.py` & `semver-3.0.1/tests/test_semver.py`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/tests/test_subclass.py` & `semver-3.0.1/tests/test_subclass.py`

 * *Files identical despite different names*

### Comparing `semver-3.0.0rc1/tox.ini` & `semver-3.0.1/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -52,30 +52,31 @@
 commands = mypy {posargs:--ignore-missing-imports --check-untyped-defs src}
 
 
 [testenv:docstrings]
 description = Check for PEP257 compatible docstrings
 basepython = python3
 deps = docformatter
-commands = docformatter --check --diff {posargs:--pre-summary-newline -r src}
+commands =
+	docformatter --check --diff {posargs:src}
 
 
 [testenv:checks]
 description = Run code style checks
 basepython = python3
 deps =
     {[testenv:black]deps}
     {[testenv:flake8]deps}
     {[testenv:mypy]deps}
     {[testenv:docstrings]deps}
 commands =
+    - {[testenv:docstrings]commands}
     {[testenv:black]commands}
     {[testenv:flake8]commands}
     {[testenv:mypy]commands}
-    {[testenv:docstrings]commands}
 
 
 [testenv:docs]
 description = Build HTML documentation
 basepython = python3
 deps = -r{toxinidir}/docs/requirements.txt
 skip_install = true
@@ -95,17 +96,15 @@
 commands = make -C docs man
 
 
 [testenv:prepare-dist]
 description = Prepare for TestPyPI
 basepython = python3
 deps =
-    wheel
     twine
-    # PEP 517 build frontend
     build
 commands =
     # Same as python3 -m build
     pyproject-build
     twine check dist/*
```

