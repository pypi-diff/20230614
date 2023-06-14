# Comparing `tmp/plopp-23.5.0.tar.gz` & `tmp/plopp-23.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plopp-23.5.0.tar", last modified: Fri Jun  2 13:20:16 2023, max compression
+gzip compressed data, was "plopp-23.5.1.tar", last modified: Wed Jun 14 08:54:03 2023, max compression
```

## Comparing `plopp-23.5.0.tar` & `plopp-23.5.1.tar`

### file list

```diff
@@ -1,199 +1,200 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.969053 plopp-23.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.949051 plopp-23.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-06-02 13:20:03.000000 plopp-23.5.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.949051 plopp-23.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     1428 2023-06-02 13:20:03.000000 plopp-23.5.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2093 2023-06-02 13:20:03.000000 plopp-23.5.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3569 2023-06-02 13:20:03.000000 plopp-23.5.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (122)      266 2023-06-02 13:20:03.000000 plopp-23.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1775 2023-06-02 13:20:03.000000 plopp-23.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-06-02 13:20:03.000000 plopp-23.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1866 2023-06-02 13:20:16.969053 plopp-23.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1122 2023-06-02 13:20:03.000000 plopp-23.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.949051 plopp-23.5.0/conda/
--rw-r--r--   0 runner    (1001) docker     (122)      878 2023-06-02 13:20:03.000000 plopp-23.5.0/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.949051 plopp-23.5.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.949051 plopp-23.5.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)   137750 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/_static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.949051 plopp-23.5.0/docs/_static/gallery/
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/_static/gallery/README.txt
--rw-r--r--   0 runner    (1001) docker     (122)    18766 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/_static/gallery/scatter3d-with-slider-thumbnail.png
--rw-r--r--   0 runner    (1001) docker     (122)    66718 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/_static/gallery/scatter3d-with-threshold-thumbnail.png
--rw-r--r--   0 runner    (1001) docker     (122)    76253 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/_static/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.949051 plopp-23.5.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (122)      600 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/_templates/scipp-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/_templates/scipp-module-template.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.949051 plopp-23.5.0/docs/_templates/sections/
--rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/_templates/sections/header-article.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.949051 plopp-23.5.0/docs/about/
--rw-r--r--   0 runner    (1001) docker     (122)     1137 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/about/about.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/about/faq.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.953051 plopp-23.5.0/docs/about/reference/
--rw-r--r--   0 runner    (1001) docker     (122)      361 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/about/reference/matplotlib.rst
--rw-r--r--   0 runner    (1001) docker     (122)      241 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/about/reference/plotly.rst
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/about/reference/pythreejs.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/about/reference.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.953051 plopp-23.5.0/docs/basics/
--rw-r--r--   0 runner    (1001) docker     (122)     5402 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/basics/image-plot.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     4446 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/basics/inspector-plot.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     8520 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/basics/line-plot.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     3151 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/basics/saving-figures.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     3793 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/basics/scatter3d-plot.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     2029 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/basics/slicer-plot.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     2984 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/basics/super-plot.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     9239 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.953051 plopp-23.5.0/docs/customization/
--rw-r--r--   0 runner    (1001) docker     (122)     5080 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/customization/subplots.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     5184 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/customization/tweaking-figures.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.953051 plopp-23.5.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (122)    19809 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/examples/custom-interfaces.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.953051 plopp-23.5.0/docs/examples/gallery/
--rw-r--r--   0 runner    (1001) docker     (122)     4574 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/examples/gallery/masking-a-range.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     3939 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/examples/gallery/nyc-taxi.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     7022 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/examples/gallery/rectangle-selection.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     3403 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/examples/gallery/scatter3d-with-slider.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     3080 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/examples/gallery/scatter3d-with-threshold.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     1120 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/examples/gallery.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.953051 plopp-23.5.0/docs/getting-started/
--rw-r--r--   0 runner    (1001) docker     (122)     8406 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/getting-started/numpy-pandas-xarray.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     8677 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/getting-started/overview.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     2337 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3865 2023-06-02 13:20:03.000000 plopp-23.5.0/docs/version.py
--rw-r--r--   0 runner    (1001) docker     (122)     1255 2023-06-02 13:20:03.000000 plopp-23.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.957052 plopp-23.5.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-06-02 13:20:03.000000 plopp-23.5.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)     2242 2023-06-02 13:20:03.000000 plopp-23.5.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-06-02 13:20:03.000000 plopp-23.5.0/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (122)      958 2023-06-02 13:20:03.000000 plopp-23.5.0/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (122)      287 2023-06-02 13:20:03.000000 plopp-23.5.0/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (122)     3273 2023-06-02 13:20:03.000000 plopp-23.5.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-06-02 13:20:03.000000 plopp-23.5.0/requirements/mini.in
--rw-r--r--   0 runner    (1001) docker     (122)      571 2023-06-02 13:20:03.000000 plopp-23.5.0/requirements/mini.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-02 13:20:03.000000 plopp-23.5.0/requirements/noplotly.in
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-06-02 13:20:03.000000 plopp-23.5.0/requirements/noplotly.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-02 13:20:03.000000 plopp-23.5.0/requirements/static.in
--rw-r--r--   0 runner    (1001) docker     (122)      586 2023-06-02 13:20:03.000000 plopp-23.5.0/requirements/static.txt
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-02 13:20:03.000000 plopp-23.5.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (122)     1173 2023-06-02 13:20:03.000000 plopp-23.5.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-02 13:20:03.000000 plopp-23.5.0/requirements/wheels.in
--rw-r--r--   0 runner    (1001) docker     (122)      295 2023-06-02 13:20:03.000000 plopp-23.5.0/requirements/wheels.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.957052 plopp-23.5.0/resources/
--rw-r--r--   0 runner    (1001) docker     (122)    53363 2023-06-02 13:20:03.000000 plopp-23.5.0/resources/logo-plopp-2022.svg
--rw-r--r--   0 runner    (1001) docker     (122)     1037 2023-06-02 13:20:16.973053 plopp-23.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.945051 plopp-23.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.957052 plopp-23.5.0/src/plopp/
--rw-r--r--   0 runner    (1001) docker     (122)     1682 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.957052 plopp-23.5.0/src/plopp/backends/
--rw-r--r--   0 runner    (1001) docker     (122)      107 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3518 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/backends/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.957052 plopp-23.5.0/src/plopp/backends/matplotlib/
--rw-r--r--   0 runner    (1001) docker     (122)     1682 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/backends/matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15050 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/backends/matplotlib/canvas.py
--rw-r--r--   0 runner    (1001) docker     (122)     7828 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/backends/matplotlib/image.py
--rw-r--r--   0 runner    (1001) docker     (122)     2521 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/backends/matplotlib/interactive.py
--rw-r--r--   0 runner    (1001) docker     (122)     8120 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/backends/matplotlib/line.py
--rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/backends/matplotlib/static.py
--rw-r--r--   0 runner    (1001) docker     (122)     2411 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/backends/matplotlib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.961052 plopp-23.5.0/src/plopp/backends/plotly/
--rw-r--r--   0 runner    (1001) docker     (122)      904 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/backends/plotly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9609 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/backends/plotly/canvas.py
--rw-r--r--   0 runner    (1001) docker     (122)     2124 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/backends/plotly/figure.py
--rw-r--r--   0 runner    (1001) docker     (122)     8413 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/backends/plotly/line.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.961052 plopp-23.5.0/src/plopp/backends/pythreejs/
--rw-r--r--   0 runner    (1001) docker     (122)      940 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/backends/pythreejs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8550 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/backends/pythreejs/canvas.py
--rw-r--r--   0 runner    (1001) docker     (122)     2794 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/backends/pythreejs/figure.py
--rw-r--r--   0 runner    (1001) docker     (122)     4920 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/backends/pythreejs/outline.py
--rw-r--r--   0 runner    (1001) docker     (122)     5115 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/backends/pythreejs/point_cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.961052 plopp-23.5.0/src/plopp/core/
--rw-r--r--   0 runner    (1001) docker     (122)      262 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3551 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/core/graph.py
--rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/core/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1501 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/core/limits.py
--rw-r--r--   0 runner    (1001) docker     (122)     7013 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/core/node.py
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/core/system.py
--rw-r--r--   0 runner    (1001) docker     (122)     7005 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1050 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/core/view.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.961052 plopp-23.5.0/src/plopp/data/
--rw-r--r--   0 runner    (1001) docker     (122)      349 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1129 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/data/examples.py
--rw-r--r--   0 runner    (1001) docker     (122)     6098 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/data/factory.py
--rw-r--r--   0 runner    (1001) docker     (122)      430 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/data/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.961052 plopp-23.5.0/src/plopp/functions/
--rw-r--r--   0 runner    (1001) docker     (122)      284 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6624 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/functions/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     3566 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/functions/inspector.py
--rw-r--r--   0 runner    (1001) docker     (122)     4895 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/functions/plot.py
--rw-r--r--   0 runner    (1001) docker     (122)     3879 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/functions/scatter3d.py
--rw-r--r--   0 runner    (1001) docker     (122)     7017 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/functions/slicer.py
--rw-r--r--   0 runner    (1001) docker     (122)     6129 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/functions/superplot.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.965052 plopp-23.5.0/src/plopp/graphics/
--rw-r--r--   0 runner    (1001) docker     (122)      347 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/graphics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/graphics/basefig.py
--rw-r--r--   0 runner    (1001) docker     (122)     5455 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/graphics/camera.py
--rw-r--r--   0 runner    (1001) docker     (122)    10419 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/graphics/colormapper.py
--rw-r--r--   0 runner    (1001) docker     (122)     6363 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/graphics/figimage.py
--rw-r--r--   0 runner    (1001) docker     (122)     5760 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/graphics/figline.py
--rw-r--r--   0 runner    (1001) docker     (122)     6224 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/graphics/figscatter3d.py
--rw-r--r--   0 runner    (1001) docker     (122)     3094 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/graphics/figure.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.965052 plopp-23.5.0/src/plopp/widgets/
--rw-r--r--   0 runner    (1001) docker     (122)      455 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1830 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/widgets/box.py
--rw-r--r--   0 runner    (1001) docker     (122)     2169 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/widgets/checkboxes.py
--rw-r--r--   0 runner    (1001) docker     (122)    11209 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/widgets/cut3d.py
--rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/widgets/drawing.py
--rw-r--r--   0 runner    (1001) docker     (122)     3619 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/widgets/slice.py
--rw-r--r--   0 runner    (1001) docker     (122)      184 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/widgets/style.py
--rw-r--r--   0 runner    (1001) docker     (122)     3935 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/widgets/toolbar.py
--rw-r--r--   0 runner    (1001) docker     (122)     7075 2023-06-02 13:20:03.000000 plopp-23.5.0/src/plopp/widgets/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.957052 plopp-23.5.0/src/plopp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1866 2023-06-02 13:20:16.000000 plopp-23.5.0/src/plopp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-06-02 13:20:16.000000 plopp-23.5.0/src/plopp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 13:20:16.000000 plopp-23.5.0/src/plopp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-06-02 13:20:16.000000 plopp-23.5.0/src/plopp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-02 13:20:16.000000 plopp-23.5.0/src/plopp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.965052 plopp-23.5.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.945051 plopp-23.5.0/tests/backends/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.965052 plopp-23.5.0/tests/backends/matplotlib/
--rw-r--r--   0 runner    (1001) docker     (122)     2721 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/backends/matplotlib/mpl_canvas_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     3485 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/backends/matplotlib/mpl_figimage_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/backends/matplotlib/mpl_figline_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      994 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/backends/matplotlib/mpl_figure_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/backends/matplotlib/mpl_image_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1151 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/backends/matplotlib/mpl_interactive_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     4575 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/backends/matplotlib/mpl_line_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.969053 plopp-23.5.0/tests/backends/plotly/
--rw-r--r--   0 runner    (1001) docker     (122)     2308 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/backends/plotly/plotly_canvas_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      649 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/backends/plotly/plotly_figure_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     3835 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/backends/plotly/plotly_line_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.969053 plopp-23.5.0/tests/backends/pythreejs/
--rw-r--r--   0 runner    (1001) docker     (122)     8406 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/backends/pythreejs/pythreejs_canvas_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/backends/pythreejs/pythreejs_figure_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     4230 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/backends/pythreejs/pythreejs_point_cloud_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1040 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.969053 plopp-23.5.0/tests/core/
--rw-r--r--   0 runner    (1001) docker     (122)     2791 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/core/graph_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2675 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/core/limits_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     5717 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/core/node_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2954 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/core/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      599 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/core/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.969053 plopp-23.5.0/tests/functions/
--rw-r--r--   0 runner    (1001) docker     (122)     1631 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/functions/common_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      397 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/functions/inspector_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    10161 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/functions/plot_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2735 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/functions/scatter3d_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     4027 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/functions/slicer_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2225 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/functions/superplot_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.969053 plopp-23.5.0/tests/graphics/
--rw-r--r--   0 runner    (1001) docker     (122)     8472 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/graphics/colormapper_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     4461 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/graphics/figimage_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     6317 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/graphics/figline_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2321 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/graphics/figscatter3d_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     3410 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/high_level_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      273 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/minimal_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:20:16.969053 plopp-23.5.0/tests/widgets/
--rw-r--r--   0 runner    (1001) docker     (122)     2602 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/widgets/box_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      983 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/widgets/checkboxes_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2434 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/widgets/cut3d_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1642 2023-06-02 13:20:03.000000 plopp-23.5.0/tests/widgets/slice_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1533 2023-06-02 13:20:03.000000 plopp-23.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.565863 plopp-23.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.541863 plopp-23.5.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-06-14 08:53:46.000000 plopp-23.5.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.541863 plopp-23.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     1428 2023-06-14 08:53:46.000000 plopp-23.5.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2093 2023-06-14 08:53:46.000000 plopp-23.5.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3657 2023-06-14 08:53:46.000000 plopp-23.5.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      266 2023-06-14 08:53:46.000000 plopp-23.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1775 2023-06-14 08:53:46.000000 plopp-23.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-06-14 08:53:46.000000 plopp-23.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1866 2023-06-14 08:54:03.565863 plopp-23.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1122 2023-06-14 08:53:46.000000 plopp-23.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.541863 plopp-23.5.1/conda/
+-rw-r--r--   0 runner    (1001) docker     (122)      878 2023-06-14 08:53:46.000000 plopp-23.5.1/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.545863 plopp-23.5.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.545863 plopp-23.5.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (122)   137750 2023-06-14 08:53:46.000000 plopp-23.5.1/docs/_static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.545863 plopp-23.5.1/docs/_static/gallery/
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-06-14 08:53:46.000000 plopp-23.5.1/docs/_static/gallery/README.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    18766 2023-06-14 08:53:46.000000 plopp-23.5.1/docs/_static/gallery/scatter3d-with-slider-thumbnail.png
+-rw-r--r--   0 runner    (1001) docker     (122)    66718 2023-06-14 08:53:46.000000 plopp-23.5.1/docs/_static/gallery/scatter3d-with-threshold-thumbnail.png
+-rw-r--r--   0 runner    (1001) docker     (122)    76253 2023-06-14 08:53:46.000000 plopp-23.5.1/docs/_static/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.545863 plopp-23.5.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2023-06-14 08:53:46.000000 plopp-23.5.1/docs/_templates/scipp-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-06-14 08:53:46.000000 plopp-23.5.1/docs/_templates/scipp-module-template.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.545863 plopp-23.5.1/docs/_templates/sections/
+-rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-06-14 08:53:46.000000 plopp-23.5.1/docs/_templates/sections/header-article.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.545863 plopp-23.5.1/docs/about/
+-rw-r--r--   0 runner    (1001) docker     (122)     1137 2023-06-14 08:53:46.000000 plopp-23.5.1/docs/about/about.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-06-14 08:53:46.000000 plopp-23.5.1/docs/about/faq.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.545863 plopp-23.5.1/docs/about/reference/
+-rw-r--r--   0 runner    (1001) docker     (122)      361 2023-06-14 08:53:46.000000 plopp-23.5.1/docs/about/reference/matplotlib.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      241 2023-06-14 08:53:46.000000 plopp-23.5.1/docs/about/reference/plotly.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-06-14 08:53:46.000000 plopp-23.5.1/docs/about/reference/pythreejs.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-06-14 08:53:46.000000 plopp-23.5.1/docs/about/reference.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.545863 plopp-23.5.1/docs/basics/
+-rw-r--r--   0 runner    (1001) docker     (122)     5402 2023-06-14 08:53:46.000000 plopp-23.5.1/docs/basics/image-plot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     4446 2023-06-14 08:53:46.000000 plopp-23.5.1/docs/basics/inspector-plot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     8520 2023-06-14 08:53:46.000000 plopp-23.5.1/docs/basics/line-plot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     3151 2023-06-14 08:53:46.000000 plopp-23.5.1/docs/basics/saving-figures.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     3793 2023-06-14 08:53:46.000000 plopp-23.5.1/docs/basics/scatter3d-plot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     2029 2023-06-14 08:53:46.000000 plopp-23.5.1/docs/basics/slicer-plot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     2984 2023-06-14 08:53:46.000000 plopp-23.5.1/docs/basics/super-plot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     9239 2023-06-14 08:53:46.000000 plopp-23.5.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.545863 plopp-23.5.1/docs/customization/
+-rw-r--r--   0 runner    (1001) docker     (122)     5080 2023-06-14 08:53:46.000000 plopp-23.5.1/docs/customization/subplots.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     5184 2023-06-14 08:53:46.000000 plopp-23.5.1/docs/customization/tweaking-figures.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.549863 plopp-23.5.1/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)    19809 2023-06-14 08:53:46.000000 plopp-23.5.1/docs/examples/custom-interfaces.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.549863 plopp-23.5.1/docs/examples/gallery/
+-rw-r--r--   0 runner    (1001) docker     (122)     4574 2023-06-14 08:53:46.000000 plopp-23.5.1/docs/examples/gallery/masking-a-range.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     3939 2023-06-14 08:53:46.000000 plopp-23.5.1/docs/examples/gallery/nyc-taxi.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     7022 2023-06-14 08:53:46.000000 plopp-23.5.1/docs/examples/gallery/rectangle-selection.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     3403 2023-06-14 08:53:46.000000 plopp-23.5.1/docs/examples/gallery/scatter3d-with-slider.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     3080 2023-06-14 08:53:46.000000 plopp-23.5.1/docs/examples/gallery/scatter3d-with-threshold.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     1120 2023-06-14 08:53:46.000000 plopp-23.5.1/docs/examples/gallery.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.549863 plopp-23.5.1/docs/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (122)     8406 2023-06-14 08:53:46.000000 plopp-23.5.1/docs/getting-started/numpy-pandas-xarray.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     8677 2023-06-14 08:53:46.000000 plopp-23.5.1/docs/getting-started/overview.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     2337 2023-06-14 08:53:46.000000 plopp-23.5.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3865 2023-06-14 08:53:46.000000 plopp-23.5.1/docs/version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1255 2023-06-14 08:53:46.000000 plopp-23.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.549863 plopp-23.5.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-06-14 08:53:46.000000 plopp-23.5.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2242 2023-06-14 08:53:46.000000 plopp-23.5.1/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-06-14 08:53:46.000000 plopp-23.5.1/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (122)      958 2023-06-14 08:53:46.000000 plopp-23.5.1/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      287 2023-06-14 08:53:46.000000 plopp-23.5.1/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3273 2023-06-14 08:53:46.000000 plopp-23.5.1/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-06-14 08:53:46.000000 plopp-23.5.1/requirements/mini.in
+-rw-r--r--   0 runner    (1001) docker     (122)      571 2023-06-14 08:53:46.000000 plopp-23.5.1/requirements/mini.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-14 08:53:46.000000 plopp-23.5.1/requirements/noplotly.in
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-06-14 08:53:46.000000 plopp-23.5.1/requirements/noplotly.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-14 08:53:46.000000 plopp-23.5.1/requirements/static.in
+-rw-r--r--   0 runner    (1001) docker     (122)      586 2023-06-14 08:53:46.000000 plopp-23.5.1/requirements/static.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-14 08:53:46.000000 plopp-23.5.1/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1173 2023-06-14 08:53:46.000000 plopp-23.5.1/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-14 08:53:46.000000 plopp-23.5.1/requirements/wheels.in
+-rw-r--r--   0 runner    (1001) docker     (122)      295 2023-06-14 08:53:46.000000 plopp-23.5.1/requirements/wheels.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.549863 plopp-23.5.1/resources/
+-rw-r--r--   0 runner    (1001) docker     (122)    53363 2023-06-14 08:53:46.000000 plopp-23.5.1/resources/logo-plopp-2022.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     1037 2023-06-14 08:54:03.565863 plopp-23.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.541863 plopp-23.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.549863 plopp-23.5.1/src/plopp/
+-rw-r--r--   0 runner    (1001) docker     (122)     1682 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.553863 plopp-23.5.1/src/plopp/backends/
+-rw-r--r--   0 runner    (1001) docker     (122)      107 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3629 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/backends/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.553863 plopp-23.5.1/src/plopp/backends/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (122)     1682 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/backends/matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15050 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/backends/matplotlib/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7828 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/backends/matplotlib/image.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2521 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/backends/matplotlib/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8120 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/backends/matplotlib/line.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/backends/matplotlib/static.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2411 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/backends/matplotlib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.553863 plopp-23.5.1/src/plopp/backends/plotly/
+-rw-r--r--   0 runner    (1001) docker     (122)      904 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/backends/plotly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10042 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/backends/plotly/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2124 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/backends/plotly/figure.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8413 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/backends/plotly/line.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.553863 plopp-23.5.1/src/plopp/backends/pythreejs/
+-rw-r--r--   0 runner    (1001) docker     (122)      940 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/backends/pythreejs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8550 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/backends/pythreejs/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2794 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/backends/pythreejs/figure.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4920 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/backends/pythreejs/outline.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5115 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/backends/pythreejs/point_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.557863 plopp-23.5.1/src/plopp/core/
+-rw-r--r--   0 runner    (1001) docker     (122)      262 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3551 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/core/graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/core/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1501 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/core/limits.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7013 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/core/node.py
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/core/system.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7028 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1050 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/core/view.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.557863 plopp-23.5.1/src/plopp/data/
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1129 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/data/examples.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6098 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/data/factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)      430 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/data/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.557863 plopp-23.5.1/src/plopp/functions/
+-rw-r--r--   0 runner    (1001) docker     (122)      284 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6624 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/functions/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3566 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/functions/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4895 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/functions/plot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3879 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/functions/scatter3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7031 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/functions/slicer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6129 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/functions/superplot.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.557863 plopp-23.5.1/src/plopp/graphics/
+-rw-r--r--   0 runner    (1001) docker     (122)      347 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/graphics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/graphics/basefig.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5455 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/graphics/camera.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10419 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/graphics/colormapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6363 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/graphics/figimage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5760 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/graphics/figline.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6224 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/graphics/figscatter3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3094 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/graphics/figure.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.561864 plopp-23.5.1/src/plopp/widgets/
+-rw-r--r--   0 runner    (1001) docker     (122)      455 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1830 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2169 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/widgets/checkboxes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11209 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/widgets/cut3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/widgets/drawing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3619 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/widgets/slice.py
+-rw-r--r--   0 runner    (1001) docker     (122)      184 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/widgets/style.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3935 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/widgets/toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7075 2023-06-14 08:53:46.000000 plopp-23.5.1/src/plopp/widgets/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.553863 plopp-23.5.1/src/plopp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1866 2023-06-14 08:54:03.000000 plopp-23.5.1/src/plopp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4969 2023-06-14 08:54:03.000000 plopp-23.5.1/src/plopp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 08:54:03.000000 plopp-23.5.1/src/plopp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-06-14 08:54:03.000000 plopp-23.5.1/src/plopp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-14 08:54:03.000000 plopp-23.5.1/src/plopp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.561864 plopp-23.5.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.541863 plopp-23.5.1/tests/backends/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.561864 plopp-23.5.1/tests/backends/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (122)     2721 2023-06-14 08:53:46.000000 plopp-23.5.1/tests/backends/matplotlib/mpl_canvas_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3485 2023-06-14 08:53:46.000000 plopp-23.5.1/tests/backends/matplotlib/mpl_figimage_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-06-14 08:53:46.000000 plopp-23.5.1/tests/backends/matplotlib/mpl_figline_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      994 2023-06-14 08:53:46.000000 plopp-23.5.1/tests/backends/matplotlib/mpl_figure_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-06-14 08:53:46.000000 plopp-23.5.1/tests/backends/matplotlib/mpl_image_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1151 2023-06-14 08:53:46.000000 plopp-23.5.1/tests/backends/matplotlib/mpl_interactive_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4575 2023-06-14 08:53:46.000000 plopp-23.5.1/tests/backends/matplotlib/mpl_line_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.561864 plopp-23.5.1/tests/backends/plotly/
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-14 08:53:46.000000 plopp-23.5.1/tests/backends/plotly/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2276 2023-06-14 08:53:46.000000 plopp-23.5.1/tests/backends/plotly/plotly_canvas_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      866 2023-06-14 08:53:46.000000 plopp-23.5.1/tests/backends/plotly/plotly_figure_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3835 2023-06-14 08:53:46.000000 plopp-23.5.1/tests/backends/plotly/plotly_line_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.561864 plopp-23.5.1/tests/backends/pythreejs/
+-rw-r--r--   0 runner    (1001) docker     (122)     8406 2023-06-14 08:53:46.000000 plopp-23.5.1/tests/backends/pythreejs/pythreejs_canvas_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-06-14 08:53:46.000000 plopp-23.5.1/tests/backends/pythreejs/pythreejs_figure_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4230 2023-06-14 08:53:46.000000 plopp-23.5.1/tests/backends/pythreejs/pythreejs_point_cloud_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1040 2023-06-14 08:53:46.000000 plopp-23.5.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.561864 plopp-23.5.1/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (122)     2791 2023-06-14 08:53:46.000000 plopp-23.5.1/tests/core/graph_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2675 2023-06-14 08:53:46.000000 plopp-23.5.1/tests/core/limits_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5717 2023-06-14 08:53:46.000000 plopp-23.5.1/tests/core/node_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2954 2023-06-14 08:53:46.000000 plopp-23.5.1/tests/core/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      599 2023-06-14 08:53:46.000000 plopp-23.5.1/tests/core/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.565863 plopp-23.5.1/tests/functions/
+-rw-r--r--   0 runner    (1001) docker     (122)     1631 2023-06-14 08:53:46.000000 plopp-23.5.1/tests/functions/common_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      397 2023-06-14 08:53:46.000000 plopp-23.5.1/tests/functions/inspector_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10161 2023-06-14 08:53:46.000000 plopp-23.5.1/tests/functions/plot_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2735 2023-06-14 08:53:46.000000 plopp-23.5.1/tests/functions/scatter3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4424 2023-06-14 08:53:46.000000 plopp-23.5.1/tests/functions/slicer_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2225 2023-06-14 08:53:46.000000 plopp-23.5.1/tests/functions/superplot_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.565863 plopp-23.5.1/tests/graphics/
+-rw-r--r--   0 runner    (1001) docker     (122)     8472 2023-06-14 08:53:46.000000 plopp-23.5.1/tests/graphics/colormapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4461 2023-06-14 08:53:46.000000 plopp-23.5.1/tests/graphics/figimage_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6317 2023-06-14 08:53:46.000000 plopp-23.5.1/tests/graphics/figline_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2321 2023-06-14 08:53:46.000000 plopp-23.5.1/tests/graphics/figscatter3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3410 2023-06-14 08:53:46.000000 plopp-23.5.1/tests/high_level_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      273 2023-06-14 08:53:46.000000 plopp-23.5.1/tests/minimal_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:54:03.565863 plopp-23.5.1/tests/widgets/
+-rw-r--r--   0 runner    (1001) docker     (122)     2602 2023-06-14 08:53:46.000000 plopp-23.5.1/tests/widgets/box_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      983 2023-06-14 08:53:46.000000 plopp-23.5.1/tests/widgets/checkboxes_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2434 2023-06-14 08:53:46.000000 plopp-23.5.1/tests/widgets/cut3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1642 2023-06-14 08:53:46.000000 plopp-23.5.1/tests/widgets/slice_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1533 2023-06-14 08:53:46.000000 plopp-23.5.1/tox.ini
```

### Comparing `plopp-23.5.0/.github/workflows/ci.yml` & `plopp-23.5.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/.github/workflows/docs.yml` & `plopp-23.5.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/.github/workflows/release.yml` & `plopp-23.5.1/.github/workflows/release.yml`

 * *Files 4% similar despite different names*

```diff
@@ -81,14 +81,16 @@
     name: Manage Versions
     runs-on: ubuntu-20.04
     outputs:
       version-new: ${{ steps.version.outputs.new }}
       version-replaced: ${{ steps.version.outputs.replaced }}
     steps:
       - uses: actions/checkout@v3
+        with:
+          fetch-depth: 0  # history required so version can be determined
       - uses: actions/setup-python@v3
         with:
           python-version: '3.10'
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/ci.txt
       - name: Set outputs
         id: version
```

### Comparing `plopp-23.5.0/.pre-commit-config.yaml` & `plopp-23.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/LICENSE` & `plopp-23.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/PKG-INFO` & `plopp-23.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plopp
-Version: 23.5.0
+Version: 23.5.1
 Summary: Plotting library based on scipp
 Home-page: https://scipp.github.io/plopp
 Author: Scipp contributors (https://github.com/scipp)
 License: BSD
 Project-URL: Bug Tracker, https://github.com/scipp/plopp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `plopp-23.5.0/README.md` & `plopp-23.5.1/README.md`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/conda/meta.yaml` & `plopp-23.5.1/conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/docs/_static/favicon.ico` & `plopp-23.5.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/docs/_static/gallery/scatter3d-with-slider-thumbnail.png` & `plopp-23.5.1/docs/_static/gallery/scatter3d-with-slider-thumbnail.png`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/docs/_static/gallery/scatter3d-with-threshold-thumbnail.png` & `plopp-23.5.1/docs/_static/gallery/scatter3d-with-threshold-thumbnail.png`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/docs/_static/logo.svg` & `plopp-23.5.1/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/docs/_templates/scipp-class-template.rst` & `plopp-23.5.1/docs/_templates/scipp-class-template.rst`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/docs/_templates/scipp-module-template.rst` & `plopp-23.5.1/docs/_templates/scipp-module-template.rst`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/docs/_templates/sections/header-article.html` & `plopp-23.5.1/docs/_templates/sections/header-article.html`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/docs/about/about.rst` & `plopp-23.5.1/docs/about/about.rst`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/docs/about/faq.ipynb` & `plopp-23.5.1/docs/about/faq.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/docs/about/reference.rst` & `plopp-23.5.1/docs/about/reference.rst`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/docs/basics/image-plot.ipynb` & `plopp-23.5.1/docs/basics/image-plot.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/docs/basics/inspector-plot.ipynb` & `plopp-23.5.1/docs/basics/inspector-plot.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/docs/basics/line-plot.ipynb` & `plopp-23.5.1/docs/basics/line-plot.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/docs/basics/saving-figures.ipynb` & `plopp-23.5.1/docs/basics/saving-figures.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/docs/basics/scatter3d-plot.ipynb` & `plopp-23.5.1/docs/basics/scatter3d-plot.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/docs/basics/slicer-plot.ipynb` & `plopp-23.5.1/docs/basics/slicer-plot.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/docs/basics/super-plot.ipynb` & `plopp-23.5.1/docs/basics/super-plot.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/docs/conf.py` & `plopp-23.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/docs/customization/subplots.ipynb` & `plopp-23.5.1/docs/customization/subplots.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/docs/customization/tweaking-figures.ipynb` & `plopp-23.5.1/docs/customization/tweaking-figures.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/docs/examples/custom-interfaces.ipynb` & `plopp-23.5.1/docs/examples/custom-interfaces.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/docs/examples/gallery/masking-a-range.ipynb` & `plopp-23.5.1/docs/examples/gallery/masking-a-range.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/docs/examples/gallery/nyc-taxi.ipynb` & `plopp-23.5.1/docs/examples/gallery/nyc-taxi.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/docs/examples/gallery/rectangle-selection.ipynb` & `plopp-23.5.1/docs/examples/gallery/rectangle-selection.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/docs/examples/gallery/scatter3d-with-slider.ipynb` & `plopp-23.5.1/docs/examples/gallery/scatter3d-with-slider.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/docs/examples/gallery/scatter3d-with-threshold.ipynb` & `plopp-23.5.1/docs/examples/gallery/scatter3d-with-threshold.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/docs/examples/gallery.ipynb` & `plopp-23.5.1/docs/examples/gallery.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/docs/getting-started/numpy-pandas-xarray.ipynb` & `plopp-23.5.1/docs/getting-started/numpy-pandas-xarray.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/docs/getting-started/overview.ipynb` & `plopp-23.5.1/docs/getting-started/overview.ipynb`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/docs/index.rst` & `plopp-23.5.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/docs/version.py` & `plopp-23.5.1/docs/version.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/pyproject.toml` & `plopp-23.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/requirements/base.txt` & `plopp-23.5.1/requirements/base.txt`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/requirements/ci.txt` & `plopp-23.5.1/requirements/ci.txt`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/requirements/docs.txt` & `plopp-23.5.1/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/requirements/mini.txt` & `plopp-23.5.1/requirements/mini.txt`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/requirements/static.txt` & `plopp-23.5.1/requirements/static.txt`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/requirements/test.txt` & `plopp-23.5.1/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/resources/logo-plopp-2022.svg` & `plopp-23.5.1/resources/logo-plopp-2022.svg`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/setup.cfg` & `plopp-23.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/__init__.py` & `plopp-23.5.1/src/plopp/__init__.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/backends/manager.py` & `plopp-23.5.1/src/plopp/backends/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
+DEFAULTS = {'2d': 'matplotlib', '3d': 'pythreejs'}
+
 
 class BackendManager:
     def __init__(self):
-        self._mapping = {'2d': 'matplotlib', '3d': 'pythreejs'}
+        self._mapping = DEFAULTS.copy()
         self._backends = {}
         self._sync()
 
     def __getitem__(self, key):
         return self._mapping[key]
 
     def __setitem__(self, key, value):
@@ -20,14 +22,18 @@
 
     def values(self):
         return self._mapping.values()
 
     def items(self):
         return self._mapping.items()
 
+    def reset(self):
+        self._mapping = DEFAULTS.copy()
+        self._sync()
+
     def _sync(self):
         if self._mapping['2d'] == 'matplotlib':
             from .matplotlib import MatplotlibBackend
 
             self._backends['2d'] = MatplotlibBackend()
         elif self._mapping['2d'] == 'plotly':
             from .plotly import PlotlyBackend
```

### Comparing `plopp-23.5.0/src/plopp/backends/matplotlib/__init__.py` & `plopp-23.5.1/src/plopp/backends/matplotlib/__init__.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/backends/matplotlib/canvas.py` & `plopp-23.5.1/src/plopp/backends/matplotlib/canvas.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/backends/matplotlib/image.py` & `plopp-23.5.1/src/plopp/backends/matplotlib/image.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/backends/matplotlib/interactive.py` & `plopp-23.5.1/src/plopp/backends/matplotlib/interactive.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/backends/matplotlib/line.py` & `plopp-23.5.1/src/plopp/backends/matplotlib/line.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/backends/matplotlib/static.py` & `plopp-23.5.1/src/plopp/backends/matplotlib/static.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/backends/matplotlib/utils.py` & `plopp-23.5.1/src/plopp/backends/matplotlib/utils.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/backends/plotly/__init__.py` & `plopp-23.5.1/src/plopp/backends/plotly/__init__.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/backends/plotly/canvas.py` & `plopp-23.5.1/src/plopp/backends/plotly/canvas.py`

 * *Files 8% similar despite different names*

```diff
@@ -70,16 +70,16 @@
                 'width': 600 if figsize is None else figsize[0],
                 'height': 400 if figsize is None else figsize[1],
             }
         )
         self.figsize = figsize
         self._user_vmin = vmin
         self._user_vmax = vmax
-        self.xunit = None
-        self.yunit = None
+        self.units = {}
+        self.dims = {}
         self._own_axes = False
         if title:
             self.title = title
 
     def to_widget(self):
         return self.fig
 
@@ -130,26 +130,47 @@
         ----------
         **limits:
             Min and max limits for each dimension to be cropped.
         """
         for xy, lims in limits.items():
             getattr(self.fig, f'update_{xy}axes')(
                 range=[
-                    maybe_variable_to_number(lims[m], unit=getattr(self, f'{xy}unit'))
+                    maybe_variable_to_number(lims[m], unit=self.units[xy])
                     for m in ('min', 'max')
                     if m in lims
                 ]
             )
 
+    def set_axes(self, dims, units):
+        """
+        Set the axes dimensions and units.
+
+        Parameters
+        ----------
+        dims:
+            The dimensions of the data.
+        units:
+            The units of the data.
+        """
+        self.units = units
+        self.dims = dims
+
+    @property
+    def empty(self) -> bool:
+        """
+        Check if the canvas is empty.
+        """
+        return not self.dims
+
     @property
     def title(self) -> str:
         """
         Get or set the title of the plot.
         """
-        return self.fig.layout.title
+        return self.fig.layout.title.text
 
     @title.setter
     def title(self, text: str):
         layout = self.fig.layout
         if not text:
             layout.margin.t = 0
         elif layout.margin.t == 0:
@@ -157,26 +178,26 @@
         layout.title = text
 
     @property
     def xlabel(self) -> str:
         """
         Get or set the label of the x-axis.
         """
-        return self.fig.layout.xaxis.title
+        return self.fig.layout.xaxis.title.text
 
     @xlabel.setter
     def xlabel(self, lab: str):
         self.fig.layout.xaxis.title = lab
 
     @property
     def ylabel(self) -> str:
         """
         Get or set the label of the y-axis.
         """
-        return self.fig.layout.yaxis.title
+        return self.fig.layout.yaxis.title.text
 
     @ylabel.setter
     def ylabel(self, lab: str):
         self.fig.layout.yaxis.title = lab
 
     @property
     def xscale(self) -> str:
```

### Comparing `plopp-23.5.0/src/plopp/backends/plotly/figure.py` & `plopp-23.5.1/src/plopp/backends/plotly/figure.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/backends/plotly/line.py` & `plopp-23.5.1/src/plopp/backends/plotly/line.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/backends/pythreejs/__init__.py` & `plopp-23.5.1/src/plopp/backends/pythreejs/__init__.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/backends/pythreejs/canvas.py` & `plopp-23.5.1/src/plopp/backends/pythreejs/canvas.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/backends/pythreejs/figure.py` & `plopp-23.5.1/src/plopp/backends/pythreejs/figure.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/backends/pythreejs/outline.py` & `plopp-23.5.1/src/plopp/backends/pythreejs/outline.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/backends/pythreejs/point_cloud.py` & `plopp-23.5.1/src/plopp/backends/pythreejs/point_cloud.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/core/graph.py` & `plopp-23.5.1/src/plopp/core/graph.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/core/helpers.py` & `plopp-23.5.1/src/plopp/core/helpers.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/core/limits.py` & `plopp-23.5.1/src/plopp/core/limits.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/core/node.py` & `plopp-23.5.1/src/plopp/core/node.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/core/utils.py` & `plopp-23.5.1/src/plopp/core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     """
     text = ""
     if name is not None:
         text = name
     else:
         text = str(var.dims[-1])
     if var.unit is not None:
-        text += f" [{var.unit}]"
+        text += (" " if text else "") + f"[{var.unit}]"
     return text
 
 
 def value_to_string(val: Union[int, float], precision: int = 3) -> str:
     """
     Convert a number to a human readable string.
```

### Comparing `plopp-23.5.0/src/plopp/core/view.py` & `plopp-23.5.1/src/plopp/core/view.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/data/examples.py` & `plopp-23.5.1/src/plopp/data/examples.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/data/factory.py` & `plopp-23.5.1/src/plopp/data/factory.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/functions/common.py` & `plopp-23.5.1/src/plopp/functions/common.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/functions/inspector.py` & `plopp-23.5.1/src/plopp/functions/inspector.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/functions/plot.py` & `plopp-23.5.1/src/plopp/functions/plot.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/functions/scatter3d.py` & `plopp-23.5.1/src/plopp/functions/scatter3d.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/functions/slicer.py` & `plopp-23.5.1/src/plopp/functions/slicer.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,32 +101,32 @@
         self.data_nodes = [Node(da) for da in ds.values()]
 
         self.slider = SliceWidget(ds, dims=[dim for dim in ds.dims if dim not in keep])
         self.slider_node = widget_node(self.slider)
         self.slice_nodes = [
             slice_dims(data_node, self.slider_node) for data_node in self.data_nodes
         ]
-        if len(keep) == 1:
-            self.figure = figure1d(
-                *self.slice_nodes,
-                crop=crop,
-                autoscale=autoscale,
-                vmin=vmin,
-                vmax=vmax,
-                **kwargs,
-            )
-        elif len(keep) == 2:
-            self.figure = figure2d(
-                *self.slice_nodes,
-                crop=crop,
-                autoscale=autoscale,
-                vmin=vmin,
-                vmax=vmax,
-                **kwargs,
+        ndims = len(keep)
+        if ndims == 1:
+            make_figure = figure1d
+        elif ndims == 2:
+            make_figure = figure2d
+        else:
+            raise ValueError(
+                f'Slicer plot: the number of dims to be kept must be 1 or 2, '
+                f'but {ndims} were requested.'
             )
+        self.figure = make_figure(
+            *self.slice_nodes,
+            crop=crop,
+            autoscale=autoscale,
+            vmin=vmin,
+            vmax=vmax,
+            **kwargs,
+        )
 
 
 def slicer(
     obj: Union[VariableLike, ndarray, Dict[str, Union[VariableLike, ndarray]]],
     keep: List[str] = None,
     *,
     autoscale: Literal['auto', 'grow', 'fixed'] = 'auto',
```

### Comparing `plopp-23.5.0/src/plopp/functions/superplot.py` & `plopp-23.5.1/src/plopp/functions/superplot.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/graphics/basefig.py` & `plopp-23.5.1/src/plopp/graphics/basefig.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/graphics/camera.py` & `plopp-23.5.1/src/plopp/graphics/camera.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/graphics/colormapper.py` & `plopp-23.5.1/src/plopp/graphics/colormapper.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/graphics/figimage.py` & `plopp-23.5.1/src/plopp/graphics/figimage.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/graphics/figline.py` & `plopp-23.5.1/src/plopp/graphics/figline.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/graphics/figscatter3d.py` & `plopp-23.5.1/src/plopp/graphics/figscatter3d.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/graphics/figure.py` & `plopp-23.5.1/src/plopp/graphics/figure.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/widgets/box.py` & `plopp-23.5.1/src/plopp/widgets/box.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/widgets/checkboxes.py` & `plopp-23.5.1/src/plopp/widgets/checkboxes.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/widgets/cut3d.py` & `plopp-23.5.1/src/plopp/widgets/cut3d.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/widgets/drawing.py` & `plopp-23.5.1/src/plopp/widgets/drawing.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/widgets/slice.py` & `plopp-23.5.1/src/plopp/widgets/slice.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/widgets/toolbar.py` & `plopp-23.5.1/src/plopp/widgets/toolbar.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp/widgets/tools.py` & `plopp-23.5.1/src/plopp/widgets/tools.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/src/plopp.egg-info/PKG-INFO` & `plopp-23.5.1/src/plopp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plopp
-Version: 23.5.0
+Version: 23.5.1
 Summary: Plotting library based on scipp
 Home-page: https://scipp.github.io/plopp
 Author: Scipp contributors (https://github.com/scipp)
 License: BSD
 Project-URL: Bug Tracker, https://github.com/scipp/plopp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `plopp-23.5.0/src/plopp.egg-info/SOURCES.txt` & `plopp-23.5.1/src/plopp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -128,14 +128,15 @@
 tests/backends/matplotlib/mpl_canvas_test.py
 tests/backends/matplotlib/mpl_figimage_test.py
 tests/backends/matplotlib/mpl_figline_test.py
 tests/backends/matplotlib/mpl_figure_test.py
 tests/backends/matplotlib/mpl_image_test.py
 tests/backends/matplotlib/mpl_interactive_test.py
 tests/backends/matplotlib/mpl_line_test.py
+tests/backends/plotly/conftest.py
 tests/backends/plotly/plotly_canvas_test.py
 tests/backends/plotly/plotly_figure_test.py
 tests/backends/plotly/plotly_line_test.py
 tests/backends/pythreejs/pythreejs_canvas_test.py
 tests/backends/pythreejs/pythreejs_figure_test.py
 tests/backends/pythreejs/pythreejs_point_cloud_test.py
 tests/core/graph_test.py
```

### Comparing `plopp-23.5.0/tests/backends/matplotlib/mpl_canvas_test.py` & `plopp-23.5.1/tests/backends/matplotlib/mpl_canvas_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/tests/backends/matplotlib/mpl_figimage_test.py` & `plopp-23.5.1/tests/backends/matplotlib/mpl_figimage_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/tests/backends/matplotlib/mpl_figline_test.py` & `plopp-23.5.1/tests/backends/matplotlib/mpl_figline_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/tests/backends/matplotlib/mpl_figure_test.py` & `plopp-23.5.1/tests/backends/matplotlib/mpl_figure_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/tests/backends/matplotlib/mpl_image_test.py` & `plopp-23.5.1/tests/backends/matplotlib/mpl_image_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/tests/backends/matplotlib/mpl_interactive_test.py` & `plopp-23.5.1/tests/backends/matplotlib/mpl_interactive_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/tests/backends/matplotlib/mpl_line_test.py` & `plopp-23.5.1/tests/backends/matplotlib/mpl_line_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/tests/backends/plotly/plotly_canvas_test.py` & `plopp-23.5.1/tests/backends/plotly/plotly_canvas_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 pytest.importorskip("plotly")
 
 
 def test_creation():
     title = 'My canvas'
     canvas = Canvas(title=title)
-    assert canvas.title['text'] == title
+    assert canvas.title == title
 
 
 def test_logx():
     canvas = Canvas()
     canvas.logx()
     assert canvas.xscale == 'log'
     canvas.logx()
@@ -32,16 +32,15 @@
     assert canvas.yscale == 'log'
     canvas.logy()
     assert canvas.yscale == 'linear'
 
 
 def test_crop():
     canvas = Canvas()
-    canvas.xunit = 'm'
-    canvas.yunit = 'm'
+    canvas.units.update(x='m', y='m')
     xmin = sc.scalar(2.1, unit='m')
     xmax = sc.scalar(102.0, unit='m')
     ymin = sc.scalar(5.5, unit='m')
     ymax = sc.scalar(22.3, unit='m')
     canvas.crop(
         x={
             'min': xmin,
@@ -54,26 +53,24 @@
     )
     assert canvas.xrange == (xmin.value, xmax.value)
     assert canvas.yrange == (ymin.value, ymax.value)
 
 
 def test_crop_unit_conversion():
     canvas = Canvas()
-    canvas.xunit = 'cm'
-    canvas.yunit = 'cm'
+    canvas.units.update(x='cm', y='cm')
     xmin = sc.scalar(2.1, unit='m')
     xmax = sc.scalar(3.3, unit='m')
     canvas.crop(x={'min': xmin, 'max': xmax})
     assert canvas.xrange == (210.0, 330.0)
 
 
 def test_crop_no_variable():
     canvas = Canvas()
-    canvas.xunit = 'm'
-    canvas.yunit = 'm'
+    canvas.units.update(x='m', y='m')
     xmin = 2.1
     xmax = 102.0
     ymin = 5.5
     ymax = 22.3
     canvas.crop(
         x={
             'min': xmin,
```

### Comparing `plopp-23.5.0/tests/backends/plotly/plotly_line_test.py` & `plopp-23.5.1/tests/backends/plotly/plotly_line_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/tests/backends/pythreejs/pythreejs_canvas_test.py` & `plopp-23.5.1/tests/backends/pythreejs/pythreejs_canvas_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/tests/backends/pythreejs/pythreejs_figure_test.py` & `plopp-23.5.1/tests/backends/pythreejs/pythreejs_figure_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/tests/backends/pythreejs/pythreejs_point_cloud_test.py` & `plopp-23.5.1/tests/backends/pythreejs/pythreejs_point_cloud_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/tests/conftest.py` & `plopp-23.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/tests/core/graph_test.py` & `plopp-23.5.1/tests/core/graph_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/tests/core/limits_test.py` & `plopp-23.5.1/tests/core/limits_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/tests/core/node_test.py` & `plopp-23.5.1/tests/core/node_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/tests/core/utils_test.py` & `plopp-23.5.1/tests/core/utils_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/tests/core/views.py` & `plopp-23.5.1/tests/core/views.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/tests/functions/common_test.py` & `plopp-23.5.1/tests/functions/common_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/tests/functions/plot_test.py` & `plopp-23.5.1/tests/functions/plot_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/tests/functions/scatter3d_test.py` & `plopp-23.5.1/tests/functions/scatter3d_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/tests/functions/slicer_test.py` & `plopp-23.5.1/tests/functions/slicer_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -84,25 +84,37 @@
     with pytest.raises(sc.DatasetError):
         Slicer({'a': a, 'b': b}, keep=['xx'])
 
 
 def test_raises_ValueError_when_given_binned_data():
     da = sc.data.table_xyz(100).bin(x=10, y=20)
     with pytest.raises(ValueError, match='Cannot plot binned data'):
-        Slicer(da, keep=['x'])
+        Slicer(da, keep=['xx'])
 
 
 def test_raises_when_requested_keep_dims_do_not_exist():
     da = data_array(ndim=3)
     with pytest.raises(
         ValueError, match='Slicer plot: one or more of the requested dims to be kept'
     ):
         Slicer(da, keep=['time'])
 
 
+def test_raises_when_number_of_keep_dims_requested_is_bad():
+    da = data_array(ndim=4)
+    with pytest.raises(
+        ValueError, match='Slicer plot: the number of dims to be kept must be 1 or 2'
+    ):
+        Slicer(da, keep=['xx', 'yy', 'zz'])
+    with pytest.raises(
+        ValueError, match='Slicer plot: the list of dims to be kept cannot be empty'
+    ):
+        Slicer(da, keep=[])
+
+
 def test_autoscale_fixed():
     da = sc.DataArray(
         data=sc.arange('x', 5 * 10 * 20).fold(dim='x', sizes={'z': 20, 'y': 10, 'x': 5})
     )
     sl = Slicer(da, keep=['y', 'x'], autoscale='fixed')
     assert sl.figure._fig.colormapper.vmin == 0
     assert sl.figure._fig.colormapper.vmax == 5 * 10 * 20 - 1
```

### Comparing `plopp-23.5.0/tests/functions/superplot_test.py` & `plopp-23.5.1/tests/functions/superplot_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/tests/graphics/colormapper_test.py` & `plopp-23.5.1/tests/graphics/colormapper_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/tests/graphics/figimage_test.py` & `plopp-23.5.1/tests/graphics/figimage_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/tests/graphics/figline_test.py` & `plopp-23.5.1/tests/graphics/figline_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/tests/graphics/figscatter3d_test.py` & `plopp-23.5.1/tests/graphics/figscatter3d_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/tests/high_level_test.py` & `plopp-23.5.1/tests/high_level_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/tests/widgets/box_test.py` & `plopp-23.5.1/tests/widgets/box_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/tests/widgets/checkboxes_test.py` & `plopp-23.5.1/tests/widgets/checkboxes_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/tests/widgets/cut3d_test.py` & `plopp-23.5.1/tests/widgets/cut3d_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/tests/widgets/slice_test.py` & `plopp-23.5.1/tests/widgets/slice_test.py`

 * *Files identical despite different names*

### Comparing `plopp-23.5.0/tox.ini` & `plopp-23.5.1/tox.ini`

 * *Files identical despite different names*

