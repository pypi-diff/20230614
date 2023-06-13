# Comparing `tmp/HandGestureRecSiliconM1-0.1.tar.gz` & `tmp/HandGestureRecSiliconM1-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HandGestureRecSiliconM1-0.1.tar", last modified: Tue Jun 13 22:05:58 2023, max compression
+gzip compressed data, was "HandGestureRecSiliconM1-0.1.2.tar", last modified: Tue Jun 13 22:27:28 2023, max compression
```

## Comparing `HandGestureRecSiliconM1-0.1.tar` & `HandGestureRecSiliconM1-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ahmadbodayr   (501) staff       (20)        0 2023-06-13 22:05:58.665540 HandGestureRecSiliconM1-0.1/
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)     1069 2023-06-13 20:47:04.000000 HandGestureRecSiliconM1-0.1/LICENSE
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)      258 2023-06-13 22:05:58.665403 HandGestureRecSiliconM1-0.1/PKG-INFO
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)     2547 2023-06-13 22:05:12.000000 HandGestureRecSiliconM1-0.1/README.md
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)       38 2023-06-13 22:05:58.665579 HandGestureRecSiliconM1-0.1/setup.cfg
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)      819 2023-06-13 20:42:52.000000 HandGestureRecSiliconM1-0.1/setup.py
-drwxr-xr-x   0 ahmadbodayr   (501) staff       (20)        0 2023-06-13 22:05:58.664382 HandGestureRecSiliconM1-0.1/src/
-drwxr-xr-x   0 ahmadbodayr   (501) staff       (20)        0 2023-06-13 22:05:58.665234 HandGestureRecSiliconM1-0.1/src/HandGestureRecSiliconM1.egg-info/
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)      258 2023-06-13 22:05:58.000000 HandGestureRecSiliconM1-0.1/src/HandGestureRecSiliconM1.egg-info/PKG-INFO
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)      468 2023-06-13 22:05:58.000000 HandGestureRecSiliconM1-0.1/src/HandGestureRecSiliconM1.egg-info/SOURCES.txt
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)        1 2023-06-13 22:05:58.000000 HandGestureRecSiliconM1-0.1/src/HandGestureRecSiliconM1.egg-info/dependency_links.txt
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)       33 2023-06-13 22:05:58.000000 HandGestureRecSiliconM1-0.1/src/HandGestureRecSiliconM1.egg-info/entry_points.txt
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)       67 2023-06-13 22:05:58.000000 HandGestureRecSiliconM1-0.1/src/HandGestureRecSiliconM1.egg-info/requires.txt
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)       85 2023-06-13 22:05:58.000000 HandGestureRecSiliconM1-0.1/src/HandGestureRecSiliconM1.egg-info/top_level.txt
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)    11233 2023-06-13 18:28:48.000000 HandGestureRecSiliconM1-0.1/src/MLScript_2.py
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)     3459 2023-06-11 20:53:14.000000 HandGestureRecSiliconM1-0.1/src/main.py
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)     2805 2023-05-17 13:36:20.000000 HandGestureRecSiliconM1-0.1/src/mainView.py
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)     1588 2023-06-12 21:52:36.000000 HandGestureRecSiliconM1-0.1/src/modelTestingView.py
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)     4229 2023-05-21 00:52:06.000000 HandGestureRecSiliconM1-0.1/src/myDataSetsView.py
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)     1309 2023-05-20 23:46:55.000000 HandGestureRecSiliconM1-0.1/src/myGesturesView.py
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)     2569 2023-06-12 23:00:37.000000 HandGestureRecSiliconM1-0.1/src/myModelsView.py
+drwxr-xr-x   0 ahmadbodayr   (501) staff       (20)        0 2023-06-13 22:27:28.419332 HandGestureRecSiliconM1-0.1.2/
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)     1069 2023-06-13 20:47:04.000000 HandGestureRecSiliconM1-0.1.2/LICENSE
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)     2847 2023-06-13 22:27:28.419176 HandGestureRecSiliconM1-0.1.2/PKG-INFO
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)     2546 2023-06-13 22:12:56.000000 HandGestureRecSiliconM1-0.1.2/README.md
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)       38 2023-06-13 22:27:28.419370 HandGestureRecSiliconM1-0.1.2/setup.cfg
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)      980 2023-06-13 22:27:24.000000 HandGestureRecSiliconM1-0.1.2/setup.py
+drwxr-xr-x   0 ahmadbodayr   (501) staff       (20)        0 2023-06-13 22:27:28.418292 HandGestureRecSiliconM1-0.1.2/src/
+drwxr-xr-x   0 ahmadbodayr   (501) staff       (20)        0 2023-06-13 22:27:28.419001 HandGestureRecSiliconM1-0.1.2/src/HandGestureRecSiliconM1.egg-info/
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)     2847 2023-06-13 22:27:28.000000 HandGestureRecSiliconM1-0.1.2/src/HandGestureRecSiliconM1.egg-info/PKG-INFO
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)      468 2023-06-13 22:27:28.000000 HandGestureRecSiliconM1-0.1.2/src/HandGestureRecSiliconM1.egg-info/SOURCES.txt
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)        1 2023-06-13 22:27:28.000000 HandGestureRecSiliconM1-0.1.2/src/HandGestureRecSiliconM1.egg-info/dependency_links.txt
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)       33 2023-06-13 22:27:28.000000 HandGestureRecSiliconM1-0.1.2/src/HandGestureRecSiliconM1.egg-info/entry_points.txt
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)       67 2023-06-13 22:27:28.000000 HandGestureRecSiliconM1-0.1.2/src/HandGestureRecSiliconM1.egg-info/requires.txt
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)       85 2023-06-13 22:27:28.000000 HandGestureRecSiliconM1-0.1.2/src/HandGestureRecSiliconM1.egg-info/top_level.txt
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)    11233 2023-06-13 18:28:48.000000 HandGestureRecSiliconM1-0.1.2/src/MLScript_2.py
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)     3459 2023-06-11 20:53:14.000000 HandGestureRecSiliconM1-0.1.2/src/main.py
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)     2805 2023-05-17 13:36:20.000000 HandGestureRecSiliconM1-0.1.2/src/mainView.py
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)     1588 2023-06-12 21:52:36.000000 HandGestureRecSiliconM1-0.1.2/src/modelTestingView.py
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)     4229 2023-05-21 00:52:06.000000 HandGestureRecSiliconM1-0.1.2/src/myDataSetsView.py
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)     1309 2023-05-20 23:46:55.000000 HandGestureRecSiliconM1-0.1.2/src/myGesturesView.py
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)     2569 2023-06-12 23:00:37.000000 HandGestureRecSiliconM1-0.1.2/src/myModelsView.py
```

### Comparing `HandGestureRecSiliconM1-0.1/LICENSE` & `HandGestureRecSiliconM1-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `HandGestureRecSiliconM1-0.1/README.md` & `HandGestureRecSiliconM1-0.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 It is comprised of:
 ### Data Collection:
  The data collection is done using OpenCV and MediaPipe, each gesture is composed of 80 videos each is 30 frames, with each frame containing the 42 landmarks for each hand. Each landmark is an X, Y,  Z  tupple which describes the location of that specific landmark.
 ### Data Storage Strategy:
 No DBMS was used instead a folder tree which is composed of 3 submodules was built. The first submodule is  a  gestures folder that contains all the gestures defined by the user, the second is a datasets submodule which contains all the datasets created by the user. A single dataset is a non null subset of the gestures.
 ### The machine learning algorithm:
 The ML. model used is an LSTM model  which was built using Tensorflow 2.X  and the Keras ApI. for tensorFlow.
-# How to uses:
+# How to use:
 install the library from $ pip using pip install HandGestureRecSiliconM1 and in your python project write at the terminal run 
 * 1)   The user define one or more gesture using the GUI. One gesture is to be defined at a time. The gesture is defined by giving it a name and pressing create gesture then OpenCV will  give the user access to the webcam, 80 videos will be taken each is 30 frames in length so the user needs to do the gesture for 80 times. The starting time of each try of the 80 will be shown on the screen.
 * 2) After the user defines 1 or more gestures, he can then use the datasets submodule to create a dataset which will then serve as an input to the ML. model. To create a dataset the user have to give it a name and choose a subset of the gestures he defiend before hand then press create dataset.
 * 3)  After having one or more datasets the user can then can to the models submodule to crerate a model to a specific dataset. There is a 1:1 relation between the datasets and the models meaning that every dataset can only contribute to only one model.
 * 4)  After creating one or more models the user can test his models using the testing submodule.
```

### Comparing `HandGestureRecSiliconM1-0.1/setup.py` & `HandGestureRecSiliconM1-0.1.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from setuptools import setup, find_packages
+with open("README.md", "r") as fh:
+    long_description = fh.read()
 setup(
+    long_description=long_description, 
+    long_description_content_type="text/markdown",
     name='HandGestureRecSiliconM1',
-    version='0.1',
+    version='0.1.2',
     description='m1 macs version',
     packages=find_packages(),
     py_modules=[
         "main",
         "MLScript_2",
         "mainView",
         "modelTestingView",
```

### Comparing `HandGestureRecSiliconM1-0.1/src/MLScript_2.py` & `HandGestureRecSiliconM1-0.1.2/src/MLScript_2.py`

 * *Files identical despite different names*

### Comparing `HandGestureRecSiliconM1-0.1/src/main.py` & `HandGestureRecSiliconM1-0.1.2/src/main.py`

 * *Files identical despite different names*

### Comparing `HandGestureRecSiliconM1-0.1/src/mainView.py` & `HandGestureRecSiliconM1-0.1.2/src/mainView.py`

 * *Files identical despite different names*

### Comparing `HandGestureRecSiliconM1-0.1/src/modelTestingView.py` & `HandGestureRecSiliconM1-0.1.2/src/modelTestingView.py`

 * *Files identical despite different names*

### Comparing `HandGestureRecSiliconM1-0.1/src/myDataSetsView.py` & `HandGestureRecSiliconM1-0.1.2/src/myDataSetsView.py`

 * *Files identical despite different names*

### Comparing `HandGestureRecSiliconM1-0.1/src/myGesturesView.py` & `HandGestureRecSiliconM1-0.1.2/src/myGesturesView.py`

 * *Files identical despite different names*

### Comparing `HandGestureRecSiliconM1-0.1/src/myModelsView.py` & `HandGestureRecSiliconM1-0.1.2/src/myModelsView.py`

 * *Files identical despite different names*

