# Comparing `tmp/nbsite-0.8.1a3.tar.gz` & `tmp/nbsite-0.8.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nbsite-0.8.1a3.tar", last modified: Wed Jun 14 14:23:47 2023, max compression
+gzip compressed data, was "nbsite-0.8.1a4.tar", last modified: Wed Jun 14 14:42:19 2023, max compression
```

## Comparing `nbsite-0.8.1a3.tar` & `nbsite-0.8.1a4.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:23:47.000000 nbsite-0.8.1a3/
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-06-14 14:23:47.000000 nbsite-0.8.1a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:23:47.000000 nbsite-0.8.1a3/nbsite/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-14 14:23:47.000000 nbsite-0.8.1a3/nbsite/.version
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:23:47.000000 nbsite-0.8.1a3/nbsite/_shared_static/
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/_shared_static/alert.css
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/_shared_static/dataframe.css
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/_shared_static/gallery.css
--rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/_shared_static/holoviz-icon-white.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/_shared_static/mystnb.css
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/_shared_static/nbsite.css
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/_shared_static/notebook.css
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/_shared_static/scroller.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:23:47.000000 nbsite-0.8.1a3/nbsite/_shared_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/_shared_templates/copyright-last-updated.html
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/_shared_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/_shared_templates/sidebar-nav-bs.html
--rw-r--r--   0 runner    (1001) docker     (123)    13156 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:23:47.000000 nbsite-0.8.1a3/nbsite/gallery/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/gallery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30951 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/gallery/gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/gallery/thumbnailer.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/ipystartup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18133 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/nbbuild.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/paramdoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:23:47.000000 nbsite-0.8.1a3/nbsite/pyodide/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/pyodide/ServiceHandler.js
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/pyodide/ServiceWorker.js
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/pyodide/WebWorker.js
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/pyodide/WorkerHandler.js
--rw-r--r--   0 runner    (1001) docker     (123)    16934 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/pyodide/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:23:47.000000 nbsite-0.8.1a3/nbsite/pyodide/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/pyodide/_static/run_cell.js
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/pyodide/_static/runbutton.css
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/pyodide/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/shared_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:23:47.000000 nbsite-0.8.1a3/nbsite/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:23:47.000000 nbsite-0.8.1a3/nbsite/templates/basic/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/templates/basic/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/templates/basic/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/templates/basic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:23:47.000000 nbsite-0.8.1a3/nbsite/templates/holoviz/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/templates/holoviz/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/templates/holoviz/about.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/templates/holoviz/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/templates/holoviz/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:23:47.000000 nbsite-0.8.1a3/nbsite/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18588 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/tests/test_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/nbsite/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:23:47.000000 nbsite-0.8.1a3/nbsite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-06-14 14:23:47.000000 nbsite-0.8.1a3/nbsite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-14 14:23:47.000000 nbsite-0.8.1a3/nbsite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 14:23:47.000000 nbsite-0.8.1a3/nbsite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-14 14:23:47.000000 nbsite-0.8.1a3/nbsite.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-14 14:23:47.000000 nbsite-0.8.1a3/nbsite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 14:23:47.000000 nbsite-0.8.1a3/nbsite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:23:47.000000 nbsite-0.8.1a3/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/scripts/nbsite_cleandisthtml.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5851 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/scripts/nbsite_fix_links.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      132 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/scripts/nbsite_from_tmplate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11126 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/scripts/nbsite_generate_modules.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      556 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/scripts/nbsite_nbpagebuild.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-14 14:23:47.000000 nbsite-0.8.1a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-06-14 14:22:33.000000 nbsite-0.8.1a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:42:19.316173 nbsite-0.8.1a4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-06-14 14:42:19.316173 nbsite-0.8.1a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:42:19.312173 nbsite-0.8.1a4/nbsite/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-14 14:42:19.000000 nbsite-0.8.1a4/nbsite/.version
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:42:19.312173 nbsite-0.8.1a4/nbsite/_shared_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/_shared_static/alert.css
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/_shared_static/dataframe.css
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/_shared_static/gallery.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/_shared_static/holoviz-icon-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/_shared_static/mystnb.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/_shared_static/nbsite.css
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/_shared_static/notebook.css
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/_shared_static/scroller.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:42:19.312173 nbsite-0.8.1a4/nbsite/_shared_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/_shared_templates/copyright-last-updated.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/_shared_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/_shared_templates/sidebar-nav-bs.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13156 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:42:19.312173 nbsite-0.8.1a4/nbsite/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/gallery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30951 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/gallery/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/gallery/thumbnailer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/ipystartup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18133 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/nbbuild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/paramdoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:42:19.312173 nbsite-0.8.1a4/nbsite/pyodide/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/pyodide/ServiceHandler.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/pyodide/ServiceWorker.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/pyodide/WebWorker.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/pyodide/WorkerHandler.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16934 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/pyodide/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:42:19.316173 nbsite-0.8.1a4/nbsite/pyodide/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/pyodide/_static/run_cell.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/pyodide/_static/runbutton.css
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/pyodide/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/shared_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:42:19.308173 nbsite-0.8.1a4/nbsite/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:42:19.316173 nbsite-0.8.1a4/nbsite/templates/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/templates/basic/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/templates/basic/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/templates/basic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:42:19.316173 nbsite-0.8.1a4/nbsite/templates/holoviz/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/templates/holoviz/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/templates/holoviz/about.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/templates/holoviz/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/templates/holoviz/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:42:19.316173 nbsite-0.8.1a4/nbsite/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18588 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/tests/test_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/nbsite/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:42:19.312173 nbsite-0.8.1a4/nbsite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-06-14 14:42:19.000000 nbsite-0.8.1a4/nbsite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-14 14:42:19.000000 nbsite-0.8.1a4/nbsite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 14:42:19.000000 nbsite-0.8.1a4/nbsite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-14 14:42:19.000000 nbsite-0.8.1a4/nbsite.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-14 14:42:19.000000 nbsite-0.8.1a4/nbsite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 14:42:19.000000 nbsite-0.8.1a4/nbsite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:42:19.316173 nbsite-0.8.1a4/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/scripts/nbsite_cleandisthtml.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5851 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/scripts/nbsite_fix_links.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      132 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/scripts/nbsite_from_tmplate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11126 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/scripts/nbsite_generate_modules.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      556 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/scripts/nbsite_nbpagebuild.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-14 14:42:19.316173 nbsite-0.8.1a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-06-14 14:41:24.000000 nbsite-0.8.1a4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nbsite-0.8.1a3/LICENSE.txt` & `nbsite-0.8.1a4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/PKG-INFO` & `nbsite-0.8.1a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbsite
-Version: 0.8.1a3
+Version: 0.8.1a4
 Summary: Build a tested, sphinx-based website from notebooks.
 Home-page: https://nbsite.holoviz.org
 Author: HoloViz developers
 Author-email: developers@holoviz.org
 Maintainer: HoloViz developers
 Maintainer-email: developers@holoviz.org
 License: BSD-3
```

### Comparing `nbsite-0.8.1a3/README.md` & `nbsite-0.8.1a4/README.md`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/nbsite/__main__.py` & `nbsite-0.8.1a4/nbsite/__main__.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/nbsite/_shared_static/alert.css` & `nbsite-0.8.1a4/nbsite/_shared_static/alert.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/nbsite/_shared_static/dataframe.css` & `nbsite-0.8.1a4/nbsite/_shared_static/dataframe.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/nbsite/_shared_static/holoviz-icon-white.svg` & `nbsite-0.8.1a4/nbsite/_shared_static/holoviz-icon-white.svg`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/nbsite/_shared_static/mystnb.css` & `nbsite-0.8.1a4/nbsite/_shared_static/mystnb.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/nbsite/_shared_static/nbsite.css` & `nbsite-0.8.1a4/nbsite/_shared_static/nbsite.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/nbsite/_shared_static/notebook.css` & `nbsite-0.8.1a4/nbsite/_shared_static/notebook.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/nbsite/_shared_static/scroller.css` & `nbsite-0.8.1a4/nbsite/_shared_static/scroller.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/nbsite/_shared_templates/copyright-last-updated.html` & `nbsite-0.8.1a4/nbsite/_shared_templates/copyright-last-updated.html`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/nbsite/_shared_templates/layout.html` & `nbsite-0.8.1a4/nbsite/_shared_templates/layout.html`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/nbsite/cmd.py` & `nbsite-0.8.1a4/nbsite/cmd.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/nbsite/gallery/gen.py` & `nbsite-0.8.1a4/nbsite/gallery/gen.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/nbsite/gallery/thumbnailer.py` & `nbsite-0.8.1a4/nbsite/gallery/thumbnailer.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/nbsite/nbbuild.py` & `nbsite-0.8.1a4/nbsite/nbbuild.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/nbsite/paramdoc.py` & `nbsite-0.8.1a4/nbsite/paramdoc.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/nbsite/pyodide/ServiceWorker.js` & `nbsite-0.8.1a4/nbsite/pyodide/ServiceWorker.js`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/nbsite/pyodide/WebWorker.js` & `nbsite-0.8.1a4/nbsite/pyodide/WebWorker.js`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/nbsite/pyodide/WorkerHandler.js` & `nbsite-0.8.1a4/nbsite/pyodide/WorkerHandler.js`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/nbsite/pyodide/__init__.py` & `nbsite-0.8.1a4/nbsite/pyodide/__init__.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/nbsite/pyodide/_static/run_cell.js` & `nbsite-0.8.1a4/nbsite/pyodide/_static/run_cell.js`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/nbsite/pyodide/_static/runbutton.css` & `nbsite-0.8.1a4/nbsite/pyodide/_static/runbutton.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/nbsite/pyodide/site.webmanifest` & `nbsite-0.8.1a4/nbsite/pyodide/site.webmanifest`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/nbsite/shared_conf.py` & `nbsite-0.8.1a4/nbsite/shared_conf.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/nbsite/templates/basic/conf.py` & `nbsite-0.8.1a4/nbsite/templates/basic/conf.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/nbsite/templates/holoviz/conf.py` & `nbsite-0.8.1a4/nbsite/templates/holoviz/conf.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/nbsite/tests/test_cmd.py` & `nbsite-0.8.1a4/nbsite/tests/test_cmd.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/nbsite/tests/test_util.py` & `nbsite-0.8.1a4/nbsite/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/nbsite/util.py` & `nbsite-0.8.1a4/nbsite/util.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/nbsite.egg-info/PKG-INFO` & `nbsite-0.8.1a4/nbsite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbsite
-Version: 0.8.1a3
+Version: 0.8.1a4
 Summary: Build a tested, sphinx-based website from notebooks.
 Home-page: https://nbsite.holoviz.org
 Author: HoloViz developers
 Author-email: developers@holoviz.org
 Maintainer: HoloViz developers
 Maintainer-email: developers@holoviz.org
 License: BSD-3
```

### Comparing `nbsite-0.8.1a3/nbsite.egg-info/SOURCES.txt` & `nbsite-0.8.1a4/nbsite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/pyproject.toml` & `nbsite-0.8.1a4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/scripts/nbsite_cleandisthtml.py` & `nbsite-0.8.1a4/scripts/nbsite_cleandisthtml.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/scripts/nbsite_fix_links.py` & `nbsite-0.8.1a4/scripts/nbsite_fix_links.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/scripts/nbsite_generate_modules.py` & `nbsite-0.8.1a4/scripts/nbsite_generate_modules.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/scripts/nbsite_nbpagebuild.py` & `nbsite-0.8.1a4/scripts/nbsite_nbpagebuild.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/setup.cfg` & `nbsite-0.8.1a4/setup.cfg`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a3/setup.py` & `nbsite-0.8.1a4/setup.py`

 * *Files identical despite different names*

