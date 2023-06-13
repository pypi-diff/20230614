# Comparing `tmp/artd_colombian_cities-0.0.15.tar.gz` & `tmp/artd_colombian_cities-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artd_colombian_cities-0.0.15.tar", last modified: Tue Jun 13 22:42:59 2023, max compression
+gzip compressed data, was "artd_colombian_cities-0.0.16.tar", last modified: Tue Jun 13 23:24:42 2023, max compression
```

## Comparing `artd_colombian_cities-0.0.15.tar` & `artd_colombian_cities-0.0.16.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:42:59.871441 artd_colombian_cities-0.0.15/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-13 22:42:54.000000 artd_colombian_cities-0.0.15/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-13 22:42:59.867441 artd_colombian_cities-0.0.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-13 22:42:54.000000 artd_colombian_cities-0.0.15/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:42:59.867441 artd_colombian_cities-0.0.15/artd_colombian_cities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 22:42:54.000000 artd_colombian_cities-0.0.15/artd_colombian_cities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-13 22:42:54.000000 artd_colombian_cities-0.0.15/artd_colombian_cities/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-06-13 22:42:54.000000 artd_colombian_cities-0.0.15/artd_colombian_cities/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-13 22:42:54.000000 artd_colombian_cities-0.0.15/artd_colombian_cities/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-13 22:42:54.000000 artd_colombian_cities-0.0.15/artd_colombian_cities/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:42:59.867441 artd_colombian_cities-0.0.15/artd_colombian_cities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-13 22:42:59.000000 artd_colombian_cities-0.0.15/artd_colombian_cities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-13 22:42:59.000000 artd_colombian_cities-0.0.15/artd_colombian_cities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 22:42:59.000000 artd_colombian_cities-0.0.15/artd_colombian_cities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-13 22:42:59.000000 artd_colombian_cities-0.0.15/artd_colombian_cities.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:42:59.867441 artd_colombian_cities-0.0.15/colombian_cities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 22:42:54.000000 artd_colombian_cities-0.0.15/colombian_cities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-13 22:42:54.000000 artd_colombian_cities-0.0.15/colombian_cities/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-13 22:42:54.000000 artd_colombian_cities-0.0.15/colombian_cities/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:42:59.867441 artd_colombian_cities-0.0.15/colombian_cities/data/
--rw-r--r--   0 runner    (1001) docker     (123)   108426 2023-06-13 22:42:54.000000 artd_colombian_cities-0.0.15/colombian_cities/data/cities.py
--rw-r--r--   0 runner    (1001) docker     (123)    33716 2023-06-13 22:42:54.000000 artd_colombian_cities-0.0.15/colombian_cities/data/countries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-13 22:42:54.000000 artd_colombian_cities-0.0.15/colombian_cities/data/regions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:42:59.867441 artd_colombian_cities-0.0.15/colombian_cities/generators/
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-13 22:42:54.000000 artd_colombian_cities-0.0.15/colombian_cities/generators/generators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:42:59.867441 artd_colombian_cities-0.0.15/colombian_cities/management/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:42:59.867441 artd_colombian_cities-0.0.15/colombian_cities/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 22:42:54.000000 artd_colombian_cities-0.0.15/colombian_cities/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-13 22:42:54.000000 artd_colombian_cities-0.0.15/colombian_cities/management/commands/create_colombian_cities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-13 22:42:54.000000 artd_colombian_cities-0.0.15/colombian_cities/management/commands/create_colombian_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-13 22:42:54.000000 artd_colombian_cities-0.0.15/colombian_cities/management/commands/create_countries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:42:59.867441 artd_colombian_cities-0.0.15/colombian_cities/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-06-13 22:42:54.000000 artd_colombian_cities-0.0.15/colombian_cities/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 22:42:54.000000 artd_colombian_cities-0.0.15/colombian_cities/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-13 22:42:54.000000 artd_colombian_cities-0.0.15/colombian_cities/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-13 22:42:54.000000 artd_colombian_cities-0.0.15/colombian_cities/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-13 22:42:54.000000 artd_colombian_cities-0.0.15/colombian_cities/views.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      677 2023-06-13 22:42:54.000000 artd_colombian_cities-0.0.15/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:42:59.867441 artd_colombian_cities-0.0.15/migrate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 22:42:54.000000 artd_colombian_cities-0.0.15/migrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-13 22:42:54.000000 artd_colombian_cities-0.0.15/migrate/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-13 22:42:54.000000 artd_colombian_cities-0.0.15/migrate/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:42:59.867441 artd_colombian_cities-0.0.15/migrate/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 22:42:54.000000 artd_colombian_cities-0.0.15/migrate/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-13 22:42:54.000000 artd_colombian_cities-0.0.15/migrate/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-13 22:42:54.000000 artd_colombian_cities-0.0.15/migrate/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-13 22:42:54.000000 artd_colombian_cities-0.0.15/migrate/views.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 22:42:59.871441 artd_colombian_cities-0.0.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-13 22:42:58.000000 artd_colombian_cities-0.0.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:24:42.355217 artd_colombian_cities-0.0.16/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-13 23:24:35.000000 artd_colombian_cities-0.0.16/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-13 23:24:42.355217 artd_colombian_cities-0.0.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-13 23:24:35.000000 artd_colombian_cities-0.0.16/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:24:42.351217 artd_colombian_cities-0.0.16/artd_colombian_cities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:24:35.000000 artd_colombian_cities-0.0.16/artd_colombian_cities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-13 23:24:35.000000 artd_colombian_cities-0.0.16/artd_colombian_cities/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-06-13 23:24:35.000000 artd_colombian_cities-0.0.16/artd_colombian_cities/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-13 23:24:35.000000 artd_colombian_cities-0.0.16/artd_colombian_cities/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-13 23:24:35.000000 artd_colombian_cities-0.0.16/artd_colombian_cities/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:24:42.351217 artd_colombian_cities-0.0.16/artd_colombian_cities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-13 23:24:42.000000 artd_colombian_cities-0.0.16/artd_colombian_cities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-13 23:24:42.000000 artd_colombian_cities-0.0.16/artd_colombian_cities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 23:24:42.000000 artd_colombian_cities-0.0.16/artd_colombian_cities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-13 23:24:42.000000 artd_colombian_cities-0.0.16/artd_colombian_cities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:24:42.351217 artd_colombian_cities-0.0.16/colombian_cities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:24:35.000000 artd_colombian_cities-0.0.16/colombian_cities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-13 23:24:35.000000 artd_colombian_cities-0.0.16/colombian_cities/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-13 23:24:35.000000 artd_colombian_cities-0.0.16/colombian_cities/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:24:42.351217 artd_colombian_cities-0.0.16/colombian_cities/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   108426 2023-06-13 23:24:35.000000 artd_colombian_cities-0.0.16/colombian_cities/data/cities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33716 2023-06-13 23:24:35.000000 artd_colombian_cities-0.0.16/colombian_cities/data/countries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-13 23:24:35.000000 artd_colombian_cities-0.0.16/colombian_cities/data/regions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:24:42.351217 artd_colombian_cities-0.0.16/colombian_cities/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-13 23:24:35.000000 artd_colombian_cities-0.0.16/colombian_cities/generators/generators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:24:42.351217 artd_colombian_cities-0.0.16/colombian_cities/management/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:24:42.351217 artd_colombian_cities-0.0.16/colombian_cities/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:24:35.000000 artd_colombian_cities-0.0.16/colombian_cities/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-13 23:24:35.000000 artd_colombian_cities-0.0.16/colombian_cities/management/commands/create_colombian_cities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-13 23:24:35.000000 artd_colombian_cities-0.0.16/colombian_cities/management/commands/create_colombian_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-13 23:24:35.000000 artd_colombian_cities-0.0.16/colombian_cities/management/commands/create_countries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:24:42.351217 artd_colombian_cities-0.0.16/colombian_cities/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-06-13 23:24:35.000000 artd_colombian_cities-0.0.16/colombian_cities/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:24:35.000000 artd_colombian_cities-0.0.16/colombian_cities/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-13 23:24:35.000000 artd_colombian_cities-0.0.16/colombian_cities/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-13 23:24:35.000000 artd_colombian_cities-0.0.16/colombian_cities/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-13 23:24:35.000000 artd_colombian_cities-0.0.16/colombian_cities/views.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      677 2023-06-13 23:24:35.000000 artd_colombian_cities-0.0.16/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:24:42.351217 artd_colombian_cities-0.0.16/migrate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:24:35.000000 artd_colombian_cities-0.0.16/migrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-13 23:24:35.000000 artd_colombian_cities-0.0.16/migrate/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-13 23:24:35.000000 artd_colombian_cities-0.0.16/migrate/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:24:42.355217 artd_colombian_cities-0.0.16/migrate/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:24:35.000000 artd_colombian_cities-0.0.16/migrate/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-13 23:24:35.000000 artd_colombian_cities-0.0.16/migrate/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-13 23:24:35.000000 artd_colombian_cities-0.0.16/migrate/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-13 23:24:35.000000 artd_colombian_cities-0.0.16/migrate/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 23:24:42.355217 artd_colombian_cities-0.0.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-13 23:24:40.000000 artd_colombian_cities-0.0.16/setup.py
```

### Comparing `artd_colombian_cities-0.0.15/PKG-INFO` & `artd_colombian_cities-0.0.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artd_colombian_cities
-Version: 0.0.15
+Version: 0.0.16
 Summary: A Django app to create Colombian cities
 Home-page: https://www.artd.com.co/
 Author: Jonathan Urzola Maladonado
 Author-email: jonathan@artd.com.co
 Keywords: pypi,cicd,python
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `artd_colombian_cities-0.0.15/README.rst` & `artd_colombian_cities-0.0.16/README.rst`

 * *Files identical despite different names*

### Comparing `artd_colombian_cities-0.0.15/artd_colombian_cities/settings.py` & `artd_colombian_cities-0.0.16/artd_colombian_cities/settings.py`

 * *Files identical despite different names*

### Comparing `artd_colombian_cities-0.0.15/artd_colombian_cities/urls.py` & `artd_colombian_cities-0.0.16/artd_colombian_cities/urls.py`

 * *Files identical despite different names*

### Comparing `artd_colombian_cities-0.0.15/artd_colombian_cities.egg-info/PKG-INFO` & `artd_colombian_cities-0.0.16/artd_colombian_cities.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artd-colombian-cities
-Version: 0.0.15
+Version: 0.0.16
 Summary: A Django app to create Colombian cities
 Home-page: https://www.artd.com.co/
 Author: Jonathan Urzola Maladonado
 Author-email: jonathan@artd.com.co
 Keywords: pypi,cicd,python
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `artd_colombian_cities-0.0.15/artd_colombian_cities.egg-info/SOURCES.txt` & `artd_colombian_cities-0.0.16/artd_colombian_cities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `artd_colombian_cities-0.0.15/colombian_cities/admin.py` & `artd_colombian_cities-0.0.16/colombian_cities/admin.py`

 * *Files identical despite different names*

### Comparing `artd_colombian_cities-0.0.15/colombian_cities/data/cities.py` & `artd_colombian_cities-0.0.16/colombian_cities/data/cities.py`

 * *Files identical despite different names*

### Comparing `artd_colombian_cities-0.0.15/colombian_cities/data/countries.py` & `artd_colombian_cities-0.0.16/colombian_cities/data/countries.py`

 * *Files identical despite different names*

### Comparing `artd_colombian_cities-0.0.15/colombian_cities/data/regions.py` & `artd_colombian_cities-0.0.16/colombian_cities/data/regions.py`

 * *Files identical despite different names*

### Comparing `artd_colombian_cities-0.0.15/colombian_cities/generators/generators.py` & `artd_colombian_cities-0.0.16/colombian_cities/generators/generators.py`

 * *Files identical despite different names*

### Comparing `artd_colombian_cities-0.0.15/colombian_cities/management/commands/create_colombian_cities.py` & `artd_colombian_cities-0.0.16/colombian_cities/management/commands/create_colombian_cities.py`

 * *Files identical despite different names*

### Comparing `artd_colombian_cities-0.0.15/colombian_cities/management/commands/create_colombian_regions.py` & `artd_colombian_cities-0.0.16/colombian_cities/management/commands/create_colombian_regions.py`

 * *Files identical despite different names*

### Comparing `artd_colombian_cities-0.0.15/colombian_cities/management/commands/create_countries.py` & `artd_colombian_cities-0.0.16/colombian_cities/management/commands/create_countries.py`

 * *Files identical despite different names*

### Comparing `artd_colombian_cities-0.0.15/colombian_cities/migrations/0001_initial.py` & `artd_colombian_cities-0.0.16/colombian_cities/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `artd_colombian_cities-0.0.15/colombian_cities/models.py` & `artd_colombian_cities-0.0.16/colombian_cities/models.py`

 * *Files identical despite different names*

### Comparing `artd_colombian_cities-0.0.15/colombian_cities/tests.py` & `artd_colombian_cities-0.0.16/colombian_cities/tests.py`

 * *Files identical despite different names*

### Comparing `artd_colombian_cities-0.0.15/manage.py` & `artd_colombian_cities-0.0.16/manage.py`

 * *Files identical despite different names*

### Comparing `artd_colombian_cities-0.0.15/setup.py` & `artd_colombian_cities-0.0.16/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-here = os.path.abspath(os.path.dirname(__file__))
+# read the contents of your README file
+from pathlib import Path
+
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.rst").read_text()
 
 setup(
     name="artd_colombian_cities",
-    version="0.0.15",
+    version="0.0.16",
     include_package_data=True,
     author="Jonathan Urzola Maladonado",
     author_email="jonathan@artd.com.co",
     description="A Django app to create Colombian cities",
     long_description_content_type="text/markdown",
     url="https://www.artd.com.co/",
     long_description="A Django app to create Colombian cities",
```

