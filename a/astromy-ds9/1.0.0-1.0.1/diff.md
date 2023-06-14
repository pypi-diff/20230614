# Comparing `tmp/astromy_ds9-1.0.0.tar.gz` & `tmp/astromy_ds9-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astromy_ds9-1.0.0.tar", last modified: Wed Jun 14 14:49:48 2023, max compression
+gzip compressed data, was "astromy_ds9-1.0.1.tar", last modified: Wed Jun 14 14:54:26 2023, max compression
```

## Comparing `astromy_ds9-1.0.0.tar` & `astromy_ds9-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mingyu     (501) staff       (20)        0 2023-06-14 14:49:48.483215 astromy_ds9-1.0.0/
--rw-r--r--   0 mingyu     (501) staff       (20)     1049 2023-06-14 12:56:10.000000 astromy_ds9-1.0.0/LICENSE
--rw-r--r--   0 mingyu     (501) staff       (20)       26 2023-06-14 12:46:30.000000 astromy_ds9-1.0.0/MANIFEST.in
--rw-r--r--   0 mingyu     (501) staff       (20)     2752 2023-06-14 14:49:48.483034 astromy_ds9-1.0.0/PKG-INFO
--rw-r--r--   0 mingyu     (501) staff       (20)     2086 2023-06-14 14:47:48.000000 astromy_ds9-1.0.0/README.md
-drwxr-xr-x   0 mingyu     (501) staff       (20)        0 2023-06-14 14:49:48.482216 astromy_ds9-1.0.0/astromy_ds9/
--rw-r--r--   0 mingyu     (501) staff       (20)     5172 2023-06-14 14:06:35.000000 astromy_ds9-1.0.0/astromy_ds9/__init__.py
--rw-r--r--   0 mingyu     (501) staff       (20)      532 2023-06-14 14:48:08.000000 astromy_ds9-1.0.0/astromy_ds9/__version__.py
-drwxr-xr-x   0 mingyu     (501) staff       (20)        0 2023-06-14 14:49:48.482834 astromy_ds9-1.0.0/astromy_ds9.egg-info/
--rw-r--r--   0 mingyu     (501) staff       (20)     2752 2023-06-14 14:49:48.000000 astromy_ds9-1.0.0/astromy_ds9.egg-info/PKG-INFO
--rw-r--r--   0 mingyu     (501) staff       (20)      263 2023-06-14 14:49:48.000000 astromy_ds9-1.0.0/astromy_ds9.egg-info/SOURCES.txt
--rw-r--r--   0 mingyu     (501) staff       (20)        1 2023-06-14 14:49:48.000000 astromy_ds9-1.0.0/astromy_ds9.egg-info/dependency_links.txt
--rw-r--r--   0 mingyu     (501) staff       (20)       14 2023-06-14 14:49:48.000000 astromy_ds9-1.0.0/astromy_ds9.egg-info/requires.txt
--rw-r--r--   0 mingyu     (501) staff       (20)       12 2023-06-14 14:49:48.000000 astromy_ds9-1.0.0/astromy_ds9.egg-info/top_level.txt
--rw-r--r--   0 mingyu     (501) staff       (20)       38 2023-06-14 14:49:48.483260 astromy_ds9-1.0.0/setup.cfg
--rw-r--r--   0 mingyu     (501) staff       (20)     3831 2023-06-14 13:49:05.000000 astromy_ds9-1.0.0/setup.py
+drwxr-xr-x   0 mingyu     (501) staff       (20)        0 2023-06-14 14:54:26.910386 astromy_ds9-1.0.1/
+-rw-r--r--   0 mingyu     (501) staff       (20)     1049 2023-06-14 12:56:10.000000 astromy_ds9-1.0.1/LICENSE
+-rw-r--r--   0 mingyu     (501) staff       (20)       26 2023-06-14 12:46:30.000000 astromy_ds9-1.0.1/MANIFEST.in
+-rw-r--r--   0 mingyu     (501) staff       (20)     2783 2023-06-14 14:54:26.910203 astromy_ds9-1.0.1/PKG-INFO
+-rw-r--r--   0 mingyu     (501) staff       (20)     2117 2023-06-14 14:53:33.000000 astromy_ds9-1.0.1/README.md
+drwxr-xr-x   0 mingyu     (501) staff       (20)        0 2023-06-14 14:54:26.909010 astromy_ds9-1.0.1/astromy_ds9/
+-rw-r--r--   0 mingyu     (501) staff       (20)     5172 2023-06-14 14:06:35.000000 astromy_ds9-1.0.1/astromy_ds9/__init__.py
+-rw-r--r--   0 mingyu     (501) staff       (20)      532 2023-06-14 14:51:31.000000 astromy_ds9-1.0.1/astromy_ds9/__version__.py
+drwxr-xr-x   0 mingyu     (501) staff       (20)        0 2023-06-14 14:54:26.909991 astromy_ds9-1.0.1/astromy_ds9.egg-info/
+-rw-r--r--   0 mingyu     (501) staff       (20)     2783 2023-06-14 14:54:26.000000 astromy_ds9-1.0.1/astromy_ds9.egg-info/PKG-INFO
+-rw-r--r--   0 mingyu     (501) staff       (20)      263 2023-06-14 14:54:26.000000 astromy_ds9-1.0.1/astromy_ds9.egg-info/SOURCES.txt
+-rw-r--r--   0 mingyu     (501) staff       (20)        1 2023-06-14 14:54:26.000000 astromy_ds9-1.0.1/astromy_ds9.egg-info/dependency_links.txt
+-rw-r--r--   0 mingyu     (501) staff       (20)       14 2023-06-14 14:54:26.000000 astromy_ds9-1.0.1/astromy_ds9.egg-info/requires.txt
+-rw-r--r--   0 mingyu     (501) staff       (20)       12 2023-06-14 14:54:26.000000 astromy_ds9-1.0.1/astromy_ds9.egg-info/top_level.txt
+-rw-r--r--   0 mingyu     (501) staff       (20)       38 2023-06-14 14:54:26.910438 astromy_ds9-1.0.1/setup.cfg
+-rw-r--r--   0 mingyu     (501) staff       (20)     3831 2023-06-14 13:49:05.000000 astromy_ds9-1.0.1/setup.py
```

### Comparing `astromy_ds9-1.0.0/LICENSE` & `astromy_ds9-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `astromy_ds9-1.0.0/PKG-INFO` & `astromy_ds9-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astromy_ds9
-Version: 1.0.0
+Version: 1.0.1
 Summary: Reproducing SAOImageDS9 Colormap in Python
 Home-page: https://github.com/lmytime/Reproduce_DS9_colormap_in_Python
 Author: Mingyu Li
 Author-email: lmytime@hotmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -32,15 +32,15 @@
 ## Usage
 ```python
 from astromy_ds9 import ds9_norm
 
 
 import astropy
 import matplotlib.pyplot as plt
-data = astropy.io.fits.getdata('https://github.com/glue-viz/ds9norm/raw/master/m51.fits')
+data = astropy.io.fits.getdata('https://github.com/lmytime/Reproduce_DS9_colormap_in_Python/raw/main/doc/data/m51.fits')
 
 norm = ds9_norm(vmin=3053.38, vmax=13513.9, bias=0.581921, contrast=0.890152, stretch='sqrt')
 plt.imshow(data, norm=norm, cmap='gray', origin='lower', interpolation='None')
 ```
 
 There are 5 input parameters for `ds9_norm` function.
 - `vmin` and `vmax`: you can find the values in `Scale` -> `Scale Parameters` -> Below the histogram, Low is `vmin` and High is `vmax`.
```

### Comparing `astromy_ds9-1.0.0/README.md` & `astromy_ds9-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ## Usage
 ```python
 from astromy_ds9 import ds9_norm
 
 
 import astropy
 import matplotlib.pyplot as plt
-data = astropy.io.fits.getdata('https://github.com/glue-viz/ds9norm/raw/master/m51.fits')
+data = astropy.io.fits.getdata('https://github.com/lmytime/Reproduce_DS9_colormap_in_Python/raw/main/doc/data/m51.fits')
 
 norm = ds9_norm(vmin=3053.38, vmax=13513.9, bias=0.581921, contrast=0.890152, stretch='sqrt')
 plt.imshow(data, norm=norm, cmap='gray', origin='lower', interpolation='None')
 ```
 
 There are 5 input parameters for `ds9_norm` function.
 - `vmin` and `vmax`: you can find the values in `Scale` -> `Scale Parameters` -> Below the histogram, Low is `vmin` and High is `vmax`.
```

### Comparing `astromy_ds9-1.0.0/astromy_ds9/__init__.py` & `astromy_ds9-1.0.1/astromy_ds9/__init__.py`

 * *Files identical despite different names*

### Comparing `astromy_ds9-1.0.0/astromy_ds9/__version__.py` & `astromy_ds9-1.0.1/astromy_ds9/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,10 +11,10 @@
 @File    :   __version__.py
 @Time    :   2023/06/14
 @Author  :   Mingyu Li
 @Contact :   lmytime@hotmail.com
 '''
 
 
-VERSION = (1, 0, 0)
+VERSION = (1, 0, 1)
 
 __version__ = '.'.join(map(str, VERSION))
```

### Comparing `astromy_ds9-1.0.0/astromy_ds9.egg-info/PKG-INFO` & `astromy_ds9-1.0.1/astromy_ds9.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astromy-ds9
-Version: 1.0.0
+Version: 1.0.1
 Summary: Reproducing SAOImageDS9 Colormap in Python
 Home-page: https://github.com/lmytime/Reproduce_DS9_colormap_in_Python
 Author: Mingyu Li
 Author-email: lmytime@hotmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -32,15 +32,15 @@
 ## Usage
 ```python
 from astromy_ds9 import ds9_norm
 
 
 import astropy
 import matplotlib.pyplot as plt
-data = astropy.io.fits.getdata('https://github.com/glue-viz/ds9norm/raw/master/m51.fits')
+data = astropy.io.fits.getdata('https://github.com/lmytime/Reproduce_DS9_colormap_in_Python/raw/main/doc/data/m51.fits')
 
 norm = ds9_norm(vmin=3053.38, vmax=13513.9, bias=0.581921, contrast=0.890152, stretch='sqrt')
 plt.imshow(data, norm=norm, cmap='gray', origin='lower', interpolation='None')
 ```
 
 There are 5 input parameters for `ds9_norm` function.
 - `vmin` and `vmax`: you can find the values in `Scale` -> `Scale Parameters` -> Below the histogram, Low is `vmin` and High is `vmax`.
```

### Comparing `astromy_ds9-1.0.0/setup.py` & `astromy_ds9-1.0.1/setup.py`

 * *Files identical despite different names*

