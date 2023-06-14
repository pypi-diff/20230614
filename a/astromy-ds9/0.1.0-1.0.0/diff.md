# Comparing `tmp/astromy_ds9-0.1.0.tar.gz` & `tmp/astromy_ds9-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astromy_ds9-0.1.0.tar", last modified: Wed Jun 14 14:45:43 2023, max compression
+gzip compressed data, was "astromy_ds9-1.0.0.tar", last modified: Wed Jun 14 14:49:48 2023, max compression
```

## Comparing `astromy_ds9-0.1.0.tar` & `astromy_ds9-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mingyu     (501) staff       (20)        0 2023-06-14 14:45:43.234258 astromy_ds9-0.1.0/
--rw-r--r--   0 mingyu     (501) staff       (20)     1049 2023-06-14 12:56:10.000000 astromy_ds9-0.1.0/LICENSE
--rw-r--r--   0 mingyu     (501) staff       (20)       26 2023-06-14 12:46:30.000000 astromy_ds9-0.1.0/MANIFEST.in
--rw-r--r--   0 mingyu     (501) staff       (20)     2681 2023-06-14 14:45:43.234073 astromy_ds9-0.1.0/PKG-INFO
--rw-r--r--   0 mingyu     (501) staff       (20)     2015 2023-06-14 14:42:54.000000 astromy_ds9-0.1.0/README.md
-drwxr-xr-x   0 mingyu     (501) staff       (20)        0 2023-06-14 14:45:43.233081 astromy_ds9-0.1.0/astromy_ds9/
--rw-r--r--   0 mingyu     (501) staff       (20)     5172 2023-06-14 14:06:35.000000 astromy_ds9-0.1.0/astromy_ds9/__init__.py
--rw-r--r--   0 mingyu     (501) staff       (20)      532 2023-06-14 14:45:40.000000 astromy_ds9-0.1.0/astromy_ds9/__version__.py
-drwxr-xr-x   0 mingyu     (501) staff       (20)        0 2023-06-14 14:45:43.233853 astromy_ds9-0.1.0/astromy_ds9.egg-info/
--rw-r--r--   0 mingyu     (501) staff       (20)     2681 2023-06-14 14:45:43.000000 astromy_ds9-0.1.0/astromy_ds9.egg-info/PKG-INFO
--rw-r--r--   0 mingyu     (501) staff       (20)      263 2023-06-14 14:45:43.000000 astromy_ds9-0.1.0/astromy_ds9.egg-info/SOURCES.txt
--rw-r--r--   0 mingyu     (501) staff       (20)        1 2023-06-14 14:45:43.000000 astromy_ds9-0.1.0/astromy_ds9.egg-info/dependency_links.txt
--rw-r--r--   0 mingyu     (501) staff       (20)       14 2023-06-14 14:45:43.000000 astromy_ds9-0.1.0/astromy_ds9.egg-info/requires.txt
--rw-r--r--   0 mingyu     (501) staff       (20)       12 2023-06-14 14:45:43.000000 astromy_ds9-0.1.0/astromy_ds9.egg-info/top_level.txt
--rw-r--r--   0 mingyu     (501) staff       (20)       38 2023-06-14 14:45:43.234314 astromy_ds9-0.1.0/setup.cfg
--rw-r--r--   0 mingyu     (501) staff       (20)     3831 2023-06-14 13:49:05.000000 astromy_ds9-0.1.0/setup.py
+drwxr-xr-x   0 mingyu     (501) staff       (20)        0 2023-06-14 14:49:48.483215 astromy_ds9-1.0.0/
+-rw-r--r--   0 mingyu     (501) staff       (20)     1049 2023-06-14 12:56:10.000000 astromy_ds9-1.0.0/LICENSE
+-rw-r--r--   0 mingyu     (501) staff       (20)       26 2023-06-14 12:46:30.000000 astromy_ds9-1.0.0/MANIFEST.in
+-rw-r--r--   0 mingyu     (501) staff       (20)     2752 2023-06-14 14:49:48.483034 astromy_ds9-1.0.0/PKG-INFO
+-rw-r--r--   0 mingyu     (501) staff       (20)     2086 2023-06-14 14:47:48.000000 astromy_ds9-1.0.0/README.md
+drwxr-xr-x   0 mingyu     (501) staff       (20)        0 2023-06-14 14:49:48.482216 astromy_ds9-1.0.0/astromy_ds9/
+-rw-r--r--   0 mingyu     (501) staff       (20)     5172 2023-06-14 14:06:35.000000 astromy_ds9-1.0.0/astromy_ds9/__init__.py
+-rw-r--r--   0 mingyu     (501) staff       (20)      532 2023-06-14 14:48:08.000000 astromy_ds9-1.0.0/astromy_ds9/__version__.py
+drwxr-xr-x   0 mingyu     (501) staff       (20)        0 2023-06-14 14:49:48.482834 astromy_ds9-1.0.0/astromy_ds9.egg-info/
+-rw-r--r--   0 mingyu     (501) staff       (20)     2752 2023-06-14 14:49:48.000000 astromy_ds9-1.0.0/astromy_ds9.egg-info/PKG-INFO
+-rw-r--r--   0 mingyu     (501) staff       (20)      263 2023-06-14 14:49:48.000000 astromy_ds9-1.0.0/astromy_ds9.egg-info/SOURCES.txt
+-rw-r--r--   0 mingyu     (501) staff       (20)        1 2023-06-14 14:49:48.000000 astromy_ds9-1.0.0/astromy_ds9.egg-info/dependency_links.txt
+-rw-r--r--   0 mingyu     (501) staff       (20)       14 2023-06-14 14:49:48.000000 astromy_ds9-1.0.0/astromy_ds9.egg-info/requires.txt
+-rw-r--r--   0 mingyu     (501) staff       (20)       12 2023-06-14 14:49:48.000000 astromy_ds9-1.0.0/astromy_ds9.egg-info/top_level.txt
+-rw-r--r--   0 mingyu     (501) staff       (20)       38 2023-06-14 14:49:48.483260 astromy_ds9-1.0.0/setup.cfg
+-rw-r--r--   0 mingyu     (501) staff       (20)     3831 2023-06-14 13:49:05.000000 astromy_ds9-1.0.0/setup.py
```

### Comparing `astromy_ds9-0.1.0/LICENSE` & `astromy_ds9-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `astromy_ds9-0.1.0/PKG-INFO` & `astromy_ds9-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astromy_ds9
-Version: 0.1.0
+Version: 1.0.0
 Summary: Reproducing SAOImageDS9 Colormap in Python
 Home-page: https://github.com/lmytime/Reproduce_DS9_colormap_in_Python
 Author: Mingyu Li
 Author-email: lmytime@hotmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -22,20 +22,20 @@
 [SAOImageDS9](https://sites.google.com/cfa.harvard.edu/saoimageds9) is an image display and visualization tool for astronomical data, which can be used for fast image processing and inspection. In DS9, we can drag the mouse on the image viewer to manipulate the colormap and then visualize data effectively and quickly. Unlike the DS9, color normalization and stretch in Python should be set manually.
 
 Here we take notes about how to reproduce the colormap of DS9 in Python, supposing that you have already tuned the colormap parameters in DS9.
 
 
 ## Installation
 ```sh
-pip install ds9_norm
+pip install astromy_ds9
 ```
 
 ## Usage
 ```python
-from astromy_ds9 import ds9norm
+from astromy_ds9 import ds9_norm
 
 
 import astropy
 import matplotlib.pyplot as plt
 data = astropy.io.fits.getdata('https://github.com/glue-viz/ds9norm/raw/master/m51.fits')
 
 norm = ds9_norm(vmin=3053.38, vmax=13513.9, bias=0.581921, contrast=0.890152, stretch='sqrt')
@@ -43,15 +43,15 @@
 ```
 
 There are 5 input parameters for `ds9_norm` function.
 - `vmin` and `vmax`: you can find the values in `Scale` -> `Scale Parameters` -> Below the histogram, Low is `vmin` and High is `vmax`.
 - `bias` and `contrast`: you can find the values in `Color` -> `Color Parameters`
 - `stretch`: you can find it in `Scale` -> see which one is marked with a check mark. Allowed values are 'linear' | 'log' | 'sqrt' | 'power' | 'squared' | 'asinh' | 'sinh'.
 
-<img src="./doc/figs/help.png" alt="help" width=600/>
+<img src="https://github.com/lmytime/Reproduce_DS9_colormap_in_Python/blob/main/doc/figs/help.png?raw=true" alt="help"/>
 
 
 **Check example code in [test](https://nbviewer.org/github/lmytime/Reproduce_DS9_colormap_in_Python/blob/main/doc/test.ipynb) and [example](https://nbviewer.org/github/lmytime/Reproduce_DS9_colormap_in_Python/blob/main/doc/example.ipynb).**
 
 
 ## Methodology
 Please check the methodology in [`doc`](https://github.com/lmytime/Reproduce_DS9_colormap_in_Python/tree/main/doc). Also see [ds9norm](https://github.com/glue-viz/ds9norm) for reference.
```

### Comparing `astromy_ds9-0.1.0/README.md` & `astromy_ds9-1.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 [SAOImageDS9](https://sites.google.com/cfa.harvard.edu/saoimageds9) is an image display and visualization tool for astronomical data, which can be used for fast image processing and inspection. In DS9, we can drag the mouse on the image viewer to manipulate the colormap and then visualize data effectively and quickly. Unlike the DS9, color normalization and stretch in Python should be set manually.
 
 Here we take notes about how to reproduce the colormap of DS9 in Python, supposing that you have already tuned the colormap parameters in DS9.
 
 
 ## Installation
 ```sh
-pip install ds9_norm
+pip install astromy_ds9
 ```
 
 ## Usage
 ```python
-from astromy_ds9 import ds9norm
+from astromy_ds9 import ds9_norm
 
 
 import astropy
 import matplotlib.pyplot as plt
 data = astropy.io.fits.getdata('https://github.com/glue-viz/ds9norm/raw/master/m51.fits')
 
 norm = ds9_norm(vmin=3053.38, vmax=13513.9, bias=0.581921, contrast=0.890152, stretch='sqrt')
@@ -24,15 +24,15 @@
 ```
 
 There are 5 input parameters for `ds9_norm` function.
 - `vmin` and `vmax`: you can find the values in `Scale` -> `Scale Parameters` -> Below the histogram, Low is `vmin` and High is `vmax`.
 - `bias` and `contrast`: you can find the values in `Color` -> `Color Parameters`
 - `stretch`: you can find it in `Scale` -> see which one is marked with a check mark. Allowed values are 'linear' | 'log' | 'sqrt' | 'power' | 'squared' | 'asinh' | 'sinh'.
 
-<img src="./doc/figs/help.png" alt="help" width=600/>
+<img src="https://github.com/lmytime/Reproduce_DS9_colormap_in_Python/blob/main/doc/figs/help.png?raw=true" alt="help"/>
 
 
 **Check example code in [test](https://nbviewer.org/github/lmytime/Reproduce_DS9_colormap_in_Python/blob/main/doc/test.ipynb) and [example](https://nbviewer.org/github/lmytime/Reproduce_DS9_colormap_in_Python/blob/main/doc/example.ipynb).**
 
 
 ## Methodology
 Please check the methodology in [`doc`](https://github.com/lmytime/Reproduce_DS9_colormap_in_Python/tree/main/doc). Also see [ds9norm](https://github.com/glue-viz/ds9norm) for reference.
```

### Comparing `astromy_ds9-0.1.0/astromy_ds9/__init__.py` & `astromy_ds9-1.0.0/astromy_ds9/__init__.py`

 * *Files identical despite different names*

### Comparing `astromy_ds9-0.1.0/astromy_ds9/__version__.py` & `astromy_ds9-1.0.0/astromy_ds9/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,10 +11,10 @@
 @File    :   __version__.py
 @Time    :   2023/06/14
 @Author  :   Mingyu Li
 @Contact :   lmytime@hotmail.com
 '''
 
 
-VERSION = (0, 1, 0)
+VERSION = (1, 0, 0)
 
 __version__ = '.'.join(map(str, VERSION))
```

### Comparing `astromy_ds9-0.1.0/astromy_ds9.egg-info/PKG-INFO` & `astromy_ds9-1.0.0/astromy_ds9.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astromy-ds9
-Version: 0.1.0
+Version: 1.0.0
 Summary: Reproducing SAOImageDS9 Colormap in Python
 Home-page: https://github.com/lmytime/Reproduce_DS9_colormap_in_Python
 Author: Mingyu Li
 Author-email: lmytime@hotmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -22,20 +22,20 @@
 [SAOImageDS9](https://sites.google.com/cfa.harvard.edu/saoimageds9) is an image display and visualization tool for astronomical data, which can be used for fast image processing and inspection. In DS9, we can drag the mouse on the image viewer to manipulate the colormap and then visualize data effectively and quickly. Unlike the DS9, color normalization and stretch in Python should be set manually.
 
 Here we take notes about how to reproduce the colormap of DS9 in Python, supposing that you have already tuned the colormap parameters in DS9.
 
 
 ## Installation
 ```sh
-pip install ds9_norm
+pip install astromy_ds9
 ```
 
 ## Usage
 ```python
-from astromy_ds9 import ds9norm
+from astromy_ds9 import ds9_norm
 
 
 import astropy
 import matplotlib.pyplot as plt
 data = astropy.io.fits.getdata('https://github.com/glue-viz/ds9norm/raw/master/m51.fits')
 
 norm = ds9_norm(vmin=3053.38, vmax=13513.9, bias=0.581921, contrast=0.890152, stretch='sqrt')
@@ -43,15 +43,15 @@
 ```
 
 There are 5 input parameters for `ds9_norm` function.
 - `vmin` and `vmax`: you can find the values in `Scale` -> `Scale Parameters` -> Below the histogram, Low is `vmin` and High is `vmax`.
 - `bias` and `contrast`: you can find the values in `Color` -> `Color Parameters`
 - `stretch`: you can find it in `Scale` -> see which one is marked with a check mark. Allowed values are 'linear' | 'log' | 'sqrt' | 'power' | 'squared' | 'asinh' | 'sinh'.
 
-<img src="./doc/figs/help.png" alt="help" width=600/>
+<img src="https://github.com/lmytime/Reproduce_DS9_colormap_in_Python/blob/main/doc/figs/help.png?raw=true" alt="help"/>
 
 
 **Check example code in [test](https://nbviewer.org/github/lmytime/Reproduce_DS9_colormap_in_Python/blob/main/doc/test.ipynb) and [example](https://nbviewer.org/github/lmytime/Reproduce_DS9_colormap_in_Python/blob/main/doc/example.ipynb).**
 
 
 ## Methodology
 Please check the methodology in [`doc`](https://github.com/lmytime/Reproduce_DS9_colormap_in_Python/tree/main/doc). Also see [ds9norm](https://github.com/glue-viz/ds9norm) for reference.
```

### Comparing `astromy_ds9-0.1.0/setup.py` & `astromy_ds9-1.0.0/setup.py`

 * *Files identical despite different names*

