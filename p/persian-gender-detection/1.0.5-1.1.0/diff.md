# Comparing `tmp/persian-gender-detection-1.0.5.tar.gz` & `tmp/persian-gender-detection-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "persian-gender-detection-1.0.5.tar", last modified: Wed Jun  7 16:53:52 2023, max compression
+gzip compressed data, was "persian-gender-detection-1.1.0.tar", last modified: Wed Jun 14 06:13:03 2023, max compression
```

## Comparing `persian-gender-detection-1.0.5.tar` & `persian-gender-detection-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-07 16:53:52.596580 persian-gender-detection-1.0.5/
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     1068 2023-06-07 16:19:28.000000 persian-gender-detection-1.0.5/LICENSE
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     2249 2023-06-07 16:53:52.596580 persian-gender-detection-1.0.5/PKG-INFO
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)      931 2023-06-07 16:31:09.000000 persian-gender-detection-1.0.5/README.md
-drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-07 16:53:52.588580 persian-gender-detection-1.0.5/persian_gender_detection/
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)       40 2023-06-07 16:13:42.000000 persian-gender-detection-1.0.5/persian_gender_detection/__init__.py
-drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-07 16:53:52.592580 persian-gender-detection-1.0.5/persian_gender_detection/gender/
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)   135092 2023-06-05 10:24:08.000000 persian-gender-detection-1.0.5/persian_gender_detection/gender/female.json
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)   125412 2023-06-07 15:15:48.000000 persian-gender-detection-1.0.5/persian_gender_detection/gender/male.json
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)   116646 2023-06-05 10:24:08.000000 persian-gender-detection-1.0.5/persian_gender_detection/gender/names.csv
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)      956 2023-06-07 16:52:33.000000 persian-gender-detection-1.0.5/persian_gender_detection/persian_gender_detection.py
-drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-07 16:53:52.592580 persian-gender-detection-1.0.5/persian_gender_detection.egg-info/
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     2249 2023-06-07 16:53:52.000000 persian-gender-detection-1.0.5/persian_gender_detection.egg-info/PKG-INFO
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)      484 2023-06-07 16:53:52.000000 persian-gender-detection-1.0.5/persian_gender_detection.egg-info/SOURCES.txt
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)        1 2023-06-07 16:53:52.000000 persian-gender-detection-1.0.5/persian_gender_detection.egg-info/dependency_links.txt
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)       25 2023-06-07 16:53:52.000000 persian-gender-detection-1.0.5/persian_gender_detection.egg-info/top_level.txt
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)       38 2023-06-07 16:53:52.596580 persian-gender-detection-1.0.5/setup.cfg
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     1759 2023-06-07 16:52:41.000000 persian-gender-detection-1.0.5/setup.py
-drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-07 16:53:52.596580 persian-gender-detection-1.0.5/test/
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     1438 2023-06-07 16:03:13.000000 persian-gender-detection-1.0.5/test/test_clean_name.py
--rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     1874 2023-06-07 16:03:13.000000 persian-gender-detection-1.0.5/test/test_get_gender.py
+drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-14 06:13:03.499870 persian-gender-detection-1.1.0/
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     1068 2023-06-07 16:19:28.000000 persian-gender-detection-1.1.0/LICENSE
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     2251 2023-06-14 06:13:03.499870 persian-gender-detection-1.1.0/PKG-INFO
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)      932 2023-06-12 09:45:11.000000 persian-gender-detection-1.1.0/README.md
+drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-14 06:13:03.483870 persian-gender-detection-1.1.0/persian_gender_detection/
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)       40 2023-06-07 16:13:42.000000 persian-gender-detection-1.1.0/persian_gender_detection/__init__.py
+drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-14 06:13:03.495870 persian-gender-detection-1.1.0/persian_gender_detection/gender/
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)   410371 2023-06-08 06:15:17.000000 persian-gender-detection-1.1.0/persian_gender_detection/gender/iranianNamesDataset.csv
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)   436494 2023-06-12 09:12:51.000000 persian-gender-detection-1.1.0/persian_gender_detection/gender/iranianNamesDataset.py
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)      923 2023-06-12 09:38:15.000000 persian-gender-detection-1.1.0/persian_gender_detection/persian_gender_detection.py
+drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-14 06:13:03.487870 persian-gender-detection-1.1.0/persian_gender_detection.egg-info/
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     2251 2023-06-14 06:13:03.000000 persian-gender-detection-1.1.0/persian_gender_detection.egg-info/PKG-INFO
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)      467 2023-06-14 06:13:03.000000 persian-gender-detection-1.1.0/persian_gender_detection.egg-info/SOURCES.txt
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)        1 2023-06-14 06:13:03.000000 persian-gender-detection-1.1.0/persian_gender_detection.egg-info/dependency_links.txt
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)       25 2023-06-14 06:13:03.000000 persian-gender-detection-1.1.0/persian_gender_detection.egg-info/top_level.txt
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)       38 2023-06-14 06:13:03.499870 persian-gender-detection-1.1.0/setup.cfg
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     1732 2023-06-14 06:12:52.000000 persian-gender-detection-1.1.0/setup.py
+drwxrwxr-x   0 mehraban  (1000) mehraban  (1000)        0 2023-06-14 06:13:03.499870 persian-gender-detection-1.1.0/test/
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     1438 2023-06-07 16:03:13.000000 persian-gender-detection-1.1.0/test/test_clean_name.py
+-rw-rw-r--   0 mehraban  (1000) mehraban  (1000)     1940 2023-06-12 09:31:58.000000 persian-gender-detection-1.1.0/test/test_get_gender.py
```

### Comparing `persian-gender-detection-1.0.5/LICENSE` & `persian-gender-detection-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `persian-gender-detection-1.0.5/PKG-INFO` & `persian-gender-detection-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: persian-gender-detection
-Version: 1.0.5
-Summary: A simple python package to detect gender by Persian first name. (With more than 6K names).
+Version: 1.1.0
+Summary: A simple python package to detect gender by Persian first name. (With more than 19K names).
 Home-page: https://github.com/zeoses/persian-gender-detection
 Author: Mehraban
 License: MIT License
 Project-URL: Source, https://github.com/zeoses/persian-gender-detection
 Project-URL: Documentation, https://github.com/zeoses/persian-gender-detection
 Keywords: persian-gender-detection,farsi gender,iranian gender,name gender,persian gender detection,gender detection
 Classifier: License :: OSI Approved :: MIT License
@@ -23,15 +23,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Localization
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Persian Gender Detection
 
-A simple python package to detect gender by Persian first name. (With more than 6K names)
+A simple python package to detect gender by Persian first name. (With more than 19K names)
 
 for this package i use this [repo](https://github.com/peymanslh/persian-gender-detection/) if you are use NPM that's great choice.
 
 Installation
 ------
 Install with PIP:
```

### Comparing `persian-gender-detection-1.0.5/README.md` & `persian-gender-detection-1.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Persian Gender Detection
 
-A simple python package to detect gender by Persian first name. (With more than 6K names)
+A simple python package to detect gender by Persian first name. (With more than 19K names)
 
 for this package i use this [repo](https://github.com/peymanslh/persian-gender-detection/) if you are use NPM that's great choice.
 
 Installation
 ------
 Install with PIP:
```

### Comparing `persian-gender-detection-1.0.5/persian_gender_detection.egg-info/PKG-INFO` & `persian-gender-detection-1.1.0/persian_gender_detection.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: persian-gender-detection
-Version: 1.0.5
-Summary: A simple python package to detect gender by Persian first name. (With more than 6K names).
+Version: 1.1.0
+Summary: A simple python package to detect gender by Persian first name. (With more than 19K names).
 Home-page: https://github.com/zeoses/persian-gender-detection
 Author: Mehraban
 License: MIT License
 Project-URL: Source, https://github.com/zeoses/persian-gender-detection
 Project-URL: Documentation, https://github.com/zeoses/persian-gender-detection
 Keywords: persian-gender-detection,farsi gender,iranian gender,name gender,persian gender detection,gender detection
 Classifier: License :: OSI Approved :: MIT License
@@ -23,15 +23,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Localization
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Persian Gender Detection
 
-A simple python package to detect gender by Persian first name. (With more than 6K names)
+A simple python package to detect gender by Persian first name. (With more than 19K names)
 
 for this package i use this [repo](https://github.com/peymanslh/persian-gender-detection/) if you are use NPM that's great choice.
 
 Installation
 ------
 Install with PIP:
```

### Comparing `persian-gender-detection-1.0.5/setup.py` & `persian-gender-detection-1.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from setuptools import setup
 
 with open('./README.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='persian-gender-detection',
-    version='1.0.5',
+    version='1.1.0',
     packages=['persian_gender_detection'],
     include_package_data=True,
     data_files=[('', [
-        'persian_gender_detection/gender/female.json',
-        'persian_gender_detection/gender/male.json',
-        'persian_gender_detection/gender/names.csv',
+        'persian_gender_detection/gender/iranianNamesDataset.py',
+        'persian_gender_detection/gender/iranianNamesDataset.csv',
     ])],
     url='https://github.com/zeoses/persian-gender-detection',
     license='MIT License',
     author='Mehraban',
-    description='A simple python package to detect gender by Persian first name. (With more than 6K names).',
+    description='A simple python package to detect gender by Persian first name. (With more than 19K names).',
     long_description=readme,
     long_description_content_type='text/markdown',
     keywords='persian-gender-detection, farsi gender, iranian gender, name gender, persian gender detection, gender detection',
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Natural Language :: Persian',
         'Natural Language :: English',
```

### Comparing `persian-gender-detection-1.0.5/test/test_clean_name.py` & `persian-gender-detection-1.1.0/test/test_clean_name.py`

 * *Files identical despite different names*

### Comparing `persian-gender-detection-1.0.5/test/test_get_gender.py` & `persian-gender-detection-1.1.0/test/test_get_gender.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import unittest
 from persian_gender_detection.persian_gender_detection import get_gender
 
 
 class TestCleanName(unittest.TestCase):
 
     def test_detect_male(self):
+        self.assertEqual(get_gender('محمدمسیحا'), 'MALE')
         self.assertEqual(get_gender('علي'), 'MALE')
         self.assertEqual(get_gender('مسیحا'), 'MALE')
         self.assertEqual(get_gender('سعید     '), 'MALE')
         self.assertEqual(get_gender('هــــادی'), 'MALE')
         self.assertEqual(get_gender('محمد   رضا'), 'MALE')
         self.assertEqual(get_gender('احسا   ن'), 'MALE')
         self.assertEqual(get_gender('كامران'), 'MALE')
@@ -22,20 +23,20 @@
         self.assertEqual(get_gender('آذر     '), 'FEMALE')
         self.assertEqual(get_gender('الـــناز'), 'FEMALE')
         self.assertEqual(get_gender('فاطمه زهرا'), 'FEMALE')
         self.assertEqual(get_gender('یلـــ❤️ــدا'), 'FEMALE')
         self.assertEqual(get_gender('  مریم  '), 'FEMALE')
         self.assertEqual(get_gender('صغری'), 'FEMALE')
         self.assertEqual(get_gender('حانیه'), 'FEMALE')
-        self.assertEqual(get_gender('هانیه'), 'FEMALE')
+        self.assertEqual(get_gender('جانان'), 'FEMALE')
         self.assertEqual(get_gender('۱۲۳مهناز۱۲۳'), 'FEMALE')
+        self.assertEqual(get_gender('فاطی'), 'FEMALE')
 
 
     def test_detect_unkown(self):
-        self.assertEqual(get_gender('فاطی'), 'UNKNOWN')
         self.assertEqual(get_gender('(فاطمه)'), 'UNKNOWN')
         self.assertEqual(get_gender('fateme'), 'UNKNOWN')
         self.assertEqual(get_gender('Ali'), 'UNKNOWN')
 
 if __name__=='__main__':
   unittest.main()
```

