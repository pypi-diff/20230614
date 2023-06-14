# Comparing `tmp/intake-esm-2022.9.18.tar.gz` & `tmp/intake-esm-2023.4.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intake-esm-2022.9.18.tar", last modified: Sun Sep 18 01:54:29 2022, max compression
+gzip compressed data, was "intake-esm-2023.4.20.tar", last modified: Thu Apr 20 13:42:04 2023, max compression
```

## Comparing `intake-esm-2022.9.18.tar` & `intake-esm-2023.4.20.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 01:54:29.992578 intake-esm-2022.9.18/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 01:54:29.988578 intake-esm-2022.9.18/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 01:54:29.988578 intake-esm-2022.9.18/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)     1257 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (121)      594 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (121)      815 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 01:54:29.988578 intake-esm-2022.9.18/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2287 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      966 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1407 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      945 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/.prettierrc.toml
--rw-r--r--   0 runner    (1001) docker     (121)    50713 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     4595 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)    11390 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1151 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     6925 2022-09-18 01:54:29.992578 intake-esm-2022.9.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5810 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 01:54:29.988578 intake-esm-2022.9.18/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     6788 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 01:54:29.984578 intake-esm-2022.9.18/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 01:54:29.988578 intake-esm-2022.9.18/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (121)    22404 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/docs/_static/images/NSF_4-Color_bitmap_Logo.png
--rw-r--r--   0 runner    (1001) docker     (121)    16213 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/docs/_static/images/nsf.png
--rw-r--r--   0 runner    (1001) docker     (121)     6467 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 01:54:29.988578 intake-esm-2022.9.18/docs/source/
--rw-r--r--   0 runner    (1001) docker     (121)     3791 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/docs/source/catalogs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     5390 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/docs/source/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 01:54:29.988578 intake-esm-2022.9.18/docs/source/how-to/
--rw-r--r--   0 runner    (1001) docker     (121)     6422 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/docs/source/how-to/build-a-catalog-from-timeseries-files.md
--rw-r--r--   0 runner    (1001) docker     (121)     5925 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/docs/source/how-to/define-and-use-derived-variable-registry.md
--rw-r--r--   0 runner    (1001) docker     (121)     2607 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/docs/source/how-to/enforce-search-query-criteria-via-require-all-on.md
--rw-r--r--   0 runner    (1001) docker     (121)     1553 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/docs/source/how-to/filter-catalog-by-substring-and-regex-criteria.md
--rw-r--r--   0 runner    (1001) docker     (121)      755 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/docs/source/how-to/install-intake-esm.md
--rw-r--r--   0 runner    (1001) docker     (121)     4263 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/docs/source/how-to/modify-catalog.md
--rw-r--r--   0 runner    (1001) docker     (121)     1228 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/docs/source/how-to/multi-variable-catalog.csv
--rw-r--r--   0 runner    (1001) docker     (121)     1229 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/docs/source/how-to/multi-variable-catalog.json
--rw-r--r--   0 runner    (1001) docker     (121)     4685 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/docs/source/how-to/understand-keys-and-how-to-change-them.md
--rw-r--r--   0 runner    (1001) docker     (121)     2370 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/docs/source/how-to/use-catalogs-with-assets-containing-multiple-variables.md
--rw-r--r--   0 runner    (1001) docker     (121)     2964 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/docs/source/index.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 01:54:29.988578 intake-esm-2022.9.18/docs/source/reference/
--rw-r--r--   0 runner    (1001) docker     (121)     1129 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/docs/source/reference/api.md
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/docs/source/reference/changelog.md
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/docs/source/reference/cmip_ap.md
--rw-r--r--   0 runner    (1001) docker     (121)     9935 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/docs/source/reference/esm-catalog-spec.md
--rw-r--r--   0 runner    (1001) docker     (121)     1114 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/docs/source/reference/faq.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 01:54:29.988578 intake-esm-2022.9.18/docs/source/tutorials/
--rw-r--r--   0 runner    (1001) docker     (121)     7011 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/docs/source/tutorials/loading-cmip6-data.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 01:54:29.992578 intake-esm-2022.9.18/intake_esm/
--rw-r--r--   0 runner    (1001) docker     (121)      543 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/intake_esm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3517 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/intake_esm/_search.py
--rw-r--r--   0 runner    (1001) docker     (121)    15515 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/intake_esm/cat.py
--rw-r--r--   0 runner    (1001) docker     (121)    32052 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/intake_esm/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     7583 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/intake_esm/derived.py
--rw-r--r--   0 runner    (1001) docker     (121)    10236 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/intake_esm/source.py
--rw-r--r--   0 runner    (1001) docker     (121)     1531 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/intake_esm/tutorial.py
--rw-r--r--   0 runner    (1001) docker     (121)     3658 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/intake_esm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 01:54:29.992578 intake-esm-2022.9.18/intake_esm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6925 2022-09-18 01:54:29.000000 intake-esm-2022.9.18/intake_esm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1902 2022-09-18 01:54:29.000000 intake-esm-2022.9.18/intake_esm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-18 01:54:29.000000 intake-esm-2022.9.18/intake_esm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-09-18 01:54:29.000000 intake-esm-2022.9.18/intake_esm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-18 01:54:29.000000 intake-esm-2022.9.18/intake_esm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-09-18 01:54:29.000000 intake-esm-2022.9.18/intake_esm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-09-18 01:54:29.000000 intake-esm-2022.9.18/intake_esm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-09-18 01:54:29.992578 intake-esm-2022.9.18/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1985 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 01:54:29.992578 intake-esm-2022.9.18/tutorial-catalogs/
--rw-r--r--   0 runner    (1001) docker     (121)    11546 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/tutorial-catalogs/AWS-CESM2-LENS.json
--rw-r--r--   0 runner    (1001) docker     (121)    16770 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/tutorial-catalogs/AWS-CMIP6.json
--rw-r--r--   0 runner    (1001) docker     (121)   108734 2022-09-18 01:54:10.000000 intake-esm-2022.9.18/tutorial-catalogs/GOOGLE-CMIP6.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:04.467929 intake-esm-2023.4.20/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:04.459928 intake-esm-2023.4.20/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:04.459928 intake-esm-2023.4.20/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:04.459928 intake-esm-2023.4.20/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/.prettierrc.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    51207 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-04-20 13:42:04.467929 intake-esm-2023.4.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:04.459928 intake-esm-2023.4.20/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:04.451928 intake-esm-2023.4.20/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:04.459928 intake-esm-2023.4.20/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    22404 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/docs/_static/images/NSF_4-Color_bitmap_Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/docs/_static/images/nsf.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:04.459928 intake-esm-2023.4.20/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/docs/source/catalogs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/docs/source/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:04.463928 intake-esm-2023.4.20/docs/source/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/docs/source/how-to/build-a-catalog-from-timeseries-files.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/docs/source/how-to/define-and-use-derived-variable-registry.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/docs/source/how-to/enforce-search-query-criteria-via-require-all-on.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/docs/source/how-to/filter-catalog-by-substring-and-regex-criteria.md
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/docs/source/how-to/install-intake-esm.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/docs/source/how-to/modify-catalog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/docs/source/how-to/multi-variable-catalog.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/docs/source/how-to/multi-variable-catalog.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/docs/source/how-to/understand-keys-and-how-to-change-them.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/docs/source/how-to/use-catalogs-with-assets-containing-multiple-variables.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/docs/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:04.463928 intake-esm-2023.4.20/docs/source/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/docs/source/reference/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/docs/source/reference/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/docs/source/reference/cmip_ap.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9985 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/docs/source/reference/esm-catalog-spec.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/docs/source/reference/faq.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:04.463928 intake-esm-2023.4.20/docs/source/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/docs/source/tutorials/loading-cmip6-data.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:04.463928 intake-esm-2023.4.20/intake_esm/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/intake_esm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/intake_esm/_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15482 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/intake_esm/cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32760 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/intake_esm/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/intake_esm/derived.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10233 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/intake_esm/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/intake_esm/tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/intake_esm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:04.467929 intake-esm-2023.4.20/intake_esm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-04-20 13:42:04.000000 intake-esm-2023.4.20/intake_esm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-04-20 13:42:04.000000 intake-esm-2023.4.20/intake_esm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 13:42:04.000000 intake-esm-2023.4.20/intake_esm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-20 13:42:04.000000 intake-esm-2023.4.20/intake_esm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 13:42:03.000000 intake-esm-2023.4.20/intake_esm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-20 13:42:04.000000 intake-esm-2023.4.20/intake_esm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-20 13:42:04.000000 intake-esm-2023.4.20/intake_esm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 13:42:04.467929 intake-esm-2023.4.20/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:04.467929 intake-esm-2023.4.20/tutorial-catalogs/
+-rw-r--r--   0 runner    (1001) docker     (123)    11546 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/tutorial-catalogs/AWS-CESM2-LENS.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16770 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/tutorial-catalogs/AWS-CMIP6.json
+-rw-r--r--   0 runner    (1001) docker     (123)   108734 2023-04-20 13:41:43.000000 intake-esm-2023.4.20/tutorial-catalogs/GOOGLE-CMIP6.json
```

### Comparing `intake-esm-2022.9.18/.github/ISSUE_TEMPLATE/bug_report.md` & `intake-esm-2023.4.20/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `intake-esm-2022.9.18/.github/ISSUE_TEMPLATE/feature_request.md` & `intake-esm-2023.4.20/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `intake-esm-2022.9.18/.github/pull_request_template.md` & `intake-esm-2023.4.20/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `intake-esm-2022.9.18/.github/workflows/ci.yaml` & `intake-esm-2023.4.20/.github/workflows/ci.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     timeout-minutes: 30
     defaults:
       run:
         shell: bash -l {0}
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.8', '3.9', '3.10']
+        python-version: ['3.9', '3.10', '3.11']
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0 # Fetch all history for all branches and tags.
 
       - name: Create conda environment
         uses: mamba-org/provision-with-micromamba@main
@@ -45,15 +45,15 @@
           conda list
 
       - name: Run Tests
         run: |
           python -m pytest
 
       - name: Upload code coverage to Codecov
-        uses: codecov/codecov-action@v3.1.0
+        uses: codecov/codecov-action@v3.1.1
         with:
           file: ./coverage.xml
           flags: unittests
           env_vars: OS,PYTHON
           name: codecov-umbrella
           fail_ci_if_error: false
 
@@ -73,15 +73,15 @@
       - name: Create conda environment
         uses: mamba-org/provision-with-micromamba@main
         with:
           cache-downloads: true
           micromamba-version: 'latest'
           environment-file: ci/environment-upstream-dev.yml
           extra-specs: |
-            python=3.10
+            python=3.11
 
       - name: Install intake-esm
         run: |
           python -m pip install -e . --no-deps --force-reinstall
           conda list
 
       - name: Run Tests
```

### Comparing `intake-esm-2022.9.18/.gitignore` & `intake-esm-2023.4.20/.gitignore`

 * *Files identical despite different names*

### Comparing `intake-esm-2022.9.18/.pre-commit-config.yaml` & `intake-esm-2023.4.20/.pre-commit-config.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,36 @@
+ci:
+  autoupdate_schedule: monthly
+
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-docstring-first
       - id: check-json
       - id: check-yaml
       - id: double-quote-string-fixer
       - id: debug-statements
       - id: mixed-line-ending
 
-  - repo: https://github.com/asottile/pyupgrade
-    rev: v2.37.3
+  - repo: https://github.com/charliermarsh/ruff-pre-commit
+    rev: 'v0.0.260'
     hooks:
-      - id: pyupgrade
-        args:
-          - '--py37-plus'
+      - id: ruff
+        args: ['--fix']
 
   - repo: https://github.com/psf/black
-    rev: 22.8.0
+    rev: 23.3.0
     hooks:
       - id: black-jupyter
 
   - repo: https://github.com/keewis/blackdoc
-    rev: v0.3.6
+    rev: v0.3.8
     hooks:
       - id: blackdoc
 
-  - repo: https://github.com/PyCQA/flake8
-    rev: 5.0.4
-    hooks:
-      - id: flake8
-
-  - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
-    hooks:
-      - id: isort
-
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.0.0-alpha.0
+    rev: v3.0.0-alpha.6
     hooks:
       - id: prettier
```

### Comparing `intake-esm-2022.9.18/CHANGELOG.md` & `intake-esm-2023.4.20/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Changelog
 
+## Unreleased
+
+### New features added
+
+- Fix the link to documentation build status [#591](https://github.com/intake/intake-esm/pull/591) ([@mgrover1](https://github.com/mgrover1))
+- Add optional `columns_with_iterables` argument to `esm_datastore` [#589](https://github.com/intake/intake-esm/pull/589) ([@dougiesquire](https://github.com/dougiesquire))
+- Add `opendap` as a possible data format [#570](https://github.com/intake/intake-esm/pull/570) ([@aulemahal](https://github.com/aulemahal))
+
 ## v2022.9.18
 
 ([full changelog](https://github.com/intake/intake-esm/compare/v2021.8.17...3e959d126663f9b8415528bfcee575967c3ef0c1))
 
 ### New features added
 
 - Add `to_dask()` method to `esm_datastore` [#403](https://github.com/intake/intake-esm/pull/403) ([@d70-t](https://github.com/d70-t))
@@ -467,15 +475,15 @@
 
 - Add `mistral` data holdings to `intake-esm-datastore` ({pr}`133`) [@aaronspring](https://github.com/aaronspring)
 
 - Add support for `NA-CORDEX` data holdings. ({pr}`115`) [@jukent](https://github.com/jukent)
 
 - Replace `.csv` with `netCDF` as serialization format when saving the built collection to disk. With `netCDF`, we can record very useful information into the global attributes of the netCDF dataset. ({pr}`119`) [@andersy005](https://github.com/andersy005)
 
-- Add string representation of ` ESMMetadataStoreCatalog`` object ({pr} `122`) [@andersy005](https://github.com/andersy005)
+- Add string representation of `ESMMetadataStoreCatalog`` object ({pr}`122`) [@andersy005](https://github.com/andersy005)
 
 - Automatically build missing collections by calling `esm_metadatastore(collection_name="GLADE-CMIP5")`. When the specified collection is part of the curated collections in `intake-esm-datastore`. ({pr}`124`) [@andersy005](https://github.com/andersy005)
 
   ```python
 
   In [1]: import intake
```

### Comparing `intake-esm-2022.9.18/CONTRIBUTING.md` & `intake-esm-2023.4.20/CONTRIBUTING.md`

 * *Files 12% similar despite different names*

```diff
@@ -55,17 +55,19 @@
 - More complementary documentation. Have you perhaps found something unclear?
 - Docstrings. There can never be too many of them.
 - Blog posts, articles and such -- they're all very appreciated.
 
 You can also edit documentation files directly in the GitHub web interface,
 without using a local copy. This can be convenient for small fixes.
 
-Build the documentation locally with the following command:
+To build the docs locally, follow the steps 1 and 2 under [Preparing Pull Requests](#preparing-pull-requests) below and then create a conda environment and build the docs with the following commands:
 
 ```bash
+$ conda env update -f ci/environment-docs.yml
+$ conda activate intake-esm-doc
 $ make docs
 ```
 
 ## Preparing Pull Requests
 
 1. Fork the [intake-esm GitHub repository](https://github.com/intake/intake-esm).
```

### Comparing `intake-esm-2022.9.18/LICENSE` & `intake-esm-2023.4.20/LICENSE`

 * *Files identical despite different names*

### Comparing `intake-esm-2022.9.18/Makefile` & `intake-esm-2023.4.20/Makefile`

 * *Files identical despite different names*

### Comparing `intake-esm-2022.9.18/PKG-INFO` & `intake-esm-2023.4.20/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intake-esm
-Version: 2022.9.18
+Version: 2023.4.20
 Summary: An intake plugin for parsing an Earth System Model (ESM) catalog and loading netCDF files and/or Zarr stores into Xarray datasets.
 Home-page: https://intake-esm.readthedocs.io
 Maintainer: NCAR XDev Team
 Maintainer-email: xdev@ucar.edu
 License: Apache 2.0
 Project-URL: Documentation, https://intake-esm.readthedocs.io
 Project-URL: Source, https://github.com/intake/intake-esm
@@ -12,19 +12,19 @@
 Keywords: intake,xarray,catalog
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Intake-esm
 
 - [Intake-esm](#intake-esm)
   - [Badges](#badges)
@@ -116,19 +116,19 @@
 
 It is also available from `conda-forge` for conda installations:
 
 ```bash
 conda install -c conda-forge intake-esm
 ```
 
-[github-ci-badge]: https://img.shields.io/github/workflow/status/intake/intake-esm/CI?label=CI&logo=github
-[github-ci-link]: https://github.com/intake/intake-esm/actions?query=workflow%3ACI
+[github-ci-badge]: https://github.com/intake/intake-esm/actions/workflows/ci.yaml/badge.svg
+[github-ci-link]: https://github.com/intake/intake-esm/actions/workflows/ci.yaml
 [codecov-badge]: https://img.shields.io/codecov/c/github/intake/intake-esm.svg?logo=codecov
 [codecov-link]: https://codecov.io/gh/intake/intake-esm
-[rtd-badge]: https://img.shields.io/readthedocs/intake-esm/latest.svg
+[rtd-badge]: https://readthedocs.org/projects/intake-esm/badge/?version=latest
 [rtd-link]: https://intake-esm.readthedocs.io/en/latest/?badge=latest
 [pypi-badge]: https://img.shields.io/pypi/v/intake-esm?logo=pypi
 [pypi-link]: https://pypi.org/project/intake-esm
 [conda-badge]: https://img.shields.io/conda/vn/conda-forge/intake-esm?logo=anaconda
 [conda-link]: https://anaconda.org/conda-forge/intake-esm
 [zenodo-badge]: https://img.shields.io/badge/DOI-10.5281%20%2F%20zenodo.3491062-blue.svg
 [zenodo-link]: https://doi.org/10.5281/zenodo.3491062
```

### Comparing `intake-esm-2022.9.18/README.md` & `intake-esm-2023.4.20/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -90,19 +90,19 @@
 
 It is also available from `conda-forge` for conda installations:
 
 ```bash
 conda install -c conda-forge intake-esm
 ```
 
-[github-ci-badge]: https://img.shields.io/github/workflow/status/intake/intake-esm/CI?label=CI&logo=github
-[github-ci-link]: https://github.com/intake/intake-esm/actions?query=workflow%3ACI
+[github-ci-badge]: https://github.com/intake/intake-esm/actions/workflows/ci.yaml/badge.svg
+[github-ci-link]: https://github.com/intake/intake-esm/actions/workflows/ci.yaml
 [codecov-badge]: https://img.shields.io/codecov/c/github/intake/intake-esm.svg?logo=codecov
 [codecov-link]: https://codecov.io/gh/intake/intake-esm
-[rtd-badge]: https://img.shields.io/readthedocs/intake-esm/latest.svg
+[rtd-badge]: https://readthedocs.org/projects/intake-esm/badge/?version=latest
 [rtd-link]: https://intake-esm.readthedocs.io/en/latest/?badge=latest
 [pypi-badge]: https://img.shields.io/pypi/v/intake-esm?logo=pypi
 [pypi-link]: https://pypi.org/project/intake-esm
 [conda-badge]: https://img.shields.io/conda/vn/conda-forge/intake-esm?logo=anaconda
 [conda-link]: https://anaconda.org/conda-forge/intake-esm
 [zenodo-badge]: https://img.shields.io/badge/DOI-10.5281%20%2F%20zenodo.3491062-blue.svg
 [zenodo-link]: https://doi.org/10.5281/zenodo.3491062
```

### Comparing `intake-esm-2022.9.18/docs/Makefile` & `intake-esm-2023.4.20/docs/Makefile`

 * *Files identical despite different names*

### Comparing `intake-esm-2022.9.18/docs/_static/images/NSF_4-Color_bitmap_Logo.png` & `intake-esm-2023.4.20/docs/_static/images/NSF_4-Color_bitmap_Logo.png`

 * *Files identical despite different names*

### Comparing `intake-esm-2022.9.18/docs/_static/images/nsf.png` & `intake-esm-2023.4.20/docs/_static/images/nsf.png`

 * *Files identical despite different names*

### Comparing `intake-esm-2022.9.18/docs/make.bat` & `intake-esm-2023.4.20/docs/make.bat`

 * *Files identical despite different names*

### Comparing `intake-esm-2022.9.18/docs/source/catalogs.yaml` & `intake-esm-2023.4.20/docs/source/catalogs.yaml`

 * *Files identical despite different names*

### Comparing `intake-esm-2022.9.18/docs/source/conf.py` & `intake-esm-2023.4.20/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `intake-esm-2022.9.18/docs/source/how-to/build-a-catalog-from-timeseries-files.md` & `intake-esm-2023.4.20/docs/source/how-to/build-a-catalog-from-timeseries-files.md`

 * *Files 2% similar despite different names*

```diff
@@ -53,17 +53,19 @@
 ## Import packages
 
 The only parts of ecgtools we need are the `Builder` object and the `parse_cesm_history` parser from the CESM parsers! We import `pathlib` to take a look at the files we are parsing.
 
 ```{code-cell} ipython3
 import pathlib
 
+import dask
 import intake
 from ecgtools import Builder
 from ecgtools.parsers.cesm import parse_cesm_timeseries
+
 ```
 
 ## Understanding the directory structure
 
 The first step to setting up the `Builder` object is determining where your files are stored. As mentioned previously, we have a sample dataset of CESM2 model output, which is stored in test directory `/tests/sample_data` directory of this repository.
 
 Taking a look at that directory, we see that there is a single case `g.e11_LENS.GECOIAF.T62_g16.009`
@@ -80,30 +82,30 @@
 
 Let's start by setting the builder object up.
 
 ```{code-cell} ipython3
 
 cat_builder = Builder(
     # Directory with the output
-    root_path=root_path,
+    paths=['../../../tests/sample_data/cesm/'],
     # Depth of 1 since we are sending it to the case output directory
     depth=1,
     # Exclude the timeseries and restart directories
     exclude_patterns=["*/tseries/*", "*/rest/*"],
     # Number of jobs to execute - should be equal to # threads you are using
-    njobs=5,
+    joblib_parallel_kwargs={'n_jobs': -1},
 )
 
 cat_builder
 ```
 
 We are good to go! Let's build the catalog by calling `.build()` on the object, passing in the `parse_cesm_history` parser, which is a built-in parser for CESM history files.
 
 ```{code-cell} ipython3
-cat_builder = cat_builder.build(parse_cesm_timeseries)
+cat_builder = cat_builder.build(parsing_func=parse_cesm_timeseries)
 ```
 
 ## Inspect the built catalog
 
 Now that the catalog is built, we can inspect the dataframe which is used to create the catalog by calling `.df` on the builder object:
 
 ```{code-cell} ipython3
@@ -130,15 +132,16 @@
 
 ## Save the catalog
 
 Now that we have our data catalog, we can save it, by specifying the path to the comma separated values file (`csv`) or compressed csv (`csv.gz`).
 
 ```{code-cell} ipython3
 cat_builder.save(
-    '/tmp/cesm_sample_data.csv',
+    name='cesm_sample_data',
+    directory='/tmp',
     # Column name including filepath
     path_column_name='path',
     # Column name including variables
     variable_column_name='variable',
     # Data file format - could be netcdf or zarr (in this case, netcdf)
     data_format="netcdf",
     # Which attributes to groupby when reading in variables using intake-esm
```

### Comparing `intake-esm-2022.9.18/docs/source/how-to/define-and-use-derived-variable-registry.md` & `intake-esm-2023.4.20/docs/source/how-to/define-and-use-derived-variable-registry.md`

 * *Files identical despite different names*

### Comparing `intake-esm-2022.9.18/docs/source/how-to/enforce-search-query-criteria-via-require-all-on.md` & `intake-esm-2023.4.20/docs/source/how-to/enforce-search-query-criteria-via-require-all-on.md`

 * *Files identical despite different names*

### Comparing `intake-esm-2022.9.18/docs/source/how-to/filter-catalog-by-substring-and-regex-criteria.md` & `intake-esm-2023.4.20/docs/source/how-to/filter-catalog-by-substring-and-regex-criteria.md`

 * *Files identical despite different names*

### Comparing `intake-esm-2022.9.18/docs/source/how-to/install-intake-esm.md` & `intake-esm-2023.4.20/docs/source/how-to/install-intake-esm.md`

 * *Files identical despite different names*

### Comparing `intake-esm-2022.9.18/docs/source/how-to/modify-catalog.md` & `intake-esm-2023.4.20/docs/source/how-to/modify-catalog.md`

 * *Files identical despite different names*

### Comparing `intake-esm-2022.9.18/docs/source/how-to/multi-variable-catalog.csv` & `intake-esm-2023.4.20/docs/source/how-to/multi-variable-catalog.csv`

 * *Files identical despite different names*

### Comparing `intake-esm-2022.9.18/docs/source/how-to/multi-variable-catalog.json` & `intake-esm-2023.4.20/docs/source/how-to/multi-variable-catalog.json`

 * *Files identical despite different names*

### Comparing `intake-esm-2022.9.18/docs/source/how-to/understand-keys-and-how-to-change-them.md` & `intake-esm-2023.4.20/docs/source/how-to/understand-keys-and-how-to-change-them.md`

 * *Files identical despite different names*

### Comparing `intake-esm-2022.9.18/docs/source/how-to/use-catalogs-with-assets-containing-multiple-variables.md` & `intake-esm-2023.4.20/docs/source/how-to/use-catalogs-with-assets-containing-multiple-variables.md`

 * *Files 25% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ---
 
 # Use catalogs with assets containing multiple variables
 
 By default, `intake-esm` assumes that the data assets (files) contain a single variable (e.g. `temperature`, `precipitation`, etc..). If you have multiple variables in your data files, intake-esm requires the following:
 
 - the `variable_column` of the catalog must contain iterables (list, tuple, set) of values (e.g. `['temperature', 'precipitation']`).
-- the user must provide a `converters` dictionary with appropriate functions for parsing values in the `variable_column` and/or any other column with iterables into iterables when loading the catalog. This is done via the `read_csv_kwargs` argument of the `open_esm_datastore` function.
+- the user must provide converters with appropriate functions for parsing values in the `variable_column` (and/or any other column with iterables) into iterables when loading the catalog. There are two ways to do this with the `open_esm_datastore` function: either pass the converter functions directly through the `read_csv_kwargs` argument, or specify the columns in `columns_with_iterables` parameter. The latter is a shortcut for the former. Both are demonstrated below.
 
 ## Inspect the catalog
 
 In the example below, we are are going to use the following catalog to
 demonstrate how to work with multi-variable assets:
 
 ```{code-cell} ipython3
@@ -29,28 +29,42 @@
 `"['SHF', 'REGION_MASK', 'ANGLE', 'DXU', 'KMT', 'NO2', 'O2']"`.
 
 ## Load the catalog
 
 ```{code-cell} ipython3
 import intake
 import ast
+import dask
+
+# Make sure this is single-threaded
+dask.config.set(scheduler='single-threaded')
 
 cat = intake.open_esm_datastore(
     "multi-variable-catalog.json",
     read_csv_kwargs={"converters": {"variable": ast.literal_eval}},
 )
 cat
 ```
 
 To confirm that intake-esm has loaded the catalog correctly, we can inspect the `.has_multiple_variable_assets` property:
 
 ```{code-cell} ipython3
 cat.esmcat.has_multiple_variable_assets
 ```
 
+Alternatively, we can specify the variable column name in the `columns_with_iterables` parameter:
+
+```{code-cell} ipython3
+cat = intake.open_esm_datastore(
+    "multi-variable-catalog.json",
+    columns_with_iterables=["variable"],
+)
+cat.esmcat.has_multiple_variable_assets
+```
+
 ## Search for datasets
 
 The search functionatilty works in the same way:
 
 ```{code-cell} ipython3
 cat_subset =cat.search(variable=["O2", "SiO3"])
 cat_subset.df
@@ -61,14 +75,23 @@
 When loading the data files into xarray datasets, `intake-esm` will load only **data variables** that were requested. For example, if a data file contains ten data variables and the user requests for two variables, intake-esm will load the two requested variables plus necessary coordinates information.
 
 ```{code-cell} ipython3
 dsets = cat_subset.to_dataset_dict()
 dsets
 ```
 
+## Why does `intake.open_esm_datastore` need the `columns_with_iterables` parameter?
+
+Why does intake `intake.open_esm_datastore` need the `columns_with_iterables` argument when we can achieve the same functionality with just `read_csv_kwargs`? Intake facilitates writing YAML descriptions of catalogs that can be opened with `intake.open_catalog`. These YAML descriptions include the information required to open the catalog: things like the catalog driver (`intake_esm.core.esm_datastore` in our case) and the arguments to pass to the driver to open the catalog. They can be included as entries in other catalogs enabling features like [catalog nesting](https://intake.readthedocs.io/en/latest/catalog.html#catalog-nesting). However, intake does not support Python function arguments like those we provided to `read_csv_kwargs` above so if we want a functional intake YAML description of an intake-esm catalog with multi-variable assets we need to use the `columns_with_iterables` argument instead. You can return an intake YAML description of an `esm_datastore` as follows:
+
+```{code-cell} ipython3
+cat.name = "my-esm-catalog"
+print(cat.yaml())
+```
+
 ```{code-cell} ipython3
 ---
 tags: [hide-input, hide-output]
 ---
 import intake_esm  # just to display version information
 intake_esm.show_versions()
 ```
```

### Comparing `intake-esm-2022.9.18/docs/source/index.md` & `intake-esm-2023.4.20/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `intake-esm-2022.9.18/docs/source/reference/api.md` & `intake-esm-2023.4.20/docs/source/reference/api.md`

 * *Files identical despite different names*

### Comparing `intake-esm-2022.9.18/docs/source/reference/cmip_ap.md` & `intake-esm-2023.4.20/docs/source/reference/cmip_ap.md`

 * *Files identical despite different names*

### Comparing `intake-esm-2022.9.18/docs/source/reference/esm-catalog-spec.md` & `intake-esm-2023.4.20/docs/source/reference/esm-catalog-spec.md`

 * *Files 0% similar despite different names*

```diff
@@ -81,19 +81,19 @@
 | column_name | string | **REQUIRED.** The name of the attribute column. Must be in the header of the CSV file. |
 | vocabulary  | string | Link to the controlled vocabulary for the attribute in the format of a URL.            |
 
 ### Assets Object
 
 An assets object describes the columns in the CSV file relevant for opening the actual data files.
 
-| Element            | Type   | Description                                                                                                                                                                                                  |
-| ------------------ | ------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
-| column_name        | string | **REQUIRED.** The name of the column containing the path to the asset. Must be in the header of the CSV file.                                                                                                |
-| format             | string | The data format. Valid values are `netcdf`, `zarr`, or `reference` ([`kerchunk`](https://github.com/fsspec/kerchunk) reference files). If specified, it means that all data in the catalog is the same type. |
-| format_column_name | string | The column name which contains the data format, allowing for variable data types in one catalog. Mutually exclusive with `format`.                                                                           |
+| Element            | Type   | Description                                                                                                                                                                                                            |
+| ------------------ | ------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| column_name        | string | **REQUIRED.** The name of the column containing the path to the asset. Must be in the header of the CSV file.                                                                                                          |
+| format             | string | The data format. Valid values are `netcdf`, `zarr`, `opendap` or `reference` ([`kerchunk`](https://github.com/fsspec/kerchunk) reference files). If specified, it means that all data in the catalog is the same type. |
+| format_column_name | string | The column name which contains the data format, allowing for variable data types in one catalog. Mutually exclusive with `format`.                                                                                     |
 
 ### Aggregation Control Object
 
 An aggregation control object defines neccessary information to use when aggregating multiple assets into a single xarray data set.
 
 | Element              | Type                                        | Description                                                                             |
 | -------------------- | ------------------------------------------- | --------------------------------------------------------------------------------------- |
```

### Comparing `intake-esm-2022.9.18/docs/source/reference/faq.md` & `intake-esm-2023.4.20/docs/source/reference/faq.md`

 * *Files identical despite different names*

### Comparing `intake-esm-2022.9.18/docs/source/tutorials/loading-cmip6-data.md` & `intake-esm-2023.4.20/docs/source/tutorials/loading-cmip6-data.md`

 * *Files identical despite different names*

### Comparing `intake-esm-2022.9.18/intake_esm/__init__.py` & `intake-esm-2023.4.20/intake_esm/__init__.py`

 * *Files identical despite different names*

### Comparing `intake-esm-2022.9.18/intake_esm/_search.py` & `intake-esm-2023.4.20/intake_esm/_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             value_ = value_.replace(fr'\{char}', '')
         return any(char in value_ for char in wildcard_chars)
     except (TypeError, AttributeError):
         return False
 
 
 def search(
-    *, df: pd.DataFrame, query: typing.Dict[str, typing.Any], columns_with_iterables: set
+    *, df: pd.DataFrame, query: dict[str, typing.Any], columns_with_iterables: set
 ) -> pd.DataFrame:
     """Search for entries in the catalog."""
 
     if not query:
         return pd.DataFrame(columns=df.columns)
     global_mask = np.ones(len(df), dtype=bool)
     for column, values in query.items():
@@ -55,16 +55,16 @@
     results = df.loc[global_mask]
     return results.reset_index(drop=True)
 
 
 def search_apply_require_all_on(
     *,
     df: pd.DataFrame,
-    query: typing.Dict[str, typing.Any],
-    require_all_on: typing.Union[str, typing.List[typing.Any]],
+    query: dict[str, typing.Any],
+    require_all_on: typing.Union[str, list[typing.Any]],
     columns_with_iterables: set = None,
 ) -> pd.DataFrame:
     _query = query.copy()
     # Make sure to remove columns that were already
     # specified in the query when specified in `require_all_on`. For example,
     # if query = dict(variable_id=["A", "B"], source_id=["FOO", "BAR"])
     # and require_all_on = ["source_id"], we need to make sure `source_id` key is
```

### Comparing `intake-esm-2022.9.18/intake_esm/cat.py` & `intake-esm-2023.4.20/intake_esm/cat.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         validate_assignment = True
 
 
 class DataFormat(str, enum.Enum):
     netcdf = 'netcdf'
     zarr = 'zarr'
     reference = 'reference'
+    opendap = 'opendap'
 
     class Config:
         validate_all = True
         validate_assignment = True
 
 
 class Attribute(pydantic.BaseModel):
@@ -82,42 +83,42 @@
             raise ValueError('Must set one of format or format_column_name')
         return values
 
 
 class Aggregation(pydantic.BaseModel):
     type: AggregationType
     attribute_name: pydantic.StrictStr
-    options: typing.Optional[typing.Dict] = {}
+    options: typing.Optional[dict] = {}
 
     class Config:
         validate_all = True
         validate_assignment = True
 
 
 class AggregationControl(pydantic.BaseModel):
     variable_column_name: pydantic.StrictStr
-    groupby_attrs: typing.List[pydantic.StrictStr]
-    aggregations: typing.List[Aggregation] = []
+    groupby_attrs: list[pydantic.StrictStr]
+    aggregations: list[Aggregation] = []
 
     class Config:
         validate_all = True
         validate_assignment = True
 
 
 class ESMCatalogModel(pydantic.BaseModel):
     """
     Pydantic model for the ESM data catalog defined in https://git.io/JBWoW
     """
 
     esmcat_version: pydantic.StrictStr
-    attributes: typing.List[Attribute]
+    attributes: list[Attribute]
     assets: Assets
-    aggregation_control: AggregationControl
+    aggregation_control: typing.Optional[AggregationControl] = None
     id: typing.Optional[str] = ''
-    catalog_dict: typing.Optional[typing.List[typing.Dict]] = None
+    catalog_dict: typing.Optional[list[dict]] = None
     catalog_file: pydantic.StrictStr = None
     description: pydantic.StrictStr = None
     title: pydantic.StrictStr = None
     last_updated: typing.Optional[typing.Union[datetime.datetime, datetime.date]] = None
     _df: typing.Optional[pd.DataFrame] = pydantic.PrivateAttr()
 
     class Config:
@@ -131,15 +132,15 @@
         catalog_dict, catalog_file = values.get('catalog_dict'), values.get('catalog_file')
         if catalog_dict is not None and catalog_file is not None:
             raise ValueError('catalog_dict and catalog_file cannot be set at the same time')
 
         return values
 
     @classmethod
-    def from_dict(cls, data: typing.Dict) -> 'ESMCatalogModel':
+    def from_dict(cls, data: dict) -> 'ESMCatalogModel':
         esmcat = data['esmcat']
         df = data['df']
         if 'last_updated' not in esmcat:
             esmcat['last_updated'] = None
         cat = cls.parse_obj(esmcat)
         cat._df = df
         return cat
@@ -148,15 +149,15 @@
         self,
         name: str,
         *,
         directory: str = None,
         catalog_type: str = 'dict',
         to_csv_kwargs: dict = None,
         json_dump_kwargs: dict = None,
-        storage_options: typing.Dict[str, typing.Any] = None,
+        storage_options: dict[str, typing.Any] = None,
     ) -> None:
         """
         Save the catalog to a file.
 
         Parameters
         -----------
         name: str
@@ -223,16 +224,16 @@
 
         print(f'Successfully wrote ESM catalog json file to: {json_file_name}')
 
     @classmethod
     def load(
         cls,
         json_file: typing.Union[str, pydantic.FilePath, pydantic.AnyUrl],
-        storage_options: typing.Dict[str, typing.Any] = None,
-        read_csv_kwargs: typing.Dict[str, typing.Any] = None,
+        storage_options: dict[str, typing.Any] = None,
+        read_csv_kwargs: dict[str, typing.Any] = None,
     ) -> 'ESMCatalogModel':
         """
         Loads the catalog from a file
 
         Parameters
         -----------
         json_file: str or pathlib.Path
@@ -242,14 +243,15 @@
             Amazon Web Service S3.
         read_csv_kwargs: dict
             Additional keyword arguments passed through to the :py:func:`~pandas.read_csv` function.
 
         """
         storage_options = storage_options if storage_options is not None else {}
         read_csv_kwargs = read_csv_kwargs or {}
+        json_file = str(json_file)  # We accept Path, but fsspec doesn't.
         _mapper = fsspec.get_mapper(json_file, **storage_options)
 
         with fsspec.open(json_file, **storage_options) as fobj:
             data = json.loads(fobj.read())
             if 'last_updated' not in data:
                 data['last_updated'] = None
             cat = cls.parse_obj(data)
@@ -268,15 +270,15 @@
                 df = pd.DataFrame(cat.catalog_dict)
 
             cat._df = df
             cat._cast_agg_columns_with_iterables()
             return cat
 
     @property
-    def columns_with_iterables(self) -> typing.Set[str]:
+    def columns_with_iterables(self) -> set[str]:
         """Return a set of columns that have iterables."""
         if self._df.empty:
             return set()
         has_iterables = (
             self._df.sample(20, replace=True)
             .applymap(type)
             .isin([list, tuple, set])
@@ -305,32 +307,29 @@
             )
         )
         if columns:
             self._df[columns] = self._df[columns].apply(tuple)
 
     @property
     def grouped(self) -> typing.Union[pd.core.groupby.DataFrameGroupBy, pd.DataFrame]:
-
         if self.aggregation_control.groupby_attrs:
             self.aggregation_control.groupby_attrs = list(
                 filter(
                     functools.partial(_allnan_or_nonan, self.df),
                     self.aggregation_control.groupby_attrs,
                 )
             )
 
         if self.aggregation_control.groupby_attrs and set(
             self.aggregation_control.groupby_attrs
         ) != set(self.df.columns):
             return self.df.groupby(self.aggregation_control.groupby_attrs)
         return self.df
 
-    def _construct_group_keys(
-        self, sep: str = '.'
-    ) -> typing.Dict[str, typing.Union[str, typing.Tuple[str]]]:
+    def _construct_group_keys(self, sep: str = '.') -> dict[str, typing.Union[str, tuple[str]]]:
         grouped = self.grouped
         if isinstance(grouped, pd.core.groupby.generic.DataFrameGroupBy):
             internal_keys = grouped.groups.keys()
             public_keys = map(
                 lambda key: key if isinstance(key, str) else sep.join(str(value) for value in key),
                 internal_keys,
             )
@@ -341,15 +340,15 @@
                 grouped[grouped.columns.tolist()]
                 .apply(lambda row: sep.join(str(v) for v in row), axis=1)
                 .tolist()
             )
 
         return dict(zip(public_keys, internal_keys))
 
-    def _unique(self) -> typing.Dict:
+    def _unique(self) -> dict:
         def _find_unique(series):
             values = series.dropna()
             if series.name in self.columns_with_iterables:
                 values = tlz.concat(values)
             return list(tlz.unique(values))
 
         data = self.df[self.df.columns]
@@ -365,16 +364,16 @@
     def nunique(self) -> pd.Series:
         """Return a series of the number of unique values for each column in the catalog."""
         return pd.Series(tlz.valmap(len, self._unique()))
 
     def search(
         self,
         *,
-        query: typing.Union['QueryModel', typing.Dict[str, typing.Any]],
-        require_all_on: typing.Union[str, typing.List[str]] = None,
+        query: typing.Union['QueryModel', dict[str, typing.Any]],
+        require_all_on: typing.Union[str, list[str]] = None,
     ) -> 'ESMCatalogModel':
         """
         Search for entries in the catalog.
 
         Parameters
         ----------
         query: dict, optional
@@ -412,17 +411,17 @@
             )
         return results
 
 
 class QueryModel(pydantic.BaseModel):
     """A Pydantic model to represent a query to be executed against a catalog."""
 
-    query: typing.Dict[pydantic.StrictStr, typing.Union[typing.Any, typing.List[typing.Any]]]
-    columns: typing.List[str]
-    require_all_on: typing.Union[str, typing.List[typing.Any]] = None
+    query: dict[pydantic.StrictStr, typing.Union[typing.Any, list[typing.Any]]]
+    columns: list[str]
+    require_all_on: typing.Union[str, list[typing.Any]] = None
 
     class Config:
         validate_all = True
         validate_assignment = True
 
     @pydantic.root_validator(pre=False)
     def validate_query(cls, values):
```

### Comparing `intake-esm-2022.9.18/intake_esm/core.py` & `intake-esm-2023.4.20/intake_esm/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import ast
 import concurrent.futures
 import typing
 import warnings
 from copy import deepcopy
 
 import dask
 
@@ -38,14 +39,18 @@
         be a Pandas DataFrame containing content that would otherwise be in a CSV file.
     sep : str, optional
         Delimiter to use when constructing a key for a query, by default '.'
     registry : DerivedVariableRegistry, optional
         Registry of derived variables to use, by default None. If not provided, uses the default registry.
     read_csv_kwargs : dict, optional
         Additional keyword arguments passed through to the :py:func:`~pandas.read_csv` function.
+    columns_with_iterables : list of str, optional
+        A list of columns in the csv file containing iterables. Values in columns specified here will be
+        converted with `ast.literal_eval` when :py:func:`~pandas.read_csv` is called (i.e., this is a
+        shortcut to passing converters to `read_csv_kwargs`).
     storage_options : dict, optional
         Parameters passed to the backend file-system such as Google Cloud Storage,
         Amazon Web Service S3.
     intake_kwargs: dict, optional
         Additional keyword arguments are passed through to the :py:class:`~intake.catalog.Catalog` base class.
 
     Examples
@@ -67,29 +72,37 @@
     """
 
     name = 'esm_datastore'
     container = 'xarray'
 
     def __init__(
         self,
-        obj: typing.Union[pydantic.FilePath, pydantic.AnyUrl, typing.Dict[str, typing.Any]],
+        obj: typing.Union[pydantic.FilePath, pydantic.AnyUrl, dict[str, typing.Any]],
         *,
         progressbar: bool = True,
         sep: str = '.',
         registry: typing.Optional[DerivedVariableRegistry] = None,
-        read_csv_kwargs: typing.Dict[str, typing.Any] = None,
-        storage_options: typing.Dict[str, typing.Any] = None,
-        intake_kwargs: typing.Dict[str, typing.Any] = None,
+        read_csv_kwargs: dict[str, typing.Any] = None,
+        columns_with_iterables: list[str] = None,
+        storage_options: dict[str, typing.Any] = None,
+        **intake_kwargs: dict[str, typing.Any],
     ):
-
         """Intake Catalog representing an ESM Collection."""
-        intake_kwargs = intake_kwargs or {}
         super().__init__(**intake_kwargs)
         self.storage_options = storage_options or {}
-        self.read_csv_kwargs = read_csv_kwargs or {}
+        read_csv_kwargs = read_csv_kwargs or {}
+        if columns_with_iterables:
+            converter = ast.literal_eval
+            read_csv_kwargs.setdefault('converters', {})
+            for col in columns_with_iterables:
+                if read_csv_kwargs['converters'].setdefault(col, converter) != converter:
+                    raise ValueError(
+                        f"Cannot provide converter for '{col}' via `read_csv_kwargs` when '{col}' is also specified in `columns_with_iterables`"
+                    )
+        self.read_csv_kwargs = read_csv_kwargs
         self.progressbar = progressbar
         self.sep = sep
         if isinstance(obj, dict):
             self.esmcat = ESMCatalogModel.from_dict(obj)
         else:
             self.esmcat = ESMCatalogModel.load(
                 obj, storage_options=self.storage_options, read_csv_kwargs=read_csv_kwargs
@@ -110,15 +123,15 @@
 
             for col in entry.query:
                 if col not in self.esmcat.df.columns:
                     raise ValueError(
                         f'Derived variable {key} depends on unknown column {col} in query: {entry.query}. Valid ESM catalog columns: {self.esmcat.df.columns.tolist()}.'
                     )
 
-    def keys(self) -> typing.List[str]:
+    def keys(self) -> list[str]:
         """
         Get keys for the catalog entries
 
         Returns
         -------
         list
             keys for the catalog entries
@@ -179,15 +192,15 @@
         Return pandas :py:class:`~pandas.DataFrame`.
         """
         return self.esmcat.df
 
     def __len__(self) -> int:
         return len(self.keys())
 
-    def _get_entries(self) -> typing.Dict[str, ESMDataSource]:
+    def _get_entries(self) -> dict[str, ESMDataSource]:
         # Due to just-in-time entry creation, we may not have all entries loaded
         # We need to make sure to create entries missing from self._entries
         missing = set(self.keys()) - set(self._entries.keys())
         for key in missing:
             _ = self[key]
         return self._entries
 
@@ -280,15 +293,15 @@
         Display the entry as a rich object in an IPython session
         """
         from IPython.display import HTML, display
 
         contents = self._repr_html_()
         display(HTML(contents))
 
-    def __dir__(self) -> typing.List[str]:
+    def __dir__(self) -> list[str]:
         rv = [
             'df',
             'to_dataset_dict',
             'to_datatree',
             'to_dask',
             'keys',
             'keys_info',
@@ -301,17 +314,15 @@
         ]
         return sorted(list(self.__dict__.keys()) + rv)
 
     def _ipython_key_completions_(self):
         return self.__dir__()
 
     @pydantic.validate_arguments
-    def search(
-        self, require_all_on: typing.Union[str, typing.List[str]] = None, **query: typing.Any
-    ):
+    def search(self, require_all_on: typing.Union[str, list[str]] = None, **query: typing.Any):
         """Search for entries in the catalog.
 
         Parameters
         ----------
         require_all_on : list, str, optional
             A dataframe column or a list of dataframe columns across
             which all entries must satisfy the query criteria.
@@ -416,17 +427,17 @@
 
     @pydantic.validate_arguments
     def serialize(
         self,
         name: pydantic.StrictStr,
         directory: typing.Union[pydantic.DirectoryPath, pydantic.StrictStr] = None,
         catalog_type: str = 'dict',
-        to_csv_kwargs: typing.Dict[typing.Any, typing.Any] = None,
-        json_dump_kwargs: typing.Dict[typing.Any, typing.Any] = None,
-        storage_options: typing.Dict[str, typing.Any] = None,
+        to_csv_kwargs: dict[typing.Any, typing.Any] = None,
+        json_dump_kwargs: dict[typing.Any, typing.Any] = None,
+        storage_options: dict[str, typing.Any] = None,
     ) -> None:
         """Serialize catalog to corresponding json and csv files.
 
         Parameters
         ----------
         name : str
             name to use when creating ESM catalog json file and csv catalog.
@@ -505,23 +516,23 @@
             self.derivedcat.keys()
         )
         return unique
 
     @pydantic.validate_arguments
     def to_dataset_dict(
         self,
-        xarray_open_kwargs: typing.Dict[str, typing.Any] = None,
-        xarray_combine_by_coords_kwargs: typing.Dict[str, typing.Any] = None,
+        xarray_open_kwargs: dict[str, typing.Any] = None,
+        xarray_combine_by_coords_kwargs: dict[str, typing.Any] = None,
         preprocess: typing.Callable = None,
-        storage_options: typing.Dict[pydantic.StrictStr, typing.Any] = None,
+        storage_options: dict[pydantic.StrictStr, typing.Any] = None,
         progressbar: pydantic.StrictBool = None,
         aggregate: pydantic.StrictBool = None,
         skip_on_error: pydantic.StrictBool = False,
         **kwargs,
-    ) -> typing.Dict[str, xr.Dataset]:
+    ) -> dict[str, xr.Dataset]:
         """
         Load catalog entries into a dictionary of xarray datasets.
 
         Column values, dataset keys and requested variables are added as global
         attributes on the returned datasets. The names of these attributes can be
         customized with :py:class:`intake_esm.utils.set_options`.
 
@@ -651,18 +662,18 @@
                         raise exc
         self.datasets = self._create_derived_variables(datasets, skip_on_error)
         return self.datasets
 
     @pydantic.validate_arguments
     def to_datatree(
         self,
-        xarray_open_kwargs: typing.Dict[str, typing.Any] = None,
-        xarray_combine_by_coords_kwargs: typing.Dict[str, typing.Any] = None,
+        xarray_open_kwargs: dict[str, typing.Any] = None,
+        xarray_combine_by_coords_kwargs: dict[str, typing.Any] = None,
         preprocess: typing.Callable = None,
-        storage_options: typing.Dict[pydantic.StrictStr, typing.Any] = None,
+        storage_options: dict[pydantic.StrictStr, typing.Any] = None,
         progressbar: pydantic.StrictBool = None,
         aggregate: pydantic.StrictBool = None,
         skip_on_error: pydantic.StrictBool = False,
         **kwargs,
     ):
         """
         Load catalog entries into a tree of xarray datasets.
```

### Comparing `intake-esm-2022.9.18/intake_esm/derived.py` & `intake-esm-2023.4.20/intake_esm/derived.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 class DerivedVariableError(Exception):
     pass
 
 
 class DerivedVariable(pydantic.BaseModel):
     func: typing.Callable
     variable: pydantic.StrictStr
-    query: typing.Dict[pydantic.StrictStr, typing.Union[typing.Any, typing.List[typing.Any]]]
+    query: dict[pydantic.StrictStr, typing.Union[typing.Any, list[typing.Any]]]
     prefer_derived: bool
 
     @pydantic.validator('query')
     def validate_query(cls, values):
         _query = values.copy()
         for key, value in _query.items():
             if isinstance(value, (str, int, float, bool)):
                 _query[key] = [value]
         return _query
 
-    def dependent_variables(self, variable_key_name: str) -> typing.List[pydantic.StrictStr]:
+    def dependent_variables(self, variable_key_name: str) -> list[pydantic.StrictStr]:
         """Return a list of dependent variables for a given variable"""
         return self.query[variable_key_name]
 
     def __call__(self, *args, variable_key_name: str = None, **kwargs) -> xr.Dataset:
         """Call the function and return the result"""
         try:
             return self.func(*args, **kwargs)
@@ -88,15 +88,15 @@
 
     @tlz.curry
     def register(
         self,
         func: typing.Callable,
         *,
         variable: str,
-        query: typing.Dict[pydantic.StrictStr, typing.Union[typing.Any, typing.List[typing.Any]]],
+        query: dict[pydantic.StrictStr, typing.Union[typing.Any, list[typing.Any]]],
         prefer_derived: bool = False,
     ) -> typing.Callable:
         """Register a derived variable
 
         Parameters
         ----------
         func : typing.Callable
@@ -130,24 +130,24 @@
 
     def __repr__(self) -> str:
         return f'DerivedVariableRegistry({self._registry})'
 
     def __len__(self) -> int:
         return len(self._registry)
 
-    def items(self) -> typing.List[typing.Tuple[str, DerivedVariable]]:
+    def items(self) -> list[tuple[str, DerivedVariable]]:
         return list(self._registry.items())
 
-    def keys(self) -> typing.List[str]:
+    def keys(self) -> list[str]:
         return list(self._registry.keys())
 
-    def values(self) -> typing.List[DerivedVariable]:
+    def values(self) -> list[DerivedVariable]:
         return list(self._registry.values())
 
-    def search(self, variable: typing.Union[str, typing.List[str]]) -> 'DerivedVariableRegistry':
+    def search(self, variable: typing.Union[str, list[str]]) -> 'DerivedVariableRegistry':
         """Search for a derived variable by name or list of names
 
         Parameters
         ----------
         variable : typing.Union[str, typing.List[str]]
             The name of the variable to search for.
 
@@ -162,18 +162,18 @@
         reg = DerivedVariableRegistry()
         reg._registry = results
         return reg
 
     def update_datasets(
         self,
         *,
-        datasets: typing.Dict[str, xr.Dataset],
+        datasets: dict[str, xr.Dataset],
         variable_key_name: str,
         skip_on_error: bool = False,
-    ) -> typing.Dict[str, xr.Dataset]:
+    ) -> dict[str, xr.Dataset]:
         """Given a dictionary of datasets, return a dictionary of datasets with the derived variables
 
         Parameters
         ----------
         datasets : typing.Dict[str, xr.Dataset]
             A dictionary of datasets to apply the derived variables to.
         variable_key_name : str
```

### Comparing `intake-esm-2022.9.18/intake_esm/source.py` & `intake-esm-2023.4.20/intake_esm/source.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,31 +44,30 @@
     xarray_open_kwargs=None,
     preprocess=None,
     requested_variables=None,
     additional_attrs=None,
     expand_dims=None,
     data_format=None,
 ):
-
     storage_options = xarray_open_kwargs.get('backend_kwargs', {}).get('storage_options', {})
     # Support kerchunk datasets, setting the file object (fo) and urlpath
     if data_format == 'reference':
         xarray_open_kwargs['backend_kwargs']['storage_options']['fo'] = urlpath
         xarray_open_kwargs['backend_kwargs']['consolidated'] = False
         urlpath = 'reference://'
 
-    if xarray_open_kwargs['engine'] == 'zarr':
+    if xarray_open_kwargs['engine'] in 'zarr' or data_format == 'opendap':
         url = urlpath
     elif fsspec.utils.can_be_local(urlpath):
         url = fsspec.open_local(urlpath, **storage_options)
     else:
         url = fsspec.open(urlpath, **storage_options).open()
 
     # Handle multi-file datasets with `xr.open_mfdataset()`
-    if '*' in url or isinstance(url, list):
+    if (isinstance(url, str) and '*' in url) or isinstance(url, list):
         # How should we handle concat_dim, and other xr.open_mfdataset kwargs?
         xarray_open_kwargs.update(preprocess=preprocess)
         xarray_open_kwargs.update(parallel=True)
         ds = xr.open_mfdataset(url, **xarray_open_kwargs)
     else:
         ds = xr.open_dataset(url, **xarray_open_kwargs)
         if preprocess is not None:
@@ -121,27 +120,27 @@
     name = 'esm_datasource'
     partition_access = True
 
     @pydantic.validate_arguments
     def __init__(
         self,
         key: pydantic.StrictStr,
-        records: typing.List[typing.Dict[str, typing.Any]],
+        records: list[dict[str, typing.Any]],
         variable_column_name: pydantic.StrictStr,
         path_column_name: pydantic.StrictStr,
         data_format: typing.Optional[DataFormat],
         format_column_name: typing.Optional[pydantic.StrictStr],
         *,
-        aggregations: typing.Optional[typing.List[Aggregation]] = None,
-        requested_variables: typing.List[str] = None,
+        aggregations: typing.Optional[list[Aggregation]] = None,
+        requested_variables: list[str] = None,
         preprocess: typing.Callable = None,
-        storage_options: typing.Dict[str, typing.Any] = None,
-        xarray_open_kwargs: typing.Dict[str, typing.Any] = None,
-        xarray_combine_by_coords_kwargs: typing.Dict[str, typing.Any] = None,
-        intake_kwargs: typing.Dict[str, typing.Any] = None,
+        storage_options: dict[str, typing.Any] = None,
+        xarray_open_kwargs: dict[str, typing.Any] = None,
+        xarray_combine_by_coords_kwargs: dict[str, typing.Any] = None,
+        intake_kwargs: dict[str, typing.Any] = None,
     ):
         """An intake compatible Data Source for ESM data.
 
         Parameters
         ----------
         key: str
             The key of the data source.
@@ -196,15 +195,14 @@
         else:
             self.df = self.df.rename(columns={format_column_name: '_data_format_'})
 
     def __repr__(self) -> str:
         return f'<{type(self).__name__}  (name: {self.key}, asset(s): {len(self.df)})>'
 
     def _get_schema(self) -> Schema:
-
         if self._ds is None:
             self._open_dataset()
             metadata = {'dims': {}, 'data_vars': {}, 'coords': ()}
             self._schema = Schema(
                 datashape=None,
                 dtype=None,
                 shape=None,
```

### Comparing `intake-esm-2022.9.18/intake_esm/tutorial.py` & `intake-esm-2023.4.20/intake_esm/tutorial.py`

 * *Files identical despite different names*

### Comparing `intake-esm-2022.9.18/intake_esm/utils.py` & `intake-esm-2023.4.20/intake_esm/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         ('zarr', lambda mod: mod.__version__),
         ('cftime', lambda mod: mod.__version__),
         ('netCDF4', lambda mod: mod.__version__),
         ('requests', lambda mod: mod.__version__),
     ]
 
     deps_blob = []
-    for (modname, ver_f) in deps:
+    for modname, ver_f in deps:
         try:
             if modname in sys.modules:
                 mod = sys.modules[modname]
             else:
                 mod = importlib.import_module(modname)
         except Exception:
             deps_blob.append((modname, None))
```

### Comparing `intake-esm-2022.9.18/intake_esm.egg-info/PKG-INFO` & `intake-esm-2023.4.20/intake_esm.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intake-esm
-Version: 2022.9.18
+Version: 2023.4.20
 Summary: An intake plugin for parsing an Earth System Model (ESM) catalog and loading netCDF files and/or Zarr stores into Xarray datasets.
 Home-page: https://intake-esm.readthedocs.io
 Maintainer: NCAR XDev Team
 Maintainer-email: xdev@ucar.edu
 License: Apache 2.0
 Project-URL: Documentation, https://intake-esm.readthedocs.io
 Project-URL: Source, https://github.com/intake/intake-esm
@@ -12,19 +12,19 @@
 Keywords: intake,xarray,catalog
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Intake-esm
 
 - [Intake-esm](#intake-esm)
   - [Badges](#badges)
@@ -116,19 +116,19 @@
 
 It is also available from `conda-forge` for conda installations:
 
 ```bash
 conda install -c conda-forge intake-esm
 ```
 
-[github-ci-badge]: https://img.shields.io/github/workflow/status/intake/intake-esm/CI?label=CI&logo=github
-[github-ci-link]: https://github.com/intake/intake-esm/actions?query=workflow%3ACI
+[github-ci-badge]: https://github.com/intake/intake-esm/actions/workflows/ci.yaml/badge.svg
+[github-ci-link]: https://github.com/intake/intake-esm/actions/workflows/ci.yaml
 [codecov-badge]: https://img.shields.io/codecov/c/github/intake/intake-esm.svg?logo=codecov
 [codecov-link]: https://codecov.io/gh/intake/intake-esm
-[rtd-badge]: https://img.shields.io/readthedocs/intake-esm/latest.svg
+[rtd-badge]: https://readthedocs.org/projects/intake-esm/badge/?version=latest
 [rtd-link]: https://intake-esm.readthedocs.io/en/latest/?badge=latest
 [pypi-badge]: https://img.shields.io/pypi/v/intake-esm?logo=pypi
 [pypi-link]: https://pypi.org/project/intake-esm
 [conda-badge]: https://img.shields.io/conda/vn/conda-forge/intake-esm?logo=anaconda
 [conda-link]: https://anaconda.org/conda-forge/intake-esm
 [zenodo-badge]: https://img.shields.io/badge/DOI-10.5281%20%2F%20zenodo.3491062-blue.svg
 [zenodo-link]: https://doi.org/10.5281/zenodo.3491062
```

### Comparing `intake-esm-2022.9.18/intake_esm.egg-info/SOURCES.txt` & `intake-esm-2023.4.20/intake_esm.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 MANIFEST.in
 Makefile
 README.md
 codecov.yml
 pyproject.toml
 readthedocs.yml
 requirements.txt
-setup.cfg
 setup.py
 .github/CODEOWNERS
 .github/dependabot.yml
 .github/pull_request_template.md
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/workflows/ci.yaml
```

### Comparing `intake-esm-2022.9.18/setup.py` & `intake-esm-2023.4.20/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,26 +20,26 @@
 CLASSIFIERS = [
     'Development Status :: 4 - Beta',
     'License :: OSI Approved :: Apache Software License',
     'Operating System :: OS Independent',
     'Intended Audience :: Science/Research',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Topic :: Scientific/Engineering',
 ]
 
 setup(
     name='intake-esm',
     description='An intake plugin for parsing an Earth System Model (ESM) catalog and loading netCDF files and/or Zarr stores into Xarray datasets.',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    python_requires='>=3.8',
+    python_requires='>=3.9',
     maintainer='NCAR XDev Team',
     maintainer_email='xdev@ucar.edu',
     classifiers=CLASSIFIERS,
     url='https://intake-esm.readthedocs.io',
     project_urls={
         'Documentation': 'https://intake-esm.readthedocs.io',
         'Source': 'https://github.com/intake/intake-esm',
```

### Comparing `intake-esm-2022.9.18/tutorial-catalogs/AWS-CESM2-LENS.json` & `intake-esm-2023.4.20/tutorial-catalogs/AWS-CESM2-LENS.json`

 * *Files identical despite different names*

### Comparing `intake-esm-2022.9.18/tutorial-catalogs/AWS-CMIP6.json` & `intake-esm-2023.4.20/tutorial-catalogs/AWS-CMIP6.json`

 * *Files identical despite different names*

### Comparing `intake-esm-2022.9.18/tutorial-catalogs/GOOGLE-CMIP6.json` & `intake-esm-2023.4.20/tutorial-catalogs/GOOGLE-CMIP6.json`

 * *Files identical despite different names*

