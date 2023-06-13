# Comparing `tmp/hveto-2.0.1.tar.gz` & `tmp/hveto-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hveto-2.0.1.tar", last modified: Wed Dec 16 20:25:17 2020, max compression
+gzip compressed data, was "hveto-2.1.0.tar", last modified: Tue Sep  6 21:34:21 2022, max compression
```

## Comparing `hveto-2.0.1.tar` & `hveto-2.1.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 alexurban   (501) staff       (20)        0 2020-12-16 20:25:17.339106 hveto-2.0.1/
--rw-r--r--   0 alexurban   (501) staff       (20)    35147 2019-03-23 19:54:17.000000 hveto-2.0.1/LICENSE
--rw-r--r--   0 alexurban   (501) staff       (20)       64 2019-03-23 19:54:17.000000 hveto-2.0.1/MANIFEST.in
--rw-r--r--   0 alexurban   (501) staff       (20)     4184 2020-12-16 20:25:17.339396 hveto-2.0.1/PKG-INFO
--rw-r--r--   0 alexurban   (501) staff       (20)     2361 2019-11-04 21:16:15.000000 hveto-2.0.1/README.rst
-drwxr-xr-x   0 alexurban   (501) staff       (20)        0 2020-12-16 20:25:17.341037 hveto-2.0.1/hveto/
--rw-r--r--   0 alexurban   (501) staff       (20)      971 2020-12-10 00:38:10.000000 hveto-2.0.1/hveto/__init__.py
--rw-r--r--   0 alexurban   (501) staff       (20)    35277 2020-12-16 20:20:25.000000 hveto-2.0.1/hveto/__main__.py
--rw-r--r--   0 alexurban   (501) staff       (20)      471 2020-12-16 20:25:17.341125 hveto-2.0.1/hveto/_version.py
-drwxr-xr-x   0 alexurban   (501) staff       (20)        0 2020-12-16 20:25:17.333708 hveto-2.0.1/hveto/cli/
--rw-r--r--   0 alexurban   (501) staff       (20)      896 2020-12-10 00:38:10.000000 hveto-2.0.1/hveto/cli/__init__.py
--rw-r--r--   0 alexurban   (501) staff       (20)    14377 2020-12-16 20:20:25.000000 hveto-2.0.1/hveto/cli/cache_events.py
-drwxr-xr-x   0 alexurban   (501) staff       (20)        0 2020-12-16 20:25:17.334663 hveto-2.0.1/hveto/cli/tests/
--rw-r--r--   0 alexurban   (501) staff       (20)      811 2020-12-16 20:20:25.000000 hveto-2.0.1/hveto/cli/tests/__init__.py
--rw-r--r--   0 alexurban   (501) staff       (20)     3063 2020-12-16 20:20:25.000000 hveto-2.0.1/hveto/cli/tests/test_trace.py
--rw-r--r--   0 alexurban   (501) staff       (20)     3976 2020-12-16 20:20:25.000000 hveto-2.0.1/hveto/cli/trace.py
--rw-r--r--   0 alexurban   (501) staff       (20)    11142 2020-12-10 00:38:10.000000 hveto-2.0.1/hveto/config.py
--rw-r--r--   0 alexurban   (501) staff       (20)     1698 2020-12-10 00:38:10.000000 hveto-2.0.1/hveto/const.py
--rw-r--r--   0 alexurban   (501) staff       (20)    10767 2020-12-10 00:38:10.000000 hveto-2.0.1/hveto/core.py
--rw-r--r--   0 alexurban   (501) staff       (20)    14564 2020-12-16 20:20:25.000000 hveto-2.0.1/hveto/html.py
--rw-r--r--   0 alexurban   (501) staff       (20)    18782 2020-12-10 00:38:10.000000 hveto-2.0.1/hveto/plot.py
--rw-r--r--   0 alexurban   (501) staff       (20)     2681 2020-12-10 00:38:10.000000 hveto-2.0.1/hveto/segments.py
-drwxr-xr-x   0 alexurban   (501) staff       (20)        0 2020-12-16 20:25:17.338403 hveto-2.0.1/hveto/tests/
--rw-r--r--   0 alexurban   (501) staff       (20)      749 2020-12-10 00:38:10.000000 hveto-2.0.1/hveto/tests/__init__.py
--rw-r--r--   0 alexurban   (501) staff       (20)     1266 2020-12-10 00:38:10.000000 hveto-2.0.1/hveto/tests/test_core.py
--rw-r--r--   0 alexurban   (501) staff       (20)     3861 2020-12-10 00:38:10.000000 hveto-2.0.1/hveto/tests/test_html.py
--rw-r--r--   0 alexurban   (501) staff       (20)     1731 2020-12-16 20:20:25.000000 hveto-2.0.1/hveto/tests/test_plot.py
--rw-r--r--   0 alexurban   (501) staff       (20)     2710 2020-12-16 20:20:25.000000 hveto-2.0.1/hveto/tests/test_segments.py
--rw-r--r--   0 alexurban   (501) staff       (20)     1896 2020-12-10 00:38:10.000000 hveto-2.0.1/hveto/tests/test_triggers.py
--rw-r--r--   0 alexurban   (501) staff       (20)     2149 2020-12-10 00:38:10.000000 hveto-2.0.1/hveto/tests/test_utils.py
--rw-r--r--   0 alexurban   (501) staff       (20)    10155 2020-12-16 20:20:25.000000 hveto-2.0.1/hveto/triggers.py
--rw-r--r--   0 alexurban   (501) staff       (20)     4477 2020-12-10 00:38:10.000000 hveto-2.0.1/hveto/utils.py
-drwxr-xr-x   0 alexurban   (501) staff       (20)        0 2020-12-16 20:25:17.332033 hveto-2.0.1/hveto.egg-info/
--rw-r--r--   0 alexurban   (501) staff       (20)     4184 2020-12-16 20:25:16.000000 hveto-2.0.1/hveto.egg-info/PKG-INFO
--rw-r--r--   0 alexurban   (501) staff       (20)      753 2020-12-16 20:25:16.000000 hveto-2.0.1/hveto.egg-info/SOURCES.txt
--rw-r--r--   0 alexurban   (501) staff       (20)        1 2020-12-16 20:25:16.000000 hveto-2.0.1/hveto.egg-info/dependency_links.txt
--rw-r--r--   0 alexurban   (501) staff       (20)      131 2020-12-16 20:25:16.000000 hveto-2.0.1/hveto.egg-info/entry_points.txt
--rw-r--r--   0 alexurban   (501) staff       (20)        1 2019-11-07 21:50:56.000000 hveto-2.0.1/hveto.egg-info/not-zip-safe
--rw-r--r--   0 alexurban   (501) staff       (20)      205 2020-12-16 20:25:16.000000 hveto-2.0.1/hveto.egg-info/requires.txt
--rw-r--r--   0 alexurban   (501) staff       (20)        6 2020-12-16 20:25:16.000000 hveto-2.0.1/hveto.egg-info/top_level.txt
--rw-r--r--   0 alexurban   (501) staff       (20)     2107 2020-12-16 20:25:17.340627 hveto-2.0.1/setup.cfg
--rw-r--r--   0 alexurban   (501) staff       (20)     1184 2020-12-10 00:38:10.000000 hveto-2.0.1/setup.py
--rw-r--r--   0 alexurban   (501) staff       (20)    65747 2019-03-23 19:54:17.000000 hveto-2.0.1/versioneer.py
+drwxr-xr-x   0 areeda     (501) staff       (20)        0 2022-09-06 21:34:21.566899 hveto-2.1.0/
+-rw-r--r--   0 areeda     (501) staff       (20)    35147 2022-09-06 21:22:40.000000 hveto-2.1.0/LICENSE
+-rw-r--r--   0 areeda     (501) staff       (20)       64 2022-09-06 21:22:40.000000 hveto-2.1.0/MANIFEST.in
+-rw-r--r--   0 areeda     (501) staff       (20)     3643 2022-09-06 21:34:21.567063 hveto-2.1.0/PKG-INFO
+-rw-r--r--   0 areeda     (501) staff       (20)     2361 2022-09-06 21:22:40.000000 hveto-2.1.0/README.rst
+drwxr-xr-x   0 areeda     (501) staff       (20)        0 2022-09-06 21:34:21.568639 hveto-2.1.0/hveto/
+-rw-r--r--   0 areeda     (501) staff       (20)      971 2022-09-06 21:22:40.000000 hveto-2.1.0/hveto/__init__.py
+-rw-r--r--   0 areeda     (501) staff       (20)    35728 2022-09-06 21:22:40.000000 hveto-2.1.0/hveto/__main__.py
+-rw-r--r--   0 areeda     (501) staff       (20)      471 2022-09-06 21:34:21.568736 hveto-2.1.0/hveto/_version.py
+drwxr-xr-x   0 areeda     (501) staff       (20)        0 2022-09-06 21:34:21.563434 hveto-2.1.0/hveto/cli/
+-rw-r--r--   0 areeda     (501) staff       (20)      896 2022-09-06 21:22:40.000000 hveto-2.1.0/hveto/cli/__init__.py
+-rw-r--r--   0 areeda     (501) staff       (20)    14377 2022-09-06 21:22:40.000000 hveto-2.1.0/hveto/cli/cache_events.py
+drwxr-xr-x   0 areeda     (501) staff       (20)        0 2022-09-06 21:34:21.564118 hveto-2.1.0/hveto/cli/tests/
+-rw-r--r--   0 areeda     (501) staff       (20)      811 2022-09-06 21:22:40.000000 hveto-2.1.0/hveto/cli/tests/__init__.py
+-rw-r--r--   0 areeda     (501) staff       (20)     3063 2022-09-06 21:22:40.000000 hveto-2.1.0/hveto/cli/tests/test_trace.py
+-rw-r--r--   0 areeda     (501) staff       (20)     3976 2022-09-06 21:22:40.000000 hveto-2.1.0/hveto/cli/trace.py
+-rw-r--r--   0 areeda     (501) staff       (20)    11142 2022-09-06 21:22:40.000000 hveto-2.1.0/hveto/config.py
+-rw-r--r--   0 areeda     (501) staff       (20)     1698 2022-09-06 21:22:40.000000 hveto-2.1.0/hveto/const.py
+-rw-r--r--   0 areeda     (501) staff       (20)    10767 2022-09-06 21:22:40.000000 hveto-2.1.0/hveto/core.py
+-rw-r--r--   0 areeda     (501) staff       (20)    14564 2022-09-06 21:22:40.000000 hveto-2.1.0/hveto/html.py
+-rw-r--r--   0 areeda     (501) staff       (20)    18808 2022-09-06 21:22:40.000000 hveto-2.1.0/hveto/plot.py
+-rw-r--r--   0 areeda     (501) staff       (20)     2681 2022-09-06 21:22:40.000000 hveto-2.1.0/hveto/segments.py
+drwxr-xr-x   0 areeda     (501) staff       (20)        0 2022-09-06 21:34:21.566601 hveto-2.1.0/hveto/tests/
+-rw-r--r--   0 areeda     (501) staff       (20)      749 2022-09-06 21:22:40.000000 hveto-2.1.0/hveto/tests/__init__.py
+-rw-r--r--   0 areeda     (501) staff       (20)     1266 2022-09-06 21:22:40.000000 hveto-2.1.0/hveto/tests/test_core.py
+-rw-r--r--   0 areeda     (501) staff       (20)     3861 2022-09-06 21:22:40.000000 hveto-2.1.0/hveto/tests/test_html.py
+-rw-r--r--   0 areeda     (501) staff       (20)     1731 2022-09-06 21:22:40.000000 hveto-2.1.0/hveto/tests/test_plot.py
+-rw-r--r--   0 areeda     (501) staff       (20)     2710 2022-09-06 21:22:40.000000 hveto-2.1.0/hveto/tests/test_segments.py
+-rw-r--r--   0 areeda     (501) staff       (20)     1896 2022-09-06 21:22:40.000000 hveto-2.1.0/hveto/tests/test_triggers.py
+-rw-r--r--   0 areeda     (501) staff       (20)     2149 2022-09-06 21:22:40.000000 hveto-2.1.0/hveto/tests/test_utils.py
+-rw-r--r--   0 areeda     (501) staff       (20)    10509 2022-09-06 21:22:40.000000 hveto-2.1.0/hveto/triggers.py
+-rw-r--r--   0 areeda     (501) staff       (20)     4477 2022-09-06 21:22:40.000000 hveto-2.1.0/hveto/utils.py
+drwxr-xr-x   0 areeda     (501) staff       (20)        0 2022-09-06 21:34:21.562362 hveto-2.1.0/hveto.egg-info/
+-rw-r--r--   0 areeda     (501) staff       (20)     3643 2022-09-06 21:34:21.000000 hveto-2.1.0/hveto.egg-info/PKG-INFO
+-rw-r--r--   0 areeda     (501) staff       (20)      753 2022-09-06 21:34:21.000000 hveto-2.1.0/hveto.egg-info/SOURCES.txt
+-rw-r--r--   0 areeda     (501) staff       (20)        1 2022-09-06 21:34:21.000000 hveto-2.1.0/hveto.egg-info/dependency_links.txt
+-rw-r--r--   0 areeda     (501) staff       (20)      130 2022-09-06 21:34:21.000000 hveto-2.1.0/hveto.egg-info/entry_points.txt
+-rw-r--r--   0 areeda     (501) staff       (20)        1 2022-09-06 21:34:21.000000 hveto-2.1.0/hveto.egg-info/not-zip-safe
+-rw-r--r--   0 areeda     (501) staff       (20)      205 2022-09-06 21:34:21.000000 hveto-2.1.0/hveto.egg-info/requires.txt
+-rw-r--r--   0 areeda     (501) staff       (20)        6 2022-09-06 21:34:21.000000 hveto-2.1.0/hveto.egg-info/top_level.txt
+-rw-r--r--   0 areeda     (501) staff       (20)     2107 2022-09-06 21:34:21.568265 hveto-2.1.0/setup.cfg
+-rw-r--r--   0 areeda     (501) staff       (20)     1184 2022-09-06 21:22:40.000000 hveto-2.1.0/setup.py
+-rw-r--r--   0 areeda     (501) staff       (20)    65747 2022-09-06 21:22:40.000000 hveto-2.1.0/versioneer.py
```

### Comparing `hveto-2.0.1/LICENSE` & `hveto-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hveto-2.0.1/PKG-INFO` & `hveto-2.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,85 +1,15 @@
 Metadata-Version: 2.1
 Name: hveto
-Version: 2.0.1
+Version: 2.1.0
 Summary: A python implementation of the HierarchicalVeto (hveto) algorithm.
 Home-page: https://github.com/gwdetchar/hveto/
 Author: Joshua Smith
 Author-email: joshua.smith@ligo.org
 License: GPL-3.0-or-later
-Description: =================
-        Hierarchical Veto
-        =================
-        
-        Hveto is a python implementation of the HierarchicalVeto algorithm. It is
-        a package designed for gravitational-wave detector characterisation and
-        data quality.
-        
-        The Hveto algorithm is fully described in `Smith et al. 2011`_
-        (Classical and Quantum Gravity).
-        
-        |PyPI version| |Conda version|
-        
-        |DOI| |License| |Supported Python versions|
-        
-        |Build Status| |Coverage Status| |Documentation Status|
-        
-        https://hveto.readthedocs.io
-        
-        ------------
-        Installation
-        ------------
-        
-        Hveto is best installed with `conda`_:
-        
-        .. code:: bash
-        
-           conda install -c conda-forge hveto
-        
-        but can also be installed with `pip`_:
-        
-        .. code:: bash
-        
-           python -m pip install hveto
-        
-        ------------
-        Contributing
-        ------------
-        
-        All code should follow the Python Style Guide outlined in `PEP 0008`_;
-        users can use the `flake8`_ package to check their code for style issues
-        before submitting.
-        
-        See `the contributions guide`_ for the recommended procedure for
-        proposing additions/changes.
-        
-        .. _PEP 0008: https://www.python.org/dev/peps/pep-0008/
-        .. _flake8: http://flake8.pycqa.org
-        .. _the contributions guide: https://github.com/gwdetchar/hveto/blob/master/CONTRIBUTING.md
-        .. _conda: https://conda.io
-        .. _pip: https://pip.pypa.io/en/stable/
-        .. _Smith et al. 2011: //dx.doi.org/10.1088/0264-9381/28/23/235005
-        
-        .. |PyPI version| image:: https://badge.fury.io/py/hveto.svg
-           :target: http://badge.fury.io/py/hveto
-        .. |Conda version| image:: https://img.shields.io/conda/vn/conda-forge/hveto.svg
-           :target: https://anaconda.org/conda-forge/hveto/
-        .. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/2584615.svg
-           :target: https://doi.org/10.5281/zenodo.2584615
-        .. |License| image:: https://img.shields.io/pypi/l/hveto.svg
-           :target: https://choosealicense.com/licenses/gpl-3.0/
-        .. |Supported Python versions| image:: https://img.shields.io/pypi/pyversions/hveto.svg
-           :target: https://pypi.org/project/hveto/
-        .. |Build Status| image:: https://travis-ci.org/gwdetchar/hveto.svg?branch=master
-           :target: https://travis-ci.org/gwdetchar/hveto
-        .. |Coverage Status| image:: https://codecov.io/gh/gwdetchar/hveto/branch/master/graph/badge.svg
-           :target: https://codecov.io/gh/gwdetchar/hveto
-        .. |Documentation Status| image:: https://readthedocs.org/projects/hveto/badge/?version=stable
-           :target: https://hveto.readthedocs.io/en/stable/?badge=stable
-        
 Keywords: physics,astronomy,gravitational-waves,ligo
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -94,7 +24,80 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.6
 Provides-Extra: doc
+License-File: LICENSE
+
+=================
+Hierarchical Veto
+=================
+
+Hveto is a python implementation of the HierarchicalVeto algorithm. It is
+a package designed for gravitational-wave detector characterisation and
+data quality.
+
+The Hveto algorithm is fully described in `Smith et al. 2011`_
+(Classical and Quantum Gravity).
+
+|PyPI version| |Conda version|
+
+|DOI| |License| |Supported Python versions|
+
+|Build Status| |Coverage Status| |Documentation Status|
+
+https://hveto.readthedocs.io
+
+------------
+Installation
+------------
+
+Hveto is best installed with `conda`_:
+
+.. code:: bash
+
+   conda install -c conda-forge hveto
+
+but can also be installed with `pip`_:
+
+.. code:: bash
+
+   python -m pip install hveto
+
+------------
+Contributing
+------------
+
+All code should follow the Python Style Guide outlined in `PEP 0008`_;
+users can use the `flake8`_ package to check their code for style issues
+before submitting.
+
+See `the contributions guide`_ for the recommended procedure for
+proposing additions/changes.
+
+.. _PEP 0008: https://www.python.org/dev/peps/pep-0008/
+.. _flake8: http://flake8.pycqa.org
+.. _the contributions guide: https://github.com/gwdetchar/hveto/blob/master/CONTRIBUTING.md
+.. _conda: https://conda.io
+.. _pip: https://pip.pypa.io/en/stable/
+.. _Smith et al. 2011: //dx.doi.org/10.1088/0264-9381/28/23/235005
+
+.. |PyPI version| image:: https://badge.fury.io/py/hveto.svg
+   :target: http://badge.fury.io/py/hveto
+.. |Conda version| image:: https://img.shields.io/conda/vn/conda-forge/hveto.svg
+   :target: https://anaconda.org/conda-forge/hveto/
+.. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/2584615.svg
+   :target: https://doi.org/10.5281/zenodo.2584615
+.. |License| image:: https://img.shields.io/pypi/l/hveto.svg
+   :target: https://choosealicense.com/licenses/gpl-3.0/
+.. |Supported Python versions| image:: https://img.shields.io/pypi/pyversions/hveto.svg
+   :target: https://pypi.org/project/hveto/
+.. |Build Status| image:: https://travis-ci.org/gwdetchar/hveto.svg?branch=master
+   :target: https://travis-ci.org/gwdetchar/hveto
+.. |Coverage Status| image:: https://codecov.io/gh/gwdetchar/hveto/branch/master/graph/badge.svg
+   :target: https://codecov.io/gh/gwdetchar/hveto
+.. |Documentation Status| image:: https://readthedocs.org/projects/hveto/badge/?version=stable
+   :target: https://hveto.readthedocs.io/en/stable/?badge=stable
+
+
```

### Comparing `hveto-2.0.1/README.rst` & `hveto-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `hveto-2.0.1/hveto/__init__.py` & `hveto-2.1.0/hveto/__init__.py`

 * *Files identical despite different names*

### Comparing `hveto-2.0.1/hveto/__main__.py` & `hveto-2.1.0/hveto/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,15 @@
                             % (tag, channel))
         elif len(trigs):  # no triggers
             LOGGER.debug("    %s Read %d events for %s"
                          % (tag, len(trigs), channel))
         else:  # everything is fine
             LOGGER.warning("    %s No events found for %s"
                            % (tag, channel))
+            out = None
     return out
 
 
 def _veto(channels):
     """Utility to apply vetoes with multiprocessing
     """
     chandict = dict((c, auxiliary[c]) for c in channels)
@@ -191,14 +192,24 @@
     pout = parser.add_argument_group('Output options')
     pout.add_argument(
         '-o',
         '--output-directory',
         default=os.curdir,
         help='path of output directory, default: %(default)s',
     )
+    parser.add_argument(
+        '-e',
+        '--extra-times',
+        action='append',
+        default=[],
+        type=float,
+        help=('extra times to add to the list of primary triggers '
+              'to include specific times that may not meet the thresholds '
+              'used to find triggers'),
+    )
 
     # return the parser
     return parser
 
 
 # -- main code block ----------------------------------------------------------
 
@@ -407,14 +418,15 @@
     if pcache is not None:  # auto-detect the file format
         LOGGER.debug('Unsetting the primary trigger file format')
         preadkw['format'] = None
         preadkw['path'] = 'triggers'
     ptrigfindkw = cp.getparams('primary', 'trigfind-')
     primary = get_triggers(pchannel, petg, analysis.active, snr=psnr,
                            frange=pfreq, cache=pcache, nproc=args.nproc,
+                           extra_times=args.extra_times,
                            trigfind_kwargs=ptrigfindkw, **preadkw)
     fcol, scol = primary.dtype.names[1:3]
 
     if len(primary):
         LOGGER.info("Read %d events for %s" % (len(primary), pchannel))
     else:
         message = "No events found for %r in %d seconds of livetime" % (
@@ -895,14 +907,15 @@
         if len(newtimes) > 0:
             LOGGER.info('Creating workflow for omega scans')
             flags = batch.get_command_line_flags(
                 ifo=ifo,
                 ignore_state_flags=True)
             condorcmds = batch.get_condor_arguments(
                 timeout=4,
+                extra_commands=["request_disk=1G"],
                 gps=start)
             batch.generate_dag(
                 newtimes,
                 flags=flags,
                 submit=True,
                 outdir=omegadir,
                 condor_commands=condorcmds)
```

### Comparing `hveto-2.0.1/hveto/cli/__init__.py` & `hveto-2.1.0/hveto/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `hveto-2.0.1/hveto/cli/cache_events.py` & `hveto-2.1.0/hveto/cli/cache_events.py`

 * *Files identical despite different names*

### Comparing `hveto-2.0.1/hveto/cli/tests/__init__.py` & `hveto-2.1.0/hveto/cli/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `hveto-2.0.1/hveto/cli/tests/test_trace.py` & `hveto-2.1.0/hveto/cli/tests/test_trace.py`

 * *Files identical despite different names*

### Comparing `hveto-2.0.1/hveto/cli/trace.py` & `hveto-2.1.0/hveto/cli/trace.py`

 * *Files identical despite different names*

### Comparing `hveto-2.0.1/hveto/config.py` & `hveto-2.1.0/hveto/config.py`

 * *Files identical despite different names*

### Comparing `hveto-2.0.1/hveto/const.py` & `hveto-2.1.0/hveto/const.py`

 * *Files identical despite different names*

### Comparing `hveto-2.0.1/hveto/core.py` & `hveto-2.1.0/hveto/core.py`

 * *Files identical despite different names*

### Comparing `hveto-2.0.1/hveto/html.py` & `hveto-2.1.0/hveto/html.py`

 * *Files identical despite different names*

### Comparing `hveto-2.0.1/hveto/plot.py` & `hveto-2.1.0/hveto/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,18 +258,19 @@
     ax = plot.gca()
     # add data
     if color is None:
         ax.scatter(a[x], a[ya], color='black', marker='o', label=label1, s=40)
     else:
         colorargs = {'edgecolor': 'none'}
         if clim:
-            colorargs['vmin'] = clim[0]
-            colorargs['vmax'] = clim[1]
             if clog:
                 colorargs['norm'] = LogNorm(vmin=clim[0], vmax=clim[1])
+            else:
+                colorargs['vmin'] = clim[0]
+                colorargs['vmax'] = clim[1]
         a = a.copy()
         a.sort(color)
         m = ax.scatter(a[x], a[ya], c=a[color], label=label1, **colorargs)
         # add colorbar
         ax.colorbar(mappable=m, cmap=cmap, label=clabel)
     if isinstance(b, (list, tuple)) and len(b) == 2:
         # aux channel used/coinc (probably)
```

### Comparing `hveto-2.0.1/hveto/segments.py` & `hveto-2.1.0/hveto/segments.py`

 * *Files identical despite different names*

### Comparing `hveto-2.0.1/hveto/tests/__init__.py` & `hveto-2.1.0/hveto/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `hveto-2.0.1/hveto/tests/test_core.py` & `hveto-2.1.0/hveto/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `hveto-2.0.1/hveto/tests/test_html.py` & `hveto-2.1.0/hveto/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `hveto-2.0.1/hveto/tests/test_plot.py` & `hveto-2.1.0/hveto/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `hveto-2.0.1/hveto/tests/test_segments.py` & `hveto-2.1.0/hveto/tests/test_segments.py`

 * *Files identical despite different names*

### Comparing `hveto-2.0.1/hveto/tests/test_triggers.py` & `hveto-2.1.0/hveto/tests/test_triggers.py`

 * *Files identical despite different names*

### Comparing `hveto-2.0.1/hveto/tests/test_utils.py` & `hveto-2.1.0/hveto/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `hveto-2.0.1/hveto/triggers.py` & `hveto-2.1.0/hveto/triggers.py`

 * *Files 6% similar despite different names*

```diff
@@ -249,15 +249,16 @@
     if etg == "pycbc_live":
         read_kwargs.setdefault("ifo", channel.split(":", 1)[0])
 
     return trigfind_kwargs, read_kwargs
 
 
 def get_triggers(channel, etg, segments, cache=None, snr=None, frange=None,
-                 raw=False, trigfind_kwargs={}, **read_kwargs):
+                 raw=False, extra_times=None, trigfind_kwargs={}, 
+                 **read_kwargs):
     """Get triggers for the given channel
     """
     etg = _sanitize_name(etg)
     # format arguments
     try:
         readfmt = read_kwargs.pop("format", DEFAULT_FORMAT[etg])
     except KeyError:
@@ -307,14 +308,24 @@
     if snr is not None:
         keep &= table[scolumn] >= snr
     if frange is not None:
         keep &= table[fcolumn] >= frange[0]
         keep &= table[fcolumn] < frange[1]
     table = table[keep]
 
+    if extra_times:
+        f_low = min(table[fcolumn])
+        s_low = min(table[scolumn])
+        for time in extra_times:
+            extra_row = numpy.zeros(len(table.colnames))
+            extra_row[0] = time
+            extra_row[1] = f_low
+            extra_row[2] = s_low
+            table.add_row(extra_row)
+
     # return basic table if 'raw'
     if raw:
         return table
 
     # rename time column so that all tables match in at least that
     if tcolumn != "time":
         table.rename_column(tcolumn, 'time')
```

### Comparing `hveto-2.0.1/hveto/utils.py` & `hveto-2.1.0/hveto/utils.py`

 * *Files identical despite different names*

### Comparing `hveto-2.0.1/hveto.egg-info/PKG-INFO` & `hveto-2.1.0/hveto.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,85 +1,15 @@
 Metadata-Version: 2.1
 Name: hveto
-Version: 2.0.1
+Version: 2.1.0
 Summary: A python implementation of the HierarchicalVeto (hveto) algorithm.
 Home-page: https://github.com/gwdetchar/hveto/
 Author: Joshua Smith
 Author-email: joshua.smith@ligo.org
 License: GPL-3.0-or-later
-Description: =================
-        Hierarchical Veto
-        =================
-        
-        Hveto is a python implementation of the HierarchicalVeto algorithm. It is
-        a package designed for gravitational-wave detector characterisation and
-        data quality.
-        
-        The Hveto algorithm is fully described in `Smith et al. 2011`_
-        (Classical and Quantum Gravity).
-        
-        |PyPI version| |Conda version|
-        
-        |DOI| |License| |Supported Python versions|
-        
-        |Build Status| |Coverage Status| |Documentation Status|
-        
-        https://hveto.readthedocs.io
-        
-        ------------
-        Installation
-        ------------
-        
-        Hveto is best installed with `conda`_:
-        
-        .. code:: bash
-        
-           conda install -c conda-forge hveto
-        
-        but can also be installed with `pip`_:
-        
-        .. code:: bash
-        
-           python -m pip install hveto
-        
-        ------------
-        Contributing
-        ------------
-        
-        All code should follow the Python Style Guide outlined in `PEP 0008`_;
-        users can use the `flake8`_ package to check their code for style issues
-        before submitting.
-        
-        See `the contributions guide`_ for the recommended procedure for
-        proposing additions/changes.
-        
-        .. _PEP 0008: https://www.python.org/dev/peps/pep-0008/
-        .. _flake8: http://flake8.pycqa.org
-        .. _the contributions guide: https://github.com/gwdetchar/hveto/blob/master/CONTRIBUTING.md
-        .. _conda: https://conda.io
-        .. _pip: https://pip.pypa.io/en/stable/
-        .. _Smith et al. 2011: //dx.doi.org/10.1088/0264-9381/28/23/235005
-        
-        .. |PyPI version| image:: https://badge.fury.io/py/hveto.svg
-           :target: http://badge.fury.io/py/hveto
-        .. |Conda version| image:: https://img.shields.io/conda/vn/conda-forge/hveto.svg
-           :target: https://anaconda.org/conda-forge/hveto/
-        .. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/2584615.svg
-           :target: https://doi.org/10.5281/zenodo.2584615
-        .. |License| image:: https://img.shields.io/pypi/l/hveto.svg
-           :target: https://choosealicense.com/licenses/gpl-3.0/
-        .. |Supported Python versions| image:: https://img.shields.io/pypi/pyversions/hveto.svg
-           :target: https://pypi.org/project/hveto/
-        .. |Build Status| image:: https://travis-ci.org/gwdetchar/hveto.svg?branch=master
-           :target: https://travis-ci.org/gwdetchar/hveto
-        .. |Coverage Status| image:: https://codecov.io/gh/gwdetchar/hveto/branch/master/graph/badge.svg
-           :target: https://codecov.io/gh/gwdetchar/hveto
-        .. |Documentation Status| image:: https://readthedocs.org/projects/hveto/badge/?version=stable
-           :target: https://hveto.readthedocs.io/en/stable/?badge=stable
-        
 Keywords: physics,astronomy,gravitational-waves,ligo
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -94,7 +24,80 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.6
 Provides-Extra: doc
+License-File: LICENSE
+
+=================
+Hierarchical Veto
+=================
+
+Hveto is a python implementation of the HierarchicalVeto algorithm. It is
+a package designed for gravitational-wave detector characterisation and
+data quality.
+
+The Hveto algorithm is fully described in `Smith et al. 2011`_
+(Classical and Quantum Gravity).
+
+|PyPI version| |Conda version|
+
+|DOI| |License| |Supported Python versions|
+
+|Build Status| |Coverage Status| |Documentation Status|
+
+https://hveto.readthedocs.io
+
+------------
+Installation
+------------
+
+Hveto is best installed with `conda`_:
+
+.. code:: bash
+
+   conda install -c conda-forge hveto
+
+but can also be installed with `pip`_:
+
+.. code:: bash
+
+   python -m pip install hveto
+
+------------
+Contributing
+------------
+
+All code should follow the Python Style Guide outlined in `PEP 0008`_;
+users can use the `flake8`_ package to check their code for style issues
+before submitting.
+
+See `the contributions guide`_ for the recommended procedure for
+proposing additions/changes.
+
+.. _PEP 0008: https://www.python.org/dev/peps/pep-0008/
+.. _flake8: http://flake8.pycqa.org
+.. _the contributions guide: https://github.com/gwdetchar/hveto/blob/master/CONTRIBUTING.md
+.. _conda: https://conda.io
+.. _pip: https://pip.pypa.io/en/stable/
+.. _Smith et al. 2011: //dx.doi.org/10.1088/0264-9381/28/23/235005
+
+.. |PyPI version| image:: https://badge.fury.io/py/hveto.svg
+   :target: http://badge.fury.io/py/hveto
+.. |Conda version| image:: https://img.shields.io/conda/vn/conda-forge/hveto.svg
+   :target: https://anaconda.org/conda-forge/hveto/
+.. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/2584615.svg
+   :target: https://doi.org/10.5281/zenodo.2584615
+.. |License| image:: https://img.shields.io/pypi/l/hveto.svg
+   :target: https://choosealicense.com/licenses/gpl-3.0/
+.. |Supported Python versions| image:: https://img.shields.io/pypi/pyversions/hveto.svg
+   :target: https://pypi.org/project/hveto/
+.. |Build Status| image:: https://travis-ci.org/gwdetchar/hveto.svg?branch=master
+   :target: https://travis-ci.org/gwdetchar/hveto
+.. |Coverage Status| image:: https://codecov.io/gh/gwdetchar/hveto/branch/master/graph/badge.svg
+   :target: https://codecov.io/gh/gwdetchar/hveto
+.. |Documentation Status| image:: https://readthedocs.org/projects/hveto/badge/?version=stable
+   :target: https://hveto.readthedocs.io/en/stable/?badge=stable
+
+
```

### Comparing `hveto-2.0.1/hveto.egg-info/SOURCES.txt` & `hveto-2.1.0/hveto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hveto-2.0.1/setup.cfg` & `hveto-2.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [versioneer]
-vcs = git
+VCS = git
 style = pep440
 versionfile_source = hveto/_version.py
 versionfile_build = hveto/_version.py
 tag_prefix = 
 parentdir_prefix = 
 
 [bdist_wheel]
```

### Comparing `hveto-2.0.1/setup.py` & `hveto-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `hveto-2.0.1/versioneer.py` & `hveto-2.1.0/versioneer.py`

 * *Files identical despite different names*

