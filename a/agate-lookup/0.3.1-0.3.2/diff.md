# Comparing `tmp/agate-lookup-0.3.1.tar.gz` & `tmp/agate-lookup-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/agate-lookup-0.3.1.tar", last modified: Mon Dec 19 22:11:30 2016, max compression
+gzip compressed data, was "agate-lookup-0.3.2.tar", last modified: Tue Jun 13 23:08:50 2023, max compression
```

## Comparing `agate-lookup-0.3.1.tar` & `agate-lookup-0.3.2.tar`

### file list

```diff
@@ -1,15 +1,33 @@
-drwxr-xr-x   0 cgroskopf (70339629) 518432175        0 2016-12-19 22:11:30.000000 agate-lookup-0.3.1/
-drwxr-xr-x   0 cgroskopf (70339629) 518432175        0 2016-12-19 22:11:30.000000 agate-lookup-0.3.1/agate_lookup.egg-info/
--rw-r--r--   0 cgroskopf (70339629) 518432175        1 2016-12-19 22:11:30.000000 agate-lookup-0.3.1/agate_lookup.egg-info/dependency_links.txt
--rw-r--r--   0 cgroskopf (70339629) 518432175     2501 2016-12-19 22:11:30.000000 agate-lookup-0.3.1/agate_lookup.egg-info/PKG-INFO
--rw-r--r--   0 cgroskopf (70339629) 518432175       42 2016-12-19 22:11:30.000000 agate-lookup-0.3.1/agate_lookup.egg-info/requires.txt
--rw-r--r--   0 cgroskopf (70339629) 518432175      275 2016-12-19 22:11:30.000000 agate-lookup-0.3.1/agate_lookup.egg-info/SOURCES.txt
--rw-r--r--   0 cgroskopf (70339629) 518432175       12 2016-12-19 22:11:30.000000 agate-lookup-0.3.1/agate_lookup.egg-info/top_level.txt
-drwxr-xr-x   0 cgroskopf (70339629) 518432175        0 2016-12-19 22:11:30.000000 agate-lookup-0.3.1/agatelookup/
--rw-r--r--   0 cgroskopf (70339629) 518432175       86 2016-12-19 21:52:54.000000 agate-lookup-0.3.1/agatelookup/__init__.py
--rw-r--r--   0 cgroskopf (70339629) 518432175     4777 2016-12-19 22:03:17.000000 agate-lookup-0.3.1/agatelookup/source.py
--rw-r--r--   0 cgroskopf (70339629) 518432175     2291 2016-12-19 21:56:05.000000 agate-lookup-0.3.1/agatelookup/table.py
--rw-r--r--   0 cgroskopf (70339629) 518432175     2501 2016-12-19 22:11:30.000000 agate-lookup-0.3.1/PKG-INFO
--rw-r--r--   0 cgroskopf (70339629) 518432175     1098 2016-03-09 13:55:21.000000 agate-lookup-0.3.1/README.rst
--rw-r--r--   0 cgroskopf (70339629) 518432175       88 2016-12-19 22:11:30.000000 agate-lookup-0.3.1/setup.cfg
--rw-r--r--   0 cgroskopf (70339629) 518432175     1451 2016-12-19 22:08:35.000000 agate-lookup-0.3.1/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-13 23:08:50.540390 agate-lookup-0.3.2/
+-rw-r--r--   0 james      (501) staff       (20)      122 2023-06-13 22:28:57.000000 agate-lookup-0.3.2/AUTHORS.rst
+-rw-r--r--   0 james      (501) staff       (20)      953 2023-06-13 23:07:15.000000 agate-lookup-0.3.2/CHANGELOG.rst
+-rw-r--r--   0 james      (501) staff       (20)     1098 2023-06-13 22:28:57.000000 agate-lookup-0.3.2/COPYING
+-rw-r--r--   0 james      (501) staff       (20)      282 2023-06-13 22:39:58.000000 agate-lookup-0.3.2/MANIFEST.in
+-rw-r--r--   0 james      (501) staff       (20)     2449 2023-06-13 23:08:50.540440 agate-lookup-0.3.2/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     1121 2023-06-13 22:52:09.000000 agate-lookup-0.3.2/README.rst
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-13 23:08:50.537454 agate-lookup-0.3.2/agate_lookup.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     2449 2023-06-13 23:08:50.000000 agate-lookup-0.3.2/agate_lookup.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      507 2023-06-13 23:08:50.000000 agate-lookup-0.3.2/agate_lookup.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-06-13 23:08:50.000000 agate-lookup-0.3.2/agate_lookup.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)      114 2023-06-13 23:08:50.000000 agate-lookup-0.3.2/agate_lookup.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       12 2023-06-13 23:08:50.000000 agate-lookup-0.3.2/agate_lookup.egg-info/top_level.txt
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-13 23:08:50.538054 agate-lookup-0.3.2/agatelookup/
+-rw-r--r--   0 james      (501) staff       (20)       86 2023-06-13 22:43:29.000000 agate-lookup-0.3.2/agatelookup/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     4758 2023-06-13 23:06:07.000000 agate-lookup-0.3.2/agatelookup/source.py
+-rw-r--r--   0 james      (501) staff       (20)     2294 2023-06-13 22:45:22.000000 agate-lookup-0.3.2/agatelookup/table.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-13 23:08:50.538975 agate-lookup-0.3.2/docs/
+-rw-r--r--   0 james      (501) staff       (20)     4610 2023-06-13 22:28:57.000000 agate-lookup-0.3.2/docs/Makefile
+-rw-r--r--   0 james      (501) staff       (20)     1265 2023-06-13 22:44:11.000000 agate-lookup-0.3.2/docs/conf.py
+-rw-r--r--   0 james      (501) staff       (20)     5503 2023-06-13 22:52:47.000000 agate-lookup-0.3.2/docs/index.rst
+-rw-r--r--   0 james      (501) staff       (20)       29 2023-06-13 22:51:22.000000 agate-lookup-0.3.2/docs/requirements.txt
+-rwxr-xr-x   0 james      (501) staff       (20)      866 2023-06-13 22:43:29.000000 agate-lookup-0.3.2/example.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-13 23:08:50.535162 agate-lookup-0.3.2/examples/
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-13 23:08:50.539567 agate-lookup-0.3.2/examples/usps/
+-rw-r--r--   0 james      (501) staff       (20)      780 2023-06-13 22:28:57.000000 agate-lookup-0.3.2/examples/usps/state.csv
+-rw-r--r--   0 james      (501) staff       (20)      350 2023-06-13 22:28:57.000000 agate-lookup-0.3.2/examples/usps/state.csv.yml
+-rw-r--r--   0 james      (501) staff       (20)      195 2023-06-13 23:08:50.540657 agate-lookup-0.3.2/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1792 2023-06-13 22:57:23.000000 agate-lookup-0.3.2/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-13 23:08:50.540162 agate-lookup-0.3.2/tests/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-06-13 22:28:57.000000 agate-lookup-0.3.2/tests/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      950 2023-06-13 23:03:21.000000 agate-lookup-0.3.2/tests/test_source.py
+-rw-r--r--   0 james      (501) staff       (20)     4359 2023-06-13 23:03:21.000000 agate-lookup-0.3.2/tests/test_table.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `agate-lookup-0.3.1/agate_lookup.egg-info/PKG-INFO` & `agate-lookup-0.3.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,55 +1,60 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: agate-lookup
-Version: 0.3.1
+Version: 0.3.2
 Summary: agate-lookup adds remote lookup tables to agate.
-Home-page: http://agate-lookup.readthedocs.org/
+Home-page: https://agate-lookup.readthedocs.org/
 Author: Christopher Groskopf
 Author-email: chrisgroskopf@gmail.com
 License: MIT
-Description: .. image:: https://travis-ci.org/wireservice/agate-lookup.png
-            :target: https://travis-ci.org/wireservice/agate-lookup
-            :alt: Build status
-        
-        .. image:: https://img.shields.io/pypi/dw/agate-lookup.svg
-            :target: https://pypi.python.org/pypi/agate-lookup
-            :alt: PyPI downloads
-        
-        .. image:: https://img.shields.io/pypi/v/agate-lookup.svg
-            :target: https://pypi.python.org/pypi/agate-lookup
-            :alt: Version
-        
-        .. image:: https://img.shields.io/pypi/l/agate-lookup.svg
-            :target: https://pypi.python.org/pypi/agate-lookup
-            :alt: License
-        
-        .. image:: https://img.shields.io/pypi/pyversions/agate-lookup.svg
-            :target: https://pypi.python.org/pypi/agate-lookup
-            :alt: Support Python versions
-        
-        agate-lookup adds one-line access to `lookup <https://github.com/wireservice/lookup>`_ tables to `agate <https://github.com/wireservice/agate>`_.
-        
-        Important links:
-        
-        * agate             http://agate.rtfd.org
-        * Documentation:    http://agate-lookup.rtfd.org
-        * Repository:       https://github.com/wireservice/agate-lookup
-        * Issues:           https://github.com/wireservice/agate-lookup/issues
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/x-rst
+Provides-Extra: test
+Provides-Extra: docs
+License-File: COPYING
+License-File: AUTHORS.rst
+
+.. image:: https://github.com/wireservice/agate-lookup/workflows/CI/badge.svg
+    :target: https://github.com/wireservice/agate-lookup/actions
+    :alt: Build status
+
+.. image:: https://img.shields.io/pypi/dw/agate-lookup.svg
+    :target: https://pypi.python.org/pypi/agate-lookup
+    :alt: PyPI downloads
+
+.. image:: https://img.shields.io/pypi/v/agate-lookup.svg
+    :target: https://pypi.python.org/pypi/agate-lookup
+    :alt: Version
+
+.. image:: https://img.shields.io/pypi/l/agate-lookup.svg
+    :target: https://pypi.python.org/pypi/agate-lookup
+    :alt: License
+
+.. image:: https://img.shields.io/pypi/pyversions/agate-lookup.svg
+    :target: https://pypi.python.org/pypi/agate-lookup
+    :alt: Support Python versions
+
+agate-lookup adds one-line access to `lookup <https://github.com/wireservice/lookup>`_ tables to `agate <https://github.com/wireservice/agate>`_.
+
+Important links:
+
+* agate             https://agate.rtfd.org
+* Documentation:    https://agate-lookup.rtfd.org
+* Repository:       https://github.com/wireservice/agate-lookup
+* Issues:           https://github.com/wireservice/agate-lookup/issues
```

### Comparing `agate-lookup-0.3.1/agatelookup/source.py` & `agate-lookup-0.3.2/agatelookup/source.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,86 +1,90 @@
 #!/usr/bin/env python
 
-import io
 import os
 
 import agate
-import six
 import requests
+import six
 import yaml
 
+
 def make_table_path(keys, value, version=None):
     """
     Generate a path to find a given lookup table.
     """
     if isinstance(keys, (list, tuple)):
         keys = '/'.join(keys)
 
-    path = '%s/%s' % (keys, value)
+    path = f'{keys}/{value}'
 
     if version:
         path += '.%s' % version
 
     path += '.csv'
 
     return path
 
+
 def make_metadata_path(keys, value, version=None):
     """
     Generate a path to find a given lookup table.
     """
     if isinstance(keys, (list, tuple)):
         keys = '/'.join(keys)
 
-    path = '%s/%s' % (keys, value)
+    path = f'{keys}/{value}'
 
     if version:
         path += '.%s' % version
 
     path += '.csv.yml'
 
     return path
 
+
 def make_type_tester(meta):
     """
     Uses parsed lookup table metadata to create a :class:`.agate.TypeTester`
     that will always use correct types for the table columns. (And avoid
     the overhead of type inference.)
     """
     force = {}
 
     for k, v in meta['columns'].items():
         force[k] = getattr(agate, v['type'])()
 
     return agate.TypeTester(force=force)
 
-class Source(object):
+
+class Source:
     """
     A reference to an archive of lookup tables. This is a remote location with
     lookup table and metadata files at a known path structure.
 
     :param root:
         The root URL to prefix all data and metadata paths.
     :param cache:
         A path in which to store cached copies of any tables that are used, so
         they can continue to be used offline.
     """
-    def __init__(self, root='http://wireservice.github.io/lookup', cache='~/.lookup'):
+
+    def __init__(self, root='https://wireservice.github.io/lookup', cache='~/.lookup'):
         self._root = root
         self._cache = os.path.expanduser(cache) if cache else None
 
     def _read_cache(self, path):
         """
         Read a file from the lookup cache.
         """
         if self._cache:
             cache_path = os.path.join(self._cache, path)
 
             if os.path.exists(cache_path):
-                with io.open(cache_path, encoding='utf-8') as f:
+                with open(cache_path, encoding='utf-8') as f:
                     text = f.read()
 
                 return text
 
         raise RuntimeError('Unable to download remote file "%s" and local cache is not available.' % path)
 
     def _write_cache(self, path, text):
@@ -91,37 +95,37 @@
             cache_path = os.path.join(self._cache, path)
 
             folder = os.path.split(cache_path)[0]
 
             if not os.path.exists(folder):
                 os.makedirs(folder)
 
-            with io.open(cache_path, 'w', encoding='utf-8') as f:
+            with open(cache_path, 'w', encoding='utf-8') as f:
                 f.write(text)
 
     def get_metadata(self, keys, value, version=None):
         """
         Fetches metadata related to a specific lookup table.
 
         See :meth:`Source.get_table` for parameter details.
         """
         path = make_metadata_path(keys, value, version)
-        url = '%s/%s' % (self._root, path)
+        url = f'{self._root}/{path}'
 
         try:
             r = requests.get(url)
             text = r.text
 
             self._write_cache(path, text)
         except (requests.ConnectionError, requests.Timeout):
             text = self._read_cache(path)
 
         try:
-            data = yaml.load(text)
-        except:
+            data = yaml.safe_load(text)
+        except yaml.YAMLError:
             raise ValueError('Failed to read or parse YAML at %s' % url)
 
         return data
 
     def get_table(self, keys, value, version=None):
         """
         Fetches and creates and agate table from a specified lookup table.
@@ -141,18 +145,18 @@
             For instance :code:`'2007'` for the 2007 edition of the NAICS codes
             or :code:`'2012'` for the 2012 version.
         """
         meta = self.get_metadata(keys, value, version)
         tester = make_type_tester(meta)
 
         path = make_table_path(keys, value, version)
-        url = '%s/%s' % (self._root, path)
+        url = f'{self._root}/{path}'
 
         if agate.utils.issequence(keys):
-            row_names = lambda r: tuple(r[k] for k in keys)
+            def row_names(r): return tuple(r[k] for k in keys)
         else:
             row_names = keys
 
         try:
             r = requests.get(url)
             text = r.text
```

### Comparing `agate-lookup-0.3.1/agatelookup/table.py` & `agate-lookup-0.3.2/agatelookup/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import agate
 
 from agatelookup.source import Source
 
 DEFAULT_SOURCE = Source()
 
+
 def lookup(self, key, value, lookup_key=None, version=None, source=None, require_match=False):
     """
     Fetch a lookup table from the remote source, matches it this table by
     its key columns, appends the value column and returns a new table
     instance.
 
     :param key:
@@ -44,19 +45,21 @@
     if source is None:
         source = DEFAULT_SOURCE
 
     table = source.get_table(lookup_key or key, value, version)
 
     return self.join(table, key, lookup_key, require_match=require_match)
 
+
 def from_lookup(cls, lookup_key, value, version=None, source=None):
     """
     Fetch a lookup table, but don't join it to anything. See
     :meth:`.TableLookup.lookup` for arguments.
     """
     if source is None:
         source = DEFAULT_SOURCE
 
     return source.get_table(lookup_key, value, version)
 
+
 agate.Table.lookup = lookup
 agate.Table.from_lookup = classmethod(from_lookup)
```

### Comparing `agate-lookup-0.3.1/PKG-INFO` & `agate-lookup-0.3.2/agate_lookup.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,55 +1,60 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: agate-lookup
-Version: 0.3.1
+Version: 0.3.2
 Summary: agate-lookup adds remote lookup tables to agate.
-Home-page: http://agate-lookup.readthedocs.org/
+Home-page: https://agate-lookup.readthedocs.org/
 Author: Christopher Groskopf
 Author-email: chrisgroskopf@gmail.com
 License: MIT
-Description: .. image:: https://travis-ci.org/wireservice/agate-lookup.png
-            :target: https://travis-ci.org/wireservice/agate-lookup
-            :alt: Build status
-        
-        .. image:: https://img.shields.io/pypi/dw/agate-lookup.svg
-            :target: https://pypi.python.org/pypi/agate-lookup
-            :alt: PyPI downloads
-        
-        .. image:: https://img.shields.io/pypi/v/agate-lookup.svg
-            :target: https://pypi.python.org/pypi/agate-lookup
-            :alt: Version
-        
-        .. image:: https://img.shields.io/pypi/l/agate-lookup.svg
-            :target: https://pypi.python.org/pypi/agate-lookup
-            :alt: License
-        
-        .. image:: https://img.shields.io/pypi/pyversions/agate-lookup.svg
-            :target: https://pypi.python.org/pypi/agate-lookup
-            :alt: Support Python versions
-        
-        agate-lookup adds one-line access to `lookup <https://github.com/wireservice/lookup>`_ tables to `agate <https://github.com/wireservice/agate>`_.
-        
-        Important links:
-        
-        * agate             http://agate.rtfd.org
-        * Documentation:    http://agate-lookup.rtfd.org
-        * Repository:       https://github.com/wireservice/agate-lookup
-        * Issues:           https://github.com/wireservice/agate-lookup/issues
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/x-rst
+Provides-Extra: test
+Provides-Extra: docs
+License-File: COPYING
+License-File: AUTHORS.rst
+
+.. image:: https://github.com/wireservice/agate-lookup/workflows/CI/badge.svg
+    :target: https://github.com/wireservice/agate-lookup/actions
+    :alt: Build status
+
+.. image:: https://img.shields.io/pypi/dw/agate-lookup.svg
+    :target: https://pypi.python.org/pypi/agate-lookup
+    :alt: PyPI downloads
+
+.. image:: https://img.shields.io/pypi/v/agate-lookup.svg
+    :target: https://pypi.python.org/pypi/agate-lookup
+    :alt: Version
+
+.. image:: https://img.shields.io/pypi/l/agate-lookup.svg
+    :target: https://pypi.python.org/pypi/agate-lookup
+    :alt: License
+
+.. image:: https://img.shields.io/pypi/pyversions/agate-lookup.svg
+    :target: https://pypi.python.org/pypi/agate-lookup
+    :alt: Support Python versions
+
+agate-lookup adds one-line access to `lookup <https://github.com/wireservice/lookup>`_ tables to `agate <https://github.com/wireservice/agate>`_.
+
+Important links:
+
+* agate             https://agate.rtfd.org
+* Documentation:    https://agate-lookup.rtfd.org
+* Repository:       https://github.com/wireservice/agate-lookup
+* Issues:           https://github.com/wireservice/agate-lookup/issues
```

### Comparing `agate-lookup-0.3.1/README.rst` & `agate-lookup-0.3.2/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-.. image:: https://travis-ci.org/wireservice/agate-lookup.png
-    :target: https://travis-ci.org/wireservice/agate-lookup
+.. image:: https://github.com/wireservice/agate-lookup/workflows/CI/badge.svg
+    :target: https://github.com/wireservice/agate-lookup/actions
     :alt: Build status
 
 .. image:: https://img.shields.io/pypi/dw/agate-lookup.svg
     :target: https://pypi.python.org/pypi/agate-lookup
     :alt: PyPI downloads
 
 .. image:: https://img.shields.io/pypi/v/agate-lookup.svg
@@ -18,11 +18,11 @@
     :target: https://pypi.python.org/pypi/agate-lookup
     :alt: Support Python versions
 
 agate-lookup adds one-line access to `lookup <https://github.com/wireservice/lookup>`_ tables to `agate <https://github.com/wireservice/agate>`_.
 
 Important links:
 
-* agate             http://agate.rtfd.org
-* Documentation:    http://agate-lookup.rtfd.org
+* agate             https://agate.rtfd.org
+* Documentation:    https://agate-lookup.rtfd.org
 * Repository:       https://github.com/wireservice/agate-lookup
 * Issues:           https://github.com/wireservice/agate-lookup/issues
```

### Comparing `agate-lookup-0.3.1/setup.py` & `agate-lookup-0.3.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,52 @@
-#!/usr/bin/env python
+from setuptools import find_packages, setup
 
-from setuptools import setup
-
-install_requires = [
-    'agate>=1.5.0',
-    'requests>=2.9.1',
-    'pyyaml>=3.11'
-]
+with open('README.rst') as f:
+    long_description = f.read()
 
 setup(
     name='agate-lookup',
-    version='0.3.1',
+    version='0.3.2',
     description='agate-lookup adds remote lookup tables to agate.',
-    long_description=open('README.rst').read(),
+    long_description=long_description,
+    long_description_content_type='text/x-rst',
     author='Christopher Groskopf',
     author_email='chrisgroskopf@gmail.com',
-    url='http://agate-lookup.readthedocs.org/',
+    url='https://agate-lookup.readthedocs.org/',
     license='MIT',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3.3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Topic :: Multimedia :: Graphics',
         'Topic :: Scientific/Engineering :: Information Analysis',
         'Topic :: Scientific/Engineering :: Visualization',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
-    packages=[
-        'agatelookup'
+    packages=find_packages(exclude=['tests', 'tests.*']),
+    install_requires=[
+        'agate>=1.5.0',
+        'requests>=2.9.1',
+        'pyyaml>=3.11'
     ],
-    install_requires=install_requires
+    extras_require={
+        'test': [
+            'pytest',
+            'pytest-cov',
+        ],
+        'docs': [
+            'Sphinx>=1.2.2',
+            'sphinx_rtd_theme>=0.1.6',
+        ],
+    }
 )
```

