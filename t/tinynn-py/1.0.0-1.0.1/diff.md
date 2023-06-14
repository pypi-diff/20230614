# Comparing `tmp/tinynn-py-1.0.0.tar.gz` & `tmp/tinynn-py-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinynn-py-1.0.0.tar", last modified: Wed Jun 14 11:51:30 2023, max compression
+gzip compressed data, was "tinynn-py-1.0.1.tar", last modified: Wed Jun 14 12:03:00 2023, max compression
```

## Comparing `tinynn-py-1.0.0.tar` & `tinynn-py-1.0.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 praneethvasarla   (501) staff       (20)        0 2023-06-14 11:51:30.539653 tinynn-py-1.0.0/
--rw-r--r--   0 praneethvasarla   (501) staff       (20)     1073 2023-05-21 08:04:09.000000 tinynn-py-1.0.0/LICENSE
--rw-r--r--   0 praneethvasarla   (501) staff       (20)     2063 2023-06-14 11:51:30.539533 tinynn-py-1.0.0/PKG-INFO
--rw-r--r--   0 praneethvasarla   (501) staff       (20)     1881 2023-06-14 10:56:57.000000 tinynn-py-1.0.0/README.md
--rw-r--r--   0 praneethvasarla   (501) staff       (20)       38 2023-06-14 11:51:30.539685 tinynn-py-1.0.0/setup.cfg
--rw-r--r--   0 praneethvasarla   (501) staff       (20)      351 2023-06-14 11:51:23.000000 tinynn-py-1.0.0/setup.py
-drwxr-xr-x   0 praneethvasarla   (501) staff       (20)        0 2023-06-14 11:51:30.534824 tinynn-py-1.0.0/tinynn/
--rw-r--r--   0 praneethvasarla   (501) staff       (20)       26 2023-05-21 08:04:09.000000 tinynn-py-1.0.0/tinynn/__init__.py
-drwxr-xr-x   0 praneethvasarla   (501) staff       (20)        0 2023-06-14 11:51:30.535594 tinynn-py-1.0.0/tinynn/activations/
--rw-r--r--   0 praneethvasarla   (501) staff       (20)       80 2023-05-21 08:04:09.000000 tinynn-py-1.0.0/tinynn/activations/__init__.py
--rw-r--r--   0 praneethvasarla   (501) staff       (20)     1963 2023-06-11 13:21:53.000000 tinynn-py-1.0.0/tinynn/activations/relu.py
--rw-r--r--   0 praneethvasarla   (501) staff       (20)      178 2023-05-21 08:04:09.000000 tinynn-py-1.0.0/tinynn/activations/sigmoid.py
--rw-r--r--   0 praneethvasarla   (501) staff       (20)     2508 2023-06-11 13:26:48.000000 tinynn-py-1.0.0/tinynn/activations/softmax.py
-drwxr-xr-x   0 praneethvasarla   (501) staff       (20)        0 2023-06-14 11:51:30.536117 tinynn-py-1.0.0/tinynn/layers/
--rw-r--r--   0 praneethvasarla   (501) staff       (20)       24 2023-06-14 11:00:29.000000 tinynn-py-1.0.0/tinynn/layers/__init__.py
--rw-r--r--   0 praneethvasarla   (501) staff       (20)     3849 2023-06-11 13:30:07.000000 tinynn-py-1.0.0/tinynn/layers/dense.py
-drwxr-xr-x   0 praneethvasarla   (501) staff       (20)        0 2023-06-14 11:51:30.537039 tinynn-py-1.0.0/tinynn/loss_functions/
--rw-r--r--   0 praneethvasarla   (501) staff       (20)       84 2023-06-14 11:29:40.000000 tinynn-py-1.0.0/tinynn/loss_functions/__init__.py
--rw-r--r--   0 praneethvasarla   (501) staff       (20)     2901 2023-06-11 13:33:39.000000 tinynn-py-1.0.0/tinynn/loss_functions/categorical_cross_entrpy.py
--rw-r--r--   0 praneethvasarla   (501) staff       (20)      671 2023-06-11 13:35:16.000000 tinynn-py-1.0.0/tinynn/loss_functions/loss.py
--rw-r--r--   0 praneethvasarla   (501) staff       (20)      588 2023-05-21 08:04:09.000000 tinynn-py-1.0.0/tinynn/loss_functions/mean_square_error.py
-drwxr-xr-x   0 praneethvasarla   (501) staff       (20)        0 2023-06-14 11:51:30.537425 tinynn-py-1.0.0/tinynn/models/
--rw-r--r--   0 praneethvasarla   (501) staff       (20)       34 2023-06-14 11:29:30.000000 tinynn-py-1.0.0/tinynn/models/__init__.py
--rw-r--r--   0 praneethvasarla   (501) staff       (20)     4993 2023-06-11 13:44:35.000000 tinynn-py-1.0.0/tinynn/models/sequential.py
-drwxr-xr-x   0 praneethvasarla   (501) staff       (20)        0 2023-06-14 11:51:30.538739 tinynn-py-1.0.0/tinynn/optimizers/
--rw-r--r--   0 praneethvasarla   (501) staff       (20)      123 2023-06-11 08:54:49.000000 tinynn-py-1.0.0/tinynn/optimizers/__init__.py
--rw-r--r--   0 praneethvasarla   (501) staff       (20)     2505 2023-06-14 08:49:57.000000 tinynn-py-1.0.0/tinynn/optimizers/adagrad.py
--rw-r--r--   0 praneethvasarla   (501) staff       (20)     3755 2023-06-14 10:02:34.000000 tinynn-py-1.0.0/tinynn/optimizers/adam.py
--rw-r--r--   0 praneethvasarla   (501) staff       (20)     2838 2023-06-14 09:39:10.000000 tinynn-py-1.0.0/tinynn/optimizers/rmsprop.py
--rw-r--r--   0 praneethvasarla   (501) staff       (20)     2868 2023-06-14 09:43:36.000000 tinynn-py-1.0.0/tinynn/optimizers/sgd.py
-drwxr-xr-x   0 praneethvasarla   (501) staff       (20)        0 2023-06-14 11:51:30.539374 tinynn-py-1.0.0/tinynn_py.egg-info/
--rw-r--r--   0 praneethvasarla   (501) staff       (20)     2063 2023-06-14 11:51:30.000000 tinynn-py-1.0.0/tinynn_py.egg-info/PKG-INFO
--rw-r--r--   0 praneethvasarla   (501) staff       (20)      726 2023-06-14 11:51:30.000000 tinynn-py-1.0.0/tinynn_py.egg-info/SOURCES.txt
--rw-r--r--   0 praneethvasarla   (501) staff       (20)        1 2023-06-14 11:51:30.000000 tinynn-py-1.0.0/tinynn_py.egg-info/dependency_links.txt
--rw-r--r--   0 praneethvasarla   (501) staff       (20)        6 2023-06-14 11:51:30.000000 tinynn-py-1.0.0/tinynn_py.egg-info/requires.txt
--rw-r--r--   0 praneethvasarla   (501) staff       (20)        7 2023-06-14 11:51:30.000000 tinynn-py-1.0.0/tinynn_py.egg-info/top_level.txt
+drwxr-xr-x   0 praneethvasarla   (501) staff       (20)        0 2023-06-14 12:03:00.306206 tinynn-py-1.0.1/
+-rw-r--r--   0 praneethvasarla   (501) staff       (20)     1073 2023-05-21 08:04:09.000000 tinynn-py-1.0.1/LICENSE
+-rw-r--r--   0 praneethvasarla   (501) staff       (20)     2085 2023-06-14 12:03:00.306085 tinynn-py-1.0.1/PKG-INFO
+-rw-r--r--   0 praneethvasarla   (501) staff       (20)     1903 2023-06-14 12:02:27.000000 tinynn-py-1.0.1/README.md
+-rw-r--r--   0 praneethvasarla   (501) staff       (20)       38 2023-06-14 12:03:00.306239 tinynn-py-1.0.1/setup.cfg
+-rw-r--r--   0 praneethvasarla   (501) staff       (20)      351 2023-06-14 12:02:55.000000 tinynn-py-1.0.1/setup.py
+drwxr-xr-x   0 praneethvasarla   (501) staff       (20)        0 2023-06-14 12:03:00.301470 tinynn-py-1.0.1/tinynn/
+-rw-r--r--   0 praneethvasarla   (501) staff       (20)       26 2023-05-21 08:04:09.000000 tinynn-py-1.0.1/tinynn/__init__.py
+drwxr-xr-x   0 praneethvasarla   (501) staff       (20)        0 2023-06-14 12:03:00.302253 tinynn-py-1.0.1/tinynn/activations/
+-rw-r--r--   0 praneethvasarla   (501) staff       (20)       80 2023-05-21 08:04:09.000000 tinynn-py-1.0.1/tinynn/activations/__init__.py
+-rw-r--r--   0 praneethvasarla   (501) staff       (20)     1963 2023-06-11 13:21:53.000000 tinynn-py-1.0.1/tinynn/activations/relu.py
+-rw-r--r--   0 praneethvasarla   (501) staff       (20)      178 2023-05-21 08:04:09.000000 tinynn-py-1.0.1/tinynn/activations/sigmoid.py
+-rw-r--r--   0 praneethvasarla   (501) staff       (20)     2508 2023-06-11 13:26:48.000000 tinynn-py-1.0.1/tinynn/activations/softmax.py
+drwxr-xr-x   0 praneethvasarla   (501) staff       (20)        0 2023-06-14 12:03:00.302691 tinynn-py-1.0.1/tinynn/layers/
+-rw-r--r--   0 praneethvasarla   (501) staff       (20)       24 2023-06-14 11:00:29.000000 tinynn-py-1.0.1/tinynn/layers/__init__.py
+-rw-r--r--   0 praneethvasarla   (501) staff       (20)     3849 2023-06-11 13:30:07.000000 tinynn-py-1.0.1/tinynn/layers/dense.py
+drwxr-xr-x   0 praneethvasarla   (501) staff       (20)        0 2023-06-14 12:03:00.303546 tinynn-py-1.0.1/tinynn/loss_functions/
+-rw-r--r--   0 praneethvasarla   (501) staff       (20)       84 2023-06-14 11:29:40.000000 tinynn-py-1.0.1/tinynn/loss_functions/__init__.py
+-rw-r--r--   0 praneethvasarla   (501) staff       (20)     2901 2023-06-11 13:33:39.000000 tinynn-py-1.0.1/tinynn/loss_functions/categorical_cross_entrpy.py
+-rw-r--r--   0 praneethvasarla   (501) staff       (20)      671 2023-06-11 13:35:16.000000 tinynn-py-1.0.1/tinynn/loss_functions/loss.py
+-rw-r--r--   0 praneethvasarla   (501) staff       (20)      588 2023-05-21 08:04:09.000000 tinynn-py-1.0.1/tinynn/loss_functions/mean_square_error.py
+drwxr-xr-x   0 praneethvasarla   (501) staff       (20)        0 2023-06-14 12:03:00.303907 tinynn-py-1.0.1/tinynn/models/
+-rw-r--r--   0 praneethvasarla   (501) staff       (20)       34 2023-06-14 11:29:30.000000 tinynn-py-1.0.1/tinynn/models/__init__.py
+-rw-r--r--   0 praneethvasarla   (501) staff       (20)     4993 2023-06-11 13:44:35.000000 tinynn-py-1.0.1/tinynn/models/sequential.py
+drwxr-xr-x   0 praneethvasarla   (501) staff       (20)        0 2023-06-14 12:03:00.305301 tinynn-py-1.0.1/tinynn/optimizers/
+-rw-r--r--   0 praneethvasarla   (501) staff       (20)      123 2023-06-11 08:54:49.000000 tinynn-py-1.0.1/tinynn/optimizers/__init__.py
+-rw-r--r--   0 praneethvasarla   (501) staff       (20)     2505 2023-06-14 08:49:57.000000 tinynn-py-1.0.1/tinynn/optimizers/adagrad.py
+-rw-r--r--   0 praneethvasarla   (501) staff       (20)     3755 2023-06-14 10:02:34.000000 tinynn-py-1.0.1/tinynn/optimizers/adam.py
+-rw-r--r--   0 praneethvasarla   (501) staff       (20)     2838 2023-06-14 09:39:10.000000 tinynn-py-1.0.1/tinynn/optimizers/rmsprop.py
+-rw-r--r--   0 praneethvasarla   (501) staff       (20)     2868 2023-06-14 09:43:36.000000 tinynn-py-1.0.1/tinynn/optimizers/sgd.py
+drwxr-xr-x   0 praneethvasarla   (501) staff       (20)        0 2023-06-14 12:03:00.305925 tinynn-py-1.0.1/tinynn_py.egg-info/
+-rw-r--r--   0 praneethvasarla   (501) staff       (20)     2085 2023-06-14 12:03:00.000000 tinynn-py-1.0.1/tinynn_py.egg-info/PKG-INFO
+-rw-r--r--   0 praneethvasarla   (501) staff       (20)      726 2023-06-14 12:03:00.000000 tinynn-py-1.0.1/tinynn_py.egg-info/SOURCES.txt
+-rw-r--r--   0 praneethvasarla   (501) staff       (20)        1 2023-06-14 12:03:00.000000 tinynn-py-1.0.1/tinynn_py.egg-info/dependency_links.txt
+-rw-r--r--   0 praneethvasarla   (501) staff       (20)        6 2023-06-14 12:03:00.000000 tinynn-py-1.0.1/tinynn_py.egg-info/requires.txt
+-rw-r--r--   0 praneethvasarla   (501) staff       (20)        7 2023-06-14 12:03:00.000000 tinynn-py-1.0.1/tinynn_py.egg-info/top_level.txt
```

### Comparing `tinynn-py-1.0.0/LICENSE` & `tinynn-py-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tinynn-py-1.0.0/PKG-INFO` & `tinynn-py-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinynn-py
-Version: 1.0.0
+Version: 1.0.1
 Summary: A tiny neural network library.
 Author: Praneeth Vasarla
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tinynn
 
@@ -28,28 +28,29 @@
 pip install tinynn
 ```
 
 ## Usage
 Here's a basic example demonstrating how to create a feedforward neural network using Tinynn:
 
 ```python
-import tinynn as tn
+from tinynn.models import Sequential
+from tinynn.layers import Dense
 import numpy as np
+
+model = Sequential()
+
 X = np.array([[1,2,3],
      [5,4,3],
      [2,3,4]])
 y = np.array([0, 0, 1])
 
+model.add(Dense(3,64))
+model.add(Dense(64,2,activation='softmax'))
 
-model = tn.models.Sequential()
-
-model.add(tn.layers.Dense(3,64))
-model.add(tn.layers.Dense(64,2,activation='softmax'))
-
-model.compile_model(learning_rate=0.01, optimizer='adam') #Also available params: decay_rate,momentum(only for sgd) and optimizer = sgd,adagrad
+model.compile_model(learning_rate=0.01, optimizer='adagrad') #Also available params: decay_rate,momentum(only for sgd) and optimizer = sgd,adagrad
 model.fit(X,y,epochs=1000)
 ```
 
 ## Contributions
 Contributions to Tinynn are welcome! Whether you want to report a bug, suggest a new feature, or submit a pull request, please feel free to do so. Let's make Tinynn better together.
 
 ## License
```

### Comparing `tinynn-py-1.0.0/README.md` & `tinynn-py-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -20,28 +20,29 @@
 pip install tinynn
 ```
 
 ## Usage
 Here's a basic example demonstrating how to create a feedforward neural network using Tinynn:
 
 ```python
-import tinynn as tn
+from tinynn.models import Sequential
+from tinynn.layers import Dense
 import numpy as np
+
+model = Sequential()
+
 X = np.array([[1,2,3],
      [5,4,3],
      [2,3,4]])
 y = np.array([0, 0, 1])
 
+model.add(Dense(3,64))
+model.add(Dense(64,2,activation='softmax'))
 
-model = tn.models.Sequential()
-
-model.add(tn.layers.Dense(3,64))
-model.add(tn.layers.Dense(64,2,activation='softmax'))
-
-model.compile_model(learning_rate=0.01, optimizer='adam') #Also available params: decay_rate,momentum(only for sgd) and optimizer = sgd,adagrad
+model.compile_model(learning_rate=0.01, optimizer='adagrad') #Also available params: decay_rate,momentum(only for sgd) and optimizer = sgd,adagrad
 model.fit(X,y,epochs=1000)
 ```
 
 ## Contributions
 Contributions to Tinynn are welcome! Whether you want to report a bug, suggest a new feature, or submit a pull request, please feel free to do so. Let's make Tinynn better together.
 
 ## License
```

### Comparing `tinynn-py-1.0.0/tinynn/activations/relu.py` & `tinynn-py-1.0.1/tinynn/activations/relu.py`

 * *Files identical despite different names*

### Comparing `tinynn-py-1.0.0/tinynn/activations/softmax.py` & `tinynn-py-1.0.1/tinynn/activations/softmax.py`

 * *Files identical despite different names*

### Comparing `tinynn-py-1.0.0/tinynn/layers/dense.py` & `tinynn-py-1.0.1/tinynn/layers/dense.py`

 * *Files identical despite different names*

### Comparing `tinynn-py-1.0.0/tinynn/loss_functions/categorical_cross_entrpy.py` & `tinynn-py-1.0.1/tinynn/loss_functions/categorical_cross_entrpy.py`

 * *Files identical despite different names*

### Comparing `tinynn-py-1.0.0/tinynn/loss_functions/loss.py` & `tinynn-py-1.0.1/tinynn/loss_functions/loss.py`

 * *Files identical despite different names*

### Comparing `tinynn-py-1.0.0/tinynn/loss_functions/mean_square_error.py` & `tinynn-py-1.0.1/tinynn/loss_functions/mean_square_error.py`

 * *Files identical despite different names*

### Comparing `tinynn-py-1.0.0/tinynn/models/sequential.py` & `tinynn-py-1.0.1/tinynn/models/sequential.py`

 * *Files identical despite different names*

### Comparing `tinynn-py-1.0.0/tinynn/optimizers/adagrad.py` & `tinynn-py-1.0.1/tinynn/optimizers/adagrad.py`

 * *Files identical despite different names*

### Comparing `tinynn-py-1.0.0/tinynn/optimizers/adam.py` & `tinynn-py-1.0.1/tinynn/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `tinynn-py-1.0.0/tinynn/optimizers/rmsprop.py` & `tinynn-py-1.0.1/tinynn/optimizers/rmsprop.py`

 * *Files identical despite different names*

### Comparing `tinynn-py-1.0.0/tinynn/optimizers/sgd.py` & `tinynn-py-1.0.1/tinynn/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `tinynn-py-1.0.0/tinynn_py.egg-info/PKG-INFO` & `tinynn-py-1.0.1/tinynn_py.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinynn-py
-Version: 1.0.0
+Version: 1.0.1
 Summary: A tiny neural network library.
 Author: Praneeth Vasarla
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tinynn
 
@@ -28,28 +28,29 @@
 pip install tinynn
 ```
 
 ## Usage
 Here's a basic example demonstrating how to create a feedforward neural network using Tinynn:
 
 ```python
-import tinynn as tn
+from tinynn.models import Sequential
+from tinynn.layers import Dense
 import numpy as np
+
+model = Sequential()
+
 X = np.array([[1,2,3],
      [5,4,3],
      [2,3,4]])
 y = np.array([0, 0, 1])
 
+model.add(Dense(3,64))
+model.add(Dense(64,2,activation='softmax'))
 
-model = tn.models.Sequential()
-
-model.add(tn.layers.Dense(3,64))
-model.add(tn.layers.Dense(64,2,activation='softmax'))
-
-model.compile_model(learning_rate=0.01, optimizer='adam') #Also available params: decay_rate,momentum(only for sgd) and optimizer = sgd,adagrad
+model.compile_model(learning_rate=0.01, optimizer='adagrad') #Also available params: decay_rate,momentum(only for sgd) and optimizer = sgd,adagrad
 model.fit(X,y,epochs=1000)
 ```
 
 ## Contributions
 Contributions to Tinynn are welcome! Whether you want to report a bug, suggest a new feature, or submit a pull request, please feel free to do so. Let's make Tinynn better together.
 
 ## License
```

### Comparing `tinynn-py-1.0.0/tinynn_py.egg-info/SOURCES.txt` & `tinynn-py-1.0.1/tinynn_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

