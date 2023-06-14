# Comparing `tmp/phenocam-snow-0.1.0.tar.gz` & `tmp/phenocam-snow-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/jason/Development/PhenoCamSnow/dist/.tmp-33s2v83s/phenocam-snow-0.1.0.tar", last modified: Thu May 25 02:08:12 2023, max compression
+gzip compressed data, was "/home/jason/Development/PhenoCamSnow/dist/.tmp-_nffzkzd/phenocam-snow-0.1.1.tar", last modified: Wed Jun 14 21:44:42 2023, max compression
```

## Comparing `phenocam-snow-0.1.0.tar` & `phenocam-snow-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-05-25 02:08:12.000000 phenocam-snow-0.1.0/
--rw-r--r--   0 jason     (1000) jason     (1000)     1068 2023-05-08 01:52:37.000000 phenocam-snow-0.1.0/LICENSE
--rw-r--r--   0 jason     (1000) jason     (1000)     3307 2023-05-25 02:08:12.000000 phenocam-snow-0.1.0/PKG-INFO
--rw-r--r--   0 jason     (1000) jason     (1000)     1849 2023-05-25 02:05:18.000000 phenocam-snow-0.1.0/README.md
--rw-r--r--   0 jason     (1000) jason     (1000)     1904 2023-05-25 02:06:22.000000 phenocam-snow-0.1.0/pyproject.toml
--rw-r--r--   0 jason     (1000) jason     (1000)       38 2023-05-25 02:08:12.000000 phenocam-snow-0.1.0/setup.cfg
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-05-25 02:08:12.000000 phenocam-snow-0.1.0/src/
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-05-25 02:08:12.000000 phenocam-snow-0.1.0/src/phenocam_snow/
--rw-r--r--   0 jason     (1000) jason     (1000)        0 2023-05-08 01:52:37.000000 phenocam-snow-0.1.0/src/phenocam_snow/__init__.py
--rw-r--r--   0 jason     (1000) jason     (1000)     8000 2023-05-08 01:52:37.000000 phenocam-snow-0.1.0/src/phenocam_snow/data.py
--rw-r--r--   0 jason     (1000) jason     (1000)     3312 2023-05-24 21:51:46.000000 phenocam-snow-0.1.0/src/phenocam_snow/model.py
--rw-r--r--   0 jason     (1000) jason     (1000)     6201 2023-05-25 02:05:18.000000 phenocam-snow-0.1.0/src/phenocam_snow/predict.py
--rw-r--r--   0 jason     (1000) jason     (1000)     9616 2023-05-25 02:05:18.000000 phenocam-snow-0.1.0/src/phenocam_snow/train.py
--rw-r--r--   0 jason     (1000) jason     (1000)    12009 2023-05-08 01:52:37.000000 phenocam-snow-0.1.0/src/phenocam_snow/utils.py
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-05-25 02:08:12.000000 phenocam-snow-0.1.0/src/phenocam_snow.egg-info/
--rw-r--r--   0 jason     (1000) jason     (1000)     3307 2023-05-25 02:08:12.000000 phenocam-snow-0.1.0/src/phenocam_snow.egg-info/PKG-INFO
--rw-r--r--   0 jason     (1000) jason     (1000)      402 2023-05-25 02:08:12.000000 phenocam-snow-0.1.0/src/phenocam_snow.egg-info/SOURCES.txt
--rw-r--r--   0 jason     (1000) jason     (1000)        1 2023-05-25 02:08:12.000000 phenocam-snow-0.1.0/src/phenocam_snow.egg-info/dependency_links.txt
--rw-r--r--   0 jason     (1000) jason     (1000)      316 2023-05-25 02:08:12.000000 phenocam-snow-0.1.0/src/phenocam_snow.egg-info/requires.txt
--rw-r--r--   0 jason     (1000) jason     (1000)       14 2023-05-25 02:08:12.000000 phenocam-snow-0.1.0/src/phenocam_snow.egg-info/top_level.txt
+drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-06-14 21:44:42.000000 phenocam-snow-0.1.1/
+-rw-r--r--   0 jason     (1000) jason     (1000)     1068 2023-05-08 01:52:37.000000 phenocam-snow-0.1.1/LICENSE
+-rw-r--r--   0 jason     (1000) jason     (1000)     3307 2023-06-14 21:44:42.000000 phenocam-snow-0.1.1/PKG-INFO
+-rw-r--r--   0 jason     (1000) jason     (1000)     1849 2023-05-25 02:05:18.000000 phenocam-snow-0.1.1/README.md
+-rw-r--r--   0 jason     (1000) jason     (1000)     1904 2023-06-14 21:43:52.000000 phenocam-snow-0.1.1/pyproject.toml
+-rw-r--r--   0 jason     (1000) jason     (1000)       38 2023-06-14 21:44:42.000000 phenocam-snow-0.1.1/setup.cfg
+drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-06-14 21:44:42.000000 phenocam-snow-0.1.1/src/
+drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-06-14 21:44:42.000000 phenocam-snow-0.1.1/src/phenocam_snow/
+-rw-r--r--   0 jason     (1000) jason     (1000)        0 2023-05-08 01:52:37.000000 phenocam-snow-0.1.1/src/phenocam_snow/__init__.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     8000 2023-05-08 01:52:37.000000 phenocam-snow-0.1.1/src/phenocam_snow/data.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     1716 2023-06-14 21:29:36.000000 phenocam-snow-0.1.1/src/phenocam_snow/get_all_images.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     3312 2023-05-24 21:51:46.000000 phenocam-snow-0.1.1/src/phenocam_snow/model.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     6595 2023-06-14 21:42:04.000000 phenocam-snow-0.1.1/src/phenocam_snow/predict.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     9616 2023-05-25 02:05:18.000000 phenocam-snow-0.1.1/src/phenocam_snow/train.py
+-rw-r--r--   0 jason     (1000) jason     (1000)    12009 2023-05-08 01:52:37.000000 phenocam-snow-0.1.1/src/phenocam_snow/utils.py
+drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-06-14 21:44:42.000000 phenocam-snow-0.1.1/src/phenocam_snow.egg-info/
+-rw-r--r--   0 jason     (1000) jason     (1000)     3307 2023-06-14 21:44:42.000000 phenocam-snow-0.1.1/src/phenocam_snow.egg-info/PKG-INFO
+-rw-r--r--   0 jason     (1000) jason     (1000)      438 2023-06-14 21:44:42.000000 phenocam-snow-0.1.1/src/phenocam_snow.egg-info/SOURCES.txt
+-rw-r--r--   0 jason     (1000) jason     (1000)        1 2023-06-14 21:44:42.000000 phenocam-snow-0.1.1/src/phenocam_snow.egg-info/dependency_links.txt
+-rw-r--r--   0 jason     (1000) jason     (1000)      316 2023-06-14 21:44:42.000000 phenocam-snow-0.1.1/src/phenocam_snow.egg-info/requires.txt
+-rw-r--r--   0 jason     (1000) jason     (1000)       14 2023-06-14 21:44:42.000000 phenocam-snow-0.1.1/src/phenocam_snow.egg-info/top_level.txt
```

### Comparing `phenocam-snow-0.1.0/LICENSE` & `phenocam-snow-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `phenocam-snow-0.1.0/PKG-INFO` & `phenocam-snow-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phenocam-snow
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pipeline for building deep learning models to classify PhenoCam images.
 Author-email: Jason Jewik <jason.jewik@cs.ucla.edu>
 Project-URL: Source, https://github.com/jasonjewik/PhenoCamSnowClassifier
 Project-URL: Issue Tracker, https://github.com/jasonjewik/PhenoCamSnowClassifier/issues
 Project-URL: Documentation, https://phenocamsnow.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phenocam-snow-0.1.0/README.md` & `phenocam-snow-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `phenocam-snow-0.1.0/pyproject.toml` & `phenocam-snow-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "phenocam-snow"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     { name = "Jason Jewik", email = "jason.jewik@cs.ucla.edu" }
 ]
 description = "Pipeline for building deep learning models to classify PhenoCam images."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `phenocam-snow-0.1.0/src/phenocam_snow/data.py` & `phenocam-snow-0.1.1/src/phenocam_snow/data.py`

 * *Files identical despite different names*

### Comparing `phenocam-snow-0.1.0/src/phenocam_snow/model.py` & `phenocam-snow-0.1.1/src/phenocam_snow/model.py`

 * *Files identical despite different names*

### Comparing `phenocam-snow-0.1.0/src/phenocam_snow/predict.py` & `phenocam-snow-0.1.1/src/phenocam_snow/predict.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Standard library imports
 from argparse import ArgumentParser
+import os
 
 # Local application imports
 from .data import *
 from .model import *
 from .utils import *
 
 # Third party imports
 import numpy as np
 import pandas as pd
 from PIL import Image
 import torch
-import torchvision.transforms as transforms
 
 
 def main():
     parser = ArgumentParser(description="Predicts image category using the given model")
     parser.add_argument(
         "site_name", help="The PhenoCam site for which we are generating predictions."
     )
@@ -30,26 +30,28 @@
     )
     parser.add_argument(
         "--directory",
         default=None,
         help="Provide this if you want to get predictions for all \
                             images in a local directory.",
     )
+    parser.add_argument(
+        "--urls",
+        default=None,
+        help="A file containing URLs, one per line."
+    )
     args = parser.parse_args()
 
-    if args.url and args.directory:
-        print("Cannot specify both --url and --directory")
-    elif not (args.url or args.directory):
-        print("Please specify either --url or --directory")
-    else:
-        model = load_model_from_file(args.model_path, args.resnet, len(args.categories))
-        if args.url:
-            run_model_online(model, args.site_name, args.categories, args.url)
-        elif args.directory:
-            run_model_offline(model, args.site_name, args.categories, args.directory)
+    model = load_model_from_file(args.model_path, args.resnet, len(args.categories))
+    if args.url:
+        run_model_online(model, args.site_name, args.categories, args.url)
+    elif args.urls:
+        run_model_online(model, args.site_name, args.categories, args.urls)
+    elif args.directory:
+        run_model_offline(model, args.site_name, args.categories, args.directory)
 
 
 def classify_online(model, categories, img_url):
     """Performs online classification.
 
     :param model: The model to use.
     :type model: PhenoCamResNet
@@ -136,57 +138,62 @@
     :param site_name: The name of the PhenoCam site.
     :type site_name: str
     :param img_dir: The directory containing the images to classify.
     :type img_dir: str
     :return: A pandas DataFrame with predictions.
     :rtype: pd.DataFrame
     """
-    ######################
-    # 1. Get predictions #
-    ######################
+    # Get predictions
     if type(img_dir) is str:
         img_dir = Path(img_dir)
     timestamps, predictions = [], []
     for img_path in img_dir.glob("*.jpg"):
         ts_arr = img_path.stem.split("_")
         ts = "-".join(ts_arr[1:4])
         hms = ts_arr[-1]
         ts += f" {hms[:2]}:{hms[2:4]}:{hms[4:]}"
         timestamps.append(ts)
         predictions.append(classify_offline(model, categories, str(img_path)))
 
-    ###################
-    # 2. Save to file #
-    ###################
+    # Save to file
     df = pd.DataFrame(zip(timestamps, predictions), columns=["timestamp", "label"])
     save_to = img_dir.joinpath("predictions.csv")
     with open(save_to, "w+") as f:
         f.write(f"# Site: {site_name}\n")
         f.write("# Categories:\n")
         for i, cat in enumerate(categories):
             f.write(f"# {i}. {cat}\n")
     df.to_csv(save_to, mode="a", line_terminator="\n", index=False)
 
 
-def run_model_online(model, site_name, categories, img_url):
-    """Gets predicted labels for all images in a directory.
+def run_model_online(model, site_name, categories, urls):
+    """Gets predicted label for image online.
 
     :param model: The model to use.
     :type model: PhenoCamResNet
     :param site_name: The name of the PhenoCam site.
     :type site_name: str
-    :param img_url: The URL of the image for which you want a prediction.
-    :type img_url: str
+    :param url: The URL of the image for which you want a prediction, or the
+        name of a file containing all the URLs, one per line.
+    :type url: str
     """
-    ######################
-    # 1. Get predictions #
-    ######################
-    img, pred = classify_online(model, categories, img_url)
-
-    ###################
-    # 2. Print result #
-    ###################
-    print(pred)
+    if os.path.exists(urls):
+        with open(urls) as f:
+            links = [l.split() for l in f.readlines()]
+        predictions = []
+        for link in links:
+            predictions.append(classify_online(model, categories, link)[1])
+        df = pd.DataFrame(zip(links, predictions), columns=["image", "label"])
+        save_to = "predictions.csv"
+        with open(save_to, "w+") as f:
+            f.write(f"# Site: {site_name}\n")
+            f.write("# Categories:\n")
+            for i, cat in enumerate(categories):
+                f.write(f"# {i}. {cat}\n")
+        df.to_csv(save_to, mode="a", line_terminator="\n", index=False)
+    else:
+        _, pred = classify_online(model, categories, urls)
+        print(pred)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `phenocam-snow-0.1.0/src/phenocam_snow/train.py` & `phenocam-snow-0.1.1/src/phenocam_snow/train.py`

 * *Files identical despite different names*

### Comparing `phenocam-snow-0.1.0/src/phenocam_snow/utils.py` & `phenocam-snow-0.1.1/src/phenocam_snow/utils.py`

 * *Files identical despite different names*

### Comparing `phenocam-snow-0.1.0/src/phenocam_snow.egg-info/PKG-INFO` & `phenocam-snow-0.1.1/src/phenocam_snow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phenocam-snow
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pipeline for building deep learning models to classify PhenoCam images.
 Author-email: Jason Jewik <jason.jewik@cs.ucla.edu>
 Project-URL: Source, https://github.com/jasonjewik/PhenoCamSnowClassifier
 Project-URL: Issue Tracker, https://github.com/jasonjewik/PhenoCamSnowClassifier/issues
 Project-URL: Documentation, https://phenocamsnow.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

