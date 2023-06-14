# Comparing `tmp/dsm_django_masterdata-0.0.3.tar.gz` & `tmp/dsm_django_masterdata-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsm_django_masterdata-0.0.3.tar", last modified: Tue Jun 13 15:58:35 2023, max compression
+gzip compressed data, was "dsm_django_masterdata-0.0.4.tar", last modified: Wed Jun 14 04:00:11 2023, max compression
```

## Comparing `dsm_django_masterdata-0.0.3.tar` & `dsm_django_masterdata-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,30 @@
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-06-13 15:58:35.193173 dsm_django_masterdata-0.0.3/
--rw-r--r--   0 naii       (501) staff       (20)     1181 2023-06-13 15:58:35.192609 dsm_django_masterdata-0.0.3/PKG-INFO
--rw-r--r--   0 naii       (501) staff       (20)      572 2023-06-13 15:58:01.000000 dsm_django_masterdata-0.0.3/README.md
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-06-13 15:58:35.182496 dsm_django_masterdata-0.0.3/dsm_django_masterdata/
--rw-r--r--   0 naii       (501) staff       (20)      153 2023-06-13 15:58:26.000000 dsm_django_masterdata-0.0.3/dsm_django_masterdata/__init__.py
--rw-r--r--   0 naii       (501) staff       (20)      291 2023-06-13 15:49:04.000000 dsm_django_masterdata-0.0.3/dsm_django_masterdata/apps.py
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-06-13 15:58:35.188667 dsm_django_masterdata-0.0.3/dsm_django_masterdata/hscode/
--rw-r--r--   0 naii       (501) staff       (20)        0 2023-06-12 09:43:46.000000 dsm_django_masterdata-0.0.3/dsm_django_masterdata/hscode/__init__.py
--rw-r--r--   0 naii       (501) staff       (20)      327 2023-06-12 10:06:08.000000 dsm_django_masterdata-0.0.3/dsm_django_masterdata/hscode/admin.py
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-06-13 15:58:35.191670 dsm_django_masterdata-0.0.3/dsm_django_masterdata/hscode/migrations/
--rw-r--r--   0 naii       (501) staff       (20)     1110 2023-06-13 15:54:02.000000 dsm_django_masterdata-0.0.3/dsm_django_masterdata/hscode/migrations/0001_initial.py
--rw-r--r--   0 naii       (501) staff       (20)      337 2023-06-13 15:50:16.000000 dsm_django_masterdata-0.0.3/dsm_django_masterdata/hscode/migrations/0002_alter_hscode_options.py
--rw-r--r--   0 naii       (501) staff       (20)        0 2023-06-12 09:50:06.000000 dsm_django_masterdata-0.0.3/dsm_django_masterdata/hscode/migrations/__init__.py
--rw-r--r--   0 naii       (501) staff       (20)      395 2023-06-12 11:19:07.000000 dsm_django_masterdata-0.0.3/dsm_django_masterdata/hscode/models.py
--rw-r--r--   0 naii       (501) staff       (20)       60 2023-06-12 09:43:33.000000 dsm_django_masterdata-0.0.3/dsm_django_masterdata/tests.py
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-06-13 15:58:35.187108 dsm_django_masterdata-0.0.3/dsm_django_masterdata.egg-info/
--rw-r--r--   0 naii       (501) staff       (20)     1181 2023-06-13 15:58:35.000000 dsm_django_masterdata-0.0.3/dsm_django_masterdata.egg-info/PKG-INFO
--rw-r--r--   0 naii       (501) staff       (20)      632 2023-06-13 15:58:35.000000 dsm_django_masterdata-0.0.3/dsm_django_masterdata.egg-info/SOURCES.txt
--rw-r--r--   0 naii       (501) staff       (20)        1 2023-06-13 15:58:35.000000 dsm_django_masterdata-0.0.3/dsm_django_masterdata.egg-info/dependency_links.txt
--rw-r--r--   0 naii       (501) staff       (20)       15 2023-06-13 15:58:35.000000 dsm_django_masterdata-0.0.3/dsm_django_masterdata.egg-info/requires.txt
--rw-r--r--   0 naii       (501) staff       (20)       22 2023-06-13 15:58:35.000000 dsm_django_masterdata-0.0.3/dsm_django_masterdata.egg-info/top_level.txt
--rw-r--r--   0 naii       (501) staff       (20)       38 2023-06-13 15:58:35.193343 dsm_django_masterdata-0.0.3/setup.cfg
--rw-r--r--   0 naii       (501) staff       (20)     1315 2023-06-13 15:58:12.000000 dsm_django_masterdata-0.0.3/setup.py
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-06-14 04:00:11.816851 dsm_django_masterdata-0.0.4/
+-rw-r--r--   0 naii       (501) staff       (20)     1181 2023-06-14 04:00:11.816228 dsm_django_masterdata-0.0.4/PKG-INFO
+-rw-r--r--   0 naii       (501) staff       (20)      572 2023-06-13 15:58:01.000000 dsm_django_masterdata-0.0.4/README.md
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-06-14 04:00:11.785139 dsm_django_masterdata-0.0.4/dsm_django_masterdata/
+-rw-r--r--   0 naii       (501) staff       (20)      218 2023-06-14 03:50:30.000000 dsm_django_masterdata-0.0.4/dsm_django_masterdata/__init__.py
+-rw-r--r--   0 naii       (501) staff       (20)      291 2023-06-13 15:49:04.000000 dsm_django_masterdata-0.0.4/dsm_django_masterdata/apps.py
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-06-14 04:00:11.802611 dsm_django_masterdata-0.0.4/dsm_django_masterdata/area/
+-rw-r--r--   0 naii       (501) staff       (20)        0 2023-06-14 04:00:07.000000 dsm_django_masterdata-0.0.4/dsm_django_masterdata/area/__init__.py
+-rw-r--r--   0 naii       (501) staff       (20)      314 2023-06-13 15:56:41.000000 dsm_django_masterdata-0.0.4/dsm_django_masterdata/area/admin.py
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-06-14 04:00:11.806860 dsm_django_masterdata-0.0.4/dsm_django_masterdata/area/migrations/
+-rw-r--r--   0 naii       (501) staff       (20)     1663 2023-06-13 15:54:17.000000 dsm_django_masterdata-0.0.4/dsm_django_masterdata/area/migrations/0001_initial.py
+-rw-r--r--   0 naii       (501) staff       (20)        0 2023-06-13 15:51:06.000000 dsm_django_masterdata-0.0.4/dsm_django_masterdata/area/migrations/__init__.py
+-rw-r--r--   0 naii       (501) staff       (20)      669 2023-06-13 15:48:47.000000 dsm_django_masterdata-0.0.4/dsm_django_masterdata/area/models.py
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-06-14 04:00:11.810379 dsm_django_masterdata-0.0.4/dsm_django_masterdata/hscode/
+-rw-r--r--   0 naii       (501) staff       (20)        0 2023-06-12 09:43:46.000000 dsm_django_masterdata-0.0.4/dsm_django_masterdata/hscode/__init__.py
+-rw-r--r--   0 naii       (501) staff       (20)      327 2023-06-12 10:06:08.000000 dsm_django_masterdata-0.0.4/dsm_django_masterdata/hscode/admin.py
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-06-14 04:00:11.815130 dsm_django_masterdata-0.0.4/dsm_django_masterdata/hscode/migrations/
+-rw-r--r--   0 naii       (501) staff       (20)     1110 2023-06-13 15:54:02.000000 dsm_django_masterdata-0.0.4/dsm_django_masterdata/hscode/migrations/0001_initial.py
+-rw-r--r--   0 naii       (501) staff       (20)      337 2023-06-13 15:50:16.000000 dsm_django_masterdata-0.0.4/dsm_django_masterdata/hscode/migrations/0002_alter_hscode_options.py
+-rw-r--r--   0 naii       (501) staff       (20)        0 2023-06-12 09:50:06.000000 dsm_django_masterdata-0.0.4/dsm_django_masterdata/hscode/migrations/__init__.py
+-rw-r--r--   0 naii       (501) staff       (20)      395 2023-06-12 11:19:07.000000 dsm_django_masterdata-0.0.4/dsm_django_masterdata/hscode/models.py
+-rw-r--r--   0 naii       (501) staff       (20)       60 2023-06-12 09:43:33.000000 dsm_django_masterdata-0.0.4/dsm_django_masterdata/tests.py
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-06-14 04:00:11.797657 dsm_django_masterdata-0.0.4/dsm_django_masterdata.egg-info/
+-rw-r--r--   0 naii       (501) staff       (20)     1181 2023-06-14 04:00:11.000000 dsm_django_masterdata-0.0.4/dsm_django_masterdata.egg-info/PKG-INFO
+-rw-r--r--   0 naii       (501) staff       (20)      848 2023-06-14 04:00:11.000000 dsm_django_masterdata-0.0.4/dsm_django_masterdata.egg-info/SOURCES.txt
+-rw-r--r--   0 naii       (501) staff       (20)        1 2023-06-14 04:00:11.000000 dsm_django_masterdata-0.0.4/dsm_django_masterdata.egg-info/dependency_links.txt
+-rw-r--r--   0 naii       (501) staff       (20)       15 2023-06-14 04:00:11.000000 dsm_django_masterdata-0.0.4/dsm_django_masterdata.egg-info/requires.txt
+-rw-r--r--   0 naii       (501) staff       (20)       22 2023-06-14 04:00:11.000000 dsm_django_masterdata-0.0.4/dsm_django_masterdata.egg-info/top_level.txt
+-rw-r--r--   0 naii       (501) staff       (20)       38 2023-06-14 04:00:11.817073 dsm_django_masterdata-0.0.4/setup.cfg
+-rw-r--r--   0 naii       (501) staff       (20)     1321 2023-06-14 03:57:54.000000 dsm_django_masterdata-0.0.4/setup.py
```

### Comparing `dsm_django_masterdata-0.0.3/PKG-INFO` & `dsm_django_masterdata-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsm_django_masterdata
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple way to use Master Data in django project.
 Home-page: https://github.com/storemesh/masterdata/tree/django-app
 Author: DigitalStoreMesh Co.,Ltd
 Author-email: contact@storemesh.com
 License: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dsm_django_masterdata-0.0.3/README.md` & `dsm_django_masterdata-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dsm_django_masterdata-0.0.3/dsm_django_masterdata/hscode/migrations/0001_initial.py` & `dsm_django_masterdata-0.0.4/dsm_django_masterdata/hscode/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `dsm_django_masterdata-0.0.3/dsm_django_masterdata.egg-info/PKG-INFO` & `dsm_django_masterdata-0.0.4/dsm_django_masterdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsm-django-masterdata
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple way to use Master Data in django project.
 Home-page: https://github.com/storemesh/masterdata/tree/django-app
 Author: DigitalStoreMesh Co.,Ltd
 Author-email: contact@storemesh.com
 License: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dsm_django_masterdata-0.0.3/dsm_django_masterdata.egg-info/SOURCES.txt` & `dsm_django_masterdata-0.0.4/dsm_django_masterdata.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -4,13 +4,18 @@
 dsm_django_masterdata/apps.py
 dsm_django_masterdata/tests.py
 dsm_django_masterdata.egg-info/PKG-INFO
 dsm_django_masterdata.egg-info/SOURCES.txt
 dsm_django_masterdata.egg-info/dependency_links.txt
 dsm_django_masterdata.egg-info/requires.txt
 dsm_django_masterdata.egg-info/top_level.txt
+dsm_django_masterdata/area/__init__.py
+dsm_django_masterdata/area/admin.py
+dsm_django_masterdata/area/models.py
+dsm_django_masterdata/area/migrations/0001_initial.py
+dsm_django_masterdata/area/migrations/__init__.py
 dsm_django_masterdata/hscode/__init__.py
 dsm_django_masterdata/hscode/admin.py
 dsm_django_masterdata/hscode/models.py
 dsm_django_masterdata/hscode/migrations/0001_initial.py
 dsm_django_masterdata/hscode/migrations/0002_alter_hscode_options.py
 dsm_django_masterdata/hscode/migrations/__init__.py
```

### Comparing `dsm_django_masterdata-0.0.3/setup.py` & `dsm_django_masterdata-0.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 
 setup(
     name='dsm_django_masterdata',
-    version='0.0.3',
+    version=get_version(),
     url='https://github.com/storemesh/masterdata/tree/django-app',
     packages=find_packages(),
     include_package_data=True,
     license='MIT License',
     description='A simple way to use Master Data in django project.',
     long_description=README,
     long_description_content_type='text/markdown',
```

