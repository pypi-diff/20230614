# Comparing `tmp/mjwt-0.0.1.tar.gz` & `tmp/mjwt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mjwt-0.0.1.tar", last modified: Fri Jun  9 18:49:38 2023, max compression
+gzip compressed data, was "mjwt-0.0.2.tar", last modified: Wed Jun 14 10:32:29 2023, max compression
```

## Comparing `mjwt-0.0.1.tar` & `mjwt-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 18:49:38.000000 mjwt-0.0.1/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-06-09 12:33:50.000000 mjwt-0.0.1/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      111 2023-04-27 10:12:58.000000 mjwt-0.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1563 2023-06-09 18:49:38.000000 mjwt-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      455 2023-06-09 17:16:53.000000 mjwt-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 18:49:38.000000 mjwt-0.0.1/mjwt/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-09 17:25:01.000000 mjwt-0.0.1/mjwt/__init__.py
--rw-r--r--   0 root         (0) root         (0)      369 2023-06-09 17:25:01.000000 mjwt-0.0.1/mjwt/_modidx.py
--rw-r--r--   0 root         (0) root         (0)     1593 2023-06-09 17:25:01.000000 mjwt-0.0.1/mjwt/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 18:49:38.000000 mjwt-0.0.1/mjwt.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1563 2023-06-09 18:49:38.000000 mjwt-0.0.1/mjwt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      295 2023-06-09 18:49:38.000000 mjwt-0.0.1/mjwt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 18:49:38.000000 mjwt-0.0.1/mjwt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-06-09 18:49:38.000000 mjwt-0.0.1/mjwt.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 14:25:28.000000 mjwt-0.0.1/mjwt.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-09 18:49:38.000000 mjwt-0.0.1/mjwt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-09 18:49:38.000000 mjwt-0.0.1/mjwt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1000 2023-06-09 12:50:03.000000 mjwt-0.0.1/settings.ini
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 18:49:38.000000 mjwt-0.0.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     2596 2023-04-27 10:12:58.000000 mjwt-0.0.1/setup.py
+drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-06-14 10:32:29.387441 mjwt-0.0.2/
+-rw-r--r--   0 jovyan    (1000) users      (100)     1072 2023-06-09 12:33:50.000000 mjwt-0.0.2/LICENSE
+-rw-rw-r--   0 jovyan    (1000) users      (100)      111 2023-04-27 10:12:58.000000 mjwt-0.0.2/MANIFEST.in
+-rw-r--r--   0 jovyan    (1000) users      (100)     1323 2023-06-14 10:32:29.384119 mjwt-0.0.2/PKG-INFO
+-rw-r--r--   0 jovyan    (1000) users      (100)      504 2023-06-14 10:00:25.000000 mjwt-0.0.2/README.md
+drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-06-14 10:32:29.231873 mjwt-0.0.2/mjwt/
+-rw-r--r--   0 jovyan    (1000) users      (100)       22 2023-06-14 10:32:11.000000 mjwt-0.0.2/mjwt/__init__.py
+-rw-r--r--   0 jovyan    (1000) users      (100)      369 2023-06-14 10:32:11.000000 mjwt-0.0.2/mjwt/_modidx.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     1664 2023-06-14 10:32:11.000000 mjwt-0.0.2/mjwt/utils.py
+drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-06-14 10:32:29.372298 mjwt-0.0.2/mjwt.egg-info/
+-rw-r--r--   0 jovyan    (1000) users      (100)     1323 2023-06-14 10:32:28.000000 mjwt-0.0.2/mjwt.egg-info/PKG-INFO
+-rw-r--r--   0 jovyan    (1000) users      (100)      295 2023-06-14 10:32:28.000000 mjwt-0.0.2/mjwt.egg-info/SOURCES.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)        1 2023-06-14 10:32:28.000000 mjwt-0.0.2/mjwt.egg-info/dependency_links.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)       30 2023-06-14 10:32:28.000000 mjwt-0.0.2/mjwt.egg-info/entry_points.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)        1 2023-06-09 14:25:28.000000 mjwt-0.0.2/mjwt.egg-info/not-zip-safe
+-rw-r--r--   0 jovyan    (1000) users      (100)        7 2023-06-14 10:32:28.000000 mjwt-0.0.2/mjwt.egg-info/requires.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)        5 2023-06-14 10:32:28.000000 mjwt-0.0.2/mjwt.egg-info/top_level.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)      835 2023-06-14 10:32:11.000000 mjwt-0.0.2/settings.ini
+-rw-r--r--   0 jovyan    (1000) users      (100)       38 2023-06-14 10:32:29.388613 mjwt-0.0.2/setup.cfg
+-rw-rw-r--   0 jovyan    (1000) users      (100)     2596 2023-04-27 10:12:58.000000 mjwt-0.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mjwt-0.0.1/LICENSE` & `mjwt-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mjwt-0.0.1/PKG-INFO` & `mjwt-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,59 @@
 Metadata-Version: 2.1
 Name: mjwt
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python package with coding tools, code snippets and notes from Menno Witteveen
 Home-page: https://github.com/mennowitteveen/mjwt
 Author: Menno Witteveen
 Author-email: menno102@hotmail.com
 License: Apache Software License 2.0
-Description: # mjwt
-        
-        <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
-        
-        Hurr durr, this will become my readme it says. is this now mjws readmoi?
-        
-        ## Install
-        
-        ``` sh
-        pip install mjwt
-        ```
-        
-        ## How to use
-        
-        Im now gonna do a short code example:
-        
-        ``` python
-        1+1
-        ```
-        
-            2
-        
-        ``` python
-        # import numpy as np
-        # from mjwt.utils import legimplot
-        # legimplot(np.random.randn(5,5), show=True)
-        ```
-        
-        Bang, an implot above.
-        
-        ``` python
-        print('something')
-        ```
-        
-            something
-        
 Keywords: nbdev jupyter notebook python
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+mjwt
+================
+
+<!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
+
+Hurr durr, this will become my readme it says. is this now mjws readmoi?
+This is new text 14-6 thunderbird
+
+## Install
+
+``` sh
+pip install mjwt
+```
+
+## How to use
+
+Im now gonna do a short code example:
+
+``` python
+1+1
+```
+
+    2
+
+``` python
+# import numpy as np
+# from mjwt.utils import legimplot
+# legimplot(np.random.randn(5,5), show=True)
+```
+
+Bang, an implot above.
+
+``` python
+print('something')
+```
+
+    something
```

### Comparing `mjwt-0.0.1/mjwt/utils.py` & `mjwt-0.0.2/mjwt/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 # import matplotlib.pyplot as plt
 # import numpy as np
 # import scipy as sp
 # import pandas as pd
 # import matplotlib.colors as mcolors
 
 def legimplot(arg):
+    print('legiplotxtras')
+    print('a string with a bunch of stuff')
     print(arg)
     return 'fun'
 # def legimplot(M, show=True, cmap=None, interpolation='none', title=None, figsize=None, **kwargs):
 #     if title is None:
 #         #title = find_varname(M) # so so..
 #         frame = inspect.getouterframes(inspect.currentframe())[1]
 #         string = inspect.getframeinfo(frame[0]).code_context[0].strip()
```

### Comparing `mjwt-0.0.1/mjwt.egg-info/PKG-INFO` & `mjwt-0.0.2/mjwt.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,59 @@
 Metadata-Version: 2.1
 Name: mjwt
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python package with coding tools, code snippets and notes from Menno Witteveen
 Home-page: https://github.com/mennowitteveen/mjwt
 Author: Menno Witteveen
 Author-email: menno102@hotmail.com
 License: Apache Software License 2.0
-Description: # mjwt
-        
-        <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
-        
-        Hurr durr, this will become my readme it says. is this now mjws readmoi?
-        
-        ## Install
-        
-        ``` sh
-        pip install mjwt
-        ```
-        
-        ## How to use
-        
-        Im now gonna do a short code example:
-        
-        ``` python
-        1+1
-        ```
-        
-            2
-        
-        ``` python
-        # import numpy as np
-        # from mjwt.utils import legimplot
-        # legimplot(np.random.randn(5,5), show=True)
-        ```
-        
-        Bang, an implot above.
-        
-        ``` python
-        print('something')
-        ```
-        
-            something
-        
 Keywords: nbdev jupyter notebook python
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+mjwt
+================
+
+<!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
+
+Hurr durr, this will become my readme it says. is this now mjws readmoi?
+This is new text 14-6 thunderbird
+
+## Install
+
+``` sh
+pip install mjwt
+```
+
+## How to use
+
+Im now gonna do a short code example:
+
+``` python
+1+1
+```
+
+    2
+
+``` python
+# import numpy as np
+# from mjwt.utils import legimplot
+# legimplot(np.random.randn(5,5), show=True)
+```
+
+Bang, an implot above.
+
+``` python
+print('something')
+```
+
+    something
```

### Comparing `mjwt-0.0.1/setup.py` & `mjwt-0.0.2/setup.py`

 * *Files identical despite different names*

