# Comparing `tmp/spade_bokeh-0.1.2.tar.gz` & `tmp/spade_bokeh-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/spade_bokeh-0.1.2.tar", last modified: Mon Sep 17 18:04:45 2018, max compression
+gzip compressed data, was "spade_bokeh-0.2.0.tar", last modified: Wed Jun 14 11:01:04 2023, max compression
```

## Comparing `spade_bokeh-0.1.2.tar` & `spade_bokeh-0.2.0.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2018-09-17 18:04:45.000000 spade_bokeh-0.1.2/
--rw-r--r--   0 jpalanca   (501) staff       (20)     2283 2018-09-17 18:04:45.000000 spade_bokeh-0.1.2/PKG-INFO
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2018-09-17 18:04:45.000000 spade_bokeh-0.1.2/spade_bokeh.egg-info/
--rw-r--r--   0 jpalanca   (501) staff       (20)     2283 2018-09-17 18:04:45.000000 spade_bokeh-0.1.2/spade_bokeh.egg-info/PKG-INFO
--rw-r--r--   0 jpalanca   (501) staff       (20)        1 2018-09-17 16:01:52.000000 spade_bokeh-0.1.2/spade_bokeh.egg-info/not-zip-safe
--rw-r--r--   0 jpalanca   (501) staff       (20)     1032 2018-09-17 18:04:45.000000 spade_bokeh-0.1.2/spade_bokeh.egg-info/SOURCES.txt
--rw-r--r--   0 jpalanca   (501) staff       (20)       40 2018-09-17 18:04:45.000000 spade_bokeh-0.1.2/spade_bokeh.egg-info/requires.txt
--rw-r--r--   0 jpalanca   (501) staff       (20)       12 2018-09-17 18:04:45.000000 spade_bokeh-0.1.2/spade_bokeh.egg-info/top_level.txt
--rw-r--r--   0 jpalanca   (501) staff       (20)        1 2018-09-17 18:04:45.000000 spade_bokeh-0.1.2/spade_bokeh.egg-info/dependency_links.txt
--rw-r--r--   0 jpalanca   (501) staff       (20)     1071 2018-09-17 15:34:04.000000 spade_bokeh-0.1.2/LICENSE
--rw-r--r--   0 jpalanca   (501) staff       (20)       41 2018-09-17 17:57:58.000000 spade_bokeh-0.1.2/requirements.txt
--rw-r--r--   0 jpalanca   (501) staff       (20)     3580 2018-09-17 15:34:04.000000 spade_bokeh-0.1.2/CONTRIBUTING.rst
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2018-09-17 18:04:45.000000 spade_bokeh-0.1.2/tests/
--rw-r--r--   0 jpalanca   (501) staff       (20)      991 2018-09-17 17:26:03.000000 spade_bokeh-0.1.2/tests/test_spade_bokeh.py
--rw-r--r--   0 jpalanca   (501) staff       (20)      317 2018-09-17 17:57:58.000000 spade_bokeh-0.1.2/MANIFEST.in
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2018-09-17 18:04:45.000000 spade_bokeh-0.1.2/docs/
--rw-r--r--   0 jpalanca   (501) staff       (20)      315 2018-09-17 15:34:04.000000 spade_bokeh-0.1.2/docs/index.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)       33 2018-09-17 15:34:04.000000 spade_bokeh-0.1.2/docs/contributing.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)      612 2018-09-17 15:34:04.000000 spade_bokeh-0.1.2/docs/Makefile
--rwxr-xr-x   0 jpalanca   (501) staff       (20)     4917 2018-09-17 16:24:45.000000 spade_bokeh-0.1.2/docs/conf.py
--rw-r--r--   0 jpalanca   (501) staff       (20)       70 2018-09-17 16:25:22.000000 spade_bokeh-0.1.2/docs/modules.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)     5209 2018-09-17 16:47:05.000000 spade_bokeh-0.1.2/docs/usage.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)      773 2018-09-17 15:34:04.000000 spade_bokeh-0.1.2/docs/make.bat
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2018-09-17 18:04:45.000000 spade_bokeh-0.1.2/docs/_build/
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2018-09-17 18:04:45.000000 spade_bokeh-0.1.2/docs/_build/html/
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2018-09-17 18:04:45.000000 spade_bokeh-0.1.2/docs/_build/html/_static/
--rw-r--r--   0 jpalanca   (501) staff       (20)       90 2018-09-17 16:23:34.000000 spade_bokeh-0.1.2/docs/_build/html/_static/plus.png
--rw-r--r--   0 jpalanca   (501) staff       (20)      222 2018-09-17 16:23:34.000000 spade_bokeh-0.1.2/docs/_build/html/_static/down-pressed.png
--rw-r--r--   0 jpalanca   (501) staff       (20)      673 2018-09-17 16:23:34.000000 spade_bokeh-0.1.2/docs/_build/html/_static/ajax-loader.gif
--rw-r--r--   0 jpalanca   (501) staff       (20)      203 2018-09-17 16:23:34.000000 spade_bokeh-0.1.2/docs/_build/html/_static/up.png
--rw-r--r--   0 jpalanca   (501) staff       (20)      286 2018-09-17 16:23:34.000000 spade_bokeh-0.1.2/docs/_build/html/_static/file.png
--rw-r--r--   0 jpalanca   (501) staff       (20)      214 2018-09-17 16:23:34.000000 spade_bokeh-0.1.2/docs/_build/html/_static/up-pressed.png
--rw-r--r--   0 jpalanca   (501) staff       (20)      202 2018-09-17 16:23:34.000000 spade_bokeh-0.1.2/docs/_build/html/_static/down.png
--rw-r--r--   0 jpalanca   (501) staff       (20)       90 2018-09-17 16:23:34.000000 spade_bokeh-0.1.2/docs/_build/html/_static/minus.png
--rw-r--r--   0 jpalanca   (501) staff       (20)      641 2018-09-17 16:23:34.000000 spade_bokeh-0.1.2/docs/_build/html/_static/comment.png
--rw-r--r--   0 jpalanca   (501) staff       (20)      829 2018-09-17 16:23:34.000000 spade_bokeh-0.1.2/docs/_build/html/_static/comment-close.png
--rw-r--r--   0 jpalanca   (501) staff       (20)      756 2018-09-17 16:23:34.000000 spade_bokeh-0.1.2/docs/_build/html/_static/comment-bright.png
--rw-r--r--   0 jpalanca   (501) staff       (20)       28 2018-09-17 15:34:04.000000 spade_bokeh-0.1.2/docs/history.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)     1179 2018-09-17 15:34:04.000000 spade_bokeh-0.1.2/docs/installation.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)       28 2018-09-17 15:34:04.000000 spade_bokeh-0.1.2/docs/authors.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)       27 2018-09-17 15:34:04.000000 spade_bokeh-0.1.2/docs/readme.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)      350 2018-09-17 16:25:22.000000 spade_bokeh-0.1.2/docs/spade_bokeh.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)     1486 2018-09-17 18:01:56.000000 spade_bokeh-0.1.2/setup.py
--rw-r--r--   0 jpalanca   (501) staff       (20)      225 2018-09-17 18:01:56.000000 spade_bokeh-0.1.2/HISTORY.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)      156 2018-09-17 15:34:04.000000 spade_bokeh-0.1.2/AUTHORS.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)      454 2018-09-17 18:04:45.000000 spade_bokeh-0.1.2/setup.cfg
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2018-09-17 18:04:45.000000 spade_bokeh-0.1.2/spade_bokeh/
--rw-r--r--   0 jpalanca   (501) staff       (20)      218 2018-09-17 18:01:56.000000 spade_bokeh-0.1.2/spade_bokeh/__init__.py
--rw-r--r--   0 jpalanca   (501) staff       (20)     3055 2018-09-17 17:00:04.000000 spade_bokeh-0.1.2/spade_bokeh/spade_bokeh.py
--rw-r--r--   0 jpalanca   (501) staff       (20)     1065 2018-09-17 16:23:29.000000 spade_bokeh-0.1.2/README.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)      191 2018-09-17 16:21:46.000000 spade_bokeh-0.1.2/requirements_dev.txt
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-14 11:01:04.919117 spade_bokeh-0.2.0/
+-rw-r--r--   0 jpalanca   (501) staff       (20)      156 2018-09-17 15:34:04.000000 spade_bokeh-0.2.0/AUTHORS.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)     3580 2018-09-17 15:34:04.000000 spade_bokeh-0.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)      382 2023-06-14 10:59:15.000000 spade_bokeh-0.2.0/HISTORY.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1071 2018-09-17 15:34:04.000000 spade_bokeh-0.2.0/LICENSE
+-rw-r--r--   0 jpalanca   (501) staff       (20)      317 2018-09-17 17:57:58.000000 spade_bokeh-0.2.0/MANIFEST.in
+-rw-r--r--   0 jpalanca   (501) staff       (20)     2036 2023-06-14 11:01:04.919373 spade_bokeh-0.2.0/PKG-INFO
+-rw-r--r--   0 jpalanca   (501) staff       (20)      983 2023-06-14 10:59:15.000000 spade_bokeh-0.2.0/README.rst
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-14 11:01:04.899223 spade_bokeh-0.2.0/docs/
+-rw-r--r--   0 jpalanca   (501) staff       (20)      612 2018-09-17 15:34:04.000000 spade_bokeh-0.2.0/docs/Makefile
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-14 11:01:04.883084 spade_bokeh-0.2.0/docs/_build/
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-14 11:01:04.883250 spade_bokeh-0.2.0/docs/_build/html/
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-14 11:01:04.910650 spade_bokeh-0.2.0/docs/_build/html/_static/
+-rw-r--r--   0 jpalanca   (501) staff       (20)      673 2018-09-17 16:23:34.000000 spade_bokeh-0.2.0/docs/_build/html/_static/ajax-loader.gif
+-rw-r--r--   0 jpalanca   (501) staff       (20)      756 2018-09-17 16:23:34.000000 spade_bokeh-0.2.0/docs/_build/html/_static/comment-bright.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      829 2018-09-17 16:23:34.000000 spade_bokeh-0.2.0/docs/_build/html/_static/comment-close.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      641 2018-09-17 16:23:34.000000 spade_bokeh-0.2.0/docs/_build/html/_static/comment.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      222 2018-09-17 16:23:34.000000 spade_bokeh-0.2.0/docs/_build/html/_static/down-pressed.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      202 2018-09-17 16:23:34.000000 spade_bokeh-0.2.0/docs/_build/html/_static/down.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      286 2018-09-17 16:23:34.000000 spade_bokeh-0.2.0/docs/_build/html/_static/file.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)       90 2018-09-17 16:23:34.000000 spade_bokeh-0.2.0/docs/_build/html/_static/minus.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)       90 2018-09-17 16:23:34.000000 spade_bokeh-0.2.0/docs/_build/html/_static/plus.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      214 2018-09-17 16:23:34.000000 spade_bokeh-0.2.0/docs/_build/html/_static/up-pressed.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)      203 2018-09-17 16:23:34.000000 spade_bokeh-0.2.0/docs/_build/html/_static/up.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)       28 2018-09-17 15:34:04.000000 spade_bokeh-0.2.0/docs/authors.rst
+-rwxr-xr-x   0 jpalanca   (501) staff       (20)     4917 2018-09-17 16:24:45.000000 spade_bokeh-0.2.0/docs/conf.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)       33 2018-09-17 15:34:04.000000 spade_bokeh-0.2.0/docs/contributing.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)       28 2018-09-17 15:34:04.000000 spade_bokeh-0.2.0/docs/history.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)      315 2018-09-17 15:34:04.000000 spade_bokeh-0.2.0/docs/index.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1179 2018-09-17 15:34:04.000000 spade_bokeh-0.2.0/docs/installation.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)      773 2018-09-17 15:34:04.000000 spade_bokeh-0.2.0/docs/make.bat
+-rw-r--r--   0 jpalanca   (501) staff       (20)       70 2018-09-17 16:25:22.000000 spade_bokeh-0.2.0/docs/modules.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)       27 2018-09-17 15:34:04.000000 spade_bokeh-0.2.0/docs/readme.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)      350 2018-09-17 16:25:22.000000 spade_bokeh-0.2.0/docs/spade_bokeh.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)     5275 2023-06-14 10:59:15.000000 spade_bokeh-0.2.0/docs/usage.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)       41 2023-06-14 11:00:42.000000 spade_bokeh-0.2.0/requirements.txt
+-rw-r--r--   0 jpalanca   (501) staff       (20)      191 2023-06-14 10:55:51.000000 spade_bokeh-0.2.0/requirements_dev.txt
+-rw-r--r--   0 jpalanca   (501) staff       (20)      454 2023-06-14 11:01:04.920696 spade_bokeh-0.2.0/setup.cfg
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1585 2023-06-14 10:59:15.000000 spade_bokeh-0.2.0/setup.py
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-14 11:01:04.912507 spade_bokeh-0.2.0/spade_bokeh/
+-rw-r--r--   0 jpalanca   (501) staff       (20)      218 2023-06-14 10:59:15.000000 spade_bokeh-0.2.0/spade_bokeh/__init__.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)     3055 2018-09-17 17:00:04.000000 spade_bokeh-0.2.0/spade_bokeh/spade_bokeh.py
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-14 11:01:04.917137 spade_bokeh-0.2.0/spade_bokeh.egg-info/
+-rw-r--r--   0 jpalanca   (501) staff       (20)     2036 2023-06-14 11:01:04.000000 spade_bokeh-0.2.0/spade_bokeh.egg-info/PKG-INFO
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1050 2023-06-14 11:01:04.000000 spade_bokeh-0.2.0/spade_bokeh.egg-info/SOURCES.txt
+-rw-r--r--   0 jpalanca   (501) staff       (20)        1 2023-06-14 11:01:04.000000 spade_bokeh-0.2.0/spade_bokeh.egg-info/dependency_links.txt
+-rw-r--r--   0 jpalanca   (501) staff       (20)        1 2023-06-14 11:01:04.000000 spade_bokeh-0.2.0/spade_bokeh.egg-info/not-zip-safe
+-rw-r--r--   0 jpalanca   (501) staff       (20)       41 2023-06-14 11:01:04.000000 spade_bokeh-0.2.0/spade_bokeh.egg-info/requires.txt
+-rw-r--r--   0 jpalanca   (501) staff       (20)       12 2023-06-14 11:01:04.000000 spade_bokeh-0.2.0/spade_bokeh.egg-info/top_level.txt
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-06-14 11:01:04.918475 spade_bokeh-0.2.0/tests/
+-rw-r--r--   0 jpalanca   (501) staff       (20)        0 2023-06-14 11:00:42.000000 spade_bokeh-0.2.0/tests/__init__.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1047 2023-06-14 11:00:42.000000 spade_bokeh-0.2.0/tests/test_spade_bokeh.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `spade_bokeh-0.1.2/PKG-INFO` & `spade_bokeh-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,71 +1,77 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: spade_bokeh
-Version: 0.1.2
+Version: 0.2.0
 Summary: Bokeh server for SPADE agents that integrates with agents web service.
 Home-page: https://github.com/javipalanca/spade_bokeh
 Author: Javi Palanca
 Author-email: jpalanca@gmail.com
 License: MIT license
-Description: =========================
-        SPADE Bokeh Server Plugin
-        =========================
-        
-        
-        .. image:: https://img.shields.io/pypi/v/spade_bokeh.svg
-                :target: https://pypi.python.org/pypi/spade_bokeh
-        
-        .. image:: https://img.shields.io/travis/javipalanca/spade_bokeh.svg
-                :target: https://travis-ci.org/javipalanca/spade_bokeh
-        
-        .. image:: https://readthedocs.org/projects/spade-bokeh/badge/?version=latest
-                :target: https://spade-bokeh.readthedocs.io/en/latest/?badge=latest
-                :alt: Documentation Status
-        
-        
-        
-        
-        Bokeh server Plugin for SPADE agents that integrates with agents web service.
-        Allows to render dynamic bokeh plots inside the agent templates in a very easy way.
-        
-        
-        * Free software: MIT license
-        * Documentation: https://spade-bokeh.readthedocs.io.
-        
-        
-        Features
-        --------
-        
-        * TODO
-        
-        Credits
-        -------
-        
-        This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-        
-        .. _Cookiecutter: https://github.com/audreyr/cookiecutter
-        .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-        
-        
-        =======
-        History
-        =======
-        
-        0.1.2 (2018-09-17)
-        ------------------
-        
-        * Added requirements file.
-        * Fixed tox configuration for CI.
-        * Fixed readthedocs configuration.
-        
-        0.1.0 (2018-09-17)
-        ------------------
-        
-        * First release on PyPI.
-        
 Keywords: spade_bokeh
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+=========================
+SPADE Bokeh Server Plugin
+=========================
+
+
+.. image:: https://img.shields.io/pypi/v/spade_bokeh.svg
+        :target: https://pypi.python.org/pypi/spade_bokeh
+
+.. image:: https://readthedocs.org/projects/spade-bokeh/badge/?version=latest
+        :target: https://spade-bokeh.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+
+
+
+
+Bokeh server Plugin for SPADE agents that integrates with agents web service.
+Allows to render dynamic bokeh plots inside the agent templates in a very easy way.
+
+
+* Free software: MIT license
+* Documentation: https://spade-bokeh.readthedocs.io.
+
+
+Features
+--------
+
+* Plot interactive bokeh plots inside the agent templates
+
+Credits
+-------
+
+This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+
+
+=======
+History
+=======
+
+0.2.0 (2023-06-14)
+------------------
+
+* Upgraded to SPADE>=3.3 (older versions are deprecated).
+* Upgraded to Python>=3.8 (older versions are deprecated).
+
+0.1.2 (2018-09-17)
+------------------
+
+* Added requirements file.
+* Fixed tox configuration for CI.
+* Fixed readthedocs configuration.
+
+0.1.0 (2018-09-17)
+------------------
+
+* First release on PyPI.
```

### Comparing `spade_bokeh-0.1.2/spade_bokeh.egg-info/PKG-INFO` & `spade_bokeh-0.2.0/spade_bokeh.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,71 +1,77 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: spade-bokeh
-Version: 0.1.2
+Version: 0.2.0
 Summary: Bokeh server for SPADE agents that integrates with agents web service.
 Home-page: https://github.com/javipalanca/spade_bokeh
 Author: Javi Palanca
 Author-email: jpalanca@gmail.com
 License: MIT license
-Description: =========================
-        SPADE Bokeh Server Plugin
-        =========================
-        
-        
-        .. image:: https://img.shields.io/pypi/v/spade_bokeh.svg
-                :target: https://pypi.python.org/pypi/spade_bokeh
-        
-        .. image:: https://img.shields.io/travis/javipalanca/spade_bokeh.svg
-                :target: https://travis-ci.org/javipalanca/spade_bokeh
-        
-        .. image:: https://readthedocs.org/projects/spade-bokeh/badge/?version=latest
-                :target: https://spade-bokeh.readthedocs.io/en/latest/?badge=latest
-                :alt: Documentation Status
-        
-        
-        
-        
-        Bokeh server Plugin for SPADE agents that integrates with agents web service.
-        Allows to render dynamic bokeh plots inside the agent templates in a very easy way.
-        
-        
-        * Free software: MIT license
-        * Documentation: https://spade-bokeh.readthedocs.io.
-        
-        
-        Features
-        --------
-        
-        * TODO
-        
-        Credits
-        -------
-        
-        This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-        
-        .. _Cookiecutter: https://github.com/audreyr/cookiecutter
-        .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-        
-        
-        =======
-        History
-        =======
-        
-        0.1.2 (2018-09-17)
-        ------------------
-        
-        * Added requirements file.
-        * Fixed tox configuration for CI.
-        * Fixed readthedocs configuration.
-        
-        0.1.0 (2018-09-17)
-        ------------------
-        
-        * First release on PyPI.
-        
 Keywords: spade_bokeh
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+=========================
+SPADE Bokeh Server Plugin
+=========================
+
+
+.. image:: https://img.shields.io/pypi/v/spade_bokeh.svg
+        :target: https://pypi.python.org/pypi/spade_bokeh
+
+.. image:: https://readthedocs.org/projects/spade-bokeh/badge/?version=latest
+        :target: https://spade-bokeh.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+
+
+
+
+Bokeh server Plugin for SPADE agents that integrates with agents web service.
+Allows to render dynamic bokeh plots inside the agent templates in a very easy way.
+
+
+* Free software: MIT license
+* Documentation: https://spade-bokeh.readthedocs.io.
+
+
+Features
+--------
+
+* Plot interactive bokeh plots inside the agent templates
+
+Credits
+-------
+
+This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+
+
+=======
+History
+=======
+
+0.2.0 (2023-06-14)
+------------------
+
+* Upgraded to SPADE>=3.3 (older versions are deprecated).
+* Upgraded to Python>=3.8 (older versions are deprecated).
+
+0.1.2 (2018-09-17)
+------------------
+
+* Added requirements file.
+* Fixed tox configuration for CI.
+* Fixed readthedocs configuration.
+
+0.1.0 (2018-09-17)
+------------------
+
+* First release on PyPI.
```

### Comparing `spade_bokeh-0.1.2/spade_bokeh.egg-info/SOURCES.txt` & `spade_bokeh-0.2.0/spade_bokeh.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -35,8 +35,9 @@
 spade_bokeh/spade_bokeh.py
 spade_bokeh.egg-info/PKG-INFO
 spade_bokeh.egg-info/SOURCES.txt
 spade_bokeh.egg-info/dependency_links.txt
 spade_bokeh.egg-info/not-zip-safe
 spade_bokeh.egg-info/requires.txt
 spade_bokeh.egg-info/top_level.txt
+tests/__init__.py
 tests/test_spade_bokeh.py
```

### Comparing `spade_bokeh-0.1.2/LICENSE` & `spade_bokeh-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spade_bokeh-0.1.2/CONTRIBUTING.rst` & `spade_bokeh-0.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `spade_bokeh-0.1.2/tests/test_spade_bokeh.py` & `spade_bokeh-0.2.0/tests/test_spade_bokeh.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 """Tests for `spade_bokeh` package."""
 from collections import namedtuple
 
+import pytest
+
 from spade_bokeh import spade_bokeh
 
-agent = namedtuple("agent", "port")(port=1024)
+
+@pytest.fixture
+def agent():
+    return namedtuple("agent", "port")(port=1024)
 
 
-def test_server():
+def test_server(agent):
     server = spade_bokeh.BokekServer(agent)
 
     assert server.agent.port == 1024
     assert not server.hostname
     assert not server.port
     assert not server.server
     assert not server.is_running
 
 
-def test_add_plot():
+def test_add_plot(agent):
     server = spade_bokeh.BokekServer(agent)
 
     server.add_plot("/my_plot", lambda x: x)
 
     assert "/my_plot" in server.apps
 
 
@@ -33,10 +38,10 @@
     server.port = 1024
 
     server.add_plot("/my_plot", lambda x: x)
 
     script = server.get_plot_script("/my_plot")
 
     assert type(script) == str
-    assert script.startswith("\n<script ")
+    assert script.startswith("<script ")
     assert "bokeh-absolute-url=http://hostname:1024/my_plot" in script
     assert script.endswith("</script>")
```

### Comparing `spade_bokeh-0.1.2/docs/Makefile` & `spade_bokeh-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spade_bokeh-0.1.2/docs/conf.py` & `spade_bokeh-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `spade_bokeh-0.1.2/docs/usage.rst` & `spade_bokeh-0.2.0/docs/usage.rst`

 * *Files 4% similar despite different names*

```diff
@@ -10,63 +10,74 @@
 own figures with python code and dinamycally thanks to a server embedded with bokeh.
 
 This plugin provides a **mixin** to include a bokeh server in an agent and to register plots to be then rendered in
 your jinja2 templates of your agent's web interface.
 
 To use SPADE Bokeh Server in a project::
 
-    from spade import agent
-    import spade_bokeh
+    import getpass
 
+    import spade
     from bokeh.layouts import column
     from bokeh.models import ColumnDataSource, Slider
     from bokeh.plotting import figure
     from bokeh.sampledata.sea_surface_temperature import sea_surface_temperature
 
+    import spade_bokeh
+
+
+    class MyBokehAgent(spade_bokeh.BokehServerMixin, spade.agent.Agent):
 
-    class MyBokehAgent(spade_bokeh.BokehServerMixin, agent.Agent):
+        async def controller(self, request):
+            script = self.bokeh_server.get_plot_script("/my_plot")
+
+            return {"script": script}
 
-        # agent setup
-        def setup(self):
+        async def setup(self):
 
             self.web.add_get("/plot", self.controller, "plot.html")
 
             self.web.start(port=10000)
-            self.bokeh_server.start(hostname="localhost", port=5006)
+            self.bokeh_server.start()
 
             self.bokeh_server.add_plot("/my_plot", self.modify_doc)
 
-        # bokeh plot creation
         def modify_doc(self, doc):
-            """ here you create your plot, see the Bokeh documentation """
             df = sea_surface_temperature.copy()
             source = ColumnDataSource(data=df)
 
-            plot = figure(x_axis_type='datetime', y_range=(0, 25),
-                          y_axis_label='Temperature (Celsius)',
+            plot = figure(x_axis_type='datetime', y_range=(0, 25), y_axis_label='Temperature (Celsius)',
                           title="Sea Surface Temperature at 43.18, -70.43")
             plot.line('time', 'temperature', source=source)
 
             def callback(attr, old, new):
                 if new == 0:
                     data = df
                 else:
                     data = df.rolling('{0}D'.format(new)).mean()
-                source.data = ColumnDataSource(data=data).data
+                source.data = data
 
             slider = Slider(start=0, end=30, value=0, step=1, title="Smoothing by N Days")
             slider.on_change('value', callback)
 
             doc.add_root(column(slider, plot))
 
-        # web controller
-        async def controller(self, request):
-            script = self.bokeh_server.get_plot_script("/my_plot")
 
-            return {"script": script}
+    async def main(jid, passwd):
+        a = MyBokehAgent(jid, passwd)
+        await a.start()
+
+        await spade.wait_until_finished(a)
+
+    if __name__ == "__main__":
+
+        jid = input("Agent JID> ")
+        passwd = getpass.getpass()
+        spade.run(main(jid, passwd))
+
 
 
 
 In the example below there are 3 different blocks: the agent setup, the web controller and the bokeh plot creation.
 
 
 Agent setup
```

### Comparing `spade_bokeh-0.1.2/docs/make.bat` & `spade_bokeh-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `spade_bokeh-0.1.2/docs/_build/html/_static/ajax-loader.gif` & `spade_bokeh-0.2.0/docs/_build/html/_static/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `spade_bokeh-0.1.2/docs/_build/html/_static/comment.png` & `spade_bokeh-0.2.0/docs/_build/html/_static/comment.png`

 * *Files identical despite different names*

### Comparing `spade_bokeh-0.1.2/docs/_build/html/_static/comment-close.png` & `spade_bokeh-0.2.0/docs/_build/html/_static/comment-close.png`

 * *Files identical despite different names*

### Comparing `spade_bokeh-0.1.2/docs/_build/html/_static/comment-bright.png` & `spade_bokeh-0.2.0/docs/_build/html/_static/comment-bright.png`

 * *Files identical despite different names*

### Comparing `spade_bokeh-0.1.2/docs/installation.rst` & `spade_bokeh-0.2.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `spade_bokeh-0.1.2/setup.py` & `spade_bokeh-0.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,24 +28,26 @@
     author="Javi Palanca",
     author_email='jpalanca@gmail.com',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
-        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
     ],
     description="Bokeh server for SPADE agents that integrates with agents web service.",
     install_requires=requirements,
     license="MIT license",
     long_description=readme + '\n\n' + history,
     include_package_data=True,
     keywords='spade_bokeh',
     name='spade_bokeh',
     packages=find_packages(include=['spade_bokeh']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/javipalanca/spade_bokeh',
-    version='0.1.2',
+    version='0.2.0',
     zip_safe=False,
 )
```

### Comparing `spade_bokeh-0.1.2/spade_bokeh/spade_bokeh.py` & `spade_bokeh-0.2.0/spade_bokeh/spade_bokeh.py`

 * *Files identical despite different names*

### Comparing `spade_bokeh-0.1.2/README.rst` & `spade_bokeh-0.2.0/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 SPADE Bokeh Server Plugin
 =========================
 
 
 .. image:: https://img.shields.io/pypi/v/spade_bokeh.svg
         :target: https://pypi.python.org/pypi/spade_bokeh
 
-.. image:: https://img.shields.io/travis/javipalanca/spade_bokeh.svg
-        :target: https://travis-ci.org/javipalanca/spade_bokeh
-
 .. image:: https://readthedocs.org/projects/spade-bokeh/badge/?version=latest
         :target: https://spade-bokeh.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 
 
 
@@ -23,15 +20,15 @@
 * Free software: MIT license
 * Documentation: https://spade-bokeh.readthedocs.io.
 
 
 Features
 --------
 
-* TODO
+* Plot interactive bokeh plots inside the agent templates
 
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
```

