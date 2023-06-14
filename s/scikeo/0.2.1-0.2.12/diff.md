# Comparing `tmp/scikeo-0.2.1.tar.gz` & `tmp/scikeo-0.2.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikeo-0.2.1.tar", last modified: Thu Apr 27 17:06:07 2023, max compression
+gzip compressed data, was "dist\scikeo-0.2.12.tar", last modified: Wed Jun 14 15:31:54 2023, max compression
```

## Comparing `scikeo-0.2.1.tar` & `scikeo-0.2.12.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 17:06:07.375306 scikeo-0.2.1/
--rw-rw-rw-   0        0        0      613 2023-03-17 15:59:10.000000 scikeo-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      130 2023-03-17 15:59:10.000000 scikeo-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     8976 2023-04-27 17:06:07.375306 scikeo-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     8013 2023-03-31 15:29:00.000000 scikeo-0.2.1/README.md
--rw-rw-rw-   0        0        0       62 2023-03-17 15:59:10.000000 scikeo-0.2.1/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-04-27 17:06:07.340357 scikeo-0.2.1/scikeo/
--rw-rw-rw-   0        0        0      143 2023-03-17 15:59:10.000000 scikeo-0.2.1/scikeo/__init__.py
--rw-rw-rw-   0        0        0    10900 2023-03-17 15:59:10.000000 scikeo-0.2.1/scikeo/atmosCorr.py
--rw-rw-rw-   0        0        0     5794 2023-03-17 15:59:10.000000 scikeo-0.2.1/scikeo/calkmeans.py
--rw-rw-rw-   0        0        0    19966 2023-03-17 15:59:10.000000 scikeo-0.2.1/scikeo/calmla.py
--rw-rw-rw-   0        0        0     9131 2023-03-17 15:59:10.000000 scikeo-0.2.1/scikeo/deeplearning.py
--rw-rw-rw-   0        0        0     6113 2023-03-17 15:59:10.000000 scikeo-0.2.1/scikeo/fusionrs.py
--rw-rw-rw-   0        0        0     6668 2023-03-17 15:59:10.000000 scikeo-0.2.1/scikeo/linearTrend.py
--rw-rw-rw-   0        0        0    25713 2023-03-23 01:18:16.000000 scikeo-0.2.1/scikeo/mla.py
--rw-rw-rw-   0        0        0     5043 2023-03-17 15:59:10.000000 scikeo-0.2.1/scikeo/pca.py
--rw-rw-rw-   0        0        0     5789 2023-03-17 15:59:10.000000 scikeo-0.2.1/scikeo/plot.py
--rw-rw-rw-   0        0        0    10277 2023-04-27 16:42:51.000000 scikeo-0.2.1/scikeo/process.py
--rw-rw-rw-   0        0        0     1871 2023-03-17 15:59:10.000000 scikeo-0.2.1/scikeo/rkmeans.py
--rw-rw-rw-   0        0        0     3819 2023-03-17 15:59:10.000000 scikeo-0.2.1/scikeo/sma.py
--rw-rw-rw-   0        0        0     5235 2023-03-17 15:59:10.000000 scikeo-0.2.1/scikeo/tassCap.py
--rw-rw-rw-   0        0        0     2068 2023-03-17 15:59:10.000000 scikeo-0.2.1/scikeo/writeRaster.py
-drwxrwxrwx   0        0        0        0 2023-04-27 17:06:07.373241 scikeo-0.2.1/scikeo.egg-info/
--rw-rw-rw-   0        0        0     8976 2023-04-27 17:06:06.000000 scikeo-0.2.1/scikeo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      516 2023-04-27 17:06:07.000000 scikeo-0.2.1/scikeo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       56 2023-04-27 17:06:06.000000 scikeo-0.2.1/scikeo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-20 19:51:08.000000 scikeo-0.2.1/scikeo.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       55 2023-04-27 17:06:06.000000 scikeo-0.2.1/scikeo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-27 17:06:06.000000 scikeo-0.2.1/scikeo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      414 2023-04-27 17:06:07.375306 scikeo-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1755 2023-04-27 16:59:24.000000 scikeo-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 15:31:54.413975 scikeo-0.2.12/
+-rw-rw-rw-   0        0        0      613 2023-03-17 15:59:10.000000 scikeo-0.2.12/LICENSE
+-rw-rw-rw-   0        0        0      130 2023-03-17 15:59:10.000000 scikeo-0.2.12/MANIFEST.in
+-rw-rw-rw-   0        0        0    10319 2023-06-14 15:31:54.413975 scikeo-0.2.12/PKG-INFO
+-rw-rw-rw-   0        0        0     7948 2023-06-12 14:56:27.000000 scikeo-0.2.12/README.md
+-rw-rw-rw-   0        0        0       62 2023-03-17 15:59:10.000000 scikeo-0.2.12/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 15:31:54.283352 scikeo-0.2.12/scikeo/
+-rw-rw-rw-   0        0        0      143 2023-03-17 15:59:10.000000 scikeo-0.2.12/scikeo/__init__.py
+-rw-rw-rw-   0        0        0    10900 2023-03-17 15:59:10.000000 scikeo-0.2.12/scikeo/atmosCorr.py
+-rw-rw-rw-   0        0        0     5794 2023-03-17 15:59:10.000000 scikeo-0.2.12/scikeo/calkmeans.py
+-rw-rw-rw-   0        0        0    19966 2023-03-17 15:59:10.000000 scikeo-0.2.12/scikeo/calmla.py
+-rw-rw-rw-   0        0        0     9681 2023-06-14 15:27:15.000000 scikeo-0.2.12/scikeo/deeplearning.py
+-rw-rw-rw-   0        0        0     6113 2023-03-17 15:59:10.000000 scikeo-0.2.12/scikeo/fusionrs.py
+-rw-rw-rw-   0        0        0     6668 2023-03-17 15:59:10.000000 scikeo-0.2.12/scikeo/linearTrend.py
+-rw-rw-rw-   0        0        0    25713 2023-06-14 15:21:56.000000 scikeo-0.2.12/scikeo/mla.py
+-rw-rw-rw-   0        0        0     5043 2023-03-17 15:59:10.000000 scikeo-0.2.12/scikeo/pca.py
+-rw-rw-rw-   0        0        0     5789 2023-03-17 15:59:10.000000 scikeo-0.2.12/scikeo/plot.py
+-rw-rw-rw-   0        0        0    10277 2023-04-27 16:42:51.000000 scikeo-0.2.12/scikeo/process.py
+-rw-rw-rw-   0        0        0     1871 2023-03-17 15:59:10.000000 scikeo-0.2.12/scikeo/rkmeans.py
+-rw-rw-rw-   0        0        0     3721 2023-06-14 15:28:55.000000 scikeo-0.2.12/scikeo/sma.py
+-rw-rw-rw-   0        0        0     5235 2023-03-17 15:59:10.000000 scikeo-0.2.12/scikeo/tassCap.py
+-rw-rw-rw-   0        0        0     2068 2023-03-17 15:59:10.000000 scikeo-0.2.12/scikeo/writeRaster.py
+drwxrwxrwx   0        0        0        0 2023-06-14 15:31:54.411980 scikeo-0.2.12/scikeo.egg-info/
+-rw-rw-rw-   0        0        0    10319 2023-06-14 15:31:49.000000 scikeo-0.2.12/scikeo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      516 2023-06-14 15:31:49.000000 scikeo-0.2.12/scikeo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       56 2023-06-14 15:31:49.000000 scikeo-0.2.12/scikeo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-20 19:51:08.000000 scikeo-0.2.12/scikeo.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       55 2023-06-14 15:31:49.000000 scikeo-0.2.12/scikeo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-14 15:31:49.000000 scikeo-0.2.12/scikeo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      414 2023-06-14 15:31:54.416966 scikeo-0.2.12/setup.cfg
+-rw-rw-rw-   0        0        0     1756 2023-06-14 15:31:13.000000 scikeo-0.2.12/setup.py
```

### Comparing `scikeo-0.2.1/LICENSE` & `scikeo-0.2.12/LICENSE`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.1/PKG-INFO` & `scikeo-0.2.12/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,34 @@
-Metadata-Version: 2.1
-Name: scikeo
-Version: 0.2.1
-Summary: Remote Sensing Tools
-Home-page: https://github.com/ytarazona/scikit-eo
-Author: Yonatan Tarazona Coronel
-Author-email: geoyons@gmail.com
-License: Apache Software License 2.0
-Keywords: scikeo
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <!-- #region -->
-# scikit-eo: A Python package for Remote Sensing Tools
+# scikit-eo: A Python package for Remote Sensing Data Analysis
 
 [![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)]()
 [![License: MIT](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![PythonVersion]( https://img.shields.io/badge/python-3.5%20%7C%203.6%20%7C%203.7%20%7C%203.8-green)]()
 [![PyPI version](https://badge.fury.io/py/scikeo.svg)](https://badge.fury.io/py/scikeo)
-[![Youtube](https://img.shields.io/badge/YouTube-Channel-red)]()     
-[![Twitter](https://img.shields.io/twitter/url?label=Follow%20%40GeoYons&style=social&url=https%3A%2F%2Ftwitter.com%2FGeoYons)](https://twitter.com/GeoYons)
+[![Youtube](https://img.shields.io/badge/YouTube-Channel-red)]()
 [![Downloads](https://pepy.tech/badge/scikeo)](https://pepy.tech/project/scikeo)
 [![Downloads](https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/docs-passing-brightgreen.svg)]()
 
 <img src="https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/scikit-eo_logo.jpg" align="right" width="220"/>
 
 
 <!-- #region -->
 # Introduction
 
-Nowadays, remotely sensed data has increased dramatically. Microwaves and optical images with different spatial and temporal resolutions are available and are using to monitor a variaty of environmental issues such as deforestation, land degradation, crop classifications, among other. Although there are efforts (i.e., Python packages, forums, communities, etc.) to make available line-of-code tools for pre-processing, processing and analysis of satellite imagery, there is still a gap that needs to be filled. In other words, too much time is still spent by many users in developing Python lines of code. Algorithms for mapping land degradation through linear trend of vegetation indices, fusion optical and radar images to classify vegetation cover, calibration of machine learning lagorithms, among others, are not available yet.
+Nowadays, remotely sensed data has increased dramatically. Microwaves and optical images with different spatial and temporal resolutions are available and are used to monitor a variety of environmental issues such as deforestation, land degradation, land use and land cover change, among others. Although there are efforts (i.e., Python packages, forums, communities, etc.) to make available line-of-code tools for pre-processing, processing and analysis of satellite imagery, there is still a gap that needs to be filled. In other words, too much time is still spent by many users developing Python lines of code. Algorithms for mapping land degradation through a linear trend of vegetation indices, fusion optical and radar images to classify vegetation cover, and calibration of machine learning algorithms, among others, are not available yet.
 
 Therefore, **scikit-eo** is a Python package that provides tools for remote sensing. This package was developed to fill the gaps in remotely sensed data processing tools. Most of the tools are based on scientific publications, and others are useful algorithms that will allow processing to be done in a few lines of code. With these tools, the user will be able to invest time in analyzing the results of their data and not spend time on elaborating lines of code, which can sometimes be stressful.
 
 # Tools for Remote Sensing
 
 | Name of functions  | Description|
 | -------------------| --------------------------------------------------------------------------|
-| **`mla`**          | Machine Learning                                                          |
-| **`calmla`**       | Calibrating supervised classification in Remote Sensing                   |
+| **`mla`**          | Machine Learning (Random Forest, Support Vector Machine, Decition Tree, Naive Bayes, Neural Network, etc.)                                                          |
+| **`calmla`**       | Calibrating supervised classification in Remote Sensing (e.g., Monte Carlo Cross-Validation, Leave-One-Out Cross-Validation, etc.)                   |
 | **`confintervalML`**       | Information of confusion matrix by proportions of area, overall accuracy, user's accuracy with confidence interval and estimated area with confidence interval as well.                                    |
 | **`rkmeans`**      | K-means classification                                                    |
 | **`calkmeans`**    | This function allows to calibrate the kmeans algorithm. It is possible to obtain the best k value and the best embedded algorithm in kmeans.                               |
 | **`pca`**          | Principal Components Analysis                                             |
 | **`atmosCorr`**    | Atmospheric Correction of satellite imagery                               |
 | **`deepLearning`** | Deep Learning algorithms                                                  |
 | **`linearTrend`**  | Linear trend is useful for mapping forest degradation or land degradation |
@@ -80,15 +58,15 @@
 ```python
 pip install git+https://github.com/ytarazona/scikit-eo
 ```
 <!-- #endregion -->
 
 # Example
 
-## 1. Applying Machine Learning
+## 1.0 Applying Machine Learning
 
 Libraries to be used:
 
 ```python
 import rasterio
 import numpy as np
 from scikeo.mla import MLA
@@ -185,15 +163,15 @@
 # Let's define the color palette
 palette = mpl.colors.ListedColormap(["#2232F9","#F922AE","#229954","#7CED5E"])
 ```
 
 Applying the ```plotRGB()``` algorithm is easy:
 
 ```python
-# LetÂ´s plot
+# Let´s plot
 fig, axes = plt.subplots(nrows = 1, ncols = 2, figsize = (15, 9))
 
 # satellite image
 plotRGB(img, title = 'Image in Surface Reflectance', ax = axes[0])
 
 # class results
 axes[1].imshow(svm_class.get('Classification_Map'), cmap = palette)
@@ -213,15 +191,11 @@
 ## Acknowledgment
 
 Special thanks to:
 - [David Montero Loaiza](https://github.com/davemlz) for the idea of the package name **scikit-eo**.
 
 - [Qiusheng Wu](https://github.com/giswqs) for the suggestions that helped to improve the package.
 
-## Dedication and inspiration
-
-Yonatan Tarazona dedicates this package to [MarÃ­a Griselda Miyasiro LÃ³pez](https://github.com/geolomera), the person who inspired to develop it. In fact, the logo of the package is inspired by fog oasis known as "Lomas", an ecosystem that she loves deeply.
-
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter)
 <!-- #endregion -->
```

### Comparing `scikeo-0.2.1/scikeo/atmosCorr.py` & `scikeo-0.2.12/scikeo/atmosCorr.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.1/scikeo/calkmeans.py` & `scikeo-0.2.12/scikeo/calkmeans.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.1/scikeo/calmla.py` & `scikeo-0.2.12/scikeo/calmla.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.1/scikeo/fusionrs.py` & `scikeo-0.2.12/scikeo/fusionrs.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.1/scikeo/linearTrend.py` & `scikeo-0.2.12/scikeo/linearTrend.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.1/scikeo/mla.py` & `scikeo-0.2.12/scikeo/mla.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.1/scikeo/pca.py` & `scikeo-0.2.12/scikeo/pca.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.1/scikeo/plot.py` & `scikeo-0.2.12/scikeo/plot.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.1/scikeo/process.py` & `scikeo-0.2.12/scikeo/process.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.1/scikeo/rkmeans.py` & `scikeo-0.2.12/scikeo/rkmeans.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.1/scikeo/sma.py` & `scikeo-0.2.12/scikeo/sma.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,98 +1,98 @@
-# +
-import rasterio
-import numpy as np
-
-def sma(image, endmembers, nodata = -99999):
-    
-    '''
-    The SMA assumes that the energy received within the field of vision of the remote sensor 
-    can be considered as the sum of the energies received from each dominant endmember. 
-    This function addresses a Linear Mixing Model.
-    
-    A regression analysis is used to obtain the fractions. In least squares inversion algorithms, 
-    the common objective is to estimate abundances that minimize the squared error between the 
-    actual spectrum and the estimated spectrum. The values of the fractions will be between 0 and 1.
-    
-    Parameters:
-    
-        image: Optical images. It must be rasterio.io.DatasetReader with 3d.
-        
-        endmembers: Endmembers must be a matrix (numpy.ndarray) and with more than one endmember. 
-                    Rows represent the endmembers and columns represent the spectral bands.
-                    The number of bands must be greater than the number of endmembers.
-                    E.g. an image with 6 bands, endmembers dimension should be $n*6$, where $n$ 
-                    is rows with the number of endmembers and 6 is the number of bands 
-                    (should be equal).
-                    
-        nodata: The NoData value to replace with -99999.
-    
-    Return:
-    
-        numpy.ndarray with 2d.
-        
-    References
-    Adams, J. B., Smith, M. O., & Gillespie, A. R. (1993). Imaging spectroscopy:
-    Interpretation based on spectral mixture analysis. In C. M. Pieters & P.
-    Englert (Eds.), Remote geochemical analysis: Elements and mineralogical
-    composition. NY: Cambridge Univ. Press 145-166 pp.
-    
-    Shimabukuro, Y.E. and Smith, J., (1991). The least squares mixing models to
-    generate fraction images derived from remote sensing multispectral data.
-    IEEE Transactions on Geoscience and Remote Sensing, 29, pp. 16-21.
-    
-    Note:
-    A regression analysis is used to obtain the fractions. In least squares
-    inversion algorithms, the common objective is to estimate abundances that
-    minimize the squared error between the actual spectrum and the estimated spectrum.
-    The values of the fractions will be between 0 and 1.
-    '''
-    
-    if not isinstance(image, (rasterio.io.DatasetReader)):
-        raise TypeError('"image" must be raster read by rasterio.open().')
-        
-    if not isinstance (endmembers, (np.ndarray)):
-        raise ErrorType('"endmembers" must be numpy.ndarray.')
-    
-    bands = image.count
-        
-    rows = image.height
-        
-    cols = image.width
-    
-    # number of endmembers
-    n_endm = endmembers.shape[0]
-    
-    # number of bands extracted for each endmember
-    b_endm = endmembers.shape[1]
-        
-    st = image.read()
-        
-    # data in [rows, cols, bands]
-    st_reorder = np.moveaxis(st, 0, -1) 
-    # data in [rows*cols, bands]
-    arr = st_reorder.reshape((rows*cols, bands))
-    
-    # nodata
-    if np.isnan(np.sum(arr)):
-        arr[np.isnan(arr)] = self.nodata
-    
-    if not arr.shape[1] > n_endm:
-        raise ValueError('The number of bands must be greater than the number of endmembers.')
-    
-    if not arr.shape[1] == b_endm:
-        raise ValueError('The number of values extracted in band should be equal.')
-    
-    M = np.transpose(endmembers)
-    
-    mat_oper = np.dot(np.linalg.inv(np.dot(np.transpose(M), M)), np.transpose(M)) 
-    
-    frac = np.zeros((rows*cols, n_endm))
-                
-    for i in np.arange(0, n_endm, 1):
-        for j in np.arange(0, rows*cols, 1):
-            f = np.dot(mat_oper, arr[j,:])
-            frac[j,i] = f[i,]
-    
-    sma_img = frac.reshape((rows, cols, n_endm))
-    
-    return sma_img
+# +
+import rasterio
+import numpy as np
+
+def sma(image, endmembers, nodata = -99999):
+    
+    '''
+    The SMA assumes that the energy received within the field of vision of the remote sensor 
+    can be considered as the sum of the energies received from each dominant endmember. 
+    This function addresses a Linear Mixing Model.
+    
+    A regression analysis is used to obtain the fractions. In least squares inversion algorithms, 
+    the common objective is to estimate abundances that minimize the squared error between the 
+    actual spectrum and the estimated spectrum. The values of the fractions will be between 0 and 1.
+    
+    Parameters:
+    
+        image: Optical images. It must be rasterio.io.DatasetReader with 3d.
+        
+        endmembers: Endmembers must be a matrix (numpy.ndarray) and with more than one endmember. 
+                    Rows represent the endmembers and columns represent the spectral bands.
+                    The number of bands must be greater than the number of endmembers.
+                    E.g. an image with 6 bands, endmembers dimension should be $n*6$, where $n$ 
+                    is rows with the number of endmembers and 6 is the number of bands 
+                    (should be equal).
+                    
+        nodata: The NoData value to replace with -99999.
+    
+    Return:
+    
+        numpy.ndarray with 2d.
+        
+    References
+    Adams, J. B., Smith, M. O., & Gillespie, A. R. (1993). Imaging spectroscopy:
+    Interpretation based on spectral mixture analysis. In C. M. Pieters & P.
+    Englert (Eds.), Remote geochemical analysis: Elements and mineralogical
+    composition. NY: Cambridge Univ. Press 145-166 pp.
+    
+    Shimabukuro, Y.E. and Smith, J., (1991). The least squares mixing models to
+    generate fraction images derived from remote sensing multispectral data.
+    IEEE Transactions on Geoscience and Remote Sensing, 29, pp. 16-21.
+    
+    Note:
+    A regression analysis is used to obtain the fractions. In least squares
+    inversion algorithms, the common objective is to estimate abundances that
+    minimize the squared error between the actual spectrum and the estimated spectrum.
+    The values of the fractions will be between 0 and 1.
+    '''
+    
+    if not isinstance(image, (rasterio.io.DatasetReader)):
+        raise TypeError('"image" must be raster read by rasterio.open().')
+        
+    if not isinstance (endmembers, (np.ndarray)):
+        raise ErrorType('"endmembers" must be numpy.ndarray.')
+    
+    bands = image.count
+        
+    rows = image.height
+        
+    cols = image.width
+    
+    # number of endmembers
+    n_endm = endmembers.shape[0]
+    
+    # number of bands extracted for each endmember
+    b_endm = endmembers.shape[1]
+        
+    st = image.read()
+        
+    # data in [rows, cols, bands]
+    st_reorder = np.moveaxis(st, 0, -1) 
+    # data in [rows*cols, bands]
+    arr = st_reorder.reshape((rows*cols, bands))
+    
+    # nodata
+    if np.isnan(np.sum(arr)):
+        arr[np.isnan(arr)] = self.nodata
+    
+    if not arr.shape[1] > n_endm:
+        raise ValueError('The number of bands must be greater than the number of endmembers.')
+    
+    if not arr.shape[1] == b_endm:
+        raise ValueError('The number of values extracted in band should be equal.')
+    
+    M = np.transpose(endmembers)
+    
+    mat_oper = np.dot(np.linalg.inv(np.dot(np.transpose(M), M)), np.transpose(M)) 
+    
+    frac = np.zeros((rows*cols, n_endm))
+                
+    for i in np.arange(0, n_endm, 1):
+        for j in np.arange(0, rows*cols, 1):
+            f = np.dot(mat_oper, arr[j,:])
+            frac[j,i] = f[i,]
+    
+    sma_img = frac.reshape((rows, cols, n_endm))
+    
+    return sma_img
```

### Comparing `scikeo-0.2.1/scikeo/tassCap.py` & `scikeo-0.2.12/scikeo/tassCap.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.1/scikeo/writeRaster.py` & `scikeo-0.2.12/scikeo/writeRaster.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.1/scikeo.egg-info/PKG-INFO` & `scikeo-0.2.12/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,227 +1,222 @@
 Metadata-Version: 2.1
 Name: scikeo
-Version: 0.2.1
+Version: 0.2.12
 Summary: Remote Sensing Tools
 Home-page: https://github.com/ytarazona/scikit-eo
 Author: Yonatan Tarazona Coronel
 Author-email: geoyons@gmail.com
 License: Apache Software License 2.0
+Description: <!-- #region -->
+        # scikit-eo: A Python package for Remote Sensing Data Analysis
+        
+        [![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)]()
+        [![License: MIT](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+        [![PythonVersion]( https://img.shields.io/badge/python-3.5%20%7C%203.6%20%7C%203.7%20%7C%203.8-green)]()
+        [![PyPI version](https://badge.fury.io/py/scikeo.svg)](https://badge.fury.io/py/scikeo)
+        [![Youtube](https://img.shields.io/badge/YouTube-Channel-red)]()
+        [![Downloads](https://pepy.tech/badge/scikeo)](https://pepy.tech/project/scikeo)
+        [![Downloads](https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/docs-passing-brightgreen.svg)]()
+        
+        <img src="https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/scikit-eo_logo.jpg" align="right" width="220"/>
+        
+        
+        <!-- #region -->
+        # Introduction
+        
+        Nowadays, remotely sensed data has increased dramatically. Microwaves and optical images with different spatial and temporal resolutions are available and are used to monitor a variety of environmental issues such as deforestation, land degradation, land use and land cover change, among others. Although there are efforts (i.e., Python packages, forums, communities, etc.) to make available line-of-code tools for pre-processing, processing and analysis of satellite imagery, there is still a gap that needs to be filled. In other words, too much time is still spent by many users developing Python lines of code. Algorithms for mapping land degradation through a linear trend of vegetation indices, fusion optical and radar images to classify vegetation cover, and calibration of machine learning algorithms, among others, are not available yet.
+        
+        Therefore, **scikit-eo** is a Python package that provides tools for remote sensing. This package was developed to fill the gaps in remotely sensed data processing tools. Most of the tools are based on scientific publications, and others are useful algorithms that will allow processing to be done in a few lines of code. With these tools, the user will be able to invest time in analyzing the results of their data and not spend time on elaborating lines of code, which can sometimes be stressful.
+        
+        # Tools for Remote Sensing
+        
+        | Name of functions  | Description|
+        | -------------------| --------------------------------------------------------------------------|
+        | **`mla`**          | Machine Learning (Random Forest, Support Vector Machine, Decition Tree, Naive Bayes, Neural Network, etc.)                                                          |
+        | **`calmla`**       | Calibrating supervised classification in Remote Sensing (e.g., Monte Carlo Cross-Validation, Leave-One-Out Cross-Validation, etc.)                   |
+        | **`confintervalML`**       | Information of confusion matrix by proportions of area, overall accuracy, user's accuracy with confidence interval and estimated area with confidence interval as well.                                    |
+        | **`rkmeans`**      | K-means classification                                                    |
+        | **`calkmeans`**    | This function allows to calibrate the kmeans algorithm. It is possible to obtain the best k value and the best embedded algorithm in kmeans.                               |
+        | **`pca`**          | Principal Components Analysis                                             |
+        | **`atmosCorr`**    | Atmospheric Correction of satellite imagery                               |
+        | **`deepLearning`** | Deep Learning algorithms                                                  |
+        | **`linearTrend`**  | Linear trend is useful for mapping forest degradation or land degradation |
+        | **`fusionrs`**     | This algorithm allows to fusion images coming from different spectral sensors (e.g., optical-optical, optical and SAR or SAR-SAR). Among many of the qualities of this function, it is possible to obtain the contribution (%) of each variable in the fused image |
+        | **`sma`**          | Spectral Mixture Analysis - Classification sup-pixel                      |
+        | **`tassCap`**      | The Tasseled-Cap Transformation                                           |
+        
+        You will find more algorithms!.
+        
+        
+        # Installation
+        
+        To use **scikit-eo** it is necessary to install it. There are two options:
+        
+        ## 1. From PyPI
+        
+        **scikit-eo** is available on [PyPI](https://pypi.org/project/scikeo/), so to install it, run this command in your terminal:
+        
+        ```python
+        pip install scikeo
+        ```
+        
+        ## 2. Installing from source
+        
+        It is also possible to install the latest development version directly from the GitHub repository with:
+        
+        ```python
+        pip install git+https://github.com/ytarazona/scikit-eo
+        ```
+        <!-- #endregion -->
+        
+        # Example
+        
+        ## 1.0 Applying Machine Learning
+        
+        Libraries to be used:
+        
+        ```python
+        import rasterio
+        import numpy as np
+        from scikeo.mla import MLA
+        import matplotlib.pyplot as plt
+        from dbfread import DBF
+        import matplotlib as mpl
+        import pandas as pd
+        ```
+        
+        ## 2.0 Optical image
+        
+        
+        Landsat-8 OLI (Operational Land Imager) will be used to obtain in order to classify using Random Forest (RF). This image, which is in surface reflectance with bands:
+        - Blue -> B2
+        - Green -> B3 
+        - Red -> B4
+        - Nir -> B5
+        - Swir1 -> B6
+        - Swir2 -> B7
+        
+        The image and signatures to be used can be downloaded [here](https://drive.google.com/drive/folders/193RhNpACu9THcOZu8OzMh-btnFCOgHrU?usp=sharing):
+        
+        
+        ## 3.0 Supervised Classification using Random Forest
+        
+        Image and endmembers
+        
+        ```python
+        path_raster = r"C:\data\ml\LC08_232066_20190727_SR.tif"
+        img = rasterio.open(path_raster)
+        
+        path_endm = r"C:\data\ml\endmembers.dbf"
+        endm = DBF(path_endm)
+        ```
+        
+        ```python
+        # endmembers
+        df = pd.DataFrame(iter(endm))
+        df.head()
+        ```
+        <p align="left">
+          <a href="https://github.com/ytarazona/scikit-eo"><img src="https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/endembers.png" alt ="header" width = 75%>
+        </a>
+        </p>
+        
+        
+        Instance of ```mla()```:
+        
+        ```python
+        inst = MLA(image = img, endmembers = endm)
+        ```
+        
+        Applying Random Forest:
+        
+        ```python
+        svm_class = inst.SVM(training_split = 0.7)
+        ```
+        
+        ## 4.0 Results
+        
+        Dictionary of results
+        
+        ```python
+        svm_class.keys()
+        ```
+        
+        Overall accuracy
+        
+        ```python
+        svm_class.get('Overall_Accuracy')
+        ```
+        
+        Kappa index
+        
+        ```python
+        svm_class.get('Kappa_Index')
+        ```
+        
+        Confusion matrix or error matrix
+        
+        ```python
+        svm_class.get('Confusion_Matrix')
+        ```
+        
+        <p align="left">
+          <a href="https://github.com/ytarazona/scikit-eo"><img src="https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/confusion_matrix.png" alt ="header" width = 80%>
+        </a>
+        </p>
+        
+        
+        Preparing the image before plotting
+        
+        ```python
+        # Let's define the color palette
+        palette = mpl.colors.ListedColormap(["#2232F9","#F922AE","#229954","#7CED5E"])
+        ```
+        
+        Applying the ```plotRGB()``` algorithm is easy:
+        
+        ```python
+        # LetÂ´s plot
+        fig, axes = plt.subplots(nrows = 1, ncols = 2, figsize = (15, 9))
+        
+        # satellite image
+        plotRGB(img, title = 'Image in Surface Reflectance', ax = axes[0])
+        
+        # class results
+        axes[1].imshow(svm_class.get('Classification_Map'), cmap = palette)
+        axes[1].set_title("Classification map")
+        axes[1].grid(False)
+        ```
+        
+        <p align="left">
+          <a href="https://github.com/ytarazona/scikit-eo"><img src="https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/classification.png" alt ="header" width = "750">
+        </a>
+        </p>
+        
+        <!-- #region -->
+        -   Free software: Apache Software License 2.0
+        -   Documentation: 
+        
+        ## Acknowledgment
+        
+        Special thanks to:
+        - [David Montero Loaiza](https://github.com/davemlz) for the idea of the package name **scikit-eo**.
+        
+        - [Qiusheng Wu](https://github.com/giswqs) for the suggestions that helped to improve the package.
+        
+        ## Credits
+        
+        This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter)
+        <!-- #endregion -->
+        
 Keywords: scikeo
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<!-- #region -->
-# scikit-eo: A Python package for Remote Sensing Tools
-
-[![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)]()
-[![License: MIT](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-[![PythonVersion]( https://img.shields.io/badge/python-3.5%20%7C%203.6%20%7C%203.7%20%7C%203.8-green)]()
-[![PyPI version](https://badge.fury.io/py/scikeo.svg)](https://badge.fury.io/py/scikeo)
-[![Youtube](https://img.shields.io/badge/YouTube-Channel-red)]()     
-[![Twitter](https://img.shields.io/twitter/url?label=Follow%20%40GeoYons&style=social&url=https%3A%2F%2Ftwitter.com%2FGeoYons)](https://twitter.com/GeoYons)
-[![Downloads](https://pepy.tech/badge/scikeo)](https://pepy.tech/project/scikeo)
-[![Downloads](https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/docs-passing-brightgreen.svg)]()
-
-<img src="https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/scikit-eo_logo.jpg" align="right" width="220"/>
-
-
-<!-- #region -->
-# Introduction
-
-Nowadays, remotely sensed data has increased dramatically. Microwaves and optical images with different spatial and temporal resolutions are available and are using to monitor a variaty of environmental issues such as deforestation, land degradation, crop classifications, among other. Although there are efforts (i.e., Python packages, forums, communities, etc.) to make available line-of-code tools for pre-processing, processing and analysis of satellite imagery, there is still a gap that needs to be filled. In other words, too much time is still spent by many users in developing Python lines of code. Algorithms for mapping land degradation through linear trend of vegetation indices, fusion optical and radar images to classify vegetation cover, calibration of machine learning lagorithms, among others, are not available yet.
-
-Therefore, **scikit-eo** is a Python package that provides tools for remote sensing. This package was developed to fill the gaps in remotely sensed data processing tools. Most of the tools are based on scientific publications, and others are useful algorithms that will allow processing to be done in a few lines of code. With these tools, the user will be able to invest time in analyzing the results of their data and not spend time on elaborating lines of code, which can sometimes be stressful.
-
-# Tools for Remote Sensing
-
-| Name of functions  | Description|
-| -------------------| --------------------------------------------------------------------------|
-| **`mla`**          | Machine Learning                                                          |
-| **`calmla`**       | Calibrating supervised classification in Remote Sensing                   |
-| **`confintervalML`**       | Information of confusion matrix by proportions of area, overall accuracy, user's accuracy with confidence interval and estimated area with confidence interval as well.                                    |
-| **`rkmeans`**      | K-means classification                                                    |
-| **`calkmeans`**    | This function allows to calibrate the kmeans algorithm. It is possible to obtain the best k value and the best embedded algorithm in kmeans.                               |
-| **`pca`**          | Principal Components Analysis                                             |
-| **`atmosCorr`**    | Atmospheric Correction of satellite imagery                               |
-| **`deepLearning`** | Deep Learning algorithms                                                  |
-| **`linearTrend`**  | Linear trend is useful for mapping forest degradation or land degradation |
-| **`fusionrs`**     | This algorithm allows to fusion images coming from different spectral sensors (e.g., optical-optical, optical and SAR or SAR-SAR). Among many of the qualities of this function, it is possible to obtain the contribution (%) of each variable in the fused image |
-| **`sma`**          | Spectral Mixture Analysis - Classification sup-pixel                      |
-| **`tassCap`**      | The Tasseled-Cap Transformation                                           |
-
-You will find more algorithms!.
-
-
-# Installation
-
-To use **scikit-eo** it is necessary to install it. There are two options:
-
-## 1. From PyPI
-
-**scikit-eo** is available on [PyPI](https://pypi.org/project/scikeo/), so to install it, run this command in your terminal:
-
-```python
-pip install scikeo
-```
-
-## 2. Installing from source
-
-It is also possible to install the latest development version directly from the GitHub repository with:
-
-```python
-pip install git+https://github.com/ytarazona/scikit-eo
-```
-<!-- #endregion -->
-
-# Example
-
-## 1. Applying Machine Learning
-
-Libraries to be used:
-
-```python
-import rasterio
-import numpy as np
-from scikeo.mla import MLA
-import matplotlib.pyplot as plt
-from dbfread import DBF
-import matplotlib as mpl
-import pandas as pd
-```
-
-## 2.0 Optical image
-
-
-Landsat-8 OLI (Operational Land Imager) will be used to obtain in order to classify using Random Forest (RF). This image, which is in surface reflectance with bands:
-- Blue -> B2
-- Green -> B3 
-- Red -> B4
-- Nir -> B5
-- Swir1 -> B6
-- Swir2 -> B7
-
-The image and signatures to be used can be downloaded [here](https://drive.google.com/drive/folders/193RhNpACu9THcOZu8OzMh-btnFCOgHrU?usp=sharing):
-
-
-## 3.0 Supervised Classification using Random Forest
-
-Image and endmembers
-
-```python
-path_raster = r"C:\data\ml\LC08_232066_20190727_SR.tif"
-img = rasterio.open(path_raster)
-
-path_endm = r"C:\data\ml\endmembers.dbf"
-endm = DBF(path_endm)
-```
-
-```python
-# endmembers
-df = pd.DataFrame(iter(endm))
-df.head()
-```
-<p align="left">
-  <a href="https://github.com/ytarazona/scikit-eo"><img src="https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/endembers.png" alt ="header" width = 75%>
-</a>
-</p>
-
-
-Instance of ```mla()```:
-
-```python
-inst = MLA(image = img, endmembers = endm)
-```
-
-Applying Random Forest:
-
-```python
-svm_class = inst.SVM(training_split = 0.7)
-```
-
-## 4.0 Results
-
-Dictionary of results
-
-```python
-svm_class.keys()
-```
-
-Overall accuracy
-
-```python
-svm_class.get('Overall_Accuracy')
-```
-
-Kappa index
-
-```python
-svm_class.get('Kappa_Index')
-```
-
-Confusion matrix or error matrix
-
-```python
-svm_class.get('Confusion_Matrix')
-```
-
-<p align="left">
-  <a href="https://github.com/ytarazona/scikit-eo"><img src="https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/confusion_matrix.png" alt ="header" width = 80%>
-</a>
-</p>
-
-
-Preparing the image before plotting
-
-```python
-# Let's define the color palette
-palette = mpl.colors.ListedColormap(["#2232F9","#F922AE","#229954","#7CED5E"])
-```
-
-Applying the ```plotRGB()``` algorithm is easy:
-
-```python
-# LetÂ´s plot
-fig, axes = plt.subplots(nrows = 1, ncols = 2, figsize = (15, 9))
-
-# satellite image
-plotRGB(img, title = 'Image in Surface Reflectance', ax = axes[0])
-
-# class results
-axes[1].imshow(svm_class.get('Classification_Map'), cmap = palette)
-axes[1].set_title("Classification map")
-axes[1].grid(False)
-```
-
-<p align="left">
-  <a href="https://github.com/ytarazona/scikit-eo"><img src="https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/classification.png" alt ="header" width = "750">
-</a>
-</p>
-
-<!-- #region -->
--   Free software: Apache Software License 2.0
--   Documentation: 
-
-## Acknowledgment
-
-Special thanks to:
-- [David Montero Loaiza](https://github.com/davemlz) for the idea of the package name **scikit-eo**.
-
-- [Qiusheng Wu](https://github.com/giswqs) for the suggestions that helped to improve the package.
-
-## Dedication and inspiration
-
-Yonatan Tarazona dedicates this package to [MarÃ­a Griselda Miyasiro LÃ³pez](https://github.com/geolomera), the person who inspired to develop it. In fact, the logo of the package is inspired by fog oasis known as "Lomas", an ecosystem that she loves deeply.
-
-## Credits
-
-This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter)
-<!-- #endregion -->
```

### Comparing `scikeo-0.2.1/scikeo.egg-info/SOURCES.txt` & `scikeo-0.2.12/scikeo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.1/setup.py` & `scikeo-0.2.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     keywords='scikeo',
     name='scikeo',
     packages=find_packages(include=['scikeo', 'scikeo.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ytarazona/scikit-eo',
-    version='0.2.1',
+    version='0.2.12',
     zip_safe=False,
 )
```

