# Comparing `tmp/ProjectAssessment-0.3.0.tar.gz` & `tmp/ProjectAssessment-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProjectAssessment-0.3.0.tar", last modified: Wed Jun 14 20:04:59 2023, max compression
+gzip compressed data, was "ProjectAssessment-0.3.1.tar", last modified: Wed Jun 14 20:53:27 2023, max compression
```

## Comparing `ProjectAssessment-0.3.0.tar` & `ProjectAssessment-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tazz       (501) staff       (20)        0 2023-06-14 20:04:59.928745 ProjectAssessment-0.3.0/
--rw-r--r--   0 tazz       (501) staff       (20)     1066 2022-06-04 12:11:30.000000 ProjectAssessment-0.3.0/LICENSE
--rw-r--r--   0 tazz       (501) staff       (20)      831 2023-06-14 20:04:59.928652 ProjectAssessment-0.3.0/PKG-INFO
-drwxr-xr-x   0 tazz       (501) staff       (20)        0 2023-06-14 20:04:59.927766 ProjectAssessment-0.3.0/ProjectAssessment/
--rw-r--r--   0 tazz       (501) staff       (20)       99 2022-06-29 18:35:17.000000 ProjectAssessment-0.3.0/ProjectAssessment/MakeTable.py
--rw-r--r--   0 tazz       (501) staff       (20)     4659 2023-06-14 19:59:55.000000 ProjectAssessment-0.3.0/ProjectAssessment/Marginal.py
--rw-r--r--   0 tazz       (501) staff       (20)    21282 2023-06-14 19:59:55.000000 ProjectAssessment-0.3.0/ProjectAssessment/Solver.py
--rw-r--r--   0 tazz       (501) staff       (20)       84 2022-12-16 11:54:15.000000 ProjectAssessment-0.3.0/ProjectAssessment/__init__.py
-drwxr-xr-x   0 tazz       (501) staff       (20)        0 2023-06-14 20:04:59.928504 ProjectAssessment-0.3.0/ProjectAssessment.egg-info/
--rw-r--r--   0 tazz       (501) staff       (20)      831 2023-06-14 20:04:59.000000 ProjectAssessment-0.3.0/ProjectAssessment.egg-info/PKG-INFO
--rw-r--r--   0 tazz       (501) staff       (20)      349 2023-06-14 20:04:59.000000 ProjectAssessment-0.3.0/ProjectAssessment.egg-info/SOURCES.txt
--rw-r--r--   0 tazz       (501) staff       (20)        1 2023-06-14 20:04:59.000000 ProjectAssessment-0.3.0/ProjectAssessment.egg-info/dependency_links.txt
--rw-r--r--   0 tazz       (501) staff       (20)       60 2023-06-14 20:04:59.000000 ProjectAssessment-0.3.0/ProjectAssessment.egg-info/requires.txt
--rw-r--r--   0 tazz       (501) staff       (20)       18 2023-06-14 20:04:59.000000 ProjectAssessment-0.3.0/ProjectAssessment.egg-info/top_level.txt
--rw-r--r--   0 tazz       (501) staff       (20)     6770 2023-06-14 19:59:55.000000 ProjectAssessment-0.3.0/README.md
--rw-r--r--   0 tazz       (501) staff       (20)       38 2023-06-14 20:04:59.928781 ProjectAssessment-0.3.0/setup.cfg
--rw-r--r--   0 tazz       (501) staff       (20)     1082 2023-06-14 19:59:55.000000 ProjectAssessment-0.3.0/setup.py
+drwxr-xr-x   0 tazz       (501) staff       (20)        0 2023-06-14 20:53:27.735282 ProjectAssessment-0.3.1/
+-rw-r--r--   0 tazz       (501) staff       (20)     1066 2022-06-04 12:11:30.000000 ProjectAssessment-0.3.1/LICENSE
+-rw-r--r--   0 tazz       (501) staff       (20)      831 2023-06-14 20:53:27.735189 ProjectAssessment-0.3.1/PKG-INFO
+drwxr-xr-x   0 tazz       (501) staff       (20)        0 2023-06-14 20:53:27.734521 ProjectAssessment-0.3.1/ProjectAssessment/
+-rw-r--r--   0 tazz       (501) staff       (20)       99 2022-06-29 18:35:17.000000 ProjectAssessment-0.3.1/ProjectAssessment/MakeTable.py
+-rw-r--r--   0 tazz       (501) staff       (20)     4659 2023-06-14 19:59:55.000000 ProjectAssessment-0.3.1/ProjectAssessment/Marginal.py
+-rw-r--r--   0 tazz       (501) staff       (20)    21282 2023-06-14 19:59:55.000000 ProjectAssessment-0.3.1/ProjectAssessment/Solver.py
+-rw-r--r--   0 tazz       (501) staff       (20)       83 2023-06-14 20:49:14.000000 ProjectAssessment-0.3.1/ProjectAssessment/__init__.py
+drwxr-xr-x   0 tazz       (501) staff       (20)        0 2023-06-14 20:53:27.735042 ProjectAssessment-0.3.1/ProjectAssessment.egg-info/
+-rw-r--r--   0 tazz       (501) staff       (20)      831 2023-06-14 20:53:27.000000 ProjectAssessment-0.3.1/ProjectAssessment.egg-info/PKG-INFO
+-rw-r--r--   0 tazz       (501) staff       (20)      349 2023-06-14 20:53:27.000000 ProjectAssessment-0.3.1/ProjectAssessment.egg-info/SOURCES.txt
+-rw-r--r--   0 tazz       (501) staff       (20)        1 2023-06-14 20:53:27.000000 ProjectAssessment-0.3.1/ProjectAssessment.egg-info/dependency_links.txt
+-rw-r--r--   0 tazz       (501) staff       (20)       60 2023-06-14 20:53:27.000000 ProjectAssessment-0.3.1/ProjectAssessment.egg-info/requires.txt
+-rw-r--r--   0 tazz       (501) staff       (20)       18 2023-06-14 20:53:27.000000 ProjectAssessment-0.3.1/ProjectAssessment.egg-info/top_level.txt
+-rw-r--r--   0 tazz       (501) staff       (20)     6770 2023-06-14 19:59:55.000000 ProjectAssessment-0.3.1/README.md
+-rw-r--r--   0 tazz       (501) staff       (20)       38 2023-06-14 20:53:27.735317 ProjectAssessment-0.3.1/setup.cfg
+-rw-r--r--   0 tazz       (501) staff       (20)     1082 2023-06-14 20:49:28.000000 ProjectAssessment-0.3.1/setup.py
```

### Comparing `ProjectAssessment-0.3.0/LICENSE` & `ProjectAssessment-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ProjectAssessment-0.3.0/PKG-INFO` & `ProjectAssessment-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ProjectAssessment
-Version: 0.3.0
+Version: 0.3.1
 Summary: Package to compute the Project-Based Assessment estimates of student and rubric proficiency.
 Home-page: https://github.com/tazzben/project-based-assessment
-Download-URL: https://github.com/tazzben/project-based-assessment/archive/v0.3.0.tar.gz
+Download-URL: https://github.com/tazzben/project-based-assessment/archive/v0.3.1.tar.gz
 Author: Ben Smith
 Author-email: bosmith@unomaha.edu
 License: MIT
 Keywords: Assessment,Projects,Statistics,Education,Bootstrap
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ProjectAssessment-0.3.0/ProjectAssessment/Marginal.py` & `ProjectAssessment-0.3.1/ProjectAssessment/Marginal.py`

 * *Files identical despite different names*

### Comparing `ProjectAssessment-0.3.0/ProjectAssessment/Solver.py` & `ProjectAssessment-0.3.1/ProjectAssessment/Solver.py`

 * *Files identical despite different names*

### Comparing `ProjectAssessment-0.3.0/ProjectAssessment.egg-info/PKG-INFO` & `ProjectAssessment-0.3.1/ProjectAssessment.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ProjectAssessment
-Version: 0.3.0
+Version: 0.3.1
 Summary: Package to compute the Project-Based Assessment estimates of student and rubric proficiency.
 Home-page: https://github.com/tazzben/project-based-assessment
-Download-URL: https://github.com/tazzben/project-based-assessment/archive/v0.3.0.tar.gz
+Download-URL: https://github.com/tazzben/project-based-assessment/archive/v0.3.1.tar.gz
 Author: Ben Smith
 Author-email: bosmith@unomaha.edu
 License: MIT
 Keywords: Assessment,Projects,Statistics,Education,Bootstrap
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ProjectAssessment-0.3.0/README.md` & `ProjectAssessment-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ProjectAssessment-0.3.0/setup.py` & `ProjectAssessment-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 
 setup(
     name='ProjectAssessment',
-    version='0.3.0',
+    version='0.3.1',
     packages=['ProjectAssessment',],
     python_requires='>3.7.0',
     license='MIT',
     install_requires=[
         'numpy>=1.21.0',
         'pandas>=1.3.0',
         'tqdm',
@@ -22,10 +22,10 @@
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.7',
     ],
     keywords = ['Assessment', 'Projects', 'Statistics', 'Education', 'Bootstrap'],
     url = 'https://github.com/tazzben/project-based-assessment',
-    download_url = 'https://github.com/tazzben/project-based-assessment/archive/v0.3.0.tar.gz',
+    download_url = 'https://github.com/tazzben/project-based-assessment/archive/v0.3.1.tar.gz',
     description = 'Package to compute the Project-Based Assessment estimates of student and rubric proficiency.',
 )
```

