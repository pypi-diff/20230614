# Comparing `tmp/napari-nanopyx-0.0.2.tar.gz` & `tmp/napari-nanopyx-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-nanopyx-0.0.2.tar", last modified: Mon Jun 12 13:40:10 2023, max compression
+gzip compressed data, was "napari-nanopyx-0.0.3.tar", last modified: Wed Jun 14 10:46:40 2023, max compression
```

## Comparing `napari-nanopyx-0.0.2.tar` & `napari-nanopyx-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 abrito   (1547774166) RAS\Domain Users (931978602)        0 2023-06-12 13:40:10.223234 napari-nanopyx-0.0.2/
--rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)     7653 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.2/LICENSE
--rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)       96 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.2/MANIFEST.in
--rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)     3273 2023-06-12 13:40:10.223316 napari-nanopyx-0.0.2/PKG-INFO
--rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)     2573 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.2/README.md
--rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)     1045 2023-06-12 13:29:33.000000 napari-nanopyx-0.0.2/pyproject.toml
--rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)     1337 2023-06-12 13:40:10.223658 napari-nanopyx-0.0.2/setup.cfg
-drwxr-xr-x   0 abrito   (1547774166) RAS\Domain Users (931978602)        0 2023-06-12 13:40:10.219364 napari-nanopyx-0.0.2/src/
-drwxr-xr-x   0 abrito   (1547774166) RAS\Domain Users (931978602)        0 2023-06-12 13:40:10.221877 napari-nanopyx-0.0.2/src/napari_nanopyx/
--rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)       41 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.2/src/napari_nanopyx/__init__.py
-drwxr-xr-x   0 abrito   (1547774166) RAS\Domain Users (931978602)        0 2023-06-12 13:40:10.223093 napari-nanopyx-0.0.2/src/napari_nanopyx/_tests/
--rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)        0 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.2/src/napari_nanopyx/_tests/__init__.py
--rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)     3980 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.2/src/napari_nanopyx/channel_registration.py
--rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)     4408 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.2/src/napari_nanopyx/drift_alignment.py
--rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)     2308 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.2/src/napari_nanopyx/napari.yaml
--rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)     3750 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.2/src/napari_nanopyx/squirrel.py
--rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)     2421 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.2/src/napari_nanopyx/srrf.py
-drwxr-xr-x   0 abrito   (1547774166) RAS\Domain Users (931978602)        0 2023-06-12 13:40:10.222929 napari-nanopyx-0.0.2/src/napari_nanopyx.egg-info/
--rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)     3273 2023-06-12 13:40:10.000000 napari-nanopyx-0.0.2/src/napari_nanopyx.egg-info/PKG-INFO
--rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)      547 2023-06-12 13:40:10.000000 napari-nanopyx-0.0.2/src/napari_nanopyx.egg-info/SOURCES.txt
--rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)        1 2023-06-12 13:40:10.000000 napari-nanopyx-0.0.2/src/napari_nanopyx.egg-info/dependency_links.txt
--rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)       62 2023-06-12 13:40:10.000000 napari-nanopyx-0.0.2/src/napari_nanopyx.egg-info/entry_points.txt
--rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)       44 2023-06-12 13:40:10.000000 napari-nanopyx-0.0.2/src/napari_nanopyx.egg-info/requires.txt
--rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)       15 2023-06-12 13:40:10.000000 napari-nanopyx-0.0.2/src/napari_nanopyx.egg-info/top_level.txt
+drwxr-xr-x   0 abrito   (1547774166) 931978602        0 2023-06-14 10:46:40.381846 napari-nanopyx-0.0.3/
+-rw-r--r--   0 abrito   (1547774166) 931978602     7653 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.3/LICENSE
+-rw-r--r--   0 abrito   (1547774166) 931978602       96 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.3/MANIFEST.in
+-rw-r--r--   0 abrito   (1547774166) 931978602     3418 2023-06-14 10:46:40.381922 napari-nanopyx-0.0.3/PKG-INFO
+-rw-r--r--   0 abrito   (1547774166) 931978602     2573 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.3/README.md
+-rw-r--r--   0 abrito   (1547774166) 931978602      179 2023-06-14 10:46:27.000000 napari-nanopyx-0.0.3/pyproject.toml
+-rw-r--r--   0 abrito   (1547774166) 931978602     1222 2023-06-14 10:46:40.382296 napari-nanopyx-0.0.3/setup.cfg
+drwxr-xr-x   0 abrito   (1547774166) 931978602        0 2023-06-14 10:46:40.378217 napari-nanopyx-0.0.3/src/
+drwxr-xr-x   0 abrito   (1547774166) 931978602        0 2023-06-14 10:46:40.380376 napari-nanopyx-0.0.3/src/napari_nanopyx/
+-rw-r--r--   0 abrito   (1547774166) 931978602       41 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.3/src/napari_nanopyx/__init__.py
+drwxr-xr-x   0 abrito   (1547774166) 931978602        0 2023-06-14 10:46:40.381705 napari-nanopyx-0.0.3/src/napari_nanopyx/_tests/
+-rw-r--r--   0 abrito   (1547774166) 931978602        0 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.3/src/napari_nanopyx/_tests/__init__.py
+-rw-r--r--   0 abrito   (1547774166) 931978602     3980 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.3/src/napari_nanopyx/channel_registration.py
+-rw-r--r--   0 abrito   (1547774166) 931978602     4408 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.3/src/napari_nanopyx/drift_alignment.py
+-rw-r--r--   0 abrito   (1547774166) 931978602     2308 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.3/src/napari_nanopyx/napari.yaml
+-rw-r--r--   0 abrito   (1547774166) 931978602     3750 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.3/src/napari_nanopyx/squirrel.py
+-rw-r--r--   0 abrito   (1547774166) 931978602     2421 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.3/src/napari_nanopyx/srrf.py
+drwxr-xr-x   0 abrito   (1547774166) 931978602        0 2023-06-14 10:46:40.381440 napari-nanopyx-0.0.3/src/napari_nanopyx.egg-info/
+-rw-r--r--   0 abrito   (1547774166) 931978602     3418 2023-06-14 10:46:40.000000 napari-nanopyx-0.0.3/src/napari_nanopyx.egg-info/PKG-INFO
+-rw-r--r--   0 abrito   (1547774166) 931978602      547 2023-06-14 10:46:40.000000 napari-nanopyx-0.0.3/src/napari_nanopyx.egg-info/SOURCES.txt
+-rw-r--r--   0 abrito   (1547774166) 931978602        1 2023-06-14 10:46:40.000000 napari-nanopyx-0.0.3/src/napari_nanopyx.egg-info/dependency_links.txt
+-rw-r--r--   0 abrito   (1547774166) 931978602       62 2023-06-14 10:46:40.000000 napari-nanopyx-0.0.3/src/napari_nanopyx.egg-info/entry_points.txt
+-rw-r--r--   0 abrito   (1547774166) 931978602       29 2023-06-14 10:46:40.000000 napari-nanopyx-0.0.3/src/napari_nanopyx.egg-info/requires.txt
+-rw-r--r--   0 abrito   (1547774166) 931978602       15 2023-06-14 10:46:40.000000 napari-nanopyx-0.0.3/src/napari_nanopyx.egg-info/top_level.txt
```

### Comparing `napari-nanopyx-0.0.2/LICENSE` & `napari-nanopyx-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-nanopyx-0.0.2/PKG-INFO` & `napari-nanopyx-0.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: napari-nanopyx
-Version: 0.0.2
-Summary: napari plugin for NanoPyx
-Author: Bruno Saraiva
-Author-email: Ricardo Henriques <ricardo.jv.henriques@gmail.com>, Bruno Saraiva <bruno.msaraiva2@gmail.com>, Inês Cunha <inescunha200@gmail.com>, António Brito <antmsbrito95@gmail.com>
-Maintainer-email: Bruno Saraiva <bruno.msaraiva2@gmail.com>
-Keywords: napari,NanoJ,Super-Resolution Microscopy,Fluorescence,BioImage Analysis
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-License-File: LICENSE
-
 # napari-nanopyx
 
 [![License GNU LGPL v3.0](https://img.shields.io/pypi/l/napari-nanopyx.svg?color=green)](https://github.com/HenriquesLab/napari-NanoPyx/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-nanopyx.svg?color=green)](https://pypi.org/project/napari-nanopyx)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-nanopyx.svg?color=green)](https://python.org)
 [![tests](https://github.com/HenriquesLab/napari-NanoPyx/workflows/tests/badge.svg)](https://github.com/HenriquesLab/napari-NanoPyx/actions)
 [![codecov](https://codecov.io/gh/brunomsaraiva/napari-nanopyx/branch/main/graph/badge.svg)](https://codecov.io/gh/brunomsaraiva/napari-nanopyx)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `napari-nanopyx-0.0.2/README.md` & `napari-nanopyx-0.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: napari-nanopyx
+Version: 0.0.3
+Summary: napari plugin of Nanoscopy Python library (NanoPyx, the successor to NanoJ) - focused on light microscopy and super-resolution imaging
+Author: Ricardo Henriques, Bruno Saraiva, Inês Cunha, António Brito
+Author-email: bruno.msaraiva2@gmail.com
+License: LGPL-3.0-only
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Framework :: napari
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Testing
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: testing
+License-File: LICENSE
+
 # napari-nanopyx
 
 [![License GNU LGPL v3.0](https://img.shields.io/pypi/l/napari-nanopyx.svg?color=green)](https://github.com/HenriquesLab/napari-NanoPyx/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-nanopyx.svg?color=green)](https://pypi.org/project/napari-nanopyx)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-nanopyx.svg?color=green)](https://python.org)
 [![tests](https://github.com/HenriquesLab/napari-NanoPyx/workflows/tests/badge.svg)](https://github.com/HenriquesLab/napari-NanoPyx/actions)
 [![codecov](https://codecov.io/gh/brunomsaraiva/napari-nanopyx/branch/main/graph/badge.svg)](https://codecov.io/gh/brunomsaraiva/napari-nanopyx)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `napari-nanopyx-0.0.2/setup.cfg` & `napari-nanopyx-0.0.3/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 [metadata]
 name = napari-nanopyx
-version = 0.0.2
+version = 0.0.3
 description = napari plugin of Nanoscopy Python library (NanoPyx, the successor to NanoJ) - focused on light microscopy and super-resolution imaging
 long_description = file: README.md
 long_description_content_type = text/markdown
-author = Bruno Saraiva
+author = Ricardo Henriques, Bruno Saraiva, Inês Cunha, António Brito
 author_email = bruno.msaraiva2@gmail.com
 license = LGPL-3.0-only
 license_files = LICENSE
 classifiers = 
 	Development Status :: 2 - Pre-Alpha
 	Framework :: napari
 	Intended Audience :: Developers
 	License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
-	Programming Language :: Python :: 3.10
 	Topic :: Software Development :: Testing
 
 [options]
 packages = find:
 python_requires = >=3.8
 include_package_data = True
 package_dir =
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `napari-nanopyx-0.0.2/src/napari_nanopyx/channel_registration.py` & `napari-nanopyx-0.0.3/src/napari_nanopyx/channel_registration.py`

 * *Files identical despite different names*

### Comparing `napari-nanopyx-0.0.2/src/napari_nanopyx/drift_alignment.py` & `napari-nanopyx-0.0.3/src/napari_nanopyx/drift_alignment.py`

 * *Files identical despite different names*

### Comparing `napari-nanopyx-0.0.2/src/napari_nanopyx/napari.yaml` & `napari-nanopyx-0.0.3/src/napari_nanopyx/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-nanopyx-0.0.2/src/napari_nanopyx/squirrel.py` & `napari-nanopyx-0.0.3/src/napari_nanopyx/squirrel.py`

 * *Files identical despite different names*

### Comparing `napari-nanopyx-0.0.2/src/napari_nanopyx/srrf.py` & `napari-nanopyx-0.0.3/src/napari_nanopyx/srrf.py`

 * *Files identical despite different names*

### Comparing `napari-nanopyx-0.0.2/src/napari_nanopyx.egg-info/PKG-INFO` & `napari-nanopyx-0.0.3/src/napari_nanopyx.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: napari-nanopyx
-Version: 0.0.2
-Summary: napari plugin for NanoPyx
-Author: Bruno Saraiva
-Author-email: Ricardo Henriques <ricardo.jv.henriques@gmail.com>, Bruno Saraiva <bruno.msaraiva2@gmail.com>, Inês Cunha <inescunha200@gmail.com>, António Brito <antmsbrito95@gmail.com>
-Maintainer-email: Bruno Saraiva <bruno.msaraiva2@gmail.com>
-Keywords: napari,NanoJ,Super-Resolution Microscopy,Fluorescence,BioImage Analysis
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Version: 0.0.3
+Summary: napari plugin of Nanoscopy Python library (NanoPyx, the successor to NanoJ) - focused on light microscopy and super-resolution imaging
+Author: Ricardo Henriques, Bruno Saraiva, Inês Cunha, António Brito
+Author-email: bruno.msaraiva2@gmail.com
+License: LGPL-3.0-only
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Framework :: napari
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 # napari-nanopyx
```

### Comparing `napari-nanopyx-0.0.2/src/napari_nanopyx.egg-info/SOURCES.txt` & `napari-nanopyx-0.0.3/src/napari_nanopyx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

