# Comparing `tmp/gender-detection-local-0.0.4.tar.gz` & `tmp/gender-detection-local-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gender-detection-local-0.0.4.tar", last modified: Tue May 23 07:35:20 2023, max compression
+gzip compressed data, was "gender-detection-local-0.0.5.tar", last modified: Wed Jun 14 09:12:47 2023, max compression
```

## Comparing `gender-detection-local-0.0.4.tar` & `gender-detection-local-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:35:20.823916 gender-detection-local-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:35:20.823916 gender-detection-local-0.0.4/CirclesGenderDetectionPython/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 07:35:10.000000 gender-detection-local-0.0.4/CirclesGenderDetectionPython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  7030816 2023-05-23 07:35:10.000000 gender-detection-local-0.0.4/CirclesGenderDetectionPython/gender_detection
--rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-05-23 07:35:10.000000 gender-detection-local-0.0.4/CirclesGenderDetectionPython/gender_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-23 07:35:10.000000 gender-detection-local-0.0.4/CirclesGenderDetectionPython/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-23 07:35:20.823916 gender-detection-local-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-23 07:35:10.000000 gender-detection-local-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:35:20.823916 gender-detection-local-0.0.4/gender_detection_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-23 07:35:20.000000 gender-detection-local-0.0.4/gender_detection_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-23 07:35:20.000000 gender-detection-local-0.0.4/gender_detection_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 07:35:20.000000 gender-detection-local-0.0.4/gender_detection_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-23 07:35:20.000000 gender-detection-local-0.0.4/gender_detection_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-23 07:35:10.000000 gender-detection-local-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 07:35:20.823916 gender-detection-local-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-23 07:35:10.000000 gender-detection-local-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:12:47.725875 gender-detection-local-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:12:47.721875 gender-detection-local-0.0.5/CirclesGenderDetectionPython/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:12:33.000000 gender-detection-local-0.0.5/CirclesGenderDetectionPython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  7030816 2023-06-14 09:12:33.000000 gender-detection-local-0.0.5/CirclesGenderDetectionPython/gender_detection
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-06-14 09:12:33.000000 gender-detection-local-0.0.5/CirclesGenderDetectionPython/gender_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-14 09:12:33.000000 gender-detection-local-0.0.5/CirclesGenderDetectionPython/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-14 09:12:47.721875 gender-detection-local-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-14 09:12:33.000000 gender-detection-local-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:12:47.721875 gender-detection-local-0.0.5/gender_detection_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-14 09:12:47.000000 gender-detection-local-0.0.5/gender_detection_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-14 09:12:47.000000 gender-detection-local-0.0.5/gender_detection_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:12:47.000000 gender-detection-local-0.0.5/gender_detection_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-14 09:12:47.000000 gender-detection-local-0.0.5/gender_detection_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-14 09:12:33.000000 gender-detection-local-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 09:12:47.725875 gender-detection-local-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-14 09:12:33.000000 gender-detection-local-0.0.5/setup.py
```

### Comparing `gender-detection-local-0.0.4/CirclesGenderDetectionPython/gender_detection` & `gender-detection-local-0.0.5/CirclesGenderDetectionPython/gender_detection`

 * *Files identical despite different names*

### Comparing `gender-detection-local-0.0.4/CirclesGenderDetectionPython/gender_detection.py` & `gender-detection-local-0.0.5/CirclesGenderDetectionPython/gender_detection.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,15 @@
-import numpy as np
-import tensorflow as tf
-import os
-from tensorflow.keras.utils import Sequence
-from keras.models import load_model
-from tensorflow.keras import Sequential,Model,Input
-from tensorflow.keras.layers import Conv2D,MaxPool2D,Flatten,Dense,Dropout,GlobalAveragePooling2D
-from keras.regularizers import l2
-import cv2
-from cv2 import VideoCapture,imshow,imwrite,waitKey
-
-from tensorflow import keras
-from tensorflow.keras.callbacks import EarlyStopping, ModelCheckpoint
-from keras.optimizers import SGD
-from keras.applications.inception_v3 import InceptionV3
-
-import random
+from numpy.random import rand
+from cv2 import VideoCapture
+from tensorflow import expand_dims
 from tensorflow.keras.metrics import categorical_crossentropy
-from tensorflow.keras.preprocessing.image import ImageDataGenerator
-
-import pandas as pd
-from keras.preprocessing.image import ImageDataGenerator as Imgen
-from keras.models import Model,Sequential
-import keras.layers as layers
+from tensorflow.io import read_file
+from tensorflow.image import decode_jpeg,resize,flip_left_right
+from tensorflow.keras.utils import image_dataset_from_directory
+from keras.models import Model,Sequential,load_model
 from keras.layers import Input,Conv2D,MaxPooling2D,Dropout,Flatten,Dense,GlobalAveragePooling2D,BatchNormalization
 from dotenv import load_dotenv
 load_dotenv()
 from CirclesLocalLoggerPython.LoggerServiceSingleton import LoggerServiceSingleton
 
 
 
@@ -41,46 +25,46 @@
     Args:
         input_shape (tuple): A tuple representing the shape of input tensor of an image.
                              (height, width, channel)
 
     Returns:
         keras.Sequential: A compiled CNN model instance. 
     """
-    CNNmodel = keras.Sequential([
-        layers.Conv2D(16, (3, 3), input_shape=input_shape, activation='relu'),
-        layers.BatchNormalization(),
-        layers.MaxPooling2D((2,2)),
-        layers.Dropout(0.2),
+    CNNmodel = Sequential([
+        Conv2D(16, (3, 3), input_shape=input_shape, activation='relu'),
+        BatchNormalization(),
+        MaxPooling2D((2,2)),
+        Dropout(0.2),
         
-        layers.Conv2D(32, (3, 3), activation='relu'),
-        layers.BatchNormalization(),
-        layers.MaxPooling2D((2,2)),
-        layers.Dropout(0.2),
-
-        layers.Conv2D(64, (3, 3), activation='relu'),
-        layers.BatchNormalization(),
-        layers.MaxPooling2D((2,2)),
-        layers.Dropout(0.2),
-
-        layers.Conv2D(128, (3, 3), activation='relu'),
-        layers.BatchNormalization(),
-        layers.MaxPooling2D((2,2)),
-        layers.Dropout(0.2),
-
-        layers.Flatten(),
-        layers.Dense(256, activation='relu'),
-        layers.Dropout(0.2),  
-        layers.Dense(128, activation = 'relu'),
-        layers.Dropout(0.2), 
-        layers.Dense(64, activation = 'relu'),
-        layers.Dropout(0.2), 
-        layers.Dense(32, activation = 'relu'),
-        layers.Dropout(0.2), 
-        layers.Dense(16, activation = 'relu'),
-        layers.Dense(1, activation = 'sigmoid')
+        Conv2D(32, (3, 3), activation='relu'),
+        BatchNormalization(),
+        MaxPooling2D((2,2)),
+        Dropout(0.2),
+
+        Conv2D(64, (3, 3), activation='relu'),
+        BatchNormalization(),
+        MaxPooling2D((2,2)),
+        Dropout(0.2),
+
+        Conv2D(128, (3, 3), activation='relu'),
+        BatchNormalization(),
+        MaxPooling2D((2,2)),
+        Dropout(0.2),
+
+        Flatten(),
+        Dense(256, activation='relu'),
+        Dropout(0.2),  
+        Dense(128, activation = 'relu'),
+        Dropout(0.2), 
+        Dense(64, activation = 'relu'),
+        Dropout(0.2), 
+        Dense(32, activation = 'relu'),
+        Dropout(0.2), 
+        Dense(16, activation = 'relu'),
+        Dense(1, activation = 'sigmoid')
     ])
 
     return CNNmodel
 
 def capture_write(filename="image.jpeg", port=0, ramp_frames=30, x=178, y=218):
     """
     Captures an image using the webcam and saves it to a file.
@@ -91,15 +75,15 @@
         ramp_frames (int): The number of frames to skip before capturing the image. Default is 30.
         x (int): The width of the image in pixels. Default is 178.
         y (int): The height of the image in pixels. Default is 218.
     
     Returns:
         numpy.ndarray: The captured image as a NumPy array.
     """
-    camera = cv2.VideoCapture(port)
+    camera = VideoCapture(port)
 
     # Set Resolution
     camera.set(3, x)
     camera.set(4, y)
 
     # Adjust camera lighting
     for i in range(ramp_frames):
@@ -129,43 +113,43 @@
         Returns:
             str: a string indicating the predicted gender ('Male' or 'Female').
         """
 
         # Test Functionality
         if image_path is not None:
            # Read the contents of the image file
-           image = tf.io.read_file(image_path)
+           image = read_file(image_path)
 
            # Decode the JPEG-encoded image into a tensor
-           image = tf.image.decode_jpeg(image)
+           image = decode_jpeg(image)
        
-           image = tf.image.resize(image, (178,218))
+           image = resize(image, (178,218))
         else:
            # Permission to use webcam and work on singular image
            inquiry = input("""
            This script will take a picture with your webcam, 
            this will only be for the purposes for determining your gender. 
            Proceed? (Y/n) """)
 
            if inquiry.lower()!="y" and inquiry.lower!="yes":
               self.lgrins.log("\nAborting\n")
               exit()
 
            # Capture Image from Webcam
-           image = tf.image.resize(capture_write(), (178, 218))
+           image = resize(capture_write(), (178, 218))
 
         # Rescale the pixel values to a range of [0, 1]
         image = image / 255.0
 
         # Apply data augmentation
-        if np.random.rand() < 0.5:
-            image = tf.image.flip_left_right(image)
+        if rand() < 0.5:
+            image = flip_left_right(image)
 
         model = load_model(model_path)
-        prediction = model.predict(tf.expand_dims(image, axis=0))[0]
+        prediction = model.predict(expand_dims(image, axis=0))[0]
         self.lgrins.log("Prediction Confidence (>0.5 Male,<=0.5 Female)",prediction)
         if prediction > 0.5:
             #print("Male")
             return "Male"
         else:
             #print("Female")
             return "Female"
@@ -181,17 +165,17 @@
 
         Args:
             save (bool): a boolean indicating whether to save the trained model or not. Defaults to True.
         """
         # Build Model With Transfer Learning from Pre-Trained VGG-Face
         model = create_model((178, 218, 3))
 
-        train = tf.keras.utils.image_dataset_from_directory("./Train", image_size=(178, 218))
-        validation = tf.keras.utils.image_dataset_from_directory("./Validation", image_size=(178, 218))
-        test = tf.keras.utils.image_dataset_from_directory("./Test", image_size=(178, 218))
+        train = image_dataset_from_directory("./Train", image_size=(178, 218))
+        validation = image_dataset_from_directory("./Validation", image_size=(178, 218))
+        test = image_dataset_from_directory("./Test", image_size=(178, 218))
 
         model.compile(loss='binary_crossentropy', optimizer="adam", metrics='accuracy')
 
         # Train your model using the custom early stopping callback
         model.fit(train, epochs=10, batch_size=32, validation_data=validation)
 
         # Evaluate the performance of the model on a validation set
```

### Comparing `gender-detection-local-0.0.4/README.md` & `gender-detection-local-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `gender-detection-local-0.0.4/setup.py` & `gender-detection-local-0.0.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
      name='gender-detection-local',  
-     version='0.0.4',
+     version='0.0.5',
      author="Circles",
      author_email="info@circles.zone",
      description="PyPI Package for gender detection",
      long_description="This is a package for running gender detection and predicting gender",
      long_description_content_type="text/markdown",
      url="https://github.com/circles-zone/gender-detection-local-python-package",
      packages=setuptools.find_packages(),
```

