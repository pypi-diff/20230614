# Comparing `tmp/fig2sketch-0.2.6.tar.gz` & `tmp/fig2sketch-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fig2sketch-0.2.6.tar", last modified: Tue Apr 18 13:57:01 2023, max compression
+gzip compressed data, was "fig2sketch-0.2.7.tar", last modified: Wed Jun 14 07:55:49 2023, max compression
```

## Comparing `fig2sketch-0.2.6.tar` & `fig2sketch-0.2.7.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:57:01.052606 fig2sketch-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-04-18 13:57:01.052606 fig2sketch-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 13:57:01.052606 fig2sketch-0.2.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:57:01.044606 fig2sketch-0.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:57:01.048606 fig2sketch-0.2.6/src/converter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/artboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/component.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/document.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/font.py
--rw-r--r--   0 runner    (1001) docker     (123)    34002 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/font_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    10565 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/positioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/prototype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/rectangle.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/shape_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/shape_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/slice.py
--rw-r--r--   0 runner    (1001) docker     (123)    12855 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)    12602 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/converter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:57:01.048606 fig2sketch-0.2.6/src/fig2sketch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-04-18 13:57:01.000000 fig2sketch-0.2.6/src/fig2sketch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-18 13:57:01.000000 fig2sketch-0.2.6/src/fig2sketch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 13:57:01.000000 fig2sketch-0.2.6/src/fig2sketch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-18 13:57:01.000000 fig2sketch-0.2.6/src/fig2sketch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-18 13:57:01.000000 fig2sketch-0.2.6/src/fig2sketch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-18 13:57:01.000000 fig2sketch-0.2.6/src/fig2sketch.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     3382 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/fig2sketch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:57:01.048606 fig2sketch-0.2.6/src/figformat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/figformat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/figformat/decodefig.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/figformat/fig2tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/figformat/kiwi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/figformat/vector_network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:57:01.052606 fig2sketch-0.2.6/src/sketchformat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/sketchformat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/sketchformat/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/sketchformat/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/sketchformat/layer_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/sketchformat/layer_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/sketchformat/layer_shape.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/sketchformat/prototype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:57:01.052606 fig2sketch-0.2.6/src/sketchformat/serialize/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/sketchformat/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/sketchformat/serialize/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/sketchformat/serialize/orjson.py
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/sketchformat/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-18 13:56:51.000000 fig2sketch-0.2.6/src/sketchformat/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:55:49.679798 fig2sketch-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-06-14 07:55:49.679798 fig2sketch-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 07:55:49.679798 fig2sketch-0.2.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:55:49.675798 fig2sketch-0.2.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:55:49.679798 fig2sketch-0.2.7/src/converter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/converter/artboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/converter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/converter/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/converter/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/converter/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/converter/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/converter/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/converter/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/converter/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34002 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/converter/font_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/converter/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11281 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/converter/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/converter/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/converter/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/converter/positioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/converter/prototype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/converter/rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/converter/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/converter/shape_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/converter/shape_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/converter/slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/converter/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/converter/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12602 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/converter/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/converter/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/converter/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/converter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:55:49.679798 fig2sketch-0.2.7/src/fig2sketch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-06-14 07:55:49.000000 fig2sketch-0.2.7/src/fig2sketch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-14 07:55:49.000000 fig2sketch-0.2.7/src/fig2sketch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 07:55:49.000000 fig2sketch-0.2.7/src/fig2sketch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-14 07:55:49.000000 fig2sketch-0.2.7/src/fig2sketch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-14 07:55:49.000000 fig2sketch-0.2.7/src/fig2sketch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-14 07:55:49.000000 fig2sketch-0.2.7/src/fig2sketch.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3382 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/fig2sketch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:55:49.679798 fig2sketch-0.2.7/src/figformat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/figformat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/figformat/decodefig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/figformat/fig2tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/figformat/kiwi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/figformat/vector_network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:55:49.679798 fig2sketch-0.2.7/src/sketchformat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/sketchformat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/sketchformat/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/sketchformat/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/sketchformat/layer_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/sketchformat/layer_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/sketchformat/layer_shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/sketchformat/prototype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:55:49.679798 fig2sketch-0.2.7/src/sketchformat/serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/sketchformat/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/sketchformat/serialize/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/sketchformat/serialize/orjson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/sketchformat/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-14 07:55:35.000000 fig2sketch-0.2.7/src/sketchformat/text.py
```

### Comparing `fig2sketch-0.2.6/LICENSE` & `fig2sketch-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.6/PKG-INFO` & `fig2sketch-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fig2sketch
-Version: 0.2.6
+Version: 0.2.7
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: fast
 Provides-Extra: dev
 License-File: LICENSE
 
 # .fig to Sketch converter
```

### Comparing `fig2sketch-0.2.6/README.md` & `fig2sketch-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.6/pyproject.toml` & `fig2sketch-0.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.6/src/converter/artboard.py` & `fig2sketch-0.2.7/src/converter/artboard.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.6/src/converter/base.py` & `fig2sketch-0.2.7/src/converter/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         **masking(fig_node),  # type: ignore
         "style": process_styles(fig_node),
     }
 
     if (
         obj["hasClippingMask"]
         and obj["clippingMaskMode"] == ClippingMaskMode.OUTLINE
-        and not fig_node.get("f2sForceOutline")
+        and not fig_node.get("f2s_cropped_image")
     ):
         # Outline mask behave differently in fig files and Sketch in regard to fill/stroke colors
         # Remove fill
         obj["style"].fills = []
         # TODO: If we have stroke, we should remove it and enlarge ourselves to occupy that space
         # which is quite tricky in things like shapePaths. This should be pretty rare in practice
```

### Comparing `fig2sketch-0.2.6/src/converter/component.py` & `fig2sketch-0.2.7/src/converter/component.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.6/src/converter/context.py` & `fig2sketch-0.2.7/src/converter/context.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.6/src/converter/convert.py` & `fig2sketch-0.2.7/src/converter/convert.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.6/src/converter/document.py` & `fig2sketch-0.2.7/src/converter/document.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.6/src/converter/font.py` & `fig2sketch-0.2.7/src/converter/font.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.6/src/converter/font_features.py` & `fig2sketch-0.2.7/src/converter/font_features.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.6/src/converter/group.py` & `fig2sketch-0.2.7/src/converter/group.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.6/src/converter/instance.py` & `fig2sketch-0.2.7/src/converter/instance.py`

 * *Files 3% similar despite different names*

```diff
@@ -236,14 +236,15 @@
 
     # Apply overrides to children
     for c in detached_children:
         apply_overrides(c, fig_instance["guid"], all_overrides, fig_instance["derivedSymbolData"])
 
     fig_instance["children"] = detached_children
     fig_instance["type"] = "FRAME"
+    fig_instance["f2s_detached"] = True
 
 
 def apply_overrides(fig_node, instance_id, overrides, derived_symbol_data):
     guid = fig_node.get("overrideKey", fig_node["guid"])
 
     # Apply overrides
     child_overrides = []
@@ -271,18 +272,30 @@
         if len(guids) > 1:
             child_derived_data.append({**derived, "guidPath": {"guids": guids[1:]}})
         else:
             if "size" in derived:
                 fig_node["size"] = derived["size"]
             if "transform" in derived:
                 fig_node["transform"] = derived["transform"]
+            # Should we do all properties instead?
+            # A lot of them can be potentially set by derived data
+            # by things like scaling the instance
+            if "strokeWeight" in derived:
+                fig_node["strokeWeight"] = derived["strokeWeight"]
 
     # Generate a unique ID by concatenating instance_id + node_id
-    fig_node["guid"] = tuple(j for i in (instance_id, guid) for j in i)
+    fig_node["guid"] = tuple(j for i in (instance_id, fig_node["guid"]) for j in i)
 
     # If it's an instance, pass the overrides down. Otherwise, convert the children
     if fig_node["type"] == "INSTANCE":
         fig_node["symbolData"]["symbolOverrides"] += child_overrides
         fig_node["derivedSymbolData"] += child_derived_data
     else:
+        if fig_node.get("f2s_detached"):
+            # This was previously an instance that was detached before this usage
+            # We didn't change the override keys of children, and they are still relative
+            # to the symbol, so we have to pass the key without our guid prefix
+            overrides = child_overrides
+            derived_symbol_data = child_derived_data
+
         for c in fig_node.get("children", []):
             apply_overrides(c, instance_id, overrides, derived_symbol_data)
```

### Comparing `fig2sketch-0.2.6/src/converter/meta.py` & `fig2sketch-0.2.7/src/converter/meta.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.6/src/converter/page.py` & `fig2sketch-0.2.7/src/converter/page.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     return page
 
 
 def make_page(guid: Sequence[int], name: str, suffix: bytes = b"") -> Page:
     return Page(
         do_objectID=utils.gen_object_id(guid, suffix),
-        frame=Rect(height=300, width=300, x=0, y=0),
+        frame=Rect(height=0, width=0, x=0, y=0),
         name=name,
         resizingConstraint=63,
         rotation=0.0,
         style=Style(do_objectID=utils.gen_object_id(guid, suffix + b"style")),
         hasClickThrough=True,
     )
```

### Comparing `fig2sketch-0.2.6/src/converter/positioning.py` & `fig2sketch-0.2.7/src/converter/positioning.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.6/src/converter/prototype.py` & `fig2sketch-0.2.7/src/converter/prototype.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.6/src/converter/rectangle.py` & `fig2sketch-0.2.7/src/converter/rectangle.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.6/src/converter/shape_group.py` & `fig2sketch-0.2.7/src/converter/shape_group.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.6/src/converter/shape_path.py` & `fig2sketch-0.2.7/src/converter/shape_path.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.6/src/converter/style.py` & `fig2sketch-0.2.7/src/converter/style.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
             # Solid color backgrounds do not support specifying the opacity
             # Instead, it must be set in the color itself
             return Fill.Color(
                 convert_color(fig_fill["color"], fig_fill["opacity"]),
                 isEnabled=fig_fill["visible"],
             )
         case {"type": "IMAGE"}:
-            if is_cropped_image(fig_fill):
+            if is_cropped_image(fig_fill) and not fig_node.get("f2s_cropped_image"):
                 # Extract images to a separate layer and retrigger conversion
                 convert_crop_image_to_mask(fig_node)
 
             if "paintFilter" in fig_fill:
                 utils.log_conversion_warning("STY005", fig_node)
 
             return Fill.Image(
@@ -164,15 +164,15 @@
             "opacity": old["opacity"],
             "resizeToFit": True,
             "children": [
                 {
                     **content,
                     "mask": True,
                     "maskType": "OUTLINE",
-                    "f2sForceOutline": True,
+                    "f2s_cropped_image": True,
                 },
                 *cropped_images,
             ],
         }
     )
     raise Fig2SketchNodeChanged
```

### Comparing `fig2sketch-0.2.6/src/converter/symbol.py` & `fig2sketch-0.2.7/src/converter/symbol.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.6/src/converter/text.py` & `fig2sketch-0.2.7/src/converter/text.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.6/src/converter/tree.py` & `fig2sketch-0.2.7/src/converter/tree.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,19 @@
 from sketchformat.layer_common import AbstractLayer
 from sketchformat.layer_group import AbstractLayerGroup
 from typing import Dict, Callable, Any
 import traceback
 from .errors import *
 from . import utils
 
+
+def ignored_layer_type(fig_layer: dict) -> AbstractLayer:
+    raise Fig2SketchWarning("LAY001")
+
+
 CONVERTERS: Dict[str, Callable[[dict], AbstractLayer]] = {
     "CANVAS": page.convert,
     "ARTBOARD": artboard.convert,
     "GROUP": group.convert,
     "ROUNDED_RECTANGLE": rectangle.convert,
     "RECTANGLE": rectangle.convert,
     "ELLIPSE": shape.convert_oval,
@@ -31,14 +36,15 @@
     "REGULAR_POLYGON": shape.convert_polygon,
     "TEXT": text.convert,
     "BOOLEAN_OPERATION": shape_group.convert,
     "LINE": shape_path.convert_line,
     "SLICE": slice.convert,
     "SYMBOL": symbol.convert,
     "INSTANCE": instance.convert,
+    "STICKY": ignored_layer_type,
 }
 
 POST_PROCESSING: Dict[str, Callable[[dict, Any], AbstractLayer]] = {
     "CANVAS": page.add_page_background,
     "ARTBOARD": artboard.post_process_frame,
     "GROUP": group.post_process_frame,
     "BOOLEAN_OPERATION": shape_group.post_process,
@@ -46,15 +52,15 @@
     "INSTANCE": instance.post_process,
 }
 
 
 def convert_node(fig_node: dict, parent_type: str) -> AbstractLayer:
     name = fig_node["name"]
     type_ = get_node_type(fig_node, parent_type)
-    logging.debug(f"{type_}: {name}")
+    logging.debug(f"{type_}: {name} {fig_node['guid']}")
 
     try:
         sketch_item = CONVERTERS[type_](fig_node)
     except Fig2SketchNodeChanged:
         # The fig_node was modified, retry converting with the new values
         # This happens on instance detaching
         return convert_node(fig_node, parent_type)
```

### Comparing `fig2sketch-0.2.6/src/converter/user.py` & `fig2sketch-0.2.7/src/converter/user.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.6/src/converter/utils.py` & `fig2sketch-0.2.7/src/converter/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,15 @@
     "GRD006": "has a row layout with an offset that is not supported. The offset will be ignored",
     "GRD007": "has a row layout with non-integer ratio between gutter and row size. The row layout will not be converted",
     "GRD008": "has a row and column layout. The rows will only be as wide as the columns (instead of taking the entire width of the artboard)",
     "IMG001": "appears to be corrupted in the .fig file, it will not be converted. Try passing --force-convert-images to try to convert it anyway",
     "IMG002": "appears to be corrupted in the .fig file, it will not be converted",
     "IMG003": "is missing from the .fig file, it will not be converted",
     "IMG004": "appears to be corrupted in the .fig file ({error}), it will not be converted",
+    "LAY001": "is an unsupported layer type, it will not be converted",
 }
 
 
 def log_conversion_warning(warning_code: str, fig_node: dict, **kw: list) -> None:
     if fig_node["guid"] not in issued_warnings:
         issued_warnings[fig_node["guid"]] = [warning_code]
     elif warning_code not in issued_warnings[fig_node["guid"]]:
```

### Comparing `fig2sketch-0.2.6/src/fig2sketch.egg-info/PKG-INFO` & `fig2sketch-0.2.7/src/fig2sketch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fig2sketch
-Version: 0.2.6
+Version: 0.2.7
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: fast
 Provides-Extra: dev
 License-File: LICENSE
 
 # .fig to Sketch converter
```

### Comparing `fig2sketch-0.2.6/src/fig2sketch.egg-info/SOURCES.txt` & `fig2sketch-0.2.7/src/fig2sketch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.6/src/fig2sketch.py` & `fig2sketch-0.2.7/src/fig2sketch.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.6/src/figformat/decodefig.py` & `fig2sketch-0.2.7/src/figformat/decodefig.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.6/src/figformat/fig2tree.py` & `fig2sketch-0.2.7/src/figformat/fig2tree.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.6/src/figformat/kiwi.py` & `fig2sketch-0.2.7/src/figformat/kiwi.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.6/src/figformat/vector_network.py` & `fig2sketch-0.2.7/src/figformat/vector_network.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.6/src/sketchformat/common.py` & `fig2sketch-0.2.7/src/sketchformat/common.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.6/src/sketchformat/document.py` & `fig2sketch-0.2.7/src/sketchformat/document.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.6/src/sketchformat/layer_common.py` & `fig2sketch-0.2.7/src/sketchformat/layer_common.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.6/src/sketchformat/layer_group.py` & `fig2sketch-0.2.7/src/sketchformat/layer_group.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.6/src/sketchformat/layer_shape.py` & `fig2sketch-0.2.7/src/sketchformat/layer_shape.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.6/src/sketchformat/prototype.py` & `fig2sketch-0.2.7/src/sketchformat/prototype.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.6/src/sketchformat/serialize/json.py` & `fig2sketch-0.2.7/src/sketchformat/serialize/json.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.6/src/sketchformat/serialize/orjson.py` & `fig2sketch-0.2.7/src/sketchformat/serialize/orjson.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.6/src/sketchformat/style.py` & `fig2sketch-0.2.7/src/sketchformat/style.py`

 * *Files identical despite different names*

### Comparing `fig2sketch-0.2.6/src/sketchformat/text.py` & `fig2sketch-0.2.7/src/sketchformat/text.py`

 * *Files identical despite different names*

