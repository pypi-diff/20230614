# Comparing `tmp/GTNLib-0.1.tar.gz` & `tmp/GTNLib-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GTNLib-0.1.tar", last modified: Wed Jun 14 04:37:12 2023, max compression
+gzip compressed data, was "GTNLib-0.2.tar", last modified: Wed Jun 14 04:50:37 2023, max compression
```

## Comparing `GTNLib-0.1.tar` & `GTNLib-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 04:37:12.092908 GTNLib-0.1/
-drwxrwxrwx   0        0        0        0 2023-06-14 04:37:12.082915 GTNLib-0.1/GTNLib/
--rw-rw-rw-   0        0        0      161 2023-06-14 04:35:33.000000 GTNLib-0.1/GTNLib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 04:37:12.091905 GTNLib-0.1/GTNLib.egg-info/
--rw-rw-rw-   0        0        0      359 2023-06-14 04:37:11.000000 GTNLib-0.1/GTNLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2023-06-14 04:37:11.000000 GTNLib-0.1/GTNLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 04:37:11.000000 GTNLib-0.1/GTNLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-14 04:36:08.000000 GTNLib-0.1/GTNLib.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-06-14 04:37:11.000000 GTNLib-0.1/GTNLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-14 04:37:11.000000 GTNLib-0.1/GTNLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      359 2023-06-14 04:37:12.092908 GTNLib-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-14 04:37:12.093933 GTNLib-0.1/setup.cfg
--rw-rw-rw-   0        0        0      563 2023-06-14 04:37:07.000000 GTNLib-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 04:50:37.519832 GTNLib-0.2/
+drwxrwxrwx   0        0        0        0 2023-06-14 04:50:37.509832 GTNLib-0.2/GTNLib/
+-rw-rw-rw-   0        0        0      507 2023-06-14 04:50:27.000000 GTNLib-0.2/GTNLib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 04:50:37.518879 GTNLib-0.2/GTNLib.egg-info/
+-rw-rw-rw-   0        0        0      395 2023-06-14 04:50:37.000000 GTNLib-0.2/GTNLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2023-06-14 04:50:37.000000 GTNLib-0.2/GTNLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 04:50:37.000000 GTNLib-0.2/GTNLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-14 04:36:08.000000 GTNLib-0.2/GTNLib.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-06-14 04:50:37.000000 GTNLib-0.2/GTNLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-14 04:50:37.000000 GTNLib-0.2/GTNLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      395 2023-06-14 04:50:37.520832 GTNLib-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-14 04:50:37.521834 GTNLib-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      623 2023-06-14 04:50:32.000000 GTNLib-0.2/setup.py
```

### Comparing `GTNLib-0.1/setup.py` & `GTNLib-0.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(name='GTNLib',
-      version='0.1',
+      version='0.2',
       author="KeyDevS",
       packages=find_packages(),
-      description='Lib for project Guess The Number by KeyDevS (KeyDevelops)',
+      description='Lib for project Guess The Number',
+      long_description='Lib for project Guess The Number by KeyDevS (KeyDevelops)',
       author_email='rumaevvadim@gmail.com',
       install_requires=[
         'requests',
       ],
       classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

