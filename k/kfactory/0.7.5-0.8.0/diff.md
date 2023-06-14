# Comparing `tmp/kfactory-0.7.5.tar.gz` & `tmp/kfactory-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfactory-0.7.5.tar", last modified: Thu Jun  1 16:20:52 2023, max compression
+gzip compressed data, was "kfactory-0.8.0.tar", last modified: Wed Jun 14 03:05:32 2023, max compression
```

## Comparing `kfactory-0.7.5.tar` & `kfactory-0.8.0.tar`

### file list

```diff
@@ -1,110 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.438962 kfactory-0.7.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.430962 kfactory-0.7.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.430962 kfactory-0.7.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-01 16:20:34.000000 kfactory-0.7.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-01 16:20:34.000000 kfactory-0.7.5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-01 16:20:34.000000 kfactory-0.7.5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.430962 kfactory-0.7.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-01 16:20:34.000000 kfactory-0.7.5/.github/workflows/pages.yml
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-01 16:20:34.000000 kfactory-0.7.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-01 16:20:34.000000 kfactory-0.7.5/.github/workflows/test_code.yml
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-01 16:20:34.000000 kfactory-0.7.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-01 16:20:34.000000 kfactory-0.7.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-01 16:20:34.000000 kfactory-0.7.5/.sourcery.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-01 16:20:34.000000 kfactory-0.7.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-01 16:20:34.000000 kfactory-0.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-01 16:20:34.000000 kfactory-0.7.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-06-01 16:20:52.438962 kfactory-0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-01 16:20:34.000000 kfactory-0.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.430962 kfactory-0.7.5/changelog.d/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-01 16:20:34.000000 kfactory-0.7.5/changelog.d/changelog_template.jinja
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.430962 kfactory-0.7.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.430962 kfactory-0.7.5/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/overrides/main.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.430962 kfactory-0.7.5/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.430962 kfactory-0.7.5/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   138035 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/source/_static/complex.png
--rw-r--r--   0 runner    (1001) docker     (123)   985194 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/source/_static/klive.webm
--rw-r--r--   0 runner    (1001) docker     (123)   129785 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/source/_static/waveguide.png
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/source/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/source/complex_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/source/config.md
--rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/source/gdsfactory.md
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/source/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/source/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/source/intro.md
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/source/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.434962 kfactory-0.7.5/docs/source/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    11378 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/source/notebooks/00_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10562 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/source/notebooks/01_references.py
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/source/notebooks/02_DRC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/source/notebooks/03_Enclosures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/source/pre.md
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/source/star.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/source/waveguide.py
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-06-01 16:20:34.000000 kfactory-0.7.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 16:20:52.438962 kfactory-0.7.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.426962 kfactory-0.7.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.434962 kfactory-0.7.5/src/kfactory/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.434962 kfactory-0.7.5/src/kfactory/cells/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/cells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/cells/bezier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/cells/circular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.434962 kfactory-0.7.5/src/kfactory/cells/dbu/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/cells/dbu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/cells/dbu/taper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/cells/dbu/waveguide.py
--rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/cells/euler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/cells/taper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/cells/waveguide.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    94080 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/kcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/pdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/placer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/port.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.434962 kfactory-0.7.5/src/kfactory/routing/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/routing/electrical.py
--rw-r--r--   0 runner    (1001) docker     (123)    12507 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/routing/manhattan.py
--rw-r--r--   0 runner    (1001) docker     (123)    20414 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/routing/optical.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.438962 kfactory-0.7.5/src/kfactory/technology/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/technology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/technology/color_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/technology/klayout_tech.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/technology/layer_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    14087 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/technology/layer_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)    41776 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/technology/layer_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/technology/xml_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/technology/yaml_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/typings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.438962 kfactory-0.7.5/src/kfactory/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55837 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/utils/enclosure.py
--rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/utils/fill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/utils/simplify.py
--rw-r--r--   0 runner    (1001) docker     (123)     9316 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/utils/violations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.438962 kfactory-0.7.5/src/kfactory/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14853 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/widgets/interactive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.434962 kfactory-0.7.5/src/kfactory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-06-01 16:20:52.000000 kfactory-0.7.5/src/kfactory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-06-01 16:20:52.000000 kfactory-0.7.5/src/kfactory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 16:20:52.000000 kfactory-0.7.5/src/kfactory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-01 16:20:52.000000 kfactory-0.7.5/src/kfactory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-01 16:20:52.000000 kfactory-0.7.5/src/kfactory.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.438962 kfactory-0.7.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-01 16:20:34.000000 kfactory-0.7.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-01 16:20:34.000000 kfactory-0.7.5/tests/test_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-06-01 16:20:34.000000 kfactory-0.7.5/tests/test_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-01 16:20:34.000000 kfactory-0.7.5/tests/test_cplxcells.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-06-01 16:20:34.000000 kfactory-0.7.5/tests/test_enclosure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-01 16:20:34.000000 kfactory-0.7.5/tests/test_extrude.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-01 16:20:34.000000 kfactory-0.7.5/tests/test_pdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-06-01 16:20:34.000000 kfactory-0.7.5/tests/test_ports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-01 16:20:34.000000 kfactory-0.7.5/tests/test_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-06-01 16:20:34.000000 kfactory-0.7.5/tests/test_routing.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-01 16:20:34.000000 kfactory-0.7.5/tests/test_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-06-01 16:20:34.000000 kfactory-0.7.5/tests/test_spiral.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:05:32.274974 kfactory-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:05:32.254974 kfactory-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:05:32.254974 kfactory-0.8.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-14 03:05:10.000000 kfactory-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-14 03:05:10.000000 kfactory-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-14 03:05:10.000000 kfactory-0.8.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:05:32.254974 kfactory-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-14 03:05:10.000000 kfactory-0.8.0/.github/workflows/pages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-14 03:05:10.000000 kfactory-0.8.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-14 03:05:10.000000 kfactory-0.8.0/.github/workflows/test_code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-14 03:05:10.000000 kfactory-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-06-14 03:05:10.000000 kfactory-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-14 03:05:10.000000 kfactory-0.8.0/.sourcery.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-14 03:05:10.000000 kfactory-0.8.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-14 03:05:10.000000 kfactory-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-14 03:05:10.000000 kfactory-0.8.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-06-14 03:05:32.274974 kfactory-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-14 03:05:10.000000 kfactory-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:05:32.254974 kfactory-0.8.0/changelog.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-14 03:05:10.000000 kfactory-0.8.0/changelog.d/changelog_template.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:05:32.254974 kfactory-0.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-14 03:05:10.000000 kfactory-0.8.0/docs/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:05:32.254974 kfactory-0.8.0/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-14 03:05:10.000000 kfactory-0.8.0/docs/overrides/main.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:05:32.258974 kfactory-0.8.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:05:32.262974 kfactory-0.8.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   138035 2023-06-14 03:05:10.000000 kfactory-0.8.0/docs/source/_static/complex.png
+-rw-r--r--   0 runner    (1001) docker     (123)   985194 2023-06-14 03:05:10.000000 kfactory-0.8.0/docs/source/_static/klive.webm
+-rw-r--r--   0 runner    (1001) docker     (123)   129785 2023-06-14 03:05:10.000000 kfactory-0.8.0/docs/source/_static/waveguide.png
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-14 03:05:10.000000 kfactory-0.8.0/docs/source/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-14 03:05:10.000000 kfactory-0.8.0/docs/source/complex_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-06-14 03:05:10.000000 kfactory-0.8.0/docs/source/config.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-06-14 03:05:10.000000 kfactory-0.8.0/docs/source/gdsfactory.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-14 03:05:10.000000 kfactory-0.8.0/docs/source/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-14 03:05:10.000000 kfactory-0.8.0/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-06-14 03:05:10.000000 kfactory-0.8.0/docs/source/intro.md
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-14 03:05:10.000000 kfactory-0.8.0/docs/source/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:05:32.262974 kfactory-0.8.0/docs/source/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    11375 2023-06-14 03:05:10.000000 kfactory-0.8.0/docs/source/notebooks/00_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-06-14 03:05:10.000000 kfactory-0.8.0/docs/source/notebooks/01_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-06-14 03:05:10.000000 kfactory-0.8.0/docs/source/notebooks/02_DRC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-14 03:05:10.000000 kfactory-0.8.0/docs/source/notebooks/03_Enclosures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-14 03:05:10.000000 kfactory-0.8.0/docs/source/pre.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-14 03:05:10.000000 kfactory-0.8.0/docs/source/star.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-14 03:05:10.000000 kfactory-0.8.0/docs/source/waveguide.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:05:32.250974 kfactory-0.8.0/gds/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:05:32.266975 kfactory-0.8.0/gds/gds_ref/
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-14 03:05:10.000000 kfactory-0.8.0/gds/gds_ref/bend_circular.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-06-14 03:05:10.000000 kfactory-0.8.0/gds/gds_ref/bend_circular_W1_R10_LWG_EWGSTD_A180_AS1.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-06-14 03:05:10.000000 kfactory-0.8.0/gds/gds_ref/bend_circular_W1_R10_LWG_EWGSTD_A90_AS1.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-06-14 03:05:10.000000 kfactory-0.8.0/gds/gds_ref/bend_circular_W1_R10_LWG_EWGSTD_T180_TS1.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-06-14 03:05:10.000000 kfactory-0.8.0/gds/gds_ref/bend_circular_W1_R10_LWG_EWGSTD_T90_TS1.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-14 03:05:10.000000 kfactory-0.8.0/gds/gds_ref/bend_euler.gds
+-rw-r--r--   0 runner    (1001) docker     (123)    11278 2023-06-14 03:05:10.000000 kfactory-0.8.0/gds/gds_ref/bend_euler_W1_R10_LWG_EWGSTD_A180_R150.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-06-14 03:05:10.000000 kfactory-0.8.0/gds/gds_ref/bend_euler_W1_R10_LWG_EWGSTD_A90_R150.gds
+-rw-r--r--   0 runner    (1001) docker     (123)    11278 2023-06-14 03:05:10.000000 kfactory-0.8.0/gds/gds_ref/bend_euler_W1_R10_LWG_EWGSTD_T180_R150.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-06-14 03:05:10.000000 kfactory-0.8.0/gds/gds_ref/bend_euler_W1_R10_LWG_EWGSTD_T90_R150.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-14 03:05:10.000000 kfactory-0.8.0/gds/gds_ref/bend_s.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-14 03:05:10.000000 kfactory-0.8.0/gds/gds_ref/bend_s_euler.gds
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-14 03:05:10.000000 kfactory-0.8.0/gds/gds_ref/straight_W500_L1000_LWG_EWGSTD.gds
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-14 03:05:10.000000 kfactory-0.8.0/gds/gds_ref/taper.gds
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-14 03:05:10.000000 kfactory-0.8.0/gds/gds_ref/waveguide.gds
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-14 03:05:10.000000 kfactory-0.8.0/gds/gds_ref/waveguide_W500_L1000_LWG_EWGSTD.gds
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-06-14 03:05:10.000000 kfactory-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 03:05:32.274974 kfactory-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:05:32.250974 kfactory-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:05:32.266975 kfactory-0.8.0/src/kfactory/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-14 03:05:10.000000 kfactory-0.8.0/src/kfactory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:05:32.270974 kfactory-0.8.0/src/kfactory/cells/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-14 03:05:10.000000 kfactory-0.8.0/src/kfactory/cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-14 03:05:10.000000 kfactory-0.8.0/src/kfactory/cells/bezier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-14 03:05:10.000000 kfactory-0.8.0/src/kfactory/cells/circular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:05:32.270974 kfactory-0.8.0/src/kfactory/cells/dbu/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-14 03:05:10.000000 kfactory-0.8.0/src/kfactory/cells/dbu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-14 03:05:10.000000 kfactory-0.8.0/src/kfactory/cells/dbu/straight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-14 03:05:10.000000 kfactory-0.8.0/src/kfactory/cells/dbu/taper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-06-14 03:05:10.000000 kfactory-0.8.0/src/kfactory/cells/euler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-14 03:05:10.000000 kfactory-0.8.0/src/kfactory/cells/straight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-14 03:05:10.000000 kfactory-0.8.0/src/kfactory/cells/taper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-14 03:05:10.000000 kfactory-0.8.0/src/kfactory/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110061 2023-06-14 03:05:10.000000 kfactory-0.8.0/src/kfactory/kcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-06-14 03:05:10.000000 kfactory-0.8.0/src/kfactory/pdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-06-14 03:05:10.000000 kfactory-0.8.0/src/kfactory/placer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-06-14 03:05:10.000000 kfactory-0.8.0/src/kfactory/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 03:05:10.000000 kfactory-0.8.0/src/kfactory/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:05:32.270974 kfactory-0.8.0/src/kfactory/routing/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-14 03:05:10.000000 kfactory-0.8.0/src/kfactory/routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-06-14 03:05:10.000000 kfactory-0.8.0/src/kfactory/routing/electrical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12507 2023-06-14 03:05:10.000000 kfactory-0.8.0/src/kfactory/routing/manhattan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20414 2023-06-14 03:05:10.000000 kfactory-0.8.0/src/kfactory/routing/optical.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:05:32.270974 kfactory-0.8.0/src/kfactory/technology/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-14 03:05:10.000000 kfactory-0.8.0/src/kfactory/technology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-06-14 03:05:10.000000 kfactory-0.8.0/src/kfactory/technology/layer_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-14 03:05:10.000000 kfactory-0.8.0/src/kfactory/typings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:05:32.270974 kfactory-0.8.0/src/kfactory/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-14 03:05:10.000000 kfactory-0.8.0/src/kfactory/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55806 2023-06-14 03:05:10.000000 kfactory-0.8.0/src/kfactory/utils/enclosure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-06-14 03:05:10.000000 kfactory-0.8.0/src/kfactory/utils/fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-14 03:05:10.000000 kfactory-0.8.0/src/kfactory/utils/simplify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9316 2023-06-14 03:05:10.000000 kfactory-0.8.0/src/kfactory/utils/violations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:05:32.270974 kfactory-0.8.0/src/kfactory/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 03:05:10.000000 kfactory-0.8.0/src/kfactory/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14853 2023-06-14 03:05:10.000000 kfactory-0.8.0/src/kfactory/widgets/interactive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:05:32.266975 kfactory-0.8.0/src/kfactory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-06-14 03:05:32.000000 kfactory-0.8.0/src/kfactory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-14 03:05:32.000000 kfactory-0.8.0/src/kfactory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 03:05:32.000000 kfactory-0.8.0/src/kfactory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-14 03:05:32.000000 kfactory-0.8.0/src/kfactory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-14 03:05:32.000000 kfactory-0.8.0/src/kfactory.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:05:32.274974 kfactory-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-14 03:05:10.000000 kfactory-0.8.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-14 03:05:10.000000 kfactory-0.8.0/tests/test_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-06-14 03:05:10.000000 kfactory-0.8.0/tests/test_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-14 03:05:10.000000 kfactory-0.8.0/tests/test_cplxcells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-06-14 03:05:10.000000 kfactory-0.8.0/tests/test_enclosure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-14 03:05:10.000000 kfactory-0.8.0/tests/test_extrude.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-14 03:05:10.000000 kfactory-0.8.0/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-14 03:05:10.000000 kfactory-0.8.0/tests/test_netlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-14 03:05:10.000000 kfactory-0.8.0/tests/test_pdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-14 03:05:10.000000 kfactory-0.8.0/tests/test_ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-06-14 03:05:10.000000 kfactory-0.8.0/tests/test_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-14 03:05:10.000000 kfactory-0.8.0/tests/test_routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-14 03:05:10.000000 kfactory-0.8.0/tests/test_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-06-14 03:05:10.000000 kfactory-0.8.0/tests/test_spiral.py
```

### Comparing `kfactory-0.7.5/.github/ISSUE_TEMPLATE/bug_report.md` & `kfactory-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.5/.github/ISSUE_TEMPLATE/feature_request.md` & `kfactory-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.5/.github/workflows/pages.yml` & `kfactory-0.8.0/.github/workflows/pages.yml`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.5/.github/workflows/release.yml` & `kfactory-0.8.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.5/.github/workflows/test_code.yml` & `kfactory-0.8.0/.github/workflows/test_code.yml`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.5/.pre-commit-config.yaml` & `kfactory-0.8.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,30 @@
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-symlinks
       - id: check-yaml
         args: []
       - id: debug-statements
       - id: end-of-file-fixer
-        exclude: "changelog.d/.*"
+        exclude: 'changelog\.d/.*|CHANGLEOG\.md'
       - id: mixed-line-ending
       - id: name-tests-test
         args: ["--pytest-test-first"]
       - id: requirements-txt-fixer
       - id: trailing-whitespace
-
+        args: [--markdown-linebreak-ext=md]
+        exclude: 'changelog\.d/.*|CHANGELOG\.md'
   - repo: https://github.com/asottile/pyupgrade
     rev: v3.4.0
     hooks:
       - id: pyupgrade
+  - repo: https://github.com/twisted/towncrier
+    rev: "23.6.0"
+    hooks:
+      - id: towncrier-check
 
   # - repo: https://github.com/pre-commit/pre-commit-hooks
   #   rev: a41c4b94b220171e928ff3e6c9bef34e71267f46
   #   hooks:
   #     - id: check-yaml
   #       exclude: ^(conda\.recipe/meta\.yaml|conda_build/templates/.*\.yaml|docs/click/meta\.yaml|conda/meta\.yaml|construct.yaml)
   #     - id: end-of-file-fixer
```

### Comparing `kfactory-0.7.5/CHANGELOG.md` & `kfactory-0.8.0/CHANGELOG.md`

 * *Files 27% similar despite different names*

```diff
@@ -4,14 +4,42 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 This project uses [*towncrier*](https://towncrier.readthedocs.io/) and the changes for the upcoming release can be found in <https://github.com/gdsfactory/kfactory/tree/main/changelog.d/>.
 
 <!-- towncrier release notes start -->
 
+## [0.8.0](https://github.com/gdsfactory/kfactory/tree/0.8.0) - 2023-06-14
+
+
+### Added
+
+- KCells now store (and retrieve) Ports and settings/info in/from GDS [#106](https://github.com/gdsfactory/kfactory/issues/106)
+- Added docs section about loguru config [#138](https://github.com/gdsfactory/kfactory/issues/138)
+- Added docs section about gdsfactory differences [#140](https://github.com/gdsfactory/kfactory/issues/140)
+- Add Netlist extraction based on klayout.db.Netlist [#147](https://github.com/gdsfactory/kfactory/issues/147)
+- Added UMKCell to allow addressing some parts in um [#158](https://github.com/gdsfactory/kfactory/issues/158)
+- Added snapping of ports to cell decorator [#159](https://github.com/gdsfactory/kfactory/issues/159)
+
+
+### Changed
+
+- KCell.create_inst doesn't take DCellInstArray args anymore, use KCell.d.create_inst instead [#158](https://github.com/gdsfactory/kfactory/issues/158)
+- Updated the Pdk to pydantic 2.0 [PR](https://github.com/gdsfactory/kfactory/pull/157) 
+- renamed waveguide -> straight [PR](https://github.com/gdsfactory/kfactory/pull/152) 
+
+
+### Fixed
+
+- Fixed incompatibility of Pdk and technology with mypy [#108](https://github.com/gdsfactory/kfactory/issues/108)
+- Fixed keep_mirror flag [#143](https://github.com/gdsfactory/kfactory/issues/143)
+- Fixed (ix)90° bends second port off-grid [#153](https://github.com/gdsfactory/kfactory/issues/153)
+- Fixed circular and euler bends having complex ports in the x*90° cases [#159](https://github.com/gdsfactory/kfactory/issues/159)
+
+
 ## [0.7.5](https://github.com/gdsfactory/kfactory/tree/0.7.5) - 2023-06-01
 
 
 ### Added
 
 - Added `mirror_x/mirror_y` to Instance, `xmin/xmax/ymin/ymax` getter & setter to Instance, `xmin/xmax/ymin/ymax` getter to KCell, `polygon_from_array`, `dpolygon_from_arry` [#92](https://github.com/gdsfactory/kfactory/issues/92)
 - Document settings/config better [#138](https://github.com/gdsfactory/kfactory/issues/138)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `kfactory-0.7.5/LICENSE` & `kfactory-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.5/Makefile` & `kfactory-0.8.0/Makefile`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.5/PKG-INFO` & `kfactory-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: kfactory
-Version: 0.7.5
+Version: 0.8.0
 Summary: KLayout API implementation of gdsfactory
 Author-email: gdsfactory community <contact@gdsfactory.com>
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: git
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: ci
 Provides-Extra: ipy
 License-File: LICENSE
 
-# KFactory 0.7.5
+# KFactory 0.8.0
 
 Kfactory is a [gdsfactory](https://github.com/gdsfactory/gdsfactory)-like tool. It is built with [KLayout](https://klayout.de) as a backend instead of gdstk, but aims to offer the similar featuers.
 
 | :exclamation:  KFactory is still experimental, expect API changes without notice (even though we try to keep it to a minimum!)   |
 |---------------------------------------------------------------------------------------------------------------------------------|
 
-It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.7.5` for example.
+It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.8.0` for example.
 
 Features similar to gdsfactory:
 
 - [x] Cells & decorator for caching & storing cells
 - [x] Simple routing (point to point and simpl bundle routes for electrical routes)
 - [x] Basic cells like euler/circular bends, taper, waveguide
 - [x] Path extrusion (no interface with CrossSections)
```

### Comparing `kfactory-0.7.5/README.md` & `kfactory-0.8.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# KFactory 0.7.5
+# KFactory 0.8.0
 
 Kfactory is a [gdsfactory](https://github.com/gdsfactory/gdsfactory)-like tool. It is built with [KLayout](https://klayout.de) as a backend instead of gdstk, but aims to offer the similar featuers.
 
 | :exclamation:  KFactory is still experimental, expect API changes without notice (even though we try to keep it to a minimum!)   |
 |---------------------------------------------------------------------------------------------------------------------------------|
 
-It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.7.5` for example.
+It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.8.0` for example.
 
 Features similar to gdsfactory:
 
 - [x] Cells & decorator for caching & storing cells
 - [x] Simple routing (point to point and simpl bundle routes for electrical routes)
 - [x] Basic cells like euler/circular bends, taper, waveguide
 - [x] Path extrusion (no interface with CrossSections)
```

### Comparing `kfactory-0.7.5/docs/mkdocs.yml` & `kfactory-0.8.0/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.5/docs/source/_static/complex.png` & `kfactory-0.8.0/docs/source/_static/complex.png`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.5/docs/source/_static/klive.webm` & `kfactory-0.8.0/docs/source/_static/klive.webm`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.5/docs/source/_static/waveguide.png` & `kfactory-0.8.0/docs/source/_static/waveguide.png`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.5/docs/source/complex_cell.py` & `kfactory-0.8.0/docs/source/complex_cell.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,29 +10,29 @@
 #   kernelspec:
 #     display_name: kernel_name
 #     language: python
 #     name: kernel_name
 # ---
 
 from layers import LAYER, si_enc
-from waveguide import waveguide
+from straight import straight
 
 import kfactory as kf
 
 
 @kf.cell
 def composite_cell() -> kf.KCell:
     c = kf.KCell()
 
     bend = c.create_inst(
         kf.cells.circular.bend_circular(
             1000 * c.kcl.dbu, 20000 * c.kcl.dbu, LAYER.SI, enclosure=si_enc
         )  # the standard kf.cells are in um, so we need to convert to dbu
     )
-    wg = c << waveguide(1000, 5000, 5000)
+    wg = c << straight(1000, 5000, 5000)
 
     wg.align("o1", bend, "o2")
 
     c.add_port(name="1", port=bend.ports["o1"])
     c.add_port(name="2", port=wg.ports["o2"])
 
     c.autorename_ports()
```

### Comparing `kfactory-0.7.5/docs/source/config.md` & `kfactory-0.8.0/docs/source/config.md`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.5/docs/source/gdsfactory.md` & `kfactory-0.8.0/docs/source/gdsfactory.md`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.5/docs/source/gen_ref_pages.py` & `kfactory-0.8.0/docs/source/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.5/docs/source/intro.md` & `kfactory-0.8.0/docs/source/intro.md`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 ```python
 from layers import LAYER
 
 import kfactory as kf
 
 
 @kf.cell
-def waveguide(width: int, length: int, width_exclude: int) -> kf.KCell:
+def straight(width: int, length: int, width_exclude: int) -> kf.KCell:
     """Waveguide: Silicon on 1/0, Silicon exclude on 1/1"""
     c = kf.KCell()
     c.shapes(LAYER.SI).insert(kf.kdb.Box(0, -width // 2, length, width // 2))
     c.shapes(LAYER.SIEXCLUDE).insert(
         kf.kdb.Box(0, -width_exclude // 2, length, width_exclude // 2)
     )
 
@@ -60,32 +60,32 @@
 
     c.autorename_ports()
 
     return c
 
 
 if __name__ == "__main__":
-    kf.show(waveguide(2000, 50000, 5000))
+    kf.show(straight(2000, 50000, 5000))
 ```
 
 The ``kf.show`` will create a GDS in the temp folder and then send the GDS by klive to KLayout (if klive is installed).
-By running this with ``python waveguide.py``, this should show us a waveguide like this:
+By running this with ``python straight.py``, this should show us a straight like this:
 
-![waveguide](./_static/waveguide.png)
+![straight](./_static/straight.png)
 
 Afterwards let's create the composite cell [`complex_cell.py`](./complex_cell.py). This one instantiates a waveguide and a circular bend and then connects them.
 
 ```python
 from layers import LAYER
 
 import kfactory as kf
 
 
 @kf.cell
-def waveguide(width: int, length: int, width_exclude: int) -> kf.KCell:
+def straight(width: int, length: int, width_exclude: int) -> kf.KCell:
     """Waveguide: Silicon on 1/0, Silicon exclude on 1/1"""
     c = kf.KCell()
     c.shapes(LAYER.SI).insert(kf.kdb.Box(0, -width // 2, length, width // 2))
     c.shapes(LAYER.SIEXCLUDE).insert(
         kf.kdb.Box(0, -width_exclude // 2, length, width_exclude // 2)
     )
 
@@ -101,15 +101,15 @@
 
     c.autorename_ports()
 
     return c
 
 
 if __name__ == "__main__":
-    kf.show(waveguide(2000, 50000, 5000))
+    kf.show(straight(2000, 50000, 5000))
 ```
 
 With `kfactory.kcell.KCell.add_port` an existing port of an instance can be added to the parent cell. `kfactory.kcell.Instance.connect` allows an instance to be transformed so that one of its ports is connected to another port.
 
 You will get a cell like this:
 
 ![complex_cell](_static/complex.png)
```

### Comparing `kfactory-0.7.5/docs/source/notebooks/00_geometry.py` & `kfactory-0.8.0/docs/source/notebooks/00_geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,15 +237,15 @@
 # %%
 c.show()  # show in klayout
 c.plot()
 
 # %% [markdown]
 # ## Ports
 #
-# Your straights wg1/wg2/wg3 are instances to other waveguide cells.
+# Your straights wg1/wg2/wg3 are instances to other straight cells.
 #
 # If you want to add ports to the new Cell `c` you can use `add_port`, where you can create a new port or use an instance an existing port from the underlying instance.
 
 # %% [markdown]
 # You can access the ports of a Cell or Instance
 
 
@@ -390,15 +390,15 @@
 
 # %% [markdown]
 # ## Move instance by port
 
 
 # %%
 c = kf.KCell()
-wg = c << kf.cells.waveguide.waveguide(width=0.5, length=1, layer=0)
+wg = c << kf.cells.straight.straight(width=0.5, length=1, layer=0)
 bend = c << kf.cells.euler.bend_euler(width=0.5, radius=1, layer=0)
 
 bend.connect("o1", wg.ports["o2"])  # connects follow Source, destination syntax
 c
 
 # %% [markdown]
 # ## Rotate instance
```

### Comparing `kfactory-0.7.5/docs/source/notebooks/01_references.py` & `kfactory-0.8.0/docs/source/notebooks/01_references.py`

 * *Files 12% similar despite different names*

```diff
@@ -140,34 +140,34 @@
 # %% [markdown]
 # As you've seen you have two ways to add an instance to our cell:
 #
 # 1. create the instance and add it to the cell
 
 # %%
 c = kf.KCell(name="instance_sample")
-w = kf.cells.waveguide.waveguide(length=10, width=0.6, layer=c.kcl.layer(1, 0))
+w = kf.cells.straight.straight(length=10, width=0.6, layer=c.kcl.layer(1, 0))
 wr = kf.kdb.CellInstArray(w._kdb_cell, kf.kdb.Trans.R0)
 c.insert(wr)
 c
 
 # %% [markdown]
 # 2. or do it in a single line
 
 # %%
 c = kf.KCell(name="instance_sample_shorter_syntax")
-wr = c << kf.cells.waveguide.waveguide(length=10, width=0.6, layer=c.kcl.layer(1, 0))
+wr = c << kf.cells.straight.straight(length=10, width=0.6, layer=c.kcl.layer(1, 0))
 c
 
 # %% [markdown]
 # in both cases you can move the instance `wr` after created
 
 # %%
 c = kf.KCell(name="two_instances")
-wr1 = c << kf.cells.waveguide.waveguide(length=10, width=0.6, layer=c.kcl.layer(1, 0))
-wr2 = c << kf.cells.waveguide.waveguide(length=10, width=0.6, layer=c.kcl.layer(1, 0))
+wr1 = c << kf.cells.straight.straight(length=10, width=0.6, layer=c.kcl.layer(1, 0))
+wr2 = c << kf.cells.straight.straight(length=10, width=0.6, layer=c.kcl.layer(1, 0))
 wr2.transform(kf.kdb.DTrans(0.0, 10.0))
 c.add_ports(wr1.ports, prefix="top_")
 c.add_ports(wr2.ports, prefix="bot_")
 
 # %%
 c.ports
 
@@ -268,29 +268,29 @@
 b1 = c << bend
 b2 = c << bend
 b2.connect("o1", b1.ports["o2"])
 c
 
 # %%
 c = kf.KCell()
-b1 = c << kf.cells.euler.bend_euler(radius=5, width=1, layer=0, theta=30)
-b2 = c << kf.cells.euler.bend_euler(radius=5, width=1, layer=0, theta=30)
+b1 = c << kf.cells.euler.bend_euler(radius=5, width=1, layer=0, angle=30)
+b2 = c << kf.cells.euler.bend_euler(radius=5, width=1, layer=0, angle=30)
 b2.connect("o1", b1.ports["o2"])
 c.show()
 c
 
 # %% [markdown]
 # ![](https://i.imgur.com/oenlUwg.png)
 #
 # This non-manhattan connect will create less than 1nm gaps that you can fix by flattening the references.
 
 # %%
 c = kf.KCell()
-b1 = c << kf.cells.euler.bend_euler(radius=5, width=1, layer=0, theta=30)
-b2 = c << kf.cells.euler.bend_euler(radius=5, width=1, layer=0, theta=30)
+b1 = c << kf.cells.euler.bend_euler(radius=5, width=1, layer=0, angle=30)
+b2 = c << kf.cells.euler.bend_euler(radius=5, width=1, layer=0, angle=30)
 b2.connect("o1", b1.ports["o2"])
 b2.flatten()
 c.show()
 c
 
 # %% [markdown]
 # Which fixes the issue.
@@ -332,10 +332,10 @@
 # - triangular
 # - path (SiEPIC)
 #
 #
 # by default `KCell.show()` will add triangular pins, so you can see the direction of the port in Klayout.
 
 # %%
-c = kf.cells.euler.bend_euler(radius=5, width=1, layer=0, theta=90)
+c = kf.cells.euler.bend_euler(radius=5, width=1, layer=0, angle=90)
 c.draw_ports()
 c
```

### Comparing `kfactory-0.7.5/docs/source/notebooks/02_DRC.py` & `kfactory-0.8.0/docs/source/notebooks/02_DRC.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.5/docs/source/notebooks/03_Enclosures.py` & `kfactory-0.8.0/docs/source/notebooks/03_Enclosures.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.5/docs/source/pre.md` & `kfactory-0.8.0/docs/source/pre.md`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.5/docs/source/star.py` & `kfactory-0.8.0/docs/source/star.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.5/docs/source/waveguide.py` & `kfactory-0.8.0/docs/source/waveguide.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from layers import LAYER
 
 import kfactory as kf
 
 
 @kf.cell
-def waveguide(width: int, length: int, width_exclude: int) -> kf.KCell:
+def straight(width: int, length: int, width_exclude: int) -> kf.KCell:
     """Waveguide: Silicon on 1/0, Silicon exclude on 1/1"""
     c = kf.KCell()
     c.shapes(LAYER.SI).insert(kf.kdb.Box(0, -width // 2, length, width // 2))
     c.shapes(LAYER.SIEXCLUDE).insert(
         kf.kdb.Box(0, -width_exclude // 2, length, width_exclude // 2)
     )
 
@@ -24,8 +24,8 @@
 
     c.autorename_ports()
 
     return c
 
 
 if __name__ == "__main__":
-    kf.show(waveguide(2000, 50000, 5000))
+    kf.show(straight(2000, 50000, 5000))
```

### Comparing `kfactory-0.7.5/pyproject.toml` & `kfactory-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,25 @@
 classifiers = [
 	"Programming Language :: Python :: 3.10",
 	"Operating System :: OS Independent",
 ]
 requires-python = ">=3.10"
 
 
-version = "0.7.5"
+version = "0.8.0"
 authors = [
     {name = "gdsfactory community", email = "contact@gdsfactory.com"},
 ]
 dependencies = [
 	"klayout >= 0.28.3",
 	"scipy",
 	"ruamel.yaml",
 	"cachetools >= 5.2.0",
-  "pydantic",
+  "pydantic >= 2.0b2",
+	"pydantic-settings >= 2.0b1",
 	"loguru",
 	"tomli",
 ]
 
 [project.optional-dependencies]
 git = [
 	"gitpython",
@@ -99,16 +100,14 @@
 
 [tool.mypy]
 python_version = "3.10"
 strict = true
 exclude = [
 	"tests",
 	"src/kfactory/widgets/interactive.py",
-	"src/kfactory/technology",
-	"src/kfactory/pdk.py",
 ]
 plugins = "pydantic.mypy, numpy.typing.mypy_plugin"
 
 [tool.pylsp-mypy]
 enabled = true
 live_mode = true
 strict = true
@@ -233,15 +232,15 @@
 
 
 [tool.tbump]
 # Uncomment this if your project is hosted on GitHub:
 # github_url = "https://github.com/<user or organization>/<project>/"
 
 [tool.tbump.version]
-current = "0.7.5"
+current = "0.8.0"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

### Comparing `kfactory-0.7.5/src/kfactory/__init__.py` & `kfactory-0.8.0/src/kfactory/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,19 +19,20 @@
     KCLayout,
     default_save,
     LayerEnum,
     show,
     polygon_from_array,
     dpolygon_from_array,
 )
-from . import cells, placer, routing, utils, port, pdk
+from . import cells, placer, routing, utils, port, pdk, technology
 from .conf import config
-from .pdk import Pdk
 
-__version__ = "0.7.5"
+# from .pdk import Pdk
+
+__version__ = "0.8.0"
 
 logger = config.logger
 
 __all__ = [
     "KCell",
     "Instance",
     "Port",
@@ -50,8 +51,9 @@
     "show",
     "config",
     "LayerEnum",
     "logger",
     "pdk",
     "polygon_from_array",
     "dpolygon_from_array",
+    "technology",
 ]
```

### Comparing `kfactory-0.7.5/src/kfactory/cells/bezier.py` & `kfactory-0.8.0/src/kfactory/cells/bezier.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.5/src/kfactory/cells/circular.py` & `kfactory-0.8.0/src/kfactory/cells/circular.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,60 +8,60 @@
 from .. import kdb
 from ..kcell import KCell, LayerEnum, cell
 from ..utils import LayerEnclosure, extrude_path
 
 __all__ = ["bend_circular"]
 
 
-@cell
+@cell(snap_ports=False)
 def bend_circular(
     width: float,
     radius: float,
     layer: int | LayerEnum,
     enclosure: LayerEnclosure | None = None,
-    theta: float = 90,
-    theta_step: float = 1,
+    angle: float = 90,
+    angle_step: float = 1,
 ) -> KCell:
     """Circular radius bend [um].
 
     Args:
         width: Width of the core. [um]
         radius: Radius of the backbone. [um]
         layer: Layer index of the target layer.
         enclosure: Optional enclosure.
-        theta: Angle amount of the bend.
-        theta_step: Angle amount per backbone point of the bend.
+        angle: Angle amount of the bend.
+        angle_step: Angle amount per backbone point of the bend.
     """
     c = KCell()
     r = radius
     backbone = [
         kdb.DPoint(x, y)
         for x, y in [
-            [np.sin(_theta / 180 * np.pi) * r, (-np.cos(_theta / 180 * np.pi) + 1) * r]
-            for _theta in np.linspace(
-                0, theta, int(theta // theta_step + 0.5), endpoint=True
+            [np.sin(_angle / 180 * np.pi) * r, (-np.cos(_angle / 180 * np.pi) + 1) * r]
+            for _angle in np.linspace(
+                0, angle, int(angle // angle_step + 0.5), endpoint=True
             )
         ]
     ]
 
     extrude_path(
         target=c,
         layer=layer,
         path=backbone,
         width=width,
         enclosure=enclosure,
         start_angle=0,
-        end_angle=theta,
+        end_angle=angle,
     )
 
     c.create_port(
         trans=kdb.Trans(2, False, 0, 0),
         width=int(width / c.kcl.dbu),
         layer=layer,
     )
     c.create_port(
-        dcplx_trans=kdb.DCplxTrans(1, theta, False, backbone[-1].to_v()),
+        dcplx_trans=kdb.DCplxTrans(1, angle, False, backbone[-1].to_v()),
         dwidth=width,
         layer=layer,
     )
     c.autorename_ports()
     return c
```

### Comparing `kfactory-0.7.5/src/kfactory/cells/dbu/taper.py` & `kfactory-0.8.0/src/kfactory/cells/dbu/taper.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.5/src/kfactory/cells/dbu/waveguide.py` & `kfactory-0.8.0/src/kfactory/cells/dbu/straight.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 The slabs and excludes can be given in the form of an
 [Enclosure][kfactory.utils.LayerEnclosure].
 """
 
 from ... import KCell, LayerEnum, cell, kdb
 from ...utils import LayerEnclosure
 
-__all__ = ["waveguide"]
+__all__ = ["straight"]
 
 
 @cell
-def waveguide(
+def straight(
     width: int,
     length: int,
     layer: int | LayerEnum,
     enclosure: LayerEnclosure | None = None,
 ) -> KCell:
     """Waveguide defined in dbu.
```

### Comparing `kfactory-0.7.5/src/kfactory/cells/euler.py` & `kfactory-0.8.0/src/kfactory/cells/euler.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,48 +160,48 @@
 
 @cell
 def bend_euler(
     width: float,
     radius: float,
     layer: int | LayerEnum,
     enclosure: LayerEnclosure | None = None,
-    theta: float = 90,
+    angle: float = 90,
     resolution: float = 150,
 ) -> KCell:
     """Create a euler bend.
 
     Args:
         width: Width of the core. [um]
         radius: Radius off the backbone. [um]
         layer: Layer index / LayerEnum of the core.
         enclosure: Slab/exclude definition. [dbu]
-        theta: Angle of the bend.
+        angle: Angle of the bend.
         resolution: Angle resolution for the backbone.
     """
     c = KCell()
     dbu = c.layout().dbu
-    backbone = euler_bend_points(theta, radius=radius, resolution=resolution)
+    backbone = euler_bend_points(angle, radius=radius, resolution=resolution)
 
     extrude_path(
         target=c,
         layer=layer,
         path=backbone,
         width=width,
         enclosure=enclosure,
         start_angle=0,
-        end_angle=theta,
+        end_angle=angle,
     )
     c.create_port(
         layer=layer,
         width=int(width / c.kcl.dbu),
         trans=kdb.Trans(2, False, backbone[0].to_itype(dbu).to_v()),
     )
 
     c.create_port(
-        dcplx_trans=kdb.DCplxTrans(1, theta, False, backbone[-1].to_v()),
+        dcplx_trans=kdb.DCplxTrans(1, angle, False, backbone[-1].to_v()),
         dwidth=width,
         layer=layer,
     )
 
     c.autorename_ports()
     return c
```

### Comparing `kfactory-0.7.5/src/kfactory/cells/taper.py` & `kfactory-0.8.0/src/kfactory/cells/taper.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.5/src/kfactory/cells/waveguide.py` & `kfactory-0.8.0/src/kfactory/cells/straight.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 
 The slabs and excludes can be given in the form of an :py:class:~`Enclosure`.
 """
 
 
 from .. import KCell, LayerEnum, kcl
 from ..utils import LayerEnclosure
-from .dbu.waveguide import waveguide as waveguide_dbu
+from .dbu.straight import straight as straight_dbu
 
-__all__ = ["waveguide", "waveguide_dbu"]
+__all__ = ["straight", "straight_dbu"]
 
 
-def waveguide(
+def straight(
     width: float,
     length: float,
     layer: int | LayerEnum,
     enclosure: LayerEnclosure | None = None,
 ) -> KCell:
     """Straight waveguide in um.
 
@@ -40,15 +40,15 @@
         │            Core             │
         │                             │
         ├─────────────────────────────┤
         │        Slab/Exclude         │
         └─────────────────────────────┘
 
     Args:
-        width: Width of the waveguide. [um]
-        length: Length of the waveguide. [um]
-        layer: Main layer of the waveguide.
+        width: Width of the straight. [um]
+        length: Length of the straight. [um]
+        layer: Main layer of the straight.
         enclosure: Definition of slabs/excludes. [um]
     """
-    return waveguide_dbu(
+    return straight_dbu(
         int(width / kcl.dbu), int(length / kcl.dbu), layer, enclosure=enclosure
     )
```

### Comparing `kfactory-0.7.5/src/kfactory/conf.py` & `kfactory-0.8.0/src/kfactory/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 import sys
 import traceback
 from itertools import takewhile
 from typing import TYPE_CHECKING, Any, ClassVar, Literal
 
 import loguru
 from loguru import logger as logger
-from pydantic import BaseModel, BaseSettings, Field
+from pydantic import BaseModel, Field
+from pydantic_settings import BaseSettings
 
 if TYPE_CHECKING:
     from loguru import Logger
 
 
 def add_traceback(record: loguru.Record) -> None:
     """Add a traceback to the logger."""
@@ -105,15 +106,15 @@
         self.logger.info("LogLevel: {}", self.logfilter.level)
 
     class Config:
         """Pydantic settings."""
 
         validation = False
         arbitrary_types_allowed = True
-        fields = {"logger": {"exclude": True}}
+        # fields = {"logger": {"exclude": True}}
         env_prefix = "kfactory_"
         env_nested_delimiter = "_"
 
 
 config = Settings()
```

### Comparing `kfactory-0.7.5/src/kfactory/kcell.py` & `kfactory-0.8.0/src/kfactory/kcell.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,77 +3,110 @@
 Defines the [KCell][kfactory.kcell.KCell] providing klayout Cells with Ports
 and other convenience functions.
 
 [Instance][kfactory.kcell.Instance] are the kfactory instances used to also acquire
 ports and other inf from instances.
 
 """
+from __future__ import annotations
 
 import functools
 import importlib
 import importlib.util
+import inspect
 import json
 import socket
 from collections.abc import Callable, Hashable, Iterable, Iterator
-from enum import Enum, IntEnum
+from enum import Enum, IntEnum, IntFlag, auto
 from hashlib import sha3_512
-from inspect import Parameter, signature
 from pathlib import Path
 from tempfile import gettempdir
-from typing import TYPE_CHECKING, Any, Literal, TypeVar, cast, overload
+from typing import TYPE_CHECKING, Any, Literal, TypeAlias, TypeVar, overload
 
 import cachetools.func
 import numpy as np
 import ruamel.yaml
 from typing_extensions import ParamSpec
 
-from . import kdb
+from . import kdb, lay
 from .conf import config
 from .port import rename_clockwise
 
 if TYPE_CHECKING:
     from .pdk import Pdk
 
 
 KCellParams = ParamSpec("KCellParams")
-
 AnyTrans = TypeVar(
     "AnyTrans", bound=kdb.Trans | kdb.DTrans | kdb.ICplxTrans | kdb.DCplxTrans
 )
+SerializableShape: TypeAlias = (
+    kdb.Box
+    | kdb.DBox
+    | kdb.Edge
+    | kdb.DEdge
+    | kdb.EdgePair
+    | kdb.DEdgePair
+    | kdb.EdgePairs
+    | kdb.Edges
+    | lay.LayerProperties
+    | kdb.Matrix2d
+    | kdb.Matrix3d
+    | kdb.Path
+    | kdb.DPath
+    | kdb.Point
+    | kdb.DPoint
+    | kdb.Polygon
+    | kdb.DPolygon
+    | kdb.SimplePolygon
+    | kdb.DSimplePolygon
+    | kdb.Region
+    | kdb.Text
+    | kdb.DText
+    | kdb.Texts
+    | kdb.Trans
+    | kdb.DTrans
+    | kdb.CplxTrans
+    | kdb.ICplxTrans
+    | kdb.DCplxTrans
+    | kdb.VCplxTrans
+    | kdb.Vector
+    | kdb.DVector
+)
 
 
 class PROPID(IntEnum):
     """Mapping for GDS properties."""
 
     NAME = 0
 
 
 class LockedError(AttributeError):
     """Raised when a locked cell is being modified."""
 
-    @config.logger.catch
-    def __init__(self, kcell: "KCell"):
+    @config.logger.catch(reraise=True)
+    def __init__(self, kcell: KCell):
         """Throw _locked error."""
         super().__init__(
             f"KCell {kcell.name} has been locked already."
             " Modification has been disabled. "
             "Modify the KCell in its autocell function or make a copy."
         )
 
 
 class PortWidthMismatch(ValueError):
     """Error thrown when two ports don't have a matching `width`."""
 
-    @config.logger.catch
+    @config.logger.catch(reraise=True)
     def __init__(
         self,
-        inst: "Instance",
-        other_inst: "Instance | Port",
-        p1: "Port",
-        p2: "Port",
+        inst: Instance,
+        other_inst: Instance | Port,
+        p1: Port,
+        p2: Port,
         *args: Any,
     ):
         """Throw error for the two ports `p1`/`p1`."""
         if isinstance(other_inst, Instance):
             super().__init__(
                 f'Width mismatch between the ports {inst.cell.name}["{p1.name}"]'
                 f'and {other_inst.cell.name}["{p2.name}"] ({p1.width}/{p2.width})',
@@ -86,22 +119,22 @@
                 *args,
             )
 
 
 class PortLayerMismatch(ValueError):
     """Error thrown when two ports don't have a matching `layer`."""
 
-    @config.logger.catch
+    @config.logger.catch(reraise=True)
     def __init__(
         self,
-        lib: "KCLayout",
-        inst: "Instance",
-        other_inst: "Instance | Port",
-        p1: "Port",
-        p2: "Port",
+        lib: KCLayout,
+        inst: Instance,
+        other_inst: Instance | Port,
+        p1: Port,
+        p2: Port,
         *args: Any,
     ):
         """Throw error for the two ports `p1`/`p1`."""
         l1 = (
             f"{p1.layer.name}({p1.layer.__int__()})"
             if isinstance(p1.layer, LayerEnum)
             else str(lib.get_info(p1.layer))
@@ -124,21 +157,21 @@
                 *args,
             )
 
 
 class PortTypeMismatch(ValueError):
     """Error thrown when two ports don't have a matching `port_type`."""
 
-    @config.logger.catch
+    @config.logger.catch(reraise=True)
     def __init__(
         self,
-        inst: "Instance",
-        other_inst: "Instance | Port",
-        p1: "Port",
-        p2: "Port",
+        inst: Instance,
+        other_inst: Instance | Port,
+        p1: Port,
+        p2: Port,
         *args: Any,
     ):
         """Throw error for the two ports `p1`/`p1`."""
         if isinstance(other_inst, Instance):
             super().__init__(
                 f'Type mismatch between the ports {inst.cell.name}["{p1.name}"]'
                 f' and {other_inst.cell.name}["{p2.name}"]'
@@ -161,18 +194,47 @@
 
 def default_save() -> kdb.SaveLayoutOptions:
     """Default options for saving GDS/OAS."""
     save = kdb.SaveLayoutOptions()
     save.gds2_write_cell_properties = True
     save.gds2_write_file_properties = True
     save.gds2_write_timestamps = False
+    # save.write_context_info = False  # True
 
     return save
 
 
+class PortCheck(IntFlag):
+    opposite = auto()
+    width = auto()
+    layer = auto()
+    port_type = auto()
+    all_opposite = opposite + width + port_type + layer
+    all_overlap = width + port_type + layer
+
+
+@config.logger.catch(reraise=True)
+def port_check(p1: Port, p2: Port, checks: PortCheck = PortCheck.all_opposite) -> None:
+    if checks & PortCheck.opposite:
+        assert (
+            p1.trans == p2.trans * kdb.Trans.R180
+            or p1.trans == p2.trans * kdb.Trans.M90
+        ), ("Transformations of ports not matching for opposite check" f"{p1=} {p2=}")
+    if (checks & PortCheck.opposite) == 0:
+        assert (
+            p1.trans == p2.trans or p1.trans == p2.trans * kdb.Trans.M0
+        ), f"Transformations of ports not matching for overlapping check {p1=} {p2=}"
+    if checks & PortCheck.width:
+        assert p1.width == p2.width, f"Width mismatch for {p1=} {p2=}"
+    if checks & PortCheck.layer:
+        assert p1.layer == p2.layer, f"Layer mismatch for {p1=} {p2=}"
+    if checks & PortCheck.port_type:
+        assert p1.port_type == p2.port_type, f"Port type mismatch for {p1=} {p2=}"
+
+
 class KCLayout(kdb.Layout):
     """Small extension to the klayout.db.Layout.
 
     It adds tracking for the [KCell][kfactory.kcell.KCell] objects
     instead of only the `klayout.db.Cell` objects.
     Additionally it allows creation and registration through `create_cell`
 
@@ -180,27 +242,27 @@
 
     Attributes:
         editable: Whether the layout should be opened in editable mode (default: True)
         rename_function: function that takes an iterable object of ports and renames
             them
     """
 
-    def __init__(self, editable: bool = True, pdk: "Pdk | None" = None) -> None:
+    def __init__(self, editable: bool = True, pdk: Pdk | None = None) -> None:
         """Create a library of cells.
 
         Args:
             editable: Open the KLayout Layout in editable mode if `True`.
             pdk: Pdk associated with the layout.
         """
-        self.kcells: dict[int, "KCell"] = {}
+        self.kcells: dict[int, KCell] = {}
         kdb.Layout.__init__(self, editable)
         self.rename_function: Callable[..., None] = rename_clockwise
-        self.pdk = pdk
+        self.pdk: Pdk | None = pdk
 
-    def dup(self, init_cells: bool = True) -> "KCLayout":
+    def dup(self, init_cells: bool = True) -> KCLayout:
         """Create a duplication of the `~KCLayout` object.
 
         Args:
             init_cells: initialize the all cells in the new KCLayout object
 
         Returns:
             Copy of itself
@@ -247,66 +309,70 @@
             return kdb.Layout.create_cell(self, name, *args)
         else:
             raise ValueError(
                 f"Cellname {name} already exists. Please make sure the cellname is"
                 " unique or pass `allow_duplicate` when creating the library"
             )
 
-    def delete_cell(self, cell: "KCell | int") -> None:
+    def delete_cell(self, cell: KCell | int) -> None:
         """Delete a cell in the kcl object."""
         if isinstance(cell, int):
             super().delete_cell(cell)
             del self.kcells[cell]
         else:
             ci = cell.cell_index()
             super().delete_cell(ci)
             del self.kcells[ci]
 
-    def register_cell(self, kcell: "KCell", allow_reregister: bool = False) -> None:
+    def register_cell(self, kcell: KCell, allow_reregister: bool = False) -> None:
         """Register an existing cell in the KCLayout object.
 
         Args:
             kcell: KCell to be registered in the KCLayout
             allow_reregister: Overwrite the existing KCell registration with this one.
                 Doesn't allow name duplication.
         """
 
-        def check_name(other: "KCell") -> bool:
+        def check_name(other: KCell) -> bool:
             return other._kdb_cell.name == kcell._kdb_cell.name
 
         if (kcell.cell_index() not in self.kcells) or allow_reregister:
             self.kcells[kcell.cell_index()] = kcell
         else:
             raise ValueError(
                 "Cannot register a new cell with a name that already"
                 " exists in the library"
             )
 
-    def __getitem__(self, obj: str | int) -> "KCell":
+    def __getitem__(self, obj: str | int) -> KCell:
         """Retrieve a cell by name(str) or index(int).
 
         Attrs:
             obj: name of cell or cell_index
         """
         if isinstance(obj, int):
             try:
                 return self.kcells[obj]
             except KeyError:
                 if self.cell(obj) is None:
                     raise
 
-                c = self.cell(obj)
-                return KCell(name=c.name, kcl=self, kdb_cell=self.cell(obj))
+                kdb_c = self.cell(obj)
+                c = KCell(name=kdb_c.name, kcl=self, kdb_cell=self.cell(obj))
+                c.get_meta_data()
+                return c
         else:
             if self.cell(obj) is not None:
                 try:
                     return self.kcells[self.cell(obj).cell_index()]
                 except KeyError:
-                    c = self.cell(obj)
-                    return KCell(name=c.name, kcl=self, kdb_cell=self.cell(obj))
+                    kdb_c = self.cell(obj)
+                    c = KCell(name=kdb_c.name, kcl=self, kdb_cell=self.cell(obj))
+                    c.get_meta_data()
+                    return c
             from pprint import pformat
 
             raise ValueError(
                 f"Library doesn't have a KCell named {obj},"
                 " available KCells are"
                 f"{pformat(sorted([cell.name for cell in self.kcells.values()]))}"
             )
@@ -333,34 +399,58 @@
             lm = kdb.Layout.read(self, fn)
         else:
             lm = kdb.Layout.read(self, fn, options)
 
         if register_cells:
             new_cells = set(self.cells("*")) - cells
             for c in new_cells:
-                KCell(kdb_cell=c, kcl=self)
+                kc = KCell(kdb_cell=c, kcl=self)
+                kc.get_meta_data()
 
         return lm
 
-    def write(  # type: ignore[override]
+    @overload  # type: ignore[override]
+    def write(self, filename: str | Path) -> None:
+        ...
+
+    @overload
+    def write(
+        self,
+        filename: str | Path,
+        options: kdb.SaveLayoutOptions,
+    ) -> None:
+        ...
+
+    @overload
+    def write(
+        self,
+        filename: str | Path,
+        options: kdb.SaveLayoutOptions = default_save(),
+        set_meta: bool = True,
+    ) -> None:
+        ...
+
+    def write(
         self,
         filename: str | Path,
-        gzip: bool = False,
         options: kdb.SaveLayoutOptions = default_save(),
+        set_meta: bool = True,
     ) -> None:
         """Write a GDS file into the existing Layout.
 
         Args:
             filename: Path of the GDS file.
-            gzip: directly make the GDS a .gds.gz file.
             options: KLayout options to load from the GDS. Can determine how merge
                 conflicts are handled for example. See
                 https://www.klayout.de/doc-qt5/code/class_LoadLayoutOptions.html
+            set_meta: Make sure all the cells have their metadata set
         """
-        return kdb.Layout.write(self, str(filename), options)
+        for kcell in self.kcells.values():
+            kcell.set_meta_data()
+        return super().write(str(filename), options)
 
 
 kcl = KCLayout()
 """Default library object.
 
 Any [KCell][kfactory.kcell.KCell] uses this object unless another one is
 specified in the constructor."""
@@ -377,19 +467,19 @@
         datatype: layer datatype
     """
 
     layer: int
     datatype: int
 
     def __new__(  # type: ignore[misc]
-        cls: "LayerEnum",
+        cls: LayerEnum,
         layer: int,
         datatype: int,
         kcl: KCLayout = kcl,
-    ) -> "LayerEnum":
+    ) -> LayerEnum:
         """Create a new Enum.
 
         Because it needs to act like an integer an enum is created and expanded.
 
         Args:
             layer: Layer number of the layer.
             datatype: Datatype of the layer.
@@ -455,42 +545,43 @@
     yaml_tag = "!Port"
     name: str | None
     kcl: KCLayout
     width: int
     layer: int | LayerEnum
     _trans: kdb.Trans | None
     _dcplx_trans: kdb.DCplxTrans | None
+    info: dict[str, int | float | str]
     port_type: str
-    d: "UMPort"
+    d: UMPort
 
     @overload
     def __init__(
         self,
         *,
         name: str | None = None,
         width: int,
         layer: LayerEnum | int,
         trans: kdb.Trans,
         kcl: KCLayout = kcl,
         port_type: str = "optical",
-        info: dict[str, Any] = {},
+        info: dict[str, int | float | str] = {},
     ):
         ...
 
     @overload
     def __init__(
         self,
         *,
         name: str | None = None,
         dwidth: float,
         layer: LayerEnum | int,
         dcplx_trans: kdb.DCplxTrans,
         kcl: KCLayout = kcl,
         port_type: str = "optical",
-        info: dict[str, Any] = {},
+        info: dict[str, int | float | str] = {},
     ):
         ...
 
     @overload
     def __init__(
         self,
         *,
@@ -498,15 +589,15 @@
         width: int,
         layer: LayerEnum | int,
         port_type: str = "optical",
         angle: int,
         position: tuple[int, int],
         mirror_x: bool = False,
         kcl: KCLayout = kcl,
-        info: dict[str, Any] = {},
+        info: dict[str, int | float | str] = {},
     ):
         ...
 
     @overload
     def __init__(
         self,
         *,
@@ -514,15 +605,15 @@
         dwidth: float,
         layer: LayerEnum | int,
         port_type: str = "optical",
         dangle: float,
         dposition: tuple[float, float],
         mirror_x: bool = False,
         kcl: KCLayout = kcl,
-        info: dict[str, Any] = {},
+        info: dict[str, int | float | str] = {},
     ):
         ...
 
     def __init__(
         self,
         *,
         name: str | None = None,
@@ -533,17 +624,17 @@
         trans: kdb.Trans | str | None = None,
         dcplx_trans: kdb.DCplxTrans | str | None = None,
         angle: int | None = None,
         dangle: float | None = None,
         position: tuple[int, int] | None = None,
         dposition: tuple[float, float] | None = None,
         mirror_x: bool = False,
-        port: "Port | None" = None,
+        port: Port | None = None,
         kcl: KCLayout = kcl,
-        info: dict[str, Any] = {},
+        info: dict[str, int | float | str] = {},
     ):
         """Create a port from dbu or um based units."""
         self.kcl = kcl
         self.d = UMPort(self)
         self.info = info.copy()
         if port is not None:
             self.name = port.name if name is None else name
@@ -591,20 +682,20 @@
 
             assert layer is not None
             self.name = name
             self.layer = layer
             self.port_type = port_type
 
     @classmethod
-    def from_yaml(cls: "type[Port]", constructor, node) -> "Port":  # type: ignore
+    def from_yaml(cls: type[Port], constructor, node) -> Port:  # type: ignore
         """Internal function used by the placer to convert yaml to a Port."""
         d = dict(constructor.construct_pairs(node))
         return cls(**d)
 
-    def copy(self, trans: kdb.Trans | kdb.DCplxTrans = kdb.Trans.R0) -> "Port":
+    def copy(self, trans: kdb.Trans | kdb.DCplxTrans = kdb.Trans.R0) -> Port:
         """Get a copy of a port.
 
         Args:
             trans: an optional transformation applied to the port to be copied
 
         Returns:
             port: a copy of the port
@@ -700,16 +791,22 @@
         The setter will set a complex transformation and overwrite the internal
         transformation (set simple to `None` and the complex to the provided value.
         """
         return self._dcplx_trans or kdb.DCplxTrans(self.trans.to_dtype(self.kcl.dbu))
 
     @dcplx_trans.setter
     def dcplx_trans(self, value: kdb.DCplxTrans) -> None:
-        self._dcplx_trans = value.dup()
-        self._trans = None
+        if value.is_complex() or value.disp != value.disp.to_itype(
+            self.kcl.dbu
+        ).to_dtype(self.kcl.dbu):
+            self._dcplx_trans = value.dup()
+            self._trans = None
+        else:
+            self._trans = value.dup().s_trans().to_itype(self.kcl.dbu)
+            self._dcplx_trans = None
 
     @property
     def angle(self) -> int:
         """Angle of the transformation.
 
         In the range of `[0,1,2,3]` which are increments in 90°. Not to be confused
         with `rot` of the transformation which keeps additional info about the
@@ -878,22 +975,24 @@
             passed to the GDS and therefore not reversible.
         _kdb_cell: Pure KLayout cell object.
         _locked: If set the cell shouldn't be modified anymore.
         ports: Manages the ports of the cell.
     """
 
     yaml_tag = "!KCell"
-    _ports: "Ports"
+    _ports: Ports
+    settings: dict[str, str | float | int | SerializableShape]
+    d: UMKCell
 
     def __init__(
         self,
         name: str | None = None,
         kcl: KCLayout = kcl,
         kdb_cell: kdb.Cell | None = None,
-        ports: "Ports | None" = None,
+        ports: Ports | None = None,
     ):
         """Constructor of KCell.
 
         Args:
             name: Name of the cell, if None will autogenerate name to
                 "Unnamed_<cell_index>".
             kcl: KCLayout the cell should be attached to.
@@ -901,15 +1000,15 @@
                 KLayout Cell
             ports: Attach an existing [Ports][kfactory.kcell.Ports] object to the KCell,
                 if `None` create an empty one.
         """
         self.kcl = kcl
         self.insts: Instances = Instances()
         self.settings: dict[str, Any] = {}
-        self.info: dict[str, Any] = {}
+        self.info: dict[str, int | float | str] = {}
         self._locked = False
         if name is None:
             _name = "Unnamed_!"
         else:
             _name = name
         self._kdb_cell = kdb_cell or kcl.create_cell(_name)
         if _name == "Unnamed_!":
@@ -917,14 +1016,15 @@
         self.kcl.register_cell(self, allow_reregister=True)
         self.ports: Ports = ports or Ports(self.kcl)
         self.complex = False
 
         if kdb_cell is not None:
             for inst in kdb_cell.each_inst():
                 self.insts.append(Instance(self.kcl, inst))
+        self.d = UMKCell(self)
 
     def __getitem__(self, key: int | str | None) -> Port:
         """Returns port from instance."""
         return self.ports[key]
 
     @property
     def name(self) -> str:
@@ -959,15 +1059,15 @@
             raise LockedError(self)
         self._kdb_cell.ghost_cell = value
 
     def __getattr__(self, name):  # type: ignore[no-untyped-def]
         """If KCell doesn't have an attribute, look in the KLayout Cell."""
         return getattr(self._kdb_cell, name)
 
-    def dup(self) -> "KCell":
+    def dup(self) -> KCell:
         """Copy the full cell.
 
         Sets `_locked` to `False`
 
         Returns:
             cell: Exact copy of the current cell.
                 The name will have `$1` as duplicate names are not allowed
@@ -977,15 +1077,15 @@
         c = KCell(kcl=self.kcl, kdb_cell=kdb_copy)
         c.ports = self.ports.copy()
         for inst in kdb_copy.each_inst():
             c.insts.append(Instance(self.kcl, instance=inst))
         # c._locked = False
         return c
 
-    def __copy__(self) -> "KCell":
+    def __copy__(self) -> KCell:
         """Enables use of `copy.copy` and `copy.deep_copy`."""
         return self.dup()
 
     def add_port(
         self, port: Port, name: str | None = None, keep_mirror: bool = False
     ) -> None:
         """Add an existing port. E.g. from an instance to propagate the port.
@@ -1015,19 +1115,19 @@
         """
         if self._locked:
             raise LockedError(self)
         self.ports.add_ports(ports=ports, prefix=prefix, keep_mirror=keep_mirror)
 
     @classmethod
     def from_yaml(
-        cls: "Callable[..., KCell]",
+        cls: Callable[..., KCell],
         constructor: Any,
         node: Any,
         verbose: bool = False,
-    ) -> "KCell":
+    ) -> KCell:
         """Internal function used by the placer to convert yaml to a KCell."""
         d = ruamel.yaml.constructor.SafeConstructor.construct_mapping(
             constructor,
             node,
             deep=True,
         )
         cell = cls(d["name"])
@@ -1219,20 +1319,20 @@
 
     def __repr__(self) -> str:
         """Return a string representation of the Cell."""
         port_names = [p.name for p in self.ports]
         return f"{self.name}: ports {port_names}, {len(self.insts)} instances"
 
     @property
-    def ports(self) -> "Ports":
+    def ports(self) -> Ports:
         """Ports associated with the cell."""
         return self._ports
 
     @ports.setter
-    def ports(self, new_ports: "InstancePorts | Ports") -> None:
+    def ports(self, new_ports: InstancePorts | Ports) -> None:
         if self._locked:
             raise LockedError(self)
         self._ports = new_ports.copy()
 
     @overload
     def create_port(
         self,
@@ -1285,75 +1385,50 @@
         if self._locked:
             raise LockedError(self)
         self.ports.create_port(**kwargs)
 
     @overload
     def create_inst(
         self,
-        cell: "KCell | int",
+        cell: KCell | int,
         trans: kdb.Trans | kdb.ICplxTrans | kdb.Vector = kdb.Trans(),
-    ) -> "Instance":
+    ) -> Instance:
         ...
 
     @overload
     def create_inst(
         self,
-        cell: "KCell | int",
-        *,
-        dtrans: kdb.DTrans | kdb.DCplxTrans | kdb.DVector,
-    ) -> "Instance":
-        ...
-
-    @overload
-    def create_inst(
-        self,
-        cell: "KCell | int",
-        trans: kdb.Trans | kdb.ICplxTrans | kdb.Vector,
+        cell: KCell | int,
+        trans: kdb.Trans | kdb.ICplxTrans | kdb.Vector = kdb.Trans(),
         *,
         a: kdb.Vector,
         b: kdb.Vector,
         na: int = 1,
         nb: int = 1,
-    ) -> "Instance":
-        ...
-
-    @overload
-    def create_inst(
-        self,
-        cell: "KCell | int",
-        *,
-        dtrans: kdb.DTrans | kdb.DCplxTrans,
-        a: kdb.DVector,
-        b: kdb.DVector,
-        na: int = 1,
-        nb: int = 1,
-    ) -> "Instance":
+    ) -> Instance:
         ...
 
     def create_inst(
         self,
-        cell: "KCell | int",
+        cell: KCell | int,
         trans: kdb.Trans | kdb.Vector | kdb.ICplxTrans = kdb.Trans(),
-        dtrans: kdb.DTrans | kdb.DCplxTrans | kdb.DVector | None = None,
-        a: kdb.Vector | kdb.DVector | None = None,
-        b: kdb.Vector | kdb.DVector | None = None,
+        a: kdb.Vector | None = None,
+        b: kdb.Vector | None = None,
         na: int = 1,
         nb: int = 1,
-    ) -> "Instance":
+    ) -> Instance:
         """Add an instance of another KCell.
 
         Args:
             cell: The cell to be added
             trans: The integer transformation applied to the reference
-            dtrans: um transformation of the reference. If not `None`,
-                will overwrite trans`
-            a: Vector (DVector if trans is um based) for the array.
+            a: Vector for the array.
                 Needs to be in positive X-direction. Usually this is only a
                 Vector in x-direction. Some foundries won't allow other Vectors.
-            b: Vector (DVector if transs is um based) for the array.
+            b: Vector for the array.
                 Needs to be in positive Y-direction. Usually this is only a
                 Vector in x-direction. Some foundries won't allow other Vectors.
             na: Number of elements in direction of `a`
             nb: Number of elements in direction of `b`
 
         Returns:
             The created instance
@@ -1361,50 +1436,32 @@
         if self._locked:
             raise LockedError(self)
         if isinstance(cell, int):
             ci = cell
         else:
             ci = cell.cell_index()
 
-        if dtrans is None:
-            if a is None:
-                ca = self._kdb_cell.insert(kdb.CellInstArray(ci, trans))
-            else:
-                if b is None:
-                    b = kdb.Vector()
-                cast(kdb.DVector, a)
-                cast(kdb.DVector, b)
-                ca = self._kdb_cell.insert(
-                    kdb.CellInstArray(ci, trans, a, b, na, nb)  # type: ignore[arg-type]
-                )
+        if a is None:
+            ca = self._kdb_cell.insert(kdb.CellInstArray(ci, trans))
         else:
-            if a is None:
-                ca = self._kdb_cell.insert(kdb.DCellInstArray(ci, dtrans))
-            else:
-                if b is None:
-                    b = kdb.DVector()
-                cast(kdb.DVector, a)
-                cast(kdb.DVector, b)
-                ca = self._kdb_cell.insert(
-                    kdb.DCellInstArray(
-                        ci, dtrans, a, b, na, nb  # type: ignore[arg-type]
-                    )
-                )
+            if b is None:
+                b = kdb.Vector()
+            ca = self._kdb_cell.insert(kdb.CellInstArray(ci, trans, a, b, na, nb))
         inst = Instance(self.kcl, ca)
         self.insts.append(inst)
         return inst
 
     def _kdb_copy(self) -> kdb.Cell:
         return self._kdb_cell.dup()
 
     def layer(self, *args: Any, **kwargs: Any) -> int:
         """Get the layer info, convenience for `klayout.db.Layout.layer`."""
         return self.kcl.layer(*args, **kwargs)
 
-    def __lshift__(self, cell: "KCell") -> "Instance":
+    def __lshift__(self, cell: KCell) -> Instance:
         """Convenience function for [create_inst][kfactory.kcell.KCell.create_inst].
 
         Args:
             cell: The cell to be added as an instance
         """
         return self.create_inst(cell)
 
@@ -1508,14 +1565,17 @@
     def write(
         self, filename: str | Path, save_options: kdb.SaveLayoutOptions = default_save()
     ) -> None:
         """Write a KCell to a GDS.
 
         See [KCLayout.write][kfactory.kcell.KCLayout.write] for more info.
         """
+        for kcell in (self.kcl[ci] for ci in self.called_cells()):
+            kcell.set_meta_data()
+        self.set_meta_data()
         return self._kdb_cell.write(str(filename), save_options)
 
     @classmethod
     def to_yaml(cls, representer, node):  # type: ignore
         """Internal function to convert the cell to yaml."""
         d = {
             "name": node.name,
@@ -1538,47 +1598,47 @@
             d["insts"] = insts
         if shapes:
             d["shapes"] = shapes
         if len(node.settings) > 0:
             d["settings"] = node.settings
         return representer.represent_mapping(cls.yaml_tag, d)
 
-    def each_inst(self) -> Iterator["Instance"]:
+    def each_inst(self) -> Iterator[Instance]:
         """Iterates over all child instances (which may actually be instance arrays)."""
         yield from (Instance(self.kcl, inst) for inst in self._kdb_cell.each_inst())
 
-    def each_overlapping_inst(self, b: kdb.Box | kdb.DBox) -> Iterator["Instance"]:
+    def each_overlapping_inst(self, b: kdb.Box | kdb.DBox) -> Iterator[Instance]:
         """Gets the instances overlapping the given rectangle."""
         yield from (
             Instance(self.kcl, inst) for inst in self._kdb_cell.each_overlapping_inst(b)
         )
 
-    def each_touching_inst(self, b: kdb.Box | kdb.DBox) -> Iterator["Instance"]:
+    def each_touching_inst(self, b: kdb.Box | kdb.DBox) -> Iterator[Instance]:
         """Gets the instances overlapping the given rectangle."""
         yield from (
             Instance(self.kcl, inst) for inst in self._kdb_cell.each_touching_inst(b)
         )
 
     @overload
     def insert(
-        self, inst: "Instance | kdb.CellInstArray | kdb.DCellInstArray"
-    ) -> "Instance":
+        self, inst: Instance | kdb.CellInstArray | kdb.DCellInstArray
+    ) -> Instance:
         ...
 
     @overload
     def insert(
-        self, inst: "kdb.CellInstArray | kdb.DCellInstArray", property_id: int
-    ) -> "Instance":
+        self, inst: kdb.CellInstArray | kdb.DCellInstArray, property_id: int
+    ) -> Instance:
         ...
 
     def insert(
         self,
-        inst: "Instance | kdb.CellInstArray | kdb.DCellInstArray",
+        inst: Instance | kdb.CellInstArray | kdb.DCellInstArray,
         property_id: int | None = None,
-    ) -> "Instance":
+    ) -> Instance:
         """Inserts a cell instance given by another reference."""
         if self._locked:
             raise LockedError(self)
         if isinstance(inst, Instance):
             return Instance(self.kcl, self._kdb_cell.insert(inst._instance))
         else:
             if not property_id:
@@ -1591,15 +1651,15 @@
     def transform(
         self,
         inst: kdb.Instance,
         trans: kdb.Trans | kdb.DTrans | kdb.ICplxTrans | kdb.DCplxTrans,
         /,
         *,
         no_warn: bool = False,
-    ) -> "Instance":
+    ) -> Instance:
         ...
 
     @overload
     def transform(
         self,
         trans: kdb.Trans | kdb.DTrans | kdb.ICplxTrans | kdb.DCplxTrans,
         /,
@@ -1615,15 +1675,15 @@
         | kdb.DTrans
         | kdb.ICplxTrans
         | kdb.DCplxTrans,
         trans: kdb.Trans | kdb.DTrans | kdb.ICplxTrans | kdb.DCplxTrans | None = None,
         /,
         *,
         no_warn: bool = False,
-    ) -> "Instance | None":
+    ) -> Instance | None:
         """Transforms the instance or cell with the transformation given."""
         config.logger.warning(
             "You are transforming the KCell {}. It is highly discouraged to do this."
             " You probably want to transform an instance instead.",
             self.name,
         )
         if self._locked:
@@ -1634,14 +1694,107 @@
                 self._kdb_cell.transform(
                     inst_or_trans, trans  # type: ignore[arg-type]
                 ),
             )
         else:
             return self._kdb_cell.transform(inst_or_trans)  # type:ignore[arg-type]
 
+    def set_meta_data(self) -> None:
+        """Set metadata of the Cell.
+
+        Currently, ports, settings and info will be set.
+        """
+        for i, port in enumerate(self.ports):
+            if port.name:
+                self.add_meta_info(
+                    kdb.LayoutMetaInfo(
+                        f"kfactory:ports:{i}:name", port.name, None, True
+                    )
+                )
+            self.add_meta_info(
+                kdb.LayoutMetaInfo(
+                    f"kfactory:ports:{i}:layer",
+                    self.kcl.get_info(port.layer).to_s(),
+                    None,
+                    True,
+                )
+            )
+            self.add_meta_info(
+                kdb.LayoutMetaInfo(f"kfactory:ports:{i}:width", port.width, None, True)
+            )
+            self.add_meta_info(
+                kdb.LayoutMetaInfo(
+                    f"kfactory:ports:{i}:port_type", port.port_type, None, True
+                )
+            )
+            if port._trans:
+                self.add_meta_info(
+                    kdb.LayoutMetaInfo(
+                        f"kfactory:ports:{i}:trans", port._trans.to_s(), None, True
+                    )
+                )
+            elif port._dcplx_trans:
+                self.add_meta_info(
+                    kdb.LayoutMetaInfo(
+                        f"kfactory:ports:{i}:dcplx_trans",
+                        port._dcplx_trans.to_s(),
+                        None,
+                        True,
+                    )
+                )
+
+        for name, setting in self.settings.items():
+            self.add_meta_info(
+                kdb.LayoutMetaInfo(f"kfactory:settings:{name}", setting, None, True)
+            )
+        for name, info in self.info.items():
+            self.add_meta_info(
+                kdb.LayoutMetaInfo(f"kfactory:info:{name}", info, None, True)
+            )
+
+    def get_meta_data(self) -> None:
+        """Read metadata from the KLayout Layout object."""
+        port_dict = {}
+        for meta in self.each_meta_info():
+            if meta.name.startswith("kfactory:ports"):
+                i, _type = meta.name.lstrip("kfactory:ports:").split(":")
+                if i not in port_dict:
+                    port_dict[i] = {_type: meta.value}
+                else:
+                    port_dict[i][_type] = meta.value
+            elif meta.name.startswith("kfactory:info"):
+                self.info[meta.name.lstrip("kfactory:info:")] = meta.value
+            elif meta.name.startswith("kfactory:settings"):
+                self.settings[meta.name.lstrip("kfactory:settings:")] = meta.value
+
+        # ports = Ports()
+        self.ports = Ports(self.kcl)
+        for index in sorted(port_dict.keys()):
+            _d = port_dict[index]
+            name = _d.get("name", None)
+            port_type = _d["port_type"]
+            layer = self.kcl.layer(kdb.LayerInfo.from_string(_d["layer"]))
+            width = _d["width"]
+            trans = _d.get("trans", None)
+            dcplx_trans = _d.get("dcplx_trans", None)
+            _port = Port(
+                name=name,
+                width=width,
+                layer=layer,
+                trans=kdb.Trans.R0,
+                kcl=self.kcl,
+                port_type=port_type,
+            )
+            if trans:
+                _port.trans = kdb.Trans.from_s(trans)
+            elif dcplx_trans:
+                _port.dcplx_trans = kdb.DCplxTrans.from_s(dcplx_trans)
+
+            self.add_port(_port, keep_mirror=True)
+
     @property
     def xmin(self) -> int:
         """Returns the x-coordinate of the left edge of the bounding box."""
         return self._kdb_cell.bbox().left
 
     @property
     def ymin(self) -> int:
@@ -1654,14 +1807,251 @@
         return self._kdb_cell.bbox().right
 
     @property
     def ymax(self) -> int:
         """Returns the x-coordinate of the left edge of the bounding box."""
         return self._kdb_cell.bbox().top
 
+    def netlist(self, port_types: tuple[str] = ("optical",)) -> kdb.Netlist:
+        """Return a netlist with this cell as the top cell."""
+        netlist = kdb.Netlist()
+
+        for ci in self.called_cells():
+            self.kcl[ci].circuit(netlist, port_types=port_types)
+
+        self.circuit(netlist, port_types=port_types)
+
+        return netlist
+
+    @cachetools.cached(cache={})
+    def circuit(
+        self, netlist: kdb.Netlist, port_types: tuple[str] = ("optical",)
+    ) -> None:
+        """Create the circuit of the KCell in the given netlist."""
+
+        def port_filter(num_port: tuple[int, Port]) -> bool:
+            return num_port[1].port_type in port_types
+
+        circ = kdb.Circuit()
+        circ.name = self.name
+        circ.cell_index = self.cell_index()
+
+        inst_ports: dict[
+            str, dict[str, list[tuple[int, int, Instance, Port, kdb.SubCircuit]]]
+        ] = {}
+        cell_ports: dict[str, dict[str, list[tuple[int, Port]]]] = {}
+
+        # sort the cell's ports by position and layer
+
+        portnames: set[str] = set()
+
+        for i, port in filter(port_filter, enumerate(self.ports)):
+            _trans = port.trans.dup()
+            _trans.angle = _trans.angle % 2
+            _trans.mirror = False
+            layer_info = self.kcl.get_info(port.layer)
+            layer = f"{layer_info.layer}_{layer_info.datatype}"
+
+            if port.name in portnames:
+                raise ValueError(
+                    "Netlist extraction is not possible with"
+                    f" colliding port names. Duplicate name: {port.name}"
+                )
+
+            v = _trans.disp
+            h = f"{v.x}_{v.y}"
+            if h not in cell_ports:
+                cell_ports[h] = {}
+            if layer not in cell_ports[h]:
+                cell_ports[h][layer] = []
+            cell_ports[h][layer].append((i, port))
+
+            if port.name:
+                portnames.add(port.name)
+
+        # create nets and connect pins for each cell_port
+        for h, layer_dict in cell_ports.items():
+            for layer, _ports in layer_dict.items():
+                net = circ.create_net(
+                    "-".join(_port[1].name or f"{_port[0]}" for _port in _ports)
+                )
+                for i, port in _ports:
+                    pin = circ.create_pin(port.name or f"{i}")
+                    circ.connect_pin(pin, net)
+
+        # sort the ports of all instances by position and layer
+        for i, inst in enumerate(self.insts):
+            name = inst.name or f"{i}_{inst.cell.name}"
+            subc = circ.create_subcircuit(
+                netlist.circuit_by_cell_index(inst.cell_index), name
+            )
+
+            for j, port in filter(port_filter, enumerate(inst.ports)):
+                _trans = port.trans.dup()
+                _trans.angle = _trans.angle % 2
+                _trans.mirror = False
+                v = _trans.disp
+                h = f"{v.x}_{v.y}"
+                layer_info = self.kcl.get_info(port.layer)
+                layer = f"{layer_info.layer}_{layer_info.datatype}"
+                if h not in inst_ports:
+                    inst_ports[h] = {}
+                if layer not in inst_ports[h]:
+                    inst_ports[h][layer] = []
+                inst_ports[h][layer].append((i, j, inst, port, subc))
+
+        # go through each position and layer and connect ports to their matching cell
+        # port or connect the instance ports
+        for h, inst_layer_dict in inst_ports.items():
+            for layer, ports in inst_layer_dict.items():
+                if h in cell_ports and layer in cell_ports[h]:
+                    # connect a cell port to its matching instance port
+                    cellports = cell_ports[h][layer]
+
+                    assert len(cellports) == 1, (
+                        "Netlists with directly connect cell ports"
+                        " are currently not supported"
+                    )
+                    assert len(ports) == 1, (
+                        f"Multiple instance {[port[4] for port in ports]}"
+                        f"ports connected to the cell port {cellports[0]}"
+                        " this is currently not supported and most likely a bug"
+                    )
+
+                    inst_port = ports[0]
+                    port = inst_port[3]
+
+                    port_check(cellports[0][1], port, PortCheck.all_overlap)
+                    subc = inst_port[4]
+                    subc.connect_pin(
+                        subc.circuit_ref().pin_by_name(port.name or str(inst_port[1])),
+                        circ.net_by_name(cellports[0][1].name or f"{cellports[0][0]}"),
+                    )
+                else:
+                    # connect instance ports to each other
+                    name = "-".join(
+                        [
+                            (inst.name or str(i)) + "_" + (port.name or str(j))
+                            for i, j, inst, port, subc in ports
+                        ]
+                    )
+
+                    net = circ.create_net(name)
+                    assert len(ports) <= 2, (
+                        "Optical connection with more than two ports are not supported "
+                        f"{[_port[3] for _port in ports]}"
+                    )
+                    if len(ports) == 2:
+                        port_check(ports[0][3], ports[1][3], PortCheck.all_opposite)
+                        for i, j, inst, port, subc in ports:
+                            subc.connect_pin(
+                                subc.circuit_ref().pin_by_name(port.name or str(j)), net
+                            )
+        netlist.add(circ)
+
+
+class UMKCell:
+    """Make the port able to dynamically give um based info."""
+
+    def __init__(self, parent: KCell):
+        """Constructor, just needs a pointer to the port.
+
+        Args:
+            parent: port that this should be attached to
+        """
+        self.parent = parent
+
+    @property
+    def xmin(self) -> float:
+        """Returns the x-coordinate of the left edge of the bounding box."""
+        return self.parent._kdb_cell.dbbox().left
+
+    @property
+    def ymin(self) -> float:
+        """Returns the x-coordinate of the left edge of the bounding box."""
+        return self.parent._kdb_cell.dbbox().bottom
+
+    @property
+    def xmax(self) -> float:
+        """Returns the x-coordinate of the left edge of the bounding box."""
+        return self.parent._kdb_cell.dbbox().right
+
+    @property
+    def ymax(self) -> float:
+        """Returns the x-coordinate of the left edge of the bounding box."""
+        return self.parent._kdb_cell.dbbox().top
+
+    @overload
+    def create_inst(
+        self,
+        cell: KCell | int,
+        *,
+        trans: kdb.DTrans | kdb.DCplxTrans | kdb.DVector = kdb.DTrans(),
+    ) -> Instance:
+        ...
+
+    @overload
+    def create_inst(
+        self,
+        cell: KCell | int,
+        *,
+        trans: kdb.DTrans | kdb.DCplxTrans | kdb.DVector = kdb.DTrans(),
+        a: kdb.DVector,
+        b: kdb.DVector,
+        na: int = 1,
+        nb: int = 1,
+    ) -> Instance:
+        ...
+
+    def create_inst(
+        self,
+        cell: KCell | int,
+        *,
+        trans: kdb.DTrans | kdb.DCplxTrans | kdb.DVector = kdb.DTrans(),
+        a: kdb.DVector | None = None,
+        b: kdb.DVector | None = None,
+        na: int = 1,
+        nb: int = 1,
+    ) -> Instance:
+        """Add an instance of another KCell.
+
+        Args:
+            cell: The cell to be added
+            trans: The integer transformation applied to the reference
+            a: Vector for the array.
+                Needs to be in positive X-direction. Usually this is only a
+                Vector in x-direction. Some foundries won't allow other Vectors.
+            b: Vector for the array.
+                Needs to be in positive Y-direction. Usually this is only a
+                Vector in x-direction. Some foundries won't allow other Vectors.
+            na: Number of elements in direction of `a`
+            nb: Number of elements in direction of `b`
+
+        Returns:
+            The created instance
+        """
+        if self.parent._locked:
+            raise LockedError(self.parent)
+        if isinstance(cell, int):
+            ci = cell
+        else:
+            ci = cell.cell_index()
+
+        if a is None:
+            ca = self.parent._kdb_cell.insert(kdb.DCellInstArray(ci, trans))
+        else:
+            if b is None:
+                b = kdb.DVector()
+            ca = self.parent._kdb_cell.insert(
+                kdb.DCellInstArray(ci, trans, a, b, na, nb)
+            )
+        inst = Instance(self.parent.kcl, ca)
+        self.parent.insts.append(inst)
+        return inst
+
 
 class Instance:
     """An Instance of a KCell.
 
     An Instance is a reference to a KCell with a transformation.
 
     Attributes:
@@ -1670,16 +2060,16 @@
         kcl: Pointer to the layout object holding the instance
         d: Helper that allows retrieval of instance information in um
     """
 
     yaml_tag = "!Instance"
     _instance: kdb.Instance
     kcl: KCLayout
-    ports: "InstancePorts"
-    d: "UMInstance"
+    ports: InstancePorts
+    d: UMInstance
 
     def __init__(self, kcl: KCLayout, instance: kdb.Instance) -> None:
         """Create an instance from a KLayout Instance."""
         self._instance = instance
         self.kcl = kcl
         self.ports = InstancePorts(self)
         self.d = UMInstance(self)
@@ -1847,25 +2237,25 @@
     ) -> None:
         ...
 
     @overload
     def connect(
         self,
         port: str | Port | None,
-        other: "Instance",
+        other: Instance,
         other_port_name: str | None,
         *,
         mirror: bool = False,
     ) -> None:
         ...
 
     def connect(
         self,
         port: str | Port | None,
-        other: "Instance | Port",
+        other: Instance | Port,
         other_port_name: str | None = None,
         *,
         mirror: bool = False,
         allow_width_mismatch: bool = False,
         allow_layer_mismatch: bool = False,
         allow_type_mismatch: bool = False,
     ) -> None:
@@ -2147,14 +2537,56 @@
         """Mirror the instance at an x-axis."""
         self.parent.transform(kdb.DTrans(2, True, 2 * x, 0))
 
     def mirror_y(self, y: float = 0) -> None:
         """Mirror the instance at an y-axis."""
         self.parent.transform(kdb.DTrans(0, True, 0, 2 * y))
 
+    @property
+    def xmin(self) -> float:
+        """Returns the x-coordinate of the left edge of the bounding box."""
+        return self.parent._instance.dbbox().left
+
+    @xmin.setter
+    def xmin(self, __val: float) -> None:
+        """Moves the instance so that the bbox's left x-coordinate."""
+        self.parent.transform(kdb.DTrans(__val - self.parent.dbbox().left, 0))
+
+    @property
+    def ymin(self) -> float:
+        """Returns the x-coordinate of the left edge of the bounding box."""
+        return self.parent._instance.dbbox().bottom
+
+    @ymin.setter
+    def ymin(self, __val: float) -> None:
+        """Moves the instance so that the bbox's left x-coordinate."""
+        self.parent.transform(
+            kdb.DTrans(0, __val - self.parent._instance.dbbox().bottom)
+        )
+
+    @property
+    def xmax(self) -> float:
+        """Returns the x-coordinate of the left edge of the bounding box."""
+        return self.parent._instance.dbbox().right
+
+    @xmax.setter
+    def xmax(self, __val: float) -> None:
+        """Moves the instance so that the bbox's left x-coordinate."""
+        self.parent.transform(kdb.DTrans(__val - self.parent.dbbox().right, 0))
+
+    @property
+    def ymax(self) -> float:
+        """Returns the x-coordinate of the left edge of the bounding box."""
+        return self.parent._instance.dbbox().top
+
+    @ymax.setter
+    def ymax(self, __val: int) -> None:
+        """Moves the instance so that the bbox's left x-coordinate."""
+        self.parent.transform(kdb.DTrans(0, __val - self.parent._instance.dbbox().top))
+
 
 class Instances:
     """Holder for instances.
 
     Allows retrieval by name or index
     """
 
@@ -2213,15 +2645,15 @@
     _locked: bool
 
     def __init__(self, kcl: KCLayout, ports: Iterable[Port] = []) -> None:
         """Constructor."""
         self._ports: list[Port] = list(ports)
         self.kcl = kcl
 
-    def copy(self) -> "Ports":
+    def copy(self) -> Ports:
         """Get a copy of each port."""
         return Ports(ports=[p.copy() for p in self._ports], kcl=self.kcl)
 
     def contains(self, port: Port) -> bool:
         """Check whether a port is already in the list."""
         return port.hash() in [v.hash() for v in self._ports]
 
@@ -2407,15 +2839,15 @@
         """Convert the ports to a yaml representations."""
         return representer.represent_sequence(
             cls.yaml_tag,
             node._ports,
         )
 
     @classmethod
-    def from_yaml(cls: "type[Ports]", constructor: Any, node: Any) -> "Ports":
+    def from_yaml(cls: type[Ports], constructor: Any, node: Any) -> Ports:
         """Load Ports from a yaml representation."""
         return cls(constructor.construct_sequence(node))
 
 
 class InstancePorts:
     """Ports of an instance.
 
@@ -2491,15 +2923,15 @@
     *,
     set_settings: bool = True,
     set_name: bool = True,
 ) -> Callable[[Callable[KCellParams, KCell]], Callable[KCellParams, KCell]]:
     ...
 
 
-@config.logger.catch
+@config.logger.catch(reraise=True)
 def autocell(
     _func: Callable[KCellParams, KCell] | None = None,
     /,
     *,
     set_settings: bool = True,
     set_name: bool = True,
     check_ports: bool = True,
@@ -2530,27 +2962,31 @@
 
 
 @overload
 def cell(
     *,
     set_settings: bool = True,
     set_name: bool = True,
+    check_ports: bool = True,
+    check_instances: bool = True,
+    snap_ports: bool = True,
 ) -> Callable[[Callable[KCellParams, KCell]], Callable[KCellParams, KCell]]:
     ...
 
 
-@config.logger.catch
+@config.logger.catch(reraise=True)
 def cell(
     _func: Callable[KCellParams, KCell] | None = None,
     /,
     *,
     set_settings: bool = True,
     set_name: bool = True,
     check_ports: bool = True,
     check_instances: bool = True,
+    snap_ports: bool = True,
 ) -> (
     Callable[KCellParams, KCell]
     | Callable[[Callable[KCellParams, KCell]], Callable[KCellParams, KCell]]
 ):
     """Decorator to cache and auto name the celll.
 
     This will use `functools.cache` to cache the function call.
@@ -2562,20 +2998,21 @@
         set_settings: Copy the args & kwargs into the settings dictionary
         set_name: Auto create the name of the cell to the functionname plus a
             string created from the args/kwargs
         check_ports: Check whether there are any non-90° ports in the cell and throw a
             warning if there are
         check_instances: Check for any complex instances. A complex instance is a an
             instance that has a magnification != 1 or non-90° rotation.
+        snap_ports: Snap the centers of the ports onto the grid (only x/y, not angle).
     """
 
     def decorator_autocell(
         f: Callable[KCellParams, KCell]
     ) -> Callable[KCellParams, KCell]:
-        sig = signature(f)
+        sig = inspect.signature(f)
 
         # previously was a KCellCache, but dict should do for most case
         cache: dict[int, Any] = {}
 
         @functools.wraps(f)
         def wrapper_autocell(
             *args: KCellParams.args, **kwargs: KCellParams.kwargs
@@ -2589,29 +3026,30 @@
             params.update(kwargs)
 
             del_parameters: list[str] = []
 
             for key, value in params.items():
                 if isinstance(value, dict):
                     params[key] = dict_to_frozen_set(value)
-                if value == Parameter.empty:
+                if value == inspect.Parameter.empty:
                     del_parameters.append(key)
 
             for param in del_parameters:
                 del params[param]
 
             @cachetools.cached(cache=cache)
             @functools.wraps(f)
             def wrapped_cell(
                 **params: KCellParams.args,
             ) -> KCell:
                 for key, value in params.items():
                     if isinstance(value, frozenset):
                         params[key] = frozenset_to_dict(value)
                 cell = f(**params)
+                dbu = cell.kcl.dbu
                 if cell._locked:
                     # If the cell is locked, it comes from a cache (most likely)
                     # and should be copied first
                     cell = cell.dup()
                 if set_name:
                     name = get_cell_name(f.__name__, **params)
                     cell.name = name
@@ -2619,15 +3057,20 @@
                     cell.settings.update(params)
                 if check_instances:
                     if any(inst.is_complex() for inst in cell.each_inst()):
                         raise ValueError(
                             "Most foundries will not allow off-grid instances. Please "
                             "flatten them or add check_instances=False to the decorator"
                         )
-
+                if snap_ports:
+                    for port in cell.ports:
+                        if port._dcplx_trans:
+                            port.dcplx_trans.disp = port._dcplx_trans.disp.to_itype(
+                                dbu
+                            ).to_dtype(dbu)
                 i = 0
                 for name, setting in cell.settings.items():
                     while cell.property(i) is not None:
                         i += 1
                     if isinstance(setting, KCell):
                         cell.set_property(i, f"{name}: {setting.name}")
                     else:
@@ -2760,16 +3203,14 @@
 ) -> None:
     """Show GDS in klayout."""
     import inspect
 
     delete = False
 
     # Find the file that calls stack
-    # stk = inspect.stack()[-1]
-
     try:
         stk = inspect.getouterframes(inspect.currentframe())
         frame = stk[2]
         name = (
             Path(frame.filename).stem + "_" + frame.function
             if frame.function != "<module>"
             else Path(frame.filename).stem
```

### Comparing `kfactory-0.7.5/src/kfactory/pdk.py` & `kfactory-0.8.0/src/kfactory/pdk.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,108 @@
 """PDK stores layers, enclosures, cell functions ..."""
 
 from __future__ import annotations
 
-import pathlib
-import warnings
-from collections.abc import Callable, Iterable
+from collections.abc import Iterable
 from inspect import getmembers, signature
-from pathlib import Path
 from types import ModuleType
-from typing import Any
 
-from pydantic import BaseModel, Field, validator
+from pydantic import BaseModel, Field
+from pydantic_settings import BaseSettings
 
-from .conf import logger
-from .kcell import KCell, LayerEnum, kcl
-from .technology import LayerStack
-from .typings import CellFactory, CellSpec, PathType
-from .utils.enclosure import KCellEnclosure, LayerEnclosure
-
-cell_settings = ["function", "cell", "settings"]
-enclosure_settings = ["function", "enclosure", "settings"]
-
-constants = {
-    "fiber_array_spacing": 127.0,
-    "fiber_spacing": 50.0,
-    "fiber_input_to_output_spacing": 200.0,
-    "metal_spacing": 10.0,
-}
+from . import kcell as kcell_mod
 
-MaterialSpec = str | float | tuple[float, float] | Callable[[str], float]
+# from .technology import LayerStack
+from .typings import CellFactory, PathType
+from .utils.enclosure import KCellEnclosure, LayerEnclosure
 
 
 def get_cells(
     modules: Iterable[ModuleType], verbose: bool = False
 ) -> dict[str, CellFactory]:
-    """Returns PCells (component functions) from a module or list of modules.
+    """Returns KCells (KCell functions) from a module or list of modules.
 
     Args:
         modules: module or iterable of modules.
         verbose: prints in case any errors occur.
     """
     cells = {}
     for module in modules:
         for t in getmembers(module):
             if callable(t[1]) and t[0] != "partial":
                 try:
                     r = signature(t[1]).return_annotation
-                    if r == KCell or (isinstance(r, str) and r.endswith("KCell")):
+                    if r == kcell_mod.KCell or (
+                        isinstance(r, str) and r.endswith("KCell")
+                    ):
                         cells[t[0]] = t[1]
                 except ValueError:
                     if verbose:
                         print(f"error in {t[0]}")
     return cells
 
 
+class LayerEnclosureModel(BaseModel):
+    """PDK access model for LayerEnclsoures."""
+
+    enclosure_map: dict[str, LayerEnclosure] = Field(default={})
+
+    def __getitem__(self, __key: str) -> LayerEnclosure:
+        """Retrieve element by string key."""
+        return self.enclosure_map[__key]
+
+    def __getattr__(self, __key: str) -> LayerEnclosure:
+        """Retrieve attribute by key."""
+        return self.enclosure_map[__key]
+
+
+class CellModel(BaseModel):
+    """PDK access model for KCell."""
+
+    cell_map: dict[str, kcell_mod.KCell] = Field(default={})
+
+    def __getitem__(self, __key: str) -> kcell_mod.KCell:
+        """Retrieve element by string key."""
+        return self.cell_map[__key]
+
+    def __getattr__(self, __key: str) -> kcell_mod.KCell:
+        """Retrieve attribute by key."""
+        return self.cell_map[__key]
+
+    class Config:
+        """Pydantic Config."""
+
+        arbitrary_types_allowed = True
+
+
+class CellFactoryModel(BaseModel):
+    """PDK access model for KCellFactories."""
+
+    cellfactory_map: dict[str, CellFactory] = Field(default={})
+
+    def __getitem__(self, __key: str) -> CellFactory:
+        """Retrieve element by string key."""
+        return self.cellfactory_map[__key]
+
+    def __getattr__(self, __key: str) -> CellFactory:
+        """Retrieve attribute by key."""
+        return self.cellfactory_map[__key]
+
+    class Config:
+        """Retrieve element by string key."""
+
+        arbitrary_types_allowed = True
+
+
+class Constants(BaseSettings):
+    """Constant Model class."""
+
+    pass
+
+
 class Pdk(BaseModel):
     """Store layers, enclosures, cell functions, simulation_settings ...
 
     only one Pdk can be active at a given time.
 
     Attributes:
         name: PDK name.
@@ -74,179 +119,123 @@
         sparameters_path: to store Sparameters simulations.
         interconnect_cml_path: path to interconnect CML (optional).
         grid_size: in um. Defaults to 1nm.
         constants: dict of constants for the PDK.
 
     """
 
-    name: str
-    layer_enclosures: dict[str, LayerEnclosure] = Field(default_factory=dict)
-    enclosure: KCellEnclosure = Field(default=KCellEnclosure(enclosures=[]))
-
-    cell_factories: dict[str, CellFactory] = Field(default_factory=dict)
-    cells: dict[str, KCell] = Field(default_factory=dict)
-    base_pdk: Pdk | None = None
-    default_decorator: Callable[[KCell], None] | None = None
-    layers: type[LayerEnum]
-    layer_stack: LayerStack | None = None
-    # layer_views: Optional[LayerViews] = None
-    layer_transitions: dict[LayerEnum | tuple[LayerEnum, LayerEnum], CellSpec] = Field(
-        default_factory=dict
-    )
-    sparameters_path: PathType | None = None
-    # modes_path: Optional[Path] = PATH.modes
-    interconnect_cml_path: PathType | None = None
-    constants: dict[str, Any] = constants
+    name: str | None = None
+    kcl: kcell_mod.KCLayout = kcell_mod.kcl
+    layer_enclosures: LayerEnclosureModel
+    enclosure: KCellEnclosure
+
+    cell_factories: CellFactoryModel
+    cells: CellModel
+    layers: type[kcell_mod.LayerEnum]
+    sparameters_path: PathType | None
+    interconnect_cml_path: PathType | None
+    constants: Constants = Field(default_factory=Constants)
 
     class Config:
         """Configuration."""
 
         arbitrary_types_allowed = True
         extra = "allow"
-        fields = {
-            "enclosures": {"exclude": True},
-            "cells": {"exclude": True},
-            "default_decorator": {"exclude": True},
-        }
-
-    class PdkCollection(dict):
-        def __setitem__(self, __key: str, __val: Any) -> None:
-            super().__setitem__(__key, __val)
-            self.__setattr__(__key, __val)
-
-        def update(self, m: dict[str, Any]):
-            super().update(m)
-            for key, val in m.items():
-                self.__setattr__(key, val)
-
-    def __init__(self, **data: Any):
-        """Add LayerLevels automatically for subclassed LayerStacks."""
-        super().__init__(**data)
-        self.kcl = kcl
-
-    @property
-    def grid_size(self) -> float:
-        return self.kcl.dbu
-
-    @grid_size.setter
-    def grid_size(self, value: float) -> None:
-        self.kcl.dbu = value
-
-    @validator("sparameters_path")
-    def is_pathlib_path(cls, path: str | Path) -> Path:
-        return pathlib.Path(path)
-
-    def activate(self) -> None:
-        """Set current pdk to as the active pdk."""
-        logger.info(f"{self.name!r} PDK is now active")
-
-        cell = self.PdkCollection()
-        cell.update(self.cells)
-        self.cells = cell
-
-        cell_factories = self.PdkCollection()
-        cell_factories.update(self.cell_factories)
-        self.cell_factories = cell_factories
-
-        if self.base_pdk:
-            enclosures = self.base_pdk.layer_enclosures
-            enclosures.update(self.layer_enclosures)
-            self.layer_enclosures = enclosures
-
-            cells = self.base_pdk.cells
-            cells.update(self.cells)
-            self.cells.update(cells)
-
-            cell_factories = self.base_pdk.cell_factories
-            cell_factories.update(self.cell_factories)
-            self.cell_factories = cell_factories
-            # layers = self.base_pdk.layers
-            # TODO dynamic creation
-            # class LAYER(BASELAYER):
-            #     b = (a,b)
-
-            if not self.default_decorator:
-                self.default_decorator = self.base_pdk.default_decorator
-        self.kcl.pdk = self
-
-    def register_cells(self, **kwargs: Callable[..., KCell]) -> None:
-        """Register cell factories."""
-        for name, cell in kwargs.items():
-            if not callable(cell):
-                raise ValueError(
-                    f"{cell} is not callable, make sure you register "
-                    "cells functions that return a KCell"
-                )
-            if name in self.cells:
-                warnings.warn(f"Overwriting cell {name!r}")
-
-            self.cells[name] = cell
 
-    def register_enclosures(self, **kwargs: LayerEnclosure) -> None:
-        """Register enclosures factories."""
-        for name, enclosure in kwargs.items():
-            if name in self.layer_enclosures:
-                warnings.warn(f"Overwriting enclosure {name!r}")
-            self.layer_enclosures[name] = enclosure
-
-    def remove_cell(self, name: str) -> None:
-        """Removes cell from a PDK."""
-        if name not in self.cells:
-            raise ValueError(f"{name!r} not in {list(self.cells.keys())}")
-        self.cells.pop(name)
-        logger.info(f"Removed cell {name!r}")
-
-    def get_cell(self, cell: CellSpec, **cell_kwargs: Any) -> KCell:
-        """Returns cell from a cell spec.
+    def __init__(
+        self,
+        name: str | None = None,
+        kcl: kcell_mod.KCLayout = kcell_mod.kcl,
+        layer_enclosures: dict[str, LayerEnclosure]
+        | LayerEnclosureModel = LayerEnclosureModel(),
+        enclosure: KCellEnclosure | None = None,
+        cell_factories: dict[str, CellFactory] | CellFactoryModel = CellFactoryModel(),
+        cells: dict[str, kcell_mod.KCell] | CellModel = CellModel(),
+        layers: type[kcell_mod.LayerEnum] | None = None,
+        sparameters_path: PathType | None = None,
+        interconnect_cml_path: PathType | None = None,
+        constants: type[Constants] | None = None,
+        base_pdk: Pdk | None = None,
+    ) -> None:
+        """Create a new pdk. Can be based on an old PDK.
 
         Args:
-         cell: A CellSpec to get from the Pdk.
-         cell_kwargs: settings for the cell.
+            name: Name of the PDK.
+            kcl: The layout object the pdk should use.
+            layer_enclosures: Additional KCellEnclosures that should be available
+                except the KCellEnclosure
+            enclosure: The standard KCellEnclosure of the PDK.
+            cell_factories: Functions for creating pcells from the PDK.
+            cells: Fixed cells of the PDK.
+            layers: A LayerEnum describing the layerstack of the PDK
+            sparameters_path: Path to the sparameters config file.
+            interconnect_cml_path: Path to the interconnect file.
+            constants: A model containing all the constants related to the PDK.
+            base_pdk: an optional basis of the PDK.
         """
-        return self._get_cell(cell=cell, cells=self.cells, **cell_kwargs)
-
-    def _get_cell(
-        self,
-        cell: CellSpec,
-        cells: dict[str, Callable[..., KCell]],
-        **kwargs: Any,
-    ) -> KCell:
-        """Returns cell from a cell spec."""
-        # cell_names = cells.keys()
-
-        if isinstance(cell, KCell):
-            if kwargs:
-                raise ValueError(f"Cannot apply kwargs {kwargs} to {cell.name!r}")
-            return cell
-        elif callable(cell):
-            return cell(**kwargs)
-        elif isinstance(cell, str):
-            try:
-                cell = cells[cell]
-            except KeyError:
-                cells_ = list(cells.keys())
-                raise ValueError(f"{cell!r} not in PDK {self.name!r} cells: {cells_} ")
-            return cell(**kwargs)
-        else:
-            raise ValueError(
-                "get_cell expects a CellSpec (KCell, CellFactory, "
-                f"string or dict), got {type(cell)}"
+        if isinstance(layer_enclosures, dict):
+            layer_enclosures = LayerEnclosureModel(enclosure_map=layer_enclosures)
+        if isinstance(cell_factories, dict):
+            cell_factories = CellFactoryModel(cellfactory_map=cell_factories)
+        if isinstance(cells, dict):
+            cells = CellModel(cell_map=cells)
+
+        if base_pdk:
+            name = name or base_pdk.name
+            lm = base_pdk.layer_enclosures.enclosure_map.copy()
+            lm.update(layer_enclosures.enclosure_map)
+            layer_enclosures = LayerEnclosureModel(enclosure_map=lm)
+            enclosure = enclosure or base_pdk.enclosure or KCellEnclosure(enclosures=[])
+            cfm = base_pdk.cell_factories.cellfactory_map.copy()
+            cfm.update(cell_factories)
+            cell_factories = CellFactoryModel(cellfactory_map=cfm)
+            cm = base_pdk.cells.cell_map.copy()
+            cm.update(cells.cell_map)
+            cells = CellModel(cell_map=cm)
+            layers = (
+                layers
+                or base_pdk.layers
+                or kcell_mod.LayerEnum(
+                    "LAYER", {}  # type: ignore[arg-type, assignment]
+                )
             )
-
-    def get_enclosure(self, enclosure: str) -> LayerEnclosure:
-        """Returns enclosure from a enclosure spec."""
-        return self.layer_enclosures[enclosure]
-
-    def get_layer(self, layer: Iterable[int] | int | str) -> LayerEnum:
-        """Returns layer from a layer spec."""
-        if isinstance(layer, int):
-            return self.layers(layer)  # type: ignore[call-arg]
-        elif isinstance(layer, str):
-            return self.layers[layer]
+            sparameters_path = sparameters_path or base_pdk.sparameters_path
+            interconnect_cml_path = (
+                interconnect_cml_path or base_pdk.interconnect_cml_path
+            )
+            _constants = constants() if constants else base_pdk.constants.copy()
         else:
-            layer = tuple(layer)
-            if len(layer) > 2:
-                raise ValueError(
-                    "layer can only contain 2 elements like (layer, datatype)."
-                )
-            layer_idx = self.kcl.layer(*layer)
-            return self.layers(layer_idx)  # type: ignore[call-arg]
+            name = name
+            layer_enclosures = layer_enclosures
+            enclosure = enclosure or KCellEnclosure(enclosures=[])
+            cell_factories = cell_factories
+            layers = layers or kcell_mod.LayerEnum(
+                "LAYER", {}  # type: ignore[arg-type, assignment]
+            )
+            sparameters_path = sparameters_path
+            interconnect_cml_path = interconnect_cml_path
+            _constants = constants() if constants else Constants()
+
+        super().__init__(
+            name=name,
+            kcl=kcl,
+            layer_enclosures=layer_enclosures,
+            enclosure=enclosure,
+            cell_factories=cell_factories,
+            cells=cells,
+            layers=layers,
+            sparameters_path=sparameters_path,
+            interconnect_cml_path=interconnect_cml_path,
+            constants=_constants,
+        )
+
+    def kcell(
+        self, name: str | None = None, ports: kcell_mod.Ports | None = None
+    ) -> kcell_mod.KCell:
+        """Create a new cell based ont he pdk's layout object."""
+        return kcell_mod.KCell(name=name, kcl=self.kcl, ports=ports)
+
+    def layer_enum(
+        self, name: str, layers: dict[str, tuple[int, int]]
+    ) -> kcell_mod.LayerEnum:
+        """Create a new LAYER enum based on the pdk's kcl."""
+        return kcell_mod.LayerEnum(name, layers, kcl=self.kcl)  # type: ignore[arg-type]
```

### Comparing `kfactory-0.7.5/src/kfactory/placer.py` & `kfactory-0.8.0/src/kfactory/placer.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.5/src/kfactory/port.py` & `kfactory-0.8.0/src/kfactory/port.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.5/src/kfactory/routing/electrical.py` & `kfactory-0.8.0/src/kfactory/routing/electrical.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.5/src/kfactory/routing/manhattan.py` & `kfactory-0.8.0/src/kfactory/routing/manhattan.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.5/src/kfactory/routing/optical.py` & `kfactory-0.8.0/src/kfactory/routing/optical.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.5/src/kfactory/typings.py` & `kfactory-0.8.0/src/kfactory/typings.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.5/src/kfactory/utils/__init__.py` & `kfactory-0.8.0/src/kfactory/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.5/src/kfactory/utils/enclosure.py` & `kfactory-0.8.0/src/kfactory/utils/enclosure.py`

 * *Files 0% similar despite different names*

```diff
@@ -1133,15 +1133,14 @@
     #                 kdb.Box(0, -half_width, half_width, half_width)
     #             ).transformed(port.dcplx_trans.to_itrans(port.kcl.dbu))
     #         )
 
     class Config:
         """pydantic config."""
 
-        allow_mutation = False
         arbitrary_types_allowed = True
 
 
 class RegionTilesOperator(kdb.TileOutputReceiver):
     """Region collector. Just getst the tile and inserts it into the target cell.
 
     As it can be used multiple times for the same tile, it needs to merge when
```

### Comparing `kfactory-0.7.5/src/kfactory/utils/fill.py` & `kfactory-0.8.0/src/kfactory/utils/fill.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.5/src/kfactory/utils/simplify.py` & `kfactory-0.8.0/src/kfactory/utils/simplify.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.5/src/kfactory/utils/violations.py` & `kfactory-0.8.0/src/kfactory/utils/violations.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.5/src/kfactory/widgets/interactive.py` & `kfactory-0.8.0/src/kfactory/widgets/interactive.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.5/src/kfactory.egg-info/PKG-INFO` & `kfactory-0.8.0/src/kfactory.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: kfactory
-Version: 0.7.5
+Version: 0.8.0
 Summary: KLayout API implementation of gdsfactory
 Author-email: gdsfactory community <contact@gdsfactory.com>
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: git
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: ci
 Provides-Extra: ipy
 License-File: LICENSE
 
-# KFactory 0.7.5
+# KFactory 0.8.0
 
 Kfactory is a [gdsfactory](https://github.com/gdsfactory/gdsfactory)-like tool. It is built with [KLayout](https://klayout.de) as a backend instead of gdstk, but aims to offer the similar featuers.
 
 | :exclamation:  KFactory is still experimental, expect API changes without notice (even though we try to keep it to a minimum!)   |
 |---------------------------------------------------------------------------------------------------------------------------------|
 
-It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.7.5` for example.
+It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.8.0` for example.
 
 Features similar to gdsfactory:
 
 - [x] Cells & decorator for caching & storing cells
 - [x] Simple routing (point to point and simpl bundle routes for electrical routes)
 - [x] Basic cells like euler/circular bends, taper, waveguide
 - [x] Path extrusion (no interface with CrossSections)
```

### Comparing `kfactory-0.7.5/src/kfactory.egg-info/SOURCES.txt` & `kfactory-0.8.0/src/kfactory.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -29,14 +29,30 @@
 docs/source/_static/complex.png
 docs/source/_static/klive.webm
 docs/source/_static/waveguide.png
 docs/source/notebooks/00_geometry.py
 docs/source/notebooks/01_references.py
 docs/source/notebooks/02_DRC.py
 docs/source/notebooks/03_Enclosures.py
+gds/gds_ref/bend_circular.gds
+gds/gds_ref/bend_circular_W1_R10_LWG_EWGSTD_A180_AS1.gds
+gds/gds_ref/bend_circular_W1_R10_LWG_EWGSTD_A90_AS1.gds
+gds/gds_ref/bend_circular_W1_R10_LWG_EWGSTD_T180_TS1.gds
+gds/gds_ref/bend_circular_W1_R10_LWG_EWGSTD_T90_TS1.gds
+gds/gds_ref/bend_euler.gds
+gds/gds_ref/bend_euler_W1_R10_LWG_EWGSTD_A180_R150.gds
+gds/gds_ref/bend_euler_W1_R10_LWG_EWGSTD_A90_R150.gds
+gds/gds_ref/bend_euler_W1_R10_LWG_EWGSTD_T180_R150.gds
+gds/gds_ref/bend_euler_W1_R10_LWG_EWGSTD_T90_R150.gds
+gds/gds_ref/bend_s.gds
+gds/gds_ref/bend_s_euler.gds
+gds/gds_ref/straight_W500_L1000_LWG_EWGSTD.gds
+gds/gds_ref/taper.gds
+gds/gds_ref/waveguide.gds
+gds/gds_ref/waveguide_W500_L1000_LWG_EWGSTD.gds
 src/kfactory/__init__.py
 src/kfactory/conf.py
 src/kfactory/kcell.py
 src/kfactory/pdk.py
 src/kfactory/placer.py
 src/kfactory/port.py
 src/kfactory/py.typed
@@ -46,43 +62,39 @@
 src/kfactory.egg-info/dependency_links.txt
 src/kfactory.egg-info/requires.txt
 src/kfactory.egg-info/top_level.txt
 src/kfactory/cells/__init__.py
 src/kfactory/cells/bezier.py
 src/kfactory/cells/circular.py
 src/kfactory/cells/euler.py
+src/kfactory/cells/straight.py
 src/kfactory/cells/taper.py
-src/kfactory/cells/waveguide.py
 src/kfactory/cells/dbu/__init__.py
+src/kfactory/cells/dbu/straight.py
 src/kfactory/cells/dbu/taper.py
-src/kfactory/cells/dbu/waveguide.py
 src/kfactory/routing/__init__.py
 src/kfactory/routing/electrical.py
 src/kfactory/routing/manhattan.py
 src/kfactory/routing/optical.py
 src/kfactory/technology/__init__.py
-src/kfactory/technology/color_utils.py
-src/kfactory/technology/klayout_tech.py
 src/kfactory/technology/layer_map.py
-src/kfactory/technology/layer_stack.py
-src/kfactory/technology/layer_views.py
-src/kfactory/technology/xml_utils.py
-src/kfactory/technology/yaml_utils.py
 src/kfactory/utils/__init__.py
 src/kfactory/utils/enclosure.py
 src/kfactory/utils/fill.py
 src/kfactory/utils/simplify.py
 src/kfactory/utils/violations.py
 src/kfactory/widgets/__init__.py
 src/kfactory/widgets/interactive.py
 tests/conftest.py
 tests/test_cell.py
 tests/test_cells.py
 tests/test_cplxcells.py
 tests/test_enclosure.py
 tests/test_extrude.py
+tests/test_meta.py
+tests/test_netlist.py
 tests/test_pdk.py
 tests/test_ports.py
 tests/test_rename.py
 tests/test_routing.py
 tests/test_shapes.py
 tests/test_spiral.py
```

### Comparing `kfactory-0.7.5/src/kfactory.egg-info/requires.txt` & `kfactory-0.8.0/src/kfactory.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 klayout>=0.28.3
 scipy
 ruamel.yaml
 cachetools>=5.2.0
-pydantic
+pydantic>=2.0b2
+pydantic-settings>=2.0b1
 loguru
 tomli
 
 [ci]
 flake8
 flake8-pyproject
 pytest
```

### Comparing `kfactory-0.7.5/tests/conftest.py` & `kfactory-0.8.0/tests/conftest.py`

 * *Files 25% similar despite different names*

```diff
@@ -19,55 +19,55 @@
 
 @pytest.fixture
 def wg_enc(LAYER):
     return kf.utils.LayerEnclosure(name="WGSTD", sections=[(LAYER.WGCLAD, 0, 2000)])
 
 
 @pytest.fixture
-def waveguide_factory(LAYER, wg_enc):
-    return partial(kf.cells.dbu.waveguide, layer=LAYER.WG, enclosure=wg_enc)
+def straight_factory(LAYER, wg_enc):
+    return partial(kf.cells.dbu.straight, layer=LAYER.WG, enclosure=wg_enc)
 
 
 @pytest.fixture
-def waveguide(LAYER, wg_enc) -> kf.KCell:
-    return kf.cells.waveguide.waveguide(
+def straight(LAYER, wg_enc) -> kf.KCell:
+    return kf.cells.straight.straight(
         width=0.5, length=1, layer=LAYER.WG, enclosure=wg_enc
     )
 
 
 @pytest.fixture
-def waveguide_blank(LAYER):
-    return kf.cells.waveguide.waveguide(width=0.5, length=1, layer=LAYER.WG)
+def straight_blank(LAYER):
+    return kf.cells.straight.straight(width=0.5, length=1, layer=LAYER.WG)
 
 
 @pytest.fixture
 def bend90(LAYER, wg_enc) -> kf.KCell:
     return kf.cells.circular.bend_circular(
-        width=1, radius=10, layer=LAYER.WG, enclosure=wg_enc, theta=90
+        width=1, radius=10, layer=LAYER.WG, enclosure=wg_enc, angle=90
     )
 
 
 @pytest.fixture
 def bend180(LAYER, wg_enc) -> kf.KCell:
     return kf.cells.circular.bend_circular(
-        width=1, radius=10, layer=LAYER.WG, enclosure=wg_enc, theta=180
+        width=1, radius=10, layer=LAYER.WG, enclosure=wg_enc, angle=180
     )
 
 
 @pytest.fixture
 def bend90_euler(LAYER, wg_enc) -> kf.KCell:
     return kf.cells.euler.bend_euler(
-        width=1, radius=10, layer=LAYER.WG, enclosure=wg_enc, theta=90
+        width=1, radius=10, layer=LAYER.WG, enclosure=wg_enc, angle=90
     )
 
 
 @pytest.fixture
 def bend180_euler(LAYER, wg_enc) -> kf.KCell:
     return kf.cells.euler.bend_euler(
-        width=1, radius=10, layer=LAYER.WG, enclosure=wg_enc, theta=180
+        width=1, radius=10, layer=LAYER.WG, enclosure=wg_enc, angle=180
     )
 
 
 @pytest.fixture
 def taper(LAYER, wg_enc) -> kf.KCell:
     c = kf.cells.taper.taper(
         width1=0.5,
@@ -89,39 +89,41 @@
         layer=LAYER.WG,
         width=1000,
         port_type="optical",
     )
 
 
 @pytest.fixture
-def cells(bend90, bend180, bend90_euler, taper, waveguide) -> list[kf.KCell]:
+def cells(bend90, bend180, bend90_euler, taper, straight) -> list[kf.KCell]:
     return [
         bend90,
         bend180,
         bend90_euler,
         taper,
-        waveguide,
+        straight,
     ]
 
 
 @pytest.fixture
-def pdk(LAYER, waveguide_factory, wg_enc):
+def pdk(LAYER, straight_factory, wg_enc):
     pdk = kf.pdk.Pdk(
         layers=LAYER,
         name="TEST_PDK",
         cell_factories={
-            "wg": waveguide_factory,
+            "wg": straight_factory,
             "bend": kf.cells.circular.bend_circular,
             "bend_euler": kf.cells.euler.bend_euler,
             "taper": kf.cells.taper.taper,
             "bezier": kf.cells.bezier.bend_s,
+            "straight": straight_factory,
         },
+        layer_enclosures={"wg": wg_enc},
     )
-    pdk.register_cells(waveguide=waveguide_factory)
-    pdk.register_enclosures(wg=wg_enc)
-    pdk.activate()
+    # pdk.register_cells(straight=straight_factory)
+    # pdk.register_enclosures(wg=wg_enc)
+    # pdk.activate()
     return pdk
 
 
 # @pytest.fixture
 # def wg():
 #     return LAYER.WG
```

### Comparing `kfactory-0.7.5/tests/test_cells.py` & `kfactory-0.8.0/tests/test_cells.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,41 +18,41 @@
     WG = (1, 0)
     WGCLAD = (111, 0)
 
 
 wg_enc = kf.utils.LayerEnclosure(name="WGSTD", sections=[(LAYER.WGCLAD, 0, 2000)])
 
 
-def waveguide() -> kf.KCell:
-    return kf.cells.waveguide.waveguide(
+def straight() -> kf.KCell:
+    return kf.cells.straight.straight(
         width=0.5, length=1, layer=LAYER.WG, enclosure=wg_enc
     )
 
 
 def bend90() -> kf.KCell:
     return kf.cells.circular.bend_circular(
-        width=1, radius=10, layer=LAYER.WG, enclosure=wg_enc, theta=90
+        width=1, radius=10, layer=LAYER.WG, enclosure=wg_enc, angle=90
     )
 
 
 def bend180() -> kf.KCell:
     return kf.cells.circular.bend_circular(
-        width=1, radius=10, layer=LAYER.WG, enclosure=wg_enc, theta=180
+        width=1, radius=10, layer=LAYER.WG, enclosure=wg_enc, angle=180
     )
 
 
 def bend90_euler() -> kf.KCell:
     return kf.cells.euler.bend_euler(
-        width=1, radius=10, layer=LAYER.WG, enclosure=wg_enc, theta=90
+        width=1, radius=10, layer=LAYER.WG, enclosure=wg_enc, angle=90
     )
 
 
 def bend180_euler() -> kf.KCell:
     return kf.cells.euler.bend_euler(
-        width=1, radius=10, layer=LAYER.WG, enclosure=wg_enc, theta=180
+        width=1, radius=10, layer=LAYER.WG, enclosure=wg_enc, angle=180
     )
 
 
 def taper() -> kf.KCell:
     c = kf.cells.taper.taper(
         width1=0.5,
         width2=1,
@@ -67,15 +67,15 @@
 
 cells = dict(
     bend90=bend90,
     bend180=bend180,
     bend180_euler=bend180_euler,
     bend90_euler=bend90_euler,
     taper=taper,
-    waveguide=waveguide,
+    straight=straight,
 )
 
 cell_names = set(cells.keys())
 
 
 @pytest.fixture(params=cell_names, scope="function")
 def cell_name(request):
@@ -93,16 +93,16 @@
         gds_ref.mkdir(parents=True, exist_ok=True)
         run_cell.write(str(ref_file))
         raise FileNotFoundError(f"GDS file not found. Saving it to {ref_file}")
     kcl_ref = kf.KCLayout()
     kcl_ref.read(gds_ref / f"{cell.name}.gds")
     ref_cell = kcl_ref[kcl_ref.top_cell().name]
 
-    for layer in kcl_ref.layer_infos():
-        layer = kcl_ref.layer(layer)
+    for layerinfo in kcl_ref.layer_infos():
+        layer = kcl_ref.layer(layerinfo)
         region_run = kdb.Region(run_cell.begin_shapes_rec(layer))
         region_ref = kdb.Region(ref_cell.begin_shapes_rec(layer))
 
         region_diff = region_run - region_ref
 
         if not region_diff.is_empty():
             layer_tuple = kcl_ref.layer_infos()[layer]
@@ -115,15 +115,17 @@
             c_ref.shapes(layer).insert(region_ref)
             c_xor.shapes(layer).insert(region_xor)
             c << c_run
             c << c_ref
             c << c_xor
             c.show()
 
-            print(f"Differences found in {cell!r} on layer {layer_tuple}")
+            kf.config.logger.critical(
+                f"Differences found in {cell!r} on layer {layer_tuple}"
+            )
             val = input("Save current GDS as new reference (Y)? [Y/n]")
             if not val.upper().startswith("N"):
                 logger.info(f"replacing file {str(ref_file)!r}")
                 run_cell.write(ref_file.name)
 
             raise GeometryDifference(
                 f"Differences found in {cell!r} on layer {layer_tuple}"
```

### Comparing `kfactory-0.7.5/tests/test_cplxcells.py` & `kfactory-0.8.0/tests/test_cplxcells.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.5/tests/test_enclosure.py` & `kfactory-0.8.0/tests/test_enclosure.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
                 (LAYER.WGCLAD, -5, -3),
                 (LAYER.WGCLAD, -4, -2),
                 (LAYER.WGCLAD, -2, 1),
             ]
         )
 
 
-def test_pdkenclosure(LAYER: kf.LayerEnum, waveguide_blank: kf.KCell) -> None:
+def test_pdkenclosure(LAYER: kf.LayerEnum, straight_blank: kf.KCell) -> None:
     c = kf.KCell("wg_slab")
 
     wg_box = kf.kdb.Box(10000, 500)
     c.shapes(LAYER.WG).insert(wg_box)
     c.shapes(LAYER.WGCLAD).insert(wg_box.enlarged(0, 2500))
     c.create_port(
         trans=kf.kdb.Trans(0, False, wg_box.right, 0),
```

### Comparing `kfactory-0.7.5/tests/test_extrude.py` & `kfactory-0.8.0/tests/test_extrude.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.5/tests/test_pdk.py` & `kfactory-0.8.0/tests/test_pdk.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import kfactory as kf
 
 import pytest
 
 
 def test_get_cell(pdk: kf.pdk.Pdk):
-    pdk.get_cell("waveguide", width=1000, length=10000)
+    pdk.cell_factories["straight"](width=1000, length=10000)
+    pdk.cell_factories.straight(width=1000, length=10000)
 
 
 def test_get_enclosure(pdk: kf.pdk.Pdk):
-    pdk.get_enclosure("wg")
+    pdk.layer_enclosures["wg"]
+    pdk.layer_enclosures.wg
 
 
 def test_cell_factory(pdk: kf.pdk.Pdk):
     assert isinstance(pdk.cell_factories.taper(2, 1, 10, 0), kf.KCell)
 
 
 def test_get_layer(pdk: kf.pdk.Pdk, LAYER: kf.LayerEnum):
-    assert pdk.get_layer((1, 0)) == LAYER.WG
-    assert pdk.get_layer(0) == LAYER.WG
-    assert pdk.get_layer("WG") == LAYER.WG
+    assert pdk.layers(pdk.kcl.layer(1, 0)) == LAYER.WG
+    assert pdk.layers(0) == LAYER.WG
+    assert pdk.layers["WG"] == LAYER.WG
 
     with pytest.raises(ValueError):
-        pdk.get_layer((1, 0, 0))
+        pdk.layers((1, 0))
```

### Comparing `kfactory-0.7.5/tests/test_ports.py` & `kfactory-0.8.0/tests/test_ports.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import kfactory as kf
 import pytest
 import re
 
 
 @kf.cell
-def waveguide(width: int, length: int, layer: int) -> kf.KCell:
+def straight(width: int, length: int, layer: int) -> kf.KCell:
     c = kf.KCell()
 
     c.shapes(layer).insert(kf.kdb.Box(0, -width // 2, length, width // 2))
 
     c.create_port(
         name="o1", trans=kf.kdb.Trans(2, False, 0, 0), width=width, layer=layer
     )
@@ -16,15 +16,15 @@
         name="o2", trans=kf.kdb.Trans(0, False, length, 0), width=width, layer=layer
     )
     return c
 
 
 @pytest.fixture()
 def wg(LAYER):
-    return waveguide(1000, 20000, LAYER.WG)
+    return straight(1000, 20000, LAYER.WG)
 
 
 @pytest.fixture()
 @kf.cell
 def wg_floating_off_grid(LAYER):
     with pytest.raises(AssertionError):
         c = kf.KCell()
@@ -48,43 +48,43 @@
         c.add_port(p2)
 
         kf.config.logfilter.regex = None
 
     return c
 
 
-def test_waveguide(LAYER):
-    waveguide(1000, 20000, LAYER.WG)
+def test_straight(LAYER):
+    straight(1000, 20000, LAYER.WG)
 
 
 def test_settings(LAYER):
-    c = waveguide(1000, 20000, LAYER.WG)
+    c = straight(1000, 20000, LAYER.WG)
 
     assert c.settings["length"] == 20000
     assert c.settings["width"] == 1000
-    assert c.name == "waveguide_W1000_L20000_LWG"
+    assert c.name == "straight_W1000_L20000_LWG"
 
 
 def test_connect_cplx_port(LAYER):
     c = kf.KCell()
-    wg1 = c << waveguide(1000, 20000, LAYER.WG)
+    wg1 = c << straight(1000, 20000, LAYER.WG)
     port = kf.kcell.Port(
         dwidth=1,
         layer=LAYER.WG,
         name="cplxp1",
         dcplx_trans=kf.kdb.DCplxTrans(1, 30, False, 5, 10),
     )
     wg1.connect("o1", port)
 
 
 def test_connect_cplx_inst(LAYER):
     c = kf.KCell()
 
-    wg1 = c << waveguide(1000, 20000, LAYER.WG)
-    wg2 = c << waveguide(1000, 20000, LAYER.WG)
+    wg1 = c << straight(1000, 20000, LAYER.WG)
+    wg2 = c << straight(1000, 20000, LAYER.WG)
     wg1.transform(kf.kdb.DCplxTrans(1, 30, False, 5, 10))
     wg2.connect("o1", wg1, "o2")
     kf.config.logfilter.regex = f"Port ({re.escape(str(wg1.ports['o1']))}|{re.escape(str(wg2.ports['o2']))}) is not an integer based port, converting to integer based"
 
     c.add_port(wg1.ports["o1"])
     c.add_port(wg2.ports["o2"])
```

### Comparing `kfactory-0.7.5/tests/test_rename.py` & `kfactory-0.8.0/tests/test_rename.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     )
 
     assert [p.name for p in port_list] == [
         f"o{i+1}" for i in inds_east + inds_north + inds_west + inds_south
     ]
 
 
-def test_rename_orientatioin() -> None:
+def test_rename_orientation() -> None:
     cell = port_tests(port.rename_by_direction)
 
     dir_names = {0: "E", 1: "N", 2: "W", 3: "S"}
 
     port_list = cell.ports._ports
 
     names = (
@@ -108,12 +108,9 @@
     c2 = kf.KCell(kcl=kcl)
     c2.create_port(
         trans=kf.kdb.Trans(2, False, 0, 0), width=1000, layer=kcl.layer(1, 0)
     )
     c2.create_port(trans=kf.kdb.Trans(), width=1000, layer=kcl.layer(1, 0))
     c2.autorename_ports()
 
-    print(c1.ports)
-    print(c2.ports)
-
     assert c1.ports[0].name == "o1"
     assert c2.ports[0].name == "W0"
```

### Comparing `kfactory-0.7.5/tests/test_routing.py` & `kfactory-0.8.0/tests/test_routing.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,27 +11,27 @@
         5000,
         0,
     ],
 )
 def test_route_straight(
     x: int,
     bend90: kf.KCell,
-    waveguide_factory: Callable[..., kf.KCell],
+    straight_factory: Callable[..., kf.KCell],
     LAYER: kf.LayerEnum,
     optical_port: kf.Port,
 ) -> None:
     c = kf.KCell()
     p1 = optical_port.copy()
     p2 = optical_port.copy()
     p2.trans = kf.kdb.Trans(2, False, x, 0)
     kf.routing.optical.route(
         c,
         p1,
         p2,
-        straight_factory=waveguide_factory,
+        straight_factory=straight_factory,
         bend90_cell=bend90,
     )
 
 
 @pytest.mark.parametrize(
     "x,y,angle2",
     [
@@ -45,15 +45,15 @@
         (500, 30000, 3),
         (-10000, 30000, 3),
         (0, 0, 2),
     ],
 )
 def test_route_bend90(
     bend90: kf.KCell,
-    waveguide_factory: Callable[..., kf.KCell],
+    straight_factory: Callable[..., kf.KCell],
     LAYER: kf.LayerEnum,
     optical_port: kf.Port,
     x: int,
     y: int,
     angle2: int,
 ) -> None:
     c = kf.KCell()
@@ -63,15 +63,15 @@
     b90r = abs(bend90.ports._ports[0].x - bend90.ports._ports[1].x)
     if abs(x) < b90r or abs(y) < b90r:
         kf.config.logfilter.regex = f"Potential collision in routing due to small distance between the port in relation to bend radius x={x}/{b90r}, y={y}/{b90r}"
     kf.routing.optical.route(
         c,
         p1,
         p2,
-        straight_factory=waveguide_factory,
+        straight_factory=straight_factory,
         bend90_cell=bend90,
     )
 
     kf.config.logfilter.regex = None
 
 
 @pytest.mark.parametrize(
@@ -80,15 +80,15 @@
         (40000, 40000, 2),
         (20000, 20000, 3),
         (10000, 10000, 3),
     ],
 )
 def test_route_bend90_euler(
     bend90_euler: kf.KCell,
-    waveguide_factory: Callable[..., kf.KCell],
+    straight_factory: Callable[..., kf.KCell],
     LAYER: kf.LayerEnum,
     optical_port: kf.Port,
     x: int,
     y: int,
     angle2: int,
 ) -> None:
     c = kf.KCell()
@@ -98,11 +98,11 @@
     b90r = abs(bend90_euler.ports._ports[0].x - bend90_euler.ports._ports[1].x)
     if abs(x) < b90r or abs(y) < b90r:
         kf.config.logfilter.regex = f"Potential collision in routing due to small distance between the port in relation to bend radius x={x}/{b90r}, y={y}/{b90r}"
     kf.routing.optical.route(
         c,
         p1,
         p2,
-        straight_factory=waveguide_factory,
+        straight_factory=straight_factory,
         bend90_cell=bend90_euler,
     )
     kf.config.logfilter.regex = None
```

### Comparing `kfactory-0.7.5/tests/test_spiral.py` & `kfactory-0.8.0/tests/test_spiral.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 
 def bend_circular(
     width: int,
     radius: int,
     layer: int,
     enclosure: Optional[kf.utils.LayerEnclosure] = None,
-    theta: int = 90,
-    theta_step: float = 1,
+    angle: int = 90,
+    angle_step: float = 1,
 ) -> kf.KCell:
     """Circular radius bend
 
     Args:
         width: Width in database units
         radius: Radius in database units
         layer: Layer index of the target layer
@@ -25,28 +25,28 @@
     """
 
     c = kf.KCell()
     r = radius * c.kcl.dbu
     backbone = [
         kf.kdb.DPoint(x, y)
         for x, y in [
-            [np.sin(_theta / 180 * np.pi) * r, (-np.cos(_theta / 180 * np.pi) + 1) * r]
-            for _theta in np.linspace(
-                0, theta, int(theta // theta_step + 0.5), endpoint=True
+            [np.sin(_angle / 180 * np.pi) * r, (-np.cos(_angle / 180 * np.pi) + 1) * r]
+            for _angle in np.linspace(
+                0, angle, int(angle // angle_step + 0.5), endpoint=True
             )
         ]
     ]
 
-    kf.utils.extrude_path(c, layer, backbone, width, enclosure, 0, theta)
+    kf.utils.extrude_path(c, layer, backbone, width, enclosure, 0, angle)
 
     c.create_port(
         name="W0", trans=kf.kdb.Trans(2, False, 0, 0), width=width, layer=layer
     )
 
-    match theta:
+    match angle:
         case 90:
             c.create_port(
                 name="N0",
                 trans=kf.kdb.Trans(1, False, radius, radius),
                 width=width,
                 layer=layer,
             )
@@ -62,16 +62,16 @@
 
 
 def dbend_circular(
     width: float,
     radius: float,
     layer: kf.kcell.LayerEnum,
     enclosure: Optional[kf.utils.LayerEnclosure] = None,
-    theta: float = 90,
-    theta_step: float = 1,
+    angle: float = 90,
+    angle_step: float = 1,
 ) -> kf.KCell:
     """Circular radius bend
 
     Args:
         width: Width in database units
         radius: Radius in database units
         layer: Layer index of the target layer
@@ -81,28 +81,28 @@
     """
 
     c = kf.KCell()
     r = radius
     backbone = [
         kf.kdb.DPoint(x, y)
         for x, y in [
-            [np.sin(_theta / 180 * np.pi) * r, (-np.cos(_theta / 180 * np.pi) + 1) * r]
-            for _theta in np.linspace(
-                0, theta, int(theta // theta_step + 0.5), endpoint=True
+            [np.sin(_angle / 180 * np.pi) * r, (-np.cos(_angle / 180 * np.pi) + 1) * r]
+            for _angle in np.linspace(
+                0, angle, int(angle // angle_step + 0.5), endpoint=True
             )
         ]
     ]
-    kf.utils.extrude_path(c, layer, backbone, width, enclosure, 0, theta)
+    kf.utils.extrude_path(c, layer, backbone, width, enclosure, 0, angle)
     dp1 = kf.kcell.Port(
         dwidth=width, layer=layer, name="W0", dcplx_trans=kf.kdb.DCplxTrans.R180
     )
     warnings.filterwarnings("ignore")
     c.add_port(dp1)
 
-    match theta:
+    match angle:
         case 90:
             dp2 = kf.Port(
                 name="N0",
                 layer=layer,
                 dwidth=width,
                 dcplx_trans=kf.kdb.DCplxTrans(1, 90, False, radius, radius),
             )
```

