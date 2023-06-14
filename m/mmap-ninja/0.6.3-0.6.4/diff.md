# Comparing `tmp/mmap_ninja-0.6.3.tar.gz` & `tmp/mmap_ninja-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmap_ninja-0.6.3.tar", last modified: Thu Mar 30 18:58:38 2023, max compression
+gzip compressed data, was "mmap_ninja-0.6.4.tar", last modified: Sat Apr  8 07:07:21 2023, max compression
```

## Comparing `mmap_ninja-0.6.3.tar` & `mmap_ninja-0.6.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 hvrigazov  (1000) hvrigazov  (1000)        0 2023-03-30 18:58:38.023388 mmap_ninja-0.6.3/
--rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)    11739 2023-03-30 18:58:38.023388 mmap_ninja-0.6.3/PKG-INFO
--rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)    10897 2022-10-08 07:05:41.000000 mmap_ninja-0.6.3/README.md
--rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)      446 2022-09-09 05:58:58.000000 mmap_ninja-0.6.3/TODO.md
--rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)     2557 2022-09-09 05:58:58.000000 mmap_ninja-0.6.3/benchmark_images.py
-drwxrwxr-x   0 hvrigazov  (1000) hvrigazov  (1000)        0 2023-03-30 18:58:38.023388 mmap_ninja-0.6.3/mmap_ninja/
--rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)       22 2023-03-30 18:58:24.000000 mmap_ninja-0.6.3/mmap_ninja/__init__.py
--rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)     7125 2023-03-02 15:49:09.000000 mmap_ninja-0.6.3/mmap_ninja/base.py
--rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)      978 2023-03-30 18:58:18.000000 mmap_ninja-0.6.3/mmap_ninja/generic.py
--rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)     6973 2023-03-15 07:45:40.000000 mmap_ninja-0.6.3/mmap_ninja/numpy.py
--rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)     6467 2023-03-19 12:40:14.000000 mmap_ninja-0.6.3/mmap_ninja/ragged.py
--rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)     4702 2023-03-30 18:51:48.000000 mmap_ninja-0.6.3/mmap_ninja/string.py
-drwxrwxr-x   0 hvrigazov  (1000) hvrigazov  (1000)        0 2023-03-30 18:58:38.023388 mmap_ninja-0.6.3/mmap_ninja.egg-info/
--rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)    11739 2023-03-30 18:58:37.000000 mmap_ninja-0.6.3/mmap_ninja.egg-info/PKG-INFO
--rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)      461 2023-03-30 18:58:38.000000 mmap_ninja-0.6.3/mmap_ninja.egg-info/SOURCES.txt
--rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)        1 2023-03-30 18:58:37.000000 mmap_ninja-0.6.3/mmap_ninja.egg-info/dependency_links.txt
--rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)       11 2023-03-30 18:58:37.000000 mmap_ninja-0.6.3/mmap_ninja.egg-info/requires.txt
--rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)       11 2023-03-30 18:58:37.000000 mmap_ninja-0.6.3/mmap_ninja.egg-info/top_level.txt
--rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)       11 2022-09-09 05:58:58.000000 mmap_ninja-0.6.3/requirements.txt
--rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)       38 2023-03-30 18:58:38.023388 mmap_ninja-0.6.3/setup.cfg
--rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)     1325 2023-02-19 17:53:50.000000 mmap_ninja-0.6.3/setup.py
-drwxrwxr-x   0 hvrigazov  (1000) hvrigazov  (1000)        0 2023-03-30 18:58:38.023388 mmap_ninja-0.6.3/tests/
--rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)     1141 2023-02-03 06:54:46.000000 mmap_ninja-0.6.3/tests/test_base.py
--rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)      309 2023-02-03 07:45:29.000000 mmap_ninja-0.6.3/tests/test_generic.py
--rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)     2523 2023-03-30 18:51:48.000000 mmap_ninja-0.6.3/tests/test_numpy.py
--rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)     5828 2023-03-30 18:51:48.000000 mmap_ninja-0.6.3/tests/test_ragged.py
--rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)     3240 2023-03-30 18:51:48.000000 mmap_ninja-0.6.3/tests/test_string.py
+drwxrwxr-x   0 hvrigazov  (1000) hvrigazov  (1000)        0 2023-04-08 07:07:21.389689 mmap_ninja-0.6.4/
+-rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)    11739 2023-04-08 07:07:21.389689 mmap_ninja-0.6.4/PKG-INFO
+-rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)    10897 2022-10-08 07:05:41.000000 mmap_ninja-0.6.4/README.md
+-rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)      446 2022-09-09 05:58:58.000000 mmap_ninja-0.6.4/TODO.md
+-rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)     2557 2022-09-09 05:58:58.000000 mmap_ninja-0.6.4/benchmark_images.py
+drwxrwxr-x   0 hvrigazov  (1000) hvrigazov  (1000)        0 2023-04-08 07:07:21.385689 mmap_ninja-0.6.4/mmap_ninja/
+-rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)       22 2023-04-08 07:06:02.000000 mmap_ninja-0.6.4/mmap_ninja/__init__.py
+-rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)     7125 2023-03-02 15:49:09.000000 mmap_ninja-0.6.4/mmap_ninja/base.py
+-rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)      978 2023-03-30 18:58:18.000000 mmap_ninja-0.6.4/mmap_ninja/generic.py
+-rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)     6926 2023-04-08 07:06:13.000000 mmap_ninja-0.6.4/mmap_ninja/numpy.py
+-rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)     6467 2023-03-19 12:40:14.000000 mmap_ninja-0.6.4/mmap_ninja/ragged.py
+-rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)     4702 2023-03-30 18:51:48.000000 mmap_ninja-0.6.4/mmap_ninja/string.py
+drwxrwxr-x   0 hvrigazov  (1000) hvrigazov  (1000)        0 2023-04-08 07:07:21.385689 mmap_ninja-0.6.4/mmap_ninja.egg-info/
+-rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)    11739 2023-04-08 07:07:21.000000 mmap_ninja-0.6.4/mmap_ninja.egg-info/PKG-INFO
+-rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)      461 2023-04-08 07:07:21.000000 mmap_ninja-0.6.4/mmap_ninja.egg-info/SOURCES.txt
+-rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)        1 2023-04-08 07:07:21.000000 mmap_ninja-0.6.4/mmap_ninja.egg-info/dependency_links.txt
+-rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)       11 2023-04-08 07:07:21.000000 mmap_ninja-0.6.4/mmap_ninja.egg-info/requires.txt
+-rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)       11 2023-04-08 07:07:21.000000 mmap_ninja-0.6.4/mmap_ninja.egg-info/top_level.txt
+-rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)       11 2022-09-09 05:58:58.000000 mmap_ninja-0.6.4/requirements.txt
+-rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)       38 2023-04-08 07:07:21.389689 mmap_ninja-0.6.4/setup.cfg
+-rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)     1325 2023-02-19 17:53:50.000000 mmap_ninja-0.6.4/setup.py
+drwxrwxr-x   0 hvrigazov  (1000) hvrigazov  (1000)        0 2023-04-08 07:07:21.389689 mmap_ninja-0.6.4/tests/
+-rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)     1141 2023-02-03 06:54:46.000000 mmap_ninja-0.6.4/tests/test_base.py
+-rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)      309 2023-02-03 07:45:29.000000 mmap_ninja-0.6.4/tests/test_generic.py
+-rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)     2517 2023-04-08 07:06:23.000000 mmap_ninja-0.6.4/tests/test_numpy.py
+-rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)     5828 2023-03-30 18:51:48.000000 mmap_ninja-0.6.4/tests/test_ragged.py
+-rw-rw-r--   0 hvrigazov  (1000) hvrigazov  (1000)     3240 2023-03-30 18:51:48.000000 mmap_ninja-0.6.4/tests/test_string.py
```

### Comparing `mmap_ninja-0.6.3/PKG-INFO` & `mmap_ninja-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmap_ninja
-Version: 0.6.3
+Version: 0.6.4
 Summary: mmap.ninja: Memory mapped data structures
 Home-page: https://github.com/hristo-vrigazov/mmap.ninja
 Author: Hristo Vrigazov
 Author-email: hvrigazov@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mmap_ninja-0.6.3/README.md` & `mmap_ninja-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `mmap_ninja-0.6.3/benchmark_images.py` & `mmap_ninja-0.6.4/benchmark_images.py`

 * *Files identical despite different names*

### Comparing `mmap_ninja-0.6.3/mmap_ninja/base.py` & `mmap_ninja-0.6.4/mmap_ninja/base.py`

 * *Files identical despite different names*

### Comparing `mmap_ninja-0.6.3/mmap_ninja/generic.py` & `mmap_ninja-0.6.4/mmap_ninja/generic.py`

 * *Files identical despite different names*

### Comparing `mmap_ninja-0.6.3/mmap_ninja/numpy.py` & `mmap_ninja-0.6.4/mmap_ninja/numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,22 +87,21 @@
     order = "F" if np.isfortran(arr) else "C"
     memmap = np.memmap(str(out_dir / "data.ninja"), mode="w+", dtype=dtype, shape=shape, order=order)
     memmap[:] = arr
     _save_mmap_kwargs(out_dir, dtype, shape, order)
     return memmap
 
 
-def from_generator(out_dir: Union[str, Path], sample_generator, batch_size: int, n: int, verbose=False) -> np.memmap:
+def from_generator(out_dir: Union[str, Path], sample_generator, batch_size: int, verbose=False) -> np.memmap:
     """
     Create a numpy memory-map from a sample generator.
 
     :param sample_generator: A generator of the samples
     :param out_dir: The output directory
     :param batch_size: How often to flush to disk
-    :param n: Total number of samples.
     :param verbose: Whether to show the progress bar.
     :return:
     """
     return from_generator_base(
         out_dir=out_dir,
         sample_generator=sample_generator,
         batch_size=batch_size,
```

### Comparing `mmap_ninja-0.6.3/mmap_ninja/ragged.py` & `mmap_ninja-0.6.4/mmap_ninja/ragged.py`

 * *Files identical despite different names*

### Comparing `mmap_ninja-0.6.3/mmap_ninja/string.py` & `mmap_ninja-0.6.4/mmap_ninja/string.py`

 * *Files identical despite different names*

### Comparing `mmap_ninja-0.6.3/mmap_ninja.egg-info/PKG-INFO` & `mmap_ninja-0.6.4/mmap_ninja.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmap-ninja
-Version: 0.6.3
+Version: 0.6.4
 Summary: mmap.ninja: Memory mapped data structures
 Home-page: https://github.com/hristo-vrigazov/mmap.ninja
 Author: Hristo Vrigazov
 Author-email: hvrigazov@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mmap_ninja-0.6.3/setup.py` & `mmap_ninja-0.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `mmap_ninja-0.6.3/tests/test_base.py` & `mmap_ninja-0.6.4/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `mmap_ninja-0.6.3/tests/test_numpy.py` & `mmap_ninja-0.6.4/tests/test_numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,27 +61,27 @@
 def simple_gen():
     for i in range(30):
         yield i
 
 
 def test_numpy_from_generator(tmp_path):
     memmap = np_ninja.from_generator(
-        out_dir=tmp_path / "generator", sample_generator=simple_gen(), n=30, batch_size=4, verbose=True
+        out_dir=tmp_path / "generator", sample_generator=simple_gen(), batch_size=4, verbose=True
     )
     memmap = np_ninja.open_existing(tmp_path / "generator")
     for i in range(30):
         assert i == memmap[i]
 
 
 def test_read_only(tmp_path):
-    out_path = tmp_path / 'read_only_numpy_memmap'
+    out_path = tmp_path / "read_only_numpy_memmap"
     arr = np.arange(10)
     np_ninja.from_ndarray(out_path, arr)
     # Make all memmap files read-only for the user
-    for p in out_path.glob(r'**/*'):
+    for p in out_path.glob(r"**/*"):
         if not p.is_file():
             continue
         os.chmod(p, stat.S_IRUSR)
     # Open in read-only mode
-    memmap = np_ninja.open_existing(out_path, mode='r')
+    memmap = np_ninja.open_existing(out_path, mode="r")
     for i, el in enumerate(arr):
         assert el == memmap[i]
```

### Comparing `mmap_ninja-0.6.3/tests/test_ragged.py` & `mmap_ninja-0.6.4/tests/test_ragged.py`

 * *Files identical despite different names*

### Comparing `mmap_ninja-0.6.3/tests/test_string.py` & `mmap_ninja-0.6.4/tests/test_string.py`

 * *Files identical despite different names*

