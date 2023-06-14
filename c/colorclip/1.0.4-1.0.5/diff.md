# Comparing `tmp/colorclip-1.0.4.tar.gz` & `tmp/colorclip-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorclip-1.0.4.tar", last modified: Tue Jun 13 15:09:06 2023, max compression
+gzip compressed data, was "colorclip-1.0.5.tar", last modified: Tue Jun 13 17:17:48 2023, max compression
```

## Comparing `colorclip-1.0.4.tar` & `colorclip-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-13 15:09:06.724513 colorclip-1.0.4/
--rw-rw----   0 root         (0) everybody  (9997)     1067 2023-06-12 23:46:56.000000 colorclip-1.0.4/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)       16 2023-06-13 12:05:40.000000 colorclip-1.0.4/MANIFEST.in
--rw-rw----   0 root         (0) everybody  (9997)     1002 2023-06-13 15:09:06.716513 colorclip-1.0.4/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      478 2023-06-13 15:05:36.000000 colorclip-1.0.4/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-13 15:09:06.632513 colorclip-1.0.4/colorclip/
--rw-rw----   0 root         (0) everybody  (9997)       24 2023-06-12 05:58:17.000000 colorclip-1.0.4/colorclip/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     6831 2023-06-13 12:15:40.000000 colorclip-1.0.4/colorclip/colorclip.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-13 15:09:06.708514 colorclip-1.0.4/colorclip.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     1002 2023-06-13 15:09:06.000000 colorclip-1.0.4/colorclip.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      215 2023-06-13 15:09:06.000000 colorclip-1.0.4/colorclip.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-13 15:09:06.000000 colorclip-1.0.4/colorclip.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       10 2023-06-13 15:09:06.000000 colorclip-1.0.4/colorclip.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-13 15:09:06.724513 colorclip-1.0.4/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      706 2023-06-13 15:08:21.000000 colorclip-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:17:48.061857 colorclip-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-13 17:17:35.000000 colorclip-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-13 17:17:35.000000 colorclip-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-13 17:17:48.061857 colorclip-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-13 17:17:35.000000 colorclip-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:17:48.061857 colorclip-1.0.5/colorclip/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-13 17:17:35.000000 colorclip-1.0.5/colorclip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-13 17:17:35.000000 colorclip-1.0.5/colorclip/colorclip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:17:48.061857 colorclip-1.0.5/colorclip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-13 17:17:48.000000 colorclip-1.0.5/colorclip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-13 17:17:48.000000 colorclip-1.0.5/colorclip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:17:48.000000 colorclip-1.0.5/colorclip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-13 17:17:48.000000 colorclip-1.0.5/colorclip.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 17:17:48.061857 colorclip-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-13 17:17:35.000000 colorclip-1.0.5/setup.py
```

### Comparing `colorclip-1.0.4/LICENSE` & `colorclip-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `colorclip-1.0.4/PKG-INFO` & `colorclip-1.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: colorclip
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python color pack library
 Home-page: https://t.me/Onefinalhug
+Download-URL: https://github.com/lillisfeb/colorclip
 Author: Bevlil
 Author-email: voidlillis@gmail.com
 License: MIT
-Download-URL: https://github.com/lillisfeb/colorclip
 Keywords: color pack library,python terminal console
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-# colorclip 1.0.4
+# colorclip 1.0.5
 
 ![Colorclip](https://i.ibb.co/4pKgVFf/Screenshot-2023-06-13-18-33-16-81-e4424258c8b8649f6e67d283a50a2cbc.jpg)
 
 Color pack library,python terminal console
 
 ### Installation
 ```
@@ -44,10 +43,9 @@
 ```
 p_ac()
 ```
 Help
 ```
 help()
 ```
-AND MORE
-
-
+CONTACT 
+[TELEGRAM](https://t.me/Onefinalhug)
```

### Comparing `colorclip-1.0.4/colorclip/colorclip.py` & `colorclip-1.0.5/colorclip/colorclip.py`

 * *Files identical despite different names*

### Comparing `colorclip-1.0.4/colorclip.egg-info/PKG-INFO` & `colorclip-1.0.5/colorclip.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: colorclip
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python color pack library
 Home-page: https://t.me/Onefinalhug
+Download-URL: https://github.com/lillisfeb/colorclip
 Author: Bevlil
 Author-email: voidlillis@gmail.com
 License: MIT
-Download-URL: https://github.com/lillisfeb/colorclip
 Keywords: color pack library,python terminal console
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-# colorclip 1.0.4
+# colorclip 1.0.5
 
 ![Colorclip](https://i.ibb.co/4pKgVFf/Screenshot-2023-06-13-18-33-16-81-e4424258c8b8649f6e67d283a50a2cbc.jpg)
 
 Color pack library,python terminal console
 
 ### Installation
 ```
@@ -44,10 +43,9 @@
 ```
 p_ac()
 ```
 Help
 ```
 help()
 ```
-AND MORE
-
-
+CONTACT 
+[TELEGRAM](https://t.me/Onefinalhug)
```

### Comparing `colorclip-1.0.4/setup.py` & `colorclip-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='colorclip',
-    version='1.0.4',
+    version='1.0.5',
     author='Bevlil',
     author_email='voidlillis@gmail.com', 
     packages=find_packages(),
     py_modules=['colorclip'],
     url='https://t.me/Onefinalhug',
     download_url='https://github.com/lillisfeb/colorclip',
     description='A Python color pack library',
```

