# Comparing `tmp/edspdf-poppler-0.0.0.tar.gz` & `tmp/edspdf-poppler-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edspdf-poppler-0.0.0.tar", last modified: Tue Jun 13 08:23:46 2023, max compression
+gzip compressed data, was "edspdf-poppler-0.1.0.tar", last modified: Tue Jun 13 09:19:13 2023, max compression
```

## Comparing `edspdf-poppler-0.0.0.tar` & `edspdf-poppler-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 perceval   (501) staff       (20)        0 2023-06-13 08:23:46.733520 edspdf-poppler-0.0.0/
--rw-r--r--   0 perceval   (501) staff       (20)    18092 2023-06-12 22:43:21.000000 edspdf-poppler-0.0.0/LICENSE
--rw-r--r--   0 perceval   (501) staff       (20)    22806 2023-06-13 08:23:46.733345 edspdf-poppler-0.0.0/PKG-INFO
--rw-r--r--   0 perceval   (501) staff       (20)     1503 2023-06-12 22:43:21.000000 edspdf-poppler-0.0.0/README.md
-drwxr-xr-x   0 perceval   (501) staff       (20)        0 2023-06-13 08:23:46.730939 edspdf-poppler-0.0.0/edspdf_poppler/
--rw-r--r--   0 perceval   (501) staff       (20)     5667 2023-06-13 08:22:46.000000 edspdf-poppler-0.0.0/edspdf_poppler/__init__.py
--rw-r--r--   0 perceval   (501) staff       (20)   467129 2023-06-13 08:23:45.000000 edspdf-poppler-0.0.0/edspdf_poppler/bindings.cpp
--rwxr-xr-x   0 perceval   (501) staff       (20)   138314 2023-06-12 22:19:39.000000 edspdf-poppler-0.0.0/edspdf_poppler/bindings.cpython-38-darwin.so
-drwxr-xr-x   0 perceval   (501) staff       (20)        0 2023-06-13 08:23:46.732541 edspdf-poppler-0.0.0/edspdf_poppler.egg-info/
--rw-r--r--   0 perceval   (501) staff       (20)    22806 2023-06-13 08:23:46.000000 edspdf-poppler-0.0.0/edspdf_poppler.egg-info/PKG-INFO
--rw-r--r--   0 perceval   (501) staff       (20)      436 2023-06-13 08:23:46.000000 edspdf-poppler-0.0.0/edspdf_poppler.egg-info/SOURCES.txt
--rw-r--r--   0 perceval   (501) staff       (20)        1 2023-06-13 08:23:46.000000 edspdf-poppler-0.0.0/edspdf_poppler.egg-info/dependency_links.txt
--rw-r--r--   0 perceval   (501) staff       (20)       71 2023-06-13 08:23:46.000000 edspdf-poppler-0.0.0/edspdf_poppler.egg-info/entry_points.txt
--rw-r--r--   0 perceval   (501) staff       (20)      497 2023-06-13 08:23:46.000000 edspdf-poppler-0.0.0/edspdf_poppler.egg-info/requires.txt
--rw-r--r--   0 perceval   (501) staff       (20)       15 2023-06-13 08:23:46.000000 edspdf-poppler-0.0.0/edspdf_poppler.egg-info/top_level.txt
--rw-r--r--   0 perceval   (501) staff       (20)     3611 2023-06-12 22:43:21.000000 edspdf-poppler-0.0.0/pyproject.toml
--rw-r--r--   0 perceval   (501) staff       (20)       38 2023-06-13 08:23:46.733565 edspdf-poppler-0.0.0/setup.cfg
--rw-r--r--   0 perceval   (501) staff       (20)     2110 2023-06-12 22:43:21.000000 edspdf-poppler-0.0.0/setup.py
-drwxr-xr-x   0 perceval   (501) staff       (20)        0 2023-06-13 08:23:46.732989 edspdf-poppler-0.0.0/tests/
--rw-r--r--   0 perceval   (501) staff       (20)      792 2023-06-12 22:43:21.000000 edspdf-poppler-0.0.0/tests/test_poppler_extractor.py
--rw-r--r--   0 perceval   (501) staff       (20)     4048 2023-06-12 22:43:21.000000 edspdf-poppler-0.0.0/tests/test_styled_aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:19:13.733200 edspdf-poppler-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-13 09:15:54.000000 edspdf-poppler-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22785 2023-06-13 09:19:13.733200 edspdf-poppler-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-13 09:15:54.000000 edspdf-poppler-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:19:13.729200 edspdf-poppler-0.1.0/edspdf_poppler/
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-06-13 09:15:54.000000 edspdf-poppler-0.1.0/edspdf_poppler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   467174 2023-06-13 09:19:12.000000 edspdf-poppler-0.1.0/edspdf_poppler/bindings.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:19:13.733200 edspdf-poppler-0.1.0/edspdf_poppler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22785 2023-06-13 09:19:13.000000 edspdf-poppler-0.1.0/edspdf_poppler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-13 09:19:13.000000 edspdf-poppler-0.1.0/edspdf_poppler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:19:13.000000 edspdf-poppler-0.1.0/edspdf_poppler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-13 09:19:13.000000 edspdf-poppler-0.1.0/edspdf_poppler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-13 09:19:13.000000 edspdf-poppler-0.1.0/edspdf_poppler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-13 09:19:13.000000 edspdf-poppler-0.1.0/edspdf_poppler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-06-13 09:15:54.000000 edspdf-poppler-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 09:19:13.733200 edspdf-poppler-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-13 09:15:54.000000 edspdf-poppler-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:19:13.733200 edspdf-poppler-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-13 09:15:54.000000 edspdf-poppler-0.1.0/tests/test_poppler_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-06-13 09:15:54.000000 edspdf-poppler-0.1.0/tests/test_styled_aggregation.py
```

### Comparing `edspdf-poppler-0.0.0/LICENSE` & `edspdf-poppler-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edspdf-poppler-0.0.0/PKG-INFO` & `edspdf-poppler-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edspdf-poppler
-Version: 0.0.0
+Version: 0.1.0
 Summary: Poppler extension for EDS-PDF
 Author-email: Perceval Wajsbürt <perceval.wajsburt-ext@aphp.fr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
@@ -345,15 +345,14 @@
         
 Project-URL: homepage, https://github.com/aphp/edspdf-poppler/
 Project-URL: repository, https://github.com/aphp/edspdf-poppler/
 Project-URL: documentation, https://aphp.github.io/edspdf-poppler/
 Requires-Python: <4.0,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-Provides-Extra: docs
 License-File: LICENSE
 
 ![Tests](https://img.shields.io/github/actions/workflow/status/aphp/edspdf-poppler/tests.yml?branch=main&label=tests&style=flat-square)
 [![Documentation](https://img.shields.io/github/actions/workflow/status/aphp/edspdf-poppler/documentation.yml?branch=main&label=docs&style=flat-square)](https://aphp.github.io/edspdf-poppler/latest/)
 [![PyPI](https://img.shields.io/pypi/v/edspdf-poppler?color=blue&style=flat-square)](https://pypi.org/project/edspdf-poppler/)
 [![Codecov](https://img.shields.io/codecov/c/github/aphp/edspdf-poppler?logo=codecov&style=flat-square)](https://codecov.io/gh/aphp/edspdf-poppler)
 [![DOI](https://zenodo.org/badge/517726737.svg)](https://zenodo.org/badge/latestdoi/517726737)
```

### Comparing `edspdf-poppler-0.0.0/README.md` & `edspdf-poppler-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `edspdf-poppler-0.0.0/edspdf_poppler/__init__.py` & `edspdf-poppler-0.1.0/edspdf_poppler/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from .bindings import Document
 except ModuleNotFoundError:
     raise ImportError(
         "Poppler was not correctly built, you won't be able to use the "
         "poppler-extractor component to parse PDFs."
     )
 
-__version__ = "0.0.0"
+__version__ = "0.1.0"
 
 
 @registry.factory.register("poppler-extractor")
 class PopplerExtractor:
     """
     We provide a PDF line extractor built on top of
     [Poppler](https://poppler.freedesktop.org/).
```

### Comparing `edspdf-poppler-0.0.0/edspdf_poppler/bindings.cpp` & `edspdf-poppler-0.1.0/edspdf_poppler/bindings.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 /* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/Users/perceval/Development/edspdf-poppler/edspdf_poppler/poppler_src/goo/GooString.h",
-            "/Users/perceval/Development/edspdf-poppler/edspdf_poppler/poppler_src/poppler/Annot.h",
-            "/Users/perceval/Development/edspdf-poppler/edspdf_poppler/poppler_src/poppler/Dict.h",
-            "/Users/perceval/Development/edspdf-poppler/edspdf_poppler/poppler_src/poppler/GlobalParams.h",
-            "/Users/perceval/Development/edspdf-poppler/edspdf_poppler/poppler_src/poppler/Object.h",
-            "/Users/perceval/Development/edspdf-poppler/edspdf_poppler/poppler_src/poppler/OutputDev.h",
-            "/Users/perceval/Development/edspdf-poppler/edspdf_poppler/poppler_src/poppler/PDFDoc.h",
-            "/Users/perceval/Development/edspdf-poppler/edspdf_poppler/poppler_src/poppler/PDFDocFactory.h",
-            "/Users/perceval/Development/edspdf-poppler/edspdf_poppler/poppler_src/poppler/Stream.h",
-            "/Users/perceval/Development/edspdf-poppler/edspdf_poppler/poppler_src/poppler/TextOutputDev.h"
+            "/home/runner/work/edspdf-poppler/edspdf-poppler/edspdf_poppler/poppler_src/goo/GooString.h",
+            "/home/runner/work/edspdf-poppler/edspdf-poppler/edspdf_poppler/poppler_src/poppler/Annot.h",
+            "/home/runner/work/edspdf-poppler/edspdf-poppler/edspdf_poppler/poppler_src/poppler/Dict.h",
+            "/home/runner/work/edspdf-poppler/edspdf-poppler/edspdf_poppler/poppler_src/poppler/GlobalParams.h",
+            "/home/runner/work/edspdf-poppler/edspdf-poppler/edspdf_poppler/poppler_src/poppler/Object.h",
+            "/home/runner/work/edspdf-poppler/edspdf-poppler/edspdf_poppler/poppler_src/poppler/OutputDev.h",
+            "/home/runner/work/edspdf-poppler/edspdf-poppler/edspdf_poppler/poppler_src/poppler/PDFDoc.h",
+            "/home/runner/work/edspdf-poppler/edspdf-poppler/edspdf_poppler/poppler_src/poppler/PDFDocFactory.h",
+            "/home/runner/work/edspdf-poppler/edspdf-poppler/edspdf_poppler/poppler_src/poppler/Stream.h",
+            "/home/runner/work/edspdf-poppler/edspdf-poppler/edspdf_poppler/poppler_src/poppler/TextOutputDev.h"
         ],
         "extra_compile_args": [
-            "-std=c++17",
-            "-stdlib=libc++"
+            "-std=c++17"
         ],
         "include_dirs": [
-            "/Users/perceval/Development/edspdf-poppler/edspdf_poppler/poppler_src",
-            "/Users/perceval/Development/edspdf-poppler/edspdf_poppler/poppler_src/poppler"
+            "/home/runner/work/edspdf-poppler/edspdf-poppler/edspdf_poppler/poppler_src",
+            "/home/runner/work/edspdf-poppler/edspdf-poppler/edspdf_poppler/poppler_src/poppler"
         ],
         "language": "c++",
         "libraries": [
             "poppler"
         ],
         "library_dirs": [
-            "/Users/perceval/Development/edspdf-poppler/edspdf_poppler/poppler_src"
+            "/home/runner/work/edspdf-poppler/edspdf-poppler/edspdf_poppler/poppler_src"
         ],
         "name": "edspdf_poppler.bindings",
         "runtime_library_dirs": [
-            "/Users/perceval/Development/edspdf-poppler/edspdf_poppler/poppler_src",
-            "/Users/perceval/Development/edspdf-poppler/edspdf_poppler"
+            "/home/runner/work/edspdf-poppler/edspdf-poppler/edspdf_poppler/poppler_src",
+            "/home/runner/work/edspdf-poppler/edspdf-poppler/edspdf_poppler"
         ],
         "sources": [
             "edspdf_poppler/bindings.pyx"
         ]
     },
     "module_name": "edspdf_poppler.bindings"
 }
```

### Comparing `edspdf-poppler-0.0.0/edspdf_poppler.egg-info/PKG-INFO` & `edspdf-poppler-0.1.0/edspdf_poppler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edspdf-poppler
-Version: 0.0.0
+Version: 0.1.0
 Summary: Poppler extension for EDS-PDF
 Author-email: Perceval Wajsbürt <perceval.wajsburt-ext@aphp.fr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
@@ -345,15 +345,14 @@
         
 Project-URL: homepage, https://github.com/aphp/edspdf-poppler/
 Project-URL: repository, https://github.com/aphp/edspdf-poppler/
 Project-URL: documentation, https://aphp.github.io/edspdf-poppler/
 Requires-Python: <4.0,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-Provides-Extra: docs
 License-File: LICENSE
 
 ![Tests](https://img.shields.io/github/actions/workflow/status/aphp/edspdf-poppler/tests.yml?branch=main&label=tests&style=flat-square)
 [![Documentation](https://img.shields.io/github/actions/workflow/status/aphp/edspdf-poppler/documentation.yml?branch=main&label=docs&style=flat-square)](https://aphp.github.io/edspdf-poppler/latest/)
 [![PyPI](https://img.shields.io/pypi/v/edspdf-poppler?color=blue&style=flat-square)](https://pypi.org/project/edspdf-poppler/)
 [![Codecov](https://img.shields.io/codecov/c/github/aphp/edspdf-poppler?logo=codecov&style=flat-square)](https://codecov.io/gh/aphp/edspdf-poppler)
 [![DOI](https://zenodo.org/badge/517726737.svg)](https://zenodo.org/badge/latestdoi/517726737)
```

### Comparing `edspdf-poppler-0.0.0/pyproject.toml` & `edspdf-poppler-0.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -20,23 +20,14 @@
 
 [project.optional-dependencies]
 dev = [
     "pre-commit~=2.18.1",
     "pytest~=7.1.1",
     "pytest-cov~=3.0.0",
 ]
-docs = [
-    "mike~=1.1.2",
-    "mkdocs@git+https://github.com/mkdocs/mkdocs.git@5af8bd30538ff8f0cfb698c8b90c3020da319f92",
-    "mkdocstrings@git+https://github.com/percevalw/mkdocstrings.git@7c50413ebdffdcbfad40b69d1574f55ba4f88a5c",
-    "mkdocs-autorefs@git+https://github.com/percevalw/mkdocs-autorefs.git@0652a0031a5402c5abcbac8cf1e846fcadbbacbc",
-    "mkdocs-material~=9.1.0",
-    "mkdocstrings-python~=0.8.3",
-    "mkdocs-autorefs~=0.4.1",
-]
 
 
 [project.entry-points."edspdf_factories"]
 # Extractors
 "poppler-extractor" = "edspdf_poppler:PopplerExtractor"
 
 [tool.setuptools.dynamic]
@@ -142,9 +133,10 @@
     exit 1
 fi
 """
 
 [tool.cibuildwheel.macos]
 # we also install gnu-sed to overcome the linux specific usage of sed in poppler's
 # CMakeLists.txt, and because we cannot upgrade poppler to enable manylinux_2014 builds
+archs = ["x86_64", "arm64"]
 before-all = "brew install freetype fontconfig gnu-sed"
 environment = { "PATH" = "/usr/local/opt/gnu-sed/libexec/gnubin:$PATH", "MACOSX_DEPLOYMENT_TARGET" = "10.13" }
```

### Comparing `edspdf-poppler-0.0.0/setup.py` & `edspdf-poppler-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `edspdf-poppler-0.0.0/tests/test_poppler_extractor.py` & `edspdf-poppler-0.1.0/tests/test_poppler_extractor.py`

 * *Files identical despite different names*

### Comparing `edspdf-poppler-0.0.0/tests/test_styled_aggregation.py` & `edspdf-poppler-0.1.0/tests/test_styled_aggregation.py`

 * *Files identical despite different names*

