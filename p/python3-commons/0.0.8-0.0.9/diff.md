# Comparing `tmp/python3-commons-0.0.8.tar.gz` & `tmp/python3-commons-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python3-commons-0.0.8.tar", last modified: Sat Feb 25 22:24:25 2023, max compression
+gzip compressed data, was "python3-commons-0.0.9.tar", last modified: Thu Mar  9 22:53:13 2023, max compression
```

## Comparing `python3-commons-0.0.8.tar` & `python3-commons-0.0.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 22:24:25.202963 python3-commons-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-02-25 22:24:10.000000 python3-commons-0.0.8/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 22:24:25.190963 python3-commons-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 22:24:25.194963 python3-commons-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-02-25 22:24:10.000000 python3-commons-0.0.8/.github/workflows/python-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-02-25 22:24:10.000000 python3-commons-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-02-25 22:24:10.000000 python3-commons-0.0.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-02-25 22:24:10.000000 python3-commons-0.0.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    34575 2023-02-25 22:24:10.000000 python3-commons-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-02-25 22:24:25.202963 python3-commons-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-25 22:24:10.000000 python3-commons-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-25 22:24:10.000000 python3-commons-0.0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 22:24:25.198963 python3-commons-0.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-02-25 22:24:10.000000 python3-commons-0.0.8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 22:24:25.198963 python3-commons-0.0.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-25 22:24:10.000000 python3-commons-0.0.8/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-25 22:24:10.000000 python3-commons-0.0.8/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-25 22:24:10.000000 python3-commons-0.0.8/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9373 2023-02-25 22:24:10.000000 python3-commons-0.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-02-25 22:24:10.000000 python3-commons-0.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-25 22:24:10.000000 python3-commons-0.0.8/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-02-25 22:24:10.000000 python3-commons-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-02-25 22:24:10.000000 python3-commons-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-25 22:24:10.000000 python3-commons-0.0.8/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-02-25 22:24:25.202963 python3-commons-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-02-25 22:24:10.000000 python3-commons-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 22:24:25.198963 python3-commons-0.0.8/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-02-25 22:24:10.000000 python3-commons-0.0.8/src/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 22:24:25.198963 python3-commons-0.0.8/src/python3_commons/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-02-25 22:24:10.000000 python3-commons-0.0.8/src/python3_commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-02-25 22:24:10.000000 python3-commons-0.0.8/src/python3_commons/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-02-25 22:24:10.000000 python3-commons-0.0.8/src/python3_commons/db.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-02-25 22:24:10.000000 python3-commons-0.0.8/src/python3_commons/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-02-25 22:24:10.000000 python3-commons-0.0.8/src/python3_commons/json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 22:24:25.202963 python3-commons-0.0.8/src/python3_commons/logging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-25 22:24:10.000000 python3-commons-0.0.8/src/python3_commons/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-02-25 22:24:10.000000 python3-commons-0.0.8/src/python3_commons/logging/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-02-25 22:24:10.000000 python3-commons-0.0.8/src/python3_commons/logging/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-02-25 22:24:10.000000 python3-commons-0.0.8/src/python3_commons/minio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-02-25 22:24:10.000000 python3-commons-0.0.8/src/python3_commons/object_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 22:24:25.202963 python3-commons-0.0.8/src/python3_commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-02-25 22:24:25.000000 python3-commons-0.0.8/src/python3_commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-02-25 22:24:25.000000 python3-commons-0.0.8/src/python3_commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-25 22:24:25.000000 python3-commons-0.0.8/src/python3_commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-25 22:24:25.000000 python3-commons-0.0.8/src/python3_commons.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-02-25 22:24:25.000000 python3-commons-0.0.8/src/python3_commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-25 22:24:25.000000 python3-commons-0.0.8/src/python3_commons.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 22:24:25.202963 python3-commons-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-02-25 22:24:10.000000 python3-commons-0.0.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 22:53:13.004127 python3-commons-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-03-09 22:53:00.000000 python3-commons-0.0.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 22:53:12.984126 python3-commons-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 22:53:12.992127 python3-commons-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-03-09 22:53:00.000000 python3-commons-0.0.9/.github/workflows/python-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-09 22:53:00.000000 python3-commons-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-09 22:53:00.000000 python3-commons-0.0.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-09 22:53:00.000000 python3-commons-0.0.9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    34575 2023-03-09 22:53:00.000000 python3-commons-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-09 22:53:13.004127 python3-commons-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-09 22:53:00.000000 python3-commons-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-09 22:53:00.000000 python3-commons-0.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 22:53:12.996127 python3-commons-0.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-03-09 22:53:00.000000 python3-commons-0.0.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 22:53:12.996127 python3-commons-0.0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-09 22:53:00.000000 python3-commons-0.0.9/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-09 22:53:00.000000 python3-commons-0.0.9/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-09 22:53:00.000000 python3-commons-0.0.9/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9373 2023-03-09 22:53:00.000000 python3-commons-0.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-03-09 22:53:00.000000 python3-commons-0.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-09 22:53:00.000000 python3-commons-0.0.9/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-09 22:53:00.000000 python3-commons-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-03-09 22:53:00.000000 python3-commons-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-09 22:53:00.000000 python3-commons-0.0.9/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-03-09 22:53:13.004127 python3-commons-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-09 22:53:00.000000 python3-commons-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 22:53:12.996127 python3-commons-0.0.9/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-03-09 22:53:00.000000 python3-commons-0.0.9/src/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 22:53:13.000127 python3-commons-0.0.9/src/python3_commons/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-03-09 22:53:00.000000 python3-commons-0.0.9/src/python3_commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-09 22:53:00.000000 python3-commons-0.0.9/src/python3_commons/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-03-09 22:53:00.000000 python3-commons-0.0.9/src/python3_commons/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-03-09 22:53:00.000000 python3-commons-0.0.9/src/python3_commons/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-03-09 22:53:00.000000 python3-commons-0.0.9/src/python3_commons/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 22:53:13.000127 python3-commons-0.0.9/src/python3_commons/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 22:53:00.000000 python3-commons-0.0.9/src/python3_commons/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-09 22:53:00.000000 python3-commons-0.0.9/src/python3_commons/logging/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-09 22:53:00.000000 python3-commons-0.0.9/src/python3_commons/logging/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-03-09 22:53:00.000000 python3-commons-0.0.9/src/python3_commons/minio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-03-09 22:53:00.000000 python3-commons-0.0.9/src/python3_commons/object_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 22:53:13.000127 python3-commons-0.0.9/src/python3_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-09 22:53:12.000000 python3-commons-0.0.9/src/python3_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-03-09 22:53:12.000000 python3-commons-0.0.9/src/python3_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 22:53:12.000000 python3-commons-0.0.9/src/python3_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 22:53:12.000000 python3-commons-0.0.9/src/python3_commons.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-09 22:53:12.000000 python3-commons-0.0.9/src/python3_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-09 22:53:12.000000 python3-commons-0.0.9/src/python3_commons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 22:53:13.004127 python3-commons-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-09 22:53:00.000000 python3-commons-0.0.9/tests/conftest.py
```

### Comparing `python3-commons-0.0.8/.coveragerc` & `python3-commons-0.0.9/.coveragerc`

 * *Files identical despite different names*

### Comparing `python3-commons-0.0.8/.github/workflows/python-publish.yaml` & `python3-commons-0.0.9/.github/workflows/python-publish.yaml`

 * *Files identical despite different names*

### Comparing `python3-commons-0.0.8/.gitignore` & `python3-commons-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `python3-commons-0.0.8/LICENSE` & `python3-commons-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python3-commons-0.0.8/PKG-INFO` & `python3-commons-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python3-commons
-Version: 0.0.8
+Version: 0.0.9
 Summary: Re-usable Python3 code
 Home-page: https://github.com/kamikaze/python3-commons
 Author: Oleg Korsak
 Author-email: kamikaze.is.waiting.you@gmail.com
 License: gpl-3
 Project-URL: Documentation, https://github.com/kamikaze/python3-commons/wiki
 Platform: any
```

### Comparing `python3-commons-0.0.8/docs/Makefile` & `python3-commons-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python3-commons-0.0.8/docs/conf.py` & `python3-commons-0.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python3-commons-0.0.8/docs/index.rst` & `python3-commons-0.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python3-commons-0.0.8/requirements.txt` & `python3-commons-0.0.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `python3-commons-0.0.8/setup.cfg` & `python3-commons-0.0.9/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python3-commons
-version = 0.0.8
+version = 0.0.9
 description = Re-usable Python3 code
 author = Oleg Korsak
 author_email = kamikaze.is.waiting.you@gmail.com
 license = gpl-3
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 url = https://github.com/kamikaze/python3-commons
@@ -22,15 +22,15 @@
 package_dir = 
 	=src
 setup_requires = pyscaffold>=3.2a0,<3.3a0
 install_requires = 
 	asyncpg==0.27.0
 	databases[postgresql]==0.7.0
 	minio==7.1.13
-	pydantic[email]==1.10.5
+	pydantic[email]==1.10.6
 python_requires = >=3.9
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
```

### Comparing `python3-commons-0.0.8/src/helpers.py` & `python3-commons-0.0.9/src/helpers.py`

 * *Files identical despite different names*

### Comparing `python3-commons-0.0.8/src/python3_commons/db.py` & `python3-commons-0.0.9/src/python3_commons/db.py`

 * *Files identical despite different names*

### Comparing `python3-commons-0.0.8/src/python3_commons/json.py` & `python3-commons-0.0.9/src/python3_commons/json.py`

 * *Files identical despite different names*

### Comparing `python3-commons-0.0.8/src/python3_commons/minio.py` & `python3-commons-0.0.9/src/python3_commons/minio.py`

 * *Files identical despite different names*

### Comparing `python3-commons-0.0.8/src/python3_commons/object_storage.py` & `python3-commons-0.0.9/src/python3_commons/object_storage.py`

 * *Files identical despite different names*

### Comparing `python3-commons-0.0.8/src/python3_commons.egg-info/PKG-INFO` & `python3-commons-0.0.9/src/python3_commons.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python3-commons
-Version: 0.0.8
+Version: 0.0.9
 Summary: Re-usable Python3 code
 Home-page: https://github.com/kamikaze/python3-commons
 Author: Oleg Korsak
 Author-email: kamikaze.is.waiting.you@gmail.com
 License: gpl-3
 Project-URL: Documentation, https://github.com/kamikaze/python3-commons/wiki
 Platform: any
```

### Comparing `python3-commons-0.0.8/src/python3_commons.egg-info/SOURCES.txt` & `python3-commons-0.0.9/src/python3_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

