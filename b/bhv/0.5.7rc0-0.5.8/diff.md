# Comparing `tmp/bhv-0.5.7rc0.tar.gz` & `tmp/bhv-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bhv-0.5.7rc0.tar", last modified: Sun Jun 11 01:19:23 2023, max compression
+gzip compressed data, was "bhv-0.5.8.tar", last modified: Sun Jun 11 01:25:23 2023, max compression
```

## Comparing `bhv-0.5.7rc0.tar` & `bhv-0.5.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-11 01:19:23.179913 bhv-0.5.7rc0/
--rw-r--r--   0 adam      (1000) adam      (1000)    35149 2023-05-25 19:11:00.000000 bhv-0.5.7rc0/LICENSE
--rw-r--r--   0 adam      (1000) adam      (1000)     1094 2023-06-11 01:19:23.179913 bhv-0.5.7rc0/PKG-INFO
--rw-r--r--   0 adam      (1000) adam      (1000)     3989 2023-06-08 12:48:26.000000 bhv-0.5.7rc0/README.md
-drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-11 01:19:23.178913 bhv-0.5.7rc0/bhv/
--rw-r--r--   0 adam      (1000) adam      (1000)       64 2023-04-07 21:25:34.000000 bhv-0.5.7rc0/bhv/__init__.py
--rw-r--r--   0 adam      (1000) adam      (1000)    14829 2023-06-06 19:12:06.000000 bhv-0.5.7rc0/bhv/abstract.py
-drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-11 01:19:23.179913 bhv-0.5.7rc0/bhv/cnative/
--rw-r--r--   0 adam      (1000) adam      (1000)     9757 2023-06-11 01:14:47.000000 bhv-0.5.7rc0/bhv/cnative/bindings.cpp
--rw-r--r--   0 adam      (1000) adam      (1000)     7130 2023-06-11 01:14:43.000000 bhv-0.5.7rc0/bhv/cnative/packed.h
--rw-r--r--   0 adam      (1000) adam      (1000)      392 2023-06-07 20:21:30.000000 bhv-0.5.7rc0/bhv/cnative/shared.h
--rw-r--r--   0 adam      (1000) adam      (1000)     2120 2023-05-25 19:11:00.000000 bhv-0.5.7rc0/bhv/embedding.py
--rw-r--r--   0 adam      (1000) adam      (1000)     4220 2023-06-06 19:12:06.000000 bhv-0.5.7rc0/bhv/lookup.py
--rw-r--r--   0 adam      (1000) adam      (1000)     1476 2023-06-11 00:46:52.000000 bhv-0.5.7rc0/bhv/native.py
--rw-r--r--   0 adam      (1000) adam      (1000)    11951 2023-05-25 19:11:00.000000 bhv-0.5.7rc0/bhv/np.py
--rw-r--r--   0 adam      (1000) adam      (1000)    11425 2023-05-25 19:11:00.000000 bhv-0.5.7rc0/bhv/poibin.py
--rw-r--r--   0 adam      (1000) adam      (1000)     8293 2023-05-25 19:11:00.000000 bhv-0.5.7rc0/bhv/pytorch.py
--rw-r--r--   0 adam      (1000) adam      (1000)     3360 2023-05-25 19:11:00.000000 bhv-0.5.7rc0/bhv/shared.py
--rw-r--r--   0 adam      (1000) adam      (1000)     1195 2023-05-25 19:11:00.000000 bhv-0.5.7rc0/bhv/slice.py
--rw-r--r--   0 adam      (1000) adam      (1000)    26226 2023-05-25 19:11:00.000000 bhv-0.5.7rc0/bhv/symbolic.py
--rw-r--r--   0 adam      (1000) adam      (1000)     1747 2023-05-25 19:11:00.000000 bhv-0.5.7rc0/bhv/unification.py
--rw-r--r--   0 adam      (1000) adam      (1000)     3456 2023-05-25 19:11:00.000000 bhv-0.5.7rc0/bhv/vanilla.py
--rw-r--r--   0 adam      (1000) adam      (1000)      782 2023-05-25 19:11:00.000000 bhv-0.5.7rc0/bhv/visualization.py
-drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-11 01:19:23.179913 bhv-0.5.7rc0/bhv.egg-info/
--rw-r--r--   0 adam      (1000) adam      (1000)     1094 2023-06-11 01:19:23.000000 bhv-0.5.7rc0/bhv.egg-info/PKG-INFO
--rw-r--r--   0 adam      (1000) adam      (1000)      441 2023-06-11 01:19:23.000000 bhv-0.5.7rc0/bhv.egg-info/SOURCES.txt
--rw-r--r--   0 adam      (1000) adam      (1000)        1 2023-06-11 01:19:23.000000 bhv-0.5.7rc0/bhv.egg-info/dependency_links.txt
--rw-r--r--   0 adam      (1000) adam      (1000)       45 2023-06-11 01:19:23.000000 bhv-0.5.7rc0/bhv.egg-info/requires.txt
--rw-r--r--   0 adam      (1000) adam      (1000)        4 2023-06-11 01:19:23.000000 bhv-0.5.7rc0/bhv.egg-info/top_level.txt
--rw-r--r--   0 adam      (1000) adam      (1000)       38 2023-06-11 01:19:23.179913 bhv-0.5.7rc0/setup.cfg
--rw-r--r--   0 adam      (1000) adam      (1000)     1634 2023-06-11 01:19:04.000000 bhv-0.5.7rc0/setup.py
+drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-11 01:25:23.386929 bhv-0.5.8/
+-rw-r--r--   0 adam      (1000) adam      (1000)    35149 2023-05-25 19:11:00.000000 bhv-0.5.8/LICENSE
+-rw-r--r--   0 adam      (1000) adam      (1000)     1091 2023-06-11 01:25:23.386929 bhv-0.5.8/PKG-INFO
+-rw-r--r--   0 adam      (1000) adam      (1000)     3989 2023-06-08 12:48:26.000000 bhv-0.5.8/README.md
+drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-11 01:25:23.385929 bhv-0.5.8/bhv/
+-rw-r--r--   0 adam      (1000) adam      (1000)       64 2023-04-07 21:25:34.000000 bhv-0.5.8/bhv/__init__.py
+-rw-r--r--   0 adam      (1000) adam      (1000)    14829 2023-06-06 19:12:06.000000 bhv-0.5.8/bhv/abstract.py
+drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-11 01:25:23.386929 bhv-0.5.8/bhv/cnative/
+-rw-r--r--   0 adam      (1000) adam      (1000)     9757 2023-06-11 01:14:47.000000 bhv-0.5.8/bhv/cnative/bindings.cpp
+-rw-r--r--   0 adam      (1000) adam      (1000)     7142 2023-06-11 01:24:16.000000 bhv-0.5.8/bhv/cnative/packed.h
+-rw-r--r--   0 adam      (1000) adam      (1000)      392 2023-06-07 20:21:30.000000 bhv-0.5.8/bhv/cnative/shared.h
+-rw-r--r--   0 adam      (1000) adam      (1000)     2120 2023-05-25 19:11:00.000000 bhv-0.5.8/bhv/embedding.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     4220 2023-06-06 19:12:06.000000 bhv-0.5.8/bhv/lookup.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     1476 2023-06-11 00:46:52.000000 bhv-0.5.8/bhv/native.py
+-rw-r--r--   0 adam      (1000) adam      (1000)    11951 2023-05-25 19:11:00.000000 bhv-0.5.8/bhv/np.py
+-rw-r--r--   0 adam      (1000) adam      (1000)    11425 2023-05-25 19:11:00.000000 bhv-0.5.8/bhv/poibin.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     8293 2023-05-25 19:11:00.000000 bhv-0.5.8/bhv/pytorch.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     3360 2023-05-25 19:11:00.000000 bhv-0.5.8/bhv/shared.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     1195 2023-05-25 19:11:00.000000 bhv-0.5.8/bhv/slice.py
+-rw-r--r--   0 adam      (1000) adam      (1000)    26226 2023-05-25 19:11:00.000000 bhv-0.5.8/bhv/symbolic.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     1747 2023-05-25 19:11:00.000000 bhv-0.5.8/bhv/unification.py
+-rw-r--r--   0 adam      (1000) adam      (1000)     3456 2023-05-25 19:11:00.000000 bhv-0.5.8/bhv/vanilla.py
+-rw-r--r--   0 adam      (1000) adam      (1000)      782 2023-05-25 19:11:00.000000 bhv-0.5.8/bhv/visualization.py
+drwxr-xr-x   0 adam      (1000) adam      (1000)        0 2023-06-11 01:25:23.386929 bhv-0.5.8/bhv.egg-info/
+-rw-r--r--   0 adam      (1000) adam      (1000)     1091 2023-06-11 01:25:23.000000 bhv-0.5.8/bhv.egg-info/PKG-INFO
+-rw-r--r--   0 adam      (1000) adam      (1000)      441 2023-06-11 01:25:23.000000 bhv-0.5.8/bhv.egg-info/SOURCES.txt
+-rw-r--r--   0 adam      (1000) adam      (1000)        1 2023-06-11 01:25:23.000000 bhv-0.5.8/bhv.egg-info/dependency_links.txt
+-rw-r--r--   0 adam      (1000) adam      (1000)       45 2023-06-11 01:25:23.000000 bhv-0.5.8/bhv.egg-info/requires.txt
+-rw-r--r--   0 adam      (1000) adam      (1000)        4 2023-06-11 01:25:23.000000 bhv-0.5.8/bhv.egg-info/top_level.txt
+-rw-r--r--   0 adam      (1000) adam      (1000)       38 2023-06-11 01:25:23.386929 bhv-0.5.8/setup.cfg
+-rw-r--r--   0 adam      (1000) adam      (1000)     1633 2023-06-11 01:25:11.000000 bhv-0.5.8/setup.py
```

### Comparing `bhv-0.5.7rc0/LICENSE` & `bhv-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bhv-0.5.7rc0/PKG-INFO` & `bhv-0.5.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.5.7rc0
+Version: 0.5.8
 Summary: Boolean Hypervectors
 Home-page: https://github.com/Adam-Vandervorst/PyBHV
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 License: UNKNOWN
 Keywords: ai binary hypervector hdc bsc
 Platform: UNKNOWN
```

### Comparing `bhv-0.5.7rc0/README.md` & `bhv-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `bhv-0.5.7rc0/bhv/abstract.py` & `bhv-0.5.8/bhv/abstract.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.7rc0/bhv/cnative/bindings.cpp` & `bhv-0.5.8/bhv/cnative/bindings.cpp`

 * *Files identical despite different names*

### Comparing `bhv-0.5.7rc0/bhv/cnative/packed.h` & `bhv-0.5.8/bhv/cnative/packed.h`

 * *Files 2% similar despite different names*

```diff
@@ -64,23 +64,23 @@
         random_into(x, p);
         return x;
     }
 
     bit_iter_t active(word_t * x) {
         bit_iter_t total = 0;
         for (word_iter_t i = 0; i < WORDS; ++i) {
-            total += std::popcount(x[i]);
+            total += __builtin_popcountl(x[i]);
         }
         return total;
     }
 
     bit_iter_t hamming(word_t * x, word_t * y) {
         bit_iter_t total = 0;
         for (word_iter_t i = 0; i < WORDS; ++i) {
-            total += std::popcount(x[i] ^ y[i]);
+            total += __builtin_popcountl(x[i] ^ y[i]);
         }
         return total;
     }
 
     bool eq(word_t * x, word_t * y) {
         for (word_iter_t i = 0; i < WORDS; ++i) {
             if (x[i] != y[i])
```

### Comparing `bhv-0.5.7rc0/bhv/embedding.py` & `bhv-0.5.8/bhv/embedding.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.7rc0/bhv/lookup.py` & `bhv-0.5.8/bhv/lookup.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.7rc0/bhv/native.py` & `bhv-0.5.8/bhv/native.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.7rc0/bhv/np.py` & `bhv-0.5.8/bhv/np.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.7rc0/bhv/poibin.py` & `bhv-0.5.8/bhv/poibin.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.7rc0/bhv/pytorch.py` & `bhv-0.5.8/bhv/pytorch.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.7rc0/bhv/shared.py` & `bhv-0.5.8/bhv/shared.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.7rc0/bhv/slice.py` & `bhv-0.5.8/bhv/slice.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.7rc0/bhv/symbolic.py` & `bhv-0.5.8/bhv/symbolic.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.7rc0/bhv/unification.py` & `bhv-0.5.8/bhv/unification.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.7rc0/bhv/vanilla.py` & `bhv-0.5.8/bhv/vanilla.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.7rc0/bhv/visualization.py` & `bhv-0.5.8/bhv/visualization.py`

 * *Files identical despite different names*

### Comparing `bhv-0.5.7rc0/bhv.egg-info/PKG-INFO` & `bhv-0.5.8/bhv.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.5.7rc0
+Version: 0.5.8
 Summary: Boolean Hypervectors
 Home-page: https://github.com/Adam-Vandervorst/PyBHV
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 License: UNKNOWN
 Keywords: ai binary hypervector hdc bsc
 Platform: UNKNOWN
```

### Comparing `bhv-0.5.7rc0/setup.py` & `bhv-0.5.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages, Extension
 
-VERSION = '0.5.7c'
+VERSION = '0.5.8'
 DESCRIPTION = 'Boolean Hypervectors'
 LONG_DESCRIPTION = 'Boolean Hypervectors with various operators for experiments in hyperdimensional computing (HDC).'
 
 native = Extension("bhv.cnative",
                    sources=['bhv/cnative/bindings.cpp'],
                    include_dirs=['bhv/cnative'],
                    extra_compile_args=['-std=c++2a', '-O3', '-march=native'],
```

