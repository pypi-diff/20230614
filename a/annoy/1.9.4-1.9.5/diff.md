# Comparing `tmp/annoy-1.9.4.tar.gz` & `tmp/annoy-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/annoy-1.9.4.tar", last modified: Sat Aug 26 02:29:43 2017, max compression
+gzip compressed data, was "dist/annoy-1.9.5.tar", last modified: Sat Sep 30 15:45:32 2017, max compression
```

## Comparing `annoy-1.9.4.tar` & `annoy-1.9.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 erikbern   (501) staff       (20)        0 2017-08-26 02:29:43.000000 annoy-1.9.4/
--rw-r--r--   0 erikbern   (501) staff       (20)   609008 2017-08-26 02:29:01.000000 annoy-1.9.4/ann.png
-drwxr-xr-x   0 erikbern   (501) staff       (20)        0 2017-08-26 02:29:43.000000 annoy-1.9.4/annoy/
--rw-r--r--   0 erikbern   (501) staff       (20)      684 2017-08-26 02:29:01.000000 annoy-1.9.4/annoy/__init__.py
-drwxr-xr-x   0 erikbern   (501) staff       (20)        0 2017-08-26 02:29:43.000000 annoy-1.9.4/annoy.egg-info/
--rw-r--r--   0 erikbern   (501) staff       (20)        1 2017-08-26 02:29:43.000000 annoy-1.9.4/annoy.egg-info/dependency_links.txt
--rw-r--r--   0 erikbern   (501) staff       (20)    11771 2017-08-26 02:29:43.000000 annoy-1.9.4/annoy.egg-info/PKG-INFO
--rw-r--r--   0 erikbern   (501) staff       (20)      253 2017-08-26 02:29:43.000000 annoy-1.9.4/annoy.egg-info/SOURCES.txt
--rw-r--r--   0 erikbern   (501) staff       (20)        6 2017-08-26 02:29:43.000000 annoy-1.9.4/annoy.egg-info/top_level.txt
--rw-r--r--   0 erikbern   (501) staff       (20)    11358 2017-08-26 02:29:01.000000 annoy-1.9.4/LICENSE
--rw-r--r--   0 erikbern   (501) staff       (20)      102 2017-08-26 02:29:01.000000 annoy-1.9.4/MANIFEST.in
--rw-r--r--   0 erikbern   (501) staff       (20)    11771 2017-08-26 02:29:43.000000 annoy-1.9.4/PKG-INFO
--rw-r--r--   0 erikbern   (501) staff       (20)     9608 2017-08-26 02:29:01.000000 annoy-1.9.4/README.rst
--rw-r--r--   0 erikbern   (501) staff       (20)       99 2017-08-26 02:29:43.000000 annoy-1.9.4/setup.cfg
--rw-r--r--   0 erikbern   (501) staff       (20)     2577 2017-08-26 02:29:41.000000 annoy-1.9.4/setup.py
-drwxr-xr-x   0 erikbern   (501) staff       (20)        0 2017-08-26 02:29:43.000000 annoy-1.9.4/src/
--rw-r--r--   0 erikbern   (501) staff       (20)    18905 2017-08-26 02:29:01.000000 annoy-1.9.4/src/annoylib.h
--rw-r--r--   0 erikbern   (501) staff       (20)    14173 2017-08-26 02:29:01.000000 annoy-1.9.4/src/annoymodule.cc
--rw-r--r--   0 erikbern   (501) staff       (20)     2234 2017-08-26 02:29:01.000000 annoy-1.9.4/src/kissrandom.h
--rw-r--r--   0 erikbern   (501) staff       (20)     4891 2017-08-26 02:29:01.000000 annoy-1.9.4/src/mman.h
+drwxr-xr-x   0 erikbern   (501) staff       (20)        0 2017-09-30 15:45:32.000000 annoy-1.9.5/
+-rw-r--r--   0 erikbern   (501) staff       (20)   609008 2017-08-26 02:29:01.000000 annoy-1.9.5/ann.png
+drwxr-xr-x   0 erikbern   (501) staff       (20)        0 2017-09-30 15:45:32.000000 annoy-1.9.5/annoy/
+-rw-r--r--   0 erikbern   (501) staff       (20)      684 2017-08-26 02:29:01.000000 annoy-1.9.5/annoy/__init__.py
+drwxr-xr-x   0 erikbern   (501) staff       (20)        0 2017-09-30 15:45:32.000000 annoy-1.9.5/annoy.egg-info/
+-rw-r--r--   0 erikbern   (501) staff       (20)        1 2017-09-30 15:45:32.000000 annoy-1.9.5/annoy.egg-info/dependency_links.txt
+-rw-r--r--   0 erikbern   (501) staff       (20)    11771 2017-09-30 15:45:32.000000 annoy-1.9.5/annoy.egg-info/PKG-INFO
+-rw-r--r--   0 erikbern   (501) staff       (20)      253 2017-09-30 15:45:32.000000 annoy-1.9.5/annoy.egg-info/SOURCES.txt
+-rw-r--r--   0 erikbern   (501) staff       (20)        6 2017-09-30 15:45:32.000000 annoy-1.9.5/annoy.egg-info/top_level.txt
+-rw-r--r--   0 erikbern   (501) staff       (20)    11358 2017-08-26 02:29:01.000000 annoy-1.9.5/LICENSE
+-rw-r--r--   0 erikbern   (501) staff       (20)      102 2017-08-26 02:29:01.000000 annoy-1.9.5/MANIFEST.in
+-rw-r--r--   0 erikbern   (501) staff       (20)    11771 2017-09-30 15:45:32.000000 annoy-1.9.5/PKG-INFO
+-rw-r--r--   0 erikbern   (501) staff       (20)     9608 2017-08-26 02:29:01.000000 annoy-1.9.5/README.rst
+-rw-r--r--   0 erikbern   (501) staff       (20)       99 2017-09-30 15:45:32.000000 annoy-1.9.5/setup.cfg
+-rw-r--r--   0 erikbern   (501) staff       (20)     2577 2017-09-30 15:42:35.000000 annoy-1.9.5/setup.py
+drwxr-xr-x   0 erikbern   (501) staff       (20)        0 2017-09-30 15:45:32.000000 annoy-1.9.5/src/
+-rw-r--r--   0 erikbern   (501) staff       (20)    18958 2017-09-30 01:29:44.000000 annoy-1.9.5/src/annoylib.h
+-rw-r--r--   0 erikbern   (501) staff       (20)    14173 2017-09-30 01:30:24.000000 annoy-1.9.5/src/annoymodule.cc
+-rw-r--r--   0 erikbern   (501) staff       (20)     2234 2017-08-26 02:29:01.000000 annoy-1.9.5/src/kissrandom.h
+-rw-r--r--   0 erikbern   (501) staff       (20)     4891 2017-08-26 02:29:01.000000 annoy-1.9.5/src/mman.h
```

### Comparing `annoy-1.9.4/ann.png` & `annoy-1.9.5/ann.png`

 * *Files identical despite different names*

### Comparing `annoy-1.9.4/annoy/__init__.py` & `annoy-1.9.5/annoy/__init__.py`

 * *Files identical despite different names*

### Comparing `annoy-1.9.4/annoy.egg-info/PKG-INFO` & `annoy-1.9.5/annoy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: annoy
-Version: 1.9.4
+Version: 1.9.5
 Summary: Approximate Nearest Neighbors in C++/Python optimized for memory usage and loading/saving to disk.
 Home-page: https://github.com/spotify/annoy
 Author: Erik Bernhardsson
 Author-email: mail@erikbern.com
 License: Apache License 2.0
 Description: .. note::
```

### Comparing `annoy-1.9.4/LICENSE` & `annoy-1.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `annoy-1.9.4/PKG-INFO` & `annoy-1.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: annoy
-Version: 1.9.4
+Version: 1.9.5
 Summary: Approximate Nearest Neighbors in C++/Python optimized for memory usage and loading/saving to disk.
 Home-page: https://github.com/spotify/annoy
 Author: Erik Bernhardsson
 Author-email: mail@erikbern.com
 License: Apache License 2.0
 Description: .. note::
```

### Comparing `annoy-1.9.4/README.rst` & `annoy-1.9.5/README.rst`

 * *Files identical despite different names*

### Comparing `annoy-1.9.4/setup.py` & `annoy-1.9.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 # Not all CPUs have march as a tuning parameter
 import platform
 cputune = ['-march=native',]
 if platform.machine() == "ppc64le":
     cputune = ['-mcpu=native',]
 
 setup(name='annoy',
-      version='1.9.4',
+      version='1.9.5',
       description='Approximate Nearest Neighbors in C++/Python optimized for memory usage and loading/saving to disk.',
       packages=['annoy'],
       ext_modules=[
         Extension(
             'annoy.annoylib', ['src/annoymodule.cc'],
             depends=['src/annoylib.h', 'src/kissrandom.h', 'src/mman.h'],
             extra_compile_args=['-O3', '-ffast-math', '-fno-associative-math'] + cputune + travis_extra_compile_args,
```

### Comparing `annoy-1.9.4/src/annoylib.h` & `annoy-1.9.5/src/annoylib.h`

 * *Files 1% similar despite different names*

```diff
@@ -359,16 +359,18 @@
       if (q == -1 && _n_nodes >= _n_items * 2)
         break;
       if (q != -1 && _roots.size() >= (size_t)q)
         break;
       if (_verbose) showUpdate("pass %zd...\n", _roots.size());
 
       vector<S> indices;
-      for (S i = 0; i < _n_items; i++)
-        indices.push_back(i);
+      for (S i = 0; i < _n_items; i++) {
+	if (_get(i)->n_descendants >= 1) // Issue #223
+	  indices.push_back(i);
+      }
 
       _roots.push_back(_make_tree(indices));
     }
     // Also, copy the roots into the last segment of the array
     // This way we can load them faster without reading the whole file
     _allocate_size(_n_nodes + (S)_roots.size());
     for (size_t i = 0; i < _roots.size(); i++)
```

### Comparing `annoy-1.9.4/src/annoymodule.cc` & `annoy-1.9.5/src/annoymodule.cc`

 * *Files identical despite different names*

### Comparing `annoy-1.9.4/src/kissrandom.h` & `annoy-1.9.5/src/kissrandom.h`

 * *Files identical despite different names*

### Comparing `annoy-1.9.4/src/mman.h` & `annoy-1.9.5/src/mman.h`

 * *Files identical despite different names*

