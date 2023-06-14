# Comparing `tmp/as-scraper-2.3.2.tar.gz` & `tmp/as-scraper-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "as-scraper-2.3.2.tar", last modified: Wed Jun 14 21:17:06 2023, max compression
+gzip compressed data, was "as-scraper-2.3.3.tar", last modified: Wed Jun 14 21:19:00 2023, max compression
```

## Comparing `as-scraper-2.3.2.tar` & `as-scraper-2.3.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:17:06.565151 as-scraper-2.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-14 21:16:46.000000 as-scraper-2.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-06-14 21:17:06.565151 as-scraper-2.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-06-14 21:16:46.000000 as-scraper-2.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:17:06.561151 as-scraper-2.3.2/as_scraper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 21:16:46.000000 as-scraper-2.3.2/as_scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:17:06.565151 as-scraper-2.3.2/as_scraper/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-14 21:16:46.000000 as-scraper-2.3.2/as_scraper/crawlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-14 21:16:46.000000 as-scraper-2.3.2/as_scraper/crawlers/crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-14 21:16:46.000000 as-scraper-2.3.2/as_scraper/crawlers/tree_crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-14 21:16:46.000000 as-scraper-2.3.2/as_scraper/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-14 21:16:46.000000 as-scraper-2.3.2/as_scraper/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-14 21:16:46.000000 as-scraper-2.3.2/as_scraper/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-06-14 21:16:46.000000 as-scraper-2.3.2/as_scraper/scraper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:17:06.565151 as-scraper-2.3.2/as_scraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-06-14 21:17:06.000000 as-scraper-2.3.2/as_scraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-14 21:17:06.000000 as-scraper-2.3.2/as_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 21:17:06.000000 as-scraper-2.3.2/as_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-14 21:17:06.000000 as-scraper-2.3.2/as_scraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-14 21:17:06.000000 as-scraper-2.3.2/as_scraper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 21:17:06.569151 as-scraper-2.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-14 21:16:46.000000 as-scraper-2.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:19:00.653712 as-scraper-2.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-14 21:18:43.000000 as-scraper-2.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-06-14 21:19:00.653712 as-scraper-2.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-06-14 21:18:43.000000 as-scraper-2.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:19:00.649712 as-scraper-2.3.3/as_scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 21:18:43.000000 as-scraper-2.3.3/as_scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:19:00.653712 as-scraper-2.3.3/as_scraper/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-14 21:18:43.000000 as-scraper-2.3.3/as_scraper/crawlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-14 21:18:43.000000 as-scraper-2.3.3/as_scraper/crawlers/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-14 21:18:43.000000 as-scraper-2.3.3/as_scraper/crawlers/tree_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-14 21:18:43.000000 as-scraper-2.3.3/as_scraper/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-14 21:18:43.000000 as-scraper-2.3.3/as_scraper/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-14 21:18:43.000000 as-scraper-2.3.3/as_scraper/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-06-14 21:18:43.000000 as-scraper-2.3.3/as_scraper/scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:19:00.653712 as-scraper-2.3.3/as_scraper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-06-14 21:19:00.000000 as-scraper-2.3.3/as_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-14 21:19:00.000000 as-scraper-2.3.3/as_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 21:19:00.000000 as-scraper-2.3.3/as_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-14 21:19:00.000000 as-scraper-2.3.3/as_scraper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-14 21:19:00.000000 as-scraper-2.3.3/as_scraper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 21:19:00.653712 as-scraper-2.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-14 21:18:43.000000 as-scraper-2.3.3/setup.py
```

### Comparing `as-scraper-2.3.2/LICENSE` & `as-scraper-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `as-scraper-2.3.2/PKG-INFO` & `as-scraper-2.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: as-scraper
-Version: 2.3.2
+Version: 2.3.3
 Summary: Python library for scraping with Selenium.
 Home-page: https://github.com/Avila-Systems/as-scraper
 Author: Alvaro Avila
 Author-email: almiavicas@gmail.com
 Project-URL: Github Project, https://github.com/Avila-Systems/as-scraper
 Project-URL: Issue Tracker, https://github.com/Avila-Systems/as-scraper/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # as-scraper
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/as-scraper.svg)](https://pypi.org/project/as-scraper/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/as-scraper)](https://pypi.org/project/as-scraper/)
```

### Comparing `as-scraper-2.3.2/README.md` & `as-scraper-2.3.3/README.md`

 * *Files identical despite different names*

### Comparing `as-scraper-2.3.2/as_scraper/crawlers/crawler.py` & `as-scraper-2.3.3/as_scraper/crawlers/crawler.py`

 * *Files identical despite different names*

### Comparing `as-scraper-2.3.2/as_scraper/crawlers/tree_crawler.py` & `as-scraper-2.3.3/as_scraper/crawlers/tree_crawler.py`

 * *Files identical despite different names*

### Comparing `as-scraper-2.3.2/as_scraper/scraper.py` & `as-scraper-2.3.3/as_scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `as-scraper-2.3.2/as_scraper.egg-info/PKG-INFO` & `as-scraper-2.3.3/as_scraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: as-scraper
-Version: 2.3.2
+Version: 2.3.3
 Summary: Python library for scraping with Selenium.
 Home-page: https://github.com/Avila-Systems/as-scraper
 Author: Alvaro Avila
 Author-email: almiavicas@gmail.com
 Project-URL: Github Project, https://github.com/Avila-Systems/as-scraper
 Project-URL: Issue Tracker, https://github.com/Avila-Systems/as-scraper/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # as-scraper
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/as-scraper.svg)](https://pypi.org/project/as-scraper/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/as-scraper)](https://pypi.org/project/as-scraper/)
```

### Comparing `as-scraper-2.3.2/setup.py` & `as-scraper-2.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def get_long_description():
     with open('README.md') as file:
         return file.read()
 
 
 setup(
     name='as-scraper',
-    version='2.3.2',
+    version='2.3.3',
     description='Python library for scraping with Selenium.',
     long_description=get_long_description(),
     long_description_content_type='text/markdown',
     author='Alvaro Avila',
     author_email='almiavicas@gmail.com',
     url='https://github.com/Avila-Systems/as-scraper',
     project_urls={
@@ -26,15 +26,15 @@
         'selenium',
         'bs4',
         'lxml',
         'pandas',
         'requests',
         'tqdm',
     ],
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     classifiers=[
         'Intended Audience :: Developers',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Operating System :: POSIX',
         'License :: OSI Approved :: MIT License',
         'Topic :: Software Development :: Libraries'
```

