# Comparing `tmp/scikit-MDR-0.4.4.tar.gz` & `tmp/scikit-MDR-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scikit-MDR-0.4.4.tar", last modified: Wed May 10 14:42:57 2017, max compression
+gzip compressed data, was "scikit-MDR-0.4.5.tar", last modified: Wed Jun 14 17:44:50 2023, max compression
```

## Comparing `scikit-MDR-0.4.4.tar` & `scikit-MDR-0.4.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 randal_olson   (501) staff       (20)        0 2017-05-10 14:42:57.000000 scikit-MDR-0.4.4/
--rw-r--r--   0 randal_olson   (501) staff       (20)     1078 2016-08-10 16:00:56.000000 scikit-MDR-0.4.4/LICENSE
--rw-r--r--   0 randal_olson   (501) staff       (20)       62 2017-01-06 21:53:39.000000 scikit-MDR-0.4.4/MANIFEST.in
-drwxr-xr-x   0 randal_olson   (501) staff       (20)        0 2017-05-10 14:42:57.000000 scikit-MDR-0.4.4/mdr/
--rw-r--r--   0 randal_olson   (501) staff       (20)     1207 2017-05-10 12:06:41.000000 scikit-MDR-0.4.4/mdr/__init__.py
--rw-r--r--   0 randal_olson   (501) staff       (20)     1079 2017-05-10 14:35:37.000000 scikit-MDR-0.4.4/mdr/_version.py
--rw-r--r--   0 randal_olson   (501) staff       (20)     6194 2017-05-10 14:35:37.000000 scikit-MDR-0.4.4/mdr/continuous_mdr.py
--rw-r--r--   0 randal_olson   (501) staff       (20)     8417 2017-05-10 12:11:00.000000 scikit-MDR-0.4.4/mdr/mdr.py
--rw-r--r--   0 randal_olson   (501) staff       (20)     5324 2017-04-18 18:41:48.000000 scikit-MDR-0.4.4/mdr/mdr_ensemble.py
-drwxr-xr-x   0 randal_olson   (501) staff       (20)        0 2017-05-10 14:42:57.000000 scikit-MDR-0.4.4/mdr/utils/
--rw-r--r--   0 randal_olson   (501) staff       (20)     1078 2017-01-06 21:53:39.000000 scikit-MDR-0.4.4/mdr/utils/__init__.py
--rw-r--r--   0 randal_olson   (501) staff       (20)    14272 2017-01-26 19:10:15.000000 scikit-MDR-0.4.4/mdr/utils/utils.py
--rw-r--r--   0 randal_olson   (501) staff       (20)     1330 2017-05-10 14:42:57.000000 scikit-MDR-0.4.4/PKG-INFO
--rw-r--r--   0 randal_olson   (501) staff       (20)     6418 2017-05-10 12:48:56.000000 scikit-MDR-0.4.4/README.md
-drwxr-xr-x   0 randal_olson   (501) staff       (20)        0 2017-05-10 14:42:57.000000 scikit-MDR-0.4.4/scikit_MDR.egg-info/
--rw-r--r--   0 randal_olson   (501) staff       (20)        1 2017-05-10 14:42:57.000000 scikit-MDR-0.4.4/scikit_MDR.egg-info/dependency_links.txt
--rw-r--r--   0 randal_olson   (501) staff       (20)     1330 2017-05-10 14:42:57.000000 scikit-MDR-0.4.4/scikit_MDR.egg-info/PKG-INFO
--rw-r--r--   0 randal_olson   (501) staff       (20)       36 2017-05-10 14:42:57.000000 scikit-MDR-0.4.4/scikit_MDR.egg-info/requires.txt
--rw-r--r--   0 randal_olson   (501) staff       (20)      371 2017-05-10 14:42:57.000000 scikit-MDR-0.4.4/scikit_MDR.egg-info/SOURCES.txt
--rw-r--r--   0 randal_olson   (501) staff       (20)        4 2017-05-10 14:42:57.000000 scikit-MDR-0.4.4/scikit_MDR.egg-info/top_level.txt
--rw-r--r--   0 randal_olson   (501) staff       (20)        1 2017-05-10 12:55:57.000000 scikit-MDR-0.4.4/scikit_MDR.egg-info/zip-safe
--rw-r--r--   0 randal_olson   (501) staff       (20)       59 2017-05-10 14:42:57.000000 scikit-MDR-0.4.4/setup.cfg
--rw-r--r--   0 randal_olson   (501) staff       (20)     1748 2017-05-10 12:21:13.000000 scikit-MDR-0.4.4/setup.py
--rw-r--r--   0 randal_olson   (501) staff       (20)    18501 2017-05-10 14:35:37.000000 scikit-MDR-0.4.4/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:44:50.588491 scikit-MDR-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-14 17:44:37.000000 scikit-MDR-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-14 17:44:37.000000 scikit-MDR-0.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-14 17:44:50.588491 scikit-MDR-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-06-14 17:44:37.000000 scikit-MDR-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:44:50.588491 scikit-MDR-0.4.5/mdr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-14 17:44:37.000000 scikit-MDR-0.4.5/mdr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-14 17:44:37.000000 scikit-MDR-0.4.5/mdr/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-06-14 17:44:37.000000 scikit-MDR-0.4.5/mdr/continuous_mdr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8769 2023-06-14 17:44:37.000000 scikit-MDR-0.4.5/mdr/mdr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-06-14 17:44:37.000000 scikit-MDR-0.4.5/mdr/mdr_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:44:50.588491 scikit-MDR-0.4.5/mdr/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-14 17:44:37.000000 scikit-MDR-0.4.5/mdr/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14272 2023-06-14 17:44:37.000000 scikit-MDR-0.4.5/mdr/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 17:44:50.588491 scikit-MDR-0.4.5/scikit_MDR.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-14 17:44:50.000000 scikit-MDR-0.4.5/scikit_MDR.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-14 17:44:50.000000 scikit-MDR-0.4.5/scikit_MDR.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 17:44:50.000000 scikit-MDR-0.4.5/scikit_MDR.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-14 17:44:50.000000 scikit-MDR-0.4.5/scikit_MDR.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-14 17:44:50.000000 scikit-MDR-0.4.5/scikit_MDR.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 17:44:50.000000 scikit-MDR-0.4.5/scikit_MDR.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 17:44:50.588491 scikit-MDR-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-14 17:44:37.000000 scikit-MDR-0.4.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19717 2023-06-14 17:44:37.000000 scikit-MDR-0.4.5/tests.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `scikit-MDR-0.4.4/LICENSE` & `scikit-MDR-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-MDR-0.4.4/mdr/__init__.py` & `scikit-MDR-0.4.5/mdr/utils/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,11 +13,8 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT
 LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
 WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
 SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
-from ._version import __version__
-from .mdr import MDR, MDRClassifier
-from .continuous_mdr import ContinuousMDR
-from .mdr_ensemble import MDREnsemble
+from .utils import *
```

### Comparing `scikit-MDR-0.4.4/mdr/_version.py` & `scikit-MDR-0.4.5/mdr/_version.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 # -*- coding: utf-8 -*-
 
 """
+scikit-MDR was primarily developed at the University of Pennsylvania by:
+    - Randal S. Olson (rso@randalolson.com)
+    - Tuan Nguyen (tnguyen4@swarthmore.edu)
+    - and many more generous open source contributors
+
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software without restriction,
 including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense,
 and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial
@@ -13,8 +18,8 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT
 LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
 WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
 SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
-__version__ = '0.4.4'
+__version__ = '0.4.5'
```

### Comparing `scikit-MDR-0.4.4/mdr/continuous_mdr.py` & `scikit-MDR-0.4.5/mdr/continuous_mdr.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 # -*- coding: utf-8 -*-
 
 """
+scikit-MDR was primarily developed at the University of Pennsylvania by:
+    - Randal S. Olson (rso@randalolson.com)
+    - Tuan Nguyen (tnguyen4@swarthmore.edu)
+    - and many more generous open source contributors
+
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software without restriction,
 including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense,
 and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial
```

### Comparing `scikit-MDR-0.4.4/mdr/mdr.py` & `scikit-MDR-0.4.5/mdr/mdr.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 # -*- coding: utf-8 -*-
 
 """
+scikit-MDR was primarily developed at the University of Pennsylvania by:
+    - Randal S. Olson (rso@randalolson.com)
+    - Tuan Nguyen (tnguyen4@swarthmore.edu)
+    - and many more generous open source contributors
+
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software without restriction,
 including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense,
 and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial
@@ -114,15 +119,16 @@
         array-like: {n_samples, 1}
             Constructed features from the provided feature matrix
 
         """
         if self.feature_map is None:
             raise ValueError('The MDR model must be fit before transform can be called.')
 
-        new_feature = np.zeros(features.shape[0], dtype=np.int)
+        # new_feature = np.zeros(features.shape[0], dtype=np.int)
+        new_feature = np.zeros(features.shape[0], dtype=np.int64)
 
         for row_i in range(features.shape[0]):
             feature_instance = tuple(features[row_i])
             if feature_instance in self.feature_map:
                 new_feature[row_i] = self.feature_map[feature_instance]
             else:
                 new_feature[row_i] = self.default_label
@@ -168,15 +174,16 @@
         array-like: {n_samples}
             Constructed features from the provided feature matrix
 
         """
         if self.feature_map is None:
             raise ValueError('The MDR model must be fit before predict can be called.')
 
-        new_feature = np.zeros(features.shape[0], dtype=np.int)
+        # new_feature = np.zeros(features.shape[0], dtype=np.int)
+        new_feature = np.zeros(features.shape[0], dtype=np.int64)
 
         for row_i in range(features.shape[0]):
             feature_instance = tuple(features[row_i])
             if feature_instance in self.feature_map:
                 new_feature[row_i] = self.feature_map[feature_instance]
             else:
                 new_feature[row_i] = self.default_label
```

### Comparing `scikit-MDR-0.4.4/mdr/mdr_ensemble.py` & `scikit-MDR-0.4.5/mdr/mdr_ensemble.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 # -*- coding: utf-8 -*-
 
 """
+scikit-MDR was primarily developed at the University of Pennsylvania by:
+    - Randal S. Olson (rso@randalolson.com)
+    - Tuan Nguyen (tnguyen4@swarthmore.edu)
+    - and many more generous open source contributors
+
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software without restriction,
 including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense,
 and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial
```

### Comparing `scikit-MDR-0.4.4/mdr/utils/__init__.py` & `scikit-MDR-0.4.5/mdr/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 # -*- coding: utf-8 -*-
 
 """
+scikit-MDR was primarily developed at the University of Pennsylvania by:
+    - Randal S. Olson (rso@randalolson.com)
+    - Tuan Nguyen (tnguyen4@swarthmore.edu)
+    - and many more generous open source contributors
+
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software without restriction,
 including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense,
 and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial
@@ -13,8 +18,11 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT
 LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
 WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
 SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
-from .utils import *
+from ._version import __version__
+from .mdr import MDR, MDRClassifier
+from .continuous_mdr import ContinuousMDR
+from .mdr_ensemble import MDREnsemble
```

### Comparing `scikit-MDR-0.4.4/mdr/utils/utils.py` & `scikit-MDR-0.4.5/mdr/utils/utils.py`

 * *Files identical despite different names*

### Comparing `scikit-MDR-0.4.4/PKG-INFO` & `scikit-MDR-0.4.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: scikit-MDR
-Version: 0.4.4
+Version: 0.4.5
 Summary: Multifactor Dimensionality Reduction (MDR)
 Home-page: https://github.com/EpistasisLab/scikit-mdr
 Author: Randal S. Olson and Tuan Nguyen
 Author-email: rso@randalolson.com
 License: License :: OSI Approved :: MIT License
-Description: 
-        A sklearn-compatible Python implementation of Multifactor Dimensionality Reduction (MDR) for feature construction.
-        
-        Contact
-        =============
-        If you have any questions or comments about scikit-MDR, please feel free to contact us via:
-        
-        E-mail: rso@randalolson.com
-        
-        or Twitter: https://twitter.com/randal_olson
-        
-        This project is hosted at https://github.com/EpistasisLab/scikit-mdr
-        
 Keywords: bioinformatics,GWAS,feature construction,single nucleotide polymorphisms,epistasis,dimesionality reduction,scikit-learn,machine learning
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+License-File: LICENSE
+
+
+A sklearn-compatible Python implementation of Multifactor Dimensionality Reduction (MDR) for feature construction.
+
+Contact
+=============
+If you have any questions or comments about scikit-MDR, please feel free to contact us via:
+
+E-mail: rso@randalolson.com
+
+or Twitter: https://twitter.com/randal_olson
+
+This project is hosted at https://github.com/EpistasisLab/scikit-mdr
```

### Comparing `scikit-MDR-0.4.4/README.md` & `scikit-MDR-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `scikit-MDR-0.4.4/scikit_MDR.egg-info/PKG-INFO` & `scikit-MDR-0.4.5/scikit_MDR.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: scikit-MDR
-Version: 0.4.4
+Version: 0.4.5
 Summary: Multifactor Dimensionality Reduction (MDR)
 Home-page: https://github.com/EpistasisLab/scikit-mdr
 Author: Randal S. Olson and Tuan Nguyen
 Author-email: rso@randalolson.com
 License: License :: OSI Approved :: MIT License
-Description: 
-        A sklearn-compatible Python implementation of Multifactor Dimensionality Reduction (MDR) for feature construction.
-        
-        Contact
-        =============
-        If you have any questions or comments about scikit-MDR, please feel free to contact us via:
-        
-        E-mail: rso@randalolson.com
-        
-        or Twitter: https://twitter.com/randal_olson
-        
-        This project is hosted at https://github.com/EpistasisLab/scikit-mdr
-        
 Keywords: bioinformatics,GWAS,feature construction,single nucleotide polymorphisms,epistasis,dimesionality reduction,scikit-learn,machine learning
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+License-File: LICENSE
+
+
+A sklearn-compatible Python implementation of Multifactor Dimensionality Reduction (MDR) for feature construction.
+
+Contact
+=============
+If you have any questions or comments about scikit-MDR, please feel free to contact us via:
+
+E-mail: rso@randalolson.com
+
+or Twitter: https://twitter.com/randal_olson
+
+This project is hosted at https://github.com/EpistasisLab/scikit-mdr
```

### Comparing `scikit-MDR-0.4.4/setup.py` & `scikit-MDR-0.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `scikit-MDR-0.4.4/tests.py` & `scikit-MDR-0.4.5/tests.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,29 @@
+# -*- coding: utf-8 -*-
+
 """
-Tuan Nguyen & Randal Olson 
+scikit-MDR was primarily developed at the University of Pennsylvania by:
+    - Randal S. Olson (rso@randalolson.com)
+    - Tuan Nguyen (tnguyen4@swarthmore.edu)
+    - and many more generous open source contributors
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software
+and associated documentation files (the "Software"), to deal in the Software without restriction,
+including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so,
+subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial
+portions of the Software.
 
-Unit tests for MDR
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT
+LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
+WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
+SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
 from mdr import MDR, MDRClassifier, ContinuousMDR
 import numpy as np
 import random
 import warnings
 import inspect
```

