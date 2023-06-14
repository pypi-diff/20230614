# Comparing `tmp/module-utilities-0.3.1.tar.gz` & `tmp/module-utilities-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "module-utilities-0.3.1.tar", last modified: Thu May  4 19:05:27 2023, max compression
+gzip compressed data, was "module-utilities-0.4.0.tar", last modified: Wed Jun 14 21:22:11 2023, max compression
```

## Comparing `module-utilities-0.3.1.tar` & `module-utilities-0.4.0.tar`

### file list

```diff
@@ -1,123 +1,122 @@
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.786108 module-utilities-0.3.1/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1369 2023-05-04 19:04:22.000000 module-utilities-0.3.1/.cruft.json
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      540 2023-05-02 03:09:02.000000 module-utilities-0.3.1/.editorconfig
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.729675 module-utilities-0.3.1/.github/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      368 2023-05-02 03:09:02.000000 module-utilities-0.3.1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1307 2023-05-02 03:09:02.000000 module-utilities-0.3.1/.gitignore
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      161 2023-04-27 23:45:36.000000 module-utilities-0.3.1/.markdownlint.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3581 2023-04-27 23:45:36.000000 module-utilities-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       20 2023-04-27 23:45:36.000000 module-utilities-0.3.1/.prettierrc.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      527 2023-05-04 19:04:22.000000 module-utilities-0.3.1/.recipe-append.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      122 2023-04-27 23:45:36.000000 module-utilities-0.3.1/AUTHORS.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      495 2023-05-03 20:28:18.000000 module-utilities-0.3.1/CHANGELOG.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9752 2023-05-04 19:04:22.000000 module-utilities-0.3.1/CONTRIBUTING.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1645 2023-04-27 23:45:36.000000 module-utilities-0.3.1/LICENSE
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      258 2023-04-27 23:45:36.000000 module-utilities-0.3.1/MANIFEST.in
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    11367 2023-05-03 02:36:13.000000 module-utilities-0.3.1/Makefile
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5998 2023-05-04 19:05:27.785460 module-utilities-0.3.1/PKG-INFO
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2844 2023-05-03 02:36:13.000000 module-utilities-0.3.1/README.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.730570 module-utilities-0.3.1/changelog.d/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       64 2023-04-27 23:45:36.000000 module-utilities-0.3.1/changelog.d/README.txt
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.731454 module-utilities-0.3.1/changelog.d/templates/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.733002 module-utilities-0.3.1/changelog.d/templates/auto-changelog/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      213 2023-04-27 23:45:36.000000 module-utilities-0.3.1/changelog.d/templates/auto-changelog/macros.jinja2
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      774 2023-04-27 23:45:36.000000 module-utilities-0.3.1/changelog.d/templates/auto-changelog/template.jinja2
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      269 2023-04-27 23:45:36.000000 module-utilities-0.3.1/changelog.d/templates/new_fragment.md.j2
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      204 2023-04-27 23:45:36.000000 module-utilities-0.3.1/conftest.py
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.742537 module-utilities-0.3.1/docs/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1401 2023-05-03 02:36:13.000000 module-utilities-0.3.1/docs/Makefile
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.711377 module-utilities-0.3.1/docs/_static/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.743007 module-utilities-0.3.1/docs/_static/css/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2937 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/_static/css/nist-combined.css
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.744198 module-utilities-0.3.1/docs/_static/js/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      767 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/_static/js/leave_notice.js
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      706 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/_static/js/nist-header-footer.js
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.748213 module-utilities-0.3.1/docs/_templates/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.750821 module-utilities-0.3.1/docs/_templates/autodocsumm/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      289 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/_templates/autodocsumm/class-noindex.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      249 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/_templates/autodocsumm/class.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      405 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/_templates/autodocsumm/module-inherit.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      424 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/_templates/autodocsumm/module-noindex.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      374 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/_templates/autodocsumm/module.rst
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.752387 module-utilities-0.3.1/docs/_templates/autosummary/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      106 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/_templates/autosummary/base.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1255 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/_templates/autosummary/class.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1119 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/_templates/autosummary/module.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1418 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/_templates/class-individual-pages.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1255 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/_templates/class-single-page.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1186 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/_templates/custom-module-template.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1212 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/_templates/module-custom-imported.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1177 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/_templates/module-custom.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1071 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/_templates/module-single.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1179 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/_templates/module-template.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       69 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/authors.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       71 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/changelog.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    14851 2023-05-03 20:28:18.000000 module-utilities-0.3.1/docs/conf.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       74 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/contributing.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.754264 module-utilities-0.3.1/docs/examples/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1675 2023-05-03 02:36:13.000000 module-utilities-0.3.1/docs/examples/example-usage-1.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1667 2023-05-03 02:36:13.000000 module-utilities-0.3.1/docs/examples/example-usage.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       89 2023-05-03 02:36:13.000000 module-utilities-0.3.1/docs/examples/index.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.755312 module-utilities-0.3.1/docs/examples/usage/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    13498 2023-05-03 02:36:13.000000 module-utilities-0.3.1/docs/examples/usage/cached.ipynb
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    18227 2023-05-03 20:28:18.000000 module-utilities-0.3.1/docs/examples/usage/docfiller.ipynb
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      224 2023-05-03 20:28:18.000000 module-utilities-0.3.1/docs/index.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      937 2023-05-03 02:36:13.000000 module-utilities-0.3.1/docs/installation.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       40 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/license.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      767 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/make.bat
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      169 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/navigation.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.756420 module-utilities-0.3.1/docs/reference/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      192 2023-05-03 02:36:13.000000 module-utilities-0.3.1/docs/reference/index.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 23:45:36.000000 module-utilities-0.3.1/docs/spelling_wordlist.txt
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.763826 module-utilities-0.3.1/environment/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      943 2023-04-27 23:45:36.000000 module-utilities-0.3.1/environment/dev-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      232 2023-05-02 03:09:02.000000 module-utilities-0.3.1/environment/dev.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      108 2023-04-27 23:45:36.000000 module-utilities-0.3.1/environment/dist-conda.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       79 2023-04-27 23:45:36.000000 module-utilities-0.3.1/environment/dist-pypi.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      574 2023-04-27 23:45:36.000000 module-utilities-0.3.1/environment/docs-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      349 2023-05-02 03:09:02.000000 module-utilities-0.3.1/environment/docs.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       64 2023-05-02 03:09:02.000000 module-utilities-0.3.1/environment/lint-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      136 2023-05-02 03:09:02.000000 module-utilities-0.3.1/environment/lint.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       25 2023-04-27 23:45:36.000000 module-utilities-0.3.1/environment/test-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      116 2023-05-02 03:09:02.000000 module-utilities-0.3.1/environment/test.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      299 2023-04-27 23:45:36.000000 module-utilities-0.3.1/environment/tools.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      113 2023-05-02 03:09:02.000000 module-utilities-0.3.1/environment.yaml
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.764729 module-utilities-0.3.1/examples/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      222 2023-04-27 23:45:36.000000 module-utilities-0.3.1/examples/README.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.766352 module-utilities-0.3.1/examples/usage/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    13498 2023-05-03 02:36:13.000000 module-utilities-0.3.1/examples/usage/cached.ipynb
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    18227 2023-05-03 20:28:18.000000 module-utilities-0.3.1/examples/usage/docfiller.ipynb
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     6147 2023-05-04 19:04:22.000000 module-utilities-0.3.1/pyproject.toml
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.772182 module-utilities-0.3.1/scripts/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      847 2023-05-04 19:04:22.000000 module-utilities-0.3.1/scripts/dist-conda.mk
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      312 2023-05-02 03:09:02.000000 module-utilities-0.3.1/scripts/dist-pypi.mk
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1099 2023-04-27 23:45:36.000000 module-utilities-0.3.1/scripts/docs-examples-symlinks.sh
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      266 2023-05-02 03:09:02.000000 module-utilities-0.3.1/scripts/lint.mk
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      598 2023-05-04 19:04:22.000000 module-utilities-0.3.1/scripts/recipe-append.sh
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       91 2023-05-02 03:09:02.000000 module-utilities-0.3.1/scripts/run-prettier.sh
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      489 2023-04-27 23:45:36.000000 module-utilities-0.3.1/scripts/tox-ipykernel-display-name.sh
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       38 2023-05-04 19:05:27.786317 module-utilities-0.3.1/setup.cfg
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.715616 module-utilities-0.3.1/src/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.778045 module-utilities-0.3.1/src/module_utilities/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      683 2023-05-02 03:09:02.000000 module-utilities-0.3.1/src/module_utilities/__init__.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2646 2023-05-02 03:09:02.000000 module-utilities-0.3.1/src/module_utilities/_doc.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    23552 2023-05-02 03:09:02.000000 module-utilities-0.3.1/src/module_utilities/_docscrape.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      382 2023-05-02 03:09:02.000000 module-utilities-0.3.1/src/module_utilities/_typing.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5930 2023-05-03 20:28:18.000000 module-utilities-0.3.1/src/module_utilities/attributedict.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9991 2023-05-03 20:28:18.000000 module-utilities-0.3.1/src/module_utilities/cached.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    20974 2023-05-03 20:28:18.000000 module-utilities-0.3.1/src/module_utilities/docfiller.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-02 03:09:02.000000 module-utilities-0.3.1/src/module_utilities/py.typed
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.782030 module-utilities-0.3.1/src/module_utilities.egg-info/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5998 2023-05-04 19:05:27.000000 module-utilities-0.3.1/src/module_utilities.egg-info/PKG-INFO
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2692 2023-05-04 19:05:27.000000 module-utilities-0.3.1/src/module_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-05-04 19:05:27.000000 module-utilities-0.3.1/src/module_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       48 2023-05-04 19:05:27.000000 module-utilities-0.3.1/src/module_utilities.egg-info/requires.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       17 2023-05-04 19:05:27.000000 module-utilities-0.3.1/src/module_utilities.egg-info/top_level.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-05-04 19:05:27.000000 module-utilities-0.3.1/src/module_utilities.egg-info/zip-safe
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:05:27.784679 module-utilities-0.3.1/tests/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       46 2023-04-27 23:45:36.000000 module-utilities-0.3.1/tests/__init__.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 23:45:36.000000 module-utilities-0.3.1/tests/conftest.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    10864 2023-05-02 03:09:02.000000 module-utilities-0.3.1/tests/test_cached.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     8959 2023-05-03 20:28:18.000000 module-utilities-0.3.1/tests/test_docfiller.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      169 2023-05-02 03:09:02.000000 module-utilities-0.3.1/tests/test_module_utilities.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4186 2023-05-04 19:04:22.000000 module-utilities-0.3.1/tox.ini
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.774150 module-utilities-0.4.0/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1367 2023-06-14 21:18:50.000000 module-utilities-0.4.0/.cruft.json
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      540 2023-05-02 03:09:02.000000 module-utilities-0.4.0/.editorconfig
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.733679 module-utilities-0.4.0/.github/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      368 2023-05-02 03:09:02.000000 module-utilities-0.4.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1371 2023-06-14 21:18:50.000000 module-utilities-0.4.0/.gitignore
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      161 2023-04-27 23:45:36.000000 module-utilities-0.4.0/.markdownlint.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3644 2023-06-14 21:18:50.000000 module-utilities-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       20 2023-04-27 23:45:36.000000 module-utilities-0.4.0/.prettierrc.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      527 2023-06-14 20:02:14.000000 module-utilities-0.4.0/.recipe-append.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      122 2023-04-27 23:45:36.000000 module-utilities-0.4.0/AUTHORS.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      645 2023-06-14 21:18:50.000000 module-utilities-0.4.0/CHANGELOG.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9874 2023-06-14 21:18:50.000000 module-utilities-0.4.0/CONTRIBUTING.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1789 2023-06-14 21:18:50.000000 module-utilities-0.4.0/LICENSE
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      258 2023-04-27 23:45:36.000000 module-utilities-0.4.0/MANIFEST.in
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9401 2023-06-14 21:18:50.000000 module-utilities-0.4.0/Makefile
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9286 2023-06-14 21:22:11.773665 module-utilities-0.4.0/PKG-INFO
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5615 2023-06-14 21:18:50.000000 module-utilities-0.4.0/README.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.734596 module-utilities-0.4.0/changelog.d/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       64 2023-04-27 23:45:36.000000 module-utilities-0.4.0/changelog.d/README.txt
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.735025 module-utilities-0.4.0/changelog.d/templates/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.736026 module-utilities-0.4.0/changelog.d/templates/auto-changelog/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      213 2023-04-27 23:45:36.000000 module-utilities-0.4.0/changelog.d/templates/auto-changelog/macros.jinja2
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      774 2023-04-27 23:45:36.000000 module-utilities-0.4.0/changelog.d/templates/auto-changelog/template.jinja2
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      269 2023-04-27 23:45:36.000000 module-utilities-0.4.0/changelog.d/templates/new_fragment.md.j2
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      204 2023-04-27 23:45:36.000000 module-utilities-0.4.0/conftest.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.740769 module-utilities-0.4.0/docs/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1401 2023-05-03 02:36:13.000000 module-utilities-0.4.0/docs/Makefile
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.718685 module-utilities-0.4.0/docs/_static/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.741128 module-utilities-0.4.0/docs/_static/css/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2937 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/_static/css/nist-combined.css
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.742006 module-utilities-0.4.0/docs/_static/js/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      767 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/_static/js/leave_notice.js
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      706 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/_static/js/nist-header-footer.js
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.744842 module-utilities-0.4.0/docs/_templates/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.746778 module-utilities-0.4.0/docs/_templates/autodocsumm/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      289 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/_templates/autodocsumm/class-noindex.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      249 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/_templates/autodocsumm/class.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      405 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/_templates/autodocsumm/module-inherit.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      424 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/_templates/autodocsumm/module-noindex.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      374 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/_templates/autodocsumm/module.rst
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.747912 module-utilities-0.4.0/docs/_templates/autosummary/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      106 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1255 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1119 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1418 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/_templates/class-individual-pages.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1255 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/_templates/class-single-page.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1186 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/_templates/custom-module-template.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1212 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/_templates/module-custom-imported.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1177 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/_templates/module-custom.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1071 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/_templates/module-single.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1179 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/_templates/module-template.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       69 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/authors.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       71 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/changelog.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    14851 2023-06-14 20:02:42.000000 module-utilities-0.4.0/docs/conf.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       74 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/contributing.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.748343 module-utilities-0.4.0/docs/examples/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       75 2023-06-14 21:18:50.000000 module-utilities-0.4.0/docs/examples/index.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.749447 module-utilities-0.4.0/docs/examples/usage/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    13498 2023-05-03 02:36:13.000000 module-utilities-0.4.0/docs/examples/usage/cached.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    18227 2023-05-03 20:28:18.000000 module-utilities-0.4.0/docs/examples/usage/docfiller.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      224 2023-06-14 20:02:45.000000 module-utilities-0.4.0/docs/index.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      940 2023-06-14 21:18:50.000000 module-utilities-0.4.0/docs/installation.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       40 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/license.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      767 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/make.bat
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      169 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/navigation.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.750032 module-utilities-0.4.0/docs/reference/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      192 2023-06-14 20:02:51.000000 module-utilities-0.4.0/docs/reference/index.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 23:45:36.000000 module-utilities-0.4.0/docs/spelling_wordlist.txt
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.754775 module-utilities-0.4.0/environment/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      227 2023-06-14 21:18:50.000000 module-utilities-0.4.0/environment/base.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      419 2023-06-14 21:18:50.000000 module-utilities-0.4.0/environment/dev.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      299 2023-06-14 21:18:50.000000 module-utilities-0.4.0/environment/dist-conda.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      225 2023-06-14 21:18:50.000000 module-utilities-0.4.0/environment/dist-pypi.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      418 2023-06-14 21:18:50.000000 module-utilities-0.4.0/environment/docs.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      136 2023-05-02 03:09:02.000000 module-utilities-0.4.0/environment/lint.yaml
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.756369 module-utilities-0.4.0/environment/lock/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       64 2023-06-14 21:18:50.000000 module-utilities-0.4.0/environment/lock/py310.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       64 2023-06-14 21:18:50.000000 module-utilities-0.4.0/environment/lock/py311.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       63 2023-06-14 21:18:50.000000 module-utilities-0.4.0/environment/lock/py38.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       63 2023-06-14 21:18:50.000000 module-utilities-0.4.0/environment/lock/py39.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      193 2023-06-14 21:18:50.000000 module-utilities-0.4.0/environment/test-extras.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      265 2023-06-14 21:18:50.000000 module-utilities-0.4.0/environment/test-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      287 2023-06-14 21:18:50.000000 module-utilities-0.4.0/environment/test.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      296 2023-06-14 21:18:50.000000 module-utilities-0.4.0/environment/typing.yaml
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.756790 module-utilities-0.4.0/examples/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      222 2023-04-27 23:45:36.000000 module-utilities-0.4.0/examples/README.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.758142 module-utilities-0.4.0/examples/usage/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    13498 2023-05-03 02:36:13.000000 module-utilities-0.4.0/examples/usage/cached.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    18227 2023-05-03 20:28:18.000000 module-utilities-0.4.0/examples/usage/docfiller.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    29603 2023-06-14 21:18:50.000000 module-utilities-0.4.0/noxfile.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     7469 2023-06-14 21:18:50.000000 module-utilities-0.4.0/pyproject.toml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       38 2023-06-14 21:22:11.774261 module-utilities-0.4.0/setup.cfg
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.723004 module-utilities-0.4.0/src/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.763036 module-utilities-0.4.0/src/module_utilities/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      546 2023-06-14 21:18:50.000000 module-utilities-0.4.0/src/module_utilities/__init__.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2646 2023-05-02 03:09:02.000000 module-utilities-0.4.0/src/module_utilities/_doc.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      382 2023-05-02 03:09:02.000000 module-utilities-0.4.0/src/module_utilities/_typing.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5930 2023-05-03 20:28:18.000000 module-utilities-0.4.0/src/module_utilities/attributedict.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9991 2023-05-03 20:28:18.000000 module-utilities-0.4.0/src/module_utilities/cached.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    21035 2023-06-14 21:18:50.000000 module-utilities-0.4.0/src/module_utilities/docfiller.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-02 03:09:02.000000 module-utilities-0.4.0/src/module_utilities/py.typed
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.770461 module-utilities-0.4.0/src/module_utilities/vendored/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1298 2023-06-14 21:18:50.000000 module-utilities-0.4.0/src/module_utilities/vendored/LICENSE.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       93 2023-06-14 21:18:50.000000 module-utilities-0.4.0/src/module_utilities/vendored/README.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       24 2023-06-14 21:18:50.000000 module-utilities-0.4.0/src/module_utilities/vendored/__init__.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    23449 2023-06-14 21:18:50.000000 module-utilities-0.4.0/src/module_utilities/vendored/docscrape.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.766773 module-utilities-0.4.0/src/module_utilities.egg-info/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9286 2023-06-14 21:22:11.000000 module-utilities-0.4.0/src/module_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2659 2023-06-14 21:22:11.000000 module-utilities-0.4.0/src/module_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-06-14 21:22:11.000000 module-utilities-0.4.0/src/module_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      719 2023-06-14 21:22:11.000000 module-utilities-0.4.0/src/module_utilities.egg-info/requires.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       17 2023-06-14 21:22:11.000000 module-utilities-0.4.0/src/module_utilities.egg-info/top_level.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-05-04 19:05:27.000000 module-utilities-0.4.0/src/module_utilities.egg-info/zip-safe
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.772576 module-utilities-0.4.0/tests/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       46 2023-04-27 23:45:36.000000 module-utilities-0.4.0/tests/__init__.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 23:45:36.000000 module-utilities-0.4.0/tests/conftest.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    10864 2023-05-02 03:09:02.000000 module-utilities-0.4.0/tests/test_cached.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     8959 2023-05-03 20:28:18.000000 module-utilities-0.4.0/tests/test_docfiller.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      169 2023-06-14 20:04:01.000000 module-utilities-0.4.0/tests/test_module_utilities.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-14 21:22:11.772964 module-utilities-0.4.0/tools/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    20805 2023-06-14 21:18:50.000000 module-utilities-0.4.0/tools/noxtools.py
```

### Comparing `module-utilities-0.3.1/.cruft.json` & `module-utilities-0.4.0/.cruft.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7986842105263158%*

 * *Differences: {"'checkout'": "'feature/nox'",*

 * * "'commit'": "'8b671d07d854bd6f5bd566267cc39118c8d76ba7'",*

 * * "'context'": "{'cookiecutter': {'conda_channel': 'conda-forge'}}"}*

```diff
@@ -1,25 +1,25 @@
 {
-    "checkout": "feature/markdown",
-    "commit": "10a9fe1a4f0b341184e41953433c344020f92c72",
+    "checkout": "feature/nox",
+    "commit": "8b671d07d854bd6f5bd566267cc39118c8d76ba7",
     "context": {
         "cookiecutter": {
             "_copy_without_render": [
                 "*.html",
                 "docs/_templates/*.rst",
                 "docs/_templates/autosummary/*.rst",
                 "docs/_templates/autodocsumm/*.rst",
                 "docs/_static/css/*",
                 "docs/_static/js/*",
                 "changelog.d/templates/*.j2",
                 "changelog.d/templates/auto-changelog/*.jinja2"
             ],
             "_template": "https://github.com/wpk-nist-gov/cookiecutter-pypackage.git",
             "command_line_interface": "No command-line interface",
-            "conda_channel": "wpk-nist",
+            "conda_channel": "conda-forge",
             "create_author_file": "y",
             "email": "wpk@nist.gov",
             "full_name": "William P. Krekelberg",
             "github_username": "usnistgov",
             "open_source_license": "NIST license",
             "project_name": "module-utilities",
             "project_short_description": "Collection of utilities to aid working with python modules.",
```

### Comparing `module-utilities-0.3.1/.editorconfig` & `module-utilities-0.4.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.1/.gitignore` & `module-utilities-0.4.0/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 # Installer logs
 pip-log.txt
 pip-delete-this-directory.txt
 
 # Unit test / coverage reports
 htmlcov/
 .tox/
+.nox/
 .coverage
 .coverage.*
 .cache
 nosetests.xml
 coverage.xml
 *.cover
 .hypothesis/
@@ -102,11 +103,14 @@
 .mypy_cache/
 
 # IDE settings
 .vscode/
 pyrightconfig.json
 .autoenv.zsh
 .autoenv_leave.zsh
+.noxconfig.toml
+cruft.patch
 /docs/**/generated/
 /monkeytype.sqlite3
 /dist-conda/
 /tmp/
+/module-utilities-feedstock*/
```

### Comparing `module-utilities-0.3.1/.pre-commit-config.yaml` & `module-utilities-0.4.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -41,21 +41,22 @@
       - id: ruff
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       # - id: black-jupyter
       # Move to just black.  use nbqa for notebook formatting
       - id: black
+        exclude: ^src/module-utilities/vendored/docscrape.py
   - repo: https://github.com/adamchainz/blacken-docs
     rev: "1.13.0"
     hooks:
       - id: blacken-docs
         additional_dependencies:
           - black==23.3.0
-        exclude: ^README.md
+        # exclude: ^README.md
   - repo: https://github.com/nbQA-dev/nbQA
     rev: 1.7.0
     hooks:
       - id: nbqa-ruff
         additional_dependencies: [ruff]
       - id: nbqa-black
         additional_dependencies: [black]
```

### Comparing `module-utilities-0.3.1/.recipe-append.yaml` & `module-utilities-0.4.0/.recipe-append.yaml`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.1/CONTRIBUTING.md` & `module-utilities-0.4.0/CONTRIBUTING.md`

 * *Files 11% similar despite different names*

```diff
@@ -39,75 +39,89 @@
 <https://github.com/usnistgov/module-utilities/issues>.
 
 If you are proposing a feature:
 
 - Explain in detail how it would work.
 - Keep the scope as narrow as possible, to make it easier to implement.
 - Remember that this is a volunteer-driven project, and that contributions are
-  welcome :)
+  welcome!
 
 ## Get Started
 
 ### Environment setup
 
 [pipx]: https://github.com/pypa/pipx
 [condax]: https://github.com/mariusvniekerk/condax
 [mamba]: https://github.com/mamba-org/mamba
 [conda-fast-setup]:
   https://www.anaconda.com/blog/a-faster-conda-for-a-growing-community
 [pre-commit]: https://pre-commit.com/
+[nox]: https://github.com/wntrblm/nox
+[noxopt]: https://github.com/rmorshea/noxopt
 [tox]: https://tox.wiki/en/latest/
-[tox-conda]: https://github.com/tox-dev/tox-conda
 [cruft]: https://github.com/cruft/cruft
-[conda-merge]: https://github.com/amitbeka/conda-merge
+[cog]: https://github.com/nedbat/cog
 [git-flow]: https://github.com/nvie/gitflow
 [scriv]: https://github.com/nedbat/scriv
 [conventional-style]: https://www.conventionalcommits.org/en/v1.0.0/
 [commitizen]: https://github.com/commitizen-tools/commitizen
 [nb_conda_kernels]: https://github.com/Anaconda-Platform/nb_conda_kernels
+[pyproject2conda]: https://github.com/wpk-nist-gov/pyproject2conda
 
 This project uses a host of tools to (hopefully) make development easier. We
 recommend installing some of these tools system wide. For this, we recommend
 using either [pipx] or [condax]. We mostly use conda/condax, but the choice is
 yours. For conda, we recommend actually using [mamba]. Alternatively, you can
 setup `conda` to use the faster `mamba` solver. See [here][conda-fast-setup] for
 details.
 
 Additional tools are:
 
 - [pre-commit]
-- [tox] and [tox-conda]
+- [nox] with [noxopt]
 - [cruft]
-- [conda-merge]
 - [scriv]
+- [commitizen] (optional)
+- [pyproject2conda] (optional)
+- [cog] (optional)
 
 These are setup using the following:
 
 ```console
-condax install pre-commit
-condax install tox
-condax inject tox tox-conda
-condax install cruft
-condax install conda-merge
-condax install commitizen
+condax/pipx install pre-commit
+condax/pipx install cruft
+condax/pipx install commitizen # optional
 pipx install scriv
+pipx install pyproject2conda # optional
+condax/pipx install cogapp # optional
 ```
 
-Alternatively, you can install these dependencies using:
+if using pipx, nox can be installed with:
 
-```console
-conda env update -n {env-name} environment/tools.yaml
+```bash
+pipx install nox
+pipx inject nox ruamel.yaml
+pipx inject nox noxopt
+```
+
+If using condax, you'll need to use:
+
+```bash
+condax install nox
+condax inject nox ruamel.yaml
+conda activate ~/.condax/nox
+pip install noxopt
 ```
 
 ### Getting the repo
 
-Ready to contribute? Here's how to set up `module_utilities` for local
+Ready to contribute? Here's how to set up `module-utilities` for local
 development.
 
-- Fork the `module_utilities` repo on GitHub.
+- Fork the `module-utilities` repo on GitHub.
 
 - Clone your fork locally:
 
   ```bash
   git clone git@github.com:your_name_here/module-utilities.git
   ```
 
@@ -124,57 +138,40 @@
   cd module-utilities
   git submodule update --init --recursive
   ```
 
 - Create development environment. There are two options to create the
   development environment.
 
-  - The recommended method is to use tox by using either:
+  - The recommended method is to use nox. First you'll need to create the
+    environment files using:
 
     ```bash
-    tox -e dev
+    nox -e pyproject2conda
     ```
 
-    or
+    Then run:
 
     ```bash
-    make dev-env
+    nox -e dev
     ```
 
-    These create a development environment located at `.tox/dev`.
-
-    ```bash
-    make tox-ipykernel-display-name
-    ```
-
-    This will add a meaningful display name for the kernel (assuming you're
-    using [nb_conda_kernels])
+    This create a development environment located at `.nox/dev`.
 
   - Alternativley, you can create centrally located conda environmentment using
     the command:
 
     ```bash
-    make mamba-dev
+    conda/mamba env create -n {env-name} -f environment/dev.yaml
     ```
 
-    This will create a conda environment 'module-utilities-env' in the default
-    location.
-
-    To install (an editable version) of the current package:
-
     ```bash
     pip install -e . --no-deps
     ```
 
-    or
-
-    ```bash
-    make install-dev
-    ```
-
 - Initiate [pre-commit] with:
 
   ```bash
   pre-commit install
   ```
 
   To update the recipe, periodically run:
@@ -207,24 +204,18 @@
 
   To run tests, use:
 
   ```bash
   pytest
   ```
 
-  To test against multiple python versions, use tox:
-
-  ```bash
-  tox
-  ```
-
-  or using the `make`:
+  To test against multiple python versions, use [nox]:
 
   ```bash
-  make test-all
+  nox -s test
   ```
 
   Additionally, you should run the following:
 
   ```bash
   make pre-commit-lint-markdown
   make pre-commit-codespell
@@ -252,152 +243,161 @@
   cz commit
   ```
 
 - Submit a pull request through the GitHub website.
 
 ### Dependency management
 
-Dependencies need to be placed in a few locations, which depend on the nature of
-the dependency.
-
-- Package dependency: `environment.yaml` and `dependencies` section of
-  `pyproject.toml`
-- Documentation dependency: `environment/docs-extras.yaml` and `test` section of
-  `pyproject.toml`
-- Development dependency: `environment/dev-extras.yaml` and `dev` section of
-  `pyproject.toml`
-
-Note that total yaml files are build using [conda-merge]. For example,
-`environment.yaml` is combined with `environment/docs-extras.yaml` to produce
-`environment/docs.yaml`. This is automated in the `Makefile`. You can also run,
-after doing any updates,
+We use [pyproject2conda] to handle conda `environment.yaml` files. This extracts
+the dependencies from `pyproject.toml`. See [pyproject2conda] for info. To make
+the `environment.yaml` files, run:
 
 ```bash
-make environment-files-build
+nox -s pyproject2conda -- [--pyproject2conda-force]
 ```
 
-which will rebuild all the needed yaml files.
+Where the option in brackets is optional.
 
 ## Pull Request Guidelines
 
 Before you submit a pull request, check that it meets these guidelines:
 
 - The pull request should include tests.
 - If the pull request adds functionality, the docs should be updated. Put your
   new functionality into a function with a docstring, and add the feature to the
   list in CHANGELOG.md. You should use [scriv] for this.
 - The pull request should work for Python 3.8, 3.9, 3.10.
 
-## Building the docs
+## ipykernel
 
-We use [tox] to isolate the documentation build. Useful commands are as follows.
+The environments created by nox `dev` and `docs` will try to add meaningful
+display names for ipykernel (assuming you're using [nb_conda_kernels])
 
-- Build the docs:
+## Building the docs
 
-  ```bash
-  tox -e docs -- build
-  ```
+We use [nox] to isolate the documentation build. Specific tasks can be run with
 
-- Spellcheck the docs:
+```bash
+nox -s docs -- -d [commands]
+```
 
-  ```bash
-  tox -e docs -- spelling
-  ```
+where commands can be one of:
 
-- Create a release of the docs:
+- clean : remove old doc build
+- build/html : build html documentation
+- spelling : check spelling
+- linkcheck : check the links
+- symlink : rebuild symlinks from `examples` to `docs/examples`
+- release : make pages branch for documentation hosting (using
+  [ghp-import](https://github.com/c-w/ghp-import))
+- livehtml : Live documentation updates
+- open : open the documentation in a web browser
 
-  ```bash
-  tox -e docs -- release
-  ```
+## Testing with nox
 
-  If you make any changes to `docs/examples`, you should run:
+The basic command is:
 
-  ```bash
-  make docs-examples-symlink
-  ```
+```bash
+nox -s test -- [--test-opts] [--no-cov]
+```
 
-  to update symlinks from `docs/examples` to `examples`.
+where you can pass in additional pytest options (properly escaped) via
+`--test-opts`. For example:
 
-  After this, the docs can be pushed to the correct branch for distribution.
+```bash
+nox -s test -- --test-opts "'-v'"
+# or
+nox -s test -- --test-opts "\-v"
+```
 
-- Live documentation updates using
+## Building distribution for conda
 
-  ```bash
-  make docs-livehtml
-  ```
+[grayskull]: https://github.com/conda/grayskull
 
-## Using tox
+For the most part, we use [grayskull] to create the conda recipe. However, I've
+had issues getting it to play nice with `pyproject.toml` for some of the 'extra'
+variables. So, we use grayskull to build the majority of the recipe, and append
+the file `.recipe-append.yaml`. For some edge cases (install name different from
+package name, etc), you'll need to manually edit this file to create the final
+recipe.
 
-The package is setup to use tox to test, build and release pip and conda
-distributions, and release the docs. Most of these tasks have a command in the
-`Makefile`. To test against multiple versions, use:
+The basic command is:
 
 ```bash
-make test-all
+nox -s dist-conda -- -c [command]
 ```
 
-To build the documentation in an isolated environment, use:
+Where `command` is one of:
 
-```bash
-make docs-build
-```
+- clean
+- recipe : create recipe via [grayskull]
+- build : build the distribution
 
-To release the documentation use:
+To upload the recipe, you'll need to run an external command like:
 
 ```bash
-make docs-release release_args='-m "commit message" -r origin -p'
+nox -s dist-conda -- --dist-conda-run "anaconda upload PATH-TO-TARBALL"
 ```
 
-Where posargs is are passed to ghp-import. Note that the branch created is
-called `nist-pages`. This can be changed in `tox.ini`.
+## Building distribution for pypi
 
-To build the distribution, use:
+The basic command is:
 
 ```bash
-make dist-pypi-[build-testrelease-release]
+nox -s dist-pypi -- -p [command]
 ```
 
-where `build` build to distro, `testrelease` tests putting on `testpypi` and
-release puts the distro on pypi.
+where `command` is one of:
+
+- clean : clean out old distribution
+- build : build distribution (if specify only this, clean will be called first)
+- testrelease : upload to testpypi
+- release : upload to pypi
+
+## Testing pypi or conda installs
 
-To build the conda distribution, use:
+Run:
 
 ```bash
-make dist-conda-[recipe, build]
+nox -s testdist-pypi -- --version [version]
 ```
 
-where `recipe` makes the conda recipe (using grayskull), and `build` makes the
-distro. This can be manually added to a channel.
-
-To test the created distributions, you can use one of:
+to test a specific version from pypi and
 
 ```bash
-tox -e test-dist-[pypi, conda]-[local,remote]-py[38,39,...]
+nox -s testdist-conda -- --version [version]
 ```
 
-or
+to to likewise from conda.
+
+## Type checking
+
+Run:
 
 ```bash
-make test-dist-[pypi, conda]-[local,remote] py=[38, 39, 310]
+nox -s typing -- -m [commands] [options]
 ```
 
-where one options in the brackets should be choosen.
-
 ## Package version
 
 [setuptools_scm]: https://github.com/pypa/setuptools_scm
 
-Versioning is handled with [setuptools_scm].The pacakge version is set by the
-git tag. For convenience, you can override the version in the makefile (calling
-tox) by setting `version=v{major}.{minor}.{micro}`. This is useful for updating
-the docs, etc.
+Versioning is handled with [setuptools_scm].The package version is set by the
+git tag. For convenience, you can override the version with nox setting
+`--version ...`. This is useful for updating the docs, etc.
 
-## Creating conda recipe
+## Notes on [nox]
 
-[grayskull]: https://github.com/conda/grayskull
+One downside of using [tox] with this particular workflow is the need for
+multiple scripts/makefiles, while with [nox], most everything is self contained
+in the file `noxfile.py`. [nox] also is allows for a mix of conda and virtualenv
+environments.
 
-For the most part, we use [grayskull] to create the conda recipe. However, I've
-had issues getting it to play nice with `pyproject.toml` for some of the 'extra'
-variables. So, we use grayskull to build the majority of the recipe, and append
-the file `.recipe-append.yaml`. For some edge cases (install name different from
-package name, etc), you'll need to manually edit this file to create the final
-recipe.
+## Serving the documentation
+
+To view to documentation with js headers/footers, you'll need to serve them:
+
+```bash
+python -m http.server -d docs/_build/html
+```
+
+Then open the address `localhost:8000` in a webbrowser.
```

### Comparing `module-utilities-0.3.1/LICENSE` & `module-utilities-0.4.0/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -18,7 +18,12 @@
 CONTRACT, TORT, OR OTHERWISE, WHETHER OR NOT INJURY WAS SUSTAINED BY PERSONS OR
 PROPERTY OR OTHERWISE, AND WHETHER OR NOT LOSS WAS SUSTAINED FROM, OR AROSE OUT
 OF THE RESULTS OF, OR USE OF, THE SOFTWARE OR SERVICES PROVIDED HEREUNDER.
 
 Distributions of NIST software should also include copyright and licensing
 statements of any third-party software that are legally bundled with the code in
 compliance with the conditions of those licenses.
+
+---
+
+module-utilities vendors a copy of docscrape.py from numpydoc.
+The license is BSD and include at "module_utilities/vendored/LICENSE.txt".
```

### Comparing `module-utilities-0.3.1/Makefile` & `module-utilities-0.4.0/Makefile`

 * *Files 21% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 clean-pyc: ## remove Python file artifacts
 	find . -name '*.pyc' -exec rm -f {} +
 	find . -name '*.pyo' -exec rm -f {} +
 	find . -name '*~' -exec rm -f {} +
 	find . -name '__pycache__' -exec rm -fr {} +
 
 clean-test: ## remove test and coverage artifacts
-	rm -fr .tox/
+	rm -fr .nox/
 	rm -f .coverage
 	rm -fr htmlcov/
 	rm -fr .pytest_cache
 
 
 
 
@@ -99,15 +99,15 @@
 
 
 ################################################################################
 # my convenience functions
 ################################################################################
 .PHONY: user-venv user-autoenv-zsh user-all
 user-venv: ## create .venv file with name of conda env
-	echo $${PWD}/.tox/dev > .venv
+	echo $${PWD}/.nox/dev > .venv
 
 user-autoenv-zsh: ## create .autoenv.zsh files
 	echo conda activate $$(cat .venv) > .autoenv.zsh
 	echo conda deactivate > .autoenv_leave.zsh
 
 user-all: user-venv user-autoenv-zsh ## runs user scripts
 
@@ -115,14 +115,17 @@
 ################################################################################
 # Testing
 ################################################################################
 .PHONY: test coverage
 test: ## run tests quickly with the default Python
 	pytest -x -v
 
+test-accept: ## run tests and accept doctest results. (using pytest-accept)
+	DOCFILLER_SUB=False pytest -v --accept
+
 coverage: ## check code coverage quickly with the default Python
 	coverage run --source module_utilities -m pytest
 	coverage report -m
 	coverage html
 	$(BROWSER) htmlcov/index.html
 
 
@@ -137,167 +140,117 @@
 	python -c 'import module_utilities; print(module_utilities.__version__)'
 
 version: version-scm version-import
 
 ################################################################################
 # Environment files
 ################################################################################
-ENVIRONMENTS = $(addsuffix .yaml,$(addprefix environment/, dev docs test))
-PRETTIER = bash scripts/run-prettier.sh
-
-environment/%.yaml: environment.yaml environment/%-extras.yaml ## create combined environment/{dev,docs,test}.yaml
-	conda-merge $^ > $@
-	$(PRETTIER) $@
-
-environment/dev.yaml: ## development environment yaml file
-environment/test.yaml: ## testing environment yaml file
-enviornment/docs.yaml: ## docs environment yaml file
-
-
-# special for linters
-environment/lint.yaml: environment.yaml $(addsuffix .yaml, $(addprefix environment/, test-extras lint-extras)) ## mypy environment
-	echo $^
-	conda-merge $^ > $@
-	$(PRETTIER) $@
-
-ENVIRONMENTS += environment/lint.yaml
-
 .PHONY: environment-files-clean
 environment-files-clean: ## clean all created environment/{dev,docs,test}.yaml
 	-rm $(ENVIRONMENTS) 2> /dev/null || true
 
 .PHONY: environment-files-build
-environment-files-build: $(ENVIRONMENTS) ## rebuild all environment files
+environment-files-build: pyproject.toml ## rebuild all environment files
+	nox -s pyproject2conda
+
+environment/%.yaml: pyproject.toml
+	nox -s pyproject2conda
 
 ################################################################################
 # virtual env
 ################################################################################
-.PHONY: mamba-env mamba-dev mamba-env-update mamba-dev-update
+.PHONY: mamba-env-update mamba-dev-update
 
-mamba-env: environment.yaml ## create base environment
+mamba-dev: environment/dev.yaml environment-files-build ## create development environment
 	mamba env create -f $<
 
-mamba-env-update: environment.yaml ## update base environment
-	mamba env update -f $<
-
-mamba-dev: environment/dev.yaml ## create development environment
-	mamba env create -f $<
-
-mamba-dev-update: environment/dev.yaml ## update development environment
+mamba-dev-update: environment/dev.yaml environment-files-build ## update development environment
 	mamba env update -f $<
 
 ################################################################################
-# TOX
+# NOX
 ###############################################################################
-tox_args?=-v
-version?=
-TOX=CONDA_EXE=mamba SETUPTOOLS_SCM_PRETEND_VERSION=$(version) tox $(tox_args)
-
-.PHONY: tox-ipykernel-display-name
-tox-ipykernel-display-name: ## Update display-name for any tox env with ipykernel
-	bash ./scripts/tox-ipykernel-display-name.sh module-utilities
-
 ## dev env
+NOX=nox
 .PHONY: dev-env
-dev-env: environment/dev.yaml ## create development environment using tox
-	tox -e dev
+dev-env: environment/dev.yaml ## create development environment using nox
+	$(NOX) -e dev
 
 ## testing
 .PHONY: test-all
-test-all: environment/test.yaml ## run tests on every Python version with tox.  can pass posargs=...
-	$(TOX) -- $(posargs)
+test-all: environment/test.yaml ## run tests on every Python version with nox.
+	$(NOX) -s test
 
 ## docs
-.PHONY: docs-examples-symlink
-docs-examples-symlink: ## create symlinks to notebooks from /examples/ to /docs/examples.
-	bash ./scripts/docs-examples-symlinks.sh
-
-
 .PHONY: docs-build docs-release docs-clean docs-command
 docs-build: ## build docs in isolation
-	$(TOX) -e docs -- build
+	$(NOX) -s docs -- -d build
 docs-clean: ## clean docs
 	rm -rf docs/_build/*
 	rm -rf docs/generated/*
 	rm -rf docs/reference/generated/*
 docs-clean-build: docs-clean docs-build ## clean and build
-docs-release: ## release docs.  use release_args=... to override stuff
-	$(TOX) -e docs -- release
-docs-command: ## run command with command=...
-	$(TOX) -e docs -- command
+docs-release: ## release docs.
+	$(NOX) -s docs -- release
+docs-command: ## run arbitrary command with command=...
+	$(NOX) -s docs -- --docs-run $(command)
 
 .PHONY: .docs-spelling docs-nist-pages docs-open docs-livehtml docs-clean-build docs-linkcheck
 docs-spelling: ## run spell check with sphinx
-	$(TOX) -e docs -- spelling
+	$(NOX) -s docs -- -d spelling
 docs-livehtml: ## use autobuild for docs
-	$(TOX) -e docs -- livehtml
+	$(NOX) -s docs -- -d livehtml
 docs-open: ## open the build
-	$(BROWSER) docs/_build/html/index.html
+	$(NOX) -s docs -- -d open
 docs-linkcheck: ## check links
-	$(TOX) -e docs -- linkcheck
+	$(NOX) -s docs -- -d linkcheck
 
 docs-build docs-release docs-command docs-clean docs-livehtml docs-linkcheck: environment/docs.yaml
 
-## linting
-.PHONY: lint-mypy lint-pyright lint-pytype lint-all lint-command
-lint-mypy: ## run mypy mypy_args=...
-	$(TOX) -e lint -- mypy
-lint-pyright: ## run pyright pyright_args=...
-	$(TOX) -e lint -- pyright
-lint-pytype: ## run pytype pytype_args=...
-	$(TOX) -e lint -- pytype
-lint-all:
-	$(TOX) -e lint -- all
-lint-command:
-	$(TOX) -e lint -- command
-
-lint-mypy lint-pyright lint-pytype lint-all lint-command: environment/lint.yaml
+## typing
+.PHONY: typing-mypy typing-pyright typing-pytype typing-all typing-command
+typing-mypy: ## run mypy mypy_args=...
+	$(NOX) -s typing -- -m mypy
+typing-pyright: ## run pyright pyright_args=...
+	$(NOX) -s typing -- -m pyright
+typing-pytype: ## run pytype pytype_args=...
+	$(NOX) -s typing -- -m pytype
+typing-all:
+	$(NOX) -s typing -- -m mypy pyright pytype
+typing-command:
+	$(NOX) -s typing -- --typing-run $(command)
+typing-mypy typing-pyright typing-pytype typing-all typing-command: environment/typing.yaml
 
 ## distribution
 .PHONY: dist-pypi-build dist-pypi-testrelease dist-pypi-release dist-pypi-command
 
 dist-pypi-build: ## build dist
-	$(TOX) -e dist-pypi -- build
+	$(NOX) -s dist-pypi -- -p build
 dist-pypi-testrelease: ## test release on testpypi
-	$(TOX) -e dist-pypi -- testrelease
+	$(NOX) -s dist-pypi -- -p testrelease
 dist-pypi-release: ## release to pypi, can pass posargs=...
-	$(TOX) -e dist-pypi -- release
+	$(NOX) -s dist-pypi -- -p release
 dist-pypi-command: ## run command with command=...
-	$(TOX) -e dist-pypi -- command
+	$(NOX) -s dist-pypi -- --dist-pypi-run $(command)
 dist-pypi-build dist-pypi-testrelease dist-pypi-release dist-pypi-command: environment/dist-pypi.yaml
 
 .PHONY: dist-conda-recipe dist-conda-build dist-conda-command
 dist-conda-recipe: ## build conda recipe can pass posargs=...
-	$(TOX) -e dist-conda -- recipe
+	$(NOX) -s dist-conda -- -c recipe
 dist-conda-build: ## build conda recipe can pass posargs=...
-	$(TOX) -e dist-conda -- build
+	$(NOX) -s dist-conda -- -c build
 dist-conda-command: ## run command with command=...
-	$(TOX) -e dist-conda -- command
+	$(NOX) -s dist-conda -- -dist-conda-run $(command)
 dist-conda-build dist-conda-recipe dist-conda-command: environment/dist-conda.yaml
 
 
-## test distribution
-.PHONY: testdist-pypi-remote testdist-conda-remote testdist-pypi-local testdist-conda-local
-
-py?=310
-testdist-pypi-remote: ## testdist-pypi-remote: ## test pypi install, can run as `make test-dist-pypi-remote py=39` to run test-dist-pypi-local-py39.  Can specify version setting, eg,  TEST_VERSION='==0.1.0'.  Note that the the format should be '=={version}'.
-	$(TOX) -e $@-py$(py) -- $(posargs)
-testdist-conda-remote: ## test conda install, can run as `make test-dist-conda-remote py=39` to run test-dist-conda-local-py39
-	$(TOX) -e $@-py$(py) -- $(poasargs)
-testdist-pypi-local: ## test pypi install, can run as `make test-dist-pypi-local py=39` to run test-dist-pypi-local-py39
-	$(TOX) -e $@-py$(py) -- $(posargs)
-testdist-conda-local: ## test conda install, can run as `make test-dist-conda-local py=39` to run test-dist-conda-local-py39
-	$(TOX) -e $@-py$(py) -- $(poasargs)
-
-testdist-pypi-remote testdist-conda-remote testdist-pypi-local testdist-conda-local: environment/test.yaml
-
 ## list all options
-.PHONY: tox-list
-tox-list:
-	$(TOX) -a
+.PHONY: nox-list
+nox-list:
+	$(NOX) --list
 
 
 ################################################################################
 # installation
 ################################################################################
 .PHONY: install install-dev
 install: ## install the package to the active Python's site-packages (run clean?)
```

### Comparing `module-utilities-0.3.1/changelog.d/templates/auto-changelog/template.jinja2` & `module-utilities-0.4.0/changelog.d/templates/auto-changelog/template.jinja2`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.1/docs/Makefile` & `module-utilities-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.1/docs/_static/css/nist-combined.css` & `module-utilities-0.4.0/docs/_static/css/nist-combined.css`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.1/docs/_static/js/leave_notice.js` & `module-utilities-0.4.0/docs/_static/js/leave_notice.js`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.1/docs/_static/js/nist-header-footer.js` & `module-utilities-0.4.0/docs/_static/js/nist-header-footer.js`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.1/docs/_templates/autosummary/class.rst` & `module-utilities-0.4.0/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.1/docs/_templates/autosummary/module.rst` & `module-utilities-0.4.0/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.1/docs/_templates/class-individual-pages.rst` & `module-utilities-0.4.0/docs/_templates/class-individual-pages.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.1/docs/_templates/class-single-page.rst` & `module-utilities-0.4.0/docs/_templates/class-single-page.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.1/docs/_templates/custom-module-template.rst` & `module-utilities-0.4.0/docs/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.1/docs/_templates/module-custom-imported.rst` & `module-utilities-0.4.0/docs/_templates/module-custom-imported.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.1/docs/_templates/module-custom.rst` & `module-utilities-0.4.0/docs/_templates/module-custom.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.1/docs/_templates/module-single.rst` & `module-utilities-0.4.0/docs/_templates/module-single.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.1/docs/_templates/module-template.rst` & `module-utilities-0.4.0/docs/_templates/module-template.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.1/docs/conf.py` & `module-utilities-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.1/docs/examples/usage/cached.ipynb` & `module-utilities-0.4.0/docs/examples/usage/cached.ipynb`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.1/docs/examples/usage/docfiller.ipynb` & `module-utilities-0.4.0/docs/examples/usage/docfiller.ipynb`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.1/docs/installation.md` & `module-utilities-0.4.0/docs/installation.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Installation
 
 ## Stable release
 
 To install module-utilities, run this command in your terminal:
 
 ```bash
-pip install module_utilities
+pip install module-utilities
 ```
 
 or
 
 ```bash
-conda install -c wpk-nist module_utilities
+conda install -c conda-forge module-utilities
 ```
 
 This is the preferred method to install module-utilities, as it will always
 install the most recent stable release.
 
 ## From sources
```

### Comparing `module-utilities-0.3.1/docs/make.bat` & `module-utilities-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.1/examples/usage/cached.ipynb` & `module-utilities-0.4.0/examples/usage/cached.ipynb`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.1/examples/usage/docfiller.ipynb` & `module-utilities-0.4.0/examples/usage/docfiller.ipynb`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.1/pyproject.toml` & `module-utilities-0.4.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -28,49 +28,110 @@
 dependencies = ["typing-extensions"]
 
 [project.urls]
 homepage = "https://github.com/usnistgov/module-utilities"
 documentation = "https://pages.nist.gov/module-utilities/"
 
 [project.optional-dependencies]
-test = ["pytest"]
-attrs = ["attrs"]
+test = [
+    "pytest", #
+    "pytest-xdist",
+    "pytest-cov",
+    "pytest-sugar",
+]
+dev-extras = [
+    "pytest-accept", # p2c: -p
+    "setuptools-scm",
+    "ipython",
+    "ipykernel",
+]
+typing-extras = [
+    # "pytype; python_version < '3.11'",
+    "mypy",
+]
+typing = [
+    "module-utilities[typing-extras]", #
+    "module-utilities[test]",
+]
+nox = [
+    "nox",
+    "noxopt", # p2c: -p
+    "ruamel.yaml",
+]
+dev = [
+    "module-utilities[test]", #
+    "module-utilities[typing-extras]",
+    "module-utilities[dev-extras]",
+]
+tools = [
+    "pre-commit", #
+    "cruft",
+    "scriv",
+]
+dev-complete = [
+    "module-utilities[dev]", #
+    "module-utilities[tools]",
+    "module-utilities[nox]",
+]
+docs = [
+    "setuptools-scm", #
+    "ipython",
+    "pyenchant",
+    "ghp-import",
+    "sphinx",
+    "sphinx-copybutton",
+    "sphinxcontrib-spelling",
+    "sphinx-autobuild",
+    "myst-nb",
+    "sphinx-book-theme",
+    "autodocsumm",
+]
+# to be parsed with pyproject2conda with --no-base option
+dist-pypi = ["twine", "build"]
+dist-conda = [
+    "anaconda-client", #
+    "grayskull",
+    "conda-build",
+    "conda-verify",
+    "boa",
+    "setuptools-scm",
+]
+
+[tool.pyproject2conda]
+channels = ["conda-forge"]
 
-# dev = []
-# docs = []
 ## grayskull still messes some things up, but use scripts/recipe-append.sh for this
 [tool.setuptools]
 zip-safe = true # if using mypy, must be False
 include-package-data = true
 license-files = ["LICENSE"]
 
 [tool.setuptools.packages.find]
 namespaces = true
 where = ["src"]
 
 ## include = []
 ## exclude = []
-##
 [tool.setuptools.dynamic]
 readme = { file = [
     "README.md",
     "CHANGELOG.md",
     "LICENSE"
 ], content-type = "text/markdown" }
 
 [tool.setuptools_scm]
 fallback_version = "999"
 
 [tool.aliases]
 test = "pytest"
 
 [tool.pytest.ini_options]
-addopts = "--doctest-modules"
-# testpaths = ["src/module_utilities", "tests"]
-testpaths = ["src", "tests"]
+addopts = "--doctest-modules --doctest-glob='*.md'"
+# testpaths = ["src/module_utilities", "tests", "./README.md"]
+testpaths = ["src", "tests", "README.md"]
 
 [tool.isort]
 profile = "black"
 skip_gitignore = true
 known_first_party = ["module_utilities"]
 
 [tool.ruff]
@@ -130,14 +191,15 @@
     "buck-out",
     "build",
     "dist",
     "node_modules",
     "venv",
     "tests/",
     "src/module_utilities/tests",
+    "src/module_utilities/vendored",
 ]
 ignore = [
     # # whitespace before ':' - doesn't work well with black
     # "E203",
     # module level import not at top of file
     "E402",
     # line too long - let black worry about that
@@ -225,28 +287,33 @@
 [tool.mypy]
 files = ["src/**/*.py", "tests/**/*.py"]
 # files = ["src", "tests"]
 show_error_codes = true
 warn_unused_ignores = true
 warn_return_any = true
 warn_unused_configs = true
-exclude = [".eggs", ".tox", "doc", "docs"]
+exclude = [".eggs", ".tox", "doc", "docs", ".nox"]
 check_untyped_defs = true
 
 [[tool.mypy.overrides]]
 ignore_missing_imports = true
 module = []
 
 [[tool.mypy.overrides]]
 ignore_errors = true
-module = []
+module = ["module_utilities.vendored.docscrape"]
 
 [tool.pyright]
 include = ["src", "tests"]
-exclude = ["**/__pycache__", ".tox/**", "**/.mypy_cache"]
+exclude = [
+    "**/__pycache__",
+    ".tox/**",
+    "**/.mypy_cache",
+    "src/module-utilities/vendored"
+]
 pythonVersion = "3.10"
 typeCheckingMode = "basic"
 # enable subset of "strict"
 reportDuplicateImport = true
 reportInvalidStubStatement = true
 reportOverlappingOverload = true
 reportPropertyTypeMismatch = true
```

### Comparing `module-utilities-0.3.1/src/module_utilities/_doc.py` & `module-utilities-0.4.0/src/module_utilities/_doc.py`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.1/src/module_utilities/_docscrape.py` & `module-utilities-0.4.0/src/module_utilities/vendored/docscrape.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,21 @@
-# type: ignore
-# flake8: noqa
 """Extract reference documentation from the NumPy source tree.
+
 """
-import copy
 import inspect
-import pydoc
-import re
-import sys
 import textwrap
+import re
+import pydoc
+from warnings import warn
 from collections import namedtuple
 from collections.abc import Callable, Mapping
-from warnings import warn
+import copy
+import sys
 
-# TODO: Remove try-except when support for Python 3.7 is dropped
-try:
-    from functools import cached_property
-except ImportError:  # cached_property added in Python 3.8
-    cached_property = property
+from functools import cached_property
 
 
 def strip_blank_lines(l):
     "Remove leading and trailing blank lines from a list of lines"
     while l and not l[0].strip():
         del l[0]
     while l and not l[-1].strip():
@@ -33,14 +28,15 @@
 
     def __init__(self, data):
         """
         Parameters
         ----------
         data : str
            String with lines separated by '\\n'.
+
         """
         if isinstance(data, list):
             self._str = data
         else:
             self._str = data.split("\n")  # store string as list of lines
 
         self.reset()
@@ -112,15 +108,17 @@
 
 
 Parameter = namedtuple("Parameter", ["name", "type", "desc"])
 
 
 class NumpyDocString(Mapping):
     """Parses a numpydoc string to an abstract representation
+
     Instances define a mapping from section title to structured data.
+
     """
 
     sections = {
         "Signature": "",
         "Summary": [""],
         "Extended Summary": [],
         "Parameters": [],
@@ -292,14 +290,15 @@
 
     def _parse_see_also(self, content):
         """
         func_name : Descriptive text
             continued text
         another_func_name : Descriptive text
         func_name1, func_name2, :meth:`func_name`, func_name3
+
         """
 
         content = dedent_lines(content)
 
         items = []
 
         def parse_item_name(text):
@@ -345,14 +344,15 @@
                 self._error_location(f"Error parsing See Also entry {line!r}")
         return items
 
     def _parse_index(self, section, content):
         """
         .. index: default
            :refguide: something, else, and more
+
         """
 
         def strip_each_in(lst):
             return [s.strip() for s in lst]
 
         out = {}
         section = section.split("::")
@@ -718,28 +718,36 @@
         if self.show_inherited_members:
             return True  # show all class members
         if name not in self._cls.__dict__:
             return False  # class member is inherited, we do not show it
         return True
 
 
-def get_doc_object(obj, what=None, doc=None, config=None):
+def get_doc_object(
+    obj,
+    what=None,
+    doc=None,
+    config=None,
+    class_doc=ClassDoc,
+    func_doc=FunctionDoc,
+    obj_doc=ObjDoc,
+):
     if what is None:
         if inspect.isclass(obj):
             what = "class"
         elif inspect.ismodule(obj):
             what = "module"
         elif isinstance(obj, Callable):
             what = "function"
         else:
             what = "object"
     if config is None:
         config = {}
 
     if what == "class":
-        return ClassDoc(obj, func_doc=FunctionDoc, doc=doc, config=config)
+        return class_doc(obj, func_doc=func_doc, doc=doc, config=config)
     elif what in ("function", "method"):
-        return FunctionDoc(obj, doc=doc, config=config)
+        return func_doc(obj, doc=doc, config=config)
     else:
         if doc is None:
             doc = pydoc.getdoc(obj)
-        return ObjDoc(obj, doc, config=config)
+        return obj_doc(obj, doc, config=config)
```

### Comparing `module-utilities-0.3.1/src/module_utilities/attributedict.py` & `module-utilities-0.4.0/src/module_utilities/attributedict.py`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.1/src/module_utilities/cached.py` & `module-utilities-0.4.0/src/module_utilities/cached.py`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.1/src/module_utilities/docfiller.py` & `module-utilities-0.4.0/src/module_utilities/docfiller.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,19 @@
 import inspect
 import os
 from textwrap import dedent
 from typing import TYPE_CHECKING, Any, Callable
 
 from . import cached
 from ._doc import doc as _pd_doc
-from ._docscrape import NumpyDocString, Parameter  # type: ignore
 from .attributedict import AttributeDict
 
+# from ._docscrape import NumpyDocString, Parameter  # type: ignore
+from .vendored.docscrape import NumpyDocString, Parameter
+
 if TYPE_CHECKING:
     from collections.abc import Mapping, Sequence
 
     from ._typing import F
 
 try:
     # Default is DOC_SUB is True
```

### Comparing `module-utilities-0.3.1/src/module_utilities.egg-info/SOURCES.txt` & `module-utilities-0.4.0/src/module_utilities.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -9,17 +9,16 @@
 CHANGELOG.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 conftest.py
-environment.yaml
+noxfile.py
 pyproject.toml
-tox.ini
 .github/ISSUE_TEMPLATE.md
 changelog.d/README.txt
 changelog.d/templates/new_fragment.md.j2
 changelog.d/templates/auto-changelog/macros.jinja2
 changelog.d/templates/auto-changelog/template.jinja2
 docs/Makefile
 docs/authors.md
@@ -46,53 +45,51 @@
 docs/_templates/autodocsumm/class.rst
 docs/_templates/autodocsumm/module-inherit.rst
 docs/_templates/autodocsumm/module-noindex.rst
 docs/_templates/autodocsumm/module.rst
 docs/_templates/autosummary/base.rst
 docs/_templates/autosummary/class.rst
 docs/_templates/autosummary/module.rst
-docs/examples/example-usage-1.rst
-docs/examples/example-usage.md
 docs/examples/index.md
 docs/examples/usage/cached.ipynb
 docs/examples/usage/docfiller.ipynb
 docs/reference/index.md
-environment/dev-extras.yaml
+environment/base.yaml
 environment/dev.yaml
 environment/dist-conda.yaml
 environment/dist-pypi.yaml
-environment/docs-extras.yaml
 environment/docs.yaml
-environment/lint-extras.yaml
 environment/lint.yaml
+environment/test-extras.txt
 environment/test-extras.yaml
 environment/test.yaml
-environment/tools.yaml
+environment/typing.yaml
+environment/lock/py310.yaml
+environment/lock/py311.yaml
+environment/lock/py38.yaml
+environment/lock/py39.yaml
 examples/README.md
 examples/usage/cached.ipynb
 examples/usage/docfiller.ipynb
-scripts/dist-conda.mk
-scripts/dist-pypi.mk
-scripts/docs-examples-symlinks.sh
-scripts/lint.mk
-scripts/recipe-append.sh
-scripts/run-prettier.sh
-scripts/tox-ipykernel-display-name.sh
 src/module_utilities/__init__.py
 src/module_utilities/_doc.py
-src/module_utilities/_docscrape.py
 src/module_utilities/_typing.py
 src/module_utilities/attributedict.py
 src/module_utilities/cached.py
 src/module_utilities/docfiller.py
 src/module_utilities/py.typed
 src/module_utilities.egg-info/PKG-INFO
 src/module_utilities.egg-info/SOURCES.txt
 src/module_utilities.egg-info/dependency_links.txt
 src/module_utilities.egg-info/requires.txt
 src/module_utilities.egg-info/top_level.txt
 src/module_utilities.egg-info/zip-safe
+src/module_utilities/vendored/LICENSE.txt
+src/module_utilities/vendored/README.txt
+src/module_utilities/vendored/__init__.py
+src/module_utilities/vendored/docscrape.py
 tests/__init__.py
 tests/conftest.py
 tests/test_cached.py
 tests/test_docfiller.py
-tests/test_module_utilities.py
+tests/test_module_utilities.py
+tools/noxtools.py
```

### Comparing `module-utilities-0.3.1/tests/test_cached.py` & `module-utilities-0.4.0/tests/test_cached.py`

 * *Files identical despite different names*

### Comparing `module-utilities-0.3.1/tests/test_docfiller.py` & `module-utilities-0.4.0/tests/test_docfiller.py`

 * *Files identical despite different names*

