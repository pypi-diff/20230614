# Comparing `tmp/cmomy-0.4.0.tar.gz` & `tmp/cmomy-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmomy-0.4.0.tar", last modified: Tue May  2 05:03:51 2023, max compression
+gzip compressed data, was "cmomy-0.4.1.tar", last modified: Thu May  4 19:42:48 2023, max compression
```

## Comparing `cmomy-0.4.0.tar` & `cmomy-0.4.1.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.710538 cmomy-0.4.0/
--rw-r--r--   0 wpk      (42033)    36681     1475 2023-05-02 05:01:33.000000 cmomy-0.4.0/.cruft.json
--rw-r--r--   0 wpk      (42033)    36681      540 2023-05-02 04:51:37.000000 cmomy-0.4.0/.editorconfig
--rw-r--r--   0 wpk      (42033)    36681       31 2023-01-25 16:37:02.000000 cmomy-0.4.0/.gitattributes
--rw-r--r--   0 wpk      (42033)    36681     1324 2023-05-02 04:51:37.000000 cmomy-0.4.0/.gitignore
--rw-r--r--   0 wpk      (42033)    36681      161 2023-04-24 20:47:28.000000 cmomy-0.4.0/.markdownlint.yaml
--rw-r--r--   0 wpk      (42033)    36681     3651 2023-05-02 04:51:37.000000 cmomy-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 wpk      (42033)    36681       20 2023-04-24 20:47:28.000000 cmomy-0.4.0/.prettierrc.yaml
--rw-r--r--   0 wpk      (42033)    36681      122 2023-04-24 20:47:28.000000 cmomy-0.4.0/AUTHORS.md
--rw-r--r--   0 wpk      (42033)    36681     2667 2023-05-02 04:51:37.000000 cmomy-0.4.0/CHANGELOG.md
--rw-r--r--   0 wpk      (42033)    36681     9153 2023-05-02 04:51:37.000000 cmomy-0.4.0/CONTRIBUTING.md
--rw-r--r--   0 wpk      (42033)    36681     1645 2023-03-15 19:07:26.000000 cmomy-0.4.0/LICENSE
--rw-r--r--   0 wpk      (42033)    36681      258 2023-04-24 20:47:28.000000 cmomy-0.4.0/MANIFEST.in
--rw-r--r--   0 wpk      (42033)    36681    11187 2023-05-02 04:51:37.000000 cmomy-0.4.0/Makefile
--rw-r--r--   0 wpk      (42033)    36681     9851 2023-05-02 05:03:51.711032 cmomy-0.4.0/PKG-INFO
--rw-r--r--   0 wpk      (42033)    36681     4601 2023-05-02 04:51:37.000000 cmomy-0.4.0/README.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.613503 cmomy-0.4.0/changelog.d/
--rw-r--r--   0 wpk      (42033)    36681       64 2023-04-24 20:47:28.000000 cmomy-0.4.0/changelog.d/README.txt
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.614426 cmomy-0.4.0/changelog.d/templates/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.616035 cmomy-0.4.0/changelog.d/templates/auto-changelog/
--rw-r--r--   0 wpk      (42033)    36681      213 2023-04-24 20:47:28.000000 cmomy-0.4.0/changelog.d/templates/auto-changelog/macros.jinja2
--rw-r--r--   0 wpk      (42033)    36681      774 2023-04-24 20:47:28.000000 cmomy-0.4.0/changelog.d/templates/auto-changelog/template.jinja2
--rw-r--r--   0 wpk      (42033)    36681      269 2023-04-24 20:47:28.000000 cmomy-0.4.0/changelog.d/templates/new_fragment.md.j2
--rw-r--r--   0 wpk      (42033)    36681      366 2023-01-25 16:37:02.000000 cmomy-0.4.0/conftest.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.625606 cmomy-0.4.0/docs/
--rw-r--r--   0 wpk      (42033)    36681     1401 2023-05-02 05:02:56.000000 cmomy-0.4.0/docs/Makefile
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.597134 cmomy-0.4.0/docs/_static/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.627106 cmomy-0.4.0/docs/_static/css/
--rw-r--r--   0 wpk      (42033)    36681     2937 2023-04-24 20:47:28.000000 cmomy-0.4.0/docs/_static/css/nist-combined.css
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.629581 cmomy-0.4.0/docs/_static/js/
--rw-r--r--   0 wpk      (42033)    36681      767 2023-04-24 20:47:28.000000 cmomy-0.4.0/docs/_static/js/leave_notice.js
--rw-r--r--   0 wpk      (42033)    36681      706 2023-04-24 20:47:28.000000 cmomy-0.4.0/docs/_static/js/nist-header-footer.js
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.633907 cmomy-0.4.0/docs/_templates/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.639177 cmomy-0.4.0/docs/_templates/autodocsumm/
--rw-r--r--   0 wpk      (42033)    36681      289 2023-03-22 20:26:04.000000 cmomy-0.4.0/docs/_templates/autodocsumm/class-noindex.rst
--rw-r--r--   0 wpk      (42033)    36681      249 2023-03-22 20:26:04.000000 cmomy-0.4.0/docs/_templates/autodocsumm/class.rst
--rw-r--r--   0 wpk      (42033)    36681      405 2023-03-22 20:26:04.000000 cmomy-0.4.0/docs/_templates/autodocsumm/module-inherit.rst
--rw-r--r--   0 wpk      (42033)    36681      424 2023-03-22 20:26:04.000000 cmomy-0.4.0/docs/_templates/autodocsumm/module-noindex.rst
--rw-r--r--   0 wpk      (42033)    36681      374 2023-03-22 20:26:04.000000 cmomy-0.4.0/docs/_templates/autodocsumm/module.rst
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.641878 cmomy-0.4.0/docs/_templates/autosummary/
--rw-r--r--   0 wpk      (42033)    36681      106 2023-03-22 20:26:04.000000 cmomy-0.4.0/docs/_templates/autosummary/base.rst
--rw-r--r--   0 wpk      (42033)    36681     1255 2023-03-22 20:26:04.000000 cmomy-0.4.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 wpk      (42033)    36681     1119 2023-03-22 20:26:04.000000 cmomy-0.4.0/docs/_templates/autosummary/module.rst
--rw-r--r--   0 wpk      (42033)    36681     1418 2023-03-22 20:26:04.000000 cmomy-0.4.0/docs/_templates/class-individual-pages.rst
--rw-r--r--   0 wpk      (42033)    36681     1177 2023-03-22 20:26:04.000000 cmomy-0.4.0/docs/_templates/module-custom.rst
--rw-r--r--   0 wpk      (42033)    36681     1071 2023-03-22 20:26:04.000000 cmomy-0.4.0/docs/_templates/module-single.rst
--rw-r--r--   0 wpk      (42033)    36681     1179 2023-03-22 20:26:04.000000 cmomy-0.4.0/docs/_templates/module-template.rst
--rw-r--r--   0 wpk      (42033)    36681       69 2023-04-24 20:47:28.000000 cmomy-0.4.0/docs/authors.md
--rw-r--r--   0 wpk      (42033)    36681       71 2023-04-24 20:47:28.000000 cmomy-0.4.0/docs/changelog.md
--rw-r--r--   0 wpk      (42033)    36681    14595 2023-05-02 04:51:37.000000 cmomy-0.4.0/docs/conf.py
--rw-r--r--   0 wpk      (42033)    36681       74 2023-04-24 20:47:28.000000 cmomy-0.4.0/docs/contributing.md
--rw-r--r--   0 wpk      (42033)    36681      891 2023-04-24 20:47:28.000000 cmomy-0.4.0/docs/example_for_readme.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.644531 cmomy-0.4.0/docs/examples/
--rw-r--r--   0 wpk      (42033)    36681      887 2023-04-24 20:47:28.000000 cmomy-0.4.0/docs/examples/create-symlinks.sh
--rw-r--r--   0 wpk      (42033)    36681       84 2023-04-24 20:47:28.000000 cmomy-0.4.0/docs/examples/index.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.647120 cmomy-0.4.0/docs/examples/usage/
--rw-r--r--   0 wpk      (42033)    36681   156774 2023-04-24 20:47:28.000000 cmomy-0.4.0/docs/examples/usage/motivation.ipynb
--rw-r--r--   0 wpk      (42033)    36681   295212 2023-04-24 20:47:28.000000 cmomy-0.4.0/docs/examples/usage/usage_notebook.ipynb
--rw-r--r--   0 wpk      (42033)    36681      224 2023-04-24 20:47:28.000000 cmomy-0.4.0/docs/index.md
--rw-r--r--   0 wpk      (42033)    36681      860 2023-04-24 20:47:28.000000 cmomy-0.4.0/docs/installation.md
--rw-r--r--   0 wpk      (42033)    36681       40 2023-04-24 20:47:28.000000 cmomy-0.4.0/docs/license.md
--rw-r--r--   0 wpk      (42033)    36681      767 2023-03-15 18:41:43.000000 cmomy-0.4.0/docs/make.bat
--rw-r--r--   0 wpk      (42033)    36681      169 2023-04-24 20:47:28.000000 cmomy-0.4.0/docs/navigation.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.651859 cmomy-0.4.0/docs/reference/
--rw-r--r--   0 wpk      (42033)    36681      158 2023-04-06 00:58:31.000000 cmomy-0.4.0/docs/reference/api-baseclasses.rst
--rw-r--r--   0 wpk      (42033)    36681      122 2023-04-06 00:58:31.000000 cmomy-0.4.0/docs/reference/api-modules.rst
--rw-r--r--   0 wpk      (42033)    36681      398 2023-04-06 00:58:31.000000 cmomy-0.4.0/docs/reference/api-public.rst
--rw-r--r--   0 wpk      (42033)    36681      194 2023-04-24 20:47:28.000000 cmomy-0.4.0/docs/reference/index.md
--rw-r--r--   0 wpk      (42033)    36681      491 2023-04-21 20:37:24.000000 cmomy-0.4.0/docs/spelling_wordlist.txt
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.663443 cmomy-0.4.0/environment/
--rw-r--r--   0 wpk      (42033)    36681      967 2023-04-24 20:47:28.000000 cmomy-0.4.0/environment/dev-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      310 2023-05-02 04:51:37.000000 cmomy-0.4.0/environment/dev.yaml
--rw-r--r--   0 wpk      (42033)    36681      108 2023-04-24 20:47:28.000000 cmomy-0.4.0/environment/dist-conda.yaml
--rw-r--r--   0 wpk      (42033)    36681       79 2023-04-24 20:47:28.000000 cmomy-0.4.0/environment/dist-pypi.yaml
--rw-r--r--   0 wpk      (42033)    36681      640 2023-04-24 20:47:28.000000 cmomy-0.4.0/environment/docs-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      463 2023-05-02 04:51:37.000000 cmomy-0.4.0/environment/docs.yaml
--rw-r--r--   0 wpk      (42033)    36681       53 2023-04-24 20:47:28.000000 cmomy-0.4.0/environment/lint-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      203 2023-05-02 04:51:37.000000 cmomy-0.4.0/environment/lint.yaml
--rw-r--r--   0 wpk      (42033)    36681       25 2023-04-24 20:47:28.000000 cmomy-0.4.0/environment/test-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      194 2023-05-02 04:51:37.000000 cmomy-0.4.0/environment/test.yaml
--rw-r--r--   0 wpk      (42033)    36681      299 2023-04-24 20:47:28.000000 cmomy-0.4.0/environment/tools.yaml
--rw-r--r--   0 wpk      (42033)    36681      187 2023-05-02 04:51:37.000000 cmomy-0.4.0/environment.yaml
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.664364 cmomy-0.4.0/examples/
--rw-r--r--   0 wpk      (42033)    36681      222 2023-04-24 20:47:28.000000 cmomy-0.4.0/examples/README.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.670757 cmomy-0.4.0/examples/archived/
--rw-r--r--   0 wpk      (42033)    36681    70967 2023-04-24 20:47:28.000000 cmomy-0.4.0/examples/archived/bootstrap.ipynb
--rw-r--r--   0 wpk      (42033)    36681   136974 2023-04-24 20:47:28.000000 cmomy-0.4.0/examples/archived/central_moments.ipynb
--rw-r--r--   0 wpk      (42033)    36681    44856 2023-04-24 20:47:28.000000 cmomy-0.4.0/examples/archived/example_usage.ipynb
--rw-r--r--   0 wpk      (42033)    36681    12217 2023-04-24 20:47:28.000000 cmomy-0.4.0/examples/archived/parallel_test.ipynb
--rw-r--r--   0 wpk      (42033)    36681    58117 2023-04-24 20:47:28.000000 cmomy-0.4.0/examples/archived/test_accumulator.ipynb
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.673055 cmomy-0.4.0/examples/usage/
--rw-r--r--   0 wpk      (42033)    36681   156774 2023-04-24 20:47:28.000000 cmomy-0.4.0/examples/usage/motivation.ipynb
--rw-r--r--   0 wpk      (42033)    36681   295212 2023-04-24 20:47:28.000000 cmomy-0.4.0/examples/usage/usage_notebook.ipynb
--rw-r--r--   0 wpk      (42033)    36681     6118 2023-05-02 04:51:37.000000 cmomy-0.4.0/pyproject.toml
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.678736 cmomy-0.4.0/scripts/
--rw-r--r--   0 wpk      (42033)    36681      392 2023-05-02 04:51:37.000000 cmomy-0.4.0/scripts/dist-conda.mk
--rw-r--r--   0 wpk      (42033)    36681      312 2023-05-02 04:51:37.000000 cmomy-0.4.0/scripts/dist-pypi.mk
--rw-r--r--   0 wpk      (42033)    36681     1099 2023-04-24 20:47:28.000000 cmomy-0.4.0/scripts/docs-examples-symlinks.sh
--rw-r--r--   0 wpk      (42033)    36681      266 2023-05-02 04:51:37.000000 cmomy-0.4.0/scripts/lint.mk
--rw-r--r--   0 wpk      (42033)    36681       91 2023-05-02 04:51:37.000000 cmomy-0.4.0/scripts/run-prettier.sh
--rw-r--r--   0 wpk      (42033)    36681      489 2023-04-24 20:47:28.000000 cmomy-0.4.0/scripts/tox-ipykernel-display-name.sh
--rw-r--r--   0 wpk      (42033)    36681      286 2023-05-02 05:03:51.712585 cmomy-0.4.0/setup.cfg
--rw-r--r--   0 wpk      (42033)    36681      323 2023-04-24 20:47:28.000000 cmomy-0.4.0/setup.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.600818 cmomy-0.4.0/src/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.694921 cmomy-0.4.0/src/cmomy/
--rw-r--r--   0 wpk      (42033)    36681     1045 2023-03-29 00:12:57.000000 cmomy-0.4.0/src/cmomy/__init__.py
--rw-r--r--   0 wpk      (42033)    36681     2736 2023-04-24 20:47:28.000000 cmomy-0.4.0/src/cmomy/_formatting.py
--rw-r--r--   0 wpk      (42033)    36681     6463 2023-03-22 20:26:04.000000 cmomy-0.4.0/src/cmomy/_resample.py
--rw-r--r--   0 wpk      (42033)    36681     2311 2023-01-25 16:37:02.000000 cmomy-0.4.0/src/cmomy/_testing.py
--rw-r--r--   0 wpk      (42033)    36681      658 2023-03-22 20:26:04.000000 cmomy-0.4.0/src/cmomy/_typing.py
--rw-r--r--   0 wpk      (42033)    36681    39729 2023-05-02 04:51:37.000000 cmomy-0.4.0/src/cmomy/abstract_central.py
--rw-r--r--   0 wpk      (42033)    36681    51582 2023-05-02 04:51:37.000000 cmomy-0.4.0/src/cmomy/central.py
--rw-r--r--   0 wpk      (42033)    36681      967 2023-01-25 16:37:02.000000 cmomy-0.4.0/src/cmomy/compile.py
--rw-r--r--   0 wpk      (42033)    36681    10920 2023-05-02 04:51:37.000000 cmomy-0.4.0/src/cmomy/convert.py
--rw-r--r--   0 wpk      (42033)    36681     3338 2023-05-02 04:51:37.000000 cmomy-0.4.0/src/cmomy/docstrings.py
--rw-r--r--   0 wpk      (42033)    36681     1834 2023-04-06 00:58:31.000000 cmomy-0.4.0/src/cmomy/options.py
--rw-r--r--   0 wpk      (42033)    36681     3122 2023-04-06 00:58:31.000000 cmomy-0.4.0/src/cmomy/pusher_interface.py
--rw-r--r--   0 wpk      (42033)    36681    14250 2023-01-25 16:37:02.000000 cmomy-0.4.0/src/cmomy/pushers.py
--rw-r--r--   0 wpk      (42033)    36681        0 2023-03-22 20:26:04.000000 cmomy-0.4.0/src/cmomy/py.typed
--rw-r--r--   0 wpk      (42033)    36681    13795 2023-04-24 20:47:28.000000 cmomy-0.4.0/src/cmomy/resample.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.709666 cmomy-0.4.0/src/cmomy/tests/
--rw-r--r--   0 wpk      (42033)    36681        0 2023-01-25 16:37:02.000000 cmomy-0.4.0/src/cmomy/tests/__init__.py
--rw-r--r--   0 wpk      (42033)    36681    11913 2023-05-02 04:51:37.000000 cmomy-0.4.0/src/cmomy/tests/conftest.py
--rw-r--r--   0 wpk      (42033)    36681     5427 2023-03-22 20:26:04.000000 cmomy-0.4.0/src/cmomy/tests/test_central.py
--rw-r--r--   0 wpk      (42033)    36681     9455 2023-05-02 04:51:37.000000 cmomy-0.4.0/src/cmomy/tests/test_central_2.py
--rw-r--r--   0 wpk      (42033)    36681     1085 2023-01-25 16:37:02.000000 cmomy-0.4.0/src/cmomy/tests/test_convert.py
--rw-r--r--   0 wpk      (42033)    36681     4085 2023-03-22 20:26:04.000000 cmomy-0.4.0/src/cmomy/tests/test_resample.py
--rw-r--r--   0 wpk      (42033)    36681     2354 2023-03-22 20:26:04.000000 cmomy-0.4.0/src/cmomy/tests/test_stability.py
--rw-r--r--   0 wpk      (42033)    36681     2682 2023-03-22 20:26:04.000000 cmomy-0.4.0/src/cmomy/tests/test_verify.py
--rw-r--r--   0 wpk      (42033)    36681     6183 2023-03-22 20:26:04.000000 cmomy-0.4.0/src/cmomy/tests/test_xcentral.py
--rw-r--r--   0 wpk      (42033)    36681     4879 2023-03-22 20:26:04.000000 cmomy-0.4.0/src/cmomy/tests/test_xcentral_constructors.py
--rw-r--r--   0 wpk      (42033)    36681     3190 2023-05-02 04:51:37.000000 cmomy-0.4.0/src/cmomy/utils.py
--rw-r--r--   0 wpk      (42033)    36681    62294 2023-05-02 04:51:37.000000 cmomy-0.4.0/src/cmomy/xcentral.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.700780 cmomy-0.4.0/src/cmomy.egg-info/
--rw-r--r--   0 wpk      (42033)    36681     9851 2023-05-02 05:03:51.000000 cmomy-0.4.0/src/cmomy.egg-info/PKG-INFO
--rw-r--r--   0 wpk      (42033)    36681     3110 2023-05-02 05:03:51.000000 cmomy-0.4.0/src/cmomy.egg-info/SOURCES.txt
--rw-r--r--   0 wpk      (42033)    36681        1 2023-05-02 05:03:51.000000 cmomy-0.4.0/src/cmomy.egg-info/dependency_links.txt
--rw-r--r--   0 wpk      (42033)    36681        1 2023-04-06 00:42:47.000000 cmomy-0.4.0/src/cmomy.egg-info/not-zip-safe
--rw-r--r--   0 wpk      (42033)    36681      113 2023-05-02 05:03:51.000000 cmomy-0.4.0/src/cmomy.egg-info/requires.txt
--rw-r--r--   0 wpk      (42033)    36681        6 2023-05-02 05:03:51.000000 cmomy-0.4.0/src/cmomy.egg-info/top_level.txt
--rw-r--r--   0 wpk      (42033)    36681     3704 2023-05-02 04:51:37.000000 cmomy-0.4.0/tox.ini
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:42:48.496295 cmomy-0.4.1/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1486 2023-05-04 19:41:42.000000 cmomy-0.4.1/.cruft.json
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      540 2023-05-02 04:51:37.000000 cmomy-0.4.1/.editorconfig
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       31 2023-01-25 16:37:02.000000 cmomy-0.4.1/.gitattributes
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1324 2023-05-02 04:51:37.000000 cmomy-0.4.1/.gitignore
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      161 2023-04-24 20:47:28.000000 cmomy-0.4.1/.markdownlint.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3651 2023-05-02 04:51:37.000000 cmomy-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       20 2023-04-24 20:47:28.000000 cmomy-0.4.1/.prettierrc.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      613 2023-05-04 19:41:42.000000 cmomy-0.4.1/.recipe-append.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      122 2023-04-24 20:47:28.000000 cmomy-0.4.1/AUTHORS.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2667 2023-05-02 04:51:37.000000 cmomy-0.4.1/CHANGELOG.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9638 2023-05-04 19:41:42.000000 cmomy-0.4.1/CONTRIBUTING.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1645 2023-03-15 19:07:26.000000 cmomy-0.4.1/LICENSE
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      258 2023-04-24 20:47:28.000000 cmomy-0.4.1/MANIFEST.in
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    11323 2023-05-04 19:41:42.000000 cmomy-0.4.1/Makefile
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9800 2023-05-04 19:42:48.495149 cmomy-0.4.1/PKG-INFO
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4601 2023-05-02 04:51:37.000000 cmomy-0.4.1/README.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:42:48.374626 cmomy-0.4.1/changelog.d/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       64 2023-04-24 20:47:28.000000 cmomy-0.4.1/changelog.d/README.txt
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:42:48.375521 cmomy-0.4.1/changelog.d/templates/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:42:48.376721 cmomy-0.4.1/changelog.d/templates/auto-changelog/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      213 2023-04-24 20:47:28.000000 cmomy-0.4.1/changelog.d/templates/auto-changelog/macros.jinja2
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      774 2023-04-24 20:47:28.000000 cmomy-0.4.1/changelog.d/templates/auto-changelog/template.jinja2
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      269 2023-04-24 20:47:28.000000 cmomy-0.4.1/changelog.d/templates/new_fragment.md.j2
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      366 2023-01-25 16:37:02.000000 cmomy-0.4.1/conftest.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:42:48.385002 cmomy-0.4.1/docs/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1401 2023-05-02 13:41:37.000000 cmomy-0.4.1/docs/Makefile
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:42:48.355456 cmomy-0.4.1/docs/_static/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:42:48.385979 cmomy-0.4.1/docs/_static/css/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2937 2023-04-24 20:47:28.000000 cmomy-0.4.1/docs/_static/css/nist-combined.css
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:42:48.387533 cmomy-0.4.1/docs/_static/js/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      767 2023-04-24 20:47:28.000000 cmomy-0.4.1/docs/_static/js/leave_notice.js
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      706 2023-04-24 20:47:28.000000 cmomy-0.4.1/docs/_static/js/nist-header-footer.js
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:42:48.391390 cmomy-0.4.1/docs/_templates/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:42:48.396999 cmomy-0.4.1/docs/_templates/autodocsumm/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      289 2023-03-22 20:26:04.000000 cmomy-0.4.1/docs/_templates/autodocsumm/class-noindex.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      249 2023-03-22 20:26:04.000000 cmomy-0.4.1/docs/_templates/autodocsumm/class.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      405 2023-03-22 20:26:04.000000 cmomy-0.4.1/docs/_templates/autodocsumm/module-inherit.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      424 2023-03-22 20:26:04.000000 cmomy-0.4.1/docs/_templates/autodocsumm/module-noindex.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      374 2023-03-22 20:26:04.000000 cmomy-0.4.1/docs/_templates/autodocsumm/module.rst
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:42:48.400845 cmomy-0.4.1/docs/_templates/autosummary/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      106 2023-03-22 20:26:04.000000 cmomy-0.4.1/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1255 2023-03-22 20:26:04.000000 cmomy-0.4.1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1119 2023-03-22 20:26:04.000000 cmomy-0.4.1/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1418 2023-03-22 20:26:04.000000 cmomy-0.4.1/docs/_templates/class-individual-pages.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1177 2023-03-22 20:26:04.000000 cmomy-0.4.1/docs/_templates/module-custom.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1071 2023-03-22 20:26:04.000000 cmomy-0.4.1/docs/_templates/module-single.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1179 2023-03-22 20:26:04.000000 cmomy-0.4.1/docs/_templates/module-template.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       69 2023-04-24 20:47:28.000000 cmomy-0.4.1/docs/authors.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       71 2023-04-24 20:47:28.000000 cmomy-0.4.1/docs/changelog.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    14595 2023-05-02 04:51:37.000000 cmomy-0.4.1/docs/conf.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       74 2023-04-24 20:47:28.000000 cmomy-0.4.1/docs/contributing.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      891 2023-04-24 20:47:28.000000 cmomy-0.4.1/docs/example_for_readme.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:42:48.401818 cmomy-0.4.1/docs/examples/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       84 2023-04-24 20:47:28.000000 cmomy-0.4.1/docs/examples/index.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:42:48.405936 cmomy-0.4.1/docs/examples/usage/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)   156774 2023-04-24 20:47:28.000000 cmomy-0.4.1/docs/examples/usage/motivation.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)   295212 2023-04-24 20:47:28.000000 cmomy-0.4.1/docs/examples/usage/usage_notebook.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      224 2023-04-24 20:47:28.000000 cmomy-0.4.1/docs/index.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      860 2023-04-24 20:47:28.000000 cmomy-0.4.1/docs/installation.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       40 2023-04-24 20:47:28.000000 cmomy-0.4.1/docs/license.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      767 2023-03-15 18:41:43.000000 cmomy-0.4.1/docs/make.bat
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      169 2023-04-24 20:47:28.000000 cmomy-0.4.1/docs/navigation.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:42:48.413065 cmomy-0.4.1/docs/reference/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      158 2023-04-06 00:58:31.000000 cmomy-0.4.1/docs/reference/api-baseclasses.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      122 2023-04-06 00:58:31.000000 cmomy-0.4.1/docs/reference/api-modules.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      398 2023-04-06 00:58:31.000000 cmomy-0.4.1/docs/reference/api-public.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      194 2023-04-24 20:47:28.000000 cmomy-0.4.1/docs/reference/index.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      491 2023-04-21 20:37:24.000000 cmomy-0.4.1/docs/spelling_wordlist.txt
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:42:48.423174 cmomy-0.4.1/environment/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      967 2023-04-24 20:47:28.000000 cmomy-0.4.1/environment/dev-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      310 2023-05-02 04:51:37.000000 cmomy-0.4.1/environment/dev.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      108 2023-04-24 20:47:28.000000 cmomy-0.4.1/environment/dist-conda.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       79 2023-04-24 20:47:28.000000 cmomy-0.4.1/environment/dist-pypi.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      640 2023-04-24 20:47:28.000000 cmomy-0.4.1/environment/docs-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      463 2023-05-02 04:51:37.000000 cmomy-0.4.1/environment/docs.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       53 2023-04-24 20:47:28.000000 cmomy-0.4.1/environment/lint-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      203 2023-05-02 04:51:37.000000 cmomy-0.4.1/environment/lint.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       25 2023-04-24 20:47:28.000000 cmomy-0.4.1/environment/test-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      194 2023-05-02 04:51:37.000000 cmomy-0.4.1/environment/test.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      299 2023-04-24 20:47:28.000000 cmomy-0.4.1/environment/tools.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      187 2023-05-02 04:51:37.000000 cmomy-0.4.1/environment.yaml
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:42:48.424195 cmomy-0.4.1/examples/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      222 2023-04-24 20:47:28.000000 cmomy-0.4.1/examples/README.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:42:48.432724 cmomy-0.4.1/examples/archived/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    70967 2023-04-24 20:47:28.000000 cmomy-0.4.1/examples/archived/bootstrap.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)   136974 2023-04-24 20:47:28.000000 cmomy-0.4.1/examples/archived/central_moments.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    44856 2023-04-24 20:47:28.000000 cmomy-0.4.1/examples/archived/example_usage.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    12217 2023-04-24 20:47:28.000000 cmomy-0.4.1/examples/archived/parallel_test.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    58117 2023-04-24 20:47:28.000000 cmomy-0.4.1/examples/archived/test_accumulator.ipynb
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:42:48.435072 cmomy-0.4.1/examples/usage/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)   156774 2023-04-24 20:47:28.000000 cmomy-0.4.1/examples/usage/motivation.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)   295212 2023-04-24 20:47:28.000000 cmomy-0.4.1/examples/usage/usage_notebook.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     6063 2023-05-04 19:41:42.000000 cmomy-0.4.1/pyproject.toml
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:42:48.442947 cmomy-0.4.1/scripts/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      836 2023-05-04 19:41:42.000000 cmomy-0.4.1/scripts/dist-conda.mk
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      312 2023-05-02 04:51:37.000000 cmomy-0.4.1/scripts/dist-pypi.mk
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1099 2023-04-24 20:47:28.000000 cmomy-0.4.1/scripts/docs-examples-symlinks.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      266 2023-05-02 04:51:37.000000 cmomy-0.4.1/scripts/lint.mk
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      598 2023-05-04 19:41:42.000000 cmomy-0.4.1/scripts/recipe-append.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       91 2023-05-02 04:51:37.000000 cmomy-0.4.1/scripts/run-prettier.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      489 2023-04-24 20:47:28.000000 cmomy-0.4.1/scripts/tox-ipykernel-display-name.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       38 2023-05-04 19:42:48.496464 cmomy-0.4.1/setup.cfg
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:42:48.359849 cmomy-0.4.1/src/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:42:48.472679 cmomy-0.4.1/src/cmomy/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1045 2023-03-29 00:12:57.000000 cmomy-0.4.1/src/cmomy/__init__.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2736 2023-04-24 20:47:28.000000 cmomy-0.4.1/src/cmomy/_formatting.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     6463 2023-03-22 20:26:04.000000 cmomy-0.4.1/src/cmomy/_resample.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2311 2023-01-25 16:37:02.000000 cmomy-0.4.1/src/cmomy/_testing.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      658 2023-03-22 20:26:04.000000 cmomy-0.4.1/src/cmomy/_typing.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    39729 2023-05-02 04:51:37.000000 cmomy-0.4.1/src/cmomy/abstract_central.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    51582 2023-05-02 04:51:37.000000 cmomy-0.4.1/src/cmomy/central.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      967 2023-01-25 16:37:02.000000 cmomy-0.4.1/src/cmomy/compile.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    10920 2023-05-02 04:51:37.000000 cmomy-0.4.1/src/cmomy/convert.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3338 2023-05-02 04:51:37.000000 cmomy-0.4.1/src/cmomy/docstrings.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1834 2023-04-06 00:58:31.000000 cmomy-0.4.1/src/cmomy/options.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3122 2023-04-06 00:58:31.000000 cmomy-0.4.1/src/cmomy/pusher_interface.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    14250 2023-01-25 16:37:02.000000 cmomy-0.4.1/src/cmomy/pushers.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-03-22 20:26:04.000000 cmomy-0.4.1/src/cmomy/py.typed
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    13795 2023-04-24 20:47:28.000000 cmomy-0.4.1/src/cmomy/resample.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:42:48.493964 cmomy-0.4.1/src/cmomy/tests/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-01-25 16:37:02.000000 cmomy-0.4.1/src/cmomy/tests/__init__.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    11913 2023-05-02 04:51:37.000000 cmomy-0.4.1/src/cmomy/tests/conftest.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5427 2023-03-22 20:26:04.000000 cmomy-0.4.1/src/cmomy/tests/test_central.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9455 2023-05-02 04:51:37.000000 cmomy-0.4.1/src/cmomy/tests/test_central_2.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1085 2023-01-25 16:37:02.000000 cmomy-0.4.1/src/cmomy/tests/test_convert.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4085 2023-03-22 20:26:04.000000 cmomy-0.4.1/src/cmomy/tests/test_resample.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2354 2023-03-22 20:26:04.000000 cmomy-0.4.1/src/cmomy/tests/test_stability.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2682 2023-03-22 20:26:04.000000 cmomy-0.4.1/src/cmomy/tests/test_verify.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     6183 2023-03-22 20:26:04.000000 cmomy-0.4.1/src/cmomy/tests/test_xcentral.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4879 2023-03-22 20:26:04.000000 cmomy-0.4.1/src/cmomy/tests/test_xcentral_constructors.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3190 2023-05-02 04:51:37.000000 cmomy-0.4.1/src/cmomy/utils.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    62294 2023-05-02 04:51:37.000000 cmomy-0.4.1/src/cmomy/xcentral.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:42:48.480702 cmomy-0.4.1/src/cmomy.egg-info/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9800 2023-05-04 19:42:48.000000 cmomy-0.4.1/src/cmomy.egg-info/PKG-INFO
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3099 2023-05-04 19:42:48.000000 cmomy-0.4.1/src/cmomy.egg-info/SOURCES.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-05-04 19:42:48.000000 cmomy-0.4.1/src/cmomy.egg-info/dependency_links.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      113 2023-05-04 19:42:48.000000 cmomy-0.4.1/src/cmomy.egg-info/requires.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        6 2023-05-04 19:42:48.000000 cmomy-0.4.1/src/cmomy.egg-info/top_level.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-05-04 19:42:47.000000 cmomy-0.4.1/src/cmomy.egg-info/zip-safe
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3940 2023-05-04 19:41:42.000000 cmomy-0.4.1/tox.ini
```

### Comparing `cmomy-0.4.0/.cruft.json` & `cmomy-0.4.1/.cruft.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9162280701754386%*

 * *Differences: {"'commit'": "'10a9fe1a4f0b341184e41953433c344020f92c72'",*

 * * "'context'": "{'cookiecutter': {'_copy_without_render': {insert: [(6, "*

 * *              "'changelog.d/templates/*.j2'), (7, "*

 * *              "'changelog.d/templates/auto-changelog/*.jinja2')], delete: [7, 6]}}}"}*

```diff
@@ -1,21 +1,21 @@
 {
     "checkout": "feature/markdown",
-    "commit": "38e14cd6d21fdc444081dcb1e34c15d0ebdc3683",
+    "commit": "10a9fe1a4f0b341184e41953433c344020f92c72",
     "context": {
         "cookiecutter": {
             "_copy_without_render": [
                 "*.html",
                 "docs/_templates/*.rst",
                 "docs/_templates/autosummary/*.rst",
                 "docs/_templates/autodocsumm/*.rst",
                 "docs/_static/css/*",
                 "docs/_static/js/*",
-                "changelog.d/templates/*",
-                "changelog.d/templates/auto-changlog/*"
+                "changelog.d/templates/*.j2",
+                "changelog.d/templates/auto-changelog/*.jinja2"
             ],
             "_template": "https://github.com/wpk-nist-gov/cookiecutter-pypackage.git",
             "command_line_interface": "No command-line interface",
             "conda_channel": "wpk-nist",
             "create_author_file": "y",
             "email": "wpk@nist.gov",
             "full_name": "William P. Krekelberg",
```

### Comparing `cmomy-0.4.0/.editorconfig` & `cmomy-0.4.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/.gitignore` & `cmomy-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/.pre-commit-config.yaml` & `cmomy-0.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/CHANGELOG.md` & `cmomy-0.4.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/CONTRIBUTING.md` & `cmomy-0.4.1/CONTRIBUTING.md`

 * *Files 6% similar despite different names*

```diff
@@ -384,7 +384,18 @@
 
 [setuptools_scm]: https://github.com/pypa/setuptools_scm
 
 Versioning is handled with [setuptools_scm].The pacakge version is set by the
 git tag. For convenience, you can override the version in the makefile (calling
 tox) by setting `version=v{major}.{minor}.{micro}`. This is useful for updating
 the docs, etc.
+
+## Creating conda recipe
+
+[grayskull]: https://github.com/conda/grayskull
+
+For the most part, we use [grayskull] to create the conda recipe. However, I've
+had issues getting it to play nice with `pyproject.toml` for some of the 'extra'
+variables. So, we use grayskull to build the majority of the recipe, and append
+the file `.recipe-append.yaml`. For some edge cases (install name different from
+package name, etc), you'll need to manually edit this file to create the final
+recipe.
```

### Comparing `cmomy-0.4.0/LICENSE` & `cmomy-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/Makefile` & `cmomy-0.4.1/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -275,15 +275,15 @@
 dist-conda-build dist-conda-recipe dist-conda-command: environment/dist-conda.yaml
 
 
 ## test distribution
 .PHONY: testdist-pypi-remote testdist-conda-remote testdist-pypi-local testdist-conda-local
 
 py?=310
-testdist-pypi-remote: ## test pypi install, can run as `make test-dist-pypi-remote py=39` to run test-dist-pypi-local-py39
+testdist-pypi-remote: ## testdist-pypi-remote: ## test pypi install, can run as `make test-dist-pypi-remote py=39` to run test-dist-pypi-local-py39.  Can specify version setting, eg,  TEST_VERSION='==0.1.0'.  Note that the the format should be '=={version}'.
 	$(TOX) -e $@-py$(py) -- $(posargs)
 testdist-conda-remote: ## test conda install, can run as `make test-dist-conda-remote py=39` to run test-dist-conda-local-py39
 	$(TOX) -e $@-py$(py) -- $(poasargs)
 testdist-pypi-local: ## test pypi install, can run as `make test-dist-pypi-local py=39` to run test-dist-pypi-local-py39
 	$(TOX) -e $@-py$(py) -- $(posargs)
 testdist-conda-local: ## test conda install, can run as `make test-dist-conda-local py=39` to run test-dist-conda-local-py39
 	$(TOX) -e $@-py$(py) -- $(poasargs)
```

### Comparing `cmomy-0.4.0/PKG-INFO` & `cmomy-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: cmomy
-Version: 0.4.0
+Version: 0.4.1
 Summary: Central (co)moment calculation/manipulation
-Home-page: https://github.com/usnistgov/cmomy
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
-License: NIST license
+License: NIST-PD
 Project-URL: homepage, https://github.com/usnistgov/cmomy
 Project-URL: documentation, https://pages.nist.gov/cmomy/
 Keywords: cmomy
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
```

### Comparing `cmomy-0.4.0/README.md` & `cmomy-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/changelog.d/templates/auto-changelog/template.jinja2` & `cmomy-0.4.1/changelog.d/templates/auto-changelog/template.jinja2`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/docs/Makefile` & `cmomy-0.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/docs/_static/css/nist-combined.css` & `cmomy-0.4.1/docs/_static/css/nist-combined.css`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/docs/_static/js/leave_notice.js` & `cmomy-0.4.1/docs/_static/js/leave_notice.js`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/docs/_static/js/nist-header-footer.js` & `cmomy-0.4.1/docs/_static/js/nist-header-footer.js`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/docs/_templates/autosummary/class.rst` & `cmomy-0.4.1/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/docs/_templates/autosummary/module.rst` & `cmomy-0.4.1/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/docs/_templates/class-individual-pages.rst` & `cmomy-0.4.1/docs/_templates/class-individual-pages.rst`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/docs/_templates/module-custom.rst` & `cmomy-0.4.1/docs/_templates/module-custom.rst`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/docs/_templates/module-single.rst` & `cmomy-0.4.1/docs/_templates/module-single.rst`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/docs/_templates/module-template.rst` & `cmomy-0.4.1/docs/_templates/module-template.rst`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/docs/conf.py` & `cmomy-0.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/docs/example_for_readme.md` & `cmomy-0.4.1/docs/example_for_readme.md`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/docs/examples/usage/motivation.ipynb` & `cmomy-0.4.1/docs/examples/usage/motivation.ipynb`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/docs/examples/usage/usage_notebook.ipynb` & `cmomy-0.4.1/docs/examples/usage/usage_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/docs/installation.md` & `cmomy-0.4.1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/docs/make.bat` & `cmomy-0.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/environment/dev-extras.yaml` & `cmomy-0.4.1/environment/dev-extras.yaml`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/environment/docs-extras.yaml` & `cmomy-0.4.1/environment/docs-extras.yaml`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/examples/archived/bootstrap.ipynb` & `cmomy-0.4.1/examples/archived/bootstrap.ipynb`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/examples/archived/central_moments.ipynb` & `cmomy-0.4.1/examples/archived/central_moments.ipynb`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/examples/archived/example_usage.ipynb` & `cmomy-0.4.1/examples/archived/example_usage.ipynb`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/examples/archived/parallel_test.ipynb` & `cmomy-0.4.1/examples/archived/parallel_test.ipynb`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/examples/archived/test_accumulator.ipynb` & `cmomy-0.4.1/examples/archived/test_accumulator.ipynb`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/examples/usage/motivation.ipynb` & `cmomy-0.4.1/examples/usage/motivation.ipynb`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/examples/usage/usage_notebook.ipynb` & `cmomy-0.4.1/examples/usage/usage_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/pyproject.toml` & `cmomy-0.4.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.2", "setuptools_scm[toml]>=7.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cmomy"
 authors = [{ name = "William P. Krekelberg", email = "wpk@nist.gov" }]
-license = { text = "NIST license" }
+license = { text = "NIST-PD" }
 description = "Central (co)moment calculation/manipulation"
 # if using markdown
 # long_description_content_type = text/markdown
 keywords = ["cmomy"]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "License :: Public Domain",
@@ -38,24 +38,24 @@
 documentation = "https://pages.nist.gov/cmomy/"
 
 [project.optional-dependencies]
 test = ["pytest"]
 
 # dev = []
 # docs = []
-## Defer this to setup.cfg
-## Will transition when everything works (grayskull in particular)
-## and will remove setup.py
-# [tool.setuptools]
-# zip-safe = true # if using mypy, must be False
-# include-package-data = true
-# license-files = ["LICENSE"]
-# [tool.setuptools.packages.find]
-# namespaces = true
-# where = ["src"]
+## grayskull still messes some things up, but use scripts/recipe-append.sh for this
+[tool.setuptools]
+zip-safe = true # if using mypy, must be False
+include-package-data = true
+license-files = ["LICENSE"]
+
+[tool.setuptools.packages.find]
+namespaces = true
+where = ["src"]
+
 ## include = []
 ## exclude = []
 ##
 [tool.setuptools.dynamic]
 readme = { file = [
     "README.md",
     "CHANGELOG.md",
```

### Comparing `cmomy-0.4.0/scripts/docs-examples-symlinks.sh` & `cmomy-0.4.1/scripts/docs-examples-symlinks.sh`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/src/cmomy/__init__.py` & `cmomy-0.4.1/src/cmomy/__init__.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/src/cmomy/_formatting.py` & `cmomy-0.4.1/src/cmomy/_formatting.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/src/cmomy/_resample.py` & `cmomy-0.4.1/src/cmomy/_resample.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/src/cmomy/_testing.py` & `cmomy-0.4.1/src/cmomy/_testing.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/src/cmomy/_typing.py` & `cmomy-0.4.1/src/cmomy/_typing.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/src/cmomy/abstract_central.py` & `cmomy-0.4.1/src/cmomy/abstract_central.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/src/cmomy/central.py` & `cmomy-0.4.1/src/cmomy/central.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/src/cmomy/compile.py` & `cmomy-0.4.1/src/cmomy/compile.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/src/cmomy/convert.py` & `cmomy-0.4.1/src/cmomy/convert.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/src/cmomy/docstrings.py` & `cmomy-0.4.1/src/cmomy/docstrings.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/src/cmomy/options.py` & `cmomy-0.4.1/src/cmomy/options.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/src/cmomy/pusher_interface.py` & `cmomy-0.4.1/src/cmomy/pusher_interface.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/src/cmomy/pushers.py` & `cmomy-0.4.1/src/cmomy/pushers.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/src/cmomy/resample.py` & `cmomy-0.4.1/src/cmomy/resample.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/src/cmomy/tests/conftest.py` & `cmomy-0.4.1/src/cmomy/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/src/cmomy/tests/test_central.py` & `cmomy-0.4.1/src/cmomy/tests/test_central.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/src/cmomy/tests/test_central_2.py` & `cmomy-0.4.1/src/cmomy/tests/test_central_2.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/src/cmomy/tests/test_convert.py` & `cmomy-0.4.1/src/cmomy/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/src/cmomy/tests/test_resample.py` & `cmomy-0.4.1/src/cmomy/tests/test_resample.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/src/cmomy/tests/test_stability.py` & `cmomy-0.4.1/src/cmomy/tests/test_stability.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/src/cmomy/tests/test_verify.py` & `cmomy-0.4.1/src/cmomy/tests/test_verify.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/src/cmomy/tests/test_xcentral.py` & `cmomy-0.4.1/src/cmomy/tests/test_xcentral.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/src/cmomy/tests/test_xcentral_constructors.py` & `cmomy-0.4.1/src/cmomy/tests/test_xcentral_constructors.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/src/cmomy/utils.py` & `cmomy-0.4.1/src/cmomy/utils.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/src/cmomy/xcentral.py` & `cmomy-0.4.1/src/cmomy/xcentral.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.4.0/src/cmomy.egg-info/PKG-INFO` & `cmomy-0.4.1/src/cmomy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: cmomy
-Version: 0.4.0
+Version: 0.4.1
 Summary: Central (co)moment calculation/manipulation
-Home-page: https://github.com/usnistgov/cmomy
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
-License: NIST license
+License: NIST-PD
 Project-URL: homepage, https://github.com/usnistgov/cmomy
 Project-URL: documentation, https://pages.nist.gov/cmomy/
 Keywords: cmomy
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
```

### Comparing `cmomy-0.4.0/src/cmomy.egg-info/SOURCES.txt` & `cmomy-0.4.1/src/cmomy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 .cruft.json
 .editorconfig
 .gitattributes
 .gitignore
 .markdownlint.yaml
 .pre-commit-config.yaml
 .prettierrc.yaml
+.recipe-append.yaml
 AUTHORS.md
 CHANGELOG.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 conftest.py
 environment.yaml
 pyproject.toml
-setup.cfg
-setup.py
 tox.ini
 changelog.d/README.txt
 changelog.d/templates/new_fragment.md.j2
 changelog.d/templates/auto-changelog/macros.jinja2
 changelog.d/templates/auto-changelog/template.jinja2
 docs/Makefile
 docs/authors.md
@@ -45,15 +44,14 @@
 docs/_templates/autodocsumm/class.rst
 docs/_templates/autodocsumm/module-inherit.rst
 docs/_templates/autodocsumm/module-noindex.rst
 docs/_templates/autodocsumm/module.rst
 docs/_templates/autosummary/base.rst
 docs/_templates/autosummary/class.rst
 docs/_templates/autosummary/module.rst
-docs/examples/create-symlinks.sh
 docs/examples/index.md
 docs/examples/usage/motivation.ipynb
 docs/examples/usage/usage_notebook.ipynb
 docs/reference/api-baseclasses.rst
 docs/reference/api-modules.rst
 docs/reference/api-public.rst
 docs/reference/index.md
@@ -76,14 +74,15 @@
 examples/archived/test_accumulator.ipynb
 examples/usage/motivation.ipynb
 examples/usage/usage_notebook.ipynb
 scripts/dist-conda.mk
 scripts/dist-pypi.mk
 scripts/docs-examples-symlinks.sh
 scripts/lint.mk
+scripts/recipe-append.sh
 scripts/run-prettier.sh
 scripts/tox-ipykernel-display-name.sh
 src/cmomy/__init__.py
 src/cmomy/_formatting.py
 src/cmomy/_resample.py
 src/cmomy/_testing.py
 src/cmomy/_typing.py
@@ -98,17 +97,17 @@
 src/cmomy/py.typed
 src/cmomy/resample.py
 src/cmomy/utils.py
 src/cmomy/xcentral.py
 src/cmomy.egg-info/PKG-INFO
 src/cmomy.egg-info/SOURCES.txt
 src/cmomy.egg-info/dependency_links.txt
-src/cmomy.egg-info/not-zip-safe
 src/cmomy.egg-info/requires.txt
 src/cmomy.egg-info/top_level.txt
+src/cmomy.egg-info/zip-safe
 src/cmomy/tests/__init__.py
 src/cmomy/tests/conftest.py
 src/cmomy/tests/test_central.py
 src/cmomy/tests/test_central_2.py
 src/cmomy/tests/test_convert.py
 src/cmomy/tests/test_resample.py
 src/cmomy/tests/test_stability.py
```

### Comparing `cmomy-0.4.0/tox.ini` & `cmomy-0.4.1/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -27,20 +27,28 @@
     python --version
     python -c 'import {[base]import_name}; print( {[base]import_name}.__version__)'
     bash -ec 'echo $PWD'
 
 [testenv]
 passenv =
         SETUPTOOLS_SCM_PRETEND_VERSION
+        TEST_VERSION
+        # general command
         command
+        # linting
         mypy_args
         pyright_args
         pytype_args
         release_args
+        # dist-conda stuff
         project_name
+        sdist_path
+        grayskull_args
+        recipe_base_path
+        recipe_append_path
 usedevelop =
     test: True
 conda_env =
     test: {[base]conda_env_test}
 allowlist_externals =
     {[base]allowlist_externals}
 commands =
@@ -88,17 +96,17 @@
     recipe: build conda recipe using grayskull (can optionally pass a local sdist)
     build: build conda distribution
     command: run arbitrary command
 skip_install = True
 envdir       = {toxworkdir}/dist-conda
 basepython   = {[base]build_python}
 conda_env    = {[base]conda_env_dist_conda}
-changedir    = {toxinidir}/dist-conda
+changedir    = {toxinidir}
 commands     =
-    make -f {toxinidir}/scripts/dist-conda.mk {posargs} project_name={[base]package_name}
+    make -f {toxinidir}/scripts/dist-conda.mk {posargs} project_name={env:project_name:{[base]package_name}}
 
 [testenv:testdist-{pypi, conda}-{local,remote}-py3{8, 9, 10, 11}]
 conda_channels =
     {[base]conda_channels}
 description =
     Test install from
     pypi: pypi
@@ -106,18 +114,18 @@
     using either
     local: local
     remote: remote
     versions.
 skip_install = True
 conda_env    = {toxinidir}/environment/test-extras.yaml
 conda_deps =
-    conda-remote: {[base]package_name}
+    conda-remote: {[base]package_name}{env:TEST_VERSION:''}
     conda-local: {posargs}
 deps =
-    pypi-remote: {[base]package_name}
+    pypi-remote: {[base]package_name}{env:TEST_VERSION:''}
     pypi-local: {posargs}
 
 [testenv:testpip-py3{8, 9, 10, 11}]
 description  =
     Test package against pip installed packages
 usedevelop   = True
 extras = test
```

